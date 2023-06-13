# Comparing `tmp/datadog-cdk-constructs-0.9.0.tar.gz` & `tmp/datadog-cdk-constructs-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datadog-cdk-constructs-0.9.0.tar", last modified: Wed Apr 19 17:00:52 2023, max compression
+gzip compressed data, was "datadog-cdk-constructs-0.9.1.tar", last modified: Tue Jun 13 14:46:14 2023, max compression
```

## Comparing `datadog-cdk-constructs-0.9.0.tar` & `datadog-cdk-constructs-0.9.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 17:00:52.123770 datadog-cdk-constructs-0.9.0/
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    11358 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/LICENSE
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)       23 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/MANIFEST.in
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    22767 2023-04-19 17:00:52.123619 datadog-cdk-constructs-0.9.0/PKG-INFO
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    21808 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/README.md
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)      106 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/pyproject.toml
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)       38 2023-04-19 17:00:52.123808 datadog-cdk-constructs-0.9.0/setup.cfg
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)     2104 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/setup.py
-drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 17:00:52.120953 datadog-cdk-constructs-0.9.0/src/
-drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 17:00:52.122075 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    61134 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/__init__.py
-drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 17:00:52.123325 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/_jsii/
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)      614 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/_jsii/__init__.py
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)   102261 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/_jsii/datadog-cdk-constructs@0.9.0.jsii.tgz
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)        1 2023-04-19 17:00:48.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/py.typed
-drwxr-xr-x   0 aj.stuyvenberg   (502) staff       (20)        0 2023-04-19 17:00:52.122972 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs.egg-info/
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)    22767 2023-04-19 17:00:52.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs.egg-info/PKG-INFO
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)      493 2023-04-19 17:00:52.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs.egg-info/SOURCES.txt
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)        1 2023-04-19 17:00:52.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs.egg-info/dependency_links.txt
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)      331 2023-04-19 17:00:52.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs.egg-info/requires.txt
--rw-r--r--   0 aj.stuyvenberg   (502) staff       (20)       23 2023-04-19 17:00:52.000000 datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs.egg-info/top_level.txt
+drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 14:46:14.313307 datadog-cdk-constructs-0.9.1/
+-rw-r--r--   0 dylan.yang   (502) staff       (20)    11358 2023-06-13 14:46:11.000000 datadog-cdk-constructs-0.9.1/LICENSE
+-rw-r--r--   0 dylan.yang   (502) staff       (20)       23 2023-06-13 14:46:11.000000 datadog-cdk-constructs-0.9.1/MANIFEST.in
+-rw-r--r--   0 dylan.yang   (502) staff       (20)    24537 2023-06-13 14:46:14.313176 datadog-cdk-constructs-0.9.1/PKG-INFO
+-rw-r--r--   0 dylan.yang   (502) staff       (20)    23578 2023-06-13 14:46:11.000000 datadog-cdk-constructs-0.9.1/README.md
+-rw-r--r--   0 dylan.yang   (502) staff       (20)      106 2023-06-13 14:46:11.000000 datadog-cdk-constructs-0.9.1/pyproject.toml
+-rw-r--r--   0 dylan.yang   (502) staff       (20)       38 2023-06-13 14:46:14.313349 datadog-cdk-constructs-0.9.1/setup.cfg
+-rw-r--r--   0 dylan.yang   (502) staff       (20)     2104 2023-06-13 14:46:11.000000 datadog-cdk-constructs-0.9.1/setup.py
+drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 14:46:14.310349 datadog-cdk-constructs-0.9.1/src/
+drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 14:46:14.311396 datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs/
+-rw-r--r--   0 dylan.yang   (502) staff       (20)    65881 2023-06-13 14:46:11.000000 datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs/__init__.py
+drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 14:46:14.312357 datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs/_jsii/
+-rw-r--r--   0 dylan.yang   (502) staff       (20)      614 2023-06-13 14:46:11.000000 datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs/_jsii/__init__.py
+-rw-r--r--   0 dylan.yang   (502) staff       (20)  1300565 2023-06-13 14:46:11.000000 datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs/_jsii/datadog-cdk-constructs@0.9.1.jsii.tgz
+-rw-r--r--   0 dylan.yang   (502) staff       (20)        1 2023-06-13 14:46:11.000000 datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs/py.typed
+drwxr-xr-x   0 dylan.yang   (502) staff       (20)        0 2023-06-13 14:46:14.312080 datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs.egg-info/
+-rw-r--r--   0 dylan.yang   (502) staff       (20)    24537 2023-06-13 14:46:14.000000 datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs.egg-info/PKG-INFO
+-rw-r--r--   0 dylan.yang   (502) staff       (20)      493 2023-06-13 14:46:14.000000 datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs.egg-info/SOURCES.txt
+-rw-r--r--   0 dylan.yang   (502) staff       (20)        1 2023-06-13 14:46:14.000000 datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs.egg-info/dependency_links.txt
+-rw-r--r--   0 dylan.yang   (502) staff       (20)      331 2023-06-13 14:46:14.000000 datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs.egg-info/requires.txt
+-rw-r--r--   0 dylan.yang   (502) staff       (20)       23 2023-06-13 14:46:14.000000 datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs.egg-info/top_level.txt
```

### Comparing `datadog-cdk-constructs-0.9.0/LICENSE` & `datadog-cdk-constructs-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `datadog-cdk-constructs-0.9.0/PKG-INFO` & `datadog-cdk-constructs-0.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-cdk-constructs
-Version: 0.9.0
+Version: 0.9.1
 Summary: CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog
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
@@ -102,14 +103,15 @@
     extension_layer_version="<EXTENSION_VERSION>",
     forwarder_arn="<FORWARDER_ARN>",
     create_forwarder_permissions=<BOOLEAN>,
     flush_metrics_to_logs=<BOOLEAN>,
     site="<SITE>",
     api_key="{Datadog_API_Key}",
     api_key_secret_arn="{Secret_ARN_Datadog_API_Key}",
+    api_key_secret=<AWS_CDK_ISECRET>,  # Only available in datadog-cdk-constructs-v2
     api_kms_key="{Encrypted_Datadog_API_Key}",
     enable_datadog_tracing=<BOOLEAN>,
     enable_merge_xray_traces=<BOOLEAN>,
     enable_datadog_logs=<BOOLEAN>,
     inject_log_context=<BOOLEAN>,
     log_level=<STRING>,
     env=<STRING>,  # Optional
@@ -204,14 +206,15 @@
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
@@ -222,14 +225,15 @@
 | `enableColdStartTracing`      | `enable_cold_start_tracing` | Set to `false` to disable Cold Start Tracing. Used in NodeJS and Python. Defaults to `true`. |
 | `coldStartTraceMinDuration`   | `min_cold_start_trace_duration` | Sets the minimum duration (in milliseconds) for a module load event to be traced via Cold Start Tracing. Number. Defaults to `3`. |
 | `coldStartTraceSkipLibs`      | `cold_start_trace_skip_libs`| Optionally skip creating Cold Start Spans for a comma-separated list of libraries. Useful to limit depth or skip known libraries. Default depends on runtime. |
 | `enableProfiling`             | `enable_profiling` | Enable the Datadog Continuous Profiler with `true`. Supported in Beta for NodeJS and Python. Defaults to `false`. |
 | `encodeAuthorizerContext`     |`encode_authorizer_context` | When set to `true` for Lambda authorizers, the tracing context will be encoded into the response for propagation. Supported for NodeJS and Python. Defaults to `true`. |
 | `decodeAuthorizerContext`     |`decode_authorizer_context` | When set to `true` for Lambdas that are authorized via Lambda authorizers, it will parse and use the encoded tracing context (if found). Supported for NodeJS and Python. Defaults to `true`.                         |
 | `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set, the tracer attempts to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
