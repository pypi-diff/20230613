# Comparing `tmp/aanalyticsact-0.0.0.9.tar.gz` & `tmp/aanalyticsact-0.0.1.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\aanalyticsact-0.0.0.9.tar", last modified: Mon Jan 17 18:20:45 2022, max compression
+gzip compressed data, was "aanalyticsact-0.0.1.31.tar", last modified: Tue Jun 13 02:26:05 2023, max compression
```

## Comparing `aanalyticsact-0.0.0.9.tar` & `aanalyticsact-0.0.1.31.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxrwx   0        0        0        0 2022-01-17 18:20:45.470867 aanalyticsact-0.0.0.9/
--rw-rw-rw-   0        0        0     1419 2022-01-17 18:20:45.470867 aanalyticsact-0.0.0.9/PKG-INFO
--rw-rw-rw-   0        0        0      765 2022-01-17 15:45:46.000000 aanalyticsact-0.0.0.9/README.md
-drwxrwxrwx   0        0        0        0 2022-01-17 18:20:45.454864 aanalyticsact-0.0.0.9/aanalyticsact/
--rw-rw-rw-   0        0        0      176 2022-01-17 15:38:59.000000 aanalyticsact-0.0.0.9/aanalyticsact/__init__.py
--rw-rw-rw-   0        0        0       23 2022-01-17 18:20:17.000000 aanalyticsact-0.0.0.9/aanalyticsact/__version__.py
--rw-rw-rw-   0        0        0     6271 2022-01-17 15:37:58.000000 aanalyticsact-0.0.0.9/aanalyticsact/actCreateSeg.py
--rw-rw-rw-   0        0        0     3237 2021-09-18 12:06:32.000000 aanalyticsact-0.0.0.9/aanalyticsact/actExecute.py
--rw-rw-rw-   0        0        0    11388 2022-01-17 18:20:23.000000 aanalyticsact-0.0.0.9/aanalyticsact/actModuler.py
--rw-rw-rw-   0        0        0     7234 2021-09-18 12:01:58.000000 aanalyticsact-0.0.0.9/aanalyticsact/actRunner.py
--rw-rw-rw-   0        0        0     3506 2022-01-17 18:20:26.000000 aanalyticsact-0.0.0.9/aanalyticsact/actUpdateSeg.py
-drwxrwxrwx   0        0        0        0 2022-01-17 18:20:45.467866 aanalyticsact-0.0.0.9/aanalyticsact.egg-info/
--rw-rw-rw-   0        0        0     1419 2022-01-17 18:20:45.000000 aanalyticsact-0.0.0.9/aanalyticsact.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      374 2022-01-17 18:20:45.000000 aanalyticsact-0.0.0.9/aanalyticsact.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-01-17 18:20:45.000000 aanalyticsact-0.0.0.9/aanalyticsact.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2022-01-17 18:20:45.000000 aanalyticsact-0.0.0.9/aanalyticsact.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2022-01-17 18:20:45.472867 aanalyticsact-0.0.0.9/setup.cfg
--rw-rw-rw-   0        0        0      689 2022-01-17 18:20:20.000000 aanalyticsact-0.0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:26:05.447511 aanalyticsact-0.0.1.31/
+-rw-rw-rw-   0        0        0     1216 2023-06-13 02:26:05.448400 aanalyticsact-0.0.1.31/PKG-INFO
+-rw-rw-rw-   0        0        0      765 2022-01-17 15:45:46.000000 aanalyticsact-0.0.1.31/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 02:26:05.404913 aanalyticsact-0.0.1.31/aanalyticsact/
+-rw-rw-rw-   0        0        0      176 2022-01-17 15:38:59.000000 aanalyticsact-0.0.1.31/aanalyticsact/__init__.py
+-rw-rw-rw-   0        0        0       24 2023-06-13 02:25:01.000000 aanalyticsact-0.0.1.31/aanalyticsact/__version__.py
+-rw-rw-rw-   0        0        0     6303 2022-02-16 05:16:30.000000 aanalyticsact-0.0.1.31/aanalyticsact/actCreateSeg.py
+-rw-rw-rw-   0        0        0     6543 2023-05-09 08:26:00.000000 aanalyticsact-0.0.1.31/aanalyticsact/actExecute.py
+-rw-rw-rw-   0        0        0    13653 2023-06-13 02:21:23.000000 aanalyticsact-0.0.1.31/aanalyticsact/actModuler.py
+-rw-rw-rw-   0        0        0     8870 2023-06-01 06:30:28.000000 aanalyticsact-0.0.1.31/aanalyticsact/actRunner.py
+drwxrwxrwx   0        0        0        0 2023-06-13 02:26:05.439424 aanalyticsact-0.0.1.31/aanalyticsact.egg-info/
+-rw-rw-rw-   0        0        0     1216 2023-06-13 02:26:04.000000 aanalyticsact-0.0.1.31/aanalyticsact.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      344 2023-06-13 02:26:05.000000 aanalyticsact-0.0.1.31/aanalyticsact.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 02:26:04.000000 aanalyticsact-0.0.1.31/aanalyticsact.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 02:26:04.000000 aanalyticsact-0.0.1.31/aanalyticsact.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 02:26:05.454384 aanalyticsact-0.0.1.31/setup.cfg
+-rw-rw-rw-   0        0        0      696 2023-06-13 02:25:02.000000 aanalyticsact-0.0.1.31/setup.py
```

### Comparing `aanalyticsact-0.0.0.9/PKG-INFO` & `aanalyticsact-0.0.1.31/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: aanalyticsact
-Version: 0.0.0.9
+Version: 0.0.1.31
 Summary: adobe analytics library for Team ACT
 Home-page: https://github.com/SunkyeongLee/aanalyticsact
 Author: Sunkyeong Lee
