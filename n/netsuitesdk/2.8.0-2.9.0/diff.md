# Comparing `tmp/netsuitesdk-2.8.0.tar.gz` & `tmp/netsuitesdk-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netsuitesdk-2.8.0.tar", last modified: Mon Jan  3 15:09:49 2022, max compression
+gzip compressed data, was "netsuitesdk-2.9.0.tar", last modified: Tue Mar  1 10:25:19 2022, max compression
```

## Comparing `netsuitesdk-2.8.0.tar` & `netsuitesdk-2.9.0.tar`

### file list

```diff
@@ -1,51 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 15:09:49.927843 netsuitesdk-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)     8526 2022-01-03 15:09:49.927843 netsuitesdk-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     7943 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 15:09:49.923843 netsuitesdk-2.8.0/netsuitesdk/
--rw-r--r--   0 runner    (1001) docker     (121)      241 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 15:09:49.927843 netsuitesdk-2.8.0/netsuitesdk/api/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/accounts.py
--rw-r--r--   0 runner    (1001) docker     (121)     5154 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/base.py
--rw-r--r--   0 runner    (1001) docker     (121)      227 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/classifications.py
--rw-r--r--   0 runner    (1001) docker     (121)     3146 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/credit_memos.py
--rw-r--r--   0 runner    (1001) docker     (121)      448 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/currencies.py
--rw-r--r--   0 runner    (1001) docker     (121)      452 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/custom_lists.py
--rw-r--r--   0 runner    (1001) docker     (121)      700 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/custom_record_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/custom_records.py
--rw-r--r--   0 runner    (1001) docker     (121)     4324 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/customers.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/departments.py
--rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/employees.py
--rw-r--r--   0 runner    (1001) docker     (121)      229 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/expense_categories.py
--rw-r--r--   0 runner    (1001) docker     (121)     3935 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/expense_reports.py
--rw-r--r--   0 runner    (1001) docker     (121)      933 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/files.py
--rw-r--r--   0 runner    (1001) docker     (121)      687 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/folders.py
--rw-r--r--   0 runner    (1001) docker     (121)     4398 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/invoices.py
--rw-r--r--   0 runner    (1001) docker     (121)     3338 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/journal_entries.py
--rw-r--r--   0 runner    (1001) docker     (121)      215 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/locations.py
--rw-r--r--   0 runner    (1001) docker     (121)      209 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/projects.py
--rw-r--r--   0 runner    (1001) docker     (121)      221 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/subsidiaries.py
--rw-r--r--   0 runner    (1001) docker     (121)      216 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/tax_groups.py
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/tax_items.py
--rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/terms.py
--rw-r--r--   0 runner    (1001) docker     (121)     3826 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/vendor_bills.py
--rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/vendor_credits.py
--rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/vendor_payments.py
--rw-r--r--   0 runner    (1001) docker     (121)     3011 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/api/vendors.py
--rw-r--r--   0 runner    (1001) docker     (121)     3146 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/connection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 15:09:49.927843 netsuitesdk-2.8.0/netsuitesdk/internal/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/internal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    24500 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/internal/client.py
--rw-r--r--   0 runner    (1001) docker     (121)     2325 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/internal/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/internal/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)     5188 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/internal/netsuite_types.py
--rw-r--r--   0 runner    (1001) docker     (121)     2274 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/netsuitesdk/internal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-01-03 15:09:49.923843 netsuitesdk-2.8.0/netsuitesdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     8526 2022-01-03 15:09:49.000000 netsuitesdk-2.8.0/netsuitesdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1312 2022-01-03 15:09:49.000000 netsuitesdk-2.8.0/netsuitesdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-01-03 15:09:49.000000 netsuitesdk-2.8.0/netsuitesdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-01-03 15:09:49.000000 netsuitesdk-2.8.0/netsuitesdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-01-03 15:09:49.000000 netsuitesdk-2.8.0/netsuitesdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-01-03 15:09:49.927843 netsuitesdk-2.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      822 2022-01-03 15:09:37.000000 netsuitesdk-2.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 10:25:19.799276 netsuitesdk-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (121)     1063 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)     8526 2022-03-01 10:25:19.799276 netsuitesdk-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     7943 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 10:25:19.795276 netsuitesdk-2.9.0/netsuitesdk/
+-rw-r--r--   0 runner    (1001) docker     (121)      241 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 10:25:19.799276 netsuitesdk-2.9.0/netsuitesdk/api/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/accounts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5154 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (121)      227 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/classifications.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3146 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/credit_memos.py
+-rw-r--r--   0 runner    (1001) docker     (121)      448 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/currencies.py
+-rw-r--r--   0 runner    (1001) docker     (121)      452 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/custom_lists.py
+-rw-r--r--   0 runner    (1001) docker     (121)      700 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/custom_record_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1893 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/custom_records.py
+-rw-r--r--   0 runner    (1001) docker     (121)      458 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/custom_segments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4324 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/customers.py
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/departments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1563 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/employees.py
+-rw-r--r--   0 runner    (1001) docker     (121)      229 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/expense_categories.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3935 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/expense_reports.py
+-rw-r--r--   0 runner    (1001) docker     (121)      933 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/files.py
+-rw-r--r--   0 runner    (1001) docker     (121)      687 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/folders.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4398 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3338 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/journal_entries.py
+-rw-r--r--   0 runner    (1001) docker     (121)      215 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/locations.py
+-rw-r--r--   0 runner    (1001) docker     (121)      209 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/projects.py
+-rw-r--r--   0 runner    (1001) docker     (121)      221 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/subsidiaries.py
+-rw-r--r--   0 runner    (1001) docker     (121)      216 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/tax_groups.py
+-rw-r--r--   0 runner    (1001) docker     (121)      219 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/tax_items.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1125 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/terms.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3826 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/vendor_bills.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1785 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/vendor_credits.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2613 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/vendor_payments.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3011 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/api/vendors.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3251 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/connection.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 10:25:19.799276 netsuitesdk-2.9.0/netsuitesdk/internal/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/internal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    24500 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/internal/client.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2346 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/internal/constants.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1081 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/internal/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5188 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/internal/netsuite_types.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2274 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/netsuitesdk/internal/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-01 10:25:19.795276 netsuitesdk-2.9.0/netsuitesdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     8526 2022-03-01 10:25:19.000000 netsuitesdk-2.9.0/netsuitesdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1347 2022-03-01 10:25:19.000000 netsuitesdk-2.9.0/netsuitesdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-01 10:25:19.000000 netsuitesdk-2.9.0/netsuitesdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2022-03-01 10:25:19.000000 netsuitesdk-2.9.0/netsuitesdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-03-01 10:25:19.000000 netsuitesdk-2.9.0/netsuitesdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-01 10:25:19.803276 netsuitesdk-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)      822 2022-03-01 10:25:11.000000 netsuitesdk-2.9.0/setup.py
```

### Comparing `netsuitesdk-2.8.0/LICENSE` & `netsuitesdk-2.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/PKG-INFO` & `netsuitesdk-2.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuitesdk
-Version: 2.8.0
+Version: 2.9.0
 Summary: Python SDK for accessing the NetSuite SOAP webservice
 Home-page: https://github.com/fylein/netsuite-sdk-py
 Author: Siva Narayanan
 Author-email: siva@fyle.in
 License: MIT
 Keywords: netsuite,api,python,sdk
 Platform: UNKNOWN