+| `redirectHandler` | `redirect_handler` | When set to `false`, skip redirecting handler to the Datadog Lambda Library's handler. Useful when only instrumenting with Datadog Lambda Extension. Defaults to `true`. |
 
 **Note**: Using the parameters above may override corresponding function level `DD_XXX` environment variables.
 
 ### Tracing
 
 Enable X-Ray Tracing on your Lambda functions. For more information, see [CDK documentation](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-lambda.Tracing.html).
 
@@ -301,14 +305,34 @@
         datadog.add_lambda_functions([<LAMBDA_FUNCTIONS>])
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

### Comparing `datadog-cdk-constructs-0.9.0/README.md` & `datadog-cdk-constructs-0.9.1/README.md`

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
@@ -78,14 +79,15 @@
     extension_layer_version="<EXTENSION_VERSION>",
     forwarder_arn="<FORWARDER_ARN>",
     create_forwarder_permissions=<BOOLEAN>,
     flush_metrics_to_logs=<BOOLEAN>,
     site="<SITE>",
     api_key="{Datadog_API_Key}",
     api_key_secret_arn="{Secret_ARN_Datadog_API_Key}",
+    api_key_secret=<AWS_CDK_ISECRET>,  # Only available in datadog-cdk-constructs-v2
     api_kms_key="{Encrypted_Datadog_API_Key}",
     enable_datadog_tracing=<BOOLEAN>,
     enable_merge_xray_traces=<BOOLEAN>,
     enable_datadog_logs=<BOOLEAN>,
     inject_log_context=<BOOLEAN>,
     log_level=<STRING>,
     env=<STRING>,  # Optional
