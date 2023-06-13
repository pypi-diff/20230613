# Comparing `tmp/sirene-0.0.1.tar.gz` & `tmp/sirene-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sirene-0.0.1.tar", last modified: Tue Jun  6 21:47:10 2023, max compression
+gzip compressed data, was "sirene-0.0.2.tar", last modified: Mon Jun 12 20:58:46 2023, max compression
```

## Comparing `sirene-0.0.1.tar` & `sirene-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-06 21:47:10.398411 sirene-0.0.1/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)     1080 2023-05-01 17:49:02.000000 sirene-0.0.1/LICENSE
--rw-rw-r--   0 felipe    (1000) felipe    (1000)       41 2023-06-06 21:14:36.000000 sirene-0.0.1/MANIFEST.in
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      554 2023-06-06 21:47:10.398411 sirene-0.0.1/PKG-INFO
--rw-rw-r--   0 felipe    (1000) felipe    (1000)       72 2023-06-06 21:09:38.000000 sirene-0.0.1/README.md
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      103 2021-04-01 21:15:48.000000 sirene-0.0.1/pyproject.toml
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      629 2023-06-06 21:47:10.398411 sirene-0.0.1/setup.cfg
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-06 21:47:10.390411 sirene-0.0.1/sirene/
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-06 21:47:10.386411 sirene-0.0.1/sirene/MCTI/
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-06 21:47:10.398411 sirene-0.0.1/sirene/MCTI/sexta_edicao/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   154072 2023-06-06 21:32:26.000000 sirene-0.0.1/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_agropecuaria.xlsx
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   106995 2023-05-17 20:22:59.000000 sirene-0.0.1/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_energia.xlsx
--rw-rw-r--   0 felipe    (1000) felipe    (1000)   117053 2023-05-17 20:23:08.000000 sirene-0.0.1/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_ippu.xlsx
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    45115 2023-05-17 20:23:17.000000 sirene-0.0.1/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_lulucf.xlsx
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    45235 2023-05-17 20:23:21.000000 sirene-0.0.1/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_residuos.xlsx
--rw-rw-r--   0 felipe    (1000) felipe    (1000)    28706 2023-05-17 20:23:25.000000 sirene-0.0.1/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_total-brasil-1.xlsx
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2021-04-01 21:15:48.000000 sirene-0.0.1/sirene/__init__.py
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      967 2023-06-06 21:44:32.000000 sirene-0.0.1/sirene/srn.py
-drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-06 21:47:10.390411 sirene-0.0.1/sirene.egg-info/
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      554 2023-06-06 21:47:10.000000 sirene-0.0.1/sirene.egg-info/PKG-INFO
--rw-rw-r--   0 felipe    (1000) felipe    (1000)      605 2023-06-06 21:47:10.000000 sirene-0.0.1/sirene.egg-info/SOURCES.txt
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        1 2023-06-06 21:47:10.000000 sirene-0.0.1/sirene.egg-info/dependency_links.txt
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        5 2023-06-06 21:47:10.000000 sirene-0.0.1/sirene.egg-info/requires.txt
--rw-rw-r--   0 felipe    (1000) felipe    (1000)        7 2023-06-06 21:47:10.000000 sirene-0.0.1/sirene.egg-info/top_level.txt
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-12 20:58:46.043776 sirene-0.0.2/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     1080 2023-05-01 17:49:02.000000 sirene-0.0.2/LICENSE
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)       41 2023-06-06 21:14:36.000000 sirene-0.0.2/MANIFEST.in
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      554 2023-06-12 20:58:46.043776 sirene-0.0.2/PKG-INFO
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)       72 2023-06-06 21:09:38.000000 sirene-0.0.2/README.md
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      103 2021-04-01 21:15:48.000000 sirene-0.0.2/pyproject.toml
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      629 2023-06-12 20:58:46.047776 sirene-0.0.2/setup.cfg
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-12 20:58:46.035776 sirene-0.0.2/sirene/
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-12 20:58:46.031776 sirene-0.0.2/sirene/MCTI/
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-12 20:58:46.043776 sirene-0.0.2/sirene/MCTI/sexta_edicao/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   154072 2023-06-06 21:32:26.000000 sirene-0.0.2/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_agropecuaria.xlsx
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   106995 2023-05-17 20:22:59.000000 sirene-0.0.2/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_energia.xlsx
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)   117053 2023-05-17 20:23:08.000000 sirene-0.0.2/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_ippu.xlsx
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    45115 2023-05-17 20:23:17.000000 sirene-0.0.2/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_lulucf.xlsx
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    45235 2023-05-17 20:23:21.000000 sirene-0.0.2/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_residuos.xlsx
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)    28706 2023-05-17 20:23:25.000000 sirene-0.0.2/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_total-brasil-1.xlsx
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        0 2021-04-01 21:15:48.000000 sirene-0.0.2/sirene/__init__.py
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)     1054 2023-06-12 20:57:50.000000 sirene-0.0.2/sirene/srn.py
+drwxrwxr-x   0 felipe    (1000) felipe    (1000)        0 2023-06-12 20:58:46.035776 sirene-0.0.2/sirene.egg-info/
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      554 2023-06-12 20:58:46.000000 sirene-0.0.2/sirene.egg-info/PKG-INFO
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)      605 2023-06-12 20:58:46.000000 sirene-0.0.2/sirene.egg-info/SOURCES.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        1 2023-06-12 20:58:46.000000 sirene-0.0.2/sirene.egg-info/dependency_links.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        5 2023-06-12 20:58:46.000000 sirene-0.0.2/sirene.egg-info/requires.txt
+-rw-rw-r--   0 felipe    (1000) felipe    (1000)        7 2023-06-12 20:58:46.000000 sirene-0.0.2/sirene.egg-info/top_level.txt
```

### Comparing `sirene-0.0.1/LICENSE` & `sirene-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sirene-0.0.1/PKG-INFO` & `sirene-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirene
-Version: 0.0.1
+Version: 0.0.2
 Summary: Import data from the 'Sistema de Registro Nacional de Emissões' (SIRENE) from MCTI
 Home-page: https://github.com/fms-1988
 Author: Felipe Morelli Da Silva
 Author-email: fms.morelli@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sirene-0.0.1/setup.cfg` & `sirene-0.0.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sirene
