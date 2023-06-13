# Comparing `tmp/NIDDL-0.1.1.tar.gz` & `tmp/NIDDL-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/NIDDL-0.1.1.tar", last modified: Tue Jun 13 18:20:40 2023, max compression
+gzip compressed data, was "dist/NIDDL-0.1.2.tar", last modified: Tue Jun 13 18:27:00 2023, max compression
```

## Comparing `NIDDL-0.1.1.tar` & `NIDDL-0.1.2.tar`

### file list

```diff
@@ -1,44 +1,44 @@
-drwxr-xr-x   0 schaudhary (16379) Domain Users (10513)        0 2023-06-13 18:20:40.551984 NIDDL-0.1.1/
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)    18092 2023-06-13 16:45:02.000000 NIDDL-0.1.1/LICENSE
-drwxr-xr-x   0 schaudhary (16379) Domain Users (10513)        0 2023-06-13 18:20:40.495984 NIDDL-0.1.1/NIDDL.egg-info/
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)      787 2023-06-13 18:20:40.000000 NIDDL-0.1.1/NIDDL.egg-info/PKG-INFO
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)      990 2023-06-13 18:20:40.000000 NIDDL-0.1.1/NIDDL.egg-info/SOURCES.txt
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)        1 2023-06-13 18:20:40.000000 NIDDL-0.1.1/NIDDL.egg-info/dependency_links.txt
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)      718 2023-06-13 18:20:40.000000 NIDDL-0.1.1/NIDDL.egg-info/requires.txt
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)       10 2023-06-13 18:20:40.000000 NIDDL-0.1.1/NIDDL.egg-info/top_level.txt
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)      787 2023-06-13 18:20:40.551984 NIDDL-0.1.1/PKG-INFO
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)    16517 2023-06-13 16:45:02.000000 NIDDL-0.1.1/README.md
-drwxr-xr-x   0 schaudhary (16379) Domain Users (10513)        0 2023-06-13 18:20:40.551984 NIDDL-0.1.1/cnn_archs/
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)      402 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/__init__.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     8284 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/baseline.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     8299 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/baseline_v.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5688 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/baseline_v2.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     6132 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/baseline_v3.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     6136 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/baseline_v4.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     1591 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/basic.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4476 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wores.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4472 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wores_synth.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5088 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wores_v2.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5706 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wores_v3.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4660 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wres.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4660 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wres_k5.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4125 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wres_patch.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4622 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wres_synth.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4311 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wres_tr.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5232 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wres_v2.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5839 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/hourglass_wres_v3.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5579 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/leap.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4656 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4645 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v2.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4641 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v2_synth.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)    14365 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v3.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)    14292 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v4.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     6931 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v4_int_sup.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     7911 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v5_int_sup.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4656 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v_k5.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     3725 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v_patch.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4627 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v_synth.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4283 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v_tr.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4328 2023-06-13 16:45:02.000000 NIDDL-0.1.1/cnn_archs/unet_v_tr_v2.py
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)       38 2023-06-13 18:20:40.551984 NIDDL-0.1.1/setup.cfg
--rw-r--r--   0 schaudhary (16379) Domain Users (10513)     2200 2023-06-13 18:07:02.000000 NIDDL-0.1.1/setup.py
+drwxr-xr-x   0 schaudhary (16379) Domain Users (10513)        0 2023-06-13 18:27:00.833649 NIDDL-0.1.2/
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)    18092 2023-06-13 16:45:02.000000 NIDDL-0.1.2/LICENSE
+drwxr-xr-x   0 schaudhary (16379) Domain Users (10513)        0 2023-06-13 18:27:00.781649 NIDDL-0.1.2/NIDDL.egg-info/
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)    17033 2023-06-13 18:27:00.000000 NIDDL-0.1.2/NIDDL.egg-info/PKG-INFO
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)      990 2023-06-13 18:27:00.000000 NIDDL-0.1.2/NIDDL.egg-info/SOURCES.txt
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)        1 2023-06-13 18:27:00.000000 NIDDL-0.1.2/NIDDL.egg-info/dependency_links.txt
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)      718 2023-06-13 18:27:00.000000 NIDDL-0.1.2/NIDDL.egg-info/requires.txt
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)       10 2023-06-13 18:27:00.000000 NIDDL-0.1.2/NIDDL.egg-info/top_level.txt
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)    17033 2023-06-13 18:27:00.833649 NIDDL-0.1.2/PKG-INFO
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)    16517 2023-06-13 16:45:02.000000 NIDDL-0.1.2/README.md
+drwxr-xr-x   0 schaudhary (16379) Domain Users (10513)        0 2023-06-13 18:27:00.833649 NIDDL-0.1.2/cnn_archs/
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)      402 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/__init__.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     8284 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/baseline.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     8299 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/baseline_v.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5688 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/baseline_v2.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     6132 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/baseline_v3.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     6136 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/baseline_v4.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     1591 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/basic.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4476 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/hourglass_wores.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4472 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/hourglass_wores_synth.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5088 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/hourglass_wores_v2.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5706 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/hourglass_wores_v3.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4660 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/hourglass_wres.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4660 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/hourglass_wres_k5.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4125 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/hourglass_wres_patch.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4622 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/hourglass_wres_synth.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4311 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/hourglass_wres_tr.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5232 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/hourglass_wres_v2.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5839 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/hourglass_wres_v3.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     5579 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/leap.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4656 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/unet_v.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4645 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/unet_v2.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4641 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/unet_v2_synth.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)    14365 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/unet_v3.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)    14292 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/unet_v4.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     6931 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/unet_v4_int_sup.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     7911 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/unet_v5_int_sup.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4656 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/unet_v_k5.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     3725 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/unet_v_patch.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4627 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/unet_v_synth.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4283 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/unet_v_tr.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     4328 2023-06-13 16:45:02.000000 NIDDL-0.1.2/cnn_archs/unet_v_tr_v2.py
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)       38 2023-06-13 18:27:00.833649 NIDDL-0.1.2/setup.cfg
+-rw-r--r--   0 schaudhary (16379) Domain Users (10513)     2325 2023-06-13 18:26:51.000000 NIDDL-0.1.2/setup.py
```

### Comparing `NIDDL-0.1.1/LICENSE` & `NIDDL-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/NIDDL.egg-info/SOURCES.txt` & `NIDDL-0.1.2/NIDDL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/NIDDL.egg-info/requires.txt` & `NIDDL-0.1.2/NIDDL.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/README.md` & `NIDDL-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/baseline.py` & `NIDDL-0.1.2/cnn_archs/baseline.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/baseline_v.py` & `NIDDL-0.1.2/cnn_archs/baseline_v.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/baseline_v2.py` & `NIDDL-0.1.2/cnn_archs/baseline_v2.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/baseline_v3.py` & `NIDDL-0.1.2/cnn_archs/baseline_v3.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/baseline_v4.py` & `NIDDL-0.1.2/cnn_archs/baseline_v4.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/basic.py` & `NIDDL-0.1.2/cnn_archs/basic.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/hourglass_wores.py` & `NIDDL-0.1.2/cnn_archs/hourglass_wores.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/hourglass_wores_synth.py` & `NIDDL-0.1.2/cnn_archs/hourglass_wores_synth.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/hourglass_wores_v2.py` & `NIDDL-0.1.2/cnn_archs/hourglass_wores_v2.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/hourglass_wores_v3.py` & `NIDDL-0.1.2/cnn_archs/hourglass_wores_v3.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/hourglass_wres.py` & `NIDDL-0.1.2/cnn_archs/hourglass_wres.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/hourglass_wres_k5.py` & `NIDDL-0.1.2/cnn_archs/hourglass_wres_k5.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/hourglass_wres_patch.py` & `NIDDL-0.1.2/cnn_archs/hourglass_wres_patch.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/hourglass_wres_synth.py` & `NIDDL-0.1.2/cnn_archs/hourglass_wres_synth.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/hourglass_wres_tr.py` & `NIDDL-0.1.2/cnn_archs/hourglass_wres_tr.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/hourglass_wres_v2.py` & `NIDDL-0.1.2/cnn_archs/hourglass_wres_v2.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/hourglass_wres_v3.py` & `NIDDL-0.1.2/cnn_archs/hourglass_wres_v3.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/leap.py` & `NIDDL-0.1.2/cnn_archs/leap.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/unet_v.py` & `NIDDL-0.1.2/cnn_archs/unet_v.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/unet_v2.py` & `NIDDL-0.1.2/cnn_archs/unet_v2.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/unet_v2_synth.py` & `NIDDL-0.1.2/cnn_archs/unet_v2_synth.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/unet_v3.py` & `NIDDL-0.1.2/cnn_archs/unet_v3.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/unet_v4.py` & `NIDDL-0.1.2/cnn_archs/unet_v4.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/unet_v4_int_sup.py` & `NIDDL-0.1.2/cnn_archs/unet_v4_int_sup.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/unet_v5_int_sup.py` & `NIDDL-0.1.2/cnn_archs/unet_v5_int_sup.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/unet_v_k5.py` & `NIDDL-0.1.2/cnn_archs/unet_v_k5.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/unet_v_patch.py` & `NIDDL-0.1.2/cnn_archs/unet_v_patch.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/unet_v_synth.py` & `NIDDL-0.1.2/cnn_archs/unet_v_synth.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/unet_v_tr.py` & `NIDDL-0.1.2/cnn_archs/unet_v_tr.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/cnn_archs/unet_v_tr_v2.py` & `NIDDL-0.1.2/cnn_archs/unet_v_tr_v2.py`

 * *Files identical despite different names*

### Comparing `NIDDL-0.1.1/setup.py` & `NIDDL-0.1.2/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,23 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.1.1'
+VERSION = '0.1.2'
 DESCRIPTION = 'Neuro Imaging Denoising via Deep Learning (NIDDL)'
-LONG_DESCRIPTION = 'NIDDL code for denoising of volumetric calcium imaging recordings. \
-        If you find our code useful please cite \
-        Chaudhary, S., Moon, S. & Lu, H. Fast, efficient, and accurate neuro-imaging denoising via supervised deep learning. Nat Commun 13, 5165 (2022). https://doi.org/10.1038/s41467-022-32886-w'
+with open("README.md", "r") as fh:
+    LONG_DESCRIPTION = fh.read()
+# LONG_DESCRIPTION = 'NIDDL code for denoising of volumetric calcium imaging recordings. \
+#         If you find our code useful please cite \
+#         Chaudhary, S., Moon, S. & Lu, H. Fast, efficient, and accurate neuro-imaging denoising via supervised deep learning. Nat Commun 13, 5165 (2022). https://doi.org/10.1038/s41467-022-32886-w'
 
 setup(
     name="NIDDL",
     version=VERSION,
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
+    long_description_content_type="text/markdown",
     author="Shivesh Chaudhary",
     author_email="shiveshc@gmail.com",
     license='MIT',
     packages=find_packages(),
     url='https://github.com/shiveshc/whole-brain_DeepDenoising',
     install_requires=[
         'absl-py==0.11.0',
```

