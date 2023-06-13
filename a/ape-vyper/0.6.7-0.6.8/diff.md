# Comparing `tmp/ape-vyper-0.6.7.tar.gz` & `tmp/ape-vyper-0.6.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ape-vyper-0.6.7.tar", last modified: Fri May 26 01:41:09 2023, max compression
+gzip compressed data, was "ape-vyper-0.6.8.tar", last modified: Tue Jun 13 16:43:43 2023, max compression
```

## Comparing `ape-vyper-0.6.7.tar` & `ape-vyper-0.6.8.tar`

### file list

```diff
@@ -1,65 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.192096 ape-vyper-0.6.7/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.192096 ape-vyper-0.6.7/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/ISSUE_TEMPLATE/work-item.md
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (123)      651 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/release-drafter.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.192096 ape-vyper-0.6.7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/workflows/commitlint.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/workflows/draft.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      616 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/workflows/prtitle.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3402 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.github/workflows/test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.mdformat.toml
--rw-r--r--   0 runner    (1001) docker     (123)      796 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/ape_vyper/
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/ape_vyper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27699 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/ape_vyper/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3818 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/ape_vyper/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-26 01:41:08.000000 ape-vyper-0.6.7/ape_vyper/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/ape_vyper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-26 01:41:09.000000 ape-vyper-0.6.7/ape_vyper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-26 01:41:09.000000 ape-vyper-0.6.7/ape_vyper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:41:09.000000 ape-vyper-0.6.7/ape_vyper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 01:41:09.000000 ape-vyper-0.6.7/ape_vyper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-05-26 01:41:09.000000 ape-vyper-0.6.7/ape_vyper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-26 01:41:09.000000 ape-vyper-0.6.7/ape_vyper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      943 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      101 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.192096 ape-vyper-0.6.7/tests/ExampleDependency/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/tests/ExampleDependency/contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/ExampleDependency/contracts/Dependency.vy
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      420 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/ape-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3184 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.192096 ape-vyper-0.6.7/tests/contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/tests/contracts/failing_contracts/
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/failing_contracts/contract_undeclared_variable.vy
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/failing_contracts/contract_unknown_pragma.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/tests/contracts/passing_contracts/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/contract.vy
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/contract_37.vy
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/contract_no_pragma.vy
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/contract_with_dev_messages.vy
--rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/erc20.vy
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 01:41:09.196096 ape-vyper-0.6.7/tests/contracts/passing_contracts/interfaces/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/interfaces/IFace.vy
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/interfaces/IFace2.vy
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/interfaces/IRegistry.vy
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/older_version.vy
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/registry.vy
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/traceback_contract.vy
--rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/use_iface.vy
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/contracts/passing_contracts/use_iface2.vy
--rw-r--r--   0 runner    (1001) docker     (123)    12531 2023-05-26 01:40:03.000000 ape-vyper-0.6.7/tests/test_compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.696535 ape-vyper-0.6.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.696535 ape-vyper-0.6.8/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1268 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/ISSUE_TEMPLATE/work-item.md
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      651 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/release-drafter.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.696535 ape-vyper-0.6.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/workflows/commitlint.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/workflows/draft.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/workflows/prtitle.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3410 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.github/workflows/test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.mdformat.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.696535 ape-vyper-0.6.8/ape_vyper/
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/ape_vyper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30501 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/ape_vyper/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/ape_vyper/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 16:43:43.000000 ape-vyper-0.6.8/ape_vyper/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.696535 ape-vyper-0.6.8/ape_vyper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-13 16:43:43.000000 ape-vyper-0.6.8/ape_vyper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2009 2023-06-13 16:43:43.000000 ape-vyper-0.6.8/ape_vyper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:43:43.000000 ape-vyper-0.6.8/ape_vyper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:43:43.000000 ape-vyper-0.6.8/ape_vyper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-13 16:43:43.000000 ape-vyper-0.6.8/ape_vyper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 16:43:43.000000 ape-vyper-0.6.8/ape_vyper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      101 2023-06-13 16:43:43.704535 ape-vyper-0.6.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.692535 ape-vyper-0.6.8/tests/ExampleDependency/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/tests/ExampleDependency/contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/ExampleDependency/contracts/Dependency.vy
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/ape-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4105 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.692535 ape-vyper-0.6.8/tests/contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/tests/contracts/failing_contracts/
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/failing_contracts/contract_undeclared_variable.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/failing_contracts/contract_unknown_pragma.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/tests/contracts/passing_contracts/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/tests/contracts/passing_contracts/DirectoryWithExtension.vy/
+-rw-r--r--   0 runner    (1001) docker     (123)      157 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/contract.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/contract_37.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/contract_no_pragma.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/contract_with_dev_messages.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     5231 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/erc20.vy
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:43:43.700535 ape-vyper-0.6.8/tests/contracts/passing_contracts/interfaces/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/interfaces/IFace.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/interfaces/IFace2.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/interfaces/IRegistry_037.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/interfaces/IRegistry_039.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/non_payable_default.vy
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/older_version.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/payable_default.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/registry_037.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/registry_039.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/traceback_contract_037.vy
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/traceback_contract_039.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/use_iface.vy
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/contracts/passing_contracts/use_iface2.vy
+-rw-r--r--   0 runner    (1001) docker     (123)    15085 2023-06-13 16:42:24.000000 ape-vyper-0.6.8/tests/test_compiler.py
```

### Comparing `ape-vyper-0.6.7/.github/ISSUE_TEMPLATE/bug.md` & `ape-vyper-0.6.8/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.7/.github/ISSUE_TEMPLATE/feature.md` & `ape-vyper-0.6.8/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.7/.github/ISSUE_TEMPLATE/work-item.md` & `ape-vyper-0.6.8/.github/ISSUE_TEMPLATE/work-item.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.7/.github/release-drafter.yml` & `ape-vyper-0.6.8/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.7/.github/workflows/commitlint.yaml` & `ape-vyper-0.6.8/.github/workflows/commitlint.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.7/.github/workflows/prtitle.yaml` & `ape-vyper-0.6.8/.github/workflows/prtitle.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.7/.github/workflows/publish.yaml` & `ape-vyper-0.6.8/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.7/.github/workflows/test.yaml` & `ape-vyper-0.6.8/.github/workflows/test.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -62,18 +62,18 @@
 
     functional:
         runs-on: ${{ matrix.os }}
 
         strategy:
             matrix:
                 os: [ubuntu-latest, macos-latest]   # eventually add `windows-latest`
-                python-version: [3.8, 3.9, "3.10"]
+                python-version: [3.8, 3.9, "3.10", "3.11"]
 
         env:
