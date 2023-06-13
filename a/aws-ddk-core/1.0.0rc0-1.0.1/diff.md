# Comparing `tmp/aws-ddk-core-1.0.0rc0.tar.gz` & `tmp/aws-ddk-core-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-ddk-core-1.0.0rc0.tar", last modified: Wed May 17 19:00:02 2023, max compression
+gzip compressed data, was "aws-ddk-core-1.0.1.tar", last modified: Tue Jun 13 18:39:14 2023, max compression
```

## Comparing `aws-ddk-core-1.0.0rc0.tar` & `aws-ddk-core-1.0.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-05-17 19:00:02.306179 aws-ddk-core-1.0.0rc0/
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)    11358 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/LICENSE
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       23 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/MANIFEST.in
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       67 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/NOTICE
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     6066 2023-05-17 19:00:02.305837 aws-ddk-core-1.0.0rc0/PKG-INFO
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     5052 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/README.md
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      234 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/pyproject.toml
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       38 2023-05-17 19:00:02.306284 aws-ddk-core-1.0.0rc0/setup.cfg
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     2082 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/setup.py
-drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-05-17 19:00:02.291633 aws-ddk-core-1.0.0rc0/src/
-drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-05-17 19:00:02.295908 aws-ddk-core-1.0.0rc0/src/aws_ddk_core/
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)   540084 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core/__init__.py
-drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-05-17 19:00:02.298863 aws-ddk-core-1.0.0rc0/src/aws_ddk_core/_jsii/
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      583 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core/_jsii/__init__.py
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)  5515151 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core/_jsii/aws-ddk-core@1.0.0-rc.0.jsii.tgz
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)        1 2023-05-17 18:59:48.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core/py.typed
-drwxr-xr-x   0 hansonlu (569507325) ANT\Domain Users (1896053708)        0 2023-05-17 19:00:02.298126 aws-ddk-core-1.0.0rc0/src/aws_ddk_core.egg-info/
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)     6066 2023-05-17 19:00:02.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core.egg-info/PKG-INFO
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      405 2023-05-17 19:00:02.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core.egg-info/SOURCES.txt
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)        1 2023-05-17 19:00:02.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core.egg-info/dependency_links.txt
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)      313 2023-05-17 19:00:02.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core.egg-info/requires.txt
--rw-r--r--   0 hansonlu (569507325) ANT\Domain Users (1896053708)       13 2023-05-17 19:00:02.000000 aws-ddk-core-1.0.0rc0/src/aws_ddk_core.egg-info/top_level.txt
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-06-13 18:39:14.557881 aws-ddk-core-1.0.1/
+-rw-r--r--   0 hansonlu (569507325) 1896053708    11358 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/LICENSE
+-rw-r--r--   0 hansonlu (569507325) 1896053708       23 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/MANIFEST.in
+-rw-r--r--   0 hansonlu (569507325) 1896053708       67 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/NOTICE
+-rw-r--r--   0 hansonlu (569507325) 1896053708     6364 2023-06-13 18:39:14.557461 aws-ddk-core-1.0.1/PKG-INFO
+-rw-r--r--   0 hansonlu (569507325) 1896053708     5387 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/README.md
+-rw-r--r--   0 hansonlu (569507325) 1896053708      234 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/pyproject.toml
+-rw-r--r--   0 hansonlu (569507325) 1896053708       38 2023-06-13 18:39:14.558003 aws-ddk-core-1.0.1/setup.cfg
+-rw-r--r--   0 hansonlu (569507325) 1896053708     2039 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/setup.py
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-06-13 18:39:14.541234 aws-ddk-core-1.0.1/src/
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-06-13 18:39:14.546616 aws-ddk-core-1.0.1/src/aws_ddk_core/
+-rw-r--r--   0 hansonlu (569507325) 1896053708   542656 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/src/aws_ddk_core/__init__.py
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-06-13 18:39:14.549755 aws-ddk-core-1.0.1/src/aws_ddk_core/_jsii/
+-rw-r--r--   0 hansonlu (569507325) 1896053708      573 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/src/aws_ddk_core/_jsii/__init__.py
+-rw-r--r--   0 hansonlu (569507325) 1896053708  5017715 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/src/aws_ddk_core/_jsii/aws-ddk-core@1.0.1.jsii.tgz
+-rw-r--r--   0 hansonlu (569507325) 1896053708        1 2023-06-13 18:38:56.000000 aws-ddk-core-1.0.1/src/aws_ddk_core/py.typed
+drwxr-xr-x   0 hansonlu (569507325) 1896053708        0 2023-06-13 18:39:14.548849 aws-ddk-core-1.0.1/src/aws_ddk_core.egg-info/
+-rw-r--r--   0 hansonlu (569507325) 1896053708     6364 2023-06-13 18:39:14.000000 aws-ddk-core-1.0.1/src/aws_ddk_core.egg-info/PKG-INFO
+-rw-r--r--   0 hansonlu (569507325) 1896053708      400 2023-06-13 18:39:14.000000 aws-ddk-core-1.0.1/src/aws_ddk_core.egg-info/SOURCES.txt
+-rw-r--r--   0 hansonlu (569507325) 1896053708        1 2023-06-13 18:39:14.000000 aws-ddk-core-1.0.1/src/aws_ddk_core.egg-info/dependency_links.txt
+-rw-r--r--   0 hansonlu (569507325) 1896053708      313 2023-06-13 18:39:14.000000 aws-ddk-core-1.0.1/src/aws_ddk_core.egg-info/requires.txt
+-rw-r--r--   0 hansonlu (569507325) 1896053708       13 2023-06-13 18:39:14.000000 aws-ddk-core-1.0.1/src/aws_ddk_core.egg-info/top_level.txt
```

### Comparing `aws-ddk-core-1.0.0rc0/LICENSE` & `aws-ddk-core-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `aws-ddk-core-1.0.0rc0/PKG-INFO` & `aws-ddk-core-1.0.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: aws-ddk-core
-Version: 1.0.0rc0
+Version: 1.0.1
 Summary: AWS DataOps Development Kit
-Home-page: https://github.com/awslabs/aws-ddk/tree/typescript-conversion
+Home-page: https://github.com/awslabs/aws-ddk/tree/main
 Author: AWS Professional Services<aws-proserve-orion-dev@amazon.com>
 License: Apache-2.0
-Project-URL: Source, https://github.com/awslabs/aws-ddk/tree/typescript-conversion
+Project-URL: Source, https://github.com/awslabs/aws-ddk/tree/main
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -22,14 +22,23 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # AWS DataOps Development Kit (DDK)
 
 ![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/build.yml/badge.svg)
+[![Downloads](https://static.pepy.tech/personalized-badge/aws-ddk-core?period=total&units=international_system&left_color=black&right_color=orange&left_text=pypi%20downloads)](https://pepy.tech/project/aws-ddk-core)
+
+##### Packages 🗳️
+
+* [NPM](https://www.npmjs.com/package/aws-ddk-core/)
+* [Pypi](https://pypi.org/project/aws-ddk-core/)
+
+---
+
 
 The AWS DataOps Development Kit is an open source development framework for customers that build data workflows and modern data architecture on AWS.
 
 Based on the [AWS CDK](https://github.com/aws/aws-cdk), it offers high-level abstractions allowing you to build pipelines that manage data flows on AWS, driven by DevOps best practices.  The framework is extensible, you can add abstractions for your own data processing infrastructure or replace our best practices with your own standards. It's easy to share templates, so everyone in your organisation can concentrate on the business logic of dealing with their data, rather than boilerplate logic.
 
 ---
 
@@ -82,16 +91,16 @@
     .add_stage(firehose_s3_stage)
     .add_stage(sqs_lambda_stage)
 )
 ...
 ```
 
 First, we import the required resources from the aws_ddk_core library, including the two stage constructs:
-[FirehoseToS3Stage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.0-beta.1/api/FirehoseToS3Stage) and
-[SqsToLambdaStage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.0-beta.1/api/SqsToLambdaStage).
+[FirehoseToS3Stage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.1/api/FirehoseToS3Stage) and
+[SqsToLambdaStage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.1/api/SqsToLambdaStage).
 These two classes are then instantiated and the delivery stream is configured with the S3 prefix (raw/).
 Finally, the DDK DataPipeline construct is used to chain these two stages together into a data pipeline.
 
 Complete source code of the data pipeline above can be found in
 [AWS DDK Examples - Basic Data Pipeline](https://github.com/aws-samples/aws-ddk-examples/tree/main/basic-data-pipeline)
 
 ### Official Resources
```

### Comparing `aws-ddk-core-1.0.0rc0/README.md` & `aws-ddk-core-1.0.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 # AWS DataOps Development Kit (DDK)
 
 ![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/build.yml/badge.svg)
+[![Downloads](https://static.pepy.tech/personalized-badge/aws-ddk-core?period=total&units=international_system&left_color=black&right_color=orange&left_text=pypi%20downloads)](https://pepy.tech/project/aws-ddk-core)
+
+##### Packages 🗳️
+
+* [NPM](https://www.npmjs.com/package/aws-ddk-core/)
+* [Pypi](https://pypi.org/project/aws-ddk-core/)
+
+---
+
 
 The AWS DataOps Development Kit is an open source development framework for customers that build data workflows and modern data architecture on AWS.
 
 Based on the [AWS CDK](https://github.com/aws/aws-cdk), it offers high-level abstractions allowing you to build pipelines that manage data flows on AWS, driven by DevOps best practices.  The framework is extensible, you can add abstractions for your own data processing infrastructure or replace our best practices with your own standards. It's easy to share templates, so everyone in your organisation can concentrate on the business logic of dealing with their data, rather than boilerplate logic.
 
 ---
 
@@ -57,16 +66,16 @@
     .add_stage(firehose_s3_stage)
     .add_stage(sqs_lambda_stage)
 )
 ...
 ```
 
 First, we import the required resources from the aws_ddk_core library, including the two stage constructs:
-[FirehoseToS3Stage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.0-beta.1/api/FirehoseToS3Stage) and
-[SqsToLambdaStage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.0-beta.1/api/SqsToLambdaStage).
+[FirehoseToS3Stage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.1/api/FirehoseToS3Stage) and
+[SqsToLambdaStage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.1/api/SqsToLambdaStage).
 These two classes are then instantiated and the delivery stream is configured with the S3 prefix (raw/).
 Finally, the DDK DataPipeline construct is used to chain these two stages together into a data pipeline.
 
 Complete source code of the data pipeline above can be found in
 [AWS DDK Examples - Basic Data Pipeline](https://github.com/aws-samples/aws-ddk-examples/tree/main/basic-data-pipeline)
 
 ### Official Resources
```

### Comparing `aws-ddk-core-1.0.0rc0/setup.py` & `aws-ddk-core-1.0.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,50 +1,50 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "aws-ddk-core",
-    "version": "1.0.0.rc0",
+    "version": "1.0.1",
     "description": "AWS DataOps Development Kit",
     "license": "Apache-2.0",
-    "url": "https://github.com/awslabs/aws-ddk/tree/typescript-conversion",
+    "url": "https://github.com/awslabs/aws-ddk/tree/main",
     "long_description_content_type": "text/markdown",
     "author": "AWS Professional Services<aws-proserve-orion-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
     },
     "project_urls": {
-        "Source": "https://github.com/awslabs/aws-ddk/tree/typescript-conversion"
+        "Source": "https://github.com/awslabs/aws-ddk/tree/main"
     },
     "package_dir": {
         "": "src"
     },
     "packages": [
         "aws_ddk_core",
         "aws_ddk_core._jsii"
     ],
     "package_data": {
         "aws_ddk_core._jsii": [
-            "aws-ddk-core@1.0.0-rc.0.jsii.tgz"
+            "aws-ddk-core@1.0.1.jsii.tgz"
         ],
         "aws_ddk_core": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.71.0, <3.0.0",
         "aws-cdk.aws-glue-alpha>=2.71.0.a0, <3.0.0",
         "aws-cdk.aws-kinesisfirehose-alpha>=2.71.0.a0, <3.0.0",
         "aws-cdk.aws-kinesisfirehose-destinations-alpha>=2.71.0.a0, <3.0.0",
         "aws-cdk.integ-tests-alpha>=2.71.0.a0, <3.0.0",
         "constructs>=10.0.5, <11.0.0",
-        "jsii>=1.80.0, <2.0.0",
+        "jsii>=1.83.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
```

### Comparing `aws-ddk-core-1.0.0rc0/src/aws_ddk_core/__init__.py` & `aws-ddk-core-1.0.1/src/aws_ddk_core/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,20 @@
 '''
 # AWS DataOps Development Kit (DDK)
 
 ![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/build.yml/badge.svg)
+[![Downloads](https://static.pepy.tech/personalized-badge/aws-ddk-core?period=total&units=international_system&left_color=black&right_color=orange&left_text=pypi%20downloads)](https://pepy.tech/project/aws-ddk-core)
+
+##### Packages 🗳️
+
+* [NPM](https://www.npmjs.com/package/aws-ddk-core/)
+* [Pypi](https://pypi.org/project/aws-ddk-core/)
+
+---
+
 
 The AWS DataOps Development Kit is an open source development framework for customers that build data workflows and modern data architecture on AWS.
 
 Based on the [AWS CDK](https://github.com/aws/aws-cdk), it offers high-level abstractions allowing you to build pipelines that manage data flows on AWS, driven by DevOps best practices.  The framework is extensible, you can add abstractions for your own data processing infrastructure or replace our best practices with your own standards. It's easy to share templates, so everyone in your organisation can concentrate on the business logic of dealing with their data, rather than boilerplate logic.
 
 ---
 
@@ -58,16 +67,16 @@
     .add_stage(firehose_s3_stage)
     .add_stage(sqs_lambda_stage)
 )
 ...
 ```
 
 First, we import the required resources from the aws_ddk_core library, including the two stage constructs:
-[FirehoseToS3Stage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.0-beta.1/api/FirehoseToS3Stage) and
-[SqsToLambdaStage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.0-beta.1/api/SqsToLambdaStage).
+[FirehoseToS3Stage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.1/api/FirehoseToS3Stage) and
+[SqsToLambdaStage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.1/api/SqsToLambdaStage).
 These two classes are then instantiated and the delivery stream is configured with the S3 prefix (raw/).
 Finally, the DDK DataPipeline construct is used to chain these two stages together into a data pipeline.
 
 Complete source code of the data pipeline above can be found in
 [AWS DDK Examples - Basic Data Pipeline](https://github.com/aws-samples/aws-ddk-examples/tree/main/basic-data-pipeline)
 
 ### Official Resources
@@ -474,41 +483,53 @@
         )
 
 
 @jsii.data_type(
     jsii_type="aws-ddk-core.AddSecurityLintStageProps",
     jsii_struct_bases=[],
     name_mapping={
+        "cfn_nag_fail_build": "cfnNagFailBuild",
         "cloud_assembly_file_set": "cloudAssemblyFileSet",
         "stage_name": "stageName",
     },
 )
 class AddSecurityLintStageProps:
     def __init__(
         self,
         *,
+        cfn_nag_fail_build: typing.Optional[builtins.bool] = None,
         cloud_assembly_file_set: typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer] = None,
         stage_name: typing.Optional[builtins.str] = None,
     ) -> None:
         '''Properties for adding a security lint stage.
 
+        :param cfn_nag_fail_build: Fail Codepipeline Build Action on failed results from CfnNag scan.
         :param cloud_assembly_file_set: Cloud assembly file set producer.
         :param stage_name: Name of the stage.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f5c6a426f2b47035ddfb61265fb0fc5f914c183c57db8be19fd6917fe3755000)
+            check_type(argname="argument cfn_nag_fail_build", value=cfn_nag_fail_build, expected_type=type_hints["cfn_nag_fail_build"])
             check_type(argname="argument cloud_assembly_file_set", value=cloud_assembly_file_set, expected_type=type_hints["cloud_assembly_file_set"])
             check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
         self._values: typing.Dict[builtins.str, typing.Any] = {}
+        if cfn_nag_fail_build is not None:
+            self._values["cfn_nag_fail_build"] = cfn_nag_fail_build
         if cloud_assembly_file_set is not None:
             self._values["cloud_assembly_file_set"] = cloud_assembly_file_set
         if stage_name is not None:
             self._values["stage_name"] = stage_name
 
     @builtins.property
+    def cfn_nag_fail_build(self) -> typing.Optional[builtins.bool]:
+        '''Fail Codepipeline Build Action on failed results from CfnNag scan.'''
+        result = self._values.get("cfn_nag_fail_build")
+        return typing.cast(typing.Optional[builtins.bool], result)
+
+    @builtins.property
     def cloud_assembly_file_set(
         self,
     ) -> typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer]:
         '''Cloud assembly file set producer.'''
         result = self._values.get("cloud_assembly_file_set")
         return typing.cast(typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer], result)
 
@@ -1457,24 +1478,27 @@
 
     @jsii.member(jsii_name="getCfnNagAction")
     @builtins.classmethod
     def get_cfn_nag_action(
         cls,
         file_set_producer: _aws_cdk_pipelines_ceddda9d.IFileSetProducer,
         stage_name: typing.Optional[builtins.str] = None,
+        fail_build: typing.Optional[builtins.bool] = None,
     ) -> _aws_cdk_pipelines_ceddda9d.ShellStep:
         '''
         :param file_set_producer: -
         :param stage_name: -
+        :param fail_build: -
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__ebe600cfab48179494151cd33416082a904aa73df681b93f5266545008838275)
             check_type(argname="argument file_set_producer", value=file_set_producer, expected_type=type_hints["file_set_producer"])
             check_type(argname="argument stage_name", value=stage_name, expected_type=type_hints["stage_name"])
-        return typing.cast(_aws_cdk_pipelines_ceddda9d.ShellStep, jsii.sinvoke(cls, "getCfnNagAction", [file_set_producer, stage_name]))
+            check_type(argname="argument fail_build", value=fail_build, expected_type=type_hints["fail_build"])
+        return typing.cast(_aws_cdk_pipelines_ceddda9d.ShellStep, jsii.sinvoke(cls, "getCfnNagAction", [file_set_producer, stage_name, fail_build]))
 
     @jsii.member(jsii_name="getCodeArtifactPublishAction")
     @builtins.classmethod
     def get_code_artifact_publish_action(
         cls,
         partition: builtins.str,
         region: builtins.str,
@@ -1736,26 +1760,30 @@
 
         return typing.cast("CICDPipelineStack", jsii.invoke(self, "addNotifications", [props]))
 
     @jsii.member(jsii_name="addSecurityLintStage")
     def add_security_lint_stage(
         self,
         *,
+        cfn_nag_fail_build: typing.Optional[builtins.bool] = None,
         cloud_assembly_file_set: typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer] = None,
         stage_name: typing.Optional[builtins.str] = None,
     ) -> "CICDPipelineStack":
         '''Add linting - cfn-nag, and bandit.
 
+        :param cfn_nag_fail_build: Fail Codepipeline Build Action on failed results from CfnNag scan.
         :param cloud_assembly_file_set: Cloud assembly file set producer.
         :param stage_name: Name of the stage.
 
         :return: reference to this pipeline.
         '''
         props = AddSecurityLintStageProps(
-            cloud_assembly_file_set=cloud_assembly_file_set, stage_name=stage_name
+            cfn_nag_fail_build=cfn_nag_fail_build,
+            cloud_assembly_file_set=cloud_assembly_file_set,
+            stage_name=stage_name,
         )
 
         return typing.cast("CICDPipelineStack", jsii.invoke(self, "addSecurityLintStage", [props]))
 
     @jsii.member(jsii_name="addSourceAction")
     def add_source_action(
         self,
@@ -2696,38 +2724,38 @@
         return typing.cast(typing.Optional[Configuration], jsii.sinvoke(cls, "getConfig", [props]))
 
     @jsii.member(jsii_name="getEnvConfig")
     @builtins.classmethod
     def get_env_config(
         cls,
         *,
-        config_path: builtins.str,
         environment_id: builtins.str,
+        config_path: typing.Optional[builtins.str] = None,
     ) -> "EnvironmentConfiguration":
         '''
-        :param config_path: 
-        :param environment_id: 
+        :param environment_id: Environment identifier.
+        :param config_path: Relative path to config file. Defaults to './ddk.json'
         '''
         props = GetEnvConfigProps(
-            config_path=config_path, environment_id=environment_id
+            environment_id=environment_id, config_path=config_path
         )
 
         return typing.cast("EnvironmentConfiguration", jsii.sinvoke(cls, "getEnvConfig", [props]))
 
     @jsii.member(jsii_name="getEnvironment")
     @builtins.classmethod
     def get_environment(
         cls,
         *,
         config_path: builtins.str,
         environment_id: typing.Optional[builtins.str] = None,
     ) -> _aws_cdk_ceddda9d.Environment:
         '''
-        :param config_path: 
-        :param environment_id: 
+        :param config_path: Relative path to config file. Defaults to './ddk.json'
+        :param environment_id: Environment identifier.
         '''
         props = GetEnvironmentProps(
             config_path=config_path, environment_id=environment_id
         )
 
         return typing.cast(_aws_cdk_ceddda9d.Environment, jsii.sinvoke(cls, "getEnvironment", [props]))
 
@@ -2736,16 +2764,16 @@
     def get_tags(
         cls,
         *,
         config_path: builtins.str,
         environment_id: typing.Optional[builtins.str] = None,
     ) -> typing.Mapping[builtins.str, builtins.str]:
         '''
-        :param config_path: 
-        :param environment_id: 
+        :param config_path: Relative path to config file. Defaults to './ddk.json'
+        :param environment_id: Environment identifier.
         '''
         props = GetTagsProps(config_path=config_path, environment_id=environment_id)
 
         return typing.cast(typing.Mapping[builtins.str, builtins.str], jsii.sinvoke(cls, "getTags", [props]))
 
     @jsii.member(jsii_name="getConfigAttribute")
     def get_config_attribute(self, attribute: builtins.str) -> typing.Any:
@@ -3263,48 +3291,53 @@
             k + "=" + repr(v) for k, v in self._values.items()
         )
 
 
 @jsii.data_type(
     jsii_type="aws-ddk-core.GetEnvConfigProps",
     jsii_struct_bases=[],
-    name_mapping={"config_path": "configPath", "environment_id": "environmentId"},
+    name_mapping={"environment_id": "environmentId", "config_path": "configPath"},
 )
 class GetEnvConfigProps:
     def __init__(
         self,
         *,
-        config_path: builtins.str,
         environment_id: builtins.str,
+        config_path: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param config_path: 
-        :param environment_id: 
+        :param environment_id: Environment identifier.
+        :param config_path: Relative path to config file. Defaults to './ddk.json'
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__392d4bf9e0a3416c4cbfe2cfcca884cc2b98f96b99a23a03e386497b6cfd2fef)
-            check_type(argname="argument config_path", value=config_path, expected_type=type_hints["config_path"])
             check_type(argname="argument environment_id", value=environment_id, expected_type=type_hints["environment_id"])
+            check_type(argname="argument config_path", value=config_path, expected_type=type_hints["config_path"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
-            "config_path": config_path,
             "environment_id": environment_id,
         }
-
-    @builtins.property
-    def config_path(self) -> builtins.str:
-        result = self._values.get("config_path")
-        assert result is not None, "Required property 'config_path' is missing"
-        return typing.cast(builtins.str, result)
+        if config_path is not None:
+            self._values["config_path"] = config_path
 
     @builtins.property
     def environment_id(self) -> builtins.str:
+        '''Environment identifier.'''
         result = self._values.get("environment_id")
         assert result is not None, "Required property 'environment_id' is missing"
         return typing.cast(builtins.str, result)
 
+    @builtins.property
+    def config_path(self) -> typing.Optional[builtins.str]:
+        '''Relative path to config file.
+
+        Defaults to './ddk.json'
+        '''
+        result = self._values.get("config_path")
+        return typing.cast(typing.Optional[builtins.str], result)
+
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
         return not (rhs == self)
 
     def __repr__(self) -> str:
@@ -3322,35 +3355,40 @@
     def __init__(
         self,
         *,
         config_path: builtins.str,
         environment_id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param config_path: 
-        :param environment_id: 
+        :param config_path: Relative path to config file. Defaults to './ddk.json'
+        :param environment_id: Environment identifier.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f1d1864ebb63e794b66b601804d8a186ccc2fe70e5c1aeea9def8ecd1ab83dde)
             check_type(argname="argument config_path", value=config_path, expected_type=type_hints["config_path"])
             check_type(argname="argument environment_id", value=environment_id, expected_type=type_hints["environment_id"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "config_path": config_path,
         }
         if environment_id is not None:
             self._values["environment_id"] = environment_id
 
     @builtins.property
     def config_path(self) -> builtins.str:
+        '''Relative path to config file.
+
+        Defaults to './ddk.json'
+        '''
         result = self._values.get("config_path")
         assert result is not None, "Required property 'config_path' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def environment_id(self) -> typing.Optional[builtins.str]:
+        '''Environment identifier.'''
         result = self._values.get("environment_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -3514,35 +3552,40 @@
     def __init__(
         self,
         *,
         config_path: builtins.str,
         environment_id: typing.Optional[builtins.str] = None,
     ) -> None:
         '''
-        :param config_path: 
-        :param environment_id: 
+        :param config_path: Relative path to config file. Defaults to './ddk.json'
+        :param environment_id: Environment identifier.
         '''
         if __debug__:
             type_hints = typing.get_type_hints(_typecheckingstub__f80411a398b3a95cafcc083fedf809e35c9f9d3c872682fa20c2c416251da930)
             check_type(argname="argument config_path", value=config_path, expected_type=type_hints["config_path"])
             check_type(argname="argument environment_id", value=environment_id, expected_type=type_hints["environment_id"])
         self._values: typing.Dict[builtins.str, typing.Any] = {
             "config_path": config_path,
         }
         if environment_id is not None:
             self._values["environment_id"] = environment_id
 
     @builtins.property
     def config_path(self) -> builtins.str:
+        '''Relative path to config file.
+
+        Defaults to './ddk.json'
+        '''
         result = self._values.get("config_path")
         assert result is not None, "Required property 'config_path' is missing"
         return typing.cast(builtins.str, result)
 
     @builtins.property
     def environment_id(self) -> typing.Optional[builtins.str]:
+        '''Environment identifier.'''
         result = self._values.get("environment_id")
         return typing.cast(typing.Optional[builtins.str], result)
 
     def __eq__(self, rhs: typing.Any) -> builtins.bool:
         return isinstance(rhs, self.__class__) and rhs._values == self._values
 
     def __ne__(self, rhs: typing.Any) -> builtins.bool:
@@ -9056,14 +9099,15 @@
     schedule: typing.Optional[_aws_cdk_aws_events_ceddda9d.Schedule] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__f5c6a426f2b47035ddfb61265fb0fc5f914c183c57db8be19fd6917fe3755000(
     *,
+    cfn_nag_fail_build: typing.Optional[builtins.bool] = None,
     cloud_assembly_file_set: typing.Optional[_aws_cdk_pipelines_ceddda9d.IFileSetProducer] = None,
     stage_name: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__c40909713474fb0ac5879649d02b6b9b99cca8e07cc03cfb0ee3a2161cabd53f(
@@ -9177,14 +9221,15 @@
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__ebe600cfab48179494151cd33416082a904aa73df681b93f5266545008838275(
     file_set_producer: _aws_cdk_pipelines_ceddda9d.IFileSetProducer,
     stage_name: typing.Optional[builtins.str] = None,
+    fail_build: typing.Optional[builtins.bool] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__203dfc08c6a839aacb072ea162bb03ae398d33f465cc8723ee83f36c65bf9fc8(
     partition: builtins.str,
     region: builtins.str,
@@ -9408,16 +9453,16 @@
     config: typing.Optional[typing.Union[builtins.str, typing.Union[Configuration, typing.Dict[builtins.str, typing.Any]]]] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__392d4bf9e0a3416c4cbfe2cfcca884cc2b98f96b99a23a03e386497b6cfd2fef(
     *,
-    config_path: builtins.str,
     environment_id: builtins.str,
+    config_path: typing.Optional[builtins.str] = None,
 ) -> None:
     """Type checking stubs"""
     pass
 
 def _typecheckingstub__f1d1864ebb63e794b66b601804d8a186ccc2fe70e5c1aeea9def8ecd1ab83dde(
     *,
     config_path: builtins.str,
```

### Comparing `aws-ddk-core-1.0.0rc0/src/aws_ddk_core/_jsii/__init__.py` & `aws-ddk-core-1.0.1/src/aws_ddk_core/_jsii/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 import aws_cdk.aws_glue_alpha._jsii
 import aws_cdk.aws_kinesisfirehose_alpha._jsii
 import aws_cdk.aws_kinesisfirehose_destinations_alpha._jsii
 import aws_cdk.integ_tests_alpha._jsii
 import constructs._jsii
 
 __jsii_assembly__ = jsii.JSIIAssembly.load(
-    "aws-ddk-core", "1.0.0-rc.0", __name__[0:-6], "aws-ddk-core@1.0.0-rc.0.jsii.tgz"
+    "aws-ddk-core", "1.0.1", __name__[0:-6], "aws-ddk-core@1.0.1.jsii.tgz"
 )
 
 __all__ = [
     "__jsii_assembly__",
 ]
 
 publication.publish()
```

### Comparing `aws-ddk-core-1.0.0rc0/src/aws_ddk_core.egg-info/PKG-INFO` & `aws-ddk-core-1.0.1/src/aws_ddk_core.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.1
 Name: aws-ddk-core
-Version: 1.0.0rc0
+Version: 1.0.1
 Summary: AWS DataOps Development Kit
-Home-page: https://github.com/awslabs/aws-ddk/tree/typescript-conversion
+Home-page: https://github.com/awslabs/aws-ddk/tree/main
 Author: AWS Professional Services<aws-proserve-orion-dev@amazon.com>
 License: Apache-2.0
-Project-URL: Source, https://github.com/awslabs/aws-ddk/tree/typescript-conversion
+Project-URL: Source, https://github.com/awslabs/aws-ddk/tree/main
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -22,14 +22,23 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 
 # AWS DataOps Development Kit (DDK)
 
 ![Actions Status](https://github.com/awslabs/aws-ddk/actions/workflows/build.yml/badge.svg)
+[![Downloads](https://static.pepy.tech/personalized-badge/aws-ddk-core?period=total&units=international_system&left_color=black&right_color=orange&left_text=pypi%20downloads)](https://pepy.tech/project/aws-ddk-core)
+
+##### Packages 🗳️
+
+* [NPM](https://www.npmjs.com/package/aws-ddk-core/)
+* [Pypi](https://pypi.org/project/aws-ddk-core/)
+
+---
+
 
 The AWS DataOps Development Kit is an open source development framework for customers that build data workflows and modern data architecture on AWS.
 
 Based on the [AWS CDK](https://github.com/aws/aws-cdk), it offers high-level abstractions allowing you to build pipelines that manage data flows on AWS, driven by DevOps best practices.  The framework is extensible, you can add abstractions for your own data processing infrastructure or replace our best practices with your own standards. It's easy to share templates, so everyone in your organisation can concentrate on the business logic of dealing with their data, rather than boilerplate logic.
 
 ---
 
@@ -82,16 +91,16 @@
     .add_stage(firehose_s3_stage)
     .add_stage(sqs_lambda_stage)
 )
 ...
 ```
 
 First, we import the required resources from the aws_ddk_core library, including the two stage constructs:
-[FirehoseToS3Stage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.0-beta.1/api/FirehoseToS3Stage) and
-[SqsToLambdaStage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.0-beta.1/api/SqsToLambdaStage).
+[FirehoseToS3Stage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.1/api/FirehoseToS3Stage) and
+[SqsToLambdaStage()](https://constructs.dev/packages/aws-ddk-core/v/1.0.1/api/SqsToLambdaStage).
 These two classes are then instantiated and the delivery stream is configured with the S3 prefix (raw/).
 Finally, the DDK DataPipeline construct is used to chain these two stages together into a data pipeline.
 
 Complete source code of the data pipeline above can be found in
 [AWS DDK Examples - Basic Data Pipeline](https://github.com/aws-samples/aws-ddk-examples/tree/main/basic-data-pipeline)
 
 ### Official Resources
```

