# Comparing `tmp/scadaUtils-0.1.1.tar.gz` & `tmp/scadaUtils-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scadaUtils-0.1.1.tar", last modified: Tue Jun 13 10:20:24 2023, max compression
+gzip compressed data, was "scadaUtils-0.2.1.tar", last modified: Tue Jun 13 16:58:15 2023, max compression
```

## Comparing `scadaUtils-0.1.1.tar` & `scadaUtils-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,62 @@
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-06-13 10:20:24.351810 scadaUtils-0.1.1/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     8694 2023-06-13 10:20:24.351810 scadaUtils-0.1.1/PKG-INFO
--rw-rw-r--   0 dorian    (1000) dorian    (1000)       61 2023-05-30 12:57:17.000000 scadaUtils-0.1.1/README.rst
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-06-13 10:20:24.351810 scadaUtils-0.1.1/scadaUtils/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    14334 2023-06-07 15:05:29.000000 scadaUtils-0.1.1/scadaUtils/Conf_generator.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    28952 2023-06-07 15:05:29.000000 scadaUtils-0.1.1/scadaUtils/GAIA.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     8748 2023-03-01 13:56:36.000000 scadaUtils-0.1.1/scadaUtils/Simulators.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    20568 2023-03-01 12:46:58.000000 scadaUtils-0.1.1/scadaUtils/VersionsManager.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2023-03-01 13:56:36.000000 scadaUtils-0.1.1/scadaUtils/__init__.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)   119034 2023-06-07 15:05:29.000000 scadaUtils-0.1.1/scadaUtils/comUtils.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    13154 2023-06-07 16:09:59.000000 scadaUtils-0.1.1/scadaUtils/dashboard.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     5904 2023-03-01 13:56:36.000000 scadaUtils-0.1.1/scadaUtils/monitoring.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    17417 2023-03-01 12:46:58.000000 scadaUtils-0.1.1/scadaUtils/old_minutely_hourly.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    14124 2023-05-30 12:55:08.000000 scadaUtils-0.1.1/scadaUtils/physics.py
--rw-rw-r--   0 dorian    (1000) dorian    (1000)    38899 2023-05-30 12:55:08.000000 scadaUtils-0.1.1/scadaUtils/utils.py
-drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-06-13 10:20:24.351810 scadaUtils-0.1.1/scadaUtils.egg-info/
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     8694 2023-06-13 10:20:24.000000 scadaUtils-0.1.1/scadaUtils.egg-info/PKG-INFO
--rw-rw-r--   0 dorian    (1000) dorian    (1000)      462 2023-06-13 10:20:24.000000 scadaUtils-0.1.1/scadaUtils.egg-info/SOURCES.txt
--rw-rw-r--   0 dorian    (1000) dorian    (1000)        1 2023-06-13 10:20:24.000000 scadaUtils-0.1.1/scadaUtils.egg-info/dependency_links.txt
--rw-rw-r--   0 dorian    (1000) dorian    (1000)      227 2023-06-13 10:20:24.000000 scadaUtils-0.1.1/scadaUtils.egg-info/requires.txt
--rw-rw-r--   0 dorian    (1000) dorian    (1000)       11 2023-06-13 10:20:24.000000 scadaUtils-0.1.1/scadaUtils.egg-info/top_level.txt
--rw-rw-r--   0 dorian    (1000) dorian    (1000)       38 2023-06-13 10:20:24.351810 scadaUtils-0.1.1/setup.cfg
--rw-rw-r--   0 dorian    (1000) dorian    (1000)     1208 2023-06-13 10:06:57.000000 scadaUtils-0.1.1/setup.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-06-13 16:58:15.832521 scadaUtils-0.2.1/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     8731 2023-06-13 16:58:15.832521 scadaUtils-0.2.1/PKG-INFO
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)       61 2023-05-30 12:57:17.000000 scadaUtils-0.2.1/README.rst
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-06-13 16:58:15.804520 scadaUtils-0.2.1/scadaUtils/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    14323 2023-06-13 11:41:40.000000 scadaUtils-0.2.1/scadaUtils/Conf_generator.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    28919 2023-06-13 11:42:02.000000 scadaUtils-0.2.1/scadaUtils/GAIA.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     8748 2023-03-01 13:56:36.000000 scadaUtils-0.2.1/scadaUtils/Simulators.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    20557 2023-06-13 11:47:57.000000 scadaUtils-0.2.1/scadaUtils/VersionsManager.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)        0 2023-03-01 13:56:36.000000 scadaUtils-0.2.1/scadaUtils/__init__.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)   119023 2023-06-13 11:41:07.000000 scadaUtils-0.2.1/scadaUtils/comUtils.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-06-13 16:58:15.808520 scadaUtils-0.2.1/scadaUtils/conf/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      990 2022-08-31 12:33:04.000000 scadaUtils-0.2.1/scadaUtils/conf/colormaps.pkl
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    21562 2023-03-01 12:46:58.000000 scadaUtils-0.2.1/scadaUtils/conf/data_values.ods
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    57151 2023-03-01 12:46:58.000000 scadaUtils-0.2.1/scadaUtils/conf/logo_sylfen.png
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     9061 2022-08-31 12:33:04.000000 scadaUtils-0.2.1/scadaUtils/conf/palettes.pkl
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      500 2023-03-01 13:56:36.000000 scadaUtils-0.2.1/scadaUtils/conf/parameters.default.conf
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      854 2023-06-07 15:05:29.000000 scadaUtils-0.2.1/scadaUtils/conf/parameters_RT.default.conf
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      486 2023-03-01 13:56:36.000000 scadaUtils-0.2.1/scadaUtils/conf/units.csv
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    13132 2023-06-13 11:41:53.000000 scadaUtils-0.2.1/scadaUtils/dashboard.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     5904 2023-03-01 13:56:36.000000 scadaUtils-0.2.1/scadaUtils/monitoring.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    17417 2023-03-01 12:46:58.000000 scadaUtils-0.2.1/scadaUtils/old_minutely_hourly.py
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    14136 2023-06-13 11:47:07.000000 scadaUtils-0.2.1/scadaUtils/physics.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-06-13 16:58:15.800520 scadaUtils-0.2.1/scadaUtils/static/
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-06-13 16:58:15.808520 scadaUtils-0.2.1/scadaUtils/static/lib/
+-rwxrwxr-x   0 dorian    (1000) dorian    (1000)    38904 2023-03-01 13:56:36.000000 scadaUtils-0.2.1/scadaUtils/static/lib/acolorpicker.js
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-06-13 16:58:15.808520 scadaUtils-0.2.1/scadaUtils/static/lib/css/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      672 2022-08-31 12:33:04.000000 scadaUtils-0.2.1/scadaUtils/static/lib/css/dropdown_filter.css
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     3026 2023-03-01 13:56:36.000000 scadaUtils-0.2.1/scadaUtils/static/lib/css/styles.css
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      971 2022-08-31 12:33:04.000000 scadaUtils-0.2.1/scadaUtils/static/lib/css/toggle_switch.css
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     7659 2022-08-31 12:33:04.000000 scadaUtils-0.2.1/scadaUtils/static/lib/daterangepicker.css
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-06-13 16:58:15.820520 scadaUtils-0.2.1/scadaUtils/static/lib/js/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    14403 2023-03-01 13:56:36.000000 scadaUtils-0.2.1/scadaUtils/static/lib/js/dashboard.js
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    66264 2022-09-13 12:00:07.000000 scadaUtils-0.2.1/scadaUtils/static/lib/js/daterangepicker.js
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    89664 2022-09-13 12:00:07.000000 scadaUtils-0.2.1/scadaUtils/static/lib/js/jquery.min.js
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      212 2022-08-31 12:33:04.000000 scadaUtils-0.2.1/scadaUtils/static/lib/js/lib.js
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      190 2022-09-13 12:00:07.000000 scadaUtils-0.2.1/scadaUtils/static/lib/js/local_dash.js
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    63499 2022-09-13 12:00:07.000000 scadaUtils-0.2.1/scadaUtils/static/lib/js/mathjax.min.js
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    63499 2022-08-31 12:33:04.000000 scadaUtils-0.2.1/scadaUtils/static/lib/js/mathjax_local.js
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    59611 2022-09-13 12:00:07.000000 scadaUtils-0.2.1/scadaUtils/static/lib/js/moment.min.js
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)  3698541 2022-09-13 12:00:07.000000 scadaUtils-0.2.1/scadaUtils/static/lib/js/plotly.js
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    75208 2022-09-13 12:00:07.000000 scadaUtils-0.2.1/scadaUtils/static/lib/js/showdown.min.js
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      173 2023-03-01 13:56:36.000000 scadaUtils-0.2.1/scadaUtils/static/lib/log_versions.md
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-06-13 16:58:15.832521 scadaUtils-0.2.1/scadaUtils/static/lib/pictures/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)  3174891 2022-08-31 12:33:04.000000 scadaUtils-0.2.1/scadaUtils/static/lib/pictures/angrypainter.gif
+-rwxrwxr-x   0 dorian    (1000) dorian    (1000)    57151 2022-08-31 12:33:04.000000 scadaUtils-0.2.1/scadaUtils/static/lib/pictures/logo_sylfen.png
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    11337 2022-08-31 12:33:04.000000 scadaUtils-0.2.1/scadaUtils/static/lib/pictures/peintrepalette.jpeg
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    29974 2022-08-31 12:33:04.000000 scadaUtils-0.2.1/scadaUtils/static/lib/search.png
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      957 2022-08-31 12:33:04.000000 scadaUtils-0.2.1/scadaUtils/static/lib/search2.png
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    57459 2022-08-31 12:33:04.000000 scadaUtils-0.2.1/scadaUtils/static/lib/sylfen.png
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    19772 2022-08-31 12:33:04.000000 scadaUtils-0.2.1/scadaUtils/static/lib/sylfen_logo.ico
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-06-13 16:58:15.832521 scadaUtils-0.2.1/scadaUtils/templates/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     7127 2023-03-01 13:56:36.000000 scadaUtils-0.2.1/scadaUtils/templates/bootstrap_dash.html
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     8570 2023-03-01 13:56:36.000000 scadaUtils-0.2.1/scadaUtils/templates/dashboard.html
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)    38899 2023-05-30 12:55:08.000000 scadaUtils-0.2.1/scadaUtils/utils.py
+drwxrwxr-x   0 dorian    (1000) dorian    (1000)        0 2023-06-13 16:58:15.804520 scadaUtils-0.2.1/scadaUtils.egg-info/
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     8731 2023-06-13 16:58:15.000000 scadaUtils-0.2.1/scadaUtils.egg-info/PKG-INFO
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     1689 2023-06-13 16:58:15.000000 scadaUtils-0.2.1/scadaUtils.egg-info/SOURCES.txt
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)        1 2023-06-13 16:58:15.000000 scadaUtils-0.2.1/scadaUtils.egg-info/dependency_links.txt
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)      227 2023-06-13 16:58:15.000000 scadaUtils-0.2.1/scadaUtils.egg-info/requires.txt
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)       11 2023-06-13 16:58:15.000000 scadaUtils-0.2.1/scadaUtils.egg-info/top_level.txt
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)       38 2023-06-13 16:58:15.832521 scadaUtils-0.2.1/setup.cfg
+-rw-rw-r--   0 dorian    (1000) dorian    (1000)     1264 2023-06-13 10:25:50.000000 scadaUtils-0.2.1/setup.py
```

### Comparing `scadaUtils-0.1.1/PKG-INFO` & `scadaUtils-0.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scadaUtils
-Version: 0.1.1
+Version: 0.2.1
 Summary: Utilities package
