# Comparing `tmp/scanoss-1.5.1.tar.gz` & `tmp/scanoss-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scanoss-1.5.1.tar", last modified: Fri Apr 21 12:28:02 2023, max compression
+gzip compressed data, was "scanoss-1.5.2.tar", last modified: Tue Jun 13 11:04:41 2023, max compression
```

## Comparing `scanoss-1.5.1.tar` & `scanoss-1.5.2.tar`

### file list

```diff
@@ -1,72 +1,72 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-04-21 12:27:38.000000 scanoss-1.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-04-21 12:27:38.000000 scanoss-1.5.1/PACKAGE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-21 12:28:02.444543 scanoss-1.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-04-21 12:27:38.000000 scanoss-1.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-04-21 12:27:38.000000 scanoss-1.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-21 12:28:02.444543 scanoss-1.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.436543 scanoss-1.5.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.440543 scanoss-1.5.1/src/scanoss/
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.440543 scanoss-1.5.1/src/scanoss/api/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/common/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/common/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/common/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/common/v2/scanoss_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/common/v2/scanoss_common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/components/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/components/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/components/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/components/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/components/v2/scanoss_components_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.436543 scanoss-1.5.1/src/scanoss/api/cryptography/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/cryptography/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/dependencies/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/dependencies/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/dependencies/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/dependencies/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/scanning/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/scanning/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/scanning/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/scanning/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/vulnerabilities/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/vulnerabilities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/api/vulnerabilities/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/vulnerabilities/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)    33773 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/csvoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/cyclonedx.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.444543 scanoss-1.5.1/src/scanoss/data/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-21 12:27:51.000000 scanoss-1.5.1/src/scanoss/data/build_date.txt
--rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/data/spdx-exceptions.json
--rw-r--r--   0 runner    (1001) docker     (123)   228794 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/data/spdx-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/filecount.py
--rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/scancodedeps.py
--rw-r--r--   0 runner    (1001) docker     (123)    41124 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/scanner.py
--rw-r--r--   0 runner    (1001) docker     (123)    12641 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/scanossapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/scanossbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/scanossgrpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/scantype.py
--rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/spdxlite.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/threadeddependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/threadedscanning.py
--rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-04-21 12:27:38.000000 scanoss-1.5.1/src/scanoss/winnowing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:28:02.440543 scanoss-1.5.1/src/scanoss.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-21 12:28:02.000000 scanoss-1.5.1/src/scanoss.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-04-21 12:28:02.000000 scanoss-1.5.1/src/scanoss.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:28:02.000000 scanoss-1.5.1/src/scanoss.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-21 12:28:02.000000 scanoss-1.5.1/src/scanoss.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-21 12:28:02.000000 scanoss-1.5.1/src/scanoss.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 12:28:02.000000 scanoss-1.5.1/src/scanoss.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-06-13 11:04:16.000000 scanoss-1.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-13 11:04:16.000000 scanoss-1.5.2/PACKAGE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-13 11:04:41.213340 scanoss-1.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4606 2023-06-13 11:04:16.000000 scanoss-1.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-06-13 11:04:16.000000 scanoss-1.5.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-06-13 11:04:41.217340 scanoss-1.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.205340 scanoss-1.5.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.209340 scanoss-1.5.2/src/scanoss/
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/common/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/common/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/common/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2158 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/common/v2/scanoss_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/common/v2/scanoss_common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/components/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/components/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/components/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/components/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3971 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/components/v2/scanoss_components_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7040 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.205340 scanoss-1.5.2/src/scanoss/api/cryptography/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/cryptography/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6732 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/dependencies/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/dependencies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/dependencies/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/dependencies/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/scanning/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/scanning/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/scanning/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/scanning/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2800 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/vulnerabilities/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/vulnerabilities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/api/vulnerabilities/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1139 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/vulnerabilities/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3724 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7208 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33722 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5918 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8661 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/csvoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/cyclonedx.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 11:04:29.000000 scanoss-1.5.2/src/scanoss/data/build_date.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17953 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/data/spdx-exceptions.json
+-rw-r--r--   0 runner    (1001) docker     (123)   228794 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/data/spdx-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6660 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/filecount.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/scancodedeps.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41153 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/scanner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12801 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/scanossapi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2319 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/scanossbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13191 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/scanossgrpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/scantype.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15441 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/spdxlite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/threadeddependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9387 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/threadedscanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12219 2023-06-13 11:04:16.000000 scanoss-1.5.2/src/scanoss/winnowing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:04:41.213340 scanoss-1.5.2/src/scanoss.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-13 11:04:41.000000 scanoss-1.5.2/src/scanoss.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1936 2023-06-13 11:04:41.000000 scanoss-1.5.2/src/scanoss.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:04:41.000000 scanoss-1.5.2/src/scanoss.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 11:04:41.000000 scanoss-1.5.2/src/scanoss.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-06-13 11:04:41.000000 scanoss-1.5.2/src/scanoss.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 11:04:41.000000 scanoss-1.5.2/src/scanoss.egg-info/top_level.txt
```

### Comparing `scanoss-1.5.1/LICENSE` & `scanoss-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/PACKAGE.md` & `scanoss-1.5.2/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/PKG-INFO` & `scanoss-1.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanoss
-Version: 1.5.1
+Version: 1.5.2
 Summary: Simple Python library to leverage the SCANOSS APIs
 Home-page: https://scanoss.com
 Author: SCANOSS
 Author-email: info@scanoss.com
 License: MIT
 Project-URL: Source, https://github.com/scanoss/scanoss.py
 Project-URL: Tracker, https://github.com/scanoss/scanoss.py/issues
