# Comparing `tmp/NIDDL-0.1.0.tar.gz` & `tmp/NIDDL-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "NIDDL-0.1.0.tar", last modified: Tue Jun 13 17:52:27 2023, max compression
+gzip compressed data, was "dist/NIDDL-0.1.1.tar", last modified: Tue Jun 13 18:20:40 2023, max compression
```

## Comparing `NIDDL-0.1.0.tar` & `NIDDL-0.1.1.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 schaudhary (16379) Domain Users (10513)        0 2023-06-13 17:52:27.031268 NIDDL-0.1.0/
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)    18092 2023-06-13 16:45:02.000000 NIDDL-0.1.0/LICENSE
-drwxr-xr-x   0 schaudhary (16379) Domain Users (10513)        0 2023-06-13 17:52:26.967269 NIDDL-0.1.0/NIDDL.egg-info/
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)      731 2023-06-13 17:52:26.000000 NIDDL-0.1.0/NIDDL.egg-info/PKG-INFO
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)      990 2023-06-13 17:52:26.000000 NIDDL-0.1.0/NIDDL.egg-info/SOURCES.txt
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)        1 2023-06-13 17:52:26.000000 NIDDL-0.1.0/NIDDL.egg-info/dependency_links.txt
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)      718 2023-06-13 17:52:26.000000 NIDDL-0.1.0/NIDDL.egg-info/requires.txt
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)       10 2023-06-13 17:52:26.000000 NIDDL-0.1.0/NIDDL.egg-info/top_level.txt
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)      731 2023-06-13 17:52:27.031268 NIDDL-0.1.0/PKG-INFO
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)    16517 2023-06-13 16:45:02.000000 NIDDL-0.1.0/README.md
-drwxr-xr-x   0 schaudhary (16379) Domain Users (10513)        0 2023-06-13 17:52:27.027269 NIDDL-0.1.0/cnn_archs/
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)      402 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/__init__.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     8284 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/baseline.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     8299 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/baseline_v.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5688 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/baseline_v2.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     6132 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/baseline_v3.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     6136 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/baseline_v4.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     1591 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/basic.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4476 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/hourglass_wores.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4472 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/hourglass_wores_synth.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5088 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/hourglass_wores_v2.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5706 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/hourglass_wores_v3.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4660 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/hourglass_wres.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4660 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/hourglass_wres_k5.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4125 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/hourglass_wres_patch.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4622 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/hourglass_wres_synth.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4311 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/hourglass_wres_tr.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5232 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/hourglass_wres_v2.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5839 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/hourglass_wres_v3.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5579 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/leap.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4656 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/unet_v.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4645 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/unet_v2.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4641 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/unet_v2_synth.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)    14365 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/unet_v3.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)    14292 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/unet_v4.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     6931 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/unet_v4_int_sup.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     7911 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/unet_v5_int_sup.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4656 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/unet_v_k5.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     3725 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/unet_v_patch.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4627 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/unet_v_synth.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4283 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/unet_v_tr.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4328 2023-06-13 16:45:02.000000 NIDDL-0.1.0/cnn_archs/unet_v_tr_v2.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)       38 2023-06-13 17:52:27.031268 NIDDL-0.1.0/setup.cfg
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     2140 2023-06-13 17:51:18.000000 NIDDL-0.1.0/setup.py
+drwxr-xr-x   0 schaudhary (16379) Domain Users (10513)        0 2023-06-13 18:20:40.551984 NIDDL-0.1.1/
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)    18092 2023-06-13 16:45:02.000000 NIDDL-0.1.1/LICENSE
+drwxr-xr-x   0 schaudhary (16379) Domain Users (10513)        0 2023-06-13 18:20:40.495984 NIDDL-0.1.1/NIDDL.egg-info/
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)      787 2023-06-13 18:20:40.000000 NIDDL-0.1.1/NIDDL.egg-info/PKG-INFO
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)      990 2023-06-13 18:20:40.000000 NIDDL-0.1.1/NIDDL.egg-info/SOURCES.txt
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)        1 2023-06-13 18:20:40.000000 NIDDL-0.1.1/NIDDL.egg-info/dependency_links.txt
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)      718 2023-06-13 18:20:40.000000 NIDDL-0.1.1/NIDDL.egg-info/requires.txt
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)       10 2023-06-13 18:20:40.000000 NIDDL-0.1.1/NIDDL.egg-info/top_level.txt
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)      787 2023-06-13 18:20:40.551984 NIDDL-0.1.1/PKG-INFO
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)    16517 2023-06-13 16:45:02.000000 NIDDL-0.1.1/README.md
+drwxr-xr-x   0 schaudhary (16379) Domain Users (10513)        0 2023-06-13 18:20:40.551984 NIDDL-0.1.1/cnn_archs/
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)      402 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/__init__.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     8284 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/baseline.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     8299 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/baseline_v.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5688 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/baseline_v2.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     6132 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/baseline_v3.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     6136 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/baseline_v4.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     1591 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/basic.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4476 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wores.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4472 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wores_synth.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5088 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wores_v2.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5706 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wores_v3.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4660 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wres.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4660 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wres_k5.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4125 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wres_patch.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4622 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wres_synth.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4311 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wres_tr.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5232 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wres_v2.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5839 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wres_v3.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5579 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/leap.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4656 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4645 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v2.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4641 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v2_synth.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)    14365 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v3.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)    14292 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v4.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     6931 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v4_int_sup.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     7911 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v5_int_sup.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4656 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v_k5.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     3725 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v_patch.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4627 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v_synth.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4283 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v_tr.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4328 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v_tr_v2.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)       38 2023-06-13 18:20:40.551984 NIDDL-0.1.1/setup.cfg
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     2200 2023-06-13 18:07:02.000000 NIDDL-0.1.1/setup.py
```

### Comparing `NIDDL-0.1.0/LICENSE` & `NIDDL-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/NIDDL.egg-info/PKG-INFO` & `NIDDL-0.1.1/NIDDL.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: NIDDL
-Version: 0.1.0
+Version: 0.1.1
 Summary: Neuro Imaging Denoising via Deep Learning (NIDDL)
 Home-page: https://github.com/shiveshc/whole-brain_DeepDenoising
 Author: Shivesh Chaudhary
 Author-email: shiveshc@gmail.com
 License: MIT
 Keywords: conversion
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
-NIDDL code for denoising of volumetric calcium imaging recordings. Chaudhary, S., Moon, S. & Lu, H. Fast, efficient, and accurate neuro-imaging denoising via supervised deep learning. Nat Commun 13, 5165 (2022). https://doi.org/10.1038/s41467-022-32886-w
+NIDDL code for denoising of volumetric calcium imaging recordings.         If you find our code useful please cite         Chaudhary, S., Moon, S. & Lu, H. Fast, efficient, and accurate neuro-imaging denoising via supervised deep learning. Nat Commun 13, 5165 (2022). https://doi.org/10.1038/s41467-022-32886-w
```

### Comparing `NIDDL-0.1.0/NIDDL.egg-info/SOURCES.txt` & `NIDDL-0.1.1/NIDDL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/NIDDL.egg-info/requires.txt` & `NIDDL-0.1.1/NIDDL.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/PKG-INFO` & `NIDDL-0.1.1/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: NIDDL
-Version: 0.1.0
+Version: 0.1.1
 Summary: Neuro Imaging Denoising via Deep Learning (NIDDL)
 Home-page: https://github.com/shiveshc/whole-brain_DeepDenoising
 Author: Shivesh Chaudhary
 Author-email: shiveshc@gmail.com
 License: MIT
 Keywords: conversion
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 License-File: LICENSE
 
