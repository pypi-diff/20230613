# Comparing `tmp/dbis-relational-calculus-1.0.6.tar.gz` & `tmp/dbis-relational-calculus-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbis-relational-calculus-1.0.6.tar", last modified: Mon Apr 10 13:51:41 2023, max compression
+gzip compressed data, was "dbis-relational-calculus-1.0.7.tar", last modified: Tue Jun 13 15:19:49 2023, max compression
```

## Comparing `dbis-relational-calculus-1.0.6.tar` & `dbis-relational-calculus-1.0.7.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 13:51:41.815073 dbis-relational-calculus-1.0.6/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/LICENSE
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-04-10 13:51:41.815073 dbis-relational-calculus-1.0.6/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11343 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/README.md
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 13:51:41.813073 dbis-relational-calculus-1.0.6/dbis_relational_calculus.egg-info/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-04-10 13:51:41.000000 dbis-relational-calculus-1.0.6/dbis_relational_calculus.egg-info/PKG-INFO
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2739 2023-04-10 13:51:41.000000 dbis-relational-calculus-1.0.6/dbis_relational_calculus.egg-info/SOURCES.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-04-10 13:51:41.000000 dbis-relational-calculus-1.0.6/dbis_relational_calculus.egg-info/dependency_links.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       32 2023-04-10 13:51:41.000000 dbis-relational-calculus-1.0.6/dbis_relational_calculus.egg-info/requires.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       20 2023-04-10 13:51:41.000000 dbis-relational-calculus-1.0.6/dbis_relational_calculus.egg-info/top_level.txt
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      709 2023-04-10 13:50:27.000000 dbis-relational-calculus-1.0.6/pyproject.toml
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 13:51:41.813073 dbis-relational-calculus-1.0.6/relational_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 13:51:41.813073 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6442 2023-04-10 13:48:50.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/DomainCalculus.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      728 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/Result.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      320 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/Variable.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1358 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 13:51:41.813073 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8294 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/Formula.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4394 2023-04-10 13:29:25.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/Tuple.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 13:51:41.814073 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/atoms/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2674 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/atoms/Equals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2512 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2503 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2506 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2497 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/atoms/LessThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/atoms/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 13:51:41.814073 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/connectives/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6785 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/connectives/And.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3258 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/connectives/Not.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6768 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/connectives/Or.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/connectives/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 13:51:41.814073 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/quantifiers/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4543 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4407 2023-04-10 12:11:51.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/quantifiers/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 13:51:41.814073 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      956 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/Result.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3462 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/TupleCalculus.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1281 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 13:51:41.814073 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    10704 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/Formula.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2120 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/Variable.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 13:51:41.814073 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/atoms/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3914 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/atoms/Equals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3760 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3753 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3757 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3747 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/atoms/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 13:51:41.814073 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/connectives/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12145 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/connectives/And.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4573 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/connectives/Not.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12108 2023-04-10 11:15:31.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/connectives/Or.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/connectives/__init__.py
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 13:51:41.815073 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/quantifiers/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8618 2023-04-10 12:19:02.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8367 2023-04-10 12:19:02.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/quantifiers/__init__.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-04-10 13:51:41.815073 dbis-relational-calculus-1.0.6/setup.cfg
-drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-04-10 13:51:41.815073 dbis-relational-calculus-1.0.6/tests/
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4425 2023-04-10 13:48:05.000000 dbis-relational-calculus-1.0.6/tests/test_domain_calculus_sql.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      580 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/tests/test_domain_calculus_validity.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3100 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/tests/test_tuple_calculus_attribute_access.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4388 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/tests/test_tuple_calculus_sql.py
--rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      733 2023-04-10 11:01:38.000000 dbis-relational-calculus-1.0.6/tests/test_tuple_calculus_validity.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 15:19:49.960529 dbis-relational-calculus-1.0.7/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11357 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/LICENSE
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-06-13 15:19:49.960529 dbis-relational-calculus-1.0.7/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11343 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/README.md
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 15:19:49.958529 dbis-relational-calculus-1.0.7/dbis_relational_calculus.egg-info/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11837 2023-06-13 15:19:49.000000 dbis-relational-calculus-1.0.7/dbis_relational_calculus.egg-info/PKG-INFO
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2739 2023-06-13 15:19:49.000000 dbis-relational-calculus-1.0.7/dbis_relational_calculus.egg-info/SOURCES.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        1 2023-06-13 15:19:49.000000 dbis-relational-calculus-1.0.7/dbis_relational_calculus.egg-info/dependency_links.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       32 2023-06-13 15:19:49.000000 dbis-relational-calculus-1.0.7/dbis_relational_calculus.egg-info/requires.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       20 2023-06-13 15:19:49.000000 dbis-relational-calculus-1.0.7/dbis_relational_calculus.egg-info/top_level.txt
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      709 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/pyproject.toml
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 15:19:49.958529 dbis-relational-calculus-1.0.7/relational_calculus/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/relational_calculus/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 15:19:49.959529 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6956 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/DomainCalculus.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      953 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/Result.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      546 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/Variable.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1358 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 15:19:49.959529 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8504 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/Formula.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4546 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/Tuple.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 15:19:49.959529 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/atoms/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2840 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/atoms/Equals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2692 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2679 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2680 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2667 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/atoms/LessThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/atoms/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 15:19:49.959529 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/connectives/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6958 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/connectives/And.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3397 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/connectives/Not.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     6939 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/connectives/Or.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/connectives/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 15:19:49.959529 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/quantifiers/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4719 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4583 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/quantifiers/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 15:19:49.959529 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1182 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/Result.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4105 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/TupleCalculus.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     1281 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 15:19:49.959529 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    11218 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/Formula.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     2289 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/Variable.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 15:19:49.960529 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/atoms/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4080 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/atoms/Equals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3940 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3929 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3931 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3917 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/atoms/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 15:19:49.960529 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/connectives/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12318 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/connectives/And.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4712 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/connectives/Not.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)    12279 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/connectives/Or.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/connectives/__init__.py
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 15:19:49.960529 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/quantifiers/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8794 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     8543 2023-06-13 15:19:25.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/quantifiers/__init__.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)       38 2023-06-13 15:19:49.960529 dbis-relational-calculus-1.0.7/setup.cfg
+drwxr-xr-x   0 tilmohr   (1000) tilmohr   (1000)        0 2023-06-13 15:19:49.960529 dbis-relational-calculus-1.0.7/tests/
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4425 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/tests/test_domain_calculus_sql.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      580 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/tests/test_domain_calculus_validity.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     3100 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/tests/test_tuple_calculus_attribute_access.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)     4388 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/tests/test_tuple_calculus_sql.py
+-rw-r--r--   0 tilmohr   (1000) tilmohr   (1000)      733 2023-06-13 14:06:12.000000 dbis-relational-calculus-1.0.7/tests/test_tuple_calculus_validity.py
```

### Comparing `dbis-relational-calculus-1.0.6/LICENSE` & `dbis-relational-calculus-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.6/PKG-INFO` & `dbis-relational-calculus-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-relational-calculus
-Version: 1.0.6
+Version: 1.0.7
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis-relational-calculus
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-relational-calculus-1.0.6/README.md` & `dbis-relational-calculus-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.6/dbis_relational_calculus.egg-info/PKG-INFO` & `dbis-relational-calculus-1.0.7/dbis_relational_calculus.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbis-relational-calculus
-Version: 1.0.6
+Version: 1.0.7
 Summary: RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme
 Author-email: Til Mohr <til.mohr@rwth-aachen.de>
 Project-URL: Homepage, https://git.rwth-aachen.de/i5/teaching/dbis-relational-calculus
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
```

### Comparing `dbis-relational-calculus-1.0.6/dbis_relational_calculus.egg-info/SOURCES.txt` & `dbis-relational-calculus-1.0.7/dbis_relational_calculus.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.6/pyproject.toml` & `dbis-relational-calculus-1.0.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "dbis-relational-calculus"
-version = "1.0.6"
+version = "1.0.7"
 description = "RWTH Aachen Computer Science i5/dbis assets for Lecture Datenbanken und Informationssysteme"
 authors = [
 	{ name = "Til Mohr", email = "til.mohr@rwth-aachen.de" },
 ]
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/DomainCalculus.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/DomainCalculus.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 import relational_calculus.domain_calculus as dc
 from relational_calculus.domain_calculus.formulas.quantifiers.Forall import Forall
 
 
 class DomainCalculus:
@@ -17,14 +19,22 @@
         formula : Formula
             The formula that every result has to satisfy.
         """
         self.result = result
         self.formula = formula
 
     @typechecked
+    def __copy__(self) -> DomainCalculus:
+        return deepcopy(self)
+
+    @typechecked
+    def __deepcopy__(self, memo) -> DomainCalculus:
+        return DomainCalculus(deepcopy(self.result, memo), deepcopy(self.formula, memo))
+
+    @typechecked
     def verify(self) -> bool:
         """
         Verify the correctness of the result/formula combination (e.g. one must specify the type of a variable before returning it).
 
         Returns
         -------
         bool
@@ -52,14 +62,26 @@
         """
         Convert the domain calculus to a SQL query.
 
         Returns
         -------
         str
             The SQL query.
+        """
+        return deepcopy(self).__to_sql()
+
+    @typechecked
+    def __to_sql(self) -> str:
+        """
+        Convert the domain calculus to a SQL query.
+
+        Returns
+        -------
+        str
+            The SQL query.
         """
         # Select Statement
         select_query = "SELECT DISTINCT "
         for variable in self.result.variables:
             select_query += f'"{variable.name}", '
         select_query = select_query[: -len(", ")]  # remove last ', '
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/Result.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/Result.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 import relational_calculus.domain_calculus as dc
 
 
 class Result:
     @typechecked
@@ -15,13 +17,21 @@
             The variables that should be returned.
         """
         if len(variables) == 0:
             raise Exception("Must return at least one variable")
         self.variables = variables
 
     @typechecked
+    def __copy__(self) -> Result:
+        return deepcopy(self)
+
+    @typechecked
+    def __deepcopy__(self, memo) -> Result:
+        return Result(deepcopy(self.variables, memo))
+
+    @typechecked
     def __repr__(self) -> str:
         output = ""
         for variable in self.variables:
             output += f"\\text{{{variable.name}}}, "
         output = output[:-2]  # remove last ', '
         return output
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/__init__.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/__init__.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/Formula.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/Formula.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from abc import abstractclassmethod
+from copy import deepcopy
 
 from docstring_inheritance import NumpyDocstringInheritanceMeta
 from typeguard import typechecked
 
 from typing import Any, Optional
 
 import relational_calculus.domain_calculus as dc
@@ -23,14 +24,23 @@
         ----------
         children : list[Formula]
             Each implementation of formula can hold a list of children that it is composed of.
         """
         self.children = children
 
     @typechecked