-          GETH_VERSION: 1.11.5
+          GETH_VERSION: 1.12.0
 
         steps:
         - uses: actions/checkout@v3
 
         - name: Setup Python
           uses: actions/setup-python@v4
           with:
```

### Comparing `ape-vyper-0.6.7/.gitignore` & `ape-vyper-0.6.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.7/.pre-commit-config.yaml` & `ape-vyper-0.6.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.7/CONTRIBUTING.md` & `ape-vyper-0.6.8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.7/LICENSE` & `ape-vyper-0.6.8/LICENSE`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.7/PKG-INFO` & `ape-vyper-0.6.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.6.7
+Version: 0.6.8
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,15 @@
 
 # Quick Start
 
 Ape compiler plugin around [VVM](https://github.com/vyperlang/vvm)
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -91,11 +91,11 @@
   import_remapping:
     - "voting=VyperVoting@v0.3.8"
 ```
 
 Import the voting contract types like this:
 
 ```python
-# @version 0.3.8
+# @version 0.3.9
 
 import voting.ballot as ballot
 ```
```

### Comparing `ape-vyper-0.6.7/README.md` & `ape-vyper-0.6.8/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Quick Start
 
 Ape compiler plugin around [VVM](https://github.com/vyperlang/vvm)
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -63,11 +63,11 @@
   import_remapping:
     - "voting=VyperVoting@v0.3.8"
 ```
 
 Import the voting contract types like this:
 
 ```python
-# @version 0.3.8
+# @version 0.3.9
 
 import voting.ballot as ballot
 ```
```

### Comparing `ape-vyper-0.6.7/ape_vyper/compiler.py` & `ape-vyper-0.6.8/ape_vyper/compiler.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import vvm  # type: ignore
 from ape.api import PluginConfig
 from ape.api.compiler import CompilerAPI
 from ape.exceptions import ContractLogicError
 from ape.types import ContractType, SourceTraceback, TraceFrame
 from ape.utils import cached_property, get_relative_path
 from eth_utils import is_0x_prefixed
-from ethpm_types import ASTNode, HexBytes, PackageManifest, PCMap
+from ethpm_types import ASTNode, HexBytes, PackageManifest, PCMap, SourceMapItem
 from ethpm_types.ast import ASTClassification
 from ethpm_types.contract_type import SourceMap
 from ethpm_types.source import ContractSource, Function
 from evm_trace.enums import CALL_OPCODES
 from semantic_version import NpmSpec, Version  # type: ignore
 from vvm.exceptions import VyperError  # type: ignore
 
@@ -278,90 +278,19 @@
                         ):
                             function_offsets.append((node.lineno, node.end_lineno))
 
                     bytecode = output["evm"]["deployedBytecode"]
                     opcodes = bytecode["opcodes"].split(" ")
                     compressed_src_map = SourceMap(__root__=bytecode["sourceMap"])
                     src_map = list(compressed_src_map.parse())[1:]
-                    pc = 0
-                    pc_map_list: List[Tuple[int, Dict[str, Optional[Any]]]] = []
-                    last_value = None
-                    revert_pc = -1
-                    if _has_empty_revert(opcodes):
-                        # Starting in vyper 0.2.14, reverts without a reason string are optimized
-                        # with a jump to the "end" of the bytecode.
-                        revert_pc = (
-                            len(opcodes)
-                            + sum(int(i[4:]) - 1 for i in opcodes if i.startswith("PUSH"))
-                            - _EMPTY_REVERT_OFFSET
-                        )
-
-                    processed_opcodes = []
-
-                    # There is only 1 non-payable check and it happens early in the bytecode.
-                    non_payable_check_found = False
-
-                    while src_map and opcodes:
-                        src = src_map.pop(0)
-                        op = opcodes.pop(0)
-                        processed_opcodes.append(op)
-                        pc += 1
-
-                        # Detect immutable state member load.
-                        # If this is the case, ignore increasing pc by push size.
-                        is_code_copy = len(opcodes) > 5 and opcodes[5] == "CODECOPY"
-
-                        if not is_code_copy and opcodes and is_0x_prefixed(opcodes[0]):
-                            last_value = int(opcodes.pop(0), 16)
-                            # Add the push number, e.g. PUSH1 adds `1`.
-                            num_pushed = int(op[4:])
-                            pc += num_pushed
-
-                        # Add content PC item.
-                        # Also check for compiler runtime error handling.
-                        # Runtime error locations are marked in the PCMap for further analysis.
-                        if src.start is not None and src.length is not None:
-                            stmt = ast.get_node(src)
-                            if stmt:
-                                # Add located item.
-                                line_nos = list(stmt.line_numbers)
-                                item: Dict = {"location": line_nos}
-                                is_revert_jump = _is_revert_jump(op, last_value, revert_pc)
-                                if op == "REVERT" or is_revert_jump:
-                                    dev = None
-                                    if stmt.ast_type in ("AugAssign", "BinOp"):
-                                        # SafeMath
-                                        for node in stmt.children:
-                                            dev = RuntimeErrorType.from_operator(node.ast_type)
-                                            if dev:
-                                                break
-
-                                    elif stmt.ast_type == "Subscript":
-                                        dev = RuntimeErrorType.INDEX_OUT_OF_RANGE
-
-                                    if dev:
-                                        val = f"dev: {dev.value}"
-                                        if is_revert_jump and len(pc_map_list) >= 1:
-                                            pc_map_list[-1][1]["dev"] = val
-                                        else:
-                                            item["dev"] = val
-
-                                pc_map_list.append((pc, item))
-
-                        elif (
-                            not non_payable_check_found
-                            and len(opcodes) >= 3
-                            and op == "CALLVALUE"
-                            and "PUSH" in opcodes[0]
-                            and is_0x_prefixed(opcodes[1])
-                            and _is_revert_jump(opcodes[2], int(opcodes[1], 16), revert_pc)
-                        ):
-                            item = {"dev": _NON_PAYABLE_STR, "location": None}
-                            pc_map_list.append((pc, item))
-                            non_payable_check_found = True
+
+                    if vyper_version < Version("0.3.8"):
+                        pcmap = _get_legacy_pcmap(ast, src_map, opcodes)
+                    else:
+                        pcmap = _get_pcmap(bytecode, src_map, opcodes)
 
                     # Find content-specified dev messages.
                     dev_messages = {}
                     for line_no, line in content.items():
                         if match := re.search(DEV_MSG_PATTERN, line):
                             dev_messages[line_no] = match.group(1).strip()
 
@@ -369,15 +298,15 @@
                         ast=ast,
                         contractName=name,
                         sourceId=source_id,
                         deploymentBytecode={"bytecode": output["evm"]["bytecode"]["object"]},
                         runtimeBytecode={"bytecode": bytecode["object"]},
                         abi=output["abi"],
                         sourcemap=compressed_src_map,