```

### Comparing `netsuitesdk-2.8.0/README.md` & `netsuitesdk-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/base.py` & `netsuitesdk-2.9.0/netsuitesdk/api/base.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/credit_memos.py` & `netsuitesdk-2.9.0/netsuitesdk/api/credit_memos.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/custom_record_types.py` & `netsuitesdk-2.9.0/netsuitesdk/api/custom_record_types.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/custom_records.py` & `netsuitesdk-2.9.0/netsuitesdk/api/custom_records.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/customers.py` & `netsuitesdk-2.9.0/netsuitesdk/api/customers.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/employees.py` & `netsuitesdk-2.9.0/netsuitesdk/api/employees.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/expense_reports.py` & `netsuitesdk-2.9.0/netsuitesdk/api/expense_reports.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/files.py` & `netsuitesdk-2.9.0/netsuitesdk/api/files.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/folders.py` & `netsuitesdk-2.9.0/netsuitesdk/api/folders.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/invoices.py` & `netsuitesdk-2.9.0/netsuitesdk/api/invoices.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/journal_entries.py` & `netsuitesdk-2.9.0/netsuitesdk/api/journal_entries.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/terms.py` & `netsuitesdk-2.9.0/netsuitesdk/api/terms.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/vendor_bills.py` & `netsuitesdk-2.9.0/netsuitesdk/api/vendor_bills.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/vendor_credits.py` & `netsuitesdk-2.9.0/netsuitesdk/api/vendor_credits.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/vendor_payments.py` & `netsuitesdk-2.9.0/netsuitesdk/api/vendor_payments.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/api/vendors.py` & `netsuitesdk-2.9.0/netsuitesdk/api/vendors.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/connection.py` & `netsuitesdk-2.9.0/netsuitesdk/connection.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 from .api.expense_reports import ExpenseReports
 from .api.folders import Folders
 from .api.files import Files
 from .api.customers import Customers
 from .api.projects import Projects
 from .api.expense_categories import ExpenseCategory
 from .api.custom_lists import CustomLists