+    def __copy__(self) -> Formula:
+        return deepcopy(self)
+
+    @typechecked
+    @abstractclassmethod
+    def __deepcopy__(self, memo) -> Formula:
+        pass
+
+    @typechecked
     @abstractclassmethod
     def __repr__(self) -> str:
         """
         Returs a string representation of a given formula formatted in Latex Math Mode.
 
         Returns
         -------
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/Tuple.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/Tuple.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 from typing import Any, Optional
 
 import relational_calculus.domain_calculus as dc
 
 
@@ -17,14 +19,18 @@
         super().__init__([])
         if len([value for value in variables if value is not None]) == 0:
             raise Exception("Must have at least one variable")
         self.type = type.upper()
         self.variables = variables
 
     @typechecked
+    def __deepcopy__(self, memo) -> Tuple:
+        return Tuple(self.type, deepcopy(self.variables, memo))
+
+    @typechecked
     def __repr__(self) -> str:
         output = f"\\text{{{self.type}}}("
         for variable in self.variables:
             if isinstance(variable, dc.Variable):
                 output += f"\\text{{{variable.name}}}, "
             elif isinstance(variable, dc.PRIMITIVE_TYPES):
                 output += f'\\text{{"{variable}"}}, '
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/atoms/Equals.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/atoms/Equals.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 from typing import Any, Optional
 
 import relational_calculus.domain_calculus as dc
 
 
@@ -15,14 +17,18 @@
         right: dc.PRIMITIVE_TYPES | dc.Variable,
     ) -> None:
         super().__init__([])
         self.left = left
         self.right = right
 
     @typechecked
+    def __deepcopy__(self, memo) -> Equals:
+        return Equals(deepcopy(self.left, memo), deepcopy(self.right, memo))
+
+    @typechecked
     def __repr__(self) -> str:
         return f"{self.left} = {self.right}"
 
     @typechecked
     def __eq__(self, other: Any) -> bool:
         return (
             isinstance(other, Equals)
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 from typing import Any, Optional
 
 import relational_calculus.domain_calculus as dc
 
 
-class GreaterEquals(dc.Formula):
+class LessEquals(dc.Formula):
     @typechecked
     def __init__(
         self,
         left: dc.PRIMITIVE_TYPES | dc.Variable,
         right: dc.PRIMITIVE_TYPES | dc.Variable,
     ) -> None:
         super().__init__([])
         self.left = left
         self.right = right
 
     @typechecked
+    def __deepcopy__(self, memo) -> LessEquals:
+        return LessEquals(deepcopy(self.left, memo), deepcopy(self.right, memo))
+
+    @typechecked
     def __repr__(self) -> str:
-        return f"{self.left} \\geq {self.right}"
+        return f"{self.left} \\leq {self.right}"
 
     @typechecked
     def __eq__(self, other: Any) -> bool:
         return (
-            isinstance(other, GreaterEquals)
+            isinstance(other, LessEquals)
             and self.left == other.left
             and self.right == other.right
         )
 
     @typechecked
     def _to_sql(self) -> Optional[str]:
         if isinstance(self.left, dc.Variable):
@@ -37,15 +43,15 @@
         else:
             left_string = f"{str(self.left)}"
         if isinstance(self.right, dc.Variable):
             right_string = f'"{self.right.name}"'
         else:
             right_string = f"{str(self.right)}"
 
-        return f"{left_string} >= {right_string}"
+        return f"{left_string} <= {right_string}"
 
     @typechecked
     def _to_normal_form(self) -> dc.Formula:
         return self
 
     @typechecked
     def contains_variable(self, variable: dc.Variable) -> bool:
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/atoms/LessThan.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 from typing import Any, Optional
 
 import relational_calculus.domain_calculus as dc
 
 
-class GreaterThan(dc.Formula):
+class LessThan(dc.Formula):
     @typechecked
     def __init__(
         self,
         left: dc.PRIMITIVE_TYPES | dc.Variable,
         right: dc.PRIMITIVE_TYPES | dc.Variable,
     ) -> None:
         super().__init__([])
         self.left = left
         self.right = right
 
     @typechecked
+    def __deepcopy__(self, memo) -> LessThan:
+        return LessThan(deepcopy(self.left, memo), deepcopy(self.right, memo))
+
+    @typechecked
     def __repr__(self) -> str:
-        return f"{self.left} > {self.right}"
+        return f"{self.left} < {self.right}"
 
     @typechecked
     def __eq__(self, other: Any) -> bool:
         return (
-            isinstance(other, GreaterThan)
+            isinstance(other, LessThan)
             and self.left == other.left
             and self.right == other.right
         )
 
     @typechecked
     def _to_sql(self) -> Optional[str]:
         if isinstance(self.left, dc.Variable):
@@ -37,15 +43,15 @@
         else:
             left_string = f"{str(self.left)}"
         if isinstance(self.right, dc.Variable):
             right_string = f'"{self.right.name}"'
         else:
             right_string = f"{str(self.right)}"
 
-        return f"{left_string} > {right_string}"
+        return f"{left_string} < {right_string}"
 
     @typechecked
     def _to_normal_form(self) -> dc.Formula:
         return self
 
     @typechecked
     def contains_variable(self, variable: dc.Variable) -> bool:
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/atoms/LessEquals.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/atoms/GreaterEquals.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 from typing import Any, Optional
 
 import relational_calculus.domain_calculus as dc
 
 
-class LessEquals(dc.Formula):
+class GreaterEquals(dc.Formula):
     @typechecked
     def __init__(
         self,
         left: dc.PRIMITIVE_TYPES | dc.Variable,
         right: dc.PRIMITIVE_TYPES | dc.Variable,
     ) -> None:
         super().__init__([])
         self.left = left
         self.right = right
 
     @typechecked
+    def __deepcopy__(self, memo) -> GreaterEquals:
+        return GreaterEquals(deepcopy(self.left, memo), deepcopy(self.right, memo))
+
+    @typechecked
     def __repr__(self) -> str:
-        return f"{self.left} \\leq {self.right}"
+        return f"{self.left} \\geq {self.right}"
 
     @typechecked
     def __eq__(self, other: Any) -> bool:
         return (
-            isinstance(other, LessEquals)
+            isinstance(other, GreaterEquals)
             and self.left == other.left
             and self.right == other.right
         )
 
     @typechecked
     def _to_sql(self) -> Optional[str]:
         if isinstance(self.left, dc.Variable):
@@ -37,15 +43,15 @@
         else:
             left_string = f"{str(self.left)}"
         if isinstance(self.right, dc.Variable):
             right_string = f'"{self.right.name}"'
         else:
             right_string = f"{str(self.right)}"
 
-        return f"{left_string} <= {right_string}"
+        return f"{left_string} >= {right_string}"
 
     @typechecked
     def _to_normal_form(self) -> dc.Formula:
         return self
 
     @typechecked
     def contains_variable(self, variable: dc.Variable) -> bool:
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/atoms/LessThan.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/atoms/GreaterThan.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,41 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 from typing import Any, Optional
 
 import relational_calculus.domain_calculus as dc
 
 
-class LessThan(dc.Formula):
+class GreaterThan(dc.Formula):
     @typechecked
     def __init__(
         self,
         left: dc.PRIMITIVE_TYPES | dc.Variable,
         right: dc.PRIMITIVE_TYPES | dc.Variable,
     ) -> None:
         super().__init__([])
         self.left = left
         self.right = right
 
     @typechecked
+    def __deepcopy__(self, memo) -> GreaterThan:
+        return GreaterThan(deepcopy(self.left, memo), deepcopy(self.right, memo))
+
+    @typechecked
     def __repr__(self) -> str:
-        return f"{self.left} < {self.right}"
+        return f"{self.left} > {self.right}"
 
     @typechecked
     def __eq__(self, other: Any) -> bool:
         return (
-            isinstance(other, LessThan)
+            isinstance(other, GreaterThan)
             and self.left == other.left
             and self.right == other.right
         )
 
     @typechecked
     def _to_sql(self) -> Optional[str]:
         if isinstance(self.left, dc.Variable):
@@ -37,15 +43,15 @@
         else:
             left_string = f"{str(self.left)}"
         if isinstance(self.right, dc.Variable):
             right_string = f'"{self.right.name}"'
         else:
             right_string = f"{str(self.right)}"
 
-        return f"{left_string} < {right_string}"
+        return f"{left_string} > {right_string}"
 
     @typechecked
     def _to_normal_form(self) -> dc.Formula:
         return self
 
     @typechecked
     def contains_variable(self, variable: dc.Variable) -> bool:
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/connectives/And.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/connectives/Or.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,117 +1,123 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 from typing import Any, Optional
 
 import relational_calculus.domain_calculus as dc
 
 
-class And(dc.Formula):
+class Or(dc.Formula):
     @typechecked
     def __init__(self, child1: dc.Formula, child2: dc.Formula) -> None:
         super().__init__([child1, child2])
 
     @typechecked
+    def __deepcopy__(self, memo) -> Or:
+        return Or(deepcopy(self.children[0], memo), deepcopy(self.children[1], memo))
+
+    @typechecked
     def __repr__(self) -> str:
         left = self.children[0]
         right = self.children[1]
 
-        if isinstance(self.children[0], And):
+        if isinstance(self.children[0], Or):
             left = (
                 f"{self.children[0].children[0]} \\land {self.children[0].children[1]}"
             )
         elif not isinstance(self.children[0], dc.Not | dc.ATOM_TYPES | dc.Tuple):
             left = f"({left})"
 
-        if isinstance(self.children[1], And):
+        if isinstance(self.children[1], Or):
             right = (
                 f"{self.children[1].children[0]} \\land {self.children[1].children[1]}"
             )
         elif not isinstance(self.children[1], dc.Not | dc.ATOM_TYPES | dc.Tuple):
             right = f"({right})"
 
-        return f"{left} \\land {right}"
+        return f"{left} \\lor {right}"
 
     @typechecked
     def __eq__(self, other: Any) -> bool:
         return (
-            isinstance(other, And)
+            isinstance(other, Or)
             and self.children[0] == other.children[0]
             and self.children[1] == other.children[1]
         )
 
     @typechecked
     def _to_sql(self) -> Optional[str]:
-        return f"({self.children[0].to_sql()} AND {self.children[1].to_sql()})"
+        return f"({self.children[0].to_sql()} OR {self.children[1].to_sql()})"
 
     @typechecked
     def _to_normal_form(self) -> dc.Formula:
         if isinstance(self.children[0], dc.Exists):
             self.children[0] = self.children[0]._to_normal_form()
             variable = self.children[0].variable
             if self.children[1].contains_variable(variable):
-                return And(
+                return Or(
                     self.children[0].rename_variable(variable), self.children[1]
                 )._to_normal_form()
             else:
                 return dc.Exists(
                     variable,
-                    And(
+                    Or(
                         self.children[0].children[0], self.children[1]
                     )._to_normal_form(),
                 )
 
         if isinstance(self.children[0], dc.Forall):
             self.children[0] = self.children[0]._to_normal_form()
             variable = self.children[0].variable
             if self.children[1].contains_variable(variable):
-                return And(
+                return Or(
                     self.children[0].rename_variable(variable), self.children[1]
                 )._to_normal_form()
             else:
                 return dc.Forall(
                     variable,
-                    And(
+                    Or(
                         self.children[0].children[0], self.children[1]
                     )._to_normal_form(),
                 )
 
         if isinstance(self.children[1], dc.Exists):
             self.children[1] = self.children[1]._to_normal_form()
             variable = self.children[1].variable
             if self.children[0].contains_variable(variable):
-                return And(
+                return Or(
                     self.children[0], self.children[1].rename_variable(variable)
                 )._to_normal_form()
             else:
                 return dc.Exists(
                     variable,
-                    And(
+                    Or(
                         self.children[0], self.children[1].children[0]
                     )._to_normal_form(),
                 )
 
         if isinstance(self.children[1], dc.Forall):
             self.children[1] = self.children[1]._to_normal_form()
             variable = self.children[1].variable
             if self.children[0].contains_variable(variable):
-                return And(
+                return Or(
                     self.children[0], self.children[1].rename_variable(variable)
                 )._to_normal_form()
             else:
                 return dc.Forall(
                     variable,
-                    And(
+                    Or(
                         self.children[0], self.children[1].children[0]
                     )._to_normal_form(),
                 )
 
-        return And(
+        return Or(
             self.children[0]._to_normal_form(), self.children[1]._to_normal_form()
         )
 
     @typechecked
     def contains_variable(self, variable: dc.Variable) -> bool:
         return self.children[0].contains_variable(variable) or self.children[
             1
@@ -129,15 +135,15 @@
             variable
         ) or self.children[1].contains_variable_quantification(variable)
 
     @typechecked
     def _rename_variable(
         self, old_variable: dc.Variable, new_variable: dc.Variable
     ) -> dc.Formula:
-        return And(
+        return Or(
             self.children[0]._rename_variable(old_variable, new_variable),
             self.children[1]._rename_variable(old_variable, new_variable),
         )
 
     @typechecked
     def _prune_tuple_atoms(self) -> dc.Formula | None:
         left = self.children[0]._prune_tuple_atoms()
@@ -146,15 +152,15 @@
         if left is None and right is None:
             return None
         elif left is None:
             return right
         elif right is None:
             return left
         else:
-            return And(left, right)
+            return Or(left, right)
 
     @typechecked
     def get_used_variables(self) -> set[dc.Variable]:
         return (
             self.children[0]
             .get_used_variables()
             .union(self.children[1].get_used_variables())
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/connectives/Not.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/connectives/Not.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,28 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 from typing import Any, Optional
 
 import relational_calculus.domain_calculus as dc
 
 
 class Not(dc.Formula):
     @typechecked
     def __init__(self, child: dc.Formula) -> None:
         super().__init__([child])
 
     @typechecked
+    def __deepcopy__(self, memo) -> Not:
+        return Not(deepcopy(self.children[0], memo))
+
+    @typechecked
     def __repr__(self) -> str:
         if isinstance(self.children[0], dc.And | dc.Or):
             return f"\\neg({self.children[0]})"
         return f"\\neg {self.children[0]}"
 
     @typechecked
     def __eq__(self, other: Any) -> bool:
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/connectives/Or.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/connectives/And.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,117 +1,123 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 from typing import Any, Optional
 
 import relational_calculus.domain_calculus as dc
 
 
-class Or(dc.Formula):
+class And(dc.Formula):
     @typechecked
     def __init__(self, child1: dc.Formula, child2: dc.Formula) -> None:
         super().__init__([child1, child2])
 
     @typechecked
+    def __deepcopy__(self, memo) -> And:
+        return And(deepcopy(self.children[0], memo), deepcopy(self.children[1], memo))
+
+    @typechecked
     def __repr__(self) -> str:
         left = self.children[0]
         right = self.children[1]
 
-        if isinstance(self.children[0], Or):
+        if isinstance(self.children[0], And):
             left = (
                 f"{self.children[0].children[0]} \\land {self.children[0].children[1]}"
             )
         elif not isinstance(self.children[0], dc.Not | dc.ATOM_TYPES | dc.Tuple):
             left = f"({left})"
 
-        if isinstance(self.children[1], Or):
+        if isinstance(self.children[1], And):
             right = (
                 f"{self.children[1].children[0]} \\land {self.children[1].children[1]}"
             )
         elif not isinstance(self.children[1], dc.Not | dc.ATOM_TYPES | dc.Tuple):
             right = f"({right})"
 
-        return f"{left} \\lor {right}"
+        return f"{left} \\land {right}"
 
     @typechecked
     def __eq__(self, other: Any) -> bool:
         return (
-            isinstance(other, Or)
+            isinstance(other, And)
             and self.children[0] == other.children[0]
             and self.children[1] == other.children[1]
         )
 
     @typechecked
     def _to_sql(self) -> Optional[str]:
-        return f"({self.children[0].to_sql()} OR {self.children[1].to_sql()})"
+        return f"({self.children[0].to_sql()} AND {self.children[1].to_sql()})"
 
     @typechecked
     def _to_normal_form(self) -> dc.Formula:
         if isinstance(self.children[0], dc.Exists):
             self.children[0] = self.children[0]._to_normal_form()
             variable = self.children[0].variable
             if self.children[1].contains_variable(variable):
-                return Or(
+                return And(
                     self.children[0].rename_variable(variable), self.children[1]
                 )._to_normal_form()
             else:
                 return dc.Exists(
                     variable,
-                    Or(
+                    And(
                         self.children[0].children[0], self.children[1]
                     )._to_normal_form(),
                 )
 
         if isinstance(self.children[0], dc.Forall):
             self.children[0] = self.children[0]._to_normal_form()
             variable = self.children[0].variable
             if self.children[1].contains_variable(variable):
-                return Or(
+                return And(
                     self.children[0].rename_variable(variable), self.children[1]
                 )._to_normal_form()
             else:
                 return dc.Forall(
                     variable,
-                    Or(
+                    And(
                         self.children[0].children[0], self.children[1]
                     )._to_normal_form(),
                 )
 
         if isinstance(self.children[1], dc.Exists):
             self.children[1] = self.children[1]._to_normal_form()
             variable = self.children[1].variable
             if self.children[0].contains_variable(variable):
-                return Or(
+                return And(
                     self.children[0], self.children[1].rename_variable(variable)
                 )._to_normal_form()
             else:
                 return dc.Exists(
                     variable,
-                    Or(
+                    And(
                         self.children[0], self.children[1].children[0]
                     )._to_normal_form(),
                 )
 
         if isinstance(self.children[1], dc.Forall):
             self.children[1] = self.children[1]._to_normal_form()
             variable = self.children[1].variable
             if self.children[0].contains_variable(variable):
-                return Or(
+                return And(
                     self.children[0], self.children[1].rename_variable(variable)
                 )._to_normal_form()
             else:
                 return dc.Forall(
                     variable,
-                    Or(
+                    And(
                         self.children[0], self.children[1].children[0]
                     )._to_normal_form(),
                 )
 
-        return Or(
+        return And(
             self.children[0]._to_normal_form(), self.children[1]._to_normal_form()
         )
 
     @typechecked
     def contains_variable(self, variable: dc.Variable) -> bool:
         return self.children[0].contains_variable(variable) or self.children[
             1
@@ -129,15 +135,15 @@
             variable
         ) or self.children[1].contains_variable_quantification(variable)
 
     @typechecked
     def _rename_variable(
         self, old_variable: dc.Variable, new_variable: dc.Variable
     ) -> dc.Formula:
-        return Or(
+        return And(
             self.children[0]._rename_variable(old_variable, new_variable),
             self.children[1]._rename_variable(old_variable, new_variable),
         )
 
     @typechecked
     def _prune_tuple_atoms(self) -> dc.Formula | None:
         left = self.children[0]._prune_tuple_atoms()
@@ -146,15 +152,15 @@
         if left is None and right is None:
             return None
         elif left is None:
             return right
         elif right is None:
             return left
         else:
-            return Or(left, right)
+            return And(left, right)
 
     @typechecked
     def get_used_variables(self) -> set[dc.Variable]:
         return (
             self.children[0]
             .get_used_variables()
             .union(self.children[1].get_used_variables())
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 from typing import Any, Optional
 
 import relational_calculus.domain_calculus as dc
 
 
-class Exists(dc.Formula):
+class Forall(dc.Formula):
     @typechecked
     def __init__(
         self, variable: dc.Variable | set[dc.Variable], child: dc.Formula
     ) -> None:
         super().__init__([child])
         self.variable = variable
         if isinstance(self.variable, set) and len(self.variable) == 0:
             raise Exception("Must quantify at least one variable")
 
     @typechecked
+    def __deepcopy__(self, memo) -> Forall:
+        return Forall(deepcopy(self.variable, memo), deepcopy(self.children[0], memo))
+
+    @typechecked
     def __repr__(self) -> str:
         if isinstance(self.variable, set):
             forall_str = ""
             for var in self.variable:
                 forall_str += f"{var.name}, "
             forall_str = forall_str[: -len(", ")]
         else:
             forall_str = self.variable.name
 
-        return f"\\exists_{{{forall_str}}}({self.children[0]})"
+        return f"\\forall_{{{forall_str}}}({self.children[0]})"
 
     @typechecked
     def __eq__(self, other: Any) -> bool:
         return (
-            isinstance(other, Exists)
+            isinstance(other, Forall)
             and self.variable == other.variable
             and self.children[0] == other.children[0]
         )
 
     @typechecked
     def _to_sql(self) -> Optional[str]:
         return None
 
     @typechecked
     def _to_normal_form(self) -> dc.Formula:
         if isinstance(self.variable, set):
             formula = self.children[0]._to_normal_form()
             for var in self.variable:
-                formula = Exists(var, formula)
+                formula = Forall(var, formula)
             return formula
-        return Exists(self.variable, self.children[0]._to_normal_form())
+        return Forall(self.variable, self.children[0]._to_normal_form())
 
     @typechecked
     def contains_variable(self, variable: dc.Variable) -> bool:
         return (
             variable in self.variable
             if isinstance(self.variable, set)
             else self.variable == variable
@@ -70,30 +76,26 @@
 
     @typechecked
     def _rename_variable(
         self, old_variable: dc.Variable, new_variable: dc.Variable
     ) -> dc.Formula:
         if isinstance(self.variable, set):
             new_set = set(self.variable)
-            for var in self.variable:
-                if var == old_variable:
-                    new_set.remove(var)
-                    new_set.add(new_variable)
-            return Exists(
+            if old_variable in self.variable:
+                new_set.remove(old_variable)
+                new_set.add(new_variable)
+            return Forall(
                 new_set, self.children[0]._rename_variable(old_variable, new_variable)
             )
         else:
             if self.variable == old_variable:
-                return Exists(
-                    new_variable,
-                    self.children[0]._rename_variable(old_variable, new_variable),
-                )
+                return Forall(new_variable, self.children[0])
             else:
-                return Exists(
-                    self.variable,
+                return Forall(
+                    new_variable,
                     self.children[0]._rename_variable(old_variable, new_variable),
                 )
 
     @typechecked
     def _prune_tuple_atoms(self) -> dc.Formula | None:
         new_child = self.children[0]._prune_tuple_atoms()
         if new_child is None:
@@ -101,19 +103,19 @@
         if isinstance(self.variable, set):
             new_set = set(self.variable)
             for var in self.variable:
                 if not new_child.contains_variable_typing(var):
                     new_set.remove(var)
             if len(new_set) == 0:
                 return new_child
-            return Exists(new_set, new_child)
+            return Forall(new_set, new_child)
         else:
             if not new_child.contains_variable_typing(self.variable):
                 return new_child
-            return Exists(self.variable, new_child)
+            return Forall(self.variable, new_child)
 
     @typechecked
     def get_used_variables(self) -> set[dc.Variable]:
         child_vars = self.children[0].get_used_variables()
         if isinstance(self.variable, set):
             return child_vars.union(self.variable)
         return child_vars.union({self.variable})
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/domain_calculus/formulas/quantifiers/Forall.py` & `dbis-relational-calculus-1.0.7/relational_calculus/domain_calculus/formulas/quantifiers/Exists.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,64 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 from typing import Any, Optional
 
 import relational_calculus.domain_calculus as dc
 
 
-class Forall(dc.Formula):
+class Exists(dc.Formula):
     @typechecked
     def __init__(
         self, variable: dc.Variable | set[dc.Variable], child: dc.Formula
     ) -> None:
         super().__init__([child])
         self.variable = variable
         if isinstance(self.variable, set) and len(self.variable) == 0:
             raise Exception("Must quantify at least one variable")
 
     @typechecked
+    def __deepcopy__(self, memo) -> Exists:
+        return Exists(deepcopy(self.variable, memo), deepcopy(self.children[0], memo))
+
+    @typechecked
     def __repr__(self) -> str:
         if isinstance(self.variable, set):
             forall_str = ""
             for var in self.variable:
                 forall_str += f"{var.name}, "
             forall_str = forall_str[: -len(", ")]
         else:
             forall_str = self.variable.name
 
-        return f"\\forall_{{{forall_str}}}({self.children[0]})"
+        return f"\\exists_{{{forall_str}}}({self.children[0]})"
 
     @typechecked
     def __eq__(self, other: Any) -> bool:
         return (
-            isinstance(other, Forall)
+            isinstance(other, Exists)
             and self.variable == other.variable
             and self.children[0] == other.children[0]
         )
 
     @typechecked
     def _to_sql(self) -> Optional[str]:
         return None
 
     @typechecked
     def _to_normal_form(self) -> dc.Formula:
         if isinstance(self.variable, set):
             formula = self.children[0]._to_normal_form()
             for var in self.variable:
-                formula = Forall(var, formula)
+                formula = Exists(var, formula)
             return formula
-        return Forall(self.variable, self.children[0]._to_normal_form())
+        return Exists(self.variable, self.children[0]._to_normal_form())
 
     @typechecked
     def contains_variable(self, variable: dc.Variable) -> bool:
         return (
             variable in self.variable
             if isinstance(self.variable, set)
             else self.variable == variable
@@ -70,46 +76,50 @@
 
     @typechecked
     def _rename_variable(
         self, old_variable: dc.Variable, new_variable: dc.Variable
     ) -> dc.Formula:
         if isinstance(self.variable, set):
             new_set = set(self.variable)
-            if old_variable in self.variable:
-                new_set.remove(old_variable)
-                new_set.add(new_variable)
-            return Forall(
+            for var in self.variable:
+                if var == old_variable:
+                    new_set.remove(var)
+                    new_set.add(new_variable)
+            return Exists(
                 new_set, self.children[0]._rename_variable(old_variable, new_variable)
             )
         else:
             if self.variable == old_variable:
-                return Forall(new_variable, self.children[0])
-            else:
-                return Forall(
+                return Exists(
                     new_variable,
                     self.children[0]._rename_variable(old_variable, new_variable),
                 )
+            else:
+                return Exists(
+                    self.variable,
+                    self.children[0]._rename_variable(old_variable, new_variable),
+                )
 
     @typechecked
     def _prune_tuple_atoms(self) -> dc.Formula | None:
         new_child = self.children[0]._prune_tuple_atoms()
         if new_child is None:
             return None
         if isinstance(self.variable, set):
             new_set = set(self.variable)
             for var in self.variable:
                 if not new_child.contains_variable_typing(var):
                     new_set.remove(var)
             if len(new_set) == 0:
                 return new_child
-            return Forall(new_set, new_child)
+            return Exists(new_set, new_child)
         else:
             if not new_child.contains_variable_typing(self.variable):
                 return new_child
-            return Forall(self.variable, new_child)
+            return Exists(self.variable, new_child)
 
     @typechecked
     def get_used_variables(self) -> set[dc.Variable]:
         child_vars = self.children[0].get_used_variables()
         if isinstance(self.variable, set):
             return child_vars.union(self.variable)
         return child_vars.union({self.variable})
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/TupleCalculus.py` & `dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/TupleCalculus.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 import relational_calculus.tuple_calculus as tc
 
 
 class TupleCalculus:
     @typechecked
@@ -16,14 +18,22 @@
         formula : Formula
             The formula that every result has to satisfy.
         """
         self.result = result
         self.formula = formula
 
     @typechecked
