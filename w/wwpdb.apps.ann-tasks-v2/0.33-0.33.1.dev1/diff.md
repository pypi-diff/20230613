# Comparing `tmp/wwpdb.apps.ann_tasks_v2-0.33.tar.gz` & `tmp/wwpdb.apps.ann_tasks_v2-0.33.1.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.ann_tasks_v2-0.33.tar", last modified: Tue Jun 13 02:46:55 2023, max compression
+gzip compressed data, was "wwpdb.apps.ann_tasks_v2-0.33.1.dev1.tar", last modified: Tue Jun 13 10:49:31 2023, max compression
```

## Comparing `wwpdb.apps.ann_tasks_v2-0.33.tar` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.908002 wwpdb.apps.ann_tasks_v2-0.33/
--rw-r--r--   0 vsts      (1001) docker     (123)      784 2023-06-13 02:46:55.908002 wwpdb.apps.ann_tasks_v2-0.33/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       77 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-13 02:46:55.912002 wwpdb.apps.ann_tasks_v2-0.33/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2542 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.892002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.892002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.892002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.892002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/assembly/
--rw-r--r--   0 vsts      (1001) docker     (123)    39726 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py
--rw-r--r--   0 vsts      (1001) docker     (123)    46849 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/assembly/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.892002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/
--rw-r--r--   0 vsts      (1001) docker     (123)     5682 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/Check.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7485 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4947 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4344 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3727 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3138 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3694 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6775 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.896002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/
--rw-r--r--   0 vsts      (1001) docker     (123)     3045 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (123)    31018 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16936 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.896002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/density/
--rw-r--r--   0 vsts      (1001) docker     (123)      998 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/density/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.896002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/depict/
--rw-r--r--   0 vsts      (1001) docker     (123)     3945 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.896002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/
--rw-r--r--   0 vsts      (1001) docker     (123)     2573 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4448 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3981 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19613 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5646 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.896002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/
--rw-r--r--   0 vsts      (1001) docker     (123)     6295 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14488 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2940 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3345 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12364 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12679 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.900002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/
--rw-r--r--   0 vsts      (1001) docker     (123)    10620 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12969 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18806 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11248 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.900002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/io/
--rw-r--r--   0 vsts      (1001) docker     (123)    15912 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9923 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/io/PisaReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.900002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/link/
--rw-r--r--   0 vsts      (1001) docker     (123)     3057 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/link/Link.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/link/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.900002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/
--rw-r--r--   0 vsts      (1001) docker     (123)     3231 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4323 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3336 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4763 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5394 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4764 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3305 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3716 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3561 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.900002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nafeatures/
--rw-r--r--   0 vsts      (1001) docker     (123)     2610 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nafeatures/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/
--rw-r--r--   0 vsts      (1001) docker     (123)    16217 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6954 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3694 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8475 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3526 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/
--rw-r--r--   0 vsts      (1001) docker     (123)     1540 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2010 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/Related.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4025 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/
--rw-r--r--   0 vsts      (1001) docker     (123)     8209 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    24814 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/
--rw-r--r--   0 vsts      (1001) docker     (123)     8612 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    80924 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    33069 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/secstruct/
--rw-r--r--   0 vsts      (1001) docker     (123)     3406 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/secstruct/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/site/
--rw-r--r--   0 vsts      (1001) docker     (123)     3094 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/site/Site.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/site/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/solvent/
--rw-r--r--   0 vsts      (1001) docker     (123)     3037 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/solvent/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/status/
--rw-r--r--   0 vsts      (1001) docker     (123)    32859 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/status/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.908002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/transformCoord/
--rw-r--r--   0 vsts      (1001) docker     (123)     3759 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/transformCoord/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.908002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)     6454 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3600 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1509 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3451 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4031 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8388 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3396 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4790 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3021 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4071 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3045 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.908002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/validate/
--rw-r--r--   0 vsts      (1001) docker     (123)    10304 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/validate/Validate.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/validate/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.908002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/view3d/
--rw-r--r--   0 vsts      (1001) docker     (123)     5085 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/view3d/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.908002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)     5627 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    40112 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)   175984 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14316 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)    73514 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16955 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.892002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      784 2023-06-13 02:46:55.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     5436 2023-06-13 02:46:55.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 02:46:55.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 02:46:02.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      325 2023-06-13 02:46:55.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-13 02:46:55.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.097142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (123)      791 2023-06-13 10:49:31.097142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       77 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-13 10:49:31.097142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2542 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.065142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.065142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.069142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/
+-rw-r--r--   0 vsts      (1001) docker     (123)      157 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.069142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/assembly/
+-rw-r--r--   0 vsts      (1001) docker     (123)    39726 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    46849 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/assembly/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.069142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5712 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/Check.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7521 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4947 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4344 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3727 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3138 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3694 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6865 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.069142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/correspnd/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3045 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    30874 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16936 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/correspnd/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.069142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/density/
+-rw-r--r--   0 vsts      (1001) docker     (123)      998 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/density/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.069142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/depict/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3945 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.073142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/editCoord/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2573 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4448 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3981 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19613 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5646 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/editCoord/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.073142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/em3d/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6295 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14488 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2940 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3345 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12364 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12679 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/em3d/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.073142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/expIoUtils/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10620 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12969 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18806 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11248 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/expIoUtils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.077142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)    15912 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9923 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/io/PisaReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.077142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/link/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3057 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/link/Link.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/link/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.077142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3231 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4323 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3336 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4763 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5394 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4764 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3305 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3716 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3561 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.081142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nafeatures/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2610 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nafeatures/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.081142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nmr/
+-rw-r--r--   0 vsts      (1001) docker     (123)    16217 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6954 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3694 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8475 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3526 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nmr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.085142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/related/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1540 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2010 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/related/Related.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4025 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/related/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.085142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/report/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8209 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    24814 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/report/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.089142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/report/styles/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8612 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    80925 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    33069 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/report/styles/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.089142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/secstruct/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3406 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/secstruct/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.089142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/site/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3094 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/site/Site.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/site/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.089142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/solvent/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3037 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/solvent/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.089142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/status/
+-rw-r--r--   0 vsts      (1001) docker     (123)    32859 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/status/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.089142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/transformCoord/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3759 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/transformCoord/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.093142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6454 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3600 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1509 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3451 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4026 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8388 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3396 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4790 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3021 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4071 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3045 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.097142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/validate/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10304 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/validate/Validate.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/validate/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.097142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/view3d/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5085 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/view3d/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.097142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5627 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    40112 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   176103 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14317 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    73514 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16955 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:46:59.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:49:31.065142 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb.apps.ann_tasks_v2.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      791 2023-06-13 10:49:30.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5436 2023-06-13 10:49:31.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 10:49:30.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb.apps.ann_tasks_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 10:48:39.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb.apps.ann_tasks_v2.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      325 2023-06-13 10:49:30.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb.apps.ann_tasks_v2.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-13 10:49:30.000000 wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb.apps.ann_tasks_v2.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/PKG-INFO` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wwpdb.apps.ann_tasks_v2
-Version: 0.33
+Name: wwpdb.apps.ann-tasks-v2
+Version: 0.33.1.dev1
 Summary: wwPDB annotation/review/status/validation module backend
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/setup.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/Check.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/Check.py`

 * *Files 0% similar despite different names*

```diff
@@ -122,16 +122,18 @@
             if self.__reportFileSize > 0:
                 dp.exp(self.__reportPath)
                 self.addDownloadPath(self.__reportPath)
             #
             self.addDownloadPath(logPath)
             #
             if self._verbose:
-                self._lfh.write("+%s.%s dictionary check version %s completed for entryId %s file %s report %s size %d\n" % (self.__class__.__name__, \
-                          inspect.currentframe().f_code.co_name, self.__dictionaryVersion, entryId, inpPath, self.__reportPath, self.__reportFileSize))
+                self._lfh.write(
+                    "+%s.%s dictionary check version %s completed for entryId %s file %s report %s size %d\n"
+                    % (self.__class__.__name__, inspect.currentframe().f_code.co_name, self.__dictionaryVersion, entryId, inpPath, self.__reportPath, self.__reportFileSize)
+                )
             #
             if self._cleanup:
                 dp.cleanup()
             #
             return True
         except:  # noqa: E722 pylint: disable=bare-except
             if self._verbose:
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 from mmcif.io.IoAdapterCore import IoAdapterCore
 from wwpdb.apps.ann_tasks_v2.utils.SessionWebDownloadUtils import SessionWebDownloadUtils
 from wwpdb.io.locator.PathInfo import PathInfo
 
 logger = logging.getLogger()
 
+
 class EmMapCheck(SessionWebDownloadUtils):
     """
     Encapsulates checking consistencies between em_map category vs. map files in archival directory
 
     Operations are performed in the current session context defined in the input
     reqObj().
 
@@ -78,16 +79,18 @@
                 return
             #
             self.__reportFileSize = self.__getSize(self.__reportPath)
             if self.__reportFileSize > 0:
                 self.addDownloadPath(self.__reportPath)
             #
             if self.__verbose:
-                self.__lfh.write("+%s.%s em_map check completed for entryId %s file %s report %s size %d\n" % (self.__class__.__name__, \
-                          inspect.currentframe().f_code.co_name, entryId, modelInputFile, self.__reportPath, self.__reportFileSize))
+                self.__lfh.write(
+                    "+%s.%s em_map check completed for entryId %s file %s report %s size %d\n"
+                    % (self.__class__.__name__, inspect.currentframe().f_code.co_name, entryId, modelInputFile, self.__reportPath, self.__reportFileSize)
+                )
             #
         except Exception as e:
             if self.__verbose:
                 logger.error("em_map check failed for entryId %s file %s error: %s", entryId, modelInputFile, str(e))
             #
             logger.exception("Failed to check XML file production")
         #
@@ -102,28 +105,27 @@
         try:
             statInfo = os.stat(fn)
             return statInfo.st_size
         except:  # noqa: E722 pylint: disable=bare-except
             return 0
         #
 
+
 class EmMapCheckTask(object):
-    """
-    """
+    """ """
+
     def __init__(self, siteId=None, sessionPath=None, verbose=False, log=sys.stderr):
-        """
-        """
+        """ """
         self.__siteId = siteId
         self.__sessionPath = sessionPath
         self.__verbose = verbose
         self.__lfh = log
 
     def run(self, entryId, modelInputFile, reportPath):
-        """
-        """
+        """ """
         # Test if em_admin present in model
         ioObj = IoAdapterCore(verbose=self.__verbose, log=self.__lfh)
         dIn = ioObj.readFile(inputFilePath=modelInputFile, selectList=["em_admin", "em_map"])
         if not dIn or len(dIn) == 0:
             return
         #
         cObj = dIn[0].getObj("em_admin")
@@ -151,46 +153,54 @@
                     recordedMapList.append(valueD["file"])
                 #
             #
         #
         pI = PathInfo(siteId=self.__siteId, sessionPath=self.__sessionPath, verbose=self.__verbose, log=self.__lfh)
         #
         archivalMapList = []
-        for mapType in ( "em-3d-classification-additional-volume", "em-additional-volume", "em-alignment-mask-volume", \
-                     "em-focus-refinement-additional-volume", "em-focused-refinement-mask-volume", "em-fsc-half-mask-volume", \
-                     "em-fsc-map-model-mask-volume", "em-half-volume", "em-mask-volume", "em-raw-volume", "em-segmentation-volume", "em-volume" ):
-            archiveFilePath = pI.getFilePath(dataSetId=entryId, wfInstanceId=None, contentType=mapType, formatType="map", fileSource="archive", \
-                                             versionId="latest", partNumber="1")
+        for mapType in (
+            "em-3d-classification-additional-volume",
+            "em-additional-volume",
+            "em-alignment-mask-volume",
+            "em-focus-refinement-additional-volume",
+            "em-focused-refinement-mask-volume",
+            "em-fsc-half-mask-volume",
+            "em-fsc-map-model-mask-volume",
+            "em-half-volume",
+            "em-mask-volume",
+            "em-raw-volume",
+            "em-segmentation-volume",
+            "em-volume",
+        ):
+            archiveFilePath = pI.getFilePath(dataSetId=entryId, wfInstanceId=None, contentType=mapType, formatType="map", fileSource="archive", versionId="latest", partNumber="1")
             if archiveFilePath and os.access(archiveFilePath, os.F_OK):
                 (_dir, fileName) = os.path.split(archiveFilePath)
                 archivalMapList.append(fileName)
             #
         #
         (_dir, modelFileName) = os.path.split(modelInputFile)
         #
         archivePath = pI.getArchivePath(dataSetId=entryId)
         oth = open(reportPath, "w")
         for mapFileName in recordedMapList:
             if os.access(os.path.join(archivePath, mapFileName), os.F_OK):
                 continue
             #
-            oth.write("Map file '%s' defined in 'em_map' category of model file '%s' can not be found in archive directory.\n" % \
-                     ( mapFileName, modelFileName )) 
+            oth.write("Map file '%s' defined in 'em_map' category of model file '%s' can not be found in archive directory.\n" % (mapFileName, modelFileName))
         #
         for mapFileName in archivalMapList:
             if mapFileName in recordedMapList:
                 continue
             #
-            oth.write("Map file '%s' is not included in 'em_map' category of model file '%s'.\n" % ( mapFileName, modelFileName )) 
+            oth.write("Map file '%s' is not included in 'em_map' category of model file '%s'.\n" % (mapFileName, modelFileName))
         #
         oth.close()
 
     def __getValueList(self, catObj):
-        """
-        """
+        """ """
         valueList = []
         attribList = catObj.getAttributeList()
         rowList = catObj.getRowList()
         for rowD in rowList:
             tD = {}
             for idxIt, itName in enumerate(attribList):
                 if rowD[idxIt] != "?" and rowD[idxIt] != ".":
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,24 +30,23 @@
     Encapsulates PDBML/XML checking.
     """
 
     def __init__(self, reqObj=None, verbose=False, log=sys.stderr):
         super(XmlCheck, self).__init__(reqObj=reqObj, verbose=verbose, log=log)
         self.__reportPath = None
         self.__reportFileSize = 0