-Author-email: sunkyong9768@gmail.com
-License: UNKNOWN
-Description: Adobe Analytics for Team ACT v.0.0.1
-        ==============
-        
-        This module has been built to provide a better environment specifically for adobe analysts in Team ACT.</br></br>
-        
-        This module itself would not contain any confidential information & nor is incapable of retrieving any data unless the correct API credential is given.
-        The guide of pulling data will be only provided internally, no inquires will be accepted from outsiders.
-        
-          
-        ## Functionalities
-        
-        
-        * Retrieve Daily, Weekly, Monthly data and automatically dumps into the DB connected in their local machine.
-        * Capable up to 2nd breakdown.
-        * Automatically retrieves data of all Reporting Suites.
-        * Update Segments
-        * Create Segments
-        
-        
-        More functionalities will be added in sooner time.<br/><br/>
-        
-Platform: UNKNOWN
+Author-email: sunkyeong.lee@concentrix.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+Adobe Analytics for Team ACT v.0.0.1
+==============
+
+This module has been built to provide a better environment specifically for adobe analysts in Team ACT.</br></br>
+
+This module itself would not contain any confidential information & nor is incapable of retrieving any data unless the correct API credential is given.
+The guide of pulling data will be only provided internally, no inquires will be accepted from outsiders.
+
+  
+## Functionalities
+
+
+* Retrieve Daily, Weekly, Monthly data and automatically dumps into the DB connected in their local machine.
+* Capable up to 2nd breakdown.
+* Automatically retrieves data of all Reporting Suites.
+* Update Segments
+* Create Segments
+
+
+More functionalities will be added in sooner time.<br/><br/>
```

### Comparing `aanalyticsact-0.0.0.9/README.md` & `aanalyticsact-0.0.1.31/README.md`

 * *Files identical despite different names*

### Comparing `aanalyticsact-0.0.0.9/aanalyticsact/actCreateSeg.py` & `aanalyticsact-0.0.1.31/aanalyticsact/actCreateSeg.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Created by  Sunkyeong Lee
-# email : sunkyong9768@gmail.com
+# Created by Sunkyeong Lee
+# Inquiry : sunkyeong.lee@concentrix.com / sunkyong9768@gmail.com
 
 import aanalytics2 as api2
 import json
 from copy import deepcopy
 from itertools import *
 import csv
 import os