+from .api.custom_segments import CustomSegments
 from .api.custom_record_types import CustomRecordTypes
 from .api.custom_records import CustomRecords
 from .api.vendor_payments import VendorPayments
 from .api.invoices import Invoices
 from .api.terms import Terms
 from .api.tax_items import TaxItems
 from .api.tax_groups import TaxGroups
@@ -53,14 +54,15 @@
         self.journal_entries = JournalEntries(ns_client)
         self.employees = Employees(ns_client)
         self.expense_reports = ExpenseReports(ns_client)
         self.folders = Folders(ns_client)
         self.files = Files(ns_client)
         self.expense_categories = ExpenseCategory(ns_client)
         self.custom_lists = CustomLists(ns_client)
+        self.custom_segments = CustomSegments(ns_client)
         self.custom_records = CustomRecords(ns_client)
         self.custom_record_types = CustomRecordTypes(ns_client)
         self.customers = Customers(ns_client)
         self.projects = Projects(ns_client)
         self.vendor_payments = VendorPayments(ns_client)
         self.invoices = Invoices(ns_client)
         self.terms = Terms(ns_client)
```

### Comparing `netsuitesdk-2.8.0/netsuitesdk/internal/client.py` & `netsuitesdk-2.9.0/netsuitesdk/internal/client.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/internal/constants.py` & `netsuitesdk-2.9.0/netsuitesdk/internal/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
     'couponCode',
     'currencyRate',
     'customer',
     'customerCategory',
     'customerMessage',
     'customerStatus',
     'customList',
+    'customSegment',
     'customRecord',
     'department',
     'employee',
     'entityGroup',
     'expenseCategory',
     'fairValuePrice',
     'file',
```

### Comparing `netsuitesdk-2.8.0/netsuitesdk/internal/exceptions.py` & `netsuitesdk-2.9.0/netsuitesdk/internal/exceptions.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/internal/netsuite_types.py` & `netsuitesdk-2.9.0/netsuitesdk/internal/netsuite_types.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk/internal/utils.py` & `netsuitesdk-2.9.0/netsuitesdk/internal/utils.py`

 * *Files identical despite different names*

### Comparing `netsuitesdk-2.8.0/netsuitesdk.egg-info/PKG-INFO` & `netsuitesdk-2.9.0/netsuitesdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netsuitesdk
-Version: 2.8.0
+Version: 2.9.0
 Summary: Python SDK for accessing the NetSuite SOAP webservice
 Home-page: https://github.com/fylein/netsuite-sdk-py
 Author: Siva Narayanan
 Author-email: siva@fyle.in
 License: MIT
 Keywords: netsuite,api,python,sdk
 Platform: UNKNOWN
```

### Comparing `netsuitesdk-2.8.0/netsuitesdk.egg-info/SOURCES.txt` & `netsuitesdk-2.9.0/netsuitesdk.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 netsuitesdk/api/base.py
 netsuitesdk/api/classifications.py
 netsuitesdk/api/credit_memos.py
 netsuitesdk/api/currencies.py
 netsuitesdk/api/custom_lists.py
 netsuitesdk/api/custom_record_types.py
 netsuitesdk/api/custom_records.py
+netsuitesdk/api/custom_segments.py
 netsuitesdk/api/customers.py
 netsuitesdk/api/departments.py
 netsuitesdk/api/employees.py
 netsuitesdk/api/expense_categories.py
 netsuitesdk/api/expense_reports.py
 netsuitesdk/api/files.py
 netsuitesdk/api/folders.py
```

### Comparing `netsuitesdk-2.8.0/setup.py` & `netsuitesdk-2.9.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='netsuitesdk',
-    version='2.8.0',
+    version='2.9.0',
     author='Siva Narayanan',
     author_email='siva@fyle.in',
     description='Python SDK for accessing the NetSuite SOAP webservice',
     license='MIT',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=['netsuite', 'api', 'python', 'sdk'],
```