-Home-page: UNKNOWN
+Home-page: https://github.com/dorian2science/scadaUtils
 Author: Dorian Drevon
 Author-email: drevondorian@gmail.com
 License: UNKNOWN
-Description: # ScadaUtils V0.1
+Description: # ScadaUtils V0.2
         
         ## DESCRIPTION
         
         This package contains utilities for :
         - comUtils : to standardize the dumping of data from different devices(Modbus,Meteo,OPCUA) with a Streamer, SuperDumper_daily and VisualisationMaster_daily
         - Simulators : to simulate the flow of data from devices(servers) from comUtils
         - utilsD : convenient plotly,pandas extensions to work faster
```

### Comparing `scadaUtils-0.1.1/scadaUtils/Conf_generator.py` & `scadaUtils-0.2.1/scadaUtils/Conf_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import pickle,os,sys,re,subprocess as sp,time,shutil
 import pandas as pd
-from sylfenUtils.comUtils import (print_file,FileSystem,create_folder_if_not)
+from .comUtils import (print_file,FileSystem,create_folder_if_not)
 import psycopg2
 
 FS=FileSystem()
 
 def create_sql_table(connParameters,db_table):
     connReq = ''.join([k + "=" + v + " " for k,v in connParameters.items()])
     try:
```

### Comparing `scadaUtils-0.1.1/scadaUtils/GAIA.py` & `scadaUtils-0.2.1/scadaUtils/GAIA.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-import sylfenUtils.comUtils as comUtils
-import sylfenUtils.Conf_generator as Conf_generator
-from sylfenUtils.dashboard import Dashboard
+import .comUtils as comUtils
+import .Conf_generator as Conf_generator
+from .dashboard import Dashboard
 import os,inspect
 from . import utils
 ##### this is the superinstance
 # put the initial parameters of the dashboard in the user_settings default file so that to start the whole
 # programm (configurating,dumping, and web service) the user should only do#
 # ====> gaia=Gaia(myproject_name,my_conf_generator_function)
 ### program should then pop up the user_settings file and ask to modify it if necessary. And tell