-                        pcmap=PCMap.parse_obj(dict(pc_map_list)),
+                        pcmap=pcmap,
                         userdoc=output["userdoc"],
                         devdoc=output["devdoc"],
                         dev_messages=dev_messages,
                     )
                     contract_types.append(contract_type)
 
         return contract_types
@@ -450,16 +379,16 @@
                 continue
 
             version_settings: Dict = {"optimize": True}
             path_args = {
                 str(get_relative_path(p.absolute(), contracts_path)): p for p in source_paths
             }
             version_settings["outputSelection"] = {s: ["*"] for s in path_args}
-            if data["evm_version"]:
-                version_settings["evmVersion"] = data["evm_version"]
+            if evm_version := data.get("evm_version"):
+                version_settings["evmVersion"] = evm_version
 
             settings[version] = version_settings
 
         return settings
 
     def _get_compiler_arguments(self, version_map: Dict, base_path: Path) -> Dict[Version, Dict]:
         base_path = base_path or self.project_manager.contracts_folder
@@ -547,42 +476,35 @@
                 else:
                     # Contract not found. Fast forward out of this call.
                     for fr in trace:
                         if fr.op == "RETURN":
                             break
 
             elif frame.op in _RETURN_OPCODES:
-                if frame.op == "RETURN" and function:
-                    return_ast_result = [x for x in function.ast.children if x.ast_type == "Return"]
-                    if return_ast_result:
-                        # Ensure return statement added.
-                        # Sometimes it is missing from the PCMap otherwise.
-                        return_ast = return_ast_result[-1]
-                        location = return_ast.line_numbers
-
-                        last_lineno = max(0, location[2] - 1)
-                        for frameset in traceback.__root__[::-1]:
-                            if frameset.end_lineno is not None:
-                                last_lineno = frameset.end_lineno
-                                break
-
-                        start = last_lineno + 1
-                        last_pcs = {last_pc + 1} if last_pc else {}
-                        traceback.last.extend(location, pcs=last_pcs, ws_start=start)
+                if frame.op in "RETURN" and function:
+                    _extend_return(function, traceback, last_pc, contract_src.source_path)
 
                 # Completed!
                 return traceback
 
             if "PUSH" in frame.op and frame.pc in contract_src.pcmap:
                 # Check if next op is SSTORE to properly use AST from push op.
                 next_frame = next(trace, None)
                 is_non_payable_hit = False
                 if next_frame and next_frame.op == "SSTORE":
                     push_location = tuple(contract_src.pcmap[frame.pc]["location"])  # type: ignore
                     pcmap = PCMap.parse_obj({next_frame.pc: {"location": push_location}})
+
+                elif next_frame and next_frame.op in _RETURN_OPCODES:
+                    if next_frame.op in "RETURN" and function:
+                        _extend_return(function, traceback, last_pc, contract_src.source_path)
+
+                    # Completed!
+                    return traceback
+
                 else:
                     pcmap = contract_src.pcmap
                     dev_val = str((pcmap[frame.pc].get("dev") or "")).replace("dev: ", "")
                     is_non_payable_hit = dev_val == RuntimeErrorType.NONPAYABLE_CHECK.value
 
                 if not is_non_payable_hit and next_frame:
                     frame = next_frame
@@ -598,15 +520,15 @@
             dev_item = pcmap[frame.pc].get("dev", "")
             dev = str(dev_item).replace("dev: ", "")
             if not location and dev in [m.value for m in RuntimeErrorType]:
                 error_type = RuntimeErrorType(dev)
                 if error_type != RuntimeErrorType.NONPAYABLE_CHECK and traceback.last is not None:
                     # If the error type is not the non-payable check,
                     # it happened in the last method.
-                    name = traceback.last.name
+                    name = traceback.last.closure.name
 
                 elif method_id in contract_src.contract_type.methods:
                     # For non-payable checks, they should hit here.
                     method_checked = contract_src.contract_type.methods[method_id]
                     name = method_checked.name
 
                 else:
@@ -667,7 +589,203 @@
     return op == "JUMPI" and value is not None and value == revert_pc
 
 
 def _has_empty_revert(opcodes: List[str]) -> bool:
     return (len(opcodes) > 12 and opcodes[-13] == "JUMPDEST" and opcodes[-9] == "REVERT") or (
         len(opcodes) > 4 and opcodes[-5] == "JUMPDEST" and opcodes[-1] == "REVERT"
     )
