# Comparing `tmp/portpy-0.0.2.tar.gz` & `tmp/portpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\portpy-0.0.2.tar", last modified: Sun Jun 11 19:16:31 2023, max compression
+gzip compressed data, was "dist\portpy-0.0.3.tar", last modified: Tue Jun 13 17:00:01 2023, max compression
```

## Comparing `portpy-0.0.2.tar` & `portpy-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 19:16:32.000000 portpy-0.0.2/
--rw-rw-rw-   0        0        0      128 2023-05-12 06:19:04.000000 portpy-0.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0     7798 2023-06-11 19:16:32.000000 portpy-0.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     6192 2023-06-06 19:15:25.000000 portpy-0.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/config_files/
-drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/config_files/clinical_criteria/
-drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/config_files/clinical_criteria/Default/
--rw-rw-rw-   0        0        0     2511 2023-01-19 21:58:41.000000 portpy-0.0.2/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
-drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/config_files/optimization_params/
--rw-rw-rw-   0        0        0     2419 2023-05-13 03:05:59.000000 portpy-0.0.2/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
-drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/images/
--rw-rw-rw-   0        0        0   184526 2023-05-12 05:53:35.000000 portpy-0.0.2/images/PortPy_logo.jpg
-drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/portpy/
--rw-rw-rw-   0        0        0       52 2023-05-12 06:21:33.000000 portpy-0.0.2/portpy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/portpy/photon/
--rw-rw-rw-   0        0        0      430 2023-05-10 05:07:25.000000 portpy-0.0.2/portpy/photon/__init__.py
--rw-rw-rw-   0        0        0     8340 2023-05-15 03:35:09.000000 portpy-0.0.2/portpy/photon/beam.py
--rw-rw-rw-   0        0        0     4992 2023-05-13 03:47:18.000000 portpy-0.0.2/portpy/photon/clinical_criteria.py
--rw-rw-rw-   0        0        0      548 2023-05-11 18:21:16.000000 portpy-0.0.2/portpy/photon/ct.py
--rw-rw-rw-   0        0        0    18530 2023-05-13 03:32:20.000000 portpy-0.0.2/portpy/photon/cvxpy_prob.py
--rw-rw-rw-   0        0        0    23387 2023-05-17 10:37:53.000000 portpy-0.0.2/portpy/photon/data_explorer.py
--rw-rw-rw-   0        0        0    14619 2023-05-13 03:32:20.000000 portpy-0.0.2/portpy/photon/evaluation.py
--rw-rw-rw-   0        0        0    53003 2023-06-07 19:53:55.000000 portpy-0.0.2/portpy/photon/influence_matrix.py
--rw-rw-rw-   0        0        0    23374 2023-05-17 09:39:36.000000 portpy-0.0.2/portpy/photon/optimization.py
--rw-rw-rw-   0        0        0    10945 2023-05-17 09:34:05.000000 portpy-0.0.2/portpy/photon/plan.py
--rw-rw-rw-   0        0        0    16378 2023-05-15 03:42:09.000000 portpy-0.0.2/portpy/photon/structures.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/portpy/photon/utils/
--rw-rw-rw-   0        0        0      262 2023-05-16 17:51:57.000000 portpy-0.0.2/portpy/photon/utils/__init__.py
--rw-rw-rw-   0        0        0     2058 2023-05-17 06:00:15.000000 portpy-0.0.2/portpy/photon/utils/get_eclipse_fluence.py
--rw-rw-rw-   0        0        0     5415 2023-05-12 05:53:35.000000 portpy-0.0.2/portpy/photon/utils/load_data.py
--rw-rw-rw-   0        0        0     4828 2023-05-12 05:53:35.000000 portpy-0.0.2/portpy/photon/utils/load_metadata.py
--rw-rw-rw-   0        0        0     2846 2023-05-15 12:19:37.000000 portpy-0.0.2/portpy/photon/utils/save_nrrd.py
--rw-rw-rw-   0        0        0     4887 2023-05-15 11:43:22.000000 portpy-0.0.2/portpy/photon/utils/save_or_load_pickle.py
--rw-rw-rw-   0        0        0     1387 2023-05-09 07:09:19.000000 portpy-0.0.2/portpy/photon/utils/slicer_script.py
--rw-rw-rw-   0        0        0     1347 2023-03-27 19:08:24.000000 portpy-0.0.2/portpy/photon/utils/sol_change_inf_matrix.py
--rw-rw-rw-   0        0        0     4132 2023-05-09 07:09:19.000000 portpy-0.0.2/portpy/photon/utils/view_in_slicer_jupyter.py
--rw-rw-rw-   0        0        0    20553 2023-05-15 11:48:55.000000 portpy-0.0.2/portpy/photon/visualization.py
-drwxrwxrwx   0        0        0        0 2023-06-11 19:16:31.000000 portpy-0.0.2/portpy.egg-info/
--rw-rw-rw-   0        0        0     7798 2023-06-11 19:16:28.000000 portpy-0.0.2/portpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1035 2023-06-11 19:16:28.000000 portpy-0.0.2/portpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 19:16:28.000000 portpy-0.0.2/portpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      352 2023-06-11 19:16:28.000000 portpy-0.0.2/portpy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-06-11 19:16:28.000000 portpy-0.0.2/portpy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-11 19:16:32.000000 portpy-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0     2502 2023-05-30 02:26:49.000000 portpy-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:00:01.000000 portpy-0.0.3/
+-rw-rw-rw-   0        0        0      142 2023-06-13 16:08:24.000000 portpy-0.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     7804 2023-06-13 17:00:01.000000 portpy-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     6198 2023-06-12 04:36:17.000000 portpy-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/config_files/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/config_files/clinical_criteria/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/config_files/clinical_criteria/Default/
+-rw-rw-rw-   0        0        0     2511 2023-01-19 21:58:41.000000 portpy-0.0.3/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/config_files/optimization_params/
+-rw-rw-rw-   0        0        0     2419 2023-05-13 03:05:59.000000 portpy-0.0.3/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/images/
+-rw-rw-rw-   0        0        0   184526 2023-05-12 05:53:35.000000 portpy-0.0.3/images/PortPy_logo.jpg
+drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy/
+-rw-rw-rw-   0        0        0       52 2023-06-13 16:55:29.000000 portpy-0.0.3/portpy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy/config_files/
+-rw-rw-rw-   0        0        0        0 2023-06-13 16:25:21.000000 portpy-0.0.3/portpy/config_files/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy/config_files/clinical_criteria/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy/config_files/clinical_criteria/Default/
+-rw-rw-rw-   0        0        0     2511 2023-01-19 21:58:41.000000 portpy-0.0.3/portpy/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy/config_files/optimization_params/
+-rw-rw-rw-   0        0        0     2419 2023-05-13 03:05:59.000000 portpy-0.0.3/portpy/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json
+drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy/photon/
+-rw-rw-rw-   0        0        0      395 2023-06-12 21:08:08.000000 portpy-0.0.3/portpy/photon/__init__.py
+-rw-rw-rw-   0        0        0     8340 2023-05-15 03:35:09.000000 portpy-0.0.3/portpy/photon/beam.py
+-rw-rw-rw-   0        0        0     4994 2023-06-13 15:49:21.000000 portpy-0.0.3/portpy/photon/clinical_criteria.py
+-rw-rw-rw-   0        0        0      702 2023-06-13 15:15:28.000000 portpy-0.0.3/portpy/photon/ct.py
+-rw-rw-rw-   0        0        0    23345 2023-06-13 16:28:27.000000 portpy-0.0.3/portpy/photon/data_explorer.py
+-rw-rw-rw-   0        0        0    15041 2023-06-13 16:20:52.000000 portpy-0.0.3/portpy/photon/evaluation.py
+-rw-rw-rw-   0        0        0    48775 2023-06-13 15:28:29.000000 portpy-0.0.3/portpy/photon/influence_matrix.py
+-rw-rw-rw-   0        0        0    22066 2023-06-13 16:00:14.000000 portpy-0.0.3/portpy/photon/optimization.py
+-rw-rw-rw-   0        0        0     5806 2023-06-13 15:50:40.000000 portpy-0.0.3/portpy/photon/plan.py
+-rw-rw-rw-   0        0        0    16378 2023-05-15 03:42:09.000000 portpy-0.0.3/portpy/photon/structures.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy/photon/utils/
+-rw-rw-rw-   0        0        0      264 2023-06-12 21:08:08.000000 portpy-0.0.3/portpy/photon/utils/__init__.py
+-rw-rw-rw-   0        0        0     2058 2023-05-17 06:00:15.000000 portpy-0.0.3/portpy/photon/utils/get_eclipse_fluence.py
+-rw-rw-rw-   0        0        0     2846 2023-05-15 12:19:37.000000 portpy-0.0.3/portpy/photon/utils/save_nrrd.py
+-rw-rw-rw-   0        0        0     4887 2023-05-15 11:43:22.000000 portpy-0.0.3/portpy/photon/utils/save_or_load_pickle.py
+-rw-rw-rw-   0        0        0     1387 2023-05-09 07:09:19.000000 portpy-0.0.3/portpy/photon/utils/slicer_script.py
+-rw-rw-rw-   0        0        0     4188 2023-06-12 16:42:02.000000 portpy-0.0.3/portpy/photon/utils/view_in_slicer_jupyter.py
+-rw-rw-rw-   0        0        0    24087 2023-06-13 15:27:59.000000 portpy-0.0.3/portpy/photon/visualization.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:00:00.000000 portpy-0.0.3/portpy.egg-info/
+-rw-rw-rw-   0        0        0     7804 2023-06-13 16:59:57.000000 portpy-0.0.3/portpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1068 2023-06-13 16:59:57.000000 portpy-0.0.3/portpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 16:59:57.000000 portpy-0.0.3/portpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      352 2023-06-13 16:59:57.000000 portpy-0.0.3/portpy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-06-13 16:59:57.000000 portpy-0.0.3/portpy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 17:00:01.000000 portpy-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0     2502 2023-05-30 02:26:49.000000 portpy-0.0.3/setup.py
```

### Comparing `portpy-0.0.2/PKG-INFO` & `portpy-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: First open-source radiation treatment planning system in Python
 Home-page: https://github.com/PortPy-Project/PortPy
 Author: Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh
 Author-email: jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct
 License: Apache License, Version 2.0
 Description: <p align="center">
           <img src="./images/PortPy_logo.jpg" width="50%">
