# Comparing `tmp/datadog-cdk-constructs-v2-1.7.1.tar.gz` & `tmp/datadog-cdk-constructs-v2-1.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog-cdk-constructs-v2-1.7.1.tar", last modified: Thu May 18 16:00:03 2023, max compression
+gzip compressed data, was "datadog-cdk-constructs-v2-1.7.3.tar", last modified: Tue Jun 13 19:44:37 2023, max compression
```

## Comparing `datadog-cdk-constructs-v2-1.7.1.tar` & `datadog-cdk-constructs-v2-1.7.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-18 16:00:03.341519 datadog-cdk-constructs-v2-1.7.1/
--rw-r--r--   0 david.lee   (503) staff       (20)    11358 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/LICENSE
--rw-r--r--   0 david.lee   (503) staff       (20)       23 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/MANIFEST.in
--rw-r--r--   0 david.lee   (503) staff       (20)    22507 2023-05-18 16:00:03.341375 datadog-cdk-constructs-v2-1.7.1/PKG-INFO
--rw-r--r--   0 david.lee   (503) staff       (20)    21527 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/README.md
--rw-r--r--   0 david.lee   (503) staff       (20)      236 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/pyproject.toml
--rw-r--r--   0 david.lee   (503) staff       (20)       38 2023-05-18 16:00:03.341569 datadog-cdk-constructs-v2-1.7.1/setup.cfg
--rw-r--r--   0 david.lee   (503) staff       (20)     1921 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/setup.py
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-18 16:00:03.338432 datadog-cdk-constructs-v2-1.7.1/src/
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-18 16:00:03.339799 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2/
--rw-r--r--   0 david.lee   (503) staff       (20)    98974 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2/__init__.py
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-18 16:00:03.341040 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2/_jsii/
--rw-r--r--   0 david.lee   (503) staff       (20)      475 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2/_jsii/__init__.py
--rw-r--r--   0 david.lee   (503) staff       (20)   134685 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.7.1.jsii.tgz
--rw-r--r--   0 david.lee   (503) staff       (20)        1 2023-05-18 15:59:59.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2/py.typed
-drwxr-xr-x   0 david.lee   (503) staff       (20)        0 2023-05-18 16:00:03.340684 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/
--rw-r--r--   0 david.lee   (503) staff       (20)    22507 2023-05-18 16:00:03.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
--rw-r--r--   0 david.lee   (503) staff       (20)      523 2023-05-18 16:00:03.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
--rw-r--r--   0 david.lee   (503) staff       (20)        1 2023-05-18 16:00:03.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
--rw-r--r--   0 david.lee   (503) staff       (20)      161 2023-05-18 16:00:03.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/requires.txt
--rw-r--r--   0 david.lee   (503) staff       (20)       26 2023-05-18 16:00:03.000000 datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/top_level.txt
+drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 19:44:37.784273 datadog-cdk-constructs-v2-1.7.3/
+-rw-r--r--   0 dylan.yang   (502) staff       (20)    11358 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/LICENSE
+-rw-r--r--   0 dylan.yang   (502) staff       (20)       23 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/MANIFEST.in
+-rw-r--r--   0 dylan.yang   (502) staff       (20)    24060 2023-06-13 19:44:37.784114 datadog-cdk-constructs-v2-1.7.3/PKG-INFO
+-rw-r--r--   0 dylan.yang   (502) staff       (20)    23080 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/README.md
+-rw-r--r--   0 dylan.yang   (502) staff       (20)      236 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/pyproject.toml
+-rw-r--r--   0 dylan.yang   (502) staff       (20)       38 2023-06-13 19:44:37.784316 datadog-cdk-constructs-v2-1.7.3/setup.cfg
+-rw-r--r--   0 dylan.yang   (502) staff       (20)     1921 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/setup.py
+drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 19:44:37.781059 datadog-cdk-constructs-v2-1.7.3/src/
+drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 19:44:37.782222 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2/
+-rw-r--r--   0 dylan.yang   (502) staff       (20)   113679 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2/__init__.py
+drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 19:44:37.783186 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2/_jsii/
+-rw-r--r--   0 dylan.yang   (502) staff       (20)      475 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2/_jsii/__init__.py
+-rw-r--r--   0 dylan.yang   (502) staff       (20)  1307963 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.7.3.jsii.tgz
+-rw-r--r--   0 dylan.yang   (502) staff       (20)        1 2023-06-13 19:44:33.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2/py.typed
+drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 19:44:37.782902 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/
+-rw-r--r--   0 dylan.yang   (502) staff       (20)    24060 2023-06-13 19:44:37.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
+-rw-r--r--   0 dylan.yang   (502) staff       (20)      523 2023-06-13 19:44:37.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan.yang   (502) staff       (20)        1 2023-06-13 19:44:37.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan.yang   (502) staff       (20)      161 2023-06-13 19:44:37.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/requires.txt
+-rw-r--r--   0 dylan.yang   (502) staff       (20)       26 2023-06-13 19:44:37.000000 datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/top_level.txt
```

### Comparing `datadog-cdk-constructs-v2-1.7.1/LICENSE` & `datadog-cdk-constructs-v2-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog-cdk-constructs-v2-1.7.1/PKG-INFO` & `datadog-cdk-constructs-v2-1.7.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-cdk-constructs-v2
-Version: 1.7.1
+Version: 1.7.3
 Summary: CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2
 Home-page: https://github.com/DataDog/datadog-cdk-constructs
 Author: Datadog
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataDog/datadog-cdk-constructs
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -38,15 +38,16 @@
 * Enabling the collection of traces and custom metrics from your Lambda functions.
 * Managing subscriptions from the Datadog Forwarder to your Lambda and non-Lambda log groups.
 
 ## AWS CDK v1 vs AWS CDK v2
 
 Two separate versions of Datadog CDK Constructs exist; `datadog-cdk-constructs` and `datadog-cdk-constructs-v2`. These are designed to work with `AWS CDK v1` and `AWS CDK v2` respectively.
 
-* `datadog-cdk-constructs-v2` requires Node 14+, while `datadog-cdk-constructs-v1` supports Node 12+.
+* `datadog-cdk-constructs-v2` requires Node >= 14, while `datadog-cdk-constructs` supports Node >= 12.
+* `datadog-cdk-constructs-v2` contains more features.
 * Otherwise, the use of the two packages is identical.
 
 ## npm Package Installation:
 
 For use with AWS CDK v2:
 
 ```
@@ -101,14 +102,15 @@
   extensionLayerVersion: "<EXTENSION_VERSION>",
   forwarderArn: "<FORWARDER_ARN>",
   createForwarderPermissions: <BOOLEAN>,
   flushMetricsToLogs: <BOOLEAN>,
   site: "<SITE>",
   apiKey: "{Datadog_API_Key}",
   apiKeySecretArn: "{Secret_ARN_Datadog_API_Key}",
+  apiKeySecret: <AWS_CDK_ISECRET>, // Only available in datadog-cdk-constructs-v2
   apiKmsKey: "{Encrypted_Datadog_API_Key}",
   enableDatadogTracing: <BOOLEAN>,
   enableMergeXrayTraces: <BOOLEAN>,
   enableDatadogLogs: <BOOLEAN>,
   injectLogContext: <BOOLEAN>,
   logLevel: <STRING>,
   env: <STRING>, //Optional
@@ -205,14 +207,15 @@
 | `extensionLayerVersion` | `extension_layer_version` | Version of the Datadog Lambda Extension layer to install, such as 5. When `extensionLayerVersion` is set, `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`) needs to be set as well. When enabled, lambda function log groups will not be subscribed by the forwarder. Learn more about the Lambda extension [here](https://docs.datadoghq.com/serverless/datadog_lambda_library/extension/). |
 | `forwarderArn` | `forwarder_arn` | When set, the plugin will automatically subscribe the Datadog Forwarder to the functions' log groups. Do not set `forwarderArn` when `extensionLayerVersion` is set. |
 | `createForwarderPermissions` | `createForwarderPermissions` | When set to `true`, creates a Lambda permission on the the Datadog Forwarder per log group. Since the Datadog Forwarder has permissions configured by default, this is unnecessary in most use cases. |
 | `flushMetricsToLogs` | `flush_metrics_to_logs` | Send custom metrics using CloudWatch logs with the Datadog Forwarder Lambda function (recommended). Defaults to `true` . If you disable this parameter, it's required to set `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`). |
 | `site` | `site` | Set which Datadog site to send data. This is only used when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. Possible values are `datadoghq.com`, `datadoghq.eu`, `us3.datadoghq.com`, `us5.datadoghq.com`, `ap1.datadoghq.com`, and `ddog-gov.com`. The default is `datadoghq.com`. |
 | `apiKey` | `api_key` | Datadog API Key, only needed when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. For more information about getting a Datadog API key, see the [API key documentation](https://docs.datadoghq.com/account_management/api-app-keys/#api-keys). |
 | `apiKeySecretArn` | `api_key_secret_arn` | The ARN of the secret storing the Datadog API key in AWS Secrets Manager. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayer` is set. Remember to add the `secretsmanager:GetSecretValue` permission to the Lambda execution role. |