-version = 0.0.1
+version = 0.0.2
 author = Felipe Morelli Da Silva
 author_email = fms.morelli@gmail.com
 description = Import data from the 'Sistema de Registro Nacional de Emissões' (SIRENE) from MCTI
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/fms-1988
 classifiers =
```

### Comparing `sirene-0.0.1/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_agropecuaria.xlsx` & `sirene-0.0.2/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_agropecuaria.xlsx`

 * *Files identical despite different names*

### Comparing `sirene-0.0.1/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_energia.xlsx` & `sirene-0.0.2/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_energia.xlsx`

 * *Files identical despite different names*

### Comparing `sirene-0.0.1/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_ippu.xlsx` & `sirene-0.0.2/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_ippu.xlsx`

 * *Files identical despite different names*

### Comparing `sirene-0.0.1/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_lulucf.xlsx` & `sirene-0.0.2/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_lulucf.xlsx`

 * *Files identical despite different names*

### Comparing `sirene-0.0.1/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_residuos.xlsx` & `sirene-0.0.2/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_residuos.xlsx`

 * *Files identical despite different names*

### Comparing `sirene-0.0.1/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_total-brasil-1.xlsx` & `sirene-0.0.2/sirene/MCTI/sexta_edicao/estim_6a_ed_1990-2020_total-brasil-1.xlsx`

 * *Files identical despite different names*

### Comparing `sirene-0.0.1/sirene/srn.py` & `sirene-0.0.2/sirene/srn.py`

 * *Files 14% similar despite different names*

```diff
@@ -34,10 +34,12 @@
     bytes_io = io.BytesIO(data)
   df = pd.read_excel(bytes_io, sheet_name=gas)
   df = df.loc[4:4+n,:]
   #set columns names
   new_columns = df.iloc[0]
   df = df[1:]
   df.columns = new_columns
+  df.set_index(df.columns[0], inplace=True)
+  df.rename_axis("NFR_code", inplace=True)
   return df
```

### Comparing `sirene-0.0.1/sirene.egg-info/PKG-INFO` & `sirene-0.0.2/sirene.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sirene
-Version: 0.0.1
+Version: 0.0.2
 Summary: Import data from the 'Sistema de Registro Nacional de Emissões' (SIRENE) from MCTI
 Home-page: https://github.com/fms-1988
 Author: Felipe Morelli Da Silva
 Author-email: fms.morelli@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sirene-0.0.1/sirene.egg-info/SOURCES.txt` & `sirene-0.0.2/sirene.egg-info/SOURCES.txt`

 * *Files identical despite different names*

