# Comparing `tmp/wwpdb.apps.ann_tasks_v2-0.32.tar.gz` & `tmp/wwpdb.apps.ann_tasks_v2-0.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.ann_tasks_v2-0.32.tar", last modified: Fri Mar 17 20:30:53 2023, max compression
+gzip compressed data, was "wwpdb.apps.ann_tasks_v2-0.33.tar", last modified: Tue Jun 13 02:46:55 2023, max compression
```

## Comparing `wwpdb.apps.ann_tasks_v2-0.32.tar` & `wwpdb.apps.ann_tasks_v2-0.33.tar`

### file list

```diff
@@ -1,146 +1,148 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.069407 wwpdb.apps.ann_tasks_v2-0.32/
--rw-r--r--   0 vsts      (1001) docker     (123)      784 2023-03-17 20:30:53.069407 wwpdb.apps.ann_tasks_v2-0.32/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       77 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-03-17 20:30:53.069407 wwpdb.apps.ann_tasks_v2-0.32/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2542 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.057407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.057407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.057407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/
--rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.057407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/assembly/
--rw-r--r--   0 vsts      (1001) docker     (123)    39726 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py
--rw-r--r--   0 vsts      (1001) docker     (123)    46849 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/assembly/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.057407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/check/
--rw-r--r--   0 vsts      (1001) docker     (123)     9140 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/check/Check.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4947 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4344 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3727 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3138 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3694 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/check/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.057407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/correspnd/
--rw-r--r--   0 vsts      (1001) docker     (123)     3045 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py
--rw-r--r--   0 vsts      (1001) docker     (123)    31018 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16936 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/correspnd/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.057407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/density/
--rw-r--r--   0 vsts      (1001) docker     (123)      998 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/density/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.057407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/depict/
--rw-r--r--   0 vsts      (1001) docker     (123)     3945 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/depict/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.057407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/editCoord/
--rw-r--r--   0 vsts      (1001) docker     (123)     2573 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4448 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3981 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py
--rw-r--r--   0 vsts      (1001) docker     (123)    19613 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5646 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/editCoord/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.061407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/em3d/
--rw-r--r--   0 vsts      (1001) docker     (123)     6295 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14488 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2940 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3345 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12364 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12679 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/em3d/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.061407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/expIoUtils/
--rw-r--r--   0 vsts      (1001) docker     (123)    10620 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12969 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    18806 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11248 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/expIoUtils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.061407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/io/
--rw-r--r--   0 vsts      (1001) docker     (123)    15912 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9923 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/io/PisaReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.061407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/link/
--rw-r--r--   0 vsts      (1001) docker     (123)     3057 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/link/Link.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/link/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.061407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/
--rw-r--r--   0 vsts      (1001) docker     (123)     3231 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4323 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3336 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4763 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5394 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4764 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3305 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3716 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3561 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.061407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nafeatures/
--rw-r--r--   0 vsts      (1001) docker     (123)     2610 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nafeatures/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.061407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nmr/
--rw-r--r--   0 vsts      (1001) docker     (123)    16217 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6954 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3694 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8475 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3526 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nmr/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.061407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/related/
--rw-r--r--   0 vsts      (1001) docker     (123)     1540 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2010 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/related/Related.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4025 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/related/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.065407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/report/
--rw-r--r--   0 vsts      (1001) docker     (123)     8209 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    24814 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/report/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.065407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/report/styles/
--rw-r--r--   0 vsts      (1001) docker     (123)     8612 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    80655 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    33069 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/report/styles/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.065407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/secstruct/
--rw-r--r--   0 vsts      (1001) docker     (123)     3406 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/secstruct/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.065407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/site/
--rw-r--r--   0 vsts      (1001) docker     (123)     3094 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/site/Site.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/site/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.065407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/solvent/
--rw-r--r--   0 vsts      (1001) docker     (123)     3037 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/solvent/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.065407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/status/
--rw-r--r--   0 vsts      (1001) docker     (123)    32859 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/status/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.065407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/transformCoord/
--rw-r--r--   0 vsts      (1001) docker     (123)     3759 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/transformCoord/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.065407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/
--rw-r--r--   0 vsts      (1001) docker     (123)     6454 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3600 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1509 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3451 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2145 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8388 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3396 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4790 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3021 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4071 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3045 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.065407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/validate/
--rw-r--r--   0 vsts      (1001) docker     (123)    10304 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/validate/Validate.py
--rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/validate/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.065407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/view3d/
--rw-r--r--   0 vsts      (1001) docker     (123)     5085 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/view3d/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.069407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)     5627 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py
--rw-r--r--   0 vsts      (1001) docker     (123)    40112 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)   171577 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14178 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)    73514 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16955 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-03-17 20:28:30.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-03-17 20:30:53.057407 wwpdb.apps.ann_tasks_v2-0.32/wwpdb.apps.ann_tasks_v2.egg-info/
--rw-rw-rw-   0 vsts      (1001) docker     (123)      784 2023-03-17 20:30:53.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO
--rw-rw-rw-   0 vsts      (1001) docker     (123)     5350 2023-03-17 20:30:53.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt
--rw-rw-rw-   0 vsts      (1001) docker     (123)        1 2023-03-17 20:30:53.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb.apps.ann_tasks_v2.egg-info/dependency_links.txt
--rw-rw-rw-   0 vsts      (1001) docker     (123)        1 2023-03-17 20:30:11.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb.apps.ann_tasks_v2.egg-info/not-zip-safe
--rw-rw-rw-   0 vsts      (1001) docker     (123)      325 2023-03-17 20:30:53.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb.apps.ann_tasks_v2.egg-info/requires.txt
--rw-rw-rw-   0 vsts      (1001) docker     (123)        6 2023-03-17 20:30:53.000000 wwpdb.apps.ann_tasks_v2-0.32/wwpdb.apps.ann_tasks_v2.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.908002 wwpdb.apps.ann_tasks_v2-0.33/
+-rw-r--r--   0 vsts      (1001) docker     (123)      784 2023-06-13 02:46:55.908002 wwpdb.apps.ann_tasks_v2-0.33/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)       77 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)      108 2023-06-13 02:46:55.912002 wwpdb.apps.ann_tasks_v2-0.33/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (123)     2542 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.892002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.892002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.892002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/
+-rw-r--r--   0 vsts      (1001) docker     (123)      150 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.892002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/assembly/
+-rw-r--r--   0 vsts      (1001) docker     (123)    39726 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    46849 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/assembly/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.892002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5682 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/Check.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7485 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4947 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4344 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3727 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3138 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3694 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6775 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.896002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3045 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    31018 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16936 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.896002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/density/
+-rw-r--r--   0 vsts      (1001) docker     (123)      998 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/density/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.896002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/depict/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3945 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/depict/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.896002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2573 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4448 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3981 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    19613 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5646 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.896002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6295 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14488 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2940 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3345 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12364 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12679 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.900002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10620 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    12969 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    18806 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    11248 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.900002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/io/
+-rw-r--r--   0 vsts      (1001) docker     (123)    15912 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     9923 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/io/PisaReader.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.900002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/link/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3057 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/link/Link.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/link/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.900002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3231 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4323 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3336 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4763 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5394 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4764 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3305 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3716 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3561 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.900002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nafeatures/
+-rw-r--r--   0 vsts      (1001) docker     (123)     2610 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nafeatures/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/
+-rw-r--r--   0 vsts      (1001) docker     (123)    16217 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     6954 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3694 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8475 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3526 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/
+-rw-r--r--   0 vsts      (1001) docker     (123)     1540 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2010 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/Related.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4025 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8209 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    24814 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/
+-rw-r--r--   0 vsts      (1001) docker     (123)     8612 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    80924 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    33069 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/secstruct/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3406 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/secstruct/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/site/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3094 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/site/Site.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/site/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/solvent/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3037 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/solvent/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.904002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/status/
+-rw-r--r--   0 vsts      (1001) docker     (123)    32859 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/status/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.908002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/transformCoord/
+-rw-r--r--   0 vsts      (1001) docker     (123)     3759 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/transformCoord/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.908002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/
+-rw-r--r--   0 vsts      (1001) docker     (123)     6454 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3600 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1509 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3451 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4031 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     8388 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3396 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4790 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3021 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4071 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3045 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.908002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/validate/
+-rw-r--r--   0 vsts      (1001) docker     (123)    10304 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/validate/Validate.py
+-rwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/validate/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.908002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/view3d/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5085 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/view3d/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.908002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5627 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    40112 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)   175984 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    14316 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    73514 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)    16955 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py
+-rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 02:44:31.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 02:46:55.892002 wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)      784 2023-06-13 02:46:55.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5436 2023-06-13 02:46:55.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 02:46:55.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 02:46:02.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)      325 2023-06-13 02:46:55.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-13 02:46:55.000000 wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/PKG-INFO` & `wwpdb.apps.ann_tasks_v2-0.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ann_tasks_v2
-Version: 0.32
+Version: 0.33
 Summary: wwPDB annotation/review/status/validation module backend
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/setup.py` & `wwpdb.apps.ann_tasks_v2-0.33/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/check/Check.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/XmlCheck.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,234 +1,178 @@
 ##
