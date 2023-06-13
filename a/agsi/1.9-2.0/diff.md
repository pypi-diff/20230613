# Comparing `tmp/agsi-1.9.tar.gz` & `tmp/agsi-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agsi-1.9.tar", last modified: Mon Jun 12 10:27:21 2023, max compression
+gzip compressed data, was "agsi-2.0.tar", last modified: Tue Jun 13 03:48:47 2023, max compression
```

## Comparing `agsi-1.9.tar` & `agsi-2.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:27:21.172641 agsi-1.9/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-1.9/.gitignore
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-12 10:27:21.172641 agsi-1.9/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-1.9/README.md
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:27:21.172641 agsi-1.9/agsi/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-1.9/agsi/__init__.py
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:27:21.172641 agsi-1.9/agsi/data/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)    15761 2023-06-12 10:27:05.000000 agsi-1.9/agsi/data/FarmData.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-1.9/agsi/data/__init__.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)     8953 2023-06-12 10:08:03.000000 agsi-1.9/agsi/data/utils.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)  1079849 2023-06-12 10:26:58.000000 agsi-1.9/agsi/demo_V2.ipynb
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-1.9/agsi/main.py
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-1.9/agsi/requirements.txt
-drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-12 10:27:21.172641 agsi-1.9/agsi.egg-info/
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-12 10:27:21.000000 agsi-1.9/agsi.egg-info/PKG-INFO
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-12 10:27:21.000000 agsi-1.9/agsi.egg-info/SOURCES.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-12 10:27:21.000000 agsi-1.9/agsi.egg-info/dependency_links.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-12 10:27:21.000000 agsi-1.9/agsi.egg-info/requires.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-12 10:27:21.000000 agsi-1.9/agsi.egg-info/top_level.txt
--rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-12 10:27:21.172641 agsi-1.9/setup.cfg
--rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-12 10:27:17.000000 agsi-1.9/setup.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-13 03:48:47.972014 agsi-2.0/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       56 2023-05-26 04:44:18.000000 agsi-2.0/.gitignore
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-13 03:48:47.972014 agsi-2.0/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      190 2023-05-25 15:22:54.000000 agsi-2.0/README.md
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-13 03:48:47.972014 agsi-2.0/agsi/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       35 2023-05-25 15:09:48.000000 agsi-2.0/agsi/__init__.py
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-13 03:48:47.972014 agsi-2.0/agsi/data/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)    15761 2023-06-12 10:27:05.000000 agsi-2.0/agsi/data/FarmData.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        0 2023-05-25 15:09:48.000000 agsi-2.0/agsi/data/__init__.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)     8933 2023-06-13 03:47:37.000000 agsi-2.0/agsi/data/utils.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)  1079849 2023-06-12 10:26:58.000000 agsi-2.0/agsi/demo_V2.ipynb
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       12 2023-05-25 15:09:48.000000 agsi-2.0/agsi/main.py
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      111 2023-05-25 15:09:48.000000 agsi-2.0/agsi/requirements.txt
+drwxrwxr-x   0 sambal    (1000) sambal    (1000)        0 2023-06-13 03:48:47.972014 agsi-2.0/agsi.egg-info/
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      212 2023-06-13 03:48:47.000000 agsi-2.0/agsi.egg-info/PKG-INFO
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      302 2023-06-13 03:48:47.000000 agsi-2.0/agsi.egg-info/SOURCES.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        1 2023-06-13 03:48:47.000000 agsi-2.0/agsi.egg-info/dependency_links.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       60 2023-06-13 03:48:47.000000 agsi-2.0/agsi.egg-info/requires.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)        5 2023-06-13 03:48:47.000000 agsi-2.0/agsi.egg-info/top_level.txt
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)       38 2023-06-13 03:48:47.972014 agsi-2.0/setup.cfg
+-rw-rw-r--   0 sambal    (1000) sambal    (1000)      367 2023-06-13 03:48:40.000000 agsi-2.0/setup.py
```

### Comparing `agsi-1.9/agsi/data/FarmData.py` & `agsi-2.0/agsi/data/FarmData.py`

 * *Files identical despite different names*

### Comparing `agsi-1.9/agsi/data/utils.py` & `agsi-2.0/agsi/data/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -196,18 +196,18 @@
 class Indices():
     def __init__(self,src):
         pass
 
     def __get_stats__(self):
         index_data=np.ma.masked_invalid(self.index_array).compressed()
         data_stats={}
-        data_stats["Max NDVI"]=index_data.max()
-        data_stats["Mean NDVI"]=index_data.mean()
-        data_stats["Median NDVI"]=np.median(index_data)
-        data_stats["Min NDVI"]=index_data.min()
+        data_stats["Max"]=index_data.max()
+        data_stats["Mean"]=index_data.mean()
+        data_stats["Median"]=np.median(index_data)
+        data_stats["Min"]=index_data.min()
         data_stats['skew']=skew(index_data)
         data_stats['kurtosis']=kurtosis(index_data)
         data_stats['skew x kurtosis']=data_stats['skew']*data_stats['kurtosis']
         return data_stats
         
     def get_histogram(self,ax=None):
```

### Comparing `agsi-1.9/agsi/demo_V2.ipynb` & `agsi-2.0/agsi/demo_V2.ipynb`

 * *Files identical despite different names*