+    def __copy__(self) -> TupleCalculus:
+        return deepcopy(self)
+
+    @typechecked
+    def __deepcopy__(self, memo) -> TupleCalculus:
+        return TupleCalculus(deepcopy(self.result, memo), deepcopy(self.formula, memo))
+
+    @typechecked
     def verify(self) -> bool:
         """
         Verify the correctness of the result/formula combination (e.g. one must specify the type of a variable before returning it).
 
         Returns
         -------
         bool
@@ -63,14 +73,31 @@
             If the query should be optimized, by default True
 
         Returns
         -------
         str
             The SQL query.
         """
+        return deepcopy(self).__to_sql(optimize)
+
+    @typechecked
+    def __to_sql(self, optimize: bool) -> str:
+        """
+        Convert the domain calculus to a SQL query.
+
+        Parameters
+        ----------
+        optimize : bool
+            If the query should be optimized
+
+        Returns
+        -------
+        str
+            The SQL query.
+        """
         # Get Types of return variables
         variables = set()
         for x in self.result.attributes:
             if isinstance(x, tc.Variable):
                 variables.add(x)
             elif isinstance(x, tuple):
                 variable, _ = x
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/__init__.py` & `dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/__init__.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/Formula.py` & `dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/Formula.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from __future__ import annotations
 
 from abc import abstractclassmethod