```

### Comparing `aanalyticsact-0.0.0.9/aanalyticsact/actModuler.py` & `aanalyticsact-0.0.1.31/aanalyticsact/actModuler.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Created by  Sunkyeong Lee
-# email : sunkyong9768@gmail.com
+# Created by Sunkyeong Lee
+# Inquiry : sunkyeong.lee@concentrix.com / sunkyong9768@gmail.com
 
 import aanalytics2 as api2
 import json
 from datetime import datetime, timedelta
 from copy import deepcopy
 from sqlalchemy import create_engine
 
@@ -147,17 +147,19 @@
             dataFrame.insert(0, "site_code", "MST", True)
         dataFrame.insert(2, "period", period, True)
         dataFrame.insert(3, "start_date", startDate, True)
         dataFrame.insert(4, "end_date", endDate, True)
         dataFrame.insert(5, "is_epp", epp, True)
 
     return dataFrame  
-
+# updated 220527. smb site code added
+# updated 221202. my bday! :D smb site code added (10.31 open)
 def filterSiteCode(dataframe):
-    return dataframe.loc[dataframe['site_code'].isin(["kw", "kw_ar", "bh", "bh_ar", "om", "om_ar", "eg_en", "jo", "jo_ar", "ma", "africa_en", "africa_fr", "africa_pt", "al", "ar", "au", "at", "az", "be", "be_fr", "br", "ba", "bd", "bg", "ca", "ca_fr", "cl", "cn", "co", "hr", "cz", "dk", "eg", "ee", "fi", "fr", "de", "gr", "hk", "hk_en", "hu", "in", "id", "iran", "ie", "il", "it", "jp", "kz_ru", "kz_kz", "sec", "lv", "levant", "levant_ar", "lt", "mk", "my", "mx", "mm", "nl", "nz", "n_africa", "no", "pk", "latin", "latin_en", "py", "pe", "ph", "pl", "pt", "ro", "ps", "ru", "sa", "sa_en", "rs", "sg", "sk", "si", "za", "es", "se", "ch", "ch_fr", "tw", "th", "tr", "ae", "ae_ar", "uk", "ua", "uy", "uz_ru", "uz_uz", "vn"])]
+    return dataframe.loc[dataframe['site_code'].isin(["uk", "de", "fr", "au", "in"])]
+    # return dataframe.loc[dataframe['site_code'].isin(["kw", "kw_ar", "bh", "bh_ar", "om", "om_ar", "eg_en", "jo", "jo_ar", "ma", "africa_en", "africa_fr", "africa_pt", "al", "ar", "au", "at", "az", "be", "be_fr", "br", "ba", "bd", "bg", "ca", "ca_fr", "cl", "cn", "co", "hr", "cz", "dk", "eg", "ee", "fi", "fr", "de", "gr", "hk", "hk_en", "hu", "in", "id", "iran", "ie", "il", "it", "jp", "kz_ru", "kz_kz", "sec", "lv", "levant", "levant_ar", "lt", "mk", "my", "mx", "mm", "nl", "nz", "n_africa", "no", "pk", "latin", "latin_en", "py", "pe", "ph", "pl", "pt", "ro", "ps", "ru", "sa", "sa_en", "rs", "sg", "sk", "si", "za", "es", "se", "ch", "ch_fr", "tw", "th", "tr", "ae", "ae_ar", "uk", "ua", "uy", "uz_ru", "uz_uz", "vn", "au-smb", "uk-smb", "fr-smb", "at-smb", "it-smb", "es-smb", "th-smb", "id-smb", "vn-smb", "my-smb", "se-smb", "dk-smb", "fi-smb", "no-smb", "ca-smb", "ca_fr-smb", "de-smb", "nl-smb", "be-smb", "be_fr-smb", "jo-smb", "jo_ar-smb", "ae-smb", "ae_ar-smb", "nz-smb", "ph-smb", "ru-smb", "iq_ar", "iq_ku", "lb", "qa", "qa_ar", "eg-smb", "pl-smb", "pt-smb", "sa_en-smb", "sa-smb", "sg-smb", "eg_en-smb", "mn", "ge"])]
 
 
 # updated 210907. added site_code_rs for us integration(due to the fact that us has no site code)
 def jsonToDb(startDate, endDate, period, jsonLocation, tbColumn, dbTableName, epp, if_site_code, site_code_rs, limit):
     df = refinedFrame(startDate, endDate, period, jsonLocation, epp, if_site_code, site_code_rs)
     df.columns = tbColumn
 