```

### Comparing `scanoss-1.5.1/README.md` & `scanoss-1.5.2/README.md`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/setup.cfg` & `scanoss-1.5.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/__init__.py` & `scanoss-1.5.2/src/scanoss/api/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,9 +17,7 @@
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
-
-__version__ = '1.5.1'
```

### Comparing `scanoss-1.5.1/src/scanoss/api/__init__.py` & `scanoss-1.5.2/src/scanoss/api/common/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/common/__init__.py` & `scanoss-1.5.2/src/scanoss/api/common/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/common/v2/__init__.py` & `scanoss-1.5.2/src/scanoss/api/components/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/common/v2/scanoss_common_pb2.py` & `scanoss-1.5.2/src/scanoss/api/common/v2/scanoss_common_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/components/__init__.py` & `scanoss-1.5.2/src/scanoss/api/components/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/components/v2/__init__.py` & `scanoss-1.5.2/src/scanoss/api/dependencies/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/components/v2/scanoss_components_pb2.py` & `scanoss-1.5.2/src/scanoss/api/components/v2/scanoss_components_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py` & `scanoss-1.5.2/src/scanoss/api/components/v2/scanoss_components_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py` & `scanoss-1.5.2/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py` & `scanoss-1.5.2/src/scanoss/api/cryptography/v2/scanoss_cryptography_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/dependencies/__init__.py` & `scanoss-1.5.2/src/scanoss/api/dependencies/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/dependencies/v2/__init__.py` & `scanoss-1.5.2/src/scanoss/api/scanning/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py` & `scanoss-1.5.2/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py` & `scanoss-1.5.2/src/scanoss/api/dependencies/v2/scanoss_dependencies_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/scanning/__init__.py` & `scanoss-1.5.2/src/scanoss/api/scanning/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/scanning/v2/__init__.py` & `scanoss-1.5.2/src/scanoss/api/vulnerabilities/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
  SPDX-License-Identifier: MIT
 
