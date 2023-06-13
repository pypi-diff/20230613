# Comparing `tmp/odoo_addons_oca_multi_company-16.0.20230525.0-py3-none-any.whl.zip` & `tmp/odoo_addons_oca_multi_company-16.0.20230612.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 1452 bytes, number of entries: 4
--rw-r--r--  2.0 unx      679 b- defN 23-May-26 04:20 odoo_addons_oca_multi_company-16.0.20230525.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-26 04:20 odoo_addons_oca_multi_company-16.0.20230525.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-26 04:20 odoo_addons_oca_multi_company-16.0.20230525.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      424 b- defN 23-May-26 04:20 odoo_addons_oca_multi_company-16.0.20230525.0.dist-info/RECORD
-4 files, 1196 bytes uncompressed, 614 bytes compressed:  48.7%
+Zip file size: 1466 bytes, number of entries: 4
+-rw-r--r--  2.0 unx      761 b- defN 23-Jun-13 04:35 odoo_addons_oca_multi_company-16.0.20230612.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 04:35 odoo_addons_oca_multi_company-16.0.20230612.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-13 04:35 odoo_addons_oca_multi_company-16.0.20230612.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      424 b- defN 23-Jun-13 04:35 odoo_addons_oca_multi_company-16.0.20230612.0.dist-info/RECORD
+4 files, 1278 bytes uncompressed, 628 bytes compressed:  50.9%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo_addons_oca_multi_company-16.0.20230525.0.dist-info/METADATA
+Filename: odoo_addons_oca_multi_company-16.0.20230612.0.dist-info/METADATA
 Comment: 
 
-Filename: odoo_addons_oca_multi_company-16.0.20230525.0.dist-info/WHEEL
+Filename: odoo_addons_oca_multi_company-16.0.20230612.0.dist-info/WHEEL
 Comment: 
 
-Filename: odoo_addons_oca_multi_company-16.0.20230525.0.dist-info/top_level.txt
+Filename: odoo_addons_oca_multi_company-16.0.20230612.0.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo_addons_oca_multi_company-16.0.20230525.0.dist-info/RECORD
+Filename: odoo_addons_oca_multi_company-16.0.20230612.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo_addons_oca_multi_company-16.0.20230525.0.dist-info/METADATA` & `odoo_addons_oca_multi_company-16.0.20230612.0.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: odoo-addons-oca-multi-company
-Version: 16.0.20230525.0
+Version: 16.0.20230612.0
 Summary: Meta package for oca-multi-company Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 16.0
 Requires-Dist: odoo-addon-account-invoice-inter-company (<16.1dev,>=16.0dev)
+Requires-Dist: odoo-addon-account-multicompany-easy-creation (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-mail-multicompany (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-product-category-company (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-product-tax-multicompany-default (<16.1dev,>=16.0dev)
 Requires-Dist: odoo-addon-res-company-search-view (<16.1dev,>=16.0dev)
 
 UNKNOWN
```