+
+
+def _get_pcmap(bytecode: Dict, src_map: List[SourceMapItem], opcodes: List[str]) -> PCMap:
+    # Find the non payable value check.
+    src_info = bytecode["sourceMapFull"]
+    pc_data = {pc: {"location": ln} for pc, ln in src_info["pc_pos_map"].items()}
+    non_payable_check = _find_non_payable_check(src_map, opcodes)
+    if not non_payable_check:
+        non_payable_check = min([int(x) for x in pc_data]) - 1
+
+    pc_data[non_payable_check] = {"dev": _NON_PAYABLE_STR, "location": None}
+
+    # Apply other errors.
+    errors = src_info["error_map"]
+    for err_pc, error_type in errors.items():
+        if "safemul" in error_type or "safeadd" in err_pc:
+            error_str = RuntimeErrorType.INTEGER_OVERFLOW.value
+        elif "safesub" in error_type:
+            error_str = RuntimeErrorType.INTEGER_UNDERFLOW.value
+        elif "safediv" in error_type:
+            error_str = RuntimeErrorType.DIVISION_BY_ZERO.value
+        elif "safemod" in error_type:
+            error_str = RuntimeErrorType.MODULO_BY_ZERO.value
+        elif "bounds check" in error_type:
+            error_str = RuntimeErrorType.INDEX_OUT_OF_RANGE.value
+        else:
+            error_str = error_type.upper().replace(" ", "_")
+
+        if err_pc in pc_data:
+            pc_data[err_pc]["dev"] = f"dev: {error_str}"
+        else:
+            pc_data[err_pc] = {"dev": f"dev: {error_str}", "location": None}
+
+    return PCMap.parse_obj(pc_data)
+
+
+def _get_legacy_pcmap(ast: ASTNode, src_map: List[SourceMapItem], opcodes: List[str]):
+    """
+    For Vyper versions < 0.3.8, allows us to still get a PCMap.
+    """
+
+    pc = 0
+    pc_map_list: List[Tuple[int, Dict[str, Optional[Any]]]] = []
+    last_value = None
+    revert_pc = -1
+    if _has_empty_revert(opcodes):
+        revert_pc = _get_revert_pc(opcodes)
+
+    processed_opcodes = []
+
+    # There is only 1 non-payable check and it happens early in the bytecode.
+    non_payable_check_found = False
+
+    # There is at most 1 fallback error PC
+    fallback_found = False
+
+    while src_map and opcodes:
+        src = src_map.pop(0)
+        op = opcodes.pop(0)
+        processed_opcodes.append(op)
+        pc += 1
+
+        # If immutable member load, ignore increasing pc by push size.
+        if _is_immutable_member_load(opcodes):
+            last_value = int(opcodes.pop(0), 16)
+            # Add the push number, e.g. PUSH1 adds `1`.
+            num_pushed = int(op[4:])
+            pc += num_pushed
+
+        # Add content PC item.
+        # Also check for compiler runtime error handling.
+        # Runtime error locations are marked in the PCMap for further analysis.
+        if src.start is not None and src.length is not None:
+            stmt = ast.get_node(src)
+            if stmt:
+                # Add located item.
+                line_nos = list(stmt.line_numbers)
+                item: Dict = {"location": line_nos}
+                is_revert_jump = _is_revert_jump(op, last_value, revert_pc)
+                if op == "REVERT" or is_revert_jump:
+                    dev = None
+                    if stmt.ast_type in ("AugAssign", "BinOp"):
+                        # SafeMath
+                        for node in stmt.children:
+                            dev = RuntimeErrorType.from_operator(node.ast_type)
+                            if dev:
+                                break
+
+                    elif stmt.ast_type == "Subscript":
+                        dev = RuntimeErrorType.INDEX_OUT_OF_RANGE
+
+                    if dev:
+                        val = f"dev: {dev.value}"
+                        if is_revert_jump and len(pc_map_list) >= 1:
+                            pc_map_list[-1][1]["dev"] = val
+                        else:
+                            item["dev"] = val
+
+                pc_map_list.append((pc, item))
+
+        elif not fallback_found and _is_fallback_check(opcodes, op):
+            # You can tell this is the Fallback jump because it is checking for the method ID.
+            item = {"dev": f"dev: {RuntimeErrorType.FALLBACK_NOT_DEFINED.value}", "location": None}
+            # PC is actually the one before but it easier to detect here.
+            pc_map_list.append((pc - 1, item))
+            fallback_found = True
+
+        elif not non_payable_check_found and _is_non_payable_check(opcodes, op, revert_pc):
+            item = {"dev": _NON_PAYABLE_STR, "location": None}
+            pc_map_list.append((pc, item))
+            non_payable_check_found = True
+
+    return PCMap.parse_obj(dict(pc_map_list))
+
+
+def _find_non_payable_check(src_map: List[SourceMapItem], opcodes: List[str]) -> Optional[int]:
+    pc = 0
+    revert_pc = -1
+    if _has_empty_revert(opcodes):
+        revert_pc = _get_revert_pc(opcodes)
+
+    while src_map and opcodes:
+        op = opcodes.pop(0)
+        pc += 1
+
+        # If immutable member load, ignore increasing pc by push size.
+        if _is_immutable_member_load(opcodes):
+            # Add the push number, e.g. PUSH1 adds `1`.
+            pc += int(op[4:])
+
+        if _is_non_payable_check(opcodes, op, revert_pc):
+            return pc
+
+    return None
+
+
+def _is_non_payable_check(opcodes: List[str], op: str, revert_pc: int) -> bool:
+    return (
+        len(opcodes) >= 3
+        and op == "CALLVALUE"
+        and "PUSH" in opcodes[0]
+        and is_0x_prefixed(opcodes[1])
+        and _is_revert_jump(opcodes[2], int(opcodes[1], 16), revert_pc)
+    )
+
+
+def _get_revert_pc(opcodes: List[str]) -> int:
+    """
+    Starting in vyper 0.2.14, reverts without a reason string are optimized
+    with a jump to the "end" of the bytecode.
+    """
+    return (
+        len(opcodes)
+        + sum(int(i[4:]) - 1 for i in opcodes if i.startswith("PUSH"))
+        - _EMPTY_REVERT_OFFSET
+    )
+
+
+def _is_immutable_member_load(opcodes: List[str]):
+    is_code_copy = len(opcodes) > 5 and opcodes[5] == "CODECOPY"
+    return not is_code_copy and opcodes and is_0x_prefixed(opcodes[0])
+
+
+def _extend_return(function: Function, traceback: SourceTraceback, last_pc: int, source_path: Path):
+    return_ast_result = [x for x in function.ast.children if x.ast_type == "Return"]
+    if not return_ast_result:
+        return
+
+    # Ensure return statement added.
+    # Sometimes it is missing from the PCMap otherwise.
+    return_ast = return_ast_result[-1]
+    location = return_ast.line_numbers
+
+    last_lineno = max(0, location[2] - 1)
+    for frameset in traceback.__root__[::-1]:
+        if frameset.end_lineno is not None:
+            last_lineno = frameset.end_lineno
+            break
+
+    start = last_lineno + 1
+    last_pcs = {last_pc + 1} if last_pc else set()
+    if traceback.last:
+        traceback.last.extend(location, pcs=last_pcs, ws_start=start)
+    else:
+        # Not sure if it ever gets here, but type-checks say it could.
+        traceback.add_jump(location, function, 1, last_pcs, source_path=source_path)
+
+
+def _is_fallback_check(opcodes: List[str], op: str) -> bool:
+    return (
+        "JUMP" in op
+        and len(opcodes) >= 7
+        and opcodes[0] == "JUMPDEST"
+        and opcodes[6] == "SHR"
+        and opcodes[5] == "0xE0"
+    )
```

### Comparing `ape-vyper-0.6.7/ape_vyper/exceptions.py` & `ape-vyper-0.6.8/ape_vyper/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -22,15 +22,17 @@
     A compiler-specific error in Vyper.
     """
 
     def __init__(self, err: Union[VyperError, str]):
         if isinstance(err, VyperError):
             self.base_err = err
             message = "\n\n".join(
-                f"{e['sourceLocation']['file']}\n{e['type']}:{e['message']}" for e in err.error_dict
+                f"{e['sourceLocation']['file']}\n{e['type']}:"
+                f"{e.get('formattedMessage', e['message'])}"
+                for e in err.error_dict
             )
         else:
             self.base_err = None
             message = str(err)
 
         super().__init__(message)
 
@@ -38,14 +40,15 @@
 class RuntimeErrorType(Enum):
     NONPAYABLE_CHECK = "Cannot send ether to non-payable function"
     INDEX_OUT_OF_RANGE = "Index out of range"
     INTEGER_OVERFLOW = "Integer overflow"
     INTEGER_UNDERFLOW = "Integer underflow"
     DIVISION_BY_ZERO = "Division by zero"
     MODULO_BY_ZERO = "Modulo by zero"
+    FALLBACK_NOT_DEFINED = "Fallback not defined"
 
     @classmethod
     def from_operator(cls, operator: str) -> Optional["RuntimeErrorType"]:
         if operator == "Add":
             return cls.INTEGER_OVERFLOW
         elif operator == "Sub":
             return cls.INTEGER_UNDERFLOW
@@ -118,15 +121,26 @@
     Raised when modding by zero.
     """
 
     def __init__(self, **kwargs):
         super().__init__(RuntimeErrorType.MODULO_BY_ZERO, **kwargs)
 
 