@@ -180,14 +182,15 @@
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
@@ -198,14 +201,15 @@
 | `enableColdStartTracing`      | `enable_cold_start_tracing` | Set to `false` to disable Cold Start Tracing. Used in NodeJS and Python. Defaults to `true`. |
 | `coldStartTraceMinDuration`   | `min_cold_start_trace_duration` | Sets the minimum duration (in milliseconds) for a module load event to be traced via Cold Start Tracing. Number. Defaults to `3`. |
 | `coldStartTraceSkipLibs`      | `cold_start_trace_skip_libs`| Optionally skip creating Cold Start Spans for a comma-separated list of libraries. Useful to limit depth or skip known libraries. Default depends on runtime. |
 | `enableProfiling`             | `enable_profiling` | Enable the Datadog Continuous Profiler with `true`. Supported in Beta for NodeJS and Python. Defaults to `false`. |
 | `encodeAuthorizerContext`     |`encode_authorizer_context` | When set to `true` for Lambda authorizers, the tracing context will be encoded into the response for propagation. Supported for NodeJS and Python. Defaults to `true`. |
 | `decodeAuthorizerContext`     |`decode_authorizer_context` | When set to `true` for Lambdas that are authorized via Lambda authorizers, it will parse and use the encoded tracing context (if found). Supported for NodeJS and Python. Defaults to `true`.                         |
 | `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set, the tracer attempts to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
+| `redirectHandler` | `redirect_handler` | When set to `false`, skip redirecting handler to the Datadog Lambda Library's handler. Useful when only instrumenting with Datadog Lambda Extension. Defaults to `true`. |
 
 **Note**: Using the parameters above may override corresponding function level `DD_XXX` environment variables.
 
 ### Tracing
 
 Enable X-Ray Tracing on your Lambda functions. For more information, see [CDK documentation](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-lambda.Tracing.html).
 
@@ -277,14 +281,34 @@
         datadog.add_lambda_functions([<LAMBDA_FUNCTIONS>])
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

### Comparing `datadog-cdk-constructs-0.9.0/setup.py` & `datadog-cdk-constructs-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "datadog-cdk-constructs",
-    "version": "0.9.0",
+    "version": "0.9.1",
     "description": "CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog",
     "license": "Apache-2.0",
     "url": "https://github.com/DataDog/datadog-cdk-constructs",
     "long_description_content_type": "text/markdown",
     "author": "Datadog",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "datadog_cdk_constructs",
         "datadog_cdk_constructs._jsii"
     ],
     "package_data": {
         "datadog_cdk_constructs._jsii": [
-            "datadog-cdk-constructs@0.9.0.jsii.tgz"
+            "datadog-cdk-constructs@0.9.1.jsii.tgz"
         ],
         "datadog_cdk_constructs": [
             "py.typed"
         ]
     },
     "python_requires": ">=3.6",
     "install_requires": [
```

### Comparing `datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/__init__.py` & `datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs/__init__.py`

 * *Files 5% similar despite different names*

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
@@ -79,14 +80,15 @@
     extension_layer_version="<EXTENSION_VERSION>",
     forwarder_arn="<FORWARDER_ARN>",
     create_forwarder_permissions=<BOOLEAN>,
     flush_metrics_to_logs=<BOOLEAN>,
     site="<SITE>",
     api_key="{Datadog_API_Key}",
     api_key_secret_arn="{Secret_ARN_Datadog_API_Key}",
+    api_key_secret=<AWS_CDK_ISECRET>,  # Only available in datadog-cdk-constructs-v2
     api_kms_key="{Encrypted_Datadog_API_Key}",
     enable_datadog_tracing=<BOOLEAN>,
     enable_merge_xray_traces=<BOOLEAN>,
     enable_datadog_logs=<BOOLEAN>,
     inject_log_context=<BOOLEAN>,
     log_level=<STRING>,
     env=<STRING>,  # Optional
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
@@ -199,14 +202,15 @@
 | `enableColdStartTracing`      | `enable_cold_start_tracing` | Set to `false` to disable Cold Start Tracing. Used in NodeJS and Python. Defaults to `true`. |
 | `coldStartTraceMinDuration`   | `min_cold_start_trace_duration` | Sets the minimum duration (in milliseconds) for a module load event to be traced via Cold Start Tracing. Number. Defaults to `3`. |
 | `coldStartTraceSkipLibs`      | `cold_start_trace_skip_libs`| Optionally skip creating Cold Start Spans for a comma-separated list of libraries. Useful to limit depth or skip known libraries. Default depends on runtime. |
 | `enableProfiling`             | `enable_profiling` | Enable the Datadog Continuous Profiler with `true`. Supported in Beta for NodeJS and Python. Defaults to `false`. |
 | `encodeAuthorizerContext`     |`encode_authorizer_context` | When set to `true` for Lambda authorizers, the tracing context will be encoded into the response for propagation. Supported for NodeJS and Python. Defaults to `true`. |
 | `decodeAuthorizerContext`     |`decode_authorizer_context` | When set to `true` for Lambdas that are authorized via Lambda authorizers, it will parse and use the encoded tracing context (if found). Supported for NodeJS and Python. Defaults to `true`.                         |
 | `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set, the tracer attempts to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
+| `redirectHandler` | `redirect_handler` | When set to `false`, skip redirecting handler to the Datadog Lambda Library's handler. Useful when only instrumenting with Datadog Lambda Extension. Defaults to `true`. |
 
 **Note**: Using the parameters above may override corresponding function level `DD_XXX` environment variables.
 
 ### Tracing
 
 Enable X-Ray Tracing on your Lambda functions. For more information, see [CDK documentation](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-lambda.Tracing.html).
 
@@ -278,14 +282,34 @@
         datadog.add_lambda_functions([<LAMBDA_FUNCTIONS>])
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
@@ -392,24 +416,27 @@
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
+        redirect_handler: typing.Optional[builtins.bool] = None,
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
@@ -426,24 +453,27 @@
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
+        :param redirect_handler: 
         :param service: 
         :param site: 
         :param source_code_integration: 
         :param tags: 
+        :param use_layers_from_account: 
         :param version: 
         '''
         props = DatadogProps(
             add_layers=add_layers,
             api_key=api_key,
             api_key_secret_arn=api_key_secret_arn,
             api_kms_key=api_kms_key,
@@ -458,24 +488,27 @@
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
+            redirect_handler=redirect_handler,
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
@@ -558,24 +591,27 @@
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
+        "redirect_handler": "redirectHandler",
         "service": "service",
         "site": "site",
         "source_code_integration": "sourceCodeIntegration",
         "tags": "tags",
+        "use_layers_from_account": "useLayersFromAccount",
         "version": "version",
     },
 )
 class DatadogProps:
     def __init__(
         self,
         *,
@@ -594,24 +630,27 @@
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
+        redirect_handler: typing.Optional[builtins.bool] = None,
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
         :param api_key_secret_arn: 
         :param api_kms_key: 
@@ -626,24 +665,27 @@
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
+        :param redirect_handler: 
         :param service: 
         :param site: 
         :param source_code_integration: 
         :param tags: 
+        :param use_layers_from_account: 
         :param version: 
         '''
         self._values: typing.Dict[str, typing.Any] = {}
         if add_layers is not None:
             self._values["add_layers"] = add_layers
         if api_key is not None:
             self._values["api_key"] = api_key
@@ -677,34 +719,40 @@
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
             self._values["min_cold_start_trace_duration"] = min_cold_start_trace_duration
         if node_layer_version is not None:
             self._values["node_layer_version"] = node_layer_version
         if python_layer_version is not None:
             self._values["python_layer_version"] = python_layer_version
+        if redirect_handler is not None:
+            self._values["redirect_handler"] = redirect_handler
         if service is not None:
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
@@ -798,14 +846,19 @@
 
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
@@ -828,14 +881,19 @@
 
     @builtins.property
     def python_layer_version(self) -> typing.Optional[jsii.Number]:
         result = self._values.get("python_layer_version")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
+    def redirect_handler(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("redirect_handler")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def service(self) -> typing.Optional[builtins.str]:
         result = self._values.get("service")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def site(self) -> typing.Optional[builtins.str]:
         result = self._values.get("site")
@@ -848,14 +906,19 @@
 
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
 
@@ -873,78 +936,85 @@
     jsii_struct_bases=[],
     name_mapping={
         "add_layers": "addLayers",
         "capture_lambda_payload": "captureLambdaPayload",
         "enable_datadog_logs": "enableDatadogLogs",
         "enable_datadog_tracing": "enableDatadogTracing",
         "enable_merge_xray_traces": "enableMergeXrayTraces",
+        "grant_secret_read_access": "grantSecretReadAccess",
         "inject_log_context": "injectLogContext",
         "api_key": "apiKey",
         "api_key_secret_arn": "apiKeySecretArn",
         "api_kms_key": "apiKmsKey",
         "extension_layer_version": "extensionLayerVersion",
         "flush_metrics_to_logs": "flushMetricsToLogs",
         "forwarder_arn": "forwarderArn",
         "java_layer_version": "javaLayerVersion",
         "log_level": "logLevel",
         "node_layer_version": "nodeLayerVersion",
         "python_layer_version": "pythonLayerVersion",
+        "redirect_handler": "redirectHandler",
         "site": "site",
         "source_code_integration": "sourceCodeIntegration",
     },
 )
 class DatadogStrictProps:
     def __init__(
         self,
         *,
         add_layers: builtins.bool,
         capture_lambda_payload: builtins.bool,
         enable_datadog_logs: builtins.bool,
         enable_datadog_tracing: builtins.bool,
         enable_merge_xray_traces: builtins.bool,
+        grant_secret_read_access: builtins.bool,
         inject_log_context: builtins.bool,
         api_key: typing.Optional[builtins.str] = None,
         api_key_secret_arn: typing.Optional[builtins.str] = None,
         api_kms_key: typing.Optional[builtins.str] = None,
         extension_layer_version: typing.Optional[jsii.Number] = None,
         flush_metrics_to_logs: typing.Optional[builtins.bool] = None,
         forwarder_arn: typing.Optional[builtins.str] = None,
         java_layer_version: typing.Optional[jsii.Number] = None,
         log_level: typing.Optional[builtins.str] = None,
         node_layer_version: typing.Optional[jsii.Number] = None,
         python_layer_version: typing.Optional[jsii.Number] = None,
+        redirect_handler: typing.Optional[builtins.bool] = None,
         site: typing.Optional[builtins.str] = None,
         source_code_integration: typing.Optional[builtins.bool] = None,
     ) -> None:
         '''
         :param add_layers: 
         :param capture_lambda_payload: 
         :param enable_datadog_logs: 
         :param enable_datadog_tracing: 
         :param enable_merge_xray_traces: 
+        :param grant_secret_read_access: 
         :param inject_log_context: 
         :param api_key: 
         :param api_key_secret_arn: 
         :param api_kms_key: 
         :param extension_layer_version: 
         :param flush_metrics_to_logs: 
         :param forwarder_arn: 
         :param java_layer_version: 
         :param log_level: 
         :param node_layer_version: 
         :param python_layer_version: 
+        :param redirect_handler: 
         :param site: 
         :param source_code_integration: 
         '''
         self._values: typing.Dict[str, typing.Any] = {
             "add_layers": add_layers,
             "capture_lambda_payload": capture_lambda_payload,
             "enable_datadog_logs": enable_datadog_logs,
             "enable_datadog_tracing": enable_datadog_tracing,
             "enable_merge_xray_traces": enable_merge_xray_traces,
+            "grant_secret_read_access": grant_secret_read_access,
             "inject_log_context": inject_log_context,
         }
         if api_key is not None:
             self._values["api_key"] = api_key
         if api_key_secret_arn is not None:
             self._values["api_key_secret_arn"] = api_key_secret_arn
         if api_kms_key is not None:
@@ -959,14 +1029,16 @@
             self._values["java_layer_version"] = java_layer_version
         if log_level is not None:
             self._values["log_level"] = log_level
         if node_layer_version is not None:
             self._values["node_layer_version"] = node_layer_version
         if python_layer_version is not None:
             self._values["python_layer_version"] = python_layer_version
+        if redirect_handler is not None:
+            self._values["redirect_handler"] = redirect_handler
         if site is not None:
             self._values["site"] = site
         if source_code_integration is not None:
             self._values["source_code_integration"] = source_code_integration
 
     @builtins.property
     def add_layers(self) -> builtins.bool:
@@ -995,14 +1067,20 @@
     @builtins.property
     def enable_merge_xray_traces(self) -> builtins.bool:
         result = self._values.get("enable_merge_xray_traces")
         assert result is not None, "Required property 'enable_merge_xray_traces' is missing"
         return typing.cast(builtins.bool, result)
 
     @builtins.property
+    def grant_secret_read_access(self) -> builtins.bool:
+        result = self._values.get("grant_secret_read_access")
+        assert result is not None, "Required property 'grant_secret_read_access' is missing"
+        return typing.cast(builtins.bool, result)
+
+    @builtins.property
     def inject_log_context(self) -> builtins.bool:
         result = self._values.get("inject_log_context")
         assert result is not None, "Required property 'inject_log_context' is missing"
         return typing.cast(builtins.bool, result)
 
     @builtins.property
     def api_key(self) -> typing.Optional[builtins.str]:
@@ -1051,14 +1129,19 @@
 
     @builtins.property
     def python_layer_version(self) -> typing.Optional[jsii.Number]:
         result = self._values.get("python_layer_version")
         return typing.cast(typing.Optional[jsii.Number], result)
 
     @builtins.property
+    def redirect_handler(self) -> typing.Optional[builtins.bool]:
+        result = self._values.get("redirect_handler")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def site(self) -> typing.Optional[builtins.str]:
         result = self._values.get("site")
         return typing.cast(typing.Optional[builtins.str], result)
 
     @builtins.property
     def source_code_integration(self) -> typing.Optional[builtins.bool]:
         result = self._values.get("source_code_integration")
```

### Comparing `datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs/_jsii/__init__.py` & `datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs/_jsii/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,17 +15,17 @@
 import aws_cdk.aws_logs._jsii
 import aws_cdk.aws_logs_destinations._jsii
 import aws_cdk.core._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
     "datadog-cdk-constructs",
-    "0.9.0",
+    "0.9.1",
     __name__[0:-6],
-    "datadog-cdk-constructs@0.9.0.jsii.tgz",
+    "datadog-cdk-constructs@0.9.1.jsii.tgz",
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `datadog-cdk-constructs-0.9.0/src/datadog_cdk_constructs.egg-info/PKG-INFO` & `datadog-cdk-constructs-0.9.1/src/datadog_cdk_constructs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datadog-cdk-constructs
-Version: 0.9.0
+Version: 0.9.1
 Summary: CDK Construct Library to automatically instrument Python and Node Lambda functions with Datadog
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
@@ -102,14 +103,15 @@
     extension_layer_version="<EXTENSION_VERSION>",
     forwarder_arn="<FORWARDER_ARN>",
     create_forwarder_permissions=<BOOLEAN>,
     flush_metrics_to_logs=<BOOLEAN>,
     site="<SITE>",
     api_key="{Datadog_API_Key}",
     api_key_secret_arn="{Secret_ARN_Datadog_API_Key}",
+    api_key_secret=<AWS_CDK_ISECRET>,  # Only available in datadog-cdk-constructs-v2
     api_kms_key="{Encrypted_Datadog_API_Key}",
     enable_datadog_tracing=<BOOLEAN>,
     enable_merge_xray_traces=<BOOLEAN>,
     enable_datadog_logs=<BOOLEAN>,
     inject_log_context=<BOOLEAN>,
     log_level=<STRING>,
     env=<STRING>,  # Optional
@@ -204,14 +206,15 @@
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
@@ -222,14 +225,15 @@
 | `enableColdStartTracing`      | `enable_cold_start_tracing` | Set to `false` to disable Cold Start Tracing. Used in NodeJS and Python. Defaults to `true`. |
 | `coldStartTraceMinDuration`   | `min_cold_start_trace_duration` | Sets the minimum duration (in milliseconds) for a module load event to be traced via Cold Start Tracing. Number. Defaults to `3`. |
 | `coldStartTraceSkipLibs`      | `cold_start_trace_skip_libs`| Optionally skip creating Cold Start Spans for a comma-separated list of libraries. Useful to limit depth or skip known libraries. Default depends on runtime. |
 | `enableProfiling`             | `enable_profiling` | Enable the Datadog Continuous Profiler with `true`. Supported in Beta for NodeJS and Python. Defaults to `false`. |
 | `encodeAuthorizerContext`     |`encode_authorizer_context` | When set to `true` for Lambda authorizers, the tracing context will be encoded into the response for propagation. Supported for NodeJS and Python. Defaults to `true`. |
 | `decodeAuthorizerContext`     |`decode_authorizer_context` | When set to `true` for Lambdas that are authorized via Lambda authorizers, it will parse and use the encoded tracing context (if found). Supported for NodeJS and Python. Defaults to `true`.                         |
 | `apmFlushDeadline` | Used to determine when to submit spans before a timeout occurs, in milliseconds. When the remaining time in an AWS Lambda invocation is less than the value set, the tracer attempts to submit the current active spans and all finished spans. Supported for NodeJS and Python. Defaults to `100` milliseconds. |
+| `redirectHandler` | `redirect_handler` | When set to `false`, skip redirecting handler to the Datadog Lambda Library's handler. Useful when only instrumenting with Datadog Lambda Extension. Defaults to `true`. |
 
 **Note**: Using the parameters above may override corresponding function level `DD_XXX` environment variables.
 
 ### Tracing
 
 Enable X-Ray Tracing on your Lambda functions. For more information, see [CDK documentation](https://docs.aws.amazon.com/cdk/api/latest/docs/@aws-cdk_aws-lambda.Tracing.html).
 
@@ -301,14 +305,34 @@
         datadog.add_lambda_functions([<LAMBDA_FUNCTIONS>])
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