```

### Comparing `scadaUtils-0.1.1/scadaUtils/Simulators.py` & `scadaUtils-0.2.1/scadaUtils/Simulators.py`

 * *Files identical despite different names*

### Comparing `scadaUtils-0.1.1/scadaUtils/VersionsManager.py` & `scadaUtils-0.2.1/scadaUtils/VersionsManager.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # #######################
 # #  VERISONS MANAGER    #
 # #######################
 import collections
 from . import comUtils
 from .comUtils import (print_file)
-from sylfenUtils.utils import Utils
+from .utils import Utils
 import glob,re,pandas as pd,os,time,pickle
 sort_list=lambda x:list(pd.Series(x).sort_values())
 import plotly.express as px
 import plotly.graph_objects as go
 import subprocess as sp
 
 class VersionsManager():
```

### Comparing `scadaUtils-0.1.1/scadaUtils/comUtils.py` & `scadaUtils-0.2.1/scadaUtils/comUtils.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import time, pytz,sys
 from time import sleep
 import sys,os,re,threading,struct, glob, pickle,struct,subprocess as sp
 import numpy as np, pandas as pd
 import psycopg2
 from multiprocessing import Pool
 import traceback
-from sylfenUtils.utils import Utils
+from .utils import Utils
 from dateutil.tz import tzlocal
 from zipfile import ZipFile
 import psutil
 
 # #######################
 # #      BASIC Utils    #
 # #######################