+class FallbackNotDefinedError(VyperRuntimeError):
+    """
+    Raised when calling a contract directly (with missing method bytes) that has no fallback
+    method defined in its ABI.
+    """
+
+    def __init__(self, **kwargs):
+        super().__init__(RuntimeErrorType.FALLBACK_NOT_DEFINED, **kwargs)
+
+
 RUNTIME_ERROR_MAP: Dict[RuntimeErrorType, Type[ContractLogicError]] = {
     RuntimeErrorType.NONPAYABLE_CHECK: NonPayableError,
     RuntimeErrorType.INDEX_OUT_OF_RANGE: IndexOutOfRangeError,
     RuntimeErrorType.INTEGER_OVERFLOW: IntegerOverflowError,
     RuntimeErrorType.INTEGER_UNDERFLOW: IntegerUnderflowError,
     RuntimeErrorType.DIVISION_BY_ZERO: DivisionByZeroError,
     RuntimeErrorType.MODULO_BY_ZERO: ModuloByZeroError,
+    RuntimeErrorType.FALLBACK_NOT_DEFINED: FallbackNotDefinedError,
 }
```

### Comparing `ape-vyper-0.6.7/ape_vyper.egg-info/PKG-INFO` & `ape-vyper-0.6.8/ape_vyper.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ape-vyper
-Version: 0.6.7
+Version: 0.6.8
 Summary: Plugin for Ape Ethereum Framework for compiling Vyper contracts
 Home-page: https://github.com/ApeWorX/ape-vyper
 Author: ApeWorX Ltd.
 Author-email: admin@apeworx.io
 License: Apache-2.0
 Keywords: ethereum
 Classifier: Development Status :: 5 - Production/Stable
