# Comparing `tmp/eurofiber_package-0.1.8.tar.gz` & `tmp/eurofiber_package-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eurofiber_package-0.1.8.tar", last modified: Wed Jan 11 12:28:38 2023, max compression
+gzip compressed data, was "eurofiber_package-0.1.9.tar", last modified: Tue Feb 21 09:21:21 2023, max compression
```

## Comparing `eurofiber_package-0.1.8.tar` & `eurofiber_package-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-01-11 12:28:38.017489 eurofiber_package-0.1.8/
--rw-rw-rw-   0        0        0      176 2023-01-11 12:28:38.016489 eurofiber_package-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-11-21 09:17:31.000000 eurofiber_package-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-01-11 12:28:37.998202 eurofiber_package-0.1.8/eurofiber_package/
--rw-rw-rw-   0        0        0        0 2022-11-21 09:21:52.000000 eurofiber_package-0.1.8/eurofiber_package/__init__.py
--rw-rw-rw-   0        0        0     1184 2023-01-09 11:40:57.000000 eurofiber_package-0.1.8/eurofiber_package/address_functions.py
--rw-rw-rw-   0        0        0     2397 2023-01-11 12:28:05.000000 eurofiber_package-0.1.8/eurofiber_package/enrichment_functions.py
--rw-rw-rw-   0        0        0     7652 2023-01-11 11:54:44.000000 eurofiber_package-0.1.8/eurofiber_package/general_functions.py
--rw-rw-rw-   0        0        0     5523 2023-01-11 11:48:17.000000 eurofiber_package-0.1.8/eurofiber_package/geographical_functions.py
-drwxrwxrwx   0        0        0        0 2023-01-11 12:28:38.014117 eurofiber_package-0.1.8/eurofiber_package.egg-info/
--rw-rw-rw-   0        0        0      176 2023-01-11 12:28:37.000000 eurofiber_package-0.1.8/eurofiber_package.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      376 2023-01-11 12:28:37.000000 eurofiber_package-0.1.8/eurofiber_package.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-01-11 12:28:37.000000 eurofiber_package-0.1.8/eurofiber_package.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       18 2023-01-11 12:28:37.000000 eurofiber_package-0.1.8/eurofiber_package.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-01-11 12:28:38.017489 eurofiber_package-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0      249 2023-01-11 12:28:18.000000 eurofiber_package-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-21 09:21:21.938488 eurofiber_package-0.1.9/
+-rw-rw-rw-   0        0        0      176 2023-02-21 09:21:21.938222 eurofiber_package-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:17:31.000000 eurofiber_package-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-21 09:21:21.925452 eurofiber_package-0.1.9/eurofiber_package/
+-rw-rw-rw-   0        0        0        0 2022-11-21 09:21:52.000000 eurofiber_package-0.1.9/eurofiber_package/__init__.py
+-rw-rw-rw-   0        0        0     1184 2023-01-09 11:40:57.000000 eurofiber_package-0.1.9/eurofiber_package/address_functions.py
+-rw-rw-rw-   0        0        0     1019 2023-02-13 13:10:47.000000 eurofiber_package-0.1.9/eurofiber_package/cocon_functions.py
+-rw-rw-rw-   0        0        0     2397 2023-01-22 19:09:33.000000 eurofiber_package-0.1.9/eurofiber_package/enrichment_functions.py
+-rw-rw-rw-   0        0        0     9366 2023-02-09 14:27:14.000000 eurofiber_package-0.1.9/eurofiber_package/general_functions.py
+-rw-rw-rw-   0        0        0     5523 2023-02-06 12:54:59.000000 eurofiber_package-0.1.9/eurofiber_package/geographical_functions.py
+-rw-rw-rw-   0        0        0     7513 2023-02-21 09:18:58.000000 eurofiber_package-0.1.9/eurofiber_package/scrapers.py
+drwxrwxrwx   0        0        0        0 2023-02-21 09:21:21.936236 eurofiber_package-0.1.9/eurofiber_package.egg-info/
+-rw-rw-rw-   0        0        0      176 2023-02-21 09:21:21.000000 eurofiber_package-0.1.9/eurofiber_package.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      443 2023-02-21 09:21:21.000000 eurofiber_package-0.1.9/eurofiber_package.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-21 09:21:21.000000 eurofiber_package-0.1.9/eurofiber_package.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       18 2023-02-21 09:21:21.000000 eurofiber_package-0.1.9/eurofiber_package.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-02-21 09:21:21.938488 eurofiber_package-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0      249 2023-02-21 09:21:09.000000 eurofiber_package-0.1.9/setup.py
```

### Comparing `eurofiber_package-0.1.8/eurofiber_package/address_functions.py` & `eurofiber_package-0.1.9/eurofiber_package/address_functions.py`

 * *Files identical despite different names*

### Comparing `eurofiber_package-0.1.8/eurofiber_package/enrichment_functions.py` & `eurofiber_package-0.1.9/eurofiber_package/enrichment_functions.py`

 * *Files identical despite different names*

### Comparing `eurofiber_package-0.1.8/eurofiber_package/general_functions.py` & `eurofiber_package-0.1.9/eurofiber_package/general_functions.py`

 * *Files 20% similar despite different names*

```diff
@@ -63,15 +63,15 @@
     for variable in args:
         new_variable_name = '_'.join(variable.split()) + '_cc_dd'    
         duns[new_variable_name] = duns[variable].astype(str)
         duns[new_variable_name] = duns[new_variable_name].apply(lambda x: x.replace('nan', '').replace('.0', ''))
         duns[new_variable_name] = duns.groupby(['deduplicate'])[new_variable_name].transform(lambda x: ' / '.join(x))
         duns[new_variable_name] = duns[new_variable_name].apply(lambda x: [item for item in list(set(x.split(' / '))) if item != 'nan'])
         duns[new_variable_name] = duns[new_variable_name].apply(lambda x: ', '.join(x))