```

### Comparing `scadaUtils-0.1.1/scadaUtils/dashboard.py` & `scadaUtils-0.2.1/scadaUtils/dashboard.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from subprocess import check_output
 import json,os,sys,glob,time,traceback
 from IPython.core.ultratb import AutoFormattedTB
 import numpy as np,pandas as pd
 import plotly.express as px
 import plotly.graph_objects as go
 from string import ascii_letters,digits
-from sylfenUtils.comUtils import (timenowstd,computetimeshow,print_file)
-from sylfenUtils.Conf_generator import create_folder_if_not
+from .comUtils import (timenowstd,computetimeshow,print_file)
+from .Conf_generator import create_folder_if_not
 NOTIFS={
     'too_many_datapoints':''' TOO MANY DATAPOINTS\n
         You have requested XXXk datapoints which is over AAAk datapoints.\n
         The plotly graph would be to slow to load and the interaction very unconvenient.\n
         Your request had been modified to limit the number of data points to AAAk by choosing a higher resampling period of : YYY.\n
         If you are not happy with these settings please select another period or/and resampling period or/and total number of tags keeping in mind that you should not exceed AAAk datapoints in total.
         Take into account as well that the more datapoints you ask the more you have to wait for the figure to load.
```

### Comparing `scadaUtils-0.1.1/scadaUtils/monitoring.py` & `scadaUtils-0.2.1/scadaUtils/monitoring.py`

 * *Files identical despite different names*

### Comparing `scadaUtils-0.1.1/scadaUtils/old_minutely_hourly.py` & `scadaUtils-0.2.1/scadaUtils/old_minutely_hourly.py`

 * *Files identical despite different names*

### Comparing `scadaUtils-0.1.1/scadaUtils/physics.py` & `scadaUtils-0.2.1/scadaUtils/physics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # import time
 # start=time.time()
 import numpy as np,pandas as pd,os,sys
-from sylfenUtils import utils
-from sylfenUtils.comUtils import (html_table,print_file)
+from . import utils
+from .comUtils import (html_table,print_file)
 import plotly.express as px
 # print(time.time()-start)
 # from conf_modeling import conf as CONF,
-from sylfenUtils.utils import inspect_simple
+from .utils import inspect_simple
 import inspect
 import pint
 from pint import UnitRegistry
 import CoolProp.CoolProp as CP
 ureg = UnitRegistry()
 ureg.load_definitions(os.path.join(os.path.dirname(__file__),'rsoc_units.txt'))
 c = pint.Context('rsoc')
@@ -39,25 +39,25 @@
             val=v.to_root_units()
             res[k]=convert_to_common_unit(val)
     res=show_pretty(pd.Series(res).T)
     print(res)
     return res
 
 coolProps_Q={
-'D':'kg/m**3',
-'H':'J/kg',
-'Q':'mol/mol',
-'S':'J/kg/K',
-'U':'K/kg',
-'A':'m/s',
-'L' :'W/m/K',
-'V':'pascal.s',
-'C' :'J/kg/K',
-'G':'J/kg',
-'M':'kg/mol',
+    'D':'kg/m**3',
+    'H':'J/kg',
+    'Q':'mol/mol',
+    'S':'J/kg/K',
+    'U':'K/kg',
+    'A':'m/s',
+    'L' :'W/m/K',
+    'V':'pascal.s',
+    'C' :'J/kg/K',
+    'G':'J/kg',
+    'M':'kg/mol',
 }
 FLUID_PROPS={}
 FLUID_PROPS['CO']={
     'L':Q_(0.018,'W/m/K'),
     'V':Q_(1.65e-5,'pascal.s'),
 }
```

### Comparing `scadaUtils-0.1.1/scadaUtils/utils.py` & `scadaUtils-0.2.1/scadaUtils/utils.py`

 * *Files identical despite different names*

### Comparing `scadaUtils-0.1.1/scadaUtils.egg-info/PKG-INFO` & `scadaUtils-0.2.1/scadaUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: scadaUtils
-Version: 0.1.1
+Version: 0.2.1
 Summary: Utilities package
-Home-page: UNKNOWN
+Home-page: https://github.com/dorian2science/scadaUtils
 Author: Dorian Drevon
 Author-email: drevondorian@gmail.com
 License: UNKNOWN
-Description: # ScadaUtils V0.1
+Description: # ScadaUtils V0.2
         
         ## DESCRIPTION
         
         This package contains utilities for :
         - comUtils : to standardize the dumping of data from different devices(Modbus,Meteo,OPCUA) with a Streamer, SuperDumper_daily and VisualisationMaster_daily
         - Simulators : to simulate the flow of data from devices(servers) from comUtils
         - utilsD : convenient plotly,pandas extensions to work faster
```

### Comparing `scadaUtils-0.1.1/setup.py` & `scadaUtils-0.2.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 setuptools.setup(
     name="scadaUtils",
     version=base_version+'.'+v_try,
     author="Dorian Drevon",
     author_email="drevondorian@gmail.com",
     description="Utilities package",
+    url='https://github.com/dorian2science/scadaUtils',
     long_description=long_description,
     long_description_content_type="text/markdown",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