+| `apiKeySecret` | `api_key_secret` | An [AWS CDK ISecret](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_secretsmanager.ISecret.html) representing a secret storing the Datadog API key in AWS Secrets Manager. Use this parameter in place of `apiKeySecretArn` to automatically grant your Lambda execution roles read access to the given secret. [See here](#automatically-grant-aws-secret-read-access-to-lambda-execution-role) for an example. **Only available in datadog-cdk-constructs-v2**. |
 | `apiKmsKey` | `api_kms_key` | Datadog API Key encrypted using KMS. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set, and you are using KMS encryption. |
 | `enableDatadogTracing` | `enable_datadog_tracing` | Enable Datadog tracing on your Lambda functions. Defaults to `true`. |
 | `enableMergeXrayTraces` | `enable_merge_xray_traces` | Enable merging X-Ray traces on your Lambda functions. Defaults to `false`. |
 | `enableDatadogLogs` | `enable_datadog_logs` | Send Lambda function logs to Datadog via the Datadog Lambda Extension.  Defaults to `true`. Note: This setting has no effect on logs sent via the Datadog Forwarder. |
 | `enableSourceCodeIntegration` | `enable_source_code_integration` | Enable Datadog Source Code Integration, connecting your telemetry with application code in your Git repositories. This requires the Datadog Github Integration to work, otherwise please follow the [alternative method](#alternative-methods-to-enable-source-code-integration). Learn more [here](https://docs.datadoghq.com/integrations/guide/source-code-integration/). Defaults to `true`. |
 | `injectLogContext` | `inject_log_context` | When set, the Lambda layer will automatically patch console.log with Datadog's tracing ids. Defaults to `true`. |
 | `logLevel` | `log_level` | When set to `debug`, the Datadog Lambda Library and Extension will log additional information to help troubleshoot issues. |
@@ -307,14 +310,34 @@
 }
 ```
 
 ### Tags
 
 Add tags to your constructs. We recommend setting an `env` and `service` tag to tie Datadog telemetry together. For more information see [official AWS documentation](https://docs.aws.amazon.com/cdk/latest/guide/tagging.html) and [CDK documentation](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.Tags.html).
 
+## Automatically grant AWS secret read access to Lambda execution role
+
+**Only available in datadog-cdk-constructs-v2**
+
+To automatically grant your Lambda execution roles read access to a given secret, pass in `apiKeySecret` in place of `apiKeySecretArn` when initializing the Datadog construct.
+
+```
+const { Secret } = require('aws-cdk-lib/aws-secretsmanager');
+
+const secret = Secret.fromSecretPartialArn(this, 'DatadogApiKeySecret', 'arn:aws:secretsmanager:us-west-1:123:secret:DATADOG_API_KEY');
+
+const datadog = new Datadog(this, 'Datadog', {
+  ...
+  apiKeySecret: secret
+  ...
+});
+```
+
+When `addLambdaFunctions` is called, the Datadog CDK construct grants your Lambda execution roles read access to the given AWS secret. This is done through the [AWS ISecret's grantRead function](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_secretsmanager.ISecret.html#grantwbrreadgrantee-versionstages).
+
 ## How it works
 
 The Datadog CDK construct takes in a list of lambda functions and installs the Datadog Lambda Library by attaching the Lambda Layers for [Java](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk), [Node.js](https://github.com/DataDog/datadog-lambda-layer-js), and [Python](https://github.com/DataDog/datadog-lambda-layer-python) to your functions. It redirects to a replacement handler that initializes the Lambda Library without any required code changes. Additional configurations added to the Datadog CDK construct will also translate into their respective environment variables under each lambda function (if applicable / required).
 
 While Lambda function based log groups are handled by the `addLambdaFunctions` method automatically, the construct has an additional function `addForwarderToNonLambdaLogGroups` which subscribes the forwarder to any additional log groups of your choosing.
 
 ## Resources to learn about CDK
```

### Comparing `datadog-cdk-constructs-v2-1.7.1/README.md` & `datadog-cdk-constructs-v2-1.7.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -14,15 +14,16 @@
 * Enabling the collection of traces and custom metrics from your Lambda functions.
 * Managing subscriptions from the Datadog Forwarder to your Lambda and non-Lambda log groups.
 
 ## AWS CDK v1 vs AWS CDK v2
 
 Two separate versions of Datadog CDK Constructs exist; `datadog-cdk-constructs` and `datadog-cdk-constructs-v2`. These are designed to work with `AWS CDK v1` and `AWS CDK v2` respectively.
 
-* `datadog-cdk-constructs-v2` requires Node 14+, while `datadog-cdk-constructs-v1` supports Node 12+.
+* `datadog-cdk-constructs-v2` requires Node >= 14, while `datadog-cdk-constructs` supports Node >= 12.
+* `datadog-cdk-constructs-v2` contains more features.
 * Otherwise, the use of the two packages is identical.
 
 ## npm Package Installation:
 
 For use with AWS CDK v2:
 
 ```
@@ -77,14 +78,15 @@
   extensionLayerVersion: "<EXTENSION_VERSION>",
   forwarderArn: "<FORWARDER_ARN>",
   createForwarderPermissions: <BOOLEAN>,
   flushMetricsToLogs: <BOOLEAN>,
   site: "<SITE>",
   apiKey: "{Datadog_API_Key}",
   apiKeySecretArn: "{Secret_ARN_Datadog_API_Key}",
+  apiKeySecret: <AWS_CDK_ISECRET>, // Only available in datadog-cdk-constructs-v2
   apiKmsKey: "{Encrypted_Datadog_API_Key}",
   enableDatadogTracing: <BOOLEAN>,
   enableMergeXrayTraces: <BOOLEAN>,
   enableDatadogLogs: <BOOLEAN>,
   injectLogContext: <BOOLEAN>,
   logLevel: <STRING>,
   env: <STRING>, //Optional
@@ -181,14 +183,15 @@
 | `extensionLayerVersion` | `extension_layer_version` | Version of the Datadog Lambda Extension layer to install, such as 5. When `extensionLayerVersion` is set, `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`) needs to be set as well. When enabled, lambda function log groups will not be subscribed by the forwarder. Learn more about the Lambda extension [here](https://docs.datadoghq.com/serverless/datadog_lambda_library/extension/). |
 | `forwarderArn` | `forwarder_arn` | When set, the plugin will automatically subscribe the Datadog Forwarder to the functions' log groups. Do not set `forwarderArn` when `extensionLayerVersion` is set. |
 | `createForwarderPermissions` | `createForwarderPermissions` | When set to `true`, creates a Lambda permission on the the Datadog Forwarder per log group. Since the Datadog Forwarder has permissions configured by default, this is unnecessary in most use cases. |
 | `flushMetricsToLogs` | `flush_metrics_to_logs` | Send custom metrics using CloudWatch logs with the Datadog Forwarder Lambda function (recommended). Defaults to `true` . If you disable this parameter, it's required to set `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`). |
 | `site` | `site` | Set which Datadog site to send data. This is only used when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. Possible values are `datadoghq.com`, `datadoghq.eu`, `us3.datadoghq.com`, `us5.datadoghq.com`, `ap1.datadoghq.com`, and `ddog-gov.com`. The default is `datadoghq.com`. |
 | `apiKey` | `api_key` | Datadog API Key, only needed when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. For more information about getting a Datadog API key, see the [API key documentation](https://docs.datadoghq.com/account_management/api-app-keys/#api-keys). |
 | `apiKeySecretArn` | `api_key_secret_arn` | The ARN of the secret storing the Datadog API key in AWS Secrets Manager. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayer` is set. Remember to add the `secretsmanager:GetSecretValue` permission to the Lambda execution role. |
+| `apiKeySecret` | `api_key_secret` | An [AWS CDK ISecret](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_secretsmanager.ISecret.html) representing a secret storing the Datadog API key in AWS Secrets Manager. Use this parameter in place of `apiKeySecretArn` to automatically grant your Lambda execution roles read access to the given secret. [See here](#automatically-grant-aws-secret-read-access-to-lambda-execution-role) for an example. **Only available in datadog-cdk-constructs-v2**. |
 | `apiKmsKey` | `api_kms_key` | Datadog API Key encrypted using KMS. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set, and you are using KMS encryption. |
 | `enableDatadogTracing` | `enable_datadog_tracing` | Enable Datadog tracing on your Lambda functions. Defaults to `true`. |
 | `enableMergeXrayTraces` | `enable_merge_xray_traces` | Enable merging X-Ray traces on your Lambda functions. Defaults to `false`. |
 | `enableDatadogLogs` | `enable_datadog_logs` | Send Lambda function logs to Datadog via the Datadog Lambda Extension.  Defaults to `true`. Note: This setting has no effect on logs sent via the Datadog Forwarder. |
 | `enableSourceCodeIntegration` | `enable_source_code_integration` | Enable Datadog Source Code Integration, connecting your telemetry with application code in your Git repositories. This requires the Datadog Github Integration to work, otherwise please follow the [alternative method](#alternative-methods-to-enable-source-code-integration). Learn more [here](https://docs.datadoghq.com/integrations/guide/source-code-integration/). Defaults to `true`. |
 | `injectLogContext` | `inject_log_context` | When set, the Lambda layer will automatically patch console.log with Datadog's tracing ids. Defaults to `true`. |
 | `logLevel` | `log_level` | When set to `debug`, the Datadog Lambda Library and Extension will log additional information to help troubleshoot issues. |
@@ -283,14 +286,34 @@
 }
 ```
 
 ### Tags
 
 Add tags to your constructs. We recommend setting an `env` and `service` tag to tie Datadog telemetry together. For more information see [official AWS documentation](https://docs.aws.amazon.com/cdk/latest/guide/tagging.html) and [CDK documentation](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.Tags.html).
 
+## Automatically grant AWS secret read access to Lambda execution role
+
+**Only available in datadog-cdk-constructs-v2**
+
+To automatically grant your Lambda execution roles read access to a given secret, pass in `apiKeySecret` in place of `apiKeySecretArn` when initializing the Datadog construct.
+
+```
+const { Secret } = require('aws-cdk-lib/aws-secretsmanager');
+
+const secret = Secret.fromSecretPartialArn(this, 'DatadogApiKeySecret', 'arn:aws:secretsmanager:us-west-1:123:secret:DATADOG_API_KEY');
+
+const datadog = new Datadog(this, 'Datadog', {
+  ...
+  apiKeySecret: secret
+  ...
+});
+```
+
+When `addLambdaFunctions` is called, the Datadog CDK construct grants your Lambda execution roles read access to the given AWS secret. This is done through the [AWS ISecret's grantRead function](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_secretsmanager.ISecret.html#grantwbrreadgrantee-versionstages).
+
 ## How it works
 
 The Datadog CDK construct takes in a list of lambda functions and installs the Datadog Lambda Library by attaching the Lambda Layers for [Java](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk), [Node.js](https://github.com/DataDog/datadog-lambda-layer-js), and [Python](https://github.com/DataDog/datadog-lambda-layer-python) to your functions. It redirects to a replacement handler that initializes the Lambda Library without any required code changes. Additional configurations added to the Datadog CDK construct will also translate into their respective environment variables under each lambda function (if applicable / required).
 
 While Lambda function based log groups are handled by the `addLambdaFunctions` method automatically, the construct has an additional function `addForwarderToNonLambdaLogGroups` which subscribes the forwarder to any additional log groups of your choosing.
 
 ## Resources to learn about CDK
```

### Comparing `datadog-cdk-constructs-v2-1.7.1/setup.py` & `datadog-cdk-constructs-v2-1.7.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "datadog-cdk-constructs-v2",
-    "version": "1.7.1",
+    "version": "1.7.3",
     "description": "CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2",
     "license": "Apache-2.0",
     "url": "https://github.com/DataDog/datadog-cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "Datadog",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "datadog_cdk_constructs_v2",
         "datadog_cdk_constructs_v2._jsii"
     ],
     "package_data": {
         "datadog_cdk_constructs_v2._jsii": [
-            "datadog-cdk-constructs-v2@1.7.1.jsii.tgz"
+            "datadog-cdk-constructs-v2@1.7.3.jsii.tgz"
         ],
         "datadog_cdk_constructs_v2": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2/__init__.py` & `datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -15,15 +15,16 @@
 * Enabling the collection of traces and custom metrics from your Lambda functions.
 * Managing subscriptions from the Datadog Forwarder to your Lambda and non-Lambda log groups.
 
 ## AWS CDK v1 vs AWS CDK v2
 
 Two separate versions of Datadog CDK Constructs exist; `datadog-cdk-constructs` and `datadog-cdk-constructs-v2`. These are designed to work with `AWS CDK v1` and `AWS CDK v2` respectively.
 
-* `datadog-cdk-constructs-v2` requires Node 14+, while `datadog-cdk-constructs-v1` supports Node 12+.
+* `datadog-cdk-constructs-v2` requires Node >= 14, while `datadog-cdk-constructs` supports Node >= 12.
+* `datadog-cdk-constructs-v2` contains more features.
 * Otherwise, the use of the two packages is identical.
 
 ## npm Package Installation:
 
 For use with AWS CDK v2:
 
 ```
@@ -78,14 +79,15 @@
   extensionLayerVersion: "<EXTENSION_VERSION>",
   forwarderArn: "<FORWARDER_ARN>",
   createForwarderPermissions: <BOOLEAN>,
   flushMetricsToLogs: <BOOLEAN>,
   site: "<SITE>",
   apiKey: "{Datadog_API_Key}",
   apiKeySecretArn: "{Secret_ARN_Datadog_API_Key}",
+  apiKeySecret: <AWS_CDK_ISECRET>, // Only available in datadog-cdk-constructs-v2
   apiKmsKey: "{Encrypted_Datadog_API_Key}",
   enableDatadogTracing: <BOOLEAN>,
   enableMergeXrayTraces: <BOOLEAN>,
   enableDatadogLogs: <BOOLEAN>,
   injectLogContext: <BOOLEAN>,
   logLevel: <STRING>,
   env: <STRING>, //Optional
@@ -182,14 +184,15 @@
 | `extensionLayerVersion` | `extension_layer_version` | Version of the Datadog Lambda Extension layer to install, such as 5. When `extensionLayerVersion` is set, `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`) needs to be set as well. When enabled, lambda function log groups will not be subscribed by the forwarder. Learn more about the Lambda extension [here](https://docs.datadoghq.com/serverless/datadog_lambda_library/extension/). |
 | `forwarderArn` | `forwarder_arn` | When set, the plugin will automatically subscribe the Datadog Forwarder to the functions' log groups. Do not set `forwarderArn` when `extensionLayerVersion` is set. |
 | `createForwarderPermissions` | `createForwarderPermissions` | When set to `true`, creates a Lambda permission on the the Datadog Forwarder per log group. Since the Datadog Forwarder has permissions configured by default, this is unnecessary in most use cases. |
 | `flushMetricsToLogs` | `flush_metrics_to_logs` | Send custom metrics using CloudWatch logs with the Datadog Forwarder Lambda function (recommended). Defaults to `true` . If you disable this parameter, it's required to set `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`). |
 | `site` | `site` | Set which Datadog site to send data. This is only used when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. Possible values are `datadoghq.com`, `datadoghq.eu`, `us3.datadoghq.com`, `us5.datadoghq.com`, `ap1.datadoghq.com`, and `ddog-gov.com`. The default is `datadoghq.com`. |
 | `apiKey` | `api_key` | Datadog API Key, only needed when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. For more information about getting a Datadog API key, see the [API key documentation](https://docs.datadoghq.com/account_management/api-app-keys/#api-keys). |
 | `apiKeySecretArn` | `api_key_secret_arn` | The ARN of the secret storing the Datadog API key in AWS Secrets Manager. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayer` is set. Remember to add the `secretsmanager:GetSecretValue` permission to the Lambda execution role. |
+| `apiKeySecret` | `api_key_secret` | An [AWS CDK ISecret](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_secretsmanager.ISecret.html) representing a secret storing the Datadog API key in AWS Secrets Manager. Use this parameter in place of `apiKeySecretArn` to automatically grant your Lambda execution roles read access to the given secret. [See here](#automatically-grant-aws-secret-read-access-to-lambda-execution-role) for an example. **Only available in datadog-cdk-constructs-v2**. |
 | `apiKmsKey` | `api_kms_key` | Datadog API Key encrypted using KMS. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set, and you are using KMS encryption. |
 | `enableDatadogTracing` | `enable_datadog_tracing` | Enable Datadog tracing on your Lambda functions. Defaults to `true`. |
 | `enableMergeXrayTraces` | `enable_merge_xray_traces` | Enable merging X-Ray traces on your Lambda functions. Defaults to `false`. |
 | `enableDatadogLogs` | `enable_datadog_logs` | Send Lambda function logs to Datadog via the Datadog Lambda Extension.  Defaults to `true`. Note: This setting has no effect on logs sent via the Datadog Forwarder. |
 | `enableSourceCodeIntegration` | `enable_source_code_integration` | Enable Datadog Source Code Integration, connecting your telemetry with application code in your Git repositories. This requires the Datadog Github Integration to work, otherwise please follow the [alternative method](#alternative-methods-to-enable-source-code-integration). Learn more [here](https://docs.datadoghq.com/integrations/guide/source-code-integration/). Defaults to `true`. |
 | `injectLogContext` | `inject_log_context` | When set, the Lambda layer will automatically patch console.log with Datadog's tracing ids. Defaults to `true`. |
 | `logLevel` | `log_level` | When set to `debug`, the Datadog Lambda Library and Extension will log additional information to help troubleshoot issues. |
@@ -284,14 +287,34 @@
 }
 ```
 
 ### Tags
 
 Add tags to your constructs. We recommend setting an `env` and `service` tag to tie Datadog telemetry together. For more information see [official AWS documentation](https://docs.aws.amazon.com/cdk/latest/guide/tagging.html) and [CDK documentation](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.Tags.html).
 
+## Automatically grant AWS secret read access to Lambda execution role
+
+**Only available in datadog-cdk-constructs-v2**
+
+To automatically grant your Lambda execution roles read access to a given secret, pass in `apiKeySecret` in place of `apiKeySecretArn` when initializing the Datadog construct.
+
+```
+const { Secret } = require('aws-cdk-lib/aws-secretsmanager');
+
+const secret = Secret.fromSecretPartialArn(this, 'DatadogApiKeySecret', 'arn:aws:secretsmanager:us-west-1:123:secret:DATADOG_API_KEY');
+
+const datadog = new Datadog(this, 'Datadog', {
+  ...
+  apiKeySecret: secret
+  ...
+});
+```
+
+When `addLambdaFunctions` is called, the Datadog CDK construct grants your Lambda execution roles read access to the given AWS secret. This is done through the [AWS ISecret's grantRead function](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_secretsmanager.ISecret.html#grantwbrreadgrantee-versionstages).
+
 ## How it works
 
 The Datadog CDK construct takes in a list of lambda functions and installs the Datadog Lambda Library by attaching the Lambda Layers for [Java](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk), [Node.js](https://github.com/DataDog/datadog-lambda-layer-js), and [Python](https://github.com/DataDog/datadog-lambda-layer-python) to your functions. It redirects to a replacement handler that initializes the Lambda Library without any required code changes. Additional configurations added to the Datadog CDK construct will also translate into their respective environment variables under each lambda function (if applicable / required).
 
 While Lambda function based log groups are handled by the `addLambdaFunctions` method automatically, the construct has an additional function `addForwarderToNonLambdaLogGroups` which subscribes the forwarder to any additional log groups of your choosing.
 
 ## Resources to learn about CDK
@@ -402,25 +425,27 @@
         enable_merge_xray_traces: typing.Optional[builtins.bool] = None,
         enable_profiling: typing.Optional[builtins.bool] = None,
         encode_authorizer_context: typing.Optional[builtins.bool] = None,
         env: typing.Optional[builtins.str] = None,
         extension_layer_version: typing.Optional[jsii.Number] = None,
         flush_metrics_to_logs: typing.Optional[builtins.bool] = None,
         forwarder_arn: typing.Optional[builtins.str] = None,
+        grant_secret_read_access: typing.Optional[builtins.bool] = None,
         inject_log_context: typing.Optional[builtins.bool] = None,
         java_layer_version: typing.Optional[jsii.Number] = None,
         log_level: typing.Optional[builtins.str] = None,
         min_cold_start_trace_duration: typing.Optional[jsii.Number] = None,
         node_layer_version: typing.Optional[jsii.Number] = None,
         python_layer_version: typing.Optional[jsii.Number] = None,
         redirect_handler: typing.Optional[builtins.bool] = None,
         service: typing.Optional[builtins.str] = None,
         site: typing.Optional[builtins.str] = None,
         source_code_integration: typing.Optional[builtins.bool] = None,
         tags: typing.Optional[builtins.str] = None,
+        use_layers_from_account: typing.Optional[builtins.str] = None,
         version: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param scope: -
         :param id: -
         :param add_layers: 
         :param api_key: 
@@ -438,25 +463,27 @@
         :param enable_merge_xray_traces: 
         :param enable_profiling: 
         :param encode_authorizer_context: 
         :param env: 
         :param extension_layer_version: 
         :param flush_metrics_to_logs: 
         :param forwarder_arn: 
+        :param grant_secret_read_access: 
         :param inject_log_context: 
         :param java_layer_version: 
         :param log_level: 
         :param min_cold_start_trace_duration: 
         :param node_layer_version: 
         :param python_layer_version: 
         :param redirect_handler: 
         :param service: 
         :param site: 
         :param source_code_integration: 
         :param tags: 
+        :param use_layers_from_account: 
         :param version: 
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__74e095ab68a1ec6a36ad77e9741c22f8922ea76270d93f498ffa8f7846214a75)
             check_type(argname="argument scope", value=scope, expected_type=type_hints["scope"])
             check_type(argname="argument id", value=id, expected_type=type_hints["id"])
         props = DatadogPropsV2(
@@ -476,25 +503,27 @@
             enable_merge_xray_traces=enable_merge_xray_traces,
             enable_profiling=enable_profiling,
             encode_authorizer_context=encode_authorizer_context,
             env=env,
             extension_layer_version=extension_layer_version,
             flush_metrics_to_logs=flush_metrics_to_logs,
             forwarder_arn=forwarder_arn,
+            grant_secret_read_access=grant_secret_read_access,
             inject_log_context=inject_log_context,
             java_layer_version=java_layer_version,
             log_level=log_level,
             min_cold_start_trace_duration=min_cold_start_trace_duration,
             node_layer_version=node_layer_version,
             python_layer_version=python_layer_version,
             redirect_handler=redirect_handler,
             service=service,
             site=site,
             source_code_integration=source_code_integration,
             tags=tags,
+            use_layers_from_account=use_layers_from_account,
             version=version,
         )
 
         jsii.create(self.__class__, self, [scope, id, props])
 
     @jsii.member(jsii_name="addForwarderToNonLambdaLogGroups")
     def add_forwarder_to_non_lambda_log_groups(
@@ -528,22 +557,25 @@
             check_type(argname="argument git_repo_url", value=git_repo_url, expected_type=type_hints["git_repo_url"])
         return typing.cast(None, jsii.invoke(self, "addGitCommitMetadata", [lambda_functions, git_commit_sha, git_repo_url]))
 
     @jsii.member(jsii_name="addLambdaFunctions")
     def add_lambda_functions(
         self,
         lambda_functions: typing.Sequence[typing.Union[_aws_cdk_aws_lambda_ceddda9d.Function, _aws_cdk_aws_lambda_nodejs_ceddda9d.NodejsFunction, _aws_cdk_aws_lambda_python_alpha_49328424.PythonFunction]],
+        construct: typing.Optional[_constructs_77d1e7e8.Construct] = None,
     ) -> None:
         '''
         :param lambda_functions: -
+        :param construct: -
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__0803e2c5aafb02535548377e1d71bf561393d99ceb98d9e94251f36f8877c881)
             check_type(argname="argument lambda_functions", value=lambda_functions, expected_type=type_hints["lambda_functions"])
-        return typing.cast(None, jsii.invoke(self, "addLambdaFunctions", [lambda_functions]))
+            check_type(argname="argument construct", value=construct, expected_type=type_hints["construct"])
+        return typing.cast(None, jsii.invoke(self, "addLambdaFunctions", [lambda_functions, construct]))
 
     @builtins.property
     @jsii.member(jsii_name="props")
     def props(self) -> "DatadogPropsV2":
         return typing.cast("DatadogPropsV2", jsii.get(self, "props"))
 
     @props.setter
@@ -575,20 +607,19 @@
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__9fbc38dc0dcc9d23ae91b812a896ee83f74291c635b835f5075d3b2e8f971337)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "transport", value)
 
 
 @jsii.data_type(
-    jsii_type="datadog-cdk-constructs-v2.DatadogPropsV2",
+    jsii_type="datadog-cdk-constructs-v2.DatadogProps",
     jsii_struct_bases=[],
     name_mapping={
         "add_layers": "addLayers",
         "api_key": "apiKey",
-        "api_key_secret": "apiKeySecret",
         "api_key_secret_arn": "apiKeySecretArn",
         "api_kms_key": "apiKmsKey",
         "apm_flush_deadline": "apmFlushDeadline",
         "capture_lambda_payload": "captureLambdaPayload",
         "cold_start_trace_skip_libs": "coldStartTraceSkipLibs",
         "create_forwarder_permissions": "createForwarderPermissions",
         "decode_authorizer_context": "decodeAuthorizerContext",
@@ -598,35 +629,36 @@
         "enable_merge_xray_traces": "enableMergeXrayTraces",
         "enable_profiling": "enableProfiling",
         "encode_authorizer_context": "encodeAuthorizerContext",
         "env": "env",
         "extension_layer_version": "extensionLayerVersion",
         "flush_metrics_to_logs": "flushMetricsToLogs",
         "forwarder_arn": "forwarderArn",
+        "grant_secret_read_access": "grantSecretReadAccess",
         "inject_log_context": "injectLogContext",
         "java_layer_version": "javaLayerVersion",
         "log_level": "logLevel",
         "min_cold_start_trace_duration": "minColdStartTraceDuration",
         "node_layer_version": "nodeLayerVersion",
         "python_layer_version": "pythonLayerVersion",
         "redirect_handler": "redirectHandler",
         "service": "service",
         "site": "site",
         "source_code_integration": "sourceCodeIntegration",
         "tags": "tags",
+        "use_layers_from_account": "useLayersFromAccount",
         "version": "version",
     },
 )
-class DatadogPropsV2:
+class DatadogProps:
     def __init__(
         self,
         *,
         add_layers: typing.Optional[builtins.bool] = None,
         api_key: typing.Optional[builtins.str] = None,
-        api_key_secret: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
         api_key_secret_arn: typing.Optional[builtins.str] = None,
         api_kms_key: typing.Optional[builtins.str] = None,
         apm_flush_deadline: typing.Optional[typing.Union[builtins.str, jsii.Number]] = None,
         capture_lambda_payload: typing.Optional[builtins.bool] = None,
         cold_start_trace_skip_libs: typing.Optional[builtins.str] = None,
         create_forwarder_permissions: typing.Optional[builtins.bool] = None,
         decode_authorizer_context: typing.Optional[builtins.bool] = None,
@@ -636,31 +668,32 @@
         enable_merge_xray_traces: typing.Optional[builtins.bool] = None,
         enable_profiling: typing.Optional[builtins.bool] = None,
         encode_authorizer_context: typing.Optional[builtins.bool] = None,
         env: typing.Optional[builtins.str] = None,
         extension_layer_version: typing.Optional[jsii.Number] = None,
         flush_metrics_to_logs: typing.Optional[builtins.bool] = None,
         forwarder_arn: typing.Optional[builtins.str] = None,
+        grant_secret_read_access: typing.Optional[builtins.bool] = None,
         inject_log_context: typing.Optional[builtins.bool] = None,
         java_layer_version: typing.Optional[jsii.Number] = None,
         log_level: typing.Optional[builtins.str] = None,
         min_cold_start_trace_duration: typing.Optional[jsii.Number] = None,
         node_layer_version: typing.Optional[jsii.Number] = None,
         python_layer_version: typing.Optional[jsii.Number] = None,
         redirect_handler: typing.Optional[builtins.bool] = None,
         service: typing.Optional[builtins.str] = None,
         site: typing.Optional[builtins.str] = None,
         source_code_integration: typing.Optional[builtins.bool] = None,
         tags: typing.Optional[builtins.str] = None,
+        use_layers_from_account: typing.Optional[builtins.str] = None,
         version: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param add_layers: 
         :param api_key: 
-        :param api_key_secret: 
         :param api_key_secret_arn: 
         :param api_kms_key: 
         :param apm_flush_deadline: 
         :param capture_lambda_payload: 
         :param cold_start_trace_skip_libs: 
         :param create_forwarder_permissions: 
         :param decode_authorizer_context: 
@@ -670,32 +703,33 @@
         :param enable_merge_xray_traces: 
         :param enable_profiling: 
         :param encode_authorizer_context: 
         :param env: 
         :param extension_layer_version: 
         :param flush_metrics_to_logs: 
         :param forwarder_arn: 
+        :param grant_secret_read_access: 
         :param inject_log_context: 
         :param java_layer_version: 
         :param log_level: 
         :param min_cold_start_trace_duration: 
         :param node_layer_version: 
         :param python_layer_version: 
         :param redirect_handler: 
         :param service: 
         :param site: 
         :param source_code_integration: 
         :param tags: 
+        :param use_layers_from_account: 
         :param version: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__605aaf2fbceb6cc8efeeafa174ece774a500681952f201662eed10acfc3ab544)
+            type_hints = typing.get_type_hints(_typecheckingstub__5b78922f591d5e7cd5e1fdd07bf0372e40211fa86d3614124736912aec2a7d33)
             check_type(argname="argument add_layers", value=add_layers, expected_type=type_hints["add_layers"])
             check_type(argname="argument api_key", value=api_key, expected_type=type_hints["api_key"])
-            check_type(argname="argument api_key_secret", value=api_key_secret, expected_type=type_hints["api_key_secret"])
             check_type(argname="argument api_key_secret_arn", value=api_key_secret_arn, expected_type=type_hints["api_key_secret_arn"])
             check_type(argname="argument api_kms_key", value=api_kms_key, expected_type=type_hints["api_kms_key"])
             check_type(argname="argument apm_flush_deadline", value=apm_flush_deadline, expected_type=type_hints["apm_flush_deadline"])
             check_type(argname="argument capture_lambda_payload", value=capture_lambda_payload, expected_type=type_hints["capture_lambda_payload"])
             check_type(argname="argument cold_start_trace_skip_libs", value=cold_start_trace_skip_libs, expected_type=type_hints["cold_start_trace_skip_libs"])
             check_type(argname="argument create_forwarder_permissions", value=create_forwarder_permissions, expected_type=type_hints["create_forwarder_permissions"])
             check_type(argname="argument decode_authorizer_context", value=decode_authorizer_context, expected_type=type_hints["decode_authorizer_context"])
@@ -705,33 +739,33 @@
             check_type(argname="argument enable_merge_xray_traces", value=enable_merge_xray_traces, expected_type=type_hints["enable_merge_xray_traces"])
             check_type(argname="argument enable_profiling", value=enable_profiling, expected_type=type_hints["enable_profiling"])
             check_type(argname="argument encode_authorizer_context", value=encode_authorizer_context, expected_type=type_hints["encode_authorizer_context"])
             check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument extension_layer_version", value=extension_layer_version, expected_type=type_hints["extension_layer_version"])
             check_type(argname="argument flush_metrics_to_logs", value=flush_metrics_to_logs, expected_type=type_hints["flush_metrics_to_logs"])
             check_type(argname="argument forwarder_arn", value=forwarder_arn, expected_type=type_hints["forwarder_arn"])
+            check_type(argname="argument grant_secret_read_access", value=grant_secret_read_access, expected_type=type_hints["grant_secret_read_access"])
             check_type(argname="argument inject_log_context", value=inject_log_context, expected_type=type_hints["inject_log_context"])
             check_type(argname="argument java_layer_version", value=java_layer_version, expected_type=type_hints["java_layer_version"])
             check_type(argname="argument log_level", value=log_level, expected_type=type_hints["log_level"])
             check_type(argname="argument min_cold_start_trace_duration", value=min_cold_start_trace_duration, expected_type=type_hints["min_cold_start_trace_duration"])
             check_type(argname="argument node_layer_version", value=node_layer_version, expected_type=type_hints["node_layer_version"])
             check_type(argname="argument python_layer_version", value=python_layer_version, expected_type=type_hints["python_layer_version"])
             check_type(argname="argument redirect_handler", value=redirect_handler, expected_type=type_hints["redirect_handler"])
             check_type(argname="argument service", value=service, expected_type=type_hints["service"])
             check_type(argname="argument site", value=site, expected_type=type_hints["site"])
             check_type(argname="argument source_code_integration", value=source_code_integration, expected_type=type_hints["source_code_integration"])
             check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument use_layers_from_account", value=use_layers_from_account, expected_type=type_hints["use_layers_from_account"])
             check_type(argname="argument version", value=version, expected_type=type_hints["version"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
         if add_layers is not None:
             self._values["add_layers"] = add_layers
         if api_key is not None:
             self._values["api_key"] = api_key
-        if api_key_secret is not None:
-            self._values["api_key_secret"] = api_key_secret
         if api_key_secret_arn is not None:
             self._values["api_key_secret_arn"] = api_key_secret_arn
         if api_kms_key is not None:
             self._values["api_kms_key"] = api_kms_key
         if apm_flush_deadline is not None:
             self._values["apm_flush_deadline"] = apm_flush_deadline
         if capture_lambda_payload is not None:
@@ -758,14 +792,16 @@
             self._values["env"] = env
         if extension_layer_version is not None:
             self._values["extension_layer_version"] = extension_layer_version
         if flush_metrics_to_logs is not None:
             self._values["flush_metrics_to_logs"] = flush_metrics_to_logs
         if forwarder_arn is not None:
             self._values["forwarder_arn"] = forwarder_arn
+        if grant_secret_read_access is not None:
+            self._values["grant_secret_read_access"] = grant_secret_read_access
         if inject_log_context is not None:
             self._values["inject_log_context"] = inject_log_context
         if java_layer_version is not None:
             self._values["java_layer_version"] = java_layer_version
         if log_level is not None:
             self._values["log_level"] = log_level
         if min_cold_start_trace_duration is not None:
@@ -780,35 +816,30 @@
             self._values["service"] = service
         if site is not None:
             self._values["site"] = site
         if source_code_integration is not None:
             self._values["source_code_integration"] = source_code_integration
         if tags is not None:
             self._values["tags"] = tags
+        if use_layers_from_account is not None:
+            self._values["use_layers_from_account"] = use_layers_from_account
         if version is not None:
             self._values["version"] = version
 
     @builtins.property
     def add_layers(self) -> typing.Optional[builtins.bool]:
         result = self._values.get("add_layers")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def api_key(self) -> typing.Optional[builtins.str]:
         result = self._values.get("api_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def api_key_secret(
-        self,
-    ) -> typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret]:
-        result = self._values.get("api_key_secret")
-        return typing.cast(typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret], result)
-
-    @builtins.property
     def api_key_secret_arn(self) -> typing.Optional[builtins.str]:
         result = self._values.get("api_key_secret_arn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def api_kms_key(self) -> typing.Optional[builtins.str]:
         result = self._values.get("api_kms_key")
@@ -888,14 +919,19 @@
 
     @builtins.property
     def forwarder_arn(self) -> typing.Optional[builtins.str]:
         result = self._values.get("forwarder_arn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def grant_secret_read_access(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("grant_secret_read_access")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def inject_log_context(self) -> typing.Optional[builtins.bool]:
         result = self._values.get("inject_log_context")
         return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def java_layer_version(self) -> typing.Optional[jsii.Number]:
         result = self._values.get("java_layer_version")
@@ -943,602 +979,690 @@
 
     @builtins.property
     def tags(self) -> typing.Optional[builtins.str]:
         result = self._values.get("tags")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def use_layers_from_account(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("use_layers_from_account")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
     def version(self) -> typing.Optional[builtins.str]:
         result = self._values.get("version")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
-        return "DatadogPropsV2(%s)" % ", ".join(
+        return "DatadogProps(%s)" % ", ".join(
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
-    jsii_type="datadog-cdk-constructs-v2.DatadogStrictProps",
+    jsii_type="datadog-cdk-constructs-v2.DatadogPropsV2",
     jsii_struct_bases=[],
     name_mapping={
         "add_layers": "addLayers",
+        "api_key": "apiKey",
+        "api_key_secret": "apiKeySecret",
+        "api_key_secret_arn": "apiKeySecretArn",
+        "api_kms_key": "apiKmsKey",
+        "apm_flush_deadline": "apmFlushDeadline",
         "capture_lambda_payload": "captureLambdaPayload",
+        "cold_start_trace_skip_libs": "coldStartTraceSkipLibs",
+        "create_forwarder_permissions": "createForwarderPermissions",
+        "decode_authorizer_context": "decodeAuthorizerContext",
+        "enable_cold_start_tracing": "enableColdStartTracing",
         "enable_datadog_logs": "enableDatadogLogs",
         "enable_datadog_tracing": "enableDatadogTracing",
         "enable_merge_xray_traces": "enableMergeXrayTraces",
-        "inject_log_context": "injectLogContext",
-        "api_key": "apiKey",
-        "api_key_secret_arn": "apiKeySecretArn",
-        "api_kms_key": "apiKmsKey",
+        "enable_profiling": "enableProfiling",
+        "encode_authorizer_context": "encodeAuthorizerContext",
+        "env": "env",
         "extension_layer_version": "extensionLayerVersion",
         "flush_metrics_to_logs": "flushMetricsToLogs",
         "forwarder_arn": "forwarderArn",
+        "grant_secret_read_access": "grantSecretReadAccess",
+        "inject_log_context": "injectLogContext",
         "java_layer_version": "javaLayerVersion",
         "log_level": "logLevel",
+        "min_cold_start_trace_duration": "minColdStartTraceDuration",
         "node_layer_version": "nodeLayerVersion",
         "python_layer_version": "pythonLayerVersion",
         "redirect_handler": "redirectHandler",
+        "service": "service",
         "site": "site",
         "source_code_integration": "sourceCodeIntegration",
+        "tags": "tags",
+        "use_layers_from_account": "useLayersFromAccount",
+        "version": "version",
     },
 )
-class DatadogStrictProps:
+class DatadogPropsV2:
     def __init__(
         self,
         *,
-        add_layers: builtins.bool,
-        capture_lambda_payload: builtins.bool,
-        enable_datadog_logs: builtins.bool,
-        enable_datadog_tracing: builtins.bool,
-        enable_merge_xray_traces: builtins.bool,
-        inject_log_context: builtins.bool,
+        add_layers: typing.Optional[builtins.bool] = None,
         api_key: typing.Optional[builtins.str] = None,
+        api_key_secret: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
         api_key_secret_arn: typing.Optional[builtins.str] = None,
         api_kms_key: typing.Optional[builtins.str] = None,
+        apm_flush_deadline: typing.Optional[typing.Union[builtins.str, jsii.Number]] = None,
+        capture_lambda_payload: typing.Optional[builtins.bool] = None,
+        cold_start_trace_skip_libs: typing.Optional[builtins.str] = None,
+        create_forwarder_permissions: typing.Optional[builtins.bool] = None,
+        decode_authorizer_context: typing.Optional[builtins.bool] = None,
+        enable_cold_start_tracing: typing.Optional[builtins.bool] = None,
+        enable_datadog_logs: typing.Optional[builtins.bool] = None,
+        enable_datadog_tracing: typing.Optional[builtins.bool] = None,
+        enable_merge_xray_traces: typing.Optional[builtins.bool] = None,
+        enable_profiling: typing.Optional[builtins.bool] = None,
+        encode_authorizer_context: typing.Optional[builtins.bool] = None,
+        env: typing.Optional[builtins.str] = None,
         extension_layer_version: typing.Optional[jsii.Number] = None,
         flush_metrics_to_logs: typing.Optional[builtins.bool] = None,
         forwarder_arn: typing.Optional[builtins.str] = None,
+        grant_secret_read_access: typing.Optional[builtins.bool] = None,
+        inject_log_context: typing.Optional[builtins.bool] = None,
         java_layer_version: typing.Optional[jsii.Number] = None,
         log_level: typing.Optional[builtins.str] = None,
+        min_cold_start_trace_duration: typing.Optional[jsii.Number] = None,
         node_layer_version: typing.Optional[jsii.Number] = None,
         python_layer_version: typing.Optional[jsii.Number] = None,
         redirect_handler: typing.Optional[builtins.bool] = None,
+        service: typing.Optional[builtins.str] = None,
         site: typing.Optional[builtins.str] = None,
         source_code_integration: typing.Optional[builtins.bool] = None,
+        tags: typing.Optional[builtins.str] = None,
+        use_layers_from_account: typing.Optional[builtins.str] = None,
+        version: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
         :param add_layers: 
+        :param api_key: 
+        :param api_key_secret: 
+        :param api_key_secret_arn: 
+        :param api_kms_key: 
+        :param apm_flush_deadline: 
         :param capture_lambda_payload: 
+        :param cold_start_trace_skip_libs: 
+        :param create_forwarder_permissions: 
+        :param decode_authorizer_context: 
+        :param enable_cold_start_tracing: 
         :param enable_datadog_logs: 
         :param enable_datadog_tracing: 
         :param enable_merge_xray_traces: 
-        :param inject_log_context: 
-        :param api_key: 
-        :param api_key_secret_arn: 
-        :param api_kms_key: 
+        :param enable_profiling: 
+        :param encode_authorizer_context: 
+        :param env: 
         :param extension_layer_version: 
         :param flush_metrics_to_logs: 
         :param forwarder_arn: 
+        :param grant_secret_read_access: 
+        :param inject_log_context: 
         :param java_layer_version: 
         :param log_level: 
+        :param min_cold_start_trace_duration: 
         :param node_layer_version: 
         :param python_layer_version: 
         :param redirect_handler: 
+        :param service: 
         :param site: 
         :param source_code_integration: 
+        :param tags: 
+        :param use_layers_from_account: 
+        :param version: 
         '''
         if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__c0d4909ff321b27042bd7da99817517e719945ec07952fd9fd3a213ccaf8b9d4)
+            type_hints = typing.get_type_hints(_typecheckingstub__605aaf2fbceb6cc8efeeafa174ece774a500681952f201662eed10acfc3ab544)
             check_type(argname="argument add_layers", value=add_layers, expected_type=type_hints["add_layers"])
+            check_type(argname="argument api_key", value=api_key, expected_type=type_hints["api_key"])
+            check_type(argname="argument api_key_secret", value=api_key_secret, expected_type=type_hints["api_key_secret"])
+            check_type(argname="argument api_key_secret_arn", value=api_key_secret_arn, expected_type=type_hints["api_key_secret_arn"])
+            check_type(argname="argument api_kms_key", value=api_kms_key, expected_type=type_hints["api_kms_key"])
+            check_type(argname="argument apm_flush_deadline", value=apm_flush_deadline, expected_type=type_hints["apm_flush_deadline"])
             check_type(argname="argument capture_lambda_payload", value=capture_lambda_payload, expected_type=type_hints["capture_lambda_payload"])
+            check_type(argname="argument cold_start_trace_skip_libs", value=cold_start_trace_skip_libs, expected_type=type_hints["cold_start_trace_skip_libs"])
+            check_type(argname="argument create_forwarder_permissions", value=create_forwarder_permissions, expected_type=type_hints["create_forwarder_permissions"])
+            check_type(argname="argument decode_authorizer_context", value=decode_authorizer_context, expected_type=type_hints["decode_authorizer_context"])
+            check_type(argname="argument enable_cold_start_tracing", value=enable_cold_start_tracing, expected_type=type_hints["enable_cold_start_tracing"])
             check_type(argname="argument enable_datadog_logs", value=enable_datadog_logs, expected_type=type_hints["enable_datadog_logs"])
             check_type(argname="argument enable_datadog_tracing", value=enable_datadog_tracing, expected_type=type_hints["enable_datadog_tracing"])
             check_type(argname="argument enable_merge_xray_traces", value=enable_merge_xray_traces, expected_type=type_hints["enable_merge_xray_traces"])
-            check_type(argname="argument inject_log_context", value=inject_log_context, expected_type=type_hints["inject_log_context"])
-            check_type(argname="argument api_key", value=api_key, expected_type=type_hints["api_key"])
-            check_type(argname="argument api_key_secret_arn", value=api_key_secret_arn, expected_type=type_hints["api_key_secret_arn"])
-            check_type(argname="argument api_kms_key", value=api_kms_key, expected_type=type_hints["api_kms_key"])
+            check_type(argname="argument enable_profiling", value=enable_profiling, expected_type=type_hints["enable_profiling"])
+            check_type(argname="argument encode_authorizer_context", value=encode_authorizer_context, expected_type=type_hints["encode_authorizer_context"])
+            check_type(argname="argument env", value=env, expected_type=type_hints["env"])
             check_type(argname="argument extension_layer_version", value=extension_layer_version, expected_type=type_hints["extension_layer_version"])
             check_type(argname="argument flush_metrics_to_logs", value=flush_metrics_to_logs, expected_type=type_hints["flush_metrics_to_logs"])
             check_type(argname="argument forwarder_arn", value=forwarder_arn, expected_type=type_hints["forwarder_arn"])
+            check_type(argname="argument grant_secret_read_access", value=grant_secret_read_access, expected_type=type_hints["grant_secret_read_access"])
+            check_type(argname="argument inject_log_context", value=inject_log_context, expected_type=type_hints["inject_log_context"])
             check_type(argname="argument java_layer_version", value=java_layer_version, expected_type=type_hints["java_layer_version"])
             check_type(argname="argument log_level", value=log_level, expected_type=type_hints["log_level"])
+            check_type(argname="argument min_cold_start_trace_duration", value=min_cold_start_trace_duration, expected_type=type_hints["min_cold_start_trace_duration"])
             check_type(argname="argument node_layer_version", value=node_layer_version, expected_type=type_hints["node_layer_version"])
             check_type(argname="argument python_layer_version", value=python_layer_version, expected_type=type_hints["python_layer_version"])
             check_type(argname="argument redirect_handler", value=redirect_handler, expected_type=type_hints["redirect_handler"])
+            check_type(argname="argument service", value=service, expected_type=type_hints["service"])
             check_type(argname="argument site", value=site, expected_type=type_hints["site"])
             check_type(argname="argument source_code_integration", value=source_code_integration, expected_type=type_hints["source_code_integration"])
-        self._values: typing.Dict[builtins.str, typing.Any] = {
-            "add_layers": add_layers,
-            "capture_lambda_payload": capture_lambda_payload,
-            "enable_datadog_logs": enable_datadog_logs,
-            "enable_datadog_tracing": enable_datadog_tracing,
-            "enable_merge_xray_traces": enable_merge_xray_traces,
-            "inject_log_context": inject_log_context,
-        }
+            check_type(argname="argument tags", value=tags, expected_type=type_hints["tags"])
+            check_type(argname="argument use_layers_from_account", value=use_layers_from_account, expected_type=type_hints["use_layers_from_account"])
+            check_type(argname="argument version", value=version, expected_type=type_hints["version"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if add_layers is not None:
+            self._values["add_layers"] = add_layers
         if api_key is not None:
             self._values["api_key"] = api_key
+        if api_key_secret is not None:
+            self._values["api_key_secret"] = api_key_secret
         if api_key_secret_arn is not None:
             self._values["api_key_secret_arn"] = api_key_secret_arn
         if api_kms_key is not None:
             self._values["api_kms_key"] = api_kms_key
+        if apm_flush_deadline is not None:
+            self._values["apm_flush_deadline"] = apm_flush_deadline
+        if capture_lambda_payload is not None:
+            self._values["capture_lambda_payload"] = capture_lambda_payload
+        if cold_start_trace_skip_libs is not None:
+            self._values["cold_start_trace_skip_libs"] = cold_start_trace_skip_libs
+        if create_forwarder_permissions is not None:
+            self._values["create_forwarder_permissions"] = create_forwarder_permissions
+        if decode_authorizer_context is not None:
+            self._values["decode_authorizer_context"] = decode_authorizer_context
+        if enable_cold_start_tracing is not None:
+            self._values["enable_cold_start_tracing"] = enable_cold_start_tracing
+        if enable_datadog_logs is not None:
+            self._values["enable_datadog_logs"] = enable_datadog_logs
+        if enable_datadog_tracing is not None:
+            self._values["enable_datadog_tracing"] = enable_datadog_tracing
+        if enable_merge_xray_traces is not None:
+            self._values["enable_merge_xray_traces"] = enable_merge_xray_traces
+        if enable_profiling is not None:
+            self._values["enable_profiling"] = enable_profiling
+        if encode_authorizer_context is not None:
+            self._values["encode_authorizer_context"] = encode_authorizer_context
+        if env is not None:
+            self._values["env"] = env
         if extension_layer_version is not None:
             self._values["extension_layer_version"] = extension_layer_version
         if flush_metrics_to_logs is not None:
             self._values["flush_metrics_to_logs"] = flush_metrics_to_logs
         if forwarder_arn is not None:
             self._values["forwarder_arn"] = forwarder_arn
+        if grant_secret_read_access is not None:
+            self._values["grant_secret_read_access"] = grant_secret_read_access
+        if inject_log_context is not None:
+            self._values["inject_log_context"] = inject_log_context
         if java_layer_version is not None:
             self._values["java_layer_version"] = java_layer_version
         if log_level is not None:
             self._values["log_level"] = log_level
+        if min_cold_start_trace_duration is not None:
+            self._values["min_cold_start_trace_duration"] = min_cold_start_trace_duration
         if node_layer_version is not None:
             self._values["node_layer_version"] = node_layer_version
         if python_layer_version is not None:
             self._values["python_layer_version"] = python_layer_version
         if redirect_handler is not None:
             self._values["redirect_handler"] = redirect_handler
+        if service is not None:
+            self._values["service"] = service
         if site is not None:
             self._values["site"] = site
         if source_code_integration is not None:
             self._values["source_code_integration"] = source_code_integration
+        if tags is not None:
+            self._values["tags"] = tags
+        if use_layers_from_account is not None:
+            self._values["use_layers_from_account"] = use_layers_from_account
+        if version is not None:
+            self._values["version"] = version
 
     @builtins.property
-    def add_layers(self) -> builtins.bool:
+    def add_layers(self) -> typing.Optional[builtins.bool]:
         result = self._values.get("add_layers")
-        assert result is not None, "Required property 'add_layers' is missing"
-        return typing.cast(builtins.bool, result)
-
-    @builtins.property
-    def capture_lambda_payload(self) -> builtins.bool:
-        result = self._values.get("capture_lambda_payload")
-        assert result is not None, "Required property 'capture_lambda_payload' is missing"
-        return typing.cast(builtins.bool, result)
-
-    @builtins.property
-    def enable_datadog_logs(self) -> builtins.bool:
-        result = self._values.get("enable_datadog_logs")
-        assert result is not None, "Required property 'enable_datadog_logs' is missing"
-        return typing.cast(builtins.bool, result)
-
-    @builtins.property
-    def enable_datadog_tracing(self) -> builtins.bool:
-        result = self._values.get("enable_datadog_tracing")
-        assert result is not None, "Required property 'enable_datadog_tracing' is missing"
-        return typing.cast(builtins.bool, result)
-
-    @builtins.property
-    def enable_merge_xray_traces(self) -> builtins.bool:
-        result = self._values.get("enable_merge_xray_traces")
-        assert result is not None, "Required property 'enable_merge_xray_traces' is missing"
-        return typing.cast(builtins.bool, result)
-
-    @builtins.property
-    def inject_log_context(self) -> builtins.bool:
-        result = self._values.get("inject_log_context")
-        assert result is not None, "Required property 'inject_log_context' is missing"
-        return typing.cast(builtins.bool, result)
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
     def api_key(self) -> typing.Optional[builtins.str]:
         result = self._values.get("api_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
+    def api_key_secret(
+        self,
+    ) -> typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret]:
+        result = self._values.get("api_key_secret")
+        return typing.cast(typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret], result)
+
+    @builtins.property
     def api_key_secret_arn(self) -> typing.Optional[builtins.str]:
         result = self._values.get("api_key_secret_arn")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def api_kms_key(self) -> typing.Optional[builtins.str]:
         result = self._values.get("api_kms_key")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    def extension_layer_version(self) -> typing.Optional[jsii.Number]:
-        result = self._values.get("extension_layer_version")
-        return typing.cast(typing.Optional[jsii.Number], result)
-
-    @builtins.property
-    def flush_metrics_to_logs(self) -> typing.Optional[builtins.bool]:
-        result = self._values.get("flush_metrics_to_logs")
-        return typing.cast(typing.Optional[builtins.bool], result)
-
-    @builtins.property
-    def forwarder_arn(self) -> typing.Optional[builtins.str]:
-        result = self._values.get("forwarder_arn")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
-    def java_layer_version(self) -> typing.Optional[jsii.Number]:
-        result = self._values.get("java_layer_version")
-        return typing.cast(typing.Optional[jsii.Number], result)
-
-    @builtins.property
-    def log_level(self) -> typing.Optional[builtins.str]:
-        result = self._values.get("log_level")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
-    def node_layer_version(self) -> typing.Optional[jsii.Number]:
-        result = self._values.get("node_layer_version")
-        return typing.cast(typing.Optional[jsii.Number], result)
-
-    @builtins.property
-    def python_layer_version(self) -> typing.Optional[jsii.Number]:
-        result = self._values.get("python_layer_version")
-        return typing.cast(typing.Optional[jsii.Number], result)
-
-    @builtins.property
-    def redirect_handler(self) -> typing.Optional[builtins.bool]:
-        result = self._values.get("redirect_handler")
-        return typing.cast(typing.Optional[builtins.bool], result)
-
-    @builtins.property
-    def site(self) -> typing.Optional[builtins.str]:
-        result = self._values.get("site")
-        return typing.cast(typing.Optional[builtins.str], result)
-
-    @builtins.property
-    def source_code_integration(self) -> typing.Optional[builtins.bool]:
-        result = self._values.get("source_code_integration")
-        return typing.cast(typing.Optional[builtins.bool], result)
-
-    def __eq__(self, rhs: typing.Any) -> builtins.bool:
-        return isinstance(rhs, self.__class__) and rhs._values == self._values
-
-    def __ne__(self, rhs: typing.Any) -> builtins.bool:
-        return not (rhs == self)
-
-    def __repr__(self) -> str:
-        return "DatadogStrictProps(%s)" % ", ".join(
-            k + "=" + repr(v) for k, v in self._values.items()
-        )
-
-
-@jsii.interface(jsii_type="datadog-cdk-constructs-v2.IDatadogProps")
-class IDatadogProps(typing_extensions.Protocol):
-    @builtins.property
-    @jsii.member(jsii_name="addLayers")
-    def add_layers(self) -> typing.Optional[builtins.bool]:
-        ...
-
-    @builtins.property
-    @jsii.member(jsii_name="apiKey")
-    def api_key(self) -> typing.Optional[builtins.str]:
-        ...
-
-    @builtins.property
-    @jsii.member(jsii_name="apiKmsKey")
-    def api_kms_key(self) -> typing.Optional[builtins.str]:
-        ...
-
-    @builtins.property
-    @jsii.member(jsii_name="apmFlushDeadline")
     def apm_flush_deadline(
         self,
     ) -> typing.Optional[typing.Union[builtins.str, jsii.Number]]:
-        ...
+        result = self._values.get("apm_flush_deadline")
+        return typing.cast(typing.Optional[typing.Union[builtins.str, jsii.Number]], result)
 
     @builtins.property
-    @jsii.member(jsii_name="captureLambdaPayload")
     def capture_lambda_payload(self) -> typing.Optional[builtins.bool]:
-        ...
+        result = self._values.get("capture_lambda_payload")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="coldStartTraceSkipLibs")
     def cold_start_trace_skip_libs(self) -> typing.Optional[builtins.str]:
-        ...
+        result = self._values.get("cold_start_trace_skip_libs")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="createForwarderPermissions")
     def create_forwarder_permissions(self) -> typing.Optional[builtins.bool]:
-        ...
+        result = self._values.get("create_forwarder_permissions")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="decodeAuthorizerContext")
     def decode_authorizer_context(self) -> typing.Optional[builtins.bool]:
-        ...
+        result = self._values.get("decode_authorizer_context")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="enableColdStartTracing")
     def enable_cold_start_tracing(self) -> typing.Optional[builtins.bool]:
-        ...
+        result = self._values.get("enable_cold_start_tracing")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="enableDatadogLogs")
     def enable_datadog_logs(self) -> typing.Optional[builtins.bool]:
-        ...
+        result = self._values.get("enable_datadog_logs")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="enableDatadogTracing")
     def enable_datadog_tracing(self) -> typing.Optional[builtins.bool]:
-        ...
+        result = self._values.get("enable_datadog_tracing")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="enableMergeXrayTraces")
     def enable_merge_xray_traces(self) -> typing.Optional[builtins.bool]:
-        ...
+        result = self._values.get("enable_merge_xray_traces")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="enableProfiling")
     def enable_profiling(self) -> typing.Optional[builtins.bool]:
-        ...
+        result = self._values.get("enable_profiling")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="encodeAuthorizerContext")
     def encode_authorizer_context(self) -> typing.Optional[builtins.bool]:
-        ...
+        result = self._values.get("encode_authorizer_context")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="env")
     def env(self) -> typing.Optional[builtins.str]:
-        ...
+        result = self._values.get("env")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="extensionLayerVersion")
     def extension_layer_version(self) -> typing.Optional[jsii.Number]:
-        ...
+        result = self._values.get("extension_layer_version")
+        return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    @jsii.member(jsii_name="flushMetricsToLogs")
     def flush_metrics_to_logs(self) -> typing.Optional[builtins.bool]:
-        ...
+        result = self._values.get("flush_metrics_to_logs")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="forwarderArn")
     def forwarder_arn(self) -> typing.Optional[builtins.str]:
-        ...
+        result = self._values.get("forwarder_arn")
+        return typing.cast(typing.Optional[builtins.str], result)
+
+    @builtins.property
+    def grant_secret_read_access(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("grant_secret_read_access")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="injectLogContext")
     def inject_log_context(self) -> typing.Optional[builtins.bool]:
-        ...
+        result = self._values.get("inject_log_context")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="javaLayerVersion")
     def java_layer_version(self) -> typing.Optional[jsii.Number]:
-        ...
+        result = self._values.get("java_layer_version")
+        return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    @jsii.member(jsii_name="logLevel")
     def log_level(self) -> typing.Optional[builtins.str]:
-        ...
+        result = self._values.get("log_level")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="minColdStartTraceDuration")
     def min_cold_start_trace_duration(self) -> typing.Optional[jsii.Number]:
-        ...
+        result = self._values.get("min_cold_start_trace_duration")
+        return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    @jsii.member(jsii_name="nodeLayerVersion")
     def node_layer_version(self) -> typing.Optional[jsii.Number]:
-        ...
+        result = self._values.get("node_layer_version")
+        return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    @jsii.member(jsii_name="pythonLayerVersion")
     def python_layer_version(self) -> typing.Optional[jsii.Number]:
-        ...
+        result = self._values.get("python_layer_version")
+        return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    @jsii.member(jsii_name="redirectHandler")
     def redirect_handler(self) -> typing.Optional[builtins.bool]:
-        ...
+        result = self._values.get("redirect_handler")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="service")
     def service(self) -> typing.Optional[builtins.str]:
-        ...
+        result = self._values.get("service")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="site")
     def site(self) -> typing.Optional[builtins.str]:
-        ...
+        result = self._values.get("site")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="sourceCodeIntegration")
     def source_code_integration(self) -> typing.Optional[builtins.bool]:
-        ...
+        result = self._values.get("source_code_integration")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="tags")
     def tags(self) -> typing.Optional[builtins.str]:
-        ...
+        result = self._values.get("tags")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="version")
-    def version(self) -> typing.Optional[builtins.str]:
-        ...
+    def use_layers_from_account(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("use_layers_from_account")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="apiKeySecretArn")
-    def api_key_secret_arn(self) -> typing.Optional[builtins.str]:
-        ...
-
-    @api_key_secret_arn.setter
-    def api_key_secret_arn(self, value: typing.Optional[builtins.str]) -> None:
-        ...
-
+    def version(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("version")
+        return typing.cast(typing.Optional[builtins.str], result)
 
-class _IDatadogPropsProxy:
-    __jsii_type__: typing.ClassVar[str] = "datadog-cdk-constructs-v2.IDatadogProps"
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
 
-    @builtins.property
-    @jsii.member(jsii_name="addLayers")
-    def add_layers(self) -> typing.Optional[builtins.bool]:
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "addLayers"))
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
 
-    @builtins.property
-    @jsii.member(jsii_name="apiKey")
-    def api_key(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "apiKey"))
+    def __repr__(self) -> str:
+        return "DatadogPropsV2(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
 
-    @builtins.property
-    @jsii.member(jsii_name="apiKmsKey")
-    def api_kms_key(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "apiKmsKey"))
 
-    @builtins.property
-    @jsii.member(jsii_name="apmFlushDeadline")
-    def apm_flush_deadline(
+@jsii.data_type(
+    jsii_type="datadog-cdk-constructs-v2.DatadogStrictProps",
+    jsii_struct_bases=[],
+    name_mapping={
+        "add_layers": "addLayers",
+        "capture_lambda_payload": "captureLambdaPayload",
+        "enable_datadog_logs": "enableDatadogLogs",
+        "enable_datadog_tracing": "enableDatadogTracing",
+        "enable_merge_xray_traces": "enableMergeXrayTraces",
+        "grant_secret_read_access": "grantSecretReadAccess",
+        "inject_log_context": "injectLogContext",
+        "api_key": "apiKey",
+        "api_key_secret_arn": "apiKeySecretArn",
+        "api_kms_key": "apiKmsKey",
+        "extension_layer_version": "extensionLayerVersion",
+        "flush_metrics_to_logs": "flushMetricsToLogs",
+        "forwarder_arn": "forwarderArn",
+        "java_layer_version": "javaLayerVersion",
+        "log_level": "logLevel",
+        "node_layer_version": "nodeLayerVersion",
+        "python_layer_version": "pythonLayerVersion",
+        "redirect_handler": "redirectHandler",
+        "site": "site",
+        "source_code_integration": "sourceCodeIntegration",
+    },
+)
+class DatadogStrictProps:
+    def __init__(
         self,
-    ) -> typing.Optional[typing.Union[builtins.str, jsii.Number]]:
-        return typing.cast(typing.Optional[typing.Union[builtins.str, jsii.Number]], jsii.get(self, "apmFlushDeadline"))
-
-    @builtins.property
-    @jsii.member(jsii_name="captureLambdaPayload")
-    def capture_lambda_payload(self) -> typing.Optional[builtins.bool]:
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "captureLambdaPayload"))
+        *,
+        add_layers: builtins.bool,
+        capture_lambda_payload: builtins.bool,
+        enable_datadog_logs: builtins.bool,
+        enable_datadog_tracing: builtins.bool,
+        enable_merge_xray_traces: builtins.bool,
+        grant_secret_read_access: builtins.bool,
+        inject_log_context: builtins.bool,
+        api_key: typing.Optional[builtins.str] = None,
+        api_key_secret_arn: typing.Optional[builtins.str] = None,
+        api_kms_key: typing.Optional[builtins.str] = None,
+        extension_layer_version: typing.Optional[jsii.Number] = None,
+        flush_metrics_to_logs: typing.Optional[builtins.bool] = None,
+        forwarder_arn: typing.Optional[builtins.str] = None,
+        java_layer_version: typing.Optional[jsii.Number] = None,
+        log_level: typing.Optional[builtins.str] = None,
+        node_layer_version: typing.Optional[jsii.Number] = None,
+        python_layer_version: typing.Optional[jsii.Number] = None,
+        redirect_handler: typing.Optional[builtins.bool] = None,
+        site: typing.Optional[builtins.str] = None,
+        source_code_integration: typing.Optional[builtins.bool] = None,
+    ) -> None:
+        '''
+        :param add_layers: 
+        :param capture_lambda_payload: 
+        :param enable_datadog_logs: 
+        :param enable_datadog_tracing: 
+        :param enable_merge_xray_traces: 
+        :param grant_secret_read_access: 
+        :param inject_log_context: 
+        :param api_key: 
+        :param api_key_secret_arn: 
+        :param api_kms_key: 
+        :param extension_layer_version: 
+        :param flush_metrics_to_logs: 
+        :param forwarder_arn: 
+        :param java_layer_version: 
+        :param log_level: 
+        :param node_layer_version: 
+        :param python_layer_version: 
+        :param redirect_handler: 
+        :param site: 
+        :param source_code_integration: 
+        '''
+        if __debug__:
+            type_hints = typing.get_type_hints(_typecheckingstub__c0d4909ff321b27042bd7da99817517e719945ec07952fd9fd3a213ccaf8b9d4)
+            check_type(argname="argument add_layers", value=add_layers, expected_type=type_hints["add_layers"])
+            check_type(argname="argument capture_lambda_payload", value=capture_lambda_payload, expected_type=type_hints["capture_lambda_payload"])
+            check_type(argname="argument enable_datadog_logs", value=enable_datadog_logs, expected_type=type_hints["enable_datadog_logs"])
+            check_type(argname="argument enable_datadog_tracing", value=enable_datadog_tracing, expected_type=type_hints["enable_datadog_tracing"])
+            check_type(argname="argument enable_merge_xray_traces", value=enable_merge_xray_traces, expected_type=type_hints["enable_merge_xray_traces"])
+            check_type(argname="argument grant_secret_read_access", value=grant_secret_read_access, expected_type=type_hints["grant_secret_read_access"])
+            check_type(argname="argument inject_log_context", value=inject_log_context, expected_type=type_hints["inject_log_context"])
+            check_type(argname="argument api_key", value=api_key, expected_type=type_hints["api_key"])
+            check_type(argname="argument api_key_secret_arn", value=api_key_secret_arn, expected_type=type_hints["api_key_secret_arn"])
+            check_type(argname="argument api_kms_key", value=api_kms_key, expected_type=type_hints["api_kms_key"])
+            check_type(argname="argument extension_layer_version", value=extension_layer_version, expected_type=type_hints["extension_layer_version"])
+            check_type(argname="argument flush_metrics_to_logs", value=flush_metrics_to_logs, expected_type=type_hints["flush_metrics_to_logs"])
+            check_type(argname="argument forwarder_arn", value=forwarder_arn, expected_type=type_hints["forwarder_arn"])
+            check_type(argname="argument java_layer_version", value=java_layer_version, expected_type=type_hints["java_layer_version"])
+            check_type(argname="argument log_level", value=log_level, expected_type=type_hints["log_level"])
+            check_type(argname="argument node_layer_version", value=node_layer_version, expected_type=type_hints["node_layer_version"])
+            check_type(argname="argument python_layer_version", value=python_layer_version, expected_type=type_hints["python_layer_version"])
+            check_type(argname="argument redirect_handler", value=redirect_handler, expected_type=type_hints["redirect_handler"])
+            check_type(argname="argument site", value=site, expected_type=type_hints["site"])
+            check_type(argname="argument source_code_integration", value=source_code_integration, expected_type=type_hints["source_code_integration"])
+        self._values: typing.Dict[builtins.str, typing.Any] = {
+            "add_layers": add_layers,
+            "capture_lambda_payload": capture_lambda_payload,
+            "enable_datadog_logs": enable_datadog_logs,
+            "enable_datadog_tracing": enable_datadog_tracing,
+            "enable_merge_xray_traces": enable_merge_xray_traces,
+            "grant_secret_read_access": grant_secret_read_access,
+            "inject_log_context": inject_log_context,
+        }
+        if api_key is not None:
+            self._values["api_key"] = api_key
+        if api_key_secret_arn is not None:
+            self._values["api_key_secret_arn"] = api_key_secret_arn
+        if api_kms_key is not None:
+            self._values["api_kms_key"] = api_kms_key
+        if extension_layer_version is not None:
+            self._values["extension_layer_version"] = extension_layer_version
+        if flush_metrics_to_logs is not None:
+            self._values["flush_metrics_to_logs"] = flush_metrics_to_logs
+        if forwarder_arn is not None:
+            self._values["forwarder_arn"] = forwarder_arn
+        if java_layer_version is not None:
+            self._values["java_layer_version"] = java_layer_version
+        if log_level is not None:
+            self._values["log_level"] = log_level
+        if node_layer_version is not None:
+            self._values["node_layer_version"] = node_layer_version
+        if python_layer_version is not None:
+            self._values["python_layer_version"] = python_layer_version
+        if redirect_handler is not None:
+            self._values["redirect_handler"] = redirect_handler
+        if site is not None:
+            self._values["site"] = site
+        if source_code_integration is not None:
+            self._values["source_code_integration"] = source_code_integration
 
     @builtins.property
-    @jsii.member(jsii_name="coldStartTraceSkipLibs")
-    def cold_start_trace_skip_libs(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "coldStartTraceSkipLibs"))
+    def add_layers(self) -> builtins.bool:
+        result = self._values.get("add_layers")
+        assert result is not None, "Required property 'add_layers' is missing"
+        return typing.cast(builtins.bool, result)
 
     @builtins.property
-    @jsii.member(jsii_name="createForwarderPermissions")
-    def create_forwarder_permissions(self) -> typing.Optional[builtins.bool]:
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "createForwarderPermissions"))
+    def capture_lambda_payload(self) -> builtins.bool:
+        result = self._values.get("capture_lambda_payload")
+        assert result is not None, "Required property 'capture_lambda_payload' is missing"
+        return typing.cast(builtins.bool, result)
 
     @builtins.property
-    @jsii.member(jsii_name="decodeAuthorizerContext")
-    def decode_authorizer_context(self) -> typing.Optional[builtins.bool]:
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "decodeAuthorizerContext"))
+    def enable_datadog_logs(self) -> builtins.bool:
+        result = self._values.get("enable_datadog_logs")
+        assert result is not None, "Required property 'enable_datadog_logs' is missing"
+        return typing.cast(builtins.bool, result)
 
     @builtins.property
-    @jsii.member(jsii_name="enableColdStartTracing")
-    def enable_cold_start_tracing(self) -> typing.Optional[builtins.bool]:
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "enableColdStartTracing"))
+    def enable_datadog_tracing(self) -> builtins.bool:
+        result = self._values.get("enable_datadog_tracing")
+        assert result is not None, "Required property 'enable_datadog_tracing' is missing"
+        return typing.cast(builtins.bool, result)
 
     @builtins.property
-    @jsii.member(jsii_name="enableDatadogLogs")
-    def enable_datadog_logs(self) -> typing.Optional[builtins.bool]:
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "enableDatadogLogs"))
+    def enable_merge_xray_traces(self) -> builtins.bool:
+        result = self._values.get("enable_merge_xray_traces")
+        assert result is not None, "Required property 'enable_merge_xray_traces' is missing"
+        return typing.cast(builtins.bool, result)
 
     @builtins.property
-    @jsii.member(jsii_name="enableDatadogTracing")
-    def enable_datadog_tracing(self) -> typing.Optional[builtins.bool]:
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "enableDatadogTracing"))
+    def grant_secret_read_access(self) -> builtins.bool:
+        result = self._values.get("grant_secret_read_access")
+        assert result is not None, "Required property 'grant_secret_read_access' is missing"
+        return typing.cast(builtins.bool, result)
 
     @builtins.property
-    @jsii.member(jsii_name="enableMergeXrayTraces")
-    def enable_merge_xray_traces(self) -> typing.Optional[builtins.bool]:
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "enableMergeXrayTraces"))
+    def inject_log_context(self) -> builtins.bool:
+        result = self._values.get("inject_log_context")
+        assert result is not None, "Required property 'inject_log_context' is missing"
+        return typing.cast(builtins.bool, result)
 
     @builtins.property
-    @jsii.member(jsii_name="enableProfiling")
-    def enable_profiling(self) -> typing.Optional[builtins.bool]:
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "enableProfiling"))
+    def api_key(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("api_key")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="encodeAuthorizerContext")
-    def encode_authorizer_context(self) -> typing.Optional[builtins.bool]:
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "encodeAuthorizerContext"))
+    def api_key_secret_arn(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("api_key_secret_arn")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="env")
-    def env(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "env"))
+    def api_kms_key(self) -> typing.Optional[builtins.str]:
+        result = self._values.get("api_kms_key")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="extensionLayerVersion")
     def extension_layer_version(self) -> typing.Optional[jsii.Number]:
-        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "extensionLayerVersion"))
+        result = self._values.get("extension_layer_version")
+        return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    @jsii.member(jsii_name="flushMetricsToLogs")
     def flush_metrics_to_logs(self) -> typing.Optional[builtins.bool]:
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "flushMetricsToLogs"))
+        result = self._values.get("flush_metrics_to_logs")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="forwarderArn")
     def forwarder_arn(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "forwarderArn"))
-
-    @builtins.property
-    @jsii.member(jsii_name="injectLogContext")
-    def inject_log_context(self) -> typing.Optional[builtins.bool]:
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "injectLogContext"))
+        result = self._values.get("forwarder_arn")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="javaLayerVersion")
     def java_layer_version(self) -> typing.Optional[jsii.Number]:
-        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "javaLayerVersion"))
+        result = self._values.get("java_layer_version")
+        return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    @jsii.member(jsii_name="logLevel")
     def log_level(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "logLevel"))
-
-    @builtins.property
-    @jsii.member(jsii_name="minColdStartTraceDuration")
-    def min_cold_start_trace_duration(self) -> typing.Optional[jsii.Number]:
-        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "minColdStartTraceDuration"))
+        result = self._values.get("log_level")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="nodeLayerVersion")
     def node_layer_version(self) -> typing.Optional[jsii.Number]:
-        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "nodeLayerVersion"))
+        result = self._values.get("node_layer_version")
+        return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    @jsii.member(jsii_name="pythonLayerVersion")
     def python_layer_version(self) -> typing.Optional[jsii.Number]:
-        return typing.cast(typing.Optional[jsii.Number], jsii.get(self, "pythonLayerVersion"))
+        result = self._values.get("python_layer_version")
+        return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
-    @jsii.member(jsii_name="redirectHandler")
     def redirect_handler(self) -> typing.Optional[builtins.bool]:
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "redirectHandler"))
-
-    @builtins.property
-    @jsii.member(jsii_name="service")
-    def service(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "service"))
+        result = self._values.get("redirect_handler")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
     @builtins.property
-    @jsii.member(jsii_name="site")
     def site(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "site"))
+        result = self._values.get("site")
+        return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
-    @jsii.member(jsii_name="sourceCodeIntegration")
     def source_code_integration(self) -> typing.Optional[builtins.bool]:
-        return typing.cast(typing.Optional[builtins.bool], jsii.get(self, "sourceCodeIntegration"))
-
-    @builtins.property
-    @jsii.member(jsii_name="tags")
-    def tags(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "tags"))
-
-    @builtins.property
-    @jsii.member(jsii_name="version")
-    def version(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "version"))
+        result = self._values.get("source_code_integration")
+        return typing.cast(typing.Optional[builtins.bool], result)
 
-    @builtins.property
-    @jsii.member(jsii_name="apiKeySecretArn")
-    def api_key_secret_arn(self) -> typing.Optional[builtins.str]:
-        return typing.cast(typing.Optional[builtins.str], jsii.get(self, "apiKeySecretArn"))
+    def __eq__(self, rhs: typing.Any) -> builtins.bool:
+        return isinstance(rhs, self.__class__) and rhs._values == self._values
 
-    @api_key_secret_arn.setter
-    def api_key_secret_arn(self, value: typing.Optional[builtins.str]) -> None:
-        if __debug__:
-            type_hints = typing.get_type_hints(_typecheckingstub__e8575dd8c5598108689e31cffc5a95a627de8ad5238fb62faa9d01bb0af57870)
-            check_type(argname="argument value", value=value, expected_type=type_hints["value"])
-        jsii.set(self, "apiKeySecretArn", value)
+    def __ne__(self, rhs: typing.Any) -> builtins.bool:
+        return not (rhs == self)
 
-# Adding a "__jsii_proxy_class__(): typing.Type" function to the interface
-typing.cast(typing.Any, IDatadogProps).__jsii_proxy_class__ = lambda : _IDatadogPropsProxy
+    def __repr__(self) -> str:
+        return "DatadogStrictProps(%s)" % ", ".join(
+            k + "=" + repr(v) for k, v in self._values.items()
+        )
 
 
 @jsii.interface(jsii_type="datadog-cdk-constructs-v2.ILambdaFunction")
 class ILambdaFunction(typing_extensions.Protocol):
     @builtins.property
     @jsii.member(jsii_name="node")
     def node(self) -> "Node":
@@ -1820,17 +1944,17 @@
             type_hints = typing.get_type_hints(_typecheckingstub__b5e4df65851315cbd779a7d51db28b4f9f2ff24e8d2030ab94830e4548e02f64)
             check_type(argname="argument value", value=value, expected_type=type_hints["value"])
         jsii.set(self, "extensionLayerVersion", value)
 
 
 __all__ = [
     "Datadog",
+    "DatadogProps",
     "DatadogPropsV2",
     "DatadogStrictProps",
-    "IDatadogProps",
     "ILambdaFunction",
     "Node",
     "Runtime",
     "RuntimeType",
     "TagKeys",
     "Transport",
 ]
@@ -1857,25 +1981,27 @@
     enable_merge_xray_traces: typing.Optional[builtins.bool] = None,
     enable_profiling: typing.Optional[builtins.bool] = None,
     encode_authorizer_context: typing.Optional[builtins.bool] = None,
     env: typing.Optional[builtins.str] = None,
     extension_layer_version: typing.Optional[jsii.Number] = None,
     flush_metrics_to_logs: typing.Optional[builtins.bool] = None,
     forwarder_arn: typing.Optional[builtins.str] = None,
+    grant_secret_read_access: typing.Optional[builtins.bool] = None,
     inject_log_context: typing.Optional[builtins.bool] = None,
     java_layer_version: typing.Optional[jsii.Number] = None,
     log_level: typing.Optional[builtins.str] = None,
     min_cold_start_trace_duration: typing.Optional[jsii.Number] = None,
     node_layer_version: typing.Optional[jsii.Number] = None,
     python_layer_version: typing.Optional[jsii.Number] = None,
     redirect_handler: typing.Optional[builtins.bool] = None,
     service: typing.Optional[builtins.str] = None,
     site: typing.Optional[builtins.str] = None,
     source_code_integration: typing.Optional[builtins.bool] = None,
     tags: typing.Optional[builtins.str] = None,
+    use_layers_from_account: typing.Optional[builtins.str] = None,
     version: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__b2299a0a72b8c17837c229cea786d90db2682af81487298b4e2cf18be55f3dc9(
     log_groups: typing.Sequence[_aws_cdk_aws_logs_ceddda9d.ILogGroup],
@@ -1889,14 +2015,15 @@
     git_repo_url: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__0803e2c5aafb02535548377e1d71bf561393d99ceb98d9e94251f36f8877c881(
     lambda_functions: typing.Sequence[typing.Union[_aws_cdk_aws_lambda_ceddda9d.Function, _aws_cdk_aws_lambda_nodejs_ceddda9d.NodejsFunction, _aws_cdk_aws_lambda_python_alpha_49328424.PythonFunction]],
+    construct: typing.Optional[_constructs_77d1e7e8.Construct] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__09c760f7e7825eca68e7aa97831bccc7713602c7ae04ada36965093ff03a5fde(
     value: DatadogPropsV2,
 ) -> None:
@@ -1911,14 +2038,53 @@
 
 def _typecheckingstub__9fbc38dc0dcc9d23ae91b812a896ee83f74291c635b835f5075d3b2e8f971337(
     value: Transport,
 ) -> None:
     """Type checking stubs"""
     pass
 
+def _typecheckingstub__5b78922f591d5e7cd5e1fdd07bf0372e40211fa86d3614124736912aec2a7d33(
+    *,
+    add_layers: typing.Optional[builtins.bool] = None,
+    api_key: typing.Optional[builtins.str] = None,
+    api_key_secret_arn: typing.Optional[builtins.str] = None,
+    api_kms_key: typing.Optional[builtins.str] = None,
+    apm_flush_deadline: typing.Optional[typing.Union[builtins.str, jsii.Number]] = None,
+    capture_lambda_payload: typing.Optional[builtins.bool] = None,
+    cold_start_trace_skip_libs: typing.Optional[builtins.str] = None,
+    create_forwarder_permissions: typing.Optional[builtins.bool] = None,
+    decode_authorizer_context: typing.Optional[builtins.bool] = None,
+    enable_cold_start_tracing: typing.Optional[builtins.bool] = None,
+    enable_datadog_logs: typing.Optional[builtins.bool] = None,
+    enable_datadog_tracing: typing.Optional[builtins.bool] = None,
+    enable_merge_xray_traces: typing.Optional[builtins.bool] = None,
+    enable_profiling: typing.Optional[builtins.bool] = None,
+    encode_authorizer_context: typing.Optional[builtins.bool] = None,
+    env: typing.Optional[builtins.str] = None,
+    extension_layer_version: typing.Optional[jsii.Number] = None,
+    flush_metrics_to_logs: typing.Optional[builtins.bool] = None,
+    forwarder_arn: typing.Optional[builtins.str] = None,
+    grant_secret_read_access: typing.Optional[builtins.bool] = None,
+    inject_log_context: typing.Optional[builtins.bool] = None,
+    java_layer_version: typing.Optional[jsii.Number] = None,
+    log_level: typing.Optional[builtins.str] = None,
+    min_cold_start_trace_duration: typing.Optional[jsii.Number] = None,
+    node_layer_version: typing.Optional[jsii.Number] = None,
+    python_layer_version: typing.Optional[jsii.Number] = None,
+    redirect_handler: typing.Optional[builtins.bool] = None,
+    service: typing.Optional[builtins.str] = None,
+    site: typing.Optional[builtins.str] = None,
+    source_code_integration: typing.Optional[builtins.bool] = None,
+    tags: typing.Optional[builtins.str] = None,
+    use_layers_from_account: typing.Optional[builtins.str] = None,
+    version: typing.Optional[builtins.str] = None,
+) -> None:
+    """Type checking stubs"""
+    pass
+
 def _typecheckingstub__605aaf2fbceb6cc8efeeafa174ece774a500681952f201662eed10acfc3ab544(
     *,
     add_layers: typing.Optional[builtins.bool] = None,
     api_key: typing.Optional[builtins.str] = None,
     api_key_secret: typing.Optional[_aws_cdk_aws_secretsmanager_ceddda9d.ISecret] = None,
     api_key_secret_arn: typing.Optional[builtins.str] = None,
     api_kms_key: typing.Optional[builtins.str] = None,
@@ -1933,37 +2099,40 @@
     enable_merge_xray_traces: typing.Optional[builtins.bool] = None,
     enable_profiling: typing.Optional[builtins.bool] = None,
     encode_authorizer_context: typing.Optional[builtins.bool] = None,
     env: typing.Optional[builtins.str] = None,
     extension_layer_version: typing.Optional[jsii.Number] = None,
     flush_metrics_to_logs: typing.Optional[builtins.bool] = None,
     forwarder_arn: typing.Optional[builtins.str] = None,
+    grant_secret_read_access: typing.Optional[builtins.bool] = None,
     inject_log_context: typing.Optional[builtins.bool] = None,
     java_layer_version: typing.Optional[jsii.Number] = None,
     log_level: typing.Optional[builtins.str] = None,
     min_cold_start_trace_duration: typing.Optional[jsii.Number] = None,
     node_layer_version: typing.Optional[jsii.Number] = None,
     python_layer_version: typing.Optional[jsii.Number] = None,
     redirect_handler: typing.Optional[builtins.bool] = None,
     service: typing.Optional[builtins.str] = None,
     site: typing.Optional[builtins.str] = None,
     source_code_integration: typing.Optional[builtins.bool] = None,
     tags: typing.Optional[builtins.str] = None,
+    use_layers_from_account: typing.Optional[builtins.str] = None,
     version: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__c0d4909ff321b27042bd7da99817517e719945ec07952fd9fd3a213ccaf8b9d4(
     *,
     add_layers: builtins.bool,
     capture_lambda_payload: builtins.bool,
     enable_datadog_logs: builtins.bool,
     enable_datadog_tracing: builtins.bool,
     enable_merge_xray_traces: builtins.bool,
+    grant_secret_read_access: builtins.bool,
     inject_log_context: builtins.bool,
     api_key: typing.Optional[builtins.str] = None,
     api_key_secret_arn: typing.Optional[builtins.str] = None,
     api_kms_key: typing.Optional[builtins.str] = None,
     extension_layer_version: typing.Optional[jsii.Number] = None,
     flush_metrics_to_logs: typing.Optional[builtins.bool] = None,
     forwarder_arn: typing.Optional[builtins.str] = None,
@@ -1974,20 +2143,14 @@
     redirect_handler: typing.Optional[builtins.bool] = None,
     site: typing.Optional[builtins.str] = None,
     source_code_integration: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
-def _typecheckingstub__e8575dd8c5598108689e31cffc5a95a627de8ad5238fb62faa9d01bb0af57870(
-    value: typing.Optional[builtins.str],
-) -> None:
-    """Type checking stubs"""
-    pass
-
 def _typecheckingstub__8fd9ea625d2ef267cd51675f7bc9ed93c806c411dc2ed28173160e9e99445ec2(
     value: Node,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__9982ab95a46df98104a3d1863d5bb0f9e9809ccc59137b73f0b2f7ff79e464a7(
```

### Comparing `datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO` & `datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-cdk-constructs-v2
-Version: 1.7.1
+Version: 1.7.3
 Summary: CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog using AWS CDK v2
 Home-page: https://github.com/DataDog/datadog-cdk-constructs
 Author: Datadog
 License: Apache-2.0
 Project-URL: Source, https://github.com/DataDog/datadog-cdk-constructs
 Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
@@ -38,15 +38,16 @@
 * Enabling the collection of traces and custom metrics from your Lambda functions.
 * Managing subscriptions from the Datadog Forwarder to your Lambda and non-Lambda log groups.
 
 ## AWS CDK v1 vs AWS CDK v2
 
 Two separate versions of Datadog CDK Constructs exist; `datadog-cdk-constructs` and `datadog-cdk-constructs-v2`. These are designed to work with `AWS CDK v1` and `AWS CDK v2` respectively.
 
-* `datadog-cdk-constructs-v2` requires Node 14+, while `datadog-cdk-constructs-v1` supports Node 12+.
+* `datadog-cdk-constructs-v2` requires Node >= 14, while `datadog-cdk-constructs` supports Node >= 12.
+* `datadog-cdk-constructs-v2` contains more features.
 * Otherwise, the use of the two packages is identical.
 
 ## npm Package Installation:
 
 For use with AWS CDK v2:
 
 ```
@@ -101,14 +102,15 @@
   extensionLayerVersion: "<EXTENSION_VERSION>",
   forwarderArn: "<FORWARDER_ARN>",
   createForwarderPermissions: <BOOLEAN>,
   flushMetricsToLogs: <BOOLEAN>,
   site: "<SITE>",
   apiKey: "{Datadog_API_Key}",
   apiKeySecretArn: "{Secret_ARN_Datadog_API_Key}",
+  apiKeySecret: <AWS_CDK_ISECRET>, // Only available in datadog-cdk-constructs-v2
   apiKmsKey: "{Encrypted_Datadog_API_Key}",
   enableDatadogTracing: <BOOLEAN>,
   enableMergeXrayTraces: <BOOLEAN>,
   enableDatadogLogs: <BOOLEAN>,
   injectLogContext: <BOOLEAN>,
   logLevel: <STRING>,
   env: <STRING>, //Optional
@@ -205,14 +207,15 @@
 | `extensionLayerVersion` | `extension_layer_version` | Version of the Datadog Lambda Extension layer to install, such as 5. When `extensionLayerVersion` is set, `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`) needs to be set as well. When enabled, lambda function log groups will not be subscribed by the forwarder. Learn more about the Lambda extension [here](https://docs.datadoghq.com/serverless/datadog_lambda_library/extension/). |
 | `forwarderArn` | `forwarder_arn` | When set, the plugin will automatically subscribe the Datadog Forwarder to the functions' log groups. Do not set `forwarderArn` when `extensionLayerVersion` is set. |
 | `createForwarderPermissions` | `createForwarderPermissions` | When set to `true`, creates a Lambda permission on the the Datadog Forwarder per log group. Since the Datadog Forwarder has permissions configured by default, this is unnecessary in most use cases. |
 | `flushMetricsToLogs` | `flush_metrics_to_logs` | Send custom metrics using CloudWatch logs with the Datadog Forwarder Lambda function (recommended). Defaults to `true` . If you disable this parameter, it's required to set `apiKey` (or if encrypted, `apiKMSKey` or `apiKeySecretArn`). |
 | `site` | `site` | Set which Datadog site to send data. This is only used when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. Possible values are `datadoghq.com`, `datadoghq.eu`, `us3.datadoghq.com`, `us5.datadoghq.com`, `ap1.datadoghq.com`, and `ddog-gov.com`. The default is `datadoghq.com`. |
 | `apiKey` | `api_key` | Datadog API Key, only needed when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set. For more information about getting a Datadog API key, see the [API key documentation](https://docs.datadoghq.com/account_management/api-app-keys/#api-keys). |
 | `apiKeySecretArn` | `api_key_secret_arn` | The ARN of the secret storing the Datadog API key in AWS Secrets Manager. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayer` is set. Remember to add the `secretsmanager:GetSecretValue` permission to the Lambda execution role. |
+| `apiKeySecret` | `api_key_secret` | An [AWS CDK ISecret](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_secretsmanager.ISecret.html) representing a secret storing the Datadog API key in AWS Secrets Manager. Use this parameter in place of `apiKeySecretArn` to automatically grant your Lambda execution roles read access to the given secret. [See here](#automatically-grant-aws-secret-read-access-to-lambda-execution-role) for an example. **Only available in datadog-cdk-constructs-v2**. |
 | `apiKmsKey` | `api_kms_key` | Datadog API Key encrypted using KMS. Use this parameter in place of `apiKey` when `flushMetricsToLogs` is `false` or `extensionLayerVersion` is set, and you are using KMS encryption. |
 | `enableDatadogTracing` | `enable_datadog_tracing` | Enable Datadog tracing on your Lambda functions. Defaults to `true`. |
 | `enableMergeXrayTraces` | `enable_merge_xray_traces` | Enable merging X-Ray traces on your Lambda functions. Defaults to `false`. |
 | `enableDatadogLogs` | `enable_datadog_logs` | Send Lambda function logs to Datadog via the Datadog Lambda Extension.  Defaults to `true`. Note: This setting has no effect on logs sent via the Datadog Forwarder. |
 | `enableSourceCodeIntegration` | `enable_source_code_integration` | Enable Datadog Source Code Integration, connecting your telemetry with application code in your Git repositories. This requires the Datadog Github Integration to work, otherwise please follow the [alternative method](#alternative-methods-to-enable-source-code-integration). Learn more [here](https://docs.datadoghq.com/integrations/guide/source-code-integration/). Defaults to `true`. |
 | `injectLogContext` | `inject_log_context` | When set, the Lambda layer will automatically patch console.log with Datadog's tracing ids. Defaults to `true`. |
 | `logLevel` | `log_level` | When set to `debug`, the Datadog Lambda Library and Extension will log additional information to help troubleshoot issues. |
@@ -307,14 +310,34 @@
 }
 ```
 
 ### Tags
 
 Add tags to your constructs. We recommend setting an `env` and `service` tag to tie Datadog telemetry together. For more information see [official AWS documentation](https://docs.aws.amazon.com/cdk/latest/guide/tagging.html) and [CDK documentation](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.Tags.html).
 
+## Automatically grant AWS secret read access to Lambda execution role
+
+**Only available in datadog-cdk-constructs-v2**
+
+To automatically grant your Lambda execution roles read access to a given secret, pass in `apiKeySecret` in place of `apiKeySecretArn` when initializing the Datadog construct.
+
+```
+const { Secret } = require('aws-cdk-lib/aws-secretsmanager');
+
+const secret = Secret.fromSecretPartialArn(this, 'DatadogApiKeySecret', 'arn:aws:secretsmanager:us-west-1:123:secret:DATADOG_API_KEY');
+
+const datadog = new Datadog(this, 'Datadog', {
+  ...
+  apiKeySecret: secret
+  ...
+});
+```
+
+When `addLambdaFunctions` is called, the Datadog CDK construct grants your Lambda execution roles read access to the given AWS secret. This is done through the [AWS ISecret's grantRead function](https://docs.aws.amazon.com/cdk/api/v2/docs/aws-cdk-lib.aws_secretsmanager.ISecret.html#grantwbrreadgrantee-versionstages).
+
 ## How it works
 
 The Datadog CDK construct takes in a list of lambda functions and installs the Datadog Lambda Library by attaching the Lambda Layers for [Java](https://docs.datadoghq.com/serverless/installation/java/?tab=awscdk), [Node.js](https://github.com/DataDog/datadog-lambda-layer-js), and [Python](https://github.com/DataDog/datadog-lambda-layer-python) to your functions. It redirects to a replacement handler that initializes the Lambda Library without any required code changes. Additional configurations added to the Datadog CDK construct will also translate into their respective environment variables under each lambda function (if applicable / required).
 
 While Lambda function based log groups are handled by the `addLambdaFunctions` method automatically, the construct has an additional function `addForwarderToNonLambdaLogGroups` which subscribes the forwarder to any additional log groups of your choosing.
 
 ## Resources to learn about CDK
```

### Comparing `datadog-cdk-constructs-v2-1.7.1/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt` & `datadog-cdk-constructs-v2-1.7.3/src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -7,8 +7,8 @@
 src/datadog_cdk_constructs_v2/py.typed
 src/datadog_cdk_constructs_v2.egg-info/PKG-INFO
 src/datadog_cdk_constructs_v2.egg-info/SOURCES.txt
 src/datadog_cdk_constructs_v2.egg-info/dependency_links.txt
 src/datadog_cdk_constructs_v2.egg-info/requires.txt
 src/datadog_cdk_constructs_v2.egg-info/top_level.txt
 src/datadog_cdk_constructs_v2/_jsii/__init__.py
-src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.7.1.jsii.tgz
+src/datadog_cdk_constructs_v2/_jsii/datadog-cdk-constructs-v2@1.7.3.jsii.tgz
```