@@ -338,7 +340,49 @@
         dataFrame.insert(6, "is_epp_integ", "Y", True)
     else:
         dataFrame.insert(6, "is_epp_integ", "N", True)
             
     dataFrame.columns = tbColumn
     
     return dataFrame
+
+## 22.04.30 added
+def refineRsIDChange_breakdown(startDate, endDate, jsonFile, jsonFile_breakdown, rsList, period, tbColumn, epp, limit):
+    datechanged = jsonDateChange(startDate, endDate, jsonFile)
+    datechanged_breakdown = jsonDateChange(startDate, endDate, jsonFile_breakdown)
+    rschanged_jsonFile = rsIDchange(datechanged, rsList[1])
+    rschanged_jsonFile_breakdown = rsIDchange(datechanged_breakdown, rsList[1])
+
+    itemIDdict = ReturnJsonchanged(startDate, endDate, rschanged_jsonFile, rschanged_jsonFile_breakdown)
+    for i in range(len(itemIDdict)):
+        dataFrame = dataRetriver_data(itemIDdict[i][1])
+
+        # limit 추가 시 넣기
+        if limit == 0:
+            dataFrame = dataFrame
+        else:
+            dataFrame = dataFrame.head(limit)
+
+        # columnList = []
+        # for i in range(dataFrame.shape[1]):
+        #     columnList.append(i)
+
+         # dataFrame.columns = columnList
+
+        dataFrame.insert(0, "site_code", rsList[0], True)
+        dataFrame.insert(2, "period", period, True)
+        dataFrame.insert(3, "start_date", startDate, True)
+        dataFrame.insert(4, "end_date", endDate, True)
+
+        if epp == True:
+            dataFrame.insert(5, "is_epp", "Y", True)
+        else:
+            dataFrame.insert(5, "is_epp", "N", True)
+
+        if (rsList[1] == "sssamsungnewus" or rsList[1] == "sssamsung4sec"):
+            dataFrame.insert(6, "is_epp_integ", "Y", True)
+        else:
+            dataFrame.insert(6, "is_epp_integ", "N", True)
+                
+        dataFrame.columns = tbColumn
+        
+        return dataFrame
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aanalyticsact-0.0.0.9/aanalyticsact/actRunner.py` & `aanalyticsact-0.0.1.31/aanalyticsact/actRunner.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-# Created by  Sunkyeong Lee
-# email : sunkyong9768@gmail.com
+# Created by Sunkyeong Lee
+# Inquiry : sunkyeong.lee@concentrix.com / sunkyong9768@gmail.com
 
 from datetime import datetime, timedelta
 from calendar import monthrange
 
 
 def dateConverter(date):
     return datetime.strptime(str(date), '%Y-%m-%d').date()
@@ -46,58 +46,76 @@
             endDate.append(str(dateKeep_end))
 
         startDate.pop()
         endDate.pop()
 
         return startDate, endDate
 
+# 230525 revised by Hyunsung Park (Monthly)
     elif (period == "monthly" or period == "Monthly"):
         startDate = []
         endDate = []
 
         startDate.append(str(start_date))
-        
+
         startDate_keep = start_date
-        while startDate_keep < end_date:
-            
-            endDate_keep = lastDayofMonth(startDate_keep)
-            startDate_keep = endDate_keep + timedelta(days=1)
-            startDate.append(str(startDate_keep))
-            endDate.append(str(endDate_keep))
+        endDate_keep = end_date
 
