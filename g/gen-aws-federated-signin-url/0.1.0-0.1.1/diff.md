# Comparing `tmp/gen-aws-federated-signin-url-0.1.0.tar.gz` & `tmp/gen-aws-federated-signin-url-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gen-aws-federated-signin-url-0.1.0.tar", last modified: Tue Jun 13 06:49:01 2023, max compression
+gzip compressed data, was "gen-aws-federated-signin-url-0.1.1.tar", last modified: Tue Jun 13 07:04:46 2023, max compression
```

## Comparing `gen-aws-federated-signin-url-0.1.0.tar` & `gen-aws-federated-signin-url-0.1.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 youyo      (501) staff       (20)        0 2023-06-13 06:49:01.827211 gen-aws-federated-signin-url-0.1.0/
-drwxr-xr-x   0 youyo      (501) staff       (20)        0 2023-06-13 06:49:01.801083 gen-aws-federated-signin-url-0.1.0/.github/
-drwxr-xr-x   0 youyo      (501) staff       (20)        0 2023-06-13 06:49:01.817583 gen-aws-federated-signin-url-0.1.0/.github/workflows/
--rw-r--r--   0 youyo      (501) staff       (20)      708 2023-05-08 16:24:55.000000 gen-aws-federated-signin-url-0.1.0/.github/workflows/publish.yaml
--rw-r--r--   0 youyo      (501) staff       (20)      135 2023-06-04 02:53:32.000000 gen-aws-federated-signin-url-0.1.0/.gitignore
--rw-r--r--   0 youyo      (501) staff       (20)       14 2023-05-08 14:27:19.000000 gen-aws-federated-signin-url-0.1.0/.tool-versions
--rw-r--r--   0 youyo      (501) staff       (20)     1090 2023-05-08 14:28:29.000000 gen-aws-federated-signin-url-0.1.0/LICENSE.txt
--rw-r--r--   0 youyo      (501) staff       (20)      223 2023-06-13 06:36:02.000000 gen-aws-federated-signin-url-0.1.0/Makefile
--rw-r--r--   0 youyo      (501) staff       (20)      622 2023-06-13 06:49:01.826855 gen-aws-federated-signin-url-0.1.0/PKG-INFO
--rw-r--r--   0 youyo      (501) staff       (20)      363 2023-06-13 06:39:04.000000 gen-aws-federated-signin-url-0.1.0/README.md
--rw-r--r--   0 youyo      (501) staff       (20)      608 2023-06-13 06:35:16.000000 gen-aws-federated-signin-url-0.1.0/pyproject.toml
--rw-r--r--   0 youyo      (501) staff       (20)       38 2023-06-13 06:49:01.827280 gen-aws-federated-signin-url-0.1.0/setup.cfg
-drwxr-xr-x   0 youyo      (501) staff       (20)        0 2023-06-13 06:49:01.801775 gen-aws-federated-signin-url-0.1.0/src/
-drwxr-xr-x   0 youyo      (501) staff       (20)        0 2023-06-13 06:49:01.821127 gen-aws-federated-signin-url-0.1.0/src/gen_aws_federated_signin_url/
--rw-r--r--   0 youyo      (501) staff       (20)      105 2023-06-13 06:06:33.000000 gen-aws-federated-signin-url-0.1.0/src/gen_aws_federated_signin_url/__init__.py
--rw-r--r--   0 youyo      (501) staff       (20)      160 2023-06-13 06:49:01.000000 gen-aws-federated-signin-url-0.1.0/src/gen_aws_federated_signin_url/_version.py
--rw-r--r--   0 youyo      (501) staff       (20)     2084 2023-06-13 06:34:44.000000 gen-aws-federated-signin-url-0.1.0/src/gen_aws_federated_signin_url/gen_aws_federated_signin_url.py
-drwxr-xr-x   0 youyo      (501) staff       (20)        0 2023-06-13 06:49:01.825804 gen-aws-federated-signin-url-0.1.0/src/gen_aws_federated_signin_url.egg-info/
--rw-r--r--   0 youyo      (501) staff       (20)      622 2023-06-13 06:49:01.000000 gen-aws-federated-signin-url-0.1.0/src/gen_aws_federated_signin_url.egg-info/PKG-INFO
--rw-r--r--   0 youyo      (501) staff       (20)      536 2023-06-13 06:49:01.000000 gen-aws-federated-signin-url-0.1.0/src/gen_aws_federated_signin_url.egg-info/SOURCES.txt
--rw-r--r--   0 youyo      (501) staff       (20)        1 2023-06-13 06:49:01.000000 gen-aws-federated-signin-url-0.1.0/src/gen_aws_federated_signin_url.egg-info/dependency_links.txt
--rw-r--r--   0 youyo      (501) staff       (20)       33 2023-06-13 06:49:01.000000 gen-aws-federated-signin-url-0.1.0/src/gen_aws_federated_signin_url.egg-info/requires.txt
--rw-r--r--   0 youyo      (501) staff       (20)       29 2023-06-13 06:49:01.000000 gen-aws-federated-signin-url-0.1.0/src/gen_aws_federated_signin_url.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:46.275691 gen-aws-federated-signin-url-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:46.271691 gen-aws-federated-signin-url-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:46.275691 gen-aws-federated-signin-url-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      708 2023-06-13 07:04:30.000000 gen-aws-federated-signin-url-0.1.1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-06-13 07:04:30.000000 gen-aws-federated-signin-url-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 07:04:30.000000 gen-aws-federated-signin-url-0.1.1/.tool-versions
+-rw-r--r--   0 runner    (1001) docker     (123)     1090 2023-06-13 07:04:30.000000 gen-aws-federated-signin-url-0.1.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-06-13 07:04:30.000000 gen-aws-federated-signin-url-0.1.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 07:04:46.275691 gen-aws-federated-signin-url-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-06-13 07:04:30.000000 gen-aws-federated-signin-url-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-13 07:04:30.000000 gen-aws-federated-signin-url-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:04:46.275691 gen-aws-federated-signin-url-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:46.271691 gen-aws-federated-signin-url-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:46.275691 gen-aws-federated-signin-url-0.1.1/src/gen_aws_federated_signin_url/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-13 07:04:30.000000 gen-aws-federated-signin-url-0.1.1/src/gen_aws_federated_signin_url/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 07:04:46.000000 gen-aws-federated-signin-url-0.1.1/src/gen_aws_federated_signin_url/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-13 07:04:30.000000 gen-aws-federated-signin-url-0.1.1/src/gen_aws_federated_signin_url/gen_aws_federated_signin_url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:46.275691 gen-aws-federated-signin-url-0.1.1/src/gen_aws_federated_signin_url.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 07:04:46.000000 gen-aws-federated-signin-url-0.1.1/src/gen_aws_federated_signin_url.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-13 07:04:46.000000 gen-aws-federated-signin-url-0.1.1/src/gen_aws_federated_signin_url.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:04:46.000000 gen-aws-federated-signin-url-0.1.1/src/gen_aws_federated_signin_url.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 07:04:46.000000 gen-aws-federated-signin-url-0.1.1/src/gen_aws_federated_signin_url.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-13 07:04:46.000000 gen-aws-federated-signin-url-0.1.1/src/gen_aws_federated_signin_url.egg-info/top_level.txt
```

### Comparing `gen-aws-federated-signin-url-0.1.0/.github/workflows/publish.yaml` & `gen-aws-federated-signin-url-0.1.1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `gen-aws-federated-signin-url-0.1.0/LICENSE.txt` & `gen-aws-federated-signin-url-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gen-aws-federated-signin-url-0.1.0/PKG-INFO` & `gen-aws-federated-signin-url-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-aws-federated-signin-url
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate AWS Federated Signin URL
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # gen_aws_federated_signin_url
```

### Comparing `gen-aws-federated-signin-url-0.1.0/pyproject.toml` & `gen-aws-federated-signin-url-0.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gen-aws-federated-signin-url-0.1.0/src/gen_aws_federated_signin_url/gen_aws_federated_signin_url.py` & `gen-aws-federated-signin-url-0.1.1/src/gen_aws_federated_signin_url/gen_aws_federated_signin_url.py`

 * *Files identical despite different names*

### Comparing `gen-aws-federated-signin-url-0.1.0/src/gen_aws_federated_signin_url.egg-info/PKG-INFO` & `gen-aws-federated-signin-url-0.1.1/src/gen_aws_federated_signin_url.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gen-aws-federated-signin-url
-Version: 0.1.0
+Version: 0.1.1
 Summary: Generate AWS Federated Signin URL
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10.0
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # gen_aws_federated_signin_url
```

### Comparing `gen-aws-federated-signin-url-0.1.0/src/gen_aws_federated_signin_url.egg-info/SOURCES.txt` & `gen-aws-federated-signin-url-0.1.1/src/gen_aws_federated_signin_url.egg-info/SOURCES.txt`

 * *Files identical despite different names*

