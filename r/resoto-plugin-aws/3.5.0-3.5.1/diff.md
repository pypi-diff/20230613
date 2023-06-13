# Comparing `tmp/resoto-plugin-aws-3.5.0.tar.gz` & `tmp/resoto-plugin-aws-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-aws-3.5.0.tar", last modified: Fri May 26 18:24:37 2023, max compression
+gzip compressed data, was "resoto-plugin-aws-3.5.1.tar", last modified: Fri Jun  2 14:57:09 2023, max compression
```

## Comparing `resoto-plugin-aws-3.5.0.tar` & `resoto-plugin-aws-3.5.1.tar`

### file list

```diff
@@ -1,100 +1,99 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:37.927827 resoto-plugin-aws-3.5.0/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-26 18:24:37.927827 resoto-plugin-aws-3.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:37.919828 resoto-plugin-aws-3.5.0/resoto_plugin_aws/
--rw-r--r--   0 runner    (1001) docker     (123)    27922 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13438 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/aws_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:37.919828 resoto-plugin-aws-3.5.0/resoto_plugin_aws/cmd/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/cmd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11161 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    10936 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:37.923828 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26970 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/apigateway.py
--rw-r--r--   0 runner    (1001) docker     (123)    10602 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/athena.py
--rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/autoscaling.py
--rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    15181 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudformation.py
--rw-r--r--   0 runner    (1001) docker     (123)    53709 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudfront.py
--rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudtrail.py
--rw-r--r--   0 runner    (1001) docker     (123)    18776 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudwatch.py
--rw-r--r--   0 runner    (1001) docker     (123)    10793 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cognito.py
--rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/dynamodb.py
--rw-r--r--   0 runner    (1001) docker     (123)   114499 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/ec2.py
--rw-r--r--   0 runner    (1001) docker     (123)    77860 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/ecs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/efs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16651 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/eks.py
--rw-r--r--   0 runner    (1001) docker     (123)    26166 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elasticache.py
--rw-r--r--   0 runner    (1001) docker     (123)    16353 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elasticbeanstalk.py
--rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elb.py
--rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elbv2.py
--rw-r--r--   0 runner    (1001) docker     (123)    10546 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/glacier.py
--rw-r--r--   0 runner    (1001) docker     (123)    31197 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/iam.py
--rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/kinesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/kms.py
--rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/lambda_.py
--rw-r--r--   0 runner    (1001) docker     (123)     5538 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/pricing.py
--rw-r--r--   0 runner    (1001) docker     (123)    39833 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/rds.py
--rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/redshift.py
--rw-r--r--   0 runner    (1001) docker     (123)     9852 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/route53.py
--rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/s3.py
--rw-r--r--   0 runner    (1001) docker     (123)   234069 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/sagemaker.py
--rw-r--r--   0 runner    (1001) docker     (123)     8571 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/service_quotas.py
--rw-r--r--   0 runner    (1001) docker     (123)    13370 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/sns.py
--rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/sqs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:37.919828 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-26 18:24:37.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-26 18:24:37.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:24:37.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-26 18:24:37.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 18:22:28.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-26 18:24:37.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-26 18:24:37.000000 resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 18:24:37.931827 resoto-plugin-aws-3.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:37.923828 resoto-plugin-aws-3.5.0/test/
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/aws_client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2817 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/collector_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/configuration_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/graphbuilder_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 18:24:37.927827 resoto-plugin-aws-3.5.0/test/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/apigateway_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/athena_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/autoscaling_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/base_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/cloudformation_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/cloudfront_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/cloudtrail_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/cloudwatch_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/cognito_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/config_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/dynamodb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/ec2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/ecs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/efs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/eks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/elasticache_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/elasticbeanstalk_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/elb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/elbv2_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/glacier_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/iam_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/kinesis_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/kms_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/lambda_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/pricing_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/rds_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/redshift_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/route53_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/s3_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/sagemaker_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/service_quotas_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/sns_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/resources/sqs_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-26 18:21:39.000000 resoto-plugin-aws-3.5.0/test/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:09.725244 resoto-plugin-aws-3.5.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-02 14:57:09.725244 resoto-plugin-aws-3.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:09.717244 resoto-plugin-aws-3.5.1/resoto_plugin_aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    31601 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14136 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/aws_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:09.717244 resoto-plugin-aws-3.5.1/resoto_plugin_aws/cmd/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/cmd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11181 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11907 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:09.721244 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27290 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/apigateway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10602 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/athena.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17277 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/autoscaling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23290 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/cloudformation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    53709 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/cloudfront.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12770 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/cloudtrail.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18755 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/cloudwatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10953 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/cognito.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20304 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/dynamodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)   115234 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/ec2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    77940 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/ecs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8580 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/efs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16731 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/eks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26166 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/elasticache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16353 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/elasticbeanstalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10700 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/elb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22707 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/elbv2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10626 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/glacier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31474 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/iam.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6989 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/kinesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7980 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/kms.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16764 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/lambda_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6342 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/pricing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39833 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/rds.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24964 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/redshift.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10012 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/route53.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14549 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/s3.py
+-rw-r--r--   0 runner    (1001) docker     (123)   234139 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/sagemaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8651 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/service_quotas.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13450 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/sns.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7034 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/sqs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:09.717244 resoto-plugin-aws-3.5.1/resoto_plugin_aws.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-06-02 14:57:09.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2991 2023-06-02 14:57:09.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:57:09.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-02 14:57:09.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:53:26.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-02 14:57:09.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-02 14:57:09.000000 resoto-plugin-aws-3.5.1/resoto_plugin_aws.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-02 14:57:09.729244 resoto-plugin-aws-3.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:09.721244 resoto-plugin-aws-3.5.1/test/
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3368 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/aws_client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2992 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/collector_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/configuration_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/graphbuilder_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:57:09.725244 resoto-plugin-aws-3.5.1/test/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     5884 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2200 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/apigateway_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/athena_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/autoscaling_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4037 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/base_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4094 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/cloudformation_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4764 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/cloudfront_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/cloudtrail_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/cloudwatch_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/cognito_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/config_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/dynamodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9650 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/ec2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/ecs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/efs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2050 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/eks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/elasticache_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3002 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/elasticbeanstalk_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/elb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/elbv2_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1748 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/glacier_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7363 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/iam_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1532 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/kinesis_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/kms_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2308 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/lambda_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/pricing_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/rds_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/redshift_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/route53_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2441 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/s3_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5652 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/sagemaker_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/service_quotas_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2935 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/sns_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/resources/sqs_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-06-02 14:52:57.000000 resoto-plugin-aws-3.5.1/test/test_utils.py
```

### Comparing `resoto-plugin-aws-3.5.0/PKG-INFO` & `resoto-plugin-aws-3.5.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.5.0
-Summary: Resoto AWS Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/aws
-License: Apache 2.0
-Keywords: cloud security
+Version: 3.5.1
+Summary: Runs collector plugins and sends the result to resotocore.
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # resoto-plugin-aws
 An AWS collector plugin for Resoto.
 
 ## Usage
 For details on how to edit configuration, please see [the documentation](https://resoto.com/docs/getting-started/configuring-resoto).
```

### Comparing `resoto-plugin-aws-3.5.0/README.md` & `resoto-plugin-aws-3.5.1/README.md`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/__init__.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,54 +1,56 @@
 import logging
 import multiprocessing
 from concurrent import futures
-from typing import List, Optional, Union, Any, Dict, Iterable
+from typing import Any, Dict, Iterable, List, Optional, Tuple, Union
 
 import boto3
 import botocore.exceptions
-from botocore.model import OperationModel, Shape, StringShape, ListShape, StructureShape
+from botocore.model import ListShape, OperationModel, Shape, StringShape, StructureShape
 from jsons import pascalcase
-from prometheus_client import Summary, Counter
+from prometheus_client import Counter, Summary
+from resoto_plugin_aws.aws_client import AwsClient
 
 import resotolib.logger
 import resotolib.proc
-from resoto_plugin_aws.aws_client import AwsClient
-from resotolib.args import ArgumentParser
-from resotolib.args import Namespace
+from resotolib.args import ArgumentParser, Namespace
 from resotolib.baseplugin import BaseCollectorPlugin
 from resotolib.baseresources import (
-    BaseResource,
-    metrics_resource_cleanup_exceptions,
     BaseAccount,
     BaseRegion,
+    BaseResource,
+    Cloud,
+    metrics_resource_cleanup_exceptions,
     metrics_resource_pre_cleanup_exceptions,
 )
-from resotolib.baseresources import Cloud
 from resotolib.config import Config, RunningConfig, current_config
 from resotolib.core.actions import CoreFeedback
 from resotolib.core.custom_command import execute_command_on_resource
-from resotolib.core.progress import ProgressTree, ProgressDone
+from resotolib.core.progress import ProgressDone, ProgressTree
 from resotolib.graph import Graph
 from resotolib.logger import log, setup_logger
 from resotolib.types import JsonElement
-from resotolib.utils import log_runtime, NoExitArgumentParser
+from resotolib.utils import NoExitArgumentParser, log_runtime
+
 from .collector import AwsAccountCollector
 from .configuration import AwsConfig
 from .resource.base import AwsAccount, AwsResource, get_client
-from .utils import aws_session
+from .utils import arn_partition_by_region, aws_session, global_region_by_partition
 
 logging.getLogger("boto").setLevel(logging.CRITICAL)
 
 metrics_collect = Summary("resoto_plugin_aws_collect_seconds", "Time it took the collect() method")
 metrics_unhandled_account_exceptions = Counter(
     "resoto_plugin_aws_unhandled_account_exceptions_total",
     "Unhandled AWS Plugin Account Exceptions",
     ["account"],
 )
 
+GLOBAL_REGIONS = ("us-east-1", "us-gov-west-1", "cn-north-1")
+
 
 class AWSCollectorPlugin(BaseCollectorPlugin):
     cloud = "aws"
 
     def __init__(self) -> None:
         super().__init__()
         self.__regions: List[str] = []
@@ -56,23 +58,26 @@
 
     @staticmethod
     def add_config(cfg: Config) -> None:
         cfg.add_config(AwsConfig)
 
     @staticmethod
     def auto_enableable() -> bool:
-        try:
-            account_id = boto3.session.Session().client("sts").get_caller_identity().get("Account")
-            log.debug(f"plugin: AWS auto discovery succeeded, running in account {account_id}.")
-            return True
-        except Exception as e:
-            log.debug(f"plugin: AWS auto discovery failed: {e}")
+        for region in GLOBAL_REGIONS:
+            try:
+                account_id = (
+                    boto3.session.Session(region_name=region).client("sts").get_caller_identity().get("Account")
+                )
+                log.debug(f"plugin: AWS auto discovery succeeded in {region}, running in account {account_id}.")
+                return True
+            except Exception as e:
+                log.debug(f"plugin: AWS auto discovery failed in {region}: {e}")
         return False
 
-    @metrics_collect.time()  # type: ignore
+    @metrics_collect.time()
     def collect(self) -> None:
         try:
             self.collect_aws()
         except Exception as ex:
             if self.core_feedback:
                 self.core_feedback.error(f"Unhandled exception in AWS Plugin: {ex}", log)
             else:
@@ -90,43 +95,36 @@
             log.error("No accounts found")
             return
 
         progress = ProgressTree(self.cloud)
         for account in accounts:
             # Even if the account is collected later, mark it as expected progress
             progress.add_progress(ProgressDone(account.dname, 0, 1))
-            add_str = ""
+            add_str = f" partition {account.partition}"
             if account.role:
                 add_str += f" role {account.role}"
             if account.profile:
                 add_str += f" profile {account.profile}"
             log.debug(f"Found {account.rtdname}{add_str}")
         self.core_feedback.progress(progress)
 
         max_workers = len(accounts) if len(accounts) < aws_config.account_pool_size else aws_config.account_pool_size
         pool_args = {"max_workers": max_workers}
-        # TODO: revert this when memory leak in AWS collector is fixed
-        # if Config.aws.fork_process:
-        #     pool_args["mp_context"] = multiprocessing.get_context("spawn")
-        #     pool_args["initializer"] = resotolib.proc.initializer
-        #     pool_executor = futures.ProcessPoolExecutor
-        # else:
-        #     pool_executor = futures.ThreadPoolExecutor  # type: ignore
         pool_executor = futures.ThreadPoolExecutor
         if aws_config.fork_process:
             collect_method = collect_in_process
         else:
             collect_method = collect_account
 
         with pool_executor(**pool_args) as executor:  # type: ignore
             wait_for = [
                 executor.submit(
                     collect_method,
                     account,
-                    self.regions(profile=account.profile),
+                    self.regions(profile=account.profile, partition=account.partition),
                     ArgumentParser.args,
                     Config.running_config,
                     self.core_feedback.with_context(cloud.id, account.dname),
                     cloud,
                 )
                 for account in accounts
             ]
@@ -136,19 +134,24 @@
                     log.debug(f"Skipping account graph of invalid type {type(account_graph)}")
                     continue
                 self.graph.merge(account_graph, skip_deferred_edges=True)
 
         # collect done, purge all session caches
         aws_config.sessions().purge_caches()
 
-    def regions(self, profile: Optional[str] = None) -> List[str]:
+    def regions(self, profile: Optional[str] = None, partition: str = "aws") -> List[str]:
         if len(self.__regions) == 0:
             if not Config.aws.region or (isinstance(Config.aws.region, list) and len(Config.aws.region) == 0):
-                log.debug("AWS region not specified, assuming all regions")
-                self.__regions = all_regions(profile=profile)
+                add_log_str = ""
+                if profile:
+                    add_log_str += f" profile {profile}"
+                if partition:
+                    add_log_str += f" partition {partition}"
+                log.debug(f"AWS region not specified, assuming all regions{add_log_str}")
+                self.__regions = all_regions(profile=profile, partition=partition)
             else:
                 self.__regions = list(Config.aws.region)
         return self.__regions
 
     @execute_command_on_resource(
         name="aws",
         info="Execute aws commands on AWS resources",
@@ -410,44 +413,115 @@
             return True
 
         raise RuntimeError(f"Unsupported resource type: {resource.rtdname}")
 
 
 def authenticated(account: AwsAccount, core_feedback: CoreFeedback) -> bool:
     try:
-        log.debug(f"AWS testing credentials for {account.rtdname}")
-        session = aws_session(account.id, account.role, account.profile)
-        _ = session.client("sts").get_caller_identity().get("Account")
+        add_log_str = ""
+        if account.role:
+            add_log_str += f" role {account.role}"
+        if account.profile:
+            add_log_str += f" profile {account.profile}"
+        if account.partition:
+            add_log_str += f" partition {account.partition}"
+        log.debug(f"AWS testing credentials for {account.rtdname}{add_log_str}")
+        session = aws_session(
+            account=account.id, role=account.role, profile=account.profile, partition=account.partition
+        )
+        _ = (
+            session.client("sts", region_name=global_region_by_partition(account.partition))
+            .get_caller_identity()
+            .get("Account")
+        )
     except botocore.exceptions.NoCredentialsError:
         core_feedback.error(f"No AWS credentials found for {account.rtdname}", log)
     except botocore.exceptions.ClientError as e:
         if e.response["Error"]["Code"] == "AuthFailure":
             core_feedback.error(f"Unable to validate the provided access credentials for {account.rtdname}", log)
         elif e.response["Error"]["Code"] == "InvalidClientTokenId":
             core_feedback.error(f"Unable to validate the provided security token for {account.rtdname}", log)
         elif e.response["Error"]["Code"] == "ExpiredToken":
             core_feedback.error(f"Security token included in the request is expired for {account.rtdname}", log)
         elif e.response["Error"]["Code"] == "AccessDenied":
             core_feedback.error(f"Access Denied to {account.rtdname}: {e}", log)
+        elif e.response["Error"]["Code"] == "SignatureDoesNotMatch":
+            core_feedback.error(f"Token signature does not match {account.rtdname}: {e}", log)
         else:
             raise
         return False
     return True
 
 
 def current_account_id(profile: Optional[str] = None) -> str:
-    session = aws_session(profile=profile)
-    return session.client("sts").get_caller_identity().get("Account")  # type: ignore
+    account_id, _ = current_account_id_and_partition(profile)
+    return account_id
+
+
+def probe_partition(account: Optional[str] = None, role: Optional[str] = None, profile: Optional[str] = None) -> str:
+    for region in GLOBAL_REGIONS:
+        partition = arn_partition_by_region(region)
+        try:
+            session = aws_session(account=account, role=role, profile=profile, partition=partition)
+            _ = session.client("sts", region_name=region).get_caller_identity().get("Account")
+        except Exception:
+            pass
+        else:
+            return partition
+    return "aws"
+
+
+def current_account_id_and_partition(profile: Optional[str] = None) -> Tuple[str, str]:
+    interesting_exception = None
+    add_log_str = ""
+    if profile:
+        add_log_str = f" with profile {profile}"
+    log.debug(f"Trying to determine current account id and partition{add_log_str}")
+    for region in GLOBAL_REGIONS:
+        partition = arn_partition_by_region(region)
+        log.debug(f"Probing region {region}")
+        try:
+            if profile:
+                account_id = (
+                    boto3.session.Session(region_name=region, profile_name=profile)
+                    .client("sts")
+                    .get_caller_identity()
+                    .get("Account")
+                )
+            else:
+                account_id = (
+                    boto3.session.Session(
+                        region_name=region,
+                        aws_access_key_id=Config.aws.access_key_id,
+                        aws_secret_access_key=Config.aws.secret_access_key,
+                    )
+                    .client("sts")
+                    .get_caller_identity()
+                    .get("Account")
+                )
+            log.debug(f"Determined partition for account {account_id} to be {partition}")
+            return account_id, partition
+        except botocore.exceptions.ClientError as e:
+            log.debug(f"Got an exception when probing partition {partition}: {e}")
+            if e.response["Error"]["Code"] != "InvalidClientTokenId":
+                interesting_exception = e
+        except Exception as e:
+            log.debug(f"Got an exception when probing partition {partition}: {e}")
+            interesting_exception = e
+    if interesting_exception:
+        raise interesting_exception
+    else:
+        raise botocore.exceptions.NoCredentialsError()
 
 
 def set_account_names(accounts: List[AwsAccount]) -> None:
     def set_account_name(account: AwsAccount) -> None:
         try:
             account_aliases = (
-                aws_session(account.id, account.role, account.profile)
+                aws_session(account=account.id, role=account.role, profile=account.profile, partition=account.partition)
                 .client("iam")
                 .list_account_aliases()
                 .get("AccountAliases", [])
             )
             if len(account_aliases) > 0:
                 account.name = account_aliases[0]
         except Exception:
@@ -488,60 +562,66 @@
     for profile in profiles:
         if profile is not None:
             log.debug(f"Finding accounts for profile {profile}")
 
         try:
             if Config.aws.role and Config.aws.scrape_org:
                 log.debug("Role and scrape_org are both set")
+                account_id, partition = current_account_id_and_partition(profile=profile)
                 accounts.extend(
                     [
-                        AwsAccount(id=aws_account_id, role=Config.aws.role, profile=profile)
+                        AwsAccount(id=aws_account_id, role=Config.aws.role, profile=profile, partition=partition)
                         for aws_account_id in get_org_accounts(
                             filter_current_account=not Config.aws.assume_current,
                             profile=profile,
                             core_feedback=core_feedback,
+                            partition=partition,
                         )
                         if aws_account_id not in Config.aws.scrape_exclude_account
                     ]
                 )
                 if not Config.aws.do_not_scrape_current:
-                    accounts.append(AwsAccount(id=current_account_id(profile=profile)))
+                    accounts.append(AwsAccount(id=account_id, partition=partition))
             elif Config.aws.role and Config.aws.account:
                 log.debug("Both, role and list of accounts specified")
-                accounts.extend(
-                    [
-                        AwsAccount(id=aws_account_id, role=Config.aws.role, profile=profile)
-                        for aws_account_id in Config.aws.account
-                    ]
-                )
+                for aws_account_id in Config.aws.account:
+                    partition = probe_partition(aws_account_id, profile=profile)
+                    accounts.append(
+                        AwsAccount(id=aws_account_id, role=Config.aws.role, profile=profile, partition=partition)
+                    )
             else:
-                accounts.extend([AwsAccount(id=current_account_id(profile=profile), profile=profile)])
+                account_id, partition = current_account_id_and_partition(profile=profile)
+                accounts.extend([AwsAccount(id=account_id, profile=profile, partition=partition)])
         except botocore.exceptions.NoCredentialsError:
             core_feedback.error(f"No AWS credentials found for {profile}", log)
         except botocore.exceptions.ClientError as e:
             if e.response["Error"]["Code"] == "AuthFailure":
                 core_feedback.error(f"Unable to validate the provided access credentials for {profile}", log)
             elif e.response["Error"]["Code"] == "InvalidClientTokenId":
                 core_feedback.error(f"Unable to validate the provided security token for {profile}", log)
             elif e.response["Error"]["Code"] == "ExpiredToken":
                 core_feedback.error(f"AWS security token included in the request is expired for {profile}", log)
             elif e.response["Error"]["Code"] == "AccessDenied":
                 core_feedback.error(f"Access denied for profile {profile}", log)
+            elif e.response["Error"]["Code"] == "SignatureDoesNotMatch":
+                core_feedback.error(f"Token signature does not match for {profile}", log)
             else:
                 core_feedback.error(f"AWS client error for profile {profile}: {e}", log)
                 raise
         except botocore.exceptions.BotoCoreError as e:
             core_feedback.error(f"Unable to get accounts for profile {profile}: {e}", log)
 
     set_account_names(accounts)
     return accounts
 
 
-def get_org_accounts(filter_current_account: bool, profile: Optional[str], core_feedback: CoreFeedback) -> List[str]:
-    session = aws_session(profile=profile)
+def get_org_accounts(
+    filter_current_account: bool, profile: Optional[str], core_feedback: CoreFeedback, partition: Optional[str] = None
+) -> List[str]:
+    session = aws_session(profile=profile, partition=partition)
     client = session.client("organizations")
     accounts = []
     try:
         response = client.list_accounts()
         accounts = response.get("Accounts", [])
         while response.get("NextToken") is not None:
             response = client.list_accounts(NextToken=response["NextToken"])
@@ -555,17 +635,17 @@
     accounts = [aws_account["Id"] for aws_account in accounts if aws_account["Id"] != filter_account_id]
     for account in accounts:
         log.debug(f"AWS found org account {account}")
     log.info(f"AWS found a total of {len(accounts)} org accounts")
     return accounts
 
 
-def all_regions(profile: Optional[str] = None) -> List[str]:
-    session = aws_session(profile=profile)
-    ec2 = session.client("ec2", region_name="us-east-1")
+def all_regions(profile: Optional[str] = None, partition: str = "aws") -> List[str]:
+    session = aws_session(profile=profile, partition=partition)
+    ec2 = session.client("ec2", region_name=global_region_by_partition(partition))
     regions = ec2.describe_regions()
     return [r["RegionName"] for r in regions["Regions"]]
 
 
 @log_runtime
 def collect_account(
     account: AwsAccount,
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/aws_client.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/aws_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 from __future__ import annotations
 
 import logging
 from datetime import datetime
 from functools import cached_property
 from itertools import islice
-from typing import Optional, Any, List, TypeVar, Callable, Dict, Set
+from typing import Any, Callable, Dict, List, Optional, Set, TypeVar
 
 from attr import define, field
 from botocore.config import Config
 from botocore.exceptions import ClientError, EndpointConnectionError
 from botocore.model import ServiceModel
+from resoto_plugin_aws.configuration import AwsConfig
 from retrying import retry
 
-from resoto_plugin_aws.configuration import AwsConfig
 from resotolib.core.actions import CoreFeedback
 from resotolib.json import value_in_path
 from resotolib.types import Json, JsonElement
-from resotolib.utils import utc_str, log_runtime
+from resotolib.utils import log_runtime, utc_str
+
+from .utils import global_region_by_partition
 
 log = logging.getLogger("resoto.plugins.aws")
 
 RetryableErrors = {
     "EC2ThrottledException",
     "LimitExceededException",
     "RequestLimitExceeded",
@@ -109,21 +111,25 @@
         self,
         config: AwsConfig,
         account_id: str,
         *,
         role: Optional[str] = None,
         profile: Optional[str] = None,
         region: Optional[str] = None,
+        partition: Optional[str] = None,
         error_accumulator: Optional[ErrorAccumulator] = None,
     ) -> None:
         self.config = config
         self.account_id = account_id
         self.role = role
         self.profile = profile
         self.region = region
+        if partition is None:
+            partition = "aws"
+        self.partition = partition
         self.error_accumulator = error_accumulator
 
     def __to_json(self, node: Any, **kwargs: Any) -> JsonElement:
         if node is None or isinstance(node, (str, int, float, bool)):
             return node
         elif isinstance(node, list):
             return [self.__to_json(item, **kwargs) for item in node]
@@ -133,29 +139,43 @@
             return utc_str(node)
         elif isinstance(node, bytes):
             return node.decode("utf-8")
         else:
             raise AttributeError(f"Unsupported type: {type(node)}")
 
     def service_model(self, aws_service: str) -> ServiceModel:
-        client = self.config.sessions().client(self.account_id, self.role, self.profile, aws_service, self.region)
+        client = self.config.sessions().client(
+            aws_account=self.account_id,
+            aws_role=self.role,
+            aws_profile=self.profile,
+            aws_service=aws_service,
+            region_name=self.region,
+            aws_partition=self.partition,
+        )
         model = client.meta.service_model
         client.close()
         return model
 
     def with_resource(self, aws_service: str, fn: Callable[[Any], T]) -> Optional[T]:
         """
         Create a boto service resource model and call the given function with it.
         The service model is created dynamically in boto3, so we can not give it a proper type, hence Any.
         Advantage: the scope of the resource is defined by this function, exceptions are handled in the client.
         :param aws_service: the service to use.
         :param fn: loan pattern: the function is handed the resource and the result is returned.
         :return: the result of the function.
         """
-        resource = self.config.sessions().resource(self.account_id, self.role, self.profile, aws_service, self.region)
+        resource = self.config.sessions().resource(
+            aws_account=self.account_id,
+            aws_role=self.role,
+            aws_profile=self.profile,
+            aws_service=aws_service,
+            region_name=self.region,
+            aws_partition=self.partition,
+        )
         try:
             return fn(resource)
         except ClientError as e:
             self.__handle_client_error(e, aws_service, "service_resource")  # might reraise the exception
             return None
         except EndpointConnectionError as e:
             log.debug(f"The Aws endpoint does not exist in this region. Skipping. {e}")
@@ -171,16 +191,23 @@
         if kwargs:
             arg_info += " with args " + ", ".join([f"{key}={value}" for key, value in kwargs.items()])
         log.debug(f"[Aws] calling service={aws_service} action={action}{arg_info}")
         py_action = action.replace("-", "_")
         # adaptive mode allows automated client-side throttling
         config = Config(retries={"max_attempts": max_attempts, "mode": "adaptive"})
         client = self.config.sessions().client(
-            self.account_id, self.role, self.profile, aws_service, self.region, config
+            aws_account=self.account_id,
+            aws_role=self.role,
+            aws_profile=self.profile,
+            aws_service=aws_service,
+            region_name=self.region,
+            config=config,
+            aws_partition=self.partition,
         )
+
         try:
             if client.can_paginate(py_action):
                 paginator = client.get_paginator(py_action)
                 result: List[Json] = []
                 for page in paginator.paginate(**kwargs):
                     log.debug2(f"[Aws] Next page for service={aws_service} action={action}{arg_info}")  # type: ignore
                     next_page: Json = self.__to_json(page)  # type: ignore
@@ -279,14 +306,15 @@
     def for_region(self, region: str) -> AwsClient:
         return AwsClient(
             self.config,
             self.account_id,
             role=self.role,
             profile=self.profile,
             region=region,
+            partition=self.partition,
             error_accumulator=self.error_accumulator,
         )
 
     def __handle_client_error(
         self, e: ClientError, aws_service: str, action: str, expected_errors: Optional[List[str]] = None
     ) -> None:
         def accumulate(error_kind: str, message: str, as_info: bool = False) -> None:
@@ -319,11 +347,10 @@
                 f"account {self.account_id} region {self.region} - skipping resources: {e}"
             )
             accumulate(code, f"An AWS API error occurred during resource collection: {code}. Skipping resources.")
 
     @cached_property
     def global_region(self) -> AwsClient:
         """
-        AWS serves some APIs only from one region: us-east-1.
-        We call it the global region in this collector.
+        AWS serves some APIs only from a global region.
         """
-        return self.for_region("us-east-1")
+        return self.for_region(global_region_by_partition(self.partition))
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/collector.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,61 +1,64 @@
 import logging
-from concurrent.futures import ThreadPoolExecutor, Future
+from concurrent.futures import Future, ThreadPoolExecutor
 from typing import List, Type
 
 from resoto_plugin_aws.aws_client import AwsClient, ErrorAccumulator
 from resoto_plugin_aws.configuration import AwsConfig
 from resoto_plugin_aws.resource import (
     apigateway,
     athena,
     autoscaling,
-    config,
     cloudformation,
     cloudfront,
     cloudtrail,
     cloudwatch,
     cognito,
+    config,
     dynamodb,
     ec2,
     ecs,
     efs,
     eks,
-    elasticbeanstalk,
     elasticache,
+    elasticbeanstalk,
     elb,
     elbv2,
     glacier,
     iam,
     kinesis,
     kms,
     lambda_,
     rds,
+    redshift,
     route53,
     s3,
     sagemaker,
     service_quotas,
     sns,
     sqs,
-    redshift,
 )
 from resoto_plugin_aws.resource.base import (
-    AwsRegion,
     AwsAccount,
+    AwsApiSpec,
+    AwsRegion,
     AwsResource,
-    GraphBuilder,
     ExecutorQueue,
-    AwsApiSpec,
     GatherFutures,
+    GraphBuilder,
 )
+
 from resotolib.baseresources import Cloud, EdgeType
 from resotolib.core.actions import CoreFeedback
-from resotolib.core.progress import ProgressTree, ProgressDone
+from resotolib.core.progress import ProgressDone, ProgressTree
 from resotolib.graph import Graph
 from resotolib.proc import set_thread_name
 
+from .utils import global_region_by_partition
+
 log = logging.getLogger("resoto.plugins.aws")
 
 global_resources: List[Type[AwsResource]] = (
     cloudfront.resources
     + dynamodb.global_resources
     + iam.resources
     + route53.resources
@@ -126,24 +129,27 @@
     def __init__(
         self, config: AwsConfig, cloud: Cloud, account: AwsAccount, regions: List[str], core_feedback: CoreFeedback
     ) -> None:
         self.config = config
         self.cloud = cloud
         self.account = account
         self.core_feedback = core_feedback
-        self.global_region = AwsRegion(id="us-east-1", tags={}, name="global", account=account)
+        self.global_region = AwsRegion(
+            id=global_region_by_partition(account.partition), tags={}, name="global", account=account
+        )
         self.regions = [AwsRegion(id=region, tags={}, account=account) for region in regions]
         self.graph = Graph(root=self.account)
         self.error_accumulator = ErrorAccumulator()
         self.client = AwsClient(
             config,
             account.id,
             role=account.role,
             profile=account.profile,
             region=self.global_region.id,
+            partition=account.partition,
             error_accumulator=self.error_accumulator,
         )
 
     def collect(self) -> None:
         with ThreadPoolExecutor(
             thread_name_prefix=f"aws_{self.account.id}", max_workers=self.config.resource_pool_size
         ) as executor:
@@ -161,21 +167,21 @@
             progress.add_progress(ProgressDone(self.global_region.safe_name, 0, 1))
             for region in self.regions:
                 progress.add_progress(ProgressDone(region.safe_name, 0, 1))
             global_builder.core_feedback.progress(progress)
 
             # all global resources
             log.info(f"[Aws:{self.account.id}] Collect global resources.")
-            self.collect_resources(global_resources, global_builder, shared_queue)
+            self.collect_resources(global_resources, global_builder)
 
             # regions are collected with the configured parallelism
             # note: when the thread pool context is left, all submitted work is done (or an exception has been thrown)
             log.info(f"[Aws:{self.account.id}] Collect regional resources.")
             for region in self.regions:
-                self.collect_resources(regional_resources, global_builder.for_region(region), shared_queue)
+                self.collect_resources(regional_resources, global_builder.for_region(region))
             shared_queue.wait_for_submitted_work()
 
             # connect nodes
             log.info(f"[Aws:{self.account.id}] Connect resources and create edges.")
             for node, data in list(self.graph.nodes(data=True)):
                 if isinstance(node, AwsResource):
                     if isinstance(node, AwsAccount):
@@ -193,20 +199,15 @@
             # wait for all futures to finish
             shared_queue.wait_for_submitted_work()
             self.core_feedback.progress_done(self.account.dname, 1, 1, context=[self.cloud.id])
             self.error_accumulator.report_all(global_builder.core_feedback)
 
             log.info(f"[Aws:{self.account.id}] Collecting resources done.")
 
-    def collect_resources(
-        self,
-        resources: List[Type[AwsResource]],
-        builder: GraphBuilder,
-        resource_queue: ExecutorQueue,
-    ) -> Future[None]:
+    def collect_resources(self, resources: List[Type[AwsResource]], builder: GraphBuilder) -> Future[None]:
         region = builder.region
 
         def collect_resource(resource: Type[AwsResource], rb: GraphBuilder) -> None:
             try:
                 set_thread_name(f"aws_{self.account.id}_{region.id}_{resource.kind}")
                 resource.collect_resources(rb)
                 log.info(f"[Aws:{self.account.id}:{region.safe_name}] finished collecting: {resource.kind}")
@@ -218,16 +219,16 @@
                 builder.core_feedback.error(msg, log)
                 raise
 
         region_futures = []
         builder.add_node(region)
         for res in resources:
             if self.config.should_collect(res.kind):
-                key = region.id + ":" + res.api_spec.service if res.api_spec else "global"
-                region_futures.append(resource_queue.submit_work(key, collect_resource, res, builder))
+                service_name = res.service_name() or "global"
+                region_futures.append(builder.submit_work(service_name, collect_resource, res, builder))
 
         def work_done(_: Future[None]) -> None:
             builder.core_feedback.progress_done(region.safe_name, 1, 1)
             self.error_accumulator.report_region(builder.core_feedback, region.id)
 
         # once all futures are done
         when_done = GatherFutures.all(region_futures)
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/configuration.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/configuration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 import logging
 import threading
 import time
 import uuid
 from datetime import timedelta
+from fnmatch import fnmatch
 from functools import lru_cache
-from typing import List, ClassVar, Optional, Type, Any, Dict, Callable
+from typing import Any, Callable, ClassVar, Dict, List, Optional, Type
 
 from attrs import define, field, fields_dict
 from boto3.session import Session as BotoSession
 from botocore.client import BaseClient
 from botocore.config import Config as BotoConfig
 
 from resotolib.durations import parse_duration
 from resotolib.json import from_json as from_js
 from resotolib.proc import num_default_threads
 from resotolib.types import Json
 
+from .utils import global_region_by_partition
+
 log = logging.getLogger("resoto.plugins.aws")
 
 
 @define(hash=True, slots=False)
 class AwsSessionHolder:
     access_key_id: Optional[str]
     secret_access_key: Optional[str]
@@ -28,86 +31,99 @@
     # Only here to override in tests
     session_class_factory: Type[BotoSession] = BotoSession
     kind: ClassVar[str] = "aws_session_holder"
     session_lock: threading.Lock = threading.Lock()
 
     # noinspection PyUnusedLocal
     @lru_cache(maxsize=128)
-    def __direct_session(self, profile: Optional[str]) -> BotoSession:
+    def __direct_session(self, profile: Optional[str], partition: str) -> BotoSession:
+        global_region = global_region_by_partition(partition)
         if profile:
-            return self.session_class_factory(profile_name=profile)
+            return self.session_class_factory(profile_name=profile, region_name=global_region)
         else:
             return self.session_class_factory(
-                aws_access_key_id=self.access_key_id, aws_secret_access_key=self.secret_access_key
+                aws_access_key_id=self.access_key_id,
+                aws_secret_access_key=self.secret_access_key,
+                region_name=global_region,
             )
 
     # noinspection PyUnusedLocal
     @lru_cache(maxsize=128)
-    def __sts_session(self, aws_account: str, aws_role: str, profile: Optional[str], cache_key: int) -> BotoSession:
+    def __sts_session(
+        self, aws_account: str, aws_role: str, profile: Optional[str], partition: str, cache_key: int
+    ) -> BotoSession:
+        global_region = global_region_by_partition(partition)
         role = self.role if self.role_override else aws_role
-        role_arn = f"arn:aws:iam::{aws_account}:role/{role}"
+        role_arn = f"arn:{partition}:iam::{aws_account}:role/{role}"
         if profile:
             session = self.session_class_factory(
                 profile_name=profile,
-                region_name="us-east-1",
+                region_name=global_region,
             )
         else:
             session = self.session_class_factory(
                 aws_access_key_id=self.access_key_id,
                 aws_secret_access_key=self.secret_access_key,
-                region_name="us-east-1",
+                region_name=global_region,
             )
         sts = session.client("sts")
         token = sts.assume_role(RoleArn=role_arn, RoleSessionName=f"{aws_account}-{str(uuid.uuid4())}")
         credentials = token["Credentials"]
         return self.session_class_factory(
             aws_access_key_id=credentials["AccessKeyId"],
             aws_secret_access_key=credentials["SecretAccessKey"],
             aws_session_token=credentials["SessionToken"],
+            region_name=global_region,
         )
 
     def _session(
-        self, aws_account: str, aws_role: Optional[str] = None, aws_profile: Optional[str] = None
+        self,
+        aws_account: str,
+        aws_role: Optional[str] = None,
+        aws_profile: Optional[str] = None,
+        aws_partition: str = "aws",
     ) -> BotoSession:
         """
         Note: the session is not thread safe - caller needs to synchronize access.
         Consider using the client() and resource() methods instead.
         """
         if aws_role is None:
-            return self.__direct_session(aws_profile)
+            return self.__direct_session(aws_profile, aws_partition)
         else:
             # Use sts to create a temporary token for the given account and role
             # Sts session is at least valid for 900 seconds (default 1 hour)
             # let's renew the session after 10 minutes
-            return self.__sts_session(aws_account, aws_role, aws_profile, int(time.time() / 600))
+            return self.__sts_session(aws_account, aws_role, aws_profile, aws_partition, int(time.time() / 600))
 
     def client(
         self,
         aws_account: str,
         aws_role: Optional[str],
         aws_profile: Optional[str],
         aws_service: str,
         region_name: Optional[str] = None,
         config: Optional[BotoConfig] = None,
+        aws_partition: str = "aws",
     ) -> BaseClient:
         with self.session_lock:
-            session = self._session(aws_account, aws_role, aws_profile)
+            session = self._session(aws_account, aws_role, aws_profile, aws_partition)
             return session.client(aws_service, region_name=region_name, config=config)
 
     def resource(
         self,
         aws_account: str,
         aws_role: Optional[str],
         aws_profile: Optional[str],
         aws_service: str,
         region_name: Optional[str] = None,
         config: Optional[BotoConfig] = None,
+        aws_partition: str = "aws",
     ) -> Any:
         with self.session_lock:
-            session = self._session(aws_account, aws_role, aws_profile)
+            session = self._session(aws_account, aws_role, aws_profile, aws_partition)
             return session.resource(aws_service, region_name=region_name, config=config)
 
     def purge_caches(self) -> None:
         self.__direct_session.cache_clear()
         self.__sts_session.cache_clear()
 
 
@@ -169,29 +185,39 @@
         default=20,
         metadata={
             "description": "Number of collector threads to run in parallel per service and region.\n"
             "Note that the total number of collector threads is limited by resource_pool_size.\n"
             "A value greater than the resource_pool_size does not have any effect."
         },
     )
-    resource_pool_tasks_per_service: Dict[str, int] = field(
+    resource_pool_tasks_per_service: Optional[Dict[str, int]] = field(
         factory=lambda: {"sagemaker": 6, "elb": 6},
         metadata={
             "description": "Define the number of collector threads allowed for an individual service.\n"
             "If the service is not defined here, the default value is used.\n"
             'Example: {"ec2": 10, "rds": 5}'
         },
     )
     collect: List[str] = field(
         factory=list,
-        metadata={"description": "List of AWS services to collect (default: all)"},
+        metadata={
+            "description": (
+                "List of AWS services to collect (default: all).\n"
+                "You can use GLOB patterns like ? and * to match multiple services."
+            )
+        },
     )
     no_collect: List[str] = field(
         factory=list,
-        metadata={"description": "List of AWS services to exclude (default: none)"},
+        metadata={
+            "description": (
+                "List of AWS services to exclude (default: none).\n"
+                "You can use GLOB patterns like ? and * to match multiple services."
+            )
+        },
     )
     cloudwatch_metrics_for_atime_mtime_period: str = field(
         default="60d",
         metadata={
             "type_hint": "duration",
             "description": "This value is used to look up atime and mtime for volumes and rds instances.\n"
             "It defines how long Resoto should look back for CloudWatch metrics.\n"
@@ -219,18 +245,19 @@
     def atime_mtime_period(self) -> timedelta:
         return parse_duration(self.cloudwatch_metrics_for_atime_mtime_period)
 
     def atime_mtime_granularity(self) -> timedelta:
         return parse_duration(self.cloudwatch_metrics_for_atime_mtime_granularity)
 
     def should_collect(self, name: str) -> bool:
+        # no_collect has precedence over collect
+        if self.no_collect and any(fnmatch(name, p) for p in self.no_collect):
+            return False
         if self.collect:
-            return name in self.collect
-        if self.no_collect:
-            return name not in self.no_collect
+            return any(fnmatch(name, p) for p in self.collect)
         return True
 
     def shared_tasks_per_key(self, regions: List[str]) -> Callable[[str], int]:
         # some services have known lower limits, the predefined limits can be overridden
         defined = self.resource_pool_tasks_per_service or {}
         tpk = {region + ":" + service: num for region in regions for service, num in defined.items()}
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/apigateway.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/apigateway.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,14 +52,18 @@
         return [
             AwsApiSpec(service_name, "tag-resource", override_iam_permission="apigateway:PATCH"),
             AwsApiSpec(service_name, "tag-resource", override_iam_permission="apigateway:POST"),
             AwsApiSpec(service_name, "tag-resource", override_iam_permission="apigateway:PUT"),
             AwsApiSpec(service_name, "untag-resource", override_iam_permission="apigateway:DELETE"),
         ]
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 @define(eq=False, slots=False)
 class AwsApiGatewayMethodResponse:
     kind: ClassVar[str] = "aws_api_gateway_method_response"
     mapping: ClassVar[Dict[str, Bender]] = {
         "status_code": S("statusCode"),
         "response_parameters": S("responseParameters"),
@@ -191,14 +195,18 @@
         )
         return True
 
     @classmethod
     def called_mutator_apis(cls) -> List[AwsApiSpec]:
         return [AwsApiSpec(service_name, "delete-resource", override_iam_permission="apigateway:DELETE")]
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 @define(eq=False, slots=False)
 class AwsApiGatewayAuthorizer(AwsResource):
     # collection of authorizer resources happens in AwsApiGatewayRestApi.collect()
     kind: ClassVar[str] = "aws_api_gateway_authorizer"
     reference_kinds: ClassVar[ModelReference] = {
         "successors": {"default": ["aws_lambda_function"]},
@@ -251,14 +259,18 @@
         )
         return True
 
     @classmethod
     def called_mutator_apis(cls) -> List[AwsApiSpec]:
         return [AwsApiSpec(service_name, "delete-authorizer", override_iam_permission="apigateway:DELETE")]
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 @define(eq=False, slots=False)
 class AwsApiGatewayCanarySetting:
     kind: ClassVar[str] = "aws_api_gateway_canary_setting"
     mapping: ClassVar[Dict[str, Bender]] = {
         "percent_traffic": S("percentTraffic"),
         "deployment_id": S("deploymentId"),
@@ -356,14 +368,18 @@
 
     @classmethod
     def called_mutator_apis(cls) -> List[AwsApiSpec]:
         return super().called_mutator_apis() + [
             AwsApiSpec(service_name, "delete-deployment", override_iam_permission="apigateway:DELETE")
         ]
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 @define(eq=False, slots=False)
 class AwsApiGatewayEndpointConfiguration:
     kind: ClassVar[str] = "aws_api_gateway_endpoint_configuration"
     mapping: ClassVar[Dict[str, Bender]] = {
         "types": S("types", default=[]),
         "vpc_endpoint_ids": S("vpcEndpointIds", default=[]),
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/athena.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/athena.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/autoscaling.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/autoscaling.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/base.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,37 +3,38 @@
 import concurrent
 import logging
 from abc import ABC
 from collections import defaultdict, deque
 from concurrent.futures import Executor, Future
 from datetime import datetime, timezone
 from functools import lru_cache, reduce
-from threading import Lock, Event
-from typing import ClassVar, Dict, Optional, List, Type, Any, TypeVar, Callable, Iterator, Deque, Tuple
+from json import dumps as json_dumps
+from threading import Event, Lock
+from typing import Any, Callable, ClassVar, Deque, Dict, Iterator, List, Optional, Tuple, Type, TypeVar
 
 from attr import evolve, field
 from attrs import define
 from boto3.exceptions import Boto3Error
-
 from resoto_plugin_aws.aws_client import AwsClient
 from resoto_plugin_aws.configuration import AwsConfig
 from resoto_plugin_aws.resource.pricing import AwsPricingPrice
 from resoto_plugin_aws.utils import arn_partition
+
 from resotolib.baseresources import (
-    BaseResource,
-    EdgeType,
-    Cloud,
     BaseAccount,
     BaseRegion,
+    BaseResource,
     BaseVolumeType,
+    Cloud,
+    EdgeType,
     ModelReference,
 )
 from resotolib.config import Config, current_config
 from resotolib.core.actions import CoreFeedback
-from resotolib.graph import Graph, EdgeKey, ByNodeId, BySearchCriteria, NodeSelector
+from resotolib.graph import ByNodeId, BySearchCriteria, EdgeKey, Graph, NodeSelector
 from resotolib.json_bender import Bender, bend
 from resotolib.lock import RWLock
 from resotolib.proc import set_thread_name
 from resotolib.types import Json
 
 log = logging.getLogger("resoto.plugins.aws")
 
@@ -100,14 +101,22 @@
     def delete_tag(self, key: str) -> bool:
         return self.delete_resource_tag(get_client(current_config(), self), key)
 
     # legacy interface
     def delete(self, graph: Graph) -> bool:
         return self.delete_resource(get_client(current_config(), self), graph)
 
+    @classmethod
+    def service_name(cls) -> Optional[str]:
+        """
+        By default, every resource has an api_spec and the service name is derived from it.
+        For resources with custom handling, you need to override this method and define the service name explicitly.
+        """
+        return cls.api_spec.service if cls.api_spec else None
+
     def set_arn(
         self,
         builder: GraphBuilder,
         region: Optional[str] = None,
         service: Optional[str] = None,
         account: Optional[str] = None,
         resource: str = "",
@@ -126,16 +135,20 @@
     def id_from_arn(arn: str) -> str:
         if "/" in arn:
             return arn.rsplit("/")[-1]
         return arn.rsplit(":")[-1]
 
     @classmethod
     def from_api(cls: Type[AwsResourceType], json: Json) -> AwsResourceType:
-        mapped = bend(cls.mapping, json)
-        return cls.from_json(mapped)
+        try:
+            mapped = bend(cls.mapping, json)
+            return cls.from_json(mapped)
+        except Exception as e:
+            log.error(f"Error while mapping {cls.__name__}: {e}. Json: {json_dumps(json)}")
+            raise
 
     @classmethod
     def collect_resources(cls: Type[AwsResource], builder: GraphBuilder) -> None:
         # Default behavior: in case the class has an ApiSpec, call the api and call collect.
         log.debug(f"Collecting {cls.__name__} in region {builder.region.name}")
         if spec := cls.api_spec:
             try:
@@ -197,14 +210,15 @@
 class AwsAccount(BaseAccount, AwsResource):
     kind: ClassVar[str] = "aws_account"
     reference_kinds: ClassVar[ModelReference] = {"successors": {"default": ["aws_region"]}}
 
     account_alias: Optional[str] = ""
     role: Optional[str] = None
     profile: Optional[str] = None
+    partition: str = "aws"
     users: Optional[int] = 0
     groups: Optional[int] = 0
     account_mfa_enabled: Optional[int] = 0
     account_access_keys_present: Optional[int] = 0
     account_signing_certificates_present: Optional[int] = 0
     mfa_devices: Optional[int] = 0
     mfa_devices_in_use: Optional[int] = 0
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudformation.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/cloudformation.py`

 * *Files 2% similar despite different names*

```diff
@@ -323,13 +323,17 @@
     stack_instance_status_reason: Optional[str] = field(default=None)
     stack_instance_stack_instance_status: Optional[str] = field(default=None)
     stack_instance_organizational_unit_id: Optional[str] = field(default=None)
     stack_instance_drift_status: Optional[str] = field(default=None)
     stack_instance_last_drift_check_timestamp: Optional[datetime] = field(default=None)
     stack_instance_last_operation_id: Optional[str] = field(default=None)
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 resources: List[Type[AwsResource]] = [
     AwsCloudFormationStack,
     AwsCloudFormationStackSet,
     AwsCloudFormationStackInstanceSummary,
 ]
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudfront.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/cloudfront.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudtrail.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cloudwatch.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/cloudwatch.py`

 * *Files 1% similar despite different names*

```diff
@@ -256,18 +256,18 @@
 
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         if kms_key_id := source.get("kmsKeyId"):
             builder.dependant_node(self, clazz=AwsKmsKey, id=AwsKmsKey.normalise_id(kms_key_id))
 
     @classmethod
     def called_mutator_apis(cls) -> List[AwsApiSpec]:
-        return super().called_mutator_apis() + [AwsApiSpec(service_name, "delete-log-group")]
+        return super().called_mutator_apis() + [AwsApiSpec("logs", "delete-log-group")]
 
     def delete_resource(self, client: AwsClient, graph: Graph) -> bool:
-        client.call(aws_service=self.api_spec.service, action="delete-log-group", logGroupName=self.name)
+        client.call(aws_service="logs", action="delete-log-group", logGroupName=self.name)
         return True
 
 
 @define(eq=False, slots=False)
 class AwsCloudwatchMetricTransformation:
     kind: ClassVar[str] = "aws_cloudwatch_metric_transformation"
     mapping: ClassVar[Dict[str, Bender]] = {
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/cognito.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/cognito.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,14 +45,18 @@
 
     def delete_resource(self, client: AwsClient, graph: Graph) -> bool:
         client.call(
             aws_service=service_name, action="delete-group", result_name=None, GroupName=self.name, UserPoolId=self.id
         )
         return True
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 @define(eq=False, slots=False)
 class AwsCognitoAttributeType:
     kind: ClassVar[str] = "aws_cognito_attribute_type"
     mapping: ClassVar[Dict[str, Bender]] = {"name": S("Name"), "value": S("Value")}
     name: Optional[str] = field(default=None)
     value: Optional[str] = field(default=None)
@@ -84,14 +88,18 @@
         "mfa_options": S("MFAOptions", default=[]) >> ForallBend(AwsCognitoMFAOptionType.mapping),
     }
     user_attributes: List[AwsCognitoAttributeType] = field(factory=list)
     enabled: Optional[bool] = field(default=None)
     user_status: Optional[str] = field(default=None)
     mfa_options: List[AwsCognitoMFAOptionType] = field(factory=list)
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 @define(eq=False, slots=False)
 class AwsCognitoCustomSMSLambdaVersionConfigType:
     kind: ClassVar[str] = "aws_cognito_custom_sms_lambda_version_config_type"
     mapping: ClassVar[Dict[str, Bender]] = {"lambda_version": S("LambdaVersion"), "lambda_arn": S("LambdaArn")}
     lambda_version: Optional[str] = field(default=None)
     lambda_arn: Optional[str] = field(default=None)
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/config.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/dynamodb.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/dynamodb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/ec2.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/ec2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import logging
 from datetime import datetime
-from typing import ClassVar, Dict, Optional, List, Type
+from typing import ClassVar, Dict, Optional, List, Type, Any
 import copy
 
 from attrs import define, field
 from resoto_plugin_aws.aws_client import AwsClient
 
-from resoto_plugin_aws.resource.base import AwsResource, GraphBuilder, AwsApiSpec
+from resoto_plugin_aws.resource.base import AwsResource, GraphBuilder, AwsApiSpec, get_client
 from resoto_plugin_aws.resource.cloudwatch import AwsCloudwatchQuery, AwsCloudwatchMetricData
 from resoto_plugin_aws.resource.kms import AwsKmsKey
 from resoto_plugin_aws.resource.s3 import AwsS3Bucket
 from resoto_plugin_aws.utils import ToDict, TagsValue
 from resotolib.baseresources import (
     BaseInstance,
     EdgeType,
@@ -25,22 +26,24 @@
     BaseGateway,
     BaseSnapshot,
     BasePeeringConnection,
     BaseEndpoint,
     BaseRoutingTable,
     ModelReference,
 )
+from resotolib.config import current_config
 from resotolib.graph import Graph
 from resotolib.json_bender import Bender, S, Bend, ForallBend, bend, MapEnum, F, K, StripNones
 from resotolib.types import Json
 
 
 # region InstanceType
 from resotolib.utils import utc
 
+log = logging.getLogger("resoto.plugins.aws")
 service_name = "ec2"
 
 
 # noinspection PyUnresolvedReferences
 class EC2Taggable:
     def update_resource_tag(self, client: AwsClient, key: str, value: str) -> bool:
         if isinstance(self, AwsResource):
@@ -1438,14 +1441,29 @@
     nic_source_dest_check: Optional[bool] = field(default=None)
     nic_subnet_id: Optional[str] = field(default=None)
     nic_tag_set: List[AwsEc2Tag] = field(factory=list)
     nic_deny_all_igw_traffic: Optional[bool] = field(default=None)
     nic_ipv6_native: Optional[bool] = field(default=None)
     nic_ipv6_address: Optional[str] = field(default=None)
 
+    def pre_cleanup(self, graph: Optional[Any] = None) -> bool:
+        client = get_client(current_config(), self)
+        if (attachment := self.nic_attachment) and (aid := attachment.attachment_id):
+            try:
+                client.call(
+                    aws_service=self.api_spec.service,
+                    action="detach-network-interface",
+                    AttachmentId=aid,
+                    Force=True,
+                )
+            except Exception as e:
+                log.warning(f"Failed to detach network interface {self.id}: {e}")
+                return False
+        return True
+
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         super().connect_in_graph(builder, source)
         if vpc_id := source.get("VpcId"):
             builder.dependant_node(self, reverse=True, delete_same_as_default=True, clazz=AwsEc2Vpc, id=vpc_id)
         if subnet_id := source.get("SubnetId"):
             builder.add_edge(self, reverse=True, clazz=AwsEc2Subnet, id=subnet_id)
         if self.nic_attachment and (iid := self.nic_attachment.instance_id):
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/ecs.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/ecs.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,14 +47,18 @@
             return True
         return False
 
     @classmethod
     def called_mutator_apis(cls) -> List[AwsApiSpec]:
         return [AwsApiSpec(service_name, "tag-resource"), AwsApiSpec(service_name, "untag-resource")]
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 @define(eq=False, slots=False)
 class AwsEcsManagedScaling:
     kind: ClassVar[str] = "aws_ecs_managed_scaling"
     mapping: ClassVar[Dict[str, Bender]] = {
         "status": S("status"),
         "target_capacity": S("targetCapacity"),
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/efs.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/efs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/eks.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/eks.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,14 +45,18 @@
             return False
         return False
 
     @classmethod
     def called_mutator_apis(cls) -> List[AwsApiSpec]:
         return [AwsApiSpec(service_name, "tag-resource"), AwsApiSpec(service_name, "untag-resource")]
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 @define(eq=False, slots=False)
 class AwsEksNodegroupScalingConfig:
     kind: ClassVar[str] = "aws_eks_nodegroup_scaling_config"
     mapping: ClassVar[Dict[str, Bender]] = {
         "min_size": S("minSize"),
         "max_size": S("maxSize"),
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elasticache.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/elasticache.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elasticbeanstalk.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/elasticbeanstalk.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elb.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/elb.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/elbv2.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/elbv2.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/glacier.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/glacier.py`

 * *Files 0% similar despite different names*

```diff
@@ -157,14 +157,18 @@
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         # noinspection PyUnboundLocalVariable
         if (o := self.glacier_job_output_location) and (s3 := o.s3) and (e := s3.encryption) and (kid := e.kms_key_id):
             builder.dependant_node(self, clazz=AwsKmsKey, id=AwsKmsKey.normalise_id(kid))
         if self.glacier_job_sns_topic:
             builder.add_edge(self, clazz=AwsSnsTopic, arn=self.glacier_job_sns_topic)
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 @define(eq=False, slots=False)
 class AwsGlacierVault(AwsResource):
     kind: ClassVar[str] = "aws_glacier_vault"
     api_spec: ClassVar[AwsApiSpec] = AwsApiSpec(service_name, "list-vaults", "VaultList")
     reference_kinds: ClassVar[ModelReference] = {
         "successors": {
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/iam.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/iam.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,14 +170,18 @@
         return True
 
     def delete_resource(self, client: AwsClient, graph: Graph) -> bool:
         client.call(aws_service=service_name, action="delete-role", result_name=None, RoleName=self.name)
         return True
 
     @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
+    @classmethod
     def called_mutator_apis(cls) -> List[AwsApiSpec]:
         return [
             AwsApiSpec(service_name, "tag-role"),
             AwsApiSpec(service_name, "untag-role"),
             AwsApiSpec(service_name, "detach-role-policy"),
             AwsApiSpec(service_name, "delete-role-policy"),
             AwsApiSpec(service_name, "delete-role"),
@@ -321,14 +325,18 @@
     def called_mutator_apis(cls) -> List[AwsApiSpec]:
         return [
             AwsApiSpec(service_name, "tag-policy"),
             AwsApiSpec(service_name, "untag-policy"),
             AwsApiSpec(service_name, "delete-policy"),
         ]
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 @define(eq=False, slots=False)
 class AwsIamGroup(AwsResource, BaseGroup):
     # Note: this resource is collected via AwsIamUser.collect.
     kind: ClassVar[str] = "aws_iam_group"
     reference_kinds: ClassVar[ModelReference] = {
         "successors": {"default": ["aws_iam_policy"], "delete": ["aws_iam_policy"]},
@@ -341,14 +349,18 @@
         "path": S("Path"),
         "arn": S("Arn"),
         "group_policies": S("GroupPolicyList", default=[]) >> ForallBend(AwsIamPolicyDetail.mapping),
     }
     path: Optional[str] = field(default=None)
     group_policies: List[AwsIamPolicyDetail] = field(factory=list)
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
     def connect_in_graph(self, builder: GraphBuilder, source: Json) -> None:
         for policy in bend(S("AttachedManagedPolicies", default=[]), source):
             builder.dependant_node(self, clazz=AwsIamPolicy, delete_same_as_default=True, arn=policy.get("PolicyArn"))
 
     def pre_delete_resource(self, client: AwsClient, graph: Graph) -> bool:
         for successor in self.successors(graph, edge_type=EdgeType.delete):
             if isinstance(successor, AwsIamPolicy):
@@ -516,14 +528,15 @@
             report = builder.client.get(service_name, "get-credential-report", expected_errors=["ReportNotPresent"])
             return CredentialReportLine.from_str(report["Content"]) if report else {}
         else:
             return {}
 
     @staticmethod
     def from_str(lines: str) -> Dict[str, "CredentialReportLine"]:
+        # noinspection PyTypeChecker
         return {i["user"]: CredentialReportLine(i) for i in csv.DictReader(lines.splitlines(), delimiter=",")}
 
 
 @define(eq=False, slots=False)
 class AwsIamVirtualMfaDevice:
     kind: ClassVar[str] = "aws_iam_virtual_mfa_device"
     mapping: ClassVar[Dict[str, Bender]] = {
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/kinesis.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/kinesis.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/kms.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/kms.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/lambda_.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/lambda_.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/pricing.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/pricing.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,36 +1,58 @@
 import json
 from datetime import datetime
 from functools import lru_cache
-from typing import ClassVar, Dict, Optional, List, Any
+from typing import Any, ClassVar, Dict, List, Optional
 
 from attr import field, frozen
 from botocore.loaders import Loader
-
 from resoto_plugin_aws.aws_client import AwsClient
+
 from resotolib.json import from_json
-from resotolib.json_bender import Bender, S, Bend, MapDict, F, ForallBend, bend
+from resotolib.json_bender import Bend, Bender, F, ForallBend, MapDict, S, bend
 from resotolib.types import Json
+from resoto_plugin_aws.utils import arn_partition_by_region
 
 service_name = "pricing"
 
 EBS_TO_PRICING_NAMES = {
     "standard": "Magnetic",
     "gp2": "General Purpose",
     "gp3": "General Purpose",
     "io1": "Provisioned IOPS",
     "st1": "Throughput Optimized HDD",
     "sc1": "Cold HDD",
 }
 
 
 @lru_cache(maxsize=None)
+def partition_index() -> Dict[str, int]:
+    """Return a mapping from partition name to partition index."""
+    index_map = {}
+    try:
+        endpoints = Loader().load_data("endpoints")
+    except Exception:
+        pass
+    else:
+        for idx, partition in enumerate(endpoints.get("partitions", [])):
+            regions = partition.get("regions", {}).keys()
+            if "us-east-1" in regions:
+                index_map["aws"] = idx
+            elif "us-gov-west-1" in regions:
+                index_map["aws-us-gov"] = idx
+            elif "cn-north-1" in regions:
+                index_map["aws-cn"] = idx
+    return index_map
+
+
+@lru_cache(maxsize=None)
 def pricing_region(region: str) -> str:
+    idx = partition_index().get(arn_partition_by_region(region), 0)
     endpoints = Loader().load_data("endpoints")
-    name: Optional[str] = bend(S("partitions")[0] >> S("regions", region, "description"), endpoints)
+    name: Optional[str] = bend(S("partitions")[idx] >> S("regions", region, "description"), endpoints)
     if name is None:
         raise ValueError(f"Unknown pricing region: {region}")
     return name.replace("Europe", "EU")  # note: Europe is named differently in the price list
 
 
 @frozen(eq=False)
 class AwsPricingProduct:
@@ -108,15 +130,15 @@
                 return dim[0].price_per_unit.get("USD", 0)
         return 0
 
     @classmethod
     def single_price_for(
         cls, client: AwsClient, service_code: str, search_filter: List[Json]
     ) -> "Optional[AwsPricingPrice]":
-        # Prices are only available in us-east-1
+        # Prices are only available in the global region
         prices = client.global_region.list(
             service_name, "get-products", "PriceList", ServiceCode=service_code, Filters=search_filter, MaxResults=1
         )
         return from_json(bend(cls.mapping, json.loads(prices[0])), AwsPricingPrice) if prices else None
 
     @classmethod
     def volume_type_price(cls, client: AwsClient, volume_type: str, region: str) -> "Optional[AwsPricingPrice]":
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/rds.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/rds.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/redshift.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/redshift.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/route53.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/route53.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,14 +180,18 @@
     reference_kinds: ClassVar[ModelReference] = {
         "successors": {
             "default": [],
             "delete": [],
         }
     }
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 @define(eq=False, slots=False)
 class AwsRoute53ResourceRecordSet(AwsResource, BaseDNSRecordSet):
     kind: ClassVar[str] = "aws_route53_resource_record_set"
     reference_kinds: ClassVar[ModelReference] = {
         "successors": {
             "default": ["aws_route53_resource_record"],
@@ -235,9 +239,13 @@
             self.dns_zone().id,
             self.id,
             self.safe_name,
             self.record_type,
             self.record_set_identifier,
         )
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 resources: List[Type[AwsResource]] = [AwsRoute53Zone, AwsRoute53ResourceRecord, AwsRoute53ResourceRecordSet]
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/s3.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/s3.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/sagemaker.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/sagemaker.py`

 * *Files 0% similar despite different names*

```diff
@@ -823,17 +823,19 @@
 
     @classmethod
     def called_collect_apis(cls) -> List[AwsApiSpec]:
         return [cls.api_spec, AwsApiSpec(service_name, "describe-app")]
 
     @classmethod
     def collect(cls: Type[AwsResource], json: List[Json], builder: GraphBuilder) -> None:
-        # TODO don't collect Apps with status "deleted"
         for app in json:
-            if app["UserProfileName"]:
+            # Don't collect Apps that are deleted
+            if app.get("AppStatus") == "Deleted":
+                continue
+            elif app["UserProfileName"]:
                 app_description = builder.client.get(
                     service_name,
                     "describe-app",
                     None,
                     UserProfileName=app["UserProfileName"],
                     DomainId=app["DomainId"],
                     AppType=app["AppType"],
@@ -1918,15 +1920,15 @@
                 "aws_sagemaker_code_repository",
                 "aws_sagemaker_project",
             ],
         }
     }
     api_spec: ClassVar[AwsApiSpec] = AwsApiSpec(service_name, "list-artifacts", "ArtifactSummaries")
     mapping: ClassVar[Dict[str, Bender]] = {
-        "id": S("ArtifactName"),
+        "id": S("ArtifactArn"),
         "name": S("ArtifactName"),
         "ctime": S("CreationTime"),
         "mtime": S("LastModifiedTime"),
         "arn": S("ArtifactArn"),
         "artifact_source": S("Source") >> Bend(AwsSagemakerArtifactSource.mapping),
         "artifact_artifact_type": S("ArtifactType"),
         "artifact_properties": S("Properties"),
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/service_quotas.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/service_quotas.py`

 * *Files 1% similar despite different names*

```diff
@@ -147,14 +147,18 @@
     @classmethod
     def called_mutator_apis(cls) -> List[AwsApiSpec]:
         return [
             AwsApiSpec(service_name, "tag-resource", override_iam_permission="servicequotas:TagResource"),
             AwsApiSpec(service_name, "untag-resource", override_iam_permission="servicequotas:UntagResource"),
         ]
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 @define
 class QuotaMatcher:
     quota_name: Union[str, Pattern[str], None]
     node_kind: str
     node_selector: Dict[str, Any] = field(factory=dict)
     region: Optional[AwsRegion] = None
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/sns.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/sns.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,14 +205,18 @@
         client.call(aws_service=service_name, action="delete-endpoint", result_name=None, EndpointArn=self.arn)
         return True
 
     @classmethod
     def called_mutator_apis(cls) -> List[AwsApiSpec]:
         return [AwsApiSpec(service_name, "delete-endpoint")]
 
+    @classmethod
+    def service_name(cls) -> str:
+        return service_name
+
 
 @define(eq=False, slots=False)
 class AwsSnsPlatformApplication(AwsResource):
     kind: ClassVar[str] = "aws_sns_platform_application"
     api_spec: ClassVar[AwsApiSpec] = AwsApiSpec(
         service_name, "list-platform-applications", "PlatformApplications", expected_errors=["InvalidAction"]
     )
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/resource/sqs.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/resource/sqs.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws/utils.py` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws/utils.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 import uuid
-from typing import Iterable, List, Dict, Optional, Any, Callable
+from typing import Any, Callable, Dict, Iterable, List, Optional
 
 from boto3.session import Session as BotoSession
 from botocore.exceptions import ConnectionClosedError, CredentialRetrievalError
 from prometheus_client import Counter
 from retrying import retry
 
 from resotolib.baseresources import BaseRegion, BaseResource
 from resotolib.config import Config
 from resotolib.graph import Graph
 from resotolib.json_bender import Bender
 from resotolib.types import Json
 
-
 metrics_session_exceptions = Counter(
     "resoto_plugin_aws_session_exceptions_total",
     "Unhandled AWS Plugin Session Exceptions",
 )
 
 
 def retry_on_session_error(e: Exception) -> bool:
@@ -29,61 +28,71 @@
 @retry(  # type: ignore
     stop_max_attempt_number=10,
     wait_random_min=1000,
     wait_random_max=6000,
     retry_on_exception=retry_on_session_error,
 )
 def aws_session(
-    account: Optional[str] = None, role: Optional[str] = None, profile: Optional[str] = None
+    account: Optional[str] = None,
+    role: Optional[str] = None,
+    profile: Optional[str] = None,
+    partition: Optional[str] = None,
 ) -> BotoSession:
+    if partition is None:
+        partition = "aws"
+    global_region = global_region_by_partition(partition)
+
     if Config.aws.role_override:
         role = Config.aws.role
     if role and account:
-        role_arn = f"arn:aws:iam::{account}:role/{role}"
+        role_arn = f"arn:{partition}:iam::{account}:role/{role}"
         if profile:
             session = BotoSession(
                 profile_name=profile,
-                region_name="us-east-1",
+                region_name=global_region,
             )
         else:
             session = BotoSession(
                 aws_access_key_id=Config.aws.access_key_id,
                 aws_secret_access_key=Config.aws.secret_access_key,
-                region_name="us-east-1",
+                region_name=global_region,
             )
         sts = session.client("sts")
         token = sts.assume_role(RoleArn=role_arn, RoleSessionName=f"{account}-{str(uuid.uuid4())}")
         credentials = token["Credentials"]
         return BotoSession(
             aws_access_key_id=credentials["AccessKeyId"],
             aws_secret_access_key=credentials["SecretAccessKey"],
             aws_session_token=credentials["SessionToken"],
+            region_name=global_region,
         )
     else:
         if profile:
             return BotoSession(
                 profile_name=profile,
+                region_name=global_region,
             )
         else:
             return BotoSession(
                 aws_access_key_id=Config.aws.access_key_id,
                 aws_secret_access_key=Config.aws.secret_access_key,
+                region_name=global_region,
             )
 
 
 def aws_client(resource: BaseResource, service: str, graph: Optional[Graph] = None) -> BotoSession:
     ac = resource.account(graph)
-    return aws_session(ac.id, ac.role, ac.profile).client(  # type: ignore
+    return aws_session(ac.id, ac.role, ac.profile, ac.partition).client(  # type: ignore
         service, region_name=resource.region(graph).id
     )
 
 
 def aws_resource(resource: BaseResource, service: str, graph: Optional[Graph] = None) -> BotoSession:
     ac = resource.account(graph)
-    return aws_session(ac.id, ac.role, ac.profile).resource(  # type: ignore
+    return aws_session(ac.id, ac.role, ac.profile, ac.partition).resource(  # type: ignore
         service, region_name=resource.region(graph).id
     )
 
 
 def paginate(method: Callable[[], List[Any]], **kwargs: Any) -> Iterable[Any]:
     """Get a paginator for a boto3 list/describe method
 
@@ -97,22 +106,55 @@
     paginator = client.get_paginator(method.__name__)
     for page in paginator.paginate(**kwargs).result_key_iters():
         for result in page:
             yield result
 
 
 def arn_partition(region: BaseRegion) -> str:
+    return arn_partition_by_region(region.id)
+
+
+def arn_partition_by_region(region: str) -> str:
     arn_partition = "aws"
-    if region.id.startswith("cn-"):
+    if region.startswith("cn-"):
         arn_partition = "aws-cn"
-    elif region.id.startswith("us-gov-"):
+    elif region.startswith("us-gov-"):
         arn_partition = "aws-us-gov"
     return arn_partition
 
 
+def global_region_by_arn(arn: str) -> str:
+    if arn.startswith("arn:aws-us-gov:"):
+        return "us-gov-west-1"
+    elif arn.startswith("arn:aws-cn:"):
+        return "cn-north-1"
+    else:
+        return "us-east-1"
+
+
+def global_region_by_partition(partition: str) -> str:
+    if partition == "aws":
+        return "us-east-1"
+    elif partition == "aws-us-gov":
+        return "us-gov-west-1"
+    elif partition == "aws-cn":
+        return "cn-north-1"
+    else:
+        return "us-east-1"
+
+
+def global_region_by_region(region: str) -> str:
+    if region.startswith("us-gov-"):
+        return "us-gov-west-1"
+    elif region.startswith("cn-"):
+        return "cn-north-1"
+    else:
+        return "us-east-1"
+
+
 def tags_as_dict(tags: List[Json]) -> Dict[str, Optional[str]]:
     return {tag["Key"]: tag["Value"] for tag in tags or []}
 
 
 class ToDict(Bender):
     def __init__(self, key: str = "Key", value: str = "Value") -> None:
         self.key = key
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/PKG-INFO` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-aws
-Version: 3.5.0
-Summary: Resoto AWS Collector Plugin
-Home-page: https://github.com/someengineering/resoto/tree/main/plugins/aws
-License: Apache 2.0
-Keywords: cloud security
+Version: 3.5.1
+Summary: Runs collector plugins and sends the result to resotocore.
+Author: Some Engineering Inc.
+Project-URL: Documentation, https://resoto.com
+Project-URL: Source, https://github.com/someengineering/resoto/tree/main/plugins/aws
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 
 # resoto-plugin-aws
 An AWS collector plugin for Resoto.
 
 ## Usage
 For details on how to edit configuration, please see [the documentation](https://resoto.com/docs/getting-started/configuring-resoto).
```

### Comparing `resoto-plugin-aws-3.5.0/resoto_plugin_aws.egg-info/SOURCES.txt` & `resoto-plugin-aws-3.5.1/resoto_plugin_aws.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 MANIFEST.in
 README.md
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 resoto_plugin_aws/__init__.py
 resoto_plugin_aws/aws_client.py
 resoto_plugin_aws/collector.py
 resoto_plugin_aws/configuration.py
 resoto_plugin_aws/utils.py
 resoto_plugin_aws.egg-info/PKG-INFO
 resoto_plugin_aws.egg-info/SOURCES.txt
```

### Comparing `resoto-plugin-aws-3.5.0/test/__init__.py` & `resoto-plugin-aws-3.5.1/test/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/aws_client_test.py` & `resoto-plugin-aws-3.5.1/test/aws_client_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/collector_test.py` & `resoto-plugin-aws-3.5.1/test/collector_test.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,16 +27,16 @@
 
     for resource in all_resources:
         assert count_kind(resource) > 0, "No instances of {} found".format(resource.__name__)
 
     # make sure all threads have been joined
     assert len(threading.enumerate()) == 1
     # ensure the correct number of nodes and edges
-    assert count_kind(AwsResource) == 204
-    assert len(account_collector.graph.edges) == 476
+    assert count_kind(AwsResource) == 205
+    assert len(account_collector.graph.edges) == 477
     assert len(account_collector.graph.deferred_edges) == 2
 
 
 def test_dependencies() -> None:
     model = dataclasses_to_resotocore_model({AwsResource})
 
     def for_edge_type(edge_type: str) -> DiGraph:
@@ -68,7 +68,12 @@
     print("\n\n", collect_statement, "\n\n")
     assert json.loads(collect_statement)
     assert len(collect_allow) >= 74
     assert "s3:ListAllMyBuckets" in collect_allow
 
     mutate_allow, mutate_statement = iam_statement("ResotoMutatePermission", called_mutator_apis())
     print("\n\n", mutate_statement, "\n\n")
+
+
+def test_service_name_is_defined_in_all_resources() -> None:
+    for rt in all_resources:
+        assert rt.service_name() is not None, rt.__name__ + " has no service_name"
```

### Comparing `resoto-plugin-aws-3.5.0/test/graphbuilder_test.py` & `resoto-plugin-aws-3.5.1/test/graphbuilder_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/__init__.py` & `resoto-plugin-aws-3.5.1/test/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/apigateway_test.py` & `resoto-plugin-aws-3.5.1/test/resources/apigateway_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/athena_test.py` & `resoto-plugin-aws-3.5.1/test/resources/athena_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/autoscaling_test.py` & `resoto-plugin-aws-3.5.1/test/resources/autoscaling_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/base_test.py` & `resoto-plugin-aws-3.5.1/test/resources/base_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/cloudformation_test.py` & `resoto-plugin-aws-3.5.1/test/resources/cloudformation_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/cloudfront_test.py` & `resoto-plugin-aws-3.5.1/test/resources/cloudfront_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/cloudtrail_test.py` & `resoto-plugin-aws-3.5.1/test/resources/cloudtrail_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/cloudwatch_test.py` & `resoto-plugin-aws-3.5.1/test/resources/cloudwatch_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/cognito_test.py` & `resoto-plugin-aws-3.5.1/test/resources/cognito_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/dynamodb_test.py` & `resoto-plugin-aws-3.5.1/test/resources/dynamodb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/ec2_test.py` & `resoto-plugin-aws-3.5.1/test/resources/ec2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/ecs_test.py` & `resoto-plugin-aws-3.5.1/test/resources/ecs_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/eks_test.py` & `resoto-plugin-aws-3.5.1/test/resources/eks_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/elasticache_test.py` & `resoto-plugin-aws-3.5.1/test/resources/elasticache_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/elasticbeanstalk_test.py` & `resoto-plugin-aws-3.5.1/test/resources/elasticbeanstalk_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/elb_test.py` & `resoto-plugin-aws-3.5.1/test/resources/elb_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/elbv2_test.py` & `resoto-plugin-aws-3.5.1/test/resources/elbv2_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/glacier_test.py` & `resoto-plugin-aws-3.5.1/test/resources/glacier_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/iam_test.py` & `resoto-plugin-aws-3.5.1/test/resources/iam_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/kinesis_test.py` & `resoto-plugin-aws-3.5.1/test/resources/kinesis_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/kms_test.py` & `resoto-plugin-aws-3.5.1/test/resources/kms_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/lambda_test.py` & `resoto-plugin-aws-3.5.1/test/resources/lambda_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/pricing_test.py` & `resoto-plugin-aws-3.5.1/test/resources/pricing_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/rds_test.py` & `resoto-plugin-aws-3.5.1/test/resources/rds_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/redshift_test.py` & `resoto-plugin-aws-3.5.1/test/resources/redshift_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/route53_test.py` & `resoto-plugin-aws-3.5.1/test/resources/route53_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/s3_test.py` & `resoto-plugin-aws-3.5.1/test/resources/s3_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/sagemaker_test.py` & `resoto-plugin-aws-3.5.1/test/resources/sagemaker_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 def test_image() -> None:
     first, builder = round_trip_for(AwsSagemakerImage)
     assert len(builder.resources_of(AwsSagemakerImage)) == 1
 
 
 def test_artifact() -> None:
     first, builder = round_trip_for(AwsSagemakerArtifact)
-    assert len(builder.resources_of(AwsSagemakerArtifact)) == 1
+    assert len(builder.resources_of(AwsSagemakerArtifact)) == 2
 
 
 def test_user_profile() -> None:
     first, builder = round_trip_for(AwsSagemakerUserProfile)
     assert len(builder.resources_of(AwsSagemakerUserProfile)) == 1
```

### Comparing `resoto-plugin-aws-3.5.0/test/resources/service_quotas_test.py` & `resoto-plugin-aws-3.5.1/test/resources/service_quotas_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/sns_test.py` & `resoto-plugin-aws-3.5.1/test/resources/sns_test.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-aws-3.5.0/test/resources/sqs_test.py` & `resoto-plugin-aws-3.5.1/test/resources/sqs_test.py`

 * *Files identical despite different names*