-   Copyright (c) 2021, SCANOSS
+   Copyright (c) 2022, SCANOSS
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
```

### Comparing `scanoss-1.5.1/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py` & `scanoss-1.5.2/src/scanoss/api/scanning/v2/scanoss_scanning_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py` & `scanoss-1.5.2/src/scanoss/api/scanning/v2/scanoss_scanning_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/vulnerabilities/__init__.py` & `scanoss-1.5.2/src/scanoss/api/vulnerabilities/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/vulnerabilities/v2/__init__.py` & `scanoss-1.5.2/src/scanoss/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
  SPDX-License-Identifier: MIT
 
-   Copyright (c) 2022, SCANOSS
+   Copyright (c) 2021, SCANOSS
 
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
@@ -17,7 +17,9 @@
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
    THE SOFTWARE.
 """
+
+__version__ = '1.5.2'
```

### Comparing `scanoss-1.5.1/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py` & `scanoss-1.5.2/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py` & `scanoss-1.5.2/src/scanoss/api/vulnerabilities/v2/scanoss_vulnerabilities_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/cli.py` & `scanoss-1.5.2/src/scanoss/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,83 +50,74 @@
     """
     Setup all the command line arguments for processing
     """
     parser = argparse.ArgumentParser(description=f'SCANOSS Python CLI. Ver: {__version__}, License: MIT, Fast Winnowing: {FAST_WINNOWING}')
     parser.add_argument('--version', '-v', action='store_true', help='Display version details')
 
     subparsers = parser.add_subparsers(title='Sub Commands', dest='subparser', description='valid subcommands',
-                                       help='sub-command help'
-                                       )
+                                       help='sub-command help')
     # Sub-command: version
     p_ver = subparsers.add_parser('version', aliases=['ver'],
                                   description=f'Version of SCANOSS CLI: {__version__}', help='SCANOSS version')
     p_ver.set_defaults(func=ver)
 
     # Sub-command: scan
     p_scan = subparsers.add_parser('scan', aliases=['sc'],
                                    description=f'Analyse/scan the given source base: {__version__}',
                                    help='Scan source code')
     p_scan.set_defaults(func=scan)
     p_scan.add_argument('scan_dir', metavar='FILE/DIR', type=str, nargs='?', help='A file or folder to scan')
     p_scan.add_argument('--wfp', '-w',  type=str,
-                        help='Scan a WFP File instead of a folder (optional)'
-                        )
+                        help='Scan a WFP File instead of a folder (optional)')
     p_scan.add_argument('--dep', '-p',  type=str,
-                        help='Use a dependency file instead of a folder (optional)'
-                        )
+                        help='Use a dependency file instead of a folder (optional)')
     p_scan.add_argument('--stdin', '-s', metavar='STDIN-FILENAME',  type=str,
-                        help='Scan the file contents supplied via STDIN (optional)'
-                        )
+                        help='Scan the file contents supplied via STDIN (optional)')
     p_scan.add_argument('--identify', '-i', type=str, help='Scan and identify components in SBOM file')
     p_scan.add_argument('--ignore',   '-n', type=str, help='Ignore components specified in the SBOM file')
     p_scan.add_argument('--output',   '-o', type=str, help='Output result file name (optional - default stdout).')
     p_scan.add_argument('--format',   '-f', type=str, choices=['plain', 'cyclonedx', 'spdxlite', 'csv'],
-                        help='Result output format (optional - default: plain)'
-                        )
+                        help='Result output format (optional - default: plain)')
     p_scan.add_argument('--threads', '-T', type=int, default=10,
-                        help='Number of threads to use while scanning (optional - default 10)'
-                        )
+                        help='Number of threads to use while scanning (optional - default 10)')
     p_scan.add_argument('--flags', '-F', type=int,
                         help='Scanning engine flags (1: disable snippet matching, 2 enable snippet ids, '
                              '4: disable dependencies, 8: disable licenses, 16: disable copyrights,'
                              '32: disable vulnerabilities, 64: disable quality, 128: disable cryptography,'
                              '256: disable best match only, 512: hide identified files, '
                              '1024: enable download_url, 2048: enable GitHub full path, '
-                             '4096: disable extended server stats)'
-                        )
+                             '4096: disable extended server stats)')
     p_scan.add_argument('--skip-snippets', '-S', action='store_true', help='Skip the generation of snippets')
     p_scan.add_argument('--post-size', '-P', type=int, default=64,
-                        help='Number of kilobytes to limit the post to while scanning (optional - default 64)'
-                        )
+                        help='Number of kilobytes to limit the post to while scanning (optional - default 64)')
     p_scan.add_argument('--timeout', '-M', type=int, default=120,
-                        help='Timeout (in seconds) for API communication (optional - default 120)'
-                        )
+                        help='Timeout (in seconds) for API communication (optional - default 120)')
+    p_scan.add_argument('--retry', '-R', type=int, default=5,
+                        help='Retry limit for API communication (optional - default 5)')
     p_scan.add_argument('--no-wfp-output', action='store_true', help='Skip WFP file generation')
     p_scan.add_argument('--all-extensions', action='store_true', help='Scan all file extensions')
     p_scan.add_argument('--all-folders', action='store_true', help='Scan all folders')
     p_scan.add_argument('--all-hidden', action='store_true', help='Scan all hidden files/folders')
-    p_scan.add_argument('--obfuscate', action='store_true', help='Obfuscate fingerprints')
+    p_scan.add_argument('--obfuscate', action='store_true', help='Obfuscate file paths and names')
     p_scan.add_argument('--dependencies', '-D', action='store_true', help='Add Dependency scanning')
     p_scan.add_argument('--dependencies-only', action='store_true', help='Run Dependency scanning only')
     p_scan.add_argument('--sc-command', type=str,
                         help='Scancode command and path if required (optional - default scancode).')
     p_scan.add_argument('--sc-timeout', type=int, default=600,
-                        help='Timeout (in seconds) for scancode to complete (optional - default 600)'
-                        )
+                        help='Timeout (in seconds) for scancode to complete (optional - default 600)')
 
     # Sub-command: fingerprint
     p_wfp = subparsers.add_parser('fingerprint', aliases=['fp', 'wfp'],
                                   description=f'Fingerprint the given source base: {__version__}',
                                   help='Fingerprint source code')
     p_wfp.set_defaults(func=wfp)
     p_wfp.add_argument('scan_dir', metavar='FILE/DIR', type=str, nargs='?',
                        help='A file or folder to scan')
     p_wfp.add_argument('--stdin', '-s', metavar='STDIN-FILENAME',  type=str,
-                        help='Fingerprint the file contents supplied via STDIN (optional)'
-                        )
+                        help='Fingerprint the file contents supplied via STDIN (optional)')
     p_wfp.add_argument('--output', '-o', type=str, help='Output result file name (optional - default stdout).')
     p_wfp.add_argument('--obfuscate', action='store_true', help='Obfuscate fingerprints')
     p_wfp.add_argument('--skip-snippets', '-S', action='store_true', help='Skip the generation of snippets')
     p_wfp.add_argument('--all-extensions', action='store_true', help='Fingerprint all file extensions')
     p_wfp.add_argument('--all-folders', action='store_true', help='Fingerprint all folders')
     p_wfp.add_argument('--all-hidden', action='store_true', help='Fingerprint all hidden files/folders')
 
@@ -222,44 +213,37 @@
                            )
     p_p_proxy.add_argument('--url', required=False, type=str, default="https://osskb.org/api",
                            help='URL to test (default: https://osskb.org/api).')
 
     # Global Scan command options
     for p in [p_scan]:
         p.add_argument('--apiurl', type=str,
-                       help='SCANOSS API URL (optional - default: https://osskb.org/api/scan/direct)'
-                       )
+                       help='SCANOSS API URL (optional - default: https://osskb.org/api/scan/direct)')
         p.add_argument('--ignore-cert-errors', action='store_true', help='Ignore certificate errors')
 
     # Global Scan/GRPC options
     for p in [p_scan, c_crypto]:
         p.add_argument('--key', '-k', type=str,
-                       help='SCANOSS API Key token (optional - not required for default OSSKB URL)'
-                       )
+                       help='SCANOSS API Key token (optional - not required for default OSSKB URL)')
         p.add_argument('--proxy', type=str, help='Proxy URL to use for connections (optional). '
                                                  'Can also use the environment variable "HTTPS_PROXY=<ip>:<port>" '
-                                                 'and "grcp_proxy=<ip>:<port>" for gRPC'
-                       )
+                                                 'and "grcp_proxy=<ip>:<port>" for gRPC')
         p.add_argument('--pac', type=str, help='Proxy auto configuration (optional). '
-                                               'Specify a file, http url or "auto" to try to discover it.'
-                       )
+                                               'Specify a file, http url or "auto" to try to discover it.')
         p.add_argument('--ca-cert', type=str, help='Alternative certificate PEM file (optional). '
                                                    'Can also use the environment variable '
                                                    '"REQUESTS_CA_BUNDLE=/path/to/cacert.pem" and '
-                                                   '"GRPC_DEFAULT_SSL_ROOTS_FILE_PATH=/path/to/cacert.pem" for gRPC'
-                       )
+                                                   '"GRPC_DEFAULT_SSL_ROOTS_FILE_PATH=/path/to/cacert.pem" for gRPC')
 
     # Global GRPC options
     for p in [p_scan, c_crypto]:
         p.add_argument('--api2url', type=str,
-                       help='SCANOSS gRPC API 2.0 URL (optional - default: https://api.osskb.org)'
-                       )
+                       help='SCANOSS gRPC API 2.0 URL (optional - default: https://api.osskb.org)')
         p.add_argument('--grpc-proxy', type=str, help='GRPC Proxy URL to use for connections (optional). '
-                                                       'Can also use the environment variable "grcp_proxy=<ip>:<port>"'
-                       )
+                                                       'Can also use the environment variable "grcp_proxy=<ip>:<port>"')
 
     # Help/Trace command options
     for p in [p_scan, p_wfp, p_dep, p_fc, p_cnv, p_c_loc, p_c_dwnld, p_p_proxy, c_crypto]:
         p.add_argument('--debug', '-d', action='store_true', help='Enable debug messages')
         p.add_argument('--trace', '-t', action='store_true', help='Enable trace messages, including API posts')
         p.add_argument('--quiet', '-q', action='store_true', help='Enable quiet mode')
 
@@ -459,14 +443,16 @@
             print_stderr("Scanning all hidden files/folders...")
         if args.skip_snippets:
             print_stderr("Skipping snippets...")
         if args.post_size != 64:
             print_stderr(f'Changing scanning POST size to: {args.post_size}k...')
         if args.timeout != 120:
             print_stderr(f'Changing scanning POST timeout to: {args.timeout}...')
+        if args.retry != 5:
+            print_stderr(f'Changing scanning POST retry to: {args.retry}...')
         if args.obfuscate:
             print_stderr("Obfuscating file fingerprints...")
         if args.proxy:
             print_stderr(f'Using Proxy {args.proxy}...')
         if args.grpc_proxy:
             print_stderr(f'Using GRPC Proxy {args.grpc_proxy}...')
         if args.pac:
@@ -474,14 +460,16 @@
         if args.ca_cert:
             print_stderr(f'Using Certificate {args.ca_cert}...')
         if flags:
             print_stderr(f'Using flags {flags}...')
     elif not args.quiet:
         if args.timeout < 5:
             print_stderr(f'POST timeout (--timeout) too small: {args.timeout}. Reverting to default.')
+        if args.retry < 0:
+            print_stderr(f'POST retry (--retry) too small: {args.retry}. Reverting to default.')
 
     if not os.access(os.getcwd(), os.W_OK):  # Make sure the current directory is writable. If not disable saving WFP
         print_stderr(f'Warning: Current directory is not writable: {os.getcwd()}')
         args.no_wfp_output = True
     if args.ca_cert and not os.path.exists(args.ca_cert):
         print_stderr(f'Error: Certificate file does not exist: {args.ca_cert}.')
         exit(1)
@@ -492,15 +480,15 @@
                       sbom_path=sbom_path, scan_type=scan_type, scan_output=scan_output, output_format=output_format,
                       flags=flags, nb_threads=args.threads, post_size=args.post_size,
                       timeout=args.timeout, no_wfp_file=args.no_wfp_output, all_extensions=args.all_extensions,
                       all_folders=args.all_folders, hidden_files_folders=args.all_hidden,
                       scan_options=scan_options, sc_timeout=args.sc_timeout, sc_command=args.sc_command,
                       grpc_url=args.api2url, obfuscate=args.obfuscate,
                       ignore_cert_errors=args.ignore_cert_errors, proxy=args.proxy, grpc_proxy=args.grpc_proxy,
-                      pac=pac_file, ca_cert=args.ca_cert
+                      pac=pac_file, ca_cert=args.ca_cert, retry=args.retry
                       )
     if args.wfp:
         if not scanner.is_file_or_snippet_scan():
             print_stderr(f'Error: Cannot specify WFP scanning if file/snippet options are disabled ({scan_options})')
             exit(1)
         if args.threads > 1:
             scanner.scan_wfp_file_threaded(args.wfp)
```

### Comparing `scanoss-1.5.1/src/scanoss/components.py` & `scanoss-1.5.2/src/scanoss/components.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/csvoutput.py` & `scanoss-1.5.2/src/scanoss/csvoutput.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/cyclonedx.py` & `scanoss-1.5.2/src/scanoss/cyclonedx.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/data/spdx-exceptions.json` & `scanoss-1.5.2/src/scanoss/data/spdx-exceptions.json`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/data/spdx-licenses.json` & `scanoss-1.5.2/src/scanoss/data/spdx-licenses.json`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/filecount.py` & `scanoss-1.5.2/src/scanoss/filecount.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/scancodedeps.py` & `scanoss-1.5.2/src/scanoss/scancodedeps.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/scanner.py` & `scanoss-1.5.2/src/scanoss/scanner.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
     def __init__(self, wfp: str = None, scan_output: str = None, output_format: str = 'plain',
                  debug: bool = False, trace: bool = False, quiet: bool = False, api_key: str = None, url: str = None,
                  sbom_path: str = None, scan_type: str = None, flags: str = None, nb_threads: int = 5,
                  post_size: int = 64, timeout: int = 120, no_wfp_file: bool = False,
                  all_extensions: bool = False, all_folders: bool = False, hidden_files_folders: bool = False,
                  scan_options: int = 7, sc_timeout: int = 600, sc_command: str = None, grpc_url: str = None,
                  obfuscate: bool = False, ignore_cert_errors: bool = False, proxy: str = None, grpc_proxy: str = None,
-                 ca_cert: str = None, pac: PACFile = None
+                 ca_cert: str = None, pac: PACFile = None, retry: int = 5
                  ):
         """
         Initialise scanning class, including Winnowing, ScanossApi and ThreadedScanning
         """
         super().__init__(debug, trace, quiet)
         self.wfp = wfp if wfp else "scanner_output.wfp"
         self.scan_output = scan_output
@@ -121,15 +121,15 @@
 
         self.winnowing = Winnowing(debug=debug, quiet=quiet, skip_snippets=self._skip_snippets,
                                    all_extensions=all_extensions, obfuscate=obfuscate
                                    )
         self.scanoss_api = ScanossApi(debug=debug, trace=trace, quiet=quiet, api_key=api_key, url=url,
                                       sbom_path=sbom_path, scan_type=scan_type, flags=flags, timeout=timeout,
                                       ver_details=ver_details, ignore_cert_errors=ignore_cert_errors,
-                                      proxy=proxy, ca_cert=ca_cert, pac=pac
+                                      proxy=proxy, ca_cert=ca_cert, pac=pac, retry=retry
                                       )
         sc_deps = ScancodeDeps(debug=debug, quiet=quiet, trace=trace, timeout=sc_timeout, sc_command=sc_command)
         grpc_api = ScanossGrpc(url=grpc_url, debug=debug, quiet=quiet, trace=trace, api_key=api_key,
                                ver_details=ver_details, ca_cert=ca_cert, proxy=proxy, pac=pac, grpc_proxy=grpc_proxy
                                )
         self.threaded_deps = ThreadedDependencies(sc_deps, grpc_api, debug=debug, quiet=quiet, trace=trace)
         self.nb_threads = nb_threads
```

### Comparing `scanoss-1.5.1/src/scanoss/scanossapi.py` & `scanoss-1.5.2/src/scanoss/scanossapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     ScanOSS REST API client class
     Currently support posting scan requests to the SCANOSS streaming API
     """
 
     def __init__(self, scan_type: str = None, sbom_path: str = None, scan_format: str = None, flags: str = None,
                  url: str = None, api_key: str = None, debug: bool = False, trace: bool = False, quiet: bool = False,
                  timeout: int = 120, ver_details: str = None, ignore_cert_errors: bool = False,
-                 proxy: str = None, ca_cert: str = None, pac: PACFile = None):
+                 proxy: str = None, ca_cert: str = None, pac: PACFile = None, retry: int = 5):
         """
         Initialise the SCANOSS API
         :param scan_type: Scan type (default identify)
         :param sbom_path: Input SBOM file to match scan type (default None)
         :param scan_format: Scan format (default plain)
         :param flags: Scanning flags (default None)
         :param url: API URL (default https://osskb.org/api/scan/direct)
@@ -78,14 +78,15 @@
         if self.api_key and not url and not os.environ.get("SCANOSS_SCAN_URL"):
             self.url = DEFAULT_URL2  # API key specific and no alternative URL, so use the default premium
         self.scan_type = scan_type
         self.scan_format = scan_format if scan_format else 'plain'
         self.sbom_path = sbom_path
         self.flags = flags
         self.timeout = timeout if timeout > 5 else 120
+        self.retry_limit = retry if retry >= 0 else 5
         self.ignore_cert_errors = ignore_cert_errors
         self.headers = {}
         if ver_details:
             self.headers['x-scanoss-client'] = ver_details
         if self.api_key:
             self.headers['X-Session'] = self.api_key
             self.headers['x-api-key'] = self.api_key
@@ -145,56 +146,56 @@
         if context:
             form_data['context'] = context
         scan_files = {'file': ("%s.wfp" % request_id, wfp)}
         headers = self.headers
         headers['x-request-id'] = request_id  # send a unique request id for each post
         r = None
         retry = 0  # Add some retry logic to cater for timeouts, etc.
-        while retry <= 5:
+        while retry <= self.retry_limit:
             retry += 1
             try:
                 r = None
                 r = self.session.post(self.url, files=scan_files, data=form_data, headers=self.headers,
                                       timeout=self.timeout
                                       )
                 # r = requests.post(self.url, files=scan_files, data=form_data, headers=self.headers,
                 #                   timeout=self.timeout, verify=self.verify, proxies=self.proxies
                 #                   )
             except (requests.exceptions.SSLError, requests.exceptions.ProxyError) as e:
                 self.print_stderr(f'ERROR: Exception ({e.__class__.__name__}) POSTing data - {e}.')
                 raise Exception(f"ERROR: The SCANOSS API request failed for {self.url}") from e
             except (requests.exceptions.Timeout, requests.exceptions.ConnectionError) as e:
-                if retry > 5:  # Timed out 5 or more times, fail
+                if retry > self.retry_limit:  # Timed out retry_limit or more times, fail
                     self.print_stderr(f'ERROR: {e.__class__.__name__} POSTing data ({request_id}) - {e}: {scan_files}')
                     raise Exception(f"ERROR: The SCANOSS API request timed out ({e.__class__.__name__}) for"
                                     f" {self.url}") from e
                 else:
                     self.print_stderr(f'Warning: {e.__class__.__name__} communicating with {self.url}. Retrying...')
                     time.sleep(5)
             except Exception as e:
                 self.print_stderr(f'ERROR: Exception ({e.__class__.__name__}) POSTing data ({request_id}) - {e}:'
                                   f' {scan_files}')
                 raise Exception(f"ERROR: The SCANOSS API request failed for {self.url}") from e
             else:
                 if r is None:
-                    if retry > 5:  # No response 5 or more times, fail
+                    if retry > self.retry_limit:  # No response retry_limit or more times, fail
                         self.save_bad_req_wfp(scan_files, request_id, scan_id)
                         raise Exception(f"ERROR: The SCANOSS API request ({request_id}) response object is empty "
                                         f"for {self.url}")
                     else:
                         self.print_stderr(f'Warning: No response received from {self.url}. Retrying...')
                         time.sleep(5)
                 elif r.status_code == 503:  # Service limits have most likely been reached
                     self.print_stderr(f'ERROR: SCANOSS API rejected the scan request ({request_id}) due to '
                                       f'service limits being exceeded')
                     self.print_stderr(f'ERROR: Details: {r.text.strip()}')
                     raise Exception(f"ERROR: {r.status_code} - The SCANOSS API request ({request_id}) rejected "
                                     f"for {self.url} due to service limits being exceeded.")
                 elif r.status_code >= 400:
-                    if retry > 5:  # No response 5 or more times, fail
+                    if retry > self.retry_limit:  # No response retry_limit or more times, fail
                         self.save_bad_req_wfp(scan_files, request_id, scan_id)
                         raise Exception(
                             f"ERROR: The SCANOSS API returned the following error: HTTP {r.status_code}, "
                             f"{r.text.strip()}")
                     else:
                         self.save_bad_req_wfp(scan_files, request_id, scan_id)
                         self.print_stderr(f'Warning: Error response code {r.status_code} ({r.text.strip()}) from '
```

### Comparing `scanoss-1.5.1/src/scanoss/scanossbase.py` & `scanoss-1.5.2/src/scanoss/scanossbase.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/scanossgrpc.py` & `scanoss-1.5.2/src/scanoss/scanossgrpc.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/scantype.py` & `scanoss-1.5.2/src/scanoss/scantype.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/spdxlite.py` & `scanoss-1.5.2/src/scanoss/spdxlite.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/threadeddependencies.py` & `scanoss-1.5.2/src/scanoss/threadeddependencies.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/threadedscanning.py` & `scanoss-1.5.2/src/scanoss/threadedscanning.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss/winnowing.py` & `scanoss-1.5.2/src/scanoss/winnowing.py`

 * *Files identical despite different names*

### Comparing `scanoss-1.5.1/src/scanoss.egg-info/PKG-INFO` & `scanoss-1.5.2/src/scanoss.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scanoss
-Version: 1.5.1
+Version: 1.5.2
 Summary: Simple Python library to leverage the SCANOSS APIs
 Home-page: https://scanoss.com
 Author: SCANOSS
 Author-email: info@scanoss.com
 License: MIT
 Project-URL: Source, https://github.com/scanoss/scanoss.py
 Project-URL: Tracker, https://github.com/scanoss/scanoss.py/issues
```

### Comparing `scanoss-1.5.1/src/scanoss.egg-info/SOURCES.txt` & `scanoss-1.5.2/src/scanoss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

