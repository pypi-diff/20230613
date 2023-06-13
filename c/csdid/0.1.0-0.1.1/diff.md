# Comparing `tmp/csdid-0.1.0.tar.gz` & `tmp/csdid-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "csdid-0.1.0.tar", last modified: Tue Jun 13 21:38:09 2023, max compression
+gzip compressed data, was "csdid-0.1.1.tar", last modified: Tue Jun 13 21:42:24 2023, max compression
```

## Comparing `csdid-0.1.0.tar` & `csdid-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 21:38:09.911240 csdid-0.1.0/
--rw-rw-rw-   0        0        0     1126 2023-06-13 21:34:25.000000 csdid-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      533 2023-06-13 21:38:09.911240 csdid-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-13 21:38:09.898237 csdid-0.1.0/csdid/
--rw-rw-rw-   0        0        0        0 2023-06-13 15:53:11.000000 csdid-0.1.0/csdid/__init__.py
--rw-rw-rw-   0        0        0     3816 2023-06-13 20:37:34.000000 csdid-0.1.0/csdid/att_gt.py
-drwxrwxrwx   0        0        0        0 2023-06-13 21:38:09.910240 csdid-0.1.0/csdid.egg-info/
--rw-rw-rw-   0        0        0      533 2023-06-13 21:38:09.000000 csdid-0.1.0/csdid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      166 2023-06-13 21:38:09.000000 csdid-0.1.0/csdid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 21:38:09.000000 csdid-0.1.0/csdid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        6 2023-06-13 21:38:09.000000 csdid-0.1.0/csdid.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 21:38:09.912240 csdid-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      607 2023-06-13 21:38:07.000000 csdid-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 21:42:24.484894 csdid-0.1.1/
+-rw-rw-rw-   0        0        0     1126 2023-06-13 21:34:25.000000 csdid-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      533 2023-06-13 21:42:24.484894 csdid-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 21:42:24.476892 csdid-0.1.1/csdid/
+-rw-rw-rw-   0        0        0        0 2023-06-13 15:53:11.000000 csdid-0.1.1/csdid/__init__.py
+-rw-rw-rw-   0        0        0     3822 2023-06-13 21:42:09.000000 csdid-0.1.1/csdid/att_gt.py
+drwxrwxrwx   0        0        0        0 2023-06-13 21:42:24.483894 csdid-0.1.1/csdid.egg-info/
+-rw-rw-rw-   0        0        0      533 2023-06-13 21:42:24.000000 csdid-0.1.1/csdid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      166 2023-06-13 21:42:24.000000 csdid-0.1.1/csdid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 21:42:24.000000 csdid-0.1.1/csdid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-13 21:42:24.000000 csdid-0.1.1/csdid.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 21:42:24.484894 csdid-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      608 2023-06-13 21:42:22.000000 csdid-0.1.1/setup.py
```

### Comparing `csdid-0.1.0/LICENSE` & `csdid-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `csdid-0.1.0/PKG-INFO` & `csdid-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.0
+Version: 0.1.1
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.0/csdid/att_gt.py` & `csdid-0.1.1/csdid/att_gt.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 # from aggte import AGGte
-from aggte_fnc.aggte import aggte as agg_te
+from .aggte_fnc.aggte import aggte as agg_te
 
-from attgt_fnc.preprocess_did import pre_process_did
-from attgt_fnc.compute_att_gt import compute_att_gt
+from .attgt_fnc.preprocess_did import pre_process_did
+from .attgt_fnc.compute_att_gt import compute_att_gt
+
+from .utils.mboot import mboot
 
-from utils.mboot import mboot
 import numpy as np
 
 # class ATTgt(AGGte):
 class ATTgt:
   def __init__(self, yname, tname, idname, gname, data, control_group = ['nevertreated', 'notyertreated'], 
   xformla: str = None, panel = True, allow_unbalanced_panel = True, 
   clustervar = None, weights_name = None, anticipation = 0,
```

### Comparing `csdid-0.1.0/csdid.egg-info/PKG-INFO` & `csdid-0.1.1/csdid.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: csdid
-Version: 0.1.0
+Version: 0.1.1
 Summary: Difference in Difference in Python
 Home-page: https://github.com/d2cml-ai/csdid
 Author: D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes
 License: MIT
 Keywords: Causal inference,Research
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Education
```

### Comparing `csdid-0.1.0/setup.py` & `csdid-0.1.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
   name = 'csdid',
-  version='0.1.0',
+  version='0.1.01',
   url='https://github.com/d2cml-ai/csdid',
   author='D2CML Team, Alexander Quispe, Carlos Guevara, Jhon Flroes',
   keywords=['Causal inference', 'Research'],
   license="MIT",
   description='Difference in Difference in Python',
   classifiers=[
         "Intended Audience :: Developers",
```