-        duns[new_variable_name] = duns[new_variable_name].replace(r'^\s*$', np.nan, regex=True) 
+        duns[new_variable_name] = duns[new_variable_name].replace(r'^\s*$', np.nan, regex=True) # replace blank lines with np.nan
 
     # sort based on employees on entity
     duns = duns.sort_values(['deduplicate', '# employees on entity'], ascending=[True, False])        
 
     # drop duplicates
     duns = duns.drop_duplicates(subset=['deduplicate'], keep='first')     
 
@@ -134,8 +134,38 @@
 #     for col in duns.columns:
 #         if '_cc_dd' not in col:
 #             column_order.append(col)
 #             if '_'.join(col.split()) + '_cc_dd' in duns:
 #                 column_order.append('_'.join(col.split()) + '_cc_dd')
 #     duns = duns[column_order] 
 
-#     return duns
+#     return duns
+
+
+def deduplicate_concatenate_general(dataframe, deduplicate_list:list, concatenate_list:list):
+    """ this function deduplicates a dataframe and concatenates variables based on provided inputs """
+
+    dataframe['deduplicate'] = dataframe[deduplicate_list].apply(lambda row: '_'.join(row.values.astype(str)), axis=1)
+
+    # for each variable mentioned, create a cc_dd (concatenate values to retain information)
+    for variable in concatenate_list:
+        new_variable_name = '_'.join(variable.split()) + '_cc_dd'    
+        dataframe[new_variable_name] = dataframe[variable].astype(str)
+        dataframe[new_variable_name] = dataframe[new_variable_name].apply(lambda x: x.replace('nan', '').replace('.0', ''))
+        dataframe[new_variable_name] = dataframe.groupby('deduplicate')[new_variable_name].transform(lambda x: ' / '.join(x))
+        dataframe[new_variable_name] = dataframe[new_variable_name].apply(lambda x: [item for item in list(set(x.split(' / '))) if item != 'nan'])
+        dataframe[new_variable_name] = dataframe[new_variable_name].apply(lambda x: ', '.join(x))
+        dataframe[new_variable_name] = dataframe[new_variable_name].replace(r'^\s*$', np.nan, regex=True) 
+
+    # drop duplicates
+    dataframe = dataframe.drop_duplicates(subset=deduplicate_list, keep='first')     
+
+    # change columns order
+    column_order = []
+    for col in dataframe.columns:
+        if '_cc_dd' not in col:
+            column_order.append(col)
+            if '_'.join(col.split()) + '_cc_dd' in dataframe:
+                column_order.append('_'.join(col.split()) + '_cc_dd')
+    dataframe = dataframe[column_order] 
+
+    return dataframe
```

### Comparing `eurofiber_package-0.1.8/eurofiber_package/geographical_functions.py` & `eurofiber_package-0.1.9/eurofiber_package/geographical_functions.py`

 * *Files identical despite different names*