-            startDate_keep = lastDayofMonth(startDate_keep) 
-        
+        while startDate_keep <= lastDayofMonth(end_date):
+            if startDate_keep.year == end_date.year and startDate_keep.month == end_date.month:
+                # 230601 end date is autofixed to the end of the month
+                endDate.append(str(lastDayofMonth(end_date)))
+                startDate_keep = endDate_keep + timedelta(days=1)
+                startDate.append(str(startDate_keep))
+                break
+
+            else:
+                endDate_keep = lastDayofMonth(startDate_keep)
+                startDate_keep = endDate_keep + timedelta(days=1)
+                startDate.append(str(startDate_keep))
+                endDate.append(str(endDate_keep))
+
+            startDate_keep = lastDayofMonth(startDate_keep)
         startDate.pop()
         return startDate, endDate
 
     elif (period == "all" or period == "All"):
         startDate = []
         endDate = []
 
         startDate.append(str(start_date))
         endDate.append(str(end_date))
 
         return startDate, endDate
     
     else:
-        raise Exception("Type withing the followings; daily, weekly, monthly, all")
+        raise Exception("Type within the followings; daily, weekly, monthly, all")
 
 def rsListGenerator(inputSiteCode, targetRSList):
     finalList = []
     for i in range(len(inputSiteCode)):
         for j in range(len(targetRSList)):
             if inputSiteCode[i] in targetRSList[j]:
                 finalList.append(targetRSList[j])
 
     return finalList
 
 
 def returnRsList(epp, inputSiteCode):