-        self.__checkArgs = None
+        self.__checkArgs = None  # pylint: disable=unused-private-member
         self.__publicCifPath = None
         self.__xmlPath = None
 
     def setArguments(self, checkArgs):
-        self.__checkArgs = checkArgs
+        self.__checkArgs = checkArgs  # pylint: disable=unused-private-member
 
     def run(self, entryId, inpPath, publicCIFlag=True):
-        """ Run the PDBML/XML check on the input PDBx/mmCIF data file
-        """
+        """Run the PDBML/XML check on the input PDBx/mmCIF data file"""
         try:
             self.clearFileList()
             #
             self.__reportPath = os.path.join(self._exportPath, entryId + "_xml-check-report_P1.txt.V1")
             if os.access(self.__reportPath, os.R_OK):
                 os.remove(self.__reportPath)
             #
@@ -62,16 +61,18 @@
             self.__generateXMLFile(entryId)
             if self.__xmlPath is None:
                 return
             #
             self.__checkXMLFile(entryId, "annot-check-xml-xmllint")
             self.__checkXMLFile(entryId, "annot-check-xml-stdinparse")
             if self._verbose:
-                self._lfh.write("+%s.%s PDBML XML check completed for entryId %s file %s report %s size %d\n" % (self.__class__.__name__, \
-                          inspect.currentframe().f_code.co_name, entryId, inpPath, self.__reportPath, self.__reportFileSize))
+                self._lfh.write(
+                    "+%s.%s PDBML XML check completed for entryId %s file %s report %s size %d\n"
+                    % (self.__class__.__name__, inspect.currentframe().f_code.co_name, entryId, inpPath, self.__reportPath, self.__reportFileSize)
+                )
             #
         except:  # noqa: E722 pylint: disable=bare-except
             if self._verbose:
                 self._lfh.write("+%s.%s PDBML XML check failed for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, entryId, inpPath))
             #
             traceback.print_exc(file=self._lfh)
         #
@@ -79,16 +80,15 @@
     def getReportSize(self):
         return self.__reportFileSize
 
     def getReportPath(self):
         return self.__reportPath
 
     def __generateXMLFile(self, entryId):
-        """ Generate noatom xml file
-        """
+        """Generate noatom xml file"""
         try:
             outputList = []
             outputList.append(os.path.join(self._exportPath, self.__publicCifPath + ".xml-noatom"))
             outputList.append(os.path.join(self._exportPath, entryId + "_generate_xml_v5.log"))
             outputList.append(os.path.join(self._exportPath, entryId + "_generate_xml_command_v5.log"))
             for filePath in outputList:
                 if os.access(filePath, os.R_OK):
@@ -107,23 +107,23 @@
                 self.__xmlPath = os.path.join(self._exportPath, self.__publicCifPath + ".xml-noatom")
             #
             if self._cleanup:
                 dp.cleanup()
             #
         except:  # noqa: E722 pylint: disable=bare-except
             if self._verbose:
-                self._lfh.write("+%s.%s XML conversion failed for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, \
-                                entryId, self.__publicCifPath))
+                self._lfh.write(
+                    "+%s.%s XML conversion failed for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, entryId, self.__publicCifPath)
+                )
             #
             traceback.print_exc(file=self._lfh)
         #
 
     def __checkXMLFile(self, entryId, op):
-        """ Check noatom xml file
-        """
+        """Check noatom xml file"""
         try:
             if (not self.__xmlPath) or (not os.access(self.__xmlPath, os.R_OK)):
                 return
             #
             if op == "annot-check-xml-xmllint":
                 statinfo = os.stat(self.__xmlPath)
                 if statinfo.st_size > 100000000:
@@ -167,12 +167,13 @@
                 #
             #
             if self._cleanup:
                 dp.cleanup()
             #
         except:  # noqa: E722 pylint: disable=bare-except
             if self._verbose:
-                self._lfh.write("+%s.%s XML (%s) checking failed for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, \
-                                op, entryId, self.__xmlPath))
+                self._lfh.write(
+                    "+%s.%s XML (%s) checking failed for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, op, entryId, self.__xmlPath)
+                )
             #
             traceback.print_exc(file=self._lfh)
         #
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py`

 * *Files 1% similar despite different names*

```diff
@@ -479,24 +479,15 @@
                 + "\n\n"
                 + myD["major_release"]
                 + "\n\n"
                 + myD["letter_footer"]
             )
         else:
             myD["full_text"] = (
-                myD["letter_header"]
-                + myD["letter_encourage"]
-                + "\n\n"
-                + myD["minor"]
-                + "\n\n"
-                + minor_text
-                + "\n\n"
-                + myD["minor_release"]
-                + "\n\n"
-                + myD["letter_footer"]
+                myD["letter_header"] + myD["letter_encourage"] + "\n\n" + myD["minor"] + "\n\n" + minor_text + "\n\n" + myD["minor_release"] + "\n\n" + myD["letter_footer"]
             )
         flist = myD["full_text"].split("\n")
         myD["rows"] = str(len(flist))
         #
         # write out default letter
         depid = self.__reqObj.getValue("entryid")
         filename = os.path.join(self.__sessionPath, depid + "_correspondence-to-depositor_P1.txt")
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/io/PisaReader.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/io/PisaReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/link/Link.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/link/Link.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/Related.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/related/Related.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py`

 * *Files 0% similar despite different names*

```diff
@@ -325,17 +325,17 @@
             # ('_pdbx_struct_assembly_gen.asym_id_list', '%s', 'str', ''),
             # ('_pdbx_struct_assembly_prop.biol_id', '%s', 'str', ''),
             # ('_pdbx_struct_assembly_prop.type', '%s', 'str', ''),
             # ('_pdbx_struct_assembly_prop.value', '%s', 'str', ''),
             # ('_pdbx_struct_assembly_prop.details', '%s', 'str', '')
         ],
         "pdbx_struct_assembly_gen": [
-            ('_pdbx_struct_assembly_gen.assembly_id', '%s', 'str', ''),
-            ('_pdbx_struct_assembly_gen.oper_expression', '%s', 'str', ''),
-            ('_pdbx_struct_assembly_gen.asym_id_list', '%s', 'str', '')
+            ("_pdbx_struct_assembly_gen.assembly_id", "%s", "str", ""),
+            ("_pdbx_struct_assembly_gen.oper_expression", "%s", "str", ""),
+            ("_pdbx_struct_assembly_gen.asym_id_list", "%s", "str", ""),
         ],
         "pdbx_struct_oper_list": [
             ("_pdbx_struct_oper_list.id", "%s", "str", ""),
             ("_pdbx_struct_oper_list.type", "%s", "str", ""),
             ("_pdbx_struct_oper_list.name", "%s", "str", ""),
             ("_pdbx_struct_oper_list.symmetry_operation", "%s", "str", ""),
             ("_pdbx_struct_oper_list.matrix[1][1]", "%s", "str", ""),
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/site/Site.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/site/Site.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,49 +35,48 @@
         super(PublicPdbxFile, self).__init__(reqObj=reqObj, verbose=verbose, log=log)
         self._verbose = verbose
         self._lfh = log
         self.__reqObj = reqObj
         self._debug = False
         self.__setup()
         #
-        self.__opMap = { "annot-cif-to-public-pdbx": ( "_model-review_P1.cif", "-public_cif.log" ), \
-                         "cif2pdbx-ext": ( "_model-next_P1.cif", "_cif2pdbx-next.log" ), \
-                         "cif2pdbx-public": ( "_model-v4-pubic_P1.cif", "_cif2pdbx-pubic.log" ) }
+        self.__opMap = {
+            "annot-cif-to-public-pdbx": ("_model-review_P1.cif", "-public_cif.log"),
+            "cif2pdbx-ext": ("_model-next_P1.cif", "_cif2pdbx-next.log"),
+            "cif2pdbx-public": ("_model-v4-pubic_P1.cif", "_cif2pdbx-pubic.log"),
+        }
         #
 
     def __setup(self):
         self._siteId = self.__reqObj.getValue("WWPDB_SITE_ID")
         self.__sObj = self.__reqObj.getSessionObj()
         self._sessionPath = self.__sObj.getPath()
-        self._exportPath = self._sessionPath
+        self._exportPath = self._sessionPath  # pylint: disable=attribute-defined-outside-init
         self._cleanup = False
 
     def setExportPath(self, exportPath):
-        """ Set the path where output files are copyied.
-        """
-        self._exportPath = exportPath
+        """Set the path where output files are copyied."""
+        self._exportPath = exportPath  # pylint: disable=attribute-defined-outside-init
 
-    def run(self, entryId, inpFile):
-        """ Create review model file
-        """
-        inpPath = os.path.join(self._sessionPath, inpFile)
-        if self.run_conversion("annot-cif-to-public-pdbx", entryId, inpPath):
+    def run(self, entryId, inpPath):
+        """Create review model file"""
+        full_inpPath = os.path.join(self._sessionPath, inpPath)
+        if self.run_conversion("annot-cif-to-public-pdbx", entryId, full_inpPath):
             return True
         #
         return False
 
     def run_conversion(self, op, entryId, inpPath):
-        """ Run conversion.
-        """
+        """Run conversion."""
         try:
             if op not in self.__opMap:
                 return
             #
             pdbxPath = os.path.join(self._exportPath, entryId + self.__opMap[op][0])
-            logPath  = os.path.join(self._exportPath, entryId + self.__opMap[op][1])
+            logPath = os.path.join(self._exportPath, entryId + self.__opMap[op][1])
             #
             for filePath in (pdbxPath, logPath):
                 if os.access(filePath, os.R_OK):
                     os.remove(filePath)
                 #
             #
             dp = RcsbDpUtility(tmpPath=self._sessionPath, siteId=self._siteId, verbose=self._verbose, log=self._lfh)
@@ -93,22 +92,20 @@
             dp.expLog(logPath)
             #
             if op != "annot-cif-to-public-pdbx":
                 self.addDownloadPath(pdbxPath)
                 self.addDownloadPath(logPath)
             #
             if self._verbose:
-                self._lfh.write("+%s.%s  creating public cif for entryId %s file %s\n" % (self.__class__.__name__, \
-                                 inspect.currentframe().f_code.co_name, entryId, inpPath))
+                self._lfh.write("+%s.%s  creating public cif for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, entryId, inpPath))
             #
             if self._cleanup:
                 dp.cleanup()
             #
             return pdbxPath
         except:  # noqa: E722 pylint: disable=bare-except
             if self._verbose:
-                self._lfh.write("+%s.%s public cif conversion failed for entryId %s file %s\n" % (self.__class__.__name__, \
-                                inspect.currentframe().f_code.co_name, entryId, inpPath))
+                self._lfh.write("+%s.%s public cif conversion failed for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, entryId, inpPath))
             #
             traceback.print_exc(file=self._lfh)
         #
         return None
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/validate/Validate.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/validate/Validate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py`

 * *Files 0% similar despite different names*

```diff
@@ -2422,22 +2422,22 @@
                     aTagList.append(duL.getAnchorTag())
                 else:
                     duL.removeFromDownload(rptPath)
 
             if "checkxml" in operationList:
                 self._lfh.write("+CommonTasksWebAppWorker._makeCheckReports() starting checkxml\n")
 
-                chk = XmlCheck(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
-                pdbxPath = os.path.join(self._sessionPath, entryId + "_model-next_P1.cif") 
+                xchk = XmlCheck(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
+                pdbxPath = os.path.join(self._sessionPath, entryId + "_model-next_P1.cif")
                 if os.access(pdbxPath, os.R_OK):
                     self._lfh.write("+CommonTasksWebAppWorker._makeCheckReports() starting checkxml using %s\n" % pdbxPath)
-                    chk.run(entryId=entryId, inpPath=pdbxPath, publicCIFlag=True)
+                    xchk.run(entryId=entryId, inpPath=pdbxPath, publicCIFlag=True)
                 else:
                     self._lfh.write("+CommonTasksWebAppWorker._makeCheckReports() starting checkxml using %s\n" % modelFilePath)
-                    chk.run(entryId=entryId, inpPath=modelFilePath, publicCIFlag=False)
+                    xchk.run(entryId=entryId, inpPath=modelFilePath, publicCIFlag=False)
                 #
                 rptPath = chk.getReportPath()
                 hasDiags = chk.getReportSize() > 0
                 if hasDiags:
                     duL.copyToDownload(rptPath)
                     aTagList.append(duL.getAnchorTag())
                 else:
@@ -2476,15 +2476,14 @@
                 hasDiags = chk.getReportSize() > 0
                 if hasDiags:
                     rptPath = chk.getReportPath()
                     duL.copyToDownload(rptPath)
                     aTagList.append(duL.getAnchorTag())
 
             if "check-emd-xml" in operationList:
-                print("XXXXXXXXXX About to start")
                 try:
                     chk = EmdXmlCheck(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
                     chk.run(entryId=entryId, modelInputFile=modelFilePath)
                 except Exception as e:
                     logger.error("Error running EmdXmlCheck %s", e)
                 hasDiags = chk.getReportSize() > 0
                 rptPath = chk.getReportPath()
@@ -2623,22 +2622,33 @@
             "check-misc": "misc-check-report",
             "check-format": "format-check-report",
             "check-geometry": "geometry-check-report",
             "check-sf": "dcc-report",
             "check-special-position": "special-position-report",
             "cif2pdb": "model-pdb",
             "check-emd-xml": "emd-xml-header-report",
-            "check-em-map": "em-map-check-report"
+            "check-em-map": "em-map-check-report",
         }
 
         rC = ResponseContent(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
         rC.setReturnFormat("json")
         if operation in ["check-all"]:
-            opList = ["cif2pdb", "checkv5", "checkNext", "checkxml", "check-format", "check-misc", "check-geometry", "check-special-position", \
-                      "check-sf", "check-emd-xml", "check-em-map"]
+            opList = [
+                "cif2pdb",
+                "checkv5",
+                "checkNext",
+                "checkxml",
+                "check-format",
+                "check-misc",
+                "check-geometry",
+                "check-special-position",
+                "check-sf",
+                "check-emd-xml",
+                "check-em-map",
+            ]
             aTagList = self._makeCheckReports([entryId], operationList=opList, fileSource=fileSource, useFileVersions=useFileVersions)
             cTList = ["model"]
             cTList.extend(sorted(opCtD.values()))
             if self._verbose:
                 self._lfh.write("+ReviewDataWebAppWorker._reviewDataInlineIdOps() content type list %r\n" % cTList)
             myD = self._renderCheckReports(entryId, fileSource="session-download", instance=None, contentTypeList=cTList, useModelFileVersion=useFileVersions)
             rC.setHtmlTextFromTemplate(templateFilePath=templateFilePath, webIncludePath=webIncludePath, parameterDict=myD, insertContext=True)
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py`

 * *Files 0% similar despite different names*

```diff
@@ -292,15 +292,15 @@
                 "check-format",
                 "check-misc",
                 "check-geometry",
                 "check-sf",
                 # 'cif2pdb',
                 "check-special-position",
                 "check-emd-xml",
-                "check-em-map"
+                "check-em-map",
             ]
             _aTagList = self._makeCheckReports([idCode], operationList=opList)  # noqa: F841
         #
         #
         if self._verbose:
             self._lfh.write("\n\n+ReviewDataWebAppWorker._generateFullHtmlCheckReport() idCode %s generating reports from data files in fileSource %s\n" % (idCode, fileSource))
         #
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: wwpdb.apps.ann-tasks-v2
-Version: 0.33
+Name: wwpdb.apps.ann_tasks_v2
+Version: 0.33.1.dev1
 Summary: wwPDB annotation/review/status/validation module backend
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt` & `wwpdb.apps.ann_tasks_v2-0.33.1.dev1/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

