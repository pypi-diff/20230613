# Comparing `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113.tar.gz` & `tmp/echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113.tar", last modified: Tue Jun  6 21:12:24 2023, max compression
+gzip compressed data, was "echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103.tar", last modified: Tue Jun 13 21:02:12 2023, max compression
```

## Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113.tar` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:12:24.869142 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/
--rw-r--r--   0 root         (0) root         (0)     1065 2023-06-06 21:11:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2462 2023-06-06 21:12:24.869142 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2113 2023-06-06 21:11:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/README.md
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-06 21:12:24.869142 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      709 2023-06-06 21:12:19.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:12:24.869142 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:12:24.869142 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-06-06 21:11:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17112 2023-06-06 21:11:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
--rw-r--r--   0 root         (0) root         (0)      642 2023-06-06 21:11:09.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-06 21:12:24.869142 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2462 2023-06-06 21:12:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      477 2023-06-06 21:12:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-06 21:12:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      127 2023-06-06 21:12:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-06-06 21:12:24.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:02:12.206186 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-06-13 21:00:58.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-06-13 21:02:12.206186 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2113 2023-06-13 21:00:58.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/README.md
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 21:02:12.206186 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      709 2023-06-13 21:02:08.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:02:12.202186 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:02:12.202186 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/src/echofish_aws_raw_to_zarr_lambda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 21:00:58.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/src/echofish_aws_raw_to_zarr_lambda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1077 2023-06-13 21:00:58.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/src/echofish_aws_raw_to_zarr_lambda/dynamo_operations.py
+-rw-r--r--   0 root         (0) root         (0)     9684 2023-06-13 21:00:58.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/src/echofish_aws_raw_to_zarr_lambda/lambda_executor.py
+-rw-r--r--   0 root         (0) root         (0)      951 2023-06-13 21:00:58.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/src/echofish_aws_raw_to_zarr_lambda/lambda_handler.py
+-rw-r--r--   0 root         (0) root         (0)     1421 2023-06-13 21:00:58.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/src/echofish_aws_raw_to_zarr_lambda/s3_operations.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 21:02:12.206186 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/src/echofish_aws_raw_to_zarr_lambda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2462 2023-06-13 21:02:12.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      587 2023-06-13 21:02:12.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/src/echofish_aws_raw_to_zarr_lambda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 21:02:12.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/src/echofish_aws_raw_to_zarr_lambda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      127 2023-06-13 21:02:12.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/src/echofish_aws_raw_to_zarr_lambda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-13 21:02:12.000000 echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/src/echofish_aws_raw_to_zarr_lambda.egg-info/top_level.txt
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/LICENSE` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/LICENSE`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230606211113
+Version: 1.0.0.dev20230613210103
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/README.md` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/README.md`

 * *Files identical despite different names*

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/setup.py` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   long_description = fh.read()
 
 with open('requirements.txt') as f:
   requirements = f.read().splitlines()
 
 setuptools.setup(
   name="echofish-aws-raw-to-zarr-lambda",
-  version="1.0.0.dev20230606211113",
+  version="1.0.0.dev20230613210103",
   description="",
   long_description=long_description,
   long_description_content_type="text/markdown",
   url="https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda",
   package_dir={'': 'src'},
   packages=setuptools.find_packages('src'),
   classifiers=[
```

### Comparing `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230606211113/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO` & `echofish-aws-raw-to-zarr-lambda-1.0.0.dev20230613210103/src/echofish_aws_raw_to_zarr_lambda.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: echofish-aws-raw-to-zarr-lambda
-Version: 1.0.0.dev20230606211113
+Version: 1.0.0.dev20230613210103
 Home-page: https://github.com/ci-cmg/echofish-aws-raw-to-zarr-lambda
 Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