@@ -26,15 +26,15 @@
         Create a directory named './data' in the current project directory and copy the downloaded file to it, e.g ./data/Lung_Phantom_Patient_1
         
         # Quick Start
         Please see below for understanding the basic functionalities of PortPy. For advance usage of PortPy, we recommend navigating through [examples](https://github.com/PortPy-Project/PortPy/tree/master/examples) folder.
         1. To understand the most important features of PortPy, we highly recommend to go through notebook [ex_1_introduction.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_1_introduction.ipynb)
         2. One of the major computational issues while optimizing the plan arise due to large size of influence matrix. We suggest you to follow [ex_2_down_sampling.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_2_downsampling.py) to understand how PortPy can assist in resolving it.
         3. You can check out [ex_3_structure_operations.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_3_structure_operations.py) to know how to perform different structure operations (e.g., boolean, margin).
-        4. For algorithm benchmarking, the global optimal solution is provided for non-convex optimization problems resulting from beam angle optimization [ex_6_boo_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_boo_benchmark.py) and incorporating DVH constraints [ex_6_dvh_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_dvh_benchmark.py) using the mixed-integer programming on down-sampled data.
+        4. For algorithm benchmarking, the global optimal solution is provided for non-convex optimization problems resulting from beam angle optimization [ex_6_boo_benchmark.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_boo_benchmark.ipynb) and incorporating DVH constraints [ex_6_dvh_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_dvh_benchmark.py) using the mixed-integer programming on down-sampled data.
         5. In addition to basic visualization capabilities, PortPy provide advanced visualization by integration with 3D Slicer. Please look out notebook [ex_7_Slicer.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_7_Slicer.ipynb)
         
         # Installing PortPy
         
         1. Installing using pip
           ```bash
           pip install portpy
```

### Comparing `portpy-0.0.2/README.md` & `portpy-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 Create a directory named './data' in the current project directory and copy the downloaded file to it, e.g ./data/Lung_Phantom_Patient_1
 
 # Quick Start
 Please see below for understanding the basic functionalities of PortPy. For advance usage of PortPy, we recommend navigating through [examples](https://github.com/PortPy-Project/PortPy/tree/master/examples) folder.
 1. To understand the most important features of PortPy, we highly recommend to go through notebook [ex_1_introduction.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_1_introduction.ipynb)
 2. One of the major computational issues while optimizing the plan arise due to large size of influence matrix. We suggest you to follow [ex_2_down_sampling.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_2_downsampling.py) to understand how PortPy can assist in resolving it.
 3. You can check out [ex_3_structure_operations.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_3_structure_operations.py) to know how to perform different structure operations (e.g., boolean, margin).
-4. For algorithm benchmarking, the global optimal solution is provided for non-convex optimization problems resulting from beam angle optimization [ex_6_boo_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_boo_benchmark.py) and incorporating DVH constraints [ex_6_dvh_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_dvh_benchmark.py) using the mixed-integer programming on down-sampled data.
+4. For algorithm benchmarking, the global optimal solution is provided for non-convex optimization problems resulting from beam angle optimization [ex_6_boo_benchmark.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_boo_benchmark.ipynb) and incorporating DVH constraints [ex_6_dvh_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_dvh_benchmark.py) using the mixed-integer programming on down-sampled data.
 5. In addition to basic visualization capabilities, PortPy provide advanced visualization by integration with 3D Slicer. Please look out notebook [ex_7_Slicer.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_7_Slicer.ipynb)
 
 # Installing PortPy
 
 1. Installing using pip
   ```bash
   pip install portpy
```

### Comparing `portpy-0.0.2/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json` & `portpy-0.0.3/config_files/clinical_criteria/Default/Lung_2Gy_30Fx.json`

 * *Files identical despite different names*

### Comparing `portpy-0.0.2/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json` & `portpy-0.0.3/config_files/optimization_params/optimization_params_Lung_2Gy_30Fx.json`

 * *Files identical despite different names*

### Comparing `portpy-0.0.2/images/PortPy_logo.jpg` & `portpy-0.0.3/images/PortPy_logo.jpg`

 * *Files identical despite different names*

### Comparing `portpy-0.0.2/portpy/photon/beam.py` & `portpy-0.0.3/portpy/photon/beam.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.2/portpy/photon/clinical_criteria.py` & `portpy-0.0.3/portpy/photon/clinical_criteria.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from typing import List
 from .data_explorer import DataExplorer
 
+
 class ClinicalCriteria:
     """
     A class representing clinical criteria.
 
     - **Attributes** ::
 
         :param clinical_criteria_dict: dictionary containing metadata about clinical criteria
```

### Comparing `portpy-0.0.2/portpy/photon/ct.py` & `portpy-0.0.3/portpy/photon/ct.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from .data_explorer import DataExplorer
 from typing import List
 
 
 class CT:
     """
     Class representing CT for the patient
+
+    - **Attributes** ::
+
+        :param ct_dict: dictionary containing ct metadata and data
+        :type patient_id: patient id of the patient
+
+
     """
 
     def __init__(self, data: DataExplorer):
         metadata = data.load_metadata()
         ct_dict = data.load_data(meta_data=metadata['ct'])
         self.ct_dict = ct_dict
         self.patient_id = data.patient_id
```

### Comparing `portpy-0.0.2/portpy/photon/cvxpy_prob.py` & `portpy-0.0.3/portpy/photon/optimization.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,100 +1,155 @@
 from __future__ import annotations
 import numpy as np
 import cvxpy as cp
-from typing import List, TYPE_CHECKING
+from typing import List, TYPE_CHECKING, Union
 
 if TYPE_CHECKING:
     from portpy.photon.plan import Plan
     from portpy.photon.influence_matrix import InfluenceMatrix
+from .clinical_criteria import ClinicalCriteria
 
 
-class CvxPyProb(object):
+class Optimization(object):
     """
-    Optimization class for creating cvxpy problem object
+    Optimization class for optimizing and creating the plan
+
+    :param my_plan: object of class Plan
+    :param inf_matrix: object of class InfluenceMatrix
+    :param clinical_criteria: clinical criteria for which plan to be optimized
+    :param opt_params: optimization parameters for modifying parameters of problem statement
+
+    - **Attributes** ::
+
+        :param obj: List containing individual objective function
+        :param constraints: List containing individual constraints
+        :param vars: Dictionary containing variable
+        :Example
+                dict = {"x": [...]}
+
+    - **Methods** ::
+        :create_cvxpy_problem(my_plan)
+            Create cvxpy objective function and constraints and save them as a list
+
     """
 
-    def __init__(self, my_plan: Plan, inf_matrix: InfluenceMatrix = None, max_constraints: List[dict] = None,
-                 mean_constraints: List[dict] = None, **opt_params):
+    def __init__(self, my_plan: Plan, inf_matrix: InfluenceMatrix = None,
+                 clinical_criteria: ClinicalCriteria = None,
+                 opt_params: dict = None):
+        # self.x = None
+        self.my_plan = my_plan
+        if inf_matrix is None:
+            inf_matrix = my_plan.inf_matrix
+        self.inf_matrix = inf_matrix
+        if clinical_criteria is None:
+            clinical_criteria = my_plan.clinical_criteria
+        self.clinical_criteria = clinical_criteria
+        self.opt_params = opt_params
+        self.prescription_gy = opt_params['prescription_gy']
+        self.obj = []
+        self.constraints = []
+        self.vars = {}
+
+    def create_cvxpy_problem(self):
         """
         It runs optimization to create optimal plan based upon clinical criteria
 
-        :param my_plan: object of class Plan
-        :param inf_matrix: object of class InfluenceMatrix
-        :param solver: default solver 'MOSEK'. check cvxpy website for available solvers
-        :param verbose: Default to True. If set to False, it will not print the solver iterations.
-        :param cvxpy_options: cvxpy and the solver settings
-        :param opt_params: optimization parameters for modifying parameters of problem statement
         :return: cvxpy problem object
 
         """
 
-        # get data for optimization
-        if max_constraints is None:
-            max_constraints = my_plan.clinical_criteria.get_criteria(
-                name='max_dose')  # returns all the max dose criteria as a list
-        if mean_constraints is None:
-            mean_constraints = my_plan.clinical_criteria.get_criteria(
-                name='mean_dose')  # returns all the mean dose criteria as a list
-
-        if inf_matrix is None:
-            inf_matrix = my_plan.inf_matrix
+        # unpack data
+        my_plan = self.my_plan
+        inf_matrix = self.inf_matrix
+        opt_params = self.opt_params
+        clinical_criteria = self.clinical_criteria
+        # self.prescription_gy = opt_params['prescription_gy']
+
+        # get opt params for optimization
+        obj_funcs = opt_params['objective_functions'] if 'objective_functions' in opt_params else []
+        opt_params_constraints = opt_params['constraints'] if 'constraints' in opt_params else []
+
+        # Creating rinds (aka rings, shells)
+        # Rinds are doughnut-shaped structures often created to control the radiation dose to non-specified structures
+        #   They can also control the dose fall-off after PTV.
 
         A = inf_matrix.A
-        num_fractions = my_plan.get_num_of_fractions()
+        num_fractions = clinical_criteria.get_num_of_fractions()
         st = inf_matrix
-        self.my_plan = my_plan
-        self.inf_matrix = inf_matrix
-
-        # Opt params
-        ptv_overdose_weight = opt_params['ptv_overdose_weight'] if 'ptv_overdose_weight' in opt_params else 10000
-        ptv_underdose_weight = opt_params['ptv_underdose_weight'] if 'ptv_underdose_weight' in opt_params else 100000
-        smoothness_weight = opt_params['smoothness_weight'] if 'smoothness_weight' in opt_params else 10
-        total_oar_weight = opt_params['total_oar_weight'] if 'total_oar_weight' in opt_params else 10
-        all_vox = np.arange(A.shape[0])
-        oar_voxels = all_vox[~np.isin(np.arange(A.shape[0]), st.get_opt_voxels_idx('PTV'))]
-        oar_weights = np.ones(A[oar_voxels, :].shape[0])
-        pres_per_frac = my_plan.get_prescription() / my_plan.get_num_of_fractions()
-        [Qx, Qy, num_rows, num_cols] = self.get_smoothness_matrix(inf_matrix.beamlets_dict)
-        smoothness_X_weight = 0.6
-        smoothness_Y_weight = 0.4
 
         # Construct optimization problem
         obj = []
         constraints = []
-
-        # Construct the problem.
-
         x = cp.Variable(A.shape[1], pos=True, name='x')
-        self.x = x
-        dO = cp.Variable(len(st.get_opt_voxels_idx('PTV')), pos=True)
-        dU = cp.Variable(len(st.get_opt_voxels_idx('PTV')), pos=True)
 
+        self.vars = {'x': x}
+
+        # Generating objective functions
         print('Objective Start')
-        # Add target objective
-        obj += [(1 / len(st.get_opt_voxels_idx('PTV'))) * (
-                ptv_overdose_weight * cp.sum_squares(dO) + ptv_underdose_weight * cp.sum_squares(dU))]
-        # Add smoothness objective
-        obj += [smoothness_weight * (smoothness_X_weight * (1 / num_cols) * cp.sum_squares(Qx @ x) +
-                                     smoothness_Y_weight * (1 / num_rows) * cp.sum_squares(Qy @ x))]
-        # Add quadratic oar objective
-        obj += [total_oar_weight * (1 / A[oar_voxels, :].shape[0]) * cp.sum_squares(
-            cp.multiply(cp.sqrt(oar_weights), A[oar_voxels, :] @ x))]
+        for i in range(len(obj_funcs)):
+            if obj_funcs[i]['type'] == 'quadratic-overdose':
+                if obj_funcs[i]['structure_name'] in my_plan.structures.get_structures():
+                    struct = obj_funcs[i]['structure_name']
+                    dose_gy = self.get_num(obj_funcs[i]['dose_gy']) / clinical_criteria.get_num_of_fractions()
+                    dO = cp.Variable(len(st.get_opt_voxels_idx(struct)), pos=True)
+                    obj += [(1 / len(st.get_opt_voxels_idx(struct))) *
+                            (obj_funcs[i]['weight'] * cp.sum_squares(dO))]
+                    constraints += [A[st.get_opt_voxels_idx(struct), :] @ x <= dose_gy + dO]
+            elif obj_funcs[i]['type'] == 'quadratic-underdose':
+                if obj_funcs[i]['structure_name'] in my_plan.structures.get_structures():
+                    struct = obj_funcs[i]['structure_name']
+                    dose_gy = self.get_num(obj_funcs[i]['dose_gy']) / clinical_criteria.get_num_of_fractions()
+                    dU = cp.Variable(len(st.get_opt_voxels_idx(struct)), pos=True)
+                    obj += [(1 / len(st.get_opt_voxels_idx(struct))) *
+                            (obj_funcs[i]['weight'] * cp.sum_squares(dU))]
+                    constraints += [A[st.get_opt_voxels_idx(struct), :] @ x >= dose_gy - dU]
+            elif obj_funcs[i]['type'] == 'quadratic':
+                if obj_funcs[i]['structure_name'] in my_plan.structures.get_structures():
+                    struct = obj_funcs[i]['structure_name']
+                    obj += [(1 / len(st.get_opt_voxels_idx(struct))) * (
+                            obj_funcs[i]['weight'] * cp.sum_squares(A[st.get_opt_voxels_idx(struct), :] @ x))]
+            elif obj_funcs[i]['type'] == 'quadratic-smoothness':
+                [Qx, Qy, num_rows, num_cols] = self.get_smoothness_matrix(inf_matrix.beamlets_dict)
+                smoothness_X_weight = 0.6
+                smoothness_Y_weight = 0.4
+                obj += [obj_funcs[i]['weight'] * (smoothness_X_weight * (1 / num_cols) * cp.sum_squares(Qx @ x) +
+                                                  smoothness_Y_weight * (1 / num_rows) * cp.sum_squares(Qy @ x))]
 
         print('Objective done')
 
         print('Constraints Start')
 
+        # add optimization constraints if present in opt params
+        for param in opt_params_constraints:
+            # add constraint
+            if param['structure_name'] in my_plan.structures.get_structures():
+                parameters = {'structure_name': param['structure_name']}
+                # total_pres = self.get_prescription()
+                if 'max' in param['type']:
+                    opt_constraints = {'limit_dose_gy': self.get_num(param['upper_limit'])}
+                    clinical_criteria.add_criterion(criterion='max_dose', parameters=parameters,
+                                                    constraints=opt_constraints)
+                if 'mean' in param['type']:
+                    opt_constraints = {'limit_dose_gy': self.get_num(param['upper_limit'])}
+                    clinical_criteria.add_criterion(criterion='mean_dose', parameters=parameters,
+                                                    constraints=opt_constraints)
+
+        # get max and mean constraints
+        max_constraints = clinical_criteria.get_criteria(
+            name='max_dose')  # returns all the max dose criteria as a list
+        mean_constraints = clinical_criteria.get_criteria(
+            name='mean_dose')  # returns all the mean dose criteria as a list
+
         # Adding max constraints
         for i in range(len(max_constraints)):
             if 'max_dose' in max_constraints[i]['name']:
                 if 'limit_dose_gy' in max_constraints[i]['constraints']:
                     limit = max_constraints[i]['constraints']['limit_dose_gy']
                     org = max_constraints[i]['parameters']['structure_name']
-                    if org != 'GTV' or org != 'CTV':
+                    if org != 'GTV' and org != 'CTV':
                         if org in my_plan.structures.structures_dict['name']:
                             constraints += [A[st.get_opt_voxels_idx(org), :] @ x <= limit / num_fractions]
                         else:
                             print('Structure {} not available!'.format(org))
 
         # Adding mean constraints
         for i in range(len(mean_constraints)):
@@ -107,106 +162,103 @@
                         constraints += [(1 / sum(st.get_opt_voxels_volume_cc(org))) *
                                         (cp.sum((cp.multiply(st.get_opt_voxels_volume_cc(org), A[st.get_opt_voxels_idx(org),
                                                                                           :] @ x)))) <= limit / num_fractions]
 
                     else:
                         print('Structure {} not available!'.format(org))
 
-        # Step 1 and 2 constraints
-        constraints += [A[st.get_opt_voxels_idx('PTV'), :] @ x <= pres_per_frac + dO]
-        constraints += [A[st.get_opt_voxels_idx('PTV'), :] @ x >= pres_per_frac - dU]
         self.obj = obj
         self.constraints = constraints
 
         print('Constraints done')
 
     def add_max(self, struct: str, dose_gy: float):
         """
         Add max constraints to the problem
 
-        :param struct: structure name
+        :param struct: struct_name name
         :param dose_gy: dose in Gy per fraction.
         :return:
         """
         A = self.inf_matrix.A
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         max_constraint = [A[st.get_opt_voxels_idx(struct), :] @ x <= dose_gy]
         self.add_constraints(max_constraint)
 
     def add_mean(self, struct: str, dose_gy: float):
         """
         Add mean constraints to the problem
 
-        :param struct: structure name
+        :param struct: struct_name name
         :param dose_gy: dose in Gy per fraction.
         :return:
         """
         A = self.inf_matrix.A
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         mean_constraint = [(1 / sum(st.get_opt_voxels_volume_cc(struct))) *
                            (cp.sum((cp.multiply(st.get_opt_voxels_volume_cc(struct),
                                                 A[st.get_opt_voxels_idx(struct),
                                                 :] @ x)))) <= dose_gy]
         self.add_constraints(mean_constraint)
 
     def add_overdose_quad(self, struct: str, dose_gy: float, weight: float = 10000):
         """
-        Add quadratic loss for the overdose voxels of the structure
+        Add quadratic loss for the overdose voxels of the struct_name
 
-        :param struct: structure name
+        :param struct: struct_name name
         :param dose_gy: dose in Gy per fraction.
         :param weight: penalty/weight in the objective for overdose
         :return:
         """
         A = self.inf_matrix.A
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         dO = cp.Variable(len(st.get_opt_voxels_idx(struct)), pos=True, name='{}_overdose'.format(struct))
         obj = (1 / len(st.get_opt_voxels_idx(struct))) * (weight * cp.sum_squares(dO))
         self.add_objective(obj)
         self.add_constraints([A[st.get_opt_voxels_idx('PTV'), :] @ x <= dose_gy + dO])
 
     def add_underdose_quad(self, struct: str, dose_gy: float, weight: float = 100000):
         """
-        Add quadratic loss for the underdose voxels of the structure
+        Add quadratic loss for the underdose voxels of the struct_name
 
-        :param struct: structure name
+        :param struct: struct_name name
         :param dose_gy: dose in Gy per fraction.
         :param weight: penalty/weight in the objective for underdose
         :return:
         """
         A = self.inf_matrix.A
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         dU = cp.Variable(len(st.get_opt_voxels_idx(struct)), pos=True, name='{}_underdose'.format(struct))
         obj = (1 / len(st.get_opt_voxels_idx(struct))) * (weight * cp.sum_squares(dU))
         self.add_objective(obj)
         self.add_constraints([A[st.get_opt_voxels_idx('PTV'), :] @ x >= dose_gy - dU])
 
     def add_quad(self, struct: str = None, voxels: np.ndarray = None, weight: float = 10,
                  voxels_weight: np.ndarray = None):
 
         """
         Add quadratic objective to the optimization problem
 
-        :param struct: structure for which quadratic loss is added to objective function
+        :param struct: struct_name for which quadratic loss is added to objective function
         :param voxels: Default to None. If set, quadratic loss will be added for the given voxels
-        :param weight: Default to 10. penalty in the objective function for the given structure.
+        :param weight: Default to 10. penalty in the objective function for the given struct_name.
         :param voxels_weight: weight for each voxel in the objective function
         :return:
         """
         A = self.inf_matrix.A
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         obj = 0
         if voxels is not None:
             if voxels_weight is None:
                 raise Exception('Please input weight array for the input voxels')
             obj = (1 / A[voxels, :].shape[0]) * cp.sum_squares(
                 cp.multiply(cp.sqrt(voxels_weight), A[voxels, :] @ x))
@@ -222,15 +274,15 @@
         :param weight: smoothness weight
         :param smoothness_X_weight: weight in X direction of MLC (parallel to MLC)
         :param smoothness_Y_weight: weight in Y direction of MLC (perpendicular to MLC)
         :return:
         """
 
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         [Qx, Qy, num_rows, num_cols] = self.get_smoothness_matrix(st.beamlets_dict)
         obj = weight * (
                 smoothness_X_weight * (1 / num_cols) * cp.sum_squares(Qx @ x) + smoothness_Y_weight * (1 / num_rows)
                 * cp.sum_squares(Qy @ x))
         self.add_objective(obj)
 
@@ -259,86 +311,98 @@
         """
         Select optimal beams from set of beams using MIP
 
         :param num_beams: number of beams to be selected
         :return:
         """
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         #  Constraints for selecting beams
         # binary variable for selecting beams
         b = cp.Variable(len(st.beamlets_dict), boolean=True)
 
         constraints = []
         constraints += [cp.sum(b) <= num_beams]
         for i in range(len(st.beamlets_dict)):
-            start_beamlet = st.beamlets_dict[i]['start_beamlet']
-            end_beamlet = st.beamlets_dict[i]['end_beamlet']
+            start_beamlet = st.beamlets_dict[i]['start_beamlet_idx']
+            end_beamlet_idx = st.beamlets_dict[i]['end_beamlet_idx']
             M = 50  # upper bound on the beamlet intensity
-            constraints += [x[start_beamlet:end_beamlet] <= b[i] * M]
+            constraints += [x[start_beamlet:end_beamlet_idx] <= b[i] * M]
 
         self.add_constraints(constraints)
 
-    def solve(self, *args, **kwargs):
+    def solve(self, *args, **kwargs) -> dict:
+        """
+                Return optimal solution and influence matrix associated with it in the form of dictionary
+
+                :Example
+                        dict = {"optimal_fluence": [..],
+                        "inf_matrix": my_plan.inf_marix
+                        }
+
+                :return: solution dictionary
+                """
+
         problem = cp.Problem(cp.Minimize(sum(self.obj)), constraints=self.constraints)
         problem.solve(*args, **kwargs)
+        return {'optimal_intensity': self.vars['x'].value, 'inf_matrix': self.inf_matrix}
 
     def get_sol(self) -> dict:
         """
         Return optimal solution and influence matrix associated with it in the form of dictionary
 
         :Example
                 dict = {"optimal_fluence": [..],
                 "inf_matrix": my_plan.inf_marix
                 }
 
         :return: solution dictionary
         """
-        return {'optimal_intensity': self.x.value, 'inf_matrix': self.inf_matrix}
+        return {'optimal_intensity': self.vars['x'].value, 'inf_matrix': self.inf_matrix}
 
     def add_dvh(self, dvh_constraint: list):
 
         A = self.inf_matrix.A
         st = self.inf_matrix
-        x = self.x
+        x = self.vars['x']
 
         import pandas as pd
         df_dvh_criteria = pd.DataFrame()
         count = 0
-        criteria = self.my_plan.clinical_criteria.clinical_criteria_dict['criteria']
+        criteria = self.clinical_criteria.clinical_criteria_dict['criteria']
         for i in range(len(dvh_constraint)):
             if 'dose_volume' in dvh_constraint[i]['name']:
                 limit_key = self.matching_keys(dvh_constraint[i]['constraints'], 'limit')
                 if limit_key in dvh_constraint[i]['constraints']:
-                    df_dvh_criteria.at[count, 'structure'] = dvh_constraint[i]['parameters']['structure_name']
+                    df_dvh_criteria.at[count, 'structure_name'] = dvh_constraint[i]['parameters']['structure_name']
                     df_dvh_criteria.at[count, 'dose_gy'] = dvh_constraint[i]['parameters']['dose_gy']
 
-                    # getting max dose_1d for the same structure
+                    # getting max dose_1d for the same struct_name
                     max_dose_struct = 1000
                     for j in range(len(criteria)):
                         if 'max_dose' in criteria[j]['name']:
                             if 'limit_dose_gy' in criteria[j]['constraints']:
                                 org = criteria[j]['parameters']['structure_name']
                                 if org == dvh_constraint[i]['parameters']['structure_name']:
                                     max_dose_struct = criteria[j]['constraints']['limit_dose_gy']
                     df_dvh_criteria.at[count, 'M'] = max_dose_struct - dvh_constraint[i]['parameters']['dose_gy']
                     if 'perc' in limit_key:
                         df_dvh_criteria.at[count, 'vol_perc'] = dvh_constraint[i]['constraints'][limit_key]
                     count = count + 1
 
         # binary variable for dvh constraints
         b_dvh = cp.Variable(
-            len(np.concatenate([st.get_opt_voxels_idx(org) for org in df_dvh_criteria.structure.to_list()])),
+            len(np.concatenate([st.get_opt_voxels_idx(org) for org in df_dvh_criteria.structure_name.to_list()])),
             boolean=True)
 
         start = 0
         constraints = []
         for i in range(len(df_dvh_criteria)):
-            struct, limit, v, M = df_dvh_criteria.loc[i, 'structure'], df_dvh_criteria.loc[i, 'dose_gy'], \
+            struct, limit, v, M = df_dvh_criteria.loc[i, 'structure_name'], df_dvh_criteria.loc[i, 'dose_gy'], \
                                   df_dvh_criteria.loc[i, 'vol_perc'], df_dvh_criteria.loc[i, 'M']
             end = start + len(st.get_opt_voxels_idx(struct))
             frac = self.my_plan.structures.get_fraction_of_vol_in_calc_box(struct)
             constraints += [
                 A[st.get_opt_voxels_idx(struct), :] @ x <= limit / self.my_plan.get_num_of_fractions()
                 + b_dvh[start:end] * M / self.my_plan.get_num_of_fractions()]
             constraints += [b_dvh @ st.get_opt_voxels_volume_cc(struct) <= (v / frac) / 100 * sum(
@@ -358,20 +422,20 @@
 
         :Example:
         Qx = [[1 -1 0 0 0 0]
               [0 0 1 -1 0 0]
               [0 0 0 0 1 -1]]
 
         """
-        sRow = np.zeros((beamReq[-1]['end_beamlet'] + 1, beamReq[-1]['end_beamlet'] + 1), dtype=int)
-        sCol = np.zeros((beamReq[-1]['end_beamlet'] + 1, beamReq[-1]['end_beamlet'] + 1), dtype=int)
+        sRow = np.zeros((beamReq[-1]['end_beamlet_idx'] + 1, beamReq[-1]['end_beamlet_idx'] + 1), dtype=int)
+        sCol = np.zeros((beamReq[-1]['end_beamlet_idx'] + 1, beamReq[-1]['end_beamlet_idx'] + 1), dtype=int)
         num_rows = 0
         num_cols = 0
         for b in range(len(beamReq)):
-            beam_map = beamReq[b]['beamlet_idx_2dgrid']
+            beam_map = beamReq[b]['beamlet_idx_2d_finest_grid']
 
             rowsNoRepeat = [0]
             for i in range(1, np.size(beam_map, 0)):
                 if (beam_map[i, :] != beam_map[rowsNoRepeat[-1], :]).any():
                     rowsNoRepeat.append(i)
             colsNoRepeat = [0]
             for j in range(1, np.size(beam_map, 1)):
@@ -416,7 +480,14 @@
         for key, val in dictionary.items():
             if search_string in key:
                 get_key = key
         if get_key is not None:
             return get_key
         else:
             return ''
+
+    def get_num(self, string: Union[str, float]):
+        if "prescription_gy" in string:
+            prescription_gy = self.prescription_gy
+            return eval(string)
+        elif isinstance(string, float) or isinstance(string, int):
+            return string
```

### Comparing `portpy-0.0.2/portpy/photon/data_explorer.py` & `portpy-0.0.3/portpy/photon/data_explorer.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,42 +7,37 @@
 from pathlib import Path
 import pandas as pd
 from tabulate import tabulate
 import webbrowser
 
 
 class DataExplorer:
+    """
+    A class for exploring the benchmark data available in PortPy
+
+    - **Attributes** ::
+
+        :param data_dir: local directory containing data
+        :param patient_id: patient id of the patient
+
+    - **Methods** ::
+        :display_patient_metadata()
+            display metadata for the patient
+        :display_list_of_patients()
+            display the patient list in portpy database
+
+
+    """
     def __init__(self, data_dir: str = None, patient_id: str = None):
         if data_dir is None:
             data_dir = os.path.join('..', 'data')
         self.data_dir = data_dir
         if patient_id is not None:
             self.patient_id = patient_id
 
-    @staticmethod
-    def list_to_dict(json_data):
-        """
-        A recursive function which constructs dictionary from list
-        :param json_data: data in json or list format
-        :return: data in dictionary format
-        """
-
-        json_dict = {}
-        if type(json_data) is list:
-            for i in range(len(json_data)):
-                elem = json_data[i]
-                if type(elem) is list:
-                    json_dict[i] = DataExplorer.list_to_dict(elem)
-                else:
-                    for key in elem:
-                        json_dict.setdefault(key, []).append(elem[key])
-        else:
-            json_dict = json_data.copy()
-        return json_dict
-
     def load_metadata(self, pat_dir: str = None) -> dict:
         """Loads metadata of a patient located in path and returns the metadata as a dictionary
 
         The data are loaded from the following .Json files:
         1- StructureSet_MetaData.json
             including data about the structures (e.g., PTV, Kidney, Lung)
         2- OptimizationVoxels_MetaData.json
@@ -108,33 +103,23 @@
                 meta_data['beams'].setdefault(key, []).append(json_data[key])
                 # dataMeta['beamsMetaData'][key].append(json_data[key])
 
         meta_data['patient_folder_path'] = pat_dir
         return meta_data
 
     @staticmethod
-    def load_config_planner_metadata(patient_id):
-        # load planner_plan config metadata
-        fname = os.path.join(Path(__file__).parents[2], 'config_files', 'planner_plan', patient_id, 'planner_plan.json')
-        # fname = os.path.join('..', 'config_files', 'planner_plan', patient_id, 'planner_plan.json')
-        # Opening JSON file
-        f = open(fname)
-        planner_metadata = json.load(f)
-        return planner_metadata
-
-    @staticmethod
     def load_config_clinical_criteria(protocol_name: str, protocol_type: str = 'Default') -> dict:
         """
         Returns json file as dictionary
         :param protocol_name: Clinical protocol name
         :param protocol_type: Default.
         :return: dictionary containing clinical criteria
         """
         # load clinical criteria config metadata
-        fname = os.path.join(Path(__file__).parents[2], 'config_files', 'clinical_criteria',
+        fname = os.path.join(Path(__file__).parents[1], 'config_files', 'clinical_criteria',
                              protocol_type, protocol_name + '.json')
         # fname = os.path.join('..', 'config_files', 'planner_plan', patient_id, 'planner_plan.json')
         # Opening JSON file
         json_data = DataExplorer.load_json(fname)
         return json_data
 
     @staticmethod
@@ -143,15 +128,15 @@
 
         Returns json file as dictionary
         :param protocol_name: Clinical protocol name
         :return: dictionary containing optimization params
 
         """
         # load opt params config metadata
-        fname = os.path.join(Path(__file__).parents[2], 'config_files', 'optimization_params',
+        fname = os.path.join(Path(__file__).parents[1], 'config_files', 'optimization_params',
                              'optimization_params_' + protocol_name + '.json')
         # fname = os.path.join('..', 'config_files', 'planner_plan', patient_id, 'planner_plan.json')
         # Opening JSON file
         json_data = DataExplorer.load_json(fname)
         return json_data
 
     @staticmethod
@@ -436,7 +421,28 @@
                     return True
                 else:
                     return False  # Other type (?)
         except NameError:
             return False  # Probably standard Python interpreter
         except:
             return False  # Probably standard Python interpreter
+
+    @staticmethod
+    def list_to_dict(json_data):
+        """
+        A recursive function which constructs dictionary from list
+        :param json_data: data in json or list format
+        :return: data in dictionary format
+        """
+
+        json_dict = {}
+        if type(json_data) is list:
+            for i in range(len(json_data)):
+                elem = json_data[i]
+                if type(elem) is list:
+                    json_dict[i] = DataExplorer.list_to_dict(elem)
+                else:
+                    for key in elem:
+                        json_dict.setdefault(key, []).append(elem[key])
+        else:
+            json_dict = json_data.copy()
+        return json_dict
```

### Comparing `portpy-0.0.2/portpy/photon/evaluation.py` & `portpy-0.0.3/portpy/photon/evaluation.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,27 @@
 
 from .plan import Plan
 from .clinical_criteria import ClinicalCriteria
 from tabulate import tabulate
 
 
 class Evaluation:
+    """
+    Class for evaluating different metrics for the plan
+
+    - **Methods** ::
+        :display_clinical_criteria(my_plan, sol)
+            display plan values corresponding to given clinical criteria
+        :get_dose(sol, struct, volume_per)
+            get dose at the given volume in percentage
+        :get_volume(sol: struct dose_value_gy)
+            Get volume at dose_1d value in Gy
+
+
+    """
 
     @staticmethod
     def get_dose(sol: dict, struct: str, volume_per: float, dose_1d: np.ndarray = None,
                  weight_flag: bool = True) -> float:
         """
         Get dose_1d at volume percentage
```

### Comparing `portpy-0.0.2/portpy/photon/influence_matrix.py` & `portpy-0.0.3/portpy/photon/influence_matrix.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,22 +16,20 @@
     """
     class of influence matrix
 
     - **Attributes** ::
 
         :param beamlet_width_mm: The width of each beamlet in millimeters. Default is 2.5. Must be a multiple of 2.5.
         :param beamlet_height_mm: The height of each beamlet in millimeters. Default is 2.5. Must be a multiple of 2.5.
-        :param _down_sample_xyz: A list of integers representing the downsampling factors for the x, y, and z axes. When set to None, the original optimization voxel resolution will be used.
-        :param structure: The target struct_name for creating the beamlets in the influence matrix. Default is 'PTV'.
-        :param opt_voxels_dict: A dictionary containing the voxels that were used in the optimization process.
+        :param opt_vox_xyz_res_mm: A list of integers representing the resolution for optimization voxels in the x, y, and z axes. When set to None, the original optimization voxel resolution will be used.
+        :param target_structure: The target struct_name for creating the beamlets in the influence matrix. Default is 'PTV'.
         :param beamlets_dict: A dictionary containing the information about beamlets used in the plan.
         :param opt_beamlets_PTV_margin_mm: A float value representing the margin_mm around the PTV that was used in creating beamlets
         :param A: influence matrix that is generated by the get_influence_matrix() method.
-        :param dose_3d: 3D dose_1d distribution. It is saved as attribute once the method dose_1d_to_3d() is called
-                so that it doesnt have to be computed again
+        :param opt_voxels_dict: A dictionary containing the information about optimization voxels
 
     - **Methods** ::
         :dose_1d_to_3d(sol)
             Convert dose_1d from 1d to 3d and return dose_1d in 3d
         :dose_3d_to_1d(dose_3d)
             Convert dose_1d from 3d to 1d voxels and return dose_1d in 1d
         :fluence_2d_to_1d(fluence_2d)
@@ -895,100 +893,7 @@
         vox_weights = self.opt_voxels_dict['voxel_volume_cc'][ind]
         # vox_ind = np.where(my_plan.opt_voxels_dict['voxel_structure_map'][0][:, ind] == 1)[0]
         return vox_weights
 
     def get_all_beam_ids(self) -> List[int]:
         ids = [self.beamlets_dict[i]['beam_id'] for i in range(len(self.beamlets_dict))]
         return ids
-
-    def plot_fluence_2d(self, beam_id: int, optimal_fluence_2d: List[np.ndarray] = None, sol: dict = None,
-                        **options) -> None:
-        """
-
-                Displays fluence in 2d for the given beam_id
-
-                :param optimal_fluence_2d:
-                :param beam_id: beam_id of the beam
-                :param sol: solution dictionary after optimization
-                :return: 2d optimal fluence plot
-
-                :Example:
-                >>> Visualization.plot_fluence_2d(beam_id=0, sol=sol)
-                """
-        # getting options_fig:
-        figsize = options['figsize'] if 'figsize' in options else (8, 8)
-        title = options['title'] if 'title' in options else None
-        filename = options['filename'] if 'filename' in options else None
-        show = options['show'] if 'show' in options else False
-        ax = options['ax'] if 'ax' in options else None
-
-        ind = [i for i in range(len(self.beamlets_dict)) if self.beamlets_dict[i]['beam_id'] == beam_id]
-        if len(ind) == 0:
-            raise IndexError('invalid beam id {}'.format(beam_id))
-        if sol is not None:
-            optimal_fluence_2d = self.fluence_1d_to_2d(sol=sol)
-        if ax is None:
-            fig, ax = plt.subplots(figsize=figsize)
-
-        mat = ax.matshow(optimal_fluence_2d[ind[0]])
-        ax.set_xlabel('x-axis (beamlets column)')
-        ax.set_ylabel('y-axis (beamlets row)')
-        plt.colorbar(mat, ax=ax)
-        if title is not None:
-            ax.set_title('{}'.format(title))
-        if filename is not None:
-            plt.savefig(filename, bbox_inches="tight", dpi=300)
-        if show:
-            plt.show()
-        return ax
-
-    def plot_fluence_3d(self, beam_id: int, optimal_fluence_2d: List[np.ndarray] = None, sol: dict = None,
-                        **options) -> None:
-        """
-                Displays fluence in 3d for the given beam_id
-
-                :param optimal_fluence_2d:
-                :param sol: solution after optimization
-                :param beam_id: beam_id of the beam
-                :return: 3d optimal fluence plot
-
-                :Example:
-                >>> Visualization.plot_fluence_3d(beam_id=0, sol=sol)
-                """
-
-        # getting options_fig:
-        figsize = options['figsize'] if 'figsize' in options else (8, 8)
-        title = options['title'] if 'title' in options else None
-        filename = options['filename'] if 'filename' in options else None
-        show = options['show'] if 'show' in options else False
-        ax = options['ax'] if 'ax' in options else None
-
-        ind = [i for i in range(len(self.beamlets_dict)) if self.beamlets_dict[i]['beam_id'] == beam_id]
-        if len(ind) == 0:
-            raise IndexError('invalid beam id {}'.format(beam_id))
-        if sol is not None:
-            optimal_fluence_2d = self.fluence_1d_to_2d(sol=sol)
-        (ax, surf) = InfluenceMatrix.surface_plot(optimal_fluence_2d[ind[0]], ax=ax, figsize=figsize,
-                                                  cmap='viridis', edgecolor='black')
-        plt.colorbar(surf, ax=ax, pad=0.2)
-        ax.set_zlabel('Fluence Intensity')
-        ax.set_xlabel('x-axis (beamlets column)')
-        ax.set_ylabel('y-axis (beamlets row)')
-
-        if title is not None:
-            ax.set_title('{}'.format(title))
-        if filename is not None:
-            plt.savefig(filename, bbox_inches="tight", dpi=300)
-        if show:
-            plt.show()
-        return ax
-
-    @staticmethod
-    def surface_plot(matrix, ax=None, figsize=(8, 8), **kwargs):
-        # acquire the cartesian coordinate matrices from the matrix
-        # x is cols, y is rows
-        (x, y) = np.meshgrid(np.arange(matrix.shape[0]), np.arange(matrix.shape[1]))
-
-        if ax is None:
-            fig, ax = plt.subplots(figsize=figsize, subplot_kw=dict(projection='3d'))
-        surf = ax.plot_surface(x, y, np.transpose(matrix), **kwargs)
-        return ax, surf
```

### Comparing `portpy-0.0.2/portpy/photon/structures.py` & `portpy-0.0.3/portpy/photon/structures.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.2/portpy/photon/utils/get_eclipse_fluence.py` & `portpy-0.0.3/portpy/photon/utils/get_eclipse_fluence.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.2/portpy/photon/utils/save_nrrd.py` & `portpy-0.0.3/portpy/photon/utils/save_nrrd.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.2/portpy/photon/utils/save_or_load_pickle.py` & `portpy-0.0.3/portpy/photon/utils/save_or_load_pickle.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.2/portpy/photon/utils/slicer_script.py` & `portpy-0.0.3/portpy/photon/utils/slicer_script.py`

 * *Files identical despite different names*

### Comparing `portpy-0.0.2/portpy/photon/utils/view_in_slicer_jupyter.py` & `portpy-0.0.3/portpy/photon/utils/view_in_slicer_jupyter.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,19 +26,19 @@
     except ImportError:
         print('Please use slicer kernel before using this method')
 
     if show_ct:
         slicer.mrmlScene.AddNewNodeByClass("vtkMRMLScalarVolumeNode", ct_name)
         ct_node = slicer.util.getNode(ct_name)
 
-        ct_node.SetOrigin(list(np.array(my_plan.ct['origin_xyz_mm']) * np.array(
+        ct_node.SetOrigin(list(np.array(my_plan.ct.ct_dict['origin_xyz_mm']) * np.array(
             [-1, -1, 1])))  # convert to RAS origin. -ve in x and y direction
-        ct_node.SetSpacing(my_plan.ct['resolution_xyz_mm'])
+        ct_node.SetSpacing(my_plan.ct.ct_dict['resolution_xyz_mm'])
         ct_node.SetIJKToRASDirections(np.array([[-1, 0, 0], [0, -1, 0], [0, 0, 1]]))  # set itk to RAS direction
-        slicer.util.updateVolumeFromArray(ct_node, my_plan.ct['ct_hu_3d'][0])
+        slicer.util.updateVolumeFromArray(ct_node, my_plan.ct.ct_dict['ct_hu_3d'][0])
         slicer.util.setSliceViewerLayers(background=ct_node)
 
     # Another way to push simple itk image
     # import sitkUtils
     # ct = sitk.GetImageFromArray(my_plan.ct['ct_hu_3d'][0])
     # ct.SetOrigin(my_plan.ct['origin_xyz_mm'])
     # ct.SetSpacing(my_plan.ct['resolution_xyz_mm'])
@@ -49,30 +49,30 @@
         if dose_1d is not None:
             dose_arr = my_plan.inf_matrix.dose_1d_to_3d(dose_1d=dose_1d)
         else:
             dose_1d = sol['inf_matrix'].A * sol['optimal_intensity'] * my_plan.get_num_of_fractions()
             dose_arr = sol['inf_matrix'].dose_1d_to_3d(dose_1d=dose_1d)
         slicer.mrmlScene.AddNewNodeByClass("vtkMRMLScalarVolumeNode", dose_name)
         dose_node = slicer.util.getNode(dose_name)
-        dose_node.SetOrigin(list(np.array(my_plan.ct['origin_xyz_mm']) * np.array([-1, -1, 1])))
-        dose_node.SetSpacing(my_plan.ct['resolution_xyz_mm'])
+        dose_node.SetOrigin(list(np.array(my_plan.ct.ct_dict['origin_xyz_mm']) * np.array([-1, -1, 1])))
+        dose_node.SetSpacing(my_plan.ct.ct_dict['resolution_xyz_mm'])
         dose_node.SetIJKToRASDirections(np.array([[-1, 0, 0], [0, -1, 0], [0, 0, 1]]))
         slicer.util.updateVolumeFromArray(dose_node, dose_arr)
         slicer.util.setSliceViewerLayers(foreground=dose_node)
         slicer.util.setSliceViewerLayers(foregroundOpacity=0.4)
         # dose_node.GetVolumeDisplayNode.
 
     # plot structures
     if show_structs:
         structure_node = slicer.mrmlScene.AddNewNodeByClass("vtkMRMLSegmentationNode", struct_set_name)
         for i, struct_name in enumerate(my_plan.structures.structures_dict['name']):
             print('Importing struct_name : ' + struct_name)
             slicer.util.addVolumeFromArray(my_plan.structures.structures_dict['structure_mask_3d'][i] * (i + 1),
                                            name=struct_name, nodeClassName="vtkMRMLLabelMapVolumeNode")
             lmap = slicer.util.getNode(struct_name)
-            lmap.SetOrigin(list(np.array(my_plan.ct['origin_xyz_mm']) * np.array([-1, -1, 1])))
-            lmap.SetSpacing(my_plan.ct['resolution_xyz_mm'])
+            lmap.SetOrigin(list(np.array(my_plan.ct.ct_dict['origin_xyz_mm']) * np.array([-1, -1, 1])))
+            lmap.SetSpacing(my_plan.ct.ct_dict['resolution_xyz_mm'])
             lmap.SetIJKToRASDirections(np.array([[-1, 0, 0], [0, -1, 0], [0, 0, 1]]))
             slicer.modules.segmentations.logic().ImportLabelmapToSegmentationNode(lmap, structure_node)
             slicer.mrmlScene.RemoveNode(lmap)
             segId = structure_node.GetSegmentation().GetNthSegment(i)
             segId.SetName(struct_name)
```

### Comparing `portpy-0.0.2/portpy/photon/visualization.py` & `portpy-0.0.3/portpy/photon/visualization.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from pathlib import Path
 from typing import List, TYPE_CHECKING
 from .ct import CT
 from .structures import Structures
 
 if TYPE_CHECKING:
     from portpy.photon.plan import Plan
+    from portpy.photon.influence_matrix import InfluenceMatrix
 try:
     from typing import Literal
 except ImportError:
     from typing_extensions import Literal
 
 
 class Visualization:
@@ -196,41 +197,103 @@
         (x, y) = np.meshgrid(np.arange(matrix.shape[0]), np.arange(matrix.shape[1]))
         fig = plt.figure()
         ax = fig.add_subplot(111, projection='3d')
         surf = ax.plot_surface(x, y, np.transpose(matrix), **kwargs)
         return ax, surf
 
     @staticmethod
-    def plot_fluence_2d(beam_id: int, sol: dict, **options):
+    def plot_fluence_2d(beam_id: int, sol: dict = None, optimal_fluence_2d: List[np.ndarray] = None,
+                        inf_matrix: InfluenceMatrix = None, **options):
         """
 
         Displays fluence in 2d for the given beam_id
 
         :param beam_id: beam_id of the beam
         :param sol: solution dictionary after optimization
+        :param optimal_fluence_2d: List of optimal fluence for all the beams
+        :param inf_matrix: Optional. Object of class influence matrix
         :return: 2d optimal fluence plot
 
         :Example:
         >>> Visualization.plot_fluence_2d(beam_id=0, sol=sol, **options)
         """
-        return sol['inf_matrix'].plot_fluence_2d(beam_id=beam_id, sol=sol, **options)
+
+        if inf_matrix is None:
+            inf_matrix = sol['inf_matrix']
+
+        # getting options_fig:
+        figsize = options['figsize'] if 'figsize' in options else (8, 8)
+        title = options['title'] if 'title' in options else None
+        filename = options['filename'] if 'filename' in options else None
+        show = options['show'] if 'show' in options else False
+        ax = options['ax'] if 'ax' in options else None
+
+        ind = [i for i in range(len(inf_matrix.beamlets_dict)) if inf_matrix.beamlets_dict[i]['beam_id'] == beam_id]
+        if len(ind) == 0:
+            raise IndexError('invalid beam id {}'.format(beam_id))
+        if sol is not None:
+            optimal_fluence_2d = inf_matrix.fluence_1d_to_2d(sol=sol)
+        if ax is None:
+            fig, ax = plt.subplots(figsize=figsize)
+
+        mat = ax.matshow(optimal_fluence_2d[ind[0]])
+        ax.set_xlabel('x-axis (beamlets column)')
+        ax.set_ylabel('y-axis (beamlets row)')
+        plt.colorbar(mat, ax=ax)
+        if title is not None:
+            ax.set_title('{}'.format(title))
+        if filename is not None:
+            plt.savefig(filename, bbox_inches="tight", dpi=300)
+        if show:
+            plt.show()
+        return ax
 
     @staticmethod
-    def plot_fluence_3d(beam_id: int, sol: dict, **options):
+    def plot_fluence_3d(beam_id: int, sol: dict = None, optimal_fluence_2d: List[np.ndarray] = None,
+                        inf_matrix: InfluenceMatrix = None, **options):
         """
         Displays fluence in 3d for the given beam_id
 
         :param sol: solution after optimization
         :param beam_id: beam_id of the beam
+        :param optimal_fluence_2d: List of optimal fluence for all the beams
+        :param inf_matrix: Optional. Object of class influence matrix
         :return: 3d optimal fluence plot
 
         :Example:
         >>> Visualization.plot_fluence_3d(beam_id=0, sol=sol, **options)
         """
-        return sol['inf_matrix'].plot_fluence_3d(beam_id=beam_id, sol=sol, **options)
+        if inf_matrix is None:
+            inf_matrix = sol['inf_matrix']
+        # getting options_fig:
+        figsize = options['figsize'] if 'figsize' in options else (8, 8)
+        title = options['title'] if 'title' in options else None
+        filename = options['filename'] if 'filename' in options else None
+        show = options['show'] if 'show' in options else False
+        ax = options['ax'] if 'ax' in options else None
+
+        ind = [i for i in range(len(inf_matrix.beamlets_dict)) if inf_matrix.beamlets_dict[i]['beam_id'] == beam_id]
+        if len(ind) == 0:
+            raise IndexError('invalid beam id {}'.format(beam_id))
+        if sol is not None:
+            optimal_fluence_2d = inf_matrix.fluence_1d_to_2d(sol=sol)
+        (ax, surf) = Visualization.surface_plot(optimal_fluence_2d[ind[0]], ax=ax, figsize=figsize,
+                                                  cmap='viridis', edgecolor='black')
+        plt.colorbar(surf, ax=ax, pad=0.2)
+        ax.set_zlabel('Fluence Intensity')
+        ax.set_xlabel('x-axis (beamlets column)')
+        ax.set_ylabel('y-axis (beamlets row)')
+
+        if title is not None:
+            ax.set_title('{}'.format(title))
+        if filename is not None:
+            plt.savefig(filename, bbox_inches="tight", dpi=300)
+        if show:
+            plt.show()
+        return ax
 
     @staticmethod
     def plot_2d_slice(my_plan: Plan = None, sol: dict = None, ct: CT = None, structs: Structures = None,
                       slice_num: int = 40, struct_names: List[str] = None, show_dose: bool = False,
                       show_struct: bool = True, show_isodose: bool = False,
                       **options) -> None:
         """
@@ -425,7 +488,18 @@
                     return True
                 else:
                     return False  # Other type (?)
         except NameError:
             return False  # Probably standard Python interpreter
         except:
             return False  # Probably standard Python interpreter
+
+    @staticmethod
+    def surface_plot(matrix, ax=None, figsize=(8, 8), **kwargs):
+        # acquire the cartesian coordinate matrices from the matrix
+        # x is cols, y is rows
+        (x, y) = np.meshgrid(np.arange(matrix.shape[0]), np.arange(matrix.shape[1]))
+
+        if ax is None:
+            fig, ax = plt.subplots(figsize=figsize, subplot_kw=dict(projection='3d'))
+        surf = ax.plot_surface(x, y, np.transpose(matrix), **kwargs)
+        return ax, surf
```

### Comparing `portpy-0.0.2/portpy.egg-info/PKG-INFO` & `portpy-0.0.3/portpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portpy
-Version: 0.0.2
+Version: 0.0.3
 Summary: First open-source radiation treatment planning system in Python
 Home-page: https://github.com/PortPy-Project/PortPy
 Author: Gourav Jhanwar, Mojtaba Tefagh, Vicki Taasti, Seppo Tuomaala, Saad Nadeem, Masoud Zarepisheh
 Author-email: jhanwarg@mskcc.struct, mtefagh@acm.struct, vicki.taasti@maastro.nl, tuomaals@mskcc.struct, nadeems@mskcc.struct, zarepism@mskcc.struct
 License: Apache License, Version 2.0
 Description: <p align="center">
           <img src="./images/PortPy_logo.jpg" width="50%">
@@ -26,15 +26,15 @@
         Create a directory named './data' in the current project directory and copy the downloaded file to it, e.g ./data/Lung_Phantom_Patient_1
         
         # Quick Start
         Please see below for understanding the basic functionalities of PortPy. For advance usage of PortPy, we recommend navigating through [examples](https://github.com/PortPy-Project/PortPy/tree/master/examples) folder.
         1. To understand the most important features of PortPy, we highly recommend to go through notebook [ex_1_introduction.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_1_introduction.ipynb)
         2. One of the major computational issues while optimizing the plan arise due to large size of influence matrix. We suggest you to follow [ex_2_down_sampling.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_2_downsampling.py) to understand how PortPy can assist in resolving it.
         3. You can check out [ex_3_structure_operations.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_3_structure_operations.py) to know how to perform different structure operations (e.g., boolean, margin).
-        4. For algorithm benchmarking, the global optimal solution is provided for non-convex optimization problems resulting from beam angle optimization [ex_6_boo_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_boo_benchmark.py) and incorporating DVH constraints [ex_6_dvh_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_dvh_benchmark.py) using the mixed-integer programming on down-sampled data.
+        4. For algorithm benchmarking, the global optimal solution is provided for non-convex optimization problems resulting from beam angle optimization [ex_6_boo_benchmark.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_boo_benchmark.ipynb) and incorporating DVH constraints [ex_6_dvh_benchmark.py](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_6_dvh_benchmark.py) using the mixed-integer programming on down-sampled data.
         5. In addition to basic visualization capabilities, PortPy provide advanced visualization by integration with 3D Slicer. Please look out notebook [ex_7_Slicer.ipynb](https://github.com/PortPy-Project/PortPy/blob/master/examples/ex_7_Slicer.ipynb)
         
         # Installing PortPy
         
         1. Installing using pip
           ```bash
           pip install portpy
```

### Comparing `portpy-0.0.2/setup.py` & `portpy-0.0.3/setup.py`

 * *Files identical despite different names*

