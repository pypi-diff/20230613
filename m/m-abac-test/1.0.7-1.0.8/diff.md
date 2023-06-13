# Comparing `tmp/m-abac-test-1.0.7.tar.gz` & `tmp/m-abac-test-1.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "m-abac-test-1.0.7.tar", last modified: Mon Jun 12 11:11:33 2023, max compression
+gzip compressed data, was "m-abac-test-1.0.8.tar", last modified: Tue Jun 13 08:41:52 2023, max compression
```

## Comparing `m-abac-test-1.0.7.tar` & `m-abac-test-1.0.8.tar`

### file list

```diff
@@ -1,99 +1,99 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.982998 m-abac-test-1.0.7/
--rw-r--r--   0 root         (0) root         (0)     1746 2023-06-12 11:11:33.982998 m-abac-test-1.0.7/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.921997 m-abac-test-1.0.7/m_abac_test.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1746 2023-06-12 11:11:33.000000 m-abac-test-1.0.7/m_abac_test.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3851 2023-06-12 11:11:33.000000 m-abac-test-1.0.7/m_abac_test.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-12 11:11:33.000000 m-abac-test-1.0.7/m_abac_test.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      100 2023-06-12 11:11:33.000000 m-abac-test-1.0.7/m_abac_test.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-06-12 11:11:33.000000 m-abac-test-1.0.7/m_abac_test.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.909997 m-abac-test-1.0.7/mobio/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.909997 m-abac-test-1.0.7/mobio/libs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.926997 m-abac-test-1.0.7/mobio/libs/abac/
--rw-r--r--   0 root         (0) root         (0)       70 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.928997 m-abac-test-1.0.7/mobio/libs/abac/adapter/
--rw-r--r--   0 root         (0) root         (0)      267 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/adapter/__init__.py
--rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/adapter/adapter.py
--rw-r--r--   0 root         (0) root         (0)    15511 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/adapter/elasticsearch_adapter.py
--rw-r--r--   0 root         (0) root         (0)     7941 2023-06-12 11:10:01.000000 m-abac-test-1.0.7/mobio/libs/abac/call_api.py
--rw-r--r--   0 root         (0) root         (0)     1243 2023-05-24 07:57:21.000000 m-abac-test-1.0.7/mobio/libs/abac/config.py
--rw-r--r--   0 root         (0) root         (0)    15699 2023-06-12 11:10:01.000000 m-abac-test-1.0.7/mobio/libs/abac/pdp.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.931997 m-abac-test-1.0.7/mobio/libs/abac/policy/
--rw-r--r--   0 root         (0) root         (0)       44 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.933997 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/__init__.py
--rw-r--r--   0 root         (0) root         (0)      715 2023-06-12 07:41:39.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/base.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.936997 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/boolean/
--rw-r--r--   0 root         (0) root         (0)       39 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/boolean/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1127 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/boolean/base.py
--rw-r--r--   0 root         (0) root         (0)     1107 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/boolean/check_bool.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.946998 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/
--rw-r--r--   0 root         (0) root         (0)      418 2023-06-12 07:41:39.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/__init__.py
--rw-r--r--   0 root         (0) root         (0)      629 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/all_in.py
--rw-r--r--   0 root         (0) root         (0)      654 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/all_not_in.py
--rw-r--r--   0 root         (0) root         (0)      742 2023-06-12 07:41:39.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/any_contains.py
--rw-r--r--   0 root         (0) root         (0)      638 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/any_in.py
--rw-r--r--   0 root         (0) root         (0)      755 2023-06-12 07:41:39.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/any_not_contains.py
--rw-r--r--   0 root         (0) root         (0)      664 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/any_not_in.py
--rw-r--r--   0 root         (0) root         (0)     1341 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/base.py
--rw-r--r--   0 root         (0) root         (0)      754 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/is_empty.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/is_in.py
--rw-r--r--   0 root         (0) root         (0)      774 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
--rw-r--r--   0 root         (0) root         (0)      728 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/is_not_in.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.953998 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/
--rw-r--r--   0 root         (0) root         (0)      243 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2524 2023-05-19 09:33:30.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/base.py
--rw-r--r--   0 root         (0) root         (0)     1345 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/date_eq.py
--rw-r--r--   0 root         (0) root         (0)     1367 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/date_gt.py
--rw-r--r--   0 root         (0) root         (0)     1389 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/date_gte.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/date_lt.py
--rw-r--r--   0 root         (0) root         (0)     1380 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/date_lte.py
--rw-r--r--   0 root         (0) root         (0)     1363 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/date_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.960998 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/
--rw-r--r--   0 root         (0) root         (0)      197 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1839 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/base.py
--rw-r--r--   0 root         (0) root         (0)     1004 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/day_eq.py
--rw-r--r--   0 root         (0) root         (0)      975 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/day_gt.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/day_gte.py
--rw-r--r--   0 root         (0) root         (0)      974 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/day_lt.py
--rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/day_lte.py
--rw-r--r--   0 root         (0) root         (0)      978 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/day_neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.963998 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/ip_address/
--rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/ip_address/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1691 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/ip_address/base.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
--rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.969998 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/
--rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/base.py
--rw-r--r--   0 root         (0) root         (0)      853 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/eq.py
--rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/gt.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/gte.py
--rw-r--r--   0 root         (0) root         (0)      863 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/lt.py
--rw-r--r--   0 root         (0) root         (0)      886 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/lte.py
--rw-r--r--   0 root         (0) root         (0)      869 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/neq.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.972998 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/others/
--rw-r--r--   0 root         (0) root         (0)       73 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/others/__init__.py
--rw-r--r--   0 root         (0) root         (0)      963 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/others/base.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/others/exists.py
--rw-r--r--   0 root         (0) root         (0)      701 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/others/not_exists.py
--rw-r--r--   0 root         (0) root         (0)     2224 2023-06-12 07:41:39.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-12 11:11:33.980998 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/
--rw-r--r--   0 root         (0) root         (0)      401 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/base.py
--rw-r--r--   0 root         (0) root         (0)     1213 2023-06-12 07:41:39.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/contains.py
--rw-r--r--   0 root         (0) root         (0)     1245 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1203 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/equals.py
--rw-r--r--   0 root         (0) root         (0)     1227 2023-06-12 07:41:39.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/not_contains.py
--rw-r--r--   0 root         (0) root         (0)     1258 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/not_ends_with.py
--rw-r--r--   0 root         (0) root         (0)     1214 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/not_equals.py
--rw-r--r--   0 root         (0) root         (0)     1277 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/not_starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1498 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/regex_match.py
--rw-r--r--   0 root         (0) root         (0)     1264 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/starts_with.py
--rw-r--r--   0 root         (0) root         (0)     1601 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/exceptions.py
--rw-r--r--   0 root         (0) root         (0)     6055 2023-06-12 11:10:01.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/policy.py
--rw-r--r--   0 root         (0) root         (0)     5148 2023-06-12 11:10:01.000000 m-abac-test-1.0.7/mobio/libs/abac/policy/utils.py
--rw-r--r--   0 root         (0) root         (0)     5170 2023-06-12 11:10:01.000000 m-abac-test-1.0.7/mobio/libs/abac/result_access.py
--rw-r--r--   0 root         (0) root         (0)      104 2023-05-15 08:15:49.000000 m-abac-test-1.0.7/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-12 11:11:33.983999 m-abac-test-1.0.7/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     9779 2023-06-12 11:11:32.000000 m-abac-test-1.0.7/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.124431 m-abac-test-1.0.8/
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-06-13 08:41:52.123431 m-abac-test-1.0.8/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      620 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.067430 m-abac-test-1.0.8/m_abac_test.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1746 2023-06-13 08:41:51.000000 m-abac-test-1.0.8/m_abac_test.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-06-13 08:41:51.000000 m-abac-test-1.0.8/m_abac_test.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 08:41:51.000000 m-abac-test-1.0.8/m_abac_test.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      100 2023-06-13 08:41:51.000000 m-abac-test-1.0.8/m_abac_test.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-06-13 08:41:51.000000 m-abac-test-1.0.8/m_abac_test.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.056429 m-abac-test-1.0.8/mobio/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.057429 m-abac-test-1.0.8/mobio/libs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.071430 m-abac-test-1.0.8/mobio/libs/abac/
+-rw-r--r--   0 root         (0) root         (0)       70 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.073430 m-abac-test-1.0.8/mobio/libs/abac/adapter/
+-rw-r--r--   0 root         (0) root         (0)      267 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/adapter/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      435 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/adapter/adapter.py
+-rw-r--r--   0 root         (0) root         (0)    15511 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/adapter/elasticsearch_adapter.py
+-rw-r--r--   0 root         (0) root         (0)     7967 2023-06-13 08:40:33.000000 m-abac-test-1.0.8/mobio/libs/abac/call_api.py
+-rw-r--r--   0 root         (0) root         (0)     1243 2023-05-24 07:57:21.000000 m-abac-test-1.0.8/mobio/libs/abac/config.py
+-rw-r--r--   0 root         (0) root         (0)    16098 2023-06-13 08:40:33.000000 m-abac-test-1.0.8/mobio/libs/abac/pdp.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.076430 m-abac-test-1.0.8/mobio/libs/abac/policy/
+-rw-r--r--   0 root         (0) root         (0)       44 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.077430 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      715 2023-06-12 07:41:39.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/base.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.079430 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/boolean/
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/boolean/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1127 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/boolean/base.py
+-rw-r--r--   0 root         (0) root         (0)     1107 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/boolean/check_bool.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.086430 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/
+-rw-r--r--   0 root         (0) root         (0)      418 2023-06-12 07:41:39.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      629 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/all_in.py
+-rw-r--r--   0 root         (0) root         (0)      654 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/all_not_in.py
+-rw-r--r--   0 root         (0) root         (0)      742 2023-06-12 07:41:39.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_contains.py
+-rw-r--r--   0 root         (0) root         (0)      638 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_in.py
+-rw-r--r--   0 root         (0) root         (0)      755 2023-06-12 07:41:39.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_not_contains.py
+-rw-r--r--   0 root         (0) root         (0)      664 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_not_in.py
+-rw-r--r--   0 root         (0) root         (0)     1341 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/base.py
+-rw-r--r--   0 root         (0) root         (0)      754 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_empty.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_in.py
+-rw-r--r--   0 root         (0) root         (0)      774 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_not_empty.py
+-rw-r--r--   0 root         (0) root         (0)      728 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_not_in.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.092430 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2524 2023-05-19 09:33:30.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/base.py
+-rw-r--r--   0 root         (0) root         (0)     1345 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_eq.py
+-rw-r--r--   0 root         (0) root         (0)     1367 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_gt.py
+-rw-r--r--   0 root         (0) root         (0)     1389 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_gte.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_lt.py
+-rw-r--r--   0 root         (0) root         (0)     1380 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_lte.py
+-rw-r--r--   0 root         (0) root         (0)     1363 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.097431 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/
+-rw-r--r--   0 root         (0) root         (0)      197 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1839 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/base.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_eq.py
+-rw-r--r--   0 root         (0) root         (0)      975 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_gt.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_gte.py
+-rw-r--r--   0 root         (0) root         (0)      974 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_lt.py
+-rw-r--r--   0 root         (0) root         (0)      977 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_lte.py
+-rw-r--r--   0 root         (0) root         (0)      978 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.100431 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/
+-rw-r--r--   0 root         (0) root         (0)       82 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1691 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/base.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py
+-rw-r--r--   0 root         (0) root         (0)      746 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.105431 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/
+-rw-r--r--   0 root         (0) root         (0)      188 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/base.py
+-rw-r--r--   0 root         (0) root         (0)      853 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/eq.py
+-rw-r--r--   0 root         (0) root         (0)      871 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/gt.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/gte.py
+-rw-r--r--   0 root         (0) root         (0)      863 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/lt.py
+-rw-r--r--   0 root         (0) root         (0)      886 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/lte.py
+-rw-r--r--   0 root         (0) root         (0)      869 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/neq.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.108431 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/
+-rw-r--r--   0 root         (0) root         (0)       73 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      963 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/base.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/exists.py
+-rw-r--r--   0 root         (0) root         (0)      701 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/not_exists.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2023-06-12 07:41:39.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 08:41:52.121431 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/
+-rw-r--r--   0 root         (0) root         (0)      401 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1497 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/base.py
+-rw-r--r--   0 root         (0) root         (0)     1213 2023-06-12 07:41:39.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/contains.py
+-rw-r--r--   0 root         (0) root         (0)     1245 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1203 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/equals.py
+-rw-r--r--   0 root         (0) root         (0)     1227 2023-06-12 07:41:39.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_contains.py
+-rw-r--r--   0 root         (0) root         (0)     1258 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_ends_with.py
+-rw-r--r--   0 root         (0) root         (0)     1214 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_equals.py
+-rw-r--r--   0 root         (0) root         (0)     1277 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1498 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/regex_match.py
+-rw-r--r--   0 root         (0) root         (0)     1264 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/starts_with.py
+-rw-r--r--   0 root         (0) root         (0)     1601 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)     6055 2023-06-12 11:10:01.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/policy.py
+-rw-r--r--   0 root         (0) root         (0)     5148 2023-06-12 11:10:01.000000 m-abac-test-1.0.8/mobio/libs/abac/policy/utils.py
+-rw-r--r--   0 root         (0) root         (0)     5170 2023-06-12 11:10:01.000000 m-abac-test-1.0.8/mobio/libs/abac/result_access.py
+-rw-r--r--   0 root         (0) root         (0)      104 2023-05-15 08:15:49.000000 m-abac-test-1.0.8/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 08:41:52.124431 m-abac-test-1.0.8/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     9779 2023-06-13 08:41:50.000000 m-abac-test-1.0.8/setup.py
```

### Comparing `m-abac-test-1.0.7/PKG-INFO` & `m-abac-test-1.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-test
-Version: 1.0.7
+Version: 1.0.8
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: ### ABAC Engine
```

### Comparing `m-abac-test-1.0.7/README.md` & `m-abac-test-1.0.8/README.md`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/m_abac_test.egg-info/PKG-INFO` & `m-abac-test-1.0.8/m_abac_test.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: m-abac-test
-Version: 1.0.7
+Version: 1.0.8
 Summary: Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)
 Home-page: https://github.com/mobiovn
 Author: MOBIO
 Author-email: contact@mobio.vn
 License: MIT
 Project-URL: Source, https://github.com/mobiovn
 Description: ### ABAC Engine
```