-NIDDL code for denoising of volumetric calcium imaging recordings. Chaudhary, S., Moon, S. & Lu, H. Fast, efficient, and accurate neuro-imaging denoising via supervised deep learning. Nat Commun 13, 5165 (2022). https://doi.org/10.1038/s41467-022-32886-w
+NIDDL code for denoising of volumetric calcium imaging recordings.         If you find our code useful please cite         Chaudhary, S., Moon, S. & Lu, H. Fast, efficient, and accurate neuro-imaging denoising via supervised deep learning. Nat Commun 13, 5165 (2022). https://doi.org/10.1038/s41467-022-32886-w
```

### Comparing `NIDDL-0.1.0/README.md` & `NIDDL-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/baseline.py` & `NIDDL-0.1.1/cnn_archs/baseline.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/baseline_v.py` & `NIDDL-0.1.1/cnn_archs/baseline_v.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/baseline_v2.py` & `NIDDL-0.1.1/cnn_archs/baseline_v2.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/baseline_v3.py` & `NIDDL-0.1.1/cnn_archs/baseline_v3.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/baseline_v4.py` & `NIDDL-0.1.1/cnn_archs/baseline_v4.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/basic.py` & `NIDDL-0.1.1/cnn_archs/basic.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/hourglass_wores.py` & `NIDDL-0.1.1/cnn_archs/hourglass_wores.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/hourglass_wores_synth.py` & `NIDDL-0.1.1/cnn_archs/hourglass_wores_synth.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/hourglass_wores_v2.py` & `NIDDL-0.1.1/cnn_archs/hourglass_wores_v2.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/hourglass_wores_v3.py` & `NIDDL-0.1.1/cnn_archs/hourglass_wores_v3.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/hourglass_wres.py` & `NIDDL-0.1.1/cnn_archs/hourglass_wres.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/hourglass_wres_k5.py` & `NIDDL-0.1.1/cnn_archs/hourglass_wres_k5.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/hourglass_wres_patch.py` & `NIDDL-0.1.1/cnn_archs/hourglass_wres_patch.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/hourglass_wres_synth.py` & `NIDDL-0.1.1/cnn_archs/hourglass_wres_synth.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/hourglass_wres_tr.py` & `NIDDL-0.1.1/cnn_archs/hourglass_wres_tr.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/hourglass_wres_v2.py` & `NIDDL-0.1.1/cnn_archs/hourglass_wres_v2.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/hourglass_wres_v3.py` & `NIDDL-0.1.1/cnn_archs/hourglass_wres_v3.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/leap.py` & `NIDDL-0.1.1/cnn_archs/leap.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/unet_v.py` & `NIDDL-0.1.1/cnn_archs/unet_v.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/unet_v2.py` & `NIDDL-0.1.1/cnn_archs/unet_v2.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/unet_v2_synth.py` & `NIDDL-0.1.1/cnn_archs/unet_v2_synth.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/unet_v3.py` & `NIDDL-0.1.1/cnn_archs/unet_v3.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/unet_v4.py` & `NIDDL-0.1.1/cnn_archs/unet_v4.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/unet_v4_int_sup.py` & `NIDDL-0.1.1/cnn_archs/unet_v4_int_sup.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/unet_v5_int_sup.py` & `NIDDL-0.1.1/cnn_archs/unet_v5_int_sup.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/unet_v_k5.py` & `NIDDL-0.1.1/cnn_archs/unet_v_k5.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/unet_v_patch.py` & `NIDDL-0.1.1/cnn_archs/unet_v_patch.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/unet_v_synth.py` & `NIDDL-0.1.1/cnn_archs/unet_v_synth.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/unet_v_tr.py` & `NIDDL-0.1.1/cnn_archs/unet_v_tr.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/cnn_archs/unet_v_tr_v2.py` & `NIDDL-0.1.1/cnn_archs/unet_v_tr_v2.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.0/setup.py` & `NIDDL-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.1.1'
 DESCRIPTION = 'Neuro Imaging Denoising via Deep Learning (NIDDL)'
-LONG_DESCRIPTION = 'NIDDL code for denoising of volumetric calcium imaging recordings. Chaudhary, S., Moon, S. & Lu, H. Fast, efficient, and accurate neuro-imaging denoising via supervised deep learning. Nat Commun 13, 5165 (2022). https://doi.org/10.1038/s41467-022-32886-w'
+LONG_DESCRIPTION = 'NIDDL code for denoising of volumetric calcium imaging recordings. \
+        If you find our code useful please cite \
+        Chaudhary, S., Moon, S. & Lu, H. Fast, efficient, and accurate neuro-imaging denoising via supervised deep learning. Nat Commun 13, 5165 (2022). https://doi.org/10.1038/s41467-022-32886-w'
 
 setup(
     name="NIDDL",
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     author="Shivesh Chaudhary",
```