+from copy import deepcopy
 
 from docstring_inheritance import NumpyDocstringInheritanceMeta
 from typeguard import typechecked
 
 import relational_calculus.tuple_calculus as tc
 
 
@@ -21,14 +22,39 @@
         ----------
         children : list[Formula]
             Each implementation of formula can hold a list of children that it is composed of.
         """
         self.children = children
 
     @typechecked
+    def __copy__(self) -> Formula:
+        """
+        Returns a copy of the formula.
+
+        Returns
+        -------
+        Formula
+            A copy of the formula.
+        """
+        return deepcopy(self)
+
+    @typechecked
+    @abstractclassmethod
+    def __deepcopy__(self, memo) -> Formula:
+        """
+        Returns a deep copy of the formula.
+
+        Returns
+        -------
+        Formula
+            A deep copy of the formula.
+        """
+        pass
+
+    @typechecked
     @abstractclassmethod
     def __repr__(self) -> str:
         """
         Returs a string representation of a given formula formatted in Latex Math Mode.
 
         Returns
         -------
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/Variable.py` & `dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/Variable.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 import relational_calculus.tuple_calculus as tc
 
 
 class Variable(tc.Formula):
     """
@@ -21,14 +23,18 @@
             The relation / type that this variable is of.
         """
         super().__init__([])
         self.name = name.lower()
         self.type = type.upper()
 
     @typechecked