### Comparing `m-abac-test-1.0.7/m_abac_test.egg-info/SOURCES.txt` & `m-abac-test-1.0.8/m_abac_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/adapter/elasticsearch_adapter.py` & `m-abac-test-1.0.8/mobio/libs/abac/adapter/elasticsearch_adapter.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/call_api.py` & `m-abac-test-1.0.8/mobio/libs/abac/call_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,25 +53,25 @@
                 params={"page": "-1"}
             )
             data = {}
             if data_res.status_code == 200:
                 if data_res.json().get("data"):
                     list_data = data_res.json().get("data")
                     for i in list_data:
-                        data[i.get("key")] = i
+                        data[i.get("resource") + ":" + i.get("key")] = i
             # print("abac_sdk admin_get_json_action: {}".format(data))
             return data
         except Exception as er:
             err_msg = "abac_sdk admin_get_json_action err: {}".format(er)
             print(err_msg)
             return {}
 
     # TODO: thay expiration cho production 15p
     @staticmethod
-    @lru_cache_redis.add(expiration=60)
+    @lru_cache_redis.add(expiration=30)
     def admin_get_list_statement(merchant_id, account_id, resource, action, service):
         """
         :param merchant_id:
         :param account_id:
         :param resource:
         :param action:
         :return: [{
```

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/config.py` & `m-abac-test-1.0.8/mobio/libs/abac/config.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/pdp.py` & `m-abac-test-1.0.8/mobio/libs/abac/pdp.py`

 * *Files 6% similar despite different names*

```diff
@@ -87,16 +87,21 @@
         if data_cache:
             data_merchant = str(data_cache.decode("utf-8")).split(";")
             if merchant_id in data_merchant:
                 use_abac = True
         return use_abac
 
     def get_policy_statement_for_target(self):
-        return CallAPI.admin_get_list_statement(self.merchant_id, self.account_id,
+        list_statement = CallAPI.admin_get_list_statement(self.merchant_id, self.account_id,
                                                 self.resource, self.action, self.service)
+        if not list_statement:
+            print("abac_sdk list_statement not found merchant_id: {} , account_id: {} , "
+                  "resource: {} , action: {} , service: {} ".format(self.merchant_id, self.account_id,
+                                                self.resource, self.action, self.service))
+        return list_statement
 
     def is_allowed(self):
         """
             Check if authorization request is allowed
 
             :param request: request object
             :return: True if authorized else False