@@ -28,15 +28,15 @@
 
 # Quick Start
 
 Ape compiler plugin around [VVM](https://github.com/vyperlang/vvm)
 
 ## Dependencies
 
-- [python3](https://www.python.org/downloads) version 3.8 or greater, python3-dev
+- [python3](https://www.python.org/downloads) version 3.8 up to 3.11.
 
 ## Installation
 
 ### via `pip`
 
 You can install the latest release via [`pip`](https://pypi.org/project/pip/):
 
@@ -91,11 +91,11 @@
   import_remapping:
     - "voting=VyperVoting@v0.3.8"
 ```
 
 Import the voting contract types like this:
 
 ```python
-# @version 0.3.8
+# @version 0.3.9
 
 import voting.ballot as ballot
 ```
```

### Comparing `ape-vyper-0.6.7/ape_vyper.egg-info/SOURCES.txt` & `ape-vyper-0.6.8/ape_vyper.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -35,16 +35,21 @@
 tests/contracts/failing_contracts/contract_undeclared_variable.vy
 tests/contracts/failing_contracts/contract_unknown_pragma.vy
 tests/contracts/passing_contracts/contract.vy
 tests/contracts/passing_contracts/contract_37.vy
 tests/contracts/passing_contracts/contract_no_pragma.vy
 tests/contracts/passing_contracts/contract_with_dev_messages.vy
 tests/contracts/passing_contracts/erc20.vy
+tests/contracts/passing_contracts/non_payable_default.vy
 tests/contracts/passing_contracts/older_version.vy
-tests/contracts/passing_contracts/registry.vy
-tests/contracts/passing_contracts/traceback_contract.vy
+tests/contracts/passing_contracts/payable_default.vy
+tests/contracts/passing_contracts/registry_037.vy
+tests/contracts/passing_contracts/registry_039.vy
+tests/contracts/passing_contracts/traceback_contract_037.vy
+tests/contracts/passing_contracts/traceback_contract_039.vy
 tests/contracts/passing_contracts/use_iface.vy
 tests/contracts/passing_contracts/use_iface2.vy
 tests/contracts/passing_contracts/DirectoryWithExtension.vy/README.md
 tests/contracts/passing_contracts/interfaces/IFace.vy
 tests/contracts/passing_contracts/interfaces/IFace2.vy
-tests/contracts/passing_contracts/interfaces/IRegistry.vy
+tests/contracts/passing_contracts/interfaces/IRegistry_037.vy
+tests/contracts/passing_contracts/interfaces/IRegistry_039.vy
```

### Comparing `ape-vyper-0.6.7/ape_vyper.egg-info/requires.txt` & `ape-vyper-0.6.8/ape_vyper.egg-info/requires.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 eth-ape<0.7,>=0.6.10
-ethpm-types<0.6,>=0.5.1
+ethpm-types
 tqdm
 vvm<0.2,>=0.1.0
 
 [dev]
 pytest>=6.0
+pytest-mock
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
 black<24,>=23.3.0
 mypy<1,>=0.991
 types-setuptools
 flake8<7,>=6.0.0
@@ -38,10 +39,11 @@
 [release]
 setuptools
 wheel
 twine
 
 [test]
 pytest>=6.0
+pytest-mock
 pytest-xdist
 pytest-cov
 hypothesis<7.0,>=6.2.0
```

### Comparing `ape-vyper-0.6.7/pyproject.toml` & `ape-vyper-0.6.8/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 # NOTE: you have to use single-quoted strings in TOML for regular expressions.
 # It's the equivalent of r-strings in Python.  Multiline strings are treated as
 # verbose regular expressions by Black.  Use [ ] to denote a significant space
 # character.
 
 [tool.black]
 line-length = 100
-target-version = ['py38', 'py39', 'py310']
+target-version = ['py38', 'py39', 'py310', 'py311']
 include = '\.pyi?$'
 
 [tool.pytest.ini_options]
 addopts = """
     -p no:ape_test
     --cov-branch
     --cov-report term
```

### Comparing `ape-vyper-0.6.7/setup.py` & `ape-vyper-0.6.8/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from setuptools import find_packages, setup
 
 extras_require = {
     "test": [  # `test` GitHub Action jobs uses this
         "pytest>=6.0",  # Core testing package
+        "pytest-mock",
         "pytest-xdist",  # multi-process runner
         "pytest-cov",  # Coverage analyzer plugin
         "hypothesis>=6.2.0,<7.0",  # Strategy-based fuzzer
     ],
     "lint": [
         "black>=23.3.0,<24",  # Auto-formatter and linter
         "mypy>=0.991,<1",  # Static type analyzer
@@ -54,15 +55,15 @@
     long_description_content_type="text/markdown",
     author="ApeWorX Ltd.",
     author_email="admin@apeworx.io",
     url="https://github.com/ApeWorX/ape-vyper",
     include_package_data=True,
     install_requires=[
         "eth-ape>=0.6.10,<0.7",
-        "ethpm-types>=0.5.1,<0.6",  # Currently bumped 1 higher than eth-ape
+        "ethpm-types",  # Use same version as eth-ape
         "tqdm",  # Use same version as eth-ape
         "vvm>=0.1.0,<0.2",
     ],
     python_requires=">=3.8,<4",
     extras_require=extras_require,
     py_modules=["ape_vyper"],
     license="Apache-2.0",
```

### Comparing `ape-vyper-0.6.7/tests/conftest.py` & `ape-vyper-0.6.8/tests/conftest.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from distutils.dir_util import copy_tree
 from pathlib import Path
 from tempfile import mkdtemp
 
 import ape
 import pytest
 import vvm  # type: ignore
+from geth.wrapper import construct_test_chain_kwargs as geth_ctor  # type: ignore
 
 from ape_vyper.compiler import VyperCompiler
 
 # NOTE: Ensure that we don't use local paths for these
 DATA_FOLDER = Path(mkdtemp()).resolve()
 PROJECT_FOLDER = Path(mkdtemp()).resolve()
 ape.config.DATA_FOLDER = DATA_FOLDER
@@ -103,30 +104,54 @@
     with config.using_project(project_dest_dir) as project:
         yield project
         if project.local_project._cache_folder.is_dir():
             shutil.rmtree(project.local_project._cache_folder)
 
 
 @pytest.fixture
-def geth_provider():
+def geth_provider(mocker):
+    # TODO: Delete this hack to fix bug in py-geth<0.3.13
+    patch = mocker.patch("ape_geth.provider.construct_test_chain_kwargs")
+
+    def side_effect(*args, **kwargs):
+        result = geth_ctor(*args, **kwargs)
+        if "miner_threads" in result:
+            del result["miner_threads"]
+
+        return result
+
+    patch.side_effect = side_effect
+
     if not ape.networks.active_provider or ape.networks.provider.name != "geth":
         with ape.networks.ethereum.local.use_provider(
             "geth", provider_settings={"uri": "http://127.0.0.1:5550"}
         ) as provider:
             yield provider
     else:
         yield ape.networks.provider
 
 
 @pytest.fixture
 def account():
     return ape.accounts.test_accounts[0]
 
 
+@pytest.fixture(params=("037", "039"))
+def traceback_contract(request, account, project, geth_provider):
+    return _get_tb_contract(request.param, project, account)
+
+
 @pytest.fixture
-def registry(geth_provider, account, project):
-    return account.deploy(project.registry)
+def traceback_contract_037(account, project, geth_provider):
+    return _get_tb_contract("037", project, account)
 
 
 @pytest.fixture
-def contract(registry, account, project):
-    return account.deploy(project.traceback_contract, registry)
+def traceback_contract_039(account, project, geth_provider):
+    return _get_tb_contract("039", project, account)
+
+
+def _get_tb_contract(version: str, project, account):
+    registry_type = project.get_contract(f"registry_{version}")
+    registry = account.deploy(registry_type)
+    contract = project.get_contract(f"traceback_contract_{version}")
+    return account.deploy(contract, registry)
```

### Comparing `ape-vyper-0.6.7/tests/contracts/passing_contracts/contract.vy` & `ape-vyper-0.6.8/tests/contracts/passing_contracts/contract.vy`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# @version 0.3.8
+# @version 0.3.9
 
 from vyper.interfaces import ERC20
 
 interface ERC20Ext:
     def decimals() -> uint8: view
 
 # Public storage (PCMap testing)
```

### Comparing `ape-vyper-0.6.7/tests/contracts/passing_contracts/contract_37.vy` & `ape-vyper-0.6.8/tests/contracts/passing_contracts/contract_37.vy`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.7/tests/contracts/passing_contracts/erc20.vy` & `ape-vyper-0.6.8/tests/contracts/passing_contracts/erc20.vy`

 * *Files identical despite different names*

### Comparing `ape-vyper-0.6.7/tests/contracts/passing_contracts/traceback_contract.vy` & `ape-vyper-0.6.8/tests/contracts/passing_contracts/traceback_contract_039.vy`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-# @version 0.3.7
+# @version 0.3.9
 
-import interfaces.IRegistry as IRegistry
+import interfaces.IRegistry_039 as IRegistry_039
 
 _balance: public(uint256)
-registry: public(IRegistry)
+registry: public(IRegistry_039)
 
 
 @external
-def __init__(registry: IRegistry):
+def __init__(registry: IRegistry_039):
     self.registry = registry
 
 
 @external
 def addBalance(
     num: uint256
 ) -> uint256:
```

### Comparing `ape-vyper-0.6.7/tests/test_compiler.py` & `ape-vyper-0.6.8/tests/test_compiler.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,32 +1,40 @@
+import re
 from pathlib import Path
 from typing import List
 
 import pytest
 from ape.exceptions import ContractLogicError
+from pkg_resources import get_distribution
 from semantic_version import Version  # type: ignore
 from vvm import compile_source  # type: ignore
 from vvm.exceptions import VyperError  # type: ignore
 
 from ape_vyper.compiler import RuntimeErrorType
 from ape_vyper.exceptions import (
+    FallbackNotDefinedError,
     IntegerOverflowError,
     NonPayableError,
     VyperCompileError,
     VyperInstallError,
 )
 
 BASE_CONTRACTS_PATH = Path(__file__).parent / "contracts"
 PASSING_BASE = BASE_CONTRACTS_PATH / "passing_contracts"
 FAILING_BASE = BASE_CONTRACTS_PATH / "failing_contracts"
 
 # Currently, this is the only version specified from a pragma spec
 OLDER_VERSION_FROM_PRAGMA = Version("0.2.8")
 VERSION_37 = Version("0.3.7")
-VERSION_FROM_PRAGMA = Version("0.3.8")
+
+# NOTE: This is really just about testing > 0.3.7.
+#  Should get switched as soon as a more stable version is released.
+VERSION_FROM_PRAGMA = Version("0.3.9")
+
+APE_VERSION = Version(get_distribution("eth-ape").version.split(".dev")[0].strip())
 
 
 @pytest.fixture
 def dev_revert_source():
     return PASSING_BASE / "contract_with_dev_messages.vy"
 
 
@@ -36,16 +44,23 @@
     """
     suffix = "passing_contracts" if passing else "failing_contracts"
     return [p.name for p in (BASE_CONTRACTS_PATH / suffix).glob("*.vy") if p.is_file()]
 
 
 PASSING_CONTRACT_NAMES = contract_test_cases(True)
 FAILING_CONTRACT_NAMES = contract_test_cases(False)
-EXPECTED_FAIL_MESSAGES = {
-    "contract_undeclared_variable": "'hello' has not been declared",
+EXPECTED_FAIL_PATTERNS = {
+    "contract_undeclared_variable": re.compile(
+        (
+            r"\w*\.vy\s*UndeclaredDefinition:'\w*' "
+            r'has not been declared\s*contract "\w*.vy"'
+            # NOTE: Following bit proves we have line numbers (see all the \d's).
+            r', function "\w*",.*\w*\d:\d\s*\d def.*\s*.*\d\s*\w* = \w*\s*-*\^\s*\d\s*.*'
+        ),
+    ),
     "contract_unknown_pragma": "",
 }
 
 
 def test_compile_project(project):
     contracts = project.load_contracts()
     assert len(contracts) == len([p.name for p in PASSING_BASE.glob("*.vy") if p.is_file()])
@@ -61,15 +76,15 @@
 
 
 @pytest.mark.parametrize(
     "contract_name", [n for n in FAILING_CONTRACT_NAMES if n != "contract_unknown_pragma.vy"]
 )
 def test_compile_failures(contract_name, compiler):
     path = FAILING_BASE / contract_name
-    with pytest.raises(VyperCompileError, match=EXPECTED_FAIL_MESSAGES[path.stem]) as err:
+    with pytest.raises(VyperCompileError, match=EXPECTED_FAIL_PATTERNS[path.stem]) as err:
         compiler.compile([path], base_path=FAILING_BASE)
 
     assert isinstance(err.value.base_err, VyperError)
 
 
 def test_install_failure(compiler):
     path = FAILING_BASE / "contract_unknown_pragma.vy"
@@ -89,22 +104,24 @@
             continue
 
         sources = ", ".join([p.name for p in actual[version]])
         fail_message = f"Unexpected version '{version}' with sources: {sources}"
         pytest.fail(fail_message)
 
     assert len(actual[OLDER_VERSION_FROM_PRAGMA]) == 1
-    assert len(actual[VERSION_FROM_PRAGMA]) == 6
+    assert len(actual[VERSION_FROM_PRAGMA]) == 8
     assert actual[OLDER_VERSION_FROM_PRAGMA] == {project.contracts_folder / "older_version.vy"}
 
     expected = (
         "contract.vy",
         "contract_no_pragma.vy",
         "contract_with_dev_messages.vy",
         "erc20.vy",
+        "registry_039.vy",
+        "traceback_contract_039.vy",
         "use_iface.vy",
         "use_iface2.vy",
     )
     names = [x.name for x in actual[VERSION_FROM_PRAGMA]]
     failures = []
     missing = []
     for ex in expected:
@@ -134,20 +151,20 @@
     vyper_028 = [c for c in manifest.compilers if str(c.version) == str(OLDER_VERSION_FROM_PRAGMA)][
         0
     ]
 
     for compiler in (vyper_028, vyper_latest):
         assert compiler.name == "vyper"
 
-    assert len(vyper_latest.contractTypes) == 6
+    assert len(vyper_latest.contractTypes) == 8
     assert len(vyper_028.contractTypes) == 1
     assert "contract" in vyper_latest.contractTypes
     assert "older_version" in vyper_028.contractTypes
     for compiler in (vyper_latest, vyper_028):
-        assert compiler.settings["evmVersion"] == "constantinople"
+        assert compiler.settings["evmVersion"] == "istanbul"
         assert compiler.settings["optimize"] is True
 
 
 def test_compile_parse_dev_messages(compiler, dev_revert_source):
     """
     Test parsing of dev messages in a contract. These follow the form of "#dev: ...".
 
@@ -183,26 +200,28 @@
     assert set(actual["contract.vy"]) == {builtin_import}
     assert len(actual["use_iface.vy"]) == 3
     assert set(actual["use_iface.vy"]) == {local_import, local_from_import, dependency_import}
     assert len(actual["use_iface2.vy"]) == 1
     assert set(actual["use_iface2.vy"]) == {local_import}
 
 
-# TODO: Test this on 0.3.8 and utilize the pcmap from the output.
-def test_pc_map(compiler, project):
+@pytest.mark.parametrize("src,vers", [("contract", "0.3.9"), ("contract_37", "0.3.7")])
+def test_pc_map(compiler, project, src, vers):
     """
     Ensure we de-compress the source map correctly by comparing to the results
     from `compile_src()` which includes the uncompressed source map data.
     """
 
-    path = PASSING_BASE / "contract_37.vy"
+    path = PASSING_BASE / f"{src}.vy"
     result = compiler.compile([path], base_path=PASSING_BASE)[0]
     actual = result.pcmap.__root__
     code = path.read_text()
-    compile_result = compile_source(code, vyper_version="0.3.7")["<stdin>"]
+    compile_result = compile_source(code, vyper_version=vers, evm_version=compiler.evm_version)[
+        "<stdin>"
+    ]
     src_map = compile_result["source_map"]
     lines = code.splitlines()
 
     # Use the old-fashioned way of gathering PCMap to ensure our creative way works
     expected = {pc: {"location": ln} for pc, ln in src_map["pc_pos_map"].items()}
     missing_pcs = []
     empty_locs = []
@@ -255,99 +274,137 @@
         # A helper for getting expected line numbers
         return [i + 1 for i, x in enumerate(lines) if cont in x][0]
 
     # Verify non-payable checks.
     nonpayable_checks = _all(RuntimeErrorType.NONPAYABLE_CHECK)
     assert len(nonpayable_checks) == 1
 
-    # Verify integer overflow checks
-    overflows = _all(RuntimeErrorType.INTEGER_OVERFLOW)
-    overflow_no = line("return (2**127-1) + i")
-    assert len(overflows) == 2
-    assert overflows[0]["location"] == [overflow_no, 12, overflow_no, 20]
-
-    # Verify integer underflow checks
-    underflows = _all(RuntimeErrorType.INTEGER_UNDERFLOW)
-    underflow_no = line("return i - (2**127-1)")
-    assert len(underflows) == 2
-    assert underflows[0]["location"] == [underflow_no, 11, underflow_no, 25]
-
-    # Verify division by zero checks
-    div_zeros = _all(RuntimeErrorType.DIVISION_BY_ZERO)
-    div_no = line("return 4 / i")
-    assert len(div_zeros) == 1
-    assert div_zeros[0]["location"] == [div_no, 11, div_no, 16]
-
-    # Verify modulo by zero checks
-    mod_zeros = _all(RuntimeErrorType.MODULO_BY_ZERO)
-    mod_no = line("return 4 % i")
-    assert len(mod_zeros) == 1
-    assert mod_zeros[0]["location"] == [mod_no, 11, mod_no, 16]
-
-    # Verify index out of range checks
-    range_checks = _all(RuntimeErrorType.INDEX_OUT_OF_RANGE)
-    range_no = line("return self.dynArray[idx]")
-    assert len(range_checks) == 1
-    assert range_checks[0]["location"] == [range_no, 11, range_no, 24]
+    # TODO: Figure out >0.3.7 issue with error maps.
+    if vers == "0.3.7":
+        # Verify integer overflow checks
+        overflows = _all(RuntimeErrorType.INTEGER_OVERFLOW)
+        overflow_no = line("return (2**127-1) + i")
+        expected_overflow_loc = [overflow_no, 12, overflow_no, 20]
+        assert len(overflows) >= 2
+        assert expected_overflow_loc in [o["location"] for o in overflows]
+
+        # Verify integer underflow checks
+        underflows = _all(RuntimeErrorType.INTEGER_UNDERFLOW)
+        underflow_no = line("return i - (2**127-1)")
+        expected_underflow_loc = [underflow_no, 11, underflow_no, 25]
+        assert len(underflows) == 2
+        assert expected_underflow_loc in [u["location"] for u in underflows]
+
+        # Verify division by zero checks
+        div_zeros = _all(RuntimeErrorType.DIVISION_BY_ZERO)
+        div_no = line("return 4 / i")
+        expected_div_0 = [div_no, 11, div_no, 16]
+
+        assert len(div_zeros) >= 1
+        assert expected_div_0 in [d["location"] for d in div_zeros]
+
+        # Verify modulo by zero checks
+        mod_zeros = _all(RuntimeErrorType.MODULO_BY_ZERO)
+        mod_no = line("return 4 % i")
+        expected_mod_0_loc = [mod_no, 11, mod_no, 16]
+        assert len(mod_zeros) >= 1
+        assert expected_mod_0_loc in [m["location"] for m in mod_zeros]
+
+        # Verify index out of range checks
+        range_checks = _all(RuntimeErrorType.INDEX_OUT_OF_RANGE)
+        range_no = line("return self.dynArray[idx]")
+        expected_range_check = [range_no, 11, range_no, 24]
+        assert len(range_checks) >= 1
+        assert expected_range_check in [r["location"] for r in range_checks]
 
 
-def test_int_overflow(geth_provider, contract, account):
+def test_enrich_error_int_overflow(geth_provider, traceback_contract_037, account):
     int_max = 2**256 - 1
     with pytest.raises(IntegerOverflowError):
-        contract.addBalance(int_max, sender=account)
+        traceback_contract_037.addBalance(int_max, sender=account)
 
 
-def test_non_payable_check(geth_provider, contract, account):
+def test_enrich_error_non_payable_check(geth_provider, traceback_contract_037, account):
     with pytest.raises(NonPayableError):
-        contract.addBalance(123, sender=account, value=1)
+        traceback_contract_037.addBalance(123, sender=account, value=1)
+
+
+@pytest.mark.skipif(APE_VERSION <= Version("0.6.10"), reason="Fallback invoked via new API")
+def test_enrich_error_fallback(geth_provider, traceback_contract_037, account):
+    """
+    Show that when attempting to call a contract's fallback method when there is
+    no fallback defined results in a custom contract logic error.
+    """
+    with pytest.raises(FallbackNotDefinedError):
+        traceback_contract_037(sender=account)
 
 
-# TODO: Run this test using 0.3.8 as well, once we get the PCMap working.
-def test_trace_source(account, geth_provider, project, contract):
-    receipt = contract.addBalance(123, sender=account)
+def test_trace_source(account, geth_provider, project, traceback_contract):
+    """
+    NOTE: Using 0.3.7 because 0.3.9 bugs and shows the wrong lines.
+    """
+
+    receipt = traceback_contract.addBalance(123, sender=account)
     actual = receipt.source_traceback
     base_folder = project.contracts_folder
+    contract_name = traceback_contract.contract_type.name
     expected = rf"""
 Traceback (most recent call last)
-  File {base_folder}/traceback_contract.vy, in addBalance
+  File {base_folder}/{contract_name}.vy, in addBalance
        27     # Comments in the middle (is a test)
        28
        29     for i in [1, 2, 3, 4, 5]:
        30         if i != num:
        31             continue
        32
   -->  33     return self._balance
 """.strip()
     assert str(actual) == expected
 
 
-def test_trace_err_source(account, geth_provider, project, contract):
-    txn = contract.addBalance_f.as_transaction(123)
+def test_trace_err_source(account, geth_provider, project, traceback_contract):
+    txn = traceback_contract.addBalance_f.as_transaction(123)
     try:
         account.call(txn)
     except ContractLogicError:
         pass
 
     receipt = geth_provider.get_receipt(txn.txn_hash.hex())
     actual = receipt.source_traceback
     base_folder = project.contracts_folder
+    contract_name = traceback_contract.contract_type.name
+    version_key = contract_name.split("traceback_contract_")[-1]
     expected = rf"""
 Traceback (most recent call last)
-  File {base_folder}/traceback_contract.vy, in addBalance_f
+  File {base_folder}/{contract_name}.vy, in addBalance_f
        44     # Run some loops.
        45     for i in [1, 2, 3, 4, 5]:
        46         if i == num:
        47             break
        48
        49     # Fail in the middle (is test)
        50     # Fails because was already set above.
   -->  51     self.registry.register_f(msg.sender)
        52
        53     for i in [1, 2, 3, 4, 5]:
        54         if i != num:
        55             continue
 
-  File {base_folder}/registry.vy, in register_f
+  File {base_folder}/registry_{version_key}.vy, in register_f
+       11 def register_f(addr: address):
   -->  12     assert self.addr != addr, "doubling."
        13     self.addr = addr
     """.strip()
     assert str(actual) == expected
+
+
+@pytest.mark.skipif(APE_VERSION <= Version("0.6.10"), reason="Fallback invoked via new API")
+def test_trace_source_default_method(geth_provider, account, project):
+    """
+    This test proves you get a working source-traceback from __default__ calls.
+    """
+    contract = project.non_payable_default.deploy(sender=account)
+    receipt = contract(sender=account)
+    src_tb = receipt.source_traceback
+    actual = str(src_tb[-1][-1]).lstrip()  # Last line in traceback (without indent).
+    expected = "8     log NotPayment(msg.sender)"
+    assert actual == expected
```