-    defaultEpp = [["us", "sssamsungnewus"], ["ae", "sssamsung4aeepp"], ["at", "sssamsung4atepp"], ["au", "sssamsung4auepp"], ["be", "sssamsung4beepp"], ["ca", "sssamsung4caepp"], ["ch", "sssamsung4chepp"], ["cn", "sssamsung4cnepp"], ["cz", "sssamsung4czepp"], ["de", "sssamsung4deepp"], ["dk", "sssamsung4dkepp"], ["ee", "sssamsung4eeepp"], ["eg", "sssamsung4egepp"], ["es", "sssamsung4esepp"], ["fi", "sssamsung4fiepp"], ["fr", "sssamsung4frepp"], ["hk", "sssamsung4hkepp"], ["hu", "sssamsung4huepp"], ["id", "sssamsung4idepp"], ["il", "sssamsung4ilepp"], ["in", "sssamsung4inepp"], ["it", "sssamsung4itepp"], ["levant", "sssamsung4levantepp"], ["lt", "sssamsung4ltepp"], ["lv", "sssamsung4lvepp"], ["my", "sssamsung4myepp"], ["n_africa", "sssamsung4nafricaepp"], ["nl", "sssamsung4nlepp"], ["no", "sssamsung4noepp"], ["nz", "sssamsung4nzepp"], ["pk", "sssamsung4pkepp"], ["pt", "sssamsung4ptepp"], ["ru", "sssamsung4ruepp"], ["sa", "sssamsung4saepp"], ["se", "sssamsung4seepp"], ["sec", "sssamsung4secepp"], ["sg", "sssamsung4sgepp"], ["sk", "sssamsung4skepp"], ["th", "sssamsung4thepp"], ["tw", "sssamsung4twepp"], ["uk", "sssamsung4ukepp"], ["vn", "sssamsung4vnepp"], ["za", "sssamsung4zaepp"]]
-    defaultNone = [["us", "sssamsungnewus"], ["sec", "sssamsung4sec"], ["ae", "sssamsung4ae"], ["ae_ar", "sssamsung4aear"], ["africa_en", "sssamsung4africaen"], ["africa_fr", "sssamsung4africafr"], ["africa_pt", "sssamsung4africapt"], ["al", "sssamsung4al"], ["ar", "sssamsung4ar"], ["at", "sssamsung4at"], ["au", "sssamsung4au"], ["ba", "sssamsung4ba"], ["be", "sssamsung4be"], ["be_fr", "sssamsung4befr"], ["bg", "sssamsung4bg"], ["br", "sssamsung4br"], ["ca", "sssamsung4ca"], ["ca_fr", "sssamsung4cafr"], ["ch", "sssamsung4ch"], ["ch_fr", "sssamsung4chfr"], ["cl", "sssamsung4cl"], ["cn", "sssamsung4cn"], ["co", "sssamsung4co"], ["cz", "sssamsung4cz"], ["de", "sssamsung4de"], ["dk", "sssamsung4dk"], ["ee", "sssamsung4ee"], ["eg", "sssamsung4eg"], ["es", "sssamsung4es"], ["fi", "sssamsung4fi"], ["fr", "sssamsung4fr"], ["gr", "sssamsung4gr"], ["hk", "sssamsung4hk"], ["hk_en", "sssamsung4hken"], ["hr", "sssamsung4hr"], ["hu", "sssamsung4hu"], ["id", "sssamsung4id"], ["ie", "sssamsung4ie"], ["il", "sssamsung4il"], ["in", "sssamsung4in"], ["iran", "sssamsung4iran"], ["it", "sssamsung4it"], ["jp", "sssamsung4jp"], ["kz_kz", "sssamsung4kzkz"], ["kz_ru", "sssamsung4kzru"], ["latin", "sssamsung4latin"], ["latin_en", "sssamsung4latinen"], ["levant", "sssamsung4levant"], ["levant_ar", "sssamsung4levantar"], ["lt", "sssamsung4lt"], ["lv", "sssamsung4lv"], ["mk", "sssamsung4mk"], ["mm", "sssamsung4mm"], ["mx", "sssamsung4mx"], ["my", "sssamsung4my"], ["n_africa", "sssamsung4nafrica"], ["nl", "sssamsung4nl"], ["no", "sssamsung4no"], ["nz", "sssamsung4nz"], ["pe", "sssamsung4pe"], ["ph", "sssamsung4ph"], ["pk", "sssamsung4pk"], ["pl", "sssamsung4pl"], ["ps", "sssamsung4ps"], ["pt", "sssamsung4pt"], ["py", "sssamsung4py"], ["ro", "sssamsung4ro"], ["rs", "sssamsung4rs"], ["ru", "sssamsung4ru"], ["sa", "sssamsung4sa"], ["sa_en", "sssamsung4saen"], ["se", "sssamsung4se"], ["sg", "sssamsung4sg"], ["si", "sssamsung4si"], ["sk", "sssamsung4sk"], ["th", "sssamsung4th"], ["tr", "sssamsung4tr"], ["tw", "sssamsung4tw"], ["ua", "sssamsung4ua"], ["uk", "sssamsung4uk"], ["uy", "sssamsung4uy"], ["uz_ru", "sssamsung4uzru"], ["uz_uz", "sssamsung4uzuz"], ["vn", "sssamsung4vn"], ["za", "sssamsung4za"], ["az", "sssamsung4az"], ["bd", "sssamsung4bd"]]
+    #22.02.10 kz_kz, ua epp 추가
+    #22.02.16 mst_vs 추가
+    #22.04.01 si, hr epp 추가
+    #22.07.26 iq_ar, lb 추가
+    #22.09.01 cl epp 추가
+    #22.10.24 ph epp 추가
+    #23.02.02 iq_ar epp 추가
+    #23.03.03 jp epp 추가
+    #23.04.24 mn, ge 추가
+    defaultEpp = [["us", "sssamsungnewus"], ["ae", "sssamsung4aeepp"], ["at", "sssamsung4atepp"], ["au", "sssamsung4auepp"], ["be", "sssamsung4beepp"], ["ca", "sssamsung4caepp"], ["ch", "sssamsung4chepp"], ["cn", "sssamsung4cnepp"], ["cz", "sssamsung4czepp"], ["de", "sssamsung4deepp"], ["dk", "sssamsung4dkepp"], ["ee", "sssamsung4eeepp"], ["eg", "sssamsung4egepp"], ["es", "sssamsung4esepp"], ["fi", "sssamsung4fiepp"], ["fr", "sssamsung4frepp"], ["hk", "sssamsung4hkepp"], ["hu", "sssamsung4huepp"], ["id", "sssamsung4idepp"], ["il", "sssamsung4ilepp"], ["in", "sssamsung4inepp"], ["it", "sssamsung4itepp"], ["levant", "sssamsung4levantepp"], ["lt", "sssamsung4ltepp"], ["lv", "sssamsung4lvepp"], ["my", "sssamsung4myepp"], ["n_africa", "sssamsung4nafricaepp"], ["nl", "sssamsung4nlepp"], ["no", "sssamsung4noepp"], ["nz", "sssamsung4nzepp"], ["pk", "sssamsung4pkepp"], ["pt", "sssamsung4ptepp"], ["ru", "sssamsung4ruepp"], ["sa", "sssamsung4saepp"], ["se", "sssamsung4seepp"], ["sec", "sssamsung4secepp"], ["sg", "sssamsung4sgepp"], ["sk", "sssamsung4skepp"], ["th", "sssamsung4thepp"], ["tw", "sssamsung4twepp"], ["uk", "sssamsung4ukepp"], ["vn", "sssamsung4vnepp"], ["za", "sssamsung4zaepp"], ["kz_kz", "sssamsung4kzkzepp"], ["ua", "sssamsung4uaepp"], ["si", "sssssamsung4siepp"], ["hr", "sssamsung4hrepp"], ["cl", "sssamsung4clepp"], ["ph", "sssamsung4phepp"], ["africa_en", "sssamsung4africaenepp"], ["co", "sssamsung4coepp"], ["gr", "sssamsung4grepp"], ["ie", "sssamsung4ieepp"], ["mx", "sssamsung4mxepp"], ["pe", "sssamsung4peepp"], ["pl", "sssamsung4plepp"], ["ro", "sssamsung4roepp"], ["iq_ar", "sssamsung4iqarepp"], ["jp", "sssamsung4jpepp"]]
+    defaultNone = [["us", "sssamsungnewus"], ["sec", "sssamsung4sec"], ["ae", "sssamsung4ae"], ["ae_ar", "sssamsung4aear"], ["africa_en", "sssamsung4africaen"], ["africa_fr", "sssamsung4africafr"], ["africa_pt", "sssamsung4africapt"], ["al", "sssamsung4al"], ["ar", "sssamsung4ar"], ["at", "sssamsung4at"], ["au", "sssamsung4au"], ["ba", "sssamsung4ba"], ["be", "sssamsung4be"], ["be_fr", "sssamsung4befr"], ["bg", "sssamsung4bg"], ["br", "sssamsung4br"], ["ca", "sssamsung4ca"], ["ca_fr", "sssamsung4cafr"], ["ch", "sssamsung4ch"], ["ch_fr", "sssamsung4chfr"], ["cl", "sssamsung4cl"], ["cn", "sssamsung4cn"], ["co", "sssamsung4co"], ["cz", "sssamsung4cz"], ["de", "sssamsung4de"], ["dk", "sssamsung4dk"], ["ee", "sssamsung4ee"], ["eg", "sssamsung4eg"], ["es", "sssamsung4es"], ["fi", "sssamsung4fi"], ["fr", "sssamsung4fr"], ["gr", "sssamsung4gr"], ["hk", "sssamsung4hk"], ["hk_en", "sssamsung4hken"], ["hr", "sssamsung4hr"], ["hu", "sssamsung4hu"], ["id", "sssamsung4id"], ["ie", "sssamsung4ie"], ["il", "sssamsung4il"], ["in", "sssamsung4in"], ["iran", "sssamsung4iran"], ["it", "sssamsung4it"], ["jp", "sssamsung4jp"], ["kz_kz", "sssamsung4kzkz"], ["kz_ru", "sssamsung4kzru"], ["latin", "sssamsung4latin"], ["latin_en", "sssamsung4latinen"], ["levant", "sssamsung4levant"], ["levant_ar", "sssamsung4levantar"], ["lt", "sssamsung4lt"], ["lv", "sssamsung4lv"], ["mk", "sssamsung4mk"], ["mm", "sssamsung4mm"], ["mx", "sssamsung4mx"], ["my", "sssamsung4my"], ["n_africa", "sssamsung4nafrica"], ["nl", "sssamsung4nl"], ["no", "sssamsung4no"], ["nz", "sssamsung4nz"], ["pe", "sssamsung4pe"], ["ph", "sssamsung4ph"], ["pk", "sssamsung4pk"], ["pl", "sssamsung4pl"], ["ps", "sssamsung4ps"], ["pt", "sssamsung4pt"], ["py", "sssamsung4py"], ["ro", "sssamsung4ro"], ["rs", "sssamsung4rs"], ["ru", "sssamsung4ru"], ["sa", "sssamsung4sa"], ["sa_en", "sssamsung4saen"], ["se", "sssamsung4se"], ["sg", "sssamsung4sg"], ["si", "sssamsung4si"], ["sk", "sssamsung4sk"], ["th", "sssamsung4th"], ["tr", "sssamsung4tr"], ["tw", "sssamsung4tw"], ["ua", "sssamsung4ua"], ["uk", "sssamsung4uk"], ["uy", "sssamsung4uy"], ["uz_ru", "sssamsung4uzru"], ["uz_uz", "sssamsung4uzuz"], ["vn", "sssamsung4vn"], ["za", "sssamsung4za"], ["az", "sssamsung4az"], ["bd", "sssamsung4bd"], ["mst_sena", "vrs_samsun0_p4webmstsena_0"], ["mst_sehk", "vrs_samsun0_p6webmstsehk"], ["mst_sebn", "vrs_samsun0_p4websebn"], ["mst_mena", "vrs_samsun0_p4webmstmena"], ["mst_seca", "vrs_samsun0_p4webmstseca"], ["mst_eu", "vrs_samsun0_p4webmsteu_0"], ["mst_seao", "vrs_samsun0_p4webmstseao"], ["iq_ar", "sssamsung4iqar"], ["lb", "sssamsung4lb"], ["mn", "sssamsung4mn"], ["ge", "sssamsung4ge"]]
 
     if epp == True:
         return rsListGenerator(inputSiteCode, defaultEpp)
     else:
         return rsListGenerator(inputSiteCode, defaultNone)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aanalyticsact-0.0.0.9/aanalyticsact.egg-info/PKG-INFO` & `aanalyticsact-0.0.1.31/aanalyticsact.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,35 +1,33 @@
 Metadata-Version: 2.1
 Name: aanalyticsact