-# File:  Check.py
-# Date:  10-Sep-2012  J. Westbrook
+# File:  XmlCheck.py
+# Date:  25-May-2023  Zukang Feng
 #
 # Update:
-#  2-July-2012  Add entry point for dictionary level checking.
-# 29-Dec -2013  Generalized for sharing and api standardized.
-# 28-Feb -2014  add base class
-#  1-Feb -2015  include pre-dictionary dialect conversion before V4 dicitonary check
-# 29-Nov -2016  Include support for new naming and extended checks (still using old rcsbDpUtilities for now (ep)
 ##
 """
-Dictionary-level PDBx/mmCIF checking
+PDBML/XML checking
 
 """
 __docformat__ = "restructuredtext en"
-__author__ = "John Westbrook"
-__email__ = "jwest@rcsb.rutgers.edu"
+__author__ = "Zukang Feng"
+__email__ = "zfeng@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.07"
 
 import sys
 import os.path
 import os
 import traceback
 import inspect
 
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
-from wwpdb.apps.ann_tasks_v2.utils.SessionWebDownloadUtils import SessionWebDownloadUtils
+from wwpdb.apps.ann_tasks_v2.utils.PublicPdbxFile import PublicPdbxFile
 
 
-class Check(SessionWebDownloadUtils):
+class XmlCheck(PublicPdbxFile):
 
     """
-    Encapsulates dictioanry-level PDBx/mmCIF checking.
-
-    Operations are performed in the current session context defined in the input
-    reqObj().
-
+    Encapsulates PDBML/XML checking.
     """
 
     def __init__(self, reqObj=None, verbose=False, log=sys.stderr):
-        super(Check, self).__init__(reqObj=reqObj, verbose=verbose, log=log)
-        self.__verbose = verbose
-        self.__lfh = log
-        self.__reqObj = reqObj
-        self.__debug = False
+        super(XmlCheck, self).__init__(reqObj=reqObj, verbose=verbose, log=log)
         self.__reportPath = None
-        self.__dictionaryVersion = "V5"
         self.__reportFileSize = 0
         self.__checkArgs = None
-        self.__exportPath = None
-        self.__firstBlock = False
-
-        self.__setup()
-
-    def __setup(self):
-        self.__siteId = self.__reqObj.getValue("WWPDB_SITE_ID")
-        self.__sObj = self.__reqObj.getSessionObj()
-        self.__sessionPath = self.__sObj.getPath()
-        self.__exportPath = self.__sessionPath
-        self.__cleanup = False
-
-    def setDictionaryVersion(self, version):
-        if version.upper() in ["V6", "V5", "V4", "DEPOSIT", "ARCHIVE_NEXT", "ARCHIVE_CURRENT"]:
-            self.__dictionaryVersion = version.upper()
-            return True
-        else:
-            return False
-
-    def setCheckFirstBlock(self, flag):
-        self.__firstBlock = flag
-
-    def setExportPath(self, exportPath):
-        """Set the path where output files are copyied."""
-        self.__exportPath = exportPath
+        self.__publicCifPath = None
+        self.__xmlPath = None
 
     def setArguments(self, checkArgs):
         self.__checkArgs = checkArgs
 
-    def __cnv(self, entryId, inpPath):
+    def run(self, entryId, inpPath, publicCIFlag=True):
+        """ Run the PDBML/XML check on the input PDBx/mmCIF data file
+        """
         try:
-            logPath = os.path.join(self.__exportPath, entryId + "_cif2pdbx-pubic.log")
-            if os.access(logPath, os.R_OK):
-                os.remove(logPath)
-            #
-            pdbxPath = os.path.join(self.__exportPath, entryId + "_model-v4-pubic_P1.cif")
-            if os.access(pdbxPath, os.R_OK):
-                os.remove(pdbxPath)
+            self.clearFileList()
             #
-            dp = RcsbDpUtility(tmpPath=self.__sessionPath, siteId=self.__siteId, verbose=self.__verbose, log=self.__lfh)
-            if self.__debug:
-                dp.setDebugMode(flag=True)
-            dp.imp(inpPath)
-            dp.op("cif2pdbx-public")
-            dp.exp(pdbxPath)
-            dp.expLog(logPath)
+            self.__reportPath = os.path.join(self._exportPath, entryId + "_xml-check-report_P1.txt.V1")
+            if os.access(self.__reportPath, os.R_OK):
+                os.remove(self.__reportPath)
             #
