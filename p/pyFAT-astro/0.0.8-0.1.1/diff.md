# Comparing `tmp/pyFAT_astro-0.0.8.tar.gz` & `tmp/pyFAT_astro-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFAT_astro-0.0.8.tar", last modified: Wed Nov 24 13:56:36 2021, max compression
+gzip compressed data, was "pyFAT_astro-0.1.1.tar", last modified: Tue Jun 13 08:07:50 2023, max compression
```

## Comparing `pyFAT_astro-0.0.8.tar` & `pyFAT_astro-0.1.1.tar`

### file list

```diff
@@ -1,42 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-24 13:56:36.920012 pyFAT_astro-0.0.8/
--rw-r--r--   0 runner    (1001) docker     (121)    35202 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      425 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      694 2021-11-24 13:56:36.920012 pyFAT_astro-0.0.8/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (121)     9850 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-24 13:56:36.916012 pyFAT_astro-0.0.8/bin/
--rw-r--r--   0 runner    (1001) docker     (121)      115 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/bin/pyFAT
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-24 13:56:36.916012 pyFAT_astro-0.0.8/pyFAT_astro/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-24 13:56:36.920012 pyFAT_astro-0.0.8/pyFAT_astro/Installation_Check/
--rw-r--r--   0 runner    (1001) docker     (121)     5762 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Installation_Check/ModelInput.def
--rw-r--r--   0 runner    (1001) docker     (121)  2825280 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Installation_Check/NGC_2903.fits
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Installation_Check/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-24 13:56:36.920012 pyFAT_astro-0.0.8/pyFAT_astro/Support/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    26505 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Support/clean_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)      529 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Support/constants.py
--rw-r--r--   0 runner    (1001) docker     (121)    48063 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Support/development_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)      781 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Support/fat_errors.py
--rw-r--r--   0 runner    (1001) docker     (121)    34138 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Support/fits_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)   123300 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Support/modify_template.py
--rw-r--r--   0 runner    (1001) docker     (121)    57583 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Support/read_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    53500 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Support/run_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)   118590 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Support/support_functions.py
--rw-r--r--   0 runner    (1001) docker     (121)    14732 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Support/tirshaker.py
--rw-r--r--   0 runner    (1001) docker     (121)    64062 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Support/write_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-24 13:56:36.920012 pyFAT_astro-0.0.8/pyFAT_astro/Templates/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Templates/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     3021 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Templates/sofia_template.par
--rw-r--r--   0 runner    (1001) docker     (121)     2291 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/Templates/template.def
--rw-r--r--   0 runner    (1001) docker     (121)     1384 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-24 13:56:36.920012 pyFAT_astro-0.0.8/pyFAT_astro/config/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5355 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/config/defaults.py
--rw-r--r--   0 runner    (1001) docker     (121)    22206 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/pyFAT_astro/main.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-11-24 13:56:36.916012 pyFAT_astro-0.0.8/pyFAT_astro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      694 2021-11-24 13:56:36.000000 pyFAT_astro-0.0.8/pyFAT_astro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1020 2021-11-24 13:56:36.000000 pyFAT_astro-0.0.8/pyFAT_astro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-11-24 13:56:36.000000 pyFAT_astro-0.0.8/pyFAT_astro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       97 2021-11-24 13:56:36.000000 pyFAT_astro-0.0.8/pyFAT_astro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2021-11-24 13:56:36.000000 pyFAT_astro-0.0.8/pyFAT_astro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-11-24 13:56:36.920012 pyFAT_astro-0.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1480 2021-11-24 13:56:25.000000 pyFAT_astro-0.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:07:50.584690 pyFAT_astro-0.1.1/
+-rwxr-xr-x   0 runner    (1001) docker     (123)    35202 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/LICENSE
+-rwxr-xr-x   0 runner    (1001) docker     (123)      498 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-13 08:07:50.584690 pyFAT_astro-0.1.1/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9854 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:07:50.576690 pyFAT_astro-0.1.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      266 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/bin/pyFAT
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:07:50.580690 pyFAT_astro-0.1.1/pyFAT_astro/
+-rw-r--r--   0 runner    (1001) docker     (123)    11583 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/FAT_Galaxy_Loop.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13637 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/FAT_Galaxy_Loops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:07:50.584690 pyFAT_astro-0.1.1/pyFAT_astro/Installation_Check/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7143 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Installation_Check/ModelInput.def
+-rwxr-xr-x   0 runner    (1001) docker     (123)  2825280 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Installation_Check/NGC_2903.fits
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Installation_Check/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:07:50.584690 pyFAT_astro-0.1.1/pyFAT_astro/Support/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        1 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Support/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    27423 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Support/clean_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      547 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Support/constants.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    48081 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Support/development_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1101 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Support/fat_errors.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    36494 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Support/fits_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   158270 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Support/modify_template.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    60270 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Support/read_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    65325 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Support/run_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   151957 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Support/support_functions.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14783 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Support/tirshaker.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    71696 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Support/write_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:07:50.584690 pyFAT_astro-0.1.1/pyFAT_astro/Templates/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Templates/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3082 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Templates/sofia_template.par
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1106 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/Templates/template.def
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1896 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:07:50.584690 pyFAT_astro-0.1.1/pyFAT_astro/config/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1313 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/config/FAT_Input_Catalogue.txt
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/config/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6173 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/config/defaults.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    13090 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/pyFAT_astro/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:07:50.580690 pyFAT_astro-0.1.1/pyFAT_astro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      639 2023-06-13 08:07:50.000000 pyFAT_astro-0.1.1/pyFAT_astro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1126 2023-06-13 08:07:50.000000 pyFAT_astro-0.1.1/pyFAT_astro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 08:07:50.000000 pyFAT_astro-0.1.1/pyFAT_astro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-06-13 08:07:50.000000 pyFAT_astro-0.1.1/pyFAT_astro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 08:07:50.000000 pyFAT_astro-0.1.1/pyFAT_astro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 08:07:50.584690 pyFAT_astro-0.1.1/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1501 2023-06-13 08:07:35.000000 pyFAT_astro-0.1.1/setup.py
```

### Comparing `pyFAT_astro-0.0.8/LICENSE` & `pyFAT_astro-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyFAT_astro-0.0.8/PKG-INFO` & `pyFAT_astro-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: pyFAT_astro
-Version: 0.0.8
+Version: 0.1.1
 Summary: Development Status :: 4 - Beta
 Home-page: https://github.com/PeterKamphuis/pyFAT
 Author: P. Kamphuis
 Author-email: peterkamphuisastronomy@gmail.com
 License: GNU GPL v3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-Not sure what is going wrong here.
-
```

### Comparing `pyFAT_astro-0.0.8/README.md` & `pyFAT_astro-0.1.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -37,21 +37,24 @@
 
   	pip install pyFAT-astro
 
 This should also install all required python dependencies.
 We recommend the use of python virtual environments. If so desired a pyFAT installation would look like:
 
   	python3 -m venv FAT_venv
+
   	source FAT_venv/bin/activate.csh
-  	pip install pyFAT-astro
+
+    pip install pyFAT-astro
 
 (In case of bash the correct middle line is 	source FAT_venv/bin/activate)
 You might have to restart the env:
 
   	deactivate
+
   	source FAT_venv/bin/activate.csh
 
 Once you have installed FAT you can check that it has been installed properly by running FAT as.
 
   	FAT>  pyFAT installation_check=True
 
 This should take typically a few minutes and should finish with the message:
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/Installation_Check/NGC_2903.fits` & `pyFAT_astro-0.1.1/pyFAT_astro/Installation_Check/NGC_2903.fits`

 * *Files identical despite different names*

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/Support/clean_functions.py` & `pyFAT_astro-0.1.1/pyFAT_astro/Support/clean_functions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,85 +1,90 @@
 # -*- coding: future_fstrings -*-
 # This module contains a set of functions and classes that are used in several different Python scripts in the Database.
 
-
+import pyFAT_astro
 import os,signal,sys
 import numpy as np
 import traceback
 from datetime import datetime
-from pyFAT_astro.Support.support_functions import print_log,finish_current_run,set_format,create_directory,get_system_string
+
 from pyFAT_astro.Support.fits_functions import make_moments
-from pyFAT_astro.Support.write_functions import make_overview_plot,plot_usage_stats,tirific,write_config
-from pyFAT_astro.Support.read_functions import tirific_template,load_tirific,load_template
-class SofiaMissingError(Exception):
-    pass
-def check_legitimacy(Configuration,debug=False):
-    if debug:
-        print_log(f'''CHECK_LEGITIMACY: Start.
-''',Configuration['OUTPUTLOG'],debug =True)
+from pyFAT_astro.Support.modify_template import get_error
+from pyFAT_astro.Support.write_functions import make_overview_plot,plot_usage_stats,tirific
+from pyFAT_astro.Support.fat_errors import SofiaMissingError
+import pyFAT_astro.Support.support_functions as sf
+import pyFAT_astro
+
+class DummyLock():
+    def __enter__(self):
+        pass
+
+    def __exit__(self, *args):
+        pass
+
+def check_legitimacy_osc(Configuration):
+    sf.print_log(f'''CHECK_LEGITIMACY_OSC: Start.
+''',Configuration,case=['debug_start'])
     if Configuration['OUTPUT_QUANTITY'] == 'error':
-        print_log(f'''CHECK_LEGITIMACY: An unspecified error is registered. The final message should reflect this.
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''CHECK_LEGITIMACY_OSC: An unspecified error is registered. The final message should reflect this.
+''',Configuration)
         return
     elif Configuration['OUTPUT_QUANTITY'] == 5:
-        print_log(f'''CHECK_LEGITIMACY: A FAT specific error is registered. The final message should reflect this.
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''CHECK_LEGITIMACY_OSC: A FAT specific error is registered. The final message should reflect this.
+''',Configuration)
         return
     else:
         fit_check=[True if 'fit_' in x.lower() else False for x in Configuration['FITTING_STAGES']]
         if any(fit_check):
             outfile = f"{Configuration['FITTING_DIR']}/{Configuration['USED_FITTING']}/{Configuration['USED_FITTING']}.def"
-    inclination = load_tirific(Configuration,outfile,Variables=['INCL'],debug=debug)[0]
+    inclination = sf.load_tirific(Configuration,outfile,Variables=['INCL'],array=True)
 
     if float(inclination[0]) < Configuration['UNRELIABLE_INCLINATION']:
         Configuration['ACCEPTED'] = False
         Configuration['FINAL_COMMENT'] = f"The final inclination is below {Configuration['UNRELIABLE_INCLINATION']}. FAT is not neccesarily reliable in this range."
-        if debug:
-            print_log(f'''CHECK_LEGITIMACY: The retrieved inclination {float(inclination[0])} is below {Configuration['UNRELIABLE_INCLINATION']} thus the fit is not accepted.
-''',Configuration['OUTPUTLOG'],debug =True)
-    if 2.*Configuration['SIZE_IN_BEAMS'] < Configuration['UNRELIABLE_SIZE']:
+        sf.print_log(f'''CHECK_LEGITIMACY_OSC: The retrieved inclination {float(inclination[0])} is below {Configuration['UNRELIABLE_INCLINATION']} thus the fit is not accepted.
+''',Configuration)
+    if np.sum(Configuration['SIZE_IN_BEAMS']) < Configuration['UNRELIABLE_SIZE']:
         Configuration['ACCEPTED'] = False
         Configuration['FINAL_COMMENT'] = f"The final size is below {Configuration['UNRELIABLE_SIZE']}. FAT is not neccesarily reliable in this range."
-        if debug:
-            print_log(f'''CHECK_LEGITIMACY: The retrieved size {2.*Configuration['SIZE_IN_BEAMS']} is below {Configuration['UNRELIABLE_SIZE']} thus the fit is not accepted.
-''',Configuration['OUTPUTLOG'],debug =True)
+        sf.print_log(f'''CHECK_LEGITIMACY_OSC: The retrieved size {np.sum(Configuration['SIZE_IN_BEAMS'])} is below {Configuration['UNRELIABLE_SIZE']} thus the fit is not accepted.
+''',Configuration)
     return
 
-check_legitimacy.__doc__ =f'''
+check_legitimacy_osc.__doc__ =f'''
  NAME:
-    check_legitimacy
+    check_legitimacy_osc
 
  PURPOSE:
     Check the final output to see if it falls in a reliable rangesee if the output fall in the range where FAT is reliable.
 
  CATEGORY:
     clean_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
 
  OPTIONAL INPUTS:
-    debug = False
 
  OUTPUTS:
     Updated final comment in the configuration
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
     !!!!!!! Until release these are set ridiculously low for testing purposes.
 '''
 
-def clean_before_sofia(Configuration, debug = False):
-    if debug:
-        print_log(f'''CLEAN_BEFORE_SOFIA: Starting.
-''',Configuration['OUTPUTLOG'],debug = True)
+def clean_before_sofia(Configuration):
+
+    sf.print_log(f'''CLEAN_BEFORE_SOFIA: Starting.
+''',Configuration,case = ['debug_start'])
     files =['_mask.fits','_mom0.fits','_mom1.fits','_chan.fits','_mom2.fits','_cat.txt']
 
     for file in files:
         try:
             os.remove(Configuration['BASE_NAME']+file)
         except FileNotFoundError:
             pass
@@ -106,38 +111,39 @@
  CATEGORY:
     clean_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
 
  OPTIONAL INPUTS:
-    debug = False
 
  OUTPUTS:
     Previous sofia output from fat is removed
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def clean_after_sofia(Configuration, debug = False):
+def clean_after_sofia(Configuration):
+    sf.print_log(f'''CLEAN_AFTER_SOFIA: Starting clean
+''',Configuration,case = ['debug_start'])
     files =['_mask.fits','_chan.fits','_cat.txt']
 
     for file in files:
         try:
             os.rename(Configuration['BASE_NAME']+file,'Sofia_Output/'+Configuration['BASE_NAME']+file )
-        except:
+        except FileNotFoundError:
             pass
     try:
         os.rename('sofia_input.par','Sofia_Output/sofia_input.par')
-    except:
+    except FileNotFoundError:
         pass
 
 clean_after_sofia.__doc__ =f'''
  NAME:
     clean_after_sofia
 
  PURPOSE:
@@ -146,50 +152,56 @@
  CATEGORY:
     clean_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
 
  OPTIONAL INPUTS:
-    debug = False
 
  OUTPUTS:
     sofia output files are moved to a dedicated directory.
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 # cleanup dirty files before starting fitting
-def cleanup(Configuration,Fits_Files, debug = False):
+def cleanup(Configuration,Fits_Files):
+    sf.print_log(f'''CLEANUP: Starting clean
+''',Configuration,case = ['debug_start'])
         #Move any existing output to the Log directory
     if os.path.exists(f"{Configuration['LOG_DIRECTORY']}ram_cpu.pdf"):
         if os.path.exists(f"{Configuration['LOG_DIRECTORY']}ram_cpu_prev.pdf"):
             os.remove(f"{Configuration['LOG_DIRECTORY']}ram_cpu_prev.pdf")
         os.rename( f"{Configuration['LOG_DIRECTORY']}ram_cpu.pdf",f"{Configuration['LOG_DIRECTORY']}ram_cpu_prev.pdf")
     #Move any existing Overview.png to the Log directory well
     if os.path.exists(f"{Configuration['FITTING_DIR']}Overview.png"):
         if os.path.exists(f"{Configuration['LOG_DIRECTORY']}Overview_prev.png"):
             os.remove(f"{Configuration['LOG_DIRECTORY']}Overview_prev.png")
-            if debug:
-                print_log(f'''CLEANUP: Removing an old Overview_prev.png from {Configuration['LOG_DIRECTORY']}
-''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''CLEANUP: Removing an old Overview_prev.png from {Configuration['LOG_DIRECTORY']}
+''',Configuration,case = ['debug_add'])
         os.rename( f"{Configuration['FITTING_DIR']}Overview.png",f"{Configuration['LOG_DIRECTORY']}Overview_prev.png")
-        if debug:
-            print_log(f'''CLEANUP: We moved an old Overview.png to {Configuration['LOG_DIRECTORY']}Overview_prev.png
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''CLEANUP: We moved an old Overview.png to {Configuration['LOG_DIRECTORY']}Overview_prev.png
+''',Configuration,case = ['debug_add'])
     #clean the log directory of all files except those named Prev_ and not the Log as it is already moved if existing
     files_in_log = ['restart_One_Step_Convergence.txt','restart_Centre_Convergence.txt',f"restart_{Configuration['USED_FITTING']}.txt",\
                     'restart_Extent_Convergence.txt','Usage_Statistics.txt', 'clean_map_0.fits','clean_map_1.fits','clean_map.fits',\
                     'dep_map_0.fits','minimum_map_0.fits','rot_map_0.fits','dep_map.fits','minimum_map.fits','rot_map.fits',\
-                    'dep_map_1.fits','minimum_map_1.fits','rot_map_1.fits','Convolved_Cube_FAT_opt.fits','CFG_Before_Fitting.txt']
+                    'dep_map_1.fits','minimum_map_1.fits','rot_map_1.fits','Convolved_Cube_FAT_opt.fits']
+
+    #add all CFG files:
+    for file in os.listdir(Configuration['LOG_DIRECTORY']):
+        split_file = os.path.splitext(file)
+        if split_file[-1] in ['.pkl', '.txt'] and 'CFG' in file:
+            files_in_log.append(file)
+
     for file in files_in_log:
         try:
             os.remove(f"{Configuration['LOG_DIRECTORY']}{file}")
         except FileNotFoundError:
             pass
     #            !!!!!!!!!!!!!!! The Directories cleanup should be removed before release
     Directories = ['Extent_Convergence', 'Centre_Convergence','tmp_incl_check','One_Step_Convergence']
@@ -217,41 +229,41 @@
         directories.append('Finalmodel')
         directories.append(Configuration['USED_FITTING'])
         files.append(f'{Configuration["USED_FITTING"]}_In.def')
 
     if 'create_fat_cube' in Configuration['FITTING_STAGES']:
         files.append(Fits_Files['FITTING_CUBE'])
 
-    if 'run_sofia' in Configuration['FITTING_STAGES'] or 'existing_sofia' in Configuration['FITTING_STAGES']:
+    if 'run_sofia' in Configuration['FITTING_STAGES'] or 'external_sofia' in Configuration['FITTING_STAGES']:
         dir =f'{Configuration["FITTING_DIR"]}Sofia_Output/'
         file_ext=['_mask.fits','_mom0.fits','_mom1.fits','_mom2.fits','_chan.fits','_cat.txt','_sofia_xv.fits']
-        print_log(f'''CLEANUP: We are cleaning the following files in the directory {dir}:
+        sf.print_log(f'''CLEANUP: We are cleaning the following files in the directory {dir}:
 {"":8s}CLEANUP: sofia_input.par,{','.join([f'{Configuration["SOFIA_BASENAME"]}{x}' for x in file_ext])}
-''',Configuration['OUTPUTLOG'], screen =True,debug=debug)
+''',Configuration,case = ['verbose'])
         for extension in file_ext:
             try:
                 os.remove(f'{dir}{Configuration["BASE_NAME"]}{extension}')
-            except:
+            except FileNotFoundError:
                 pass
         try:
             os.remove(f'{dir}sofia_input.par')
-        except:
+        except FileNotFoundError:
             pass
     if 'tirshaker' in Configuration['FITTING_STAGES']:
         directories.append('Error_Shaker')
     # Existing_Sofia
 
 
 
     if directories:
-        print_log(f'''CLEANUP: We are cleaning the following directories:
+        sf.print_log(f'''CLEANUP: We are cleaning the following directories:
 {"":8s}CLEANUP: {','.join(directories)}
 {"":8s}CLEANUP: and the following files:
 {"":8s}CLEANUP: {','.join(files)}
-''',Configuration['OUTPUTLOG'], screen =True,debug=debug)
+''',Configuration, case=['verbose'])
 
 
         ext=['.fits','_Prev.fits','.log','.ps','.def']
         moments = ['mom0','mom1','mom2', 'xv']
         #then specific files in the working directory
         #os.chdir(Configuration['FITTING_DIR'])
         #for configuration purposes we remove the old dirs
@@ -263,36 +275,34 @@
                 for fe in ext:
                     if dir == 'Finalmodel' and fe in ['.fits','.def']:
                         try:
                             os.unlink(f'{Configuration["FITTING_DIR"]}{dir}/{dir}{fe}')
                         except FileNotFoundError:
                             pass
                     elif dir == Configuration['USED_FITTING'] and fe in ['.def']:
-                        target = get_system_string(f"{Configuration['FITTING_DIR']}{dir}/{dir}*{fe}")
+                        target = sf.get_system_string(f"{Configuration['FITTING_DIR']}{dir}/{dir}*{fe}")
                         os.system(f'rm -f {target}')
                     else:
                         try:
                             os.remove(f'{Configuration["FITTING_DIR"]}{dir}/{dir}{fe}')
                         except FileNotFoundError:
                             pass
 
                 for mom in moments:
                     try:
                         os.remove(f'{Configuration["FITTING_DIR"]}{dir}/{dir}_{mom}.fits')
                     except FileNotFoundError:
                         pass
 
 
-        for file in files:
-            try:
-                os.remove(f'{Configuration["FITTING_DIR"]}{file}')
-            except FileNotFoundError:
-                pass
-        #Change back to original dir
-        #os.chdir(Configuration['START_DIRECTORY'])
+    for file in files:
+        try:
+            os.remove(f'{Configuration["FITTING_DIR"]}{file}')
+        except FileNotFoundError:
+            pass
 
 cleanup.__doc__ =f'''
  NAME:
     cleanup
 
  PURPOSE:
     Clean up any existing files before fitting start, it will only remove specific
@@ -302,30 +312,29 @@
     clean_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
 
  OPTIONAL INPUTS:
-    debug = False
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def cleanup_final(Configuration,Fits_Files, debug =False):
-    if debug:
-         print_log(f'''Starting the final cleanup of the directory.
-''',Configuration['OUTPUTLOG'],debug = True)
+def cleanup_final(Configuration,Fits_Files):
+    sf.print_log(f'''CLEANUP_FINAL: Starting the final cleanup of the directory.
+{'':8s} The request is {Configuration['OUTPUT_QUANTITY']}
+''',Configuration,case = ['debug_start','verbose'] )
 
     if Configuration['USED_FITTING'] == 'Fit_Tirific_OSC':
         clean_files = [Fits_Files['OPTIMIZED_CUBE'],f"{Configuration['USED_FITTING']}_In.def",\
                         "clean_map_0.fits","dep_map_0.fits","minimum_map_0.fits","rot_map_0.fits",\
                         "clean_map_1.fits","dep_map_1.fits","minimum_map_1.fits","rot_map_1.fits",
                         "tmp_incl_check_In.def"\
                         ]
@@ -337,15 +346,14 @@
             if Configuration['OUTPUT_QUANTITY'] >= 5 or Configuration['OUTPUT_QUANTITY'] == 0:
                 os.rename(f"{Configuration['FITTING_DIR']}{file}",f"{Configuration['LOG_DIRECTORY']}{file}")
             else:
                 os.remove(f"{Configuration['FITTING_DIR']}{file}")
         except FileNotFoundError:
             pass
 
-    #fit_directories = ['Centre_Convergence', 'Extent_Convergence']
     fit_directories = [Configuration['USED_FITTING']]
     delete_ext = ['.log']
     if Configuration['OUTPUT_QUANTITY'] == 4:
         delete_ext.append('.fits')
 
     for dir in fit_directories:
         try:
@@ -356,18 +364,22 @@
         for file in files_in_dir:
             name,extension = os.path.splitext(f"{Configuration['FITTING_DIR']}{dir}/{file}")
             if extension in delete_ext:
                 try:
                     os.remove(f"{Configuration['FITTING_DIR']}{dir}/{file}")
                 except FileNotFoundError:
                     pass
-            if (Configuration['OUTPUT_QUANTITY'] == 2 and extension != ".fits") or (5 >= Configuration['OUTPUT_QUANTITY'] >= 3) :
-                if (file != f"{Configuration['USED_FITTING']}.def" and file != f"{Configuration['USED_FITTING']}.fits") :
+                except IsADirectoryError:
+                    pass
+            if (Configuration['OUTPUT_QUANTITY'] == 2 and extension != ".fits") \
+                or (5 > Configuration['OUTPUT_QUANTITY'] >= 3):
+                if file != f"{Configuration['USED_FITTING']}.def" and file != f"{Configuration['USED_FITTING']}.fits":
                     try:
-                        os.remove(f"{Configuration['FITTING_DIR']}{dir}/{file}")
+                        if not (Configuration['DEBUG'] and extension == '.def'):
+                            os.remove(f"{Configuration['FITTING_DIR']}{dir}/{file}")
                     except FileNotFoundError:
                         pass
     stage_dirs = []
     if os.path.isdir(f"{Configuration['FITTING_DIR']}tmp_incl_check"):
         stage_dirs.append('tmp_incl_check')
     if 'tirshaker' in Configuration['FITTING_STAGES']:
         stage_dirs.append('Error_Shaker')
@@ -379,18 +391,18 @@
                 try:
                     os.remove(f"{Configuration['FITTING_DIR']}{dirs}/{file}")
                 except FileNotFoundError:
                     pass
             os.rmdir(f"{Configuration['FITTING_DIR']}{dirs}")
         else:
             # else move this directory to the LOG
-            target = get_system_string(f"{Configuration['LOG_DIRECTORY']}{dirs}")
+            target = sf.get_system_string(f"{Configuration['LOG_DIRECTORY']}{dirs}")
             if  os.path.isdir(f"{Configuration['LOG_DIRECTORY']}{dirs}"):
                 os.system(f"rm -Rf {target}")
-            source = get_system_string(f"{Configuration['FITTING_DIR']}{dirs}")
+            source = sf.get_system_string(f"{Configuration['FITTING_DIR']}{dirs}")
             os.system(f"mv {source} {target}")
 
 
 cleanup_final.__doc__ =f'''
  NAME:
     cleanup_final
 
@@ -402,15 +414,14 @@
     clean_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
 
  OPTIONAL INPUTS:
-    debug = False
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
@@ -418,53 +429,52 @@
  NOTE:
 '''
 
 
 
 
 
-def installation_check(Configuration, debug =False):
-    if debug:
-         print_log(f'''INSTALLATION_CHECK: Starting to compare the output to what is expected.
-''',Configuration['OUTPUTLOG'],debug = True)
+def installation_check(Configuration):
+    sf.print_log(f'''INSTALLATION_CHECK: Starting to compare the output to what is expected.
+''',Configuration, case = ['debug_start', 'main'])
 
-    Model = tirific_template(filename = 'Installation_Check', debug= debug)
+    Model = sf.tirific_template(filename = 'Installation_Check')
     Variables_to_Compare = ['VROT','INCL','PA','SBR','SDIS','Z0','XPOS','YPOS','VSYS']
-    Model_values = load_template(Configuration,Model,Variables = Variables_to_Compare,unpack = False,debug=debug)
+    Model_values = sf.load_tirific(Configuration,Model,\
+        Variables = Variables_to_Compare,array=True)
     #Then the fitted file
-    Fitted_values =load_tirific(Configuration,f"{Configuration['FITTING_DIR']}Finalmodel/Finalmodel.def",Variables = Variables_to_Compare,unpack = False,debug=debug)
+    Fitted_values =sf.load_tirific(Configuration,\
+        f"{Configuration['FITTING_DIR']}Finalmodel/Finalmodel.def",\
+        Variables = Variables_to_Compare,array = True)
     succes = False
+    diff = np.abs(Model_values-Fitted_values)
 
-    try:
-        diff = np.abs(np.array(Model_values,dtype=float)-np.array(Fitted_values,dtype=float))
-        if debug:
-            print_log(f'''INSTALLATION_CHECK: the found differences
+    sf.print_log(f'''INSTALLATION_CHECK: the found differences
 {'':8s}{diff}
-''',Configuration['OUTPUTLOG'])
-        too_much = np.array(np.where(diff > 1e-3),dtype=bool)
-        if debug:
-            print_log(f'''INSTALLATION_CHECK: at the locations
+''',Configuration, case = ['verbose'])
+    too_much = np.array(np.where(diff > 1e-3),dtype=bool)
+
+    sf.print_log(f'''INSTALLATION_CHECK: at the locations
 {'':8s}{too_much}{np.where(diff > 1e-3)}
 {'':8s}{too_much.size}
-''',Configuration['OUTPUTLOG'])
+''',Configuration, case = ['verbose'])
+
+    if too_much.size == 0.:
+        succes = True
 
-        if too_much.size == 0.:
-            succes = True
-    except:
-        pass
 
     if succes:
-        print_log(f'''
+        sf.print_log(f'''
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 !!!!!!!!!!!!!!!!!!! All parameters are fitted within the expected variance. !!!!!!!!!!!!!!!!
 !!!!!!!!!!!!!!!!!!!        We think pyFAT is installed succesfully          !!!!!!!!!!!!!!!!
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-''',Configuration['OUTPUTLOG'],screen =True)
+''',Configuration, case = ['main','screen'])
     else:
-        print_log(f'''
+        sf.print_log(f'''
 !!!!---------------------------------------------!!!!!
 !!!! FAT ran through the fitting process but the !!!!!
 !!!! fitted values differ too much from their    !!!!!
 !!!! expectations. Please update SoFiA and other !!!!!
 !!!! dependencies. I f you have done so and this !!!!!
 !!!! message remains, the check is likely out of !!!!!
 !!!! date. If you are unable to resolve the issue!!!!!
@@ -472,15 +482,15 @@
 !!!!                                             !!!!!
 !!!! https://github.com/PeterKamphuis/pyFAT/issues !!!!!
 !!!!                                             !!!!!
 !!!! Please add the Log.txt file in the directory!!!!!
 !!!!{Configuration['LOG_DIRECTORY']}!!!!!
 !!!! and the Finalmodel.def.                     !!!!!
 !!!!---------------------------------------------!!!!!
-''',Configuration['OUTPUTLOG'],screen =True)
+''',Configuration,case = ['main','screen'])
 
 installation_check.__doc__ =f'''
  NAME:
     installation_check
 
  PURPOSE:
     Check the installation check run against the template.
@@ -488,167 +498,192 @@
  CATEGORY:
     clean_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
 
  OPTIONAL INPUTS:
-    debug = False
 
  OUTPUTS:
     Message with succes or not to the screen and log
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def finish_galaxy(Configuration,maximum_directory_length,current_run = 'Not initialized', Fits_Files= None, debug = False,exiting = None):
+def finish_galaxy(Configuration,current_run = 'Not initialized',\
+        timing_lock= DummyLock(), catalogue_lock = DummyLock(),
+        Fits_Files= {'ORIGINAL_CUBE': "Unset.fits"},exiting = None):
     Configuration['END_TIME'] = datetime.now()
-    if debug:
-        print_log(f'''FINISH_GALAXY: These fits files are used:
+    sf.print_log(f'''FINISH_GALAXY: These fits files are used:
 {'':8s} {Fits_Files}
-''',Configuration['OUTPUTLOG'])
-        write_config(f'{Configuration["LOG_DIRECTORY"]}CFG_At_Finish.txt',Configuration,debug = True)
+''',Configuration,case = ['debug_start','verbose'])
+    if Configuration['DEBUG']:
+        sf.write_config(f'{Configuration["LOG_DIRECTORY"]}CFG_At_Finish.txt',Configuration)
 
     #make sure we are not leaving stuff
-    finish_current_run(Configuration,current_run,debug=debug)
+    sf.finish_current_run(Configuration,current_run)
     # We need to check if the final output is legit
-    if Configuration['USED_FITTING']:
-        check_legitimacy(Configuration,debug=debug)
+    if Configuration['USED_FITTING'] == 'Fit_Tirific_OSC':
+        check_legitimacy_osc(Configuration)
 
-    # Need to write to results catalog
-    if Configuration['OUTPUT_CATALOGUE']:
-        with open(Configuration['OUTPUT_CATALOGUE'],'a') as output_catalogue:
-            output_catalogue.write(f"{Configuration['FITTING_DIR'].split('/')[-2]:{maximum_directory_length}s} {str(Configuration['ACCEPTED']):>6s} {Configuration['FINAL_COMMENT']} \n")
 
     if Configuration['OUTPUT_QUANTITY'] == 'error':
         error_message = '''
             Your code has crashed for some reason. If this message completely baffles you then please submit the trace back as a bug report to: \n
             https://github.com/PeterKamphuis/pyFAT/issues \n
             If the error occured while fitting a galaxy, please attach your fitting log as well
 '''
         log_statement = f'''------------When filing a bug report please copy all output  below this line------------
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 {"":8s}FAT did not run the full fitting routines for catalog entry {Configuration['ID']}.
 {"":8s}Which is the galaxy in directory {Configuration['FITTING_DIR']}.
 {"":8s}Please check this log and output_catalogue carefully for what went wrong.
-{"":8s}The detected exit reason is {Configuration['FINAL_COMMENT']}.
+{"":8s}The detected exit reason is: "{Configuration['FINAL_COMMENT']}".
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
 '''
-        print_log(log_statement,Configuration['OUTPUTLOG'], screen = True)
-        print_log(error_message,Configuration['OUTPUTLOG'], screen = True)
+        sf.print_log(log_statement,Configuration, case = ['main','screen'])
+        sf.print_log(error_message,Configuration, case = ['main','screen'])
 
         if exiting:
             with open(Configuration['OUTPUTLOG'],'a') as log_file:
-                traceback.print_tb(exiting.__traceback__,file=log_file)
-            traceback.print_tb(exiting.__traceback__)
-        sys.exit(1)
+                traceback.print_exception(type(exiting),exiting,exiting.__traceback__,file=log_file)
+            traceback.print_exception(type(exiting),exiting,exiting.__traceback__)
+        if Configuration['MULTIPROCESSING']:
+            Configuration['ACCEPTED'] = False
+            Configuration['FINAL_COMMENT'] = f"The code crashed while fitting this galaxy please check it's log."
+            Configuration['OUTPUT_QUANTITY'] = 5
+        else:
+            if exiting:
+                sys.exit(1)
+            else:
+                Configuration['ACCEPTED'] = False
+                Configuration['FINAL_COMMENT'] = f"The code crashed while fitting this galaxy please check it's log."
+                Configuration['OUTPUT_QUANTITY'] = 5
     elif Configuration['OUTPUT_QUANTITY'] == 5:
-        log_statement = f'''
+        sf.print_log(f'''
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-{"":8s}FAT did not run the full fitting routines for the galaxy in directory {Configuration['FITTING_DIR']}.
-{"":8s}Please check this log and output_catalogue carefully for what went wrong.
-{"":8s}The detected exit reason is {Configuration['FINAL_COMMENT']}.
+{"":8s}FAT could not find an acceptable model for the galaxy in directory {Configuration['FITTING_DIR']}.
+{"":8s}Please check the log in {Configuration['LOG_DIRECTORY']} and the output_catalogue carefully for more information.
+{"":8s}The detected exit reason is: "{Configuration['FINAL_COMMENT']}".
 !!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
-'''
-        print_log(log_statement,Configuration['OUTPUTLOG'])
-        #No traceback as it is a proper exiting error
-        #if exiting:
-        #    with open(Configuration['OUTPUTLOG'],'a') as log_file:
-        #        traceback.print_tb(exiting.__traceback__,file=log_file)
-        #    traceback.print_tb(exiting.__traceback__)
+''',Configuration, case = ['main','screen'])
+
     elif Configuration['OUTPUT_QUANTITY'] < 4:
-        print_log( f'''Producing final output in {Configuration['FITTING_DIR']}.
-''',Configuration['OUTPUTLOG'], screen = True)
+        sf.print_log( f'''Producing final output in {Configuration['FITTING_DIR']}.
+''',Configuration)
         # We need to produce a FinalModel Directory with moment maps and an XV-Diagram of the model.
         if any([True if 'fit_' in x else False for x in Configuration['FITTING_STAGES']]):
-            create_directory('Finalmodel',Configuration['FITTING_DIR'])
-            transfer_errors(Configuration,fit_type=Configuration['USED_FITTING'])
-            linkname = f"../{Configuration['USED_FITTING']}/{Configuration['USED_FITTING']}"
-            os.symlink(f"{linkname}.fits",f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel.fits")
-            os.symlink(f"{linkname}.def",f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel.def")
-
-            # We need to produce a FinalModel Directory with moment maps and an XV-Diagram of the model.
-            if Fits_Files and os.path.exists(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel.fits"):
-                make_moments(Configuration,Fits_Files,fit_type = 'Generic_Final',vel_unit = 'm/s',debug=debug)
-                make_overview_plot(Configuration,Fits_Files,debug=debug)
+            if not 'Fit_Make_Your_Own' in  Configuration['USED_FITTING']:
+                sf.create_directory('Finalmodel',Configuration['FITTING_DIR'])
+                if 'tirshaker' not in Configuration['FITTING_STAGES'] and not Configuration['INSTALLATION_CHECK']:
+                    transfer_errors(Configuration,fit_type=Configuration['USED_FITTING'])
+                linkname = f"../{Configuration['USED_FITTING']}/{Configuration['USED_FITTING']}"
+                os.symlink(f"{linkname}.fits",f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel.fits")
+                os.symlink(f"{linkname}.def",f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel.def")
+
+                # We need to produce a FinalModel Directory with moment maps and an XV-Diagram of the model.
+                if Fits_Files and os.path.exists(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel.fits"):
+                    make_moments(Configuration,Fits_Files,fit_type = 'Generic_Final',vel_unit = 'm/s')
+                    make_overview_plot(Configuration,Fits_Files)
 
-    log_statement = f'''Finished final output in {Configuration['FITTING_DIR']}.
-'''
-    print_log(log_statement,Configuration['OUTPUTLOG'], screen = True)
+
+    sf.print_log(f'''Finished the fitting in {Configuration['FITTING_DIR']}.
+''',Configuration, case = ['main','screen'])
     # Need to organize the fitting output orderly
     # Need to write date and Time to timing log
     if Configuration['TIMING']:
-
-        plot_usage_stats(Configuration,debug = debug)
-        timing_result = open(Configuration['MAIN_DIRECTORY']+'/Timing_Result.txt','a')
-        timing_result.write(f'''The galaxy in directory {Configuration['FITTING_DIR']} started at {Configuration['START_TIME']}.
-Finished preparations at {Configuration['PREP_END_TIME']} \n''')
-        timing_result.write(f'''Converged to a galaxy size at {Configuration['END_TIME']}. \n''')
-        timing_result.write(f'''It finished the whole process at {datetime.now()}
+        plot_usage_stats(Configuration)
+        with timing_lock:
+            with open(Configuration['MAIN_DIRECTORY']+'/Timing_Result.txt','a') as timing_result:
+                timing_result.write(f'''The galaxy in directory {Configuration['FITTING_DIR']} started at {Configuration['START_TIME']}.
+Finished preparations at {Configuration['PREP_END_TIME']}.
+Converged to a galaxy size at {Configuration['END_TIME']}.
+It finished the whole process at {datetime.now()}.
 ''')
-        timing_result.close()
-        log_statement = f'''Finished timing statistics for the galaxy in {Configuration['FITTING_DIR']}.
-'''
-        print_log(log_statement,Configuration['OUTPUTLOG'], screen = True)
 
-    cleanup_final(Configuration,Fits_Files, debug=debug)
+        sf.print_log(f'''Finished timing statistics for the galaxy in {Configuration['FITTING_DIR']}.
+''',Configuration)
+
+    cleanup_final(Configuration,Fits_Files)
+    # Need to write to results catalog
+    catalogue_line = f"{Configuration['FITTING_DIR'].split('/')[-2]:{Configuration['MAXIMUM_DIRECTORY_LENGTH']}s} {str(Configuration['ACCEPTED']):>6s} {Configuration['FINAL_COMMENT']} \n"
+
+    if Configuration['OUTPUT_CATALOGUE']:
+        with catalogue_lock:
+            with open(Configuration['OUTPUT_CATALOGUE'],'a') as output_catalogue:
+                output_catalogue.write(catalogue_line)
+
+    return catalogue_line
 
 finish_galaxy.__doc__ =f'''
  NAME:
     finish_galaxy
 
  PURPOSE:
     Write the final logs, Produce an Overview plot if required and make sure the directory is clean and organized.
 
  CATEGORY:
     clean_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
-    maximum_directory_length = the maximum string length of the input directory names
+
 
  OPTIONAL INPUTS:
-    debug = False
     current_run = subproccess structure of the currently running tirific
     Fits_Files = Standard FAT dictionary with filenames
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE: This function should always be followed by a continue statement
 '''
 
-def transfer_errors(Configuration,fit_type='Undefined',debug = False):
+def transfer_errors(Configuration,fit_type='Undefined'):
+    sf.print_log(f'''TRANSFER_ERROR: Start.
+''',Configuration, case = ['debug_start'])
     # Load the final file
-    Tirific_Template = tirific_template(filename = f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def",debug= debug)
-    # Get the errors from the input
-    errors_to_transfer= ['VROT_ERR','VROT_2_ERR','INCL_ERR','INCL_2_ERR','PA_ERR','PA_2_ERR','SDIS_ERR','SDIS_2_ERR','Z0_ERR','Z0_2_ERR']
-    FAT_Model = load_tirific(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}_In.def",Variables=errors_to_transfer,unpack=False,debug=debug)
-    # add to the templatethere
+    Tirific_Template = sf.tirific_template(filename = f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def")
+    variables = ['INCL','PA','VROT','SDIS','SBR','VSYS','XPOS','YPOS','Z0']
+    weights = sf.get_ring_weights(Configuration,Tirific_Template)
+    for parameter in variables:
+        sf.print_log(f'''TRANSFER_ERROR: Creating errors for {parameter}.
+''',Configuration, case = ['debug_add'])
+        profile = sf.load_tirific(Configuration,Tirific_Template,\
+            [parameter,f"{parameter}_2"],array=True)
+        sm_profile = sf.load_tirific(Configuration,\
+            f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Iteration_{Configuration['ITERATIONS']}.def",\
+            Variables=[parameter,f"{parameter}_2"],array=True)
+            #it is possible that the last iteration of the fitted smooth check
+            #Crashes and is rerun with
+        if parameter == 'VROT':
+            apply_max= False
+        else:
+            apply_max = True
+        errors = get_error(Configuration,sm_profile,profile,parameter,\
+            min_error=Configuration['MIN_ERROR'][parameter],\
+            apply_max_error = apply_max,weights = weights)
+        format = sf.set_format(parameter)
+        Tirific_Template.insert(parameter,f"# {parameter}_ERR",f"{' '.join([f'{x:{format}}' for x in errors[0]])}")
+        Tirific_Template.insert(f"{parameter}_2",f"# {parameter}_2_ERR",f"{' '.join([f'{x:{format}}' for x in errors[1]])}")
+
     Tirific_Template['GR_CONT']=' '
     Tirific_Template.insert('GR_CONT','RESTARTID','0')
     Tirific_Template.insert('MINDELTA','DISTANCE',Configuration['DISTANCE'])
-    length_of_current = int(Tirific_Template['NUR'])
-    for key in errors_to_transfer:
-        format = set_format(key[:-4])
-        Tirific_Template.insert(key[:-4],f"# {key}",f"{' '.join([f'{x:{format}}' for x in FAT_Model[:length_of_current,errors_to_transfer.index(key)]])}")
-        if length_of_current > len(FAT_Model[:,errors_to_transfer.index(key)]):
-            Tirific_Template[f"# {key}"] = Tirific_Template[f"# {key}"]+\
-                             f"{' '.join([f'{FAT_Model[-1,errors_to_transfer.index(key)]:{format}}' for x in range(length_of_current-len(FAT_Model[:,errors_to_transfer.index(key)]))])}"
     # write back to the File
-    tirific(Configuration,Tirific_Template, name = f"{fit_type}/{fit_type}.def", debug = debug)
+    tirific(Configuration,Tirific_Template, name = f"{fit_type}/{fit_type}.def")
 
 transfer_errors.__doc__ =f'''
  NAME:
     transfer_errors
 
  PURPOSE:
     Transfer the errors from the input file to the output as tirific removes the commented lines.
@@ -656,15 +691,14 @@
  CATEGORY:
     clean_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
 
  OPTIONAL INPUTS:
-    debug = False
     fit_type = 'Undefined'
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/Support/constants.py` & `pyFAT_astro-0.1.1/pyFAT_astro/Support/constants.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -*- coding: future_fstrings -*-
-
+import pyFAT_astro
 #def initialize():
 global H_0
 H_0 = 69.7 #km/s/Mpc
 global c
 c=299792458                  #light speed in m/s
 global pc
 pc=3.086e+18                  #parsec in cm
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/Support/development_functions.py` & `pyFAT_astro-0.1.1/pyFAT_astro/Support/development_functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: future_fstrings -*-
 # This module contains a set of functions and classes that written for developments purposes but are not included in the main part of the code.
 # If you are too lazy to properly document please keep the functions in this file until you do document.
-
+import pyFAT_astro
 from pyFAT.Support.support_functions import print_log, convert_type,set_limits,rename_fit_products,\
                               set_ring_size,calc_rings,get_usage_statistics,get_inner_fix,convertskyangle,\
                               finish_current_run, remove_inhomogeneities,get_from_template,set_format, \
                               set_rings, convertRADEC, is_available
 from pyFAT.Support.clean_functions import clean_before_sofia,clean_after_sofia
 from pyFAT.Support.fits_functions import cut_cubes,extract_pv,make_moments
 from pyFAT.Support.modify_template import write_new_to_template,smooth_profile,set_cflux,fix_sbr, \
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/Support/fat_errors.py` & `pyFAT_astro-0.1.1/pyFAT_astro/Support/fat_errors.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,51 @@
 # -*- coding: future_fstrings -*-
+import pyFAT_astro
 #Define some errors
 class BadCatalogueError(Exception):
     pass
 class BadConfigurationError(Exception):
     pass
+class BadCubeError(Exception):
+    pass
+class BadMaskError(Exception):
+    pass
 class BadSourceError(Exception):
     pass
+class BadHeaderError(Exception):
+    pass
 class CfluxError(Exception):
     pass
 class DefFileError(Exception):
     pass
+class FaintSourceError(Exception):
+    pass
 class FileNotFoundError(Exception):
     pass
+class FittingError(Exception):
+    pass
 class FunctionCallError(Exception):
     pass
 class InclinationRunError(Exception):
     pass
 class InitializeError(Exception):
     pass
 class InputError(Exception):
     pass
-class ProgramError(Exception):
-    pass
 class NoConfigFile(Exception):
     pass
+class MissingProgramError(Exception):
+    pass
+class ProgramError(Exception):
+    pass
 class SmallSourceError(Exception):
     pass
-class SofiaFaintError(Exception):
+class SofiaMissingError(Exception):
     pass
 class SofiaRunError(Exception):
     pass
 class SupportRunError(Exception):
     pass
+class TirificOutputError(Exception):
+    pass
 class TirificKillError(Exception):
     pass
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/Support/fits_functions.py` & `pyFAT_astro-0.1.1/pyFAT_astro/Support/fits_functions.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,58 +1,53 @@
 # -*- coding: future_fstrings -*-
 # This module contains a set of functions and classes that are used in several different Python scripts in the Database.
 from astropy.io import fits
 from astropy.wcs import WCS
-from pyFAT_astro.Support.support_functions import linenumber,print_log,set_limits,\
-                                                clean_header,obtain_border_pix,set_boundaries
-from pyFAT_astro.Support.fat_errors import FunctionCallError
+
+from pyFAT_astro.Support.fat_errors import FunctionCallError,BadHeaderError,\
+                                        BadCubeError,BadMaskError
+import pyFAT_astro.Support.support_functions as sf
+
 #from pyFAT_astro.Support.read_functions import obtain_border_pix
+import pyFAT_astro
 from scipy import ndimage
 import numpy as np
 import copy
 import warnings
 import os
 
-class BadHeaderError(Exception):
-    pass
-class BadCubeError(Exception):
-    pass
-class BadMaskError(Exception):
-    pass
 #Check that the mask only contains the selected sources
-def check_mask(Configuration,id,Fits_Files,debug=False):
-    if debug:
-        print_log(f'''CHECK_MASK: Checking the mask to contain only the correct source.
-''',Configuration['OUTPUTLOG'],debug=True)
-    mask = fits.open(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Fits_Files['MASK']}",uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
+def check_mask(Configuration,id,Fits_Files):
+    sf.print_log(f'''CHECK_MASK: Checking the mask to contain only the correct source.
+''',Configuration, case =['debug_start','verbose'])
+    mask = fits.open(f"{Configuration['FITTING_DIR']}/{Fits_Files['MASK']}",uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
 
     if float(id) not in mask[0].data:
-        print_log(f'''CHECK_MASK: We cannot find the selected source in the mask. This will lead to errors. Aborting the fit.
-''',Configuration['OUTPUTLOG'],screen = True,debug=debug)
+        sf.print_log(f'''CHECK_MASK: We cannot find the selected source in the mask. This will lead to errors. Aborting the fit.
+''',Configuration,case=['main','screen'])
         BadMaskError(f" We can not find the sofia source id in the mask.")
     else:
         data = copy.deepcopy(mask[0].data)
         data[data != float(id)] = 0.
         diff = data-mask[0].data
         neg_index = np.where(diff < 0.)[0]
-        if neg_index.shape:
-            if debug:
-                print_log(f'''CHECK_MASK: The initial mask had more than a single source. redoing the mask.
-''',Configuration['OUTPUTLOG'],screen = True)
+        if len(neg_index) != 0:
+            sf.print_log(f'''CHECK_MASK: The initial mask had more than a single source. redoing the mask.
+''',Configuration, case = ['verbose'])
             mask[0].data = data
-            fits.writeto(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Fits_Files['MASK']}",mask[0].data,mask[0].header, overwrite = True)
+            fits.writeto(f"{Configuration['FITTING_DIR']}{Fits_Files['MASK']}",mask[0].data,mask[0].header, overwrite = True)
 # to ensure compatible units and calculations with th models we make the maps ourselves
     del mask[0].header['C*3']
     mask[0].data[mask[0].data> 0.5] = 1.
     chan_map = np.array(np.nansum(mask[0].data,axis=0),dtype =float)
     mask[0].header['BITPIX'] = -32
     fits.writeto(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Configuration['BASE_NAME']}_chan.fits",chan_map,header=mask[0].header,overwrite = True)
     mask.close()
     if Configuration['SOFIA_RAN']:
-        make_moments(Configuration, Fits_Files,fit_type='Generic_Initialize',vel_unit = 'm/s',debug=debug)
+        make_moments(Configuration, Fits_Files,fit_type='Generic_Initialize',vel_unit = 'm/s')
 check_mask.__doc__ =f'''
  NAME:
     check_mask
 
  PURPOSE:
     Check that the mask only contains the source we want and not parts of other nearby sources.
     Subsequently make the channel_map and the moment maps.
@@ -63,15 +58,14 @@
  INPUTS:
     Configuration = Standard FAT configuration
     id = the SoFiA ID of the source we are interested in
     Fits_Files = Standard FAT dictionary with filenames
     Tirific_Template = Standard FAT Tirific Template
 
  OPTIONAL INPUTS:
-    debug = False
     fit_type = 'Undefined'
 
  OUTPUTS:
     moment maps and the channel map
 
  OPTIONAL OUTPUTS:
     a cleaned mask
@@ -82,40 +76,44 @@
  NOTE:
 '''
 
 
 
 
 # Create a cube suitable for FAT
-def create_fat_cube(Configuration, Fits_Files,sofia_catalogue=False,id='No default',name='No default', debug = False):
+def create_fat_cube(Configuration, Fits_Files,sofia_catalogue=False,\
+        id='No default',name='No default'):
     #First get the cubes
     if sofia_catalogue:
-        Cube = fits.open(f"{Configuration['SOFIA_DIR']}{name}_{id}_cube.fits",uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
+        Cube = fits.open(f"{Configuration['SOFIA_DIR']}{name}_{id}_cube.fits",\
+            uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
     else:
-        Cube = fits.open(Configuration['FITTING_DIR']+Fits_Files['ORIGINAL_CUBE'],uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
+        Cube = fits.open(Configuration['FITTING_DIR']+Fits_Files['ORIGINAL_CUBE'],\
+            uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
     data = Cube[0].data
     hdr = Cube[0].header
     if hdr['NAXIS'] == 4:
         data = data[0,:,:,:]
         del hdr['NAXIS4']
         hdr['NAXIS'] = 3
     # clean the header
-    hdr = clean_header(Configuration,hdr,debug=debug)
-    data = prep_cube(Configuration,hdr,data,debug=debug)
+    hdr = sf.clean_header(Configuration,hdr)
+    data = prep_cube(Configuration,hdr,data)
     # and write our new cube
-    log_statement = f'''CREATE_FAT_CUBE: We are writing a FAT modfied cube to be used for the fitting. This cube is called {Configuration['FITTING_DIR']+Fits_Files['FITTING_CUBE']}
-'''
-    print_log(log_statement,Configuration["OUTPUTLOG"])
+
+    sf.print_log(f'''CREATE_FAT_CUBE: We are writing a FAT modified cube to be used for the fitting. This cube is called {Configuration['FITTING_DIR']+Fits_Files['FITTING_CUBE']}
+''',Configuration)
     if sofia_catalogue:
         fits.writeto(f"{Configuration['MAIN_DIRECTORY']}{name}_FAT_cubelets/{name}_{id}/{name}_{id}_FAT.fits",data,hdr)
     else:
         fits.writeto(Configuration['FITTING_DIR']+Fits_Files['FITTING_CUBE'],data,hdr)
     # Release the arrays
 
     Cube.close()
+
     data = []
     hdr = []
 create_fat_cube.__doc__ =f'''
  NAME:
     create_fat_cube
 
  PURPOSE:
@@ -129,29 +127,29 @@
     fits_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
 
  OPTIONAL INPUTS:
-    debug = False
 
  OUTPUTS:
     The FAT input cube
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def cut_cubes(Configuration, Fits_Files, galaxy_box, debug = False):
-
+def cut_cubes(Configuration, Fits_Files, galaxy_box):
+    sf.print_log(f'''CUT_CUBES: Starting to cut the cube_size.
+''', Configuration, case= ['debug_start'])
     cube_edge= [6.,5.*round(Configuration['BEAM_IN_PIXELS'][0]),5.*round(Configuration['BEAM_IN_PIXELS'][0])]
     cube_size= []
     new_cube = []
     for i in [2,1,0]:
         cube_size.append(Configuration['NAXES'][i])
         new_cube.append([0,Configuration['NAXES'][i]])
     new_cube = np.array(new_cube,dtype=int)
@@ -159,48 +157,49 @@
     for i,limit in enumerate(galaxy_box):
         if limit[0] > cube_edge[i]:
             cut = True
             new_cube[i,0] = limit[0]-int(cube_edge[i])
         if limit[1] < cube_size[i] - cube_edge[i]:
             cut = True
             new_cube[i,1] = limit[1]+int(cube_edge[i])
-
-
-    if cut:
-        files_to_cut = [Fits_Files['FITTING_CUBE'],'Sofia_Output/'+Fits_Files['MASK'],\
-                        'Sofia_Output/'+Fits_Files['MOMENT0'],\
-                        'Sofia_Output/'+Fits_Files['MOMENT1'],\
-                        'Sofia_Output/'+Fits_Files['MOMENT2'],\
-                        'Sofia_Output/'+Fits_Files['CHANNEL_MAP'],\
+    if 'restart_fitting' in [x.lower() for x in Configuration['FITTING_STAGES']]:
+        if 'create_fat_cube' in [x.lower() for x in Configuration['FITTING_STAGES']]:
+            files_to_cut = [Fits_Files['FITTING_CUBE']]
+        else:
+            cut = False
+    else:
+        files_to_cut = [Fits_Files['FITTING_CUBE'],Fits_Files['MASK'],\
+                        Fits_Files['MOMENT0'],\
+                        Fits_Files['MOMENT1'],\
+                        Fits_Files['MOMENT2'],\
+                        Fits_Files['CHANNEL_MAP'],\
                         ]
-
-
-        print_log(f'''CUT_CUBES: Your input cube is significantly larger than the detected source.
+    if cut:
+        sf.print_log(f'''CUT_CUBES: Your input cube is significantly larger than the detected source.
 {"":8s}CUT_CUBES: we will cut to x-axis = [{new_cube[2,0]},{new_cube[2,1]}] y-axis = [{new_cube[1,0]},{new_cube[1,1]}]
 {"":8s}CUT_CUBES: z-axis = [{new_cube[2,0]},{new_cube[2,1]}].
 {"":8s}CUT_CUBES: We will cut the following files:
 {"":8s}CUT_CUBES: {', '.join(files_to_cut)}
-''', Configuration['OUTPUTLOG'])
+''', Configuration)
 
         for file in files_to_cut:
-            if debug:
-                print_log(f'''CUT_CUBES: We are cutting the file {file}
-''', Configuration['OUTPUTLOG'],screen=True)
+            sf.print_log(f'''CUT_CUBES: We are cutting the file {file}
+''', Configuration)
             if os.path.exists(f"{Configuration['FITTING_DIR']}{file}"):
-                cutout_cube(Configuration,file,new_cube,debug=debug)
+                cutout_cube(Configuration,file,new_cube)
             else:
-                if file == 'Sofia_Output/'+Fits_Files['CHANNEL_MAP']:
+                if file == Fits_Files['CHANNEL_MAP']:
                     pass
                 else:
                     raise FunctionCallError(f'We are trying to cut {file} but it does not exist')
 
 
     #We want to check if the cube has a decent number of pixels per beam.
     if not os.path.exists(f"{Configuration['FITTING_DIR']}/{Fits_Files['OPTIMIZED_CUBE']}"):
-        optimized_cube(Configuration, Fits_Files,debug=debug)
+        optimized_cube(Configuration, Fits_Files)
     return new_cube
 cut_cubes.__doc__ =f'''
  NAME:
     cut_cubes
 
  PURPOSE:
     Cut all FAT related output back in size to a system that fits snugly around the sofia detection
@@ -212,30 +211,29 @@
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
     galaxy_box = array that contains the new size as
                  [[z_min,z_max],[y_min,y_max], [x_min,x_max]]
                  adhering to fits' idiotic way of reading fits files
 
  OPTIONAL INPUTS:
-    debug = False
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     cutout_cube, optimized_cube
 
  NOTE: The cut cubes will overwrite the _FAT products
        down to size and overwrite the existing files,
        User supplied SoFIA products are hence copied as fat products.
        To keep them safe.
 '''
 
-def cutout_cube(Configuration,filename,sub_cube, debug = False):
+def cutout_cube(Configuration,filename,sub_cube):
     Cube = fits.open(Configuration['FITTING_DIR']+filename,uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
     hdr = Cube[0].header
 
     if hdr['NAXIS'] == 3:
         data = Cube[0].data[sub_cube[0,0]:sub_cube[0,1],sub_cube[1,0]:sub_cube[1,1],sub_cube[2,0]:sub_cube[2,1]]
         hdr['NAXIS1'] = sub_cube[2,1]-sub_cube[2,0]
         hdr['NAXIS2'] = sub_cube[1,1]-sub_cube[1,0]
@@ -249,17 +247,17 @@
             warnings.simplefilter("ignore")
             coordinate_frame = WCS(hdr)
             xlow,ylow,zlow = coordinate_frame.wcs_pix2world(1,1,1., 1.)
             xhigh,yhigh,zhigh = coordinate_frame.wcs_pix2world(*Configuration['NAXES'], 1.)
             xlim = np.sort([xlow,xhigh])
             ylim = np.sort([ylow,yhigh])
             zlim =np.sort([zlow,zhigh])/1000.
-            set_boundaries(Configuration,'VSYS',*zlim,input=True,debug=debug)
-            set_boundaries(Configuration,'XPOS',*xlim,input=True,debug=debug)
-            set_boundaries(Configuration,'YPOS',*ylim,input=True,debug=debug)
+            sf.set_boundaries(Configuration,'VSYS',*zlim,input=True)
+            sf.set_boundaries(Configuration,'XPOS',*xlim,input=True)
+            sf.set_boundaries(Configuration,'YPOS',*ylim,input=True)
 
     elif hdr['NAXIS'] == 2:
         data = Cube[0].data[sub_cube[1,0]:sub_cube[1,1],sub_cube[2,0]:sub_cube[2,1]]
         hdr['NAXIS1'] = sub_cube[2,1]-sub_cube[2,0]
         hdr['NAXIS2'] = sub_cube[1,1]-sub_cube[1,0]
         hdr['CRPIX1'] = hdr['CRPIX1'] -sub_cube[2,0]
         hdr['CRPIX2'] = hdr['CRPIX2'] -sub_cube[1,0]
@@ -280,36 +278,34 @@
     Configuration = Standard FAT configuration
     filename = name of the cube to be cut
     sub_cube = array that contains the new size as
                 [[z_min,z_max],[y_min,y_max], [x_min,x_max]]
                 adhering to fits' idiotic way of reading fits files.
 
  OPTIONAL INPUTS:
-    debug = False
 
  OUTPUTS:
     the cut cube is written to disk.
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 # Extract a PV-Diagrams
-def extract_pv(Configuration,cube_in,angle,center=[-1,-1,-1],finalsize=[-1,-1],convert=-1, debug = False):
-    if debug:
-        print_log(f'''EXTRACT_PV: We are the extraction of a PV-Diagram
+def extract_pv(Configuration,cube_in,angle,center=[-1,-1,-1],finalsize=[-1,-1],convert=-1):
+    sf.print_log(f'''EXTRACT_PV: We are the extraction of a PV-Diagram
 {'':8s} PA = {angle}
 {'':8s} center = {center}
 {'':8s} finalsize = {finalsize}
 {'':8s} convert = {convert}
-''', Configuration['OUTPUTLOG'], debug =True)
+''', Configuration, case = ['debug_start'])
 
 
     cube = copy.deepcopy(cube_in)
     hdr = copy.deepcopy(cube[0].header)
     TwoD_hdr= copy.deepcopy(cube[0].header)
     data = copy.deepcopy(cube[0].data)
     #Because astro py is even dumber than Python
@@ -334,21 +330,21 @@
     nz, ny, nx = data.shape
     if finalsize[0] != -1:
         if finalsize[1] >nz:
             finalsize[1] = nz
         if finalsize[0] > nx:
             finalsize[0] = nx
     # if the center is not set assume the crval values
-    if debug:
-        print_log(f'''EXTRACT_PV: The shape of the output
+
+    sf.print_log(f'''EXTRACT_PV: The shape of the output
 {'':8s} nz = {nz}
 {'':8s} ny = {ny}
 {'':8s} nx = {nx}
-''', Configuration['OUTPUTLOG'])
-    x1,x2,y1,y2 = obtain_border_pix(Configuration,angle,[xcenter,ycenter],debug=debug)
+''', Configuration,case=['verbose'])
+    x1,x2,y1,y2 = sf.obtain_border_pix(Configuration,angle,[xcenter,ycenter])
     linex,liney,linez = np.linspace(x1,x2,nx), np.linspace(y1,y2,nx), np.linspace(0,nz-1,nz)
     #This only works when ny == nx hence nx is used in liney
     new_coordinates = np.array([(z,y,x)
                         for z in linez
                         for y,x in zip(liney,linex)
                         ],dtype=float).transpose().reshape((-1,nz,nx))
     #spatial_resolution = abs((abs(x2-x1)/nx)*np.sin(np.radians(angle)))+abs(abs(y2-y1)/ny*np.cos(np.radians(angle)))
@@ -359,60 +355,58 @@
     if finalsize[0] == -1:
         # then lets update the header
         # As python is stupid making a simple copy will mean that these changes are still applied to hudulist
         TwoD_hdr['NAXIS2'] = nz
         TwoD_hdr['NAXIS1'] = nx
 
         TwoD_hdr['CRPIX2'] = hdr['CRPIX3']
-        if convert !=-1:
-            TwoD_hdr['CRVAL2'] = hdr['CRVAL3']/convert
-        else:
-            TwoD_hdr['CRVAL2'] = hdr['CRVAL3']
         TwoD_hdr['CRPIX1'] = xcenter+1
     else:
-        zstart = set_limits(int(zcenter-finalsize[1]/2.),0,int(nz))
-        zend = set_limits(int(zcenter+finalsize[1]/2.),0,int(nz))
-        xstart = set_limits(int(xcenter-finalsize[0]/2.),0,int(nx))
-        xend = set_limits(int(xcenter+finalsize[0]/2.),0,int(nx))
+        zstart = sf.set_limits(int(zcenter-finalsize[1]/2.),0,int(nz))
+        zend = sf.set_limits(int(zcenter+finalsize[1]/2.),0,int(nz))
+        xstart = sf.set_limits(int(xcenter-finalsize[0]/2.),0,int(nx))
+        xend = sf.set_limits(int(xcenter+finalsize[0]/2.),0,int(nx))
+
         PV =  PV[zstart:zend, xstart:xend]
         TwoD_hdr['NAXIS2'] = int(finalsize[1])
         TwoD_hdr['NAXIS1'] = int(finalsize[0])
         TwoD_hdr['CRPIX2'] = hdr['CRPIX3']-int(nz/2.-finalsize[1]/2.)
-        if convert !=-1:
-            TwoD_hdr['CRVAL2'] = hdr['CRVAL3']/convert
-        else:
-            TwoD_hdr['CRVAL2'] = hdr['CRVAL3']
-
         TwoD_hdr['CRPIX1'] = int(finalsize[0]/2.)+1
+
     if convert !=-1:
+        TwoD_hdr['CRVAL2'] = hdr['CRVAL3']/convert
         TwoD_hdr['CDELT2'] = hdr['CDELT3']/convert
     else:
+        TwoD_hdr['CRVAL2'] = hdr['CRVAL3']
         TwoD_hdr['CDELT2'] = hdr['CDELT3']
     TwoD_hdr['CTYPE2'] = hdr['CTYPE3']
     try:
-        if hdr['CUNIT3'].lower() == 'm/s' and convert == -1:
+        if hdr['CUNIT3'].lower() == 'm/s' and convert == 1000. :
             TwoD_hdr['CDELT2'] = hdr['CDELT3']/1000.
             TwoD_hdr['CRVAL2'] = hdr['CRVAL3']/1000.
             TwoD_hdr['CUNIT2'] = 'km/s'
             del (TwoD_hdr['CUNIT3'])
         elif  convert != -1:
             del (TwoD_hdr['CUNIT3'])
-            del (TwoD_hdr['CUNIT2'])
+            try:
+                del (TwoD_hdr['CUNIT2'])
+            except KeyError:
+                pass
         else:
             TwoD_hdr['CUNIT2'] = hdr['CUNIT3']
             del (TwoD_hdr['CUNIT3'])
-    except:
-        print_log(f'''EXTRACT_PV: We could not find units in the header for the 3rd axis.
-''', Configuration['OUTPUTLOG'])
+    except KeyError:
+        sf.print_log(f'''EXTRACT_PV: We could not find units in the header for the 3rd axis.
+''', Configuration)
     del (TwoD_hdr['CRPIX3'])
     del (TwoD_hdr['CRVAL3'])
     del (TwoD_hdr['CDELT3'])
     del (TwoD_hdr['CTYPE3'])
-
     del (TwoD_hdr['NAXIS3'])
+    TwoD_hdr['NAXIS'] = 2
     TwoD_hdr['CRVAL1'] = 0.
     #Because we used nx in the linspace for liney we also use it here
     TwoD_hdr['CDELT1'] = np.sqrt(((x2-x1)*abs(hdr['CDELT1'])/nx)**2+((y2-y1)*abs(hdr['CDELT2'])/nx)**2)*3600.
 
     TwoD_hdr['CTYPE1'] = 'OFFSET'
     TwoD_hdr['CUNIT1'] = 'ARCSEC'
     TwoD_hdr['HISTORY'] = f'EXTRACT_PV: PV diagram extracted with angle {angle} and center {center}'
@@ -442,98 +436,99 @@
 
     finalsize = [-1,-1,-1]
     final size of the PV-diagram in pixels, default is no cutting
 
     convert=-1
     conversion factor for velocity axis, default no conversion
 
-    debug = False
-
  KEYWORD PARAMETERS:
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 
-def prep_cube(Configuration,hdr,data, debug = False):
-    if debug:
-        print_log( f'''PREPROCESSING: starting the preprocessing of the cube
-''',Configuration['OUTPUTLOG'],debug = True)
+def prep_cube(Configuration,hdr,data):
+    sf.print_log( f'''PREPROCESSING: starting the preprocessing of the cube
+''',Configuration, case = ['debug_start'])
 
     if hdr['CDELT3'] < -1:
-        print_log( f'''PREPROCESSING: Your velocity axis is declining with increasing channels
+        sf.print_log( f'''PREPROCESSING: Your velocity axis is declining with increasing channels
 {"":8s}PREPROCESSING: We reversed the velocity axis.
-''', Configuration['OUTPUTLOG'])
+''', Configuration)
         hdr['CDELT3'] = abs(hdr['CDELT3'])
         hdr['CRPIX3'] = hdr['NAXIS3']-hdr['CRPIX3']+1
         data = data[::-1,:,:]
     #Check for zeros
     if np.where(data == 0.):
-        print_log(f'''PREPROCESSING: Your cube contains values exactly 0. If this is padding these should be blanks.
+        sf.print_log(f'''PREPROCESSING: Your cube contains values exactly 0. If this is padding these should be blanks.
 {"":8s}PREPROCESSING: We have changed them to blanks.
-''', Configuration['OUTPUTLOG'])
+''', Configuration)
         data[np.where(data == 0.)] = float('NaN')
 
     # check for blank channels and noise statistics
     cube_ok = False
     prev_first_comparison = 0.
     prev_last_comparison = 0.
     times_cut_first_channel = 0
     times_cut_last_channel = 0
+    corner_box_size = int(np.floor(2*hdr['BMAJ']/abs(hdr['CDELT1'])))
+    if corner_box_size > np.mean([hdr['NAXIS1'],hdr['NAXIS2']])/10.:
+        corner_box_size=int(np.floor(np.mean([hdr['NAXIS1'],hdr['NAXIS2']])/10.))
     while not cube_ok:
         while np.isnan(data[0,:,:]).all():
             data=data[1:,:,:]
             hdr['NAXIS3'] = hdr['NAXIS3']-1
+            hdr['CRPIX3'] = hdr['CRPIX3'] - 1
             if hdr['NAXIS3'] < 5:
-                print_log(f'''PREPROCESSING: This cube has too many blanked channels.
-''', Configuration['OUTPUTLOG'],screen=True)
+                sf.print_log(f'''PREPROCESSING: This cube has too many blanked channels.
+''', Configuration,case = ['main', 'screen'])
                 raise BadCubeError("The cube has too many blanked channels")
             log_statement = f'''PREPROCESSING: We are cutting the cube as the first channel is completely blank.
 '''
-            print_log(f'''PREPROCESSING: We are cutting the cube as the first channel is completely blank.
-''', Configuration['OUTPUTLOG'])
+            sf.print_log(f'''PREPROCESSING: We are cutting the cube as the first channel is completely blank.
+''', Configuration)
         while np.isnan(data[-1,:,:]).all():
             data=data[:-1,:,:]
             hdr['NAXIS3'] = hdr['NAXIS3']-1
             if hdr['NAXIS3'] < 5:
-                print_log(f'''PREPROCESSING: This cube has too many blanked channels.
-''', Configuration['OUTPUTLOG'],screen = True)
+                sf.print_log(f'''PREPROCESSING: This cube has too many blanked channels.
+''', Configuration,case = ['main', 'screen'])
                 raise BadCubeError("The cube has too many blanked channels")
-            print_log(f'''PREPROCESSING: We are cutting the cube as the last channel is completely blank.
-''', Configuration['OUTPUTLOG'])
+            sf.print_log(f'''PREPROCESSING: We are cutting the cube as the last channel is completely blank.
+''', Configuration)
         #Then check the noise statistics
         noise_first_channel = np.nanstd(data[0,:,:])
         noise_last_channel = np.nanstd(data[-1,:,:])
-        noise_bottom_right =  np.nanstd(data[:,:6,-6:])
-        noise_top_right =  np.nanstd(data[:,-6:,-6:])
-        noise_bottom_left =  np.nanstd(data[:,:6,:6])
-        noise_top_left =  np.nanstd(data[:,-6:,:6])
+        noise_bottom_right =  np.nanstd(data[:,:corner_box_size,-corner_box_size:])
+        noise_top_right =  np.nanstd(data[:,-corner_box_size:,-corner_box_size:])
+        noise_bottom_left =  np.nanstd(data[:,:corner_box_size,:corner_box_size])
+        noise_top_left =  np.nanstd(data[:,-corner_box_size:,:corner_box_size])
         noise_corner = np.nanmean([noise_top_right,noise_bottom_right,noise_bottom_left,noise_top_left])
         channel_noise = np.nanmean([noise_first_channel,noise_last_channel])
         if ~np.isfinite(noise_corner):
             noise_corner = copy.deepcopy(channel_noise)
         difference = abs((noise_first_channel-noise_last_channel)/noise_first_channel)
         if noise_corner/channel_noise >1.5 and difference < 0.2:
             noise_corner = copy.deepcopy(channel_noise)
         difference2 = abs(channel_noise-noise_corner)/channel_noise
         if difference < 0.2 and np.isfinite(difference) and difference2 < 0.25:
             cube_ok = True
         else:
-            print_log(f'''PREPROCESSING: We are cutting the cube as clearly the noise statistics are off.
+            sf.print_log(f'''PREPROCESSING: We are cutting the cube as clearly the noise statistics are off.
 {"":8s}PREPROCESSING: Noise in the first channel is {noise_first_channel}
 {"":8s}PREPROCESSING: Noise in the last channel is {noise_last_channel}
 {"":8s}PREPROCESSING: Noise in the corners is {noise_corner}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['verbose'])
             first_comparison = abs(noise_first_channel-noise_corner)/noise_corner
             last_comparison = abs(noise_last_channel-noise_corner)/noise_corner
             if prev_first_comparison == 0:
                 prev_first_comparison = first_comparison
             if prev_last_comparison == 0.:
                 prev_last_comparison = last_comparison
             if (first_comparison > last_comparison and \
@@ -553,43 +548,71 @@
                     data=data[:-1,:,:]
                     hdr['NAXIS3'] = hdr['NAXIS3'] - 1
                 else:
                     cube_ok = True
 
             if times_cut_first_channel >= 8 and times_cut_last_channel >= 8:
                 cube_ok = True
-                print_log( f'''PREPROCESSING: This cube has non-uniform noise statistics.'
-''',Configuration['OUTPUTLOG'])
+                sf.print_log( f'''PREPROCESSING: This cube has non-uniform noise statistics.'
+''',Configuration)
             if hdr['NAXIS3'] < 5:
-                print_log(f'''PREPROCESSING: This cube has noise statistics that cannot be dealt with.
-''',Configuration['OUTPUTLOG'],screen=True)
+                sf.print_log(f'''PREPROCESSING: This cube has noise statistics that cannot be dealt with.
+''',Configuration,case = ['main','screen'])
                 raise BadCubeError('The Cube has noise statistics that cannot be dealt with')
     if ~np.isfinite(noise_corner):
-        print_log(f'''PREPROCESSING: This cube has noise statistics that cannot be dealt with.
-''',Configuration['OUTPUTLOG'],screen=True)
+        sf.print_log(f'''PREPROCESSING: This cube has noise statistics that cannot be dealt with.
+''',Configuration,case = ['main','screen'])
         raise BadCubeError('The Cube has noise statistics that cannot be dealt with')
-    hdr['FATNOISE'] = noise_corner
+    #hdr['FATNOISE'] = noise_corner
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         low_noise_indices = np.where(data < -10*noise_corner)
-    if len(low_noise_indices) > 0:
+    if len(low_noise_indices) > 0.0001*hdr['NAXIS1']*hdr['NAXIS2']*hdr['NAXIS3']:
         data[low_noise_indices] = float('NaN')
-        print_log(f'''PREPROCESSING: Your cube had values below -10*sigma. If you do not have a central absorption source there is something seriously wrong with the cube.
+        sf.print_log(f'''PREPROCESSING: Your cube had a significant amount of values below -10*sigma. If you do not have a central absorption source there is something seriously wrong with the cube.
+{"":8s}PREPROCESSING: We blanked these values.
+''',Configuration)
+
+    #Let's make sure that a central absorption source is treated the same regardless od the size of the cube
+    with warnings.catch_warnings():
+        warnings.simplefilter("ignore")
+        buffer=5.*hdr['BMAJ']/np.mean([abs(hdr['CDELT1']),abs(hdr['CDELT2'])])
+        central = data[:,int(hdr['NAXIS2']/2.-buffer):int(hdr['NAXIS2']/2.+buffer),\
+                        int(hdr['NAXIS1']/2.-buffer):int(hdr['NAXIS1']/2.+buffer)]
+
+        central_noise_indices = np.where(central < -10*noise_corner)
+    if len(central_noise_indices) > 0.0001*4*buffer*hdr['NAXIS3']:
+        central[central_noise_indices] = float('NaN')
+        data[:,int(hdr['NAXIS2']/2.-buffer):int(hdr['NAXIS2']/2.+buffer),\
+                        int(hdr['NAXIS1']/2.-buffer):int(hdr['NAXIS1']/2.+buffer)] =\
+                        central
+        sf.print_log(f'''PREPROCESSING: Your cube had a significant amount of values below -10*sigma. If you do not have a central absorption source there is something seriously wrong with the cube.
 {"":8s}PREPROCESSING: We blanked these values.
-''',Configuration['OUTPUTLOG'])
+''',Configuration)
+
 
     # Check whether any channels got fully blanked
     blanked_channels = []
     for z in range(hdr['NAXIS3']):
         if np.isnan(data[z,:,:]).all():
             blanked_channels.append(str(z))
     if len(blanked_channels) == 0.:
         blanked_channels = ['-1']
     hdr['BL_CHAN'] = ','.join(blanked_channels)
     #Previously SoFiA was not dealing with blanks properly and the statement went here
+    #finally we want to get the noise level from the negative in the final cube
+
+    new_noise = np.nanstd(np.hstack([data[data<0],-1.*data[data<0]]))
+    #If we have noiseles cubes this will be far to low
+    if abs(new_noise/np.mean([channel_noise,noise_corner])) > 4. \
+        or abs(new_noise/np.mean([channel_noise,noise_corner])) < 0.25:
+            sf.print_log(f'''PREPROCESSING: There is something odd in the noise statistics of your cube. We are not using the nehgative values
+''',Configuration)
+            #new_noise = np.mean([channel_noise,noise_corner])
+    hdr['FATNOISE'] = new_noise
 
     return data
 prep_cube.__doc__ =f'''
  NAME:
     prep_cube
 
  PURPOSE:
@@ -601,56 +624,55 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     hdr = header to be cleaned
     data = data array to be cleaned
 
  OPTIONAL INPUTS:
-    debug = False
 
  OUTPUTS:
     the updated header
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 #Create an optimized cube if required
-def optimized_cube(Configuration,Fits_Files, debug = False):
+def optimized_cube(Configuration,Fits_Files):
     pix_per_beam = Configuration['BEAM_IN_PIXELS'][1]
     if pix_per_beam > Configuration['OPT_PIXEL_BEAM']:
         cube = fits.open(Configuration['FITTING_DIR']+Fits_Files['FITTING_CUBE'])
         data = cube[0].data
         hdr = cube[0].header
         if f"{abs(hdr['CDELT1']):.16f}" != f"{abs(hdr['CDELT2']):.16f}":
-            print_log(f'''OPTIMIZED_CUBE: Your input cube does not have square pixels.
+            sf.print_log(f'''OPTIMIZED_CUBE: Your input cube does not have square pixels.
 {"":8s}OPTIMIZED_CUBE: FAT cannot optimize your cube.
-''', Configuration['OUTPUTLOG'])
+''', Configuration)
         cube.close()
         required_cdelt = hdr['BMIN']/int(Configuration['OPT_PIXEL_BEAM'])
         ratio = required_cdelt/abs(hdr['CDELT2'])
         opt_data,opt_hdr = regrid_cube(data, hdr, ratio)
 
         fits.writeto(Configuration['FITTING_DIR']+Fits_Files['OPTIMIZED_CUBE'], opt_data,opt_hdr)
 
         Configuration['OPTIMIZED'] = True
-        print_log(f'''OPTIMIZED_CUBE: Your input cube has {pix_per_beam} pixels along the minor FWHM.
+        sf.print_log(f'''OPTIMIZED_CUBE: Your input cube has {pix_per_beam} pixels along the minor FWHM.
 {"":8s}OPTIMIZED_CUBE: You requested { Configuration['OPT_PIXEL_BEAM']} therefore we regridded the cube into a new cube.
 {"":8s}OPTIMIZED_CUBE: We are using the pixel size of {required_cdelt}.
-''', Configuration['OUTPUTLOG'])
+''', Configuration)
 
     else:
-        print_log(f'''OPTIMIZED_CUBE: Your input cube has {pix_per_beam} pixels along the minor FWHM.
+        sf.print_log(f'''OPTIMIZED_CUBE: Your input cube has {pix_per_beam} pixels along the minor FWHM.
 {"":8s}OPTIMIZED_CUBE: You requested {Configuration['OPT_PIXEL_BEAM']} but we cannot improve the resolution.
 {"":8s}OPTIMIZED_CUBE: We are using the pixel size of the original cube.
-''', Configuration['OUTPUTLOG'])
+''', Configuration)
 optimized_cube.__doc__ =f'''
  NAME:
     optimized_cube
 
  PURPOSE:
     Check the amount of pixels that are in the minor axis FWHM,
     if more than OPT_PIXELBEAM regrid the cube to less pixels
@@ -660,46 +682,47 @@
     fits_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
 
  OPTIONAL INPUTS:
-    debug = False
 
  OUTPUTS:
     An optimized cube is created and written to disk.
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 def make_moments(Configuration,Fits_Files,fit_type = 'Undefined',
                  moments = [0,1,2],overwrite = False, level=None,
-                  vel_unit= None, debug = False):
+                  vel_unit= None):
+    sf.print_log(f'''MAKE_MOMENTS: We are starting to create the moment maps.
+''',Configuration, case = ['debug_start'])
     if fit_type == 'Generic_Initialize':
         filename = f"{Configuration['FITTING_DIR']}{Fits_Files['FITTING_CUBE']}"
         basename = f"{Configuration['BASE_NAME']}"
         directory = f"{Configuration['FITTING_DIR']}/Sofia_Output/"
-        mask_cube = f"{Configuration['FITTING_DIR']}/Sofia_Output/{Fits_Files['MASK']}"
+        mask_cube = f"{Configuration['FITTING_DIR']}/{Fits_Files['MASK']}"
     elif fit_type == 'Generic_Final':
         filename = f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel.fits"
         basename = 'Finalmodel'
         directory = f"{Configuration['FITTING_DIR']}/Finalmodel/"
-        mask_cube = f"{Configuration['FITTING_DIR']}/Sofia_Output/{Fits_Files['MASK']}"
+        mask_cube = f"{Configuration['FITTING_DIR']}/{Fits_Files['MASK']}"
     else:
         filename = f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.fits"
         basename = fit_type
         directory = f"{Configuration['FITTING_DIR']}{fit_type}"
         if not level:
-            mask_cube = f"{Configuration['FITTING_DIR']}/Sofia_Output/{Fits_Files['MASK']}"
+            mask_cube = f"{Configuration['FITTING_DIR']}/{Fits_Files['MASK']}"
 
     cube = fits.open(filename)
     if vel_unit:
         cube[0].header['CUNIT3'] = vel_unit
     if mask_cube:
         mask = fits.open(mask_cube)
         with np.errstate(invalid='ignore', divide='ignore'):
@@ -708,24 +731,24 @@
     else:
         if not level:
             level = 3.*np.mean([np.nanstd(cube[0].data[0:2,:,:]),np.nanstd(cube[0].data[-3:-1,:,:])])
         with np.errstate(invalid='ignore', divide='ignore'):
             cube[0].data[cube[0].data < level] = float('NaN')
     try:
         if cube[0].header['CUNIT3'].lower().strip() == 'm/s':
-            print_log(f"We convert your m/s to km/s", Configuration['OUTPUTLOG'])
+            sf.print_log(f"MAKE_MOMENTS: We convert your m/s to km/s. \n", Configuration, case=['verbose'])
             cube[0].header['CUNIT3'] = 'km/s'
             cube[0].header['CDELT3'] = cube[0].header['CDELT3']/1000.
             cube[0].header['CRVAL3'] = cube[0].header['CRVAL3']/1000.
         elif cube[0].header['CUNIT3'].lower().strip() == 'km/s':
             pass
         else:
-            print_log(f"Your Velocity unit {cube[0].header['CUNIT3']} is weird. Your units could be off", Configuration['OUTPUTLOG'])
+            sf.print_log(f"MAKE_MOMENTS: Your Velocity unit {cube[0].header['CUNIT3']} is weird. Your units could be off", Configuration)
     except KeyError:
-        print_log(f"Your CUNIT3 is missing, that is bad practice. We'll add a blank one but we're not guessing the value", Configuration['OUTPUTLOG'])
+        sf.print_log(f"MAKE_MOMENTS: Your CUNIT3 is missing, that is bad practice. We'll add a blank one but we're not guessing the value", Configuration)
         cube[0].header['CUNIT3'] = 'Unknown'
     #Make a 2D header to use
     hdr2D = copy.deepcopy(cube[0].header)
     hdr2D.remove('NAXIS3')
     hdr2D['NAXIS'] = 2
     # removing the third axis means we cannot correct for varying platescale, Sofia does so this is and issue so let's not do this
     hdr2D.remove('CDELT3')
@@ -735,38 +758,56 @@
     hdr2D.remove('CRVAL3')
 
     # we need a moment 0 for the moment 2 as well
     if 0 in moments:
         hdr2D['BUNIT'] = f"{cube[0].header['BUNIT']}*{cube[0].header['CUNIT3']}"
         moment0 = np.nansum(cube[0].data, axis=0) * cube[0].header['CDELT3']
         moment0[np.invert(np.isfinite(moment0))] = float('NaN')
-        hdr2D['DATAMAX'] = np.nanmax(moment0)
-        hdr2D['DATAMIN'] = np.nanmin(moment0)
-        fits.writeto(f"{directory}/{basename}_mom0.fits",moment0,hdr2D,overwrite = overwrite)
+        try:
+            hdr2D['DATAMAX'] = np.nanmax(moment0)
+            hdr2D['DATAMIN'] = np.nanmin(moment0)
+            fits.writeto(f"{directory}/{basename}_mom0.fits",moment0,hdr2D,overwrite = overwrite)
+        except ValueError:
+            sf.print_log(f"MAKE_MOMENTS: Your Moment 0 has bad data and we could not write the moment 0 fits file", Configuration)
+
+
+        
     if 1 in moments or 2 in moments:
         zaxis = cube[0].header['CRVAL3'] + (np.arange(cube[0].header['NAXIS3'])+1 \
               - cube[0].header['CRPIX3']) * cube[0].header['CDELT3']
         c=np.transpose(np.resize(zaxis,[cube[0].header['NAXIS1'],cube[0].header['NAXIS2'],len(zaxis)]),(2,1,0))
         hdr2D['BUNIT'] = f"{cube[0].header['CUNIT3']}"
         # Remember Python is stupid so z,y,x
         with np.errstate(invalid='ignore', divide='ignore'):
             moment1 = np.nansum(cube[0].data*c, axis=0)/ np.nansum(cube[0].data, axis=0)
         moment1[np.invert(np.isfinite(moment1))] = float('NaN')
-        hdr2D['DATAMAX'] = np.nanmax(moment1)
-        hdr2D['DATAMIN'] = np.nanmin(moment1)
-        if 1 in moments:
-            fits.writeto(f"{directory}/{basename}_mom1.fits",moment1,hdr2D,overwrite = overwrite)
+        try:
+            hdr2D['DATAMAX'] = np.nanmax(moment1)
+            hdr2D['DATAMIN'] = np.nanmin(moment1)
+            if 1 in moments:
+                fits.writeto(f"{directory}/{basename}_mom1.fits",moment1,hdr2D,\
+                    overwrite = overwrite)
+
+        except ValueError:
+            sf.print_log(f"MAKE_MOMENTS: Your Moment 1 has bad data and we could not write the moment 0 fits file", Configuration)
+
         if 2 in moments:
             d = c - np.resize(moment1,[len(zaxis),cube[0].header['NAXIS2'],cube[0].header['NAXIS1']])
             with np.errstate(invalid='ignore', divide='ignore'):
                 moment2 = np.sqrt(np.nansum(cube[0].data*d**2, axis=0)/ np.nansum(cube[0].data, axis=0))
             moment2[np.invert(np.isfinite(moment1))] = float('NaN')
-            hdr2D['DATAMAX'] = np.nanmax(moment2)
-            hdr2D['DATAMIN'] = np.nanmin(moment2)
-            fits.writeto(f"{directory}/{basename}_mom2.fits",moment2,hdr2D,overwrite = overwrite)
+            try:
+                hdr2D['DATAMAX'] = np.nanmax(moment2)
+                hdr2D['DATAMIN'] = np.nanmin(moment2)
+                fits.writeto(f"{directory}/{basename}_mom2.fits",\
+                    moment2,hdr2D,overwrite = overwrite)
+
+            except ValueError:
+                sf.print_log(f"MAKE_MOMENTS: Your Moment 1 has bad data and we could not write the moment 0 fits file", Configuration)
+
     cube.close()
 
 make_moments.__doc__ =f'''
  NAME:
     make_moments
 
  PURPOSE:
@@ -777,16 +818,14 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
 
 
  OPTIONAL INPUTS:
-    debug = False
-
     fit_type = 'Undefined'
     type of ftting
 
     moments = [0,1,2]
     moment maps to create
 
     overwrite = False
@@ -823,28 +862,28 @@
     regrid_hdr['CRPIX1'] =   (regrid_hdr['CRPIX1']-1)/real_ratio[2]+1
     regrid_hdr['CRPIX2'] =   (regrid_hdr['CRPIX2']-1)/real_ratio[1]+1
     wcs_found = False
     try:
         regrid_hdr['CDELT1'] =   regrid_hdr['CDELT1']*real_ratio[2]
         regrid_hdr['CDELT2'] =   regrid_hdr['CDELT2']*real_ratio[1]
         wcs_found = True
-    except:
+    except KeyError:
         print("No CDELT found")
     try:
         regrid_hdr['CD1_1'] =   regrid_hdr['CD1_1']*real_ratio[2]
         regrid_hdr['CD2_2'] =   regrid_hdr['CD2_2']*real_ratio[1]
         wcs_found = True
-    except:
+    except KeyError:
         if not wcs_found:
             print("No CD corr matrix found")
     try:
         regrid_hdr['CD1_2'] =   regrid_hdr['CD1_2']*real_ratio[2]
         regrid_hdr['CD2_1'] =   regrid_hdr['CD2_1']*real_ratio[1]
         wcs_found = True
-    except:
+    except KeyError:
         if not wcs_found:
             print("No CD cross-corr matrix found")
 
     regrid_hdr['NAXIS1'] =   new_shape[2]
     regrid_hdr['NAXIS2'] =   new_shape[1]
     return regrid_data,regrid_hdr
 regrid_cube.__doc__ =f'''
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/Support/modify_template.py` & `pyFAT_astro-0.1.1/pyFAT_astro/Support/modify_template.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,125 @@
 # -*- coding: future_fstrings -*-
 # This module contains a set of functions and classes that are used to Modify the Tirific_Template
 
 
 
 import copy
-from pyFAT_astro.Support.support_functions import set_rings,convertskyangle,sbr_limits,set_limits,print_log,set_limit_modifier,\
-                              set_ring_size,calc_rings,finish_current_run,set_format,get_from_template,gaussian_function,fit_gaussian,\
-                              get_ring_weights,set_boundaries
-from pyFAT_astro.Support.fat_errors import InitializeError,CfluxError,FunctionCallError,BadConfigurationError
+
+from pyFAT_astro.Support.fat_errors import InitializeError,CfluxError,\
+    FunctionCallError,BadConfigurationError,FittingError,FaintSourceError
+import pyFAT_astro.Support.support_functions as sf
+import pyFAT_astro
+
 import numpy as np
 import os
-from scipy.optimize import curve_fit
+import warnings
+from scipy.optimize import curve_fit, OptimizeWarning
 from scipy.signal import savgol_filter
 from scipy.interpolate import CubicSpline,Akima1DInterpolator
 
 
-def arc_tan_function(axis,center,length,amplitude,mean):
+
+def apply_new_size(Configuration, new_size ):
+    ''' Check whether we want to apply our new size '''
+    # we want to have at least a quarter beam difference to apply the size.
+
+    difference = [abs(Configuration['SIZE_IN_BEAMS'][x]-new_size[x]) for x in [0,1]]
+
+
+    if all([(x < Configuration['RING_SIZE']/2.) for x in difference]):
+        sf.print_log(f'''APPLY_NEW_SIZE: The new sizes equal those of the previous fit. Not changing
+''', Configuration,case=['verbose'])
+        return False
+    sf.print_log(f'''APPLY_NEW_SIZE: The new sizes differ from those of the previous fit.
+''', Configuration,case=['verbose'])
+    for i in [0,1]:
+        for sizes in Configuration['OLD_SIZE'][:-1]:
+            if abs(sizes[i] - new_size[i]) < Configuration['RING_SIZE']/2.:
+                sf.print_log(f'''APPLY_NEW_SIZE: The side {i} has been fitted before fixing it.
+''', Configuration,case=['verbose'])
+                Configuration['FIX_SIZE'][i] = True
+    return True
+apply_new_size.__doc__ =f'''
+ NAME:
+    apply new size
+
+ PURPOSE:
+    determine whether the newly calculated size should be written to the configuration
+    by comparing to previous sizes
+
+ CATEGORY:
+    modify_template
+
+ INPUTS:
+    Configuration = Standard configuration Dictionary
+    new_size = the new sizes to check
+
+ OPTIONAL INPUTS:
+
+ OUTPUTS:
+    boolean
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+
+
+def arc_tan_sdis_function(axis,center,length,amplitude,mean):
     # to prevent instant turnover
     c = axis[-1]*0.1
     #and the turnover has to be beyon 20*of the inner part
-    c2 = set_limits(axis[-1]*0.2,axis[2],axis[int(len(axis)/1.5)])
-    return -1*np.arctan((axis-(c2+abs(center)))/(c+abs(length)))*amplitude/np.pi + mean
+    c2 = sf.set_limits(axis[-1]*0.2,axis[2],axis[int(len(axis)/1.5)])
+    return -1*np.arctan((axis-(c2+abs(center)))/(c+abs(length)))*abs(amplitude)/np.pi + abs(mean)
+arc_tan_sdis_function.__doc__ =f'''
+ NAME:
+    arc_tan_function
+
+ PURPOSE:
+    arc tangent function for fitting the SDIS this one can only be declining
+
+ CATEGORY:
+    modify_template
+
+ INPUTS:
+    axis = xaxis
+    center = 0 point of the acrtan
+    length = turnover length
+    amplitude = height of the arctan
+    mean = amplitude zero point
+
+ OPTIONAL INPUTS:
+
+ OUTPUTS:
+    arctan function
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+
+def arc_tan_function(axis,center,length,amplitude,mean):
+    # to prevent instant turnover
+    c = axis[-1]*0.2
+    #and the turnover has to be beyon 20*of the inner part
+    c2 = sf.set_limits(axis[-1]*0.2,axis[2],axis[int(len(axis)/1.5)])
+    return np.arctan((axis-(c2+abs(center)))/(c+abs(length)))*amplitude/np.pi + abs(mean)
 arc_tan_function.__doc__ =f'''
  NAME:
     arc_tan_function
 
  PURPOSE:
-    arc tangent function
+    arc tangent function that can be declining or increain
 
  CATEGORY:
     modify_template
 
  INPUTS:
     axis = xaxis
     center = 0 point of the acrtan
@@ -47,29 +136,275 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def check_angles(Configuration,Tirific_Template, debug = False):
-    incl = get_from_template(Configuration,Tirific_Template, ['INCL','INCL_2'],debug=debug)
+def calc_new_size(Configuration,Tirific_Template,radii,sbr_in,sbr_ring_limits ):
+
+    sbr=copy.deepcopy(sbr_in)
+
+    for i in [0,1]:
+        if sbr[i,-1] > 5*  sbr[i,-2]:
+              sbr[i,-1]= 0.8*sbr[i,-2]
+
+    sm_sbr = smooth_profile(Configuration,Tirific_Template,'SBR',
+                            min_error= sbr_ring_limits,no_apply = True,
+                            fix_sbr_call = True, profile_in = sbr )
+    old_size = copy.deepcopy(Configuration['SIZE_IN_BEAMS'])
+    new_size = copy.deepcopy(Configuration['SIZE_IN_BEAMS'])
+    difference_with_limit = np.array(sbr-sbr_ring_limits,dtype=float)
+    smooth_diff = smooth_profile(Configuration,{'EMPTY':None}, 'ARBITRARY' ,\
+        profile_in=difference_with_limit, min_error=[0.,0.],no_fix=True,no_apply=True)
+    sf.print_log(f'''CALC_NEW_SIZE: We find the following smoothed difference profile:
+{'':8s} smooth_diff = {smooth_diff}
+''',Configuration,case=['debug_start'])
+    for i in [0,1]:
+        #If all last three values are above the limit we need to extend
+        if np.all(smooth_diff[i,-3:] > 0.):
+            #We fit a Gaussian to the SBR and see where it drops below the last SBR Limit
+            try:
+                vals = sf.fit_gaussian(Configuration,radii,sm_sbr[i,:],errors=sbr_ring_limits[i,:])
+                extend_radii = np.linspace(0.,Configuration['MAX_SIZE_IN_BEAMS']*Configuration['BEAM'][0],1000)
+                Gauss_diff = sf.gaussian_function(extend_radii,*vals)-sbr_ring_limits[i,-1]
+                this_size=sf.set_limits(extend_radii[np.where(Gauss_diff < 0.)[0][0]]/Configuration['BEAM'][0]+0.5, Configuration['MIN_SIZE_IN_BEAMS'], Configuration['MAX_SIZE_IN_BEAMS'])
+            except FittingError:
+                #If we cannot fit a gaussian we extend by a beam
+                this_size=sf.set_limits(radii[-1]/Configuration['BEAM'][0]+1.0, Configuration['MIN_SIZE_IN_BEAMS'], Configuration['MAX_SIZE_IN_BEAMS'])
+            except IndexError:
+                #If we do not find any values in the gaussian below the limits we extend 2 beams
+                this_size=sf.set_limits(radii[-1]/Configuration['BEAM'][0]+2.0, Configuration['MIN_SIZE_IN_BEAMS'], Configuration['MAX_SIZE_IN_BEAMS'])
+
+            if this_size > new_size[i]+0.5:
+                new_size[i]= copy.deepcopy(this_size)
+        else:
+            #we need to find where we cross the zero line
+            #but have to make sure it is the first from the end
+            loc = 0
+            counter = len(smooth_diff[i,:])-1
+            while loc == 0:
+                if smooth_diff[i,counter-1] < 0. and counter > 1:
+                    counter -= 1
+                else:
+                    if counter < 1:
+                        loc = 1
+                    else:
+                        loc = counter
+            x1 = float(radii[loc-1])
+            x2 = float(radii[loc])
+            y1 = float(smooth_diff[i,loc-1])
+            y2 = float(smooth_diff[i,loc])
+            this_size = sf.set_limits((x1+y1*(x2-x1)/(y1-y2))/Configuration['BEAM'][0],Configuration['MIN_SIZE_IN_BEAMS'], Configuration['MAX_SIZE_IN_BEAMS'])
+
+
+            sf.print_log(f'''CALC_NEW_SIZE: The profile for {i} drop below 0. between {x1} and {x2}.
+{'':8s} with y1 = {y1} and y2 = {y2}
+{'':8s} the new size is {this_size}
+''',Configuration,case= ['debug_add'])
+            if this_size < new_size[i]-0.5:
+                new_size[i]= copy.deepcopy(this_size)
+        if Configuration['FIX_RING_SIZE']:
+            real_size = new_size[i]-1./5.
+            rings = int(real_size/Configuration['RING_SIZE'])
+            new_size[i] = rings * Configuration['RING_SIZE']+1./5.
+        if new_size[i] < Configuration['TOO_SMALL_GALAXY']:
+             new_size[i] = Configuration['TOO_SMALL_GALAXY']
+
+    sf.print_log(f'''CALC_NEW_SIZE: We have the new_size {new_size} compared to what we had before {old_size}
+''',Configuration,case = ['debug_add'])
+
+    return new_size
+calc_new_size.__doc__ =f'''
+ NAME:
+    calc_new_size
+
+ PURPOSE:
+    Based on the current SBR profiles and sbr_limits calc ulate the size of the galaxy
+
+ CATEGORY:
+    modify_template
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    radii = The current radii of the model
+    sbr = The current sbr of the model (Both sides)
+    sbr_ring_limits = The current sbr limits
+
+ OPTIONAL INPUTS:
+
+
+ OUTPUTS:
+    new_size
+    a 2 element array indicating the new size for both sides of the model
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+NOTE:
+    The new size is neveer applied to Configuration
+'''
+
+def calculate_change_boundary(Configuration,multiple_used,theta_zero,phi_zero ):
+    change_boundary = []
+    for i in range(3):
+        if i == 0:
+            multiple=multiple_used[0]
+        else:
+            multiple=multiple_used[i-1]
+        poss_theta_bound= []
+        poss_phi_bound = []
+        #we need theta and phi for all options of PA and INCL
+        pa_lim= [Configuration['PA_CURRENT_BOUNDARY'][i][0],\
+                Configuration['PA_CURRENT_BOUNDARY'][i][0],\
+                Configuration['PA_CURRENT_BOUNDARY'][i][1],\
+                Configuration['PA_CURRENT_BOUNDARY'][i][1]]
+        incl_lim = [Configuration['INCL_CURRENT_BOUNDARY'][i][0],\
+                Configuration['INCL_CURRENT_BOUNDARY'][i][1],\
+                Configuration['INCL_CURRENT_BOUNDARY'][i][0],\
+                Configuration['INCL_CURRENT_BOUNDARY'][i][1]]
+        for x,y in zip(pa_lim,incl_lim):
+            theta_tmp,phi_tmp,multiple_tmp = sf.calculate_am_vector(Configuration,[x],[y])
+            # if the multiples do not correspond in the vector can be infinite
+
+            if multiple_tmp[0] != multiple:
+                poss_theta_bound.append(float('NaN'))
+                poss_phi_bound.append(float('NaN'))
+            else:
+                poss_theta_bound.append(float(theta_tmp))
+                poss_phi_bound.append(float(phi_tmp))
+        minimum = -1*np.sqrt(np.min(np.array([x-theta_zero[0] for x in poss_theta_bound],dtype=float))**2\
+                            +np.min(np.array([x-phi_zero[0] for x in poss_phi_bound],dtype=float))**2)
+        maximum = np.sqrt(np.max(np.array([x-theta_zero[0] for x in poss_theta_bound],dtype=float))**2\
+                            +np.max(np.array([x-phi_zero[0] for x in poss_phi_bound],dtype=float))**2)
+        if np.isnan(minimum):
+            minumum = 0.
+        if np.isnan(maximum):
+            maximum = 0.
+        change_boundary.append([minimum,maximum])
+    return change_boundary
+
+calculate_change_boundary.__doc__ =f'''
+ NAME:
+    calculate_change_boundary
+
+ PURPOSE:
+    when regularising the PA and incl we do this through the change in the am vector
+    but it should still maintain within the boundary limit this calculates the boundary
+    limits for the change vector
+
+ CATEGORY:
+    modify_template
+
+ INPUTS:
+    Configuration = Configuration
+    pa_incl =  array with PA, PA_2,INCL,INCL_2
+    theta_zero = the centra theta value
+    phi_zero = the central phi value
+
+
+ OPTIONAL INPUTS:
+
+
+ OUTPUTS:
+    boundaries that the for the combined theta and phi change cannot cross
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+
+
+def check_angles(Configuration,Tirific_Template):
+    changed_angles=False
+    incl_in = sf.load_tirific(Configuration,Tirific_Template,Variables= ['INCL','INCL_2'])
+    pa_in = sf.load_tirific(Configuration,Tirific_Template,Variables= ['PA','PA_2'])
+    incl = copy.deepcopy(incl_in)
+    pa = copy.deepcopy(pa_in)
+    rad =[float(x) for x in Tirific_Template['RADI'].split()]
+
+    sf.print_log(f'''CHECK_ANGLES: We start with
+{'':8s} radius = {rad}
+{'':8s} PA appr = {pa[0]}
+{'':8s} PA rec = {pa[1]}
+{'':8s} INCL appr = {incl[0]}
+{'':8s} INCL rec = {incl[1]}
+{'':8s} Changed_Angle = {changed_angles}
+''', Configuration,case=['debug_start'])
+
+    for side in [0,1]:
+        incl_too_large = (np.array(incl[side],dtype=float) > 90.)
+        if incl_too_large.any():
+
+            sf.print_log(f'''CHECK_ANGLES: Several INCL values were too large
+''', Configuration,case = ['verbose'])
+            incl[side] = [180.-x if y else x for x,y in zip(incl[side],incl_too_large)]
+            #changed_angles = True
+
+        pa_too_large = (np.array(pa[side],dtype=float) > 360.)
+        if pa_too_large.any():
+            if np.mean(np.array(pa[side],dtype=float)[~pa_too_large]) < 180.:
+                pa[side] = [x-360. if y else x for x,y in zip(pa[side],pa_too_large)]
+                #changed_angles = True
+                sf.print_log(f'''CHECK_ANGLES: Several PA values were too large
+''', Configuration,case=['verbose'])
+
+        pa_too_small = (np.array(pa[side],dtype=float) < 0.)
+        if pa_too_small.any():
+            if np.mean(np.array(pa[side],dtype=float)[~pa_too_small]) > 180.:
+                pa[side] = [x+360. if y else x for x,y in zip(pa[side],pa_too_small)]
+                #changed_angles = True
+
+                sf.print_log(f'''CHECK_ANGLES: Several PA values were too small
+''', Configuration,case=['verbose'])
+        pa_tmp,incl_tmp,changed_angles = sf.check_angular_momentum_vector(Configuration,\
+                                            rad,pa[side],incl[side],modified= changed_angles,\
+                                            side=side)
+        #pa_tmp = sf.max_profile_change(Configuration,rad,pa[side],'PA',slope = Configuration['WARP_SLOPE'][side])
+        pa[side] = pa_tmp
+        #incl_tmp = sf.max_profile_change(Configuration,rad,incl[side],'INCL',slope = Configuration['WARP_SLOPE'][side])
+        incl[side] = incl_tmp
+
+        #exit()
+
+    #Ensure that we have not made PA differences
+    if pa[0][0] != pa[1][0]:
+        if abs( pa[0][0]-pa[1][0]) > Configuration['MIN_ERROR']['PA'][0]:
+            sf.print_log(f'''CHECK_ANGLES: The central PA differs by too much:
+{'':8s} differece = { abs( pa[0][0]-pa[1][0])}, max allowed = {Configuration['MIN_ERROR']['PA'][0]}
+    ''', Configuration,case=['verbose'])
+            changed_angles = True
+        else:
+            sf.print_log(f'''CHECK_ANGLES: We correct some computational changes in the PA
+    ''', Configuration,case=['verbose'])
+        if (pa[0][0] > 360. and pa[1][0] < 360.) or \
+            (pa[0][0] < 0. and pa[1][0] > 0.):
+                pa[0][0:3] = pa[1][0:3]
+        elif(pa[0][0] < 360. and pa[1][0] > 360.) or \
+            (pa[0][0] > 0. and pa[1][0] < 0.):
+                pa[1][0:3] = pa[0][0:3]
+
+
+    Tirific_Template['INCL'] = f"{' '.join(f'{x:.2e}' for x in incl[0])}"
+    Tirific_Template['INCL_2'] = f"{' '.join(f'{x:.2e}' for x in incl[1])}"
+    Tirific_Template['PA'] = f"{' '.join(f'{x:.2e}' for x in pa[0])}"
+    Tirific_Template['PA_2'] = f"{' '.join(f'{x:.2e}' for x in pa[1])}"
+    sf.print_log(f'''CHECK_ANGLES: We wrote to the template
+{'':8s} PA appr = {Tirific_Template['PA']}
+{'':8s} PA rec = {Tirific_Template['PA_2']}
+{'':8s} INCL appr = {Tirific_Template['INCL']}
+{'':8s} INCL rec = {Tirific_Template['INCL_2']}
+''', Configuration,case=['verbose'])
+
+    return changed_angles
+
 
-    if incl[0][0] > 90. and incl[1][0] > 90.:
-        Tirific_Template['INCL'] = f"{' '.join(f'{180.-x:.2e}' for x in incl[0])}"
-        Tirific_Template['INCL_2'] = f"{' '.join(f'{180.-x:.2e}' for x in incl[1])}"
-    pa = get_from_template(Configuration,Tirific_Template, ['PA','PA_2'],debug=debug)
-
-    if pa[0][0] > 360. and pa[1][0] > 360.:
-        Tirific_Template['PA'] = f"{' '.join(f'{x-360.:.2e}' for x in pa[0])}"
-        Tirific_Template['PA_2'] = f"{' '.join(f'{x-360.:.2e}' for x in pa[1])}"
-
-    if pa[0][0] < 0. and pa[1][0] < 0.:
-        Tirific_Template['PA'] = f"{' '.join(f'{360.-x:.2e}' for x in pa[0])}"
-        Tirific_Template['PA_2'] = f"{' '.join(f'{360.-x:.2e}' for x in pa[1])}"
 check_angles.__doc__=f'''
  NAME:
     check_angles
 
  PURPOSE:
        Check whether PA and INCLination are in the range 0-360. and < 90 in the center. If not modify all angles such that they are.
 
@@ -77,74 +412,72 @@
        modify_template
 
  INPUTS:
     Configuration  = Standard FAT configuration
     Tirific_Template = Standard FAT Tirific Template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
-    No output Tirific_Template is modified
+    Tirific_Template is modified
+    output is boolean indicating changes were made or not.
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
-      get_from_template, join
+      load_tirific, join
 
  NOTE:
 '''
 
 
-def check_flat(Configuration,profile,error,key, last_reliable_ring = -1,inner_fix = 4, debug = False):
-    if last_reliable_ring == -1:
+def check_flat(Configuration,profile,error,key, last_reliable_ring = -1,inner_fix = 4):
+    if last_reliable_ring == -1 or last_reliable_ring > len(profile)-1:
         last_reliable_ring = len(profile)-1
-    if debug:
-        print_log(f'''CHECK_FLAT: checking flatness
+
+    sf.print_log(f'''CHECK_FLAT: checking flatness
 {'':8s}profile = {profile}
 {'':8s}error = {error}
 {'':8s}last_reliable_ring = {last_reliable_ring}
-''',Configuration['OUTPUTLOG'],debug = True)
+''',Configuration, case= ['debug_start'])
 
     inner = np.mean(profile[:inner_fix])
     mean_error = np.mean(error[:last_reliable_ring])
     if inner_fix+1 < last_reliable_ring:
         outer = np.mean(profile[inner_fix+1:last_reliable_ring])
         outer_std = np.std(profile[inner_fix+1:last_reliable_ring])
     else:
         outer = inner
         outer_std = np.mean(error)
 
     if key in ['SDIS']:
+        mean_error = mean_error*0.5
         outer_std = 2.*mean_error
     if abs(outer-inner) < mean_error or outer_std  < mean_error:
-        if debug:
-            print_log(f'''CHECK_FLAT: If  {abs(outer-inner)} less than {mean_error} or
+        sf.print_log(f'''CHECK_FLAT: If  {abs(outer-inner)} less than {mean_error} or
 {'':8s} The outer variation {outer_std} less than the median error {mean_error} we break and set flat.
-''',Configuration['OUTPUTLOG'])
+''',Configuration, case=['debug_add'])
         return True
     if key in ['INCL','INCL_2']:
         if outer < 40. or inner < 40.:
-            if debug:
-                print_log(f'''CHECK_FLAT: If  the outer profile is {outer} hence we set this to flat.
-''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''CHECK_FLAT: If  the outer profile is {outer} hence we set this to flat.
+''',Configuration, case=['debug_add'])
             return True
 
     for e,x,y in zip(error[1:last_reliable_ring],profile[1:last_reliable_ring],profile[0:last_reliable_ring]):
-        if debug:
-            print_log(f'''CHECK_FLAT: x = {x}, y = {y}, e = {e}
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''CHECK_FLAT: x = {x}, y = {y}, e = {e}
+''',Configuration, case=['debug_add'])
         if not x-e/2. < y < x+e/2.:
-            if debug:
-                print_log(f'''CHECK_FLAT: This taco is bend
-''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''CHECK_FLAT: This taco is bend
+''',Configuration, case=['debug_add'])
             return False
-    if debug:
-            print_log(f'''CHECK_FLAT: All values were within the error of eachother
-''',Configuration['OUTPUTLOG'])
+
+    sf.print_log(f'''CHECK_FLAT: All values were within the error of eachother
+''',Configuration, case=['debug_add'])
     return True
 check_flat.__doc__ = '''
  NAME:
     check_flat
 
  PURPOSE:
        Check whether within its errors a routine is varying compared to the prvious rings
@@ -154,15 +487,15 @@
 
  INPUTS:
     Configuration  = Standard FAT configuration
     profile = the profile to examine
     error = The accompanying error
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     last_reliable_ring = -1
     the last ring in the profile that can be trusted
 
  OUTPUTS:
        True if no variation is found false if variation is found
 
@@ -170,172 +503,96 @@
 
  PROCEDURES CALLED:
       zip(),np.std,np.mean,abs,print_log
 
  NOTE:
 '''
 
-def check_size(Configuration,Tirific_Template, fit_type = 'Undefined', stage = 'initial', Fits_Files= 'No Files' ,debug = False,current_run='Not Initialized'):
-    if debug:
-        print_log(f'''CHECK_SIZE: Starting a new Check_size with the following parameters:
-{'':8s}CHECK_SIZE: Rings = {Configuration['NO_RINGS']}
-{'':8s}CHECK_SIZE: Size in Beams = {Configuration['SIZE_IN_BEAMS']}
-''',Configuration['OUTPUTLOG'],debug=True)
+def check_size(Configuration,Tirific_Template, fit_type = 'Undefined', \
+        stage = 'initial', Fits_Files= 'No Files' ,current_run='Not Initialized',
+        no_apply=False):
 
+    sf.print_log(f'''CHECK_SIZE: Starting check_size with the following parameters:
+{'':8s}Rings = {Configuration['NO_RINGS']}, Size in Beams = {Configuration['SIZE_IN_BEAMS']}
+''',Configuration,case=['debug_start'])
 
-    radii, sbr_ring_limits = sbr_limits(Configuration,systemic = float(Tirific_Template['VSYS'].split()[0]),debug=debug)
+
+    radii, sbr_ring_limits = sf.sbr_limits(Configuration,Tirific_Template)
     #get the sbr profiles
 
-    sbr = np.array(get_from_template(Configuration,Tirific_Template, ['SBR','SBR_2'],debug=debug),dtype = float)
-    if debug:
-        print_log(f'''CHECK_SIZE: This is the sizes
-{'':8s}CHECK_SIZE: SBR = {len(sbr[0])},{len(sbr[1])}
-{'':8s}CHECK_SIZE: limits = {len(sbr_ring_limits)}
-{'':8s}CHECK_SIZE: No. Rings  = {Configuration['NO_RINGS']}
-''',Configuration['OUTPUTLOG'])
+    sbr = sf.load_tirific(Configuration,Tirific_Template,Variables=['SBR','SBR_2'],\
+        array=True)
     if len(sbr[0]) != len(sbr_ring_limits):
         #Check what the appropriate size should be
-        if debug:
-            print_log(f'''CHECK_SIZE: Equalizing the sizes
-''',Configuration['OUTPUTLOG'])
+
+        sf.print_log(f'''CHECK_SIZE: Equalizing the sizes
+''',Configuration,case= ['debug_add'])
         if len(sbr[0]) != Configuration['NO_RINGS']:
-            if debug:
-                print_log(f'''CHECK_SIZE: Interpolating SBR
-''',Configuration['OUTPUTLOG'])
-            old_radii = np.array(get_from_template(Configuration,Tirific_Template, ['RADI'],debug=debug),dtype = float)
+
+            sf.print_log(f'''CHECK_SIZE: Interpolating SBR
+''',Configuration,case= ['debug_add'])
+            old_radii = np.array(sf.load_tirific(Configuration,Tirific_Template, ['RADI']),dtype = float)
             for i in [0,1]:
                 sbr[i] = np.interp(np.array(radii,dtype=float),np.array(old_radii[0],dtype=float),np.array(sbr[i],dtype=float))
-
-    if debug:
-        print_log(f'''CHECK_SIZE: This after correcting.
-{'':8s}CHECK_SIZE: SBR = {len(sbr[0])}
-{'':8s}CHECK_SIZE: limits = {len(sbr_ring_limits)}
-{'':8s}CHECK_SIZE: No. Rings  = {Configuration['NO_RINGS']}
-''',Configuration['OUTPUTLOG'])
+    sf.print_log(f'''CHECK_SIZE: These are the ring SBRs and limits we will use:
+{'':8s}SBR = {sbr}
+{'':8s}limits = {sbr_ring_limits}
+{'':8s}No. Rings  = {Configuration['NO_RINGS']}
+''',Configuration,case= ['debug_add'])
     #sbr_ring_limits = 1.25*np.array([sbr_ring_limits,sbr_ring_limits])
     sbr_ring_limits = np.array([sbr_ring_limits,sbr_ring_limits],dtype=float)
-    new_rings = get_number_of_rings(Configuration,sbr,sbr_ring_limits, debug=debug)
-    # if all of the last points are  below the limit we start checking how far to cut
+
+    #This part has to change in something new
+    size_in_beams = calc_new_size(Configuration,Tirific_Template,radii,sbr,sbr_ring_limits)
+    if not no_apply:
+        apply_size = apply_new_size(Configuration,size_in_beams)
+    else:
+        apply_size = False
+    sf.print_log(f'''CHECK_SIZE: These have been fitted before {Configuration['OLD_SIZE']}
+{'':8s} This is new_size {size_in_beams}, This is what currently is in {Configuration['SIZE_IN_BEAMS']}
+''',Configuration,case= ['debug_add'])
+    if apply_size:
+        Configuration['OLD_SIZE'].append(list(copy.deepcopy(Configuration['SIZE_IN_BEAMS'])))
+        for i in [0,1]:
+            if not Configuration['FIX_SIZE'][i]:
+                Configuration['SIZE_IN_BEAMS'][i] = copy.deepcopy(size_in_beams[i])
+        ring_size, number_of_rings = sf.set_ring_size(Configuration)
+        sf.print_log(f'''CHECK_SIZE: Applied the size of {Configuration['SIZE_IN_BEAMS']}, ring size {ring_size} resulting in {number_of_rings} rings
+''',Configuration,case=['verbose'])
+
+
+    # Set the unreliable parameters
     #the lower the inclination the sooner the RC becomes unreliable
-    limit_factor = set_limits(2.5*np.mean(Configuration['LIMIT_MODIFIER']) ,2.,4.)
-    if debug:
-        print_log(f'''CHECK_SIZE: Using a limit factor for reliable RC of  {limit_factor}
-''',Configuration['OUTPUTLOG'])
-    Configuration['RC_UNRELIABLE'] = get_number_of_rings(Configuration,sbr,limit_factor*sbr_ring_limits, debug=debug)-1
+    limit_factor = sf.set_limits(2.5*np.mean(Configuration['LIMIT_MODIFIER']) ,2.,4.)
+    sf.print_log(f'''CHECK_SIZE: Using a limit factor to calculate where the RC is reliable of  {limit_factor}
+''',Configuration,case= ['debug_add'])
+    Configuration['RC_UNRELIABLE'] = get_number_of_rings(Configuration,sbr,limit_factor*sbr_ring_limits)-1
     if Configuration['RC_UNRELIABLE'] == Configuration['NO_RINGS']:
         Configuration['RC_UNRELIABLE'] -= 1
     for i in [0,1]:
-        corr_val = np.where(sbr[i,2:] > sbr_ring_limits[i,2:])[0]+2
+        corr_val = np.where(sbr[i,2:] > sbr_ring_limits[i,2:]*3.)[0]+2
         if corr_val.size > 0:
             Configuration['LAST_RELIABLE_RINGS'][i] = corr_val[-1]+1
         else:
             Configuration['LAST_RELIABLE_RINGS'][i] = Configuration['NO_RINGS']
-    if debug:
-        print_log(f'''CHECK_SIZE: We set these as the last reliable rings {Configuration['LAST_RELIABLE_RINGS']}
-''',Configuration['OUTPUTLOG'])
-    #if we haven't subtracted we check if we should add
-    if int(new_rings) == int(Configuration['NO_RINGS']):
-        if (np.any(sbr[:,-2] > sbr_ring_limits[:,-2]*7.) and np.any(sbr[:,-1] > sbr_ring_limits[:,-1]*3.)) or \
-            np.any(sbr[:,-1] > sbr_ring_limits[:,-1]*5.):
-            if debug:
-                print_log(f'''CHECK_SIZE: The last rings were found to be:
-{'':8s}{sbr[:,-2:]}
-{'':8s}and the limits:
-{'':8s}{sbr_ring_limits[:,-2:]}
-{'':8s}Thus we add a ring.
-''', Configuration['OUTPUTLOG'])
-            new_rings += 1
-        else:
-            if debug:
-                print_log(f'''CHECK_SIZE: The last rings were found to be:
-{'':8s}{sbr[:,-2:]}
-{'':8s}and the limits:
-{'':8s}{sbr_ring_limits[:,-2:]}
-{'':8s}Thus we keep the ring size.
-''', Configuration['OUTPUTLOG'])
-    else:
-        if debug:
-            print_log(f'''CHECK_SIZE: The last rings were found to be:
-{'':8s}{sbr[:,-2:]}
-{'':8s}and the limits:
-{'':8s}{sbr_ring_limits[:,-2:]}
-{'':8s}Thus we have subtracted a set of rings.
-''', Configuration['OUTPUTLOG'])
 
-    if new_rings <= Configuration['NO_RINGS']:
-        size_in_beams = (radii[new_rings-1]-1./5.*Configuration['BEAM'][0])/Configuration['BEAM'][0]
-    else:
-        size_in_beams = (radii[-1]-1./5.*Configuration['BEAM'][0])/Configuration['BEAM'][0]+Configuration['RING_SIZE']
-    if debug:
-        print_log(f'''CHECK_SIZE: Before checking against the minimum and maximum the size in beams = {size_in_beams}
-''', Configuration['OUTPUTLOG'],debug=True)
-    size_in_beams = set_limits(size_in_beams, Configuration['MIN_SIZE_IN_BEAMS'], Configuration['MAX_SIZE_IN_BEAMS'])
-    # limit between 3 and the maximum allowed from the sofia estimate
-    size_in_beams,ring_size,number_of_rings = set_ring_size(Configuration, size_in_beams=size_in_beams,check_set_rings = True, debug=debug)
-
-    print_log(f'''CHECK_SIZE: We find the following size in beams {size_in_beams:.1f} with size {ring_size:.1f}.
-{'':8s}CHECK_SIZE: The previous iteration had a size of {Configuration['SIZE_IN_BEAMS']:.1f} with rings  {Configuration['RING_SIZE']:.1f} times the beam. .
-{'':8s}CHECK_SIZE: This results in {int(number_of_rings):.1f} rings in the model compared to {int(Configuration['NO_RINGS'])} previously.
-''', Configuration['OUTPUTLOG'],screen=True)
-    if f"{ring_size:.1f}" != f"{Configuration['RING_SIZE']:.1f}":
-        Configuration['NEW_RING_SIZE'] = True
-    else:
-        Configuration['NEW_RING_SIZE'] = False
-    if debug:
-        print_log(f'''CHECK_SIZE: The previous rings were {Configuration['OLD_RINGS']}
-''',Configuration['OUTPUTLOG'])
+    sf.print_log(f'''CHECK_SIZE: We set these as the last reliable rings {Configuration['LAST_RELIABLE_RINGS']}
+{'':8s}The RC is deemed unrliable from ring {Configuration['RC_UNRELIABLE']} on.
+''',Configuration,case= ['debug_add'])
 
-    if f"{size_in_beams:.1f}" == Configuration['OLD_RINGS'][-1]:
-        return True
-    elif f"{size_in_beams:.1f}" in Configuration['OLD_RINGS']:
-        print_log(f'''CHECK_SIZE: We have processed this size before.
-''', Configuration['OUTPUTLOG'])
-        ind = Configuration['OLD_RINGS'].index(f"{size_in_beams:.1f}")
-        if Configuration['OLD_RINGS'][ind+1] > Configuration['OLD_RINGS'][ind]:
-            print_log(f'''CHECK_SIZE: After which we increased the size.
-''', Configuration['OUTPUTLOG'])
-            if Configuration['OLD_RINGS'][ind+1] == Configuration['OLD_RINGS'][-1]:
-                print_log(f'''CHECK_SIZE: Which is the current fit so that's ok.
-''', Configuration['OUTPUTLOG'])
-                return True
-            else:
-                print_log(f'''CHECK_SIZE: Which is not the current fit so we refit this size.
-''', Configuration['OUTPUTLOG'])
-            Configuration['OLD_RINGS'].append(f"{size_in_beams:.1f}")
-        else:
-            print_log(f'''CHECK_SIZE: After which we decreased so we allow this addition. But no more.
-''', Configuration['OUTPUTLOG'])
-            Configuration['OLD_RINGS'].append(f"{size_in_beams:.1f}")
-    else:
-        if debug:
-            print_log(f'''CHECK_SIZE: Adding the new ring size to OLD_RINGS.
-''', Configuration['OUTPUTLOG'])
-        Configuration['OLD_RINGS'].append(f"{size_in_beams:.1f}")
-
-    Configuration['RING_SIZE'] = ring_size
-    Configuration['SIZE_IN_BEAMS'] = size_in_beams
-    Configuration['NO_RINGS'] = calc_rings(Configuration,debug=debug)
-    print_log(f'''CHECK_SIZE: We need to modify the number of rings in the model.
-''', Configuration['OUTPUTLOG'],screen=True)
-
-    if Configuration['RC_UNRELIABLE'] > Configuration['NO_RINGS']:
-        Configuration['RC_UNRELIABLE'] = Configuration['NO_RINGS']
-    for i in [0,1]:
-        if Configuration['LAST_RELIABLE_RINGS'][i] > Configuration['NO_RINGS']:
-            Configuration['LAST_RELIABLE_RINGS'][i] = Configuration['NO_RINGS']
-    if debug:
-        print_log(f'''CHECK_SIZE: We trust the RC upto ring {Configuration['RC_UNRELIABLE']}
-{'':8s} and the rings in general upto {Configuration['LAST_RELIABLE_RINGS']}
-''',Configuration['OUTPUTLOG'])
-    if Fits_Files == 'No Files':
-        raise InitializeError('CHECK_SIZE: Trying to adapt the model size but the fits files were not provided.')
-    else:
+    if apply_size:
         # Do not move this from here else other routines such as sbr_limits are messed up
-        set_new_size(Configuration,Tirific_Template,Fits_Files,fit_type= fit_type, stage = stage ,debug = debug,current_run = current_run)
-    return False
+        set_new_size(Configuration,Tirific_Template,fit_type= fit_type\
+            ,current_run = current_run)
+        set_overall_parameters(Configuration, Fits_Files,Tirific_Template ,fit_type=fit_type)
+        return False
+    elif no_apply:
+        return False
+    else:
+        return True
 check_size.__doc__  =f'''
  NAME:
     check_size
 
  PURPOSE:
     Check and update the size of the model. Update RC_UNRELIABLE and LAST_RELIABLE_RINGS
 
@@ -343,15 +600,15 @@
     modify_template
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = Standard FAT Tirific Template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     fit_type = 'Undefined'
     type of fitting
 
     stage = 'initial'
     Stage of the fitting process
 
@@ -367,37 +624,147 @@
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE: Configuration['RC_UNRELIABLE'] = modified and updated here.
 '''
+def check_for_ring_addition(Configuration,Tirific_Template,sbr,sbr_ring_limits ):
+    new_rings = Configuration['NO_RINGS']
+    if Configuration['OUTER_RINGS_DOUBLED']:
+        factors = [[10.,3.],[7.5,4.],[6.]]
+    else:
+        if Configuration['NO_RINGS'] <= 8:
+            factors = [[5.,1.],[4.,2.],[3.]]
+        elif Configuration['NO_RINGS'] <= 12:
+            factors = [[5.5,1.5],[4.5,2.5],[3.5]]
+        else:
+            factors = [[6.,2.],[5.,3.],[4]]
+    add = False
+    for side in [0,1]:
+        if (sbr[side,-2] > sbr_ring_limits[side,-2]*factors[0][0] and sbr[side,-1] > sbr_ring_limits[side,-1]*factors[0][1]) or \
+            (sbr[side,-2] > sbr_ring_limits[side,-2]*factors[1][0] and sbr[side,-1] > sbr_ring_limits[side,-1]*factors[1][1]) or \
+            sbr[side,-1] > sbr_ring_limits[side,-1]*factors[2][0]:
+            sf.print_log(f'''CHECK_FOR_RING_ADDITION: Checking side {side}:
+{'':8s}{sbr[side,-2:]}
+{'':8s}and the limits:
+{'':8s}{sbr_ring_limits[side,-2:]}
+{'':8s}Thus we check for gaps.
+''', Configuration,case= ['debug_start'])
+
+
+            rad= np.array(sf.load_tirific(Configuration,Tirific_Template, [f'RADI']),dtype = float)
+
+            gap= np.where(sbr[side] < sbr_ring_limits[side])[0]
+            if gap.size > 0:
+                if gap[-1] == len(sbr[side])-1:
+                    sf.print_log(f'''CHECK_FOR_RING_ADDITION: We found a gap (ring = {', '.join([str(x+1) for x in gap])}) that runs to the last ring.
+{'':8s} Not adding based on this side.
+''', Configuration,case= ['debug_add'])
+                    continue
+                while gap[0] < int(len(sbr[side])/2.):
+                    gap = gap[1:]
+                    if len(gap) == 0:
+                        break
+
+            if gap.size > 0:
+                sf.print_log(f'''CHECK_FOR_RING_ADDITION: We found a gap in the rings {',  '.join([str(x+1) for x in gap])}.
+{'':8s}{sbr[side]}
+{'':8s}We will check the change in PA and INCLINATION.
+''', Configuration,case= ['debug_add'])
+                ext = ''
+                if side == 1:
+                    ext='_2'
+                angles = sf.load_tirific(Configuration,Tirific_Template,\
+                    Variables=[f'PA{ext}',f'INCL{ext}'],array=True)
+                PA_change =  np.sum(np.array([np.abs(x-y) for x,y in zip(angles[0,gap[0]-1:],angles[0,gap[0]:])]))
+                INCL_change = np.sum(np.array([np.abs(x-y) for x,y in zip(angles[1,gap[0]-1:],angles[1,gap[0]:])]))
+
+                gap_size = sf.convertskyangle(Configuration,[rad[gap[0]],rad[-1]])
+
+                sf.print_log(f'''CHECK_FOR_RING_ADDITION: We found a gap {[rad[gap[0]],rad[-1]]} arcsec = {gap_size} kpc
+{'':8s}PA variation = {[np.abs(x-y) for x,y in zip(angles[0,gap[0]-1:],angles[0,gap[0]:])]}
+{'':8s}INCL variation = {[np.abs(x-y) for x,y in zip(angles[1,gap[0]-1:],angles[1,gap[0]:])]}
+''', Configuration,case= ['debug_add'])
+                gap_size = float(gap_size[1]-gap_size[0])
+                if PA_change/gap_size  < Configuration['MAX_CHANGE']['PA'] and INCL_change/gap_size < Configuration['MAX_CHANGE']['INCL']:
+                    add = True
+                sf.print_log(f'''CHECK_FOR_RING_ADDITION: We found a change  of {PA_change/gap_size} in PA and {INCL_change/gap_size} in INCL.
+{'':8s} The gap is {gap_size} kpc
+''', Configuration,case= ['debug_add'])
+
+
+            else:
+                sf.print_log(f'''CHECK_FOR_RING_ADDITION: We did not find a gap so we were are adding.
+''', Configuration,case= ['debug_add'])
+                add=True
 
 
-def fit_arc(Configuration,radii,sm_profile,error, debug = False ):
+    if add:
+        sf.print_log(f'''CHECK_FOR_RING_ADDITION:  We are adding a ring (new no ring = {new_rings+1.})
+''', Configuration,case= ['verbose'])
+        new_rings += 1
+    else:
+        sf.print_log(f'''CHECK_FOR_RING_ADDITION: The last rings were found to be:
+{'':8s}{sbr[:,-2:]}
+{'':8s}and the limits:
+{'':8s}{sbr_ring_limits[:,-2:]}
+{'':8s}Thus we keep the ring size.
+''', Configuration,case=['debug_add'])
+    return new_rings
 
-    c2 = set_limits(radii[-1]*0.2,radii[2],radii[int(len(radii)/1.5)])
+def fit_arc(Configuration,radii,sm_profile,error, function_to_fit,key ):
+    c2 = sf.set_limits(radii[-1]*0.2,radii[2],radii[int(len(radii)/1.5)])
     est_center = radii[-1]/2.-c2
     est_length = radii[-1]*0.1
-    est_amp = abs(np.max(sm_profile)-np.min(sm_profile))
+    if key in ['SDIS']:
+        est_amp = abs(np.max(sm_profile)-np.min(sm_profile))
+    else:
+        est_amp = np.mean(sm_profile[3:])-np.mean(sm_profile[:4])
     est_mean = np.mean(sm_profile)
 
     if not error.any():
         error = np.full(len(y),1.)
         absolute_sigma = False
     else:
         absolute_sigma = True
-    try:
-        arc_par,arc_cov  =  curve_fit(arc_tan_function, radii, sm_profile,p0=[est_center,est_length,est_amp,est_mean]\
-                                    ,sigma=error,absolute_sigma=absolute_sigma)
-    except OptimizeWarning:
-        pass
-    new_profile = arc_tan_function(radii,*arc_par)
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        succes = False
+        maxfev= int(100*(len(radii)))
+
+        while not succes:
 
-    new_profile[:3] = np.mean(new_profile[:3])
+            sf.print_log(f'''FIT_ARC: Starting the curve fit with {maxfev}
+''',Configuration,case= ['debug_start'])
+            try:
+                arc_par,arc_cov  =  curve_fit(function_to_fit, radii, sm_profile,p0=[est_center,est_length,est_amp,est_mean]\
+                                            ,sigma=error,absolute_sigma=absolute_sigma,maxfev=maxfev)
+                new_profile = function_to_fit(radii,*arc_par)
+                new_profile[:3] = np.mean(new_profile[:3])
+                succes = True
+            except OptimizeWarning:
+                maxfev =  2000*(len(radii))
+            except RuntimeError as e:
+                split_error = str(e)
+                if 'Optimal parameters not found: Number of calls to function has reached maxfev' in \
+                    split_error:
+                    maxfev += 100*int(len(radii))
+                    sf.print_log(f'''FIT_ARC: We failed to find an optimal fit due to the maximum number of evaluations. increasing maxfev to {maxfev}
+''',Configuration,case= ['debug_add'])
+                else:
+                    sf.print_log(f'''FIT_ARC: Fit arc crashed with an unknow error:
+{'':8s}{split_error}
+''',Configuration)
+                    raise RuntimeError(split_error)
+            if maxfev >  1000*(len(radii)):
+                sf.print_log(f'''FIT_ARC: We failed to find an optimal fit to dispersion, returning the smoothed profile.
+''',Configuration,case = ['verbose'])
+                succes = True
+                new_profile = copy.deepcopy(sm_profile)
 
     return new_profile#,new_error
 fit_arc.__doc__ =f'''
  NAME:
     fit_arc
  PURPOSE:
     Fit an arc tangent function
@@ -407,144 +774,171 @@
  INPUTS:
     Configuration = Standard FAT configuration
     radii = the horizontal axis
     sm_profile = the  profile to examine
     error = The accompanying error
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     the fitted profile
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def fit_polynomial(Configuration,radii,profile,sm_profile,error, key, Tirific_Template,inner_fix = 4,min_error =0.,boundary_limits = [0,0.], debug = False ):
-    if debug:
-        print_log(f'''FIT_POLYNOMIAL: starting to fit the polynomial with the following input:
+def fit_polynomial(Configuration,radii,profile,sm_profile,error, key, Tirific_Template,\
+                    inner_fix = 4,min_error =0.,boundary_limits = [0,0.],\
+                    allowed_order=[None,None],return_order= False ):
+
+    sf.print_log(f'''FIT_POLYNOMIAL: starting to fit the polynomial with the following input:
 {'':8s} key = {key}
 {'':8s} radii = {radii}
 {'':8s} profile = {profile}
 {'':8s} sm_profile = {sm_profile}
 {'':8s} error = {error}
-''',Configuration['OUTPUTLOG'], debug=debug)
+''',Configuration, case = ['debug_start'])
     only_inner = False
-    if key in ['PA','INCL','Z0']:
+    if key in ['PA','INCL','Z0','ARBITRARY']:
         fixed = inner_fix
-        only_inner =True
+        only_inner = True
         error[:fixed] = error[:fixed]/10.
     elif key in ['VROT']:
         #fixed =len(radii)-Configuration['OUTER_SLOPE_START']
-        fixed =set_limits(len(radii)-np.min(Configuration['LAST_RELIABLE_RINGS']),1,len(radii))
+        fixed =sf.set_limits(len(radii)-np.min(Configuration['LAST_RELIABLE_RINGS']),1,len(radii))
         error[np.min(Configuration['LAST_RELIABLE_RINGS']):] = Configuration['CHANNEL_WIDTH']
         error[0] = Configuration['CHANNEL_WIDTH']
         error[1] = error[1]*3.
     else:
         fixed = 1
-    if len(radii) > 15.:
-        start_order = int(len(radii)/5)
+
+    if len(radii) > 10.:
+        start_order = int(len(radii)/5.)
     else:
         start_order = 0
 
+
+
     st_fit = int(0)
     if key in ['VROT']:
+
         if np.mean(profile[1:3]) > 120.:
             st_fit = int(1)
 
         #This needs another -1 because the 0 and 1/5. ring are more or less 1 ring
-        max_order = set_limits(len(radii)-fixed-2,3,8)
+        max_order = sf.set_limits(len(radii)-fixed-2,3,8)
         #The rotation curve varies a lot so the lower limit should be as high as possible
         #But at least 3 less than max order and maximally 4
         if len(radii)-fixed-2 <= 6:
-            lower_limit=set_limits(3,3,max_order-2)
+            lower_limit=sf.set_limits(3,3,max_order-2)
         elif len(radii)-fixed-2 <= 10:
-            lower_limit=set_limits(4,3,max_order-2)
+            lower_limit=sf.set_limits(4,3,max_order-2)
         else:
-            lower_limit=set_limits(5,3,max_order-2)
-        start_order = set_limits(start_order,lower_limit,max_order)
+            lower_limit=sf.set_limits(5,3,max_order-2)
+        start_order = sf.set_limits(start_order,lower_limit,max_order)
 
     else:
         if key in ['PA','INCL','Z0']:
-            max_order = set_limits(len(radii)-fixed,3,7)
-        else:
-            max_order = set_limits(len(radii)-1,3,7)
-
-
+            max_order = sf.set_limits(len(radii)-fixed,3,5)
+        elif key in ['SBR']:
+            max_order = sf.set_limits(len(radii)-2,4,8)
+            start_order = 3
+        else:
+            max_order = sf.set_limits(len(radii)-1,3,7)
+
+    if allowed_order[0]:
+        if start_order < allowed_order[0]:
+            start_order=  allowed_order[0]
     if start_order >= max_order:
-        max_order = max_order+1
-    if debug:
-        print_log(f'''FIT_POLYNOMIAL: For {key} we start at {start_order} because we have {len(radii)} rings of which {fixed} are fixed
+        max_order = start_order+1
+    if allowed_order[1]:
+        if max_order > allowed_order[1]:
+            max_order=  allowed_order[1]
+
+    sf.print_log(f'''FIT_POLYNOMIAL: For {key} we start at {start_order} because we have {len(radii)} rings of which {fixed} are fixed
 {'':8s} this gves us a maximum order of {max_order}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case = ['debug_add'])
 
     reduced_chi = []
     order = range(start_order,max_order+1)
-    if debug:
-        print_log(f'''FIT_POLYNOMIAL: We will fit the following radii.
+
+    sf.print_log(f'''FIT_POLYNOMIAL: We will fit the following radii.
 {'':8s}{radii[st_fit:]}
 {'':8s} and the following profile:
 {'':8s}{profile[st_fit:]}
 {'':8s} weights = {1./error[st_fit:]}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case = ['debug_add'])
 
     #make sure there are no 0. in the errors
     zero_locations = np.where(error[st_fit:] == 0.)[0]
     if zero_locations.size > 0.:
         error[zero_locations+st_fit] = 1./np.nanmax(1./error)
 
     for ord in order:
         fit_prof = np.poly1d(np.polyfit(radii[st_fit:],profile[st_fit:],ord,w=1./error[st_fit:]))
+
         if st_fit > 0.:
             fit_profile = np.concatenate(([sm_profile[0]],[e for e in fit_prof(radii[st_fit:])]))
         else:
             fit_profile = fit_prof(radii)
         #fit_profile = fit_prof(radii)
+
         if key != 'SBR':
             fit_profile = fix_profile(Configuration, key, fit_profile, Tirific_Template,inner_fix=inner_fix, singular = True,only_inner =only_inner)
+        else:
+            for i in range(len(fit_profile)-5,len(fit_profile)):
+                if fit_profile[i-1] < fit_profile[i]:
+                    fit_profile[i]=fit_profile[i-1]*0.9
         red_chi = np.sum((profile[st_fit:]-fit_profile[st_fit:])**2/error[st_fit:])/(len(radii[st_fit:])-ord)
         #We penailze profiles that go outside the boundaries
 
         if np.sum(np.absolute(np.array(boundary_limits,dtype=float))) != 0.:
-                diff = np.sum(np.array([abs(x-set_limits(x,\
+                diff = np.sum(np.array([abs(x-sf.set_limits(x,\
                                                   boundary_limits[0],\
                                                   boundary_limits[1])) \
                                         for x in  fit_profile[st_fit:]],dtype = float))
                 if diff > 1.:
                     red_chi = red_chi*(diff)
 
         reduced_chi.append(red_chi)
         #if key in ['VROT'] and Configuration['NO_RINGS'] < 2.5*max_order:
         #    reduced_chi[-1] = reduced_chi[-1]*(ord/Configuration['NO_RINGS'])**2.5
-    if debug:
-        print_log(f'''FIT_POLYNOMIAL: We have fitted these:
+    sf.print_log(f'''FIT_POLYNOMIAL: We have fitted these:
 {'':8s} order = {[x for x in order]}
 {'':8s} reducuced chi = {reduced_chi}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case = ['debug_add'])
     reduced_chi = np.array(reduced_chi,dtype = float)
     final_order = order[np.where(np.min(reduced_chi ) == reduced_chi )[0][0]]
 
-    print_log(f'''FIT_POLYNOMIAL: We have regularised {key} with a polynomial of order {final_order}.
-''',Configuration['OUTPUTLOG'])
+    sf.print_log(f'''FIT_POLYNOMIAL: We have regularised {key} with a polynomial of order {final_order}.
+''',Configuration,case=['verbose'])
     fit_profile = np.poly1d(np.polyfit(radii[st_fit:],profile[st_fit:],final_order,w=1./error[st_fit:]))
     if st_fit > 0.:
         new_profile = np.concatenate(([sm_profile[0]],[e for e in fit_profile(radii[st_fit:])]))
     else:
         new_profile = fit_profile(radii)
     #if key in ['VROT'] and profile[1] < profile[2]:
     #    new_profile[1] = profile[1]
     if key != 'SBR':
-        new_profile = fix_profile(Configuration, key, new_profile, Tirific_Template,debug =debug,inner_fix=inner_fix,singular = True,only_inner =only_inner)
-
-    return new_profile#,new_error
+        new_profile = fix_profile(Configuration, key, new_profile, \
+            Tirific_Template,inner_fix=inner_fix,singular = True,\
+            only_inner =only_inner)
+    else:
+        for i in range(len(fit_profile)-5,len(fit_profile)):
+            if fit_profile[i-1] < fit_profile[i]:
+                fit_profile[i]=fit_profile[i-1]*0.9
+    if return_order:
+        return new_profile,final_order
+    else:
+        return new_profile#,new_error
 fit_polynomial.__doc__ =f'''
  NAME:
     fit_polynomial
 
  PURPOSE:
     Fit a polynomial between 3 and 8 order and determine the one with the optimal reduced Chi^2 and return the regularised profile
 
@@ -557,15 +951,15 @@
     profile = profile to be regularised
     sm_profile = smoothed profile
     error = errors on the profile
     key = parameter that is being regularised
     Tirific_Template = standard tirific template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     min_error =0.
     the error should always be large than this value
 
  OUTPUTS:
     polynomial fitted profile
 
@@ -573,43 +967,43 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def fix_outer_rotation(Configuration,profile, debug = False):
-    if debug:
-        print_log(f'''FIX_OUTER_ROTATION: adjust last rings of VROT profile:
+def fix_outer_rotation(Configuration,profile):
+
+    sf.print_log(f'''FIX_OUTER_ROTATION: adjust last rings of VROT profile:
 {'':8s}{profile}
-''',Configuration['OUTPUTLOG'],debug = True)
+{'':8s} from ring {Configuration['RC_UNRELIABLE']} we do not trust the rings.
+''',Configuration,case = ['debug_start'])
     profile = np.array(profile,dtype=float)
-    inner_slope = Configuration['RC_UNRELIABLE']
     # if the outer parts are less then 5 channels there is something wrong And we just take a flat curve from max
-    if np.mean(profile[inner_slope:]) < 5.*Configuration['CHANNEL_WIDTH']:
-        inner_slope = int(np.where(np.max(profile) == profile)[0][0])
-        if debug:
-            print_log(f'''FIX_OUTER_ROTATION: we adjusted the unreliable part.
-''',Configuration['OUTPUTLOG'],debug = True)
-    if debug:
-        print_log(f'''FIX_OUTER_ROTATION: this is the inner slope {inner_slope}
-''',Configuration['OUTPUTLOG'])
-    NUR = Configuration['NO_RINGS']
-    #inner_slope = int(round(set_limits(NUR*(4.-Configuration['LIMIT_MODIFIER'][0])/4.,round(NUR/2.),NUR-2)))
-    if inner_slope != NUR-1 and np.mean(profile[1:3]) > 180.:
-        profile[inner_slope:] = profile[inner_slope-1]
+    if np.mean(profile[Configuration['RC_UNRELIABLE']:]) < 5.*Configuration['CHANNEL_WIDTH']:
+        Configuration['RC_UNRELIABLE'] = int(np.where(np.max(profile) == profile)[0][0])+1
+        if Configuration['RC_UNRELIABLE'] < Configuration['NO_RINGS']-1:
+            profile[Configuration['RC_UNRELIABLE']:] = profile[Configuration['RC_UNRELIABLE']-1]
+
+            sf.print_log(f'''FIX_OUTER_ROTATION: we adjusted the unreliable part.
+{'':8s}{profile}
+{'':8s} from ring {Configuration['RC_UNRELIABLE']} we do not trust the rings.
+    ''',Configuration, case= ['debug_add'])
+
+    #inner_slope = int(round(sf.set_limits(NUR*(4.-Configuration['LIMIT_MODIFIER'][0])/4.,round(NUR/2.),NUR-2)))
+    if Configuration['RC_UNRELIABLE'] < Configuration['NO_RINGS']-1 and np.mean(profile[1:3]) > 180.:
+        profile[Configuration['RC_UNRELIABLE']:] = profile[Configuration['RC_UNRELIABLE']-1]
 
     for i in range(int(Configuration['NO_RINGS']*3./4),Configuration['NO_RINGS']-1):
         if profile[i+1] > profile[i]*1.3:
             profile[i+1] = profile[i]*1.3
 
-    if debug:
-        print_log(f'''FIX_OUTER_ROTATION: this is corrected profile:
+    sf.print_log(f'''FIX_OUTER_ROTATION: this is corrected profile:
 {profile}
-''',Configuration['OUTPUTLOG'])
+''',Configuration, case= ['debug_add'])
 
     return profile
 fix_outer_rotation.__doc__ =f'''
  NAME:
     fix_outer_rotation
 
  PURPOSE:
@@ -619,114 +1013,111 @@
     modify_template
 
  INPUTS:
     Configuration = Standard FAT configuration
     profile = the RC
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     profile = the corrected profile
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE: Declining rotation curves are dealt with in no_declining_vrot
 '''
 
-def fix_profile(Configuration, key, profile, Tirific_Template, debug= False, inner_fix = [4,4], singular = False,only_inner = False ):
-
+def fix_profile(Configuration, key, profile, Tirific_Template, inner_fix = [4,4],\
+                    singular = False,only_inner = False ):
     if isinstance(inner_fix,int):
         inner_fix = [inner_fix]
-    if debug:
-        print_log(f'''FIX_PROFILE: Starting to fix {key} with the input values:
+    sf.print_log(f'''FIX_PROFILE: Starting to fix {key} with the input values:
 {'':8s}{profile}
-''', Configuration['OUTPUTLOG'],debug=True)
+''', Configuration, case= ['debug_add'])
 
     if key == 'SBR':
-        print_log(f'''FIX_PROFILE: To fix sbr profiles use FIX_SBR.
-''', Configuration['OUTPUTLOG'],screen=True)
+        sf.print_log(f'''FIX_PROFILE: To fix sbr profiles use FIX_SBR.
+''', Configuration,case = ['main','screen'])
         raise FunctionCallError("FIX_PROFILE: To fix sbr profiles use check SBR.")
     if singular:
         indexes = [0]
         profile = np.array([profile,profile])
         inner_mean = np.nanmean([profile[0,:inner_fix[0]]])
     else:
         indexes = [0,1]
         if np.sum(inner_fix) != 0.:
             inner_mean = np.nanmean(np.concatenate((profile[0,:inner_fix[0]],profile[1,:inner_fix[1]])))
-
+        else:
+            inner_mean= 0.
 
     profile = np.array(profile,dtype=float)
-
+    rad = [float(x) for x in Tirific_Template['RADI'].split()]
 
     if key in ['VROT']:
         indexes = [0]
         inner_mean = 0.
+        profile[0,0] = 0.
     else:
         for i in indexes:
             profile[i,:inner_fix[i]] = inner_mean
-        if debug:
-            print_log(f'''FIX_PROFILE: the  {inner_fix} inner rings are fixed for the profile:
+        sf.print_log(f'''FIX_PROFILE: the  {inner_fix} inner rings are fixed for the profile:
 {'':8s} profile = {profile[i,:]}
-''', Configuration['OUTPUTLOG'])
-    if debug:
-        print_log(f'''FIX_PROFILE: the  inner mean is {inner_mean}.
-''', Configuration['OUTPUTLOG'])
+''', Configuration,case=['debug_add'])
+    sf.print_log(f'''FIX_PROFILE: the  inner mean is {inner_mean}.
+''', Configuration,case=['debug_add'])
 
     for i in indexes:
+        sf.print_log(f'''FIX_PROFILE: From ring {Configuration['LAST_RELIABLE_RINGS'][i]} on we do not trust these rings.
+''', Configuration,case=['debug_add'])
         if Configuration['LAST_RELIABLE_RINGS'][i] < len(profile[i,:]) and not only_inner:
-            if debug:
-                print_log(f'''FIX_PROFILE: From ring {Configuration['LAST_RELIABLE_RINGS'][i]} on we do not trust these rings.
-''', Configuration['OUTPUTLOG'])
             #profile[i,Configuration['LAST_RELIABLE_RINGS'][i]:] = profile[i,Configuration['LAST_RELIABLE_RINGS'][i]:]*0.25+profile[i,Configuration['LAST_RELIABLE_RINGS'][i]-1]*0.75
             profile[i,Configuration['LAST_RELIABLE_RINGS'][i]:] = profile[i,Configuration['LAST_RELIABLE_RINGS'][i]-1]
-        if debug:
-            print_log(f'''FIX_PROFILE:After fixing the last reliable rings
+        sf.print_log(f'''FIX_PROFILE:After fixing the last reliable rings
 {'':8s} profile = {profile[i,:]}
-''', Configuration['OUTPUTLOG'])
+''', Configuration,case=['debug_add'])
         if key == 'VROT':
-            profile[i] =fix_outer_rotation(Configuration,profile[i],debug= debug)
-        if key in ['PA','INCL','Z0']:
-            xrange = set_limits((int(round(len(profile[0])-5.)/4.)),1,4)
+            profile[i] =fix_outer_rotation(Configuration,profile[i])
+        elif inner_fix[i] != 0:
+            xrange = sf.set_limits((int(round(len(profile[0])-5.)/4.)),1,4)
         # need to make sure this connects smoothly
             for x in range(0,xrange):
                 if inner_fix[i]+x < len(profile[i,:]):
                     profile[i,inner_fix[i]+x] = 1/(x+4./xrange)*inner_mean+ (1-1/(x+4./xrange))*profile[i,inner_fix[i]+x]
-
-        if debug:
-            print_log(f'''FIX_PROFILE:After smoothe transition
+            #if key in ['PA','INCL']:
+            #    profile[i,:] = sf.max_profile_change(Configuration,rad,profile[i,:],key)
+        sf.print_log(f'''FIX_PROFILE:After smoothed transition
 {'':8s} profile = {profile[i,:]}
-''', Configuration['OUTPUTLOG'])
+''', Configuration,case=['debug_add'])
         #profile[:,:Configuration['INNER_FIX']] = np.nanmean(profile[:,:Configuration['INNER_FIX']])
         if key in ['SDIS']:
             inner_max = np.nanmax(profile[i,:int(len(profile[i,:])/2.)])
-            if inner_mean < inner_max:
+            mean = np.nanmean(profile[i,:])
+            if inner_mean < mean or inner_mean < np.nanmean(profile[i,-3:]):
                 ind = np.where(profile[i,:] == inner_max)[0]
                 if ind.size > 1:
                     ind = int(ind[0])
                 else:
                     ind = int(ind)
                 profile[i,:ind] = inner_max
             profile[i] =np.hstack([[profile[i,0]],[y if y <= x else x*0.95 for x,y in zip(profile[i,:],profile[i,1:])]])
     if key == 'VROT':
-        tmp  = no_declining_vrot(Configuration,Tirific_Template,profile = profile[0],debug=debug)
+        tmp  = no_declining_vrot(Configuration,Tirific_Template,profile = profile[0])
         profile[0] = tmp
         profile[1] = tmp
     if singular:
         profile = profile[0]
 
 
-    if debug:
-        print_log(f'''FIX_PROFILE: The final profile for {key} is:
+    sf.print_log(f'''FIX_PROFILE: The final profile for {key} is:
 {'':8s}{profile}
-''', Configuration['OUTPUTLOG'])
+''', Configuration,case=['debug_add'])
     return profile
 fix_profile.__doc__ =f'''
  NAME:
     fix_profile
 
  PURPOSE:
     Modify a fitted profile to be stable against outliers
@@ -737,15 +1128,15 @@
  INPUTS:
     Configuration = Standard FAT configuration
     key = Parameter to be fixed
     profile = profile to be fixed # Maybe we can read this from the template?
     Tirific_Template = Standard Tirific template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     singular = False
     Profile is a single side
 
     only_inner = False
     Only fix the inner part not the outer parts
 
@@ -757,90 +1148,89 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def fix_sbr(Configuration,Tirific_Template, smooth = False, debug=False):
-    if debug:
-        print_log(f'''FIX_SBR: Starting a SBR check.
-''',Configuration['OUTPUTLOG'],debug=True)
+def fix_sbr(Configuration,Tirific_Template, smooth = False, initial = False ):
+    sf.print_log(f'''FIX_SBR: Starting a SBR check.
+''',Configuration,case=['debug_start'])
 
     # get the cutoff limits
-    vsys = float(Tirific_Template['VSYS'].split()[0])
-    radii,cutoff_limits = sbr_limits(Configuration, systemic=vsys)
+    radii,cutoff_limits = sf.sbr_limits(Configuration,Tirific_Template)
     cutoff_limits = np.array([cutoff_limits,cutoff_limits],dtype=float)
     # Then get the profile from the template
-    sbr = np.array(get_from_template(Configuration,Tirific_Template,['SBR','SBR_2']),dtype=float)
-    if debug:
-        print_log(f'''FIX_SBR: Before modify.
+    sbr = sf.load_tirific(Configuration,Tirific_Template,Variables=['SBR','SBR_2'],\
+        array=True)
+    sf.print_log(f'''FIX_SBR: Before modify.
 {'':8s}sbr from template = {sbr}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
     # First make a correction on the inner 2 values
-    sbr = inner_sbr_fix(Configuration,sbr,cutoff_limits,debug=debug)
+    sbr = inner_sbr_fix(Configuration,sbr,cutoff_limits)
     # Let's use a smoothed profile for the fittings
     sm_sbr = smooth_profile(Configuration,Tirific_Template,'SBR',
                             min_error= cutoff_limits,no_apply = True,
-                            fix_sbr_call = True,profile_in = sbr ,debug=debug)
+                            fix_sbr_call = True,profile_in = sbr )
 
-    if debug:
-        print_log(f'''FIX_SBR: Before modify.
+    sf.print_log(f'''FIX_SBR: Before modify.
 {'':8s}sbr  = {sbr}
 {'':8s}sm_sbr  = {sm_sbr}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
 
     # We interpolate negative values as well as values below the limits inner part with a cubi
-    errors = get_error(Configuration,sbr,sm_sbr,'SBR',min_error=cutoff_limits,debug=debug)
-    if debug:
-        print_log(f'''FIX_SBR: retrieved errors.
+    errors = get_error(Configuration,sbr,sm_sbr,'SBR',min_error=cutoff_limits)
+    sf.print_log(f'''FIX_SBR: retrieved errors.
 {'':8s}errors  = {errors}
-''',Configuration['OUTPUTLOG'])
-    error_weights = cutoff_limits/sm_sbr*1./np.nanmin(cutoff_limits[:,2:]/sm_sbr[:,2:])
+''',Configuration,case=['debug_add'])
+    no_zero_sbr = copy.deepcopy(sm_sbr)
+    zeros = np.where(no_zero_sbr < 1e-9)
+    no_zero_sbr[zeros] = 0.1*cutoff_limits[zeros]
+    error_weights = cutoff_limits/no_zero_sbr*1./np.nanmin(cutoff_limits[:,2:]/no_zero_sbr[:,2:])
     error_weights[:,0] = 3.
+    for i in [0,1]:
+        error_weights[i] = [x if x <100. else 100. for x in error_weights[i]]
     errors =errors*error_weights
-    if debug:
-        print_log(f'''FIX_SBR: weighed errors errors.
+    sf.print_log(f'''FIX_SBR: weighed errors errors.
 {'':8s}sm_sbr = {sm_sbr}
 {'':8s}cutoff_limits  = {cutoff_limits}
 {'':8s}errors  = {errors}
 {'':8s}weights  = {error_weights}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
 
 
     store_gaussian = []
     for i in [0,1]:
         corr_val = np.where(sbr[i,2:] > cutoff_limits[i,2:])[0]+2
         # If we have enough safe values in the profile we attempt to fit it
         if corr_val.size > 3.:
             fit_sbr = sm_sbr[i,corr_val]
-            if debug:
-                print_log(f'''FIX_SBR: The values used for fitting are {fit_sbr}.
-''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''FIX_SBR: The values used for fitting are {fit_sbr}.
+''',Configuration,case=['debug_add'])
             try:
-                if 'SBR' in Configuration['FIXED_PARAMETERS'][0]:
-                    vals = fit_gaussian(Configuration,radii[corr_val],fit_sbr,errors=errors[i,corr_val],debug=debug)
-                    gaussian = gaussian_function(radii,*vals)
+                if 'SBR' in Configuration['FIXED_PARAMETERS'][0] \
+                    or initial:
+                    vals = sf.fit_gaussian(Configuration,radii[corr_val],fit_sbr,errors=errors[i,corr_val])
+                    gaussian = sf.gaussian_function(radii,*vals)
                 else:
                     gaussian = fit_polynomial(Configuration,radii,sbr[i,:],sm_sbr[i,:],errors[i,:],'SBR', Tirific_Template,\
-                                             min_error=cutoff_limits[i,:],debug= debug)
+                                             min_error=cutoff_limits[i,:])
                 # if the peak of this gaussian is in the inner two points replace it with the smoothed profile
                 if np.any(np.where(np.max(gaussian) == gaussian)[0] < 2):
-                    if debug:
-                        print_log(f'''FIX_SBR: We are trying to replace the inner gaussian.
+                    sf.print_log(f'''FIX_SBR: We are trying to replace the inner gaussian.
 {'':8s} gaussian = {gaussian[[0,1]]}
 {'':8s} sm_sbr = {sm_sbr[i,[0,1]]}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
                     gaussian[[0,1]] = sm_sbr[i,[0,1]]
-            except RuntimeError:
+            except FittingError:
                 # If we fail we try a CubicSpline interpolation
                 try:
                     tmp = CubicSpline(radii[corr_val],fit_sbr,extrapolate = True,bc_type ='natural')
                     gaussian = tmp(radii)
-                except:
+                except RuntimeError:
                     # and if that fails we just let the values be what they are in the smoothed profile
                     gaussian= sm_sbr[i,:]
             store_gaussian.append(gaussian)
         else:
             #if there are not enough points we simply use the smoothed profile
             store_gaussian.append(sm_sbr[i,:])
 
@@ -852,36 +1242,89 @@
         sbr[np.where(sbr<cutoff_limits)] = store_gaussian[np.where(sbr<cutoff_limits)]
         sbr[:,[0,1,-1]] = store_gaussian[:,[0,1,-1]]
 
     # Need to make sure there are no nans
     sbr[np.isnan(sbr)] = 2.*cutoff_limits[np.isnan(sbr)]
     # and where we are lower than the cutoff we replace with the 1.2 *cutoff unless we smoothed
     if not smooth:
-        sbr[np.where(sbr<cutoff_limits)] = 1.2*cutoff_limits[np.where(sbr<cutoff_limits)]
+        sbr[np.where(sbr<cutoff_limits)] = 2.*cutoff_limits[np.where(sbr<cutoff_limits)]
+        #if our warp_slope is very small we want to increase the SBR significantly
+        for i in [0,1]:
+            if Configuration['WARP_SLOPE'][i] <  0.75*(Configuration['NO_RINGS']) and Configuration['WARP_SLOPE'][i] != None:
+                sbr[i,Configuration['WARP_SLOPE'][i]:] = 0.5*sbr[i,Configuration['WARP_SLOPE'][i]-1]+2.5*sbr[i,Configuration['WARP_SLOPE'][i]:]
     else:
-        sbr[np.where(sbr<cutoff_limits/2.)] = 1e-16
+
+        #sbr[np.where(sbr<cutoff_limits/2.)] = 1e-16
         #no rising outer end profiles
         for i in [0,1]:
+            counter = len(sbr[i,:])-1
+            found_good  = False
+            sf.print_log(f'''FIX_SBR: check sbr vs limits
+{'':8s}sbr = {sbr[i, :]}
+{'':8s}cutoff_limits  = {cutoff_limits[i, :]}
+{'':8s}counter = {counter}
+''',Configuration,case=['debug_add'])
+            while not found_good and counter > 0:
+                if sbr[i, counter] < cutoff_limits[i,counter]/2.:
+                    if counter > 3:
+                        sbr[i, counter] = 1e-16
+                    else:
+                        sbr[i, counter] = cutoff_limits[i,counter]*1.5
+                    counter -= 1
+                else:
+                    found_good =True
+            if counter == 0:
+                sf.print_log(f'''FIX_SBR: We set all off the SBR to 1e-16
+{'':8s}sbr = {sbr[i, :]}
+{'':8s}cutoff_limits  = {cutoff_limits[i, :]}
+{'':8s}counter = {counter}
+''',Configuration,case=['debug_add'])
+                raise FaintSourceError(f"After correcting the SBRs all values we're below the cutoff limit, your source is too faint.")
             if sbr[i,-2] < sbr[i,-1]:
                 last = sbr[i,-1]
                 second = sbr[i,-2]
                 sbr[i,-2] = last
                 sbr[i,-1] = second
+            sf.print_log(f'''FIX_SBR: check sbr vs limits after
+{'':8s}sbr = {sbr[i, :]}
+{'':8s}cutoff_limits  = {cutoff_limits[i, :]}
+{'':8s}counter = {counter}
+''',Configuration,case=['debug_add'])
 
     # and ensure that both sides the inner two rings are the same
     sbr[:,[0,1]] = np.mean(sbr[:,[0,1]])
+    sf.print_log(f'''FIX_SBR: after ensuring both ring are the same
+{'':8s}sbr = {sbr[i, :]}
+''',Configuration,case=['debug_add'])
+    #And that they are less then 3/4 of ring 3 unless ring 3 is blanked
+    ring_three = np.min(sbr[[0,1],2])
+    if ring_three < 1e-15:
+        ring_three = sbr[0,1]*4
+
+    if sbr[0,1] > 3/4.* ring_three:
+        sbr[:,[0,1]] = 3/4.* ring_three
+
+    sf.print_log(f'''FIX_SBR: after ring three
+{'':8s}sbr = {sbr[i, :]}
+''',Configuration,case=['debug_add'])
+    if smooth and len(sbr[0]) > 6:
+        for j in [0,1]:
+            fit_profile = sbr[j]
+            for i in range(len(fit_profile)-5,len(fit_profile)):
+                if fit_profile[i-1] < fit_profile[i]:
+                    fit_profile[i]=fit_profile[i-1]*0.9
+            sbr[j] = fit_profile
 
-    if debug:
-        print_log(f'''FIX_SBR: After modify.
+    sf.print_log(f'''FIX_SBR: After modify.
 {'':8s}{sbr}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
     Tirific_Template['SBR'] = f"{' '.join([f'{x:.2e}' for x in sbr[0]])}"
     Tirific_Template['SBR_2'] = f"{' '.join([f'{x:.2e}' for x in sbr[1]])}"
-    print_log(f'''FIX_SBR: We checked the surface brightness profiles.
-''',Configuration['OUTPUTLOG'])
+    sf.print_log(f'''FIX_SBR: We checked the surface brightness profiles.
+''',Configuration,case=['verbose'])
 fix_sbr.__doc__ =f'''
  NAME:
     fix_sbr
 
  PURPOSE:
     Correct the surface brightness profile against outliers.
 
@@ -889,15 +1332,15 @@
     modify_template
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = standard tirific template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     smooth= False
     Normally only bad points (Not bright enough) and problematic inner points are corrected.
     When smooth is set the profile is either fitted  with a Gaussian function When FIX_SBR = True
     or fitted with a polynomial of n degree. When these fail the profile is
     interpolated with a cubic spline or smoothed with a savgol kernel.
 
@@ -908,22 +1351,23 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def fix_vrot_for_incl_change(Configuration,Tirific_Template, incl_original,incl_modified,debug=False):
-    vrot = np.array(get_from_template(Configuration,Tirific_Template,["VROT","VROT_2"]),dtype = float)
+def fix_vrot_for_incl_change(Configuration,Tirific_Template, incl_original,incl_modified ):
+    vrot = sf.load_tirific(Configuration,Tirific_Template,Variables=["VROT","VROT_2"],\
+                array=True)
     new_vrot = copy.deepcopy(vrot)
     for i in [0,1]:
         vobs = np.array([x*np.sin(np.radians(y)) for x,y in zip(vrot[i],incl_original[i])],dtype=float)
         new_vrot[i] = np.array([x/np.sin(np.radians(y)) for x,y in zip(vobs,incl_modified[i])],dtype=float)
     vrot = np.array([np.mean([x,y]) for x,y in zip(new_vrot[0],new_vrot[1])],dtype=float)
-    format = set_format("VROT")
+    format = sf.set_format("VROT")
     Tirific_Template["VROT"]= f"{' '.join([f'{x:{format}}' for x in vrot[:int(Configuration['NO_RINGS'])]])}"
     Tirific_Template[f"VROT_2"]= f"{' '.join([f'{x:{format}}' for x in vrot[:int(Configuration['NO_RINGS'])]])}"
 
 fix_vrot_for_incl_change.__doc__ =f'''
  NAME:
     fix_vrot_for_incl_change
 
@@ -936,31 +1380,32 @@
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = standard tirific template
     incl_original = profile before modification
     incl_modified = profile after modification
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     The template is corrected
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def flatten_the_curve(Configuration,Tirific_Template,debug = False):
+def flatten_the_curve(Configuration,Tirific_Template):
     to_flatten = ['INCL','Z0','PA','SDIS']
     for key in to_flatten:
-        profile = get_from_template(Configuration,Tirific_Template, [key,f'{key}_2'] ,debug=debug)
+        profile = sf.load_tirific(Configuration,Tirific_Template,Variables=\
+            [key,f'{key}_2'],array=True)
         new_profile = [np.mean(profile) for x in profile[0]]
         Tirific_Template[key] =f" {' '.join([f'{x:.2f}' for x in new_profile])}"
         Tirific_Template[f'{key}_2'] =f" {' '.join([f'{x:.2f}' for x in new_profile])}"
 flatten_the_curve.__doc__ =f'''
  NAME:
     flatten_the_curve
 
@@ -971,89 +1416,89 @@
     modify_template
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = Standard FAT Tirific Template
 
  OPTIONAL INPUTS:
-    debug = False
+
     fit_type = 'Undefined'
 
  OUTPUTS:
     the flattened profiles for PA, INLC, SDIS and Z0 are written to the template
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def get_error(Configuration,profile,sm_profile,key,min_error = [0.],singular = False,weights= [1.],apply_max_error = False,debug=False):
+def get_error(Configuration,profile,sm_profile,key,min_error = [0.],singular = False,weights= [1.],apply_max_error = False ):
 
     try:
         size= len(min_error)
         min_error = np.array(min_error,dtype=float)
     except TypeError:
         min_error = np.array([min_error],dtype=float)
 
-    if debug:
-        print_log(f'''GET_ERROR: starting;
+    sf.print_log(f'''GET_ERROR: starting;
 {'':8s}original profile = {profile}
 {'':8s}new profile = {sm_profile}
 {'':8s}weights = {weights}
 {'':8s}singular = {singular}
 {'':8s}min_error = {min_error}
 {'':8s}max_error = {apply_max_error}
-''',Configuration['OUTPUTLOG'],debug = True)
+''',Configuration, case=['debug_start'])
 
     if singular:
         if len(weights) == 1:
             weights = np.full((len(profile)),weights[0])
         profile = [profile]
         sm_profile = [sm_profile]
         error =[[]]
         sides = [0]
 
     else:
         error = [[],[]]
         if len(weights) == 1:
             weights = np.full((len(profile[0]),len(profile[1])),1.)
         sides =[0,1]
-    if debug:
-        print_log(f'''GET_ERROR: using these weights =
+    sf.print_log(f'''GET_ERROR: using these weights =
 {'':8s}{weights}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
     for i in sides:
         error[i] = abs(profile[i]-sm_profile[i])/2.
         error[i]= error[i]/weights[i]
         if len(min_error.shape) == 2:
             error[i] = [np.max([y,x]) for x,y in zip(error[i],min_error[i])]
         elif len(min_error) == len(error[i]):
             error[i] = [np.max([y,x]) for x,y in zip(error[i],min_error)]
         else:
             error[i] = [np.max([x,min_error[0]]) for x in error[i]]
         if apply_max_error:
             if len(Configuration['MAX_ERROR'][key]) == len(error[i]):
                 error[i] = [np.nanmin([x,y]) for x,y in zip(error[i],Configuration['MAX_ERROR'][key])]
             else:
                 error[i] = [np.nanmin([x,float(Configuration['MAX_ERROR'][key][0])]) for x in error[i]]
-        if key in ['PA','INCL','Z0']:
+        if key in ['PA','INCL','Z0','ARBITRARY']:
             error[i][:Configuration['INNER_FIX'][i]+1] = [np.min(min_error) for x in error[i][:Configuration['INNER_FIX'][i]+1]]
     if singular:
         error = np.array(error[0],dtype=float)
     else:
         error = np.array(error,dtype=float)
-    error[error == 0.] = np.min(error[error > 0.])
+    if np.sum(error) == 0.:
+        error[:] = min_error
+    if 0. in error:
+        error[error == 0.] = np.min(error[error > 0.])
 
-    if debug:
-        print_log(f'''GET_ERROR: error =
+    sf.print_log(f'''GET_ERROR: error =
 {'':8s}{error}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
     return error
 get_error.__doc__ =f'''
  NAME:
     get_error
 
  PURPOSE:
     get the errors associated with a profile
@@ -1064,15 +1509,15 @@
  INPUTS:
     Configuration = Standard FAT configuration
     profile = the profile to consider
     sm_profile = the smoothed version of the profile
     key = the parameter to consider
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     min_error = [0.]
     Errors should always be bigger than this value
 
     singular = False
     If true a single parameter is expected not both sides
 
@@ -1088,66 +1533,59 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE: the maximum errors are defined in main.py
 '''
 
-def get_number_of_rings(Configuration,sbr,sbr_ring_limits, debug=False):
+
+def get_number_of_rings(Configuration,sbr,sbr_ring_limits ):
+    '''Determine whether the amount of rings is good for the limits or not'''
     new_rings = Configuration['NO_RINGS']
     difference_with_limit = np.array(sbr-sbr_ring_limits,dtype=float)
     if np.all(difference_with_limit[:,-1] < 0.):
-        if debug:
-            print_log(f'''GET_NUMBER_OF_RINGS: both last rings are below the limit
-''',Configuration['OUTPUTLOG'],debug=True)
+        sf.print_log(f'''GET_NUMBER_OF_RINGS: both last rings are below the limit
+''',Configuration,case=['debug_start'])
         for i in range(len(difference_with_limit[0,:])-1,int(new_rings/2.),-1):
-            if debug:
-                print_log(f'''GET_NUMBER_OF_RINGS: Checking ring {i}
-''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''GET_NUMBER_OF_RINGS: Checking ring {i}
+''',Configuration,case=['debug_add'])
             if np.all(difference_with_limit[:,i] < 0.):
                 #check that 1 any of the lesser rings are bright enough
                 if np.any(sbr[:,i-1] > 1.5 *sbr_ring_limits[:,i-1]):
                     new_rings = i+1
-                    if debug:
-                        print_log(f'''GET_NUMBER_OF_RINGS: we find that the previous rings are bright enough, rings = {new_rings}
-''',Configuration['OUTPUTLOG'])
+                    sf.print_log(f'''GET_NUMBER_OF_RINGS: we find that the previous rings are bright enough, rings = {new_rings}
+''',Configuration,case=['debug_add'])
                     break
                 else:
-                    if debug:
-                        print_log(f'''GET_NUMBER_OF_RINGS: the previous rings are not bright enough so we reduce 1, old_rings = {new_rings}, new_rings = {i}
-''',Configuration['OUTPUTLOG'])
+                    sf.print_log(f'''GET_NUMBER_OF_RINGS: the previous rings are not bright enough so we reduce 1, old_rings = {new_rings}, new_rings = {i}
+''',Configuration,case=['debug_add'])
                     new_rings = i
             else:
                 #if not both values are below than this is the extend we want
                 new_rings = i+1
-                if debug:
-                    print_log(f'''GET_NUMBER_OF_RINGS: Not both rings warrant cutting, rings = {new_rings}
-''',Configuration['OUTPUTLOG'])
+                sf.print_log(f'''GET_NUMBER_OF_RINGS: Not both rings warrant cutting, rings = {new_rings}
+''',Configuration,case=['debug_add'])
                 break
     else:
-        if debug:
-            print_log(f'''GET_NUMBER_OF_RINGS: Not both last rings are below the limit
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''GET_NUMBER_OF_RINGS: Not both last rings are below the limit
+''',Configuration,case=['debug_add'])
         # if they are not we first check wether both second to last rings are
         if ((difference_with_limit[0,-2] < 0.) and (sbr[0,-1] < 2*sbr_ring_limits[0,-1]) and (difference_with_limit[1,-1] < 0.)) or \
             ((difference_with_limit[1,-2] < 0.) and (sbr[1,-1] < 2*sbr_ring_limits[1,-1]) and (difference_with_limit[0,-1] < 0.)) or\
             ((difference_with_limit[0,-2] < 0.) and (difference_with_limit[1,-2] < 0.) and (sbr[0,-1] < 3*sbr_ring_limits[0,-1]) and (sbr[1,-1] < 3*sbr_ring_limits[1,-1])):
             new_rings -= 1
-            if debug:
-                print_log(f'''GET_NUMBER_OF_RINGS: A second ring is too faint, rings = {new_rings}
-''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''GET_NUMBER_OF_RINGS: A second ring is too faint, rings = {new_rings}
+''',Configuration,case=['debug_add'])
         elif np.all(difference_with_limit[:,-2] < 0.) and np.all(sbr[:,-1] < 5*sbr_ring_limits[:,-1]):
             new_rings -= 1
-            if debug:
-                print_log(f'''GET_NUMBER_OF_RINGS: Both second rings are too faint, rings = {new_rings}
-''',Configuration['OUTPUTLOG'])
-        else:
-            if debug:
-                print_log(f'''GET_NUMBER_OF_RINGS: The second rings are too bright and do not allow for cutting.
-''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''GET_NUMBER_OF_RINGS: Both second rings are too faint, rings = {new_rings}
+''',Configuration,case=['debug_add'])
+        else:
+            sf.print_log(f'''GET_NUMBER_OF_RINGS: The second rings are too bright and do not allow for cutting.
+''',Configuration,case=['debug_add'])
     return new_rings
 get_number_of_rings.__doc__ =f'''
  NAME:
     get_number_of_rings
 
  PURPOSE:
     Determine whether the amount of rings is good for the limits or not should change or not
@@ -1157,72 +1595,78 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     sbr = sbr profiles
     sbr_ring_limits = the limits to evaluate
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     new_rings = the required number of rings
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def get_warp_slope(Configuration,Tirific_Template, debug = False):
-    if debug:
-        print_log(f'''GET_WARP_SLOPE: We have {Tirific_Template['NUR']} rings in the template. and this should be {Configuration['NO_RINGS']}
-''', Configuration['OUTPUTLOG'],debug = True)
-    radii, sbr_ring_limits = sbr_limits(Configuration,systemic = float(Tirific_Template['VSYS'].split()[0]),debug=debug)
+def get_warp_slope(Configuration,Tirific_Template):
+    sf.print_log(f'''GET_WARP_SLOPE: We have {Tirific_Template['NUR']} rings in the template. and this should be {Configuration['NO_RINGS']}
+''', Configuration,case=['debug_start'])
+    radii, sbr_ring_limits = sf.sbr_limits(Configuration,Tirific_Template)
     #get the sbr profiles
-    sbr = np.array(get_from_template(Configuration,Tirific_Template, ['SBR','SBR_2'],debug=debug),dtype = float)
-    if debug:
-        print_log(f'''GET_WARP_SLOPE: We have {len(sbr_ring_limits)} rings in our limits.
+    sbr = sf.load_tirific(Configuration,Tirific_Template,Variables=['SBR','SBR_2'],\
+                array=True)
+    sf.print_log(f'''GET_WARP_SLOPE: We have {len(sbr_ring_limits)} rings in our limits.
 {'':8s}GET_WARP_SLOPE: And we have {len(sbr[0])} rings in our profiles.
-''', Configuration['OUTPUTLOG'])
-    warp_slope = [Tirific_Template['NUR'],Tirific_Template['NUR']]
-    sbr_ring_limits = 2.*np.array([sbr_ring_limits,sbr_ring_limits],dtype=float)
+''', Configuration,case=['debug_add'])
+    warp_slope = [int(Tirific_Template['NUR']),int(Tirific_Template['NUR'])]
+    sbr_ring_limits = 1.5*np.array([sbr_ring_limits,sbr_ring_limits],dtype=float)
     difference_with_limit = np.array(sbr-sbr_ring_limits,dtype=float)
     for i in [0,1]:
         slope = difference_with_limit[i]
         final = slope[slope < 0.]
         if len(slope) > len(final) > 0.:
             not_found = True
             counter = len(slope)-1
             while not_found:
                 if not slope[counter] < 0.:
                     not_found = False
                     final = counter+1
                 else:
                     counter -= 1
         elif len(final) == len(slope):
-            final = 1.
+            final = Configuration['LAST_RELIABLE_RINGS'][i]-1
             for parameter in ['INCL',"PA",'SDIS','Z0']:
                 if parameter not in Configuration['FIXED_PARAMETERS'][0]:
                     Configuration['FIXED_PARAMETERS'][0].append(parameter)
         else:
             final = len(slope)
-        if final > Configuration['LAST_RELIABLE_RINGS'][i]:
-            final = Configuration['LAST_RELIABLE_RINGS'][i]
-        warp_slope[i] = final
-    if debug:
-        print_log(f'''GET_WARP_SLOPE: We find a slope of {warp_slope}.
-''', Configuration['OUTPUTLOG'])
+
+        if final > Configuration['LAST_RELIABLE_RINGS'][i]-1:
+            final = Configuration['LAST_RELIABLE_RINGS'][i]-1
+        # we have to vary some rings else tirific will break with a segmentation fault
+        if final < 2:
+            final = 2
+
+        warp_slope[i] = int(final)
+    sf.print_log(f'''GET_WARP_SLOPE: We find a slope of {warp_slope}.
+''', Configuration,case=['debug_add'])
     Configuration['WARP_SLOPE'] = warp_slope
-    incl = np.array(get_from_template(Configuration,Tirific_Template, ['INCL','INCL_2'],debug=debug),dtype = float)
+    incl = sf.load_tirific(Configuration,Tirific_Template,Variables=['INCL','INCL_2'],\
+            array=True)
     if np.mean(incl[:,:int(Configuration['NO_RINGS']/2.)]) < 35. :
         if 'INCL' not in Configuration['FIXED_PARAMETERS'][0]:
             Configuration['FIXED_PARAMETERS'][0].append('INCL')
-
+    else:
+        if 'INCL' in Configuration['FIXED_PARAMETERS'][0] and 'INCL' not in Configuration['FIXED_PARAMETERS'][1]:
+            Configuration['FIXED_PARAMETERS'][0].remove('INCL')
 get_warp_slope.__doc__ =f'''
  NAME:
     get_warp_slope
 
  PURPOSE:
     Get the rings where the warp should be sloped
 
@@ -1230,66 +1674,59 @@
     modify_template
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = Standard FAT Tirific Template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def inner_sbr_fix(Configuration,sbr,cutoff_limits,debug=False):
-    if debug:
-        print_log(f'''INNER_SBR_FIX: Checking the SBR inner points for runaway values
+def inner_sbr_fix(Configuration,sbr,cutoff_limits ):
+    sf.print_log(f'''INNER_SBR_FIX: Checking the SBR inner points for runaway values
 {'':8s} sbr in  = {sbr}
-''',Configuration['OUTPUTLOG'], debug = True)
+''',Configuration,case=['debug_start'])
 
     if np.all(sbr[:,0] > 2*sbr[:,2]) or np.all(sbr[:,1] > 2*sbr[:,2]):
-        if debug:
-            print_log(f'''INNER_SBR_FIX: We need to correct
+        sf.print_log(f'''INNER_SBR_FIX: We need to correct
 {'':8s} sbr 0  = {sbr[:,0]} sbr 1  = {sbr[:,1]} sbr 2  = {sbr[:,2]}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
         if np.mean(sbr[:,2]) > cutoff_limits[0,2]:
             sbr[:,[0,1]] = np.mean(sbr[:,2])
-            if debug:
-                print_log(f'''INNER_SBR_FIX: We need to correct with mean
+            sf.print_log(f'''INNER_SBR_FIX: We need to correct with mean
 {'':8s} mean = {np.mean(sbr[:,2])}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
         else:
-            if debug:
-                print_log(f'''INNER_SBR_FIX: We need to correct with cut_off_limits
+            sf.print_log(f'''INNER_SBR_FIX: We need to correct with cut_off_limits
 {'':8s} limit = {1.5*cutoff_limits[0,2]}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
             sbr[:,[0,1,2]] = 1.5*cutoff_limits[0,2]
     if np.any(sbr[:,0] > sbr[:,1]):
-        if debug:
-                print_log(f'''INNER_SBR_FIX: We correct 0 point
+        sf.print_log(f'''INNER_SBR_FIX: We correct 0 point
 {'':8s} mean 1 = {np.mean(sbr[:,1])}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
         sbr[:,0] = np.mean(sbr[:,1])
 
     for i in [0,1]:
         if np.any(sbr[:,i] < cutoff_limits[:,2]):
-            if debug:
-                print_log(f'''INNER_SBR_FIX: correcting ring {i}
-''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''INNER_SBR_FIX: correcting ring {i}
+''',Configuration,case=['debug_add'])
             sbr[:,i] = 1.5*cutoff_limits[0,2]
 
-    if debug:
-                print_log(f'''INNER_SBR_FIX: the fixed sbr {sbr}
-''',Configuration['OUTPUTLOG'])
+    sf.print_log(f'''INNER_SBR_FIX: the fixed sbr {sbr}
+''',Configuration,case=['debug_add'])
 
     return sbr
 inner_sbr_fix.__doc__ =f'''
  NAME:
     inner_sbr_fix
 
  PURPOSE:
@@ -1300,57 +1737,51 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     sbr = SBR profile for bothe sides
     cutoff_limits = The reliability limits of the fit
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     sbr = profile with the modified inner points if required
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def modify_flat(Configuration,profile,original_profile,errors,key,inner_fix = [4,4], debug=False):
+def modify_flat(Configuration,profile,original_profile,errors,key,inner_fix = [4,4] ):
 
-    if debug:
-         print_log(f'''MODIFY_FLAT: These {key} profiles are checked to be flat.
+    sf.print_log(f'''MODIFY_FLAT: These {key} profiles are checked to be flat.
 {'':8s} profile = {profile}
 {'':8s} original_profile = {original_profile}
 {'':8s} errors = {errors}
-''',Configuration['OUTPUTLOG'],debug = True)
+''',Configuration,case=['debug_start'])
 
     flatness = []
 
 
     for side in [0,1]:
          flatness.append(check_flat(Configuration,profile[side],errors[side],key,inner_fix=inner_fix[side]\
-                                    ,last_reliable_ring= Configuration['LAST_RELIABLE_RINGS'][side],debug=debug))
-    if debug:
-         print_log(f'''MODIFY_FLAT: Side 0 is flat = {flatness[0]}
+                                    ,last_reliable_ring= Configuration['LAST_RELIABLE_RINGS'][side]))
+    sf.print_log(f'''MODIFY_FLAT: Side 0 is flat = {flatness[0]}
 {'':8s} Side 1 is flat = {flatness[1]}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
 
     if all(flatness):
         if key in ['PA','INCL']:
             profile[:] = profile[0,0]
-        #elif key in ['INCL'] and 30. < np.nanmedian(original_profile[:,-4:]) < 50.:
-        #    profile[:] = np.nanmedian(original_profile[:,:])
-        #elif key in ['INCL'] and np.nanmedian(original_profile[:,-4:]) <= 30.:
-        #    profile[:] = np.nanmedian(original_profile[:,:])
         else:
             profile[:] = np.nanmedian(original_profile[:,:round(len(original_profile)/2.)])
-        errors = get_error(Configuration,original_profile,profile,key,apply_max_error = True,min_error =np.nanmin(errors) , debug=debug)
+        errors = get_error(Configuration,original_profile,profile,key,apply_max_error = True,min_error =np.nanmin(errors))
     else:
         if any(flatness):
             if key not in ['SDIS']:
                 for side in [0,1]:
                     if flatness[side]:
                         if key in ['PA','INCL']:
                             profile[side,:] = profile[side,0]
@@ -1358,26 +1789,29 @@
                         #    profile[side,:] = np.nanmedian(original_profile[side,:])
                         #elif key in ['INCL'] and 30.< np.nanmedian(original_profile[side,round(len(original_profile)/2.):]) <= 30.:
                         #    profile[side,:] = np.nanmedian(original_profile[side,:])
                         else:
                             profile[side,:]  = np.median(original_profile[side,:round(len(original_profile)/2.)])
 
                         flat_val = profile[side,0]
-                        errors[side] = get_error(Configuration,original_profile[side],profile[side],key,apply_max_error = True,min_error =np.nanmin(errors[side]),singular = True ,debug=debug)
+                        errors[side] = get_error(Configuration,\
+                            original_profile[side],profile[side],key,\
+                            apply_max_error = True,\
+                            min_error =np.nanmin(errors[side]),singular = True )
                 profile[:,0:3] = flat_val
                 profile[:,4] = (flat_val+profile[:,4])/2.
             else:
                 profile[:] = np.nanmedian(original_profile[:,:round(len(original_profile)/2.)])
-                errors = get_error(Configuration,original_profile,profile,key,apply_max_error = True,min_error =np.nanmin(errors) , debug=debug)
+                errors = get_error(Configuration,original_profile,profile,key,\
+                        apply_max_error = True,min_error =np.nanmin(errors))
 
-    if debug:
-        print_log(f'''MODIFY_FLAT: Returning:
+    sf.print_log(f'''MODIFY_FLAT: Returning:
 {'':8s} profile = {profile}
 {'':8s} errors = {errors}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
     return profile,errors
 modify_flat.__doc__ =f'''
  NAME:
     modify_flat
 
  PURPOSE:
     Check if a profile should be flat within its errors and if so make it flat
@@ -1389,58 +1823,54 @@
     Configuration = Standard FAT configuration
     profile = the profile to check
     original_profile = the original unmodified profile
     errors = the errors on the profile
     key = the parameter to be checked
 
  OPTIONAL INPUTS:
-    debug = False
+
     fit_type = 'Undefined'
 
  OUTPUTS:
     the final profile and errors
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def no_declining_vrot(Configuration, Tirific_Template, profile = None, debug = False):
-    if debug:
-        print_log(f'''NO_DECLINING_VROT: make RC flat from highest point on.
+def no_declining_vrot(Configuration, Tirific_Template, profile = None):
+    sf.print_log(f'''NO_DECLINING_VROT: make RC flat from highest point on.
 {'':8s}NO_DECLINING_VROT: But only for low value RCs
-''',Configuration['OUTPUTLOG'],debug = True)
+''',Configuration, case=['debug_start'])
     no_input = False
     if profile is None:
         no_input = True
-        profile = np.array(get_from_template(Configuration,Tirific_Template,['VROT'], debug = debug)[0],dtype = float)
-
+        profile = sf.load_tirific(Configuration,Tirific_Template,Variables=['VROT'],\
+                    array=True)
     RCval = np.mean(profile[2:])
     RCmax = np.where(profile == np.max(profile))[0]
     if len(RCmax) > 1:
         RCmax = RCmax[0]
-    if debug:
-            print_log(f'''NO_DECLINING_VROT: We find the maximum at ring {RCmax}
+    sf.print_log(f'''NO_DECLINING_VROT: We find the maximum at ring {RCmax}
 {'':8s}NO_DECLINING_VROT: And a mean value of {RCval}.
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
     Configuration['OUTER_SLOPE_START'] = Configuration['NO_RINGS']-1
     if RCmax < len(profile)/2. or RCval > 180.:
-        if debug:
-            print_log(f'''NO_DECLINING_VROT: We shan't adapt the RC
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''NO_DECLINING_VROT: We shan't adapt the RC
+''',Configuration,case=['debug_add'])
     else:
         for i in range(int(len(profile)/2.),len(profile)-1):
             if profile[i+1] < profile[i]:
                 profile[i:] =profile[i]
-                if debug:
-                    print_log(f'''NO_DECLINING_VROT: Flattening from ring {i} on.)
-    ''',Configuration['OUTPUTLOG'])
+                sf.print_log(f'''NO_DECLINING_VROT: Flattening from ring {i} on.)
+    ''',Configuration,case=['debug_add'])
                 Configuration['OUTER_SLOPE_START'] = i+2
                 break
 
     #and we check that the last parts are not declining too much in anycase
     # For galaxies with more than 10 rings let's make sure the last quarter is not declinining steeply
     if Configuration['NO_RINGS'] > 10:
         for i in range(int(Configuration['NO_RINGS']*3./4),Configuration['NO_RINGS']-1):
@@ -1449,15 +1879,15 @@
     else:
         if profile[-1] < profile[-2]*0.8:
             profile[-1] = profile[-2]*0.8
 
 
     if Configuration['OUTER_SLOPE_START'] > Configuration['NO_RINGS']:
         Configuration['OUTER_SLOPE_START'] = Configuration['NO_RINGS']
-    format = set_format('VROT')
+    format = sf.set_format('VROT')
     if no_input:
         Tirific_Template['VROT'] = f"{' '.join([f'{x:{format}}' for x in profile])}"
         Tirific_Template['VROT_2'] = f"{' '.join([f'{x:{format}}' for x in profile])}"
     else:
         return profile
 no_declining_vrot.__doc__ =f'''
  NAME:
@@ -1470,15 +1900,15 @@
     modify_template
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = Standard tirific template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     profile = None
     Normally the RC is read from the Template however if profile is set it is taken from there.
     This allows for the profile to be modified before it is checked.
 
  OUTPUTS:
     If profile was set the modified profile is returned else the new profile is written to the template which return modified.
@@ -1487,100 +1917,100 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def regularise_profile(Configuration,Tirific_Template, key,min_error= [0.],debug = False, no_apply =False):
-    # We start by getting an estimate for the errors
+
+def regularise_profile(Configuration,Tirific_Template, key,min_error= [0.], no_apply =False):
+    if key in ['PA','INCL']:
+        raise FunctionCallError('The warp is regularised in regularise_warp. regularise profile is for singular profiles only.')
+
+        # We start by getting an estimate for the errors
     min_error=np.array(min_error,dtype=float)
-    profile = np.array(get_from_template(Configuration,Tirific_Template, [key,f"{key}_2"]),dtype=float)
-    weights = get_ring_weights(Configuration,Tirific_Template,debug=debug)
+    weights = sf.get_ring_weights(Configuration,Tirific_Template)
+    #For a lot of things it is important to use a unmodified input profile but we have to avoid the declining vrot
+    if key == 'VROT':
+        no_declining_vrot(Configuration, Tirific_Template)
+    profile = np.array(sf.load_tirific(Configuration,Tirific_Template, [key,f"{key}_2"]),dtype=float)
+    diff = np.sum(profile[0]-profile[1])#Check that we have two profiles
 
+    if diff <1e-8:
+        diff =0.
 
     #First if we have an RC we flatten the curve
-    if debug:
-        print_log(f'''REGULARISE_PROFILE: profile of {key} before regularistion
+    sf.print_log(f'''REGULARISE_PROFILE: profile of {key} before regularistion
 {'':8s}{profile[0]}
 {'':8s}{profile[1]}
 {'':8s}The minimal error is
 {'':8s}{min_error}
-''',Configuration['OUTPUTLOG'],debug = True)
+''',Configuration,case=['debug_start'])
     # get a smoothed profiles
-    sm_profile = smooth_profile(Configuration,Tirific_Template, key ,min_error=min_error,debug=debug,no_apply=True)
+    sm_profile = smooth_profile(Configuration,Tirific_Template, key ,min_error=min_error,no_apply=True)
+
+    error = get_error(Configuration,profile,sm_profile,key,min_error=min_error,weights = weights)
 
-    error = get_error(Configuration,profile,sm_profile,key,min_error=min_error,weights = weights,debug=debug)
 
-    #Check that we have two profiles
-    diff = np.sum(profile[0]-profile[1])
     if key in ['SDIS','VROT']:
         diff = False
     if diff:
-        if debug:
-            print_log(f'''REGULARISE_PROFILE: Treating both sides independently.
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''REGULARISE_PROFILE: Treating both sides independently.
+''',Configuration,case=['debug_add'])
         sides = [0,1]
     else:
-        if debug:
-            print_log(f'''REGULARISE_PROFILE: Found symmetric profiles.
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''REGULARISE_PROFILE: Found symmetric profiles.
+''',Configuration,case=['debug_add'])
         sides = [0]
         error[0] = np.array([np.mean([x,y]) for x,y in zip(error[0],error[1])],dtype=float)
 
-    radii =set_rings(Configuration,debug=debug)
+    radii =sf.set_rings(Configuration)
     for i in sides:
 
-        if key == 'SDIS':
-            try:
-                fit_profile = fit_arc(Configuration,radii,sm_profile[i],error[i],debug= debug)
-            except:
-                fit_profile = np.full(len(sm_profile[i]), np.mean(sm_profile[i]))
-
-
+        if key in ['SDIS']:
+            function_to_fit =arc_tan_sdis_function
+            fit_profile = fit_arc(Configuration,radii,sm_profile[i],error[i],function_to_fit,key)
         else:
 
             fit_profile = fit_polynomial(Configuration,radii,profile[i],sm_profile[i],error[i],key, Tirific_Template,\
                                          inner_fix = Configuration['INNER_FIX'][i],min_error=min_error,\
-                                         boundary_limits= Configuration[f"{key}_CURRENT_BOUNDARY"][i+1],debug= debug)
+                                         boundary_limits= Configuration[f"{key}_CURRENT_BOUNDARY"][i+1])
         profile[i] = fit_profile
 
     if not diff:
         profile[1] = profile[0]
 
-    original = np.array(get_from_template(Configuration,Tirific_Template, [key,f"{key}_2"]),dtype=float)
-    error = get_error(Configuration,original,profile,key,weights=weights,apply_max_error = True,min_error=min_error,debug=debug)
-    if debug:
-            print_log(f'''REGULARISE_PROFILE: This the fitted profile without corrections:
+    original = np.array(sf.load_tirific(Configuration,Tirific_Template, [key,f"{key}_2"]),dtype=float)
+    error = get_error(Configuration,original,profile,key,weights=weights,apply_max_error = True,min_error=min_error)
+    sf.print_log(f'''REGULARISE_PROFILE: This the fitted profile without corrections:
 {'':8s}{profile}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
 #then we want to fit the profiles with a polynomial
     if key not in ['SBR','VROT','SDIS']:
         #We should not fix the profile again as the fitted profile is fixed should be good
 
-        profile,error = modify_flat(Configuration, profile, original, error,key,inner_fix= Configuration['INNER_FIX'],debug=debug)
+        profile,error = modify_flat(Configuration, profile, original, error,key,inner_fix= Configuration['INNER_FIX'])
 
 
-    format = set_format(key)
+    format = sf.set_format(key)
 
     if not no_apply:
         Tirific_Template[key]= f"{' '.join([f'{x:{format}}' for x in profile[0,:int(Configuration['NO_RINGS'])]])}"
         Tirific_Template[f"{key}_2"]= f"{' '.join([f'{x:{format}}' for x in profile[1,:int(Configuration['NO_RINGS'])]])}"
         Tirific_Template.insert(key,f"# {key}_ERR",f"{' '.join([f'{x:{format}}' for x in error[0,:int(Configuration['NO_RINGS'])]])}")
         Tirific_Template.insert(f"{key}_2",f"# {key}_2_ERR",f"{' '.join([f'{x:{format}}' for x in error[1,:int(Configuration['NO_RINGS'])]])}")
         #if key in ['INCL'] and np.mean( profile[:,int(Configuration['NO_RINGS']/2.):int(Configuration['NO_RINGS'])]) < 40.:
-        #    fix_vrot_for_incl_change(Configuration,Tirific_Template,original,profile,debug=debug)
+        #    fix_vrot_for_incl_change(Configuration,Tirific_Template,original,profile)
 
-        if debug:
-            print_log(f'''REGULARISE_PROFILE: And this has gone to the template.
+        sf.print_log(f'''REGULARISE_PROFILE: And this has gone to the template.
 {'':8s}{key} = {Tirific_Template[key]}
 {'':8s}{key}_2 ={Tirific_Template[f"{key}_2"]}
 {'':8s}# {key}_ERR ={Tirific_Template[f"# {key}_ERR"]}
 {'':8s}# {key}_2_ERR ={Tirific_Template[f"# {key}_2_ERR"]}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
     return profile
 regularise_profile.__doc__ =f'''
  NAME:
     regularise_profile
 
  PURPOSE:
     Regularise a parameter profile with a polynomial or a arctan when it is the SDIS
@@ -1590,15 +2020,210 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
     key = parameter to fix
 
  OPTIONAL INPUTS:
-    debug = False
+
+
+    no_apply = false
+    if true do not apply the regularised profile to the template
+
+    min_error = [0.]
+    error should alway be larger than this
+
+ OUTPUTS:
+    the regularised profile
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE: Errors are not returned but they are written to the template
+'''
+
+
+def regularise_warp(Configuration,Tirific_Template, min_error= [0.,0.], no_apply =False,smooth_only=False):
+        # We start by getting an estimate for the errors
+    min_error=np.array(min_error,dtype=float)
+    weights = sf.get_ring_weights(Configuration,Tirific_Template)
+    profile = np.array(sf.load_tirific(Configuration,Tirific_Template, [f"PA",f"PA_2",f"INCL",f"INCL_2"]),dtype=float)
+    diff = np.sum(profile[0]-profile[1])+np.sum(profile[2]-profile[3])  #Check that we have two profiles
+    if diff <1e-8:
+        diff = False
+    else:
+        diff = True
+
+    sf.print_log(f'''REGULARISE_WARP: profile of the warp before regularistion
+{'':8s}PA = {profile[0]}
+{'':8s}PA_2 = {profile[1]}
+{'':8s}INCL = {profile[2]}
+{'':8s}INCL_2 = {profile[3]}
+{'':8s}The minimal error is
+{'':8s}PA min Error = {min_error[0]}, INCL min Error = {min_error[1]}
+''',Configuration,case=['debug_start'])
+    # get a smoothed profiles
+    Theta,Phi,multiple= sf.calculate_am_vector(Configuration,profile[0],profile[2])
+    plus_Theta,plus_Phi,plus_multiple= sf.calculate_am_vector(Configuration,profile[1],profile[3])
+    Theta = np.array([Theta,plus_Theta],dtype=float)
+    Phi = np.array([Phi,plus_Phi],dtype=float)
+    multiple = np.array([multiple,plus_multiple],dtype=float)
+
+    high_theta,high_phi,high_multiple = sf.calculate_am_vector(Configuration,profile[0]+min_error[0],profile[2]+min_error[1])
+    if not np.array_equiv(high_multiple,multiple):
+        high_theta,high_phi,high_multiple = sf.calculate_am_vector(Configuration,profile[0]-min_error[0],profile[2]-min_error[1])
+    low_theta,low_phi,low_multiple = sf.calculate_am_vector(Configuration,profile[1]+min_error[0],profile[3]+min_error[1])
+    if not np.array_equiv(low_multiple,multiple):
+        low_theta,low_phi,low_multiple = sf.calculate_am_vector(Configuration,profile[1]-min_error[0],profile[3]-min_error[1])
+
+    min_change_error = np.sqrt(np.min(np.array([np.min([abs(x-y),abs(w-z)]) for x,y,w,z in zip(Theta[0],high_theta,Theta[1],low_theta)],dtype=float))**2+\
+            np.min(np.array([np.min([abs(x-y),abs(w-z)]) for x,y,w,z in zip(Phi[0],high_phi,Phi[1],low_phi)],dtype=float))**2)
+
+    sf.print_log(f'''REGULARISE_WARP: These converted arrays
+{'':8s}Theta = {Theta[0,:]}
+{'':8s}Theta_2 = {Theta[1,:]}
+{'':8s}Phi = {Phi[0,:]}
+{'':8s}Phi_2 = {Phi[1,:]}
+{'':8s}The minimal error is
+{'':8s}min change Error = {min_change_error}
+''',Configuration,case=['debug_add'])
+
+    theta_zero = Theta[:,0]
+    phi_zero = Theta[:,0]
+    multiple_zero = multiple[:,0]
+     #Let's combine the variation as fraction of the existing angle
+    theta_change= np.array([[float(x-theta_zero[0]) for x in Theta[0]],\
+                            [float(x-theta_zero[1]) for x in Theta[1]]],dtype=float)
+    phi_change= np.array([[float(x-phi_zero[0]) for x in Phi[0]],\
+                            [float(x-phi_zero[1]) for x in Phi[1]]],dtype=float)
+
+    with warnings.catch_warnings():
+        warnings.filterwarnings("ignore",message="invalid value encountered in true_divide"\
+                            ,category=RuntimeWarning)
+        theta_factor = np.sqrt(theta_change**2/(theta_change**2+phi_change**2))\
+                    *(theta_change)/abs(theta_change)
+        theta_factor[np.where(np.array(theta_change) == 0.)] = 0.
+        phi_factor = np.sqrt(phi_change**2/(theta_change**2+phi_change**2))*(phi_change)/abs(phi_change)
+        phi_factor[np.where(np.array(phi_change) == 0.)] = 0.
+    sf.print_log(f'''REGULARISE_WARP: These converted arrays
+{'':8s}Theta_factor = {theta_factor[0,:]}
+{'':8s}Theta_factor_2 = {theta_factor[1,:]}
+{'':8s}Phi_factor = {phi_factor[0,:]}
+{'':8s}Phi_factor_2 = {phi_factor[1,:]}
+''',Configuration,case=['debug_add'])
+    in_zero = np.where(np.array(theta_change+phi_change) == 0.)
+    phi_factor[in_zero]=0.
+    theta_factor[in_zero]=0.
+    change_angle = np.sqrt(theta_change**2+phi_change**2)
+    change_angle[in_zero] =0.
+    change_boundary = calculate_change_boundary(Configuration,multiple_zero,theta_zero,phi_zero)
+    sm_change_angle = smooth_profile(Configuration,Tirific_Template, 'ARBITRARY' ,profile_in=change_angle, min_error=min_change_error,no_apply=True)
+    sm_theta_factor = smooth_profile(Configuration,Tirific_Template, 'ARBITRARY' ,profile_in=theta_factor, min_error=0.005,no_apply=True)
+    sm_phi_factor = smooth_profile(Configuration,Tirific_Template, 'ARBITRARY' ,profile_in=phi_factor, min_error=0.005,no_apply=True)
+
+    error_change_angle = get_error(Configuration,change_angle,sm_change_angle,'ARBITRARY',min_error=min_change_error,weights = weights)
+    error_theta_factor = get_error(Configuration,theta_factor,sm_theta_factor,'ARBITRARY',min_error=0.005,weights = weights)
+    error_phi_factor = get_error(Configuration,phi_factor,sm_phi_factor,'ARBITRARY',min_error=0.005,weights = weights)
+
+    if diff:
+        sf.print_log(f'''REGULARISE_WARP: Treating both sides independently.
+''',Configuration,case=['debug_add'])
+        sides = [0,1]
+    else:
+        sf.print_log(f'''REGULARISE_WARP: Found symmetric profiles.
+''',Configuration,case=['debug_add'])
+        sides = [0]
+
+    radii =sf.set_rings(Configuration)
+    for i in sides:
+        sf.print_log(f'''REGULARISE_WARP: For side {i} we  regularise the following profile.
+{'':8s} change_angle = {change_angle[i]}
+{'':8s} sm_change_angle = {sm_change_angle[i]}
+''',Configuration,case=['debug_add'])
+        if smooth_only:
+            new_change_angle = sm_change_angle[i]
+            new_theta_factor = theta_factor[i]
+            new_phi_factor = phi_factor[i]
+        else:
+            new_change_angle,fit_order = fit_polynomial(Configuration,radii,change_angle[i],sm_change_angle[i],error_change_angle[i],'ARBITRARY', Tirific_Template,\
+                                         inner_fix = Configuration['INNER_FIX'][i],min_error=min_change_error,\
+                                         allowed_order= [2,5],boundary_limits= change_boundary[i+1], return_order=True)
+            new_theta_factor = fit_polynomial(Configuration,radii,theta_factor[i],sm_theta_factor[i],error_theta_factor[i],'ARBITRARY', Tirific_Template,\
+                                         inner_fix = Configuration['INNER_FIX'][i],min_error=0.005,\
+                                         allowed_order= [fit_order,fit_order],boundary_limits= [0.,1.])
+            new_phi_factor = fit_polynomial(Configuration,radii,phi_factor[i],sm_phi_factor[i],error_phi_factor[i],'ARBITRARY', Tirific_Template,\
+                                         inner_fix = Configuration['INNER_FIX'][i],min_error=0.005,\
+                                         allowed_order= [fit_order,fit_order],boundary_limits= [0.,1.])
+        sf.print_log(f'''REGULARISE_WARP:
+{'':8s} new_change_angle = {new_change_angle}
+{'':8s} new_theta_factor = {new_theta_factor}
+{'':8s} new_phi_factor  = {new_phi_factor}
+''',Configuration,case=['debug_add'])
+        new_theta_change = new_change_angle*new_theta_factor
+        new_phi_change = new_change_angle*new_phi_factor
+
+        Theta[i] = theta_zero[i]+new_theta_change
+        Phi[i] = phi_zero[i]+new_phi_change
+        sf.print_log(f'''REGULARISE_WARP:
+{'':8s} Theta = {Theta[i]}
+{'':8s} Phi = {Phi[i]}
+''',Configuration,case=['debug_add'])
+        pa,inclination=sf.calculate_am_vector(Configuration,Theta[i],Phi[i],multiple = multiple[i], invert=True)
+        profile[i]=pa
+        profile[i+2]=inclination
+
+
+    if not diff:
+        profile[1] = profile[0]
+        profile[3] = profile[2]
+    #exit()
+    error= copy.deepcopy(profile)
+    error[:] = 0
+    for i,key in enumerate(['PA','INCL']):
+        original = np.array(sf.load_tirific(Configuration,Tirific_Template, [key,f"{key}_2"]),dtype=float)
+        sm_profile = smooth_profile(Configuration,Tirific_Template, key ,profile_in=profile[2*i:2*i+2], min_error=min_error[i]/3.,no_fix=True,no_apply=True)
+        sm_error =  get_error(Configuration,original,sm_profile,key,weights=weights,apply_max_error = True,min_error=min_error[i]/3.)
+        # As there is too much in flux we do not want to flatten the warp in the first iteration
+        if Configuration['ITERATIONS'] > 1:
+            sm_profile,sm_error = modify_flat(Configuration, sm_profile, original, sm_error,key,inner_fix= Configuration['INNER_FIX'])
+        profile[2*i:2*i+2]=sm_profile
+        error[2*i:2*i+2] = get_error(Configuration,original,profile[2*i:2*i+2],key,weights=weights,apply_max_error = True,min_error=min_error[i])
+        format = sf.set_format(key)
+        if not no_apply:
+            Tirific_Template[key]= f"{' '.join([f'{x:{format}}' for x in profile[2*i,:int(Configuration['NO_RINGS'])]])}"
+            Tirific_Template[f"{key}_2"]= f"{' '.join([f'{x:{format}}' for x in profile[2*i+1,:int(Configuration['NO_RINGS'])]])}"
+            Tirific_Template.insert(key,f"# {key}_ERR",f"{' '.join([f'{x:{format}}' for x in error[2*i,:int(Configuration['NO_RINGS'])]])}")
+            Tirific_Template.insert(f"{key}_2",f"# {key}_2_ERR",f"{' '.join([f'{x:{format}}' for x in error[2*i+1,:int(Configuration['NO_RINGS'])]])}")
+
+            sf.print_log(f'''REGULARISE_PROFILE: This has gone to the template.
+{'':8s}{key} = {Tirific_Template[key]}
+{'':8s}{key}_2 ={Tirific_Template[f"{key}_2"]}
+{'':8s}# {key}_ERR ={Tirific_Template[f"# {key}_ERR"]}
+{'':8s}# {key}_2_ERR ={Tirific_Template[f"# {key}_2_ERR"]}
+''',Configuration,case=['debug_add'])
+    return profile
+regularise_warp.__doc__ =f'''
+ NAME:
+    regularise_warp
+
+ PURPOSE:
+    Regularise a the PA and INCL by smoothing the AM vector
+
+ CATEGORY:
+    modify_template
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    Fits_Files = Standard FAT dictionary with filenames
+    key = parameter to fix
+
+ OPTIONAL INPUTS:
+
 
     no_apply = false
     if true do not apply the regularised profile to the template
 
     min_error = [0.]
     error should alway be larger than this
 
@@ -1609,97 +2234,100 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE: Errors are not returned but they are written to the template
 '''
 
-def set_boundary_limits(Configuration,Tirific_Template,key,values = [0.,0.],  tolerance = 0.01, fixed = False, debug = False):
-    if debug:
-        print_log(f'''SET_BOUNDARY_LIMITS: checking limits for {key},
+
+def set_boundary_limits(Configuration,Tirific_Template,key,values = [0.,0.],  tolerance = 0.01, fixed = False):
+    sf.print_log(f'''SET_BOUNDARY_LIMITS: checking limits for {key},
 {'':8s} current Boundaries = {Configuration[f"{key}_CURRENT_BOUNDARY"]}
 {'':8s} values = {values}
-''',Configuration['OUTPUTLOG'],debug = True)
-    profile = np.array(get_from_template(Configuration,Tirific_Template, [key,f"{key}_2"]),dtype = float)
+''',Configuration,case=['debug_start'])
+    profile = np.array(sf.load_tirific(Configuration,Tirific_Template, [key,f"{key}_2"]),dtype = float)
     current_boundaries = Configuration[f"{key}_CURRENT_BOUNDARY"]
 
-    if key == 'VROT':
+    if key == 'VROT' and np.sum(values) != 0.:
         current_boundaries =[[values[0]-values[1]*5.,values[0]+values[1]*5.] for x in range(3)]
     if np.sum(current_boundaries) == 0. and np.sum(values) != 0.:
         current_boundaries =[[values[0]-values[1],values[0]+values[1]] for x in range(3)]
-        if debug:
-                print_log(f'''SET_BOUNDARY_LIMITS: set boundaries from values
+        sf.print_log(f'''SET_BOUNDARY_LIMITS: set boundaries from values
 {'':8s} current Boundaries = {current_boundaries}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
     elif np.sum(current_boundaries) == 0. and np.sum(values) == 0.:
-        raise FunctionCallError(f'SET_BOUNDARY_LIMITS: if boundaries are not set in the Configuration call set_boundarylimits with values')
+        raise FunctionCallError(f'SET_BOUNDARY_LIMITS: if boundaries are not set in the Configuration call set_boundary_limits with values')
     else:
-        if debug:
-                print_log(f'''SET_BOUNDARY_LIMITS: Checking
+        sf.print_log(f'''SET_BOUNDARY_LIMITS: Checking
 {'':8s} current Boundaries = {current_boundaries}
 {'':8s} Applying to the profiles {profile}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
 
         if fixed:
             range_to_check = [0]
         else:
             range_to_check = [0,1,2]
         for i in range_to_check:
 
             buffer = np.array(float(current_boundaries[i][1]-current_boundaries[i][0])*2,dtype=float)\
-                    *np.array([tolerance,0.1],dtype=float)
-            if debug:
-                print_log(f'''SET_BOUNDARY_LIMITS: Using a buffer of {buffer[0]}.
-    ''',Configuration['OUTPUTLOG'])
+                    *np.array([tolerance,0.25],dtype=float)
+            sf.print_log(f'''SET_BOUNDARY_LIMITS: Using a buffer of {buffer[0]} and a change of {buffer[1]}.
+''',Configuration,case=['debug_add'])
             if i == 0:
-                profile_part = profile[0,:int(np.mean(Configuration['INNER_FIX']))+1]
+                profile_part = profile[0,:int(np.min(Configuration['INNER_FIX']))+1]
+                infix = np.min(Configuration['INNER_FIX'])
             else:
                 profile_part = profile[i-1,Configuration['INNER_FIX'][i-1]:]
-            if debug:
-                print_log(f'''SET_BOUNDARY_LIMITS: Checking {profile_part}.
-    ''',Configuration['OUTPUTLOG'])
+                infix = Configuration['INNER_FIX'][i-1]
+                #Configuration['LAST_RELIABLE_RINGS'][i-1]]
+            sf.print_log(f'''SET_BOUNDARY_LIMITS: Checking {profile_part}.
+{'':8s} because for this part the inner fix = {infix}
+    ''',Configuration,case=['debug_add'])
             #check the upper bounderies
             on_boundary = np.where(profile_part > float(current_boundaries[i][1])-buffer[0])[0]
-            if debug:
-                print_log(f'''SET_BOUNDARY_LIMITS: Found the following on the upper {on_boundary}.
-    ''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''SET_BOUNDARY_LIMITS: Found the following on the upper {on_boundary}.
+    ''',Configuration,case=['debug_add'])
             if len(on_boundary) > 0:
                 if on_boundary[0] != len(profile[0])-1:
-                    current_boundaries[i][1] = current_boundaries[i][1] + np.prod(buffer)
+                    current_boundaries[i][1] = current_boundaries[i][1] + buffer[1]
             #check the lower boundaries.
             on_boundary = np.where(profile_part < float(current_boundaries[i][0])+buffer[0])[0]
-            if debug:
-                print_log(f'''SET_BOUNDARY_LIMITS: Found the following on the lower {on_boundary}.
-    ''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''SET_BOUNDARY_LIMITS: Found the following on the lower {on_boundary}.
+    ''',Configuration,case=['debug_add'])
             if len(on_boundary) > 0:
                 if on_boundary[0] != len(profile[0])-1:
-                    current_boundaries[i][0] = current_boundaries[i][0] - np.prod(buffer)
+                    current_boundaries[i][0] = current_boundaries[i][0] - buffer[1]
     low = [x[0] for x in current_boundaries]
     high= [x[1] for x in current_boundaries]
     if key == 'Z0':
-        inc = np.array(get_from_template(Configuration,Tirific_Template, ['INCL'])[0],dtype = float)
+        inc = np.array(sf.load_tirific(Configuration,Tirific_Template, ['INCL']),dtype = float)
          # Linear increase of the maximum from 30-70 inc
-        min,max = convertskyangle(Configuration,[0.2,set_limits(float(inc[0])/20.-1,0.5,2.5)],Configuration['DISTANCE'], physical = True)
-        high = [set_limits(x,min,max) for x in high]
-        max,min = convertskyangle(Configuration,[0.05,0.2],Configuration['DISTANCE'], physical = True)
-        low = [set_limits(x,min,max) for x in low]
+        min,max = sf.convertskyangle(Configuration,[0.2,sf.set_limits(float(inc[0])/20.-1,0.5,2.5)], physical = True)
+        high = [sf.set_limits(x,min,max) for x in high]
+        min,max = sf.convertskyangle(Configuration,[0.05,0.2], physical = True)
+        low = [sf.set_limits(x,min,max) for x in low]
     elif key == 'INCL':
         # for inclination the other boundaries are bracketed by the input boundary
         high = [x if x > 50. else 50. for x in high]
         low = [x if x < 60. else 60. for x in low]
     elif key == 'PA':
         # for inclination the other boundaries are bracketed by the input boundary
         high = [x if x > 170. else 170. for x in high]
         low = [x if x < 190. else 190. for x in low]
-    set_boundaries(Configuration,key,low,high,debug=debug)
-    #Configuration[f"{key}_CURRENT_BOUNDARY"] = current_boundaries
-    if debug:
-        print_log(f'''SET_BOUNDARY_LIMITS: We have adjusted the boundaries to  {Configuration[f"{key}_CURRENT_BOUNDARY"]}.
-''',Configuration['OUTPUTLOG'])
-    return current_boundaries
+        if abs(high[1]-high[2]) > 30:
+            high[1:] = [np.max(high[1:]) for x in high[1:]]
+        if abs(low[1]-low[2]) > 30:
+            low[1:] = [np.min(low[1:]) for x in low[1:]]
+
+    sf.print_log(f'''SET_BOUNDARY_LIMITS:We use these low = {low} and these high {high} to set {Configuration[f"{key}_CURRENT_BOUNDARY"]}.
+''',Configuration,case=['debug_add'])
+    sf.set_boundaries(Configuration,key,low,high)
+    sf.print_log(f'''SET_BOUNDARY_LIMITS: We have adjusted the boundaries to  {Configuration[f"{key}_CURRENT_BOUNDARY"]}.
+''',Configuration,case=['debug_add'])
+
 set_boundary_limits.__doc__ =f'''
  NAME:
     set_boundary_limits
 
  PURPOSE:
     Update the boundary limits of parameters when too many rings are on the boundary.
 
@@ -1708,15 +2336,15 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = Standard FAT Tirific Template
     key = parameter to check
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     tolerance = 0.01,
     The minimum difference with the boundary
 
     fixed = False
     If true it is assumed there is only one boundary value to check else three
 
@@ -1728,41 +2356,41 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def set_cflux(Configuration,Tirific_Template,debug = False):
+def set_cflux(Configuration,Tirific_Template):
 
     if any(np.isnan(Configuration['NO_POINTSOURCES'])):
-        print_log(f'''SET_CFLUX: We detected an infinite number of model point sources.
+        sf.print_log(f'''SET_CFLUX: We detected an infinite number of model point sources.
 {"":8s}SET_CFLUX: This must be an error. Exiting the fitting.
-''',Configuration['OUTPUTLOG'],screen = True)
+''',Configuration,case=['main','screen'])
         raise CfluxError('The model had infinite point sources')
-    if Configuration['SIZE_IN_BEAMS'] < 15:
+    if np.max(Configuration['SIZE_IN_BEAMS']) < 15:
         factor = 1.
     else:
-        factor=(Configuration['SIZE_IN_BEAMS']/15.)**1.5
+        factor=(np.max(Configuration['SIZE_IN_BEAMS'])/15.)**1.5
     triggered = 0
     if not 0.5e6 < Configuration['NO_POINTSOURCES'][0] < 2.2e6:
-        new_cflux = set_limits(float(Tirific_Template['CFLUX'])*Configuration['NO_POINTSOURCES'][0]/(factor*1e6),1e-7,5e-3)
-        print_log(f'''SET_CFLUX: CFLUX is adapted from {Tirific_Template['CFLUX']} to {new_cflux:.2e}
-''',Configuration['OUTPUTLOG'])
+        new_cflux = sf.set_limits(float(Tirific_Template['CFLUX'])*Configuration['NO_POINTSOURCES'][0]/(factor*1e6),1e-7,5e-3)
+        sf.print_log(f'''SET_CFLUX: CFLUX is adapted from {Tirific_Template['CFLUX']} to {new_cflux:.2e}
+''',Configuration,case=['verbose'])
         Tirific_Template['CFLUX'] = f"{new_cflux:.2e}"
         triggered = 1
     if not 0.5e6 < Configuration['NO_POINTSOURCES'][1] < 2.2e6:
-        new_cflux = set_limits(float(Tirific_Template['CFLUX_2'])*Configuration['NO_POINTSOURCES'][1]/(factor*1e6),1e-7,5e-3)
-        print_log(f'''SET_CFLUX: CFLUX_2 is adapted from {Tirific_Template['CFLUX_2']} to {new_cflux:.2e}
-''',Configuration['OUTPUTLOG'])
+        new_cflux = sf.set_limits(float(Tirific_Template['CFLUX_2'])*Configuration['NO_POINTSOURCES'][1]/(factor*1e6),1e-7,5e-3)
+        sf.print_log(f'''SET_CFLUX: CFLUX_2 is adapted from {Tirific_Template['CFLUX_2']} to {new_cflux:.2e}
+''',Configuration,case=['verbose'])
         Tirific_Template['CFLUX_2'] = f"{new_cflux:.2e}"
         triggered = 1
     if not triggered:
-        print_log(f'''SET_CFLUX: CFLUXES are within the required limits.
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''SET_CFLUX: CFLUXES are within the required limits.
+''',Configuration,case=['verbose'])
 set_cflux.__doc__ =f'''
  NAME:
     set_cflux
 
  PURPOSE:
     Check CFLUX values and make sure they are in the right order for the amount of point sources
 
@@ -1770,37 +2398,37 @@
     modify_template
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = Standard FAT Tirific Template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     Updated CFLUX values in template
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def set_errors(Configuration,Tirific_Template,key,min_error = 0.,debug = False):
+def set_errors(Configuration,Tirific_Template,key,min_error = 0.):
     error = np.full((2,int(Configuration['NO_RINGS'])),min_error)
-    format=set_format(key)
+    format=sf.set_format(key)
     Tirific_Template.insert(key,f"# {key}_ERR",f"{' '.join([f'{x:{format}}' for x in error[0,:int(Configuration['NO_RINGS'])]])}")
     Tirific_Template.insert(f"{key}_2",f"# {key}_2_ERR",f"{' '.join([f'{x:{format}}' for x in error[1,:int(Configuration['NO_RINGS'])]])}")
-    if debug:
-        print_log(f'''SET_ERRORS: This has gone to the template.
+
+    sf.print_log(f'''SET_ERRORS: This has gone to the template.
 {'':8s}# {key}_ERR ={Tirific_Template[f"# {key}_ERR"]}
 {'':8s}# {key}_2_ERR ={Tirific_Template[f"# {key}_2_ERR"]}
-''',Configuration['OUTPUTLOG'],debug = True)
+''',Configuration,case=['debug_start'])
 set_errors.__doc__ =f'''
  NAME:
     set_errors
 
  PURPOSE:
     Write the errors for flat profiles to the template
 
@@ -1809,15 +2437,15 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = Standard tirific template
     key = parameter to write the errors for
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     min_error =0 .
     the error to be used for all rings
 
  OUTPUTS:
     Updated Tirific Template
 
@@ -1825,219 +2453,314 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def set_fitting_parameters(Configuration, Tirific_Template, parameters_to_adjust  = ['NO_ADJUSTMENT'], modifiers = ['EMPTY'], stage = 'initial', initial_estimates = ['EMPTY'],debug = False):
-    if debug:
-        print_log(f'''SET_FITTING_PARAMETERS: We are starting with these modifiers.
+def set_fitting_parameters(Configuration, Tirific_Template, parameters_to_adjust  = ['NO_ADJUSTMENT'], modifiers = ['EMPTY'], stage = 'initial', initial_estimates = ['EMPTY']):
+    sf.print_log(f'''SET_FITTING_PARAMETERS: We are starting with these modifiers.
 {'':8s} {modifiers}
-''',Configuration['OUTPUTLOG'],debug=True)
+''',Configuration,case=['debug_start'])
     try:
         if modifiers[0] == 'EMPTY':
             modifiers = {}
     except KeyError:
         pass
     try:
         if initial_estimates[0] == 'EMPTY':
             initial_estimates = {}
     except KeyError:
         pass
+    if Configuration['INSTALLATION_CHECK']:
+        Tirific_Template['LOOPS'] = "1"
+    elif Configuration['ITERATIONS'] < 3:
+        Tirific_Template['LOOPS'] = "10"
+    else:
+        Tirific_Template['LOOPS'] = f"{Configuration['LOOPS']}"
     fitting_settings = {}
     fitting_keys = ['VARY','VARINDX','MODERATE','DELEND','DELSTART','MINDELTA','PARMAX','PARMIN']
 
     if 'INCL' not in initial_estimates:
         profile = np.array([np.mean([x,y]) for x,y in \
-                    zip(get_from_template(Configuration,Tirific_Template, ['INCL']),\
-                    get_from_template(Configuration,Tirific_Template, [f"INCL_2"]) )],dtype=float)
+                    zip(sf.load_tirific(Configuration,Tirific_Template, ['INCL']),\
+                    sf.load_tirific(Configuration,Tirific_Template, [f"INCL_2"]) )],dtype=float)
         diff = abs(np.max(profile)-np.min(profile))/10.
-        initial_estimates['INCL'] = [profile[0],set_limits(diff,1,5)/np.sin(np.radians(profile[0]))]
+        initial_estimates['INCL'] = [profile[0],sf.set_limits(diff,1.,5.)/np.sin(np.radians(profile[0]))]
 
     if parameters_to_adjust[0] == 'NO_ADJUSTMENT':
         if stage in ['initial','run_cc','after_cc']:
             if initial_estimates['INCL'][0] < 30.:
                 parameters_to_adjust = ['VSYS','SBR','XPOS','YPOS','PA','SDIS','INCL','VROT']
             elif initial_estimates['INCL'][0] < 50.:
                 parameters_to_adjust = ['VSYS','XPOS','YPOS','SBR','PA','SDIS','VROT','INCL']
             elif initial_estimates['INCL'][0] > 75.:
                 parameters_to_adjust = ['VSYS','XPOS','YPOS','VROT','SBR','PA','INCL','SDIS','Z0']
             else:
                 parameters_to_adjust = ['VSYS','XPOS','YPOS','SBR','VROT','PA','INCL','SDIS']
         elif stage in ['initialize_ec','run_ec','after_ec']:
             parameters_to_adjust = ['INCL','PA','VROT','SDIS','SBR','Z0','XPOS','YPOS','VSYS']
         elif stage in  ['initialize_os','run_os','after_os']:
-            parameters_to_adjust = ['VSYS','XPOS','YPOS','INCL','PA','SBR','VROT','SDIS','Z0']
+            if Configuration['ITERATIONS'] == 0:
+                parameters_to_adjust = ['VSYS','XPOS','YPOS','SBR','VROT','SDIS','INCL','PA','Z0']
+            else:
+                if initial_estimates['INCL'][0] < 30.:
+                    parameters_to_adjust = ['SBR','PA','SDIS','INCL','VROT']
+                elif initial_estimates['INCL'][0] < 50.:
+                    parameters_to_adjust = ['SBR','PA','SDIS','VROT','INCL']
+                elif initial_estimates['INCL'][0] > 75.:
+                    parameters_to_adjust = ['VROT','SBR','PA','INCL','SDIS','Z0']
+                else:
+                    parameters_to_adjust = ['SBR','VROT','PA','INCL','SDIS','Z0']
+
+                if Configuration['CENTRAL_CONVERGENCE']:
+                    parameters_to_adjust = parameters_to_adjust+['VSYS','XPOS','YPOS']
+                else:
+                    parameters_to_adjust = ['VSYS','XPOS','YPOS']+parameters_to_adjust
         else:
-            if debug:
-                print_log(f'''SET_FITTING_PARAMETERS: No default adjustment for unknown stage.
-''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''SET_FITTING_PARAMETERS: No default adjustment for unknown stage.
+''',Configuration)
             raise InitializeError('No default adjustment for unknown stage. ')
 
+    for center in Configuration['CENTRAL_FIX']:
+        if center in parameters_to_adjust:
+            parameters_to_adjust.remove(center)
+
+    #VSYS should always be in the initial estimates as sbr setting uses it
+    for key in ['VSYS']:
+        if key not in initial_estimates:
+            profile = np.array(sf.load_tirific(Configuration,Tirific_Template, ['VSYS']),dtype=float)
+            initial_estimates['VSYS'] = [profile[0],Configuration['CHANNEL_WIDTH']/2.]
+
     for key in parameters_to_adjust:
         if key not in initial_estimates:
             profile = np.array([np.mean([x,y]) for x,y in \
-                                zip(get_from_template(Configuration,Tirific_Template, [key])[0],\
-                                get_from_template(Configuration,Tirific_Template, [f"{key}_2"])[0] )],dtype=float)
+                                zip(sf.load_tirific(Configuration,Tirific_Template, [key]),\
+                                sf.load_tirific(Configuration,Tirific_Template, [f"{key}_2"]))],dtype=float)
             diff = abs(np.max(profile)-np.min(profile))/10.
             if key == 'PA':
-                initial_estimates['PA'] = [profile[0],set_limits(diff,0.5,10)]
+                initial_estimates['PA'] = [profile[0],sf.set_limits(diff,0.5,10)]
             elif key == 'VROT':
-                initial_estimates['VROT'] = [np.nanmax(profile),set_limits(np.nanstd(profile[1:]),np.nanmax(profile)-np.nanmin(profile[1:]),np.nanmax(profile))]
+                initial_estimates['VROT'] = [np.nanmax(profile),sf.set_limits(np.nanstd(profile[1:]),np.nanmax(profile)-np.nanmin(profile[1:]),np.nanmax(profile))]
             elif key == 'XPOS':
-                initial_estimates['XPOS'] = [profile[0],Configuration['BEAM_IN_PIXELS'][1]*Configuration['PIXEL_SIZE']]
+                initial_estimates['XPOS'] = [profile[0],0.1*Configuration['BEAM_IN_PIXELS'][1]*Configuration['PIXEL_SIZE']]
             elif key == 'YPOS':
-                initial_estimates['YPOS'] = [profile[0],Configuration['BEAM_IN_PIXELS'][1]*Configuration['PIXEL_SIZE']]
-            elif key == 'VSYS':
-                initial_estimates['VSYS'] = [profile[0],Configuration['CHANNEL_WIDTH']/2.]
+                initial_estimates['YPOS'] = [profile[0],0.1*Configuration['BEAM_IN_PIXELS'][1]*Configuration['PIXEL_SIZE']]
             elif key == 'SDIS':
                 initial_estimates['SDIS'] = [np.mean(profile),Configuration['CHANNEL_WIDTH']]
             elif key == 'Z0':
-                initial_estimates['Z0'] = convertskyangle(Configuration,[0.2,0.05],Configuration['DISTANCE'], physical = True)
+                initial_estimates['Z0'] = sf.convertskyangle(Configuration,[0.2,0.05], physical = True)
+
         if key not in modifiers:
-            if debug:
-                print_log(f'''SET_FITTING_PARAMETERS: Adding {key} to the modifiers
-''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''SET_FITTING_PARAMETERS: Adding {key} to the modifiers
+''',Configuration,case=['debug_add'])
             if key == 'Z0': modifiers['Z0'] = [0.5,0.5,2.]
-            elif key in ['XPOS','YPOS']: modifiers[key] = [1.,1.,1.]
-            elif key == 'VSYS': modifiers[key] = [2.,0.5,0.1]
+            elif key in ['XPOS','YPOS']:
+                if Configuration['CENTRAL_CONVERGENCE']:
+                    modifiers[key] = [0.5,0.5,1.]
+                else:
+                    modifiers[key] = [1.,1.,2.]
+            elif key == 'VSYS':
+                if Configuration['CENTRAL_CONVERGENCE']:
+                    modifiers[key] = [0.5,0.5,1.]
+                else:
+                    modifiers[key] = [2.,0.5,0.5]
             elif stage in  ['initial','run_cc','after_cc','after_ec','after_os','final_os']:
                 if key == 'INCL': modifiers['INCL'] = [1.,1.,1.]
-                elif key == 'PA': modifiers['PA'] = [1.,1.,1.]
+                elif key == 'PA': modifiers['PA'] = [3.,1.,1.]
                 elif key == 'SDIS': modifiers['SDIS'] =  [1.,1.,2.]
             else:
                 if key == 'INCL': modifiers['INCL'] = [2.0,0.5,0.5]
                 elif key == 'PA': modifiers['PA'] =[1.0,1.0,2.0]
                 elif key == 'SDIS': modifiers['SDIS'] =  [1.,1.,0.5]
-    if debug:
-        for key in modifiers:
-            print_log(f'''SET_FITTING_PARAMETERS: This {key} is in modifiers
+
+    for key in modifiers:
+        sf.print_log(f'''SET_FITTING_PARAMETERS: This {key} is in modifiers
 {'':8s} With these values {modifiers[key]}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
+    ###############-- Modfier adaptations for large galaxies ####################
+    if Configuration['OUTER_RINGS_DOUBLED']:
+        for par_to_change in ['XPOS','YPOS']:
+            if par_to_change in modifiers:
+                modifiers[par_to_change]  = np.array(modifiers[par_to_change],dtype=float)*\
+                                            np.array([4.,3.,5.],dtype=float)
+    if  Configuration['VEL_SMOOTH_EXTENDED']:
+        if 'VSYS' in modifiers:
+            modifiers['VSYS']  = np.array(modifiers['VSYS'],dtype=float)*\
+                                        np.array([2.,2.,3.],dtype=float)
+    ###############-- Modfier adaptations based on the inclination ####################
     if stage not in ['final_os']:
         if initial_estimates['INCL'][0] < 30.:
             if 'Z0' in modifiers:
                 modifiers['Z0'][0:1] = np.array(modifiers['Z0'][0:1],dtype=float)*(0.2/0.5)
                 modifiers['Z0'][2] = float(modifiers['Z0'][2])*1.5
             if 'INCL' in modifiers:
                 modifiers['INCL'][0:1] =np.array(modifiers['INCL'][0:1],dtype=float)*(0.1/1.0)
-                modifiers['INCL'][2] = float(modifiers['INCL'][2])*2.
+                modifiers['INCL'][2] = float(modifiers['INCL'][2])*5.
             if 'SDIS' in modifiers:
                 modifiers['SDIS'][0:1] = np.array(modifiers['SDIS'][0:1],dtype=float)*1.5
                 modifiers['SDIS'][2] = float(modifiers['SDIS'][2])*0.5
-            if debug:
-                print_log(f'''SET_FITTING_PARAMETERS: These are the  modifiers after correcting < 30.
+            if 'VSYS' in modifiers:
+                modifiers['VSYS'][0] = modifiers['VSYS'][0]*1.5
+            sf.print_log(f'''SET_FITTING_PARAMETERS: These are the  modifiers after correcting < 30.
 {'':8s} {modifiers}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
         elif initial_estimates['INCL'][0] < 50.:
             if 'Z0' in modifiers:
                 modifiers['Z0'][0:1] = np.array(modifiers['Z0'][0:1],dtype=float)*(0.4/0.5)
                 modifiers['Z0'][2] = float(modifiers['Z0'][2])*1.2
             if 'INCL' in modifiers:
                 modifiers['INCL'][0:1] =np.array( modifiers['INCL'][0:1],dtype=float)*(0.5/1.0)
                 modifiers['INCL'][2] = float(modifiers['INCL'][2])*1.5
-            if debug:
-                print_log(f'''SET_FITTING_PARAMETERS: These are the  modifiers after correcting < 50.
+            sf.print_log(f'''SET_FITTING_PARAMETERS: These are the  modifiers after correcting < 50.
 {'':8s} {modifiers}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
         elif initial_estimates['INCL'][0] > 75.:
             if 'Z0' in modifiers:
                 modifiers['Z0'][0:1] = np.array(modifiers['Z0'][0:1],dtype=float)*(1.25)
                 modifiers['Z0'][2] = float(modifiers['Z0'][2])*0.5
             if 'INCL' in modifiers:
                 modifiers['INCL'][0:1] = np.array(modifiers['INCL'][0:1],dtype=float)*(1.5/1.0)
                 modifiers['INCL'][2] = float(modifiers['INCL'][2])*0.25
             if 'SDIS' in modifiers:
                 modifiers['SDIS'][0:1] = np.array(modifiers['SDIS'][0:1],dtype=float)*0.5
                 modifiers['SDIS'][2] = float(modifiers['SDIS'][2])*1.5
-            if debug:
-                print_log(f'''SET_FITTING_PARAMETERS: These are the modifiers after correcting > 75.
+            sf.print_log(f'''SET_FITTING_PARAMETERS: These are the modifiers after correcting > 75.
 {'':8s} {modifiers}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
         else:
             pass
     else:
         if initial_estimates['INCL'][0] < 40.:
             if 'INCL' in modifiers:
                 modifiers['INCL'] = np.array(modifiers['INCL'],dtype=float)*(0.2)
-
+    if stage in ['initial','initialize_os']:
+        no_boun_check = ['SBR']
+    else:
+        no_boun_check =  ['SBR', 'INCL', 'PA']
     for key in parameters_to_adjust:
         if key in Configuration['FIXED_PARAMETERS'][0]:
             fixed=True
         else:
             fixed =False
-        if key != 'SBR':
-            set_boundary_limits(Configuration,Tirific_Template,key, values=initial_estimates[key], tolerance = 0.1\
-                            ,fixed = fixed,debug=debug)
+
+        if key not in no_boun_check:
+            bracket_values = initial_estimates[key]
+            if key == 'PA':
+                if initial_estimates['INCL'][0] > 35:
+                    upper_limit = 20.
+                else:
+                    upper_limit= 90.
+                bracket_values[1] = sf.set_limits(bracket_values[1]*10., 10.,upper_limit)
+            if key == 'INCL':
+                if bracket_values[0] > 40.:
+                    bracket_values[1] = sf.set_limits(bracket_values[1]*2., 5.,15.)
+            if key == 'VROT':
+                bracket_values[1] = sf.set_limits(bracket_values[1], 10., 75.)
+            # PA and INCL are set in check_angles after the initial
+            set_boundary_limits(Configuration,Tirific_Template,key, values=bracket_values , tolerance = 0.01\
+                            ,fixed = fixed)
         if key == 'VROT':
-            fitting_settings['VROT'] = set_vrot_fitting(Configuration,stage = stage, rotation = initial_estimates['VROT'], debug = debug )
+            fitting_settings['VROT'] = set_vrot_fitting(Configuration,stage = stage, rotation = initial_estimates['VROT'] )
         elif key == 'SBR':
-            fitting_settings['SBR'] = set_sbr_fitting(Configuration,stage = stage, systemic = initial_estimates['VSYS'][0], debug = debug)
+            fitting_settings['SBR'] = set_sbr_fitting(Configuration,Tirific_Template,stage = stage)
         else:
             flat_slope = False
             symmetric = False
             if key in ['PA','INCL','Z0']:
                 slope = Configuration['WARP_SLOPE']
+                profile = np.array(sf.load_tirific(Configuration,Tirific_Template, [key,f"{key}_2"]),dtype=float)
+                for i in [0,1]:
+                    if slope[i] != None:
+                        with warnings.catch_warnings():
+                            warnings.simplefilter("error")
+                            try:
+                                if slope[i] < Configuration['NO_RINGS'] and \
+                                    (np.mean(profile[i,:3]) > np.mean(profile[i,3:slope[i]]) < np.mean(profile[i,slope[i]:]) or \
+                                    np.mean(profile[i,:3]) < np.mean(profile[i,3:slope[i]]) > np.mean(profile[i,slope[i]:])):
+                                    flat_slope = True
+                            except RuntimeWarning:
+                                flat_slope = False
+
+
                 if stage in ['initialize_os']:
-                    inner = int(set_limits(Configuration['NO_RINGS']*1./3., 3,Configuration['NO_RINGS']-2 ))
+                    inner = int(sf.set_limits(Configuration['NO_RINGS']*1./3., 3,Configuration['NO_RINGS']-2 ))
                 else:
                     inner =  Configuration['INNER_FIX']
             elif key in ['SDIS']:
                 flat_slope = True
                 symmetric = True
-                inner = int(set_limits(Configuration['NO_RINGS']*0.33,4,Configuration['NO_RINGS']*0.5))
+                inner = int(sf.set_limits(Configuration['NO_RINGS']*0.33,4,Configuration['NO_RINGS']*0.5))
                 slope = [int(Configuration['NO_RINGS']*0.66),int(Configuration['NO_RINGS']*0.66)]
             else:
                 inner = 4
-                slope = [0.,0.]
+                slope = [None ,None ]
 
             if key in ['SDIS','INCL']:
-                fact = set_limits(float(initial_estimates['INCL'][0])/20.-2.5,1.,2.)
+                fact = sf.set_limits(float(initial_estimates['INCL'][0])/20.-2.5,1.,2.)
                 try:
-                    inner[0] = int(set_limits(inner[0]*fact,4,Configuration['NO_RINGS']/2.))
-                    inner[1] = int(set_limits(inner[1]*fact,4,Configuration['NO_RINGS']/2.))
-                except:
-                    inner = int(set_limits(inner*fact,4,Configuration['NO_RINGS']/2.))
-
-            fitting_settings[key] =  set_generic_fitting(Configuration,key,stage = stage, values = initial_estimates[key],\
-                                                        debug = debug,slope= slope, flat_slope = flat_slope,\
-                                                         fixed =fixed, flat_inner = inner, step_modifier = modifiers[key], \
-                                                         symmetric = symmetric)
+                    inner[0] = int(sf.set_limits(inner[0]*fact,4,Configuration['NO_RINGS']/2.))
+                    inner[1] = int(sf.set_limits(inner[1]*fact,4,Configuration['NO_RINGS']/2.))
+                except TypeError:
+                    inner = int(sf.set_limits(inner*fact,4,Configuration['NO_RINGS']/2.))
+            # set the moderate value
+            moderate = set_generic_moderate(Configuration,key)
+
+
+            fitting_settings[key] =  set_generic_fitting(Configuration,key,\
+                stage = stage, basic_variation = initial_estimates[key][1],\
+                slope= slope, flat_slope = flat_slope,fixed =fixed, \
+                flat_inner = inner, step_modifier = modifiers[key], \
+                symmetric = symmetric,moderate = moderate)
 
     # Reset the fitting parameters
     for fit_key in fitting_keys:
         Tirific_Template[fit_key]= ''
     #write the new parameters
     for key in parameters_to_adjust:
         if key in fitting_settings:
             for fit_key in fitting_keys:
                 if  fit_key in fitting_settings[key]:
+                    format = sf.set_format(key)
 
                     if fit_key in ['DELSTART','DELEND','MINDELTA']:
                     #if fit_key in ['DELEND','MINDELTA']:
                         # These should never be 0.
-                        format = set_format(key)
+                        if fit_key == 'MINDELTA':
+                            sf.print_log(f'''SET_FITTING_PARAMETERS: The MINDELTA for {key} should never be below {Configuration['MIN_ERROR'][key][0]*0.1}.
+''',Configuration,case=['debug_add'])
+
                         for i,x in enumerate(fitting_settings[key][fit_key]):
                             while float(f'{fitting_settings[key][fit_key][i]:{format}}') == 0.:
                                 if float(fitting_settings[key][fit_key][i]) == 0.:
                                     fitting_settings[key][fit_key][i] += 0.01
                                 else:
                                     fitting_settings[key][fit_key][i] *= 2.
+                            if fit_key in ['MINDELTA','DELEND'] and key not in ['SBR']:
+                                if fitting_settings[key][fit_key][i] < Configuration['MIN_ERROR'][key][0]*0.05:
+                                    fitting_settings[key][fit_key][i] = Configuration['MIN_ERROR'][key][0]*0.05
+                            if not Configuration['ACCEPTED_TIRIFIC'] and fit_key == 'MINDELTA':
+                                fitting_settings[key][fit_key][i] = fitting_settings[key][fit_key][i]*sf.set_limits(Configuration['LOOPS']-9,1,4)
+
+
+
+
+
+
 
                     if fit_key == 'VARY':
                         if len(Tirific_Template[fit_key]) == 0:
                             Tirific_Template[fit_key] = ', '.join([f'{x:<10s}' for x in fitting_settings[key][fit_key]])
                         else:
                             Tirific_Template[fit_key] = f"{Tirific_Template[fit_key]}, {', '.join([f'{x:<10s}' for x in fitting_settings[key][fit_key]])}"
                     else:
                         if fit_key == 'VARINDX':
                             format = '<10s'
                         else:
-                            format = set_format(key)
+                            format = sf.set_format(key)
                         Tirific_Template[fit_key] = f"{Tirific_Template[fit_key]} {' '.join([f'{x:{format}}' for x in fitting_settings[key][fit_key]])}"
 set_fitting_parameters.__doc__ = '''
  NAME:
     set_fitting_parameters
 
  PURPOSE:
     Set the parameters that control the fitting in the Tirific template
@@ -2046,15 +2769,15 @@
     modify_template
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = The tirific template to be modified
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     parameters_to_adjust  = ['NO_ADJUSTMENT']
     a list of parameters that have to be set
 
     modifiers = ['EMPTY']
     modifies for startdelt,enddelts,mindelt
 
@@ -2072,52 +2795,45 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def set_generic_fitting(Configuration, key , stage = 'initial', values = [60,5.], \
-                        debug = False, slope = [0, 0], flat_slope = False , symmetric = False,\
+
+
+def set_generic_fitting(Configuration, key , stage = 'initial', basic_variation = 5., \
+                        slope = [None, None], flat_slope = False , symmetric = False,\
                         fixed = True, moderate = 3, step_modifier = [1.,1.,1.],\
                         flat_inner = 3):
-    if debug:
-        print_log(f'''SET_GENERIC_FITTING: We are processing {key}.
-''', Configuration['OUTPUTLOG'] ,debug = True)
+    sf.print_log(f'''SET_GENERIC_FITTING: We are processing {key}.
+''', Configuration, case=['debug_start'])
     if isinstance(flat_inner,int):
         flat_inner = [flat_inner,flat_inner]
     NUR = Configuration['NO_RINGS']
-    if all(x == 0. for x in np.array(slope,dtype=float)):
-        slope = [NUR,NUR]
-
-
-
     input= {}
-    if debug:
-            print_log(f'''SET_GENERIC_FITTING: flat is {fixed}
-''', Configuration['OUTPUTLOG'])
+    sf.print_log(f'''SET_GENERIC_FITTING: flat is {fixed}
+''', Configuration,case=['debug_add'])
     if (stage in ['after_os','final_os','after_cc','after_ec','parameterized']) or fixed:
-        if debug:
-            print_log(f'''SET_GENERIC_FITTING: Fitting all as 1.
-''', Configuration['OUTPUTLOG'])
+        sf.print_log(f'''SET_GENERIC_FITTING: Fitting all as 1.
+''', Configuration,case=['debug_add'])
         input['VARY'] =  np.array([f"{key} 1:{NUR} {key}_2 1:{NUR}"],dtype=str)
         input['PARMAX'] = np.array([Configuration[f'{key}_CURRENT_BOUNDARY'][0][1]],dtype=float)
         input['PARMIN'] = np.array([Configuration[f'{key}_CURRENT_BOUNDARY'][0][0]],dtype=float)
         input['MODERATE'] = np.array([moderate],dtype=int) #How many steps from del start to del end
-        input['DELSTART'] = np.array([values[1]*step_modifier[0]],dtype=float) # Starting step
-        input['DELEND'] = np.array([0.1*values[1]*step_modifier[1]],dtype=float) #Ending step
-        input['MINDELTA'] = np.array([0.05*values[1]*step_modifier[2]],dtype=float) #saturation criterum when /SIZE SIZE should be 10 troughout the code
+        input['DELSTART'] = np.array([basic_variation*step_modifier[0]],dtype=float) # Starting step
+        input['DELEND'] = np.array([0.1*basic_variation*step_modifier[1]],dtype=float) #Ending step
+        input['MINDELTA'] = np.array([0.05*basic_variation*step_modifier[2]],dtype=float) #saturation criterum when /SIZE SIZE should be 10 troughout the code
     else:
         if not symmetric:
-            if debug:
-                print_log(f'''SET_GENERIC_FITTING: implementing a varying non-symmetric profile.
+            sf.print_log(f'''SET_GENERIC_FITTING: implementing a varying non-symmetric profile.
 {'':8s} step_modifier = {step_modifier}
-{'':8s} values = {values}
+{'':8s} variations = {basic_variation}
 {'':8s} limits = {Configuration[f'{key}_CURRENT_BOUNDARY']}
-''', Configuration['OUTPUTLOG'])
+''', Configuration,case=['debug_add'])
             input['VARY'] = []
             end = []
             add = ''
             for i in[0,1]:
                 if i == 1: add='_2'
                 if flat_inner[i]+1 >= NUR:
                     input['VARY'].append(f"!{key}{add} {NUR}")
@@ -2132,46 +2848,45 @@
                                         Configuration[f'{key}_CURRENT_BOUNDARY'][2][1],\
                                         Configuration[f'{key}_CURRENT_BOUNDARY'][0][1]],dtype=float)
 
             input['PARMIN'] = np.array([Configuration[f'{key}_CURRENT_BOUNDARY'][1][0],\
                                         Configuration[f'{key}_CURRENT_BOUNDARY'][2][0],\
                                         Configuration[f'{key}_CURRENT_BOUNDARY'][0][0]],dtype=float)
             input['MODERATE'] =np.array([moderate,moderate,moderate],dtype=float) #How many steps from del start to del end
-            input['DELSTART'] =np.array([2.,2.,0.5],dtype=float)*step_modifier[0]*values[1]# Starting step
-            input['DELEND'] = np.array([0.1,0.1,0.05],dtype=float)*step_modifier[1]*values[1] #Ending step
-            input['MINDELTA'] = np.array([0.1,0.1,0.075],dtype=float)*step_modifier[2]*values[1] #saturation criterum when /SIZE SIZE should be 10 troughout the code
+            input['DELSTART'] =np.array([2.,2.,0.5],dtype=float)*step_modifier[0]*basic_variation# Starting step
+            input['DELEND'] = np.array([0.1,0.1,0.05],dtype=float)*step_modifier[1]*basic_variation#Ending step
+            input['MINDELTA'] = np.array([0.1,0.1,0.075],dtype=float)*step_modifier[2]*basic_variation #saturation criterum when /SIZE SIZE should be 10 troughout the code
         else:
-            if debug:
-                print_log(f'''SET_GENERIC_FITTING: implementing a varying symmetric profile
+            sf.print_log(f'''SET_GENERIC_FITTING: implementing a varying symmetric profile
 {'':8s} step_modifier = {step_modifier}
-{'':8s} values = {values}
+{'':8s} basic_variation = {basic_variation}
 {'':8s} limits = {Configuration[f'{key}_CURRENT_BOUNDARY']}
-''', Configuration['OUTPUTLOG'])
+''', Configuration,case=['debug_add'])
             flat_inner = int(np.min(flat_inner))
             if flat_inner+1 >= NUR:
                 input['VARY'] =  np.concatenate((np.array([f"!{key} {NUR} {key}_2 {NUR}"],dtype=str),\
                                                  np.array([f"{key} 1:{NUR-1} {key}_2 1:{NUR-1}"],dtype=str)))
             else:
                 input['VARY'] =  np.concatenate((np.array([f"!{key} {NUR}:{flat_inner+1} {key}_2 {NUR}:{flat_inner+1}"],dtype=str),\
                                                  np.array([f"{key} 1:{flat_inner} {key}_2 1:{flat_inner}"],dtype=str)))
             input['PARMAX'] = np.array([Configuration[f'{key}_CURRENT_BOUNDARY'][1][1],\
                                         Configuration[f'{key}_CURRENT_BOUNDARY'][0][1]],dtype=float)
             input['PARMIN'] = np.array([Configuration[f'{key}_CURRENT_BOUNDARY'][1][0],\
                                         Configuration[f'{key}_CURRENT_BOUNDARY'][0][0]],dtype=float)
             input['MODERATE'] =np.array([moderate,moderate],dtype=float) #How many steps from del start to del end
-            input['DELSTART'] =np.array([2.,0.5],dtype=float)*step_modifier[0]*values[1] # Starting step
-            input['DELEND'] = np.array([0.1,0.05],dtype=float)*step_modifier[1]*values[1] #Ending step
-            input['MINDELTA'] = np.array([0.1,0.075],dtype=float)*step_modifier[2]*values[1] #saturation criterum when /SIZE SIZE should be 10 troughout the code
+            input['DELSTART'] =np.array([2.,0.5],dtype=float)*step_modifier[0]*basic_variation # Starting step
+            input['DELEND'] = np.array([0.1,0.05],dtype=float)*step_modifier[1]*basic_variation #Ending step
+            input['MINDELTA'] = np.array([0.1,0.075],dtype=float)*step_modifier[2]*basic_variation #saturation criterum when /SIZE SIZE should be 10 troughout the code
         # then we need to set the warp slope
 
         forvarindex = ''
         if Configuration['NO_RINGS'] > 5:
             implement_keys = [key, f"{key}_2"]
             for i,cur_key in enumerate(implement_keys):
-                if slope[i] < NUR:
+                if slope[i] < NUR and slope[i] != None:
                     if flat_slope:
                         if slope[i]+1 == NUR:
                             forvarindex = forvarindex+f"{cur_key} {NUR} "
                         else:
                             forvarindex = forvarindex+f"{cur_key} {NUR}:{slope[i]+1} "
                     else:
                         if slope[i]+1 >= NUR-1:
@@ -2194,23 +2909,25 @@
     modify_template
 
  INPUTS:
     Configuration = Standard FAT configuration
     key = parameter to set the fitting for
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     stage = 'initial'
     STAGE OF THE FITTING WE ARE IN
 
-    values = [60,5.]
-    mean values of the parameter
+    basic_variation = 5.
+        the basic variation parameters which is the base for delstart
+        delstart =  basic_variation  without modifiers
+        delend and mindelt = 0.1*basic_variation without modifiers
 
-    slope = [0, 0]
+    slope = [None, None]
     outer rings to be fitted as slope
 
     flat_slope = False
     if true slope should include the last ring
 
     symmetric = False
     Both sides are fitted as one
@@ -2238,43 +2955,44 @@
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
+def set_generic_moderate(Configuration,key):
+    ''' set the moderate value for a parameter
+    This does not include VROT and SBR '''
+    if not Configuration['CENTRAL_CONVERGENCE'] and key in ['VSYS','XPOS','YPOS']:
+        moderate = 3
+    else:
+        moderate = 3
+    return moderate
+
 
 #Function
-def set_model_parameters(Configuration, Tirific_Template,Model_Values, stage = 'initial',debug = False):
+def set_model_parameters(Configuration, Tirific_Template,Model_Values, stage = 'initial'):
     parameters_to_set = ['RADI','VROT_profile','Z0','SBR_profile','INCL','PA','XPOS','YPOS','VSYS','SDIS']
 
 
     check_parameters = []
     if 'VSYS' in Model_Values:
-        vsys =Model_Values['VSYS'][0]/1000.
+        vsys = Model_Values['VSYS']
     else:
         vsys=100.
     scramble = np.zeros(len(parameters_to_set))
-    # If the inclination is low we want to throw the inclination and VROT out of Vobs hence we scramble with random values
-    #if stage == 'initialize_def_file':
-    #        if 'INCL' in parameters_to_set:
-    #            if Model_Values['INCL'][0] < 40.:
-    #                scramble[parameters_to_set.index('INCL')] = np.random.uniform(-5,5,1)[0]
-                    #if 'VROT_profile' in parameters_to_set:
-                    #    Model_Values['VROT_profile'] = [set_limits(x+np.random.uniform(-2.*Configuration['CHANNEL_WIDTH'],2.*Configuration['CHANNEL_WIDTH'],1)[0], 0,600.) for x in Model_Values['VROT_profile'] ]
-                    #    scramble[parameters_to_set.index('VROT_profile')] = np.mean([x*np.sin(np.radians(Model_Values['INCL'][0]))/np.sin(np.radians(Model_Values['INCL'][0]))])
 
     for key in parameters_to_set:
         if key in Model_Values:
             if key in ['VROT_profile','SBR_profile']:
                 key_to_set = key.split('_')[0]
             else:
                 key_to_set = key
             # if 2 long we have a value and error
-            format = set_format(key_to_set)
+            format = sf.set_format(key_to_set)
             if len(Model_Values[key]) == 2:
                 Tirific_Template[key_to_set]= f"{Model_Values[key][0]+scramble[parameters_to_set.index(key)]:{format}}"
             else:
                 Tirific_Template[key_to_set]= f"{' '.join([f'{x+scramble[parameters_to_set.index(key)]:{format}}' for x in Model_Values[key][:int(Configuration['NO_RINGS'])]])}"
             if key_to_set != 'RADI':
                 key_write = f"{key_to_set}_2"
                 if f"{key}_2" in Model_Values:
@@ -2283,28 +3001,25 @@
                     Tirific_Template[key_write]= f"{Model_Values[key][0]+scramble[parameters_to_set.index(key)]:{format}}"
                 else:
                     Tirific_Template[key_write]= f"{' '.join([f'{x+scramble[parameters_to_set.index(key)]:{format}}' for x in Model_Values[key][:int(Configuration['NO_RINGS'])]])}"
 
             check_parameters.append(key)
         else:
             if key == 'RADI':
-                rad = set_rings(Configuration,debug=debug)
-                if len(Configuration['OLD_RINGS']) == 0:
-                    size_in_beams = (rad[-1]-1./5.*Configuration['BEAM'][0])/Configuration['BEAM'][0]
-                    Configuration['OLD_RINGS'].append(f"{size_in_beams:.1f}")
+                rad = sf.set_rings(Configuration)
                 Tirific_Template['RADI']= f"{' '.join([f'{x:.2f}' for x in rad])}"
                 Tirific_Template['NUR']=str(len(rad))
                 check_parameters.append('RADI')
             elif key == 'Z0':
                 check_parameters.append('Z0')
                 if Model_Values['INCL'][0] > 80:
-                    Tirific_Template['Z0'] = f"{np.max([convertskyangle(Configuration,0.2,distance=Configuration['DISTANCE'],physical= True),Configuration['BEAM'][0]/4.]):.3f}"
+                    Tirific_Template['Z0'] = f"{np.max([sf.convertskyangle(Configuration,0.2,physical= True),Configuration['BEAM'][0]/4.]):.3f}"
 
                 else:
-                    Tirific_Template['Z0'] = f"{convertskyangle(Configuration,0.2,distance=Configuration['DISTANCE'],physical= True):.3f}"
+                    Tirific_Template['Z0'] = f"{sf.convertskyangle(Configuration,0.2,physical= True):.3f}"
 
 
                 Tirific_Template['Z0_2'] = Tirific_Template['Z0']
 
             elif key == 'SDIS':
                 check_parameters.append('SDIS')
                 Tirific_Template['SDIS'] = '8.'
@@ -2337,15 +3052,15 @@
                 raise InitializeError(f"The parameter {key} is not set in the initialization")
 
     #make sure that the first value in VROT = 0
     vrot = Tirific_Template['VROT'].split()
     if float(vrot[0]) != 0.:
         Tirific_Template['VROT']=f" 0. {' '.join([f'{x}' for x in vrot[:int(Configuration['NO_RINGS']-1)]])}"
         Tirific_Template['VROT_2']=f" 0. {' '.join([f'{x}' for x in vrot[:int(Configuration['NO_RINGS']-1)]])}"
-    no_declining_vrot(Configuration, Tirific_Template, debug = debug)
+    no_declining_vrot(Configuration, Tirific_Template)
 set_model_parameters.__doc__ =f'''
  NAME:
     set_model_parameters
 
  PURPOSE:
     Set the model values parameters in the tirific file that are singular values that apply to all of the fitting such as names and other issues
 
@@ -2354,138 +3069,132 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = Standard FAT Tirific Template
     Model_Values = the values for setting
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     stage = 'initial'
     stage of the fitting process
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 #function to check that all parameters in template have the proper length.
-def set_new_size(Configuration,Tirific_Template, Fits_Files, fit_type = 'Undefined', stage = 'initial',
-                    current_run='Not Initialized', debug = False, Variables =
+def set_new_size(Configuration,Tirific_Template, fit_type = 'Undefined',
+                    current_run='Not Initialized', Variables =
                     ['VROT','Z0', 'SBR', 'INCL','PA','XPOS','YPOS','VSYS','SDIS','VROT_2',  'Z0_2','SBR_2',
                      'INCL_2','PA_2','XPOS_2','YPOS_2','VSYS_2','SDIS_2', 'AZ1P', 'AZ1W' ,'AZ1P_2','AZ1W_2', 'RADI']):
-    if debug:
-        print_log(f'''SET_NEW_SIZE: Starting the adaptation of the size in the template
-''',Configuration['OUTPUTLOG'],debug =True)
+    sf.print_log(f'''SET_NEW_SIZE: Starting the adaptation of the size in the template
+''',Configuration,case=['debug_start'])
     for key in Variables:
         if not key in Tirific_Template:
             Variables.remove(key)
-    parameters = get_from_template(Configuration,Tirific_Template,Variables,debug = debug)
+    parameters = sf.load_tirific(Configuration,Tirific_Template,Variables)
     # do a check on whether we need to modify all
-    radii = set_rings(Configuration,debug=debug)
+    radii = sf.set_rings(Configuration)
     if not Configuration['NEW_RING_SIZE']:
-        print_log(f'''SET_NEW_SIZE: The rings size is stable and we are not interpolating
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''SET_NEW_SIZE: The rings size is stable and we are not interpolating
+''',Configuration,case=['debug_add'])
         interpolate = False
     else:
-        print_log(f'''SET_NEW_SIZE: The rings size is updated and we are interpolating the old values.
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''SET_NEW_SIZE: The rings size is updated and we are interpolating the old values.
+''',Configuration,case= ['verbose'])
         old_radii = parameters[Variables.index('RADI')]
         Configuration['NEW_RING_SIZE'] = False
         interpolate = True
     #if we add a ring we need to make sure that the radius gets extended
     if len(radii) > len(parameters[Variables.index('RADI')]):
         parameters[Variables.index('RADI')] = radii
         #and the last SBR values are far too high, set them to zero such that fix_sbr will correct them
         for i in [-3,-2,-1]:
             parameters[Variables.index('SBR')][i] = 0.
             parameters[Variables.index('SBR_2')][i] = 0.
 
 
     for i,key in enumerate(Variables):
-
-        if debug:
-            print_log(f'''SET_NEW_SIZE: We are processing {key}
+        sf.print_log(f'''SET_NEW_SIZE: We are processing {key}
 {'':8s}SET_NEW_SIZE: We have a parameter of length {len(parameters[i])}.
 {'':8s}SET_NEW_SIZE: Our current number of rings in the model is {Configuration['NO_RINGS']}.
 {'':8s}SET_NEW_SIZE: {parameters[i]}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
         if key == 'RADI':
             Tirific_Template[key] = f" {' '.join([f'{x:.2f}' for x in radii])}"
         else:
             if interpolate:
-                if debug:
-                    print_log(f'''SET_NEW_SIZE: We are interpolating par = {parameters[i]} old radii={old_radii} new radii={radii}
-    ''',Configuration['OUTPUTLOG'])
-                if len(parameters[i]) > len(old_radii):
-                    if debug:
-                        print_log(f'''SET_NEW_SIZE: The parameters have more values than the radii. Cutting the end.
-    ''',Configuration['OUTPUTLOG'])
-                        parameters[i] = parameters[i][:len(old_radii)-1]
-                elif len(parameters[i]) < len(old_radii):
-                    if debug:
-                        print_log(f'''SET_NEW_SIZE: The parameters have less values than the radii. Adding the last value until match.
-    ''',Configuration['OUTPUTLOG'])
-                        while len(parameters[i]) < len(old_radii):
-                            parameters[i].append(parameters[i][-1])
-
-                parameters[i] = list(np.interp(np.array(radii,dtype=float),np.array(old_radii,dtype=float),np.array(parameters[i],dtype=float)))
-
-            format = set_format(key)
+                radii_int=np.array(radii,dtype=float)
+                old_radii_int = np.array(old_radii,dtype=float)
+                parameters_int = copy.deepcopy(parameters[i])
+                sf.print_log(f'''SET_NEW_SIZE: We are interpolating par = {parameters_int} old radii={old_radii_int} new radii={radii_int}
+    ''',Configuration,case=['debug_add'])
+                if len(parameters_int) > len(old_radii_int):
+                    sf.print_log(f'''SET_NEW_SIZE: The parameters have more values than the radii. Cutting the end.
+    ''',Configuration,case=['debug_add'])
+                    parameters_int = parameters_int[:len(old_radii)-1]
+                elif len(parameters_int) < len(old_radii_int):
+                    sf.print_log(f'''SET_NEW_SIZE: The parameters have less values than the radii. Adding the last value until match.
+    ''',Configuration,case=['debug_add'])
+                    while len(parameters_int) < len(old_radii_int):
+                        parameters_int.append(parameters_int[-1])
+
+                parameters[i] = list(np.interp(radii_int,old_radii_int,np.array(parameters_int,dtype=float)))
+                del radii_int
+                del old_radii_int
+                del parameters_int
+            format = sf.set_format(key)
 
             if len(parameters[i]) > Configuration['NO_RINGS']-1:
                 # if we are cutting a ring it is likely the outer ring have done weird stuff so we flatten the curve
 
                 Tirific_Template[key] =f" {' '.join([f'{x:{format}}' for x in parameters[i][:int(Configuration['NO_RINGS'])]])}"
             elif len(parameters[i]) <= Configuration['NO_RINGS']-1:
                 # We simply add the last value
                 counter = len(parameters[i])
                 while counter !=  Configuration['NO_RINGS']:
                     Tirific_Template[key] = Tirific_Template[key] + f" {parameters[i][-1]:{format}}"
                     counter += 1
-
-
-        if debug:
-            print_log(f'''SET_NEW_SIZE: We wrote the following line {Tirific_Template[key]}
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''SET_NEW_SIZE: We wrote the following line {Tirific_Template[key]}
+''',Configuration,case=['debug_add'])
 
     #Replace the old ring numbers in VARY and VARINDX
-    old_rings = calc_rings(Configuration,size_in_beams = int(round(float(Configuration['OLD_RINGS'][-2]))), ring_size  = 0.,debug=debug)
-    current_rings = calc_rings(Configuration,debug=debug)
+    old_rings = sf.calc_rings(Configuration,size_in_beams = int(round(np.max([float(Configuration['OLD_SIZE'][-1][0]),float(Configuration['OLD_SIZE'][-1][1])]))), ring_size  = 0.)
+    current_rings = sf.calc_rings(Configuration)
     #This could lead to replacing a value smaller than the other side
     Tirific_Template['VARY'] = Tirific_Template['VARY'].replace(f"{old_rings}",f"{current_rings}")
     Tirific_Template['VARINDX'] = Tirific_Template['VARINDX'].replace(f"{old_rings-1}",f"{current_rings-1}")
     Tirific_Template['NUR'] = f"{current_rings}"
     # if we cut we want to flatten things
     #if current_rings < old_rings:
-    #    flatten_the_curve(Configuration,Tirific_Template,debug=debug)
+    #    flatten_the_curve(Configuration,Tirific_Template)
     # Check whether the galaxy has become to small for variations
-    if Configuration['SIZE_IN_BEAMS'] > Configuration['MINIMUM_WARP_SIZE']:
+    if np.sum(Configuration['SIZE_IN_BEAMS']) > Configuration['MINIMUM_WARP_SIZE']:
         Configuration['FIXED_PARAMETERS'][0] = Configuration['FIXED_PARAMETERS'][1]
     else:
         for parameter in ['INCL','Z0','SDIS','PA']:
             if parameter not in Configuration['FIXED_PARAMETERS'][0]:
                 Configuration['FIXED_PARAMETERS'][0].append(parameter)
-        flatten_the_curve(Configuration,Tirific_Template,debug=debug)
-    if debug:
-        print_log(f'''The following parameters will be fixed'
+        flatten_the_curve(Configuration,Tirific_Template)
+    sf.print_log(f'''The following parameters will be fixed'
 {'':8s} {Configuration['FIXED_PARAMETERS'][0]}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
 
     #update the limit_modifier
-    Inclination = np.array([(float(x)+float(y))/2. for x,y in zip(Tirific_Template['INCL'].split(),Tirific_Template['INCL_2'].split())],dtype=float)
-    set_limit_modifier(Configuration,Inclination,debug=debug)
+    sf.set_limit_modifier(Configuration,Tirific_Template)
     # Maybe increase the amount of loops in smaller galaxies
-    set_overall_parameters(Configuration, Fits_Files,Tirific_Template ,fit_type=fit_type, debug=debug,stage=stage)
+    #set_overall_parameters(Configuration, Fits_Files,Tirific_Template ,fit_type=fit_type)
     # if we change the radii we need to restart tirific
-    finish_current_run(Configuration,current_run,debug=debug)
+    sf.finish_current_run(Configuration,current_run)
 set_new_size.__doc__ =f'''
  NAME:
     set_new_size
 
  PURPOSE:
     Set the parameters in the template when the rings need to be adjusted.
 
@@ -2494,21 +3203,19 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
     Tirific_Template = Standard FAT Tirific Template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     fit_type = 'Undefined'
     type of fitting
 
-    stage = 'initial'
-    stage of the fitting
 
     current_run='Not Initialized'
     subprocess structure running tirific
 
     Variables =['VROT','Z0', 'SBR', 'INCL','PA','XPOS','YPOS','VSYS','SDIS','VROT_2',  'Z0_2','SBR_2',
                      'INCL_2','PA_2','XPOS_2','YPOS_2','VSYS_2','SDIS_2', 'AZ1P', 'AZ1W' ,'AZ1P_2','AZ1W_2', 'RADI']
     Variables to be updated
@@ -2520,61 +3227,43 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def set_overall_parameters(Configuration, Fits_Files,Tirific_Template,stage = 'initial',fit_type='Undefined', flux = None,debug = False):
+def set_overall_parameters(Configuration, Fits_Files,Tirific_Template,fit_type='Undefined', flux = None):
 
             if Configuration['OPTIMIZED']:
                 Tirific_Template['INSET'] = f"{Fits_Files['OPTIMIZED_CUBE']}"
             else:
                 Tirific_Template['INSET'] = f"{Fits_Files['FITTING_CUBE']}"
-            #if stage in ['run_ec','initialize_ec']:
-            #    if Configuration['NO_RINGS'] < 5:
-            #        Tirific_Template['INIMODE'] = '1'
-            #    elif Configuration['NO_RINGS'] < 15:
-            #        Tirific_Template['INIMODE'] = '2'
-            #    else:
-            #        Tirific_Template['INIMODE'] = '3'
-            #else:
+
             if Configuration['NO_RINGS'] < 20:
                 Tirific_Template['INIMODE'] = '1'
             elif Configuration['NO_RINGS'] < 30:
                 Tirific_Template['INIMODE'] = '2'
             else:
                 Tirific_Template['INIMODE'] = '3'
 
-            if Configuration['NO_RINGS'] > 3.:
+            if Configuration['NO_RINGS'] > 8.:
 
                 Tirific_Template['INTY'] = 0
                 #Tirific_Template['INDINTY'] = 0
             else:
                 #This should not be used with 8 <  rings.
-                Tirific_Template['INTY'] = 1
+                Tirific_Template['INTY'] = 2
                 #preferably we'd use the akima spline but there is an issue with that where the final ring does not get modified
                 #Tirific_Template['INDINTY'] = 2
             Tirific_Template['NUR'] = f"{Configuration['NO_RINGS']}"
             #current_cwd = os.getcwd()
             short_log = Configuration['LOG_DIRECTORY'].replace(Configuration['FITTING_DIR'],'')
             Tirific_Template['RESTARTNAME'] = f"{short_log}restart_{fit_type}.txt"
             #this could be fancier
-            '''
-            if Configuration['NO_RINGS'] < 3:
-                Tirific_Template['NCORES'] = '2'
-            elif Configuration['NO_RINGS'] < 6:
-                Tirific_Template['NCORES'] = '3'
-            elif Configuration['NO_RINGS'] < 12:
-                Tirific_Template['NCORES'] = '4'
-            else:
-                Tirific_Template['NCORES'] = '6'
-            '''
-
-            Tirific_Template['NCORES'] = Configuration['NCPU']
+            Tirific_Template['NCORES'] = Configuration['PER_GALAXY_NCPU']
 
             Tirific_Template['LOOPS'] = f"{Configuration['LOOPS']}"
             Tirific_Template['DISTANCE'] = f"{Configuration['DISTANCE']}"
             out_keys = ['LOGNAME','OUTSET','TIRDEF']
             out_extensions = ['log','fits','def']
             for i,key in enumerate(out_keys):
                 Tirific_Template[key] = f"{fit_type}/{fit_type}.{out_extensions[i]}"
@@ -2592,16 +3281,16 @@
             elif Configuration['CHANNEL_DEPENDENCY'].lower() == 'independent':
                 instrumental_vres = 0.
             else:
                 raise BadConfigurationError('Something went wrong in the Configuration setup')
 
             Tirific_Template['CONDISP'] = f"{instrumental_vres:.2f}"
             if flux:
-                Tirific_Template['CFLUX'] = f"{set_limits(flux/1.5e7,1e-6,1e-3):.2e}"
-                Tirific_Template['CFLUX_2'] = f"{set_limits(flux/1.5e7,1e-6,1e-3):.2e}"
+                Tirific_Template['CFLUX'] = f"{sf.set_limits(flux/1.5e7,1e-6,1e-3):.2e}"
+                Tirific_Template['CFLUX_2'] = f"{sf.set_limits(flux/1.5e7,1e-6,1e-3):.2e}"
 set_overall_parameters.__doc__ =f'''
  NAME:
     set_overall_parameters
 
  PURPOSE:
     Set the parameters in the tirific file that are singular values that apply to all of the fitting such as names and other issues
 
@@ -2610,18 +3299,16 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
     Tirific_Template = Standard FAT Tirific Template
 
  OPTIONAL INPUTS:
-    debug = False
 
-    stage = 'initial'
-    stage of fitting
+
 
     fit_type='Undefined_Stage'
     type of fitting
 
     flux = None,
     Total flux in the model
 
@@ -2631,69 +3318,159 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
  '''
 
-def set_sbr_fitting(Configuration,systemic = 100., stage = 'no_stage',debug = False):
-    if debug:
-        print_log(f'''SET_SBR_FITTING: We are setting the SBR limits.
+def set_sbr_fitting(Configuration,Tirific_Template, stage = 'no_stage'):
+    sf.print_log(f'''SET_SBR_FITTING: We are setting the SBR limits.
 {'':8s} No_Rings = {Configuration['NO_RINGS']}
-''',Configuration['OUTPUTLOG'],debug = True)
+''',Configuration,case=['debug_start'])
     sbr_input = {}
     inner_ring = 2
+    sbr_profile=np.array(sf.load_tirific(Configuration,Tirific_Template, ['SBR','SBR_2']),dtype=float)
     if stage in ['initial','run_cc','initialize_ec','run_ec','initialize_os','run_os']:
-        radii,sbr_ring_limits = sbr_limits(Configuration,systemic = systemic, debug = debug)
+        radii,sbr_ring_limits = sf.sbr_limits(Configuration,Tirific_Template)
         if stage in ['run_ec','run_os']:
             sbr_ring_limits[-4:]=[x/5 for x in sbr_ring_limits[-4:]]
-        if debug:
-            print_log(f'''SET_SBR_FITTING: Using these SBR limits.
+        sf.print_log(f'''SET_SBR_FITTING: Using these SBR limits.
 {'':8s} limits = {sbr_ring_limits}
 {'':8s} no of limits = {len(sbr_ring_limits)}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
         if stage in ['initial','run_cc']:
             max_size = 4
         elif stage in ['initialize_ec','run_ec','initialize_os','run_os']:
             max_size = 2.
+        #Make sure the SBR profile is not dropping below the minimum we are setting
+
+        fact= [2.,2.]
+        format = sf.set_format('SBR')
+        pmax = copy.deepcopy(sbr_profile)
+        pmin = copy.deepcopy(sbr_profile)
+        pmax[:,:] = 1.
+        pmin[:,:] = 0.
+        for i in [0,1]:
+            if stage in ['initialize_os']:
+                fact[i] = 0.75
+            elif Configuration['SIZE_IN_BEAMS'][i] < max_size:
+                fact[i]=2.5
+
+            for x in range(len(radii)-1,inner_ring-1,-1):
+                if radii[x] < Configuration['SIZE_IN_BEAMS'][i]*Configuration['BEAM'][0]:
+                    sbr_profile[i,x] = sf.set_limits(sbr_profile[i,x],sbr_ring_limits[x]/fact[i]*2.,1.)
+
+                else:
+                    sbr_profile[i,x] = 0.
+            sbr_profile[i,:inner_ring] = [sf.set_limits(x,np.min(sbr_ring_limits),1.) for x in sbr_profile[i,:inner_ring]]
+            if i == 0:
+                ext=''
+            else:
+                ext='_2'
+            Tirific_Template[f"SBR{ext}"]= f"{' '.join([f'{x:{format}}' for x in sbr_profile[i]])}"
+
+        sbr_smoothed_profile = smooth_profile(Configuration,Tirific_Template,'SBR',
+                                min_error= [sbr_ring_limits,sbr_ring_limits],no_apply = True,
+                                fix_sbr_call = True,profile_in = sbr_profile )
+        sbr_av_smoothed = [(x+y)/2. for x,y in zip(sbr_smoothed_profile[0],sbr_smoothed_profile[1])]
+        sf.print_log(f'''SET_SBR_FITTING:
+{'':8s} This is the mean SNR {Configuration['SNR']}
+beamarea = {Configuration['BEAM_AREA']}, channelwidth = {Configuration['CHANNEL_WIDTH']}, noise = {Configuration['NOISE']}
+''',Configuration,case=['debug_add'])
+
+        #if x < 4:
+        limits_for_max = True
+        if Configuration['SNR'] > 10:
+            limits_for_max = False
+            sf.print_log(f'''SET_SBR_FITTING:
+{'':8s} The SNR is so high that we will not use the ring limits for parmax
+''',Configuration,case=['debug_add'])
+
+        for i in [0,1]:
+            mean_signal = Configuration['SNR']*Configuration['NOISE']/\
+                    (Configuration['BEAM_AREA']*Configuration['SIZE_IN_BEAMS'][i]/2.)\
+                    *Configuration['CHANNEL_WIDTH'] #in Jy/arcsec *km/s
+            sf.print_log(f'''SET_SBR_FITTING:
+{'':8s} mean_signal = {mean_signal}
+''',Configuration,case=['debug_add'])
+            for x in range(len(radii)-1,inner_ring-1,-1):
+
+                #    min_max = sf.set_limits(sbr_ring_limits[x]*30.,1e-3,0.9 )
+                #else:
+                #    min_max = sbr_ring_limits[x]*30.
+
+                if  sbr_profile[i,x] > 0.:
+                    if limits_for_max:
+                        pmax[i,x] = sf.set_limits(sbr_av_smoothed[x-1]*20.,sbr_ring_limits[x]*30.,1.)
+                    else:
+                        pmax[i,x] = sf.set_limits(sbr_av_smoothed[x-1]*20.,\
+                            mean_signal*100./(radii[x])**0.5,1.)
+                    pmin[i,x] = sbr_ring_limits[x]/fact[i]
+                else:
+                    if limits_for_max:
+                        pmax[i,x] = sf.set_limits(sbr_av_smoothed[x-1]*5.\
+                        ,sbr_ring_limits[x]*10.,sbr_ring_limits[x]*30.)
+                    else:
+                        pmax[i,x] = sf.set_limits(sbr_av_smoothed[x-1]*5.\
+                        , mean_signal*50./(radii[x])**0.5, mean_signal*200./(radii[x])**0.5)
+                    pmin[i,x] = 0.
 
-        if Configuration['SIZE_IN_BEAMS'] < max_size:
+
+
+        if np.mean(Configuration['SIZE_IN_BEAMS']) < max_size:
             sbr_input['VARY'] =  np.array([f"SBR {x+1} SBR_2 {x+1}" for x in range(len(radii)-1,inner_ring-1,-1)],dtype=str)
-            sbr_input['PARMAX'] = np.array([1 for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float)
+
+
+            sbr_input['PARMAX'] = np.array([sf.set_limits(sbr_av_smoothed[x-1]*10.,np.mean(pmax[:,x]),1.) for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float)
             #if stage in ['initial','run_cc']:
             #    sbr_input['PARMIN'] = np.array([sbr_ring_limits[x]/2. if x <= (3./4.)*len(radii) else 0 for x in range(len(radii)-1,inner_ring-1,-1)])
             #elif stage in ['initialize_ec','run_ec']:
-            sbr_input['PARMIN'] = np.array([sbr_ring_limits[x]/1.5 for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float)
+
+            sbr_input['PARMIN'] = np.array([sbr_ring_limits[x]/np.max(fact) for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float)
             sbr_input['MODERATE'] = np.array([5 for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float) #How many steps from del start to del end
             sbr_input['DELSTART'] = np.array([1e-4 for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float) # Starting step
             sbr_input['DELEND'] = np.array([2.5e-6 for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float) #Ending step
             sbr_input['MINDELTA'] = np.array([5e-6 for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float) #saturation criterum when /SIZE SIZE should be 10 troughout the code
         else:
             sbr_input['VARY'] =  np.array([[f"SBR {x+1}",f"SBR_2 {x+1}"] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=str).reshape((len(radii)-inner_ring)*2)
-            sbr_input['PARMAX'] = np.array([[1,1] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2)
+
+
+
+
+            #pmax = np.array([np.full(2,sf.set_limits(sbr_av_smoothed[x-1]*20.,sbr_ring_limits[x]*30.,1.)) for x in range(len(radii)-1,inner_ring-1,-1)], dtype=float)
+            sbr_input['PARMAX'] = np.array([[pmax[0,x],pmax[1,x]] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2)
+            #sbr_input['PARMAX'] = np.array([[sf.set_limits(sbr_smoothed_profile[0,x-1]*20.,sbr_ring_limits[x]*30.,1.),sf.set_limits(sbr_smoothed_profile[1,x-1]*20.,sbr_ring_limits[x]*30.,1.)] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2)
         #if stage in ['initial','run_cc']:
             #    sbr_input['PARMIN'] = np.array([[sbr_ring_limits[x]/2.,sbr_ring_limits[x]/2.] if x <= (3./4.)*len(radii) else [0.,0.] for x in range(len(radii)-1,inner_ring-1,-1)]).reshape((len(radii)-inner_ring)*2)
             #elif stage in ['initialize_ec','run_ec']:
-            sbr_input['PARMIN'] = np.array([[sbr_ring_limits[x]/4.,sbr_ring_limits[x]/4.] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2)
+            sbr_input['PARMIN']  = np.array([[pmin[0,x],pmin[1,x]] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2)
+            #sbr_input['PARMIN'] = np.array([[sbr_ring_limits[x]/fact[0],sbr_ring_limits[x]/fact[1]] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2)
             sbr_input['MODERATE'] = np.array([[5,5] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2) #How many steps from del start to del end
             sbr_input['DELSTART'] = np.array([[1e-4,1e-4] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2) # Starting step
             sbr_input['DELEND'] = np.array([[sbr_ring_limits[x]/20.,sbr_ring_limits[x]/20.] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2)
             sbr_input['MINDELTA'] = np.array([[sbr_ring_limits[x]/20.,sbr_ring_limits[x]/20.] for x in range(len(radii)-1,inner_ring-1,-1)],dtype=float).reshape((len(radii)-inner_ring)*2)
 
         sbr_input['VARY'] = np.concatenate((sbr_input['VARY'],[f"SBR {' '.join([str(int(x)) for x in range(1,inner_ring+1)])} SBR_2 {' '.join([str(int(x)) for x in range(1,inner_ring+1)])}"]),axis=0)
-        sbr_input['PARMAX'] = np.concatenate((sbr_input['PARMAX'],[2e-3]))
-        sbr_input['PARMIN'] = np.concatenate((sbr_input['PARMIN'],[np.min(sbr_ring_limits)]))
+        if limits_for_max:
+            sbr_input['PARMAX'] = np.concatenate((sbr_input['PARMAX'],[sf.set_limits(np.mean([sbr_smoothed_profile[0,2:4],sbr_smoothed_profile[1,2:4]])*4.,sbr_ring_limits[2],np.max(sbr_profile))]))
+        else:
+            sbr_input['PARMAX'] = np.concatenate((sbr_input['PARMAX'],[sf.set_limits(np.mean([sbr_smoothed_profile[0,2:4],sbr_smoothed_profile[1,2:4]])*4.,mean_signal*100,1.)]))
+
+        if Configuration['CENTRAL_CONVERGENCE']:
+            sbr_input['PARMIN'] = np.concatenate((sbr_input['PARMIN'],[np.min(sbr_ring_limits)]))
+        else:
+            sbr_input['PARMIN'] = np.concatenate((sbr_input['PARMIN'],[sbr_ring_limits[inner_ring]*1.5]))
         sbr_input['MODERATE'] = np.concatenate((sbr_input['MODERATE'],[5]))
         sbr_input['DELSTART'] = np.concatenate((sbr_input['DELSTART'],[1e-5]))
         sbr_input['DELEND'] = np.concatenate((sbr_input['DELEND'],[1e-6]))
         sbr_input['MINDELTA'] = np.concatenate((sbr_input['MINDELTA'],[2e-6]))
     elif stage in ['after_cc','after_ec','after_os']:
         #Used in Fit_Smoothed_Check
         sbr_input['VARY'] = [f"SBR 3:{Configuration['NO_RINGS']}, SBR_2 3:{Configuration['NO_RINGS']}"]
-        sbr_input['PARMAX'] = np.concatenate(([2e-3],[2e-3]))
+        sbr_input['PARMAX'] = np.concatenate(([np.max(sbr_profile[0,2:])*3.],[np.max(sbr_profile[1,2:])*3.]))
         sbr_input['PARMIN'] = np.concatenate(([0],[0]))
         sbr_input['MODERATE'] = np.concatenate(([5],[5]))
         sbr_input['DELSTART'] = np.concatenate(([1e-5],[1e-5]))
         sbr_input['DELEND'] = np.concatenate(([1e-6],[1e-6]))
         sbr_input['MINDELTA'] = np.concatenate(([2e-6],[2e-6]))
 
     return sbr_input
@@ -2708,17 +3485,16 @@
     modify_template
 
  INPUTS:
     Configuration = Standard FAT configuration
 
 
  OPTIONAL INPUTS:
-    debug = False
 
-    systemic = 100.
+
     systemic velocity of the source
 
     stage = 'no_stage'
     stage of the fitting
 
  OUTPUTS:
     a fitting dictionary
@@ -2727,23 +3503,22 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def set_vrot_fitting(Configuration, stage = 'initial', rotation = [100,5.], debug = False):
+def set_vrot_fitting(Configuration, stage = 'initial', rotation = [100,5.]):
     NUR = Configuration['NO_RINGS']
     vrot_input = {}
 
-    if debug:
-        print_log(f'''SET_VROT_FITTING: We are setting the VROT limits.
+    sf.print_log(f'''SET_VROT_FITTING: We are setting the VROT limits.
 {'':8s} No_Rings = {Configuration['NO_RINGS']}
 {'':8s} Limits = {Configuration['VROT_CURRENT_BOUNDARY'][0]}
-''',Configuration['OUTPUTLOG'],debug = True)
+''',Configuration,case=['debug_start'])
     if stage in ['final_os']:
         modifier= [Configuration['LIMIT_MODIFIER'][0]/2.,Configuration['LIMIT_MODIFIER'][0],Configuration['LIMIT_MODIFIER'][0]/4.]
     elif stage in ['after_os']:
         modifier= [Configuration['LIMIT_MODIFIER'][0]/3.,Configuration['LIMIT_MODIFIER'][0]/2.,Configuration['LIMIT_MODIFIER'][0]/5.]
     else:
         modifier= [Configuration['LIMIT_MODIFIER'][0]/2,Configuration['LIMIT_MODIFIER'][0],Configuration['LIMIT_MODIFIER'][0]/3.]
 
@@ -2763,15 +3538,15 @@
     #if there is not values in the center we connect the inner ring to the next ring
     forvarindex = ''
     if Configuration['NO_RINGS'] > 5:
         if Configuration['EXCLUDE_CENTRAL'] or rotation[0] > 150.:
             forvarindex = 'VROT 2 VROT_2 2 '
         if Configuration['OUTER_SLOPE_START'] == NUR:
             if Configuration['NO_RINGS'] > 5:
-                inner_slope =  int(round(set_limits(Configuration['RC_UNRELIABLE'],round(NUR/2.),NUR-1)))
+                inner_slope =  int(round(sf.set_limits(Configuration['RC_UNRELIABLE'],round(NUR/2.),NUR-1)))
             else:
                 inner_slope = NUR
             if Configuration['NO_RINGS'] > 15 and inner_slope > int(Configuration['NO_RINGS']*4./5.) :
                 inner_slope = int(Configuration['NO_RINGS']*4./5.)
             Configuration['OUTER_SLOPE_START'] = inner_slope
         else:
             inner_slope = Configuration['OUTER_SLOPE_START']
@@ -2801,15 +3576,15 @@
  CATEGORY:
     modify_template
 
  INPUTS:
     Configuration = Standard FAT configuration
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     stage = 'initial'
     stage of the fitting
 
     rotation = [100,5.]
     estimate of mean rotation curve and error
 
@@ -2820,59 +3595,66 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def smooth_profile(Configuration,Tirific_Template,key,min_error = 0.,debug=False ,profile_in = None, no_apply =False,fix_sbr_call = False):
-
+def smooth_profile(Configuration,Tirific_Template,key,min_error = 0.  \
+                    ,profile_in = None, no_apply =False,no_fix = False,fix_sbr_call=False):
+    sf.print_log(f'''SMOOTH_PROFILE: Starting to smooth the {key} profile.
+''',Configuration,case= ['debug_start'])
     if key == 'SBR' and not fix_sbr_call:
         error_message = f'''SMOOTH_PROFILE: Do not use smooth_profile for the SBR, SBR is regularised in fix_sbr'''
-        print_log(error_message,Configuration['OUTPUTLOG'],screen=True,debug = debug)
+        sf.print_log(error_message,Configuration,\
+            case= ['main','screen'])
+        raise FunctionCallError(error_message)
+    if fix_sbr_call:
+        no_fix=True
+    if key in 'ARBITRARY' and (profile_in is None or no_apply is not True):
+        error_message = f'''SMOOTH_PROFILE: We cannot read or write an ARBITRARY profile from the template.'''
+        sf.print_log(error_message,Configuration,\
+            case= ['main','screen'])
         raise FunctionCallError(error_message)
 
-    if debug:
-        print_log(f'''SMOOTH_PROFILE: Starting to smooth the {key} profile.
-''',Configuration['OUTPUTLOG'],debug = True)
 
     if profile_in is None:
-        profile = np.array(get_from_template(Configuration,Tirific_Template,[key,f"{key}_2"]),dtype = float)
+        profile = np.array(sf.load_tirific(Configuration,Tirific_Template,[key,f"{key}_2"]),dtype = float)
     else:
         profile= copy.deepcopy(profile_in)
 
     original_profile = copy.deepcopy(profile)
     min_error = np.array(min_error,dtype=float)
     if min_error.size == 1:
         min_error = np.full(profile.size,min_error)
-    if key in ['INCL','Z0', 'PA']:
+    if key in ['INCL','Z0', 'PA','ARBITRARY']:
         inner_fixed = Configuration['INNER_FIX']
     elif key in ['SDIS']:
         inner_fixed = [4,4]
     else:
         inner_fixed = [0,0]
 
-    #he sbr profile is already fixed before geting to the smoothing
-    if not fix_sbr_call:
-        profile =fix_profile(Configuration, key, profile, Tirific_Template,inner_fix = inner_fixed,debug=debug)
+    #he sbr profile is already fixed before getting to the smoothing
+    if not no_fix:
+        profile =fix_profile(Configuration, key, profile, Tirific_Template,\
+                    inner_fix = inner_fixed)
 
     if key == 'VROT':
         #if profile[0,1] > profile[0,2] or np.mean(profile[1:3]) > 120.:
-        if np.mean(profile[1:3]) > 120.:
+        if np.mean([profile[0][1:3],profile[1][1:3]]) > 120.:
             shortened =True
             profile = np.delete(profile, 0, axis = 1)
         else:
             shortened = False
-    if debug:
-        print_log(f'''SMOOTH_PROFILE: retrieved profile.
+    sf.print_log(f'''SMOOTH_PROFILE: retrieved profile.
 {'':8s}{profile}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
     # savgol filters do not work for small array
     for i in [0,1]:
-        if len(profile[i]) < 8:
+        if len(profile[i]) <= 8:
             #In this case we are using a cubic spline so no smoothing required
             pass
         elif len(profile[i]) < 15:
             profile[i] = savgol_filter(profile[i], 3, 1)
         elif len(profile[i]) < 20:
             profile[i] = savgol_filter(profile[i], 5, 2)
         elif len(profile[i]) < 25:
@@ -2884,53 +3666,51 @@
             if below_zero.size > 0.:
                 profile[i,below_zero] = min_error[i,below_zero]
             below_zero = np.where(profile[i,int(len(profile)/2.):] < 0.)[0]+int(len(profile)/2.)
             if below_zero.size > 0.:
                 profile[i,below_zero] = profile[i,below_zero-1]/2.
 
     # Fix the settings
-    format = set_format(key)
+    format = sf.set_format(key)
     if key == 'VROT':
         if shortened:
             tmp = [[],[]]
             tmp[0] = np.hstack([[0.], profile[0]])
             tmp[1] = np.hstack([[0.], profile[1]])
             profile =  np.array(tmp,dtype=float)
         else:
             profile[:,0] = 0.
 
-    if not fix_sbr_call:
-        profile =fix_profile(Configuration, key, profile, Tirific_Template,inner_fix=inner_fixed,debug=debug)
+    if not no_fix:
+        profile =fix_profile(Configuration, key, profile, Tirific_Template,inner_fix=inner_fixed)
 
 
-    if debug:
-        print_log(f'''SMOOTH_PROFILE: profile after smoothing.
+    sf.print_log(f'''SMOOTH_PROFILE: profile after smoothing.
 {'':8s}{profile}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
     if not no_apply:
-        weights = get_ring_weights(Configuration,Tirific_Template,debug=debug)
-        errors = get_error(Configuration,original_profile,profile,key,weights = weights, min_error=min_error,debug=debug)
+        weights = sf.get_ring_weights(Configuration,Tirific_Template)
+        errors = get_error(Configuration,original_profile,profile,key,weights = weights, min_error=min_error)
         if key not in ['VROT']:
             # Check whether it should be flat
-            profile,errors =modify_flat(Configuration,profile,original_profile,errors,key,inner_fix=inner_fixed,debug=debug)
+            profile,errors =modify_flat(Configuration,profile,original_profile,errors,key,inner_fix=inner_fixed)
 
         Tirific_Template[key]= f"{' '.join([f'{x:{format}}' for x in profile[0,:int(Configuration['NO_RINGS'])]])}"
         Tirific_Template[f"{key}_2"]= f"{' '.join([f'{x:{format}}' for x in profile[1,:int(Configuration['NO_RINGS'])]])}"
         Tirific_Template.insert(key,f"# {key}_ERR",f"{' '.join([f'{x:{format}}' for x in errors[0,:int(Configuration['NO_RINGS'])]])}")
         Tirific_Template.insert(f"{key}_2",f"# {key}_2_ERR",f"{' '.join([f'{x:{format}}' for x in errors[1,:int(Configuration['NO_RINGS'])]])}")
         #if key in ['INCL'] and np.mean( profile[:,int(Configuration['NO_RINGS']/2.):int(Configuration['NO_RINGS'])]) < 40.:
-        #    fix_vrot_for_incl_change(Configuration,Tirific_Template,original_profile,profile,debug=debug)
+        #    fix_vrot_for_incl_change(Configuration,Tirific_Template,original_profile,profile)
 
-        if debug:
-            print_log(f'''SMOOTH_PROFILE: This has gone to the template
+        sf.print_log(f'''SMOOTH_PROFILE: This has gone to the template
 {'':8s}{key} = {Tirific_Template[key]}
 {'':8s}{key}_2 ={Tirific_Template[f"{key}_2"]}
 {'':8s}# {key}_ERR ={Tirific_Template[f"# {key}_ERR"]}
 {'':8s}# {key}_2_ERR ={Tirific_Template[f"# {key}_2_ERR"]}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
 
     return profile
 smooth_profile.__doc__ =f'''
  NAME:
     smooth_profile
 
  PURPOSE:
@@ -2941,15 +3721,15 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = Standard FAT Template
     key = Tirific value to be smoothed
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     min_error = 0.
     The minimum eror that should be used
 
     profile_in = None
     if provided this will be smoothed instead of the key being extracted from the Template
 
@@ -2968,31 +3748,29 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  EXAMPLE:
 '''
 
-def update_disk_angles(Configuration,Tirific_Template,debug = False):
+def update_disk_angles(Configuration,Tirific_Template):
     extension = ['','_2']
     for ext in extension:
-        PA = np.array(get_from_template(Configuration,Tirific_Template,[f'PA{ext}'],debug=debug),dtype=float)[0]
-        inc = np.array(get_from_template(Configuration,Tirific_Template,[f'INCL{ext}'],debug=debug),dtype=float)[0]
-        if debug:
-            print_log(f'''UPDATE_DISK_ANGLES: abtained  this from the template
+        PA = np.array(sf.load_tirific(Configuration,Tirific_Template,[f'PA{ext}']),dtype=float)
+        inc = np.array(sf.load_tirific(Configuration,Tirific_Template,[f'INCL{ext}']),dtype=float)
+        sf.print_log(f'''UPDATE_DISK_ANGLES: abtained  this from the template
 {'':8s} inc{ext} = {inc}
 {'':8s} PA{ext} = {PA}
-''', Configuration['OUTPUTLOG'])
+''', Configuration,case= ['debug_start'])
         angle_adjust=np.array(np.tan((PA[0]-PA)*np.cos(inc*np.pi/180.)*np.pi/180.)*180./np.pi,dtype = float)
         if ext == '_2':
             angle_adjust[:] +=180.
-        if debug:
-            print_log(f'''UPDATE_DISK_ANGLES: adusting AZ1P{ext} with these angles
+        sf.print_log(f'''UPDATE_DISK_ANGLES: adusting AZ1P{ext} with these angles
 {'':8s}{angle_adjust}
-''', Configuration['OUTPUTLOG'])
+''', Configuration,case= ['debug_add'])
         Tirific_Template.insert(f'AZ1W{ext}',f'AZ1P{ext}',f"{' '.join([f'{x:.2f}' for x in angle_adjust])}")
 update_disk_angles.__doc__ =f'''
  NAME:
     update_disk_angles
 
  PURPOSE:
     Update the AZ1W and AZ1P parameters to match the warp
@@ -3001,33 +3779,33 @@
     modify_template
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = Standard FAT Tirific Template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     Updated template
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def write_center(Configuration,Tirific_Template,center,debug=False):
+def write_center(Configuration,Tirific_Template,center ):
     extension = ['','_2']
     variables = ['XPOS','YPOS','VSYS']
     for i,var in enumerate(variables):
         values= [center[i]]*int(Tirific_Template['NUR'])
-        format= set_format(var)
+        format= sf.set_format(var)
         for ext in extension:
             Tirific_Template[f"{var}{ext}"] = f"{' '.join([f'{x:{format}}' for x in values])}"
 
 write_center.__doc__ =f'''
  NAME:
     write_center
 
@@ -3039,15 +3817,15 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = Standard FAT Tirific Template
     center = [xpos,ypos,vsys]
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     Updated template
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
@@ -3055,25 +3833,26 @@
 
  NOTE:
 '''
 
 
 def write_new_to_template(Configuration, filename,Tirific_Template, Variables = ['VROT',
                  'Z0', 'SBR', 'INCL','PA','XPOS','YPOS','VSYS','SDIS','VROT_2',  'Z0_2','SBR_2',
-                 'INCL_2','PA_2','XPOS_2','YPOS_2','VSYS_2','SDIS_2'], debug = False):
+                 'INCL_2','PA_2','XPOS_2','YPOS_2','VSYS_2','SDIS_2']):
+    '''Write a def file into the template'''
     with open(filename, 'r') as tmp:
         # Separate the keyword names
         for line in tmp.readlines():
             key = str(line.split('=')[0].strip().upper())
             if key in Variables:
                 Tirific_Template[key] = str(line.split('=')[1].strip())
     # If we have written the INCL we need to update the limit modifier
     if 'INCL' in Variables or 'INCL_2' in Variables:
         Inclination = np.array([(float(x)+float(y))/2. for x,y in zip(Tirific_Template['INCL'].split(),Tirific_Template['INCL_2'].split())],dtype=float)
-        set_limit_modifier(Configuration,Inclination,debug= debug)
+        sf.set_limit_modifier(Configuration,Tirific_Template)
 write_new_to_template.__doc__ =f'''
  NAME:
     write_new_to_template
 
  PURPOSE:
     Write a def file into the template
 
@@ -3082,15 +3861,15 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     filename = the name of the def file
     Tirific_Template = Standard FAT Tirific Template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     Variables = ['VROT', 'Z0', 'SBR', 'INCL','PA','XPOS','YPOS','VSYS','SDIS','VROT_2',  'Z0_2','SBR_2',
                  'INCL_2','PA_2','XPOS_2','YPOS_2','VSYS_2','SDIS_2']
     the parameters to be updated from the file
 
  OUTPUTS:
     The template is updated
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/Support/read_functions.py` & `pyFAT_astro-0.1.1/pyFAT_astro/Support/read_functions.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # -*- coding: future_fstrings -*-
 # This module contains a set of functions and classes that are used in FAT to read input files
 
-from pyFAT_astro.Support.support_functions import Proper_Dictionary,print_log,convertRADEC,set_limits, remove_inhomogeneities, \
-                                obtain_border_pix, get_inclination_pa,get_vel_pa,columndensity,get_profile, get_kinematical_center,\
-                                create_directory,copy_homemade_sofia,clean_header,get_new_center,update_statistic,set_boundaries
-from pyFAT_astro.Support.fits_functions import check_mask,clean_header,create_fat_cube
-from pyFAT_astro.Support.fat_errors import BadCatalogueError, NoConfigFile
+from pyFAT_astro.Support.fits_functions import check_mask,create_fat_cube
+from pyFAT_astro.Support.fat_errors import BadCatalogueError, NoConfigFile, \
+    BadSourceError
+from pyFAT_astro.Support.modify_template import fix_sbr
+import pyFAT_astro.Support.support_functions as sf
+import pyFAT_astro
+
 
 from astropy.io import fits
 from astropy.wcs import WCS
 from scipy import ndimage
 import warnings
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
@@ -34,31 +36,57 @@
 import traceback
 
 
 from pyFAT_astro import Templates as templates
 #Function to read a FAT input Catalogue
 
 
-def catalogue(filename, debug = False):
-    Catalogue = Proper_Dictionary({})
+def catalogue(filename,split_char='|'):
+    Catalogue = sf.Proper_Dictionary({})
     with open(filename,'r') as tmpfile:
-        #Define the exsiting catalogue input()
-        input_columns = [x.strip().upper() for x in tmpfile.readline().split('|')]
-        Catalogue['ENTRIES'] = ['ENTRIES']
-        Catalogue['ENTRIES'].extend(input_columns)
+        firstline = tmpfile.readline()
+        all_columns_check = False
+        required_columns= ['ID','DISTANCE','DIRECTORYNAME','CUBENAME']
+
+        while not all_columns_check:
+            input_columns = [x.strip().upper() for x in firstline.split(split_char)]
+            Catalogue['ENTRIES'] = ['ENTRIES']
+            Catalogue['ENTRIES'].extend(input_columns)
+            required_columns= ['ID','DISTANCE','DIRECTORYNAME','CUBENAME']
+
+            for key in required_columns:
+                if key not in Catalogue['ENTRIES']:
+                    if split_char == '|':
+                        print(f'Key {key} not found')
+                        split_char=' '
+                        all_columns_check = False
+                        break
+                    else:
+                        raise BadCatalogueError(f'We can not find the column for {key} in your input catalogue')
+                else:
+                    all_columns_check = True
+                    continue
+
+
+
         for key in input_columns:
             Catalogue[key] = []
 
+
         for line in tmpfile.readlines():
-            input = [x.strip() for x  in line.split('|')]
-            for i,key in enumerate(input_columns):
-                if key == 'DISTANCE':
-                    Catalogue[key].append(float(input[i]))
-                else:
-                    Catalogue[key].append(input[i])
+            input = [x.strip() for x  in line.split(split_char)]
+            if len(input) == len(input_columns):
+                for i,key in enumerate(input_columns):
+                    if key == 'DISTANCE':
+                        Catalogue[key].append(float(input[i]))
+                    else:
+                        Catalogue[key].append(input[i])
+            else:
+                print(f'READ_CATALOGUE: Your line "{line}" in the input catalogue does not have correct number of columns, skipping it')
+
     #if 'NUMBER' in Catalogue['ENTRIES']:
     #    Catalogue['NUMBER'] = np.array(Catalogue['NUMBER'],dtype=int)
 
     return Catalogue
 catalogue.__doc__ =f'''
  NAME:
     catalogue
@@ -69,46 +97,46 @@
  CATEGORY:
     read_functions
 
  INPUTS:
     filename = name of the catalogue to read
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     Catalogue = dictionary with the read file
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def check_edge_limits(xmin,xmax,ymin,ymax,zmin,zmax,Configuration,debug=False ,beam_edge = 0.5, vel_edge = 0.5 ):
+def check_edge_limits(xmin,xmax,ymin,ymax,zmin,zmax,Configuration ,beam_edge = 0.5, vel_edge = 0.5 ):
     diff = np.array([xmin,abs(xmax - Configuration['NAXES'][0]),
                      ymin,abs(ymax - Configuration['NAXES'][1])],dtype = float)
-    if debug:
-        print_log(f'''CHECK_EDGE_LIMIT: We find these differences and this edge size {beam_edge*Configuration['BEAM_IN_PIXELS'][0]}
+    sf.print_log(f'''CHECK_EDGE_LIMIT: We find these differences and this edge size {beam_edge*Configuration['BEAM_IN_PIXELS'][0]}
 {'':8s} diff  = {diff}
-''',Configuration['OUTPUTLOG'],debug= True)
+''',Configuration, case=['debug_start'])
     if np.where(diff < beam_edge*Configuration['BEAM_IN_PIXELS'][0])[0].size:
         return True
     diff = np.array([zmin,abs(zmax-Configuration['NAXES'][2])],dtype=float)
-    if debug:
-        print_log(f'''CHECK_EDGE_LIMIT: And for velocity edge =  {vel_edge}
+    sf.print_log(f'''CHECK_EDGE_LIMIT: And for velocity edge =  {vel_edge}
 {'':8s} diff  = {diff}
-''',Configuration['OUTPUTLOG'])
+''',Configuration, case=['debug_add'])
     if np.where(diff < vel_edge)[0].size:
-        print_log(f"On the edge",Configuration['OUTPUTLOG'])
+        sf.print_log(f"CHECK_EDGE_LIMIT: On the edge",Configuration,\
+            case=['verbose'])
         return True
     else:
-        print_log(f"Off the edge",Configuration['OUTPUTLOG'])
+        sf.print_log(f"CHECK_EDGE_LIMIT: Off the edge",Configuration,\
+            case=['verbose'])
         return False
 check_edge_limits.__doc__ =f'''
  NAME:
     check_edge_limits
 
  PURPOSE:
     Check whether a Sofia source is properly separated from the edge of the cube.
@@ -118,16 +146,14 @@
     read_functions
 
  INPUTS:
     xmin,xmax,ymin,ymax,zmin,zmax,header,Configuration
     these are the parameters that describe the mask + header + Configuration
 
  OPTIONAL INPUTS:
-    debug=False
-
     beam_edge = 0.5
     minimum tolerance for spatial edges
 
     vel_edge = 0.5
     minimum tolerance for velocity
 
  OUTPUTS:
@@ -137,29 +163,27 @@
 
  PROCEDURES CALLED:
     abs, np.where, np.array, print_log,
 
  NOTE:
 '''
 
-def extract_vrot(Configuration,map ,angle,center, debug= False):
-    if debug:
-        print_log(f'''EXTRACT_VROT: starting extraction of initial VROT.
+def extract_vrot(Configuration,map ,angle,center):
+    sf.print_log(f'''EXTRACT_VROT: starting extraction of initial VROT.
 {'':8s} PA= {angle}
 {'':8s} center= {center}
-''',Configuration['OUTPUTLOG'], debug = True)
-    maj_profile,maj_axis,maj_resolution = get_profile(Configuration,map,angle,center=center,debug=debug)
+''',Configuration, case=['debug_start'])
+    maj_profile,maj_axis,maj_resolution = sf.get_profile(Configuration,map,angle,center=center)
     # We should base extracting the RC on where the profile is negative and positive to avoid mistakes in the ceneter coming through
     neg_index = np.where(maj_profile < 0.)[0]
     pos_index = np.where(maj_profile > 0.)[0]
 
-    if debug:
-        print_log(f'''EXTRACT_VROT: The resolution on the extracted axis
+    sf.print_log(f'''EXTRACT_VROT: The resolution on the extracted axis
 {'':8s} resolution = {maj_resolution}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
     avg_profile = []
     neg_profile = []
     #pos_profile = []
     diff = 0.
     counter = 1.
     for i in range(np.nanmin([neg_index.size,pos_index.size])):
         if not np.all(np.isnan([maj_profile[neg_index[neg_index.size-i-1]],-1*maj_profile[pos_index[i]]])):
@@ -180,49 +204,45 @@
         if Configuration['BEAM_IN_PIXELS'][0]/maj_resolution < i < -2.*beam_back:
             avg_profile[beam_back] = avg_profile[beam_back]+0.25*avg_profile[int(beam_back/2.)]+0.1*avg_profile[-1]
         elif -2.*beam_back <= i < -3.*beam_back:
             avg_profile[beam_back] = avg_profile[beam_back]+0.25/counter*avg_profile[int(beam_back/2.)]+0.1/counter*avg_profile[-1]
             counter += 1
             #neg_profile[beam_back] = neg_profile[beam_back]+0.5*neg_profile[int(beam_back/2.)]+0.1*neg_profile[-1]
             #pos_profile[beam_back] = pos_profile[beam_back]+0.5*pos_profile[int(beam_back/2.)]+0.1*pos_profile[-1]
-    if debug:
-        print_log(f'''EXTRACT_VROT: starting extraction of initial VROT.
-''',Configuration['OUTPUTLOG'])
+    sf.print_log(f'''EXTRACT_VROT: starting extraction of initial VROT.
+''',Configuration,case= ['debug_add'])
     ring_size_req = Configuration['BEAM_IN_PIXELS'][0]/maj_resolution
-    if debug:
-        print_log(f'''EXTRACT_VROT: We need a rings size of
+    sf.print_log(f'''EXTRACT_VROT: We need a rings size of
 {'':8s} ringsize= {ring_size_req}
 {'':8s} because bmaj in pixels  ={Configuration['BEAM_IN_PIXELS'][0]}  and the resolution of the profile = {maj_resolution} pixels
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
     profile = np.array(avg_profile[0::int(ring_size_req)],dtype=float)
 
     try:
         profile[np.isnan(profile)] = profile[~np.isnan(profile)][-1]
     except IndexError:
         profile = []
 
     if len(profile) < 1:
         if len(avg_profile) > 0.:
             profile = np.array([np.max(avg_profile)],dtype=float)
         else:
             profile = np.array([Configuration['CHANNEL_WIDTH']*2.],dtype=float)
-    if debug:
-        print_log(f'''EXTRACT_VROT: Unlimited profile
+    sf.print_log(f'''EXTRACT_VROT: Unlimited profile
 {'':8s} unlimited  RC= {profile}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
     profile[profile > 300.] = 300.
     profile[profile < Configuration['CHANNEL_WIDTH']*2.] = Configuration['CHANNEL_WIDTH']*2.
 
 
     #profile[0] = 0.
-    if debug:
-        print_log(f'''EXTRACT_VROT: Constructing the final RC
+    sf.print_log(f'''EXTRACT_VROT: Constructing the final RC
 {'':8s} initial RC= {profile}
 {'':8s} at step width= {ring_size_req}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
     return profile
 extract_vrot.__doc__ =f'''
  NAME:
     extract_vrot
 
  PURPOSE:
     Extract a profile from the velocity field and average it over both sides from the center.
@@ -233,34 +253,36 @@
  INPUTS:
     Configuration = Standard FAT configuration
     map = the velocity field
     angle = PA of major axis
     center = center of the galaxy in pixel coordinates
 
  OPTIONAL INPUTS:
-    debug = False
+
     fit_type = 'Undefined'
 
  OUTPUTS:
     profile = The RC at given ring locations averaged over the approaching and receding side
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def get_DHI(Configuration,Model='Finalmodel' ,debug=False):
+def get_DHI(Configuration,Model='Finalmodel' ):
     #Get the sbrs
-    radi,sbr,sbr_2,systemic = load_tirific(Configuration,f"{Configuration['FITTING_DIR']}{Model}/{Model}.def",Variables = ['RADI','SBR','SBR_2','VSYS'],debug=debug)
+    radi,sbr,sbr_2,systemic = sf.load_tirific(Configuration,\
+        f"{Configuration['FITTING_DIR']}{Model}/{Model}.def",\
+        Variables = ['RADI','SBR','SBR_2','VSYS'],array=True)
     #convert to solar_mass/pc^2
-    sbr_msolar = columndensity(Configuration,sbr*1000.,systemic=systemic[0],arcsquare=True,solar_mass_output=True)
-    sbr_2_msolar = columndensity(Configuration,sbr_2*1000.,systemic=systemic[0],arcsquare=True,solar_mass_output=True)
+    sbr_msolar = sf.columndensity(Configuration,sbr*1000.,systemic=systemic[0],arcsquare=True,solar_mass_output=True)
+    sbr_2_msolar = sf.columndensity(Configuration,sbr_2*1000.,systemic=systemic[0],arcsquare=True,solar_mass_output=True)
     # interpolate these to ~1" steps
     new_radii = np.linspace(0,radi[-1],int(radi[-1]))
     new_sbr_msolar = np.interp(new_radii,radi,sbr_msolar)
     new_sbr_2_msolar = np.interp(new_radii,radi,sbr_2_msolar)
 
     index_1 = np.where(new_sbr_msolar > 1.)[0]
     index_2 = np.where(new_sbr_2_msolar > 1.)[0]
@@ -283,35 +305,37 @@
  CATEGORY:
     read_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     Model = 'Finalmodel'
     location of the def file to get DHI from. it should be in the fitting dir in the {{Model}}/{{Model}}.def
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def get_totflux(Configuration,map_name,debug=False):
+def get_totflux(Configuration,map_name):
     image = fits.open(f"{Configuration['FITTING_DIR']}{map_name}")
-    flux = np.nansum(image[0].data)
+    #We are taking these from the moment map so we have to divide out the km/s
+    flux = float(np.nansum(image[0].data)/Configuration['BEAM_IN_PIXELS'][2]/Configuration['CHANNEL_WIDTH'])
+    #Should this not have an additional channel width parameter
     error = np.sqrt((np.where(image[0].data> 0.)[0].size)/Configuration['BEAM_IN_PIXELS'][2])*Configuration['NOISE']
     image.close()
-    return [float(flux/Configuration['BEAM_IN_PIXELS'][2]),error]
+    return [flux,error]
 get_totflux.__doc__ =f'''
  NAME:
     get_totflux
 
  PURPOSE:
     Get the total flux from a intensity map
 
@@ -319,107 +343,158 @@
     read_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     map_name = name of the intensity fits file
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     total flux in the map in Jy*km/s
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 # Function to get the PA and inclination from the moment 0 for initial estimates
-def guess_orientation(Configuration,Fits_Files, v_sys = -1 ,center = None, debug = False):
+def guess_orientation(Configuration,Fits_Files, vsys = -1 ,center = None, smooth = False):
     #open the moment 0
 
-    print_log(f'''GUESS_ORIENTATION: starting extraction of initial parameters.
-''',Configuration['OUTPUTLOG'], debug = debug, screen =True)
-    update_statistic(Configuration, message= "Starting the guess orientation run", debug=debug)
+    sf.print_log(f'''GUESS_ORIENTATION: starting extraction of initial parameters.
+''',Configuration, case=['debug_start','verbose'])
+    sf.update_statistic(Configuration, message= "Starting the guess orientation run")
 
-    Image = fits.open(f"{Configuration['FITTING_DIR']}Sofia_Output/{Fits_Files['MOMENT0']}",\
+    Image = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MOMENT0']}",\
             uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
     map = Image[0].data
     hdr = Image[0].header
     mom0 = copy.deepcopy(Image)
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         mom0_wcs = WCS(hdr)
     Image.close()
 
     if not center:
         center = [hdr['NAXIS1']/2.-1,hdr['NAXIS2']/2.-1]
-    Image = fits.open(f"{Configuration['FITTING_DIR']}Sofia_Output/{Fits_Files['CHANNEL_MAP']}",\
+    Image = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['CHANNEL_MAP']}",\
             uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
     noise_map = np.sqrt(Image[0].data)*Configuration['NOISE']*Configuration['CHANNEL_WIDTH']
 
+    #these guesses get thrown off for very large galaxies so smooth when we have those:
+    if smooth:
+        sigma = sf.set_limits(Configuration['BEAM_IN_PIXELS'][0]*Configuration['MAX_SIZE_IN_BEAMS']/12.*2.,Configuration['BEAM_IN_PIXELS'][0],Configuration['BEAM_IN_PIXELS'][0]*5)
+        sf.print_log(f'''GUESS_ORIENTATION: We are smoothing the maps with {sigma} pixels
+''',Configuration,case= ['debug_add'])
+        tmp =  ndimage.gaussian_filter(map, sigma=(sigma, sigma), order=0)
+        tmp[map <= 0.] = 0.
+        map = copy.deepcopy(tmp)
+        if Configuration['DEBUG']:
+            fits.writeto(f"{Configuration['LOG_DIRECTORY']}smooth_mom_map.fits",map,hdr,overwrite = True)
+        tmp = ndimage.gaussian_filter(noise_map, sigma=(sigma, sigma), order=0)
+        tmp[noise_map <= 0.] = 0.
+        noise_map = copy.deepcopy(tmp)
+        if Configuration['DEBUG']:
+            fits.writeto(f"{Configuration['LOG_DIRECTORY']}smooth_noise_map.fits",noise_map,hdr,overwrite = True)
+
+
     SNR = np.nanmean(map[noise_map > 0.]/noise_map[noise_map > 0.])
+    Configuration['SNR'] = SNR
     noise_hdr = Image[0].header
     Image.close()
     noise_map [0. > map ] =0.
     median_noise_in_map = np.nanmedian(noise_map[noise_map > 0.])
     minimum_noise_in_map = np.nanmin(noise_map[noise_map > 0.])
 
+    # if we have extended low level wings that are significant we do not really want to include then
     map[0.5*minimum_noise_in_map > noise_map] = 0.
     #Also remove negative values
     #map[0. > map ] =0
+
+
     mom0[0].data= map
-    scale_factor = set_limits(SNR/3.*minimum_noise_in_map/median_noise_in_map, 0.05, 1.)
-    if debug:
-        print_log(f'''GUESS_ORIENTATION: We find SNR = {SNR} and a scale factor {scale_factor} and the noise median {median_noise_in_map}
+
+
+    scale_factor = sf.set_limits(SNR/3.*minimum_noise_in_map/median_noise_in_map, 0.05, 1.)
+    sf.print_log(f'''GUESS_ORIENTATION: We find SNR = {SNR} and a scale factor {scale_factor} and the noise median {median_noise_in_map}
 {'':8s} minimum {minimum_noise_in_map}
-''',Configuration['OUTPUTLOG'])
-    beam_check=[Configuration['BEAM_IN_PIXELS'][0],Configuration['BEAM_IN_PIXELS'][0]/2.]
+''',Configuration,case= ['debug_add'])
+    '''
+    if np.mean(Configuration['SIZE_IN_BEAMS']) >10:
+        beam_check=[Configuration['BEAM_IN_PIXELS'][0],Configuration['BEAM_IN_PIXELS'][0]/2.]
+    else:
+    '''
+    beam_check=[Configuration['BEAM_IN_PIXELS'][0]/2.]
     center_stable = False
     checked_center = False
     center_counter = 0.
     original_center = copy.deepcopy(center)
-    print_log(f'''GUESS_ORIENTATION: Looking for the center, pa and inclination
-''',Configuration['OUTPUTLOG'], debug = debug, screen =True)
+    sf.print_log(f'''GUESS_ORIENTATION: Looking for the center, pa and inclination
+''',Configuration, case= ['verbose'])
 
-    update_statistic(Configuration, message= "Starting the initial search for the pa, inclination and center.", debug=debug)
+    sf.update_statistic(Configuration, message= "Starting the initial search for the pa, inclination and center.")
 
     while not center_stable:
-        inclination_av, pa_av, maj_extent_av = get_inclination_pa(Configuration, mom0, center, cutoff = scale_factor* median_noise_in_map, figure_name=f'{Configuration["LOG_DIRECTORY"]}loc_{center[0]:.2f}_{center[1]:.2f}',debug = debug)
-
+        inclination_av, pa_av, maj_extent_av = sf.get_inclination_pa(Configuration, mom0, center, cutoff = scale_factor* median_noise_in_map, figure_name=f'{Configuration["LOG_DIRECTORY"]}loc_{center[0]:.2f}_{center[1]:.2f}')
         inclination_av = [inclination_av]
         int_weight = [2.]
         pa_av = [pa_av]
         maj_extent_av = [maj_extent_av]
+        sf.print_log(f'''GUESS_ORIENTATION: From the the initial guess with center {center}.
+{'':8s} We get pa = {pa_av}, inclination = {inclination_av}, maj_extent_av {maj_extent_av}
+''',Configuration,case= ['debug_add'])
         for mod in beam_check:
+
             for i in [[-1,-1],[-1,1],[1,-1],[1,1]]:
                 center_tmp = [center[0]+mod*i[0],center[1]+mod*i[1]]
-                inclination_tmp, pa_tmp, maj_extent_tmp= get_inclination_pa(Configuration, mom0, center_tmp, cutoff = scale_factor* median_noise_in_map, figure_name=f'{Configuration["LOG_DIRECTORY"]}loc_{center_tmp[0]:.2f}_{center_tmp[1]:.2f}',debug = debug)
+
+                sf.print_log(f'''GUESS_ORIENTATION: Checking at location RA = {center_tmp[0]} pix, DEC = {center_tmp[1]} pix
+''',Configuration,case= ['debug_add'])
+
+                inclination_tmp, pa_tmp, maj_extent_tmp= \
+                    sf.get_inclination_pa(Configuration, mom0, center_tmp,\
+                    cutoff = scale_factor* median_noise_in_map,\
+                    figure_name=f'{Configuration["LOG_DIRECTORY"]}loc_{center_tmp[0]:.2f}_{center_tmp[1]:.2f}')
                 inclination_av.append(inclination_tmp)
                 pa_av.append(pa_tmp)
                 int_weight.append(mod/beam_check[0]*0.25)
                 maj_extent_av.append(maj_extent_tmp)
+
+        if np.isnan(np.array(inclination_av,dtype=float)).all():
+            sf.print_log(f'''GUESS_ORIENTATION: We are unable to find an  inclination.
+''',Configuration,case= ['main','screen'])
+            raise BadSourceError(f'We are unable to find an initial inclination.')
+
         int_weight = np.array(int_weight)
         weight = np.array([1./x[1] for x in inclination_av],dtype= float)*int_weight
+
         inclination = np.array([np.nansum(np.array([x[0] for x in inclination_av],dtype=float)*weight)/np.nansum(weight),\
                                 np.nansum(np.array([x[1] for x in inclination_av],dtype=float)*weight)/np.nansum(weight)],dtype=float)
+
+
+        if np.isnan(np.array(inclination_av,dtype=float)).all():
+            sf.print_log(f'''GUESS_ORIENTATION: We are unable to find an PA.
+''',Configuration,case=['main','screen'])
+            raise BadSourceError(f'We are unable to find an initial PA.')
         weight = np.array([1./x[1] for x in pa_av],dtype= float)
-        if debug:
-            print_log(f'''GUESS_ORIENTATION: We find these pa_av
+        sf.print_log(f'''GUESS_ORIENTATION: We find these pa and inclination
 {'':8s} pa = {' '.join([f'{float(x[0]):.2f}' for x in pa_av])}
+{'':8s} inclination = {' '.join([f'{float(x[0]):.2f}' for x in inclination_av])}
 {'':8s} int_weights = {' '.join([f'{float(x):.2f}' for x in int_weight])}
 {'':8s} weights = {' '.join([f'{float(x):.2f}' for x in weight])}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
         pa = np.array([np.nansum(np.array([x[0] for x in pa_av],dtype=float)*weight)/np.nansum(weight),\
                                 np.nansum(np.array([x[1] for x in pa_av],dtype=float)*weight)/np.nansum(weight)],dtype=float)
 
         maj_extent= np.nansum(maj_extent_av*weight)/np.nansum(weight)
+
         if center_counter == 0:
             original_pa = copy.deepcopy(pa)
             original_maj_extent = copy.deepcopy(maj_extent)
             original_inclination = copy.deepcopy(inclination)
 
         if center_counter > 0 and not any([np.isfinite(maj_extent),np.isfinite(pa[0]),np.isfinite(inclination[0])]):
             pa=original_pa
@@ -428,23 +503,22 @@
         #    center =original_center
         #    center_stable=True
         #    break
         # For very small galaxies we do not want to correct the extend
         if maj_extent/Configuration['BEAM'][0]/3600. > 3.:
             maj_extent = maj_extent+(Configuration['BEAM'][0]/3600.*0.2/scale_factor)
 
-        if debug:
-            print_log(f'''GUESS_ORIENTATION: From the maps we find
+        sf.print_log(f'''GUESS_ORIENTATION: From the maps we find
 {'':8s} inclination = {inclination}
 {'':8s} pa = {pa}
 {'':8s} size in beams = {maj_extent/(Configuration['BEAM'][0]/3600.)}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
                 #map[3*minimum_noise_in_map > noise_map] = 0.
         # From these estimates we also get an initial SBR
-        maj_profile,maj_axis,maj_resolution = get_profile(Configuration,map, pa[0],center,debug=debug)
+        maj_profile,maj_axis,maj_resolution = sf.get_profile(Configuration,map, pa[0],center)
         # let's get an intensity weighted center for the extracted profile.
 
         center_of_profile = np.sum(maj_profile*maj_axis)/np.sum(maj_profile)
         neg_index = np.where(maj_axis < 0.)[0]
         pos_index = np.where(maj_axis > 0.)[0]
         avg_profile = []
         neg_profile = []
@@ -453,180 +527,242 @@
         for i in range(np.nanmin([neg_index.size,pos_index.size])):
             avg_profile.append(np.nanmean([maj_profile[neg_index[neg_index.size-i-1]],maj_profile[pos_index[i]]]))
             neg_profile.append(maj_profile[neg_index[neg_index.size-i-1]])
             pos_profile.append(maj_profile[pos_index[i]])
             #diff = diff+abs(avg_profile[i]-neg_profile[i])+abs(avg_profile[i]-pos_profile[i])
             diff = diff+abs(pos_profile[-1]-neg_profile[-1])*abs(np.mean([pos_profile[-1],neg_profile[-1]]))
         diff = diff/np.nanmin([neg_index.size,pos_index.size])
-        if debug:
-            print_log(f'''GUESS_ORIENTATION:'BMAJ in pixels, center of profile, center, difference between pos and neg
-{'':8s}{Configuration['BEAM_IN_PIXELS'][0]*0.5} {center_of_profile} {center} {diff}
-''',Configuration['OUTPUTLOG'],screen=True)
+        sf.print_log(f'''GUESS_ORIENTATION:'BMAJ in pixels, center of the profile, current center, difference between pos and neg
+{'':8s}{Configuration['BEAM_IN_PIXELS'][0]} {center_of_profile} {center} {diff}
+''',Configuration,case= ['debug_add'])
 
         # if the center of the profile is more than half a beam off from the Sofia center let's see which on provides a more symmetric profile
+        #if False:
         if (abs(center_of_profile/(2.*np.sin(np.radians(pa[0])))*maj_resolution) > Configuration['BEAM_IN_PIXELS'][0]*0.5 \
             or abs(center_of_profile/(2.*np.cos(np.radians(pa[0])))*maj_resolution) > Configuration['BEAM_IN_PIXELS'][0]*0.5) and SNR > 3. and not checked_center:
-            if debug:
-                print_log(f'''GUESS_ORIENTATION: The SoFiA center and that of the SBR profile are separated by more than half a beam.
+            sf.print_log(f'''GUESS_ORIENTATION: The SoFiA center and that of the SBR profile are separated by more than half a beam.
 {'':8s}GUESS_ORIENTATION: Determining the more symmetric profile.
-''',Configuration['OUTPUTLOG'])
-            center,checked_center,center_stable = get_new_center(Configuration,map,center,maj_extent,noise=median_noise_in_map,debug=debug)
-            center_counter += 1
+''',Configuration,case= ['debug_add'])
+            # let's check against a central absorption
 
+            cube = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['FITTING_CUBE']}",\
+                    uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
+            buffer = int(round(np.mean(Configuration['BEAM_IN_PIXELS'][:2])/2.))
+            central = cube[0].data[:,int(round(center[1]-buffer)):int(round(center[1]+buffer)),int(round(center[0]-buffer)):int(round(center[0]+buffer))]
+
+            if np.count_nonzero(np.isnan(central))/central.size < 0.1:
+                center,checked_center,center_stable = sf.get_new_center(Configuration,map,inclination=inclination[0],pa=pa[0],noise=median_noise_in_map)
+                center_counter += 1
+                sf.print_log(f'''GUESS_ORIENTATION: We calculated a new center {center}.
+''',Configuration,case= ['debug_add'])
+            else:
+                center_stable = True
+                sf.print_log(f'''GUESS_ORIENTATION: There appears to be a central absorption source. We are relying on sofia
+''',Configuration,case= ['debug_add'])
 
         else:
+            sf.print_log(f'''GUESS_ORIENTATION: The previous center and that of the SBR profile are not separated by more than half a beam.
+{'':8s}GUESS_ORIENTATION: Keeping the last center
+''',Configuration,case= ['debug_add'])
             center_stable = True
-    print_log(f'''GUESS_ORIENTATION: Looking for the Initial surface brightness profile.
-''',Configuration['OUTPUTLOG'], debug = debug, screen =True)
-    update_statistic(Configuration, message= "Starting the initial search for the SBR and VROT.", debug=debug)
 
-    ring_size_req = Configuration['BEAM_IN_PIXELS'][0]/maj_resolution
+    sf.print_log(f'''GUESS_ORIENTATION: Looking for the Initial surface brightness profile.
+''',Configuration, case= ['verbose'])
+    sf.update_statistic(Configuration, message= "Starting the initial search for the SBR and VROT.")
+    Configuration['SIZE_IN_BEAMS'] = np.full(2,sf.set_limits(maj_extent/(Configuration['BEAM'][0]/3600.),1.0,Configuration['MAX_SIZE_IN_BEAMS']))
+
+    ring_size_req = Configuration['BEAM_IN_PIXELS'][0]/maj_resolution*Configuration['RING_SIZE']
+
     SBR_initial = avg_profile[0::int(ring_size_req)]/(np.pi*Configuration['BEAM'][0]*Configuration['BEAM'][1]/(4.*np.log(2.))) # Jy*km/s
+    #deproject the SBR
+    SBR_initial = SBR_initial*np.cos(np.radians(inclination[0]))
     SBR_initial =np.hstack((SBR_initial[0],SBR_initial,SBR_initial[-1]))
-
+    # unclear why we have this extra correction on the inner 3 points
     SBR_initial[0:3] = SBR_initial[0:3] * (1.2 -float(inclination[0])/90.)
-
-
+    # make sure it is the right size
+    number_of_rings = sf.calc_rings(Configuration)
+    SBR_initial = list(SBR_initial)
+    while len(SBR_initial) < number_of_rings:
+         SBR_initial.append(SBR_initial[-1])
+    while len(SBR_initial) > number_of_rings:
+         SBR_initial.pop()
+    SBR_initial = np.array(SBR_initial,dtype=float)
     #We need to know which is the approaching side and which is receding
 
 
-    print_log(f'''GUESS_ORIENTATION: Looking for the Initial Rotation Curve.
-''',Configuration['OUTPUTLOG'], debug = debug, screen =True)
-    Image = fits.open(f"{Configuration['FITTING_DIR']}Sofia_Output/{Fits_Files['MOMENT1']}",\
+    sf.print_log(f'''GUESS_ORIENTATION: Looking for the Initial Rotation Curve.
+''',Configuration,case= ['verbose'])
+    Image = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MOMENT1']}",\
             uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
     map = copy.deepcopy(Image[0].data)
+
     hdr = Image[0].header
-    if debug:
-        print_log(f'''GUESS_ORIENTATION: This is the amount of values we find initially {len(map[noise_map > 0.])}
-''',Configuration['OUTPUTLOG'])
+    sf.print_log(f'''GUESS_ORIENTATION: This is the amount of values we find initially {len(map[noise_map > 0.])}
+''',Configuration,case= ['debug_add'])
     #Image.close()
     #map[3*minimum_noise_in_map > noise_map] = float('NaN')
+
     map[3.*minimum_noise_in_map > noise_map] = float('NaN')
-    if debug:
-        print_log(f'''GUESS_ORIENTATION: This is the amount of values we find after blanking low SNR {len(map[~np.isnan(map)])}
-''',Configuration['OUTPUTLOG'])
-    if len(map[~np.isnan(map)]) < 5:
+    sf.print_log(f'''GUESS_ORIENTATION: This is the amount of values we find after blanking low SNR {len(map[~np.isnan(map)])}
+''',Configuration,case= ['debug_add'])
+    if vsys == -1 or center_counter > 0.:
+        #As python is utterly moronic the center goes in back wards to the map
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore",message="Mean of empty slice"\
+                            ,category=RuntimeWarning)
+            map_vsys = np.nanmean(map[int(round(center[1]-buffer)):int(round(center[1]+buffer)),int(round(center[0]-buffer)):int(round(center[0]+buffer))])
+        if np.mean(Configuration['SIZE_IN_BEAMS']) < 10.:
+            map_vsys = (vsys+map_vsys)/2.
+    else:
+        map_vsys = vsys
+
+
+    if len(map[~np.isnan(map)]) < 10 or np.isnan(map_vsys):
         no_values  = True
         noise_level = 2.5
         sigma = [0.5,0.5]
         while no_values:
-            if debug:
-                print_log(f'''GUESS_ORIENTATION: We smooth the velocity field to use a lower Noise threshold
-''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''GUESS_ORIENTATION: We smooth the velocity field to use a lower Noise threshold
+''',Configuration,case= ['debug_add'])
             tmp = copy.deepcopy(Image[0].data)
             tmp =  ndimage.gaussian_filter(Image[0].data, sigma=(sigma[1], sigma[0]), order=0)
             tmp[noise_level*minimum_noise_in_map > noise_map] =  float('NaN')
-            if debug:
-                print_log(f'''GUESS_ORIENTATION: We used the threshold {noise_level} and sigme = {sigma}
-{'':8s}We find the len {len(tmp[~np.isnan(tmp)])}
-''',Configuration['OUTPUTLOG'])
-            if len(tmp[~np.isnan(tmp)]) < 5:
+            #We need the cnter to be found else we get a crash
+            if vsys == -1 or center_counter > 0.:
+                #As python is utterly moronic the center goes in back wards to the map
+                with warnings.catch_warnings():
+                    warnings.filterwarnings("error",message="Mean of empty slice"\
+                            ,category=RuntimeWarning)
+                    try:
+                        map_vsys = np.nanmean(tmp[int(round(center[1]-buffer)):int(round(center[1]+buffer)),int(round(center[0]-buffer)):int(round(center[0]+buffer))])
+                    except RuntimeWarning:
+                        map_vsys = vsys
+
+                if np.mean(Configuration['SIZE_IN_BEAMS']) < 10.:
+                    map_vsys = (vsys+map_vsys)/2.
+
+
+            sf.print_log(f'''GUESS_ORIENTATION: We used the threshold {noise_level} and sigma = {sigma}
+{'':8s}We find the len {len(tmp[~np.isnan(tmp)])} and the central velocity {map_vsys}
+''',Configuration,case= ['debug_add'])
+            if len(tmp[~np.isnan(tmp)]) < 10 or np.isnan(map_vsys):
                 sigma = [sigma[0]+0.5,sigma[0]+0.5]
                 noise_level -= 0.5
             else:
                 no_values = False
                 map = tmp
             if noise_level < 1. and no_values:
                 VROT_initial = [0]
                 SBR_initial = [0]
                 Image.close()
-                return np.array(pa,dtype=float),np.array(inclination,dtype=float),SBR_initial,maj_extent,center[0],center[1],VROT_initial
+                return np.array(pa,dtype=float),np.array(inclination,dtype=float),SBR_initial,center[0],center[1],float('NaN'),VROT_initial
 
     Image.close()
+    #we want to make sure the SBr is gaussian
+    # We want to make this is sure this is a decent profile and thus we fit it with the gaussian
+    #Configuration['SIZE_IN_BEAMS'] = len(SBR_initial)-1
+    format = sf.set_format('SBR')
+    Temp_template = {'SBR':' '.join([f'{float(x):{format}}' for x in SBR_initial])\
+                        ,'SBR_2':' '.join([f'{float(x):{format}}' for x in SBR_initial]),\
+                        'VSYS':' '.join([f'{float(x):{sf.set_format("VSYS")}}' for x in [vsys,vsys]])}
+    SBR_initial = fix_sbr(Configuration,Temp_template,\
+                        smooth = True,initial=True)
+    SBR_initial = np.array([float(x) for x in Temp_template['SBR'].split()],dtype=float)
+
     noise_map = []
 
     # First we look for the kinematics center
-    #found_vsys = get_kinematical_center(Configuration,map,float(pa[0]),center=center)
-    #map_vsys = found_vsys[0]
-    #if np.sum([abs(found_vsys[1]), abs(found_vsys[2])]) != 0.:
-    #    center = [center[0]+found_vsys[1], center[1]+found_vsys[2]]
-    #    print_log(f'''GUESS_ORIENTATION: We are updating the center with x,y = {found_vsys[1:]}
-#{'':8s}to {center}
-#''',Configuration['OUTPUTLOG'])
-    #if debug:
-    #    print_log(f'''GUESS_ORIENTATION: We found the following initial VSYS:
-#{'':8s}vsys = {map_vsys}, at {center}
-#''',Configuration['OUTPUTLOG'])
-    try:
-        vel_pa = get_vel_pa(Configuration,map,center=center,debug=debug)
-    except:
-        vel_pa = [float('NaN'),float('NaN')]
 
-    maj_profile,maj_axis,maj_resolution = get_profile(Configuration,map,pa[0], center=center,debug=debug)
+    vel_pa = sf.get_vel_pa(Configuration,map,center=center)
+
+    maj_profile,maj_axis,maj_resolution = sf.get_profile(Configuration,map,pa[0], center=center)
+    zeros = np.where(maj_profile == 0.)[0]
+    maj_profile[zeros] = float('NaN')
+    if all(np.isnan(maj_profile)):
+        sf.print_log(f'''GUESS_ORIENTATION: The RC extracted from the VF is all NaN's, this means something has gone very wrong.
+{'':8s} Raising an error.
+''' , Configuration,case= ['main','screen'])
+        VROT_initial = [0]
+        SBR_initial = [0]
+        Image.close()
+        return np.array(pa,dtype=float),np.array(inclination,dtype=float),SBR_initial,center[0],center[1],float('NaN'),VROT_initial
+
     loc_max = np.mean(maj_axis[np.where(maj_profile == np.nanmax(maj_profile))[0]])
+    loc_min = np.mean(maj_axis[np.where(maj_profile == np.nanmin(maj_profile))[0]])
 
-    if loc_max > 0.:
+    if loc_max > loc_min:
         pa[0] = pa[0]+180
-        print_log(f'''GUESS_ORIENTATION: We have modified the pa by 180 deg as we found the maximum velocity west of the center.
-''' , Configuration['OUTPUTLOG'])
+        sf.print_log(f'''GUESS_ORIENTATION: We have modified the pa by 180 deg as we found the maximum velocity west of the minimum.
+''' , Configuration)
+
+    sf.print_log(f'''GUESS_ORIENTATION: this is the pa {pa} and the vel_pa {vel_pa}
+''' , Configuration,case= ['debug_add'])
 
-    if debug:
-        print_log(f'''GUESS_ORIENTATION: this is the pa {pa} and the vel_pa {vel_pa}
-''' , Configuration['OUTPUTLOG'])
+    if abs(pa[0]-vel_pa[0]) > 300.:
+        if pa[0] > 180.:
+            vel_pa[0] += 360.
+        else:
+            vel_pa[0] -= 360.
     if abs(pa[0]-vel_pa[0]) > 25. and ~np.isnan(vel_pa[0])  :
         # if the vel pa has a ridiculous error we use the normal pa
+        morph_pa=copy.deepcopy(pa)
         if vel_pa[1] < 60.:
             pa=vel_pa
+        #if the galaxy has a low inclination we do allow an error of the difference
+        if inclination[0] < 35.:
+            pa[1]=abs(morph_pa[0]-vel_pa[0])
     else:
         if ~np.isnan(vel_pa[0]):
-            pa = [np.nansum([vel_pa[0]/vel_pa[1],pa[0]/pa[1]])/np.nansum([1./vel_pa[1],1./pa[1]]),2.*1./np.sqrt(np.nansum([1./vel_pa[1],1./pa[1]]))]
+            pa = [np.nansum([vel_pa[0]/vel_pa[1],\
+                pa[0]/pa[1]])/np.nansum([1./vel_pa[1],1./pa[1]]),\
+                2.*1./np.sqrt(np.nansum([1./vel_pa[1],1./pa[1]]))]
+    sf.print_log(f'''GUESS_ORIENTATION: this is the final pa {pa}
+''' , Configuration,case= ['debug_add'])
 
-    if debug:
-        print_log(f'''GUESS_ORIENTATION: this is the final pa {pa}
-''' , Configuration['OUTPUTLOG'])
-    #As python is utterly moronic the center goes in back wards to the map
-    buffer = int(round(np.mean(Configuration['BEAM_IN_PIXELS'][:2])/2.))
-    if debug:
-        print_log(f'''GUESS_ORIENTATION: We start with vsys = {v_sys:.2f} km/s
-''' , Configuration['OUTPUTLOG'])
-
-    if v_sys == -1 or center_counter > 0.:
-        map_vsys = np.nanmean(map[int(round(center[1]-buffer)):int(round(center[1]+buffer)),int(round(center[0]-buffer)):int(round(center[0]+buffer))])
+    if smooth:
+        buffer = int(Configuration['BEAM_IN_PIXELS'][0]*5.)
     else:
-        map_vsys = v_sys
-
+        buffer = int(round(np.mean(Configuration['BEAM_IN_PIXELS'][:2])/2.))
+    sf.print_log(f'''GUESS_ORIENTATION: We start with vsys = {vsys:.2f} km/s
+{'':8s}GUESS_ORIENTATION:We subtract {map_vsys:.2f} km/s from the moment 1 map to get the VROT
+''' , Configuration,case= ['debug_add'])
 
-    if debug:
-        print_log(f'''GUESS_ORIENTATION: We subtract {map_vsys:.2f} km/s from the moment 1 map to get the VROT
-''' , Configuration['OUTPUTLOG'])
     map = map  - map_vsys
-    VROT_initial = extract_vrot(Configuration,map ,pa[0],center, debug= debug)
+    VROT_initial = extract_vrot(Configuration,map ,pa[0],center)
     min_RC_length= len(VROT_initial)
     if pa[1] < 10.:
         for x in [pa[0]-pa[1],pa[0]-pa[1]/2.,pa[0]+pa[1]/2.,pa[0]+pa[1]]:
-            tmp  = extract_vrot(Configuration,map ,x,center, debug= debug)
+            tmp  = extract_vrot(Configuration,map ,x,center)
             if len(tmp) > 0.:
                 RC_length = len(tmp)
                 if RC_length < min_RC_length:
                     min_RC_length = RC_length
-                if debug:
-                    print_log(f'''GUESS_ORIENTATION: We found the lengths for the angled rotation curves:
+                sf.print_log(f'''GUESS_ORIENTATION: We found the lengths for the angled rotation curves:
 {'':8s}GUESS_ORIENTATION: RC length = {RC_length}, min_RC length = {min_RC_length}, Vrot ini = {len(VROT_initial)}, tmnp = {len(tmp)}
 {'':8s}GUESS_ORIENTATION: Vrot {VROT_initial}
 {'':8s}GUESS_ORIENTATION: tmp {tmp}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
                 VROT_initial = np.vstack((VROT_initial[:min_RC_length],tmp[:min_RC_length]))
                 VROT_initial = np.mean(VROT_initial,axis=0)
 
     map= []
     if len(VROT_initial) < 1:
         VROT_initial = 0.
     elif len(VROT_initial) == 1:
         VROT_initial = np.array([0.,VROT_initial[0]])
     else:
         VROT_initial[0] = 0
 
     VROT_initial = np.abs(VROT_initial/np.sin(np.radians(inclination[0])))
 
 
-    if debug:
-        print_log(f'''GUESS_ORIENTATION: We found the following initial rotation curve:
+    sf.print_log(f'''GUESS_ORIENTATION: We found the following initial rotation curve:
 {'':8s}GUESS_ORIENTATION: RC = {VROT_initial}
-''',Configuration['OUTPUTLOG'])
-    return np.array(pa,dtype=float),np.array(inclination,dtype=float),SBR_initial,maj_extent,center[0],center[1],map_vsys,VROT_initial
+''',Configuration,case= ['debug_add'])
+    return np.array(pa,dtype=float),np.array(inclination,dtype=float),SBR_initial,center[0],center[1],map_vsys,VROT_initial
 guess_orientation.__doc__ =f'''
  NAME:
     guess_orientation
 
  PURPOSE:
     Obtain the initial estimates for the galaxy from the SoFiA products
 
@@ -634,15 +770,15 @@
     read_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     center = None
     Will assume the center of the map provided when unset.
     In pixel coordinates
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
@@ -657,15 +793,15 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 # load the basic info file to get the Sofia FAT Initial_Estimates
-def load_basicinfo(Configuration,filename, Variables = ['RA','DEC','VSYS','PA','Inclination','Max VRot','V_mask','Tot FLux','D_HI','Distance','HI_Mass' ,'D_HI_kpc' ], unpack = True, debug = False):
+def load_basicinfo(Configuration,filename, Variables = ['RA','DEC','VSYS','PA','Inclination','Max VRot','V_mask','Tot FLux','D_HI','Distance','HI_Mass' ,'D_HI_kpc' ], unpack = True):
     outputarray = np.zeros((2,len(Variables)), dtype=float)
     try:
         with open(filename, 'r') as tmp:
             fileline = tmp.readlines()
     except FileNotFoundError:
         print("That Basic info file does not exist. Returning empty array.")
         if unpack:
@@ -675,15 +811,15 @@
     Var_inFile = [f.strip() for f in fileline[3].split('  ') if f != '']
     del Var_inFile[0]
     invalues = [f.strip() for f in fileline[6].split('  ') if f != '']
     for i,var in enumerate(Variables):
         if var == 'RA' or var == 'DEC':
             tmp_str = invalues[Var_inFile.index('RA')].split('+/-')
             tmp_str2 = invalues[Var_inFile.index('DEC')].split('+/-')
-            RA, DEC = convertRADEC(Configuration,tmp_str[0],tmp_str2[0],invert=True,debug=debug)
+            RA, DEC = sf.convertRADEC(Configuration,tmp_str[0],tmp_str2[0],invert=True)
             if var == 'RA':
                 outputarray[:,i] = [RA,float(tmp_str[1])]
             if var == 'DEC':
                 outputarray[:,i] = [DEC,float(tmp_str2[1])]
         else:
             outputarray[:,i] = invalues[Var_inFile.index(var)].split('+/-')
     if unpack:
@@ -705,190 +841,39 @@
  OPTIONAL INPUTS:
     Variables = ['RA','DEC','VSYS','PA','Inclination','Max VRot','V_mask','Tot FLux','D_HI','Distance','HI_Mass' ,'D_HI' ]
     Variable to extract from the file
 
     unpack = True
     Unpack the values when returning or not
 
-    debug = False
+
 
  OUTPUTS:
     outputarray = Array with values of all requested parameters
 
  OPTIONAL OUTPUTS:
        -
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-#Function for loading the variables of a tirific def file into a set of variables to be used
-def load_template(Configuration,Template,Variables = ['BMIN','BMAJ','BPA','RMS','DISTANCE','NUR','RADI','VROT',
-                 'Z0', 'SBR', 'INCL','PA','XPOS','YPOS','VSYS','SDIS','VROT_2',  'Z0_2','SBR_2',
-                 'INCL_2','PA_2','XPOS_2','YPOS_2','VSYS_2','SDIS_2','CONDISP','CFLUX','CFLUX_2'],
-                 unpack = True  ,debug = False):
-    Variables = np.array([e.upper() for e in Variables],dtype=str)
-    if debug:
-        print_log(f'''LOAD_TEMPLATE: We get the following number of rings from the template {Template['NUR']}
-''',Configuration['OUTPUTLOG'], debug=True)
-    numrings = int(Template['NUR'])
-    outputarray=np.zeros((numrings,len(Variables)),dtype=float)
-    counter = 0
-    for var in Variables:
-        if debug:
-            print_log(f'''LOAD_TEMPLATE: We are processing {var}.
-{'':8s}LOAD_TEMPLATE: With the following values {Template[var]}
-''',Configuration['OUTPUTLOG'])
-        tmp =  np.array(Template[var].rsplit(),dtype=float)
-        outputarray[0:len(tmp),counter] = tmp[0:len(tmp)]
-        counter +=1
-
-    if unpack:
-        return (*outputarray.T,)
-    else:
-        return outputarray
-load_template.__doc__ =f'''
- NAME:
-    load_template
-
- PURPOSE:
-    Load values from variables set in the tirific templates
-
- CATEGORY:
-    read_functions
-
- INPUTS:
-    Configuration = Standard FAT configuration
-    Template = The tirific template to extract values from, this is a dictionary where the def file is set as  Template['parameter'] = values
-
- OPTIONAL INPUTS:
-    Variables = ['BMIN','BMAJ','BPA','RMS','DISTANCE','NUR','RADI','VROT',
-                 'Z0', 'SBR', 'INCL','PA','XPOS','YPOS','VSYS','SDIS','VROT_2',  'Z0_2','SBR_2',
-                 'INCL_2','PA_2','XPOS_2','YPOS_2','VSYS_2','SDIS_2','CONDISP','CFLUX','CFLUX_2']
-
-    unpack = True
-    if true unpack the values
-
-    debug = False
-
- OUTPUTS:
-    outputarray array with all the values of the parameters requested
-
- OPTIONAL OUTPUTS:
-
- PROCEDURES CALLED:
-    Unspecified
-
- NOTE:
-'''
-
-
-#Function for loading the variables of a tirific def file into a set of variables to be used
-def load_tirific(Configuration,filename,Variables = ['BMIN','BMAJ','BPA','RMS','DISTANCE','NUR','RADI','VROT',
-                 'Z0', 'SBR', 'INCL','PA','XPOS','YPOS','VSYS','SDIS','VROT_2',  'Z0_2','SBR_2',
-                 'INCL_2','PA_2','XPOS_2','YPOS_2','VSYS_2','SDIS_2','CONDISP','CFLUX','CFLUX_2'],
-                 unpack = True , debug = False ):
-    if debug:
-        print_log(f'''LOAD_TIRIFIC: Starting to extract the following paramaters:
-{'':8s}{Variables}
-''',Configuration['OUTPUTLOG'], debug = True)
-    Variables = np.array([e.upper() for e in Variables],dtype=str)
-    numrings = []
-    while len(numrings) < 1:
-        time.sleep(0.1)
-        with open(filename, 'r') as tmp:
-            numrings = [int(e.split('=')[1].strip()) for e in tmp.readlines() if e.split('=')[0].strip().upper() == 'NUR']
-
-    outputarray=np.zeros((numrings[0],len(Variables)),dtype=float)
-    with open(filename, 'r') as tmp:
-        unarranged = tmp.readlines()
-    # Separate the keyword names
-    for line in unarranged:
-        var_concerned = str(line.split('=')[0].strip().upper())
-        if len(var_concerned) < 1:
-            var_concerned = 'xxx'
-        varpos = np.where(Variables == var_concerned)[0]
-        if varpos.size > 0:
-            tmp =  np.array(line.split('=')[1].rsplit(),dtype=float)
-            if len(outputarray[:,0]) < len(tmp):
-                tmp_out=outputarray
-                outputarray = np.zeros((len(tmp), len(Variables)), dtype=float)
-                outputarray[0:len(tmp_out),:] = tmp_out
-            outputarray[0:len(tmp),int(varpos)] = tmp[0:len(tmp)]
-        else:
-            if var_concerned[0] == '#':
-                varpos = np.where(var_concerned[2:].strip() == Variables)[0]
-                if varpos.size > 0:
-                    tmp = np.array(line.split('=')[1].rsplit(),dtype=float)
-                    if len(outputarray[:, 0]) < len(tmp):
-                        tmp_out = outputarray
-                        outputarray = np.zeros((len(tmp), len(Variables)), dtype=float)
-                        outputarray[0:len(tmp_out), :] = tmp_out
-                    outputarray[0:len(tmp),int(varpos)] = tmp[:]
-    if unpack:
-        return (*outputarray.T,)
-    else:
-        return outputarray
-load_tirific.__doc__ =f'''
- NAME:
-    load_tirific
-
- PURPOSE:
-    Load values from variables set in the tirific files
-
- CATEGORY:
-    read_functions
-
- INPUTS:
-    filename = Path to the tirific def file
-
- OPTIONAL INPUTS:
-    Variables = ['BMIN','BMAJ','BPA','RMS','DISTANCE','NUR','RADI','VROT',
-                 'Z0', 'SBR', 'INCL','PA','XPOS','YPOS','VSYS','SDIS','VROT_2',  'Z0_2','SBR_2',
-                 'INCL_2','PA_2','XPOS_2','YPOS_2','VSYS_2','SDIS_2','CONDISP','CFLUX','CFLUX_2']
-
-    unpack = True
-    if true unpack the values
-
-    debug = False
-
- OUTPUTS:
-    outputarray array with all the values of the parameters requested
-
- OPTIONAL OUTPUTS:
-
- PROCEDURES CALLED:
-    Unspecified
-
- NOTE:
-'''
-
-def read_cube(Configuration,cube,debug=False):
+def read_cube(Configuration,cube):
     cube_hdr = fits.getheader(f"{Configuration['FITTING_DIR']}{cube}")
     Configuration['NOISE'] = cube_hdr['FATNOISE']
     Configuration['CHANNEL_WIDTH'] = cube_hdr['CDELT3']/1000.
     Configuration['PIXEL_SIZE'] = np.mean([abs(cube_hdr['CDELT1']),abs(cube_hdr['CDELT2'])])
     Configuration['NAXES'] = [cube_hdr['NAXIS1'],cube_hdr['NAXIS2'], cube_hdr['NAXIS3']]
-    with warnings.catch_warnings():
-        warnings.simplefilter("ignore")
-        coordinate_frame = WCS(cube_hdr)
-        xlow,ylow,zlow = coordinate_frame.wcs_pix2world(1,1,1., 1.)
-        xhigh,yhigh,zhigh = coordinate_frame.wcs_pix2world(*Configuration['NAXES'], 1.)
-        xlim = np.sort([xlow,xhigh])
-        ylim = np.sort([ylow,yhigh])
-        zlim =np.sort([zlow,zhigh])/1000.
-        set_boundaries(Configuration,'VSYS',*zlim,input=True,debug=debug)
-        set_boundaries(Configuration,'XPOS',*xlim,input=True,debug=debug)
-        set_boundaries(Configuration,'YPOS',*ylim,input=True,debug=debug)
+
     if np.sum(Configuration['VROT_INPUT_BOUNDARY']) == 0.:
-        set_boundaries(Configuration,'VROT',Configuration['CHANNEL_WIDTH'],600.,input=True,debug=debug)
+        sf.set_boundaries(Configuration,'VROT',Configuration['CHANNEL_WIDTH'],600.,input=True)
     if np.sum(Configuration['SDIS_INPUT_BOUNDARY']) == 0.:
-        set_boundaries(Configuration,'SDIS',Configuration['CHANNEL_WIDTH'],25.,input=True,debug=debug)
+        sf.set_boundaries(Configuration,'SDIS',Configuration['CHANNEL_WIDTH']/3.,25.,input=True)
 
     # We write the pixels per beam info to Configuration such that it is easily accesible
     beamarea=(np.pi*abs(cube_hdr['BMAJ']*cube_hdr['BMIN']))/(4.*np.log(2.))
     Configuration['BEAM_AREA'] = beamarea*3600.**2 # beamarea in arcsec
     Configuration['BEAM_IN_PIXELS'] = [cube_hdr['BMAJ']/np.mean([abs(cube_hdr['CDELT1']),abs(cube_hdr['CDELT2'])]),\
                                        cube_hdr['BMIN']/np.mean([abs(cube_hdr['CDELT1']),abs(cube_hdr['CDELT2'])]),\
                                        beamarea/(abs(cube_hdr['CDELT1'])*abs(cube_hdr['CDELT2']))]
@@ -912,21 +897,49 @@
                                   'INCL': [2.],\
                                   'SDIS': [Configuration['CHANNEL_WIDTH']*0.1],\
                                   'Z0' : [Configuration['BEAM'][0]*0.1],\
                                   'XPOS': [cube_hdr['BMAJ']*0.1],\
                                   'YPOS': [cube_hdr['BMAJ']*0.1],\
                                 }
 
+read_cube.__doc__ =f'''
+ NAME:
+    read_cube
+
+ PURPOSE:
+    Load values from the cube header into the Configuration
+
+ CATEGORY:
+    read_functions
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    cube = cube to read values from
+
+ OPTIONAL INPUTS:
+
+
+
+ OUTPUTS:
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+
+'''
+
 
 # function to read the sofia catalogue
 def sofia_catalogue(Configuration,Fits_Files, Variables =['id','x','x_min','x_max','y','y_min','y_max','z','z_min','z_max','ra',\
-                    'dec','v_app','f_sum','kin_pa','w50','err_f_sum','err_x','err_y','err_z'], debug = False):
-    if debug:
-        print_log(f'''SOFIA_CATALOGUE: Reading the source from the catalogue.
-''',Configuration['OUTPUTLOG'],debug= True)
+                    'dec','v_app','f_sum','kin_pa','w50','err_f_sum','err_x','err_y','err_z','rms']):
+    sf.print_log(f'''SOFIA_CATALOGUE: Reading the source from the catalogue.
+''',Configuration,case= ['debug_start'])
     outlist = [[] for x in Variables]
     with open(Configuration['FITTING_DIR']+'Sofia_Output/'+Configuration['BASE_NAME']+'_cat.txt') as sof_cat:
         for line in sof_cat.readlines():
             tmp =line.split()
             if line.strip() == '' or line.strip() == '#':
                 pass
             elif tmp[0] == '#' and len(tmp) > 1:
@@ -938,21 +951,21 @@
                     for col in input_columns:
                         column_locations.append(line.find(col)+len(col))
                     # check that we found all parameters
                     for value in Variables:
                         if value.lower() in input_columns:
                             continue
                         else:
-                            print_log(f'''SOFIA_CATALOGUE: We cannot find the required column for {value} in the sofia catalogue.
+                            sf.print_log(f'''SOFIA_CATALOGUE: We cannot find the required column for {value} in the sofia catalogue.
 {"":8s}SOFIA_CATALOGUE: This can happen because a) you have tampered with the sofiainput.txt file in the Support directory,
 {"":8s}SOFIA_CATALOGUE: b) you are using an updated version of SoFiA2 where the names have changed and FAT is not yet updated.'
 {"":8s}SOFIA_CATALOGUE:    In this case please file a bug report at https://github.com/PeterKamphuis/FAT/issues/'
 {"":8s}SOFIA_CATALOGUE: c) You are using pre processed SoFiA output of your own and do not have all the output'
 {"":8s}SOFIA_CATALOGUE:    Required output is {','.join(Variables)})
-''',Configuration['OUTPUTLOG'],screen= True)
+''',Configuration,case= ['main','screen'])
                             raise BadCatalogueError("SOFIA_CATALOGUE: The required columns could not be found in the sofia catalogue.")
             else:
                 for col in Variables:
                     if input_columns.index(col) == 0:
                         start = 0
                     else:
                         start = column_locations[input_columns.index(col)-1]
@@ -971,17 +984,16 @@
                 outlist[Variables.index('f_sum')][i] = float(outlist[Variables.index('f_sum')][i])/Configuration['BEAM_IN_PIXELS'][2]*Configuration['CHANNEL_WIDTH']
         if 'err_f_sum' in Variables:
             for i in range(len(outlist[0])):
                 outlist[Variables.index('err_f_sum')][i] = float(outlist[Variables.index('err_f_sum')][i])/Configuration['BEAM_IN_PIXELS'][2]*Configuration['CHANNEL_WIDTH']
 
     # we want to fit a specific source
     if len(outlist[0]) > 1 and 'f_sum' in Variables:
-        if debug:
-            print_log(f'''SOFIA_CATALOGUE: Multiple sources were found we will try to select the correct one.
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''SOFIA_CATALOGUE: Multiple sources were found we will try to select the correct one.
+''',Configuration,case= ['debug_add'])
         if Configuration['SOFIA_RAN']:
             found = False
             beam_edge=2.
             if Configuration['VEL_SMOOTH_EXTENDED'] or Configuration['CHANNEL_DEPENDENCY'].lower() == 'hanning':
                 vel_edge = 1.
                 min_vel_edge = 0.
             else:
@@ -995,15 +1007,15 @@
 
                     edge = check_edge_limits(float(many_sources[Variables.index('x_min')][i]),
                                     float(many_sources[Variables.index('x_max')][i]),
                                     float(many_sources[Variables.index('y_min')][i]),
                                     float(many_sources[Variables.index('y_max')][i]),
                                     float(many_sources[Variables.index('z_min')][i]),
                                     float(many_sources[Variables.index('z_max')][i]),
-                                    Configuration, debug = debug,beam_edge = beam_edge, vel_edge= vel_edge)
+                                    Configuration,beam_edge = beam_edge, vel_edge= vel_edge)
                     if edge:
                         many_sources[Variables.index('f_sum')][i]=0.
                 if np.nansum(many_sources[Variables.index('f_sum')]) == 0.:
                     if beam_edge > 0.5:
                         beam_edge = beam_edge/2.
                     elif vel_edge > min_vel_edge:
                         vel_edge = vel_edge/2.
@@ -1015,75 +1027,86 @@
                             cube= float(Configuration['NAXES'][0])*float(Configuration['NAXES'][1])* \
                                     (float(many_sources[Variables.index('z_max')][i])-float(many_sources[Variables.index('z_min')][i]))
                             source_size=(float(many_sources[Variables.index('z_max')][i])-float(many_sources[Variables.index('z_min')][i]))* \
                                         (float(many_sources[Variables.index('y_max')][i])-float(many_sources[Variables.index('y_min')][i]))* \
                                         (float(many_sources[Variables.index('x_max')][i])-float(many_sources[Variables.index('x_min')][i]))
 
                             if source_size/cube > 0.5:
-                                print_log(f'''SOFIA_CATALOGUE: We discarded a very large source, so we will restore is and try for that.
-    !!!!!!!!!!!!!!!!!!!!!!!!! This means your original cube is in principle too small!!!!!!!!!!!!!!!!!!!!!!!!
-    ''',Configuration['OUTPUTLOG'],screen=True)
+                                sf.print_log(f'''SOFIA_CATALOGUE: We discarded a very large source, so we will restore is and try for that.
+!!!!!!!!!!!!!!!!!!!!!!!!! This means your original cube is in principle too small!!!!!!!!!!!!!!!!!!!!!!!!
+''',Configuration)
                                 many_sources[Variables.index('f_sum')][i]=outlist[Variables.index('f_sum')][i]
                         if np.nansum(many_sources[Variables.index('f_sum')]) == 0.:
-                            print_log(f'''SOFIA_CATALOGUE:The found sources are too close to the edges of the cube. And not large enough to warrant trying them.
-    {'':8s} The edge limits were {beam_edge} beams spatially and {vel_edge} channels.
-    ''',Configuration['OUTPUTLOG'],screen=True)
+                            sf.print_log(f'''SOFIA_CATALOGUE:The found sources are too close to the edges of the cube. And not large enough to warrant trying them.
+{'':8s} The edge limits were {beam_edge} beams spatially and {vel_edge} channels.
+''',Configuration,case= ['main','screen'])
                             raise BadCatalogueError("The found sources are too close to the edges of the cube. And not large enough to warrant trying them.")
                         else:
                             found = True
                 else:
                     found = True
             # We need to check we are not throwing away a source that is infinitely brighter
             fluxes = np.array(many_sources[Variables.index('f_sum')],dtype =float)
             if np.any(fluxes == 0.):
                 no_edge_fluxes = np.array(outlist[Variables.index('f_sum')],dtype =float)
                 if np.nanmax(no_edge_fluxes) > 10.* np.nanmax(fluxes):
-                    if debug:
-                        print_log(f'''SOFIA_CATALOGUE: We discarded a very bright source, let's check wether it satisfies our minimum boundaries.
-    ''',Configuration['OUTPUTLOG'])
+                    sf.print_log(f'''SOFIA_CATALOGUE: We discarded a very bright source, let's check wether it satisfies our minimum boundaries.
+''',Configuration,case= ['debug_add'])
                     index = np.where(np.nanmax(no_edge_fluxes) == no_edge_fluxes)[0][0]
                     edge = check_edge_limits(float(outlist[Variables.index('x_min')][index]),
                                     float(outlist[Variables.index('x_max')][index]),
                                     float(outlist[Variables.index('y_min')][index]),
                                     float(outlist[Variables.index('y_max')][index]),
                                     float(outlist[Variables.index('z_min')][index]),
                                     float(outlist[Variables.index('z_max')][index]),
-                                    Configuration,debug = debug,vel_edge=min_vel_edge)
-
-                    if edge:
-                        print_log(f'''SOFIA_CATALOGUE: The bright source is very close to limits
-    ''',Configuration['OUTPUTLOG'])
+                                    Configuration,vel_edge=min_vel_edge)
+                    cube= float(Configuration['NAXES'][0])*float(Configuration['NAXES'][1])
+                    source_size=(float(many_sources[Variables.index('y_max')][index])-float(many_sources[Variables.index('y_min')][index]))* \
+                                (float(many_sources[Variables.index('x_max')][index])-float(many_sources[Variables.index('x_min')][index]))
+
+                    if edge and source_size/cube < 0.5:
+                        sf.print_log(f'''SOFIA_CATALOGUE: The bright source is very close to limits and not more than half a channel in size.
+''',Configuration)
+
+                        if float(outlist[Variables.index('rms')][index])*1e6 < float(outlist[Variables.index('f_sum')][index]):
+                            sf.print_log(f'''SOFIA_CATALOGUE: There appears to be no noise in this cube. restoring the source.
+''',Configuration)
+                            many_sources  = copy.deepcopy(outlist)
+                            fluxes = np.array(outlist[Variables.index('f_sum')],dtype =float)
                     else:
-                        print_log(f'''SOFIA_CATALOGUE: The bright source is acceptable, restoring its flux
-    ''',Configuration['OUTPUTLOG'])
+                        if edge and source_size/cube >= 0.5:
+                            sf.print_log(f'''SOFIA_CATALOGUE: The bright source is very close to limits but spans more than half a channel so we are restoring it.
+In principle your cube is too small.
+''',Configuration)
+                        else:
+                            sf.print_log(f'''SOFIA_CATALOGUE: The bright source is acceptable, restoring its flux.
+''',Configuration)
                         many_sources  = copy.deepcopy(outlist)
                         fluxes = np.array(outlist[Variables.index('f_sum')],dtype =float)
-            if debug:
-                print_log(f'''SOFIA_CATALOGUE: after checking edges we find these fluxes
+            sf.print_log(f'''SOFIA_CATALOGUE: after checking edges we find these fluxes:
 {'':8s}{many_sources[Variables.index('f_sum')]}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
         else:
             #If we did not run SoFia we simply assume we want to fit the brightest source in the cube
             many_sources  = copy.deepcopy(outlist)
             fluxes = np.array(outlist[Variables.index('f_sum')],dtype =float)
         outlist = []
         #We want the source with the most total flux.
         index = np.where(np.nanmax(fluxes) == fluxes)[0][0]
-        print_log(f'''SOFIA_CATALOGUE: We select the {index} source of this list.
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''SOFIA_CATALOGUE: We select the {index} source of this list.
+''',Configuration)
         outlist = [x[index] for x in many_sources]
         # check that our mask has the selected source
     else:
         outlist = [x[0] for x in outlist]
 
-    check_mask(Configuration,outlist[Variables.index('id')],Fits_Files,debug=debug)
-    if debug:
-        print_log(f'''SOFIA_CATALOGUE: we found these values
-{'':8s}{outlist}
-''',Configuration['OUTPUTLOG'])
+    check_mask(Configuration,outlist[Variables.index('id')],Fits_Files)
+    sf.print_log(f'''SOFIA_CATALOGUE: we found these values:
+{chr(10).join([f'{"":8s}{x} = {y}' for x,y in zip(Variables,outlist)])}
+''',Configuration,case= ['debug_add'])
     return outlist
 sofia_catalogue.__doc__ =f'''
  NAME:
     sofia_catalogue
 
  PURPOSE:
        Read the sofia catalogue and extract several basic parameters from into a list.
@@ -1100,29 +1123,29 @@
     Variables =['id','x','x_min','x_max','y','y_min','y_max','z','z_min','z_max','ra',\
                         'dec','v_app','f_sum','kin_pa','w50','err_f_sum','err_x','err_y','err_z']
     Variables to read from the catalogue
 
     header = None
     header of the initial cube to translate units
 
-    debug = False
+
 
  OUTPUTS:
     outlist = list with the requested values for the brightest source in the catalogue provided it is not on the edge of the cube.
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def sofia_input_catalogue(Configuration,debug=False):
-    Catalogue = Proper_Dictionary({})
+def sofia_input_catalogue(Configuration):
+    Catalogue = sf.Proper_Dictionary({})
 
     Catalogue = {'ENTRIES':  ['ENTRIES','DISTANCE','ID','DIRECTORYNAME','CUBENAME'],\
                 'DISTANCE': [],'DIRECTORYNAME': [],\
                 'ID': [], 'CUBENAME': []}
     basename = Configuration['CATALOGUE'].split('_cat.txt')[0]
     Variables =['id','x','x_min','x_max','y','y_min','y_max','z','z_min','z_max','ra',\
                     'dec','v_app','f_sum','kin_pa','w50','err_f_sum','err_x','err_y','err_z']
@@ -1148,78 +1171,107 @@
                         column_locations.append(line.find(col)+len(col))
 
                     # check that we found all parameters
                     for value in Variables:
                         if value.lower() in input_columns:
                             continue
                         else:
-                            print_log(f'''SOFIA_CATALOGUE: We cannot find the required column for {value} in the sofia catalogue.
+                            sf.print_log(f'''SOFIA_CATALOGUE: We cannot find the required column for {value} in the sofia catalogue.
 {"":8s}SOFIA_CATALOGUE: This can happen because a) you have tampered with the sofiainput.txt file in the Support directory,
 {"":8s}SOFIA_CATALOGUE: b) you are using an updated version of SoFiA2 where the names have changed and FAT is not yet updated.'
 {"":8s}SOFIA_CATALOGUE:    In this case please file a bug report at https://github.com/PeterKamphuis/FAT/issues/'
 {"":8s}SOFIA_CATALOGUE: c) You are using pre processed SoFiA output of your own and do not have all the output'
 {"":8s}SOFIA_CATALOGUE:    Required output is {','.join(Variables)})
-''',Configuration['OUTPUTLOG'],screen= True)
+''',Configuration,case= ['main','screen'])
                             raise BadCatalogueError("SOFIA_CATALOGUE: The required columns could not be found in the sofia catalogue.")
             else:
 
                 outlist = ['' for x in input_columns]
                 for col in input_columns:
                     if input_columns.index(col) == 0:
                         start = 0
                     else:
                         start = column_locations[input_columns.index(col)-1]
                     end = column_locations[input_columns.index(col)]
                     outlist[input_columns.index(col)] = line[start:end].strip()
 
                 if not os.path.exists(f"{Configuration['MAIN_DIRECTORY']}{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}"):
-                    create_directory(f"{Configuration['MAIN_DIRECTORY']}{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}",f"{Configuration['MAIN_DIRECTORY']}")
+                    sf.create_directory(f"{Configuration['MAIN_DIRECTORY']}{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}",f"{Configuration['MAIN_DIRECTORY']}")
 
                 if 'create_fat_cube' in Configuration['FITTING_STAGES']:
-                    create_fat_cube(Configuration, Fits_Files,sofia_catalogue=True,name=basename,id = outlist[input_columns.index('id')],debug=debug)
+                    create_fat_cube(Configuration, Fits_Files,sofia_catalogue=True,name=basename,id = outlist[input_columns.index('id')])
                 else:
                     Cube = fits.open(f"{Configuration['SOFIA_DIR']}{basename}_{outlist[input_columns.index('id')]}_cube.fits",uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
                     data = Cube[0].data
                     hdr = Cube[0].header
                     if hdr['NAXIS'] == 4:
                         data = data[0,:,:,:]
                         del hdr['NAXIS4']
                         hdr['NAXIS'] = 3
                     # clean the header
-                    hdr = clean_header(Configuration,hdr,debug=debug)
-                    low_chan = float('NAN')
+                    hdr = sf.clean_header(Configuration,hdr)
                     channel=int(0)
-                    while np.isnan(low_chan):
-                        low_chan = np.nanstd(data[channel,:,:])
+                    while np.isnan(data[channel,:,:]).all():
                         channel+=1
-                    high_chan = float('NAN')
+                    low_chan =np.nanstd(data[channel,:,:])
+
                     channel=int(-1)
-                    while np.isnan(high_chan):
-                        high_chan = np.nanstd(data[channel,:,:])
+                    while np.isnan(data[channel,:,:]).all():
                         channel-=1
+                    high_chan = np.nanstd(data[channel,:,:])
 
                     hdr['FATNOISE'] = np.mean([low_chan,high_chan])
 
                     if hdr['CDELT3'] < -1:
                         raise InputError(f"Your velocity axis is declining this won't work. exiting")
+                    #Translate the big cube to parameters in this cube.
+                    with warnings.catch_warnings():
+                        warnings.simplefilter("ignore")
+                        coordinate_frame = WCS(hdr)
+                        x,y,z =coordinate_frame.wcs_world2pix(float(outlist[input_columns.index('ra')]),\
+                                                          float(outlist[input_columns.index('dec')]), \
+                                                          float(outlist[input_columns.index('v_app')]), 1.)
+                    shift = [int(float(outlist[input_columns.index('x')]) - x), \
+                            int(float(outlist[input_columns.index('y')]) - y),\
+                            int(float(outlist[input_columns.index('z')]) - z)]
+
+                    for i,coord in enumerate(['x','y','z']):
+                        for chang in ['','_min','_max','_peak']:
+                            val = f'{coord}{chang}'
+                            if chang == '':
+                                outlist[input_columns.index(val)] = f'{float(outlist[input_columns.index(val)])-shift[i]:.6f}'
+                            else:
+                                outlist[input_columns.index(val)] = f'{int(outlist[input_columns.index(val)])-shift[i]:d}'
+
+
                     fits.writeto(f"{Configuration['MAIN_DIRECTORY']}{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}/{basename}_{outlist[input_columns.index('id')]}_FAT.fits",data,hdr,overwrite=True)
-                create_directory(f"{Configuration['MAIN_DIRECTORY']}{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}/Sofia_Output",f"{Configuration['MAIN_DIRECTORY']}")
+                sf.create_directory(f"{Configuration['MAIN_DIRECTORY']}{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}/Sofia_Output",f"{Configuration['MAIN_DIRECTORY']}")
 
                 Configuration['FITTING_DIR']=f"{Configuration['MAIN_DIRECTORY']}{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}/"
                 Configuration['SOFIA_BASENAME'] = f"{basename}_{outlist[input_columns.index('id')]}"
                 Configuration['BASE_NAME'] =  f"{basename}_{outlist[input_columns.index('id')]}_FAT"
-                copy_homemade_sofia(Configuration,no_cat=True,debug=False)
+                sf.copy_homemade_sofia(Configuration,no_cat=True)
                 Catalogue['DISTANCE'].append(float(-1))
                 Catalogue['ID'].append(f"{outlist[input_columns.index('id')]}")
                 Catalogue['DIRECTORYNAME'].append(f"{basename}_FAT_cubelets/{basename}_{outlist[input_columns.index('id')]}")
                 Catalogue['CUBENAME'].append(f"{basename}_{outlist[input_columns.index('id')]}")
                 with open(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Configuration['BASE_NAME']}_cat.txt",'w') as cat:
                     for hline in headerlines:
                         cat.write(f"{hline}\n")
-                    cat.write(line)
+                    comline=''
+                    for col in input_columns:
+                        if input_columns.index(col) == 0:
+                            start = 0
+                        else:
+                            start = column_locations[input_columns.index(col)-1]
+                        end = column_locations[input_columns.index(col)]
+                        strlenfor = f'>{int(end-start)}s'
+                        comline = f'{comline}{outlist[input_columns.index(col)]:{strlenfor}}'
+                    cat.write(comline)
+
     Configuration['SOFIA_BASENAME'] = None
     Configuration['BASE_NAME'] = 'Unset'
     Configuration['FITTING_DIR'] = 'Unset'
     return Catalogue
 sofia_input_catalogue.__doc__=f'''
 NAME:
     sofia_input_catalogue
@@ -1242,15 +1294,15 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def sofia_template(debug = False):
+def sofia_template():
     with pack_open_txt(templates, 'sofia_template.par') as tmp:
         template = tmp.readlines()
     result = {}
     counter = 0
     counter2 = 0
     # Separate the keyword names
     for line in template:
@@ -1273,72 +1325,19 @@
 
  CATEGORY:
     read_functions
 
  INPUTS:
 
  OPTIONAL INPUTS:
-    debug = False
-
- OUTPUTS:
-    result = dictionary with the read file
-
- OPTIONAL OUTPUTS:
-
- PROCEDURES CALLED:
-    split, strip, open
 
- NOTE:
-'''
-
-def tirific_template(filename = '', debug = False):
-    if filename == '':
-        with pack_open_txt(templates, 'template.def') as tmp:
-            template = tmp.readlines()
-    elif filename == 'Installation_Check':
-        from pyFAT_astro import Installation_Check as IC
-        with pack_open_txt(IC, 'ModelInput.def') as tmp:
-            template = tmp.readlines()
-    else:
-        with open(filename, 'r') as tmp:
-            template = tmp.readlines()
-    result = Proper_Dictionary()
-    counter = 0
-    # Separate the keyword names
-    for line in template:
-        key = str(line.split('=')[0].strip().upper())
-        if key == '':
-            result[f'EMPTY{counter}'] = line
-            counter += 1
-        else:
-            result[key] = str(line.split('=')[1].strip())
-    return result
-tirific_template.__doc__ ='''
- NAME:
-    tirific_template
-
- PURPOSE:
-    Read a tirific def file into a dictionary to use as a template.
-    The parameter ill be the dictionary key with the values stored in that key
-
- CATEGORY:
-    read_functions
-
- INPUTS:
-    filename = Name of the def file
-
- OPTIONAL INPUTS:
-    filename = ''
-    Name of the def file, if unset the def file in Templates is used
-
-    debug =False
 
  OUTPUTS:
     result = dictionary with the read file
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
-      split, strip, open
+    split, strip, open
 
  NOTE:
 '''
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/Support/run_functions.py` & `pyFAT_astro-0.1.1/pyFAT_astro/Support/run_functions.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,124 +1,209 @@
 # -*- coding: future_fstrings -*-
 # This module contains a set of functions and classes that are used to run external programs
 
 
 
-from pyFAT_astro.Support.support_functions import print_log, convert_type,set_limits,rename_fit_products,\
-                              set_ring_size,calc_rings,get_inner_fix,convertskyangle,\
-                              finish_current_run, remove_inhomogeneities,get_from_template,set_format, \
-                              set_rings, convertRADEC,sbr_limits, create_directory,get_system_string,\
-                              get_fit_groups,run_tirific,update_statistic,set_boundaries
 from pyFAT_astro.Support.clean_functions import clean_before_sofia,clean_after_sofia
 from pyFAT_astro.Support.fits_functions import cut_cubes,extract_pv,make_moments
-from pyFAT_astro.Support.read_functions import load_template,tirific_template
 
-from pyFAT_astro.Support.modify_template import write_new_to_template,smooth_profile,set_cflux,fix_sbr, \
-                                          regularise_profile,set_fitting_parameters,check_size, \
-                                          no_declining_vrot,set_errors,get_warp_slope,check_angles,write_center
+from pyFAT_astro.Support.modify_template import write_new_to_template,\
+    smooth_profile,set_cflux,fix_sbr,regularise_profile,set_fitting_parameters,\
+    check_size,no_declining_vrot,set_errors,get_warp_slope,check_angles,write_center,\
+    set_boundary_limits,regularise_warp,set_new_size
 from pyFAT_astro.Support.constants import H_0
-from pyFAT_astro.Support.fat_errors import SofiaFaintError,BadConfigurationError,\
-                                              InclinationRunError,SofiaRunError,BadSourceError
+from pyFAT_astro.Support.fat_errors import FaintSourceError,BadConfigurationError,\
+                                              InclinationRunError,SofiaRunError,\
+                                              BadSourceError,TirificOutputError,ProgramError
 from pyFAT_astro.Support.tirshaker import tirshaker
 
 from astropy.wcs import WCS
 from astropy.io import fits
-
 import pyFAT_astro.Support.read_functions as rf
+import pyFAT_astro.Support.support_functions as sf
 import pyFAT_astro.Support.write_functions as wf
+import pyFAT_astro
+
 import os
 import sys
-import time
 import copy
 
 import subprocess
 import numpy as np
 import traceback
 import warnings
 
 import re
 from datetime import datetime
 
+def check_angle_convergence(Configuration,Tirific_Template, fit_type = 'Undefined'):
+    angles= {'PA': 20., 'INCL': 10.}
+    angles_ok = True
+    for key in angles:
+        new_angle = sf.load_tirific(Configuration,\
+            f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def",\
+            Variables = [key],array=True)
+        old_angle = sf.load_tirific(Configuration,\
+            f"{Configuration['FITTING_DIR']}{fit_type}_In.def",\
+            Variables = [key],array=True)
+
+        sf.print_log(f'''CHECK_ANGLE_CONVERGENCE: For {key} we had {old_angle[0]} which changed to {new_angle[0]}.
+the maximum change is {float(Configuration['MIN_ERROR'][key][0])*float(angles[key])}
+''',Configuration,case= ['debug_add'])
+        if abs(old_angle[0]-new_angle[0]) > float(Configuration['MIN_ERROR'][key][0])*float(angles[key]):
+            sf.print_log(f'''CHECK_ANGLE_CONVERGENCE: The {key} changed too much between iterations.
+''',Configuration)
+            angles_ok = False
+        if key in Configuration['FIXED_PARAMETERS'][0]:
+            fixed=True
+        else:
+            fixed =False
+        old_boun = np.array(Configuration[f'{key}_CURRENT_BOUNDARY'])
+        set_boundary_limits(Configuration,Tirific_Template,key, tolerance = 0.01\
+                    ,fixed = fixed)
+        new_boun = np.array(Configuration[f'{key}_CURRENT_BOUNDARY'])
+
+        if not np.array_equiv(old_boun,new_boun):
+            sf.print_log(f'''CHECK_ANGLE_CONVERGENCE: The {key} boundaries changed from:
+{'':8s} old boundaries =  {old_boun}
+{'':8s} new boundaries =  {new_boun}
+''',Configuration,case= ['verbose'])
+            angles_ok = False
+
+    #And we chek that the angles are well behaved
+    changed_angles = check_angles(Configuration,Tirific_Template)
+    if changed_angles:
+        sf.print_log(f'''CHECK_ANGLE_CONVERGENCE: The angles were modified in check_angles
+''',Configuration)
+        angles_ok = False
+    else:
+        sf.print_log(f'''CHECK_ANGLE_CONVERGENCE: The angles were unchanged in check_angles
+''',Configuration,case= ['debug_add'])
+    return angles_ok
+check_angle_convergence.__doc__ =f'''
+ NAME:
+    check_angle_convergence
 
-def check_central_convergence(Configuration,Tirific_Template, fit_type = 'Undefined', debug = False):
-    #The new values are already loaded into the Tirific_Template so if we do accept we have to reset the values
-    if debug:
-        print_log(f'''CHECK_CENTRAL_CONVERGE: Starting stage {fit_type}.
-''',Configuration['OUTPUTLOG'],debug = True)
-    update_statistic(Configuration, message= "Starting the central convergence run", debug=debug)
+ PURPOSE:
+    Check whether the inclination and PA have converged, are not hitting the boundaries and do not change too much from ring to ring.
+
+ CATEGORY:
+    run_functions
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    Fits_Files = Standard FAT dictionary with filenames
+
+ OPTIONAL INPUTS:
+
+
+    fit_type = 'Undefined'
+    type of fitting being done.
+
+ OUTPUTS:
+    Returns a boolean that is true when the change is within the limits false when not
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
 
-    new_xpos,new_ypos,new_vsys = rf.load_tirific(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def",Variables = ['XPOS','YPOS','VSYS'],debug = debug)
-    old_xpos,old_ypos,old_vsys = rf.load_tirific(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}_In.def",Variables = ['XPOS','YPOS','VSYS'],debug = debug)
+ NOTE:
+'''
+
+def check_central_convergence(Configuration,Tirific_Template, fit_type = 'Undefined'):
+    #The new values are already loaded into the Tirific_Template so if we do accept we have to reset the values
+    sf.print_log(f'''CHECK_CENTRAL_CONVERGE: Starting stage {fit_type}.
+''',Configuration,case= ['debug_start'])
+    sf.update_statistic(Configuration, message= "Starting the central convergence run")
+
+    new_pos = sf.load_tirific(Configuration,\
+        f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def",\
+        Variables = ['XPOS','YPOS','VSYS'],array=True)
+    old_pos = sf.load_tirific(Configuration,\
+        f"{Configuration['FITTING_DIR']}{fit_type}_In.def",\
+        Variables = ['XPOS','YPOS','VSYS'],array=True)
     if Configuration['OUTER_RINGS_DOUBLED']:
-        shift_beam_frac =Configuration['SIZE_IN_BEAMS']*0.05
+        shift_beam_frac = sf.set_limits(np.mean(Configuration['SIZE_IN_BEAMS'])*0.1/Configuration['CENTRAL_CONVERGENCE_COUNTER'],np.mean(Configuration['SIZE_IN_BEAMS'])*0.05,np.mean(Configuration['SIZE_IN_BEAMS'])*0.15)
+        #shift_beam_frac =Configuration['SIZE_IN_BEAMS']*0.05
     else:
-        shift_beam_frac =0.15
-    ra_lim = set_limits(shift_beam_frac*Configuration['BEAM'][0]/3600.,np.max([Configuration['PIXEL_SIZE'],1./3600.]),Configuration['BEAM'][0]/3600.,debug = debug )
-    dec_lim =set_limits(shift_beam_frac*Configuration['BEAM'][0]/3600.,np.max([Configuration['PIXEL_SIZE'],1./3600.]),Configuration['BEAM'][0]/3600.,debug = debug )
-    sys_lim = set_limits(0.5*Configuration['CHANNEL_WIDTH'],2.5, 2.*Configuration['CHANNEL_WIDTH'],debug = debug )
-    if abs(new_xpos[0] - old_xpos[0]) > ra_lim or \
-       abs(new_ypos[0] - old_ypos[0]) > dec_lim or \
-       abs(new_vsys[0] - old_vsys[0]) > sys_lim:
-        if Configuration['SIZE_IN_BEAMS'] < 20:
+        #shift_beam_frac = 0.15
+        shift_beam_frac = sf.set_limits(0.25/Configuration['CENTRAL_CONVERGENCE_COUNTER'],0.15,0.3)
+    limits = [sf.set_limits(shift_beam_frac*Configuration['BEAM'][0]/3600.,np.max([Configuration['PIXEL_SIZE'],1./3600.]),Configuration['BEAM'][0]/3600. ), \
+              sf.set_limits(shift_beam_frac*Configuration['BEAM'][0]/3600.,np.max([Configuration['PIXEL_SIZE'],1./3600.]),Configuration['BEAM'][0]/3600. ), \
+              sf.set_limits(0.5*Configuration['CHANNEL_WIDTH'],2.5, 2.*Configuration['CHANNEL_WIDTH'] )]
+    vars = ['RA','DEC','VSYS']
+    outstr = ""
+    for i,var in enumerate(vars):
+        outstr = outstr+f'{"":8s}The {var} has shifted from {old_pos[i][0]} to  {new_pos[i][0]} which is a difference of {abs(new_pos[i][0] - old_pos[i][0])} needed = {limits[i]}.\n'
+
+    if any([True if abs(x[0]-y[0]) > lim else False for x,y,lim in zip(old_pos,new_pos,limits) ]):
+        if np.sum(Configuration['SIZE_IN_BEAMS']) < 40:
             apply_limit = 2.*Configuration['BEAM'][0]/3600.
+
         else:
-            apply_limit = Configuration['BEAM'][0]/3600.*Configuration['SIZE_IN_BEAMS']*0.2
-        if abs(new_xpos[0] - old_xpos[0]) > apply_limit or\
-           abs(new_ypos[0] - old_ypos[0]) > apply_limit:
-           print_log(f'''CHECK_CONVERGENCE: The center shifted more than {apply_limit/(Configuration['BEAM'][0]/3600.)} FWHM.
+            if Configuration['OUTER_RINGS_DOUBLED'] and Configuration['ITERATIONS'] <= 2:
+                apply_limit = Configuration['BEAM'][0]/3600.*np.mean(Configuration['SIZE_IN_BEAMS'])
+            else:
+                apply_limit = Configuration['BEAM'][0]/3600.*np.mean(Configuration['SIZE_IN_BEAMS'])*0.2
+        if any([True if abs(x[0]-y[0]) > apply_limit else False for x,y in zip(old_pos[:-1],new_pos[:-1]) ]):
+           sf.print_log(f'''CHECK_CONVERGENCE: The center shifted more than {apply_limit/(Configuration['BEAM'][0]/3600.)} FWHM.
 {"":8s}CHECK_CONVERGENCE: Not applying this shift
-''', Configuration['OUTPUTLOG'])
-           write_center(Configuration,Tirific_Template, [old_xpos[0],old_ypos[0],old_vsys[0]])
+''', Configuration,case= ['verbose'])
+           write_center(Configuration,Tirific_Template, [x[0] for x in old_pos])
 
            #write_new_to_template(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template, Variables = ['VROT',
-            #             'Z0', 'SBR', 'INCL','PA','SDIS','VROT_2',  'Z0_2','SBR_2','INCL_2','PA_2','SDIS_2'],debug=debug)
+            #             'Z0', 'SBR', 'INCL','PA','SDIS','VROT_2',  'Z0_2','SBR_2','INCL_2','PA_2','SDIS_2'])
            return False
         else:
-            try:
-                old_xpos,old_ypos,old_vsys = rf.load_tirific(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Prev2.def",Variables = ['XPOS','YPOS','VSYS'],debug=debug)
-                if abs(new_xpos[0] - old_xpos[0]) < ra_lim and \
-                   abs(new_ypos[0] - old_ypos[0]) < dec_lim and \
-                   abs(new_vsys[0] - old_vsys[0]) < sys_lim:
-                   print_log(f'''CHECK_CONVERGENCE: The center shifted back to the old position. Moving on to the next stage.
-''', Configuration['OUTPUTLOG'])
-                   #write_new_to_template(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template,debug=debug)
-                   return True
-            except:
-                pass
-            print_log(f'''CHECK_CONVERGENCE: The center shifted too much trying again with new center.
-{"":8s}The RA has shifted from {old_xpos[0]} to  {new_xpos[0]} which is a difference of {abs(new_xpos[0] - old_xpos[0])} needed = {ra_lim}.
-{"":8s}The DEC has shifted from {old_ypos[0]} to  {new_ypos[0]} which is a difference of {abs(new_ypos[0] - old_ypos[0])} needed = {dec_lim}.
-{"":8s}The VSYS has shifted from {old_vsys[0]} to  {new_vsys[0]} which is a difference of {abs(new_vsys[0] - old_vsys[0])} needed = {sys_lim}.
-''', Configuration['OUTPUTLOG'])
-            #write_new_to_template(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template,debug=debug)
+            if Configuration['ITERATIONS'] >= 3:
+                old_pos_2 = sf.load_tirific(Configuration,\
+                    f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Iteration_{Configuration['ITERATIONS']-2}.def",\
+                    Variables = ['XPOS','YPOS','VSYS'],array=True)
+                if any([True if abs(x[0]-y[0]) > lim else False for x,y,lim in zip(old_pos_2,new_pos,limits) ]):
+                    sf.print_log(f'''CHECK_CONVERGENCE: The center shifted back to the old position. Moving on to the next stage.
+''', Configuration,case= ['debug_add'])
+                   #write_new_to_template(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template)
+                    return True
+            sf.print_log(f'''CHECK_CONVERGENCE: The center shifted too much trying again with new center.
+{outstr}''', Configuration)
+            if np.sum(Configuration['SIZE_IN_BEAMS']) > 16.:
+                for i,var in enumerate(vars):
+                    if  abs(new_pos[i][0] - old_pos[i][0]) < limits[i]:
+                        sf.print_log(f'''CHECK_CONVERGENCE: We are fixing the {var}.
+''', Configuration,case= ['debug_add'])
+                        if var not in Configuration['CENTRAL_FIX']:
+                            Configuration['CENTRAL_FIX'].append(var)
+                    else:
+                        if var in Configuration['CENTRAL_FIX']:
+                            Configuration['CENTRAL_FIX'].remove(var)
+
+            #write_new_to_template(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template)
             return False
     else:
-        print_log(f'''CHECK_CONVERGENCE: The center is accepted. The shift is:
-{"":8s}The RA has shifted from {old_xpos[0]} to  {new_xpos[0]} which is a difference of {abs(new_xpos[0] - old_xpos[0])} needed = {ra_lim}.
-{"":8s}The DEC has shifted from {old_ypos[0]} to  {new_ypos[0]} which is a difference of {abs(new_ypos[0] - old_ypos[0])} needed = {dec_lim}.
-{"":8s}The VSYS has shifted from {old_vsys[0]} to  {new_vsys[0]} which is a difference of {abs(new_vsys[0] - old_vsys[0])} needed = {sys_lim}.
-''', Configuration['OUTPUTLOG'])
-        #write_new_to_template(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template,debug=debug)
+        sf.print_log(f'''CHECK_CONVERGENCE: The center is accepted. The shift is:
+{outstr}''', Configuration,case= ['verbose'])
+        #write_new_to_template(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template)
         return True
 check_central_convergence.__doc__ =f'''
  NAME:
     check_central_convergence
 
  PURPOSE:
     Check whether the center coodinates have converged to within the limits.
 
  CATEGORY:
     run_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
-    Fits_Files = Standard FAT dictionary with filenames
+    Tirific_Template = Standard FAT dictionary with the tirific Template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     fit_type = 'Undefined'
     type of fitting being done.
 
  OUTPUTS:
     Returns a boolean that is true when the change is within the limits false when not
 
@@ -126,162 +211,151 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def check_inclination(Configuration,Tirific_Template,Fits_Files, fit_type = 'Undefined', debug =False):
-    if debug:
-        print_log(f'''CHECK_INCLINATION: estimating whether our inclination estimate is decent.
-''',Configuration['OUTPUTLOG'],debug = True)
-    update_statistic(Configuration, message= "Starting the the inclination run", debug=debug)
+def check_inclination(Configuration,Tirific_Template,Fits_Files, fit_type = 'Undefined'):
+    sf.print_log(f'''CHECK_INCLINATION: estimating whether our inclination estimate is decent.
+''',Configuration,case= ['debug_start'])
+    sf.update_statistic(Configuration, message= "Starting the the inclination run")
 
     to_extract=['VROT','INCL','INCL_2','PA','XPOS','YPOS']
-    current = rf.load_template(Configuration,Tirific_Template,
-                Variables= to_extract)
+    current = sf.load_tirific(Configuration,Tirific_Template,
+                Variables= to_extract,array=True)
 
 
     inclination = float(current[to_extract.index('INCL')][0])
-    if debug:
-        print_log(f'''CHECK_INCLINATION: This is the initial inclination {inclination}
-''',Configuration['OUTPUTLOG'],debug = True)
+    sf.print_log(f'''CHECK_INCLINATION: This is the initial inclination {inclination}
+''',Configuration,case= ['debug_add'])
 
-    if Configuration['SIZE_IN_BEAMS'] < 5:
+    if np.sum(Configuration['SIZE_IN_BEAMS']) < 10.:
         incl_to_check = np.linspace(-15.,+15.,20)
     else:
         max=inclination-10
         min=inclination-50
         incl_to_check = np.linspace(min,max,20)
     # Let's make a directory to put things in
     tmp_stage = 'tmp_incl_check'
-    create_directory(tmp_stage,f"{Configuration['FITTING_DIR']}")
+    sf.create_directory(tmp_stage,f"{Configuration['FITTING_DIR']}")
 
     other_run = [Configuration['TIRIFIC_RUNNING'],Configuration['TIRIFIC_PID']]
-    try:
-        Configuration['TIRIFIC_RUNNING'] = False
-        #and a copy of the tirific template
-        if debug:
-                print_log(f'''CHECK_INCLINATION: python is so stupid
-    {'':8s}PA = {Tirific_Template['PA']}
-    ''',Configuration['OUTPUTLOG'])
-        Check_Template = copy.deepcopy(Tirific_Template)
-        #write_new_to_template(Configuration, f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Check_Template,debug = debug)
-        Check_Template['LOOPS'] = '0'
-        Check_Template['INIMODE'] = '0'
-        Check_Template['INSET'] = f"{Fits_Files['FITTING_CUBE']}"
-        current_cwd = os.getcwd()
-        short_log = Configuration['LOG_DIRECTORY'].replace(Configuration['FITTING_DIR'],'')
-        Check_Template['RESTARTNAME'] = f"{short_log}restart_{tmp_stage}.txt"
-        #Check_Template['RESTARTNAME'] = get_system_string(f"{Configuration['LOG_DIRECTORY']}restart_{tmp_stage}.txt")
-        #Check_Template['RESTARTNAME'] = f"./Logs/06-09-2021/restart_tmp_incl_check.txt"
-
-        #These are small galaxies make sure the VARINDX is not meesing things up
-        Check_Template['VARINDX'] = ''
-
-        out_keys = ['LOGNAME','OUTSET','TIRDEF']
-        out_extensions = ['log','fits','def']
-        incl_run= 'Not Initialized'
-        for i,key in enumerate(out_keys):
-            Check_Template[key] = f"{tmp_stage}/{tmp_stage}.{out_extensions[i]}"
-
-
-        vobs = [x*np.sin(np.radians(np.mean([float(y),float(z)]))) for x,y,z in \
-                zip(current[to_extract.index('VROT')][:],current[to_extract.index('INCL')][:],current[to_extract.index('INCL_2')][:])]
-        if debug:
-            print_log(f'''CHECK_INCLINATION: These are the values we get as input
-    {'':8s}Inclination = {current[to_extract.index('INCL')][:]}, {current[to_extract.index('INCL_2')][:]}
-    {'':8s}Vrot = {current[to_extract.index('VROT')][:]}
-    {'':8s}Vobs = {vobs}
-    {'':8s}PA = {Check_Template['PA']}
-    ''',Configuration['OUTPUTLOG'])
-        mom_chi = []
-        model_mom0 = fits.open(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Fits_Files['MOMENT0']}")
-        #model_mom0 = remove_inhomogeneities(Configuration,model_mom0,inclination=float(current[1][0]), pa = float(current[2][0]), center = [current[3][0],current[4][0]],debug=debug)
-        chan_map = fits.open(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Fits_Files['CHANNEL_MAP']}")
-        noisemap = np.sqrt(chan_map[0].data)*Configuration['NOISE']/np.nanmax(model_mom0[0].data)
-        max_in_moment = np.nanmax(model_mom0[0].data)
-        model_mom0[0].data = model_mom0[0].data
-        #/max_in_moment
-        for incl in incl_to_check:
-            #print(f'We are doing this inclination {incl}')
-            vrot = [x/np.sin(np.radians(inclination+incl)) for x in vobs]
-            format = set_format('INCL')
-            for key in ['INCL','INCL_2']:
-                Check_Template[key]= f"{' '.join([f'{x+incl:{format}}' for x in current[to_extract.index(key)][:]])}"
-            format = set_format('VROT')
-            for key in ['VROT','VROT_2']:
-                Check_Template[key]= f"{' '.join([f'{x:{format}}' for x in vrot])}"
-            wf.tirific(Configuration,Check_Template,name = f'{tmp_stage}_In.def',debug=True)
-            accepted,incl_run = run_tirific(Configuration,incl_run, stage = 'incl_check', fit_type=tmp_stage,debug=False)
-            make_moments(Configuration,Fits_Files,fit_type=tmp_stage,\
-                         moments = [0], \
-                         overwrite = True, vel_unit = 'm/s',debug=False)
-            #make_moments(filename = f"{Configuration['FITTING_DIR']}{tmp_stage}/{tmp_stage}.fits", basename = 'tmp_incl', directory = f"{Configuration['FITTING_DIR']}{tmp_stage}/",\
-            #             moments = [0],level = 3.*Configuration['NOISE'], \
-            #             overwrite = True, log= Configuration['OUTPUTLOG'], vel_unit = 'm/s',debug=debug)
-            incl_mom0 = fits.open(f"{Configuration['FITTING_DIR']}{tmp_stage}/{tmp_stage}_mom0.fits")
-            if debug:
-                try:
-                    os.remove(f"{Configuration['FITTING_DIR']}{tmp_stage}/tmp_{incl:.1f}_mom0.fits")
-                except:
-                    pass
-                os.rename(f"{Configuration['FITTING_DIR']}{tmp_stage}/{tmp_stage}_mom0.fits",f"{Configuration['FITTING_DIR']}{tmp_stage}/tmp_{incl:.1f}_mom0.fits")
-            chi = np.nansum((model_mom0[0].data[noisemap > 0.]-incl_mom0[0].data[noisemap > 0.])**2/noisemap[noisemap > 0.]**2)
-            mom_chi.append(abs(chi))
-            incl_mom0.close()
-        Check_Template = []
-        chan_map.close()
-        model_mom0.close()
-        finish_current_run(Configuration, incl_run)
-    except:
-        finish_current_run(Configuration, incl_run)
-        Configuration['TIRIFIC_RUNNING'] = other_run[0]
-        Configuration['TIRIFIC_PID'] =  other_run[1]
-        raise InclinationRunError('Something went wrong while estimating the inclination. This should not happen.')
+    Configuration['TIRIFIC_RUNNING'] = False
+    #and a copy of the tirific template
+    sf.print_log(f'''CHECK_INCLINATION: python is so stupid
+{'':8s}PA = {Tirific_Template['PA']}
+''',Configuration,case= ['debug_add'])
+    Check_Template = copy.deepcopy(Tirific_Template)
+    #write_new_to_template(Configuration, f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Check_Template)
+    Check_Template['LOOPS'] = '0'
+    Check_Template['INIMODE'] = '0'
+    Check_Template['INSET'] = f"{Fits_Files['FITTING_CUBE']}"
+    current_cwd = os.getcwd()
+    short_log = Configuration['LOG_DIRECTORY'].replace(Configuration['FITTING_DIR'],'')
+    Check_Template['RESTARTNAME'] = f"{short_log}restart_{tmp_stage}.txt"
+    #Check_Template['RESTARTNAME'] = sf.get_system_string(f"{Configuration['LOG_DIRECTORY']}restart_{tmp_stage}.txt")
+    #Check_Template['RESTARTNAME'] = f"./Logs/06-09-2021/restart_tmp_incl_check.txt"
+
+    #These are small galaxies make sure the VARINDX is not meesing things up
+    Check_Template['VARINDX'] = ''
+
+    out_keys = ['LOGNAME','OUTSET','TIRDEF']
+    out_extensions = ['log','fits','def']
+    incl_run= 'Not Initialized'
+    for i,key in enumerate(out_keys):
+        Check_Template[key] = f"{tmp_stage}/{tmp_stage}.{out_extensions[i]}"
+
+
+    vobs = [x*np.sin(np.radians(np.mean([float(y),float(z)]))) for x,y,z in \
+            zip(current[to_extract.index('VROT')][:],current[to_extract.index('INCL')][:],current[to_extract.index('INCL_2')][:])]
+    sf.print_log(f'''CHECK_INCLINATION: These are the values we get as input
+{'':8s}Inclination = {current[to_extract.index('INCL')][:]}, {current[to_extract.index('INCL_2')][:]}
+{'':8s}Vrot = {current[to_extract.index('VROT')][:]}
+{'':8s}Vobs = {vobs}
+{'':8s}PA = {Check_Template['PA']}
+''',Configuration,case= ['debug_add'])
+    mom_chi = []
+    model_mom0 = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MOMENT0']}")
+    #model_mom0 = sf.remove_inhomogeneities(Configuration,model_mom0,inclination=float(current[1][0]), pa = float(current[2][0]), center = [current[3][0],current[4][0]])
+    chan_map = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['CHANNEL_MAP']}")
+    noisemap = np.sqrt(chan_map[0].data)*Configuration['NOISE']/np.nanmax(model_mom0[0].data)
+    max_in_moment = np.nanmax(model_mom0[0].data)
+    model_mom0[0].data = model_mom0[0].data
+    #/max_in_moment
+    for incl in incl_to_check:
+        #print(f'We are doing this inclination {incl}')
+        vrot = [x/np.sin(np.radians(inclination+incl)) for x in vobs]
+        format = sf.set_format('INCL')
+        for key in ['INCL','INCL_2']:
+            Check_Template[key]= f"{' '.join([f'{x+incl:{format}}' for x in current[to_extract.index(key)][:]])}"
+        format = sf.set_format('VROT')
+        for key in ['VROT','VROT_2']:
+            Check_Template[key]= f"{' '.join([f'{x:{format}}' for x in vrot])}"
+        wf.tirific(Configuration,Check_Template,name = f'{tmp_stage}_In.def')
+
+        accepted,incl_run = sf.run_tirific(Configuration,incl_run, stage = 'incl_check', fit_type=tmp_stage)
+
+        make_moments(Configuration,Fits_Files,fit_type=tmp_stage,\
+                     moments = [0], \
+                     overwrite = True, vel_unit = 'm/s')
+        #make_moments(filename = f"{Configuration['FITTING_DIR']}{tmp_stage}/{tmp_stage}.fits", basename = 'tmp_incl', directory = f"{Configuration['FITTING_DIR']}{tmp_stage}/",\
+        #             moments = [0],level = 3.*Configuration['NOISE'], \
+        #             overwrite = True, log= Configuration, vel_unit = 'm/s')
+        incl_mom0 = fits.open(f"{Configuration['FITTING_DIR']}{tmp_stage}/{tmp_stage}_mom0.fits")
+        if Configuration['DEBUG']:
+            try:
+                os.remove(f"{Configuration['FITTING_DIR']}{tmp_stage}/tmp_{incl:.1f}_mom0.fits")
+            except FileNotFoundError:
+                pass
+            os.rename(f"{Configuration['FITTING_DIR']}{tmp_stage}/{tmp_stage}_mom0.fits",f"{Configuration['FITTING_DIR']}{tmp_stage}/tmp_{incl:.1f}_mom0.fits")
+        chi = np.nansum((model_mom0[0].data[noisemap > 0.]-incl_mom0[0].data[noisemap > 0.])**2/noisemap[noisemap > 0.]**2)
+        mom_chi.append(abs(chi))
+        incl_mom0.close()
+    Check_Template = []
+    chan_map.close()
+    model_mom0.close()
+    sf.finish_current_run(Configuration, incl_run)
     Configuration['TIRIFIC_RUNNING'] = other_run[0]
     Configuration['TIRIFIC_PID'] =  other_run[1]
     low= np.where(mom_chi == np.nanmin(mom_chi))[0]
     if low.size > 1:
         low = low[0]
     new_incl = float(incl_to_check[low])
-    if debug:
-        print_log(f'''CHECK_INCLINATION: This is the new inclination {new_incl} it was {current[1][0]}.
+    sf.print_log(f'''CHECK_INCLINATION: This is the new inclination {new_incl} it was {current[1][0]}.
 {'':8s}mom_chi = {mom_chi}
 {'':8s}low = {low}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
 
 
     #exit()
     incl_err = 5.
     #np.mean(np.array([current[to_extract.index('INCL_ERR')],current[to_extract.index('INCL_2_ERR')]],dtype=float))
     if incl_err < 5.:
         incl_err = 5.
     if not current[1][0]-incl_err < new_incl < current[1][0]+incl_err:
-        if debug:
-            print_log(f'''CHECK_INCLINATION: The inclination has changed, writing to file.
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''CHECK_INCLINATION: The inclination has changed, writing to file.
+''',Configuration,case= ['debug_add'])
 
         vrot = [x/np.sin(np.radians(np.mean([float(y),float(z)])+new_incl)) for x,y,z in \
             zip(vobs,current[to_extract.index('INCL')][:],current[to_extract.index('INCL_2')][:])]
-        format = set_format(key)
+        format = sf.set_format(key)
         for key in ['INCL','INCL_2']:
             Tirific_Template[key]= f"{' '.join([f'{x+new_incl:{format}}' for x in current[to_extract.index(key)][:]])}"
-        format = set_format(key)
+        format = sf.set_format(key)
         for key in ['VROT','VROT_2']:
             Tirific_Template[key]= f"{' '.join([f'{x:{format}}' for x in vrot])}"
-            if debug:
-                print_log(f'''CHECK_INCLINATION: This has gone to the template
+            sf.print_log(f'''CHECK_INCLINATION: This has gone to the template
 {'':8s} vrot = {Tirific_Template['VROT']}
 {'':8s} incl = {Tirific_Template['INCL']}
 {'':8s} incl_2 = {Tirific_Template['INCL_2']}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
 
         #Tirific_Template = copy.deepcopy(Check_Template)
-        wf.tirific(Configuration,Tirific_Template,name = f"{fit_type}/{fit_type}.def",debug=debug)
+        wf.tirific(Configuration,Tirific_Template,name = f"{fit_type}/{fit_type}.def")
     #return Tirific_Template
 check_inclination.__doc__ =f'''
  NAME:
     check_inclination
 
  PURPOSE:
     For low inclinations do a better check on the inclinations. Comparing the Chi^2 of the models over different inclinations
@@ -291,209 +365,233 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
     Tirific_Template = Standard FAT Tirific Template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     fit_type = 'Undefined'
     type of fitting
 
  OUTPUTS:
     A new file with modified inclination if it has decreased.
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
- NOTE: This should efinitely be further explored.
+ NOTE: This should definitely be further explored.
 '''
 
-def check_source(Configuration, Fits_Files, debug = False):
-    if debug:
-        print_log(f'''CHECK_SOURCE: Starting.
-''',Configuration['OUTPUTLOG'],debug = True)
-    update_statistic(Configuration, message= "Starting the check source run", debug=debug)
+def check_source(Configuration, Fits_Files):
+    sf.print_log(f'''CHECK_SOURCE: Starting.
+''',Configuration,case= ['debug_start'])
+    sf.update_statistic(Configuration, message= "Starting the check source run")
 
 
     name,x,x_min,x_max,y,y_min,y_max,z,z_min,z_max,ra,dec,v_app,f_sum,kin_pa, \
-        w50,err_f_sum, err_x,err_y,err_z= rf.sofia_catalogue(Configuration,Fits_Files,debug=debug)
+        w50,err_f_sum, err_x,err_y,err_z,source_rms= rf.sofia_catalogue(Configuration,Fits_Files)
 
-    x_min,x_max,y_min,y_max,z_min,z_max = convert_type([x_min,x_max,y_min,y_max,z_min,z_max], type = 'int')
-    x,y,z,ra,dec,v_app,f_sum,kin_pa,f_sum_err , err_x,err_y,err_z= convert_type([x,y,z,ra,dec,v_app,f_sum,kin_pa,err_f_sum, err_x,err_y,err_z])
+    x_min,x_max,y_min,y_max,z_min,z_max = sf.convert_type([x_min,x_max,y_min,y_max,z_min,z_max], type = 'int')
+    x,y,z,ra,dec,v_app,f_sum,kin_pa,f_sum_err , err_x,err_y,err_z= sf.convert_type([x,y,z,ra,dec,v_app,f_sum,kin_pa,err_f_sum, err_x,err_y,err_z])
     #How does sofia 2 deal with the fully flagged channels?
     v_app = v_app/1000.
 
 
     # Need to check for that here if NaNs are included
     if f_sum < 0.:
-        print_log(f'''CHECK_SOURCE: This galaxy has negative total flux. That will not work. Aborting.
-''',Configuration['OUTPUTLOG'],screen = True)
+        sf.print_log(f'''CHECK_SOURCE: This galaxy has negative total flux. That will not work. Aborting.
+''',Configuration,case=['main','screen'])
         raise BadSourceError('We found an initial negative total flux.')
-    galaxy_box = [[z_min,z_max],[y_min,y_max],[x_min,x_max]]
-    if debug:
-        print_log(f'''CHECK_SOURCE:  From the catalogue we got {Configuration['DISTANCE']}
-''',Configuration['OUTPUTLOG'])
+    sf.print_log(f'''CHECK_SOURCE:  From the input we get Distance = {Configuration['DISTANCE']}
+''',Configuration,case= ['debug_add'])
     # If the provided distance  = -1 we assume a Hubble follow
     if float(Configuration['DISTANCE']) == -1.:
         Configuration['DISTANCE'] = v_app/H_0
     if float(Configuration['DISTANCE']) < 0.5:
         Configuration['DISTANCE'] = 0.5
-    if debug:
-        print_log(f'''CHECK_SOURCE: We use a distance of {Configuration['DISTANCE']}.
-''',Configuration['OUTPUTLOG'])
+    sf.print_log(f'''CHECK_SOURCE: After the checks we get Distance = {Configuration['DISTANCE']}.
+''',Configuration,case= ['debug_add'])
     if np.sum(Configuration['Z0_INPUT_BOUNDARY']) == 0.:
-        set_boundaries(Configuration,'Z0',*convertskyangle(Configuration,[0.05,2.5],Configuration['DISTANCE'], physical = True),input=True,debug=debug)
+        sf.set_boundaries(Configuration,'Z0',*sf.convertskyangle(Configuration,[0.05,1.0], physical = True),input=True)
 
-    #Check whether the cube is very large, if so cut it down
+    #Check whether the cube is very large, if so cut it down, Not if we are using a Sofia_Catalogue
+    if not 'sofia_catalogue' in Configuration['FITTING_STAGES']:
+        galaxy_box = [[z_min,z_max],[y_min,y_max],[x_min,x_max]]
+        new_box = cut_cubes(Configuration, Fits_Files, galaxy_box)
+
+        #update our pixel values to match the new sizes
+        for i in range(len(new_box)):
+            shift = new_box[i,0]
+            if i == 0:
+                z -= shift; z_min -= shift; z_max -= shift
+            elif i == 1:
+                y -= shift; y_min -= shift; y_max -= shift
+            elif i == 2:
+                x -= shift; x_min -= shift; x_max -= shift
 
-    new_box = cut_cubes(Configuration, Fits_Files, galaxy_box,debug=debug)
-    #update our pixel values to match the new sizes
-    for i in range(len(new_box)):
-        shift = new_box[i,0]
-        if i == 0:
-            z -= shift; z_min -= shift; z_max -= shift
-        elif i == 1:
-            y -= shift; y_min -= shift; y_max -= shift
-        elif i == 2:
-            x -= shift; x_min -= shift; x_max -= shift
+    Cube = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['FITTING_CUBE']}",uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
 
-    Cube = fits.open(Configuration['FITTING_DIR']+Fits_Files['FITTING_CUBE'],uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
     data = Cube[0].data
+    masked_data = Cube[0].data
     header = Cube[0].header
+    Mask = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MASK']}",uint = False, do_not_scale_image_data=True,ignore_blank = True, output_verify= 'ignore')
+    masked_data[Mask[0].data < 0.5] = float('NaN')#Let's first check that this source has reasonable SNR
+#Check that the source is bright enough
+
+    Max_SNR = np.nanmax(masked_data)/Configuration['NOISE']
+    if Max_SNR < 2.5:
+        sf.print_log(f'''CHECK_SOURCE: The max SNR of the pixels in the mask is {Max_SNR}, that is not enough for a fit.
+''', Configuration,case= ['main','screen'])
+        raise BadSourceError(f"The max SNR of the pixels in the mask is {Max_SNR}. This is too faint.")
+    else:
+        sf.print_log(f'''CHECK_SOURCE: The Max SNR of the pixels in the mask is {Max_SNR}.
+''', Configuration)
+
+    Mean_SNR = np.nanmean(masked_data[masked_data > 0.])/Configuration['NOISE']
+    del masked_data
+    if Mean_SNR < 0.75:
+        sf.print_log(f'''CHECK_SOURCE: The mean SNR of the pixels in the mask is {Mean_SNR}, that is not enough for a fit.
+''', Configuration,case= ['main','screen'])
+        raise BadSourceError(f"The mean SNR of the pixels in the mask is {Mean_SNR}. This is too faint.")
+    else:
+        sf.print_log(f'''CHECK_SOURCE: The mean SNR of the pixels in the mask is {Mean_SNR}.
+''', Configuration)
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         cube_wcs = WCS(header)
     # convert the boundaries to real coordinates
     ralow,declow,vellow = cube_wcs.wcs_pix2world(x_min,y_min,z_min,1)
     rahigh,dechigh,velhigh = cube_wcs.wcs_pix2world(x_max,y_max,z_max,1)
 
     DECboun = np.sort([float(declow),float(dechigh)])
     RAboun = np.sort([float(ralow),float(rahigh)])
     VELboun = np.sort([float(vellow),float(velhigh)])
-    vsys_error= np.mean(np.abs(np.array(VELboun,dtype=float)-v_app))*0.05
-    rahr,dechr = convertRADEC(Configuration,ra,dec,debug=debug)
+    vsys_error= sf.set_limits(np.mean(np.abs(np.array(VELboun/1000.,dtype=float)-v_app))*0.05,\
+                    Configuration['CHANNEL_WIDTH']*2,Configuration['CHANNEL_WIDTH']*10.)
+
+    rahr,dechr = sf.convertRADEC(Configuration,ra,dec)
     # We write the results of the cut cube to the log
-    print_log(f'''CHECK_SOURCE: The source finder found the following center in pixels.
+    sf.print_log(f'''CHECK_SOURCE: The source finder found the following center in pixels.
 {"":8s}CHECK_SOURCE: RA center = {x} with boundaries {x_min}, {x_max}
 {"":8s}CHECK_SOURCE: DEC center = {y} with boundaries {y_min}, {y_max}
 {"":8s}CHECK_SOURCE: V_sys center = {z} with boundaries {z_min}, {z_max}
 {"":8s}CHECK_SOURCE: This should correspond to the WCS coordinates:
-{"":8s}CHECK_SOURCE: RA center = {ra} deg or {rahr}  with boundaries {','.join(convert_type(RAboun,type='str'))}
-{"":8s}CHECK_SOURCE: DEC center = {dec} deg  or {dechr}  with boundaries {','.join(convert_type(DECboun,type='str'))}
-{"":8s}CHECK_SOURCE: Sofia V_sys center = {v_app:.2f} with boundaries {','.join(convert_type(VELboun/1000.,type='str'))}
-''', Configuration['OUTPUTLOG'])
+{"":8s}CHECK_SOURCE: RA center = {ra} deg or {rahr}  with boundaries {','.join(sf.convert_type(RAboun,type='str'))}
+{"":8s}CHECK_SOURCE: DEC center = {dec} deg  or {dechr}  with boundaries {','.join(sf.convert_type(DECboun,type='str'))}
+{"":8s}CHECK_SOURCE: Sofia V_sys center = {v_app:.2f} with boundaries {','.join(sf.convert_type(VELboun/1000.,type='str'))}
+''', Configuration)
 
     #There is a factor of two missing here but this is necessary otherwise the maxima are far to small
     Configuration['MAX_SIZE_IN_BEAMS'] = int(round(np.sqrt(((x_max-x_min)/2.)**2+((y_max-y_min)/2.)**2) \
                 /(Configuration['BEAM_IN_PIXELS'][0])+5.))
+    sf.print_log(f'''CHECK_SOURCE: From Sofia we find a max extend of {Configuration['MAX_SIZE_IN_BEAMS']}
+''', Configuration,case= ['verbose'])
+    if Configuration['MAX_SIZE_IN_BEAMS'] > 20.:
+        smooth_field = True
+    else:
+        smooth_field = False
 
-
-    pa, inclination, SBR_initial, maj_extent,x_new,y_new,new_vsys,VROT_initial = rf.guess_orientation(Configuration,Fits_Files, center = [x,y],debug=debug)
+    pa, inclination, SBR_initial,x_new,y_new,new_vsys,VROT_initial =\
+        rf.guess_orientation(Configuration,Fits_Files, vsys= v_app, \
+            smooth = smooth_field,center = [x,y])
 
     if x_new != x or y_new != y or new_vsys != v_app:
-
         x,y,z_new=cube_wcs.wcs_world2pix(ra,dec,new_vsys*1000.,1)
         x=float(x_new)
         y=float(y_new)
         z=float(z_new)
         ra,dec,v_app = cube_wcs.wcs_pix2world(x,y,z,1)
         v_app = v_app/1000.
-        print_log(f'''CHECK_SOURCE: The center is updated to.
-{"":8s}CHECK_SOURCE: RA center = {ra} with boundaries {','.join(convert_type(RAboun,type='str'))}
-{"":8s}CHECK_SOURCE: DEC center = {dec} with boundaries {','.join(convert_type(DECboun,type='str'))}
-{"":8s}CHECK_SOURCE: V_sys center = {v_app:.2f} with boundaries {','.join(convert_type(VELboun/1000.,type='str'))}
-''', Configuration['OUTPUTLOG'])
+        sf.print_log(f'''CHECK_SOURCE: The center is updated to.
+{"":8s}CHECK_SOURCE: RA center = {ra} with boundaries {','.join(sf.convert_type(RAboun,type='str'))}
+{"":8s}CHECK_SOURCE: DEC center = {dec} with boundaries {','.join(sf.convert_type(DECboun,type='str'))}
+{"":8s}CHECK_SOURCE: V_sys center = {v_app:.2f} with boundaries {','.join(sf.convert_type(VELboun/1000.,type='str'))}
+''', Configuration)
+    sf.set_boundaries(Configuration,'XPOS',*RAboun,input=True)
+    sf.set_boundaries(Configuration,'YPOS',*DECboun,input=True)
+    sf.set_boundaries(Configuration,'VSYS',*VELboun/1000.,input=True)
+
     if np.sum(pa) == 0. or any(np.isnan(pa)) or \
         np.sum(inclination) == 0. or any(np.isnan(inclination)) or \
-        np.sum(maj_extent) == 0. or np.isnan(maj_extent) or \
         np.sum(SBR_initial) == 0. or all(np.isnan(SBR_initial)) or \
         np.sum(VROT_initial) == 0. or all(np.isnan(VROT_initial)):
-        print_log(f'''CHECK_SOURCE: We could not establish proper initial estimates from the moment maps. These are what we got
+        sf.print_log(f'''CHECK_SOURCE: We could not establish proper initial estimates from the moment maps. These are what we got
 {"":8s}CHECK_SOURCE: pa = {pa}
 {"":8s}CHECK_SOURCE: inclination = {inclination}
-{"":8s}CHECK_SOURCE: maj_extent = {maj_extent}
+{"":8s}CHECK_SOURCE: maj_extent = {Configuration['SIZE_IN_BEAMS']}
 {"":8s}CHECK_SOURCE: SBR_initial = {SBR_initial}
 {"":8s}CHECK_SOURCE: VROT_initial = {VROT_initial}
-''', Configuration['OUTPUTLOG'])
+''', Configuration)
 
         raise BadSourceError("No initial estimates. Likely the source is too faint.")
      # Determine whether the centre is blanked or not
 
 
-    #if debug:
-    #    print_log(f'''CHECK_SOURCE: In the center we find the vsys {Central_Velocity} km/s around the location:
-#{"":8s}CHECK_SOURCE: x,y,z = {int(round(x))}, {int(round(y))}, {int(round(z))}.
-#{'':8s}CHECK_SOURCE: we will use a systemic velocity of {v_app}
-#''',Configuration['OUTPUTLOG'])
+    sf.print_log(f'''CHECK_SOURCE: In the center we find the vsys {new_vsys} km/s around the location:
+{"":8s}CHECK_SOURCE: x,y,z = {int(round(x))}, {int(round(y))}, {int(round(z))}.
+{'':8s}CHECK_SOURCE: we will use a systemic velocity of {v_app}
+Checking the central flux in a box with size of {Configuration['BEAM_IN_PIXELS'][0]} in pixels around the central coordinates
+''',Configuration,case= ['debug_add'])
     Central_Flux = np.mean(data[int(round(z-1)):int(round(z+1)),\
                                 int(round(y-Configuration['BEAM_IN_PIXELS'][0]/2.)):int(round(y+Configuration['BEAM_IN_PIXELS'][0]/2.)),\
                                 int(round(x-Configuration['BEAM_IN_PIXELS'][0]/2.)):int(round(x+Configuration['BEAM_IN_PIXELS'][0]/2.))])
-    if debug:
-        print_log(f'''CHECK_SOURCE: In the center we find an average flux of  {Central_Flux} Jy/beam around the location:
+    del data
+    sf.print_log(f'''CHECK_SOURCE: In the center we find an average flux of  {Central_Flux} Jy/beam around the location:
 {"":8s}CHECK_SOURCE: x,y,z = {int(round(x))}, {int(round(y))}, {int(round(z))}.
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
 
     if not np.isfinite(Central_Flux):
         Configuration['EXCLUDE_CENTRAL'] = True
-        print_log(f'''CHECK_SOURCE: The flux in the central part is blanked. We exclude the central rings.
-''',Configuration['OUTPUTLOG'])
+        sf.print_log(f'''CHECK_SOURCE: The flux in the central part is blanked. We exclude the central rings.
+''',Configuration,case=['verbose'])
     else:
         Configuration['EXCLUDE_CENTRAL'] = False
 
-    #Check that the source is bright enough
-    Max_SNR = np.nanmax(data)/Configuration['NOISE']
-    if Max_SNR < 2.5:
-        log_statement = f'''CHECK_SOURCE: The maximum Signal to Noise in this cube is {Max_SNR} that is not enough for a fit.
-'''
-        print_log(log_statement, Configuration['OUTPUTLOG'],screen = True)
-        raise BadSourceError(log_statement)
 
     # Size of the galaxy in beams
-    Configuration['SIZE_IN_BEAMS'] = set_limits(maj_extent/(Configuration['BEAM'][0]/3600.),1.0,Configuration['MAX_SIZE_IN_BEAMS'])
-    if Configuration['SIZE_IN_BEAMS'] <= Configuration['TOO_SMALL_GALAXY']:
-        print_log(f'''CHECK_SOURCE: This galaxy has an estimated size of  {2*Configuration['SIZE_IN_BEAMS']} beams in diameter.
+    if np.sum(Configuration['SIZE_IN_BEAMS']) <= 2.*Configuration['TOO_SMALL_GALAXY']:
+        sf.print_log(f'''CHECK_SOURCE: This galaxy has an estimated size of  {np.sum(Configuration['SIZE_IN_BEAMS'])} beams in diameter.
 {'':8s}This is not large enough too fit. We will exit this fit.
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['main','screen'])
         raise BadSourceError('The extracted source is too small')
-    set_ring_size(Configuration, debug = debug)
+    ring_size, number_of_rings = sf.set_ring_size(Configuration)
     old_radii = np.linspace(0.,Configuration['BEAM'][0]*(len(SBR_initial)-1),len(SBR_initial))
-    new_radii = set_rings(Configuration, debug = debug)
+    new_radii = sf.set_rings(Configuration)
     SBR_initial = np.interp(new_radii,old_radii, SBR_initial)
     old_radii = np.linspace(0.,Configuration['BEAM'][0]*(len(VROT_initial)-1),len(VROT_initial))
     VROT_initial = np.interp(new_radii,old_radii, VROT_initial)
     Configuration['OUTER_SLOPE_START'] = Configuration['NO_RINGS']
-    if debug:
-        print_log(f'''CHECK_SOURCE: Interpolating the SBR and VROT estimates to these radi.
+    sf.print_log(f'''CHECK_SOURCE: Interpolating the SBR and VROT estimates to these radi.
 {'':8s} {new_radii}
 {'':8s} We got SBR = {SBR_initial}, VROT = {VROT_initial}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
 
 
     # The extent is fairly well determined and the maximum should be no more than +3 beams and a minimum no less than 4
     # Swithcing here from doubled outer rings causes problems though
-    SNR_range=set_limits(Max_SNR,1.9, 2.6)
+    SNR_range=sf.set_limits(Max_SNR,1.9, 2.6)
 
-    Configuration['MAX_SIZE_IN_BEAMS'] = set_limits(Configuration['SIZE_IN_BEAMS']*3.125/SNR_range+3.,1.,Configuration['MAX_SIZE_IN_BEAMS'])
-    Configuration['MIN_SIZE_IN_BEAMS'] = set_limits(Configuration['SIZE_IN_BEAMS']-3.,Configuration['TOO_SMALL_GALAXY'],Configuration['SIZE_IN_BEAMS'])
-    Configuration['NO_RINGS'] = calc_rings(Configuration,debug=debug)
+    Configuration['MAX_SIZE_IN_BEAMS'] = sf.set_limits(np.max(Configuration['SIZE_IN_BEAMS'])*3.125/SNR_range+3.,1.,Configuration['MAX_SIZE_IN_BEAMS'])
+    Configuration['MIN_SIZE_IN_BEAMS'] = sf.set_limits(np.max(Configuration['SIZE_IN_BEAMS'])-3.,Configuration['TOO_SMALL_GALAXY'],np.max(Configuration['SIZE_IN_BEAMS']))
+    Configuration['NO_RINGS'] = sf.calc_rings(Configuration)
     Configuration['LAST_RELIABLE_RINGS'] = [Configuration['NO_RINGS'],Configuration['NO_RINGS']]
-    print_log(f'''CHECK_SOURCE: From the original Configuration and SoFiA we find:
+    sf.print_log(f'''CHECK_SOURCE: From the original Configuration and SoFiA we find:
 {"":8s}CHECK_SOURCE: The maximum diameter we will allow  is  {2.*Configuration['MAX_SIZE_IN_BEAMS']} beams. This is based on a SNR range of {SNR_range}
 {"":8s}CHECK_SOURCE: The minimum diameter we will allow  is  {2.*Configuration['MIN_SIZE_IN_BEAMS']} beams.
-{"":8s}CHECK_SOURCE: We start with a diameter of {2*Configuration['SIZE_IN_BEAMS']} beams in the model.
+{"":8s}CHECK_SOURCE: We start with a diameter of {np.sum(Configuration['SIZE_IN_BEAMS'])} beams in the model.
 {"":8s}CHECK_SOURCE: SoFiA found a PA of {kin_pa:.2f} and we use a PA = {pa[0]:.2f} +/- {pa[1]:.2f}
 {"":8s}CHECK_SOURCE: We start with an inclination of {inclination[0]:.2f} +/- {inclination[1]:.2f}{"":8s}
 {"":8s}CHECK_SOURCE: SoFiA found a W50 of {w50:.2f} km/s
-{"":8s}CHECK_SOURCE: We will use {2.*Configuration['NO_RINGS']} for the model with a ring size of {Configuration['RING_SIZE']}.
-''',Configuration['OUTPUTLOG'])
+{"":8s}CHECK_SOURCE: We will use {2.*(Configuration['NO_RINGS']-1)} rings for the model with a ring size of {Configuration['RING_SIZE']}.
+''',Configuration)
 
 
 
 
     if Configuration['CHANNEL_DEPENDENCY'].lower() == 'hanning':
         vres = (Configuration['CHANNEL_WIDTH']*2)/(2.*np.sqrt(2.*np.log(2)))
     elif Configuration['CHANNEL_DEPENDENCY'].lower() == 'sinusoidal' :
@@ -503,48 +601,61 @@
     else:
         raise BadConfigurationError('Something went wrong in the Configuration setup')
 
     #if inclination[0] < 40:
     #    max_vrot=w50/2./np.sin(np.radians(abs(inclination[0]+5.)))
     #else:
     max_vrot=w50/2./np.sin(np.radians(abs(inclination[0])))
-    max_vrot_dev=set_limits((VELboun[1]-VELboun[0])/4000./np.sin(np.radians(inclination[0])),4.*vres,20*vres,debug=debug)
+    max_vrot_dev=sf.set_limits((VELboun[1]-VELboun[0])/4000./np.sin(np.radians(inclination[0])),4.*vres,20*vres)
 
 
     #Write the info to the Basic info File
     wf.basicinfo(Configuration,initialize = True,
               RA=[ra,abs(err_x*header['CDELT1'])],
               DEC=[dec,abs(err_y*header['CDELT2'])],
               VSYS =[v_app,abs(err_z*header['CDELT3']/1000.)],
               PA=pa, Inclination = inclination, Max_Vrot = [max_vrot,max_vrot_dev], Tot_Flux = [f_sum,f_sum_err], V_mask = [VELboun[1]-VELboun[0],vres],
-              Distance = Configuration['DISTANCE'] , DHI = [2*maj_extent*3600.,Configuration['BEAM'][0]*Configuration['RING_SIZE']],debug=debug)
+              Distance = Configuration['DISTANCE'] , DHI = [2*Configuration['SIZE_IN_BEAMS'][0]*Configuration['BEAM'][0],Configuration['BEAM'][0]*Configuration['RING_SIZE']])
 
 
     # extract a PV-Diagram
     if not os.path.exists(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Configuration['SOFIA_BASENAME']}_sofia_xv.fits"):
         PV =extract_pv(Configuration,Cube, pa[0], center=[ra,dec,v_app*1000.], convert = 1000.,
-                       finalsize = [int(round(maj_extent/np.mean([abs(header['CDELT1']),abs(header['CDELT2'])])*1.25+header['NAXIS1']*0.2)),
-                                    int(round(z_max-z_min)+10.)],debug=debug)
+                       finalsize = [int(round(Configuration['SIZE_IN_BEAMS'][0]*Configuration['BEAM'][0]/np.mean([abs(header['CDELT1']),abs(header['CDELT2'])])*1.25+header['NAXIS1']*0.2)),
+                                    int(round(z_max-z_min)+10.)])
         fits.writeto(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Configuration['BASE_NAME']}_sofia_xv.fits",PV[0].data,PV[0].header)
     Cube.close()
     Initial_Parameters = {}
-    Initial_Parameters['XPOS'] = [ra,set_limits(abs(err_x*header['CDELT1']),0.1/3600.*Configuration['BEAM'][0],3./3600.*Configuration['BEAM'][0] )]
-    Initial_Parameters['YPOS'] = [dec,set_limits(abs(err_y*header['CDELT2']),0.1/3600.*Configuration['BEAM'][0],3./3600.*Configuration['BEAM'][0] )]
-    Initial_Parameters['VSYS'] =[v_app*1000.,vsys_error]
+    Initial_Parameters['XPOS'] = [ra,sf.set_limits(abs(err_x*header['CDELT1']),0.1/3600.*Configuration['BEAM'][0],3./3600.*Configuration['BEAM'][0] )]
+    Initial_Parameters['YPOS'] = [dec,sf.set_limits(abs(err_y*header['CDELT2']),0.1/3600.*Configuration['BEAM'][0],3./3600.*Configuration['BEAM'][0] )]
+    Initial_Parameters['VSYS'] =[v_app,vsys_error]
+
+    if Configuration['OUTER_RINGS_DOUBLED']:
+        for par in ['XPOS','YPOS']:
+            Initial_Parameters[par][1]= Initial_Parameters[par][1]*np.mean(Configuration['SIZE_IN_BEAMS'])*10.
+        Initial_Parameters['VSYS'][1] = Initial_Parameters['VSYS'][1]*Configuration['NAXES'][2]/10.*Configuration['CHANNEL_WIDTH']
     Initial_Parameters['SBR_profile'] = SBR_initial
     #Initial_Parameters['VROT'] = [max_vrot/1000.,max_vrot_dev/1000.]
     Initial_Parameters['VROT_profile'] = VROT_initial
     Initial_Parameters['VROT'] = [np.max(VROT_initial) ,(np.max(VROT_initial)-np.min(VROT_initial))]
     Initial_Parameters['PA'] = pa
     Initial_Parameters['INCL'] = inclination
     Initial_Parameters['FLUX'] = [f_sum,f_sum_err]
     new_errors = np.array([pa[1],inclination[1],vsys_error])*0.1
     para = ['PA','INCL','VSYS']
     for err,parameter in zip(new_errors,para):
-        Configuration['MIN_ERROR'][parameter] = [set_limits(err,Configuration['MIN_ERROR'][parameter][0],Configuration['MAX_ERROR'][parameter][0]/2.)]
+        Configuration['MIN_ERROR'][parameter] = [sf.set_limits(err,Configuration['MIN_ERROR'][parameter][0],Configuration['MAX_ERROR'][parameter][0]/2.)]
+    #if the source is small we fix the warping
+    if np.mean(Configuration['SIZE_IN_BEAMS']) <= Configuration['MINIMUM_WARP_SIZE']:
+        for parameter in ['INCL','Z0','SDIS','PA']:
+            if parameter not in Configuration['FIXED_PARAMETERS'][0]:
+                Configuration['FIXED_PARAMETERS'][0].append(parameter)
+
+    Initial_Parameters = check_initial_boundaries(Configuration, Initial_Parameters)
+
 
     return Initial_Parameters
 check_source.__doc__='''
  NAME:
     check_source
 
  PURPOSE:
@@ -554,62 +665,267 @@
     run_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Locations of the Fits files used by FAT
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     Initial_Parameters = Dictionary with all initial values obtained from the Sofia source finding and processing.
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
+def check_initial_boundaries(Configuration, Initial_Parameters):
+    sf.print_log(f'''CHECK_INITIAL_BOUNDARIES: Starting Check
+''',Configuration,case= ['debug_start'])
+    for parameter in Initial_Parameters:
+        #some initial parameters we do not want to check as they are not in the models
+        if parameter in ['FLUX']:
+            continue
+        if parameter in ['VROT_profile','SBR_profile']:
+            stripped_parameter= parameter.split('_')[0]
+            length = len(Initial_Parameters[parameter])
+            if parameter == 'VROT_profile':
+                error=  sf.set_limits(Initial_Parameters[stripped_parameter][1]/10.,0.,\
+                    Configuration[f'{stripped_parameter}_INPUT_BOUNDARY'][0][0]*1.05)
+            elif parameter == 'SBR_profile':
+                error=Initial_Parameters[parameter][-1]/5.
+            else:
+                error=0.
+        else:
+            stripped_parameter= parameter
+            length=1
+            error = sf.set_limits(abs(Initial_Parameters[parameter][1]/10.),0.,\
+                abs(Configuration[f'{stripped_parameter}_INPUT_BOUNDARY'][0][0])*1.05)
+        if np.sum(Configuration[f'{stripped_parameter}_INPUT_BOUNDARY']) != 0.:
+            sf.print_log(f'''CHECK_INITIAL_BOUNDARIES: Checking {parameter}
+{'':8s} stripped_parameter = {stripped_parameter}
+{'':8s} boundaries = {Configuration[f'{stripped_parameter}_INPUT_BOUNDARY']}
+{'':8s} length = {length}
+{'':8s} error = {error}
+''',Configuration,case= ['debug_add'])
+            for i in range(length):
+                Initial_Parameters[parameter][i] = sf.set_limits(\
+                    Initial_Parameters[parameter][i],\
+                    Configuration[f'{stripped_parameter}_INPUT_BOUNDARY'][0][0]+error,\
+                    Configuration[f'{stripped_parameter}_INPUT_BOUNDARY'][0][1]-error)
+
+
+
+    return Initial_Parameters
+
+def check_vobs(Configuration,Tirific_Template,fit_type = 'Undefined'):
+    passed = False
+    vrot,incl,incl_2 = sf.load_tirific(Configuration,Tirific_Template, \
+            Variables=['VROT','INCL','INCL_2'],array=True)
+    #print(vrot,incl,incl_2)
+    vobs= [[x*np.sin(np.radians(y)),x*np.sin(np.radians(z))] for x,y,z in zip(vrot,incl,incl_2)]
+    delta = [[abs(x-x1),abs(y-y1),abs(z-z1)] for x,y,z,x1,y1,z1 in zip(vrot,incl,incl_2,vrot[1:],incl[1:],incl_2[1:]) ]
+    #print(delta)
+
+
+    for i,pair in enumerate(vobs):
+        sf.print_log(f'''CHECK_VOBS:For ring {i} we find vobs {pair}
+{'':8s} And the differences {[delta[i-1] if i >0 else [0,0,0]]}.
+''',Configuration,case= ['debug_add'])
+
+    passed=True
+    return passed
+
+check_vobs.__doc__='''
+ NAME:
+    check_vobs.
+
+ PURPOSE:
+    Check that the current vrot*sin(i) corresponds to the minimal changes in vrot and incl
+
+ CATEGORY:
+    run_functions
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    Tirific_Template = Standard FAT dictionary with the tirific Template
+
+ OPTIONAL INPUTS:
+
+
+    fit_type = 'Undefined'
+    type of fitting being done.
+
+ OUTPUTS:
+    Returns a boolean that is true when the change is within the limits false when not
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+def construct_kernels(Configuration,sofia_template):
+    #we always want the unsmoothed cube
+    spatial_kernels= [0]
+    if np.sum(Configuration['NAXES'][:2])/(2.*int(round(Configuration['BEAM_IN_PIXELS'][0])))  > 5:
+        spatial_kernels.append(int(round(Configuration['BEAM_IN_PIXELS'][0])))
+    if np.sum(Configuration['NAXES'][:2])/(2.*int(round(Configuration['BEAM_IN_PIXELS'][0])))  > 15:
+        spatial_kernels.append(int(round(Configuration['BEAM_IN_PIXELS'][0]*2.)))
+    if np.sum(Configuration['NAXES'][:2])/(2.*int(round(Configuration['BEAM_IN_PIXELS'][0])))  > 30:
+        spatial_kernels.append(int(round(Configuration['BEAM_IN_PIXELS'][0]))*3)
+    if np.sum(Configuration['NAXES'][:2])/(2.*int(round(Configuration['BEAM_IN_PIXELS'][0])))  > 45:
+        spatial_kernels.append(int(round(Configuration['BEAM_IN_PIXELS'][0]))*4)
+
+    sf.print_log(f'''CONSTRUCT_KERNELS: We use the following spatial_kernels
+{'':8s} spatial kernels = {spatial_kernels}
+''', Configuration)
+    velocity_kernels = [0]
+    if Configuration['NAXES'][2] > 12:
+        velocity_kernels.append(3)
+    if Configuration['NAXES'][2] > 24:
+        velocity_kernels.append(6)
+    if Configuration['NAXES'][2] > 48:
+        velocity_kernels.append(12)
+    if Configuration['NAXES'][2] > 52:
+        velocity_kernels.append(16)
+        Configuration['VEL_SMOOTH_EXTENDED'] = True
+        sf.print_log(f'''CONSTRUCT_KERNELS: Using a very extended velocity smoothing as the cube has more than 52 channels.
+''', Configuration)
+
+    sf.print_log(f'''CONSTRUCT_KERNELS: We use the following velocity kernels
+{'':8s} velocity kernels = {velocity_kernels}
+''', Configuration)
+    sofia_template['scfind.kernelsXY'] = ','.join([str(x) for x in spatial_kernels])
+    sofia_template['scfind.kernelsZ'] = ','.join([str(x) for x in velocity_kernels])
+    return spatial_kernels,velocity_kernels
+
+construct_kernels.__doc__ =f'''
+ NAME:
+    construct_kernels
+
+ PURPOSE:
+    run sofia on the cube to get a source mask and initial estimates.
+
+ CATEGORY:
+    run_functions
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    Fits_Files = Standard FAT dictionary with filenames
+
+ OPTIONAL INPUTS:
+
+
+
+ OUTPUTS:
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+def failed_fit(Configuration,Tirific_Template,current_run, Fits_Files,\
+        stage='initial', fit_type='Fit_Tirific_OSC'):
+    sf.print_log(f'''FAILED_FIT: Tirific failed to produce output in {fit_type}. It might be an unspecified crash.
+we try once more else we break off the fitting. As this sometimes happens due to a gsl interpolation error we modify the ring size by 5%
+''',Configuration, case=['main','screen'])
+    # There appears to be a case where the last ring can cause an interpolation error.
+    # Deal with this we take 0.95% of the beam ring size and run again
+    # I don't understand why we removed this again.
+    Configuration['OLD_SIZE'].append(list(copy.deepcopy(Configuration['SIZE_IN_BEAMS'])))
+    Configuration['SIZE_IN_BEAMS'] = Configuration['SIZE_IN_BEAMS']*0.95
+    ring_size, number_of_rings = sf.set_ring_size(Configuration)
+    set_new_size(Configuration,Tirific_Template,fit_type= fit_type\
+            ,current_run = current_run)
+    if stage == 'full_res':
+
+        #if the crash happens when make the full resolution  we need to
+        # rescale the last iteration
+        sf.print_log(f'''FAILED_FIT: We are rescaleing {Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Iteration_{Configuration['ITERATIONS']}.def
+    ''',Configuration,case=['main'])
+        Last_Iteration = sf.tirific_template(f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Iteration_{Configuration['ITERATIONS']}.def")
+        set_new_size(Configuration,Last_Iteration,fit_type= fit_type
+                ,current_run = 'Not Zed')
+        wf.tirific(Configuration,Tirific_Template,name = \
+            f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Iteration_{Configuration['ITERATIONS']}.def",
+            full_name=True)
+    wf.tirific(Configuration,Tirific_Template,name = f'{fit_type}_In.def')
+    accepted,current_run = sf.run_tirific(Configuration,current_run,stage = stage, fit_type = fit_type)
+    return accepted,current_run
+
+failed_fit.__doc__ =f'''
+ NAME:
+    failed_fit
+
+ PURPOSE:
+    sometimes tirific fails on a gsl interpolation error and we have to rerun with slightly different rings
+
+ CATEGORY:
+    run_functions
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    Fits_Files = Standard FAT dictionary with filenames
+
+ OPTIONAL INPUTS:
+
+
+
+ OUTPUTS:
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
 def fitting_osc(Configuration,Fits_Files,Tirific_Template,Initial_Parameters):
     current_run = 'Not Initialized'
-    create_directory(Configuration['USED_FITTING'],Configuration['FITTING_DIR'])
+    sf.create_directory(Configuration['USED_FITTING'],Configuration['FITTING_DIR'])
     wf.initialize_def_file(Configuration, Fits_Files,Tirific_Template, \
                            Initial_Parameters= Initial_Parameters, \
-                           fit_type=Configuration['USED_FITTING'],\
-                           debug=Configuration['DEBUG'])
-    print_log(f'''FITTING_OSC: The initial def file is written and we will now start fitting.
-''' ,Configuration['OUTPUTLOG'], screen =True, debug = Configuration['DEBUG'])
+                           fit_type=Configuration['USED_FITTING'])
+    sf.print_log(f'''FITTING_OSC: The initial def file is written and we will now start fitting.
+''' ,Configuration)
     Configuration['PREP_END_TIME'] = datetime.now()
         # If we have no directory to put the output we create it
 
     while not Configuration['ACCEPTED'] and Configuration['ITERATIONS'] <  Configuration['MAX_ITERATIONS']:
         Configuration['ITERATIONS'] = Configuration['ITERATIONS']+1
         # Run the step
-        current_run = one_step_converge(Configuration, Fits_Files,Tirific_Template,current_run,debug = Configuration['DEBUG'])
+        current_run = one_step_converge(Configuration, Fits_Files,Tirific_Template,current_run)
 
-        if (Configuration['ITERATIONS'] == 1 or Configuration['ACCEPTED']) and Configuration['SIZE_IN_BEAMS'] < 4:
-            if Configuration['DEBUG']:
-                        print_log(f'''FITTING_OSC: Checking the inclination due to small galaxy size.
+        if (Configuration['ITERATIONS'] == 1  and np.sum(Configuration['SIZE_IN_BEAMS']) < 10.6) or  (Configuration['ACCEPTED'] and np.sum(Configuration['SIZE_IN_BEAMS']) < 6.6):
+            sf.print_log(f'''FITTING_OSC: Checking the inclination due to small galaxy size.
 {'':8s}PA = {Tirific_Template['PA']}
 {'':8s}INCL = {Tirific_Template['INCL']}
-''',Configuration['OUTPUTLOG'])
-            check_inclination(Configuration,Tirific_Template,Fits_Files, fit_type =Configuration['USED_FITTING'], debug = Configuration['DEBUG'])
+''',Configuration,case= ['debug_add'])
+            check_inclination(Configuration,Tirific_Template,Fits_Files, fit_type =Configuration['USED_FITTING'])
 
     if Configuration['ACCEPTED']:
-        print_log(f'''FITTING_OSC: The model has converged in center and extent and we make a smoothed version.
-''',Configuration['OUTPUTLOG'],screen =True)
-        check_angles(Configuration, Tirific_Template,debug=Configuration['DEBUG'] )
-        current_run = fit_smoothed_check(Configuration, Fits_Files,Tirific_Template,current_run,stage = 'after_os', fit_type = Configuration['USED_FITTING'],debug = Configuration['DEBUG'])
+        sf.print_log(f'''FITTING_OSC: The model has converged in center and extent and we make a smoothed version.
+''',Configuration)
+        current_run = fit_smoothed_check(Configuration, Fits_Files,\
+            Tirific_Template,current_run,stage = 'after_os',\
+             fit_type = Configuration['USED_FITTING'])
         if Configuration['OPTIMIZED']:
-            make_full_resolution(Configuration,Tirific_Template,Fits_Files,current_run = current_run,fit_type = Configuration['USED_FITTING'],debug=Configuration['DEBUG'])
+            make_full_resolution(Configuration,Tirific_Template,Fits_Files,\
+                current_run = current_run,fit_type = Configuration['USED_FITTING'])
     elif Configuration['INSTALLATION_CHECK']:
-        print_log(f'''FITTING_OSC: The Installation_check has run a fit successfully.
-''',Configuration['OUTPUTLOG'],screen =True)
+        sf.print_log(f'''FITTING_OSC: The Installation_check has run a fit successfully.
+''',Configuration)
     else:
         Configuration['FINAL_COMMENT'] = 'We could not converge on the extent or centre of the galaxy'
         Configuration['OUTPUT_QUANTITY'] = 5
     return current_run
 fitting_osc.__doc__ =f'''
  NAME:
     fitting_osc
@@ -635,95 +951,116 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE: This is the main fitting routine if you want to make your own start by looking here. And then add it in main.py
        This is the fitting type done for the installation check.
 '''
 
-def fit_smoothed_check(Configuration, Fits_Files,Tirific_Template,current_run, stage = 'initial',fit_type='Undefined', debug = False):
-    update_statistic(Configuration, message= "Starting the smoothed check run", debug=debug)
-    if debug:
-        print_log(f'''FIT_SMOOTHED_CHECK: Starting stage {stage} and fit_type {fit_type}.
-''',Configuration['OUTPUTLOG'],debug = True)
+def fit_smoothed_check(Configuration, Fits_Files,Tirific_Template,current_run, stage = 'initial',fit_type='Undefined'):
+    sf.update_statistic(Configuration, message= "Starting the smoothed check run")
+    sf.print_log(f'''FIT_SMOOTHED_CHECK: Starting stage {stage} and fit_type {fit_type}.
+''',Configuration,case= ['debug_start'])
+    if Configuration['DEBUG']:
+        sf.write_config(
+            f'{Configuration["LOG_DIRECTORY"]}CFG_Before_Smoothing.txt', Configuration)
+        wf.tirific(Configuration,Tirific_Template, name = 'Input_to_Smooth.def')
+        os.system(f'''mv {Configuration['FITTING_DIR']}/Input_to_Smoothed_Check.def {Configuration['LOG_DIRECTORY']}''')
+
     #if we have only a few rings we only smooth. else we fit a polynomial to the RC and smooth the SBR
-    #smoothed_sbr = smooth_profile(Configuration,Tirific_Template,'SBR',hdr, min_error= np.max([float(Tirific_Template['CFLUX']),float(Tirific_Template['CFLUX_2'])]),debug = debug)
-    fix_sbr(Configuration,Tirific_Template,smooth = True, debug = debug)
+    #smoothed_sbr = smooth_profile(Configuration,Tirific_Template,'SBR',hdr, min_error= np.max([float(Tirific_Template['CFLUX']),float(Tirific_Template['CFLUX_2'])]))
+    fix_sbr(Configuration,Tirific_Template,smooth = True)
     if stage == 'after_cc':
-        smoothed_vrot = smooth_profile(Configuration,Tirific_Template,'VROT',min_error = Configuration['CHANNEL_WIDTH'],debug = debug)
+        smoothed_vrot = smooth_profile(Configuration,Tirific_Template,'VROT',min_error = Configuration['CHANNEL_WIDTH'])
     else:
         min_error = []
         pars_to_smooth = []
         not_to_smooth = []
         fixed_errors = []
         for parameter in ['VROT','INCL','Z0','SDIS','PA','XPOS','YPOS','VSYS']:
             if parameter in Configuration['FIXED_PARAMETERS'][0]:
                 not_to_smooth.append(parameter)
             else:
                 pars_to_smooth.append(parameter)
             min_error.append(Configuration['MIN_ERROR'][parameter])
-
+        warp_triggered = False
         for key,min_err in zip(pars_to_smooth,min_error):
-                smoothed = regularise_profile(Configuration,Tirific_Template,key,min_error = Configuration['MIN_ERROR'][parameter],debug = debug)
+                if key in ['PA','INCL']:
+                    if not warp_triggered:
+                        smoothed = regularise_warp(Configuration,Tirific_Template,\
+                            min_error = [Configuration['MIN_ERROR']['PA'],\
+                            Configuration['MIN_ERROR']['INCL']])
+                        warp_triggered = True
+                    else:
+                        pass
+                else:
+                    smoothed = regularise_profile(Configuration,Tirific_Template,key,min_error = Configuration['MIN_ERROR'][parameter])
                 if key == 'VROT':
                     smoothed_vrot=copy.deepcopy(smoothed)
 
         for key,min_err in zip(not_to_smooth,fixed_errors):
-            set_errors(Configuration,Tirific_Template,key,min_error = Configuration['MIN_ERROR'][parameter],debug = debug)
-
-    #if stage == 'after_cc':
-    #    smoothed_vrot = smooth_profile(Configuration,Tirific_Template,'VROT',min_error = Configuration['CHANNEL_WIDTH'],debug = debug)
-    #else:
-    #    smoothed_vrot = regularise_profile(Configuration,Tirific_Template,'VROT',min_error = Configuration['CHANNEL_WIDTH'],debug = debug)
-
-    #If our fit stage is after cc we want to make sure we do an extra check on low inclinations or small Galaxies
-    #if stage =='after_cc' and (Configuration['SIZE_IN_BEAMS'] < 5 or incl[0] < 50.):
-    #    check_inclination(Configuration,Tirific_Template,Fits_Files,debug=debug)
+            set_errors(Configuration,Tirific_Template,key,min_error = Configuration['MIN_ERROR'][parameter])
+    #
     if stage == 'after_cc':
 
         Tirific_Template['LOOPS'] = 1.
         if Configuration['OPTIMIZED']:
             Tirific_Template['INSET'] = f"{Fits_Files['FITTING_CUBE']}"
             Tirific_Template['INIMODE'] = "0"
-            finish_current_run(Configuration,current_run,debug= debug)
+            sf.finish_current_run(Configuration,current_run)
     else:
         Tirific_Template['LOOPS'] = f"{Configuration['LOOPS']}"
-        xpos,ypos,vsys,pa,incl = rf.load_tirific(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def",Variables = ['XPOS','YPOS','VSYS','PA','INCL'])
+        xpos,ypos,vsys,pa,incl = sf.load_tirific(Configuration,\
+            f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def",\
+            Variables = ['XPOS','YPOS','VSYS','PA','INCL'],array=True)
         parameters = {'VSYS': [vsys[0], Configuration['CHANNEL_WIDTH']], \
                       'XPOS': [xpos[0], Configuration['PIXEL_SIZE']],
                       'YPOS': [ypos[0], Configuration['PIXEL_SIZE']],
                       'INCL':[incl[0],10./np.sin(np.radians(incl[0]))],
                       'PA':  [pa[0],5.],
                       'VROT': [np.max(smoothed_vrot),np.max(smoothed_vrot)*0.05],  }
 
         if incl[0] < 40 and Configuration['NO_RINGS'] > 5.:
                 parameters_to_adjust = ['VSYS','SBR','XPOS','YPOS','PA','SDIS','VROT']
         else:
             parameters_to_adjust = ['NO_ADJUSTMENT'] #This triggers the default settings in set_fitting_parameters
 
         set_fitting_parameters(Configuration, Tirific_Template,stage = stage,\
-                          initial_estimates = parameters,parameters_to_adjust = parameters_to_adjust, debug = debug)
-
+                          initial_estimates = parameters,parameters_to_adjust = parameters_to_adjust)
 
-    target = f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Last_Unsmoothed_Input.def"
-    source = get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}_In.def")
-    target = get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Last_Unsmoothed_Input.def")
-    os.system(f"cp {source} {target}")
-    wf.tirific(Configuration,Tirific_Template,name = f'{fit_type}_In.def',debug=debug)
-    accepted,current_run = run_tirific(Configuration,current_run, stage = stage, fit_type=fit_type,debug=debug)
+    if Configuration['DEBUG']:
+        source = sf.get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}_In.def")
+        target = sf.get_system_string(f"{Configuration['LOG_DIRECTORY']}/{fit_type}_Last_Unsmoothed_Input.def")
+        os.system(f"cp {source} {target}")
+    wf.tirific(Configuration,Tirific_Template,name = f'{fit_type}_In.def')
+    if Configuration['DEBUG']:
+        source = sf.get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}_In.def")
+        target = sf.get_system_string(f"{Configuration['LOG_DIRECTORY']}/{fit_type}_Smoothed_Input.def")
+        os.system(f"cp {source} {target}")
+    try:
+        accepted,current_run = sf.run_tirific(Configuration,current_run, stage = stage, fit_type=fit_type)
+    except TirificOutputError:
+        accepted,current_run = failed_fit(Configuration,Tirific_Template,current_run,\
+            Fits_Files, stage=stage, fit_type=fit_type)
 
-    write_new_to_template(Configuration, f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template,debug = debug)
+    write_new_to_template(Configuration, f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template)
     if Configuration['NO_RINGS'] > 5.:
-        smoothed_vrot = regularise_profile(Configuration,Tirific_Template,'VROT',min_error = Configuration['CHANNEL_WIDTH'],debug = debug)
+        smoothed_vrot = regularise_profile(Configuration,Tirific_Template,'VROT',min_error = Configuration['CHANNEL_WIDTH'])
         set_fitting_parameters(Configuration, Tirific_Template,stage = 'final_os',\
-                          initial_estimates = parameters,parameters_to_adjust  = ['VROT'], debug = debug)
-        source = get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}_In.def")
-        target = get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_First_Smoothed_Input.def")
-        os.system(f"cp {source} {target}")
-        wf.tirific(Configuration,Tirific_Template,name = f'{fit_type}_In.def',debug=debug)
-        accepted,current_run = run_tirific(Configuration,current_run, stage = 'final_os', fit_type=fit_type,debug=debug)
+                          initial_estimates = parameters,parameters_to_adjust  = ['VROT'])
+
+        wf.tirific(Configuration,Tirific_Template,name = f'{fit_type}_In.def')
+        if Configuration['DEBUG']:
+            source = sf.get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}_In.def")
+            target = sf.get_system_string(f"{Configuration['LOG_DIRECTORY']}/{fit_type}_Second_Smoothed_Input.def")
+            os.system(f"cp {source} {target}")
+        try:
+            accepted,current_run = sf.run_tirific(Configuration,current_run, stage = 'final_os', fit_type=fit_type)
+        except TirificOutputError:
+            accepted,current_run = failed_fit(Configuration,Tirific_Template,\
+                current_run,Fits_Files, stage='final_os', fit_type=fit_type)
 
     return current_run
 fit_smoothed_check.__doc__ =f'''
  NAME:
     fit_smoothed_check
 
  PURPOSE:
@@ -735,15 +1072,15 @@
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
     Tirific_Template = Standard FAT Tirific Template
     current_run = subprocces structure of active tirific
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     stage = 'initial'
     stage of the fitting
 
     fit_type = 'Undefined'
     type of the fitting
 
@@ -753,27 +1090,40 @@
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
-def make_full_resolution(Configuration,Tirific_Template,Fits_Files,fit_type = 'Undefined', current_run = 'Not zed', debug = False):
-    update_statistic(Configuration, message= "Starting to make a full resolution model run", debug=debug)
-    if debug:
-        print_log(f'''MAKE_FULL_RESOLUTION: creating full resolution for stage {fit_type}.
-''',Configuration['OUTPUTLOG'],debug = True)
-    write_new_to_template(Configuration, f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template,debug = debug)
+def make_full_resolution(Configuration,Tirific_Template,Fits_Files,fit_type = 'Undefined', current_run = 'Not zed'):
+    sf.update_statistic(Configuration, message= "Starting to make a full resolution model run")
+
+    sf.print_log(f'''MAKE_FULL_RESOLUTION: creating full resolution for stage {fit_type}.
+''',Configuration,case= ['main','debug_start'])
+    write_new_to_template(Configuration, f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def", Tirific_Template)
     Tirific_Template['INSET'] = f"{Fits_Files['FITTING_CUBE']}"
+    Tirific_Template['VARY'] = f" VROT 1:3"
+    Tirific_Template['VARINDX'] = f" "
     Tirific_Template['LOOPS'] = "0"
     Tirific_Template['INIMODE'] = "0"
     wf.tirific(Configuration,Tirific_Template,name = f'{fit_type}_In.def')
-    finish_current_run(Configuration,current_run,debug= debug)
-    accepted,current_run = run_tirific(Configuration,'Not zed', stage = 'full_res', fit_type=fit_type,debug = debug)
-    finish_current_run(Configuration,current_run,debug= debug)
+    if Configuration['DEBUG']:
+        wf.tirific(Configuration,Tirific_Template,\
+            name = f'{Configuration["LOG_DIRECTORY"]}/Full_Resolution_Input.def',\
+            full_name = True )
+    sf.finish_current_run(Configuration,current_run)
+    try:
+        accepted,current_run = sf.run_tirific(Configuration,'Not zed', \
+            stage = 'full_res', fit_type=fit_type)
+    except TirificOutputError:
+        accepted,current_run = failed_fit(Configuration,Tirific_Template,\
+            'Not Zed', Fits_Files,stage='full_res', fit_type=fit_type)
+
+
+    sf.finish_current_run(Configuration,current_run)
 make_full_resolution.__doc__ =f'''
  NAME:
     make_full_resolution
 
  PURPOSE:
     If we used an optimized cube we want to make the final fit at the original resolution.
 
@@ -782,15 +1132,15 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
     Tirific_Template = Standard FAT Tirific Template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     fit_type = 'Undefined'
     type of fitting
 
     current_run = 'Not zed'
     subprocess structure of tirific
 
@@ -800,89 +1150,122 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def one_step_converge(Configuration, Fits_Files,Tirific_Template,current_run, debug = False):
+def one_step_converge(Configuration, Fits_Files,Tirific_Template,current_run):
 
-    print_log(f'''ONE_STEP_CONVERGENCE: Starting with loop {Configuration['ITERATIONS']} out of maximum {Configuration['MAX_ITERATIONS']}.
-''',Configuration['OUTPUTLOG'],screen=True,debug = debug)
+    sf.print_log(f'''ONE_STEP_CONVERGENCE: For {Configuration['ID']} we are starting loop {Configuration['ITERATIONS']} out of maximum {Configuration['MAX_ITERATIONS']}.
+''',Configuration, case=['main','screen','debug_start'])
     fit_type = 'Fit_Tirific_OSC'
     stage = 'run_os'
     #First we run tirific
-    accepted,current_run = run_tirific(Configuration,current_run,stage = stage, fit_type = fit_type, debug= debug)
+    try:
+        accepted,current_run = sf.run_tirific(Configuration,current_run,\
+            stage = stage, fit_type = fit_type)
+    except TirificOutputError:
+        accepted,current_run = failed_fit(Configuration,Tirific_Template,\
+            current_run, Fits_Files,stage=stage, fit_type=fit_type)
+
+
+    if not accepted:
+        Configuration['ACCEPTED_TIRIFIC'] = False
+        if Configuration['LOOPS'] < 20.:
+            sf.print_log(f'''ONE_STEP_CONVERGENCE: Tirific ran the maximum amount of loops ({Configuration['LOOPS']}) increasing this by 1.
+''',Configuration)
+            Configuration['LOOPS'] += 1
+    else:
+        Configuration['ACCEPTED_TIRIFIC'] = True
     #Then we load the produced output into our template
-    write_new_to_template(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def" , Tirific_Template, debug = debug)
+    write_new_to_template(Configuration,f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.def" , Tirific_Template)
     #Check that the centre does not deviate too much
-    if debug:
-        print_log(f'''CHECK THAT WE CAHANGE !!!!!!
-{Tirific_Template['VROT']}
-{Tirific_Template['PA']}
-{Tirific_Template['XPOS']}
-''',Configuration['OUTPUTLOG'])
-    accepted_central = check_central_convergence(Configuration,Tirific_Template, fit_type = fit_type,debug=debug)
-    if debug:
-        print_log(f'''CHECK THAT WE CAHANGE !!!!!!
-{Tirific_Template['VROT']}
-{Tirific_Template['PA']}
-{Tirific_Template['XPOS']}
-''',Configuration['OUTPUTLOG'])
+
+    accepted_central = check_central_convergence(Configuration,Tirific_Template, fit_type = fit_type)
+    if accepted_central:
+        Configuration['CENTRAL_CONVERGENCE'] = True
+        Configuration['CENTRAL_CONVERGENCE_COUNTER'] += 1.
+        Configuration['CENTRAL_FIX'] = []
 
     # Check whether we have the correct sizes,
-    accepted_size = check_size(Configuration,Tirific_Template, fit_type = fit_type, stage = stage, current_run = current_run, debug=debug,Fits_Files=Fits_Files)
-    if accepted and accepted_size and accepted_central:
+
+    #This currently doesn't do anything
+    #accepted_proj_vrot = check_vobs(Configuration,Tirific_Template, fit_type = fit_type)
+    # Check whether the central INCL and PA are stable. But only if the center is accepted
+    if accepted_central:
+        accepted_angle = check_angle_convergence(Configuration,Tirific_Template, fit_type = fit_type)
+    else:
+        accepted_angle = False
+    #We only adapt the size if the other checks are ok
+    if not all(Configuration['FIX_SIZE']) and accepted_central and accepted_angle:
+        no_apply_size_change = False
+    else:
+        no_apply_size_change = True
+    accepted_size = check_size(Configuration,Tirific_Template, \
+        no_apply = no_apply_size_change, fit_type = fit_type, stage = stage, \
+        current_run = current_run,Fits_Files=Fits_Files)
+    if all(Configuration['FIX_SIZE']):
+        accepted_size = True
+    if accepted and accepted_size and accepted_central and accepted_angle: #and accepted_proj_vrot:
         Configuration['ACCEPTED'] = True
     else:
         Configuration['ACCEPTED'] = False
         if Configuration['ITERATIONS'] > Configuration['MAX_ITERATIONS']:
-                print_log(f'''ONE_STEP_CONVERGENCE: We have ran the convergence more than {Configuration['MAX_ITERATIONS']} times aborting the fit.
-    ''',Configuration['OUTPUTLOG'])
+                sf.print_log(f'''ONE_STEP_CONVERGENCE: We have ran the convergence more than {Configuration['MAX_ITERATIONS']} times aborting the fit.
+''',Configuration)
                 return current_run
         if not accepted:
-            print_log(f'''ONE_STEP_CONVERGENCE: Tirific ran the maximum amount of loops hence we do not accept and we smooth and retry.
-''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''ONE_STEP_CONVERGENCE: Tirific ran the maximum amount of loops hence we do not accept and we smooth and retry.
+''',Configuration)
         if not accepted_central:
-            print_log(f'''ONE_STEP_CONVERGENCE: The center varied too much hence we do not accept and we smooth and retry.
-''',Configuration['OUTPUTLOG'])
-        if not accepted_size:
-            print_log(f'''ONE_STEP_CONVERGENCE: FAT adjusted the rings. Refitting with new settings after smoothing them.
-''',Configuration['OUTPUTLOG'])
+            sf.print_log(f'''ONE_STEP_CONVERGENCE: The center varied too much hence we do not accept and we smooth and retry.
+''',Configuration)
+        elif not accepted_angle:
+            sf.print_log(f'''ONE_STEP_CONVERGENCE: The central disk PA or INCL have changed too much or the boundaries have been adapted.
+''',Configuration)
+        elif not accepted_size:
+            sf.print_log(f'''ONE_STEP_CONVERGENCE: FAT adjusted the rings. Refitting with new settings after smoothing them.
+''',Configuration)
 
-        check_angles(Configuration,Tirific_Template,debug = debug)
 
-                    # First we fix the SBR we are left with also to set the reliable ring to configuration.
-        fix_sbr(Configuration,Tirific_Template,debug = debug)    # Then we determine the inner rings that should remain fixed
+        #if not accepted_proj_vrot:
+        #    sf.print_log(f'''ONE_STEP_CONVERGENCE: The outer VROT and INCL did not converge on the minimumal change that allows for VROT*Sin(INCL)
+#''',Configuration)
 
-        get_inner_fix(Configuration, Tirific_Template,debug=debug)
+
+        # First we fix the SBR we are left with also to set the reliable ring to configuration.
+        fix_sbr(Configuration,Tirific_Template,smooth = True)    # Then we determine the inner rings that should remain fixed
+
+        sf.get_inner_fix(Configuration, Tirific_Template)
 
         if all([True if x  in Configuration['FIXED_PARAMETERS'][0] else False for x in ['PA','INCL','Z0','SDIS']] ):
         #if all([Configuration['FIX_INCLINATION'][0],Configuration['FIX_PA'][0],Configuration['FIX_Z0'][0],Configuration['FIX_SDIS'][0]]):
-            Configuration['WARP_SLOPE'] = [0.,0.]
+            Configuration['WARP_SLOPE'] = [None ,None ]
         else:
-            get_warp_slope(Configuration,Tirific_Template, debug=debug)
+            get_warp_slope(Configuration,Tirific_Template)
 
-        set_cflux(Configuration,Tirific_Template,debug = debug)
-        keys_to_smooth =['INCL','PA','SDIS','Z0','VROT']
-        min_errors = [3.*np.mean(Configuration['LIMIT_MODIFIER']),2.,Configuration['CHANNEL_WIDTH']/(2.*Configuration['LIMIT_MODIFIER']), \
-                        convertskyangle(Configuration,0.1,Configuration['DISTANCE'],physical= True)/Configuration['LIMIT_MODIFIER'],\
+        set_cflux(Configuration,Tirific_Template)
+        #keys_to_smooth =['INCL','PA','SDIS','Z0','VROT']
+        #min_errors = [3.*np.mean(Configuration['LIMIT_MODIFIER']),2.,Configuration['CHANNEL_WIDTH']/(2.*Configuration['LIMIT_MODIFIER']), \
+        #                sf.convertskyangle(Configuration,0.1,physical= True)/Configuration['LIMIT_MODIFIER'],\
+        #                Configuration['CHANNEL_WIDTH']/(Configuration['LIMIT_MODIFIER'])]
+        keys_to_smooth =['SDIS','Z0','VROT']
+        min_errors = [Configuration['CHANNEL_WIDTH']/(2.*Configuration['LIMIT_MODIFIER']), \
+                        sf.convertskyangle(Configuration,0.1,physical= True)/Configuration['LIMIT_MODIFIER'],\
                         Configuration['CHANNEL_WIDTH']/(Configuration['LIMIT_MODIFIER'])]
         for j,key in enumerate(keys_to_smooth):
             #Smoothing the profile also fixes it
-            smoothed = smooth_profile(Configuration,Tirific_Template,key,debug=debug,min_error=min_errors[j])
+            smoothed = smooth_profile(Configuration,Tirific_Template,key,min_error=min_errors[j])
+        smoothed = regularise_warp(Configuration,Tirific_Template,
+                    min_error=[2.,3.*np.mean(Configuration['LIMIT_MODIFIER'])],smooth_only=True)
+
+        set_fitting_parameters(Configuration, Tirific_Template,stage = 'run_os')
 
-        set_fitting_parameters(Configuration, Tirific_Template,stage = 'run_os',\
-                             debug = debug)
-        print_log(f'''CHECK THAT WE CAHANGE !!!!!!
-        {Tirific_Template['VROT']}
-        {Tirific_Template['PA']}
-        {Tirific_Template['XPOS']}
-        ''',Configuration['OUTPUTLOG'])
-        wf.tirific(Configuration,Tirific_Template,name = f"{Configuration['USED_FITTING']}_In.def",debug = debug)
+        wf.tirific(Configuration,Tirific_Template,name = f"{Configuration['USED_FITTING']}_In.def")
     return current_run
 one_step_converge.__doc__ =f'''
  NAME:
     one_step_converge
 
  PURPOSE:
     Converge on a best fitmodel without smoothing.
@@ -893,87 +1276,74 @@
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
     Tirific_Template = Standard FAT Tirific Template
     current_run = subprocess structure of tirific
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     current_run = subprocess structure with the current tirific call.
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE: This routine sets the Configuration['ACCEPTED']
 '''
 
-def sofia(Configuration, Fits_Files, debug = False):
-    if debug:
-        print_log(f'''RUN_SOFIA: starting sofia run from the template.
-''',Configuration['OUTPUTLOG'],debug = True)
-    update_statistic(Configuration, message= "Starting the SoFiA run", debug=debug)
+def sofia(Configuration, Fits_Files):
+    sf.print_log(f'''RUN_SOFIA: starting sofia run from the template.
+''',Configuration,case= ['debug_start'])
+    sf.update_statistic(Configuration, message= "Starting the SoFiA run")
 
-    sofia_template = rf.sofia_template(debug=debug)
-    create_directory('Sofia_Output',Configuration['FITTING_DIR'])
+    sofia_template = rf.sofia_template()
+    sf.create_directory('Sofia_Output',Configuration['FITTING_DIR'])
     os.chdir(Configuration['FITTING_DIR'])
     threshold = 5.
     counter = 3
     sofia_template['input.data'] = Fits_Files['FITTING_CUBE']
-    spatial_kernels = [0,int(round(Configuration['BEAM_IN_PIXELS'][0])),int(round(Configuration['BEAM_IN_PIXELS'][0]))*2]
-    if np.sum(Configuration['NAXES'][:2])/(2.*int(round(Configuration['BEAM_IN_PIXELS'][0])))  > 30:
-        spatial_kernels.append(int(round(Configuration['BEAM_IN_PIXELS'][0]))*3)
-        print_log(f'''RUN_SOFIA: Adding an extra kernel scale as the cube is more than 30 beams across.
-''', Configuration['OUTPUTLOG'])
+    spatial_kernels,velocity_kernels = construct_kernels(Configuration,sofia_template)
 
-    velocity_kernels = [0,3,6,12]
-    if Configuration['NAXES'][2] > 52:
-        velocity_kernels.append(16)
-        Configuration['VEL_SMOOTH_EXTENDED'] = True
-        print_log(f'''RUN_SOFIA: Adding an extra kernel scale as the cube has more than 52 channels.
-''', Configuration['OUTPUTLOG'])
-    sofia_template['scfind.kernelsXY'] = ','.join([str(x) for x in spatial_kernels])
-    sofia_template['scfind.kernelsZ'] = ','.join([str(x) for x in velocity_kernels])
     sofia_ok = False
     while not sofia_ok:
-        clean_before_sofia(Configuration,debug=debug)
+        clean_before_sofia(Configuration)
         sofia_template['scfind.threshold'] = str(threshold)
         wf.sofia(sofia_template,'sofia_input.par')
-        print_log("RUN_SOFIA: Running SoFiA. \n",Configuration['OUTPUTLOG'],screen = True)
+        sf.print_log("RUN_SOFIA: Running SoFiA. \n",Configuration)
         # Check which sofia to start
         sfrun = subprocess.Popen([Configuration['SOFIA2'],'sofia_input.par'], stdout = subprocess.PIPE, stderr = subprocess.PIPE)
         sofia_run, sofia_warnings_are_annoying = sfrun.communicate()
-        print_log(sofia_run.decode("utf-8"), Configuration['OUTPUTLOG'])
+        sf.print_log(sofia_run.decode("utf-8"), Configuration)
 
         if sfrun.returncode == 8:
             if threshold > 3.:
                 log_statement = f'''RUN_SOFIA: We did not find a source at a threshold of {threshold}
 {"":8s} RUN_SOFIA: Lowering the threshold and trying again."
 '''
-                print_log(log_statement,Configuration['OUTPUTLOG'])
-                threshold -= 1
+                sf.print_log(log_statement,Configuration)
+                threshold -= 2
             else:
                 clean_after_sofia(Configuration)
                 log_statement = f'''RUN_SOFIA: We did not find a source above a threshold of {threshold}.
 {"":8s}RUN_SOFIA: We cannot lower the threshold lower as the risk of fitting noise becomes too high.
 {"":8s}Continuing to the next galaxy.
 '''
-                print_log(log_statement,Configuration['OUTPUTLOG'])
-                raise SofiaFaintError("RUN_SOFIA:Sofia cannot find a source above a threshold of 3.")
+                sf.print_log(log_statement,Configuration)
+                raise FaintSourceError("RUN_SOFIA:Sofia cannot find a source above a threshold of 3.")
         elif sfrun.returncode == 0:
             sofia_ok = True
         else:
-            print_log(sofia_warnings_are_annoying.decode("utf-8"), Configuration['OUTPUTLOG'])
+            sf.print_log(sofia_warnings_are_annoying.decode("utf-8"), Configuration,case=['main','screen'])
             raise SofiaRunError("RUN_SOFIA:Sofia did not execute properly. See log for details")
 
     #Move sofia output to the desired Directory
-    clean_after_sofia(Configuration,debug=debug)
+    clean_after_sofia(Configuration)
     Configuration['SOFIA_RAN'] = True
     os.chdir(Configuration['START_DIRECTORY'])
 sofia.__doc__ =f'''
  NAME:
     sofia
 
  PURPOSE:
@@ -983,118 +1353,81 @@
     run_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
 
  OPTIONAL INPUTS:
-    debug = False
+
 
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def tirshaker_call(Configuration,debug = False):
+
+def tirshaker_call(Configuration):
     # First we make a directory to keep all contained
-    update_statistic(Configuration, message= "Starting the Tirshaker call run", debug=debug)
+    sf.update_statistic(Configuration, message= "Starting the Tirshaker call run")
     if not os.path.isdir(f"{Configuration['FITTING_DIR']}/Error_Shaker/"):
         os.mkdir(f"{Configuration['FITTING_DIR']}/Error_Shaker/")
 
 
     # Then we open the final file
     filename = f"{Configuration['FITTING_DIR']}Error_Shaker/Error_Shaker_In.def"
 
     final_FAT_file= f"{Configuration['FITTING_DIR']}{Configuration['USED_FITTING']}/{Configuration['USED_FITTING']}.def"
 
-    Tirific_Template = tirific_template(filename = final_FAT_file \
-                    , debug = debug)
+    Tirific_Template = sf.tirific_template(filename = final_FAT_file \
+                    )
     #Change the name and run only 2 LOOPS
     Tirific_Template['RESTARTNAME']= f"restart_Error_Shaker.txt"
     Tirific_Template['INSET'] = f"../{Tirific_Template['INSET']}"
     Tirific_Template['TIRDEF']= f"Error_Shaker_Out.def"
     Tirific_Template['LOOPS'] = '1'
 
     outfilename = 'Error_Shaker.def'
     outfileprefix = 'Error_Shaker'
 
     #This we need to remove from the actual run
     #Configuration['NO_RINGS'] = int(Tirific_Template['NUR'])
     #Configuration['RING_SIZE'] = 1.
     #Configuration['SIZE_IN_BEAMS'] = Configuration['NO_RINGS']-2
-    set_fitting_parameters(Configuration, Tirific_Template,stage = 'run_os',\
-                         debug = debug)
+    set_fitting_parameters(Configuration, Tirific_Template,stage = 'run_os')
 
     #Write it back to the file
-    wf.tirific(Configuration,Tirific_Template, name =f"Error_Shaker/Error_Shaker_In.def" , debug = debug)
+    wf.tirific(Configuration,Tirific_Template, name =f"Error_Shaker/Error_Shaker_In.def" )
 
     #Determine the error block from the last fit settings.
-    parameter_groups,rings,block,variation,variation_type = get_fit_groups(Configuration,Tirific_Template,debug = debug)
-    if debug:
-        print_log(f'''TIRSHAKER_CALL: We are shaking with the following parameters:
+    parameter_groups,rings,block,variation,variation_type = sf.get_fit_groups(Configuration,Tirific_Template)
+    sf.print_log(f'''TIRSHAKER_CALL: We are shaking with the following parameters:
 {'':8s}groups = {parameter_groups}
 {'':8s}rings = {rings}
 {'':8s}block = {block}
 {'':8s}variation = {variation}
 {'':8s}variation_type = {variation_type}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_add'])
 
     iterations = Configuration['SHAKER_ITERATIONS']
     random_seed = 2
     os.chdir(f"{Configuration['FITTING_DIR']}/Error_Shaker/")
     tirshaker(Configuration,Tirific_Template, outfilename = outfilename,\
                 outfileprefix = outfileprefix, parameter_groups = parameter_groups, \
                 rings = rings, block = block, variation = variation,\
                  variation_type = variation_type, iterations = iterations,
-                 random_seed = random_seed, mode = 'mad',debug=debug)
+                 random_seed = random_seed, mode = 'mad')
     os.chdir(f"{Configuration['START_DIRECTORY']}")
-    '''
-    try:
-        os.remove(f"{Configuration['FITTING_DIR']}Error_Shaker/blatirshin")
-    except:
-        pass
-    try:
-        os.remove(f"{Configuration['FITTING_DIR']}Error_Shaker/blatirlog")
-    except:
-        pass
-    #remove the duplicate line in the shaker output
-    # make sure all duplicate are removed
-
-    outshaker = open(f"{Configuration['FITTING_DIR']}Error_Shaker/{outfilename}", 'r').readlines()
-    lines_set = set(outshaker)
-
-    with open(f"{Configuration['FITTING_DIR']}Error_Shaker/{outfilename}", 'w') as out:
-        for line in lines_set:
-            out.write(line)
-
-    #Let's load the   the tirshaker output
-    err_var =[]
-    for group in parameter_groups:
-        for par in group:
-            if f'ERR_{par[:-1]}' not in err_var:
-                err_var.append(f'ERR_{par[:-1]}')
-    errors = rf.load_tirific(Configuration,f"{Configuration['FITTING_DIR']}Error_Shaker/{outfilename}",Variables = err_var,
-                     unpack = False , debug = debug )
-
-    for para in err_var:
-        key=para[4:]
-        FAT_err = f'# {key}_ERR'
-        format = set_format(key)
-        if FAT_err in Tirific_Template:
-            Tirific_Template[FAT_err]= f"{' '.join([f'{x:{format}}' for x in errors[:int(Configuration['NO_RINGS']),err_var.index(para)]])}"
-        else:
-            Tirific_Template.insert(key,f"# {key}_ERR",f"{' '.join([f'{x:{format}}' for x in errors[:int(Configuration['NO_RINGS']),err_var.index(para)]])}")
-'''
-    wf.tirific(Configuration,Tirific_Template,name=f"{Configuration['USED_FITTING']}/{Configuration['USED_FITTING']}.def", debug = debug)
+
+    wf.tirific(Configuration,Tirific_Template,name=f"{Configuration['USED_FITTING']}/{Configuration['USED_FITTING']}.def")
 
 tirshaker_call.__doc__ =f'''
  NAME:
     tirshaker
 
  PURPOSE:
     function to setup the right input for tirshaker and call it and afterwards process the results
@@ -1102,15 +1435,15 @@
  CATEGORY:
     run_functions
 
  INPUTS:
     Configuration
 
  OPTIONAL INPUTS:
-    debug = False
+
 
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/Support/support_functions.py` & `pyFAT_astro-0.1.1/pyFAT_astro/Support/support_functions.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,44 +1,52 @@
 # -*- coding: future_fstrings -*-
 # This module contains a set of functions and classes that are used in several different Python scripts in the Database.
-
+import pyFAT_astro
 from pyFAT_astro.Support.fat_errors import SupportRunError,SmallSourceError,\
                                               FileNotFoundError,TirificKillError,\
-                                              InputError,ProgramError,DefFileError
+                                              InputError,ProgramError,DefFileError,\
+                                              BadHeaderError,FittingError,TirificOutputError
+
+from pyFAT_astro import Templates as templates
 from collections import OrderedDict #used in Proper_Dictionary
 from inspect import getframeinfo,stack
-
+from numpy.linalg import LinAlgError
 from scipy.optimize import curve_fit, OptimizeWarning
 from scipy import ndimage
+from scipy.signal import savgol_filter
 from astropy.wcs import WCS
 from astropy.io import fits
 from dataclasses import  asdict
 try:
     from importlib.resources import files as import_pack_files
 except ImportError:
     # Try backported to PY<37 `importlib_resources`.
     # For Py<3.9 files is not available
     from importlib_resources import files as import_pack_files
-
+try:
+    from importlib.resources import open_text as pack_open_txt
+except ImportError:
+    # Try backported to PY<37 `importlib_resources`.
+    from importlib_resources import open_text as pack_open_txt
 import matplotlib.pyplot as plt
 import os
 import sys
 import inspect
 import psutil as psu
 import signal
 import time
 import traceback
 import numpy as np
 import copy
 import warnings
 import re
 import subprocess
+import omegaconf
 from datetime import datetime
-class BadHeaderError(Exception):
-    pass
+
 # A class of ordered dictionary where keys can be inserted in at specified locations or at the end.
 class Proper_Dictionary(OrderedDict):
     def __setitem__(self, key, value):
         if key not in self:
             # If it is a new item we only allow it if it is not Configuration or Original_Cube or if we are in setup_configuration
             function,variable,empty = traceback.format_stack()[-2].split('\n')
             function = function.split()[-1].strip()
@@ -72,38 +80,37 @@
         if not done:
             print("----!!!!!!!!We were unable to add your key!!!!!!---------")
 
 Proper_Dictionary.__doc__=f'''
 A class of ordered dictionary where keys can be inserted in at specified locations or at the end.
 '''
 
-def calc_rings(Configuration,size_in_beams = 0., ring_size  = 0.,debug=False):
+def calc_rings(Configuration,size_in_beams = 0., ring_size  = 0.):
     if ring_size == 0.:
         ring_size = Configuration['RING_SIZE']
     if size_in_beams == 0.:
-        size_in_beams = Configuration['SIZE_IN_BEAMS']
-    if debug:
-        print_log(f'''CALC_RINGS: Calculating the number of rings in the model.
+        size_in_beams = np.max(Configuration['SIZE_IN_BEAMS'])
+    print_log(f'''CALC_RINGS: Calculating the number of rings in the model.
 {'':8s} size in beams = {size_in_beams}
 {'':8s} ring_size = {ring_size}
 {'':8s} the maximum amount of rings = {Configuration['MAX_SIZE_IN_BEAMS']}
-''',Configuration['OUTPUTLOG'],debug = True)
-    est_rings = round((size_in_beams)/(ring_size)+2.)
+''',Configuration,case= ['debug_start'])
+
+    est_rings = round((size_in_beams-1./5.)/(ring_size)+2.)
     #if est_rings > 20 and Configuration['MAX_SIZE_IN_BEAMS'] > 25:
     if est_rings > 20:
         Configuration['OUTER_RINGS_DOUBLED'] = True
         # 0.5 should always be rounding up else we get problemsin the reverse
         no_rings = 2+10+np.floor((est_rings-12)/2.+0.5)
     else:
         Configuration['OUTER_RINGS_DOUBLED'] = False
         no_rings = est_rings
-    if debug:
-        print_log(f'''CALC_RINGS: The model will have {no_rings} Rings.
-{'':8s} We estimated {est_rings} and double outer rings is {Configuration['OUTER_RINGS_DOUBLED']}
-''',Configuration['OUTPUTLOG'])
+    print_log(f'''CALC_RINGS: We started with ring size = {ring_size} and the size in beams {size_in_beams}.
+{'':8s}The model will have {no_rings} rings and the rings are {'doubled' if Configuration['OUTER_RINGS_DOUBLED'] else 'not doubled'}.
+''',Configuration,case= ['debug_add'])
     return int(no_rings)
 
 calc_rings.__doc__ =f'''
  NAME:
     calc_rings
 
  PURPOSE:
@@ -112,15 +119,15 @@
  CATEGORY:
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     size_in_beams = 0.
     Radius of the model in beams. Default from Configuration
 
     ring_size  = 0.
     size of the rings in the model. Default from Configuration
 
@@ -130,16 +137,337 @@
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
+def calculate_number_processes(Configuration):
+    cores_set = False
+    no_galaxies = set_limits(Configuration['CATALOGUE_END_ID']-Configuration['CATALOGUE_START_ID'],1,float('inf'))
+    while not cores_set:
+        no_process= int(np.floor(Configuration['NCPU']/ Configuration['PER_GALAXY_NCPU']))
+        while no_process > no_galaxies:
+            no_process -= 1
+            cores_set = True
+        extra_cores=  Configuration['NCPU']-  Configuration['PER_GALAXY_NCPU']*no_process
+        if not cores_set and \
+            extra_cores >= Configuration['PER_GALAXY_NCPU']*no_process/2. and \
+            Configuration['PER_GALAXY_NCPU'] > 3.:
+            Configuration['PER_GALAXY_NCPU'] -= 1
+        else:
+            cores_set = True
+
+
+    while no_process < extra_cores:
+        extra_cores -= no_process
+        Configuration['PER_GALAXY_NCPU'] += 1
+
+    input_cores = copy.deepcopy(Configuration['PER_GALAXY_NCPU'])
+    while no_process <= extra_cores:
+        Configuration['PER_GALAXY_NCPU'] += 1
+        extra_cores -= no_process
+    if Configuration['PER_GALAXY_NCPU'] > 2.*input_cores:
+        Configuration['PER_GALAXY_NCPU'] =  2.*input_cores
+
+    print(f"We use {no_process} processes for {no_galaxies} galaxies")
+    print(f"With {Configuration['PER_GALAXY_NCPU']} per galaxy")
+    #The updated Configuration should be modified automatically
+    return no_process
+
+calculate_number_processes.__doc__ =f'''
+ NAME:
+    calculate_number_processes
+
+ PURPOSE:
+    Calculate the optimal number of processs and create Configurations for each of them.
+
+ CATEGORY:
+    support_functions
+
+ INPUTS:
+    Configuration = Standard Original FAT configuration
+
+ OPTIONAL INPUTS:
+
+ OUTPUTS:
+    a set of Configurations for each process.
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+def complex_am_invert(Configuration,Theta_in,Phi_in):
+    print_log(f'''COMPLEX_AM_INVERT:  as PA or INCL in {Configuration['FIXED_PARAMETERS']} we are doing a complex invert.
+''',Configuration,case= ['debug_start'])
+
+    Theta_out = copy.deepcopy(Theta_in)
+    Phi_out = copy.deepcopy(Phi_in)
+    Theta_out[0]=Theta_in[0]
+    Phi_out[0]=Phi_in[0]
+    if 'INCL' in Configuration['FIXED_PARAMETERS'] and 'PA' in Configuration['FIXED_PARAMETERS']:
+        Theta_out[:]=Theta_in[0]
+        Phi_out[:]=Phi_in[0]
+        print_log(f'''COMPLEX_AM_INVERT:  both PA and INCL are fixed returning the centra Phi and Theta.
+''',Configuration,case= ['debug_add'])
+    else:
+        #Create the PA and Inclination plane
+        Theta = np.linspace(0,np.pi,1000)
+        Phi = np.linspace(0,np.pi,1000)
 
-def check_sofia(Configuration,Fits_Files,debug=False):
+
+        if 'INCL' in Configuration['FIXED_PARAMETERS']:
+            Inclination_plane =   np.zeros((len(Theta),len(Phi)))
+            with warnings.catch_warnings():
+                warnings.filterwarnings("ignore",message="divide by zero encountered in true_divide"\
+                                    ,category=RuntimeWarning)
+                for i in range(len(Theta)):
+                    Inclination_plane[:,i]= 90-np.arctan(1./(np.cos(Theta[i])*np.tan(Phi[:])))*(360./(2*np.pi))
+            Inclination_plane[np.where(Inclination_plane > 90.)] = 180 - Inclination_plane[np.where(Inclination_plane > 90.)]
+            Inclination_plane[np.where(Inclination_plane < 0.)] = -1 * Inclination_plane[np.where(Inclination_plane < 0.)]
+            current_inclination =  90-np.arctan(1./(np.cos(Theta_in[:])*np.tan(Phi_in[:])))*(360./(2*np.pi))
+            current_inclination[np.where(current_inclination > 90.)] = 180 - current_inclination[np.where(current_inclination > 90.)]
+            current_inclination[np.where(current_inclination < 0.)] = -1 * current_inclination[np.where(current_inclination < 0.)]
+            current_diff = np.array([abs(x-current_inclination[0]) for x in current_inclination],dtype=float)
+            not_flat = np.where(current_diff > 0.25)[0]
+            if not_flat.size != 0:
+                options_are = np.where(np.logical_and(current_inclination[0]-0.25 < Inclination_plane, Inclination_plane < current_inclination[0]+0.25))
+                options_Phi = Phi[options_are[0][:]]
+                options_Theta = Theta[options_are[1][:]]
+                for i in range(not_flat.size):
+                    diff = [abs(x-Phi_in[not_flat[i]])+abs(y-Theta_in[not_flat[i]]) for x,y in zip(options_Phi,options_Theta)]
+                    location= np.where(np.min(diff) == diff)[0]
+                    Phi_out[not_flat[i]]=options_Phi[location[0]]
+                    Theta_out[not_flat[i]]=options_Theta[location[0]]
+        if 'PA' in Configuration['FIXED_PARAMETERS']:
+            PA_plane =   np.zeros((len(Theta),len(Phi)))
+            with warnings.catch_warnings():
+                warnings.filterwarnings("ignore",message="divide by zero encountered in true_divide"\
+                                    ,category=RuntimeWarning)
+                for i in range(len(Theta)):
+                    PA_plane[:,i] = abs(np.arctan(np.sin(Theta[i])*np.tan(Phi[:]))*(360./(2*np.pi)))
+
+            current_pa = abs(np.arctan(np.sin(Theta_in[:])*np.tan(Phi_in[:]))*(360./(2*np.pi)))
+            current_diff = np.array([abs(x-current_pa[0]) for x in current_pa],dtype=float)
+            not_flat = np.where(current_diff > 0.25)[0]
+            if not_flat.size != 0:
+                print(f'Starting the search for a constant PA')
+                options_are = np.where(np.logical_and(current_pa[0]-0.25 < PA_plane, PA_plane < current_pa[0]+0.25))
+                options_Phi = Phi[options_are[0][:]]
+                options_Theta = Theta[options_are[1][:]]
+                for i in range(not_flat.size):
+                    diff = [abs(x-Phi_in[not_flat[i]])+abs(y-Theta_in[not_flat[i]]) for x,y in zip(options_Phi,options_Theta)]
+                    location= np.where(np.min(diff) == diff)[0]
+                    Phi_out[not_flat[i]]=options_Phi[location[0]]
+                    Theta_out[not_flat[i]]=options_Theta[location[0]]
+
+
+    return Theta_out,Phi_out
+
+
+def calculate_am_vector(Configuration,PA_in,Inclination_in,multiple = [None], invert=False):
+    if multiple[0] == None and invert:
+        print_log(f'''CALCULATE_AM_VECTOR: inverting phi and theta without the multiple will result in all PAs being in the first quadrant.
+''',Configuration,case= ['debug_start'])
+        multiple=np.zeros(len(PA_in))
+
+    if invert:
+        Theta=np.array(PA_in,dtype=float)
+        Phi=np.array(Inclination_in,dtype=float)
+        if 'INCL' in Configuration['FIXED_PARAMETERS'] or 'PA' in Configuration['FIXED_PARAMETERS']:
+            Theta,Phi = complex_am_invert(Configuration,Theta,Phi)
+
+        Inclination=90-np.arctan(1./(np.cos(Theta)*np.tan(Phi)))*(360./(2*np.pi))
+    # return inclination boundary adjustements
+        Inclination[np.where(Inclination > 90.)] = 180 - Inclination[np.where(Inclination > 90.)]
+        Inclination[np.where(Inclination < 0.)] = -1 * Inclination[np.where(Inclination < 0.)]
+        if (Phi[0] < np.pi/2.) and (Phi[-1] > np.pi/2) and (Inclination[0] < 5.):
+            PA= np.arctan(np.sin(Theta)*np.tan(Phi-np.pi/2.))*(360./(2*np.pi))\
+                        +multiple*90.+np.arctan(np.sin(Theta[0])*np.tan(Phi[0]))*(360./(2*np.pi))
+        else:
+            PA= abs(np.arctan(np.sin(Theta)*np.tan(Phi))*(360./(2*np.pi)))+multiple*90.
+        # And make sure the inner 3 rings are the same
+        Inclination[0:3] = np.mean(Inclination[0:3])
+        PA[0:3] = np.mean(PA[0:3])
+        return PA,Inclination
+    else:
+        # For this the PA has to be between 0-90
+        PA=np.array(PA_in,dtype=float)
+        Inclination=np.array(Inclination_in,dtype=float)
+        multiple=np.floor(PA/90.)
+        PA= PA-multiple*90.
+        #if any(PA > 90.):
+
+        Inclination= 90.-Inclination
+        PA[np.where(PA == 0.)] = 0.001
+        Inclination[np.where(Inclination == 0.)] = 0.001
+        Theta=np.arctan(abs(np.tan(Inclination*(np.pi/180.)))*abs(np.tan(PA*(np.pi/180.))))
+        Phi = np.arctan(abs(np.tan(PA*(np.pi/180.)))/np.sin(Theta))
+
+        return Theta,Phi,multiple
+calculate_am_vector.__doc__ =f'''
+ NAME:
+    calculate_am_vector
+
+ PURPOSE:
+    Calculate the optimal number of processs and create Configurations for each of them.
+
+ CATEGORY:
+    support_functions
+
+ INPUTS:
+    Configuration = Standard Original FAT configuration
+
+ OPTIONAL INPUTS:
+
+ OUTPUTS:
+    a set of Configurations for each process.
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+
+
+def check_angular_momentum_vector(Configuration,radius_in,pa_in,inclination_in,\
+                                    modified= False,side=0):
+
+    inclination = np.array(inclination_in)
+    pa = np.array(pa_in)
+    inclination_in = np.array(inclination_in)
+    pa_in = np.array(pa_in)
+    radius = np.array(radius_in,dtype=float)
+    radkpc = convertskyangle(Configuration,radius)
+    #radkpc = np.array([convertskyangle(Configuration,float(x)) for x in radius],dtype=float)
+    #phi is dependent on theta but the max change should be the same
+    max_shift = np.arctan(np.tan(Configuration['MAX_CHANGE']['INCL']*(np.pi/180.))\
+                    *np.tan(Configuration['MAX_CHANGE']['PA']*(np.pi/180.)))
+    print_log(f'''CHECK_ANGULAR_MOMENTUM_VECTOR: The maximum allowed shift = {max_shift}.
+''',Configuration,case= ['debug_start'])
+    succes = False
+    counter = 0.
+    while not succes:
+        print_log(f'''CHECK_ANGULAR_MOMENTUM_VECTOR: Calculating Phi and Theta from these PA and inclination
+PA = {pa}
+Inclination = {inclination}
+''',Configuration,case= ['debug_add'])
+        Theta,Phi,quadrant = calculate_am_vector(Configuration,pa,inclination )
+        theta_zero = Theta[0]
+        phi_zero = Phi[0]
+
+        #Let's combine the variation as fraction of the existing angle
+        theta_change= np.array([float(x-theta_zero) for x in Theta],dtype=float)
+        phi_change= np.array([float(x-phi_zero) for x in Phi],dtype=float)
+
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore",message="invalid value encountered in true_divide"\
+                                ,category=RuntimeWarning)
+            theta_factor = np.sqrt(theta_change**2/(theta_change**2+phi_change**2))\
+                        *(theta_change)/abs(theta_change)
+            theta_factor[np.where(np.array(theta_change) == 0.)] = 0.
+            phi_factor = np.sqrt(phi_change**2/(theta_change**2+phi_change**2))*(phi_change)/abs(phi_change)
+            phi_factor[np.where(np.array(phi_change) == 0.)] = 0.
+
+        in_zero = np.where(np.array(theta_change+phi_change) == 0.)
+        phi_factor[in_zero]=0.
+        theta_factor[in_zero]=0.
+
+        change_angle = np.sqrt(theta_change**2+phi_change**2)
+        change_angle[in_zero] =0.
+        new_change_angle = max_profile_change(Configuration,radkpc,change_angle,'ARBITRARY',\
+            slope = Configuration['WARP_SLOPE'][side],max_change=max_shift, kpc_radius=True )
+
+
+        new_theta_change = new_change_angle*theta_factor
+        new_phi_change = new_change_angle*phi_factor
+        new_theta = theta_zero+new_theta_change
+        new_phi = phi_zero+new_phi_change
+        print_log(f'''We put in the difference of
+phi {phi_change}, theta {theta_change}, angle {change_angle}
+new values
+phi {new_phi_change}, theta {new_theta_change}, angle {new_change_angle}
+''',Configuration,case= ['debug_add'])
+
+        diff_phi = np.array(np.where(np.array([abs(x-y) for x,y in zip(Phi,new_phi) ],dtype=float) > 1e-6))
+        diff_theta = np.array(np.where(np.array([abs(x-y) for x,y in zip(Theta,new_theta)],dtype=float) > 1e-6))
+
+        if diff_phi.size != 0. or \
+            diff_theta.size != 0.:
+            print_log(f'''CHECK_ANGULAR_MOMENTUM_VECTOR
+{'':8s} Phi = {Phi}, new_phi = {new_phi}
+{'':8s} Phi diff = {np.array([abs(x-y) for x,y in zip(Phi,new_phi) ],dtype=float)}{'':8s}
+{'':8s} Theta = {Theta}, new_theta = {new_theta}
+{'':8s} Theta diff = {np.array([abs(x-y) for x,y in zip(Theta,new_theta) ],dtype=float)}
+''',Configuration,case= ['debug_add'])
+
+
+            pa,inclination = calculate_am_vector(Configuration,new_theta,new_phi,\
+                                multiple=quadrant,invert=True )
+            print_log(f'''CHECK_ANGULAR_MOMENTUM_VECTOR: new PA and inclination
+PA = {pa}
+Inclination = {inclination}
+''',Configuration,case= ['debug_add'])
+            counter += 1
+            if counter > 1000.:
+                #It is not really a succes but we have to exit the loop and one point.
+                succes = True
+        else:
+            succes = True
+
+    print_log(f'''CHECK_ANGULAR_MOMENTUM_VECTOR: Before checking we have modified = {modified}
+''',Configuration,case= ['debug_add'])
+    #if len(np.where(np.array([abs(x-y) for x,y in zip(pa_in,pa) ],dtype=float) != 0.)) != 0. or \
+    #    len(np.where(np.array([abs(x-y) for x,y in zip(inclination_in,inclination) ],dtype=float) != 0.)) != 0.:
+
+    if not np.isclose(pa_in,pa, atol=float(Configuration['MIN_ERROR']['PA'][0])*3.).any() or \
+        not np.isclose(inclination_in,inclination, atol=float(Configuration['MIN_ERROR']['INCL'][0])*3.).any():
+        modified= True
+    return pa,inclination, modified
+check_angular_momentum_vector.__doc__ =f'''
+ NAME:
+    check_angular_momentum_vector
+
+ PURPOSE:
+    Check the output warp by ensuring that the angular momentum is varying smoothly
+
+ CATEGORY:
+    support_functions
+
+ INPUTS:
+    Configuration = Standard Original FAT configuration
+    radius = radius of the model
+    pa = PA of the model
+    inclination = inclination of the model
+
+ OPTIONAL INPUTS:
+    angle_check = False
+    indicates whether we have modified the angles
+
+ OUTPUTS:
+    pa_new = the modfied PA
+    incl_new= the modified incl
+    modified = boolean indicating whether the PA and incl ave beet modfied.
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+
+
+
+def check_sofia(Configuration,Fits_Files):
     files =['_mask.fits','_mom0.fits','_mom1.fits','_chan.fits','_mom2.fits','_cat.txt']
     for file in files:
         if os.path.exists(f'{Configuration["FITTING_DIR"]}Sofia_Output/{Configuration["BASE_NAME"]}{file}'):
             pass
         else:
             raise InputError()
 
@@ -154,40 +482,39 @@
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def check_tiltogram(Configuration, tiltogram,inner_min=3,debug=False):
+def check_tiltogram(Configuration, tiltogram,inner_min=3):
     for i in [0,1]:
         theta_inner = np.array([np.mean(tiltogram[i,0:x+1,0:x+1]) for x in range(tiltogram.shape[1])],dtype=float)
         theta_mutual = np.array([np.mean(tiltogram[i,x:,0:x+1]) for x in range(tiltogram.shape[1])],dtype=float)
         #theta_outer = np.array([np.mean(tiltogram[i,x+1:,x+1:]) for x in range(tiltogram.shape[1])],dtype=float)
         #And then we want to apply the rules
         # (i) the difference between theta_inner and theta_mutual is larger than the differences observed at other radii
         # (ii) theta_inner < 5 deg
         # (iii) thetamut > 15 deg
         diff = np.array(abs(theta_inner-theta_mutual),dtype = float)
-        if debug:
-            print_log(f'''CHECK_TILTOGRAM: Checking the tiltogram in side {i}.
+        print_log(f'''CHECK_TILTOGRAM: Checking the tiltogram in side {i}.
 {'':8s} Diff = {diff}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case= ['debug_start'])
         rings_found = False
         while not rings_found:
             ring_location = np.where(np.nanmax(diff) == diff)[0]
             if ring_location.size > 1:
                 ring_location = ring_location[0]
             if theta_inner[ring_location] < 5. and theta_mutual[ring_location] > 15.:
                 Configuration['INNER_FIX'][i] = int(set_limits(ring_location-1,inner_min,Configuration['NO_RINGS']*3./4.-1))
@@ -209,164 +536,170 @@
    support_functions
 
 INPUTS:
    Configuration = standard FAT Configuration
    tiltogram = the array containing the tiltogram for both sides
 
 OPTIONAL INPUTS:
-   debug = False
+
    inner_min = minimum set of inner rings that should be fixed
 
 OUTPUTS:
    Updates Configuration['INNER_FIX']
 
 OPTIONAL OUTPUTS:
 
 PROCEDURES CALLED:
    Unspecified
 
 NOTE:
 
 '''
 # clean the header
-def clean_header(Configuration,hdr_in,two_dim=False,mask_file=False, debug = False):
+def clean_header(Configuration,hdr_in,two_dim=False,mask_file=False):
     hdr = copy.deepcopy(hdr_in)
-    if debug:
-        print_log(f'''CLEAN_HEADER: Starting to clean the header.
-''',Configuration['OUTPUTLOG'],debug=True)
+    print_log(f'''CLEAN_HEADER: Starting to clean the header.
+''',Configuration,case= ['debug_start'])
     keywords = ['CDELT','CUNIT','CRPIX','CRVAL','CTYPE']
     for key in keywords:
         try:
             del hdr[f'{key}4']
-        except:
+        except KeyError:
             pass
     if not two_dim:
         hdr['NAXIS'] = 3
         if not 'CUNIT3' in hdr:
-            if hdr['CDELT3'] > 500:
+            if abs(hdr['CDELT3']) > 500:
                 hdr['CUNIT3'] = 'm/s'
             else:
                 hdr['CUNIT3'] = 'km/s'
-            print_log(f'''CLEAN_HEADER: Your header did not have a unit for the third axis, that is bad policy.
-    {"":8s} We have set it to {hdr['CUNIT3']}. Please ensure that is correct.'
-    ''',Configuration['OUTPUTLOG'])
+            print_log(f'''CLEAN_HEADER:
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+Your header did not have a unit for the third axis, that is bad policy.
+{"":8s} We have set it to {hdr['CUNIT3']}. Please ensure that is correct.'
+!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!!
+''',Configuration)
         if hdr['CUNIT3'].upper() == 'HZ' or hdr['CTYPE3'].upper() == 'FREQ':
-            print_log('CLEAN_HEADER: FREQUENCY IS NOT A SUPPORTED VELOCITY AXIS.', Configuration['OUTPUTLOG'],screen=True)
+            print_log('CLEAN_HEADER: FREQUENCY IS NOT A SUPPORTED VELOCITY AXIS.', Configuration, case=['main','screen'])
             raise BadHeaderError('The Cube has frequency as a velocity axis this is not supported')
 
         vel_types = ['VELO-HEL','VELO-LSR','VELO', 'VELOCITY']
         if hdr['CTYPE3'].upper() not in vel_types:
             if hdr['CTYPE3'].split('-')[0].upper() in ['RA','DEC']:
                 print_log(f'''CLEAN_HEADER: Your zaxis is a spatial axis not a velocity axis.
-    {"":8s}CLEAN_HEADER: Please arrange your cube logically
-    ''',Configuration['OUTPUTLOG'],screen=True)
+{"":8s}CLEAN_HEADER: Please arrange your cube logically
+''',Configuration,case= ['main','screen'])
                 raise BadHeaderError("The Cube's third axis is not a velocity axis")
             hdr['CTYPE3'] = 'VELO'
             print_log(f'''CLEAN_HEADER: Your velocity projection is not standard. The keyword is changed to VELO (relativistic definition). This might be dangerous.
-    ''',Configuration['OUTPUTLOG'])
+''',Configuration)
 
         if hdr['CUNIT3'].lower() == 'km/s':
             print_log( f'''CLEAN_HEADER: The channels in your input cube are in km/s. This sometimes leads to problems with wcs lib, hence we change it to m/s.'
-    ''',Configuration['OUTPUTLOG'])
+''',Configuration)
             hdr['CUNIT3'] = 'm/s'
             hdr['CDELT3'] = hdr['CDELT3']*1000.
             hdr['CRVAL3'] = hdr['CRVAL3']*1000.
         #because astropy is truly stupid
 
         if hdr['CUNIT3'] == 'M/S':
             hdr['CUNIT3'] = 'm/s'
 
     if not 'EPOCH' in hdr:
         if 'EQUINOX' in hdr:
             print_log(f'''CLEAN_HEADER: Your cube has no EPOCH keyword but we found EQUINOX.
 {"":8s}We have set EPOCH to {hdr['EQUINOX']}
-''',Configuration['OUTPUTLOG'])
+''',Configuration)
             hdr['EPOCH'] = hdr['EQUINOX']
             del hdr['EQUINOX']
         else:
             print_log(f'''CLEAN_HEADER: Your cube has no EPOCH keyword
 {"":8s}CLEAN_HEADER: We assumed J2000
-''',Configuration['OUTPUTLOG'])
+''',Configuration)
             hdr['EPOCH'] = 2000.
 
 
-
+    #FAT cannot deal with the PC nonsense
     if f'PC01_01' in hdr:
         del hdr['PC0*_0*']
+    if f'PC1_1' in hdr:
+        del hdr['PC*_*']
 
 
     # Check for the beam
     if not 'BMAJ' in hdr and not mask_file:
         if 'BMMAJ' in hdr:
             hdr['BMAJ']= hdr['BMMAJ']/3600.
         else:
             found = False
-            for line in hdr['HISTORY']:
-                tmp = [x.strip().upper() for x in line.split()]
-                if 'BMAJ=' in tmp:
-                    hdr['BMAJ'] = tmp[tmp.index('BMAJ=') + 1]
-                    found = True
-                if 'BMIN=' in tmp:
-                    hdr['BMIN'] = tmp[tmp.index('BMIN=') + 1]
-                if 'BPA=' in tmp:
-                    hdr['BPA'] = tmp[tmp.index('BPA=') + 1]
-                if found:
-                    break
+            if 'HISTORY' in hdr:
+                for line in hdr['HISTORY']:
+                    tmp = [x.strip().upper() for x in line.split()]
+                    if 'BMAJ=' in tmp:
+                        hdr['BMAJ'] = tmp[tmp.index('BMAJ=') + 1]
+                        found = True
+                    if 'BMIN=' in tmp:
+                        hdr['BMIN'] = tmp[tmp.index('BMIN=') + 1]
+                    if 'BPA=' in tmp:
+                        hdr['BPA'] = tmp[tmp.index('BPA=') + 1]
+                    if found:
+                        break
             if not found:
                 print_log(f'''CLEAN_HEADER: WE CANNOT FIND THE MAJOR AXIS FWHM IN THE HEADER
-''',Configuration['OUTPUTLOG'],screen=True)
+''',Configuration,case= ['main','screen'])
                 raise BadHeaderError("The Cube has no major axis FWHM in the header.")
     if not 'CTYPE1' in hdr or not 'CTYPE2' in hdr:
         print_log(f'''CLEAN_HEADER: Your spatial axes have no ctype. this can lead to errors.
-''',Configuration['OUTPUTLOG'],screen=True)
+''',Configuration,case= ['main','screen'])
         raise BadHeaderError("The Cube header has no ctypes.")
 
     if hdr['CTYPE1'].split('-')[0].upper() in ['DEC']:
         print_log(f'''CLEAN_HEADER: !!!!!!!!!!Your declination is in the first axis. !!!!!!!!!!!!!!!!!
 {"":8s}CLEAN_HEADER: !!!!!!!!!!         This will not work.          !!!!!!!!!!!!!!!!
-''',Configuration['OUTPUTLOG'],screen = True)
+''',Configuration,case= ['main','screen'])
         raise BadHeaderError("Your spatial axes are reversed")
     if hdr['CTYPE2'].split('-')[0].upper() in ['RA']:
         print_log( f'''CLEAN_HEADER: !!!!!!!!!!Your right ascension is on the second axis. !!!!!!!!!!!!!!!!!
 {"":8s}CLEAN_HEADER: !!!!!!!!!!         This will not work.          !!!!!!!!!!!!!!!!
-''',Configuration['OUTPUTLOG'],screen = True)
+''',Configuration,case= ['main','screen'])
         raise BadHeaderError("Your spatial axes are reversed")
     if hdr['CRVAL1'] < 0.:
         print_log(f'''CLEAN_HEADER: your RA crval is negative, this can lead to errors. Adding 360. deg
-''',Configuration['OUTPUTLOG'])
+''',Configuration)
         hdr['CRVAL1'] = hdr['CRVAL1']+360.
     if not 'BMIN' in hdr and not mask_file:
         if 'BMMIN' in hdr:
             hdr['BMIN']= hdr['BMMIN']/3600.
         else:
             print_log(f'''CLEAN_HEADER: We cannot find the minor axis FWHM. Assuming a circular beam.
-''',Configuration['OUTPUTLOG'])
+''',Configuration)
             hdr['BMIN'] = hdr['BMAJ']
     if not 'BPA' in hdr and not mask_file:
             print_log(f'''CLEAN_HEADER: We cannot find the Beam PA assuming it to be 0
-''',Configuration['OUTPUTLOG'])
+''',Configuration)
             hdr['BPA'] = 0.
 
     try:
         if len(hdr['HISTORY']) > 10:
             del hdr['HISTORY']
-            print_log( f'''CLEAN_HEADER: Your cube has a significant history attached we are removing it for easier interpretation.
-''',Configuration['OUTPUTLOG'])
+            if Configuration:
+                print_log( f'''CLEAN_HEADER: Your cube has a significant history attached we are removing it for easier interpretation.
+''',Configuration)
     except KeyError:
         pass
     try:
         if abs(hdr['BMAJ']/hdr['CDELT1']) < 2:
             print_log( f'''CLEAN_HEADER: !!!!!!!!!!Your cube has less than two pixels per beam major axis.!!!!!!!!!!!!!!!!!
-    {"":8s}CLEAN_HEADER: !!!!!!!!!!           This will lead to bad results.              !!!!!!!!!!!!!!!!'
-    ''',Configuration['OUTPUTLOG'])
+{"":8s}CLEAN_HEADER: !!!!!!!!!!           This will lead to bad results.              !!!!!!!!!!!!!!!!'
+''',Configuration)
 
         if abs(hdr['BMAJ']/hdr['CDELT1']) > hdr['NAXIS1']:
             print_log( f'''CLEAN_HEADER: !!!!!!!!!!Your cube is smaller than the beam major axis. !!!!!!!!!!!!!!!!!
     {"":8s}CLEAN_HEADER: !!!!!!!!!!         This will not work.          !!!!!!!!!!!!!!!!
-    ''',Configuration['OUTPUTLOG'])
+    ''',Configuration,case= ['main','screen'])
             raise BadHeaderError("Your cube is too small for your beam")
     except KeyError:
         pass
     #Make sure the header is WCS compatible
     if not mask_file:
         try:
             with warnings.catch_warnings():
@@ -384,68 +717,66 @@
     Clean up the cube header and make sure it has all the right
     variables that we require in the process of fitting
 
  CATEGORY:
     supprot_functions
 
  INPUTS:
-    Configuration = Standard FAT configuration
+   Configuration = Standard FAT configuration
     hdr = header to be cleaned
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     the updated header
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def columndensity(Configuration,levels,systemic = 100.,beam=[-1.,-1.],channel_width=-1.,column= False,arcsquare=False,solar_mass_input =False,solar_mass_output=False, debug = False):
+def columndensity(Configuration,levels,systemic = 100.,beam=[-1.,-1.],channel_width=-1.,column= False,arcsquare=False,solar_mass_input =False,solar_mass_output=False):
 
     if beam[0] == -1:
         if not arcsquare:
             beam = Configuration['BEAM'][:2]
     if channel_width == -1:
         if arcsquare:
             channel_width = 1.
         else:
             channel_width = Configuration['CHANNEL_WIDTH']
-
-    if debug:
-        print_log(f'''COLUMNDENSITY: Starting conversion from the following input.
+    print_log(f'''COLUMNDENSITY: Starting conversion from the following input.
 {'':8s}Levels = {levels}
 {'':8s}Beam = {beam}
 {'':8s}channel_width = {channel_width}
-''',Configuration['OUTPUTLOG'],debug =True)
+''',Configuration,case= ['debug_start'])
     beam=np.array(beam,dtype=float)
     f0 = 1.420405751786E9 #Hz rest freq
     c = 299792.458 # light speed in km / s
     pc = 3.086e+18 #parsec in cm
     solarmass = 1.98855e30 #Solar mass in kg
     mHI = 1.6737236e-27 #neutral hydrogen mass in kg
-    if debug:
-        print_log(f'''COLUMNDENSITY: We have the following input for calculating the columns.
+    print_log(f'''COLUMNDENSITY: We have the following input for calculating the columns.
 {'':8s}COLUMNDENSITY: level = {levels}, channel_width = {channel_width}, beam = {beam}, systemic = {systemic})
-''',Configuration['OUTPUTLOG'])
-    if systemic > 10000:
-        systemic = systemic/1000.
+''',Configuration,case= ['debug_add'])
+
     f = f0 * (1 - (systemic / c)) #Systemic frequency
     if arcsquare:
+        #Should we have the (f0/f)**2 factor here????
         HIconv = 605.7383 * 1.823E18 * (2. *np.pi / (np.log(256.)))
         if column:
             # If the input is in solarmass we want to convert back to column densities
             if solar_mass_input:
-                levels=levels*solarmass/(mHI*pc**2)
+                levels=np.array([x*solarmass/(mHI*pc**2) for x in levels],dtype=float)
             #levels=levels/(HIconv*channel_width)
+
             levels = levels/(HIconv*channel_width)
         else:
 
             levels = HIconv*levels*channel_width
             if solar_mass_output:
                 levels=levels*mHI/solarmass*pc*pc
     else:
@@ -456,15 +787,15 @@
             if solar_mass_input:
                 levels=levels*solarmass/(mHI*pc**2)
             TK = levels/(1.823e18*channel_width)
             levels = TK/(((605.7383)/(b))*(f0/f)**2)
         else:
             TK=((605.7383)/(b))*(f0/f)**2*levels
             levels = TK*(1.823e18*channel_width)
-    if ~column and solar_mass_input:
+    if not column and solar_mass_input:
         levels = levels*mHI*pc**2/solarmass
     return levels
 
 columndensity.__doc__ =f'''
  NAME:
     columndensity
 
@@ -475,15 +806,15 @@
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     levels = the values to convert
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     systemic = 100.
     the systemic velocity of the source
 
     beam  = [-1.,-1.]
     the FWHM of the beam in arcsec, if unset taken from Configuration
 
@@ -508,24 +839,23 @@
     The converted values
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
- NOTE:
+ NOTE: Cosmological column densities are taken from Meyer et al 2017
 '''
 
         # a Function to convert the RA and DEC into hour angle (invert = False) and vice versa (default)
-def convertRADEC(Configuration,RAin,DECin,invert=False, colon=False,debug = False):
-    if debug:
-        print_log(f'''CONVERTRADEC: Starting conversion from the following input.
+def convertRADEC(Configuration,RAin,DECin,invert=False, colon=False):
+    print_log(f'''CONVERTRADEC: Starting conversion from the following input.
     {'':8s}RA = {RAin}
     {'':8s}DEC = {DECin}
-''',Configuration['OUTPUTLOG'],debug =True)
+''',Configuration,case= ['debug_start'])
     RA = copy.deepcopy(RAin)
     DEC = copy.deepcopy(DECin)
     if not invert:
         try:
             _ = (e for e in RA)
         except TypeError:
             RA= [RA]
@@ -589,15 +919,15 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     RAin = RA to be converted
     DECin = DEC to be converted
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     invert=False
     if true input is hour angle string to be converted to degree
 
     colon=False
     hour angle separotor is : instead of hms
 
@@ -645,20 +975,22 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 # function for converting kpc to arcsec and vice versa
-def convertskyangle(Configuration, angle, distance=1., unit='arcsec', distance_unit='Mpc', physical=False,debug = False):
-    if debug:
-        print_log(f'''CONVERTSKYANGLE: Starting conversion from the following input.
+def convertskyangle(Configuration, angle, distance=-1., unit='arcsec', distance_unit='Mpc', physical=False):
+    if distance == -1.:
+        distance = Configuration['DISTANCE']
+    print_log(f'''CONVERTSKYANGLE: Starting conversion from the following input.
     {'':8s}Angle = {angle}
     {'':8s}Distance = {distance}
-''',Configuration['OUTPUTLOG'],debug =True)
+''',Configuration,case= ['debug_start'])
+
     try:
         _ = (e for e in angle)
     except TypeError:
         angle = [angle]
 
         # if physical is true default unit is kpc
     angle = np.array(angle,dtype=float)
@@ -667,41 +999,44 @@
     if distance_unit.lower() == 'mpc':
         distance = distance * 10 ** 3
     elif distance_unit.lower() == 'kpc':
         distance = distance
     elif distance_unit.lower() == 'pc':
         distance = distance / (10 ** 3)
     else:
-        print_log('CONVERTSKYANGLE: ' + distance_unit + ' is an unknown unit to convertskyangle.\n',Configuration['OUTPUTLOG'],screen=True)
-        print_log('CONVERTSKYANGLE: please use Mpc, kpc or pc.\n',Configuration['OUTPUTLOG'],screen=True)
+        print_log(f'''CONVERTSKYANGLE: {distance_unit} is an unknown unit to convertskyangle.
+{'':8s}CONVERTSKYANGLE: please use Mpc, kpc or pc.
+''',Configuration,case= ['main','screen'])
         raise SupportRunError('CONVERTSKYANGLE: ' + distance_unit + ' is an unknown unit to convertskyangle.')
     if not physical:
         if unit.lower() == 'arcsec':
             radians = (angle / 3600.) * ((2. * np.pi) / 360.)
         elif unit.lower() == 'arcmin':
             radians = (angle / 60.) * ((2. * np.pi) / 360.)
         elif unit.lower() == 'degree':
             radians = angle * ((2. * np.pi) / 360.)
         else:
-            print_log('CONVERTSKYANGLE: ' + unit + ' is an unknown unit to convertskyangle.\n',Configuration['OUTPUTLOG'],screen=True)
-            print_log('CONVERTSKYANGLE: please use arcsec, arcmin or degree.\n',Configuration['OUTPUTLOG'],screen=True)
+            print_log(f'''CONVERTSKYANGLE: {unit} is an unknown unit to convertskyangle.
+{'':8s}CONVERTSKYANGLE: arcsec, arcmin or degree.
+''',Configuration,case= ['main','screen'])
             raise SupportRunError('CONVERTSKYANGLE: ' + unit + ' is an unknown unit to convertskyangle.')
 
 
         kpc = 2. * (distance * np.tan(radians / 2.))
     else:
         if unit.lower() == 'kpc':
             kpc = angle
         elif unit.lower() == 'mpc':
-            kpc = angle / (10 ** 3)
-        elif unit.lower() == 'pc':
             kpc = angle * (10 ** 3)
+        elif unit.lower() == 'pc':
+            kpc = angle / (10 ** 3)
         else:
-            print_log('CONVERTSKYANGLE: ' + unit + ' is an unknown unit to convertskyangle.\n',Configuration['OUTPUTLOG'],screen=True)
-            print_log('CONVERTSKYANGLE: please use kpc, Mpc or pc.\n',Configuration['OUTPUTLOG'],screen=True)
+            print_log(f'''CONVERTSKYANGLE: {unit} is an unknown unit to convertskyangle.
+{'':8s}CONVERTSKYANGLE: please use Mpc, kpc or pc.
+''',Configuration,case= ['main','screen'])
             raise SupportRunError('CONVERTSKYANGLE: ' + unit + ' is an unknown unit to convertskyangle.')
 
         radians = 2. * np.arctan(kpc / (2. * distance))
         kpc = (radians * (360. / (2. * np.pi))) * 3600.
     if len(kpc) == 1:
         kpc = float(kpc[0])
     return kpc
@@ -717,15 +1052,15 @@
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     angle = the angles or lengths to be converted
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     distance=1.
     Distance to the galaxy for the conversion
 
     unit='arcsec'
     Unit of the angle or length options are arcsec (default),arcmin, degree, pc, kpc(default) and Mpc
 
@@ -743,52 +1078,54 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 
-def copy_homemade_sofia(Configuration,no_cat=False,debug=False):
+def copy_homemade_sofia(Configuration,no_cat=False):
     create_directory('Sofia_Output',Configuration['FITTING_DIR'])
     files =['_mask.fits','_mom0.fits','_mom1.fits','_chan.fits','_mom2.fits']
     if not no_cat:
         files.append('_cat.txt')
     for file in files:
         source = get_system_string(f"{Configuration['SOFIA_DIR']}{Configuration['SOFIA_BASENAME']}{file}")
         target = get_system_string(f"{Configuration['FITTING_DIR']}Sofia_Output/{Configuration['BASE_NAME']}{file}")
+        os.system(f'''rm -f {target}''')
         os.system(f'''cp {source} {target}''')
         if not os.path.exists(f"{Configuration['FITTING_DIR']}Sofia_Output/{Configuration['BASE_NAME']+file}"):
             if file in ['_mask.fits','_cat.txt']:
                 print_log(f'''COPY_HOMEMADE_SOFIA: Something went wrong copying the file  {Configuration['SOFIA_DIR']}{Configuration['SOFIA_BASENAME']+file}
 {'':8s} to the file {Configuration['FITTING_DIR']}Sofia_Output/{Configuration['BASE_NAME']+file}.
 {'':8s}We are aborting this fit as we cannot make it without Sofia input.
-''',Configuration['OUTPUTLOG'],screen=True,debug=debug )
+''',Configuration,case= ['main','screen'])
                 raise SofiaMissingError("Either the sofia mask or catalogue is missing. We can not run without it")
             else:
                 pass
+
         elif file != '_cat.txt':
             #make sure the header is decent
             two_dim = True
             mask_file=False
 
             if file == '_mask.fits':
                 two_dim = False
                 mask_file = True
 
             initial = fits.open(f"{Configuration['FITTING_DIR']}Sofia_Output/{Configuration['BASE_NAME']}{file}")
             hdr_in = initial[0].header
             data=initial[0].data
             initial.close()
-            hdr = clean_header(Configuration,hdr_in,two_dim=two_dim,mask_file=mask_file,debug=debug)
+            hdr = clean_header(Configuration,hdr_in,two_dim=two_dim,mask_file=mask_file )
             update = False
             for key in hdr:
                 try:
                     if hdr[key] != hdr_in[key]:
                         update =True
-                except:
+                except KeyError:
                     update = True
             if file == '_mom0.fits':
                 if hdr['BUNIT'].strip().lower() == 'jy/beam*m/s':
                     update = True
                     hdr['BUNIT'] = 'Jy/beam*km/s'
                     data = data/1000.
             if file in ['_mom1.fits','_mom2.fits'] :
@@ -811,29 +1148,29 @@
     clean_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
 
 
  OPTIONAL INPUTS:
-    debug = False
+
     check = False
     if set to true FAT merely checks for the existings of the sofia files where they expect them
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 
-def create_directory(directory,base_directory,debug=False):
+def create_directory(directory,base_directory):
     split_directory = [x for x in directory.split('/') if x]
     split_directory_clean = [x for x in directory.split('/') if x]
     split_base = [x for x in base_directory.split('/') if x]
     #First remove the base from the directory but only if the first directories are the same
     if split_directory[0] == split_base[0]:
         for dirs,dirs2 in zip(split_base,split_directory):
             if dirs == dirs2:
@@ -856,39 +1193,38 @@
     support_functions
 
  INPUTS:
     directory = string with directory to be created
     base_directory = string with directory that exists and from where to start the check from
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
     The requested directory is created but only if it does not yet exist
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def deproject(Configuration,map,angle, center = 0., invert = False,debug=False):
+def deproject(Configuration,map,angle, center = 0., invert = False):
     axis = np.array(range(len(map[:,0])),dtype=float)-center
     if invert:
         newaxis = axis/np.cos(np.radians(angle))
     else:
         newaxis = axis*np.cos(np.radians(angle))
     for x in range(len(map[0,:])):
         profile = copy.deepcopy(map[:,x])
         new_profile = np.interp(np.array(newaxis,dtype=float),np.array(axis,dtype=float),np.array(profile,dtype=float))
         map[:,x] = new_profile
     return map
-
 deproject.__doc__ =f'''
  NAME:
     deproject
 
  PURPOSE:
     Deproject an image assuming circular orienation and an inclination given by the angle
 
@@ -897,15 +1233,15 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     map = the image to deproject
     angle = the inclination angle
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     center = 0.
     height on the yaxis to rotate around
 
     invert = False
     If true the image is inclined by tangle instead of deprojected
 
@@ -916,107 +1252,314 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def finish_current_run(Configuration,current_run,debug=False):
-    print_log(f"FINISH_CURRENT_RUN: Is Tirific Running? {Configuration['TIRIFIC_RUNNING']}. \n",Configuration['OUTPUTLOG'],debug=debug)
+def ensure_list(variable):
+    '''Make sure that variable is a list'''
+    if not isinstance(variable,list):
+        if not isiterable(list1):
+            variable=[variable]
+        else:
+            variable=[x for x in variable]
+    return variable
+ensure_list.__doc__ =f'''
+ NAME:
+    ensure_list
+
+ PURPOSE:
+    Make sure that variable is a list
+
+ CATEGORY:
+    support_functions
+
+ INPUTS:
+    variable = variable to check and transform
+
+ OPTIONAL INPUTS:
+
+ OUTPUTS:
+    variable = variable in list form
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+
+def find_program(name,search):
+    '''check whether a program is available for use.'''
+    found = False
+    while not found:
+        try:
+            run = subprocess.Popen([name], stdout = subprocess.PIPE, stderr = subprocess.PIPE)
+            run.stdout.close()
+            run.stderr.close()
+            os.kill(run.pid, signal.SIGKILL)
+            found = True
+        except FileNotFoundError:
+            name = input(f'''You have indicated to use {name} for using {search} but it cannot be found.
+Please provide the correct name : ''')
+    return name
+find_program.__doc__ =f'''
+ NAME:
+    find_program
+
+ PURPOSE:
+    check whether a program is available for use.
+
+ CATEGORY:
+    support_functions
+
+ INPUTS:
+    name = command name of the program to run
+    search = Program we are looking for
+ OPTIONAL INPUTS:
+
+ OUTPUTS:
+    the correct command for running the program
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+
+def finish_current_run(Configuration,current_run):
+    print_log(f'''FINISH_CURRENT_RUN: Is Tirific Running? {Configuration['TIRIFIC_RUNNING']}.
+''',Configuration)
     if Configuration['TIRIFIC_RUNNING']:
         try:
             current_run.stdout.close()
             current_run.stderr.close()
         except:
+            print_log(f'''FINISH_CURRENT_RUN: We failed to close the pipe to the current run even though there should be one.
+''',Configuration)
             pass
         try:
             os.kill(Configuration['TIRIFIC_PID'], signal.SIGKILL)
-            print_log(f"FINISH_CURRENT_RUN: We killed PID = {Configuration['TIRIFIC_PID']}. \n",Configuration['OUTPUTLOG'])
+            print_log(f'''FINISH_CURRENT_RUN: We killed PID = {Configuration['TIRIFIC_PID']}.
+''',Configuration)
         except:
             try:
                 current_run.kill()
-                print_log(f"FINISH_CURRENT_RUN: We killed the current run although we failed on the PID = {Configuration['TIRIFIC_PID']}. \n",\
-                          Configuration['OUTPUTLOG'])
+                print_log(f'''FINISH_CURRENT_RUN: We killed the current run although we failed on the PID = {Configuration['TIRIFIC_PID']}.
+''',Configuration)
             except AttributeError:
-                print_log(f"FINISH_CURRENT_RUN: We failed to kill the current run with PID {Configuration['TIRIFIC_PID']} even though we have tirific running",Configuration['OUTPUTLOG'],screen=True)
+                print_log(f'''FINISH_CURRENT_RUN: We failed to kill the current run with PID {Configuration['TIRIFIC_PID']} even though we have tirific running
+''',Configuration,case=['main','screen'])
                 raise TirificKillError('FINISH_CURRENT_RUN: Despite having an initialized tirific we could not kill it. This should not happen.')
         Configuration['TIRIFIC_RUNNING'] = False
         Configuration['TIRIFIC_PID'] = 'Not Initialized'
     else:
-        print_log(f"FINISH_CURRENT_RUN: No run is initialized. \n",Configuration['OUTPUTLOG'])
-
+        print_log(f'''FINISH_CURRENT_RUN: No run is initialized.
+''',Configuration)
 finish_current_run.__doc__ =f'''
  NAME:
     finish_current_run
  PURPOSE:
     make sure that the initiated tirific is cleaned when pyFAT stops
  CATEGORY:
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     current_run = subprocess structure for the current tirific run
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     kills tirific if initialized or raises an error when it fails to do so while tirific is running
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def fit_sine(Configuration,x,y,debug = False):
-    if debug:
-        print_log(f'''FIT_SINE: Starting to fit a sin.
+def fit_center_ellipse(Configuration,map,inclination= -1, pa = -1):
+    max = np.max(map)
+    ellipses = np.linspace(max/2.,max,num=10)
+    parameters =[]
+    for el_out,el_in in zip(ellipses,ellipses[1:]):
+        map_to_fit = np.zeros(map.shape)
+        map_to_fit[map < el_in ] = 1.
+        map_to_fit[map < el_out ] = 0.
+        y,x = np.where(map_to_fit == 1.)
+        cx,cy,a,b, orient = fit_ellipse(Configuration,x,y)
+        if np.isnan(cx) or np.isnan(cx):
+            continue
+        else:
+            if a < b:
+                tmp = copy.deepcopy(a)
+                a = copy.deepcopy(b)
+                b = copy.deepcopy(tmp)
+                orient = orient-90.
+
+
+            ratio = float(set_limits(b/a,0.2,1.0))
+            inc = np.degrees(np.arccos(np.sqrt((ratio**2-0.2**2)/0.96)))
+            parameters.append([cx,cy,inc , orient,len(y)])
+
+    x_in = [x[0] for x  in parameters]
+    y_in = [x[1] for x  in parameters]
+    if inclination == -1. or pa == -1.:
+        weight = [x[-1]  for x in parameters ]
+    else:
+        weight = [x[-1]/((abs(x[2]-inclination)+abs(x[3]-inclination)))  for x in parameters ]
+    x_center = np.sum([x*y for x,y in zip(x_in,weight)])/np.sum(weight)
+    y_center = np.sum([x*y for x,y in zip(y_in,weight)])/np.sum(weight)
+
+    return [x_center,y_center]
+fit_center_ellipse.__doc__= '''
+NAME:
+   fit_center_ellipse
+PURPOSE:
+   determine the center through ellipse fits
+
+CATEGORY:
+   support_functions
+
+INPUTS:
+  Configuration = stadard configurstion
+  map = moment 0 map
+  inclination= current inclination
+  pa = current pa
+
+OPTIONAL INPUTS:
+
+
+
+OUTPUTS:
+   center
+   the fitted center in pixels
+
+OPTIONAL OUTPUTS:
+
+PROCEDURES CALLED:
+   Unspecified
+
+NOTE:
+'''
+
+
+def fit_ellipse(Configuration,x,y):
+    x=x[:,None]
+    y=y[:,None]
+    diag = np.hstack([x*x,x*y,y*y,x,y,np.ones(x.shape)])
+    dmult = np.dot(diag.T,diag)
+    constant=np.zeros([6,6])
+    constant[0,2]=constant[2,0]=2
+    constant[1,1]=-1
+    try:
+        eigen,vec=np.linalg.eig(np.dot(np.linalg.inv(dmult),constant))
+    except LinAlgError:
+        return float('NaN'),float('NaN'),float('NaN'),float('NaN'),float('NaN')
+    n= np.argmax(eigen)
+    # if we have more then 3 arguments then we have complex numbers which is pointless for our center
+    if n > 3:
+        return float('NaN'),float('NaN'),float('NaN'),float('NaN'),float('NaN')
+    a=vec[:,n]
+        #-------------------Fit ellipse-------------------
+    b,c,d,f,g,a=a[1]/2., a[2], a[3]/2., a[4]/2., a[5], a[0]
+    bb=b**2
+    num=b**2-a*c
+    new_x=(c*d-b*f)/num
+    new_y=(a*f-b*d)/num
+
+    angle=0.5*np.arctan(2*b/(a-c))*180/np.pi+90.
+    up = 2*(a*f**2+c*d**2+g*bb-2*b*d*f-a*c*g)
+    down1=(bb-a*c)*( (c-a)*np.sqrt(1+4*bb/((a-c)*(a-c)))-(c+a))
+    down2=(bb-a*c)*( (a-c)*np.sqrt(1+4*bb/((a-c)*(a-c)))-(c+a))
+    a=np.sqrt(abs(up/down1))
+    b=np.sqrt(abs(up/down2))
+
+    return new_x,new_y,a,b,angle
+
+fit_ellipse.__doc__= '''
+NAME:
+   fit_ellipse
+PURPOSE:
+   fit ellipse to a bunch of coordinates
+
+CATEGORY:
+   support_functions
+
+INPUTS:
+  Configuration = stadard configurstion
+  x = x -coordinates to evaluated
+  y = y -coordinates to evaluated
+
+OPTIONAL INPUTS:
+
+
+
+OUTPUTS:
+   new_x = new x center
+   new_y = new y center
+   a =  major axis
+   b = minor axis
+   angle= orientaion of ellipse
+
+
+OPTIONAL OUTPUTS:
+
+PROCEDURES CALLED:
+   Unspecified
+
+NOTE:
+'''
+
+def fit_sine(Configuration,x,y):
+    print_log(f'''FIT_SINE: Starting to fit a sin.
 {'':8s}x = {x}
 {'':8s}y = {y}
 {'':8s} x size = {x.size} y size = {y.size}
-''', Configuration['OUTPUTLOG'],debug =True)
+''', Configuration,case=['debug_start'])
     # Make sure we have numpy arrays
     x= np.array(x,dtype=float)
     y= np.array(y,dtype=float)
     est_peak = np.nanmax(y)-np.mean(y)
     peak_location = np.where(y == np.nanmax(y))[0]
     if peak_location.size > 1:
         peak_location = int(peak_location[0])
     min_location =  np.where(y == np.nanmin(y))[0]
     if min_location.size > 1:
         min_location = int(min_location[0])
     est_width = float(abs(x[peak_location]-x[min_location])/(2.*np.pi))
-
-    #print(est_width)
     est_amp = np.mean(y)
     peak_location = np.where(y == np.nanmax(y))[0]
     if peak_location.size > 1:
         peak_location = int(peak_location[0])
 
     est_center = float(x[peak_location])
 
     est_width=est_width*(2.*np.pi/180.)
-    #print(est_peak,est_center,est_width,est_amp)
     with warnings.catch_warnings():
         warnings.simplefilter("error", OptimizeWarning)
         try:
             sin_parameters, sin_covariance = curve_fit(sine, x[~np.isnan(y)], y[~np.isnan(y)],p0=[est_peak,est_center,est_width,est_amp])
         except RuntimeError:
             sin_parameters = [float('NaN') for z in range(4)]
         except OptimizeWarning:
-            if debug:
-                print_log(f'''FIT_SINE: the covariance could not be estimated. Using initial estimates
+            print_log(f'''FIT_SINE: the covariance could not be estimated. Using initial estimates
 {'':8s}peak est = {est_peak}
 {'':8s}center est = {est_center}
 {'':8s}width est = {est_width}
 {'':8s}amp est = {est_amp}
-''', Configuration['OUTPUTLOG'],debug =True)
+''', Configuration,case=['debug_add'])
             sin_parameters = [0.,0.,0.,0.]
 
     if not 0.4 < sin_parameters[2] <0.6:
         ratios = y
         sin_parameters = [est_peak,est_center,est_width,est_amp]
     else:
         ratios = sine(x,*sin_parameters)
@@ -1034,52 +1577,80 @@
 INPUTS:
    x = x-axis of profile
    y = y-axis of profile
    Configuration = Standard FAT configuration
 
 OPTIONAL INPUTS:
 
-   debug = False
+
 
 OUTPUTS:
    ratios
    the fitted sin profile or when the  width is too small or to wide the original profiles
 
 OPTIONAL OUTPUTS:
 
 PROCEDURES CALLED:
    Unspecified
 
 NOTE:
 '''
 
 
-def fit_gaussian(Configuration,x,y, covariance = False,errors = None, debug = False):
-    if debug:
-        print_log(f'''FIT_GAUSSIAN: Starting to fit a Gaussian.
+def fit_gaussian(Configuration,x,y, covariance = False,errors = None):
+    print_log(f'''FIT_GAUSSIAN: Starting to fit a Gaussian.
 {'':8s}x = {x}
 {'':8s}y = {y}
-''', Configuration['OUTPUTLOG'],debug =True)
+''', Configuration,case=['debug_start'])
     # Make sure we have numpy arrays
     x= np.array(x,dtype=float)
     y= np.array(y,dtype=float)
     # First get some initial estimates
     est_peak = np.nanmax(y)
     if not errors.any():
         errors = np.full(len(y),1.)
         absolute_sigma = False
     else:
         absolute_sigma = True
     peak_location = np.where(y == est_peak)[0]
     if peak_location.size > 1:
         peak_location = peak_location[0]
     est_center = float(x[peak_location])
-
     est_sigma = np.nansum(y*(x-est_center)**2)/np.nansum(y)
-    gauss_parameters, gauss_covariance = curve_fit(gaussian_function, x, y,p0=[est_peak,est_center,est_sigma],sigma= errors,absolute_sigma= absolute_sigma)
+
+    with warnings.catch_warnings():
+        warnings.simplefilter("error")
+        succes = False
+        maxfev= int(100*(len(x)))
+
+        while not succes:
+            print_log(f'''FIT_GAUSSIAN: Starting the curve fit with {maxfev}
+''',Configuration,case=['debug_add'])
+            try:
+                gauss_parameters, gauss_covariance = curve_fit(gaussian_function, \
+                        x, y,p0=[est_peak,est_center,est_sigma],sigma= errors,\
+                        absolute_sigma= absolute_sigma,maxfev=maxfev)
+                succes = True
+            except OptimizeWarning:
+                maxfev =  2000*(len(x))
+            except RuntimeError as e:
+                split_error = str(e)
+                if 'Optimal parameters not found: Number of calls to function has reached maxfev' in \
+                    split_error:
+                    maxfev += 100*int(len(x))
+                    print_log(f'''FIT_GAUSSIAN: We failed to find an optimal fit due to the maximum number of evaluations. increasing maxfev to {maxfev}
+''',Configuration,case=['debug_add'])
+                else:
+                    print_log(f'''FIT_GAUSSIAN: failed due to the following error {split_error}
+''',Configuration,case=['main','screen'])
+                    raise RuntimeError(split_error)
+            if maxfev >  1000*(len(x)):
+                raise FittingError("FIT_GAUSSIAN: failed to find decent gaussian parameters")
+
+    #gauss_parameters, gauss_covariance = curve_fit(gaussian_function, x, y,p0=[est_peak,est_center,est_sigma],sigma= errors,absolute_sigma= absolute_sigma)
     if covariance:
         return gauss_parameters, gauss_covariance
     else:
         return gauss_parameters
 
 fit_gaussian.__doc__ =f'''
  NAME:
@@ -1094,15 +1665,15 @@
     y = y-axis of profile
     Configuration = Standard FAT configuration
 
  OPTIONAL INPUTS:
     covariance = false
     return to covariance matrix of the fit or not
 
-    debug = False
+
 
  OUTPUTS:
     gauss_parameters
     the parameters describing the fitted Gaussian
 
  OPTIONAL OUTPUTS:
     gauss_covariance
@@ -1144,41 +1715,40 @@
  PROCEDURES CALLED:
     Unspecified
 
  EXAMPLE:
 
  NOTE:
 '''
-def get_fit_groups(Configuration,Tirific_Template,debug = False):
+
+def get_fit_groups(Configuration,Tirific_Template):
     parameter_groups = []
     block = []
     rings = []
     groups = Tirific_Template['VARY'].split(',')
     variation_type = []
     variation = []
-    radii,cut_off_limits = sbr_limits(Configuration, systemic= float(Tirific_Template['VSYS'].split(' ')[0]) , debug = debug)
+    radii,cut_off_limits = sbr_limits(Configuration,Tirific_Template )
     sbr_standard = np.mean(cut_off_limits) * 5.
     paramater_standard_variation = {'PA': [10.,'a'],
                                    'INCL': [10.,'a'],
                                    'VROT': [Configuration['CHANNEL_WIDTH']*3.,'a'],
                                    'VSYS': [Configuration['CHANNEL_WIDTH'],'a'],
                                    'XPOS': [Configuration['BEAM'][0]/3600.,'a'],
                                    'YPOS': [Configuration['BEAM'][0]/3600.,'a'],
                                    'SBR': [sbr_standard,'a'],
                                    'Z0': [Configuration['BEAM'][0]*2.,'a'],
                                    'SDIS': [Configuration['CHANNEL_WIDTH']*1.5,'a'],
                                    }
-    if debug:
-        print_log(f'''GET_FIT_GROUPS: We have found the following unformatted groups from VARY:
+    print_log(f'''GET_FIT_GROUPS: We have found the following unformatted groups from VARY:
 {'':8s}{groups}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
     for group in groups:
-        if debug:
-            print_log(f'''GET_FIT_GROUPS: We are processing {group}
-''',Configuration['OUTPUTLOG'])
+        print_log(f'''GET_FIT_GROUPS: We are processing {group}
+''',Configuration,case=['debug_add'])
         parts = group.split()
         if parts[0][0] == '!':
             block.append(False)
             parts[0] = parts[0][1:]
         else:
             block.append(True)
         found_rings = []
@@ -1205,43 +1775,42 @@
         if len(found_rings) == 1:
             block[-1] = False
         parameter_groups.append(preliminary_group)
         rings.append(found_rings)
         block_str = 'as a block.'
         if not block[-1]:
             block_str = 'individually.'
-        if debug:
-            print_log(f'''GET_FIT_GROUPS: We determined the group {parameter_groups[-1]}
+        print_log(f'''GET_FIT_GROUPS: We determined the group {parameter_groups[-1]}
 {'':8s}with rings {rings[-1]}
 {'':8s} which are varied {block_str}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
         # Then get current errors that are present
         per_par_variation  = []
         current_par = ''
         for par in parameter_groups[-1]:
             if current_par == '':
                 current_par = par
                 if current_par[-1] == '2':
                     current_par=current_par[:-2]
             par = [f'# {par}_ERR']
-            all_errors = np.array(get_from_template(Configuration,Tirific_Template, par,debug=debug)[0],dtype=float)
+            all_errors = load_tirific(Configuration,Tirific_Template, par,\
+                array=True )
             current_rings = np.array(rings[-1],dtype=int)-1
             if current_rings.size == 1:
                 current_rings = int(current_rings)
             if len(all_errors) ==0. and current_par != 'SBR':
                 if block[-1]:
                     per_par_variation.append(paramater_standard_variation[current_par][0]/3.)
                 else:
                     per_par_variation.append(paramater_standard_variation[current_par][0])
             elif current_par == 'SBR':
-                if debug:
-                    print_log(f'''GET_FIT_GROUPS: For SBR we are setting
+                print_log(f'''GET_FIT_GROUPS: For SBR we are setting
 {'':8s}the cut_off_limits {cut_off_limits}
 {'':8s} in ring {current_rings}  == {cut_off_limits[current_rings]}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
                 if block[-1]:
                     per_par_variation.append(np.mean(cut_off_limits[current_rings])*3.)
                 else:
                     per_par_variation.append(np.max(cut_off_limits[current_rings])*3.)
             else:
 
                 if block[-1]:
@@ -1285,149 +1854,74 @@
     Unspecified
 
  EXAMPLE:
 
  NOTE:
 '''
 
-def get_from_template(Configuration,Tirific_Template,Variables, debug = False):
-    out = []
-    if debug:
-        print_log(f'''GET_FROM_TEMPLATE: Trying to get the following profiles {Variables}
-''',Configuration['OUTPUTLOG'] ,debug= True)
-    for key in Variables:
-        try:
-            out.append([float(x) for x  in Tirific_Template[key].split()])
-        except KeyError:
-            out.append([])
-    #Because lists are stupid i.e. sbr[0][0] = SBR[0], sbr[1][0] = SBR_2[0] but  sbr[:][0] = SBR[:] not SBR[0],SBR_2[0] as logic would demand
-    if debug:
-        print_log(f'''GET_FROM_TEMPLATE: We extracted the following profiles from the Template.
-{'':8s}GET_FROM_TEMPLATE: {out}
-''',Configuration['OUTPUTLOG'])
-    #Beware that lists are stupid i.e. sbr[0][0] = SBR[0], sbr[1][0] = SBR_2[0] but  sbr[:][0] = SBR[:] not SBR[0],SBR_2[0] as logic would demand
-    # However if you make a np. array from it make sure that you specify float  or have lists of the same length else you get an array of lists which behave just as dumb
-    return out
-
-get_from_template.__doc__ =f'''
- NAME:
-    get_from_template
- PURPOSE:
-    Return a specified list of prameters from the template. This puts the template values in a list !!!!!!!!
-
- CATEGORY:
-    support_functions
-
- INPUTS:
-    Configuration = Standard FAT configuration
-    Tirific_Template =  Standard tirific template
-    Variables = parameters to be extracted
-
- OPTIONAL INPUTS:
-    debug = False
-
- OUTPUTS:
-    list with the values of the requested variables
-
- OPTIONAL OUTPUTS:
-
- PROCEDURES CALLED:
-    Unspecified
-
- NOTE:
-    This is very similar to load_template in read_functions but this returns an
-    unchecked list whereas load_template return a np array with length NUR,
-    the latter can thus can include zeros
-'''
-
-def get_inclination_pa(Configuration, Image, center, cutoff = 0., debug = False,figure_name = 'test'):
+def get_inclination_pa(Configuration, Image, center, cutoff = 0.,figure_name = 'test'):
     map = copy.deepcopy(Image[0].data)
     for i in [0,1]:
-        if debug:
-            print_log(f'''GET_INCLINATION_PA: Doing iteration {i} in the estimates
-''',Configuration['OUTPUTLOG'])
+        print_log(f'''GET_INCLINATION_PA: Doing iteration {i} in the estimates
+''',Configuration,case=['debug_start'])
         # now we need to get profiles under many angles let's say 100
         #extract the profiles under a set of angles
         angles = np.linspace(0, 360, 180)
-        ratios, maj_extent = obtain_ratios(Configuration,map, center, angles,noise = cutoff,debug=debug)
+        ratios, maj_extent = obtain_ratios(Configuration,map, center, angles,noise = cutoff)
         if np.any(np.isnan(ratios)):
             return [float('NaN'),float('NaN')],  [float('NaN'),float('NaN')],float('NaN')
-        sin_ratios,sin_parameters = fit_sine(Configuration,angles,ratios,debug=debug)
+        sin_ratios,sin_parameters = fit_sine(Configuration,angles,ratios)
         if np.any(np.isnan(sin_parameters)):
             return [float('NaN'),float('NaN')],  [float('NaN'),float('NaN')],float('NaN')
-
-
-
-        #matplotlib.use('MacOSX')
-        #if debug:
-        #    name= f'{figure_name}_{i}.pdf'
-        #    fig = plt.figure()
-        #    plt.plot(angles,ratios)
-        #    plt.plot(angles,sin_ratios,'k--')
-        #    plt.savefig(name, bbox_inches='tight')
-        #    plt.close()
-
         ratios=sin_ratios
-        if debug:
-            if i == 0:
-                print_log(f'''GET_INCLINATION_PA: We initially find radius of {maj_extent*3600./(Configuration['BEAM'][0])} beams.
-''',Configuration['OUTPUTLOG'], debug = True)
-                print_log(f'''GET_INCLINATION_PA: We initially find the ratios:
-{'':8s} ratios = {ratios}
-''',Configuration['OUTPUTLOG'])
-            else:
-                print_log(f'''GET_INCLINATION_PA: From the cleaned map we find radius of {maj_extent*3600./Configuration['BEAM'][0]} beams.
-''',Configuration['OUTPUTLOG'])
-                print_log(f'''GET_INCLINATION_PA: We  find these ratios from the cleaned map:
-{'':8s} ratios = {ratios}
-''',Configuration['OUTPUTLOG'])
+
         max_index = np.where(ratios == np.nanmax(ratios))[0]
         if max_index.size > 1:
             max_index =int(max_index[0])
         min_index = np.where(ratios == np.nanmin(ratios))[0]
+
         if min_index.size > 1:
             min_index =int(min_index[0])
         max_index = set_limits(max_index,2,177)
         min_index = set_limits(min_index,2,177)
-        if debug:
-            if i == 0:
-                print_log(f'''GET_INCLINATION_PA: We initially find these indeces min {min_index } {angles[min_index]} max {max_index} {angles[max_index]}.
-''',Configuration['OUTPUTLOG'])
-            else:
-                print_log(f'''GET_INCLINATION_PA: From the cleaned map we find these indeces min {min_index }  {angles[min_index]} max {max_index} {angles[max_index]}.
-''',Configuration['OUTPUTLOG'])
+
+        if min_index > 135 and max_index < 45:
+            min_index=min_index-90
+        if max_index > 135 and min_index < 45:
+            max_index=max_index-90
+        if i == 0:
+            print_log(f'''GET_INCLINATION_PA: We initially find these indeces min {min_index } {angles[min_index]} max {max_index} {angles[max_index]}.
+''',Configuration,case=['debug_add'])
+        else:
+            print_log(f'''GET_INCLINATION_PA: From the cleaned map we find these indeces min {min_index }  {angles[min_index]} max {max_index} {angles[max_index]}.
+''',Configuration,case=['debug_add'])
         #get a 10% bracket
 
         tenp_max_index = np.where(ratios > np.nanmax(ratios)*0.9)[0]
         tenp_min_index = np.where(ratios < np.nanmin(ratios)*1.1)[0]
 
         if tenp_max_index.size <= 1 and 2 <= max_index <=177 :
             tenp_max_index= [max_index-2,max_index+2]
 
         if tenp_min_index.size <= 1:
             tenp_min_index= [min_index-2,min_index+2]
-        if angles[min_index]-90 > 0.:
-            if angles[max_index] > 165:
-                pa = float(np.nanmean(np.array([angles[min_index]+90,angles[max_index]],dtype=float)))
-            else:
-                pa = float(np.nanmean(np.array([angles[min_index]-90,angles[max_index]],dtype=float)))
+
+        if angles[min_index] > angles[max_index]:
+            pa = float(np.nanmean(np.array([angles[min_index]-90,angles[max_index]],dtype=float)))
         else:
-            if angles[max_index] < 15:
-                pa = float(np.nanmean(np.array([angles[min_index]-90,angles[max_index]],dtype=float)))
-            else:
-                pa = float(np.nanmean(np.array([angles[min_index]+90,angles[max_index]],dtype=float)))
+            pa = float(np.nanmean(np.array([angles[min_index]+90,angles[max_index]],dtype=float)))
         if 180. < pa:
             pa = pa -180
-        if debug:
-            if i == 0:
-                print_log(f'''GET_INCLINATION_PA: The initial final pa = {pa}.
-''',Configuration['OUTPUTLOG'])
-            else:
-                print_log(f'''GET_INCLINATION_PA: The pa from the cleaned map  = {pa}.
-''',Configuration['OUTPUTLOG'])
+
+        if i == 0:
+            print_log(f'''GET_INCLINATION_PA: The initial  pa = {pa}.
+''',Configuration,case=['debug_add'])
+        else:
+            print_log(f'''GET_INCLINATION_PA: The pa from the cleaned map  = {pa}.
+''',Configuration,case=['debug_add'])
         pa_error = set_limits(np.nanmean([abs(float(angles[int(tenp_min_index[0])])-float(angles[min_index])),\
                             abs(float(angles[int(tenp_min_index[-1])])-float(angles[min_index])),\
                             abs(float(angles[int(tenp_max_index[0])])-float(angles[max_index])), \
                             abs(float(angles[int(tenp_min_index[-1])])-float(angles[max_index]))]), \
                             0.5,15.)
         ratios[ratios < 0.204] = 0.204
         ratios[1./ratios < 0.204] = 1./0.204
@@ -1452,24 +1946,24 @@
             inclination = float(inclination-(inclination*0.01/(ratios[max_index]-ratios[min_index])))
             if i == 0:
                 inclination_error = float(inclination_error*0.4/(ratios[max_index]-ratios[min_index]))
         if maj_extent*3600./Configuration['BEAM'][0] < 4:
             inclination = float(inclination+(inclination/10.*np.sqrt(4./(maj_extent/Configuration['BEAM'][0]*3600.))))
             if i == 0:
                 inclination_error = float(inclination_error*4./(maj_extent*3600./Configuration['BEAM'][0]))
-        if debug:
-            if i == 0:
-                print_log(f'''GET_INCLINATION_PA: The initial inclination = {inclination}.
-''',Configuration['OUTPUTLOG'])
-            else:
-                print_log(f'''GET_INCLINATION_PA: From the cleaned map we find inclination = {inclination}.
-''',Configuration['OUTPUTLOG'])
+
+        if i == 0:
+            print_log(f'''GET_INCLINATION_PA: The initial inclination = {inclination}.
+''',Configuration,case=['debug_add'])
+        else:
+            print_log(f'''GET_INCLINATION_PA: From the cleaned map we find inclination = {inclination}.
+''',Configuration,case=['debug_add'])
         # this leads to trouble for small sources due to uncertain PA and inclination estimates
         if inclination < 70. and maj_extent*3600./Configuration['BEAM'][0] > 4:
-            Image_clean = remove_inhomogeneities(Configuration,Image,inclination=inclination, pa = pa,iteration=i, center = center,WCS_center = False, debug=debug)
+            Image_clean = remove_inhomogeneities(Configuration,Image,inclination=inclination, pa = pa,iteration=i, center = center,WCS_center = False )
             map = Image_clean[0].data
             Image_clean.close()
         else:
             break
     inclination_error = inclination_error/np.sin(np.radians(inclination))
     return [inclination,inclination_error], [pa,pa_error],maj_extent
 
@@ -1484,15 +1978,15 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     Image = the intensity map to be evaluated, this should be an astropy structure
     center = center of the galaxy in pixels
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     cutoff = 0.
     Limit to trust the map to, below this values are not evaluated
 
  OUTPUTS:
     inclination,inclination_error = inclination and error
     pa,pa_error =  pa and errror
@@ -1502,29 +1996,18 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def get_new_center(Configuration, map_in, center, maj_extent, noise= 0., debug = False):
+def get_new_center(Configuration, map_in, inclination=-1,pa=-1, noise= 0.):
+
+    new_center = fit_center_ellipse(Configuration,map_in,inclination=inclination,pa=pa )
 
-    map = copy.deepcopy(map_in)
-    map[map < noise]= 0.
-    size_in_beam = set_limits(2*maj_extent/(Configuration['BEAM'][0]/3600.),1.0,Configuration['MAX_SIZE_IN_BEAMS'])
-    if size_in_beam > 8.:
-        sigma = [Configuration['BEAM_IN_PIXELS'][1]*size_in_beam/8.,Configuration['BEAM_IN_PIXELS'][0]*size_in_beam/8.]
-        map = ndimage.gaussian_filter(map, sigma=(sigma[1], sigma[0]), order=0)
-    map[map < np.max(map)/2.] = 0.
-    x =  range(0,len(map[0,:]))
-    y =  range(0,len(map[:,0]))
-    M10 = np.sum((x-center[0])*np.sum(map,axis=0))
-    M01 = np.sum((y-center[1])*np.sum(map,axis=1))
-    M00=np.sum(map)
-    new_center=[center[0]+M10/M00, center[1]+M01/M00]
 
     return new_center,True,False
 
 
 get_new_center.__doc__ =f'''
  NAME:
     get_new-center
@@ -1532,94 +2015,52 @@
     Get the best fitting center for the galaxy.
 
  CATEGORY:
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
-    map = the intensity map to be evaluated, this should be an astropy structure
-    center = center of the galaxy in pixels
+    map_in = the intensity map to be evaluated, this should be an astropy structure
+    inclination = the current inclination for weighing purposes
+    pa =  the current inclination for weighing purposes
 
  OPTIONAL INPUTS:
-    debug = False
 
-    noise = 0.
-    Limit to trust the map to, below this values are not evaluated
+
 
  OUTPUTS:
     center = the newly determined center
     center_stable = whether the center has shifted or now.
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 
-def find_program(name,search):
-    found = False
-    while not found:
-        try:
-            run = subprocess.Popen([name], stdout = subprocess.PIPE, stderr = subprocess.PIPE)
-            run.stdout.close()
-            run.stderr.close()
-            os.kill(run.pid, signal.SIGKILL)
-            found = True
-        except:
-            name = input(f'''You have indicated to use {name} for using {search} but it cannot be found.
-Please provide the correct name : ''')
-    return name
-
-find_program.__doc__ =f'''
- NAME:
-    find_program
-
- PURPOSE:
-    check whether a program is available for use.
-
- CATEGORY:
-    support_functions
-
- INPUTS:
-    name = command name of the program to run
-    search = Program we are looking for
- OPTIONAL INPUTS:
-
- OUTPUTS:
-    the correct command for running the program
-
- OPTIONAL OUTPUTS:
-
- PROCEDURES CALLED:
-    Unspecified
-
- NOTE:
-'''
-
 # Function to get the amount of inner rings to fix
-def get_inner_fix(Configuration,Tirific_Template, debug =False):
-    if debug:
-        print_log(f'''GET_INNER_FIX: Attempting to get the inner rings to be fixed.
-''',Configuration['OUTPUTLOG'], debug = True)
+def get_inner_fix(Configuration,Tirific_Template ):
+    print_log(f'''GET_INNER_FIX: Attempting to get the inner rings to be fixed.
+''',Configuration,case=['debug_start'])
     sbr_av = np.array([(float(x)+float(y))/2. for x,y  in zip(Tirific_Template['SBR'].split(),Tirific_Template['SBR_2'].split())],dtype = float)
-    column_levels = columndensity(Configuration,sbr_av, arcsquare = True, debug = debug)
+    column_levels = columndensity(Configuration,sbr_av, arcsquare = True )
     column_levels[0]= 1e21
     tmp = np.where(column_levels > 1e20)[0]
     if Configuration['OUTER_RINGS_DOUBLED']:
         inner_min =set_limits(Configuration['NO_RINGS']/3.,5.,11)
     else:
         inner_min =set_limits(Configuration['NO_RINGS']/5.,4.,Configuration['NO_RINGS']*0.7)
     inner_min = int(set_limits(np.floor(tmp[-1]/1.5-1), inner_min, Configuration['NO_RINGS']*0.9))
 
 
-    tiltogram = make_tiltogram(Configuration,Tirific_Template,debug=debug)
-    check_tiltogram(Configuration,tiltogram,inner_min=inner_min,debug=debug)
+    tiltogram = make_tiltogram(Configuration,Tirific_Template )
+    check_tiltogram(Configuration,tiltogram,inner_min=inner_min )
 get_inner_fix.__doc__ =f'''
  NAME:
     get_inner_fix
 
  PURPOSE:
     Obtain the number of rings that should be fixed to a single value in the inner parts
     All ring > 1e20 column density should be fixed upt to a maximum of 90% and a minimu of 4 rings.
@@ -1628,46 +2069,46 @@
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = Standard Tirific template containing the SBR profiles
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     Update INNER_FIX in the configuration
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
     !!!!!!!!!!!!!This appears to currently not be working well.
 '''
 
-def get_kinematical_center(Configuration,map,angle,center= [0.,0],debug=False ):
+def get_kinematical_center(Configuration,map,angle,center= [0.,0] ):
     if np.sum(center) == 0.:
         center = [len(map[0,:])/2.,len(map[:,0])/2.]
     if angle > 180.:
         angle= angle-180.
 
     if angle < 90:
         angle = angle+90.
     else:
         angle= angle-90.
     buffer = int(round(np.mean(Configuration['BEAM_IN_PIXELS'][:2])/3.))
-    min_axis_prof, min_axis, min_res = get_profile(Configuration,map,angle,center= center,debug=debug)
+    min_axis_prof, min_axis, min_res = get_profile(Configuration,map,angle,center= center )
     found_vsys = [np.nanmean(min_axis_prof),0,0]
     found_diff=  abs(np.nanmin(min_axis_prof)-np.nanmax(min_axis_prof))+ np.nansum([abs(x-found_vsys[0]) for x in min_axis_prof])
     for x in range(-buffer,buffer):
         for y in range(-buffer,buffer):
                 var_center = [int(round(center[0]+x)),int(round(center[1]+y))]
-                min_axis_prof, min_axis, min_res = get_profile(Configuration,map,angle,center= var_center,debug=debug)
+                min_axis_prof, min_axis, min_res = get_profile(Configuration,map,angle,center= var_center )
                 var_diff=  abs(np.nanmin(min_axis_prof)-np.nanmax(min_axis_prof))+np.nansum([abs(x-np.nanmean(min_axis_prof)) for x in min_axis_prof])
                 if var_diff < found_diff:
                     found_diff = copy.deepcopy(var_diff)
                     found_vsys = [np.nanmean(min_axis_prof),x,y]
     return found_vsys
 
 get_kinematical_center.__doc__=f'''
@@ -1682,15 +2123,15 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     map = the 2D array with the map
     angle = the angle of the major axis, with error
 
  OPTIONAL INPUTS:
-    debug = False
+
     center= [0.,0.]
     default is the cenetr of the map given in pixels
 
  OUTPUTS:
     profile, the corresponding axis in pixel size, resolution of a step on the axis
 
  OPTIONAL OUTPUTS:
@@ -1699,18 +2140,18 @@
     Unspecified
 
  NOTE:
 '''
 
 
 
-def get_profile(Configuration,map,angle,center= [0.,0.],debug=False):
+def get_profile(Configuration,map,angle,center= [0.,0.]):
     if np.sum(center) == 0.:
         center = [len(map[0,:])/2.,len(map[:,0])/2.]
-    x1,x2,y1,y2 = obtain_border_pix(Configuration,angle,center,debug=debug)
+    x1,x2,y1,y2 = obtain_border_pix(Configuration,angle,center )
     linex,liney = np.linspace(x1,x2,1000), np.linspace(y1,y2,1000)
     resolution = np.sqrt((x2-x1)**2+(y2-y1)**2)/1000.
     #maj_resolution = abs((abs(x2-x1)/1000.)*np.sin(np.radians(pa[0])))+abs(abs(y2-y1)/1000.*np.cos(np.radians(pa[0])))
     profile = ndimage.map_coordinates(map, np.vstack((liney,linex)),order=1)
     axis =  np.linspace(0,1000*resolution,1000)- (abs((abs(center[0]))*np.sin(np.radians(angle)))+abs(abs(center[1])*np.cos(np.radians(angle))))
     return profile,axis,resolution
 get_profile.__doc__=f'''
@@ -1725,47 +2166,50 @@
 
  INPUTS:
     Configuration = Standard FAT configuration
     map = the 2D array with the map
     pa = the angle
 
  OPTIONAL INPUTS:
-    debug = False
+
     center= [0.,0.]
     default is the cenetr of the map given in pixels
 
  OUTPUTS:
     profile, the corresponding axis in pixel size, resolution of a step on the axis
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def get_ring_weights(Configuration,Tirific_Template,debug = False):
-    if debug:
-        print_log(f'''GET_RING_WEIGTHS: Getting the importance of the rings in terms of SBR.
-''',Configuration['OUTPUTLOG'], debug = True)
-    sbr = np.array(get_from_template(Configuration,Tirific_Template, ["SBR",f"SBR_2"]),dtype=float)
-    systemic = np.array(get_from_template(Configuration,Tirific_Template, ["VSYS"]),dtype=float)
-    systemic = systemic[0,0]
-    radii,cut_off_limits = sbr_limits(Configuration, systemic= systemic , debug = debug)
+def get_ring_weights(Configuration,Tirific_Template):
+    print_log(f'''GET_RING_WEIGTHS: Getting the importance of the rings in terms of SBR.
+''',Configuration,case=['debug_start'])
+    sbr = load_tirific(Configuration,Tirific_Template,Variables=["SBR",f"SBR_2"],\
+                array=True )
+    print_log(f'''GET_RING_WEIGTHS: retrieve this sbr.
+{'':8s} sbr = {sbr}
+''',Configuration,case=['debug_add'])
+    radii,cut_off_limits = sbr_limits(Configuration,Tirific_Template )
+    print_log(f'''GET_RING_WEIGTHS: retrieved these cut_off_limits.
+{'':8s} col = {cut_off_limits}
+''',Configuration,case=['debug_add'])
     weights= [[],[]]
     for i in [0,1]:
         weights[i] = [set_limits(x/y,0.1,10.) for x,y in zip(sbr[i],cut_off_limits)]
         weights[i] = weights[i]/np.nanmax(weights[i])
         weights[i][0:2] = np.nanmin(weights[i])
         weights[i] = [set_limits(x,0.1,1.) for x in weights[i]]
-    if debug:
-        print_log(f'''GET_RING_WEIGTHS: Obtained the following weights.
+    print_log(f'''GET_RING_WEIGTHS: Obtained the following weights.
 {'':8s}{weights}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
     return np.array(weights,dtype = float)
 
 get_ring_weights.__doc__=f'''
  NAME:
     get_ring_weights
 
  PURPOSE:
@@ -1775,15 +2219,15 @@
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = Standard Tirific template containg the SBR profiles
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     numpy array with the weight normalized to the the maximum.
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
@@ -1791,88 +2235,125 @@
 
  NOTE:
     Weight 1 is most important, weight 0. least important.
     Errors should be divided by these weights to reflect the importance
 '''
 
 def get_system_string(string):
+    '''Escape any spaces in string with backlash'''
     if len(string.split()) > 1:
         string = "\ ".join(string.split())
     return string
+get_system_string.__doc__=f'''
+ NAME:
+    get_system_string
 
-def get_usage_statistics(Configuration,process, debug = False):
+ PURPOSE:
+    Escape any spaces in string with backlash
+
+ CATEGORY:
+    support_functions
+
+ INPUTS:
+    string = is input string with spaces
+
+ OPTIONAL INPUTS:
+
+
+ OUTPUTS:
+    string = string with escaped spaces
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+def get_tirific_output_names(Configuration,work_dir,deffile):
+    print_log(f'''GET_TIRIFIC_OUTPUT_NAMES: Starting the extraction of the output names in {deffile} tot be ran in {work_dir})
+''',Configuration,case=['debug_start'])
+
+    fitsfile,deffile = load_tirific(Configuration,f'{work_dir}/{deffile}' ,\
+        Variables=['OUTSET','TIRDEF'])
+    output_fits = f'{work_dir}/{fitsfile[0]}'
+    output_deffile = f'{work_dir}/{deffile[0]}'
+    return output_fits,output_deffile
+get_tirific_output_names.__doc__=f'''
+ NAME:
+    get_tirific_output_names
+
+ PURPOSE:
+    get the  name of the output fits file and def file as defined in the running directory + deffile
+
+ CATEGORY:
+    support_functions
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    work_dir = The directory where the def file is ran as tirific input can be relative
+    deffile = the tirific input deffile
+
+
+ OPTIONAL INPUTS:
+
+
+ OUTPUTS:
+    output_fits = the full output name
+    output_deffile = the full output def file name
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+
+def get_usage_statistics(Configuration,process):
     #try:
     memory_in_mb = (process.memory_info()[0])/2**20. #psutilreturns bytes
     cpu_percent = process.cpu_percent(interval=1)
     #except:
     #    cpu_percent= 0.
     #    memory_in_mb=0.
     return cpu_percent,memory_in_mb
 
-def get_usage_statistics_old(Configuration,process_id, debug = False):
-    result = subprocess.check_output(['top',f'-p {process_id}','-d 1','-n 1'])
-    #result = subprocess.check_output(['ps','u'])
-    lines = result.decode('utf8').split('\n')
-    column_names = [x.upper() for x in lines[6].strip().split()]
-    if debug:
-        print_log(f'''{'':8s}GET_usage_statistics: We extracted the following column names {column_names}
-''',Configuration['OUTPUTLOG'],debug=True)
-    CPU = float(0.)
-    mem=float(0.)
-    column_var = [x for x in lines[7].strip().split()]
-    if debug:
-        print_log(f'''{'':8s}GET_usage_statistics: We extracted the following variables {column_var}
-''',Configuration['OUTPUTLOG'])
-    try:
-        if int(column_var[column_names.index('PID')]) == int(process_id):
-            CPU = float(column_var[column_names.index('%CPU')])
-            mem = float(column_var[column_names.index('RES')])/1024**2
-    except:
-        #if the PID is not numeric it got merged with the crap in shiftcentercounter
-        try:
-            if column_var[column_names.index('COMMAND')-1] == 'tirific':
-                CPU = float(column_var[column_names.index('%CPU')-1])
-                mem = float(column_var[column_names.index('RES')-1])/1024**2
-        except:
-            pass
-    return CPU,mem
-
 get_usage_statistics.__doc__ =f'''
  NAME:
     get_usage_statistics
  PURPOSE:
     use psutil to get the current CPU and memory usage of tirific
 
  CATEGORY:
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     process_id = process id of the tirific currently running.
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     CPU = The current CPU usage
     mem = current memory usage in Mb
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
     pyFAT version < 1.0.0 uses top which only works on unix and has an error in the MB calculation
 '''
 
-def get_vel_pa(Configuration,velocity_field,center= [0.,0.], debug =False):
-    if debug:
-        print_log(f'''GET_VEL_PA: This is the center we use {center}
-''',Configuration['OUTPUTLOG'],debug = True)
+def get_vel_pa(Configuration,velocity_field,center= [0.,0.] ):
+    print_log(f'''GET_VEL_PA: This is the center we use {center}
+''',Configuration,case=['debug_start'])
     # because python is stupid the ceneter should be reversed to match the map
     center.reverse()
     if np.sum(center) == 0.:
         center = [x/2. for x in velocity_field.shape]
 
     sigma = [3.,3.]
     sm_velocity_field = ndimage.gaussian_filter(velocity_field, sigma=(sigma[1], sigma[0]), order=0)
@@ -1885,17 +2366,16 @@
     max_pos = np.where(np.nanmax(sm_velocity_field) == sm_velocity_field)
     #Python is a super weird language so make a decent list of np output
 
     max_pos = [float(max_pos[0]),float(max_pos[1])]
     min_pos = np.where(np.nanmin(sm_velocity_field) == sm_velocity_field)
     min_pos = [float(min_pos[0]),float(min_pos[1])]
 
-    if debug:
-        print_log(f'''GET_VEL_PA: This is the location of the maximum {max_pos} and minimum {min_pos}
-''',Configuration['OUTPUTLOG'])
+    print_log(f'''GET_VEL_PA: This is the location of the maximum {max_pos} and minimum {min_pos}
+''',Configuration,case=['debug_add'])
     try:
         pa_from_max = np.arctan((center[1]-max_pos[1])/(center[0]-max_pos[0]))
     except ZeroDivisionError:
         if center[1]-max_pos[1] >= 0.:
             pa_from_max = np.radians(90.)
         else:
             pa_from_max = np.radians(-90.)
@@ -1940,28 +2420,25 @@
             else:
                 pa = np.radians(360.) - pa
         elif pos1[1]-pos2[1] > 0:
             if pa < 0.:
                 pa = abs(pa)
             else:
                 pa = np.radians(180.) - pa
-    if debug:
-        print_log(f'''GET_VEL_PA: This is the PA
+    print_log(f'''GET_VEL_PA: This is the PA
 {'':8s} pa = {pa} pa_from_max = {pa_from_max} pa_from_min = {pa_from_min}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
     if np.degrees(abs(pa-pa_from_max)) > 170. or   np.degrees(abs(pa-pa_from_min)) > 170:
         pa = pa
     else:
         pa = np.nanmean([pa,pa_from_max,pa_from_min])
     center.reverse()
-    if debug:
-        print_log(f'''GET_VEL_PA: This is the PA we extract from the velpa {np.degrees(pa)}
-''',Configuration['OUTPUTLOG'])
+    print_log(f'''GET_VEL_PA: This is the PA we extract from the velpa {np.degrees(pa)}
+''',Configuration,case=['debug_add'])
     return np.degrees([pa, np.nanstd([pa,pa_from_max,pa_from_min])])
-
 get_vel_pa.__doc__ =f'''
  NAME:
     get_vel_pa
 
  PURPOSE:
     Routine to obtain the PA from a moment 1 map of a galaxy
 
@@ -1969,40 +2446,86 @@
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     velocity_field = the VF
 
  OPTIONAL INPUTS:
-    debug = False
+
     center = center of the galaxy
 
  OUTPUTS:
     mean and standard deviation of the pa from minimum value to center, maximum to center and minimum to maximum
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
+def isiterable(variable):
+    '''Check whether variable is iterable'''
+    #First check it is not a string as those are iterable
+    if isinstance(variable,str):
+        return False
+    try:
+        iter(variable)
+    except TypeError:
+        return False
+
+    return True
+isiterable.__doc__ =f'''
+ NAME:
+    isiterable
+
+ PURPOSE:
+    Check whether variable is iterable
+
+ CATEGORY:
+    support_functions
+
+ INPUTS:
+    variable = variable to check
+
+ OPTIONAL INPUTS:
+
+ OUTPUTS:
+    True if iterable False if not
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+
+
 # A simple function to return the line numbers in the stack from where the functions are called
-def linenumber(debug=False):
+def linenumber(debug='short'):
+    '''get the line number of the print statement in the main.'''
     line = []
     for key in stack():
         if key[1] == 'main.py':
             break
-        if key[3] != 'linenumber' and key[3] != 'print_log':
+        if key[3] != 'linenumber' and key[3] != 'print_log' and key[3] != '<module>':
             file = key[1].split('/')
-            line.append(f"In the function {key[3]} at line {key[2]} in file {file[-1]}")
+            to_add= f"In the function {key[3]} at line {key[2]}"
+            if debug == 'long':
+                to_add = f"{to_add} in file {file[-1]}."
+            else:
+                to_add = f"{to_add}."
+            line.append(to_add)
     if len(line) > 0:
-        if debug:
+        if debug == 'long':
             line = ', '.join(line)+f'\n{"":8s}'
+        elif debug == 'short':
+            line = line[0]+f'\n{"":8s}'
         else:
             line = f'{"":8s}'
     else:
         for key in stack():
             if key[1] == 'main.py':
                 line = f"{'('+str(key[2])+')':8s}"
                 break
@@ -2017,38 +2540,171 @@
 
  CATEGORY:
     support_functions
 
  INPUTS:
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     the line number of the print statement
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
     If debug = True the full stack of the line print will be given, in principle
     the first debug message in every function should set this to true and later messages not.
     !!!!Not sure whether currently the linenumber is produced due to the restructuring.
 '''
-def make_tiltogram(Configuration,Tirific_Template,debug =False):
-    if debug:
-        print_log(f'''MAKE_TILTOGRAM: Starting tiltogram.
-''',Configuration['OUTPUTLOG'])
-    pa_incl = np.array(get_from_template(Configuration,Tirific_Template,Variables=['PA','PA_2','INCL','INCL_2']),dtype=float)
-    sbr = np.array(get_from_template(Configuration,Tirific_Template, ["SBR",f"SBR_2"]),dtype=float)
-    systemic = np.array(get_from_template(Configuration,Tirific_Template, ["VSYS"]),dtype=float)
-    systemic = systemic[0,0]
-    radii,cut_off_limits = sbr_limits(Configuration, systemic= systemic , debug = debug)
+
+#The functions load_tirifiic,load_template and get_from template were extremely similar
+#This replaces all with a single function
+def load_tirific(Configuration,def_input,Variables = ['BMIN','BMAJ','BPA','RMS',\
+            'DISTANCE','NUR','RADI','VROT','Z0', 'SBR', 'INCL','PA','XPOS','YPOS',\
+            'VSYS','SDIS','VROT_2',  'Z0_2','SBR_2','INCL_2','PA_2','XPOS_2',\
+            'YPOS_2','VSYS_2','SDIS_2','CONDISP','CFLUX','CFLUX_2'],\
+             array = False,ensure_rings =False ):
+    # if the input is a string we first load the template
+    if isinstance(def_input,str):
+        def_input = tirific_template(filename = def_input )
+
+    out = []
+    for key in Variables:
+        try:
+            out.append([float(x) for x  in def_input[key].split()])
+        except KeyError:
+            out.append([])
+        except ValueError:
+            out.append([x for x  in def_input[key].split()])
+
+    #Because lists are stupid i.e. sbr[0][0] = SBR[0], sbr[1][0] = SBR_2[0] but  sbr[:][0] = SBR[:] not SBR[0],SBR_2[0] as logic would demand
+
+    if array:
+        tmp = out
+        #We can ensure that the output has the same number of values as there are rings
+        if ensure_rings:
+            length=int(def_input['NUR'])
+        else:
+            #or just take the longest input as the size
+            length = max(map(len,out))
+        #let's just order this in variable, values such that it unpacks properly into a list of variables
+        out = np.zeros((len(Variables),length),dtype=float)
+        for i,variable in enumerate(tmp):
+            if len(variable) > 0.:
+                out[i,0:len(variable)] = variable[0:len(variable)]
+
+    if len(Variables) == 1:
+        out= out[0]
+    print_log(f'''LOAD_TIRIFIC: We extracted the following profiles from the Template.
+{'':8s}Requested Variables = {Variables}
+{'':8s}Extracted = {out}
+''',Configuration,case=['debug_start'])
+    #Beware that lists are stupid i.e. sbr[0][0] = SBR[0], sbr[1][0] = SBR_2[0] but  sbr[:][0] = SBR[:] not SBR[0],SBR_2[0] as logic would demand
+    # However if you make a np. array from it make sure that you specify float  or have lists of the same length else you get an array of lists which behave just as dumb
+    return out
+load_tirific.__doc__ =f'''
+ NAME:
+    load_tirific
+
+ PURPOSE:
+    Load values from variables set in the tirific files
+
+ CATEGORY:
+    read_functions
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    def_input = Path to the tirific def file or a FAT tirific template dictionary
+
+ OPTIONAL INPUTS:
+    Variables = ['BMIN','BMAJ','BPA','RMS','DISTANCE','NUR','RADI','VROT',
+                 'Z0', 'SBR', 'INCL','PA','XPOS','YPOS','VSYS','SDIS','VROT_2',  'Z0_2','SBR_2',
+                 'INCL_2','PA_2','XPOS_2','YPOS_2','VSYS_2','SDIS_2','CONDISP','CFLUX','CFLUX_2']
+
+
+    array = False
+        Specify that the output should be an numpy array with all varables having the same length
+
+    ensure_rings =false
+        Specify that the output array should have the length of the NUR parameter in the def file
+ OUTPUTS:
+    outputarray array with all the values of the parameters requested
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+    This replaces load_tirific,load_template and get_from_template.
+'''
+
+
+def make_equal_length(list1_in,list2_in):
+    '''ensure that 2 lists have the same length'''
+    #python is a silly language
+    list1=list1_in.copy()
+    list2=list2_in.copy()
+
+    #We can only do this with lists so first we ensure lists
+    list1 = ensure_list(list1)
+    list2 = ensure_list(list2)
+
+    #We are matching the lists on the highest level only so if
+    if isiterable(list1[0]) or isiterable(list2[0]):
+        raise TypeError('make_equal_length only works on 1D arrays or scalars')
+
+    while len(list1) < len(list2):
+        list1.append(list1[-1])
+    while len(list1) > len(list2):
+        list2.append(list2[-1])
+    return list1, list2
+make_equal_length.__doc__ =f'''
+ NAME:
+    make_equal_length
+
+ PURPOSE:
+    ensure that 2 lists have the same length
+
+ CATEGORY:
+    support_functions
+
+ INPUTS:
+    list1, list2
+
+ OPTIONAL INPUTS:
+
+
+ OUTPUTS:
+    the lists with the same length.
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+    Lists are mutable objects so if the input are lists the return could give the impression that
+    the original lists remain unmodified. To ensure proper behaviour and not python magic the input
+    is copied at the start.
+'''
+
+
+def make_tiltogram(Configuration,Tirific_Template):
+    print_log(f'''MAKE_TILTOGRAM: Starting tiltogram.
+''',Configuration,case=['debug_start'])
+    pa_incl = load_tirific(Configuration,Tirific_Template,\
+            Variables=['PA','PA_2','INCL','INCL_2'],array=True)
+    sbr = load_tirific(Configuration,Tirific_Template,Variables=["SBR",f"SBR_2"]\
+            ,array=True)
+    radii,cut_off_limits = sbr_limits(Configuration,Tirific_Template )
     add = [[],[]]
     Theta = [[],[]]
     phi = [[],[]]
     x = [[],[]]
     y = [[],[]]
     z = [[],[]]
     tiltogram = [[],[]]
@@ -2059,20 +2715,19 @@
         with warnings.catch_warnings():
             warnings.simplefilter("ignore")
             Theta[i] = np.arctan(np.tan(np.radians(pa_incl[i+2]))*np.tan(np.radians(pa_incl[i])))
             phi[i] = np.arctan(np.tan(np.radians(pa_incl[i]))/np.sin(Theta[i]))
             x[i]=np.sin(Theta[i])*np.cos(phi[i])
             y[i]=np.sin(Theta[i])*np.sin(phi[i])
             z[i]=np.cos(Theta[i])
-            if debug:
-                print_log(f'''MAKE_TILTOGRAM: For the cartesian coordinates we find in side {i}
+            print_log(f'''MAKE_TILTOGRAM: For the cartesian coordinates we find in side {i}
 {'':8s} x = {x[i]}
 {'':8s} y = {y[i]}
 {'':8s} z = {z[i]}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
 
             tiltogram[i] = np.degrees(np.arccos(np.multiply.outer(x[i], x[i]).ravel().reshape(len(x[i]),len(x[i])) + \
                                          np.multiply.outer(y[i], y[i]).ravel().reshape(len(x[i]),len(x[i])) + \
                                          np.multiply.outer(z[i], z[i]).ravel().reshape(len(x[i]),len(x[i]))))
     tiltogram = np.array(tiltogram,dtype = float)
     tiltogram[np.isnan(tiltogram)]= 0.
 
@@ -2089,29 +2744,121 @@
     support_functions
 
  INPUTS:
     Configuration = standard FAT Configuration
     Tirific_Template = Standard Tirific template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     a multidimensionals array containig the tiltograms for both sides
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 
 '''
 
-def obtain_border_pix(Configuration,angle,center, debug = False):
+
+
+def max_profile_change(Configuration,radius,profile,key,max_change=None,\
+                        slope = None, kpc_radius=False):
+    if not kpc_radius:
+        radkpc = convertskyangle(Configuration,radius)
+    else:
+        radkpc = copy.deepcopy(radius)
+    new_profile = copy.deepcopy(profile)
+    sm_profile = savgol_filter(profile, 3, 1)
+    if key == 'ARBITRARY' and not max_change:
+        raise InputError('For arbitrary checks you have to set the max_change.')
+    if key != 'ARBITRARY':
+        max_change=Configuration['MAX_CHANGE'][key]
+    diff_rad =  [float(y-x) for x,y in zip(radkpc,radkpc[1:])]
+    diff_profile = [float(y-x) for x,y in zip(profile,profile[1:])]
+    diff_sm_profile = [float(y-x) for x,y in zip(sm_profile,sm_profile[1:])]
+    print_log(f'''MAX_CHANGE_PROFILE: The profile {key} starts with.
+{'':8s} {key} = {new_profile} and max change = {max_change}
+{'':8s} smoothed {key}  = {sm_profile}
+{'':8s} diff per ring = {diff_profile}
+{'':8s} smoothed dif per ring = {diff_sm_profile}
+{'':8s} slope = {slope}
+{'':8s} diff/kpc = {[x/y for x,y in zip(diff_profile,diff_rad)]}
+''', Configuration,case=['debug_start'])
+
+    for i,diff in enumerate(diff_profile):
+        if abs(diff)/diff_rad[i] > max_change:
+            #if it is the last point we simply limit it
+            if i == len(diff_profile)-1:
+                new_profile[i+1] = profile[i]+ diff/abs(diff)*(max_change*0.5*diff_rad[i])
+            elif i+1 == slope:
+                # if we have the start of the slope on the max_change then put it to value of the previous ring
+                new_profile[i+1] = new_profile[i]
+            elif diff_sm_profile[i]/diff_rad[i] < max_change*0.5:
+                new_profile[i+1] = sm_profile[i+1]
+            elif diff_profile[i+1] == 0:
+                new_profile[i+1] = profile[i]+ diff/abs(diff)*(max_change*0.9*diff_rad[i])
+                #If the change does not reverse we simply limit
+            elif diff/abs(diff) == diff_profile[i+1]/abs(diff_profile[i+1]):
+                new_profile[i+1] = profile[i]+ diff/abs(diff)*(max_change*0.9*diff_rad[i])
+            else:
+                if abs(diff) > abs(diff_profile[i+1]):
+                    gapped_diff = radkpc[i+2] - radkpc[i]
+                    if abs(new_profile[i]-new_profile[i+2])/gapped_diff < max_change:
+                        new_profile[i+1] = np.mean([new_profile[i],new_profile[i+2]])
+                    else:
+                        new_profile[i+1] = new_profile[i]
+                else:
+
+                    new_profile[i+1] = profile[i]+ diff/abs(diff)*(max_change*0.9*diff_rad[i])
+
+            if i < len(diff_profile)-1:
+                diff_profile[i+1] = float(new_profile[i+2]-new_profile[i+1])
+
+    print_log(f'''MAX_CHANGE_PROFILE: The returned profile is:
+{'':8s}{key} = {new_profile}
+''', Configuration,case=['debug_add'])
+    return new_profile
+max_profile_change.__doc__ =f'''
+ NAME:
+     max_profile_change
+
+ PURPOSE:
+    Check that the profile is not change more than the maximum per kpc and correct if it does
+
+ CATEGORY:
+    support_functions
+
+ INPUTS:
+    Configuration = standard FAT Configuration
+    radius = radius corresponding to the profile
+    profile = profile to examine
+    key = the parameter to indicate the type of profile
+
+ OPTIONAL INPUTS:
+
+
+ OUTPUTS:
+    new_profile
+    the modified profile
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+
+'''
+
+
+def obtain_border_pix(Configuration,angle,center):
     rotate = False
     # only setup for 0-180 but 180.-360 is the same but -180
     if angle > 180.:
         angle -= 180.
         rotate = True
 
     if angle < 90.:
@@ -2162,59 +2909,53 @@
  INPUTS:
     Configuration = standard FAT Configuration
     hdr = header of the map
     angle = the angle of the line running through the map
     center = center of the line running through the map
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     x,y
     pixel locations of how the line runs through the map
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     np.tan,np.radians,.reverse()
 
  NOTE:
 '''
 
-def obtain_ratios(Configuration, map, center, angles, noise = 0. ,debug = False):
+def obtain_ratios(Configuration, map, center, angles, noise = 0. ):
     ratios = []
     max_extent = 0.
     for angle in angles:
         #major axis
-        maj_profile,maj_axis,maj_resolution = get_profile(Configuration,map,angle,center=center,debug=debug)
+        maj_profile,maj_axis,maj_resolution = get_profile(Configuration,map,angle,center=center )
         tmp = np.where(maj_profile > noise)[0]
-        #gauss =fit_gaussian(maj_axis[tmp], maj_profile[tmp])
-        #maj_gaus = gaussian_function(maj_profile, *gauss)
-        #tmp = np.where(maj_gaus > 0.2*np.nanmax(maj_gaus))[0]
         if tmp.shape[0] == 0.:
              width_maj = 0.
         else:
             width_maj = (tmp[-1]-tmp[0])*maj_resolution
             if width_maj**2 > Configuration['BEAM_IN_PIXELS'][0]**2:
                 width_maj = np.sqrt(width_maj**2 - Configuration['BEAM_IN_PIXELS'][0]**2)
             else:
                 if width_maj < Configuration['BEAM_IN_PIXELS'][0]:
                     width_maj = Configuration['BEAM_IN_PIXELS'][0]
 
         if width_maj > max_extent:
             max_extent = width_maj
         #minor axis
         if angle < 90:
-            min_profile,min_axis,min_resolution = get_profile(Configuration,map,angle+90,center=center,debug=debug)
+            min_profile,min_axis,min_resolution = get_profile(Configuration,map,angle+90,center=center )
         else:
-            min_profile,min_axis,min_resolution = get_profile(Configuration,map,angle-90,center=center,debug=debug)
+            min_profile,min_axis,min_resolution = get_profile(Configuration,map,angle-90,center=center )
         tmp = np.where(min_profile > noise)[0]
-        #gauss =fit_gaussian(min_axis[tmp], maj_profile[tmp])
-        #min_gaus = gaussian_function(min_profile,*gauss)
-        #tmp = np.where(min_gaus > 0.2*np.nanmax(min_gaus))[0]
         if tmp.shape[0] == 0.:
              width_min = 0.
         else:
             width_min = (tmp[-1]-tmp[0])*min_resolution
             if width_min**2 > Configuration['BEAM_IN_PIXELS'][0]**2:
                 width_min = np.sqrt(width_min**2 - Configuration['BEAM_IN_PIXELS'][0]**2)
             else:
@@ -2249,50 +2990,67 @@
        center = estimated center
        angles = angles to look for the ratios
 
  OPTIONAL INPUTS:
        noise = 0.
        noise level in the map
 
-       debug = False
+
 
  OUTPUTS:
          ratios =  ratios corresponding to the input angles
          max_extent = the maximum extend of any profile analysed (in degree)
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
       np.mean, ndimage.map_coordinates, np.linspace, np.vstack, np.cos, np.radians, np.sin
 
  NOTE:
 '''
 
-def print_log(log_statement,log, screen = False,debug = False):
+def print_log(log_statement,Configuration,case=['main']):
+
+    if Configuration['DEBUG']:
+        if 'debug_start' in case:
+            debug = 'long'
+        else:
+            debug= 'short'
+    else:
+        debug = 'empty'
     log_statement = f"{linenumber(debug=debug)}{log_statement}"
-    if screen or not log:
-        print(log_statement)
-    if log:
-        with open(log,'a') as log_file:
-            log_file.write(log_statement)
+    print_statement = False
+    if (Configuration['DEBUG'] and ('debug_start' in case or 'debug_add' in case))\
+        or ('verbose' in case and (Configuration['VERBOSE_LOG'] or Configuration['DEBUG']))\
+         or 'main' in case:
+            print_statement = True
+    if print_statement:
+        if Configuration['VERBOSE_SCREEN'] \
+            or not Configuration['OUTPUTLOG']  \
+            or 'screen' in case \
+            or (Configuration['VERBOSE_LOG'] and 'main' in case):
+            print(log_statement)
+        if Configuration['OUTPUTLOG']:
+            with open(Configuration['OUTPUTLOG'],'a') as log_file:
+                log_file.write(log_statement)
 
 print_log.__doc__ =f'''
  NAME:
     print_log
  PURPOSE:
     Print statements to log if existent and screen if Requested
  CATEGORY:
     support_functions
 
  INPUTS:
     log_statement = statement to be printed
-    log = log to print to, can be None
+    Configuration = Standard FAT Configuration
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     screen = False
     also print the statement to the screen
 
  OUTPUTS:
     line in the log or on the screen
 
@@ -2302,52 +3060,51 @@
     linenumber, .write
 
  NOTE:
     If the log is None messages are printed to the screen.
     This is useful for testing functions.
 '''
 
-def remove_inhomogeneities(Configuration,fits_map_in,inclination=30., pa = 90. , center = [0.,0.],WCS_center = True, iteration= 0 , debug=False):
+def remove_inhomogeneities(Configuration,fits_map_in,inclination=30., pa = 90. , center = [0.,0.],WCS_center = True, iteration= 0 ):
     fits_map = copy.deepcopy(fits_map_in)
-    if debug:
-        print_log(f'''REMOVE_INHOMOGENEITIES: These are the values we get as input
+    print_log(f'''REMOVE_INHOMOGENEITIES: These are the values we get as input
 {'':8s}Inclination = {inclination}
 {'':8s}pa = {pa}
 {'':8s}center = {center}, WCS = {WCS_center}
 {'':8s}map shape = {np.shape(fits_map[0].data)}
-''',Configuration['OUTPUTLOG'],debug = True)
+''',Configuration,case=['debug_start'])
     map = fits_map[0].data
     # first rotate the pa
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         map_wcs = WCS(fits_map[0].header)
     # convert the boundaries to real coordinates
     if WCS_center:
         x, y = map_wcs.wcs_world2pix(*center, 1)
     else:
         x = center[0]
         y = center[1]
-    rot_map = rotateImage(Configuration,map,pa-90,[x,y],debug=debug)
+    rot_map = rotateImage(Configuration,map,pa-90,[x,y] )
     # deproject
-    dep_map = deproject(Configuration,copy.deepcopy(rot_map),inclination,center = y, debug=debug)
+    dep_map = deproject(Configuration,copy.deepcopy(rot_map),inclination,center = y )
 
-    if debug:
+    if Configuration['DEBUG']:
         fits.writeto(f"{Configuration['FITTING_DIR']}rot_map_{int(iteration)}.fits",rot_map,fits_map[0].header,overwrite = True)
         fits.writeto(f"{Configuration['FITTING_DIR']}dep_map_{int(iteration)}.fits",dep_map,fits_map[0].header,overwrite = True)
 
     angles = np.linspace(5.,360.,71)
     minimum_map = copy.deepcopy(dep_map)
     for angle in angles:
-        rot_dep_map =  rotateImage(Configuration,copy.deepcopy(dep_map),angle,[x,y],debug=debug)
+        rot_dep_map =  rotateImage(Configuration,copy.deepcopy(dep_map),angle,[x,y] )
 
         #tmp = np.where(rot_dep_map < minimum_map)[0]
         minimum_map[rot_dep_map < minimum_map] =rot_dep_map[rot_dep_map < minimum_map]
-    clean_map = rotateImage(Configuration,deproject(Configuration,copy.deepcopy(minimum_map),inclination,center = y,invert= True,debug=debug),-1*(pa-90),[x,y],debug=debug)
+    clean_map = rotateImage(Configuration,deproject(Configuration,copy.deepcopy(minimum_map),inclination,center = y,invert= True ),-1*(pa-90),[x,y] )
 
-    if debug:
+    if Configuration['DEBUG']:
         fits.writeto(f"{Configuration['FITTING_DIR']}minimum_map_{int(iteration)}.fits",minimum_map,fits_map[0].header,overwrite = True)
         fits.writeto(f"{Configuration['FITTING_DIR']}clean_map_{int(iteration)}.fits",clean_map,fits_map[0].header,overwrite = True)
     fits_map[0].data = clean_map
     return fits_map
 
 remove_inhomogeneities.__doc__ =f'''
  NAME:
@@ -2361,15 +3118,15 @@
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     fits_map = intensity map of the galaxy as an astropy structure, i.e fits_map[0].header and fits_map[0].data
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     inclination=30.
     inclination of the galaxy
 
     pa = 90.
     PA of the galaxy
 
@@ -2395,15 +3152,15 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def rename_fit_products(Configuration,stage = 'initial', fit_type='Undefined',debug = False):
+def rename_fit_products(Configuration,stage = 'initial', fit_type='Undefined'):
     extensions = ['def','log','ps','fits']
     for filetype in extensions:
         source = get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.{filetype}")
         if filetype == 'log':
             if os.path.exists(f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.{filetype}"):
                 target = get_system_string(f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Prev.{filetype}")
                 os.system(f"cp {source} {target}")
@@ -2435,15 +3192,15 @@
  CATEGORY:
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     stage = 'initial'
     stage of the type of fitting
 
     fit_type='Undefined'
     Type of fitting
 
@@ -2454,15 +3211,15 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 #function to rotate an image without losing info
-def rotateImage(Configuration,image, angle, pivot, debug = False):
+def rotateImage(Configuration,image, angle, pivot):
     padX = [int(image.shape[1] - pivot[0]), int(pivot[0])]
     padY = [int(image.shape[0] - pivot[1]), int(pivot[1])]
     imgP = np.pad(image, [padY, padX], 'constant')
     imgR = ndimage.rotate(imgP, angle, axes=(1, 0), reshape=False)
     return imgR[padY[0]: -padY[1], padX[0]: -padX[1]]
 
 rotateImage.__doc__ =f'''
@@ -2478,119 +3235,139 @@
  INPUTS:
     Configuration = Standard FAT configuration
     image = Image to rotate
     angle =  the angle to rotate the image by
     pivot = the center around which to rotate
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     The rotated image is returned
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 
-def run_tirific(Configuration, current_run, stage = 'initial',fit_type = 'Undefined',deffile='Undefined', debug = False):
-    if debug:
-        print_log(f'''RUN_TIRIFIC: Starting a new run in stage {stage} and fit_type {fit_type}
-''',Configuration['OUTPUTLOG'], screen = True,debug = debug)
+def run_tirific(Configuration, current_run, stage = 'initial',fit_type = 'Undefined',deffile='Undefined'):
+    print_log(f'''RUN_TIRIFIC: For the galaxy {Configuration['ID']} in directory {Configuration['SUB_DIR']} we are starting a new TiRiFiC.
+We are in in stage {stage} and fit_type {fit_type} and have done {Configuration['ITERATIONS']} loops
+''',Configuration,case=['debug_start'])
     if deffile == 'Undefined':
         deffile=f"{fit_type}_In.def"
 
     # First move the previous fits
-    rename_fit_products(Configuration,fit_type = fit_type, stage=stage, debug = debug)
-    # Then if already running change restart file
+    rename_fit_products(Configuration,fit_type = fit_type, stage=stage )
+    #If we are debug let's write the config file
+    if Configuration['DEBUG']:
+        if stage == 'run_os':
+            write_config(
+                f'{Configuration["LOG_DIRECTORY"]}CFG_Before_Iteration_{Configuration["ITERATIONS"]}.txt', Configuration)
     if fit_type == 'Error_Shaker':
         work_dir = os.getcwd()
         restart_file = f"restart_Error_Shaker.txt"
     else:
         restart_file = f"{Configuration['LOG_DIRECTORY']}restart_{fit_type}.txt"
         work_dir = Configuration['FITTING_DIR']
+    #Get the output fits file and def file defined in workdir+ deffile
+    output_fits,output_deffile = get_tirific_output_names(Configuration,work_dir,deffile )
+    # Then if already running change restart file
     if Configuration['TIRIFIC_RUNNING']:
-        print_log(f'''RUN_TIRIFIC: We are using an initialized tirific in {Configuration['FITTING_DIR']}
-''',Configuration['OUTPUTLOG'], screen = True)
+        print_log(f'''RUN_TIRIFIC: We are using an initialized tirific in {Configuration['FITTING_DIR']} with the file {deffile}
+''',Configuration)
 
         with open(restart_file,'a') as file:
             file.write("Restarting from previous run \n")
     else:
-        print_log(f'''RUN_TIRIFIC: We are starting a new TiRiFiC in {Configuration['FITTING_DIR']}
-''',Configuration['OUTPUTLOG'], screen = True)
+        print_log(f'''RUN_TIRIFIC: We are starting a new TiRiFiC in {Configuration['FITTING_DIR']} with the file {deffile}
+''',Configuration)
         with open(restart_file,'w') as file:
             file.write("Initialized a new run \n")
         current_run = subprocess.Popen([Configuration['TIRIFIC'],f"DEFFILE={deffile}","ACTION= 1"],\
                                        stdout = subprocess.PIPE, stderr = subprocess.PIPE,\
                                        cwd=work_dir,universal_newlines = True)
 
 
         Configuration['TIRIFIC_RUNNING'] = True
         Configuration['TIRIFIC_PID'] = current_run.pid
     currentloop =1
     max_loop = 0
     counter = 0
+
     current_process= psu.Process(current_run.pid)
+
     if Configuration['TIMING']:
         time.sleep(0.1)
         with open(f"{Configuration['LOG_DIRECTORY']}Usage_Statistics.txt",'a') as file:
             file.write(f"# TIRIFIC: Initializing Tirific at stage = {fit_type} {datetime.now()} \n")
             CPU,mem = get_usage_statistics(Configuration,current_process)
             file.write(f"{datetime.now()} CPU = {CPU} % Mem = {mem} Mb for TiRiFiC \n")
     else:
         time.sleep(0.1)
-    print(f"\r{'':8s}RUN_TIRIFIC: 0 % Completed", end =" ",flush = True)
+    if Configuration['VERBOSE_SCREEN']:
+        print(f"\r{'':8s}RUN_TIRIFIC: 0 % Completed", end =" ",flush = True)
     triggered = False
     for tir_out_line in current_run.stdout:
         tmp = re.split(r"[/: ]+",tir_out_line.strip())
         counter += 1
         if (counter % 50) == 0:
             if Configuration['TIMING']:
                 with open(f"{Configuration['LOG_DIRECTORY']}Usage_Statistics.txt",'a') as file:
                     if tmp[0] == 'L' and not triggered:
                         if tmp[1] == '1':
                             file.write(f"# TIRIFIC: Started the actual fitting {datetime.now()} \n")
                             triggered = True
                     CPU,mem = get_usage_statistics(Configuration,current_process)
                     file.write(f"{datetime.now()} CPU = {CPU} % Mem = {mem} Mb for TiRiFiC \n")
         if tmp[0] == 'L':
-            if int(tmp[1]) != currentloop:
-                print(f"\r{'':8s}RUN_TIRIFIC: {float(tmp[1])/float(max_loop)*100.:.1f} % Completed", end =" ",flush = True)
+            if int(tmp[1]) != currentloop and Configuration['VERBOSE_SCREEN']:
+                print(f"\r{'':8s}RUN_TIRIFIC: {set_limits(float(tmp[1])-1.,0.,float(max_loop))/float(max_loop)*100.:.1f} % Completed", end =" ",flush = True)
             currentloop  = int(tmp[1])
             if max_loop == 0:
                 max_loop = int(tmp[2])
-            try:
-                Configuration['NO_POINTSOURCES'] = np.array([tmp[18],tmp[19]],dtype=float)
-            except:
-                #If this fails for some reason an old number suffices, if the code really crashed problems will occur elsewhere.
-                pass
+
+            Configuration['NO_POINTSOURCES'] = np.array([tmp[18],tmp[19]],dtype=float)
+
         if tmp[0].strip() == 'Finished':
             break
         if tmp[0].strip() == 'Abort':
             break
-    print(f'\n')
+    if Configuration['VERBOSE_SCREEN']:
+        print(f'\n')
     if Configuration['TIMING']:
         with open(f"{Configuration['LOG_DIRECTORY']}Usage_Statistics.txt",'a') as file:
             file.write(f"# TIRIFIC: Finished this run {datetime.now()} \n")
             CPU,mem = get_usage_statistics(Configuration,current_process)
             file.write(f"{datetime.now()} CPU = {CPU} % Mem = {mem} Mb for TiRiFiC \n")
-    print(f"{'':8s}RUN_TIRIFIC: Finished the current tirific run.")
+    if Configuration['VERBOSE_SCREEN']:
+        print(f"{'':8s}RUN_TIRIFIC: Finished the current tirific run.")
 
     #The break off goes faster sometimes than the writing of the file so let's make sure it is present
     time.sleep(1.0)
     wait_counter = 0
     if fit_type != 'Error_Shaker':
-        while not os.path.exists(f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}.fits") and wait_counter < 1000.:
-            print(f"\r Waiting ", end = "", flush = True)
-            time.sleep(0.5)
+        while not os.path.exists(output_fits) and wait_counter < 100.:
+            time.sleep(0.3)
             wait_counter += 1
+            if wait_counter/10. == int(wait_counter/10.):
+                print(f"\r Waiting for {output_fits}. \n", end = "", flush = True)
+                print_log(f'''RUN_TIRIFIC: we have waited {0.3*wait_counter} seconds for the output of tirific but it is not there yet.
+''',Configuration)
+        if not  os.path.exists(output_fits) \
+            or not  os.path.exists(output_deffile):
+            print_log(f'''RUN_TIRIFIC: After 30 seconds we could not find the expected output from the tirific run. We are raising an error for this galaxy.
+''',Configuration,case=['main','screen'])
+            raise TirificOutputError(f'''The tirific subprocess did not produce the correct output, most likely it crashed.
+We were running {deffile} and failed to find the output {output_fits} or {output_deffile}.
+''')
 
     if currentloop != max_loop:
         return 1,current_run
     else:
         return 0,current_run
 run_tirific.__doc__ =f'''
  NAME:
@@ -2603,15 +3380,15 @@
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     current_run = subprocess structure of tirific
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     fit_type = 'Undefined'
     type of fitting
 
     stage = 'initial'
     stage of the fitting process
 
@@ -2622,15 +3399,18 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 
-def set_boundaries(Configuration,key,lower,upper,input=False,debug=False):
+def set_boundaries(Configuration,key,lower,upper,input=False):
+    print_log(f'''SET_BOUNDARIES: Starting to implement the boundaries for {key} with lower = {lower} and upper = {upper}.
+''',Configuration,case=['debug_start'])
+
     check=False
     key = key.upper()
     if np.sum(Configuration[f'{key}_INPUT_BOUNDARY']) != 0.:
         check = True
     if input:
         boundary = f'{key}_INPUT_BOUNDARY'
     else:
@@ -2669,29 +3449,81 @@
  INPUTS:
     Configuration = Standard FAT configuration
     key = name of the parameter
     lower = the lower boundary
     upper = upper boundary
 
  OPTIONAL INPUTS:
-    debug = False
+
     input = False
     if set to true the user input parameters are updated. this should only be used
     when reading the cube to set the input VSYS, XPOS and YPOS limits.
 
  OUTPUTS:
     updated boundary limits. When user input is set these can never be loewer/higher than those limits.
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
+#Set the indivdual configuration such that the loop can run without the full catalogue
+def set_individual_configuration(current_galaxy_index,Full_Catalogue,Original_Configuration):
+    Configuration = copy.deepcopy(Original_Configuration)
+    Configuration['ID'] = Full_Catalogue['ID'][current_galaxy_index]
+    if Full_Catalogue['DISTANCE'][current_galaxy_index] != -1.:
+        Configuration['DISTANCE'] = Full_Catalogue['DISTANCE'][current_galaxy_index]
+    Configuration['SUB_DIR'] = Full_Catalogue['DIRECTORYNAME'][current_galaxy_index]
+    Configuration['BASE_NAME'] = Full_Catalogue['CUBENAME'][current_galaxy_index]+'_FAT'
+    if not Configuration['SOFIA_BASENAME']:
+        if 'BASENAME' in Full_Catalogue['ENTRIES']:
+            Configuration['SOFIA_BASENAME'] = Full_Catalogue['BASENAME'][current_galaxy_index]
+        else:
+            Configuration['SOFIA_BASENAME'] = Configuration['BASE_NAME']
+    #Add our fitting directory to the Configuration
+    #Maindir always ends in slash already
+    if Full_Catalogue['DIRECTORYNAME'][current_galaxy_index] == './':
+        Configuration['FITTING_DIR'] = f"{Configuration['MAIN_DIRECTORY']}"
+    else:
+        Configuration['FITTING_DIR'] = f"{Configuration['MAIN_DIRECTORY']}{Full_Catalogue['DIRECTORYNAME'][current_galaxy_index]}/"
+
+    Configuration['INPUT_CUBE']= f"{Full_Catalogue['CUBENAME'][current_galaxy_index]}.fits"
+    return(Configuration)
+set_individual_configuration.__doc__ =f'''
+ NAME:
+    set_individual_configuration
+
+ PURPOSE:
+    Fill the parameters of the configuration file that come from the catalogue
+
+ CATEGORY:
+    support_functions
+
+ INPUTS:
+    current_galaxy_index = index in the full catalogue
+
+    Full_Catalogue = the full catalogue
+
+    Original_Configuration = The original Configuration that applies to each galaxy
+
+
+ OPTIONAL INPUTS:
+
+ OUTPUTS:
+    A configuration for an individual galaxy
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:Configf
+'''
 
 #Function to read FAT configuration file into a dictionary
 def setup_configuration(cfg):
     if cfg.installation_check:
         cfg.fitting.fixed_parameters=['INCL','PA','SDIS']
         cfg.advanced.max_iterations= 1
         cfg.advanced.loops= 1
@@ -2701,119 +3533,139 @@
         cfg.cube_name = 'NGC_2903.fits'
         test_files = ['NGC_2903.fits','ModelInput.def']
         if not os.path.isdir(cfg.input.main_directory):
             os.mkdir(cfg.input.main_directory)
         else:
             for file in test_files:
                 try:
-                    os.remove(test_dir+file)
-                except:
+                    os.remove(f'{cfg.input.main_directory}/{file}')
+                except FileNotFoundError:
                     pass
 
         my_resources = import_pack_files('pyFAT_astro.Installation_Check')
         for file in test_files:
             data = (my_resources / file).read_bytes()
             with open(cfg.input.main_directory+file,'w+b') as tmp:
                 tmp.write(data)
     if cfg.cube_name:
         cfg.input.catalogue = None
+        cfg.advanced.multiprocessing = False
         cfg.fitting.catalogue_start_id= '-1'
         cfg.fitting.catalogue_end_id= '-1'
 
-
     Configuration = Proper_Dictionary({})
 
     for key in cfg._content:
         input_key = getattr(cfg,key)
-        check_type=str(type(input_key))
-        if check_type[0] =='<':
-            check_type =  check_type.split('\'')[1]
-        if check_type == 'omegaconf.dictconfig.DictConfig':
+
+        if isinstance(input_key,omegaconf.dictconfig.DictConfig):
             for sub_key in input_key._content:
                 if str(key) == 'output' and str(sub_key) == 'catalogue':
                     Configuration['OUTPUT_CATALOGUE'] =  getattr(input_key,sub_key)
                 elif str(key) == 'fitting' and str(sub_key) == 'fixed_parameters':
                     value = getattr(input_key,sub_key)
-                    for req_key in ['Z0','XPOS','YPOS','VSYS']:
+                    for req_key in ['XPOS','YPOS','VSYS']:
                         if req_key not in value:
                             value.append(req_key)
                     Configuration[str(sub_key).upper()] =  [value,value]
+                elif isinstance(getattr(input_key,sub_key),omegaconf.listconfig.ListConfig):
+                    Configuration[str(sub_key).upper()] = list(getattr(input_key,sub_key))
+                    for i,oyt in enumerate(Configuration[str(sub_key).upper()]):
+                        if isinstance(oyt,omegaconf.listconfig.ListConfig):
+                            Configuration[str(sub_key).upper()][i] = list(oyt)
                 else:
                     Configuration[str(sub_key).upper()] =  getattr(input_key,sub_key)
         else:
             Configuration[str(key).upper()] = input_key
+
+
     # None cfg additions, that is additions that should be reset for every galaxy
 
     boolean_keys = ['OPTIMIZED', # Are we fitting an optimized cube
                 'TIRIFIC_RUNNING', # Is there a tirific initialized
                 'OUTER_RINGS_DOUBLED', #Do the outer rings have twice the size of the inner rings
                 'NEW_RING_SIZE',  #Have we update the size of the ring while not yet updating the template
                 'VEL_SMOOTH_EXTENDED', # Is the velocity smoothing extended ????
                 'EXCLUDE_CENTRAL', # Do we exclude the central part of the fitting due to blanks/an absorption source
                 'ACCEPTED',
+                'FIX_RING_SIZE', #Do we allow FAT to vary the rings size (False) or not (True)
+                'ACCEPTED_TIRIFIC', #Did Tirific run the full loops (False) or not (True)
                 'SOFIA_RAN', #Check if we have ran Sofia
-                'NO_RADEC'
+                'NO_RADEC',
+                'CENTRAL_CONVERGENCE' #Have we found the center
                 ]
 #
     for key in boolean_keys:
         Configuration[key] = False
-
+    if Configuration['RING_SIZE'] < 0.:
+        Configuration['FIX_RING_SIZE'] = True
+        Configuration['RING_SIZE'] = abs(Configuration['RING_SIZE'])
+    Configuration['FIX_SIZE'] = [False,False]# If we have before fitted a size we want to fix to this size to avoid looping
     other_keys={'ID': 'Unset', # ID of the galaxy in the catalogue , set from the catalogue at start of loop
                'SUB_DIR': 'Unset', # Name of the directory in which galaxy resides, set from the catalogue at start of loop
                'FITTING_DIR': 'Unset', # Full path of the directory in which the fitting takes place, set at start of loop
                'BASE_NAME': 'Unset', #Basename for FAT products, typically {input_cube}_FAT, set at start of loop
                'LOG_DIR': 'Unset', #Directory to put log files from run, set at start of loop
-
+               'INPUT_CUBE': 'Unset', # Name of the input cube as listed in full catalogue
+               'STOP_INDIVIDUAL_ERRORS': ['SmallSourceError','BadSourceError'\
+                                        ,'FaintSourceError','BadHeaderError',\
+                                        'BadCubeError','BadMaskError',\
+                                        'BadCatalogueError'],
+               'MAXIMUM_DIRECTORY_LENGTH': len('Directory Name'),
                'PREP_END_TIME': 'Not completed',
                'START_TIME':'Not completed',
                'END_TIME':'Not completed',
-               'OUTPUTLOG':'Not set yet',
+               'OUTPUTLOG': None,
                'RUN_COUNTER': 0,
+               'CENTRAL_CONVERGENCE_COUNTER': 1.,
                'ITERATIONS': 0,
                'CURRENT_STAGE': 'initial', #Current stage of the fitting process, set at switiching stages
                'USED_FITTING': None,
                'TIRIFIC_PID': 'Not Initialized', #Process ID of tirific that is running
                'FAT_PID': os.getpid(), #Process ID of FAT that is running
                'FAT_PSUPROCESS': 'cant copy',
-               'FINAL_COMMENT': "This fitting stopped with an unregistered exit.",
+               'FINAL_COMMENT': "This fitting stopped with an unregistered exit.", 
 
                'MAX_SIZE_IN_BEAMS': 30, # The galaxy is not allowed to extend beyond this number of beams in radius, set in check_source
                'MIN_SIZE_IN_BEAMS': 0., # Minimum allowed radius in number of beams of the galaxy, set in check_source
-               'SIZE_IN_BEAMS': 0, # The radius of the galaxy in number of beams, adapted after running Sofia
+               'SIZE_IN_BEAMS': np.full(2,0.,dtype=float),  #The radius of the galaxy in number of beams, adapted after running Sofia
                'NO_RINGS': 0., # The number of rings in the fit,
                'LAST_RELIABLE_RINGS': [0.,0.], # Location of the rings where the SBR drops below the cutoff limits, adapted after every run. Should only be modified in check_size
                'LIMIT_MODIFIER': [1.], #Modifier for the cutoff limits based on the inclination , adapted after every run.
-               'OLD_RINGS': [], # List to keep track of the ring sizes that have been fitted.
+               'OLD_SIZE': [[0.,0.]], # List to keep track of the size in beams.
 
                'NO_POINTSOURCES': 0. , # Number of point sources, set in run_tirific
 
-               'INNER_FIX': [4.,4.], #Number of rings that are fixed in the inner part for the INCL and PA, , adapted after every run in get_inner_fix in support_functions and for both sides
-               'WARP_SLOPE': [0.,0.], #Ring numbers from which outwards the warping should be fitted as a slope, set in get_warp_slope in modify_template
+               'INNER_FIX': [4,4], #Number of rings that are fixed in the inner part for the INCL and PA, , adapted after every run in get_inner_fix in support_functions and for both sides
+               'CENTRAL_FIX': [], #Parameters of the center to fix. This set in check_central_convergence
+               'WARP_SLOPE': [None, None], #Ring numbers from which outwards the warping should be fitted as a slope, set in get_warp_slope in modify_template
                'OUTER_SLOPE_START': 1, # Ring number from where the RC is fitted as a slope
                'RC_UNRELIABLE': 1, # Ring number from where the RC values are set flat. Should only be set in check_size
 
                'NOISE': 0. , #Noise of the input cube in Jy/beam, set in read_cube
-               'BEAM_IN_PIXELS': [0.,0.,0.], #FWHM BMAJ, BMIN in pixels and total number of pixels in beam area, set in main
+               'SNR': 0, # the mean SNR in the moment 0 map sofia mask these are set in guess_orientation
+               'BEAM_IN_PIXELS': [0.,0.,0.], #FWHM BMAJ, BMIN in pixels and total number of pixels in beam area, set in read_cube in read_functions
                'BEAM': [0.,0.,0.], #  FWHM BMAJ, BMIN in arcsec and BPA, set in main
                'BEAM_AREA': 0., #BEAM_AREA in arcsec set in main
                'NAXES': [0.,0.,0.], #  Size of the cube in pixels x,y,z arranged like sane people not python, set in main
                'MAX_ERROR': {}, #The maximum allowed errors for the parameters, set in main derived from cube
                'MIN_ERROR': {}, #The minumum allowed errors for the parameters, initially set in check_source but can be modified through out INCL,PA,SDSIS,Z0 errors change when the parameters is fixed or release
+               'MAX_CHANGE': {'INCL': 6.25, 'PA': 25.}, #The maximum change in a parameter in unit/kpc
                'CHANNEL_WIDTH': 0., #Width of the channel in the cube in km/s, set in main derived from cube
                'PIXEL_SIZE': 0., #'Size of the pixels in degree'
                }
     #####!!!!!!!!!!!!!!!!!!!!!!!!!!!! The use of min_error is not full implemented yet!!!!!!!!!!!!!!!!!!!!!!!!!
     for key in other_keys:
         Configuration[key] = other_keys[key]
 
     #If the input boundaries are unset we will set some reasonable limits
 
 
 # The parameters that need boundary limits are set here
-    boundary_limit_keys = ['PA','INCL', 'SDIS', 'Z0','VSYS','XPOS','YPOS','VROT']
+    boundary_limit_keys = ['PA','INCL', 'SDIS', 'Z0','VSYS','XPOS','YPOS','VROT','SBR']
     for key in boundary_limit_keys:
         if np.sum(Configuration[f"{key}_INPUT_BOUNDARY"]) == 0.:
             if key == 'INCL':
                 Configuration[f"{key}_INPUT_BOUNDARY"] = [[5.,90.] for x in range(3)]
             elif key == 'PA':
                 Configuration[f"{key}_INPUT_BOUNDARY"] = [[-10.,370.] for x in range(3)]
             else:
@@ -2827,24 +3679,30 @@
         Configuration['MAIN_DIRECTORY'] = f"{Configuration['MAIN_DIRECTORY']}/"
 
     while not os.path.isdir(Configuration['MAIN_DIRECTORY']):
         Configuration['MAIN_DIRECTORY'] = input(f'''
 Your main fitting directory ({Configuration['MAIN_DIRECTORY']}) does not exist.
 Please provide the correct directory.
 :  ''')
+
     if Configuration['CATALOGUE']:
+        if not os.path.exists(Configuration['CATALOGUE']) and len(Configuration['CATALOGUE'].split('/')) == 1:
+            Configuration['CATALOGUE']= f'''{Configuration['MAIN_DIRECTORY']}{Configuration['CATALOGUE']}'''
+
         while not os.path.exists(Configuration['CATALOGUE']):
             Configuration['CATALOGUE'] = input(f'''
 Your input catalogue ({Configuration['CATALOGUE']}) does not exist.
-Please provide the correct file name.
+Please provide the correct path and file name.
 : ''')
     #Make sure there is only one Fit_ stage
 
     # Make sure all selected stages exist
-    possible_stages = ['Fit_Tirific_OSC','Create_FAT_Cube','Run_Sofia','Existing_Sofia','Sofia_Catalogue','Tirshaker']
+    possible_stages = ['Fit_Tirific_OSC','Create_FAT_Cube',\
+        'Run_Sofia','Restart_Fitting','External_Sofia','Sofia_Catalogue',\
+        'Tirshaker','Fit_Make_Your_Own']
     possible_stages_l = [x.lower() for x in possible_stages]
     approved_stages = []
     fit_count = 0
     for stage in Configuration['FITTING_STAGES']:
         while stage.lower() not in possible_stages_l:
             stage = input(f'''
 The stage {stage} is not supported by FAT.
@@ -2852,29 +3710,30 @@
 : ''')
 
         if 'fit_' in stage.lower():
             fit_count += 1
             if fit_count == 1:
                 Configuration['USED_FITTING'] = possible_stages[possible_stages_l.index(stage.lower())]
 
+
         if fit_count > 1 and 'fit_' in stage.lower():
             print(f''' FAT only supports one single fitting stage. You have already selected one and hence {stage} will be ignored.
     ''')
         else:
             approved_stages.append(stage.lower())
 
     Configuration['FITTING_STAGES'] =approved_stages
-    if 'sofia_catalogue' in Configuration['FITTING_STAGES'] and 'existing_sofia' in Configuration['FITTING_STAGES']:
-        Configuration['FITTING_STAGES'].remove('existing_sofia')
-    if ('sofia_catalogue' in Configuration['FITTING_STAGES'] or 'existing_sofia' in Configuration['FITTING_STAGES']) and 'run_sofia' in Configuration['FITTING_STAGES']:
+    if 'sofia_catalogue' in Configuration['FITTING_STAGES'] and 'external_sofia' in Configuration['FITTING_STAGES']:
+        Configuration['FITTING_STAGES'].remove('external_sofia')
+    if ('sofia_catalogue' in Configuration['FITTING_STAGES'] or 'external_sofia' in Configuration['FITTING_STAGES']) and 'run_sofia' in Configuration['FITTING_STAGES']:
         Configuration['FITTING_STAGES'].remove('run_sofia')
     if 'sofia_catalogue' in Configuration['FITTING_STAGES'] and 'create_fat_cube' in Configuration['FITTING_STAGES']:
         Configuration['FITTING_STAGES'].remove('create_fat_cube')
 
-    if 'run_sofia' in Configuration['FITTING_STAGES'] and 'existing_sofia' in Configuration['FITTING_STAGES']:
+    if 'run_sofia' in Configuration['FITTING_STAGES'] and 'external_sofia' in Configuration['FITTING_STAGES']:
         raise InputError(f"You are both providing existing sofia input and ask for sofia to be ran. This won't work exiting.")
 
     #Check that the channel_dependency is acceptable
     while Configuration['CHANNEL_DEPENDENCY'].lower() not in ['sinusoidal','independent','hanning']:
         Configuration['CHANNEL_DEPENDENCY'] = input(f'''
 The channel dependency  {'CHANNEL_DEPENDENCY'} is not supported by FAT.
 Please pick one of the following {', '.join(['sinusoidal','independent','hanning'])}.
@@ -2888,15 +3747,16 @@
             check_dir = '/'.join(output_catalogue_dir[:-1])
             while not os.path.isdir(check_dir):
                 check_dir= input(f'''
                         The directory for your output catalogue ({Configuration['OUTPUT_CATALOGUE']}) does not exist.
                         Please provide the correct directory name.
                         ''')
                 Configuration['OUTPUT_CATALOGUE'] = f"{check_dir}/{output_catalogue_dir[-1]}"
-
+        elif len(output_catalogue_dir) == 1:
+            Configuration['OUTPUT_CATALOGUE'] = f"{Configuration['MAIN_DIRECTORY']}{Configuration['OUTPUT_CATALOGUE']}"
 
     if Configuration['RING_SIZE'] < 0.5:
         Configuration['RING_SIZE'] = 0.5
     if Configuration['OUTPUT_QUANTITY'] == 5:
         Configuration['OUTPUT_QUANTITY'] = 4
     if Configuration['SHAKER_ITERATIONS'] < 2:
         Configuration['SHAKER_ITERATIONS'] = 2
@@ -2912,15 +3772,15 @@
  CATEGORY:
     support_functions
 
  INPUTS:
     cfg = OmegaConf input object
 
  OPTIONAL INPUTS:
-    debug = False
+
     fit_type = 'Undefined'
 
  OUTPUTS:
     Configuration = dictionary with the config file input
 
  OPTIONAL OUTPUTS:
 
@@ -2928,69 +3788,71 @@
     Unspecified
 
  NOTE: Only this function can add entries to Original_Configuration or Configuration
 '''
 
 
 
-def sbr_limits(Configuration, systemic= 100. , debug = False):
-    radii = set_rings(Configuration,debug=debug)
-    if debug:
-        print_log(f'''SBR_LIMITS: Got {len(radii)} radii
-''',Configuration['OUTPUTLOG'], debug=True)
+def sbr_limits(Configuration, Tirific_Template ):
+    radii = set_rings(Configuration )
+    print_log(f'''SBR_LIMITS: Got {len(radii)} radii
+''',Configuration, case=['debug_start'])
     level = Configuration['NOISE']*1000
-    noise_in_column = columndensity(Configuration,level,systemic = systemic)
+    noise_in_column = columndensity(Configuration,level,systemic = \
+        float(load_tirific(Configuration,Tirific_Template,Variables=['VSYS'] )[0]))
     J2007col=9.61097e+19
+    #J2007scl= 2. #arcsec in a sech^2 layer
     ratio=(noise_in_column/J2007col)**0.5
+    #*np.sqrt(J2007scl/scaleheight)
     beamsolid=(np.pi*Configuration['BEAM'][0]*Configuration['BEAM'][1])/(4.*np.log(2.))
     ringarea= [0 if radii[0] == 0 else np.pi*((radii[0]+radii[1])/2.)**2]
     ringarea = np.hstack((ringarea,
                          [np.pi*(((y+z)/2.)**2-((y+x)/2.)**2) for x,y,z in zip(radii,radii[1:],radii[2:])],
                          [np.pi*((radii[-1]+0.5*(radii[-1]-radii[-2]))**2-((radii[-1]+radii[-2])/2.)**2)]
                          ))
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         sbr_ring_limits=9e-4*(ringarea/beamsolid)**(-0.82)*ratio
     if ringarea[0] == 0.:
          sbr_ring_limits[0]=np.nanmin(sbr_ring_limits)
          sbr_ring_limits[1]=sbr_ring_limits[2]/2.
+    print_log(f'''SBR_LIMITS: Applying the modifiier:
+{'':8s}{Configuration['LIMIT_MODIFIER']}
+''',Configuration,case=['debug_add'])
     if len(Configuration['LIMIT_MODIFIER']) == 1:
-
-        sbr_ring_limits= sbr_ring_limits*Configuration['LIMIT_MODIFIER']
+        sbr_ring_limits= sbr_ring_limits*float(Configuration['LIMIT_MODIFIER'][0])
     else:
         mod_list = list(Configuration['LIMIT_MODIFIER'])
         while len(mod_list) < len(sbr_ring_limits):
             mod_list.append(Configuration['LIMIT_MODIFIER'][-1])
         Configuration['LIMIT_MODIFIER'] = np.array(mod_list,dtype=float)
         sbr_ring_limits=[x*y for x,y in zip(sbr_ring_limits,Configuration['LIMIT_MODIFIER'])]
-    if debug:
-        print_log(f'''SBR_LIMITS: Retrieved these radii and limits:
+    print_log(f'''SBR_LIMITS: Retrieved these radii and limits:
 {'':8s}{radii}
 {'':8s}{sbr_ring_limits}
-''',Configuration['OUTPUTLOG'])
+''',Configuration,case=['debug_add'])
     return radii,sbr_ring_limits
 
 sbr_limits.__doc__ =f'''
  NAME:
     sbr_limits
 
  PURPOSE:
     Calculate the sbr limits below which rings can not be trusted.
 
  CATEGORY:
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
+    Tirific_Template = Standard Tirific template
+
 
  OPTIONAL INPUTS:
-    debug = False
 
-    systemic= 100.
-    systemic velocity
 
  OUTPUTS:
     radii = the radii of the rings in arcsec
     sbr_ring_limits = the limits of reliability for each ring based on the noise in the cube in Jy/arcsec^2 x km/s
 
  OPTIONAL OUTPUTS:
 
@@ -3032,66 +3894,90 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 #simple function keep track of how to modify the edge limits
-def set_limit_modifier(Configuration,Inclination, debug= False):
-    if debug:
-        print_log(f'''SET_LIMIT_MODIFIER: Checking the limit modifier.
-''', Configuration['OUTPUTLOG'], debug=True)
-    if not Inclination.shape:
-        Inclination = [Inclination]
+def set_limit_modifier(Configuration,Tirific_Template):
+    '''Write to the Configuration a value or list of values to modify sbr dependent values.'''
+    Profiles = load_tirific(Configuration,Tirific_Template,
+        Variables=['INCL','INCL_2','Z0','Z0_2'],array=True )
+    Inclination = [np.mean([x,y]) for x,y in zip(Profiles[0],Profiles[1])]
+    Z0_av = [np.mean([x,y]) for x,y in zip(Profiles[2],Profiles[3])]
+    kpc_radius=convertskyangle(Configuration,load_tirific(Configuration,\
+        Tirific_Template,['RADI'] ))
     modifier_list = []
+    # This should be per kpc
+    if len(Inclination) > 1:
+        if np.abs(Inclination[-1]-Inclination[-2])/(kpc_radius[-1]-kpc_radius[-2]) > Configuration['MAX_CHANGE']['INCL']:
+            Inclination[-1] = Inclination[-2]
     # Correction because the noise applies to non-face on rings while the SBR is face on,correction is normalized to the average inclination
     # The square root is because of the square root between the noise in cube and the noise in J2007
     # The lower limit corresponds to a inclination 80 above which the cos becomes too steep
-    for inc in Inclination:
+    for i,inc in enumerate(Inclination):
         if inc > 90.:
             inc  = 180.-inc
         if inc < 0.:
             inc= abs(inc)
-        modifier_list.append(set_limits(np.sqrt(np.cos(np.radians(inc))/np.cos(np.radians(60.))),0.75,2.))
+        if i < 10.:
+            modifier_list.append(set_limits(np.sqrt(np.cos(np.radians(inc))/np.cos(np.radians(60.))),0.75,2.))
+        else:
+            modifier_list.append(set_limits(np.sqrt(np.cos(np.radians(inc))/np.cos(np.radians(60.)))*i/10.,0.8,1.75))
+
     if Configuration['OUTER_RINGS_DOUBLED']:
         if len(modifier_list) > 10:
             modifier_list[10:]= np.sqrt(modifier_list[10:])
+    #We also need a correction based on Z0
+    #Get the avergae scaleheight for each ring
+    Z0_av,modifier_list = make_equal_length(Z0_av,modifier_list)
+    Z0_kpc = convertskyangle(Configuration,Z0_av)
+
+    if not isiterable(Z0_kpc):
+        Z0_kpc = [Z0_kpc]
+    #Scale the limits with the deviation away from 0.2 kpc as this is more or less the unmodified scale height
+
+    modifier_list=[set_limits(x*(1.125-0.625*y)*set_limits(((Configuration['RING_SIZE']*Configuration['BEAM'][0])/45.)**0.25,0.75,1.25),0.5,3.) for x,y in zip(modifier_list,Z0_kpc)]
+
     Configuration['LIMIT_MODIFIER'] = np.array(modifier_list,dtype=float)
-    print_log(f'''SET_LIMIT_MODIFIER: We updated the LIMIT_MODIFIER to {Configuration['LIMIT_MODIFIER']}.
-''', Configuration['OUTPUTLOG'])
+    print_log(f'''SET_LIMIT_MODIFIER: Based on a Z0 in kpc {Z0_kpc}
+{'':8s} and Inclination = {Inclination}
+{'':8s} We updated the LIMIT_MODIFIER to {Configuration['LIMIT_MODIFIER']}.
+''', Configuration,case=['debug_start'])
+
 
 set_limit_modifier.__doc__ =f'''
  NAME:
     set_limit_modifier
 
  PURPOSE:
-    Write to the Configuration a value or list of values to modify inclination dependent values. Foremost the sbr_limits
+    Write to the Configuration a value or list of values to modify sbr dependent values. Foremost the sbr_limits
 
  CATEGORY:
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
-    Inclination = Inclination of the model, can be singular or for all rings.
+    Tirific_Template = Standard Tirific template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     'LIMIT_MODIFIER' is updated in the Configuration.
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def set_limits(value,minv,maxv,debug = False):
+def set_limits(value,minv,maxv):
     if value < minv:
         return minv
     elif value > maxv:
         return maxv
     else:
         return value
 
@@ -3105,74 +3991,76 @@
 
  INPUTS:
     value = value to evaluate
     minv = minimum acceptable value
     maxv = maximum allowed value
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     the limited Value
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
-
-def set_ring_size(Configuration, debug = False, size_in_beams = 0., check_set_rings = False):
+def set_ring_size(Configuration,requested_ring_size = 0., size_in_beams = 0., check_set_rings = False):
+    double_size = False
     if size_in_beams == 0.:
-        size_in_beams =  Configuration['SIZE_IN_BEAMS']
-    ring_size = Configuration['RING_SIZE']
-    no_rings = calc_rings(Configuration,ring_size=ring_size,size_in_beams=size_in_beams,debug=debug)
-    if debug:
-        print_log(f'''SET_RING_SIZE: Starting with the following parameters.
-{'':8s}SIZE_IN_BEAMS = {size_in_beams}
-{'':8s}RING_SIZE = {ring_size}
-''', Configuration['OUTPUTLOG'],debug=True)
+        size_in_beams =  np.min(Configuration['SIZE_IN_BEAMS'])
+        double_size=True
+    if requested_ring_size == 0.:
+         requested_ring_size =  Configuration['RING_SIZE']
+
+    print_log(f'''SET_RING_SIZE: Starting with the following parameters.
+{'':8s}size in beams = {size_in_beams}
+{'':8s}requested ring size = {requested_ring_size}
+''', Configuration,case=['debug_start'])
+    if not Configuration['FIX_RING_SIZE']:
+        no_rings = 0.
+        ring_size = 100.
+        while (requested_ring_size > 0.5 and no_rings < Configuration['MINIMUM_RINGS']) or no_rings == 0.:
+
+            est_rings = set_limits(round((size_in_beams-1./5.)/(requested_ring_size)),8.,float('NaN'))
+
+            ring_size = set_limits((size_in_beams-1./5.)/est_rings,0.5,float('NaN') )
+
+            no_rings = calc_rings(Configuration,ring_size=ring_size,size_in_beams=size_in_beams )
+
+            if no_rings < Configuration['MINIMUM_RINGS'] and requested_ring_size > 0.5:
+                previous_ringsize = copy.deepcopy(requested_ring_size)
+                requested_ring_size = set_limits(requested_ring_size/1.25,0.5,float('NaN') )
+                print_log(f'''SET_RING_SIZE: Because we had less than {Configuration['MINIMUM_RINGS']} rings we have reduced the requested ring size from {previous_ringsize} to {requested_ring_size}
+    ''',Configuration)
+
+        if double_size:
+            # we had two values in the size_in beams we get the number of rings from the maximum
+            #As we used the minimum to calate the ring size we need to recalculated the number of rings
+            no_rings = calc_rings(Configuration,ring_size=ring_size,size_in_beams=np.max(Configuration['SIZE_IN_BEAMS']) )
+    else:
+        ring_size = requested_ring_size
+        no_rings = calc_rings(Configuration,ring_size=ring_size,size_in_beams=np.max(Configuration['SIZE_IN_BEAMS']) )
 
-    while ring_size > 0.5 and  no_rings < 8.:
-        previous_ringsize = ring_size
-        ring_size = set_limits(ring_size/1.5,0.5,float('NaN'),debug=debug)
-        no_rings = calc_rings(Configuration,ring_size=ring_size,size_in_beams=size_in_beams,debug=debug)
-        print_log(f'''SET_RING_SIZE: Because we had less than four rings we have reduced the ring size from {previous_ringsize} to {ring_size}
-''',Configuration['OUTPUTLOG'])
-
-    while no_rings < Configuration['MINIMUM_RINGS'] and not size_in_beams >=  Configuration['MAX_SIZE_IN_BEAMS']:
-        size_in_beams = set_limits(size_in_beams+1.*ring_size,1, Configuration['MAX_SIZE_IN_BEAMS'])
-        no_rings = calc_rings(Configuration,ring_size=ring_size,size_in_beams=size_in_beams,debug=debug)
-        print_log(f'''SET_RING_SIZE: The initial estimate is too small to fit adding a ring to it.
-''',Configuration['OUTPUTLOG'])
-
-    if check_set_rings:
-        if debug:
-            print_log(f'''SET_RING_SIZE: Setting the following parameters.
-{'':8s}SIZE_IN_BEAMS = {size_in_beams}
-{'':8s}RING_SIZE = {ring_size}
-{'':8s}NO_RINGS = {no_rings}
-''', Configuration['OUTPUTLOG'])
-        return size_in_beams,ring_size,int(no_rings)
-    else:
-        if debug:
-            print_log(f'''SET_RING_SIZE: Setting the following parameters.
-{'':8s}SIZE_IN_BEAMS = {size_in_beams}
-{'':8s}RING_SIZE = {ring_size}
-{'':8s}NO_RINGS = {no_rings}
-''', Configuration['OUTPUTLOG'])
+    print_log(f'''SET_RING_SIZE: After checking the size we get
+{'':8s}size in beams = {size_in_beams}, ring size = {ring_size} and the number of ring = {no_rings}
+''', Configuration,case=['debug_add'])
+
+    if not check_set_rings:
+        if no_rings <  Configuration['MINIMUM_RINGS']:
+            print_log(f'''SET_RING_SIZE: With a ring size of {ring_size} we still only find {no_rings}.
+{"":8s}SET_RING_SIZE: This is not enough for a fit.
+''',Configuration,case=['main','screen'])
+            raise SmallSourceError('This source is too small to reliably fit.')
         Configuration['NO_RINGS'] = int(no_rings)
-        Configuration['SIZE_IN_BEAMS'] = size_in_beams
         Configuration['RING_SIZE'] = ring_size
-        if Configuration['NO_RINGS'] < Configuration['MINIMUM_RINGS']:
-            print_log(f'''SET_RING_SIZE: With a ring size of {Configuration['RING_SIZE']} we still only find {Configuration['NO_RINGS']}.
-    {"":8s}SET_RING_SIZE: This is not enough for a fit.
-    ''',Configuration['OUTPUTLOG'],screen=True)
-            raise SmallSourceError('This source is too small to reliably fit.')
+    return ring_size,int(no_rings)
 
 set_ring_size.__doc__ =f'''
  NAME:
     set_ring_size
 
  PURPOSE:
     Calculate the size and number of rings and the galaxy size in beams and update them in the Configuration dictionary
@@ -3180,15 +4068,15 @@
  CATEGORY:
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     size_in_beams = 0.
     The size of the galaxy in beams across the major axis radius, if unset it is taken from the Configuration
 
     check_set_rings = False
     Set this parameter to True to not apply the calaculated ring size and number and size of the model to the
     Configuration but to return the parameters as  size_in_beams,ring_size,no_rings
@@ -3201,53 +4089,51 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def set_rings(Configuration,ring_size = 0. , debug = False):
+def set_rings(Configuration,ring_size = 0. ):
     if ring_size == 0.:
         ring_size = Configuration['RING_SIZE']
-    if debug:
-        print_log(f'''SET_RINGS: Starting with the following parameters.
+    print_log(f'''SET_RINGS: Starting with the following parameters.
 {'':8s}RING_SIZE = {ring_size}
-''', Configuration['OUTPUTLOG'],debug=True)
-    no_rings = calc_rings(Configuration,debug=debug)
-    if debug:
-        print_log(f'''SET_RINGS: We find {no_rings} rings.
-''', Configuration['OUTPUTLOG'])
+''', Configuration, case=['debug_start'])
+    no_rings = calc_rings(Configuration )
+    print_log(f'''SET_RINGS: We find {no_rings} rings.
+''', Configuration, case=['debug_add'])
     if Configuration['OUTER_RINGS_DOUBLED']:
         print_log(f'''SET_RINGS: This is a large galaxy. Therefore we use twice the ring size in the outer parts.
-''',Configuration['OUTPUTLOG'],screen =True)
+''',Configuration,case=['verbose'])
         radii = [0.,1./5.*Configuration['BEAM'][0]]
         radii = np.hstack((radii,(np.linspace(Configuration['BEAM'][0]*ring_size,Configuration['BEAM'][0]*10.*ring_size, \
                                         10)+1./5*Configuration['BEAM'][0])))
         radii = np.hstack((radii,(np.linspace(Configuration['BEAM'][0]*12.*ring_size, \
                                               Configuration['BEAM'][0]*ring_size*(10+(no_rings-12.)*2.), \
                                               no_rings-12)) \
                                               +1./5*Configuration['BEAM'][0]))
 
     else:
         radii = [0.,1./5.*Configuration['BEAM'][0]]
         radii = np.hstack((radii,(np.linspace(Configuration['BEAM'][0]*ring_size,Configuration['BEAM'][0]*ring_size*(no_rings-2.), \
                                         no_rings-2)+1./5.*Configuration['BEAM'][0])))
-    if debug:
+    if Configuration['DEBUG']:
         if Configuration['OUTER_RINGS_DOUBLED']:
             req_outer_ring = 2.*Configuration['BEAM'][0]*ring_size
         else:
             req_outer_ring = Configuration['BEAM'][0]*ring_size
         print_log(f'''SET_RINGS: Got the following radii.
 {'':8s}{radii}
 {'':8s}We should have {Configuration['NO_RINGS']} or we incorrectly updated and should have {no_rings}
 {'':8s}We have {len(radii)} rings.
-{'':8s}The last ring should be around {Configuration['BEAM'][0]*Configuration['SIZE_IN_BEAMS']}
+{'':8s}The last ring should be around {Configuration['BEAM'][0]*np.max(Configuration['SIZE_IN_BEAMS'])}
 {'':8s}The rings should be size {Configuration['BEAM'][0]*ring_size} and outer rings {req_outer_ring}
-{'':8s}They are {radii[3]-radii[2]} and {radii[-1]-radii[-2]}
-''', Configuration['OUTPUTLOG'])
+{'':8s}They are {radii[2]-radii[1]} and {radii[-1]-radii[-2]}
+''', Configuration, case=['debug_add'])
     return np.array(radii,dtype = float)
 
 set_rings.__doc__ =f'''
  NAME:
     set_rings
  PURPOSE:
     Calculate the radii of all rings required for the model
@@ -3255,15 +4141,15 @@
  CATEGORY:
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     ring_size = 0.
     Width of the rings
 
  OUTPUTS:
     numpy array with the central locations of the rings in arcsec.
 
@@ -3303,30 +4189,29 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def sofia_output_exists(Configuration,Fits_Files, debug = False):
-    if debug:
-        print_log(f'''SOFIA_OUTPUT_EXISTS: Starting check
-''', Configuration['OUTPUTLOG'],debug = True)
+def sofia_output_exists(Configuration,Fits_Files):
+    print_log(f'''SOFIA_OUTPUT_EXISTS: Starting check
+''', Configuration, case=['debug_start'])
     req_files= ['MOMENT1','MOMENT0','MASK']
     for file in req_files:
-        if os.path.exists(Configuration['FITTING_DIR']+'Sofia_Output/'+Fits_Files[file]):
+        if os.path.exists(f"{Configuration['FITTING_DIR']}{Fits_Files[file]}"):
             continue
         else:
-            log_statement = f"SOFIA_OUTPUT_EXISTS: The file {Configuration['FITTING_DIR']+'Sofia_Output/'+Fits_Files[file]} is not found."
-            print_log(log_statement, Configuration['OUTPUTLOG'],screen =True)
+            log_statement=f'''SOFIA_OUTPUT_EXISTS: The file {Configuration['FITTING_DIR']}{Fits_Files[file]} is not found.'''
+            print_log(log_statement, Configuration,case=['main','screen'])
             raise FileNotFoundError(log_statement)
 
     if not os.path.exists(Configuration['FITTING_DIR']+'Sofia_Output/'+Configuration['BASE_NAME']+'_cat.txt'):
-        log_statement = f"SOFIA_OUTPUT_EXISTS: The file {Configuration['FITTING_DIR']+'Sofia_Output/'+Configuration['BASE_NAME']+'_cat.txt'} is not found."
-        print_log(log_statement, Configuration['OUTPUTLOG'],screen =True)
+        log_statement=f'''SOFIA_OUTPUT_EXISTS: The file {Configuration['FITTING_DIR']+'Sofia_Output/'+Configuration['BASE_NAME']+'_cat.txt'} is not found.'''
+        print_log(log_statement, Configuration,case=['main','screen'])
         raise FileNotFoundError(log_statement)
 
 sofia_output_exists.__doc__ =f'''
  NAME:
 
  PURPOSE:
     Simple function to make sure all sofia output is present as expected
@@ -3334,36 +4219,136 @@
     support_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     Raises a FileNotFoundError if the files are not found.
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def update_statistic(Configuration,process= None,message = None ,debug=False):
+def tirific_template(filename = ''):
+    if filename == '':
+        with pack_open_txt(templates, 'template.def') as tmp:
+            template = tmp.readlines()
+    elif filename == 'Installation_Check':
+        from pyFAT_astro import Installation_Check as IC
+        with pack_open_txt(IC, 'ModelInput.def') as tmp:
+            template = tmp.readlines()
+    else:
+        with open(filename, 'r') as tmp:
+            template = tmp.readlines()
+    result = Proper_Dictionary()
+    counter = 0
+    # Separate the keyword names
+    for line in template:
+        key = str(line.split('=')[0].strip().upper())
+        if key == '':
+            result[f'EMPTY{counter}'] = line
+            counter += 1
+        else:
+            result[key] = str(line.split('=')[1].strip())
+    return result
+tirific_template.__doc__ ='''
+ NAME:
+    tirific_template
+
+ PURPOSE:
+    Read a tirific def file into a dictionary to use as a template.
+    The parameter ill be the dictionary key with the values stored in that key
+
+ CATEGORY:
+    read_functions
+
+ INPUTS:
+    filename = Name of the def file
+
+ OPTIONAL INPUTS:
+    filename = ''
+    Name of the def file, if unset the def file in Templates is used
+
+
+
+ OUTPUTS:
+    result = dictionary with the read file
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+      split, strip, open
+
+ NOTE:
+'''
+
+def update_statistic(Configuration,process= None,message = None ):
     if Configuration['TIMING']:
-        function,variable,empty = traceback.format_stack()[-2].split('\n')
-        function = function.split()[-1].strip()
+        function = traceback.format_stack()[-2].split('\n')
+        function = function[0].split()[-1].strip()
         if not process:
             process = Configuration['FAT_PSUPROCESS']
             program = 'pyFAT'
         else:
             program = 'TiRiFiC'
 
         CPU,mem = get_usage_statistics(Configuration,process)
         with open(f"{Configuration['LOG_DIRECTORY']}Usage_Statistics.txt",'a') as file:
             if message:
                 file.write(f"# {function.upper()}: {message} at {datetime.now()} \n")
             # We cannot copy the process so initialize in the configuration
             file.write(f"{datetime.now()} CPU = {CPU} % Mem = {mem} Mb for {program} \n")
+
+def write_config(file,Configuration ):
+    #be clear we are pickle dumping
+    tmp = os.path.splitext(file)
+    file = f'{tmp[0]}.pkl'
+    print_log(f'''WRITE_CONFIG: writing the configuration to {file}
+''',Configuration,case=['debug_start'])
+    # Separate the keyword names
+    #Proper dictionaries are not pickable
+
+    Pick_Configuration = {}
+    for key in Configuration:
+        Pick_Configuration[key] = Configuration[key]
+        if key == 'FAT_PSUPROCESS':
+            Pick_Configuration[key] = None
+    import pickle
+    with open(file,'wb') as tmp:
+        pickle.dump(Pick_Configuration,tmp)
+
+
+write_config.__doc__ =f'''
+ NAME:
+    write_config
+
+ PURPOSE:
+    Write a config file to the fitting directory.
+
+ CATEGORY:
+    write_functions
+
+ INPUTS:
+    file = name of the file to write to
+    Configuration = Standard FAT configuration
+
+ OPTIONAL INPUTS:
+
+
+ OUTPUTS:
+    A FAT config file.
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE: This doesn't work in python 3.6
+'''
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/Support/tirshaker.py` & `pyFAT_astro-0.1.1/pyFAT_astro/Support/tirshaker.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,24 +14,25 @@
 import matplotlib as mpl
 import astropy.units as u
 import astropy.constants as c
 import scipy.special as spec
 from scipy.optimize import least_squares
 from matplotlib import colors as mplcolors
 from scipy import stats
-from pyFAT_astro.Support.support_functions import run_tirific,print_log,set_format,finish_current_run
+
 from pyFAT_astro.Support.write_functions import tirific as write_tirific
-from pyFAT_astro.Support.read_functions import load_tirific
+import pyFAT_astro.Support.support_functions as sf
+import pyFAT_astro
 
 #
 #tirshaker
 def tirshaker(Configuration, Tirific_Template, outfilename = 'test_out.def', \
               outfileprefix = 'tirsh_', parameter_groups = [], rings = [], block = []\
               , variation = [], variation_type = [], iterations = 0, random_seed = 0,\
-               mode = 'mad',debug=False,fit_type='Error_Shaker'):
+               mode = 'mad',fit_type='Error_Shaker'):
     # Initiate rng
     random.seed(random_seed)
 
     # Find the number of lines
     nur = int(Tirific_Template['NUR'])
 
 
@@ -65,25 +66,27 @@
         Tirific_Template['INIMODE'] = 2
     else:
         Tirific_Template['INIMODE'] = 3
 
     Tirific_Template['LOGNAME'] = 'Error_Shaker.log'
     Tirific_Template['TIRDEF'] = 'Error_Shaker_Out.def'
     current_run='not set'
+    original_running = copy.deepcopy(Configuration['TIRIFIC_RUNNING'])
+    Configuration['TIRIFIC_RUNNING'] = False
     for i in range(iterations):
         Current_Template = copy.deepcopy(Tirific_Template)
         Current_Template['RESTARTID']= i
         # Provide some info where we are
-        print_log(f'''
+        sf.print_log(f'''
         ******************************
         ******************************
         *** Tirshaker iteration {i:02d} ***
         ******************************
         ******************************
-''',Configuration['OUTPUTLOG'],screen=True)
+''',Configuration)
 
     #fortestin
     #    break
 
         # Find a name for a logfile and an output.def file
         #inname = 'blatirshin'
         #while os.path.exists(inname):
@@ -110,34 +113,37 @@
                 while len(current_list) < nur:
                     current_list.append(current_list[-1])
                 for l in range(len(rings[j])):
                     if variation_type[j] == 'a':
                         current_list[rings[j][l]-1] = current_list[rings[j][l]-1]+variations[l]
                     else:
                         current_list[rings[j][l]-1] = current_list[rings[j][l]-1]*(1.+variations[l])
-                format = set_format(parameter_groups[j][k])
+                format = sf.set_format(parameter_groups[j][k])
                 Current_Template[parameter_groups[j][k]] = ' '.join([f'{x:{format}}' for x in current_list])
 
 
 
         #Current_Template['LOGNAME'] = logname
         #Current_Template['TIRDEF'] = defname
 
-        write_tirific(Configuration,Current_Template, name =f'Error_Shaker/{fit_type}_In.def' , debug = debug)
-        accepted,current_run = run_tirific(Configuration, current_run, stage = 'shaker',fit_type = fit_type, debug = debug)
+        write_tirific(Configuration,Current_Template, name =f'Error_Shaker/{fit_type}_In.def' )
+        accepted,current_run = sf.run_tirific(Configuration, current_run, stage = 'shaker',fit_type = fit_type)
         #os.system('tirific deffile= '+inname)
 
         # Read the values of the parameters requested
 
         allnumbers_out_part = []
         for j in range(len(parameter_groups)):
             numbers = []
             # Then go through the parameter_groups
             for k in range(len(parameter_groups[j])):
-                numbers.append([float(x) for x in load_tirific(Configuration,f"{Configuration['FITTING_DIR']}Error_Shaker/Error_Shaker_Out.def",Variables = [parameter_groups[j][k]],debug=debug)[0]])
+                numbers.append([float(x) for x in \
+                    sf.load_tirific(Configuration,\
+                        f"{Configuration['FITTING_DIR']}Error_Shaker/Error_Shaker_Out.def",\
+                        Variables = [parameter_groups[j][k]],array=True)[0]])
                 if parameter_groups[j][k] == 'CONDISP':
                     pass
                 else:
                     while len(numbers[-1]) < nur:
                         numbers[-1].append(numbers[-1][-1])
 
             allnumbers_out_part.append(numbers)
@@ -193,38 +199,41 @@
                     average = np.average(np.array(allparamsturned[j][k][l]))
                     # Wow, np.std is the standard deviation using N and not N-1 in the denominator. So one has to use
                     std = np.sqrt(float(len(allparamsturned[j][k][l]))/float(len(allparamsturned[j][k][l])-1))*np.std(np.array(allparamsturned[j][k][l]))
                     allnumbers_final[j][k].append(stats.tmean(np.array(allparamsturned[j][k][l]), (median-3*madsigma, median+3*madsigma)))
                     allnumbers_final_err[j][k].append(stats.tstd(np.array(allparamsturned[j][k][l]), (median-3*madsigma, median+3*madsigma)))
                     #allnumbers_final[j][k].append(stats.tmean(np.array(allparamsturned[j][k][l])))
                     #allnumbers_final_err[j][k].append(stats.tstd(np.array(allparamsturned[j][k][l])))
-                    print_log('TIRSHAKER: Parameter: {:s} Ring: {:d} Pure average+-std: {:.3e}+-{:.3e} Median+-madsigma: {:.3e}+-{:.3e} Average+-sigma filtered: {:.3e}+-{:.3e} \n'.format(\
+                    sf.print_log('TIRSHAKER: Parameter: {:s} Ring: {:d} Pure average+-std: {:.3e}+-{:.3e} Median+-madsigma: {:.3e}+-{:.3e} Average+-sigma filtered: {:.3e}+-{:.3e} \n'.format(\
                                 parameter_groups[j][k], l+1, average, std, median, madsigma, allnumbers_final[j][k][-1], allnumbers_final_err[j][k][-1])\
-                                ,Configuration['OUTPUTLOG'],screen=False)
+                                ,Configuration)
                 else:
                     allnumbers_final[j][k].append(np.average(np.array(allparamsturned[j][k][l])))
                     allnumbers_final_err[j][k].append(np.sqrt(float(len(allparamsturned[j][k][l]))/float(len(allparamsturned[j][k][l])-1))*np.std(np.array(allparamsturned[j][k][l])))
     #print 'allnumbers_final'
     #print allnumbers_final
     #print 'allnumbers_final_err'
     #print allnumbers_final_err
 
 
     for j in range(len(parameter_groups)):
         for k in range(len(parameter_groups[j])):
-            format = set_format(parameter_groups[j][k])
+            format = sf.set_format(parameter_groups[j][k])
             #Tirific_Template[parameter_groups[j][k]] = ' '.join([f'{x:{format}}' for x in allnumbers_final[j][k]])
             Tirific_Template.insert(f'{parameter_groups[j][k]}',f'# {parameter_groups[j][k]}_ERR',f"{' '.join([f'{x:{format}}' for x in allnumbers_final_err[j][k]])}")
 
             #Tirific_Template.insert(f'{parameter_groups[j][k]}',f'# {parameter_groups[j][k]}_ERR',' '.join([f'{x:{format}}' for x in allnumbers_final_err[j][k]]))
 
     # Put them into the output file
     # Write it to a copy of the file replacing the parameters
-    finish_current_run(Configuration, current_run)
-    write_tirific(Configuration,Tirific_Template, name =f'Error_Shaker/{outfilename}' , debug = debug)
+
+
+    sf.finish_current_run(Configuration, current_run)
+    write_tirific(Configuration,Tirific_Template, name =f'Error_Shaker/{outfilename}' )
+    Configuration['TIRIFIC_RUNNING'] = original_running
 
 tirshaker.__doc__ =f'''
  NAME:
     tirshaker
 
  PURPOSE:
     obtain errors through a FAT implemention of tirshaker developed by G.I.G. Jozsa.
@@ -241,15 +250,14 @@
     variation (list of float)              : Amplitude of variation
     variation_type (list of str)           : Type of variation, 'a' for absolute, 'r' for relative
     iterations (int)                       : Number of re-runs
     random_seed (int)                      : Seed for random generator
     mode (str)                             : If 'mad' implements an outlier rejection.
 
  OPTIONAL INPUTS:
-    debug = False
 
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/Support/write_functions.py` & `pyFAT_astro-0.1.1/pyFAT_astro/Support/write_functions.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,42 @@
 # -*- coding: future_fstrings -*-
 # This module contains a set of functions and classes that are used to write text files to Disk
 
-from pyFAT_astro.Support.support_functions import print_log,convertRADEC,convertskyangle,\
-                                set_limit_modifier,columndensity,set_limits,\
-                                get_inner_fix,linenumber
+
 from pyFAT_astro.Support.modify_template import set_model_parameters, set_overall_parameters,\
                                 set_fitting_parameters,get_warp_slope, update_disk_angles
 from pyFAT_astro.Support.fits_functions import extract_pv
-from pyFAT_astro.Support.read_functions import load_tirific,load_basicinfo, load_template
+from pyFAT_astro.Support.read_functions import load_basicinfo
 from pyFAT_astro.Support.fat_errors import ProgramError
+import pyFAT_astro.Support.support_functions as sf
+import pyFAT_astro
+
+
 import copy
 import numpy as np
+import psutil as psu
+import time
 import warnings
 from datetime import datetime
 import traceback
 import os
-from datetime import datetime
+
 with warnings.catch_warnings():
     warnings.simplefilter("ignore")
     import matplotlib
     matplotlib.use('pdf')
     import matplotlib.pyplot as plt
     from mpl_toolkits.axes_grid1 import make_axes_locatable
     from matplotlib.patches import Ellipse
     import matplotlib.axes as maxes
+    import matplotlib.font_manager as mpl_fm
 from astropy.io import fits
 from astropy.wcs import WCS
 # create or append to the basic ifo file
-def basicinfo(Configuration,initialize = False,stage='TiRiFiC', debug = False,
+def basicinfo(Configuration,initialize = False,stage='TiRiFiC' ,
               RA=[float('NaN'),float('NaN')], DEC=[float('NaN'),float('NaN')],
               VSYS =[float('NaN'),float('NaN')], PA=[float('NaN'),float('NaN')],
               Inclination = [float('NaN'),float('NaN')], Max_Vrot = [float('NaN'),float('NaN')],
               Tot_Flux = [float('NaN'),float('NaN')], V_mask = [float('NaN'),float('NaN')],
               Distance = float('NaN') , DHI = float('NaN'), template = ['EMPTY']):
 
     try:
@@ -46,38 +51,39 @@
 #D_HI is determined as the diameter where the major axis with given PA cuts the 10^20 column of the moment0 map
 # {'RA':>25s} {'DEC':>25s} {'VSYS':>20s} {'PA':>20s} {'Inclination':>20s} {'Max VRot':>20s} {'V_mask':>20s} {'Tot FLux':>20s} {'D_HI':>20s} {'Distance':>20s} {'HI Mass':>20s} {'D_HI_kpc':>20s}
 # {'hh:mm:ss':>25s} {'dd:mm:ss':>25s} {'km/s':>20s} {'deg':>20s} {'deg':>20s} {'km/s':>20s} {'km/s':>20s} {'Jy':>20s} {'arcsec':>20s} {'Mpc':>20s} {'M_solar':>20s} {'kpc':>20s}
 # The initial input
 ''')
     else:
         Vars_to_Set =  ['XPOS','YPOS','VSYS','VROT','INCL','PA','SDIS','SBR','SBR_2','Z0']
-        FAT_Model = load_template(Configuration,template,Variables= Vars_to_Set,unpack=False, debug=debug)
-        RA=[FAT_Model[0,Vars_to_Set.index('XPOS')],abs(Configuration['BEAM'][0]/(3600.*2.))]
-        DEC=[FAT_Model[0,Vars_to_Set.index('YPOS')],abs(Configuration['BEAM'][0]/(3600.*2.))]
-        VSYS =np.array([FAT_Model[0,Vars_to_Set.index('VSYS')],Configuration['CHANNEL_WIDTH']],dtype=float)
-        PA=[FAT_Model[0,Vars_to_Set.index('PA')], 3.]
-        Inclination = [FAT_Model[0,Vars_to_Set.index('INCL')], 3.]
-        Max_Vrot = [np.max(FAT_Model[:,Vars_to_Set.index('VROT')]),np.max(FAT_Model[:,Vars_to_Set.index('VROT')])-np.min(FAT_Model[1:,Vars_to_Set.index('VROT')]) ]
+        FAT_Model = sf.load_tirific(Configuration,template,\
+            Variables= Vars_to_Set,array=True )
+        RA=[FAT_Model[Vars_to_Set.index('XPOS'),0],abs(Configuration['BEAM'][0]/(3600.*2.))]
+        DEC=[FAT_Model[Vars_to_Set.index('YPOS'),0],abs(Configuration['BEAM'][0]/(3600.*2.))]
+        VSYS =np.array([FAT_Model[Vars_to_Set.index('VSYS'),0],Configuration['CHANNEL_WIDTH']],dtype=float)
+        PA=[FAT_Model[Vars_to_Set.index('PA'),0], 3.]
+        Inclination = [FAT_Model[Vars_to_Set.index('INCL'),0], 3.]
+        Max_Vrot = [np.max(FAT_Model[Vars_to_Set.index('VROT'),:]),np.max(FAT_Model[Vars_to_Set.index('VROT'),:])-np.min(FAT_Model[Vars_to_Set.index('VROT'),1:]) ]
         Distance = Configuration['DISTANCE']
 
     with open(f"{Configuration['FITTING_DIR']}{Configuration['BASE_NAME']}-Basic_Info.txt",'a') as file:
         if not initialize:
             file.write(f'''#These are the values from {stage}. \n''')
-        RAhr,DEChr = convertRADEC(Configuration,RA[0],DEC[0],debug=debug)
+        RAhr,DEChr = sf.convertRADEC(Configuration,RA[0],DEC[0] )
         RA_c = f'{RAhr}+/-{RA[1]*3600.:0.2f}'
         DEC_c = f'{DEChr}+/-{DEC[1]*3600.:0.2f}'
         VSYS_c = f'{VSYS[0]:.2f}+/-{VSYS[1]:.2f}'
         PA_c = f'{PA[0]:.2f}+/-{PA[1]:.2f}'
         INCL_c = f'{Inclination[0]:.2f}+/-{Inclination[1]:.2f}'
         MVROT_c = f'{Max_Vrot[0]:.2f}+/-{Max_Vrot[1]:.2f}'
         Vmask_c = f'{V_mask[0]/1000.:.2f}+/-{V_mask[1]/1000.:.2f}'
         DHI_a = f'{DHI[0]:.2f}+/-{DHI[1]:.2f}'
         Dist = f'{Distance:.2f}'
         HIMass  = f'{Tot_Flux[0]*2.36E5*Distance**2:.2e}'
-        DHI_k = f'{convertskyangle(Configuration,DHI[0],Distance):.2f}'
+        DHI_k = f'{sf.convertskyangle(Configuration,DHI[0]):.2f}'
         Flux_c = f'{Tot_Flux[0]:.2f}+/-{Tot_Flux[1]:.2f}'
         file.write(f'''  {RA_c:>25s} {DEC_c:>25s} {VSYS_c:>20s} {PA_c:>20s} {INCL_c:>20s} {MVROT_c:>20s} {Vmask_c:>20s} {Flux_c:>20s} {DHI_a:>20s} {Dist:>20s} {HIMass:>20s} {DHI_k:>20s}
 ''')
 
 basicinfo.__doc__ =f'''
  NAME:
     basicinfo
@@ -88,15 +94,15 @@
  CATEGORY:
     write_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     initialize = False
     If true a new file with header but and first guess values will be created.
     These parameters need to be provided through the keywords below.
 
     stage = 'Tirific'
 
@@ -136,62 +142,65 @@
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 # Function to write the first def file for a galaxy
-def initialize_def_file(Configuration, Fits_Files,Tirific_Template,Initial_Parameters = ['EMPTY'], fit_type = 'Undefined',debug = False):
+def initialize_def_file(Configuration, Fits_Files,Tirific_Template,Initial_Parameters = ['EMPTY'], fit_type = 'Undefined' ):
     try:
         if Initial_Parameters[0] == 'EMPTY':
             Initial_Parameters = {}
     except KeyError:
         pass
 
     #First we set some basic parameters that will hardly change
     if fit_type == 'Centre_Convergence':
 
-        if 'VSYS' in Initial_Parameters:
-            Initial_Parameters['VSYS'] = [x/1000. for x in Initial_Parameters['VSYS']]
-        set_overall_parameters(Configuration, Fits_Files,Tirific_Template,fit_type=fit_type, flux = Initial_Parameters['FLUX'][0], debug=debug)
+        #if 'VSYS' in Initial_Parameters:
+        #    Initial_Parameters['VSYS'] = [x/1000. for x in Initial_Parameters['VSYS']]
+        set_overall_parameters(Configuration, Fits_Files,Tirific_Template,\
+            fit_type=fit_type, flux = Initial_Parameters['FLUX'][0] )
         # Then set the values for the various parameters of the model
 
-        set_model_parameters(Configuration, Tirific_Template,Initial_Parameters, debug=debug)
+        set_model_parameters(Configuration, Tirific_Template,Initial_Parameters )
 
-        set_limit_modifier(Configuration,Initial_Parameters['INCL'][0], debug=debug )
+        sf.set_limit_modifier(Configuration,Tirific_Template  )
 
         set_fitting_parameters(Configuration, Tirific_Template,stage = 'initial',
-                                initial_estimates = Initial_Parameters, debug=debug)
-        if 'VSYS' in Initial_Parameters:
-            Initial_Parameters['VSYS'] = [x*1000. for x in Initial_Parameters['VSYS']]
+                                initial_estimates = Initial_Parameters )
+        #if 'VSYS' in Initial_Parameters:
+        #    Initial_Parameters['VSYS'] = [x*1000. for x in Initial_Parameters['VSYS']]
     elif fit_type in ['Extent_Convergence','Fit_Tirific_OSC']:
-        if 'VSYS' in Initial_Parameters and fit_type == 'Fit_Tirific_OSC':
-            Initial_Parameters['VSYS'] = [x/1000. for x in Initial_Parameters['VSYS']]
-        set_overall_parameters(Configuration, Fits_Files,Tirific_Template ,fit_type=fit_type, debug=debug,stage='initialize_ec')
+        #if 'VSYS' in Initial_Parameters and fit_type == 'Fit_Tirific_OSC':
+        #    Initial_Parameters['VSYS'] = [x/1000. for x in Initial_Parameters['VSYS']]
+        set_overall_parameters(Configuration, Fits_Files,Tirific_Template ,\
+            fit_type=fit_type)
         Vars_to_Set =  ['XPOS','YPOS','VSYS','VROT','INCL','PA','SDIS','SBR','SBR_2','Z0']
         if fit_type == 'Fit_Tirific_OSC':
-            set_model_parameters(Configuration, Tirific_Template,Initial_Parameters,stage='initialize_def_file', debug=debug)
-        FAT_Model = load_template(Configuration,Tirific_Template,Variables= Vars_to_Set,unpack=False, debug=debug)
+            set_model_parameters(Configuration, Tirific_Template,Initial_Parameters,stage='initialize_def_file' )
 
         # Finally we set how these parameters are fitted.
-        set_limit_modifier(Configuration,FAT_Model[0,Vars_to_Set.index('INCL')], debug=debug)
-        get_inner_fix(Configuration,Tirific_Template, debug=debug)
-        get_warp_slope(Configuration,Tirific_Template, debug=debug)
-
-        parameters = {'VSYS': [FAT_Model[0,Vars_to_Set.index('VSYS')], Configuration['CHANNEL_WIDTH']], \
-                      'XPOS': [FAT_Model[0,Vars_to_Set.index('XPOS')], Configuration['BEAM'][0]/3600.] ,
-                      'YPOS': [FAT_Model[0,Vars_to_Set.index('YPOS')], Configuration['BEAM'][0]/3600.],
-                      'INCL': [FAT_Model[0,Vars_to_Set.index('INCL')], 3.],
-                      'PA':  [FAT_Model[0,Vars_to_Set.index('PA')], 3.],
-                      'VROT':[np.mean(FAT_Model[:,Vars_to_Set.index('VROT')]),np.max(FAT_Model[:,Vars_to_Set.index('VROT')])-np.min(FAT_Model[1:,Vars_to_Set.index('VROT')]) ]  }
+        sf.set_limit_modifier(Configuration,Tirific_Template )
+        #get_inner_fix(Configuration,Tirific_Template )
+        get_warp_slope(Configuration,Tirific_Template )
+        #if Configuration['OUTER_RINGS_DOUBLED']:
+        Initial_Parameters['XPOS'][1]= sf.set_limits(Initial_Parameters['XPOS'][1],Configuration['BEAM'][0]/3600.,Configuration['BEAM'][0]/3600.*5)
+        Initial_Parameters['YPOS'][1]= sf.set_limits(Initial_Parameters['YPOS'][1],Configuration['BEAM'][0]/3600.,Configuration['BEAM'][0]/3600.*5)
+        Initial_Parameters['VSYS'][1]= sf.set_limits(Initial_Parameters['VSYS'][1],Configuration['CHANNEL_WIDTH']/2.,Configuration['CHANNEL_WIDTH']*5)
+        if Initial_Parameters['INCL'][0] >35:
+            Initial_Parameters['PA'][1]= sf.set_limits(Initial_Parameters['PA'][1],1.,15)
+        Initial_Parameters['INCL'][1]= sf.set_limits(Initial_Parameters['INCL'][1],3.,15)
+
+
         set_fitting_parameters(Configuration, Tirific_Template,stage = 'initialize_os',
-                               initial_estimates=parameters, debug=debug)
+                               initial_estimates=Initial_Parameters )
+
+    tirific(Configuration,Tirific_Template,name = f'{fit_type}_In.def' )
 
-    tirific(Configuration,Tirific_Template,name = f'{fit_type}_In.def', debug=debug)
-    
 initialize_def_file.__doc__ =f'''
  NAME:
     initialize_def_file
 
  PURPOSE:
     setup the first def file to be used in the fitting. As it is the first instance it has some special requirements.
 
@@ -201,94 +210,202 @@
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Standard FAT dictionary with filenames
     Tirific_Template = Standard FAT Tirific Template
 
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     Initial_Parameters = ['EMPTY']
     The initial parameters to be used to set up the def file.
 
     fit_type = 'Undefined'
     type of fitting being done
 
  OUTPUTS:
 
  OPTIONAL OUTPUTS:
 
- PROCEDURES CALLED:
+ PROCEDURES CALLED:"/usr/share/fonts/truetype/msttcorefonts/Times_New_Roman.ttf"
     Unspecified
 
  NOTE:
 '''
 
-def make_overview_plot(Configuration,Fits_Files, debug = False):
+
+class full_system_tracking:
+    def __init__(self,Configuration):
+        self.stop = False
+        self.pid = os.getpid()
+        self.main_pyFAT = psu.Process(self.pid)
+        self.user = self.main_pyFAT.username()
+        self.python = self.main_pyFAT.name()
+        self.tirific = Configuration['TIRIFIC']
+        self.font_file = Configuration['FONT_FILE']
+        self.sofia = Configuration['SOFIA2']
+        self.file = f"{Configuration['MAIN_DIRECTORY']}FAT_Resources_Used.txt"
+        self.plot_name= f"{Configuration['MAIN_DIRECTORY']}pyFAT_Resources_Monitor.pdf"
+        self.cpus= psu.cpu_count()
+        with open(self.file,'w') as resources:
+            resources.write("# This file contains an estimate of all resources used for a pyFAT run. \n")
+            resources.write(f"# {'Time':20s} {'Sys CPU':>10s} {'Sys RAM':>10s} {'FAT CPU':>10s} {'FAT RAM':>10s} \n")
+            resources.write(f"# {'YYYY-MM-DD hh:mm:ss':20s} {'%':>10s} {'Gb':>10s} {'%':>10s} {'Gb':>10s} \n")
+        self.interval = 60 # amount of second when to do new monitor
+
+    def start_monitoring(self):
+        while not self.stop:
+            try:
+                self.sys_cpu= psu.cpu_percent(interval=1)
+                self.sys_ram= psu.virtual_memory().used/2**30.
+                self.CPU = 0.
+                self.RAM = 0.
+                for proc in psu.process_iter():
+                    if proc.username() == self.user \
+                        and proc.status() == 'running'\
+                        and (proc.name() == self.python or\
+                         proc.name() == self.tirific or\
+                         proc.name() == self.sofia or\
+                         proc.name() == 'python3'):
+                        try:
+                            self.CPU += proc.cpu_percent(interval=0.5)/self.cpus
+                            self.RAM += (proc.memory_info()[0])/2**30.
+                        except:
+                            pass
+                #file.write(f"{datetime.now()} CPU = {CPU} % Mem = {mem} Gb for TiRiFiC \n")
+                with open(self.file,'a') as resources:
+                    resources.write(f"{datetime.now().strftime('%Y-%m-%d %H:%M:%S'):20s} {self.sys_cpu:>10.1f} {self.sys_ram:>10.2f} {self.CPU:>10.1f} {self.RAM:>10.2f} \n")
+            except Exception as e:
+                #We do not care if something goes wrong once. We don't want the monitor to crash
+                #but we would like to know what went wrong
+                traceback.print_exception(type(e),e,e.__traceback__)
+                pass
+            time.sleep(self.interval)
+
+    def stop_monitoring(self):
+        self.stop = True
+        loads = {'Time':[]}
+        keys=['SCPU','SRAM','FCPU','FRAM']
+        for key in keys:
+            loads[key]  = []
+        with open(self.file) as file:
+            lines = file.readlines()
+        startdate = 0
+        #load data from file into dictionary
+        for line in lines:
+            line = line.split()
+            if line[0] == '#':
+                continue
+            else:
+                date = extract_date(f"{line[0]} {line[1]}")
+            if startdate == 0:
+                startdate = date
+            diff = date - startdate
+            time = diff.total_seconds()/(3600.)
+            loads['Time'].append(time)
+            for i,key in enumerate(keys):
+                loads[key].append(float(line[int(2+i)]))
+        #Plot the parameters
+        try:
+            mpl_fm.fontManager.addfont(self.font_file)
+            font_name = mpl_fm.FontProperties(fname=self.font_file).get_name()
+        except FileNotFoundError:
+            font_name = 'DejaVu Sans'
+        labelfont = {'family': font_name,
+                 'weight': 'normal',
+                 'size': 4}
+        fig, ax1 = plt.subplots(figsize = (8,6))
+        fig.subplots_adjust(left = 0.1, right = 0.9, bottom = 0.3, top = 0.7)
+        ax1.plot(loads['Time'],loads['SRAM'],'b--',lw=0.5,alpha=0.5, label='System RAM')
+        ax1.plot(loads['Time'],loads['FRAM'],'b-',lw=0.5,alpha=1.0, label='pyFAT RAM')
+        ax1.set_ylim(0,np.max(np.array(loads['SRAM']+loads['FRAM'],dtype=float))*1.1)
+        ax1.set_ylabel('RAM (Gb) ', color='b')
+        ax1.tick_params(axis='y', labelcolor='b')
+        ax1.set_xlabel('Run Duration (h)', color='k',zorder=5)
+        ax2 = ax1.twinx()
+        ax2.plot(loads['Time'],loads['SCPU'],'r--',lw=0.5,alpha=0.5, label='System CPU')
+        ax2.plot(loads['Time'],loads['FCPU'],'r-',lw=0.5,alpha=1.0, label='pyFAT CPU')
+        ax2.set_ylim(0,np.max(np.array(loads['SCPU']+loads['FCPU'],dtype=float))*1.1)
+        ax2.set_ylabel('CPUs (%)',color='r')
+        ax2.tick_params(axis='y', labelcolor='r')
+        fig.savefig(self.plot_name)
+        plt.close()
+
+def make_overview_plot(Configuration,Fits_Files ):
     fit_type = Configuration['USED_FITTING']
-    if debug:
-        print_log(f'''MAKE_OVERVIEW_PLOT: We are starting the overview plot.
-''',Configuration['OUTPUTLOG'],debug =True )
+    sf.print_log(f'''MAKE_OVERVIEW_PLOT: We are starting the overview plot.
+''',Configuration,case=['debug_start'])
 
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
         cube_mod = fits.open(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel.fits")
         moment0_mod = fits.open(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel_mom0.fits")
         moment1_mod = fits.open(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel_mom1.fits")
         moment2_mod = fits.open(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel_mom2.fits")
         cube = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['FITTING_CUBE']}")
-        moment0 = fits.open(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Fits_Files['MOMENT0']}")
-        moment1 = fits.open(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Fits_Files['MOMENT1']}")
-        moment2 = fits.open(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Fits_Files['MOMENT2']}")
-        channels_map = fits.open(f"{Configuration['FITTING_DIR']}/Sofia_Output/{Fits_Files['CHANNEL_MAP']}")
-        im_wcs = WCS(moment0[0].header)
+        moment0 = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MOMENT0']}")
+        moment1 = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MOMENT1']}")
+        moment2 = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['MOMENT2']}")
+        channels_map = fits.open(f"{Configuration['FITTING_DIR']}{Fits_Files['CHANNEL_MAP']}")
+        im_wcs = WCS(moment0[0].header).celestial
 
     # Open the model info
-    if debug:
-        print_log(f'''MAKE_OVERVIEW_PLOT: Reading the variables from the final model
-''',Configuration['OUTPUTLOG'],debug =True )
+    sf.print_log(f'''MAKE_OVERVIEW_PLOT: Reading the variables from the final model
+''',Configuration,case=['debug_add'])
     Vars_to_plot_short= ['RADI','XPOS','YPOS','VSYS','VROT','INCL','PA','SDIS',\
                     'SBR','Z0']
     Vars_to_plot=copy.deepcopy(Vars_to_plot_short)
     for x in Vars_to_plot_short:
         if x != 'RADI':
-            Vars_to_plot.append(f'{x}_ERR')
+            Vars_to_plot.append(f'# {x}_ERR')
         if x not in ['XPOS','YPOS','VSYS']:
             Vars_to_plot.append(f'{x}_2')
-            Vars_to_plot.append(f'{x}_2_ERR')
-    FAT_Model = load_tirific(Configuration,f"{Configuration['FITTING_DIR']}Finalmodel/Finalmodel.def",Variables= Vars_to_plot,unpack=False,debug=debug)
+            Vars_to_plot.append(f'# {x}_2_ERR')
+    FAT_Model = sf.load_tirific(Configuration,\
+        f"{Configuration['FITTING_DIR']}Finalmodel/Finalmodel.def",\
+        Variables= Vars_to_plot,array=True )
     Extra_Model_File = f"{Configuration['FITTING_DIR']}{fit_type}/{fit_type}_Iteration_{Configuration['ITERATIONS']}.def"
 
     if os.path.exists(Extra_Model_File):
-        Extra_Model = load_tirific(Configuration,Extra_Model_File,Variables= Vars_to_plot,unpack=False,debug=debug)
+        Extra_Model = sf.load_tirific(Configuration,Extra_Model_File,\
+            Variables= Vars_to_plot,array=True )
     else:
         Extra_Model = []
-    if debug:
-        print_log(f'''MAKE_OVERVIEW_PLOT: We find the following model values.
-{'':8s}{[f"{x} = {FAT_Model[:,i]}" for i,x in enumerate(Vars_to_plot)]}
-''',Configuration['OUTPUTLOG'])
+    sf.print_log(f'''MAKE_OVERVIEW_PLOT: We find the following model values.
+{'':8s}{[f"{x} = {FAT_Model[i,:]}" for i,x in enumerate(Vars_to_plot)]}
+''',Configuration,case=['debug_add'])
 
     if os.path.exists(f"{Configuration['FITTING_DIR']}ModelInput.def"):
-        Input_Model = load_tirific(Configuration,f"{Configuration['FITTING_DIR']}ModelInput.def",Variables= Vars_to_plot,unpack=False,debug=debug)
+        Input_Model = sf.load_tirific(Configuration,\
+            f"{Configuration['FITTING_DIR']}ModelInput.def",\
+            Variables= Vars_to_plot,array=True )
     else:
         Input_Model = []
     sof_basic_ra,sof_basic_dec, sof_basic_vsys,sof_basic_maxrot,sof_basic_pa,sof_basic_inclination,sof_basic_extent = load_basicinfo(Configuration,
         f"{Configuration['FITTING_DIR']}{Configuration['BASE_NAME']}-Basic_Info.txt",Variables=['RA','DEC','VSYS','Max VRot','PA','Inclination','D_HI'])
 
 
     #Let's start plotting
+    ysize = 23.2
+    xsize = 0.7*ysize
+    Overview = plt.figure(2, figsize=(xsize, ysize), dpi=300, facecolor='w', edgecolor='k')
 
-    Overview = plt.figure(2, figsize=(8.2, 11.6), dpi=300, facecolor='w', edgecolor='k')
+    size_factor= ysize/11.6
+    size_ratio = ysize/xsize
 
-    size_ratio = 11.6/8.2
     #stupid pythonic layout for grid spec, which means it is yx instead of xy like for normal human beings
     gs = Overview.add_gridspec(int(20*size_ratio),20)
-    labelfont = {'family': 'Times New Roman',
+    try:
+        mpl_fm.fontManager.addfont(Configuration['FONT_FILE'])
+        font_name = mpl_fm.FontProperties(fname=Configuration['FONT_FILE']).get_name()
+    except FileNotFoundError:
+        font_name = 'DejaVu Sans'
+    labelfont = {'family': font_name,
              'weight': 'normal',
-             'size': 8}
+             'size': 8*size_factor}
     plt.rc('font', **labelfont)
     plt.rcParams['xtick.direction'] = 'in'
     plt.rcParams['ytick.direction'] = 'in'
 # First some textual information
 
     if Configuration['SUB_DIR'] == './':
         name = Configuration['BASE_NAME']
@@ -303,18 +420,18 @@
         bottom=False,      # ticks along the bottom edge are off
         top=False,         # ticks along the top edge are off
         labelbottom=False,
         right = False,
         left= False,
         labelleft = False)
     ax_text.text(0.5,1.0,f'''Overview for {name}''',rotation=0, va='top',ha='center', color='black',transform = ax_text.transAxes,
-      bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=14)
+      bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=14*size_factor)
     ax_text.text(0.5,0.25,f'''The ring size used in the model is {Configuration['RING_SIZE']:.2f} x BMAJ, with BMAJ = {Configuration['BEAM'][0]:.1f} arcsec. We assumed a distance  of {Configuration['DISTANCE']:.1f} Mpc.'''
       ,rotation=0, va='top',ha='center', color='black',transform = ax_text.transAxes,
-      bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=10)
+      bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=10*size_factor)
 
 
 #-----------------------------------------------------------------Moment 0 ------------------------------------------------------
     ax_moment0 = Overview.add_subplot(gs[2:8,0:6], projection=im_wcs)
     ax_moment0.set_label('Intensity Map')
     #Comp_ax1.set_facecolor('black')
     # we need contour levels and
@@ -338,28 +455,31 @@
     maxdism0 = np.max(moment0[0].data) * 0.8
     if mindism0 > maxdism0:
         mindism0 = 0.1*maxdism0
     if maxdism0 < 16*mindism0:
         momlevel = np.array([1,4,8,12],dtype=float)* mindism0
     elif maxdism0 < 32*mindism0:
         momlevel = np.array([1,4,8,16,24,32],dtype=float)* mindism0
-    else:
+    elif maxdism0 < 256*mindism0:
         momlevel = np.array([1,4,8,32,64,128],dtype=float) * mindism0
+    else:
+        momlevel = np.array([0,1,2,3,4,5,6,7],dtype=float) * (maxdism0-mindism0)/7+ mindism0
+
     #print("We find this {} as the minimum of the moment0 map".format(mindism0))
     momlevel = np.array([x for x in momlevel if x < np.max(moment0[0].data)*0.95],dtype=float)
     if momlevel.size == 0:
         momlevel=0.5*mindism0
     ax_moment0.contour(moment0[0].data, transform=ax_moment0.get_transform(im_wcs),
-               levels=momlevel, colors='white',linewidths=1.5 , zorder =4)
+               levels=momlevel, colors='white',linewidths=1.5*size_factor , zorder =4)
     ax_moment0.contour(moment0[0].data, transform=ax_moment0.get_transform(im_wcs),
-              levels=momlevel, colors='k',zorder=6, linewidths=1.2)
+              levels=momlevel, colors='k',zorder=6, linewidths=1.2*size_factor)
     ax_moment0.contour(moment0_mod[0].data, transform=ax_moment0.get_transform(im_wcs),
-               levels=momlevel, colors='white',linewidths=1.2 , zorder =7)
+               levels=momlevel, colors='white',linewidths=1.2*size_factor , zorder =7)
     ax_moment0.contour(moment0_mod[0].data, transform=ax_moment0.get_transform(im_wcs),
-              levels=momlevel, colors='r',zorder=8, linewidths=0.9)
+              levels=momlevel, colors='r',zorder=8, linewidths=0.9*size_factor)
     xmin, xmax = ax_moment0.get_xlim()
     ymin, ymax = ax_moment0.get_ylim()
     if xmax > ymax:
         diff = int(xmax-ymax)/2.
         ax_moment0.set_ylim(ymin-diff,ymax+diff)
         ymin, ymax = ax_moment0.get_ylim()
     else:
@@ -368,29 +488,30 @@
         xmin, xmax = ax_moment0.get_xlim()
     ghxloc, ghyloc = im_wcs.wcs_pix2world(float(xmin+(xmax-xmin)/18.), float(ymin+(ymax-ymin)/18.), 1.)
     localoc = [float(ghxloc),float(ghyloc) ]
     widthb = moment0[0].header['BMIN']
     heightb = moment0[0].header['BMAJ']
     try:
         angleb  = moment0[0].header['BPA']
-    except:
+    except KeyError:
         angleb = 0.
     beam = Ellipse(xy=localoc, width=widthb, height=heightb, angle=angleb, transform=ax_moment0.get_transform('fk4'),
            edgecolor='k', lw=1, facecolor='none', hatch='/////',zorder=15)
     ax_moment0.add_patch(beam)
     # colorbar
     divider = make_axes_locatable(ax_moment0)
     cax = divider.append_axes("top", size="5%", pad=0.05, axes_class=maxes.Axes)
     cbar = plt.colorbar(moment0_plot, cax=cax, orientation='horizontal')
     cax.xaxis.set_ticks_position('top')
     cbar.set_ticks([min_color, max_color])
-    cbar.ax.set_title(f"{moment0[0].header['BUNIT']}", y= 0.2)
-
+    cbar.ax.set_title(f"{moment0[0].header['BUNIT']}", y= 0.2*size_factor**2)
 
-    column_levels = columndensity(Configuration,momlevel*1000.,systemic = FAT_Model[0,Vars_to_plot.index('VSYS')])
+    '''the channel width should be 1 as the map is already in Jy/beam*km/s'''
+    column_levels = sf.columndensity(Configuration,momlevel*1000.,\
+        systemic = FAT_Model[Vars_to_plot.index('VSYS'),0], channel_width=1)
 
     if 1e21 < np.min(column_levels):
         fact= 1e21
         str_fact = r'$\times 10^{21} {\rm cm}^{-2}$'
     elif 1e20 < np.min(column_levels) < 1e21:
         fact= 1e20
         str_fact = r'$\times 10^{20} {\rm cm}^{-2}$'
@@ -419,35 +540,35 @@
     moment0.close()
     moment0_mod.close()
 #-----------------------------------------------------------------Velocity Field------------------------------------------------------
     ax_moment1 = Overview.add_subplot(gs[10:16, 0:6], projection=im_wcs)
     ax_moment1.set_label('Velocity Field')
     #Comp_ax1.set_facecolor('black')
     # we need contour levels and
-    inclination_correction = set_limits(FAT_Model[0,Vars_to_plot.index('INCL')]+12.5,20.,90.)
-    velocity_width= set_limits(1.25*np.nanmax(FAT_Model[:,Vars_to_plot.index('VROT')])*np.sin(np.radians(inclination_correction)),30.,700.)
+    inclination_correction = sf.set_limits(FAT_Model[Vars_to_plot.index('INCL'),0]+12.5,20.,90.)
+    velocity_width= sf.set_limits(1.25*np.nanmax(FAT_Model[Vars_to_plot.index('VROT'),:])*np.sin(np.radians(inclination_correction)),30.,700.)
 
-    max_color= FAT_Model[0,Vars_to_plot.index('VSYS')]+velocity_width
-    min_color= FAT_Model[0,Vars_to_plot.index('VSYS')]-velocity_width
+    max_color= FAT_Model[Vars_to_plot.index('VSYS'),0]+velocity_width
+    min_color= FAT_Model[Vars_to_plot.index('VSYS'),0]-velocity_width
 
     moment1_plot = ax_moment1.imshow(moment1[0].data, cmap='rainbow', origin='lower', alpha=1, vmin = min_color, vmax = max_color )
     plt.ylabel('DEC (J2000)')
     #Stupid python suddenly finds its own labels
     plt.xlabel('RA J2000')
 
     # contours
-    velocity_step=set_limits(int((int(max_color-min_color)*0.9)/20.),1.,30.)
+    velocity_step=sf.set_limits(int((int(max_color-min_color)*0.9)/20.),1.,30.)
     integer_array = np.linspace(0,20,21)-10
-    momlevel = [FAT_Model[0,Vars_to_plot.index('VSYS')]+x*velocity_step for x in integer_array if min_color < FAT_Model[0,Vars_to_plot.index('VSYS')]+x*velocity_step < max_color]
+    momlevel = [FAT_Model[Vars_to_plot.index('VSYS'),0]+x*velocity_step for x in integer_array if min_color < FAT_Model[Vars_to_plot.index('VSYS'),0]+x*velocity_step < max_color]
     ax_moment1.contour(moment1[0].data, transform=ax_moment1.get_transform(im_wcs),
-               levels=momlevel, colors='white',linewidths=1.2 , zorder =4)
+               levels=momlevel, colors='white',linewidths=1.5 *size_factor, zorder =4)
     ax_moment1.contour(moment1[0].data, transform=ax_moment1.get_transform(im_wcs),
-              levels=momlevel, colors='k',zorder=6, linewidths=0.9)
+              levels=momlevel, colors='k',zorder=6, linewidths=0.9*size_factor)
     ax_moment1.contour(moment1_mod[0].data, transform=ax_moment1.get_transform(im_wcs),
-               levels=momlevel, colors='white',linewidths=1.2 , zorder =7)
+               levels=momlevel, colors='white',linewidths=1.2*size_factor , zorder =7)
     #ax_moment1.contour(moment1_mod[0].data, transform=ax_moment1.get_transform(im_wcs),
     #          levels=momlevel, colors='r',zorder=8, linewidths=0.9)
     xmin, xmax = ax_moment1.get_xlim()
     ymin, ymax = ax_moment1.get_ylim()
     if xmax > ymax:
         diff = int(xmax-ymax)/2.
         ax_moment1.set_ylim(ymin-diff,ymax+diff)
@@ -458,63 +579,63 @@
         ax_moment1.set_xlim(xmin-diff,xmax+diff)
     ghxloc, ghyloc = im_wcs.wcs_pix2world(float(xmin+(xmax-xmin)/18.), float(ymin+(ymax-ymin)/18.), 1.)
     localoc = [float(ghxloc),float(ghyloc) ]
     widthb = moment1[0].header['BMIN']
     heightb = moment1[0].header['BMAJ']
     try:
         angleb  = moment1[0].header['BPA']
-    except:
+    except KeyError:
         angleb = 0.
     beam = Ellipse(xy=localoc, width=widthb, height=heightb, angle=angleb, transform=ax_moment1.get_transform('fk4'),
            edgecolor='k', lw=1, facecolor='none', hatch='/////',zorder=15)
     ax_moment1.add_patch(beam)
     # colorbar
     divider = make_axes_locatable(ax_moment1)
     cax = divider.append_axes("top", size="5%", pad=0.05, axes_class=maxes.Axes)
     cbar = plt.colorbar(moment1_plot, cax=cax, orientation='horizontal')
     cax.xaxis.set_ticks_position('top')
     cbar.set_ticks([min_color, max_color])
-    cbar.ax.set_title(f"{moment1[0].header['BUNIT']}", y= 0.2)
+    cbar.ax.set_title(f"{moment1[0].header['BUNIT']}", y= 0.2*size_factor**2)
 
     column_levels = ', '.join(["{:.1f}".format(x) for x in momlevel])
     info_string= f'''The contours start at {float(momlevel[0]):.1f} km/s'''
     if len(momlevel) > 1:
-        info_string=f'''{info_string} and increase with {float(momlevel[1])-float(momlevel[0]):.1f} km/s.'''
+        info_string=f'''{info_string} \n and increase with {float(momlevel[1])-float(momlevel[0]):.1f} km/s.'''
     else:
         info_string=f'''{info_string}.'''
 
 
     ax_moment1.text(-0.1,-0.2,info_string, va='top',ha='left', color='black',transform = ax_moment1.transAxes,
           bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7)
     # No further need for the moment maps
     moment1.close()
     moment1_mod.close()
 #-----------------------------------------------------------------Moment 2------------------------------------------------------
     ax_moment2 = Overview.add_subplot(gs[10:16:, 8:14], projection=im_wcs)
     ax_moment2.set_label('Moment2')
     #Comp_ax1.set_facecolor('black')
     # we need contour levels and
-    max_color= set_limits(np.nanmax(moment2[0].data),15,50)
+    max_color= sf.set_limits(np.nanmax(moment2[0].data),15,50)
     min_color= 0.
 
     moment2_plot = ax_moment2.imshow(moment2[0].data, cmap='rainbow' ,origin='lower', alpha=1, vmin = min_color, vmax = max_color )
     plt.ylabel('DEC (J2000)')
     #Stupid python suddenly finds its own labels
     plt.xlabel('RA J2000')
 
     # contours
 
     momlevel = np.linspace(min_color,max_color*0.8,5)
 
     ax_moment2.contour(moment2[0].data, transform=ax_moment2.get_transform(im_wcs),
-               levels=momlevel, colors='white',linewidths=1.5 , zorder =4)
+               levels=momlevel, colors='white',linewidths=1.5*size_factor , zorder =4)
     ax_moment2.contour(moment2[0].data, transform=ax_moment2.get_transform(im_wcs),
-              levels=momlevel, colors='k',zorder=6, linewidths=1.2)
+              levels=momlevel, colors='k',zorder=6, linewidths=1.2*size_factor)
     ax_moment2.contour(moment2_mod[0].data, transform=ax_moment2.get_transform(im_wcs),
-               levels=momlevel, colors='white',linewidths=1.2 , zorder =7)
+               levels=momlevel, colors='white',linewidths=1.2*size_factor , zorder =7)
 
     xmin, xmax = ax_moment2.get_xlim()
     ymin, ymax = ax_moment2.get_ylim()
     if xmax > ymax:
         diff = int(xmax-ymax)/2.
         ax_moment2.set_ylim(ymin-diff,ymax+diff)
         ymin, ymax = ax_moment2.get_ylim()
@@ -525,30 +646,30 @@
 
     ghxloc, ghyloc = im_wcs.wcs_pix2world(float(xmin+(xmax-xmin)/18.), float(ymin+(ymax-ymin)/18.), 1.)
     localoc = [float(ghxloc),float(ghyloc) ]
     widthb = moment2[0].header['BMIN']
     heightb = moment2[0].header['BMAJ']
     try:
         angleb  = moment2[0].header['BPA']
-    except:
+    except KeyError:
         angleb = 0.
 
     beam = Ellipse(xy=localoc, width=widthb, height=heightb, angle=angleb, transform = ax_moment2.get_transform('fk4'),
            edgecolor='k', lw=1, facecolor='none', hatch='/////',zorder=15)
     ax_moment2.add_patch(beam)
 
 
     # colorbar
     divider = make_axes_locatable(ax_moment2)
     cax = divider.append_axes("top", size="5%", pad=0.05, axes_class=maxes.Axes)
     cbar = plt.colorbar(moment2_plot, cax=cax, orientation='horizontal')
     cax.xaxis.set_ticks_position('top')
     cbar.set_ticks([min_color, max_color])
     #cbar.set_title(label=f"{moment2[0].header['BUNIT']}")
-    cbar.ax.set_title(f"{moment2[0].header['BUNIT']}", y= 0.2)
+    cbar.ax.set_title(f"{moment2[0].header['BUNIT']}", y= 0.2*size_factor**2)
 
     column_levels = ', '.join(["{:.1f}".format(x) for x in momlevel])
     if len(momlevel) < 4:
         info_string = f"The contours are at {column_levels} km/s."
     else:
         info_string = f"The contours are at {', '.join(['{:.1f}'.format(x) for x in momlevel[0:4]])}"
         counter = 4
@@ -563,80 +684,93 @@
     moment2.close()
     moment2_mod.close()
 
 
 
 #__________________------------------------------------------------------------PV Diagram
 
-    extract_angle = np.mean(FAT_Model[0:round(len(FAT_Model[:,Vars_to_plot.index('PA')])/2.),Vars_to_plot.index('PA')])
+    extract_angle = np.mean(FAT_Model[Vars_to_plot.index('PA'),0:round(len(FAT_Model[Vars_to_plot.index('PA'),:])/2.)])
     PV = extract_pv(Configuration,cube,extract_angle, \
-                    center = [float(FAT_Model[0,Vars_to_plot.index('XPOS')]),float(FAT_Model[0,Vars_to_plot.index('YPOS')]),float(FAT_Model[0,Vars_to_plot.index('VSYS')]*1000.)], \
+                    center = [float(FAT_Model[Vars_to_plot.index('XPOS'),0]),float(FAT_Model[Vars_to_plot.index('YPOS'),0]),float(FAT_Model[Vars_to_plot.index('VSYS'),0]*1000.)], \
                     convert=1000.)
     if not os.path.exists(f"{Configuration['FITTING_DIR']}/Finalmodel/{Configuration['BASE_NAME']}_final_xv.fits"):
         fits.writeto(f"{Configuration['FITTING_DIR']}/Finalmodel/{Configuration['BASE_NAME']}_final_xv.fits",PV[0].data,PV[0].header)
     PV_model = extract_pv(Configuration,cube_mod,extract_angle, \
-                    center = [float(FAT_Model[0,Vars_to_plot.index('XPOS')]),float(FAT_Model[0,Vars_to_plot.index('YPOS')]),float(FAT_Model[0,Vars_to_plot.index('VSYS')]*1000.)], \
+                    center = [float(FAT_Model[Vars_to_plot.index('XPOS'),0]),float(FAT_Model[Vars_to_plot.index('YPOS'),0]),float(FAT_Model[Vars_to_plot.index('VSYS'),0]*1000.)], \
                     convert=1000.)
     if not os.path.exists(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel_xv.fits"):
         fits.writeto(f"{Configuration['FITTING_DIR']}/Finalmodel/Finalmodel_xv.fits",PV_model[0].data,PV_model[0].header)
     ratio=PV[0].header['NAXIS2']/PV[0].header['NAXIS1']
     # Then we want to plot our PV-Diagram
+    '''
     with warnings.catch_warnings():
         warnings.simplefilter("ignore")
-        xv_proj = WCS(PV[0].header)
-        xv_model_proj = WCS(PV_model[0].header)
-    ax_PV = Overview.add_subplot(gs[2:8,8:14], projection=xv_proj)
+        #As astropy is the dumbest piece of software ever invented and it cannot separate stray keywords from extra dimensions
+        # we need to specify we want the first two axes.
+        xv_proj = WCS(PV[0].header,naxis=[0,1])
+        xv_model_proj = WCS(PV_model[0].header,naxis=[0,1])
+    # As astropy is really a dumb piece of shit using a WCS messes up the the axes modifications
+    #ax_PV = Overview.add_subplot(gs[2:8,8:14], projection=xv_proj)
+    '''
+    ax_PV = Overview.add_subplot(gs[2:8,8:14])
     #Comp_ax2.set_title('PV-Diagram')
 
     maxint= np.nanmax(PV[0].data)*0.85
     minint= np.nanmin(PV[0].data)/3.
 
 
     PV_plot = ax_PV.imshow(PV[0].data,  cmap='hot_r', origin='lower', alpha=1, vmin=minint, vmax=maxint,aspect='auto')
+
     xaxis = [PV[0].header['CRVAL1'] + (i - PV[0].header['CRPIX1'] + 1) * (PV[0].header['CDELT1']) for i in
              range(PV[0].header['NAXIS1'])]
     yaxis = [PV[0].header['CRVAL2'] + (i - PV[0].header['CRPIX2'] + 1) * (PV[0].header['CDELT2']) for i in
              range(PV[0].header['NAXIS2'])]
-    plt.gca().set_xticks(range(len(xaxis))[0:-1:int(len(xaxis) / 5)])
-    plt.gca().set_yticks(range(len(yaxis))[0:-1:int(len(yaxis) / 5)])
-    plt.gca().set_xticklabels(['{:10.0f}'.format(i) for i in xaxis[0:-1:int(len(xaxis) / 5)]])
-    plt.gca().set_yticklabels(['{:10.1f}'.format(i) for i in yaxis[0:-1:int(len(yaxis) / 5)]])
+    #something is going wrong here, Fixed as usual astropy was fucking thing up
+    ax_PV.set_xticks(range(len(xaxis))[0:-1:int(len(xaxis) / 5)])
+    ax_PV.set_yticks(range(len(yaxis))[0:-1:int(len(yaxis) / 5)])
+    ax_PV.set_xticklabels(['{:10.1f}'.format(i) for i in xaxis[0:-1:int(len(xaxis) / 5)]])
+    ax_PV.set_yticklabels(['{:10.1f}'.format(i) for i in yaxis[0:-1:int(len(yaxis) / 5)]])
 
     #Add some contours
     neg_cont = np.array([-3,-1.5],dtype=float)*Configuration['NOISE']
-    pos_cont =  np.array([1.5,3.,6,12,24,48,96],dtype=float)*Configuration['NOISE']
-    pos_cont = np.array([x for x in pos_cont if x < np.nanmax(PV[0].data) * 0.95],dtype=float)
-    if debug:
-            print_log(f'''MAKE_OVERVIEW_PLOT: postive {pos_cont}, negative {neg_cont}, noise {Configuration['NOISE']}
-    ''',Configuration['OUTPUTLOG'],debug =True )
+    if  np.nanmax(PV[0].data) * 0.95 < 96*Configuration['NOISE']:
+        pos_cont =  np.array([1.5,3.,6,12,24,48,96],dtype=float)*Configuration['NOISE']
+    else:
+        pos_cont =  np.array([0,1,2,3,4,5,6,7],dtype=float)*(np.nanmax(PV[0].data) * 0.95-3.*Configuration['NOISE'])/7. +3.*Configuration['NOISE']
+    pos_cont = np.array([x for x in pos_cont if x <= np.nanmax(PV[0].data) * 0.95],dtype=float)
+    sf.print_log(f'''MAKE_OVERVIEW_PLOT: postive {pos_cont}, negative {neg_cont}, noise {Configuration['NOISE']}
+''',Configuration,case=['debug_add'] )
     if pos_cont.size == 0:
         pos_cont = 0.5 * np.nanmax(PV[0].data) * 0.95
-    try:
-        ax_PV.contour(PV[0].data, levels=pos_cont, colors='k',transform=ax_PV.get_transform(xv_proj))
-        ax_PV.contour(PV[0].data, levels=neg_cont, colors='grey',linestyles='--',transform=ax_PV.get_transform(xv_proj))
-        ax_PV.contour(PV_model[0].data, levels=pos_cont, colors='b',transform=ax_PV.get_transform(xv_model_proj),linewidths=1.)
-        momlevel = np.hstack((neg_cont,pos_cont))
-        column_levels = ', '.join(["{:.1f}".format(x*1000.) for x in momlevel])
-        if len(momlevel) < 4:
-            info_string = f"The contours are at {column_levels} mJy/beam"
-        else:
-            info_string = f"The contours are at {', '.join(['{:.1f}'.format(x*1000.) for x in momlevel[0:4]])}"
-            counter = 5
-            while counter < len(momlevel):
-                info_string = info_string+f"\n {', '.join(['{:.1f}'.format(x*1000.) for x in momlevel[counter:counter+7]])}"
-                counter += 7
-            info_string = info_string+" mJy/beam."
-    except:
-        info_string = f"Something went wrong plotting the contours."
+
+    #ax_PV.contour(PV[0].data, levels=pos_cont, colors='k',transform=ax_PV.get_transform(xv_proj))
+    #ax_PV.contour(PV[0].data, levels=neg_cont, colors='grey',linestyles='--',transform=ax_PV.get_transform(xv_proj))
+    #ax_PV.contour(PV_model[0].data, levels=pos_cont, colors='b',transform=ax_PV.get_transform(xv_model_proj),linewidths=1.)
+    ax_PV.contour(PV[0].data, levels=pos_cont,linewidths=1.*size_factor, colors='k')
+    ax_PV.contour(PV[0].data, levels=neg_cont,linewidths=1.*size_factor, colors='grey',linestyles='--')
+    ax_PV.contour(PV_model[0].data, levels=pos_cont, colors='b',linewidths=1.*size_factor)
+
+    momlevel = np.hstack((neg_cont,pos_cont))
+    column_levels = ', '.join(["{:.1f}".format(x*1000.) for x in momlevel])
+    if len(momlevel) < 4:
+        info_string = f"The contours are at {column_levels} mJy/beam"
+    else:
+        info_string = f"The contours are at {', '.join(['{:.1f}'.format(x*1000.) for x in momlevel[0:4]])}"
+        counter = 5
+        while counter < len(momlevel):
+            info_string = info_string+f"\n {', '.join(['{:.1f}'.format(x*1000.) for x in momlevel[counter:counter+7]])}"
+            counter += 7
+        info_string = info_string+" mJy/beam."
+
     divider = make_axes_locatable(ax_PV)
     cax = divider.append_axes("top", size="5%", pad=0.05, axes_class=maxes.Axes)
     cbar = plt.colorbar(PV_plot, cax=cax, orientation='horizontal')
     cax.xaxis.set_ticks_position('top')
     cbar.set_ticks([minint, maxint])
-    cbar.ax.set_title(f"{PV[0].header['BUNIT']}", y= 0.2)
+    cbar.ax.set_title(f"{PV[0].header['BUNIT']}", y= 0.2*size_factor**2)
 
     ax_PV.text(-0.1,-0.2,info_string, va='top',ha='left', color='black',transform = ax_PV.transAxes,
           bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7)
 
     #cf.plot_fits(filename, Comp_ax2, cmap='hot_r', aspect=ratio, cbar ='horizontal')
     ax_PV.set_xlabel("Offset (arcsec)")
     ax_PV.set_ylabel("Velocity (km s$^{-1}$)")
@@ -671,33 +805,33 @@
 
     chartBox = ax_legend.get_position()
     ax_legend.set_position([chartBox.x0, chartBox.y0, chartBox.width*1.0, chartBox.height])
     ax_legend.legend(loc='upper left', bbox_to_anchor = (-1.0,1.03),shadow=True, ncol=1)
 
 
 # ------------------------------Rotation curves------------------------------------
-    labelfont= {'family':'Times New Roman',
+
+    labelfont= {'family':font_name,
             'weight':'normal',
-            'size':10}
+            'size':10*size_factor}
     ax_RC = plot_parameters(Configuration,Vars_to_plot,FAT_Model,gs[19:22,3:9],\
                             Overview,'VROT',Input_Model = Input_Model,initial_extent= sof_basic_extent[0], \
-                            initial = sof_basic_maxrot[0],Extra_Model = Extra_Model,\
-                            debug=debug)
-    ymin =np.min([FAT_Model[1:,Vars_to_plot.index('VROT')],FAT_Model[1:,Vars_to_plot.index('VROT_2')]])
+                            initial = sof_basic_maxrot[0],Extra_Model = Extra_Model)
+    ymin =np.min([FAT_Model[Vars_to_plot.index('VROT'),1:],FAT_Model[Vars_to_plot.index('VROT_2'),1:]])
     if len(Extra_Model) > 0:
-        ymin2 =np.min([Extra_Model[1:,Vars_to_plot.index('VROT')],Extra_Model[1:,Vars_to_plot.index('VROT_2')]])
-        ymax2 =np.max([Extra_Model[1:,Vars_to_plot.index('VROT')],Extra_Model[1:,Vars_to_plot.index('VROT_2')]])
+        ymin2 =np.min([Extra_Model[Vars_to_plot.index('VROT'),1:],Extra_Model[Vars_to_plot.index('VROT_2'),1:]])
+        ymax2 =np.max([Extra_Model[Vars_to_plot.index('VROT'),1:],Extra_Model[Vars_to_plot.index('VROT_2'),1:]])
     else:
         ymin2 = ymin
         ymax2 = ymax
-    ymax =np.max([FAT_Model[1:,Vars_to_plot.index('VROT')],FAT_Model[1:,Vars_to_plot.index('VROT_2')]])
+    ymax =np.max([FAT_Model[Vars_to_plot.index('VROT'),1:],FAT_Model[Vars_to_plot.index('VROT_2'),1:]])
 
     if len(Input_Model) > 0:
-        ymin3 =np.min([Input_Model[1:,Vars_to_plot.index('VROT')],Input_Model[1:,Vars_to_plot.index('VROT_2')]])
-        ymax3 =np.max([Input_Model[1:,Vars_to_plot.index('VROT')],Input_Model[1:,Vars_to_plot.index('VROT_2')]])
+        ymin3 =np.min([Input_Model[Vars_to_plot.index('VROT'),1:],Input_Model[Vars_to_plot.index('VROT_2'),1:]])
+        ymax3 =np.max([Input_Model[Vars_to_plot.index('VROT'),1:],Input_Model[Vars_to_plot.index('VROT_2'),1:]])
     else:
         ymin3=ymin
         ymax3= ymax
     ymin = np.min([ymin,ymin2,ymin3])
     ymax = np.max([ymax,ymax2,ymax3])
 
     buffer = np.mean([ymin,ymax])/20.
@@ -712,120 +846,120 @@
         direction = 'in',
         bottom=True,      # ticks along the bottom edge are off
         top=True,         # ticks along the top edge are off
         labelbottom=False)
     plt.ylabel('RC (km s$^{-1}$)',**labelfont)
     arcmin,arcmax = ax_RC.get_xlim()
     sec_ax = ax_RC.twiny()
-    sec_ax.set_xlim(convertskyangle(Configuration,arcmin,Configuration['DISTANCE']),convertskyangle(Configuration,arcmax,Configuration['DISTANCE']))
+    sec_ax.set_xlim(sf.convertskyangle(Configuration,arcmin),sf.convertskyangle(Configuration,arcmax))
     sec_ax.figure.canvas.draw()
     sec_ax.set_xlabel('Radius (kpc)',va='bottom',**labelfont)
 
 # ------------------------------Inclination------------------------------------
     ax_INCL = plot_parameters(Configuration,Vars_to_plot,FAT_Model,gs[22:25,3:9],\
                               Overview,'INCL',Input_Model = Input_Model,initial_extent= sof_basic_extent[0], \
-                              initial =sof_basic_inclination[0],Extra_Model = Extra_Model ,debug=debug)
+                              initial =sof_basic_inclination[0],Extra_Model = Extra_Model  )
 
     plt.tick_params(
         axis='x',          # changes apply to the x-axis
         which='both',      # both major and minor ticks are affected
         direction = 'in',
         bottom=True,      # ticks along the bottom edge are off
         top=True,         # ticks along the top edge are off
         labelbottom=False)
     if 'INCL' in Configuration['FIXED_PARAMETERS'][0]:
         ax_INCL.text(1.01,0.5,'Forced Flat', rotation =-90,va='center',ha='left', color='black',transform = ax_INCL.transAxes,
-          bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=10)
+          bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=10*size_factor)
     plt.ylabel('Incl ($^{\circ}$)',**labelfont)
     arcmin,arcmax = ax_INCL.get_xlim()
     sec_ax = ax_INCL.twiny()
-    sec_ax.set_xlim(convertskyangle(Configuration,arcmin,Configuration['DISTANCE']),convertskyangle(Configuration,arcmax,Configuration['DISTANCE']))
+    sec_ax.set_xlim(sf.convertskyangle(Configuration,arcmin),sf.convertskyangle(Configuration,arcmax))
     sec_ax.set_xticklabels([])
     sec_ax.figure.canvas.draw()
 
 # ------------------------------PA------------------------------------
     ax_PA = plot_parameters(Configuration,Vars_to_plot,FAT_Model,gs[25:28,3:9],\
                             Overview,'PA',Input_Model = Input_Model,initial_extent= sof_basic_extent[0],\
-                            initial = sof_basic_pa[0],Extra_Model = Extra_Model,debug=debug)
+                            initial = sof_basic_pa[0],Extra_Model = Extra_Model )
 
     plt.tick_params(
         axis='x',          # changes apply to the x-axis
         which='both',      # both major and minor ticks are affected
         direction = 'in',
         bottom=True,      # ticks along the bottom edge are off
         top=True,         # ticks along the top edge are off
         labelbottom=True)
     if 'PA' in Configuration['FIXED_PARAMETERS'][0]:
         ax_PA.text(1.01,0.5,'Forced Flat', va='center',ha='left', color='black',rotation = -90, transform = ax_PA.transAxes,
-          bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=10)
+          bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=10*size_factor)
     plt.xlabel('Radius (arcsec)',**labelfont)
     plt.ylabel('PA ($^{\circ}$)',**labelfont)
     arcmin,arcmax = ax_PA.get_xlim()
     sec_ax = ax_PA.twiny()
-    sec_ax.set_xlim(convertskyangle(Configuration,arcmin,Configuration['DISTANCE']),convertskyangle(Configuration,arcmax,Configuration['DISTANCE']))
+    sec_ax.set_xlim(sf.convertskyangle(Configuration,arcmin),sf.convertskyangle(Configuration,arcmax))
     sec_ax.set_xticklabels([])
     sec_ax.figure.canvas.draw()
 
 # ------------------------------SDIS------------------------------------
     ax_SDIS = plot_parameters(Configuration,Vars_to_plot,FAT_Model,gs[19:22,12:18],\
                               Overview,'SDIS',Input_Model = Input_Model,initial_extent= sof_basic_extent[0],\
-                              Extra_Model = Extra_Model,initial = 8.,debug=debug)
+                              Extra_Model = Extra_Model,initial = 8. )
     plt.tick_params(
         axis='x',          # changes apply to the x-axis
         which='both',      # both major and minor ticks are affected
         direction = 'in',
         bottom=True,      # ticks along the bottom edge are off
         top=True,         # ticks along the top edge are off
         labelbottom=False,
         labeltop= True)
     if 'SDIS' in Configuration['FIXED_PARAMETERS'][0]:
         ax_SDIS.text(1.01,0.5,'Forced Flat',rotation=-90, va='center',ha='left', color='black',transform = ax_SDIS.transAxes,
-          bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=10)
+          bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=10*size_factor)
 
     plt.ylabel('Disp (km s$^{-1}$)',**labelfont)
     arcmin,arcmax = ax_SDIS.get_xlim()
     sec_ax = ax_SDIS.twiny()
-    sec_ax.set_xlim(convertskyangle(Configuration,arcmin,Configuration['DISTANCE']),convertskyangle(Configuration,arcmax,Configuration['DISTANCE']))
+    sec_ax.set_xlim(sf.convertskyangle(Configuration,arcmin),sf.convertskyangle(Configuration,arcmax))
     sec_ax.figure.canvas.draw()
     sec_ax.set_xlabel('Radius (kpc)',va='bottom',**labelfont)
 
 
 # ------------------------------Scale height------------------------------------
     ax_Z0 = plot_parameters(Configuration,Vars_to_plot,FAT_Model,gs[22:25,12:18],\
                             Overview,'Z0',Input_Model = Input_Model,initial_extent= sof_basic_extent[0],\
-                            Extra_Model = Extra_Model,initial = convertskyangle(Configuration,0.2,Configuration['DISTANCE'],physical=True),debug=debug)
+                            Extra_Model = Extra_Model,initial = sf.convertskyangle(Configuration,0.2,physical=True) )
 
     plt.tick_params(
         axis='x',          # changes apply to the x-axis
         which='both',      # both major and minor ticks are affected
         direction = 'in',
         bottom=True,      # ticks along the bottom edge are off
         top=True,         # ticks along the top edge are off
         labelbottom=False,
         labeltop=False)
     if 'Z0' in Configuration['FIXED_PARAMETERS'][0]:
         ax_Z0.text(1.25,0.5,'Forced Flat',rotation=-90, va='center',ha='left', color='black',transform = ax_Z0.transAxes,
-          bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=10)
+          bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=10*size_factor)
     plt.ylabel('Z0 (arcsec)',**labelfont)
     arcmin,arcmax = ax_Z0.get_ylim()
     sec_ax = ax_Z0.twinx()
-    sec_ax.set_ylim(convertskyangle(Configuration,arcmin,Configuration['DISTANCE']),convertskyangle(Configuration,arcmax,Configuration['DISTANCE']))
+    sec_ax.set_ylim(sf.convertskyangle(Configuration,arcmin),sf.convertskyangle(Configuration,arcmax))
     sec_ax.figure.canvas.draw()
     sec_ax.set_ylabel('Z0 (kpc)',rotation=-90,va='bottom',**labelfont)
     arcmin,arcmax = ax_Z0.get_xlim()
     sec_ax = ax_Z0.twiny()
     sec_ax.set_xticklabels([])
-    sec_ax.set_xlim(convertskyangle(Configuration,arcmin,Configuration['DISTANCE']),convertskyangle(Configuration,arcmax,Configuration['DISTANCE']))
+    sec_ax.set_xlim(sf.convertskyangle(Configuration,arcmin),sf.convertskyangle(Configuration,arcmax))
     sec_ax.figure.canvas.draw()
 
 
 # ------------------------------SBR------------------------------------
     ax_SBR = plot_parameters(Configuration,Vars_to_plot,FAT_Model,gs[25:28,12:18],\
                              Overview,'SBR',Input_Model = Input_Model,initial_extent= sof_basic_extent[0],\
-                             Extra_Model = Extra_Model,debug=debug)
+                             Extra_Model = Extra_Model )
 
     plt.tick_params(
         axis='x',          # changes apply to the x-axis
         which='both',      # both major and minor ticks are affected
         direction = 'in',
         bottom=True,      # ticks along the bottom edge are off
         top=True,         # ticks along the top edge are off
@@ -833,167 +967,165 @@
 
 
     plt.ylabel('SBR \n (Jy km s$^{-1}$ arcsec$^{-2}$)',**labelfont)
     plt.xlabel('Radius (arcsec)',**labelfont)
 
     jymin,jymax = ax_SBR.get_ylim()
     sec_ax = ax_SBR.twinx()
-    sec_ax.set_ylim(columndensity(Configuration,jymin*1000.,arcsquare = True)/1e20,columndensity(Configuration,jymax*1000.,arcsquare = True)/1e20)
+    sec_ax.set_ylim(sf.columndensity(Configuration,jymin*1000.,arcsquare = True)/1e20,sf.columndensity(Configuration,jymax*1000.,arcsquare = True)/1e20)
     sec_ax.set_ylabel('Col. Dens. \n (x10$^{20}$ cm$^{-2}$)',rotation=-90,va='bottom',**labelfont)
     sec_ax.figure.canvas.draw()
     if 'SBR' in Configuration['FIXED_PARAMETERS'][0]:
         ax_SBR.text(1.25,0.5,'Forced Gaussian',rotation=-90, va='center',ha='left', color='black',transform = ax_SBR.transAxes,
-          bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=10)
+          bbox=dict(facecolor='white',edgecolor='white',pad=0.,alpha=0.),zorder=7,fontsize=10*size_factor)
     sec_ax = ax_SBR.twiny()
     arcmin,arcmax = ax_SBR.get_xlim()
     sec_ax.set_xticklabels([])
-    sec_ax.set_xlim(convertskyangle(Configuration,arcmin,Configuration['DISTANCE']),convertskyangle(Configuration,arcmax,Configuration['DISTANCE']))
+    sec_ax.set_xlim(sf.convertskyangle(Configuration,arcmin),sf.convertskyangle(Configuration,arcmax))
     sec_ax.figure.canvas.draw()
 
 
 #----------------------------------------------Distance vs VSYS -----------------------------------------
     ax_VSYS = Overview.add_subplot(gs[2:6,16:20])
     plt.xlabel('Sys. Vel. (km s$^{-1}$)',**labelfont)
     plt.ylabel('Distance (Mpc)',**labelfont)
 
-    plt.errorbar(float(FAT_Model[0,Vars_to_plot.index('VSYS')]),float(Configuration['DISTANCE'])\
-                ,xerr=float(FAT_Model[0,Vars_to_plot.index('VSYS_ERR')]), c='k',zorder= 3,fmt="o")
+    plt.errorbar(float(FAT_Model[Vars_to_plot.index('VSYS'),0]),float(Configuration['DISTANCE'])\
+                ,xerr=float(FAT_Model[Vars_to_plot.index('# VSYS_ERR'),0]), c='k',zorder= 3,fmt="o")
     #plt.scatter(float(FAT_Model[0,Vars_to_plot.index('VSYS')]),float(Configuration['DISTANCE']),c='k',zorder= 3)
     if len(Extra_Model) > 0:
-        plt.scatter(float(Extra_Model[0,Vars_to_plot.index('VSYS')]),float(Configuration['DISTANCE']),c='r',alpha = 0.5,zorder=1)
+        plt.scatter(float(Extra_Model[Vars_to_plot.index('VSYS'),0]),float(Configuration['DISTANCE']),c='r',alpha = 0.5,zorder=1)
     if len(Input_Model) > 0:
-        plt.scatter(float(Input_Model[0,Vars_to_plot.index('VSYS')]),float(Configuration['DISTANCE']),c='b',zorder= 2)
+        plt.scatter(float(Input_Model[Vars_to_plot.index('VSYS'),0]),float(Configuration['DISTANCE']),c='b',zorder= 2)
     plt.scatter(sof_basic_vsys[0],float(Configuration['DISTANCE']),marker='x',alpha=0.5, c = 'k')
     xmin,xmax = ax_VSYS.get_xlim()
     ymin,ymax = ax_VSYS.get_ylim()
 
     #plt.scatter(sof_basic_vsys[0],float(Configuration['DISTANCE']),marker='x',alpha=0.5, c = 'k')
     vall= np.linspace(0,15000,100)
     Distanc=vall/70.
     plt.plot(vall,Distanc,'k--',alpha=0.5)
     ax_VSYS.set_xlim(xmin, xmax)
-    left = float(FAT_Model[0,Vars_to_plot.index('VSYS')])-cube[0].header['CDELT3']/2000.
+    left = float(FAT_Model[Vars_to_plot.index('VSYS'),0])-cube[0].header['CDELT3']/2000.
     bottom = ymin-5
     width =  cube[0].header['CDELT3']/1000.
     height = ymax-ymin+50
 #plt.fill([sof_basic_vsys[0]-Cube[0].header['CDELT3']/2000.,sof_basic_vsys[0]+Cube[0].header['CDELT3']/2000.],[ymin-50,ymax+50],c='k',alpha=0.5)
     why = plt.Rectangle((left,bottom), width,height,facecolor='black',alpha=0.4 , zorder=1)
     ax_VSYS.add_patch(why)
     ax_VSYS.set_ylim(ymin, ymax)
 #----------------------------------------------RA vs DEC -----------------------------------------
     ax_RAD = Overview.add_subplot(gs[8:12,16:20])
 
-    plt.errorbar(float(FAT_Model[0,Vars_to_plot.index('XPOS')]),\
-                 float(FAT_Model[0,Vars_to_plot.index('YPOS')]),
-                xerr=float(FAT_Model[0,Vars_to_plot.index('XPOS_ERR')]),\
-                yerr=float(FAT_Model[0,Vars_to_plot.index('YPOS_ERR')]), c='k',zorder= 3,fmt="o")
+    plt.errorbar(float(FAT_Model[Vars_to_plot.index('XPOS'),0]),\
+                 float(FAT_Model[Vars_to_plot.index('YPOS'),0]),
+                xerr=float(FAT_Model[Vars_to_plot.index('# XPOS_ERR'),0]),\
+                yerr=float(FAT_Model[Vars_to_plot.index('# YPOS_ERR'),0]), c='k',zorder= 3,fmt="o")
 
-    plt.scatter(float(FAT_Model[0,Vars_to_plot.index('XPOS')]),float(FAT_Model[0,Vars_to_plot.index('YPOS')]),c='k',zorder=3,label = 'Final')
+    plt.scatter(float(FAT_Model[Vars_to_plot.index('XPOS'),0]),float(FAT_Model[Vars_to_plot.index('YPOS'),0]),c='k',zorder=3,label = 'Final')
     if len(Extra_Model) > 0:
         lab = 'Unsmoothed'
         alpha =0.5
-        plt.scatter(float(Extra_Model[0,Vars_to_plot.index('XPOS')]),float(Extra_Model[0,Vars_to_plot.index('YPOS')]),c='r',zorder=1,alpha=alpha,label=lab)
+        plt.scatter(float(Extra_Model[Vars_to_plot.index('XPOS'),0]),float(Extra_Model[Vars_to_plot.index('YPOS'),0]),c='r',zorder=1,alpha=alpha,label=lab)
     if len(Input_Model) > 0:
-        plt.scatter(float(Input_Model[0,Vars_to_plot.index('XPOS')]),float(Input_Model[0,Vars_to_plot.index('YPOS')]),c='b',zorder =2,label='Input')
+        plt.scatter(float(Input_Model[Vars_to_plot.index('XPOS'),0]),float(Input_Model[Vars_to_plot.index('YPOS'),0]),c='b',zorder =2,label='Input')
     plt.scatter(sof_basic_ra[0],sof_basic_dec[0],marker='x',alpha=0.5, c = 'k',label='Initial')
-    mod_ell = Ellipse(xy=[float(FAT_Model[0,Vars_to_plot.index('XPOS')]),float(FAT_Model[0,Vars_to_plot.index('YPOS')])], width=cube[0].header['BMAJ'] , height=cube[0].header['BMAJ'], angle=0,
+    mod_ell = Ellipse(xy=[float(FAT_Model[Vars_to_plot.index('XPOS'),0]),float(FAT_Model[Vars_to_plot.index('YPOS'),0])], width=cube[0].header['BMAJ'] , height=cube[0].header['BMAJ'], angle=0,
                edgecolor='none', alpha=0.4, lw=4, facecolor='k', hatch = None, zorder=-1)
     ax_RAD.add_patch(mod_ell)
     ax_RAD.legend(loc='upper left', bbox_to_anchor=(0.0, -0.3), shadow=True, ncol=1)
     plt.xlabel('RA ($^{\circ}$)',**labelfont)
     plt.ylabel('DEC ($^{\circ}$)',**labelfont)
     cube_mod.close()
     cube.close()
     channels_map.close()
-
     plt.savefig(f"{Configuration['FITTING_DIR']}Overview.png", bbox_inches='tight')
+    #plt.savefig(f"Overview_Test.png", bbox_inches='tight')
     plt.close()
 
 make_overview_plot.__doc__ =f'''
  NAME:
-    make_overview_plot(Configuration,Fits_Files, debug = False):
+    make_overview_plot(Configuration,Fits_Files ):
 
  PURPOSE:
     Create a plot that shows the various stages of the fitting and output in a handy overview
 
  CATEGORY:
     write_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     Fits_Files = Locations of the Fits files used by FAT
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     The overview plot
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
 def plot_parameters(Configuration,Vars_to_plot,FAT_Model,location,Figure,parameter,\
                     Input_Model = [],legend = ['Empty','Empty','Empty','Empty'],
-                    initial = None, initial_extent=  None, Extra_Model = [], debug = False):
-    if debug:
-        print_log(f'''PLOT_PARAMETERS: We are starting to plot {parameter}
-''', Configuration['OUTPUTLOG'], debug = True)
+                    initial = None, initial_extent=  None, Extra_Model = [] ):
+    sf.print_log(f'''PLOT_PARAMETERS: We are starting to plot {parameter}
+''', Configuration,case=['debug_start'])
     ax = Figure.add_subplot(location)
     try:
-        yerr = FAT_Model[:,Vars_to_plot.index(f'{parameter}_ERR')]
-    except:
-        yerr =np.zeros(len(FAT_Model[:,Vars_to_plot.index('RADI')]))
-    if debug:
-        print_log(f'''PLOT_PARAMETERS: We found these errors {yerr}
-''', Configuration['OUTPUTLOG'])
-
-    ax.errorbar(FAT_Model[:,Vars_to_plot.index('RADI')],FAT_Model[:,Vars_to_plot.index(f'{parameter}')],yerr= yerr, c ='k', label=f'{legend[0]}',zorder=3)
-    ax.plot(FAT_Model[:,Vars_to_plot.index('RADI')],FAT_Model[:,Vars_to_plot.index(f'{parameter}')],'ko', ms = 3.,zorder=3)
-    if np.sum(FAT_Model[:,Vars_to_plot.index(f'{parameter}_2')]) != 0.:
-        diff = np.sum(abs(FAT_Model[:,Vars_to_plot.index(f'{parameter}_2')]-FAT_Model[:,Vars_to_plot.index(f'{parameter}')]))
+        yerr = FAT_Model[Vars_to_plot.index(f'# {parameter}_ERR'),:]
+    except ValueError:
+        yerr =np.zeros(len(FAT_Model[Vars_to_plot.index('RADI'),:]))
+    sf.print_log(f'''PLOT_PARAMETERS: We found these errors {yerr}
+''', Configuration,case=['debug_add'])
+
+    ax.errorbar(FAT_Model[Vars_to_plot.index('RADI'),:],FAT_Model[Vars_to_plot.index(f'{parameter}'),:],yerr= yerr, c ='k', label=f'{legend[0]}',zorder=3)
+    ax.plot(FAT_Model[Vars_to_plot.index('RADI'),:],FAT_Model[Vars_to_plot.index(f'{parameter}'),:],'ko', ms = 3.,zorder=3)
+    if np.sum(FAT_Model[Vars_to_plot.index(f'{parameter}_2'),:]) != 0.:
+        diff = np.sum(abs(FAT_Model[Vars_to_plot.index(f'{parameter}_2'),:]-FAT_Model[Vars_to_plot.index(f'{parameter}'),:]))
         if diff != 0.:
             try:
-                yerr = FAT_Model[:,Vars_to_plot.index(f'{parameter}_2_ERR')]
-            except:
-                yerr =np.zeros(len(FAT_Model[:,Vars_to_plot.index('RADI')]))
-            ax.errorbar(FAT_Model[:,Vars_to_plot.index('RADI')],FAT_Model[:,Vars_to_plot.index(f'{parameter}_2')],yerr= yerr, c ='r', label=f'{legend[1]}',zorder=3)
-            ax.plot(FAT_Model[:,Vars_to_plot.index('RADI')],FAT_Model[:,Vars_to_plot.index(f'{parameter}_2')],'ro', ms = 3.,zorder=3)
+                yerr = FAT_Model[Vars_to_plot.index(f'# {parameter}_2_ERR'),:]
+            except ValueError:
+                yerr =np.zeros(len(FAT_Model[Vars_to_plot.index('RADI'),:]))
+            ax.errorbar(FAT_Model[Vars_to_plot.index('RADI'),:],FAT_Model[Vars_to_plot.index(f'{parameter}_2'),:],yerr= yerr, c ='r', label=f'{legend[1]}',zorder=3)
+            ax.plot(FAT_Model[Vars_to_plot.index('RADI'),:],FAT_Model[Vars_to_plot.index(f'{parameter}_2'),:],'ro', ms = 3.,zorder=3)
 
     if len(Input_Model) > 0:
-        if np.sum(Input_Model[:,Vars_to_plot.index(f'{parameter}')]) != 0.:
-            last_index = int(np.where(Input_Model[:,Vars_to_plot.index(f'{parameter}')] != 0.)[0][-1])
+        if np.sum(Input_Model[Vars_to_plot.index(f'{parameter}'),:]) != 0.:
+            last_index = int(np.where(Input_Model[Vars_to_plot.index(f'{parameter}'),:] != 0.)[0][-1])
             try:
-                yerr = Input_Model[:last_index,Vars_to_plot.index(f'# {parameter}_ERR')]
-            except:
-                yerr =np.zeros(len(Input_Model[:last_index,Vars_to_plot.index('RADI')]))
-            ax.errorbar(Input_Model[:last_index,Vars_to_plot.index('RADI')],Input_Model[:last_index,Vars_to_plot.index(f'{parameter}')],yerr= yerr, c ='b',linestyle='-', label=f'{legend[2]}',zorder=2)
-            ax.plot(Input_Model[:last_index,Vars_to_plot.index('RADI')],Input_Model[:last_index,Vars_to_plot.index(f'{parameter}')],'bo',linestyle='-', ms = 3.,zorder=2)
-        if np.sum(Input_Model[:,Vars_to_plot.index(f'{parameter}_2')]) != 0.:
-            diff = np.sum(abs(Input_Model[:,Vars_to_plot.index(f'{parameter}_2')]-Input_Model[:,Vars_to_plot.index(f'{parameter}')]))
+                yerr = Input_Model[Vars_to_plot.index(f'# {parameter}_ERR'),:last_index]
+            except ValueError:
+                yerr =np.zeros(len(Input_Model[Vars_to_plot.index('RADI'),:last_index]))
+            ax.errorbar(Input_Model[Vars_to_plot.index('RADI'),:last_index],Input_Model[Vars_to_plot.index(f'{parameter}'),:last_index],yerr= yerr, c ='b',linestyle='-', label=f'{legend[2]}',zorder=2)
+            ax.plot(Input_Model[Vars_to_plot.index('RADI'),:last_index],Input_Model[Vars_to_plot.index(f'{parameter}'),:last_index],'bo',linestyle='-', ms = 3.,zorder=2)
+        if np.sum(Input_Model[Vars_to_plot.index(f'{parameter}_2'),:]) != 0.:
+            diff = np.sum(abs(Input_Model[Vars_to_plot.index(f'{parameter}_2'),:]-Input_Model[Vars_to_plot.index(f'{parameter}'),:]))
             if diff != 0.:
-                last_index = int(np.where(Input_Model[:,Vars_to_plot.index(f'{parameter}_2')] != 0.)[0][-1])
-                try:
-                    yerr = Input_Model[:last_index,Vars_to_plot.index(f'# {parameter}_2_ERR')]
-                except:
-                    yerr =np.zeros(len(Input_Model[:last_index,Vars_to_plot.index('RADI')]))
+                last_index = int(np.where(Input_Model[Vars_to_plot.index(f'{parameter}_2'),:] != 0.)[0][-1])
+                try: ###### Keep swapping indices
+                    yerr = Input_Model[Vars_to_plot.index(f'# {parameter}_2_ERR'),:last_index]
+                except ValueError:
+                    yerr =np.zeros(len(Input_Model[Vars_to_plot.index('RADI'),:last_index]))
 
-                ax.errorbar(Input_Model[:last_index,Vars_to_plot.index('RADI')],Input_Model[:last_index,Vars_to_plot.index(f'{parameter}_2')],yerr= yerr, c ='yellow', label=f'{legend[3]}',zorder=2)
-                ax.plot(Input_Model[:last_index,Vars_to_plot.index('RADI')],Input_Model[:last_index,Vars_to_plot.index(f'{parameter}_2')],'yellow',zorder=2,marker ='o',linestyle='-' , ms = 3.)
+                ax.errorbar(Input_Model[Vars_to_plot.index('RADI'),:last_index],Input_Model[Vars_to_plot.index(f'{parameter}_2'),:last_index],yerr= yerr, c ='yellow', label=f'{legend[3]}',zorder=2)
+                ax.plot(Input_Model[Vars_to_plot.index('RADI'),:last_index,],Input_Model[Vars_to_plot.index(f'{parameter}_2'),:last_index],'yellow',zorder=2,marker ='o',linestyle='-' , ms = 3.)
     ymin,ymax = ax.get_ylim()
     if len(Extra_Model) > 0:
-        ax.plot(Extra_Model[:,Vars_to_plot.index('RADI')],Extra_Model[:,Vars_to_plot.index(f'{parameter}')],'ko',linestyle='-', ms = 3., alpha=0.2,zorder=1)
-        if np.sum(Extra_Model[:,Vars_to_plot.index(f'{parameter}_2')]) != 0.:
-            diff = np.sum(abs(Extra_Model[:,Vars_to_plot.index(f'{parameter}_2')]-Extra_Model[:,Vars_to_plot.index(f'{parameter}')]))
+        ax.plot(Extra_Model[Vars_to_plot.index('RADI'),:],Extra_Model[Vars_to_plot.index(f'{parameter}'),:],'ko',linestyle='-', ms = 3., alpha=0.2,zorder=1)
+        if np.sum(Extra_Model[Vars_to_plot.index(f'{parameter}_2'),:]) != 0.:
+            diff = np.sum(abs(Extra_Model[Vars_to_plot.index(f'{parameter}_2'),:]-Extra_Model[Vars_to_plot.index(f'{parameter}'),:]))
             if diff != 0.:
-                ax.plot(Extra_Model[:,Vars_to_plot.index('RADI')],Extra_Model[:,Vars_to_plot.index(f'{parameter}_2')],'r', alpha=0.2,zorder=1,marker ='o',linestyle='-' , ms = 3.)
+                ax.plot(Extra_Model[Vars_to_plot.index('RADI'),:],Extra_Model[Vars_to_plot.index(f'{parameter}_2'),:],'r', alpha=0.2,zorder=1,marker ='o',linestyle='-' , ms = 3.)
     xmin,xmax = ax.get_xlim()
     if initial:
         ax.plot([xmin-5,xmax+5],[float(initial),float(initial)],c='k',alpha=0.4, linestyle ='--')
     if initial_extent:
         ax.plot([float(initial_extent)/2.,float(initial_extent)/2.],[ymin-5,ymax+5],c='k',alpha=0.4, linestyle ='--')
     ax.set_xlim(xmin,xmax)
     ax.set_ylim(ymin,ymax)
@@ -1014,15 +1146,15 @@
         Vars_to_plot =List with order of the variables in the FAT_Model
         FAT_Model = Array with the values for all parameters
         location = location in the figure where to put this subplot
         Figure = the figure in which we are plotting
         parameter = the parameter to plot
 
      OPTIONAL INPUTS:
-        debug = False
+
 
         Input_Model = []
         A model to compare to, should be ordered the same as the FAT_Model
 
         legend = ['Empty','Empty','Empty','Empty']
         legend names for fat_model and Input model
 
@@ -1039,21 +1171,28 @@
 
      PROCEDURES CALLED:
         Unspecified
 
      NOTE:
 '''
 
-def plot_usage_stats(Configuration,debug = False):
+
+
+def plot_usage_stats(Configuration ):
     with open(f"{Configuration['LOG_DIRECTORY']}Usage_Statistics.txt") as file:
         lines = file.readlines()
 
     labels = {'FAT': {'label':[], 'Time':[]}, 'Tirific':{'label':[], 'Time':[]}}
     loads = {'FAT':{'CPU':[],'MEM':[],'Time':[]},'Tirific':{'CPU':[],'MEM':[],'Time': []}}
-    labelfont = {'family': 'Times New Roman',
+    try:
+        mpl_fm.fontManager.addfont(Configuration['FONT_FILE'])
+        font_name = mpl_fm.FontProperties(fname=Configuration['FONT_FILE']).get_name()
+    except FileNotFoundError:
+        font_name = 'DejaVu Sans'
+    labelfont = {'family': font_name,
              'weight': 'normal',
              'size': 4}
     current_stage = 'Not_Found'
     current_module = 'Unknown'
     startdate = 0
     for line in lines:
         line = line.strip()
@@ -1108,97 +1247,120 @@
         }
         comb_list= labels['Tirific']['Time']+labels['FAT']['Time']
         comb_label = labels['Tirific']['label']+labels['FAT']['label']
 
         labels_times=np.array([x for x, _ in sorted(zip(comb_list, comb_label))],dtype=float)
         labels_comb = [x for _, x in sorted(zip(comb_list, comb_label))]
 
-        fig, ax1 = plt.subplots(figsize = (8,4))
-        fig.subplots_adjust(left = 0.1, right = 0.9, bottom = 0.15, top = 0.7)
+        fig, ax1 = plt.subplots(figsize = (8,6))
+        fig.subplots_adjust(left = 0.1, right = 0.9, bottom = 0.3, top = 0.7)
 
 
         ax1.plot(combined_time,combined_loads['Tirific']['MEM'],'b-',lw=0.5)
         ax1.plot(combined_time,combined_loads['FAT']['MEM'],'b--',lw=0.5)
         ax1.set_ylim(0,np.max([combined_loads['Tirific']['MEM'],combined_loads['FAT']['MEM']]) \
                       +np.max([combined_loads['Tirific']['MEM'],combined_loads['FAT']['MEM']])/10.)
         ax1.set_ylabel('RAM (Mb) ', color='b')
         ax1.tick_params(axis='y', labelcolor='b')
-        ax1.set_xlabel('time (min)', color='k')
+        ax1.set_xlabel('time (min)', color='k',zorder=5)
         ax2 = ax1.twinx()
         ax2.plot(combined_time,combined_loads['Tirific']['CPU'],'r-',lw=0.5)
+        ax2.plot(combined_time,combined_loads['FAT']['CPU'],'r--',lw=0.5)
         #ax2.plot(combined_time,combined_loads['FAT']['CPU'],'r--',lw=0.5)
         ax2.set_ylabel('CPUs (%)',color='r')
         ax2miny,ax2maxy = ax2.get_ylim()
         ax2.tick_params(axis='y', labelcolor='r')
         last_label = -100
         label_sep = combined_time[-1]/30.
         color, linest = '0.5', '--'
-        labelfont = {'family': 'Times New Roman',
+        labelfont = {'family': font_name,
                  'weight': 'normal',
                  'size': 6.5}
         prev_label = ''
+
+        last_label_top = 0.
+        last_label_bottom = 0.
         #for label,time in zip(labels['Tirific']['label'],labels['Tirific']['Time']):
         for label,time in zip(labels_comb,labels_times):
 
             if label in labels['Tirific']['label']:
-                offset =20.
-            else:
-                offset = 50.
-            if color == '0.5':
+                offset = 20.
+                xoffset = 0.05
+                vertical_start = ax2maxy
+                va= 'bottom'
+                ha= 'left'
                 color = 'k'
-            elif color == 'k':
-                color = '0.5'
-            if linest == '--':
                 linest = '-'
-            elif linest == '-':
+            else:
+                offset=-50
+                xoffset = 0.025
+                vertical_start = ax2miny
+                va= 'top'
+                ha='right'
+                color = '0.5'
                 linest = '--'
 
+
             if (prev_label == 'Initializing tmp_incl_check' or prev_label == 'Ended tmp_incl_check'):
                 if (label != 'Initializing tmp_incl_check' and label != 'Ended tmp_incl_check') or \
                         time == labels_times[-1]    :
 
                     if time != labels_times[-1]:
                         ax2.axvline(x=prev_time, linestyle=linest, color=color, linewidth=0.05)
-                        last_label = max(prev_time,last_label+label_sep)
-                        ax2.text(last_label,ax2maxy+offset,prev_label, va='bottom',ha='left',rotation= 60, color='black',
+                        if label in labels['Tirific']['label']:
+                            last_label = last_label_top = max(prev_time,last_label_top+label_sep)
+                        else:
+                            last_label = last_label_bottom = max(prev_time,last_label_bottom+label_sep)
+                        ax2.text(last_label,vertical_start+offset,prev_label, va=va,ha=ha,rotation= 60, color='black',
                               bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
-                        ax2.plot([prev_time,last_label+0.1],[ax2maxy,ax2maxy+offset],linest,color=color,linewidth=0.05,clip_on=False)
+                        ax2.plot([prev_time,last_label+xoffset],[vertical_start,vertical_start+offset],linest,color=color,linewidth=0.05,clip_on=False)
                     ax2.axvline(x=time, linestyle=linest, color=color, linewidth=0.05)
-                    last_label = max(time,last_label+label_sep)
-                    ax2.text(last_label,ax2maxy+offset,label, va='bottom',ha='left',rotation= 60, color='black',
+                    if label in labels['Tirific']['label']:
+                        last_label = last_label_top = max(time,last_label_top+label_sep)
+                    else:
+                        last_label = last_label_bottom = max(time,last_label_bottom+label_sep)
+                    ax2.text(last_label,vertical_start+offset,label, va=va,ha=ha,rotation= 60, color='black',
                           bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
-                    ax2.plot([time,last_label+0.1],[ax2maxy,ax2maxy+offset],linest,color=color,linewidth=0.05,clip_on=False)
+                    ax2.plot([time,last_label+xoffset],[vertical_start,vertical_start+offset],linest,color=color,linewidth=0.05,clip_on=False)
                 else:
                     prev_time = time
             elif (prev_label == 'Initializing Error_Shaker' or prev_label == 'Ended Error_Shaker' or prev_label == 'Started Error_Shaker'):
                 if (label != 'Initializing Error_Shaker' and label != 'Ended Error_Shaker' and  label != 'Started Error_Shaker') or \
                         time == labels_times[-1]:
 
                     #ax2.axvline(x=prev_time, linestyle=linest, color=color, linewidth=0.05)
                     #last_label = max(prev_time,last_label+label_sep)
                     #ax2.text(last_label,ax2maxy+20.,prev_label, va='bottom',ha='left',rotation= 60, color='black',
                     #      bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
                     #ax2.plot([prev_time,last_label+0.1],[ax2maxy,ax2maxy+20.],linest,color=color,linewidth=0.05,clip_on=False)
                     ax2.axvline(x=time, linestyle=linest, color=color, linewidth=0.05)
-                    last_label = max(time,last_label+label_sep)
-                    ax2.text(last_label,ax2maxy+offset,label, va='bottom',ha='left',rotation= 60, color='black',
+                    if label in labels['Tirific']['label']:
+                        last_label = last_label_top = max(time,last_label_top+label_sep)
+                    else:
+                        last_label = last_label_bottom = max(time,last_label_bottom+label_sep)
+                    ax2.text(last_label,vertical_start+offset,label, va=va,ha=ha,rotation= 60, color='black',
                           bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
-                    ax2.plot([time,last_label+0.1],[ax2maxy,ax2maxy+offset],linest,color=color,linewidth=0.05,clip_on=False)
+                    ax2.plot([time,last_label+xoffset],[vertical_start,vertical_start+offset],linest,color=color,linewidth=0.05,clip_on=False)
                 else:
                     prev_label = label
                     prev_time = time
             else:
                 ax2.axvline(x=time, linestyle=linest, color=color, linewidth=0.05)
-                last_label = max(time,last_label+label_sep)
-                ax2.text(last_label,ax2maxy+offset,label, va='bottom',ha='left',rotation= 60, color='black',
+                if label in labels['Tirific']['label']:
+                    last_label = last_label_top = max(time,last_label_top+label_sep)
+                else:
+                    last_label = last_label_bottom= max(time,last_label_bottom+label_sep)
+                ax2.text(last_label,vertical_start+offset,label,va=va,ha=ha,rotation= 60, color='black',
                       bbox=dict(facecolor='white',edgecolor='white',pad= 0.,alpha=0.),zorder=7,fontdict = labelfont)
-                ax2.plot([time,last_label+0.1],[ax2maxy,ax2maxy+offset],linest,color=color,linewidth=0.05,clip_on=False)
+                #This should be the line to the label
+                ax2.plot([time,last_label+xoffset],[vertical_start,vertical_start+offset],linest,color=color,linewidth=0.05,clip_on=False)
             prev_label = label
 
 
+
         #This is beyond stupid again, but hey it is python so needed to make things work.
         ax2.set_ylim([ax2miny,ax2maxy])
         fig.savefig(f"{Configuration['LOG_DIRECTORY']}ram_cpu.pdf")
         plt.close()
 
 plot_usage_stats.__doc__ =f'''
  NAME:
@@ -1210,27 +1372,83 @@
  CATEGORY:
     write_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
 
  OPTIONAL INPUTS:
-    debug = False
+
 
  OUTPUTS:
     ram_cpu.pdf in the Logs directory
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
+def reorder_output_catalogue(Configuration,Full_Catalogue):
+    #Read in the output catalogue
+    with open(Configuration['OUTPUT_CATALOGUE']) as file:
+        lines = file.readlines()
+    #Determine column sizes
+    header = lines[0]
+    output = lines[1:]
+    #IDs cannot have spaces
+    outputIDs = []
+    for line in output:
+        outputIDs.append(line.split()[0].strip())
+    #Sort based on the inpu IDs
+    with open(Configuration['OUTPUT_CATALOGUE'],'w') as file:
+        file.write(header)
+        for galaxy in Full_Catalogue['DIRECTORYNAME']:
+            print(galaxy)
+            try:
+                index_no = np.where(galaxy == \
+                    np.array(outputIDs))[0][0]
+                print(index_no)
+                file.write(output[index_no])
+            except IndexError:
+                pass
+
+
+
+
+reorder_output_catalogue.__doc__ =f'''
+ NAME:
+    reorder_output_catalogue
+
+ PURPOSE:
+    When running in multiprocessing mode the output catalogue can be
+    in a different order as the input. This function makes sure the are sorted
+
+ CATEGORY:
+    write_functions
+
+ INPUTS:
+    Configuration = Standard FAT configuration
+    Full_Catalogue = Full input catalogue
+
+ OPTIONAL INPUTS:
+
+
+ OUTPUTS:
+    reorder output catalogue
+
+ OPTIONAL OUTPUTS:
+
+ PROCEDURES CALLED:
+    Unspecified
+
+ NOTE:
+'''
+
 def extract_date(string):
     tmp = string.split(' ')
     tmp2 = tmp[0].split('-')
     if len(tmp2) == 3:
         try:
             date =  datetime.strptime(f"{tmp[0]} {tmp[1]}", '%Y-%m-%d %H:%M:%S.%f')
         except ValueError:
@@ -1267,22 +1485,26 @@
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
 '''
 
-def tirific(Configuration,Tirific_Template, name = 'tirific.def', debug = False):
+def tirific(Configuration,Tirific_Template, name = 'tirific.def', full_name = False  ):
     #IF we're writing we bump up the restart_ID and adjust the AZ1P angles to the current warping
-    update_disk_angles(Configuration,Tirific_Template, debug= debug)
+    update_disk_angles(Configuration,Tirific_Template )
     try:
         Tirific_Template['RESTARTID'] = str(int(Tirific_Template['RESTARTID'])+1)
-    except:
+    except ValueError:
         Tirific_Template['RESTARTID'] = 0
-    with open(Configuration['FITTING_DIR']+name, 'w') as file:
+    if full_name:
+        file_name = name
+    else:
+        file_name = f'{Configuration["FITTING_DIR"]}{name}'
+    with open(file_name, 'w') as file:
         for key in Tirific_Template:
             if key[0:5] == 'EMPTY':
                 file.write('\n')
             else:
                 file.write((f"{key}= {Tirific_Template[key]} \n"))
 tirific.__doc__ =f'''
  NAME:
@@ -1295,60 +1517,22 @@
     write_functions
 
  INPUTS:
     Configuration = Standard FAT configuration
     Tirific_Template = Standard FAT Tirific Template
 
  OPTIONAL INPUTS:
-    debug = False
+
 
     name = 'tirific.def'
     name of the file to write to
 
  OUTPUTS:
     Tirific def file
 
  OPTIONAL OUTPUTS:
 
  PROCEDURES CALLED:
     Unspecified
 
  NOTE:
  '''
-
-
-def write_config(file,Configuration,debug = False):
-    if debug:
-        print_log(f'''WRITE_CONFIG: writing the configuration to {file}
-''',Configuration['OUTPUTLOG'], screen = True)
-    # Separate the keyword names
-    with open(file,'w') as tmp:
-        for key in Configuration:
-            tmp.write(f'{key} = {Configuration[key]} \n')
-
-write_config.__doc__ =f'''
- NAME:
-    write_config
-
- PURPOSE:
-    Write a config file to the fitting directory.
-
- CATEGORY:
-    write_functions
-
- INPUTS:
-    file = name of the file to write to
-    Configuration = Standard FAT configuration
-
- OPTIONAL INPUTS:
-    debug = False
-
- OUTPUTS:
-    A FAT config file.
-
- OPTIONAL OUTPUTS:
-
- PROCEDURES CALLED:
-    Unspecified
-
- NOTE:
-'''
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/Templates/sofia_template.par` & `pyFAT_astro-0.1.1/pyFAT_astro/Templates/sofia_template.par`

 * *Files 6% similar despite different names*

```diff
@@ -48,14 +48,19 @@
 
 # S+C finder
 
 scfind.kernelsXY =  0, 4, 8
 scfind.kernelsZ =  2, 4, 8, 16
 scfind.threshold =  5.0
 
+# Dilation
+
+dilation.enable = True
+dilation.iterationsZ = 1
+
 # Linker
 
 linker.radiusXY = 3
 linker.radiusZ = 3
 linker.minSizeXY = 6
 linker.minSizeZ = 8
 linker.positivity = True
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/__init__.py` & `pyFAT_astro-0.1.1/pyFAT_astro/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -30,9 +30,25 @@
             result = None
         if result != None and 'fatal' not in result:
             return __version__+'-'+result
         else:
             # we are probably in an installed version
             return __version__
 
+def report_branch():
+    path = os.path.dirname(os.path.abspath(__file__))
+    result = None
+    try:
+        branches = subprocess.check_output(\
+            'cd %s; git branch' % path, shell=True, stderr=subprocess.STDOUT).rstrip().decode().split()
+        for i,line in enumerate(branches):
+            if line == '*':
+                result=branches[i+1]
+                break
+    except subprocess.CalledProcessError:
+        result= None
+    return result
 
 __version__ = report_version()
+__branch__ =report_branch()
+
+#set_logger_values()
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro/config/defaults.py` & `pyFAT_astro-0.1.1/pyFAT_astro/config/defaults.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,83 +1,120 @@
 # -*- coding: future_fstrings -*-
 
-from dataclasses import dataclass,field
 import omegaconf
-from omegaconf import MISSING
-from typing import List,Optional
 import os
+import pyFAT_astro
+from dataclasses import dataclass, field
 from datetime import datetime
+from omegaconf import MISSING
+#from multiprocessing import cpu_count
+from psutil import cpu_count
+from typing import List, Optional
+
 
 @dataclass
 class Fitting:
 
-
-    catalogue_start_id: str = '-1' #Catalogue ID of the first galaxy to be fitted. -1 Means start at the beginning
-    catalogue_end_id: str = '-1' #the last galaxy to be fitted, if set to -1 the whole catalogue will be fitted
-    fitting_stages: List = field(default_factory=lambda: ['Create_FAT_Cube','Run_Sofia','Fit_Tirific_OSC'])
+    # Catalogue ID of the first galaxy to be fitted. -1 Means start at the beginning
+    catalogue_start_id: str = '-1'
+    # the last galaxy to be fitted, if set to -1 the whole catalogue will be fitted
+    catalogue_end_id: str = '-1'
+    fitting_stages: List = field(default_factory=lambda: [
+                                 'Create_FAT_Cube', 'Run_Sofia', 'Fit_Tirific_OSC'])
     # Possible stages are
     # Create_FAT_Cube: Create a FAT compatible cube from the original cube. This will overwrite any previous FAT cube present. If omitted it is assumed the Cube is present in the fitting directory
     # Sofia_Catalogue: The catalogue is assumed to be a sofia catalogue and all sources in the catalogue are to be fitted
     # Run_Sofia: Run Sofia on the FAT cube and  process the output
     # Existing_Sofia: It is assumed the Sofia output exist and specified in the fitting catalogue, this means a catalogue exists for every cubelet
     # Fit_Tirific_OSC: Run FAT using the Tirific program in multiple iterations and smooth
     # Tirshaker: Bootstrap errors for the final model. This can take a long time
-    ring_size: float = 1.1 # The size of the rings in number of beams
-    fixed_parameters:  List = field(default_factory=lambda: ['Z0','XPOS','YPOS','VSYS']) #Options are INCL, PA, SDIS, SBR
-    opt_pixel_beam: int=4
-    ncpu: int = 6
-    distance: float = -1. # Distance to the galaxy, set from the catalogue at start of loop in case of batch fitting
+    ring_size: float = 1.1  # The size of the rings in number of beams
+    fixed_parameters:  List = field(default_factory=lambda: [
+                                    'Z0', 'XPOS', 'YPOS', 'VSYS'])  # Options are INCL, PA, SDIS, SBR
+    opt_pixel_beam: int = 4
+
+    distance: float = -1.  # Distance to the galaxy, set from the catalogue at start of loop in case of batch fitting
+
 
 @dataclass
 class Input:
-    main_directory: str =f'{os.getcwd()}'
-    channel_dependency: str = 'independent' #'Options are independent, sinusoidal, hanning
+    main_directory: str = f'{os.getcwd()}'
+    # 'Options are independent, sinusoidal, hanning
+    channel_dependency: str = 'independent'
     catalogue: Optional[str] = None
-    tirific: str = "tirific" #Command to call tirific
-    sofia2: str = "sofia2"   #Command to call sofia 2
+    tirific: str = "tirific"  # Command to call tirific
+    sofia2: str = "sofia2"  # Command to call sofia 2
     sofia_basename: Optional[str] = None
-    sofia_dir: Optional[str] = None #Directory of the existing Sofia output. Only used if the input catalogue is sofia or pre-processed sofia is somewhere
+    # Directory of the existing Sofia output. Only used if the input catalogue is sofia or pre-processed sofia is somewhere
+    sofia_dir: Optional[str] = None
+
 
 @dataclass
 class Output:
-    log_directory: str = f'Logs/{datetime.now().strftime("%d-%m-%Y")}' # Name of the log dir
-    log_file: str = 'Log.txt' #Name of the log file
+    # Name of the log dir
+    log_directory: str = f'Logs/{datetime.now().strftime("%d-%m-%Y")}'
+    log_file: str = 'Log.txt'  # Name of the log file
     catalogue: str = 'pyFAT_results.txt'
-    new_output: bool = True # Create all output anew
+    new_output: bool = True  # Create all output anew
     # How much output you would like to maintain for each galaxy. 0 just organize the output and keep all (This will also happen when a fit is unsuccesful, this can be a lot of files); 1 remove optimized files, log files and input files; 2  remove optimized files, log files, input files, ps files and unsmoothed files; 3 (Default) remove optimized files, log files, input files, ps files, unsmoothed files and all model fits files except the final model; 4 keep only the def files and remove all other output. 5 indicates a failed fit clean up. >6 is the same as 0. Residuals are created for all cases where the fits files are maintained.
     output_quantity: int = 3
-    warp_output: bool = False #If you want FAT to output a warp radius, tiltograms and warp radius set warp_output (Default = n)
+    # If you want FAT to output a warp radius, tiltograms and warp radius set warp_output (Default = n)
+    warp_output: bool = False
+    # The font to be used in the plots
+    font_file: str = "/usr/share/fonts/truetype/msttcorefonts/Times_New_Roman.ttf"
     debug: bool = False
     timing: bool = False
+    verbose_log: bool = False
+    verbose_screen: bool = False
 
 @dataclass
 class Advanced:
-    start_directory: str =f'{os.getcwd()}'
-    max_iterations: int=15 #The maximum number of iterations that FAT tries to calls trific bfeore it call it quits
-    loops: int =10 #The number of full loops set for tirific in a  single iteration
-    minimum_warp_size: float = 3. # if the number of beams across the major axis/2. is less than this size we will only fit a flat disc,set here.
-    minimum_rings: int = 3  # we need at least this amount of rings (Including 0 and 1/5 beam), set here
-    too_small_galaxy: float = 1. # if the number of beams across the major axis/2 is less than this we will not fit the galaxy, set here
-    unreliable_size: float = 2. #If the final diameter is smaller than this the fit is considered unreliable
-    unreliable_inclination: float = 10. #If the final inclination is below this the fit is considered unreliable
+    start_directory: str = f'{os.getcwd()}'
+    # The maximum number of iterations that FAT tries to calls trific bfeore it call it quits
+    max_iterations: int = 15
+    loops: int = 7  # The number of full loops set for tirific in a  single iteration, this is increased every time the maximum is reach upto max 15 loops
+    # if the number of beams across the major axis/2. is less than this size we will only fit a flat disc,set here.
+    minimum_warp_size: float = 3.
+    # we need at least this amount of rings (Including 0 and 1/5 beam), set here
+    minimum_rings: int = 3
+    too_small_galaxy: float = 1.  # if the number of beams across the major axis/2 is less than this we will not fit the galaxy, set here
+    unreliable_size: float = 2.  # If the final diameter is smaller than this the fit is considered unreliable
+    unreliable_inclination: float = 10.  # If the final inclination is below this the fit is considered unreliable
     shaker_iterations: int = 20
+    multiprocessing: bool = True
+    #We do not want to use too many cores per galaxy.
+    per_galaxy_ncpu: int = 4
+    catalogue_split_character: str = '|'
     # Allow for the user to set the boundaries in the fitting
-    pa_input_boundary:  List[float] = field(default_factory=lambda: [[0.,0.],[0.,0.],[0.,0.]])
-    incl_input_boundary:  List[float] = field(default_factory=lambda: [[0.,0.],[0.,0.],[0.,0.]])
-    sdis_input_boundary:  List[float] = field(default_factory=lambda: [[0.,0.],[0.,0.],[0.,0.]])
-    z0_input_boundary:  List[float] = field(default_factory=lambda: [[0.,0.],[0.,0.],[0.,0.]])
-    vsys_input_boundary:  List[float] = field(default_factory=lambda: [[0.,0.],[0.,0.],[0.,0.]])
-    xpos_input_boundary:  List[float] = field(default_factory=lambda: [[0.,0.],[0.,0.],[0.,0.]])
-    ypos_input_boundary:  List[float] = field(default_factory=lambda: [[0.,0.],[0.,0.],[0.,0.]])
-    vrot_input_boundary: List[float] = field(default_factory=lambda: [[0.,0.],[0.,0.],[0.,0.]])
+    pa_input_boundary:  List = field(
+        default_factory=lambda: [[0., 0.], [0., 0.], [0., 0.]])
+    incl_input_boundary:  List = field(
+        default_factory=lambda: [[0., 0.], [0., 0.], [0., 0.]])
+    sdis_input_boundary:  List = field(
+        default_factory=lambda: [[0., 0.], [0., 0.], [0., 0.]])
+    z0_input_boundary:  List = field(
+        default_factory=lambda: [[0., 0.], [0., 0.], [0., 0.]])
+    vsys_input_boundary:  List = field(
+        default_factory=lambda: [[0., 0.], [0., 0.], [0., 0.]])
+    xpos_input_boundary:  List = field(
+        default_factory=lambda: [[0., 0.], [0., 0.], [0., 0.]])
+    ypos_input_boundary:  List = field(
+        default_factory=lambda: [[0., 0.], [0., 0.], [0., 0.]])
+    vrot_input_boundary: List = field(
+        default_factory=lambda: [[0., 0.], [0., 0.], [0., 0.]])
+    sbr_input_boundary: List = field(
+        default_factory=lambda: [[0., 0.], [0., 0.], [0., 0.]])
 
     # Add the channel dependency, minimum inclination,
+
+
 @dataclass
 class defaults:
-    print_examples: bool=False
-    installation_check: bool=False
+    ncpu: int = cpu_count()-1
+    print_examples: bool = False
+    installation_check: bool = False
     cube_name: Optional[str] = None
     configuration_file: Optional[str] = None
     input: Input = Input()
     output: Output = Output()
     fitting: Fitting = Fitting()
     advanced: Advanced = Advanced()
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro.egg-info/PKG-INFO` & `pyFAT_astro-0.1.1/pyFAT_astro.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,17 @@
 Metadata-Version: 2.1
 Name: pyFAT-astro
-Version: 0.0.8
+Version: 0.1.1
 Summary: Development Status :: 4 - Beta
 Home-page: https://github.com/PeterKamphuis/pyFAT
 Author: P. Kamphuis
 Author-email: peterkamphuisastronomy@gmail.com
 License: GNU GPL v3
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-
-Not sure what is going wrong here.
-
```

### Comparing `pyFAT_astro-0.0.8/pyFAT_astro.egg-info/SOURCES.txt` & `pyFAT_astro-0.1.1/pyFAT_astro.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 bin/pyFAT
+pyFAT_astro/FAT_Galaxy_Loop.py
+pyFAT_astro/FAT_Galaxy_Loops.py
 pyFAT_astro/__init__.py
 pyFAT_astro/main.py
 pyFAT_astro.egg-info/PKG-INFO
 pyFAT_astro.egg-info/SOURCES.txt
 pyFAT_astro.egg-info/dependency_links.txt
 pyFAT_astro.egg-info/requires.txt
 pyFAT_astro.egg-info/top_level.txt
@@ -24,9 +26,10 @@
 pyFAT_astro/Support/run_functions.py
 pyFAT_astro/Support/support_functions.py
 pyFAT_astro/Support/tirshaker.py
 pyFAT_astro/Support/write_functions.py
 pyFAT_astro/Templates/__init__.py
 pyFAT_astro/Templates/sofia_template.par
 pyFAT_astro/Templates/template.def
+pyFAT_astro/config/FAT_Input_Catalogue.txt
 pyFAT_astro/config/__init__.py
 pyFAT_astro/config/defaults.py
```

### Comparing `pyFAT_astro-0.0.8/setup.py` & `pyFAT_astro-0.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 #!/usr/bin/env python
-
+''' This is the setup script for the pyFAT package'''
 import os
 
 try:
     from setuptools import setup
-except ImportError as e:
+except ImportError:
     from distutils.core import setup
 
 requirements = [
     'numpy>=1.14',
     'scipy',
     'astropy',
-    'omegaconf',
+    'omegaconf>=2.2.2',
     'matplotlib',
     'future-fstrings',
     'psutil',
     'importlib_resources>=3.3.0',
 ]
 
 PACKAGE_NAME = 'pyFAT_astro'
-__version__ = 'v0.0.8'
+__version__ = 'v0.1.1'
 
 
 #with open("README.md", "r") as fh:
 #    long_description = fh.read()
-long_description = "Not sure what is going wrong here."
+long_description = ""
 
 setup(name=PACKAGE_NAME,
       version=__version__,
       description="Development Status :: 4 - Beta",
       long_description=long_description,
       long_description_content_type="text/markdown",
       author="P. Kamphuis",
```