-Version: 0.0.0.9
+Version: 0.0.1.31
 Summary: adobe analytics library for Team ACT
 Home-page: https://github.com/SunkyeongLee/aanalyticsact
 Author: Sunkyeong Lee
-Author-email: sunkyong9768@gmail.com
-License: UNKNOWN
-Description: Adobe Analytics for Team ACT v.0.0.1
-        ==============
-        
-        This module has been built to provide a better environment specifically for adobe analysts in Team ACT.</br></br>
-        
-        This module itself would not contain any confidential information & nor is incapable of retrieving any data unless the correct API credential is given.
-        The guide of pulling data will be only provided internally, no inquires will be accepted from outsiders.
-        
-          
-        ## Functionalities
-        
-        
-        * Retrieve Daily, Weekly, Monthly data and automatically dumps into the DB connected in their local machine.
-        * Capable up to 2nd breakdown.
-        * Automatically retrieves data of all Reporting Suites.
-        * Update Segments
-        * Create Segments
-        
-        
-        More functionalities will be added in sooner time.<br/><br/>
-        
-Platform: UNKNOWN
+Author-email: sunkyeong.lee@concentrix.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
+
+Adobe Analytics for Team ACT v.0.0.1
+==============
+
+This module has been built to provide a better environment specifically for adobe analysts in Team ACT.</br></br>
+
+This module itself would not contain any confidential information & nor is incapable of retrieving any data unless the correct API credential is given.
+The guide of pulling data will be only provided internally, no inquires will be accepted from outsiders.
+
+  
+## Functionalities
+
+
+* Retrieve Daily, Weekly, Monthly data and automatically dumps into the DB connected in their local machine.
+* Capable up to 2nd breakdown.
+* Automatically retrieves data of all Reporting Suites.
+* Update Segments
+* Create Segments
+
+
+More functionalities will be added in sooner time.<br/><br/>
```

### Comparing `aanalyticsact-0.0.0.9/setup.py` & `aanalyticsact-0.0.1.31/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="aanalyticsact",
-    version="0.0.0.9",
+    version="0.0.1.31",
     author="Sunkyeong Lee",
-    author_email="sunkyong9768@gmail.com",
+    author_email="sunkyeong.lee@concentrix.com",
     description="adobe analytics library for Team ACT",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/SunkyeongLee/aanalyticsact",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
```