-            self.addDownloadPath(logPath)
-            self.addDownloadPath(pdbxPath)
-
-            if self.__verbose:
-                self.__lfh.write("+%s.%s  creating public cif for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, entryId, inpPath))
+            if not publicCIFlag:
+                self.__publicCifPath = self.run_conversion("cif2pdbx-ext", entryId, inpPath)
+            else:
+                self.__publicCifPath = inpPath
+            #
+            if self.__publicCifPath is None:
+                return
+            #
+            self.__generateXMLFile(entryId)
+            if self.__xmlPath is None:
+                return
+            #
+            self.__checkXMLFile(entryId, "annot-check-xml-xmllint")
+            self.__checkXMLFile(entryId, "annot-check-xml-stdinparse")
+            if self._verbose:
+                self._lfh.write("+%s.%s PDBML XML check completed for entryId %s file %s report %s size %d\n" % (self.__class__.__name__, \
+                          inspect.currentframe().f_code.co_name, entryId, inpPath, self.__reportPath, self.__reportFileSize))
+            #
+        except:  # noqa: E722 pylint: disable=bare-except
+            if self._verbose:
+                self._lfh.write("+%s.%s PDBML XML check failed for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, entryId, inpPath))
+            #
+            traceback.print_exc(file=self._lfh)
+        #
 
-            if self.__cleanup:
-                dp.cleanup()
+    def getReportSize(self):
+        return self.__reportFileSize
 
-            return pdbxPath
-        except:  # noqa: E722 pylint: disable=bare-except
-            if self.__verbose:
-                self.__lfh.write(
-                    "+%s.%s public cif conversion failed for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, entryId, inpPath)
-                )
-                traceback.print_exc(file=self.__lfh)
-        return None
+    def getReportPath(self):
+        return self.__reportPath
 
-    def __cnvNext(self, entryId, inpPath):
+    def __generateXMLFile(self, entryId):
+        """ Generate noatom xml file
+        """
         try:
-            logPath = os.path.join(self.__exportPath, entryId + "_cif2pdbx-next.log")
-            if os.access(logPath, os.R_OK):
-                os.remove(logPath)
-            #
-            pdbxPath = os.path.join(self.__exportPath, entryId + "_model-next_P1.cif")
-            if os.access(pdbxPath, os.R_OK):
-                os.remove(pdbxPath)
+            outputList = []
+            outputList.append(os.path.join(self._exportPath, self.__publicCifPath + ".xml-noatom"))
+            outputList.append(os.path.join(self._exportPath, entryId + "_generate_xml_v5.log"))
+            outputList.append(os.path.join(self._exportPath, entryId + "_generate_xml_command_v5.log"))
+            for filePath in outputList:
+                if os.access(filePath, os.R_OK):
+                    os.remove(filePath)
+                #
             #
-            dp = RcsbDpUtility(tmpPath=self.__sessionPath, siteId=self.__siteId, verbose=self.__verbose, log=self.__lfh)
-            if self.__debug:
+            dp = RcsbDpUtility(tmpPath=self._sessionPath, siteId=self._siteId, verbose=self._verbose, log=self._lfh)
+            if self._debug:
                 dp.setDebugMode(flag=True)
-            dp.imp(inpPath)
-            dp.addInput(name="destination", value="archive_next")
-            dp.op("cif2pdbx-ext")
-            dp.exp(pdbxPath)
-            dp.expLog(logPath)
             #
-            self.addDownloadPath(logPath)
-            self.addDownloadPath(pdbxPath)
-
-            if self.__verbose:
-                self.__lfh.write("+%s.%s  creating test cif for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, entryId, inpPath))
-
-            if self.__cleanup:
+            dp.imp(self.__publicCifPath)
+            dp.op("annot-public-pdbx-to-xml-noatom")
+            dp.expList(outputList)
+            #
+            if os.access(os.path.join(self._exportPath, self.__publicCifPath + ".xml-noatom"), os.R_OK):
+                self.__xmlPath = os.path.join(self._exportPath, self.__publicCifPath + ".xml-noatom")
+            #
+            if self._cleanup:
                 dp.cleanup()
-
-            return pdbxPath
+            #
         except:  # noqa: E722 pylint: disable=bare-except
-            if self.__verbose:
-                self.__lfh.write("+%s.%s test cif conversion failed for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, entryId, inpPath))
-                traceback.print_exc(file=self.__lfh)
-        return None
-
-    def run(self, entryId, inpPath, updateInput=True):  # pylint: disable=unused-argument
-        """Run the dictionary-level check on the input PDBx/mmCIF data file -"""
+            if self._verbose:
+                self._lfh.write("+%s.%s XML conversion failed for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, \
+                                entryId, self.__publicCifPath))
+            #
+            traceback.print_exc(file=self._lfh)
+        #
+
+    def __checkXMLFile(self, entryId, op):
+        """ Check noatom xml file
+        """
         try:
-            self.clearFileList()
-
-            logPath = os.path.join(self.__exportPath, entryId + "_dict-check-report.log")
-            self.__reportPath = os.path.join(self.__exportPath, entryId + "_dict-check-report_P1.txt.V1")
+            if (not self.__xmlPath) or (not os.access(self.__xmlPath, os.R_OK)):
+                return
             #
-            dp = RcsbDpUtility(tmpPath=self.__sessionPath, siteId=self.__siteId, verbose=self.__verbose, log=self.__lfh)
-            if self.__debug:
-                dp.setDebugMode(flag=True)
-            if self.__checkArgs is not None:
-                dp.addInput(name="check_arguments", value=self.__checkArgs)
-            if self.__firstBlock:
-                dp.addInput("first_block")
-
-            if self.__dictionaryVersion in ["V5", "DEPOSIT"]:
-                dp.imp(inpPath)
-                dp.op("check-cif")
-
-            elif self.__dictionaryVersion in ["V4", "ARCHIVE_CURRENT"]:
-                cnvInpPath = self.__cnv(entryId, inpPath)
-                if cnvInpPath is not None:
-                    dp.imp(cnvInpPath)
-                else:
-                    dp.imp(inpPath)
-                dp.op("check-cif-v4")
-                logPath = os.path.join(self.__exportPath, entryId + "_dict-check-report-r4.log")
-                self.__reportPath = os.path.join(self.__exportPath, entryId + "_dict-check-report-r4_P1.txt.V1")
-
-            elif self.__dictionaryVersion in ["ARCHIVE_NEXT"]:
-                cnvInpPath = self.__cnvNext(entryId, inpPath)
-                if cnvInpPath is not None:
-                    dp.imp(cnvInpPath)
-                else:
-                    dp.imp(inpPath)
-                dp.op("check-cif-ext")
-                dp.addInput(name="dictionary", value="archive_next")
-                logPath = os.path.join(self.__exportPath, entryId + "_dict-check-report-next.log")
-                self.__reportPath = os.path.join(self.__exportPath, entryId + "_dict-check-report-next_P1.txt.V1")
-
-            elif self.__dictionaryVersion in ["V6"]:
-                dp.imp(inpPath)
-                dp.op("check-cif-v6")
-            else:
-                dp.imp(inpPath)
-                dp.op("check-cif")
+            if op == "annot-check-xml-xmllint":
+                statinfo = os.stat(self.__xmlPath)
+                if statinfo.st_size > 100000000:
+                    return
+                #
+            #
+            inReportPath = os.path.join(self._exportPath, entryId + ".xml.diag")
+            if os.access(inReportPath, os.R_OK):
+                os.remove(inReportPath)
             #
-            if os.access(logPath, os.R_OK):
-                os.remove(logPath)
+            outputList = []
+            outputList.append(inReportPath)
             #
-            if os.access(self.__reportPath, os.R_OK):
-                os.remove(self.__reportPath)
+            dp = RcsbDpUtility(tmpPath=self._sessionPath, siteId=self._siteId, verbose=self._verbose, log=self._lfh)
+            if self._debug:
+                dp.setDebugMode(flag=True)
             #
-            dp.expLog(logPath)
+            dp.imp(self.__xmlPath)
+            dp.op(op)
+            dp.expList(outputList)
+            #
+            if os.access(inReportPath, os.R_OK):
+                ith = open(inReportPath, "r")
+                data = ith.read()
+                ith.close()
+                if len(data) > 0:
+                    oth = open(self.__reportPath, "a")
+                    for line in data.split("\n"):
+                        strip_line = line.strip()
+                        if (strip_line == "") or (strip_line == "input_file_1 validates") or strip_line.startswith("stdin:"):
+                            continue
+                        elif strip_line.startswith("input_file_1:") or strip_line.startswith("input_file_1 "):
+                            oth.write("%s\n" % strip_line[13:])
+                        else:
+                            oth.write("%s\n" % strip_line)
+                        #
+                    #
+                    oth.close()
+                    statinfo = os.stat(self.__reportPath)
+                    self.__reportFileSize = statinfo.st_size
+                #
             #
-            self.__reportFileSize = dp.expSize()
-            if self.__reportFileSize > 0:
-                dp.exp(self.__reportPath)
-                self.addDownloadPath(self.__reportPath)
-            #
-            self.addDownloadPath(logPath)
-
-            if self.__verbose:
-                self.__lfh.write(
-                    "+%s.%s dictionary check version %s completed for entryId %s file %s report %s size %d\n"
-                    % (self.__class__.__name__, inspect.currentframe().f_code.co_name, self.__dictionaryVersion, entryId, inpPath, self.__reportPath, self.__reportFileSize)
-                )
-
-            if self.__cleanup:
+            if self._cleanup:
                 dp.cleanup()
-            return True
+            #
         except:  # noqa: E722 pylint: disable=bare-except
-            if self.__verbose:
-                self.__lfh.write("+%s.%s dictionary check failed for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, entryId, inpPath))
-            traceback.print_exc(file=self.__lfh)
-            return False
-
-    def getReportSize(self):
-        return self.__reportFileSize
-
-    def getReportPath(self):
-        return self.__reportPath
+            if self._verbose:
+                self._lfh.write("+%s.%s XML (%s) checking failed for entryId %s file %s\n" % (self.__class__.__name__, inspect.currentframe().f_code.co_name, \
+                                op, entryId, self.__xmlPath))
+            #
+            traceback.print_exc(file=self._lfh)
+        #
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/FormatCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/depict/PdbxDepictBootstrapBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorForm.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CSEditorUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorForm_v2.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/editCoord/CoordEditorUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmAutoFix.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmEditUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmHeaderUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmMapAutoFixVers.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmModelUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/em3d/EmUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/MtzTommCIF.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpIoUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/PdbxExpUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/expIoUtils/ReSetFreeRinSFmmCIF.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/io/PdbxIoUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/io/PisaReader.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/io/PisaReader.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/link/Link.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/link/Link.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/BisoFullCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/DccCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/DccRefineCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/MapCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/MapDisplay.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/NpCcMapCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/ReassignAltIdsCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionCalc.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/mapcalc/SpecialPositionUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nafeatures/NAFeatures.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftProcessUtilsTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsMiscChecks.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrChemShiftsUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/nmr/NmrModelUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/DaInternalDb.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/related/Related.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/Related.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/related/UpdateRelated.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/PdbxReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/PdbxReportDepictBootstrap.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/DCCReport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/ModelReport.py`

 * *Files 0% similar despite different names*

```diff
@@ -324,14 +324,19 @@
             # ('_pdbx_struct_assembly_gen.oper_expression', '%s', 'str', ''),
             # ('_pdbx_struct_assembly_gen.asym_id_list', '%s', 'str', ''),
             # ('_pdbx_struct_assembly_prop.biol_id', '%s', 'str', ''),
             # ('_pdbx_struct_assembly_prop.type', '%s', 'str', ''),
             # ('_pdbx_struct_assembly_prop.value', '%s', 'str', ''),
             # ('_pdbx_struct_assembly_prop.details', '%s', 'str', '')
         ],
+        "pdbx_struct_assembly_gen": [
+            ('_pdbx_struct_assembly_gen.assembly_id', '%s', 'str', ''),
+            ('_pdbx_struct_assembly_gen.oper_expression', '%s', 'str', ''),
+            ('_pdbx_struct_assembly_gen.asym_id_list', '%s', 'str', '')
+        ],
         "pdbx_struct_oper_list": [
             ("_pdbx_struct_oper_list.id", "%s", "str", ""),
             ("_pdbx_struct_oper_list.type", "%s", "str", ""),
             ("_pdbx_struct_oper_list.name", "%s", "str", ""),
             ("_pdbx_struct_oper_list.symmetry_operation", "%s", "str", ""),
             ("_pdbx_struct_oper_list.matrix[1][1]", "%s", "str", ""),
             ("_pdbx_struct_oper_list.matrix[1][2]", "%s", "str", ""),
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/report/styles/PdbxIo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/secstruct/SecondaryStructure.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/site/Site.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/site/Site.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/solvent/Solvent.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/status/StatusUpdate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/transformCoord/TransformCoord.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/GetCloseContact.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/MergeXyz.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/NmrRemediationUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/PdbFile.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,67 +1,93 @@
 ##
-# File:  PublicPdbxFile.py
-# Date:  14-Oct-2013
+# File:  TerminalAtoms.py
+# Date:  12-Dec-2013  J. Westbrook
 #
 # Update:
-# 28-Feb -2014  jdw Add base class
-# 4-Jun-2014    jdw Added V4 dictionary argument --
+# 28-Feb -2014  Add base class
 ##
 """
-Generate public pdbx cif file.
+Manage utility to remove or rename  terminal OXT atoms.
 
 """
 __docformat__ = "restructuredtext en"
-__author__ = "Zukang Feng"
-__email__ = "zfeng@rcsb.rutgers.edu"
+__author__ = "John Westbrook"
+__email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.07"
 
-import os
-import os.path
 import sys
+import os.path
+import os
 import traceback
 
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
-
 from wwpdb.apps.ann_tasks_v2.utils.SessionWebDownloadUtils import SessionWebDownloadUtils
 
 
-class PublicPdbxFile(SessionWebDownloadUtils):
-    """The PublicPdbxFile class encapsulates conversion internal pdbx cif to public pdbx cif file."""
+class TerminalAtoms(SessionWebDownloadUtils):
+    """
+    TerminalAtoms class encapsulates removing or renaming  terminal OXT atoms.
+
+    """
 
     def __init__(self, reqObj=None, verbose=False, log=sys.stderr):
-        super(PublicPdbxFile, self).__init__(reqObj=reqObj, verbose=verbose, log=log)
+        super(TerminalAtoms, self).__init__(reqObj=reqObj, verbose=verbose, log=log)
         self.__verbose = verbose
         self.__lfh = log
         self.__reqObj = reqObj
+        self.__status = "none"
+        #
         self.__setup()
 
     def __setup(self):
         self.__siteId = self.__reqObj.getValue("WWPDB_SITE_ID")
         self.__sObj = self.__reqObj.getSessionObj()
         self.__sessionPath = self.__sObj.getPath()
-        #
 
-    def run(self, entryId, inpFile):
-        """Run conversion."""
+    def getLastStatus(self):
+        return self.__status
+
+    def __checkStatus(self, logFilePath):
+        status = "ok"
+        if os.access(logFilePath, os.R_OK):
+            ifh = open(logFilePath, "r")
+            for line in ifh:
+                if str(line).upper().startswith("++ERROR"):
+                    return "error"
+                if str(line).upper().startswith("++WARN"):
+                    return "warn"
+            ifh.close()
+        else:
+            return "error"
+
+        return status
+
+    def run(self, entryId, inpFile, updateInput=True, updateOption="delete"):
+        """Run the calculation - updateOption = delete|rename"""
         try:
             inpPath = os.path.join(self.__sessionPath, inpFile)
-            logPath = os.path.join(self.__sessionPath, entryId + "-public_cif.log")
-            retPath = os.path.join(self.__sessionPath, entryId + "_model-review_P1.cif")
-            #
-            for filePath in (logPath, retPath):
-                if os.access(filePath, os.R_OK):
-                    os.remove(filePath)
-                #
+            logPath1 = os.path.join(self.__sessionPath, entryId + "-terminal-atoms.log")
+            retPath = os.path.join(self.__sessionPath, entryId + "_model-updated_P1.cif")
             #
             dp = RcsbDpUtility(tmpPath=self.__sessionPath, siteId=self.__siteId, verbose=self.__verbose, log=self.__lfh)
             dp.imp(inpPath)
-            dp.op("annot-cif-to-public-pdbx")
+            dp.addInput(name="option", value=updateOption)
+
+            dp.op("annot-update-terminal-atoms")
+            dp.expLog(logPath1)
             dp.exp(retPath)
-            dp.expLog(logPath)
-            dp.cleanup()
+            self.addDownloadPath(retPath)
+            self.addDownloadPath(logPath1)
+            if updateInput:
+                dp.exp(inpPath)
+
             #
+            self.__status = self.__checkStatus(logPath1)
+            if self.__verbose:
+                self.__lfh.write("+TerminalAtoms.run-  completed with status %s for entryId %s file %s\n" % (self.__status, entryId, inpPath))
+
+            dp.cleanup()
             return True
         except:  # noqa: E722 pylint: disable=bare-except
             traceback.print_exc(file=self.__lfh)
             return False
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/SessionDownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/SessionWebDownloadUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/TaskSessionState.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/TerminalAtoms.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,93 +1,95 @@
 ##
-# File:  TerminalAtoms.py
-# Date:  12-Dec-2013  J. Westbrook
+# File:  UpdateCloseContact.py
+# Date:  29-Sep-2020  Zukang Feng
 #
 # Update:
-# 28-Feb -2014  Add base class
 ##
 """
-Manage utility to remove or rename  terminal OXT atoms.
+Manage utility to correct TLS problems
 
 """
 __docformat__ = "restructuredtext en"
-__author__ = "John Westbrook"
-__email__ = "jwest@rcsb.rutgers.edu"
+__author__ = "Zukang Feng"
+__email__ = "zfeng@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.07"
 
 import sys
 import os.path
 import os
 import traceback
 
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
 from wwpdb.apps.ann_tasks_v2.utils.SessionWebDownloadUtils import SessionWebDownloadUtils
 
 
-class TerminalAtoms(SessionWebDownloadUtils):
+class UpdateCloseContact(SessionWebDownloadUtils):
     """
-    TerminalAtoms class encapsulates removing or renaming  terminal OXT atoms.
+    UpdateCloseContact class encapsulates correcting close contact problems.
 
     """
 
     def __init__(self, reqObj=None, verbose=False, log=sys.stderr):
-        super(TerminalAtoms, self).__init__(reqObj=reqObj, verbose=verbose, log=log)
+        super(UpdateCloseContact, self).__init__(reqObj=reqObj, verbose=verbose, log=log)
         self.__verbose = verbose
         self.__lfh = log
         self.__reqObj = reqObj
-        self.__status = "none"
         #
         self.__setup()
 
     def __setup(self):
         self.__siteId = self.__reqObj.getValue("WWPDB_SITE_ID")
         self.__sObj = self.__reqObj.getSessionObj()
         self.__sessionPath = self.__sObj.getPath()
 
-    def getLastStatus(self):
-        return self.__status
-
     def __checkStatus(self, logFilePath):
-        status = "ok"
+        status = "error"
         if os.access(logFilePath, os.R_OK):
             ifh = open(logFilePath, "r")
             for line in ifh:
-                if str(line).upper().startswith("++ERROR"):
-                    return "error"
-                if str(line).upper().startswith("++WARN"):
-                    return "warn"
-            ifh.close()
-        else:
-            return "error"
-
+                if str(line).startswith("Finished!"):
+                    status = "ok"
+                    break
+                #
+            #
+        #
         return status
 
-    def run(self, entryId, inpFile, updateInput=True, updateOption="delete"):
-        """Run the calculation - updateOption = delete|rename"""
+    def run(self, entryId, inpFile, closeContactList):
+        """Run the calculation"""
         try:
             inpPath = os.path.join(self.__sessionPath, inpFile)
-            logPath1 = os.path.join(self.__sessionPath, entryId + "-terminal-atoms.log")
-            retPath = os.path.join(self.__sessionPath, entryId + "_model-updated_P1.cif")
+            logPath = os.path.join(self.__sessionPath, entryId + "-close-contact.log")
+            dataPath = os.path.join(self.__sessionPath, entryId + "-close-contact.txt")
+            for filePath in (logPath, dataPath):
+                if os.access(filePath, os.R_OK):
+                    os.remove(filePath)
+                #
+            #
+            ofh = open(dataPath, "w")
+            for closeContact in closeContactList:
+                ofh.write("%s\n" % closeContact)
+            #
+            ofh.close()
             #
+            status = False
             dp = RcsbDpUtility(tmpPath=self.__sessionPath, siteId=self.__siteId, verbose=self.__verbose, log=self.__lfh)
+            #
             dp.imp(inpPath)
-            dp.addInput(name="option", value=updateOption)
-
-            dp.op("annot-update-terminal-atoms")
-            dp.expLog(logPath1)
-            dp.exp(retPath)
-            self.addDownloadPath(retPath)
-            self.addDownloadPath(logPath1)
-            if updateInput:
-                dp.exp(inpPath)
-
+            dp.addInput(name="datafile", value=dataPath)
+            dp.op("annot-convert-close-contact-to-link")
+            dp.expLog(dstPath=logPath, appendMode=False)
+            if os.access(logPath, os.R_OK):
+                self.addDownloadPath(logPath)
+                if self.__checkStatus(logPath) == "ok":
+                    dp.exp(inpPath)
+                    self.addDownloadPath(inpPath)
+                    status = True
+                #
             #
-            self.__status = self.__checkStatus(logPath1)
-            if self.__verbose:
-                self.__lfh.write("+TerminalAtoms.run-  completed with status %s for entryId %s file %s\n" % (self.__status, entryId, inpPath))
-
             dp.cleanup()
-            return True
+            return status
         except:  # noqa: E722 pylint: disable=bare-except
             traceback.print_exc(file=self.__lfh)
             return False
+        #
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/TlsRange.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/utils/UpdateCloseContact.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/utils/PublicPdbxFile.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,95 +1,114 @@
 ##
-# File:  UpdateCloseContact.py
-# Date:  29-Sep-2020  Zukang Feng
+# File:  PublicPdbxFile.py
+# Date:  14-Oct-2013
 #
 # Update:
+# 28-Feb -2014  jdw Add base class
+# 4-Jun-2014    jdw Added V4 dictionary argument --
+# 25-May-2023   zf  Added run_conversion() method to generate different flavor of public PDBx/mmCIF files
 ##
 """
-Manage utility to correct TLS problems
+Generate public pdbx cif file.
 
 """
 __docformat__ = "restructuredtext en"
 __author__ = "Zukang Feng"
 __email__ = "zfeng@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.07"
 
-import sys
-import os.path
 import os
+import os.path
+import sys
 import traceback
+import inspect
 
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
-from wwpdb.apps.ann_tasks_v2.utils.SessionWebDownloadUtils import SessionWebDownloadUtils
 
+from wwpdb.apps.ann_tasks_v2.utils.SessionWebDownloadUtils import SessionWebDownloadUtils
 
-class UpdateCloseContact(SessionWebDownloadUtils):
-    """
-    UpdateCloseContact class encapsulates correcting close contact problems.
 
-    """
+class PublicPdbxFile(SessionWebDownloadUtils):
+    """The PublicPdbxFile class encapsulates conversion internal pdbx cif to public pdbx cif file."""
 
     def __init__(self, reqObj=None, verbose=False, log=sys.stderr):
-        super(UpdateCloseContact, self).__init__(reqObj=reqObj, verbose=verbose, log=log)
-        self.__verbose = verbose
-        self.__lfh = log
+        super(PublicPdbxFile, self).__init__(reqObj=reqObj, verbose=verbose, log=log)
+        self._verbose = verbose
+        self._lfh = log
         self.__reqObj = reqObj
-        #
+        self._debug = False
         self.__setup()
+        #
+        self.__opMap = { "annot-cif-to-public-pdbx": ( "_model-review_P1.cif", "-public_cif.log" ), \
+                         "cif2pdbx-ext": ( "_model-next_P1.cif", "_cif2pdbx-next.log" ), \
+                         "cif2pdbx-public": ( "_model-v4-pubic_P1.cif", "_cif2pdbx-pubic.log" ) }
+        #
 
     def __setup(self):
-        self.__siteId = self.__reqObj.getValue("WWPDB_SITE_ID")
+        self._siteId = self.__reqObj.getValue("WWPDB_SITE_ID")
         self.__sObj = self.__reqObj.getSessionObj()
-        self.__sessionPath = self.__sObj.getPath()
-
-    def __checkStatus(self, logFilePath):
-        status = "error"
-        if os.access(logFilePath, os.R_OK):
-            ifh = open(logFilePath, "r")
-            for line in ifh:
-                if str(line).startswith("Finished!"):
-                    status = "ok"
-                    break
-                #
-            #
+        self._sessionPath = self.__sObj.getPath()
+        self._exportPath = self._sessionPath
+        self._cleanup = False
+
+    def setExportPath(self, exportPath):
+        """ Set the path where output files are copyied.
+        """
+        self._exportPath = exportPath
+
+    def run(self, entryId, inpFile):
+        """ Create review model file
+        """
+        inpPath = os.path.join(self._sessionPath, inpFile)
+        if self.run_conversion("annot-cif-to-public-pdbx", entryId, inpPath):
+            return True
         #
-        return status
+        return False
 
-    def run(self, entryId, inpFile, closeContactList):
-        """Run the calculation"""
+    def run_conversion(self, op, entryId, inpPath):
+        """ Run conversion.
+        """
         try:
-            inpPath = os.path.join(self.__sessionPath, inpFile)
-            logPath = os.path.join(self.__sessionPath, entryId + "-close-contact.log")
-            dataPath = os.path.join(self.__sessionPath, entryId + "-close-contact.txt")
-            for filePath in (logPath, dataPath):
+            if op not in self.__opMap:
+                return
+            #
+            pdbxPath = os.path.join(self._exportPath, entryId + self.__opMap[op][0])
+            logPath  = os.path.join(self._exportPath, entryId + self.__opMap[op][1])
+            #
+            for filePath in (pdbxPath, logPath):
                 if os.access(filePath, os.R_OK):
                     os.remove(filePath)
                 #
             #
-            ofh = open(dataPath, "w")
-            for closeContact in closeContactList:
-                ofh.write("%s\n" % closeContact)
+            dp = RcsbDpUtility(tmpPath=self._sessionPath, siteId=self._siteId, verbose=self._verbose, log=self._lfh)
+            if self._debug:
+                dp.setDebugMode(flag=True)
             #
-            ofh.close()
+            dp.imp(inpPath)
+            if op == "cif2pdbx-ext":
+                dp.addInput(name="destination", value="archive_next")
             #
-            status = False
-            dp = RcsbDpUtility(tmpPath=self.__sessionPath, siteId=self.__siteId, verbose=self.__verbose, log=self.__lfh)
+            dp.op(op)
+            dp.exp(pdbxPath)
+            dp.expLog(logPath)
             #
-            dp.imp(inpPath)
-            dp.addInput(name="datafile", value=dataPath)
-            dp.op("annot-convert-close-contact-to-link")
-            dp.expLog(dstPath=logPath, appendMode=False)
-            if os.access(logPath, os.R_OK):
+            if op != "annot-cif-to-public-pdbx":
+                self.addDownloadPath(pdbxPath)
                 self.addDownloadPath(logPath)
-                if self.__checkStatus(logPath) == "ok":
-                    dp.exp(inpPath)
-                    self.addDownloadPath(inpPath)
-                    status = True
-                #
             #
-            dp.cleanup()
-            return status
+            if self._verbose:
+                self._lfh.write("+%s.%s  creating public cif for entryId %s file %s\n" % (self.__class__.__name__, \
+                                 inspect.currentframe().f_code.co_name, entryId, inpPath))
+            #
+            if self._cleanup:
+                dp.cleanup()
+            #
+            return pdbxPath
         except:  # noqa: E722 pylint: disable=bare-except
-            traceback.print_exc(file=self.__lfh)
-            return False
+            if self._verbose:
+                self._lfh.write("+%s.%s public cif conversion failed for entryId %s file %s\n" % (self.__class__.__name__, \
+                                inspect.currentframe().f_code.co_name, entryId, inpPath))
+            #
+            traceback.print_exc(file=self._lfh)
         #
+        return None
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/validate/Validate.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/validate/Validate.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/view3d/ModelViewer3D.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebApp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/AnnTasksWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/CommonTasksWebAppWorker.py`

 * *Files 1% similar despite different names*

```diff
@@ -76,15 +76,17 @@
 from wwpdb.utils.wf.dbapi.WfTracking import WfTracking
 from wwpdb.utils.wf.process.ProcessRunner import ProcessRunner
 from wwpdb.utils.wf.WfDataObject import WfDataObject
 
 from wwpdb.apps.ann_tasks_v2.assembly.AssemblyInput import AssemblyInput
 from wwpdb.apps.ann_tasks_v2.assembly.AssemblySelect import AssemblySelect
 from wwpdb.apps.ann_tasks_v2.check.Check import Check
+from wwpdb.apps.ann_tasks_v2.check.XmlCheck import XmlCheck
 from wwpdb.apps.ann_tasks_v2.check.EmdXmlCheck import EmdXmlCheck
+from wwpdb.apps.ann_tasks_v2.check.EmMapCheck import EmMapCheck
 from wwpdb.apps.ann_tasks_v2.check.ExtraCheck import ExtraCheck
 from wwpdb.apps.ann_tasks_v2.check.FormatCheck import FormatCheck
 from wwpdb.apps.ann_tasks_v2.check.GeometryCalc import GeometryCalc
 from wwpdb.apps.ann_tasks_v2.check.GeometryCheck import GeometryCheck
 
 #
 from wwpdb.apps.ann_tasks_v2.correspnd.CorresPNDGenerator import CorresPNDGenerator
@@ -1595,14 +1597,18 @@
         pth = de.copyToSession(contentType="validation-report-2fo-map-coef", formatType="pdbx", version="latest", partitionNumber=1)
         pth = de.copyToSession(contentType="validation-report-fo-map-coef", formatType="pdbx", version="latest", partitionNumber=1)
         #
         # dictionary check file
         #
         pth = de.copyToSession(contentType="dict-check-report", formatType="txt", version="latest", partitionNumber=1)
         #
+        # PDBML XML check file
+        #
+        pth = de.copyToSession(contentType="xml-check-report", formatType="txt", version="latest", partitionNumber=1)
+        #
         #  Handle maps if input option is set --
         if getMaps:
             pth = de.copyToSession(contentType="map-2fofc", formatType="map", version="latest", partitionNumber=1)
             pth = de.copyToSession(contentType="map-fofc", formatType="map", version="latest", partitionNumber=1)
             pth = de.copyToSession(contentType="map-omit-2fofc", formatType="map", version="latest", partitionNumber=1)
             pth = de.copyToSession(contentType="map-omit-fofc", formatType="map", version="latest", partitionNumber=1)
             de.copyDirToSession(dirName="np-cc-maps")
@@ -2040,14 +2046,15 @@
         Content types --
 
         'model'                       :  (['pdbx'], 'model'),
         'model-pdb'                   :  (['pdb'], 'model'),
         'dict-check-report'           :  (['txt'], 'dict-check-report'),
         'dict-check-report-r4'        :  (['txt'], 'dict-check-report-r4'),
         'dict-check-report-next'      :  (['txt'], 'dict-check-report-next'),
+        'xml-check-report'            :  (['txt'], 'xml-check-report'),
         'format-check-report'         :  (['txt'], 'format-check-report'),
         'misc-check-report'           :  (['txt'], 'misc-check-report'),
         'special-position-report'     :  (['txt'], 'special-position-report'),
         'dcc-report'                  :  (['pdbx','txt'], 'dcc-report'),
         'geometry-check-report'       :  (['pdbx'],'geometry-check-report'),
 
         Special key 'entry-info' contains a dictionary of items to populate page  header/title -
@@ -2066,16 +2073,18 @@
             "dcc-report",
             "geometry-check-report",
             "misc-check-report",
             "format-check-report",
             "dict-check-report",
             "dict-check-report-r4",
             "dict-check-report-next",
+            "xml-check-report",
             "special-position-report",
             "emd-xml-header-report",
+            "em-map-check-report",
             "downloads",
         ]:
             myD[ky] = None
         myD["entry-info"] = {
             "pdb_id": "",
             "struct_title": "",
             "my_entry_id": entryId,
@@ -2170,14 +2179,23 @@
                 if ok:
                     downloadPath = du.getDownloadPath()
                     aTagList.append(du.getAnchorTag())
                     myD[cT] = self.__getFileTextWithMarkup(downloadPath)
                 else:
                     # myD[cT] = self.__getMessageTextWithMarkup('No dictionary check issues.')
                     myD[cT] = self.__getMessageTextWithMarkup("")
+            elif cT == "xml-check-report":
+                # Dictionary check report
+                ok = du.fetchId(entryId, contentType="xml-check-report", formatType="txt", fileSource=fileSource, instance=instance)
+                if ok:
+                    downloadPath = du.getDownloadPath()
+                    aTagList.append(du.getAnchorTag())
+                    myD[cT] = self.__getFileTextWithMarkup(downloadPath)
+                else:
+                    myD[cT] = self.__getMessageTextWithMarkup("")
             elif cT == "dict-check-report-r4":
                 # Dictionary check report
                 ok = du.fetchId(entryId, contentType="dict-check-report-r4", formatType="txt", fileSource=fileSource, instance=instance)
                 if ok:
                     downloadPath = du.getDownloadPath()
                     aTagList.append(du.getAnchorTag())
                     myD[cT] = self.__getFileTextWithMarkup(downloadPath)
@@ -2190,14 +2208,24 @@
                 if ok:
                     downloadPath = du.getDownloadPath()
                     aTagList.append(du.getAnchorTag())
                     myD[cT] = self.__getFileTextWithMarkup(downloadPath)
                 else:
                     # myD[cT] = self.__getMessageTextWithMarkup('No dictionary check issues.')
                     myD[cT] = self.__getMessageTextWithMarkup("")
+            elif cT == "xml-check-report":
+                # Xml check report
+                ok = du.fetchId(entryId, contentType="xml-check-report", formatType="txt", fileSource=fileSource, instance=instance)
+                if ok:
+                    downloadPath = du.getDownloadPath()
+                    aTagList.append(du.getAnchorTag())
+                    myD[cT] = self.__getFileTextWithMarkup(downloadPath)
+                else:
+                    # myD[cT] = self.__getMessageTextWithMarkup('No xml check issues.')
+                    myD[cT] = self.__getMessageTextWithMarkup("")
             elif cT == "special-position-report":
                 #
                 ok = du.fetchId(entryId, contentType="special-position-report", formatType="txt", fileSource=fileSource, instance=instance)
                 if ok:
                     downloadPath = du.getDownloadPath()
                     aTagList.append(du.getAnchorTag())
                     myD[cT] = self.__getFileTextWithMarkup(downloadPath)
@@ -2214,14 +2242,24 @@
                     downloadPath = du.getDownloadPath()
                     aTagList.append(du.getAnchorTag())
                     myD[cT] = self.__getFileTextWithMarkup(downloadPath)
                 else:
                     # myD[cT] = self.__getMessageTextWithMarkup('No XML generation report.')
                     myD[cT] = self.__getMessageTextWithMarkup("")
 
+            elif cT == "em-map-check-report":
+                # em_map checking report
+                ok = du.fetchId(entryId, contentType="em-map-check-report", formatType="txt", fileSource=fileSource, instance=instance)
+                if ok:
+                    downloadPath = du.getDownloadPath()
+                    aTagList.append(du.getAnchorTag())
+                    myD[cT] = self.__getFileTextWithMarkup(downloadPath)
+                else:
+                    myD[cT] = self.__getMessageTextWithMarkup("")
+
         # downloads
 
         for data_file in (
             ("model", "pdbx"),
             ("model", "pdb"),
             ("structure-factors", "pdbx"),
             ("nmr-chemical-shifts", "pdbx"),
@@ -2301,20 +2339,22 @@
              and return a list of html anchors tags for the report files.
 
         Content type list --
 
         'dict-check-report'           :  (['txt'], 'dict-check-report'),
         'dict-check-report-r4'        :  (['txt'], 'dict-check-report-r4'),
         'dict-check-report-next'      :  (['txt'], 'dict-check-report-next'),
+        'xml-check-report'            :  (['txt'], 'xml-check-report'),
         'format-check-report'         :  (['txt'], 'format-check-report'),
         'misc-check-report'           :  (['txt'], 'misc-check-report'),
         'special-position-report'     :  (['txt'], 'special-position-report'),
         'dcc-report'                  :  (['pdbx','txt'], 'dcc-report'),
         'geometry-check-report'       :  (['pdbx'],'geometry-check-report'),
         'emd-xml-header-report'       :  (['txt'], 'emd-xml-header-report'),
+        'em-map-check-report'         :  (['txt'], 'em-map-check-report'),
 
         """
         #
         if operationList is None:
             operationList = ["check"]
 
         if useFileVersions:
@@ -2344,42 +2384,68 @@
             if "checkv5" in operationList:
                 chk = Check(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
                 chk.setDictionaryVersion(version="V5")
                 # Internal model file - check first block only
                 chk.setCheckFirstBlock(True)
 
                 chk.run(entryId=entryId, inpPath=modelFilePath)
+                rptPath = chk.getReportPath()
                 hasDiags = chk.getReportSize() > 0
                 if hasDiags:
-                    rptPath = chk.getReportPath()
                     duL.copyToDownload(rptPath)
                     aTagList.append(duL.getAnchorTag())
+                else:
+                    duL.removeFromDownload(rptPath)
 
             if "checkv4" in operationList:
                 chk = Check(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
                 chk.setDictionaryVersion(version="V4")
                 chk.run(entryId=entryId, inpPath=modelFilePath)
+                rptPath = chk.getReportPath()
                 hasDiags = chk.getReportSize() > 0
                 if hasDiags:
-                    rptPath = chk.getReportPath()
                     duL.copyToDownload(rptPath)
                     aTagList.append(duL.getAnchorTag())
+                else:
+                    duL.removeFromDownload(rptPath)
 
             if "checkNext" in operationList:
                 self._lfh.write("+CommonTasksWebAppWorker._makeCheckReports() starting checkNext\n")
 
                 chk = Check(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
                 # Public check - should have first block only
                 chk.setDictionaryVersion(version="archive_next")
                 chk.run(entryId=entryId, inpPath=modelFilePath)
+                rptPath = chk.getReportPath()
+                hasDiags = chk.getReportSize() > 0
+                if hasDiags:
+                    duL.copyToDownload(rptPath)
+                    aTagList.append(duL.getAnchorTag())
+                else:
+                    duL.removeFromDownload(rptPath)
+
+            if "checkxml" in operationList:
+                self._lfh.write("+CommonTasksWebAppWorker._makeCheckReports() starting checkxml\n")
+
+                chk = XmlCheck(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
+                pdbxPath = os.path.join(self._sessionPath, entryId + "_model-next_P1.cif") 
+                if os.access(pdbxPath, os.R_OK):
+                    self._lfh.write("+CommonTasksWebAppWorker._makeCheckReports() starting checkxml using %s\n" % pdbxPath)
+                    chk.run(entryId=entryId, inpPath=pdbxPath, publicCIFlag=True)
+                else:
+                    self._lfh.write("+CommonTasksWebAppWorker._makeCheckReports() starting checkxml using %s\n" % modelFilePath)
+                    chk.run(entryId=entryId, inpPath=modelFilePath, publicCIFlag=False)
+                #
+                rptPath = chk.getReportPath()
                 hasDiags = chk.getReportSize() > 0
                 if hasDiags:
-                    rptPath = chk.getReportPath()
                     duL.copyToDownload(rptPath)
                     aTagList.append(duL.getAnchorTag())
+                else:
+                    duL.removeFromDownload(rptPath)
 
             if "check-format" in operationList:
                 chk = FormatCheck(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
                 chk.run(entryId=entryId, inpPath=modelFilePath)
                 hasDiags = chk.getReportSize() > 0
                 if hasDiags:
                     rptPath = chk.getReportPath()
@@ -2410,27 +2476,42 @@
                 hasDiags = chk.getReportSize() > 0
                 if hasDiags:
                     rptPath = chk.getReportPath()
                     duL.copyToDownload(rptPath)
                     aTagList.append(duL.getAnchorTag())
 
             if "check-emd-xml" in operationList:
+                print("XXXXXXXXXX About to start")
                 try:
                     chk = EmdXmlCheck(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
                     chk.run(entryId=entryId, modelInputFile=modelFilePath)
                 except Exception as e:
                     logger.error("Error running EmdXmlCheck %s", e)
                 hasDiags = chk.getReportSize() > 0
                 rptPath = chk.getReportPath()
                 if hasDiags:
                     duL.copyToDownload(rptPath)
                     aTagList.append(duL.getAnchorTag())
                 else:
                     duL.removeFromDownload(rptPath)
 
+            if "check-em-map" in operationList:
+                try:
+                    chk = EmMapCheck(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
+                    chk.run(entryId=entryId, modelInputFile=modelFilePath)
+                except Exception as e:
+                    logger.error("Error running EmMapCheck %s", e)
+                hasDiags = chk.getReportSize() > 0
+                rptPath = chk.getReportPath()
+                if hasDiags:
+                    duL.copyToDownload(rptPath)
+                    aTagList.append(duL.getAnchorTag())
+                else:
+                    duL.removeFromDownload(rptPath)
+
             if "check-sf" in operationList:
                 ok = duL.fetchId(entryId, contentType="structure-factors", formatType="pdbx", fileSource=fileSource, versionId=versionId)
                 expFilePath = duL.getDownloadPath()
                 chk = DccCalc(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
                 ok = chk.run(entryId=entryId, modelInputPath=modelFilePath, expInputPath=expFilePath)
                 if ok:
                     rptPath = chk.getReportPath()
@@ -2534,27 +2615,30 @@
         #
         # opCtD - this dictionary maps input check request operation names to project report content types -
         #
         opCtD = {
             "checkv5": "dict-check-report",
             # 'checkv4': 'dict-check-report-r4',
             "checkNext": "dict-check-report-next",
+            "checkxml": "xml-check-report",
             "check-misc": "misc-check-report",
             "check-format": "format-check-report",
             "check-geometry": "geometry-check-report",
             "check-sf": "dcc-report",
             "check-special-position": "special-position-report",
             "cif2pdb": "model-pdb",
             "check-emd-xml": "emd-xml-header-report",
+            "check-em-map": "em-map-check-report"
         }
 
         rC = ResponseContent(reqObj=self._reqObj, verbose=self._verbose, log=self._lfh)
         rC.setReturnFormat("json")
         if operation in ["check-all"]:
-            opList = ["cif2pdb", "checkv5", "checkNext", "check-format", "check-misc", "check-geometry", "check-special-position", "check-sf", "check-emd-xml"]
+            opList = ["cif2pdb", "checkv5", "checkNext", "checkxml", "check-format", "check-misc", "check-geometry", "check-special-position", \
+                      "check-sf", "check-emd-xml", "check-em-map"]
             aTagList = self._makeCheckReports([entryId], operationList=opList, fileSource=fileSource, useFileVersions=useFileVersions)
             cTList = ["model"]
             cTList.extend(sorted(opCtD.values()))
             if self._verbose:
                 self._lfh.write("+ReviewDataWebAppWorker._reviewDataInlineIdOps() content type list %r\n" % cTList)
             myD = self._renderCheckReports(entryId, fileSource="session-download", instance=None, contentTypeList=cTList, useModelFileVersion=useFileVersions)
             rC.setHtmlTextFromTemplate(templateFilePath=templateFilePath, webIncludePath=webIncludePath, parameterDict=myD, insertContext=True)
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/ReviewDataWebAppWorker.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,22 +164,23 @@
                 chk.setDictionaryVersion(version="V4")
             elif operation in ["checkv5"]:
                 chk.setDictionaryVersion(version="V5")
             elif operation in ["checkNext"]:
                 chk.setDictionaryVersion(version="archive_next")
             chk.run(entryId=idCode, inpPath=filePath)
             hasDiags = chk.getReportSize() > 0
+            rptPath = chk.getReportPath()
+            duL = SessionDownloadUtils(self._reqObj, verbose=self._verbose, log=self._lfh)
             if hasDiags:
-                rptPath = chk.getReportPath()
-                duL = SessionDownloadUtils(self._reqObj, verbose=self._verbose, log=self._lfh)
                 duL.copyToDownload(rptPath)
                 aTagList.append(duL.getAnchorTag())
                 rC.setHtmlLinkText('<span class="url-list">Download: %s</span>' % ",".join(aTagList))
                 rC.setStatus(statusMsg="Check completed")
             else:
+                duL.removeFromDownload(rptPath)
                 rC.setStatus(statusMsg="No diagnostics for %s" % fileName)
 
         if hasDiags and operation in ["updatewithcheck"]:
             return rC
 
         if operation in ["update", "updatewithcheck"]:
             if (idCode is None) or (len(idCode) < 1) or (contentType is None) or (len(contentType) < 1) or (contentFormat is None) or (len(contentFormat) < 1):
@@ -291,14 +292,15 @@
                 "check-format",
                 "check-misc",
                 "check-geometry",
                 "check-sf",
                 # 'cif2pdb',
                 "check-special-position",
                 "check-emd-xml",
+                "check-em-map"
             ]
             _aTagList = self._makeCheckReports([idCode], operationList=opList)  # noqa: F841
         #
         #
         if self._verbose:
             self._lfh.write("\n\n+ReviewDataWebAppWorker._generateFullHtmlCheckReport() idCode %s generating reports from data files in fileSource %s\n" % (idCode, fileSource))
         #
@@ -306,16 +308,18 @@
             "model",
             "dcc-report",
             "special-position-report",
             "geometry-check-report",
             "misc-check-report",
             "format-check-report",
             "dict-check-report",
+            "xml-check-report",
             # 'model-pdb',
             "emd-xml-header-report",
+            "em-map-check-report",
             "downloads",
         ]
         reportD = self._renderCheckReports(idCode, fileSource=fileSource, instance=instance, contentTypeList=cTL)
         #
         reportD["sessionid"] = self._reqObj.getSessionId()
         reportD["entryid"] = idCode
         #
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/StatusUpdateWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb/apps/ann_tasks_v2/webapp/ValidationTasksWebAppWorker.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.ann-tasks-v2
-Version: 0.32
+Version: 0.33
 Summary: wwPDB annotation/review/status/validation module backend
 Home-page: https://github.com/rcsb/py-wwpdb_apps_ann_tasks_v2
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.ann_tasks_v2-0.32/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt` & `wwpdb.apps.ann_tasks_v2-0.33/wwpdb.apps.ann_tasks_v2.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -10,19 +10,21 @@
 wwpdb.apps.ann_tasks_v2.egg-info/top_level.txt
 wwpdb/apps/__init__.py
 wwpdb/apps/ann_tasks_v2/__init__.py
 wwpdb/apps/ann_tasks_v2/assembly/AssemblyInput.py
 wwpdb/apps/ann_tasks_v2/assembly/AssemblySelect.py
 wwpdb/apps/ann_tasks_v2/assembly/__init__.py
 wwpdb/apps/ann_tasks_v2/check/Check.py
+wwpdb/apps/ann_tasks_v2/check/EmMapCheck.py
 wwpdb/apps/ann_tasks_v2/check/EmdXmlCheck.py
 wwpdb/apps/ann_tasks_v2/check/ExtraCheck.py
 wwpdb/apps/ann_tasks_v2/check/FormatCheck.py
 wwpdb/apps/ann_tasks_v2/check/GeometryCalc.py
 wwpdb/apps/ann_tasks_v2/check/GeometryCheck.py
+wwpdb/apps/ann_tasks_v2/check/XmlCheck.py
 wwpdb/apps/ann_tasks_v2/check/__init__.py
 wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDGenerator.py
 wwpdb/apps/ann_tasks_v2/correspnd/CorresPNDTemplate.py
 wwpdb/apps/ann_tasks_v2/correspnd/ValidateXml.py
 wwpdb/apps/ann_tasks_v2/correspnd/__init__.py
 wwpdb/apps/ann_tasks_v2/density/DensityGeneration.py
 wwpdb/apps/ann_tasks_v2/density/__init__.py
```