+    def __deepcopy__(self, memo) -> Variable:
+        return Variable(deepcopy(self.name, memo), deepcopy(self.type, memo))
+
+    @typechecked
     def __repr__(self) -> str:
         return f"\\text{{{self.name}}} \\in \\text{{{self.type}}}"
 
     @typechecked
     def __eq__(self, other) -> bool:
         return (
             isinstance(other, Variable)
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/atoms/Equals.py` & `dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/atoms/Equals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 import relational_calculus.tuple_calculus as tc
 
 
 class Equals(tc.Formula):
     """
@@ -25,14 +27,18 @@
             Right-hand side of the comparison.
         """
         super().__init__([])
         self.left = left
         self.right = right
 
     @typechecked
+    def __deepcopy__(self, memo) -> Equals:
+        return Equals(deepcopy(self.left, memo), deepcopy(self.right, memo))
+
+    @typechecked
     def __repr__(self) -> str:
         if isinstance(self.left, tuple):  # (variable, attr_name)
             left_string = f"\\text{{{self.left[0].name}.{self.left[1]}}}"
         else:
             left_string = f"\\text{{{self.left}}}"
         if isinstance(self.right, tuple):  # (variable, attr_name)
             right_string = f"\\text{{{self.right[0].name}.{self.right[1]}}}"
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py` & `dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 import relational_calculus.tuple_calculus as tc
 
 
-class GreaterEquals(tc.Formula):
+class LessEquals(tc.Formula):
     """
-    A class representing the comparison '>='.
+    A class representing the comparison '<='.
     """
 
     @typechecked
     def __init__(
         self,
         left: tuple[tc.Variable, str] | tc.PRIMITIVE_TYPES,
         right: tuple[tc.Variable, str] | tc.PRIMITIVE_TYPES,
@@ -25,29 +27,33 @@
             Right-hand side of the comparison.
         """
         super().__init__([])
         self.left = left
         self.right = right
 
     @typechecked
+    def __deepcopy__(self, memo) -> LessEquals:
+        return LessEquals(deepcopy(self.left, memo), deepcopy(self.right, memo))
+
+    @typechecked
     def __repr__(self) -> str:
         if isinstance(self.left, tuple):  # (variable, attr_name)
             left_string = f"\\text{{{self.left[0].name}.{self.left[1]}}}"
         else:
             left_string = f"\\text{{{self.left}}}"
         if isinstance(self.right, tuple):  # (variable, attr_name)
             right_string = f"\\text{{{self.right[0].name}.{self.right[1]}}}"
         else:
             right_string = f"\\text{{{self.right}}}"
-        return f"{left_string} >= {right_string}"
+        return f"{left_string} \\leq {right_string}"
 
     @typechecked
     def __eq__(self, other) -> bool:
         return (
-            isinstance(other, GreaterEquals)
+            isinstance(other, LessEquals)
             and self.left == other.left
             and self.right == other.right
         )
 
     @typechecked
     def expand_quantifiers(self) -> tc.Formula:
         return self
@@ -68,15 +74,15 @@
             left_string = f"{self.left[0].name}.{self.left[1]}"
         else:
             left_string = f"{self.left}"
         if isinstance(self.right, tuple):  # (variable, attr_name)
             right_string = f"{self.right[0].name}.{self.right[1]}"
         else:
             right_string = f"{self.right}"
-        return f"{left_string} >= {right_string}"
+        return f"{left_string} <= {right_string}"
 
     @typechecked
     def flatten_quantifiers(self) -> tc.Formula:
         return self
 
     @typechecked
     def _to_normal_form(self) -> tc.Formula:
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py` & `dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/atoms/GreaterEquals.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 import relational_calculus.tuple_calculus as tc
 
 
-class GreaterThan(tc.Formula):
+class GreaterEquals(tc.Formula):
     """
-    A class representing the comparison '>'.
+    A class representing the comparison '>='.
     """
 
     @typechecked
     def __init__(
         self,
         left: tuple[tc.Variable, str] | tc.PRIMITIVE_TYPES,
         right: tuple[tc.Variable, str] | tc.PRIMITIVE_TYPES,
@@ -25,29 +27,33 @@
             Right-hand side of the comparison.
         """
         super().__init__([])
         self.left = left
         self.right = right
 
     @typechecked
+    def __deepcopy__(self, memo) -> GreaterEquals:
+        return GreaterEquals(deepcopy(self.left, memo), deepcopy(self.right, memo))
+
+    @typechecked
     def __repr__(self) -> str:
         if isinstance(self.left, tuple):  # (variable, attr_name)
             left_string = f"\\text{{{self.left[0].name}.{self.left[1]}}}"
         else:
             left_string = f"\\text{{{self.left}}}"
         if isinstance(self.right, tuple):  # (variable, attr_name)
             right_string = f"\\text{{{self.right[0].name}.{self.right[1]}}}"
         else:
             right_string = f"\\text{{{self.right}}}"
-        return f"{left_string} > {right_string}"
+        return f"{left_string} >= {right_string}"
 
     @typechecked
     def __eq__(self, other) -> bool:
         return (
-            isinstance(other, GreaterThan)
+            isinstance(other, GreaterEquals)
             and self.left == other.left
             and self.right == other.right
         )
 
     @typechecked
     def expand_quantifiers(self) -> tc.Formula:
         return self
@@ -68,15 +74,15 @@
             left_string = f"{self.left[0].name}.{self.left[1]}"
         else:
             left_string = f"{self.left}"
         if isinstance(self.right, tuple):  # (variable, attr_name)
             right_string = f"{self.right[0].name}.{self.right[1]}"
         else:
             right_string = f"{self.right}"
-        return f"{left_string} > {right_string}"
+        return f"{left_string} >= {right_string}"
 
     @typechecked
     def flatten_quantifiers(self) -> tc.Formula:
         return self
 
     @typechecked
     def _to_normal_form(self) -> tc.Formula:
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/atoms/LessEquals.py` & `dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 import relational_calculus.tuple_calculus as tc
 
 
-class LessEquals(tc.Formula):
+class LessThan(tc.Formula):
     """
-    A class representing the comparison '<='.
+    A class representing the comparison '<'.
     """
 
     @typechecked
     def __init__(
         self,
         left: tuple[tc.Variable, str] | tc.PRIMITIVE_TYPES,
         right: tuple[tc.Variable, str] | tc.PRIMITIVE_TYPES,
@@ -25,29 +27,33 @@
             Right-hand side of the comparison.
         """
         super().__init__([])
         self.left = left
         self.right = right
 
     @typechecked
+    def __deepcopy__(self, memo) -> LessThan:
+        return LessThan(deepcopy(self.left, memo), deepcopy(self.right, memo))
+
+    @typechecked
     def __repr__(self) -> str:
         if isinstance(self.left, tuple):  # (variable, attr_name)
             left_string = f"\\text{{{self.left[0].name}.{self.left[1]}}}"
         else:
             left_string = f"\\text{{{self.left}}}"
         if isinstance(self.right, tuple):  # (variable, attr_name)
             right_string = f"\\text{{{self.right[0].name}.{self.right[1]}}}"
         else:
             right_string = f"\\text{{{self.right}}}"
-        return f"{left_string} \\leq {right_string}"
+        return f"{left_string} < {right_string}"
 
     @typechecked
     def __eq__(self, other) -> bool:
         return (
-            isinstance(other, LessEquals)
+            isinstance(other, LessThan)
             and self.left == other.left
             and self.right == other.right
         )
 
     @typechecked
     def expand_quantifiers(self) -> tc.Formula:
         return self
@@ -68,15 +74,15 @@
             left_string = f"{self.left[0].name}.{self.left[1]}"
         else:
             left_string = f"{self.left}"
         if isinstance(self.right, tuple):  # (variable, attr_name)
             right_string = f"{self.right[0].name}.{self.right[1]}"
         else:
             right_string = f"{self.right}"
-        return f"{left_string} <= {right_string}"
+        return f"{left_string} < {right_string}"
 
     @typechecked
     def flatten_quantifiers(self) -> tc.Formula:
         return self
 
     @typechecked
     def _to_normal_form(self) -> tc.Formula:
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/atoms/LessThan.py` & `dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/atoms/GreaterThan.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 import relational_calculus.tuple_calculus as tc
 
 
-class LessThan(tc.Formula):
+class GreaterThan(tc.Formula):
     """
-    A class representing the comparison '<'.
+    A class representing the comparison '>'.
     """
 
     @typechecked
     def __init__(
         self,
         left: tuple[tc.Variable, str] | tc.PRIMITIVE_TYPES,
         right: tuple[tc.Variable, str] | tc.PRIMITIVE_TYPES,
@@ -25,29 +27,33 @@
             Right-hand side of the comparison.
         """
         super().__init__([])
         self.left = left
         self.right = right
 
     @typechecked
+    def __deepcopy__(self, memo) -> GreaterThan:
+        return GreaterThan(deepcopy(self.left, memo), deepcopy(self.right, memo))
+
+    @typechecked
     def __repr__(self) -> str:
         if isinstance(self.left, tuple):  # (variable, attr_name)
             left_string = f"\\text{{{self.left[0].name}.{self.left[1]}}}"
         else:
             left_string = f"\\text{{{self.left}}}"
         if isinstance(self.right, tuple):  # (variable, attr_name)
             right_string = f"\\text{{{self.right[0].name}.{self.right[1]}}}"
         else:
             right_string = f"\\text{{{self.right}}}"
-        return f"{left_string} < {right_string}"
+        return f"{left_string} > {right_string}"
 
     @typechecked
     def __eq__(self, other) -> bool:
         return (
-            isinstance(other, LessThan)
+            isinstance(other, GreaterThan)
             and self.left == other.left
             and self.right == other.right
         )
 
     @typechecked
     def expand_quantifiers(self) -> tc.Formula:
         return self
@@ -68,15 +74,15 @@
             left_string = f"{self.left[0].name}.{self.left[1]}"
         else:
             left_string = f"{self.left}"
         if isinstance(self.right, tuple):  # (variable, attr_name)
             right_string = f"{self.right[0].name}.{self.right[1]}"
         else:
             right_string = f"{self.right}"
-        return f"{left_string} < {right_string}"
+        return f"{left_string} > {right_string}"
 
     @typechecked
     def flatten_quantifiers(self) -> tc.Formula:
         return self
 
     @typechecked
     def _to_normal_form(self) -> tc.Formula:
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/connectives/And.py` & `dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/connectives/And.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 import relational_calculus.tuple_calculus as tc
 
 
 class And(tc.Formula):
     """
@@ -19,14 +21,18 @@
             Left subformula.
         right : Formula
             Right subformula.
         """
         super().__init__([left, right])
 
     @typechecked
+    def __deepcopy__(self, memo) -> And:
+        return And(deepcopy(self.children[0], memo), deepcopy(self.children[1], memo))
+
+    @typechecked
     def __repr__(self) -> str:
         left = self.children[0]
         right = self.children[1]
 
         if isinstance(self.children[0], And):
             left = (
                 f"{self.children[0].children[0]} \\land {self.children[0].children[1]}"
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/connectives/Not.py` & `dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/connectives/Not.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 import relational_calculus.tuple_calculus as tc
 
 
 class Not(tc.Formula):
     """
@@ -17,14 +19,18 @@
         ----------
         child : Formula
             Subformula.
         """
         super().__init__([child])
 
     @typechecked
+    def __deepcopy__(self, memo) -> Not:
+        return Not(deepcopy(self.children[0], memo))
+
+    @typechecked
     def __repr__(self) -> str:
         if isinstance(self.children[0], tc.And | tc.Or):
             return f"\\neg({self.children[0]})"
         return f"\\neg {self.children[0]}"
 
     @typechecked
     def __eq__(self, other) -> bool:
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/connectives/Or.py` & `dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/connectives/Or.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 import relational_calculus.tuple_calculus as tc
 
 
 class Or(tc.Formula):
     """
@@ -19,14 +21,18 @@
             Left subformula.
         right : Formula
             Right subformula.
         """
         super().__init__([left, right])
 
     @typechecked
+    def __deepcopy__(self, memo) -> Or:
+        return Or(deepcopy(self.children[0], memo), deepcopy(self.children[1], memo))
+
+    @typechecked
     def __repr__(self) -> str:
         left = self.children[0]
         right = self.children[1]
 
         if isinstance(self.children[0], Or):
             left = (
                 f"{self.children[0].children[0]} \\land {self.children[0].children[1]}"
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py` & `dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/quantifiers/Exists.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 import relational_calculus.tuple_calculus as tc
 
 
 class Exists(tc.Formula):
     """
@@ -24,14 +26,18 @@
         """
         super().__init__([child])
         self.variable = variable
         if isinstance(self.variable, set) and len(self.variable) == 0:
             raise Exception("Must quantify at least one variable")
 
     @typechecked
+    def __deepcopy__(self, memo) -> Exists:
+        return Exists(deepcopy(self.variable, memo), deepcopy(self.children[0], memo))
+
+    @typechecked
     def __repr__(self) -> str:
         if isinstance(self.variable, set):
             forall_str = ""
             type_str = ""
             for var in self.variable:
                 forall_str += f"{var.name}, "
                 type_str += f"\\text{{{var.name}}} \\in \\text{{{var.type}}} \\land "
```

### Comparing `dbis-relational-calculus-1.0.6/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py` & `dbis-relational-calculus-1.0.7/relational_calculus/tuple_calculus/formulas/quantifiers/Forall.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 from __future__ import annotations
 
+from copy import deepcopy
+
 from typeguard import typechecked
 
 import relational_calculus.tuple_calculus as tc
 
 
 class Forall(tc.Formula):
     """
@@ -24,14 +26,18 @@
         """
         super().__init__([child])
         self.variable = variable
         if isinstance(self.variable, set) and len(self.variable) == 0:
             raise Exception("Must quantify at least one variable")
 
     @typechecked
+    def __deepcopy__(self, memo) -> Forall:
+        return Forall(deepcopy(self.variable, memo), deepcopy(self.children[0], memo))
+
+    @typechecked
     def __repr__(self) -> str:
         if isinstance(self.variable, set):
             forall_str = ""
             type_str = ""
             for var in self.variable:
                 forall_str += f"{var.name}, "
                 type_str += f"\\text{{{var.name}}} \\in \\text{{{var.type}}} \\land "
```

### Comparing `dbis-relational-calculus-1.0.6/tests/test_domain_calculus_sql.py` & `dbis-relational-calculus-1.0.7/tests/test_domain_calculus_sql.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.6/tests/test_domain_calculus_validity.py` & `dbis-relational-calculus-1.0.7/tests/test_domain_calculus_validity.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.6/tests/test_tuple_calculus_attribute_access.py` & `dbis-relational-calculus-1.0.7/tests/test_tuple_calculus_attribute_access.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.6/tests/test_tuple_calculus_sql.py` & `dbis-relational-calculus-1.0.7/tests/test_tuple_calculus_sql.py`

 * *Files identical despite different names*

### Comparing `dbis-relational-calculus-1.0.6/tests/test_tuple_calculus_validity.py` & `dbis-relational-calculus-1.0.7/tests/test_tuple_calculus_validity.py`

 * *Files identical despite different names*