@@ -280,22 +285,23 @@
             print(msg_err)
             self.result_access.add_log_error(msg_err)
             result_allow = False
         return result_allow
 
     def check_info_action(self):
         action_info = CallAPI.admin_get_json_action(merchant_id=self.merchant_id)
+        key_check = self.resource + ":" + self.action
         if not action_info:
             raise ValueError("action for merchant_id {} not found".format(self.merchant_id))
-        if not action_info.get(self.action):
-            raise ValueError("action {} not found".format(self.action))
-        self.access_level = action_info.get(self.action, {}).get("access_level", "").lower()
+        if not action_info.get(key_check):
+            raise ValueError("action {} not found".format(key_check))
+        self.access_level = action_info.get(key_check, {}).get("access_level", "").lower()
         if not self.access_level:
-            raise ValueError("access_level {} not valid".format(self.action))
-        self.service = action_info.get(self.action, {}).get("service", "")
+            raise ValueError("access_level {} not valid".format(key_check))
+        self.service = action_info.get(key_check, {}).get("service", "")
         if not self.service:
             raise ValueError("service {} not valid".format(self.service))
 
     def is_allowed_list(self, data: list):
         """
             Check if authorization request is allowed data
         """
```

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/base.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/boolean/base.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/boolean/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/boolean/check_bool.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/boolean/check_bool.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/all_in.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/all_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/all_not_in.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/all_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/any_contains.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/any_in.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/any_not_contains.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/any_not_in.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/any_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/base.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/is_empty.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/is_in.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/is_not_empty.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_not_empty.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/collection/is_not_in.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/collection/is_not_in.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/base.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/date_eq.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/date_gt.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/date_gte.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/date_lt.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/date_lte.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/date_time/date_neq.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/date_time/date_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/base.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/day_eq.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/day_gt.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/day_gte.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/day_lt.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/day_lte.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/day/day_neq.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/day/day_neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/ip_address/base.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/ip_address/not_in_subnet.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/base.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/eq.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/eq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/gt.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/gt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/gte.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/gte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/lt.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/lt.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/lte.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/lte.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/numeric/neq.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/numeric/neq.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/others/base.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/others/exists.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/others/not_exists.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/others/not_exists.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/schema.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/schema.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/base.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/base.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/contains.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/ends_with.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/equals.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/not_contains.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_contains.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/not_ends_with.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_ends_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/not_equals.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_equals.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/not_starts_with.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/not_starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/regex_match.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/regex_match.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/conditions/string/starts_with.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/conditions/string/starts_with.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/exceptions.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/exceptions.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/policy.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/policy.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/policy/utils.py` & `m-abac-test-1.0.8/mobio/libs/abac/policy/utils.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/mobio/libs/abac/result_access.py` & `m-abac-test-1.0.8/mobio/libs/abac/result_access.py`

 * *Files identical despite different names*

### Comparing `m-abac-test-1.0.7/setup.py` & `m-abac-test-1.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -45,15 +45,15 @@
         ]
         # with open(Requirements.requirements_path) as req_file:
         #     for line in req_file.read().splitlines():
         #         if not line.strip().startswith("#"):
         #             requirements.append(line)
         return requirements
 
-version_dev='1.0.7'
+version_dev='1.0.8'
 version_prod='1.0.0'
 
 run_mode='-test'
 
 setup(
     # This is the name of your project. The first time you publish this
     # package, this name will be registered for you. It will determine how
@@ -70,15 +70,15 @@
     # options={"bdist_wheel": {"universal": True}},
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version='1.0.7',  # Required
+    version='1.0.8',  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Thư viện xử lý kiểm tra quyền theo logic ABAC (Attribute-based access control)",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

