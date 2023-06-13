# Comparing `tmp/wwpdb.apps.seqmodule-0.24.9.dev1.tar.gz` & `tmp/wwpdb.apps.seqmodule-0.24.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.apps.seqmodule-0.24.9.dev1.tar", last modified: Tue Jun 13 10:53:46 2023, max compression
+gzip compressed data, was "wwpdb.apps.seqmodule-0.24.dev1.tar", last modified: Mon Jun 13 22:32:31 2022, max compression
```

## Comparing `wwpdb.apps.seqmodule-0.24.9.dev1.tar` & `wwpdb.apps.seqmodule-0.24.dev1.tar`

### file list

```diff
@@ -1,86 +1,86 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:53:46.110957 wwpdb.apps.seqmodule-0.24.9.dev1/
--rw-r--r--   0 vsts      (1001) docker     (123)      728 2023-06-13 10:53:46.110957 wwpdb.apps.seqmodule-0.24.9.dev1/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)       49 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)      279 2023-06-13 10:53:46.110957 wwpdb.apps.seqmodule-0.24.9.dev1/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (123)     2395 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:53:46.086957 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:53:46.090957 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/
--rw-r--r--   0 vsts      (1001) docker     (123)       65 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:53:46.090957 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/
--rw-r--r--   0 vsts      (1001) docker     (123)      157 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:53:46.090957 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/
--rw-r--r--   0 vsts      (1001) docker     (123)    24748 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentBackEndEditingTools.py
--rw-r--r--   0 vsts      (1001) docker     (123)    41710 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentDepictionTools.py
--rw-r--r--   0 vsts      (1001) docker     (123)    11005 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentExport.py
--rw-r--r--   0 vsts      (1001) docker     (123)    36179 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentFrontEndUIEditor.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16415 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentStatistics.py
--rw-r--r--   0 vsts      (1001) docker     (123)     8547 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentStatisticsTests.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10981 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentToolUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    62563 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentTools.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:53:46.094956 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/
--rw-r--r--   0 vsts      (1001) docker     (123)    22921 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/DataImporter.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5322 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/SequenceDataAssembleExample.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10781 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/SequenceDataAssembleTests.py
--rw-r--r--   0 vsts      (1001) docker     (123)    54712 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/SequenceDataAssemble_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)    17428 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/SequenceDataPrepTests.py
--rw-r--r--   0 vsts      (1001) docker     (123)    21259 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/SummaryViewDepiction.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13712 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/SummaryViewTests.py
--rw-r--r--   0 vsts      (1001) docker     (123)    45386 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/SummaryView_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:53:46.102957 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/
--rw-r--r--   0 vsts      (1001) docker     (123)    26442 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/AlignmentDataStore.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10295 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/BlastPlusReader.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9979 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/FetchSeqInfoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    14298 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/ModelSequenceUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6195 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/ModelSequenceUtilsTests.py
--rw-r--r--   0 vsts      (1001) docker     (123)    72352 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/PdbxIoUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10250 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/SequenceDataExportTests.py
--rw-r--r--   0 vsts      (1001) docker     (123)    35573 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/SequenceDataExport_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)    26125 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/SequenceDataStore.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9251 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/SequenceDataStoreTests.py
--rw-r--r--   0 vsts      (1001) docker     (123)    10047 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/SequenceEditStore.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9165 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/SequenceEditStoreTests.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1822 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/TaxonomyDbUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7438 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/TaxonomyUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     9497 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/TaxonomyUtilsTests.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)      638 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/testAuto.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:53:46.102957 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/link/
--rw-r--r--   0 vsts      (1001) docker     (123)     3032 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/link/PolymerLinkageDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/link/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:53:46.102957 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/update/
--rw-r--r--   0 vsts      (1001) docker     (123)    38471 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/update/UpdatePolymerEntityPartitions.py
--rw-r--r--   0 vsts      (1001) docker     (123)    12325 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/update/UpdatePolymerEntityReference_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)    37375 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/update/UpdatePolymerEntitySourceDetails.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/update/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:53:46.106957 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/
--rw-r--r--   0 vsts      (1001) docker     (123)     1614 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/Autodict.py
--rw-r--r--   0 vsts      (1001) docker     (123)    13790 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/FetchReferenceSequenceUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    25653 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/GetSameSeqAnnotationWithTaxIdOnly.py
--rw-r--r--   0 vsts      (1001) docker     (123)    48387 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/LocalBlastSearchUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1554 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/MultiProcLimit.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6271 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/SearchEntityPolySeqs.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4902 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/SeqReferenceSearchUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)    22278 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/SequenceAssign.py
--rw-r--r--   0 vsts      (1001) docker     (123)    91749 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/SequenceExamples.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16288 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/SequenceFeatureDepict.py
--rw-r--r--   0 vsts      (1001) docker     (123)    46003 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/SequenceLabel.py
--rw-r--r--   0 vsts      (1001) docker     (123)    16959 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/SequenceReferenceData.py
--rw-r--r--   0 vsts      (1001) docker     (123)    29391 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/UpdateSequenceDataStoreUtils.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:53:46.106957 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/view3d/
--rw-r--r--   0 vsts      (1001) docker     (123)     6541 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/view3d/ModelViewer3D.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/view3d/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:53:46.106957 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/webapp/
--rw-r--r--   0 vsts      (1001) docker     (123)    67721 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/webapp/SeqModWebApp_v2.py
--rw-r--r--   0 vsts      (1001) docker     (123)    15467 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/webapp/SeqModWebRequest.py
--rw-r--r--   0 vsts      (1001) docker     (123)        0 2023-06-13 10:52:25.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/webapp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-06-13 10:53:46.086957 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb.apps.seqmodule.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)      728 2023-06-13 10:53:45.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb.apps.seqmodule.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     3265 2023-06-13 10:53:46.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb.apps.seqmodule.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 10:53:45.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb.apps.seqmodule.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-06-13 10:53:31.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb.apps.seqmodule.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)      266 2023-06-13 10:53:45.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb.apps.seqmodule.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        6 2023-06-13 10:53:45.000000 wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb.apps.seqmodule.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-13 22:32:31.470489 wwpdb.apps.seqmodule-0.24.dev1/
+-rw-r--r--   0 vsts      (1001) docker     (121)      726 2022-06-13 22:32:31.470489 wwpdb.apps.seqmodule-0.24.dev1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)       49 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (121)      108 2022-06-13 22:32:31.482490 wwpdb.apps.seqmodule-0.24.dev1/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (121)     2337 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-13 22:32:31.458489 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (121)       65 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-13 22:32:31.462489 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/
+-rw-r--r--   0 vsts      (1001) docker     (121)       65 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-13 22:32:31.462489 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/
+-rw-r--r--   0 vsts      (1001) docker     (121)      155 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-13 22:32:31.462489 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/
+-rw-r--r--   0 vsts      (1001) docker     (121)    24748 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentBackEndEditingTools.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    41660 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentDepictionTools.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    11005 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentExport.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    36179 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentFrontEndUIEditor.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16415 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentStatistics.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     8547 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentStatisticsTests.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10981 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentToolUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    61840 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentTools.py
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-13 22:32:31.462489 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/
+-rw-r--r--   0 vsts      (1001) docker     (121)    22921 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/DataImporter.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5322 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/SequenceDataAssembleExample.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10781 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/SequenceDataAssembleTests.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    52444 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/SequenceDataAssemble_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    17428 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/SequenceDataPrepTests.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    21259 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/SummaryViewDepiction.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    13712 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/SummaryViewTests.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    30389 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/SummaryView_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-13 22:32:31.466489 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/
+-rw-r--r--   0 vsts      (1001) docker     (121)    26122 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/AlignmentDataStore.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     7917 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/BlastPlusReader.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     5784 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/FetchSeqInfoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    14298 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/ModelSequenceUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6195 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/ModelSequenceUtilsTests.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    72352 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/PdbxIoUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10250 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/SequenceDataExportTests.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    35573 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/SequenceDataExport_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    26125 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/SequenceDataStore.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9251 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/SequenceDataStoreTests.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    10047 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/SequenceEditStore.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9165 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/SequenceEditStoreTests.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1822 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/TaxonomyDbUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6722 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/TaxonomyUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9497 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/TaxonomyUtilsTests.py
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (121)      638 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/testAuto.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-13 22:32:31.466489 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/link/
+-rw-r--r--   0 vsts      (1001) docker     (121)     3032 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/link/PolymerLinkageDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/link/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-13 22:32:31.466489 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/update/
+-rw-r--r--   0 vsts      (1001) docker     (121)    38348 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/update/UpdatePolymerEntityPartitions.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    12404 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/update/UpdatePolymerEntityReference_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    37399 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/update/UpdatePolymerEntitySourceDetails.py
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/update/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-13 22:32:31.470489 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/
+-rw-r--r--   0 vsts      (1001) docker     (121)     1614 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/Autodict.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     9548 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/FetchReferenceSequenceUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    24030 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/GetSameSeqAnnotationWithTaxIdOnly.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    41935 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/LocalBlastSearchUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     1554 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/MultiProcLimit.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     6271 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/SearchEntityPolySeqs.py
+-rw-r--r--   0 vsts      (1001) docker     (121)     4557 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/SeqReferenceSearchUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    22278 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/SequenceAssign.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    91749 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/SequenceExamples.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15842 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/SequenceFeatureDepict.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    45865 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/SequenceLabel.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    16959 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/SequenceReferenceData.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    28101 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/UpdateSequenceDataStoreUtils.py
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-13 22:32:31.470489 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/view3d/
+-rw-r--r--   0 vsts      (1001) docker     (121)     6541 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/view3d/ModelViewer3D.py
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/view3d/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-13 22:32:31.470489 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/webapp/
+-rw-r--r--   0 vsts      (1001) docker     (121)    65657 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/webapp/SeqModWebApp_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (121)    15467 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/webapp/SeqModWebRequest.py
+-rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-06-13 22:30:47.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/webapp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-06-13 22:32:31.462489 wwpdb.apps.seqmodule-0.24.dev1/wwpdb.apps.seqmodule.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (121)      726 2022-06-13 22:32:30.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb.apps.seqmodule.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (121)     3265 2022-06-13 22:32:31.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb.apps.seqmodule.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-13 22:32:30.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb.apps.seqmodule.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-06-13 22:31:43.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb.apps.seqmodule.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (121)      222 2022-06-13 22:32:31.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb.apps.seqmodule.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (121)        6 2022-06-13 22:32:31.000000 wwpdb.apps.seqmodule-0.24.dev1/wwpdb.apps.seqmodule.egg-info/top_level.txt
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/PKG-INFO` & `wwpdb.apps.seqmodule-0.24.dev1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.seqmodule
-Version: 0.24.9.dev1
+Version: 0.24.dev1
 Summary: wwPDB sequence module
 Home-page: https://github.com/wwPDB/py-wwpdb_apps_seqmodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/setup.py` & `wwpdb.apps.seqmodule-0.24.dev1/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -38,23 +38,23 @@
         "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
     ],
     #
     install_requires=[
-        "wwpdb.utils.config >= 0.33",
-        "wwpdb.io >= 0.27",
-        "wwpdb.utils.session >= 0.14",
-        "wwpdb.utils.wf >= 0.30",
-        "wwpdb.utils.seqdb_v2 ~= 0.11",
-        "wwpdb.utils.align >= 0.11",
-        "wwpdb.utils.detach >= 0.4.2",
-        "wwpdb.utils.dp >= 0.42",
-        "wwpdb.utils.db >= 0.28",
+        "wwpdb.utils.config >= 0.24",
+        "wwpdb.io",
+        "wwpdb.utils.session",
+        "wwpdb.utils.wf",
+        "wwpdb.utils.seqdb_v2 ~= 0.4",
+        "wwpdb.utils.align",
+        "wwpdb.utils.detach",
+        "wwpdb.utils.dp",
+        "wwpdb.utils.db",
         "rcsb.utils.multiproc",
     ],
     packages=find_packages(exclude=["wwpdb.apps.tests-seqmodule", "mock-data"]),
     # Enables Manifest to be used
     # include_package_data = True,
     package_data={
         # If any package contains *.md or *.rst ...  files, include them:
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentBackEndEditingTools.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentBackEndEditingTools.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentDepictionTools.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentDepictionTools.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,18 +66,17 @@
         """Render alignment, conflict table, annotations & warning"""
         self.__setup()
         authIdx = self._seqAlignLabelIndices[self._authLabel]
         self._checkPartStartEndPosMap(authIdx, self._authLabel)
         self.__buildAlignIndexOrder()
         self._clearAllConflicts(authIdx)
         totalSeqCoodConflict = self._assignAllConflicts(self._authLabel, self.__selectedIdList)
-        self.serialize()
         if len(self.__alignIdList) > len(self.__selectedIdList):
             self._clearAllConflicts(authIdx)
-            _numSeqCoodConflict = self._assignAllConflicts(self._authLabel, self.__alignIdList, writeConflictFlag=False)  # noqa: F841
+            _numSeqCoodConflict = self._assignAllConflicts(self._authLabel, self.__alignIdList)  # noqa: F841
         #
         self.__renderAlignment()
         self.__renderConflictTable(authIdx)
         self.__renderAnnotations()
         self.__renderWarning(authIdx)
         # self.__writeMisMatchTypeText()
         self.__updateSeqCoodConflict(totalSeqCoodConflict)
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentExport.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentExport.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentFrontEndUIEditor.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentFrontEndUIEditor.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentStatistics.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentStatistics.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentStatisticsTests.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentStatisticsTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentToolUtils.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentToolUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/align/AlignmentTools.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/align/AlignmentTools.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,46 @@
 ##
 # File:  AlignmentTools.py
 # Date:  25-Oct-2018
 #
-# Updates:
-# 29-Sep-2022: zf added 'auth_numbering' as 4th value in seqTuple for coodinate sequence in __generateInputSeqInfoForPseudoMultiAlignFromSeqList() method.
-#              added self.__conflictMap for new entity summary page.
-#
 """
 Methods to manage sequence alignments.
 """
 __docformat__ = "restructuredtext en"
 __author__ = "Zukang Feng"
 __email__ = "zfeng@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
 __version__ = "V0.09"
 
 import copy
 import os
 import sys
 import traceback
 
+from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
 from wwpdb.apps.seqmodule.align.AlignmentToolUtils import getSeqAlignment, mergeSeqAlignment, codeSeqIndex, decodeIndex, assignConflict
 from wwpdb.apps.seqmodule.io.AlignmentDataStore import AlignmentDataStore
 from wwpdb.utils.align.alignlib import PseudoMultiAlign  # pylint: disable=no-name-in-module
 from wwpdb.io.file.mmCIFUtil import mmCIFUtil
-from wwpdb.io.locator.ChemRefPathInfo import ChemRefPathInfo
 
 
 class AlignmentTools(AlignmentDataStore):
     """Manage sequence alignments"""
 
     def __init__(self, reqObj=None, entityId=None, pathInfo=None, seqDataStore=None, deserializeFlag=True, verbose=False, log=sys.stderr):
         super(AlignmentTools, self).__init__(
             reqObj=reqObj, entityId=entityId, pathInfo=pathInfo, seqDataStore=seqDataStore, deserializeFlag=deserializeFlag, verbose=verbose, log=log
         )
         #
         self._longExpressionTagCountCutoff = 20
         self.__clearLocalVariables()
         self.__local_authLabel = self._authLabel
         #
+        self.__cICommon = ConfigInfoAppCommon(self._siteId)
+        self.__ccTopPath = self.__cICommon.get_site_cc_cvs_path()
         self.__standardList = (
             "ALA",
             "ARG",
             "ASN",
             "ASP",
             "CYS",
             "GLN",
@@ -84,17 +82,27 @@
         self.__partInfoDict = {}
         self.__refAlignIndexDict = {}
         self.__selectedIdList = []
         self.__xyzLabel = []
         self.__newXyzAlignIndexListFlag = False
         self.__xyzAlignIndexList = []
         self.__extraAuthLabel = []
-        # Should be safe to initialize here - not in base class
+        # Should be safe to initialize here
         self._partPosDict = {}
+        self._seqAlignList = []
         self._selfRefPartIdList = []
+        self._authDefinedMutationList = []
+        self._xyzAlignList = []
+        self._missingSeqMap = {}
+        self._xyzAlignLabelIndices = {}
+        self._reverseXyzAlignLabelIndices = {}
+        self._hasAlignmentFlag = True
+        self._authLabel = ""
+        self._reverseSeqAlignLabelIndices = {}
+        self._seqAlignLabelIndices = {}
 
     def __clearLocalVariables(self):
         """Clear all local variables"""
         self.__local_authLabel = ""
         self.__alignFlag = True
         self.__selectedIdList = []
         self.__xyzLabel = []
@@ -587,21 +595,20 @@
                     if (not alignRecord[5].startswith("ANNOTATED:")) or (rowIdx in selfRefPosPartIdDict):
                         alignRecord[5] = ""
                     #
                 #
             #
         #
 
-    def _assignAllConflicts(self, authLabel, selectedIdList, writeConflictFlag=True):
+    def _assignAllConflicts(self, authLabel, selectedIdList):
         """Assign numeric conflicts and conflicting comments"""
         self._missingSeqMap = {}
         #
         authIdx = self._seqAlignLabelIndices[authLabel]
         #
-        self.__conflictMap = {}  # pylint: disable=attribute-defined-outside-init
         totalSeqCoodConflict = 0
         for otherIdx in sorted(self._reverseSeqAlignLabelIndices.keys()):
             otherLabel = self._reverseSeqAlignLabelIndices[otherIdx]
             if (not otherLabel.startswith("xyz")) or (otherLabel not in selectedIdList):
                 continue
             #
             numConflict, missingAuthSeqList = self.__assignNumericConflicts(authIdx, otherIdx, "xyz", 0, len(self._seqAlignList) - 1)
@@ -624,21 +631,15 @@
             end_position = len(self._seqAlignList) - 1
             if int(seqPartId) in self._partPosDict:
                 start_position = self._partPosDict[int(seqPartId)][0]
                 end_position = self._partPosDict[int(seqPartId)][1]
             #
             self.__getRefSeqVariants(otherLabel)
             numConflict, missingAuthSeqList = self.__assignNumericConflicts(authIdx, otherIdx, "ref", start_position, end_position)
-            self.__annotateConflictingComments(authIdx, otherIdx, start_position, end_position, writeConflictFlag)
-        #
-        if writeConflictFlag:
-            if totalSeqCoodConflict > 0:
-                self.__conflictMap["mismatch"] = totalSeqCoodConflict
-            #
-            self._missingSeqMap["summary_page"] = self.__conflictMap
+            self.__annotateConflictingComments(authIdx, otherIdx, start_position, end_position)
         #
         return totalSeqCoodConflict
 
     def _checkPartStartEndPosMap(self, authIdx, authLabel):
         """Get auth sequence part start & end pos range in alignment if it does not exist"""
         if self._partPosDict:
             return
@@ -1113,17 +1114,15 @@
         #
         returnSeqList = []
         for (i, seqTup) in enumerate(inputSeqList):
             if (i < start) or (i > end):
                 continue
             #
             if seqType == "xyz":
-                # added 'auth_numbering' as 4th value in seqTuple. See setCoordinateInstanceInfo() method in
-                # util/UpdateSequenceDataStoreUtils.py for the definition of all values in coordinate seqTup
-                returnSeqList.append((str(seqTup[0]).upper(), str(i), str(seqTup[6]), str(seqTup[1])))
+                returnSeqList.append((str(seqTup[0]).upper(), str(i), str(str(seqTup[6]))))
             else:
                 returnSeqList.append((str(seqTup[0]).upper(), str(i)))
             #
         #
         return returnSeqList
 
     def __generateInputSeqInfoForPseudoMultiAlignFromAlignList(self, alignList):
@@ -1175,15 +1174,15 @@
                 alignTup[authIdx][7] = authConflict[1]
                 alignTup[otherIdx][6] = otherConflict[0]
                 alignTup[otherIdx][7] = otherConflict[1]
             #
         #
         return numConflict, missingAuthSeqList
 
-    def __annotateConflictingComments(self, authIdx, refIdx, beg_pos, end_pos, writeConflictFlag):
+    def __annotateConflictingComments(self, authIdx, refIdx, beg_pos, end_pos):
         """Add default 'expression tag annotation comments' for leading or trailing gap residues, and
         comments for any conflicts which can be attributed to a residue modification.
         """
         first_fragment = False
         if beg_pos < 10:
             first_fragment = True
         #
@@ -1233,22 +1232,14 @@
             elif self._seqAlignList[i][authIdx][1] == self._gapSymbol:
                 comment = "deletion"
             else:
                 comment = self.__annotateRealConflict(self._seqAlignList[i][authIdx], self._seqAlignList[i][refIdx])
             #
             finalComment = self.__consolidateConflict(comment, self._seqAlignList[i][authIdx][5], self._seqAlignList[i][refIdx][5])
             self._seqAlignList[i][authIdx][5] = finalComment
-            if writeConflictFlag:
-                _commentType, commentValue = self._decodeComment(finalComment)
-                if commentValue in self.__conflictMap:
-                    self.__conflictMap[commentValue] += 1
-                else:
-                    self.__conflictMap[commentValue] = 1
-                #
-            #
         #
 
     def __annotateRealConflict(self, authAlignTuple, refAlignTuple):
         """Annotate "modified residue", "engineered mutation", and "conflict" """
         comment = ""
         if authAlignTuple[1] == refAlignTuple[1]:
             comment = ""
@@ -1306,17 +1297,16 @@
         aCompId = authCompId.upper().strip()
         if (aCompId in self.__parentCompIdMap) and (self.__parentCompIdMap[aCompId] == rCompId):
             return True
         #
         if aCompId in self.__standardList:
             return False
         #
-        crpi = ChemRefPathInfo(siteId=self._siteId, verbose=self._verbose, log=self._lfh)
-        ccPath = crpi.getFilePath(aCompId, "CC")
-        if ccPath and os.access(ccPath, os.F_OK):
+        ccPath = os.path.join(self.__ccTopPath, aCompId[0], aCompId, aCompId + ".cif")
+        if os.access(ccPath, os.F_OK):
             cifObj = mmCIFUtil(filePath=ccPath)
             parentCompId = cifObj.GetSingleValue("chem_comp", "mon_nstd_parent_comp_id")
             if parentCompId:
                 pCompId = parentCompId.upper().strip()
                 self.__parentCompIdMap[aCompId] = pCompId
                 if pCompId == rCompId:
                     return True
@@ -1504,14 +1494,15 @@
         #
         polymerTypeCode = "AA"
         if "POLYMER_TYPE" in featureD:
             polymerTypeCode = featureD["POLYMER_TYPE"]
         #
         editList = []
         for alignPos in gapList:
+            self._lfh.flush()
             xyzRecord = self._seqAlignList[alignPos][chainIdx]
             #
             currId = self._getResLabelId(
                 seqType=seqType,
                 seqInstId=seqInstId,
                 seqAltId=seqAltId,
                 seqVersion=seqVersion,
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/DataImporter.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/DataImporter.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/SequenceDataAssembleExample.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/SequenceDataAssembleExample.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/SequenceDataAssembleTests.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/SequenceDataAssembleTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/SequenceDataAssemble_v2.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/SequenceDataAssemble_v2.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,17 +11,14 @@
 #   3-Dec-2013 jdw  skip PDB format data file production
 #  19-Jan-2014 jdw  add 'HOST_ORG_CELL_LINE'
 #  19-Jan-2014 jdw  standardize path polymer link report using getPolyLinkReportFilePath()
 #  01-Feb-2015 jdw  add host org variant
 #  24-Aug-2017  zf  remove __doAssembleFromArchive() & __doAssembleFromModel(), move all file copy operations into DataImporter.py
 #                   modify __calcPolymerLinkages(), also modify backend C++ code to speed up file process
 #                   modify __doReferenceSearch() to use previous blast results if existing & applicable
-#  01-Oct-2022  zf  modified __getAuthDefinedRefD() method to include author provided "seq_align_begin", "seq_align_end", "db_align_end",
-#                   "db_align_beg", & "db_seq_one_letter_code" information
-#                   improved process to handle the author-provided reference IDs and new entity summary page
 ##
 """
 Assemble sequence and other required data to start/restart the sequence editor tool.
 
 """
 __docformat__ = "restructuredtext en"
 __author__ = "John Westbrook"
@@ -49,15 +46,15 @@
 from wwpdb.apps.seqmodule.align.AlignmentTools import AlignmentTools
 from wwpdb.apps.seqmodule.io.AlignmentDataStore import AlignmentDataStore
 from wwpdb.apps.seqmodule.io.SequenceDataExport_v2 import SequenceDataExport
 from wwpdb.apps.seqmodule.link.PolymerLinkageDepict import PolymerLinkageDepict
 from wwpdb.apps.seqmodule.update.UpdatePolymerEntitySourceDetails import UpdatePolymerEntitySourceDetails
 from wwpdb.apps.seqmodule.util.LocalBlastSearchUtils import LocalBlastSearchUtils
 from wwpdb.apps.seqmodule.util.SeqReferenceSearchUtils import SeqAnnotationSearchUtils
-# from wwpdb.apps.seqmodule.util.SeqReferenceSearchUtils import SeqReferenceSearchUtils
+from wwpdb.apps.seqmodule.util.SeqReferenceSearchUtils import SeqReferenceSearchUtils
 from wwpdb.apps.seqmodule.util.SequenceLabel import SequenceLabel
 from wwpdb.apps.seqmodule.util.UpdateSequenceDataStoreUtils import UpdateSequenceDataStoreUtils
 from wwpdb.apps.seqmodule.util.MultiProcLimit import MultiProcLimit
 from wwpdb.utils.config.ConfigInfo import ConfigInfo
 from rcsb.utils.multiproc.MultiProcUtil import MultiProcUtil
 from wwpdb.io.locator.PathInfo import PathInfo
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
@@ -380,49 +377,36 @@
                 continue
             #
             entity_id = key.strip()
             codeList = []
             refList = []
             for refD in valD["ref_list"]:
                 data = []
-                for item in ("db_name", "db_accession", "db_code", "seq_align_begin", "seq_align_end", "db_align_end",
-                             "db_align_beg", "db_seq_one_letter_code"):
-                    if (item in refD) and refD[item]:
-                        data.append(refD[item].strip().upper())
-                    else:
-                        data.append("")
+                for item in ("db_accession", "db_code"):
+                    if (item not in refD) or (not refD[item]):
+                        continue
                     #
+                    data.append(refD[item].strip().upper())
                 #
-                if (data[0] == "") or ((data[1] == "") and (data[2] == "")):
+                if not data:
                     continue
                 #
-                for idx in (1, 2):
-                    val = data[idx]
-                    if val and (val not in codeList):
+                for val in data:
+                    if val not in codeList:
                         codeList.append(val)
                     #
                 #
-                refList.append(data)
-            #
-            if len(refList) == 0:
-                continue
-            elif len(refList) > 1:
-                # Chimera case: check the "seq_align_begin", "seq_align_end" values
-                missingSeqAlignRange = False
-                for refData in refList:
-                    if (refData[3] == "") or (refData[4] == ""):
-                        missingSeqAlignRange = True
-                        break
-                    #
-                #
-                if missingSeqAlignRange:
-                    continue
+                if ("db_name" in refD) and refD["db_name"]:
+                    data.insert(0, refD["db_name"].strip().upper())
+                    refList.append(data)
                 #
             #
-            self.__authDefinedRefD[entity_id] = (codeList, refList)
+            if len(codeList) > 0:
+                self.__authDefinedRefD[entity_id] = (codeList, refList)
+            #
         #
 
     def __renderPolymerLinkages(self, polymerLinkDistList, polyLinkHtmlPath):
         """Create HTML table rendering of the input polymer linkage distance list.
 
         HTML output is written to the "polyLinkHtmlPath":
 
@@ -629,27 +613,14 @@
                     or ((polyTypeCode in ["AA"]) and (seqLen < self.__minSearchSequenceLengthAA))
                 )
                 #
                 NA_flag = False
                 if polyTypeCode == "DNA":
                     NA_flag = True
                 #
-                if skip and (polyTypeCode == "AA"):
-                    oneLetterCodeSeq = str(eD["SEQ_ENTITY_1_CAN"]).strip().upper()
-                    countALA = 0
-                    for oneLetterCode in oneLetterCodeSeq:
-                        if oneLetterCode == "A":
-                            countALA += 1
-                        #
-                    #
-                    # Stop autoProcess for poly-ALA Seq per ticket# DAOTHER-8256
-                    if (10 * countALA) > (9 * seqLen):
-                        self.__autoProcessFlag = False
-                    #
-                #
                 if self._verbose:
                     self._lfh.write("+SequenceDataAssemble.__doReferenceSearch() search for entity id %s type %s length %d skip status %r\n" % (eId, polyTypeCode, seqLen, skip))
                     self._lfh.flush()
                 #
                 if sId in self.__authDefinedRefD:
                     entityTupList.append((sId, eD, self.__authDefinedRefD[sId], skip, NA_flag))
                 else:
@@ -675,19 +646,19 @@
             naList = []
             if self.__reRunBlastSearchFlag:
                 blastList = entityTupList
                 self.__autoProcessFlag = False
             else:
                 for entityTup in entityTupList:
                     hasOwnRef = False
-                    if (entityTup[0] in ownRefD) and ("auto_match_status" in ownRefD[entityTup[0]]) and ownRefD[entityTup[0]]["auto_match_status"]:
+                    if entityTup[0] in ownRefD:
                         hasOwnRef = True
                     #
                     hasSameSeqRef = False
-                    if (entityTup[0] in otherRefD) and ("auto_match_status" in otherRefD[entityTup[0]]) and otherRefD[entityTup[0]]["auto_match_status"]:
+                    if entityTup[0] in otherRefD:
                         hasSameSeqRef = True
                     #
                     if hasOwnRef:
                         continue
                     elif hasSameSeqRef:
                         if self.__forceBlastSearchFlag and (not entityTup[3]):
                             blastList.append(entityTup)
@@ -699,27 +670,24 @@
                         skipList.append(entityTup)
                     #
                     if (len(entityTup[2]) > 0) or (not entityTup[3]):
                         blastList.append(entityTup)
                         if not entityTup[3]:
                             if entityTup[4]:
                                 naList.append(entityTup[0])
-#                           else:
-#                               self.__autoProcessFlag = False
+                            else:
+                                self.__autoProcessFlag = False
                             #
                         #
                     #
                 #
             #
             refD = {}
             if blastList:
-                autoMatchStatus, refD = self.__runSeqBlastSearch(blastList)
-                if (not autoMatchStatus) or (not refD):
-                    self.__autoProcessFlag = False
-                #
+                refD = self.__runSeqBlastSearch(blastList)
             #
             if refD:
                 for k, _v in refD.items():
                     if k in naList:
                         self.__autoProcessFlag = False
                     #
                 #
@@ -807,27 +775,27 @@
     #             self._lfh.write("+SequenceDataAssemble.__runSeqAllSearches() - failing \n")
     #             traceback.print_exc(file=self._lfh)
     #         #
     #     #
     #     return {}, {}, {}
 
     # EP: Believe unused
-#   def runMultiReferenceSearches(self, dataList, procName, optionsD, workingDir):  # pylint: disable=unused-argument
-#       """Multiple reference sequence search processing API"""
-#       ncbilock = optionsD.get("ncbilock", None)
-#       rList = []
-#       for tupL in dataList:
-#           seqSearchUtil = SeqReferenceSearchUtils(
-#               siteId=self.__siteId, sessionPath=self.__sessionPath, pathInfo=self.__pI, verbose=self._verbose, log=self._lfh, ncbilock=ncbilock
-#           )
-#           eRefD, selfRefD, sameSeqRefD = seqSearchUtil.run(self.__dataSetId, tupL[1], tupL[2], self.__doRefSearchFlag, self.__forceBlastSearchFlag)
-#           rList.append((tupL[0], eRefD, selfRefD, sameSeqRefD))
-#           #
-#       #
-#       return rList, rList, []
+    def runMultiReferenceSearches(self, dataList, procName, optionsD, workingDir):  # pylint: disable=unused-argument
+        """Multiple reference sequence search processing API"""
+        ncbilock = optionsD.get("ncbilock", None)
+        rList = []
+        for tupL in dataList:
+            seqSearchUtil = SeqReferenceSearchUtils(
+                siteId=self.__siteId, sessionPath=self.__sessionPath, pathInfo=self.__pI, verbose=self._verbose, log=self._lfh, ncbilock=ncbilock
+            )
+            eRefD, selfRefD, sameSeqRefD = seqSearchUtil.run(self.__dataSetId, tupL[1], tupL[2], self.__doRefSearchFlag, self.__forceBlastSearchFlag)
+            rList.append((tupL[0], eRefD, selfRefD, sameSeqRefD))
+            #
+        #
+        return rList, rList, []
 
     def __runSameSeqAnnotationSearch(self, entityTupList):
         """Search same sequence annotation information from processed entries"""
         try:
             startTime = time.time()
             #
             if self.__cI.get("USE_COMPUTE_CLUSTER"):
@@ -869,15 +837,15 @@
         return {}, {}
 
     def runMultiSameSeqAnnotationSearches(self, dataList, procName, optionsD, workingDir):  # pylint: disable=unused-argument
         """Multiple same sequence annotation search processing API"""
         rList = []
         for tupL in dataList:
             seqSearchUtil = SeqAnnotationSearchUtils(siteId=self.__siteId, sessionPath=self.__sessionPath, pathInfo=self.__pI, verbose=self._verbose, log=self._lfh)
-            selfRefD, sameSeqRefD = seqSearchUtil.getSameSeqRefInfo(self.__dataSetId, tupL[1], tupL[2])
+            selfRefD, sameSeqRefD = seqSearchUtil.getSameSeqRefInfo(self.__dataSetId, tupL[1])
             rList.append((tupL[0], selfRefD, sameSeqRefD))
         #
         return rList, rList, []
 
     def __runSeqBlastSearch(self, entityTupList):
         """Perform blast reference sequence search"""
         try:
@@ -904,45 +872,36 @@
                 rate = 1
             #
             mpl = MultiProcLimit(rate)
             mpu.setOptions({"ncbilock": mpl})
             #
             _ok, _failList, retLists, _diagList = mpu.runMulti(dataList=entityTupList, numProc=numProc, numResults=1)
             #
-            autoMatchStatus = True
             refD = {}
             for tupList in retLists:
                 for tup in tupList:
                     if tup[1]:
                         refD[tup[0]] = tup[1]
-                        if (len(tup) != 3) or (not tup[2]):
-                            autoMatchStatus = False
-                        #
-                    else:
-                        autoMatchStatus = False
                     #
                 #
             #
-            if not refD:
-                autoMatchStatus = False
-            #
             if self._verbose:
                 endTime = time.time()
                 self._lfh.write(
                     "+SequenceDataAssemble.__runSeqBlastSearch()  completed at %s (%.2f seconds)\n" % (time.strftime("%Y %m %d %H:%M:%S", time.localtime()), endTime - startTime)
                 )
             #
-            return autoMatchStatus, refD
+            return refD
         except:  # noqa: E722 pylint: disable=bare-except
             if self._verbose:
                 self._lfh.write("+SequenceDataAssemble.__runSeqBlastSearch() - failing \n")
                 traceback.print_exc(file=self._lfh)
             #
         #
-        return False, {}
+        return {}
 
     def runMultiBlastReferenceSearches(self, dataList, procName, optionsD, workingDir):  # pylint: disable=unused-argument
         """Multiple blast reference sequence search processing API"""
         ncbilock = optionsD.get("ncbilock", None)
         rList = []
         for tupL in dataList:
             seqSearchUtil = LocalBlastSearchUtils(
@@ -950,16 +909,16 @@
                 sessionPath=self.__sessionPath,
                 pathInfo=self.__pI,
                 doRefSearchFlag=self.__doRefSearchFlag,
                 verbose=self._verbose,
                 log=self._lfh,
                 ncbilock=ncbilock,
             )
-            autoMatchStatus, eRefD = seqSearchUtil.searchSeqReference(dataSetId=self.__dataSetId, entityD=tupL[1], authRefList=tupL[2])
-            rList.append((tupL[0], eRefD, autoMatchStatus))
+            eRefD = seqSearchUtil.searchSeqReference(dataSetId=self.__dataSetId, entityD=tupL[1], authRefList=tupL[2])
+            rList.append((tupL[0], eRefD))
             #
         #
         return rList, rList, []
 
     def __createSeqMatchFileAndMisMatchPickleFile(
         self, sortedEntityIdList, entityD, ownRefD, eSSRefD, prevEntityIdList, prevMisMatchList, prevNotFoundMatchList, seqSimilarityInfoList
     ):
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/SequenceDataPrepTests.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/SequenceDataPrepTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/SummaryViewDepiction.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/SummaryViewDepiction.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/SummaryViewTests.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/SummaryViewTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/control/SummaryView_v2.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/SequenceDataExport_v2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,732 +1,602 @@
 ##
-# File:    SummaryView.py
-# Date:    19-Jan-2010
+# File:  SequenceDataExport_v2.py
+# Date:  14-Feb-2010
+#
 # Updates:
-# 09-Feb-2010  jdw Adopt SequenceFeature() to access to feature dictionaries.
-# 12-Feb-2010  jdw Move example data loader to the SequenceDataImportExample class.
-# 14-Feb-2010  jdw Add statistics updater after primary sequence data load.
-# 20-Apr-2010  jdw Ported to module seqmodule
-# 27-Apr-2010  jdw Add row-level data dictionary to the summary data object.
-# 02-May-2010  jdw Add SequenceSelection()
-# 09-Aug-2010  rps __loadSummary() --> Highest numbered version of coordinate sequence to be selected by default in "SELECT" column of UI
-# 08-Jan-2013  jdw Select higher version of author sequence in reload operations
-# 03-Mar-2013  jdw Refactor -
-# 05-Mar-2013  jdw Move default sequence selection from SequenceSelection()
-#                  Add default self-reference selections
-#                  Implement stored sorting order for reference sequeneces --
-#                  Limit reference sequence to maxRefAlign --
-# 12-Mar-2013  jdw adjust the assembly of author sequence details -
-# 13-Apr-2013  jdw change self reference identifiers
-# 15-Nov-2013  jdw major overhaul to support expanded author content display and entity review
-# 12-Dec-2013  jdw make default alignment selections.
-# 19-Dec-2013  jdw select any added or edited reference sequence by default
-# 15-May-2014  jdw add status field for instance id with xyz sequence groups
-# 22-May-2014  jdw add method to provide entry details --
-# 30-Aug-2017  zf  change self.__reqObj.getSummaryAlignList & self.__reqObj.getSummarySelectList to use latest UI input values
-# 29-Jun-2021  zf  added self.__checkPolyAlaAssignment()
-# 19-Oct-2022  zf  added section for generation summary landing page
+#   20-Apr-2010 jdw Ported to module seqmodule.
+#   23-Apr-2010 jdw Added method for self-references.
+#   02-May-2010 jdw Add file path to constructor, move makeDefaultSelection() to SequenceSelection class.
+#                   Add handling of self-references...
+#  01-Mar-2013  jdw remove SiteInterface -
+#  08-Mar-2013  jdw adpot the standard file name conventions.
+#  08-Mar-2013  jdw add support use of sequence parts.
+#  07-Apr-2013  jdw add support for isoforms/filter self references from db references
+#  23-Apr-2013  jdw add separate category for export of modified residues
+#  05-May-2013  jdw filter gap residues from author/xyz mapping list
+#  20-Sep-2013  jdw fix filter for mapping from auth/xyz mapping
+#  14-Nov-2013  jdw add new entity details export
+#  18-Dec-2013  jdw adjust conflict array lengths after alignment --
+#  19-Jan-2014  jdw "HOST_ORG_CELL_LINE"
+#  27-Apr-2014  jdw working on fix to source detail export -
+#  28-Apr-2014  jdw verify that updateArchive=False is default --
+#                   Changes will always be applied to the first model in the session  --
+#
+# 19-May-2014   jdw refactor to better reuse new stored alignment data -
+# 22-May-2014   jdw add output conflict list
+#  3-Jun-2014   jdw fix self-reference issue
+# 16-Oct-2014   jdw add explicit flag for sequence heterogeneity
+# 22-Oct-2014   jdw add combination microheterogeneity/modified residue
+# 01-Feb-2015   jdw add host org variant
+# 01-Feb-2016   jdw change file handling for model merge -
+# 07-Sep-2017   zf  add __cifCatAnnoDbRef() to export annotator's editing db reference information
+# 31-Oct-2018   zf  split orignial SequenceDataExport into SequenceDataExport_v2 & AlignmentExport
 ##
 """
-Controlling class for the production of data for the summary sequence view.
+Export sequence and alignment details to production RCSB pipeline.
 
 """
 __docformat__ = "restructuredtext en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
-__version__ = "V0.08"
-
-try:
-    import cPickle as pickle
-except ImportError:
-    import pickle as pickle
-#
+__version__ = "V0.07"
 
 import os
 import sys
 import traceback
 
-from wwpdb.apps.seqmodule.io.AlignmentDataStore import AlignmentDataStore
-from wwpdb.apps.seqmodule.io.FetchSeqInfoUtils import FetchSeqInfoUtils
-from wwpdb.apps.seqmodule.io.SequenceDataStore import SequenceDataStore
-from wwpdb.apps.seqmodule.util.SequenceLabel import SequenceLabel, SequenceFeature
-from wwpdb.apps.seqmodule.util.SequenceFeatureDepict import SequenceFeatureDepict
+from mmcif.api.DataCategory import DataCategory
+from mmcif.api.PdbxContainers import DataContainer
+from mmcif.io.PdbxWriter import PdbxWriter
 
-from wwpdb.apps.seqmodule.util.SequenceAssign import SequenceAssignDepositor
-from wwpdb.apps.seqmodule.update.UpdatePolymerEntitySourceDetails import UpdatePolymerEntitySourceDetails
+#
+from wwpdb.apps.seqmodule.align.AlignmentExport import AlignmentExport
+from wwpdb.apps.seqmodule.io.SequenceDataStore import SequenceDataStore
+from wwpdb.apps.seqmodule.util.SequenceReferenceData import SequenceReferenceData
+from wwpdb.apps.seqmodule.util.SequenceLabel import SequenceLabel
+from wwpdb.apps.seqmodule.util.Autodict import Autodict
 
+#
 from wwpdb.io.misc.FormatOut import FormatOut
+from wwpdb.io.locator.PathInfo import PathInfo
+from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
 
 
-class SummaryView(object):
-    """Controlling class for the production of data for the summary sequence view.
-
-    Supported operations:
-
-     load             = load summary from current sequence data store using default sequence selection.
-     reload           = reload summary using current sequence data and current user selections.
+class SequenceDataExport(object):
+    """
+    This class encapsulates all of the data export operations
+    of sequence and other data to the RCSB/WF data pipeline.
 
+    Storage model - exported data is loaded from the sequence data store
+                    where it is managed by the SequenceDataStore() class.
     """
 
-    def __init__(self, reqObj=None, maxRefAlign=100, verbose=False, log=sys.stderr):
+    def __init__(self, reqObj=None, exportList=None, verbose=False, log=sys.stderr):
         self.__verbose = verbose
-        self.__debug = False
         self.__reqObj = reqObj
         self.__lfh = log
-        self.__maxRefAlign = maxRefAlign
-        #
-        # placeholders for sequence identifiers picked on the summary page as selected and/or to be aligned.
-        self.__summarySeqAlignList = []
-        self.__summarySeqSelectList = ""
-        #
-        self.__natureSourceTaxIds = {}
-        self.__partRangeErrorMsg = ""
-        self.__sds = None
+        if exportList is None:
+            exportList = []
+        self.__debug = False
+        self.__sessionObj = None
+        self.__sessionPath = "."
         #
-        self.__summaryPageInfoMap = {}
+        # This is the setting for all selected sequences to be exported -
         #
+        self.__summarySeqSelectList = exportList
+        self.__selfRefList = []
         self.__setup()
 
     def __setup(self):
         try:
             self.__sessionObj = self.__reqObj.getSessionObj()
-            self.__sessionPath = self.__sessionObj.getPath()  # pylint: disable=unused-private-member
+            self.__sessionPath = self.__sessionObj.getPath()
+
+            self.__siteId = self.__reqObj.getValue("WWPDB_SITE_ID")
+            self.__identifier = self.__reqObj.getValue("identifier")
+
+            self.__srd = SequenceReferenceData(verbose=self.__verbose, log=self.__lfh)
+
+            self.__pI = PathInfo(siteId=self.__siteId, sessionPath=self.__sessionPath, verbose=self.__verbose, log=self.__lfh)
+            self.__exportFilePathSession = self.__pI.getSequenceAssignmentFilePath(self.__identifier, fileSource="session", versionId="next")
+            if self.__verbose:
+                self.__lfh.write("+SequenceDataExport.__setup() session assignment file path %s\n" % self.__exportFilePathSession)
+            #
             self.__sds = SequenceDataStore(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
-            self.__sdu = UpdatePolymerEntitySourceDetails(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
+            if self.__debug:
+                self.__sds.dump(self.__lfh)
             #
-            # Selections coming from the the web request --
+            if not self.__summarySeqSelectList:
+                self.__summarySeqSelectList = self.__sds.getSelectedIds()
             #
-            # self.__summarySeqAlignList = self.__reqObj.getSummaryAlignList(usingRevAllAlignIds=False)
-            # self.__summarySeqSelectList = self.__reqObj.getSummarySelectList(usingRevSlectIds=False)
-            self.__summarySeqAlignList = str(self.__reqObj.getValue("allalignids")).split(",")
-            self.__summarySeqSelectList = str(self.__reqObj.getValue("selectids")).split(",")
-            self.__updateSelectList()
+            self.__selfReferenceEntityList = []
+            self.__trueSelfReferenceEntityList = []
+            self.__annoRefDbL = []
+            self.__annoSeqAuthRefMap = {}
+            self.__I = self.__makeExportIndex(self.__summarySeqSelectList)
+            self.__makeSelfReferenceIndex(self.__summarySeqSelectList)
             if self.__verbose:
-                self.__lfh.write("+SummaryView.__setup() request input align list  %r\n" % (self.__summarySeqAlignList))
-                self.__lfh.write("+SummaryView._setup()  request input select list %r\n" % (self.__summarySeqSelectList))
+                self.__lfh.write("+SequenceDataExport.__setup() incoming selected id list %r\n" % (self.__summarySeqSelectList))
+                self.__lfh.write("+SequenceDataExport.__setup() self reference list %r\n" % self.__selfReferenceEntityList)
             #
-            # Reset any newly loaded reference sequence id as it is included above --
-            self.__reqObj.setNewRefId("")
-        except Exception as _e:  # noqa: F841
+        except:  # noqa: E722 pylint: disable=bare-except
+            self.__lfh.write("+SequenceDataExport.__setup() failed for entry id %s\n" % (self.__identifier))
+            traceback.print_exc(file=self.__lfh)
+        #
+
+    def exportAssignments(self):
+        """Export assign file and associated updated model data file --"""
+        numConflicts = 0
+        conflictList = []
+        try:
+            ok, numConflicts, conflictList, warningMsg = self.__exportSeqMapping()
+            return ok, numConflicts, conflictList, warningMsg
+        except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
-                self.__lfh.write("+SummaryView.__setup() sessionId %s failed\n" % (self.__sessionObj.getId()))
+                self.__lfh.write("+SequenceDataExport.exportAssignments() failed for entry id %s\n" % (self.__identifier))
                 traceback.print_exc(file=self.__lfh)
             #
         #
+        return False, numConflicts, conflictList, ""
 
-    def __updateSelectList(self):
-        """ """
-        updatedids = str(self.__reqObj.getValue("updatedids"))
-        if not updatedids:
-            return
-        #
-        updatedList = updatedids.split(",")
-        #
-        entityId = str(self.__reqObj.getValue("activegroupid"))
-        chainIdList = self.__sds.getGroup(entityId)
-        for seqId in self.__summarySeqSelectList:
-            tL = str(seqId).strip().split("_")
-            if len(tL) < 3:
-                continue
+    def getAllEntityIdList(self):
+        """Interface to get all entity Id list from SequenceDataStore"""
+        return self.__sds.getGroupIds()
+
+    def applyAssignmentsToModel(self):
+        """Create an updated model file in the current session --"""
+        try:
+            #  ----------------
+            # Changes will always be applied to the earliest model in the current session  --
             #
-            elif (tL[0] in ("selfref", "auth", "ref")) and (tL[1] == entityId):
-                continue
-            elif (tL[0] == "xyz") and (tL[1] in chainIdList):
-                continue
+            for v in ["1", "2", "3", "4"]:
+                pdbxPath = self.__pI.getModelPdbxFilePath(self.__identifier, fileSource="session", versionId=v)
+                self.__lfh.write("\n+SequenceDataExport.applyAssignmentsToModel() verifying starting model target path %s\n" % pdbxPath)
+                if os.access(pdbxPath, os.R_OK):
+                    break
+                #
+            #
+            pdbxPathNext = self.__pI.getModelPdbxFilePath(self.__identifier, fileSource="session", versionId="next")
+            logPath = os.path.join(self.__sessionPath, "annot-seqmod-merge.log")
+            if os.access(logPath, os.R_OK):
+                os.remove(logPath)
+            #
+            self.__lfh.write("\n+SequenceDataExport.applyAssignmentsToModel() starting model target path %s\n" % pdbxPath)
+            self.__lfh.write("+SequenceDataExport.applyAssignmentsToModel() model output path %s\n" % pdbxPathNext)
+            self.__lfh.write("+SequenceDataExport.applyAssignmentsToModel() assignment file path %s\n" % self.__exportFilePathSession)
+
+            dp = RcsbDpUtility(tmpPath=self.__sessionPath, siteId=self.__siteId, verbose=self.__verbose, log=self.__lfh)
+            dp.setDebugMode()
+            dp.imp(pdbxPath)
+            dp.addInput(name="seqmod_assign_file_path", value=self.__exportFilePathSession, type="file")
+            dp.op("annot-merge-sequence-data")
+            dp.exp(pdbxPathNext)
+            dp.expLog(logPath)
+            # dp.cleanup()
+            if not os.access(pdbxPathNext, os.R_OK):
+                return False
             #
-            updatedList.append(seqId)
+        except:  # noqa: E722 pylint: disable=bare-except
+            if self.__verbose:
+                self.__lfh.write("+SequenceDataExport.applyAssignmentsToModel() model update failed for assignment file  %s\n" % self.__exportFilePathSession)
+                traceback.print_exc(file=self.__lfh)
+            return False
         #
-        self.__summarySeqSelectList = updatedList
+        return True
+
+    def printIt(self):
+        fOut = FormatOut()
+        fOut.autoFormat("Summary Selection List", self.__summarySeqSelectList, 3, 3)
+        fOut.autoFormat("Self Reference List", self.__selfReferenceEntityList, 3, 3)
+        fOut.autoFormat("Selection Index", self.__I, 3, 3)
+        fOut.writeStream(self.__lfh)
+        fOut.clear()
+
+    def __makeExportIndex(self, selectIdList):
+        """Return an index dictionary for the input sequence id list -
+
+        The sequence labels  have the format:
 
-    def __finish(self):
+        seqType + "_" + seqInstId + "_" + seqPartId + "_" + seqAltId  + "_" + seqVersion
+
+        or, for the special case of a self reference --
+
+        "selfref"  "_"  entityId  "_"  partId
+        """
+        if self.__verbose:
+            self.__lfh.write("+SequenceDataExport.__makeExportIndex() selected sequence id list %r\n" % selectIdList)
+        #
+        I = Autodict()  # noqa: E741
         try:
-            # Persist the current summary selection list --
-            self.__reqObj.setSummarySelectList(self.__summarySeqSelectList)
-            self.__reqObj.setSummaryAlignList(self.__summarySeqAlignList)
-            self.__sds.setSelectedIds(idList=self.__summarySeqSelectList)
-            self.__sds.serialize()
-        except Exception as _e:  # noqa: F841
+            for seqId in selectIdList:
+                tup = seqId.strip().split("_")
+                # Skip self reference ids
+                if str(tup[0]).strip() == "selfref":
+                    self.__selfRefList.append(seqId)
+                    continue
+                #
+                I[tup[0]][tup[1]][int(tup[2])] = (int(tup[3]), int(tup[4]))
+            #
+        except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
-                self.__lfh.write("+SummaryView.__finish() sessionId %s failed\n" % (self.__sessionObj.getId()))
+                self.__lfh.write("+SequenceDataExport.__makeExportIndex() failed \n")
                 traceback.print_exc(file=self.__lfh)
+            #
+        #
+        return I
 
-    def getEntryDetails(self, kyList=None):
-        if kyList is None:
-            kyList = ["STRUCT_TITLE", "CITATION_TITLE", "PDB_ID"]
-
-        eD = {}
-        for ky in kyList:
-            eD[ky] = self.__sds.getEntryDetail(detailKey=ky)
-        #
-        return eD
-
-    def loadSummary(self, operation="load"):
-        """Create the data structure to populate the HTML pages containing alignment summary --
-
-        Options for operation:
-        + load   - Performs a default selection of the best matching reference sequences then
-                   creates the summary data structure.
-        + reload - reloads current data from the sequence and alignment data stores.
-        """
-        if self.__verbose:
-            self.__lfh.write("+SummaryView.loadSummary() operation %s : sessionId %s\n" % (operation, self.__sessionObj.getId()))
-            self.__lfh.write("+SummaryView.loadSummary() request input align list  %r\n" % (self.__summarySeqAlignList))
-            self.__lfh.write("+SummaryView.loadSummary() request input select list %r\n" % (self.__summarySeqSelectList))
-        if operation == "load":
-            # Using coming from persisted data only here
-            #  -- ignore user selections from web context as these may not exist or may need to be overridden --
-            self.__summarySeqSelectList = self.__sds.getSelectedIds()
-        #
-        self.__summarySeqAlignList = self.__summarySeqSelectList
-
-        self.__sdu.updateAuthEntityDetails(selectIdList=self.__summarySeqSelectList)
-        self.__sds = SequenceDataStore(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
-        return self.__loadSummary(op=operation)
+    def __makeSelfReferenceIndex(self, selectIdList):
+        """Return the list self referenced entities for the input sequence id list -
 
-    def getGroupIdList(self):
-        return self.__sds.getGroupIds()
+        The sequence labels  have the format:
 
-    def getSummaryPageObj(self):
-        return self.__summaryPageInfoMap
+        seqType + "_" + seqInstId + "_" + seqPartId + "_" + seqAltId  + "_" + seqVersion
 
-    def __loadSummary(self, op="load"):
-        """Assemble the data for sequence summary view using current contents of the session sequence data store.
+        or, for the special case of a self reference --
 
-        Returns:  summaryDataObj [<entity/groupId>]  ['auth'|'xyz'] ->  {data dict}
-                                                     ['ref']        -> [(partId,{data dict}),(partId,{data dict}),...]
-                               {data dict}  with keys
-
-                               dT['ROW_IDS']       =rowIdList
-                               dT['ROW_STATUS']    =rowStatusList
-                               dT['ROW_DATA_DICT'] =rowDataDictList
-                               dT['SELF_REFERENCE_FLAG']=Boolean
+        "selfref"  "_"  entityId  "_"  partId
         """
-        #
         if self.__verbose:
-            self.__lfh.write("+SummaryView.__loadSummary() with sessionId %s\n" % self.__sessionObj.getId())
+            self.__lfh.write("+SequenceDataExport.__makeSelfReferenceIndex() selected sequence id list %r\n" % selectIdList)
+        #
+        try:
+            for seqId in selectIdList:
+                tup = seqId.strip().split("_")
+                if str(tup[0]).strip() == "selfref":
+                    if self.__verbose:
+                        self.__lfh.write("+SequenceDataExport.__makeSelfReferenceIndex() - assigning reference for sequence entity %s part %s (%s)\n" % (tup[1], tup[2], tup[0]))
+                    #
+                    seqId = str(tup[1]).strip()
+                    partId = str(tup[2]).strip()
+                    self.__selfReferenceEntityList.append((seqId, partId))
+                    foundAnnInputRefInfo = False
+                    if (seqId in self.__I["auth"]) and (int(partId) in self.__I["auth"][seqId]):
+                        altId = self.__I["auth"][seqId][int(partId)][0]
+                        verId = self.__I["auth"][seqId][int(partId)][1]
+                        seqAuthFD = self.__sds.getFeature(seqId=seqId, seqType="auth", partId=int(partId), altId=altId, version=verId)
+                        row = []
+                        row.append(len(self.__annoRefDbL) + 1)
+                        row.append(seqId)
+                        for item in ("ANNO_EDIT_DB_NAME", "ANNO_EDIT_DB_CODE", "ANNO_EDIT_DB_ACCESSION", "ANNO_EDIT_DB_ALIGN_BEGIN", "ANNO_EDIT_DB_ALIGN_END"):
+                            if (item in seqAuthFD) and seqAuthFD[item]:
+                                row.append(seqAuthFD[item])
+                            else:
+                                break
+                            #
+                        #
+                        if len(row) == 7:
+                            seqAuthRefMap = []
+                            if (seqId in self.__annoSeqAuthRefMap) and self.__annoSeqAuthRefMap[seqId]:
+                                seqAuthRefMap = self.__annoSeqAuthRefMap[seqId]
+                            else:
+                                seqAuthIdx = self.__sds.getSequence(seqId=seqId, seqType="auth", partId=int(partId), altId=altId, version=verId)
+                                idx = 1
+                                for seqAuth in seqAuthIdx:
+                                    seqAuthRefMap.append([".", seqId, seqAuth[0], str(idx), seqId, ".", ".", "."])
+                                    idx += 1
+                                #
+                            #
+                            if seqAuthRefMap:
+                                authFObj = self.__sds.getFeatureObj(seqId, "auth", partId=int(partId), altId=altId, version=verId)
+                                _authPartId, authSeqBeg, authSeqEnd, _authSeqPartType = authFObj.getAuthPartDetails()
+                                partBeg = int(authSeqBeg)
+                                partEnd = int(authSeqEnd)
+                                foundMap = False
+                                startNum = int(row[5])
+                                for seqAuth in seqAuthRefMap:
+                                    idx = int(seqAuth[3])
+                                    if (idx >= partBeg) and (idx <= partEnd):
+                                        if idx > partBeg:
+                                            startNum += 1
+                                        #
+                                        seqAuth[5] = seqAuth[2]
+                                        seqAuth[6] = str(startNum)
+                                        seqAuth[7] = str(partId)
+                                        foundMap = True
+                                    #
+                                #
+                                if foundMap:
+                                    row.append(partId)
+                                    self.__annoRefDbL.append(row)
+                                    foundAnnInputRefInfo = True
+                                    self.__annoSeqAuthRefMap[seqId] = seqAuthRefMap
+                                #
+                            #
+                        #
+                    #
+                    if not foundAnnInputRefInfo:
+                        self.__trueSelfReferenceEntityList.append((seqId, partId))
+                    #
+                #
+            #
+        except:  # noqa: E722 pylint: disable=bare-except
+            if self.__verbose:
+                self.__lfh.write("+SequenceDataExport.__makeSelfReferenceIndex() failed \n")
+                traceback.print_exc(file=self.__lfh)
+            #
+        #
 
+    def __exportSeqMapping(self):
+        """Export worker function -"""
         #
-        summaryDataObj = {}
+        # Get entry ids
+        depDataSetId = self.__sds.getEntryDetail("DEPOSITION_DATA_SET_ID")
+        # pdbId = self.__sds.getEntryDetail("PDB_ID")
         #
+        # Get the entity group list -
         gIdList = self.__sds.getGroupIds()
+        if len(gIdList) < 1:
+            if self.__verbose:
+                self.__lfh.write("+SequenceDataExport.__exportSeqMapping() for data set %s group list is empty\n" % depDataSetId)
+            #
         #
         if self.__verbose:
-            self.__lfh.write("+SummaryView.__loadSummary() group list is %r\n" % gIdList)
-            self.__lfh.write("+SummaryView.__loadSummary() starting selection list %r\n" % self.__summarySeqSelectList)
-            self.__lfh.write("+SummaryView.__loadSummary() starting alignment list %r\n" % self.__summarySeqAlignList)
+            self.__lfh.write("+SequenceDataExport.__exportSeqMapping() number of groups %d depDataSetId %s\n" % (len(gIdList), depDataSetId))
+        #
+
+        seqLabel = SequenceLabel()
+        refFeatureD = {}
+        rptRefL = []
+        rptXyzL = []
+        rptCommentL = []
+        rptCommentModL = []
+        rptDeleteL = []
+        allRefSeqIdxD = {}
+        numConflicts = 0
+        conflictList = []
+        warningMsg = ""
+        natureSourceTaxIds = {}
         #
         polyAlaCaseList = []
         for gId in gIdList:
             #
-            summaryDataObj[gId] = {}
-            #
-            dT, polyALA_assignment, authSummaryPageD, method, polyType, dbAccessionList = self.__buildAuthSection(groupId=gId, op=op)
-            if polyALA_assignment > 0:
-                polyAlaCaseList.append((gId, polyALA_assignment))
+            # Get seqIds in group -
             #
-            summaryDataObj[gId]["auth"] = dT
+            seqIdList = self.__sds.getGroup(gId)
+            if len(seqIdList) < 1:
+                if self.__verbose:
+                    self.__lfh.write("+SequenceDataExport.__exportSeqMapping() skipping entity group %s which has no instances\n" % (gId))
+                #
+                continue
             #
-            rL, withGapScoreList, withoutGapScoreList, hitDbInfoList, hitDbIdList, authTaxIdList = self.__buildReferenceSection(groupId=gId)
-            summaryDataObj[gId]["ref"] = rL
+            if self.__verbose:
+                self.__lfh.write("+SequenceDataExport.__exportSeqMapping() group %s sequence list %r\n" % (gId, seqIdList))
             #
-            summaryDataObj[gId]["xyz"] = self.__buildCoordinateSection(groupId=gId)
+            # Author sequence -
             #
-            decoration_start = ""
-            decoration_end = ""
-            if len(self.__sds.getGroup(gId)) == 0:
-                decoration_start = '<p style="text-decoration: line-through;">'
-                decoration_end = "</p>"
+            sourceInfo = ""
+            idAuthSeq = ""
+            first = True
+            if gId in self.__I["auth"]:
+                if self.__verbose:
+                    self.__lfh.write("+SequenceDataExport.__exportSeqMapping() entity group %s author sequence s list %r\n" % (gId, list(self.__I["auth"][gId].items())))
+                #
+                for partId, (altId, ver) in self.__I["auth"][gId].items():
+                    fD = self.__sds.getFeature(gId, seqType="auth", partId=partId, altId=altId, version=ver)
+                    if ("SOURCE_METHOD" in fD) and fD["SOURCE_METHOD"].upper() == "NAT":
+                        sourceInfo = "NAT"
+                        if ("SOURCE_TAXID" in fD) and fD["SOURCE_TAXID"]:
+                            if fD["SOURCE_TAXID"] in natureSourceTaxIds:
+                                if gId not in natureSourceTaxIds[fD["SOURCE_TAXID"]]:
+                                    natureSourceTaxIds[fD["SOURCE_TAXID"]].append(gId)
+                                #
+                            else:
+                                natureSourceTaxIds[fD["SOURCE_TAXID"]] = [gId]
+                            #
+                        #
+                    #
+                    seqLabel.set(seqType="auth", seqInstId=gId, seqPartId=partId, seqAltId=altId, seqVersion=ver)
+                    idAuthSeq = seqLabel.pack()
+                    if self.__verbose:
+                        self.__lfh.write("+SequenceDataExport.__exportSeqMapping() from entity group %s exporting author sequence %s\n" % (gId, idAuthSeq))
+                    #
+                    if first and ("POLYMER_TYPE" in fD) and (fD["POLYMER_TYPE"] == "AA"):
+                        seqAuth = self.__sds.getSequence(seqId=gId, seqType="auth", partId=partId, altId=altId, version=ver)
+                        polyALA_assignment = self.__checkPolyAlaAssignment(seqAuth)
+                        if polyALA_assignment > 0:
+                            polyAlaCaseList.append((gId, polyALA_assignment))
+                        #
+                    #
+                    first = False
+                #
             #
-            self.__summaryPageInfoMap[gId] = {}
-            if decoration_start:
-                self.__summaryPageInfoMap[gId]["entity_id"] = decoration_start + '<span class="width20px"> &nbsp;' + gId + '&nbsp; </span>' + decoration_end
-            else:
-                # self.__summaryPageInfoMap[gId]["entity_id"] = '<a id="page_' + gId + '" href="#" class="page_control"><span class="width20px"> &nbsp;' \
-                self.__summaryPageInfoMap[gId]["entity_id"] = '<a id="page_' + gId + '" href="#closecompleted" class="page_control"><span class="width20px">' \
-                    + ' &nbsp;' + gId + '&nbsp; </span></a>'
-            #
-            self.__summaryPageInfoMap[gId]["chain_ids"] = ",".join(self.__sds.getGroup(gId))
-            for tupL in (("mol_names", "ENTITY_DESCRIPTION"), ("source_names", "SOURCE_ORGANISM"), ("tax_ids", "SOURCE_TAXID")):
-                self.__summaryPageInfoMap[gId][tupL[0]] = decoration_start + self.__buildNameSourceSummaryPage(tupL[1], authSummaryPageD) + decoration_end
-            #
-            if (len(withGapScoreList) > 0) and (len(withoutGapScoreList) > 0):
-                self.__summaryPageInfoMap[gId]["identity_scores"] = decoration_start + '<span class="detailkey">w/ gaps: </span><span class="detailvalue">' + \
-                    ",".join(withGapScoreList) + '</span><br/><span class="detailkey">w/o gaps: </span><span class="detailvalue">' + \
-                    ",".join(withoutGapScoreList) + '</span>' + decoration_end
+            if not idAuthSeq:
+                # report missing author sequence
+                if self.__verbose:
+                    self.__lfh.write("+SequenceDataExport.__exportSeqMapping() missing author sequence from entity group %s\n" % gId)
+                #
+                continue
             #
-            if len(hitDbInfoList) > 0:
-                self.__summaryPageInfoMap[gId]["ref_db_ids"] = decoration_start + "/".join(hitDbInfoList) + "<br/>"
-            else:
-                self.__summaryPageInfoMap[gId]["ref_db_ids"] = decoration_start + "-<br/>"
+            # Reference sequences -
             #
-            if len(dbAccessionList) > 0:
-                displayList = []
-                for valTup in dbAccessionList:
-                    accCode = valTup[0]
-                    if hitDbIdList and (valTup[0] not in hitDbIdList):
-                        accCode = '<span style="color:red">' + valTup[0] + '</span>'
-                    #
-                    taxId = ""
-                    if len(valTup[1]) > 0:
-                        taxId = "[" + valTup[1] + "]"
-                        if valTup[1] not in authTaxIdList:
-                            taxId = '[<span style="color:red">' + valTup[1] + '</span>]'
-                        #
+            idListRef = []
+            if gId in self.__I["ref"]:
+                for partId, (altId, ver) in self.__I["ref"][gId].items():
+                    seqRefIdx = self.__sds.getSequence(seqId=gId, seqType="ref", partId=partId, altId=altId, version=ver)
+                    seqRefFD = self.__sds.getFeature(seqId=gId, seqType="ref", partId=partId, altId=altId, version=ver)
+                    seqLabel.set(seqType="ref", seqInstId=gId, seqPartId=partId, seqAltId=altId, seqVersion=ver)
+                    idRefSeq = seqLabel.pack()
+                    idListRef.append(idRefSeq)
                     #
-                    if taxId:
-                        accCode += " " + taxId
+                    refFeatureD[(gId, partId)] = (idRefSeq, altId, seqRefFD, partId)
+                    allRefSeqIdxD[idRefSeq] = seqRefIdx
+                    #
+                    if self.__verbose:
+                        self.__lfh.write("+SequenceDataExport.__exportSeqMapping() from entity group %s part %s exporting reference sequence %s\n" % (gId, partId, idRefSeq))
                     #
-                    displayList.append(accCode)
                 #
-                self.__summaryPageInfoMap[gId]["ref_db_ids"] += "(" + "/".join(displayList) + ")" + decoration_end
             else:
-                self.__summaryPageInfoMap[gId]["ref_db_ids"] += "(-)" + decoration_end
+                # report missing reference sequence
+                if self.__verbose:
+                    self.__lfh.write("+SequenceDataExport.__exportSeqMapping() missing reference sequence from group %s\n" % gId)
+                #
             #
-            displayMethod = method.upper()
-            warningErrorMsgs = ""
-            alignData = AlignmentDataStore(reqObj=self.__reqObj, entityId=gId, verbose=self.__verbose, log=self.__lfh)
-            warningErrorD = alignData.getSummaryPageInfo()
-            if warningErrorD:
-                for item in ("acetylation", "amidation", "cloning artifact", "conflict", "chromophore", "deletion", "engineered mutation", "expression tag",
-                             "initiating methionine", "insertion", "linker", "microheterogeneity", "microheterogeneity/modified residue", "mismatch",
-                             "modified residue", "variant"):
-                    if item not in warningErrorD:
-                        continue
-                    #
-                    redFlag = False
-                    if item == "mismatch":
-                        redFlag = True
-                    elif item == "expression tag":
-                        if displayMethod == "NAT":
-                            displayMethod = '<span style="color:red">' + method.upper() + '</span>'
-                            redFlag = True
-                        elif warningErrorD[item] > 19:
-                            redFlag = True
-                        #
-                    #
-                    if redFlag:
-                        val = '<span style="color:red">' + item.capitalize() + '(' + str(warningErrorD[item]) + ')</span>'
-                    else:
-                        val = item.capitalize() + "(" + str(warningErrorD[item]) + ")"
-                    #
-                    if warningErrorMsgs != "":
-                        warningErrorMsgs += "<br/>"
+            # Coordinate sequences -
+            #
+            idListXyz = []
+            for seqId in seqIdList:
+                if seqId in self.__I["xyz"]:
+                    for partId, (altId, ver) in self.__I["xyz"][seqId].items():
+                        seqLabel.set(seqType="xyz", seqInstId=seqId, seqPartId=partId, seqAltId=altId, seqVersion=ver)
+                        idXyzSeq = seqLabel.pack()
+                        idListXyz.append(idXyzSeq)
                     #
-                    warningErrorMsgs += val
+                else:
+                    # report missing coordinate sequence
+                    pass
                 #
             #
-            if not warningErrorMsgs:
-                warningErrorMsgs = "-"
+            if (len(idListRef) < 1) and (len(idListXyz) < 1):
+                continue
             #
-            self.__summaryPageInfoMap[gId]["entity_types"] = decoration_start + displayMethod + "<br/>" + polyType + decoration_end
-            self.__summaryPageInfoMap[gId]["warn_err_msgs"] = decoration_start + warningErrorMsgs + decoration_end
-        #
-        self.__finish()
+            alignExport = AlignmentExport(reqObj=self.__reqObj, entityId=gId, pathInfo=self.__pI, seqDataStore=self.__sds, verbose=self.__verbose, log=self.__lfh)
+            localRptRefL, localRptCommentL, localRptCommentModL, localRptDeleteL, localRptXyzL, message, numC = alignExport.doExport(
+                idAuthSeq, idListRef, idListXyz, self.__selfRefList, sourceInfo
+            )
+            if self.__verbose:
+                errMsg = alignExport.getErrorMessage()
+                if errMsg:
+                    self.__lfh.write("\nError message for entity '%s'\n%s\n" % (gId, errMsg))
+                #
+            #
+            if len(localRptRefL) > 0:
+                rptRefL.extend(localRptRefL)
+            #
+            if len(localRptCommentL) > 0:
+                rptCommentL.extend(localRptCommentL)
+            #
+            if len(localRptCommentModL) > 0:
+                rptCommentModL.extend(localRptCommentModL)
+            #
+            if len(localRptDeleteL) > 0:
+                rptDeleteL.extend(localRptDeleteL)
+            #
+            if len(localRptXyzL) > 0:
+                rptXyzL.extend(localRptXyzL)
+            #
+            if message:
+                warningMsg += message
+            #
+            if numC > 0:
+                numConflicts += numC
+                conflictList.append((gId, numC))
+            #
+        #  END of iteration over  --- gId  ----
         #
-        warningMsg = ""
-        if len(self.__natureSourceTaxIds) > 1:
+        if len(natureSourceTaxIds) > 1:
             warningMsg += "Entry contains multiple natural sources:<br />\n"
-            for k, v in self.__natureSourceTaxIds.items():
+            for k, v in natureSourceTaxIds.items():
                 if len(v) > 1:
                     warningMsg += "Entities '" + "', '".join(v) + "' have "
                 else:
                     warningMsg += "Entity '" + "', '".join(v) + "' has "
                 #
                 warningMsg += "source taxonomy Id '" + k + "'.<br />\n"
             #
         #
-        if self.__partRangeErrorMsg != "":
-            if warningMsg:
-                warningMsg += "<br />\n"
-            #
-            warningMsg += "Part range errors:<br />\n" + self.__partRangeErrorMsg
-        #
         if polyAlaCaseList:
             for polyAlaCaseTupL in polyAlaCaseList:
                 if warningMsg:
                     warningMsg += "<br />\n"
                 #
                 warningMsg += "Entity [" + polyAlaCaseTupL[0] + "]"
                 if polyAlaCaseTupL[1] == 1:
                     warningMsg += " is composed only of poly-ALA.<br />\n"
                 else:
                     warningMsg += " has stretches of poly-ALA.<br />\n"
                 #
             #
-        #
-        return summaryDataObj, warningMsg
-
-    def __buildAuthSection(self, groupId=None, op="load"):
-        """Assemble the data content for the author sequence summary view.
-
-        Returns: summaryDataObject)
-
-        ** Always show a single full sequence for each entity and store multi-part information as details
-
-        """
-        #
-        # Each author entity sequence is shown once and is labeled by its first instance in the group.
-        #
-        # seqId0 = groupId
-        #
-        partIdList = self.__sds.getPartIds(groupId, dataType="sequence", seqType="auth")
-        if len(partIdList) == 0:
-            return {}, 0, {}, "", "", []
-        #
-        altId = 1
-        verList = self.__sds.getVersionIds(groupId, partId=partIdList[0], altId=altId, dataType="sequence", seqType="auth")
-        if len(verList) == 0:
-            return {}, 0, {}, "", "", []
-        #
-        if self.__verbose:
-            self.__lfh.write("SummaryView.__buildAuthSection() groupId %r op %s \n" % (groupId, op))
-        #
-        detailsD, dbAccessionList = self.__getAuthFeaturesAll(groupId, groupId, partIdList)
-        #
-        dT = self.__getAuthSection(groupId, partIdList[0], altId, verList, detailsD, len(partIdList))
-        #
-        # Get polyALA_assignment
-        #
-        polyALA_assignment, method, polyType = self.__checkPolyAlaAssignment(seqId=groupId, partId=partIdList[0], altId=altId, version=verList[0])
-        #
-        summaryPageD = self.__getSummaryPageInfo(seqId=groupId, partIdList=partIdList, altId=altId)
-        #
-        return dT, polyALA_assignment, summaryPageD, method, polyType, dbAccessionList
+        # ref FeatureD ---
+        rptRefDbL = self.__refDdReport(refFeatureD)
+        # rptDeleteL = self.__deletionReport(refFeatureD, allRefSeqIdxD)
 
-    def __buildCoordinateSection(self, groupId=None):
-        """Assemble the data content for the coordinate sequence summary view.
-
-        Returns: summaryDataObject
-
-        """
-        seqLabel = SequenceLabel()
-        seqFeature = SequenceFeature()
-
-        #
-        # For each coordinate sequence -
-        #
-        seqIdList = self.__sds.getGroup(groupId)
-
-        rowIdList = []
-        rowStatusList = []
-        rowDataDictList = []
-        #
-        partId = 1
-        altId = 1
-        for seqId in seqIdList:
-            verList = self.__sds.getVersionIds(seqId=seqId, partId=partId, altId=altId, dataType="sequence", seqType="xyz")
-            if len(verList) < 1:
-                continue
-            maxVrsnNum = verList[0]
-            seqLabel.set(seqType="xyz", seqInstId=seqId, seqPartId=partId, seqAltId=altId, seqVersion=maxVrsnNum)
-            maxSeqXyzId = seqLabel.pack()
-
-            # select the highest version sequence
-            if not (maxSeqXyzId in self.__summarySeqSelectList):
-                self.__summarySeqSelectList.append(maxSeqXyzId)
-                self.__summarySeqAlignList.append(maxSeqXyzId)
-
-            for ver in verList:
-                seqXyz = self.__sds.getSequence(seqId, "xyz", partId=partId, altId=altId, version=ver)
-                seqXyzFD = self.__sds.getFeature(seqId, "xyz", partId=partId, altId=altId, version=ver)
-                seqLabel.set(seqType="xyz", seqInstId=seqId, seqPartId=partId, seqAltId=altId, seqVersion=ver)
-                seqXyzId = seqLabel.pack()
-                #
-                seqFeature.set(seqXyzFD)
-                sfd = SequenceFeatureDepict(sfObj=seqFeature, verbose=self.__verbose, log=self.__lfh)
-                detailString = sfd.markupXyzFeatures()
-                #
-                rowLabel = seqId
-                rowIdList.append(seqXyzId)
-                #
-                # unselect any selected lower version for this sequence -
-                if (ver < maxVrsnNum) and (seqXyzId in self.__summarySeqSelectList):
-                    self.__summarySeqSelectList.remove(seqXyzId)
-                    if seqXyzId in self.__summarySeqAlignList:
-                        self.__summarySeqAlignList.remove(seqXyzId)
-                #
-                isSelected = seqXyzId in self.__summarySeqSelectList
-                isAligned = seqXyzId in self.__summarySeqAlignList
-                # JDW add instance here to provide a selection group
-                if ver == maxVrsnNum:
-                    rowStatusList.append((isSelected, isAligned, seqId, "maxver"))
-                else:
-                    rowStatusList.append((isSelected, isAligned, seqId, ""))
-                #
-                rowDataDict = {}
-                rowDataDict["ROW_ID_CODE"] = rowLabel
-                rowDataDict["ROW_VERSION"] = ver
-                rowDataDict["ROW_SEQ_LENGTH"] = len(seqXyz)
-                rowDataDict["ROW_DETAIL_STRING"] = detailString
-                rowDataDict.update(seqXyzFD)
-                rowDataDictList.append(rowDataDict)
-        #
-        dT = {}
-        dT["ROW_IDS"] = rowIdList
-        dT["ROW_STATUS"] = rowStatusList
-        dT["ROW_DATA_DICT"] = rowDataDictList
-        return dT
-
-    def __buildReferenceSection(self, groupId=None):
-        """Assemble the data content for the reference sequence summary view.
-
-        Returns: [(partId,summaryDataObject),]
-
-               where:
-                  partId is the integer identifier for pieces of a multipart entity sequence
-                  summaryDataObject contains the 'ref' sequence summary data for the input groupId.
-        """
-        rL = []
-        withGapScoreList = []
-        withoutGapScoreList = []
-        hitDbInfoList = []
-        hitDbIdList = []
-        authTaxIdList = []
-        seqLabel = SequenceLabel()
-        seqFeature = SequenceFeature()
-        #
-        # use the leading sequence Id in the group as the id for the reference -
-        #
-        seqIdRef = groupId
-        #
-        partInfoList = []
-        partIdList = self.__sds.getPartIds(seqIdRef, dataType="sequence", seqType="auth")
-        for partId in partIdList:
-            #
-            authVerList = self.__sds.getVersionIds(seqId=seqIdRef, partId=partId, altId=1, dataType="feature", seqType="auth")
-            # Changed to original tax ID ( DAOTHER-6126 )
-            OrigTaxId = ""
-            skipPart = False
-            if len(authVerList) > 0:
-                authFObj = self.__sds.getFeatureObj(seqIdRef, "auth", partId=partId, altId=1, version=authVerList[0])
-                sourceInfo = authFObj.getEntitySourceMethod().upper()
-                OrigTaxId = authFObj.getSourceTaxIdOrig()
-                if OrigTaxId and (OrigTaxId not in authTaxIdList):
-                    authTaxIdList.append(OrigTaxId)
-                #
-                TaxId = authFObj.getSourceTaxId()
-                if (sourceInfo == "NAT") and TaxId:
-                    if TaxId in self.__natureSourceTaxIds:
-                        self.__natureSourceTaxIds[TaxId].append(groupId)
-                    else:
-                        self.__natureSourceTaxIds[TaxId] = [groupId]
-                    #
-                #
-                authPartId, authSeqBeg, authSeqEnd, authSeqPartType = authFObj.getAuthPartDetails()
-                partInfoList.append((authPartId, authSeqBeg, authSeqEnd))
-                skipPart = len(authSeqPartType) > 1 and authSeqPartType.lower() != "biological sequence"
-            #
-            if skipPart:
-                self.__lfh.write("+SummaryView.__buildReferenceSection() entity %s skipping part %s type %s\n" % (groupId, partId, authSeqPartType))
-                continue
-            #
-            rowIdList = []
-            rowStatusList = []
-            rowDataDictList = []
-            # List of reference sequences for this group only for the leading sequence -
-            #
-            altIdList = self.__sds.getAlternativeIds(seqIdRef, dataType="sequence", seqType="ref", partId=partId)
-
-            srId = "selfref_" + str(groupId) + "_" + str(partId)
-            if srId in self.__summarySeqSelectList:
-                if self.__verbose:
-                    self.__lfh.write("+SummaryView.__buildReferenceSection() using self-refereence for entity %s part %s\n" % (groupId, partId))
-                selfRefFlag = True
-            else:
-                selfRefFlag = False
-            #
-            for altId in altIdList[: self.__maxRefAlign]:
-                #
-                verList = self.__sds.getVersionIds(seqId=seqIdRef, partId=partId, altId=altId, dataType="sequence", seqType="ref")
-                for ver in verList:
-                    #
-                    seqRefFD = self.__sds.getFeature(seqIdRef, "ref", partId=partId, altId=altId, version=ver)
-                    seqFeature.set(seqRefFD)
-                    seqLabel.set(seqType="ref", seqInstId=seqIdRef, seqPartId=partId, seqAltId=altId, seqVersion=ver)
-                    seqRefId = seqLabel.pack()
-                    #
-                    taxIdWarningFlag = False
-                    RefTaxId = seqFeature.getSourceTaxId()
-                    if OrigTaxId and RefTaxId and (OrigTaxId != RefTaxId):
-                        taxIdWarningFlag = True
-                    #
-                    isSelected = seqRefId in self.__summarySeqSelectList
-                    if isSelected:
-                        if ("AUTH_REF_SEQ_SIM_WITH_GAPS" in seqRefFD) and (float(seqRefFD["AUTH_REF_SEQ_SIM_WITH_GAPS"]) > 0.001):
-                            withGapScoreList.append("%6.3f" % float(seqRefFD["AUTH_REF_SEQ_SIM_WITH_GAPS"]))
-                        #
-                        if ("AUTH_REF_SEQ_SIM" in seqRefFD) and (float(seqRefFD["AUTH_REF_SEQ_SIM"]) > 0.001):
-                            withoutGapScoreList.append("%6.3f" % float(seqRefFD["AUTH_REF_SEQ_SIM"]))
-                        #
-                        dbName = ""  # noqa: F841 pylint: disable=unused-variable
-                        if ("DB_NAME" in seqRefFD) and seqRefFD["DB_NAME"]:
-                            dbName = seqRefFD["DB_NAME"]  # noqa: F841
-                        #
-                        dbAccession = ""
-                        if ("DB_ACCESSION" in seqRefFD) and seqRefFD["DB_ACCESSION"]:
-                            dbAccession = seqRefFD["DB_ACCESSION"]
-                        #
-                        if ("DB_ISOFORM" in seqRefFD) and seqRefFD["DB_ISOFORM"]:
-                            dbAccession = seqRefFD["DB_ISOFORM"]
-                        #
-                        if dbAccession:
-                            refTaxId = RefTaxId
-                            if taxIdWarningFlag:
-                                refTaxId = '<span style="color:red">' + RefTaxId + "</span>"
-                            #
-                            if refTaxId:
-                                hitDbInfoList.append(dbAccession + " [" + refTaxId + "]")
-                            else:
-                                hitDbInfoList.append(dbAccession)
-                            #
-                            if dbAccession not in hitDbIdList:
-                                hitDbIdList.append(dbAccession)
-                            #
-                        #
-                    #
-                    isAligned = seqRefId in self.__summarySeqAlignList
-                    rowStatusList.append((isSelected, isAligned))
-                    #
-                    sfd = SequenceFeatureDepict(sfObj=seqFeature, verbose=self.__verbose, log=self.__lfh)
-                    detailString = sfd.markupReferenceAlignmentFeatures()
-                    featureString = sfd.markupReferenceFeatures()
-                    rowLabel = sfd.markupDatabaseReferenceWithUrl(altId)
-                    rowIdList.append(seqRefId)
-
-                    lengthRefSeq = seqFeature.getMatchLength()
-                    # authSimWithGaps = seqFeature.getAuthRefSimWithGaps()
-                    #
-                    #
-                    rowDataDict = {}
-                    rowDataDict["ROW_ID_CODE"] = rowLabel
-                    rowDataDict["ROW_VERSION"] = ver
-                    rowDataDict["ROW_SEQ_LENGTH"] = lengthRefSeq
-                    # rowDataDict['ROW_AUTH_REF_SIM'] = "%.3f" % authSimWithGaps
-                    rowDataDict["ROW_AUTH_REF_SIM"] = sfd.markupReferenceSimilarttFeatures()
-                    rowDataDict["ROW_DETAIL_STRING"] = detailString
-                    rowDataDict["ROW_FEATURE_STRING"] = featureString
-                    rowDataDict["ROW_IS_SELECTED"] = isSelected
-                    rowDataDict["ROW_IS_ALIGNED"] = isAligned
-                    # rowDataDict.update(seqRefFD)
-                    for key, _val in seqRefFD.items():
-                        if (key == "SOURCE_TAXID") and taxIdWarningFlag:
-                            rowDataDict[key] = '<span style="color:red">' + seqRefFD[key] + "</span>"
-                        else:
-                            rowDataDict[key] = seqRefFD[key]
-                        #
-                    #
-                    rowDataDictList.append(rowDataDict)
-            #
-            dT = {}
-            dT["ROW_IDS"] = rowIdList
-            dT["ROW_STATUS"] = rowStatusList
-            dT["ROW_DATA_DICT"] = rowDataDictList
-            dT["SELF_REFERENCE_FLAG"] = selfRefFlag
-            rL.append((partId, dT))
-        #
-        self.__checkPartRange(groupId, partInfoList)
-        #
-        return rL, withGapScoreList, withoutGapScoreList, hitDbInfoList, hitDbIdList, authTaxIdList
-
-    def __buildNameSourceSummaryPage(self, key, summaryInfoD):
-        """
-        """
-        currList = []
-        origList = []
-        if (key in summaryInfoD) and summaryInfoD[key]:
-            for val in summaryInfoD[key]:
-                if val:
-                    currList.append(val)
-                else:
-                    currList.append("-")
-                #
-            #
-        else:
-            currList.append("-")
-        #
-        origKey = key + "_ORIG"
-        if (origKey in summaryInfoD) and summaryInfoD[origKey]:
-            for val in summaryInfoD[origKey]:
-                if val:
-                    origList.append(val)
-                else:
-                    origList.append("-")
-                #
+        try:
+            # Make a local copy of the mapping file in the session directory and then copy the file as needed.
             #
-        else:
-            origList.append("-")
-        #
-        chimera = ""
-        if (key == "ENTITY_DESCRIPTION") and (len(currList) > 1):
-            chimera = " chimera"
-        #
-        return "/".join(currList) + chimera + "<br/>(" + "/".join(origList) + chimera + ")"
-
-    def __getAuthFeaturesAll(self, entityId, seqId0, partIdList):
-        """Consolidate the feature data for the author sequences entity sequence respecting
-        potential mutiple source details.
-
-        Original and current features are assembled.
-
-        Returns a dictionaries of features for each sequence version.
-
-        Details[ver][partId]['current']={'partdetails','sourceAndStrain','description','hostorg'}
-        Details[ver][partId]['author']={'partdetails','sourceAndStrain','description','hostorg'}
-        """
-        if self.__verbose:
-            self.__lfh.write("+SummaryView.__getAuthFeaturesAll() entityId %r seqId0 %r partIdList %r\n" % (entityId, seqId0, partIdList))
-
-        #
-        authRefAssignText, dbAccessionList = self.__markupAuthorAssignments(entityId)
-        #
-        #
-        altId = 1
-        detailsD = {}
-        for partId in partIdList:
-            verList = self.__sds.getVersionIds(seqId0, partId=partId, altId=altId, dataType="sequence", seqType="auth")
-            for ver in verList:
-                if ver not in detailsD:
-                    detailsD[ver] = {}
-
-                sfObj = self.__sds.getFeatureObj(seqId=seqId0, seqType="auth", partId=partId, altId=altId, version=ver)
-                sfd = SequenceFeatureDepict(sfObj=sfObj, verbose=self.__verbose, log=self.__lfh)
-
-                if partId not in detailsD[ver]:
-                    detailsD[ver][partId] = {}
-
-                detailsD[ver][partId]["current"] = sfd.markupCurrentEntityDetails()
-                detailsD[ver][partId]["author"] = sfd.markupAuthorEntityDetails()
+            blockList = []
+            ofh = open(self.__exportFilePathSession, "w")
+            dataBlock = DataContainer(depDataSetId)
+            if len(self.__trueSelfReferenceEntityList) > 0:
+                dataBlock.append(self.__cifCatSelfReference(self.__trueSelfReferenceEntityList))
+            #
+            if len(rptRefDbL) > 0:
+                dataBlock.append(
+                    self.__writeGeneralCifCategory(
+                        "pdbx_seqtool_db_ref", ("ordinal", "entity_id", "db_name", "db_code", "db_accession", "db_isoform", "match_begin", "match_end", "entity_part_id"), rptRefDbL
+                    )
+                )
+            #
+            if len(self.__annoRefDbL) > 0:
+                dataBlock.append(
+                    self.__writeGeneralCifCategory(
+                        "pdbx_seqtool_anno_db_ref", ("ordinal", "entity_id", "db_name", "db_code", "db_accession", "match_begin", "match_end", "entity_part_id"), self.__annoRefDbL
+                    )
+                )
+                #
+                for k, seqAuthRefMap in self.__annoSeqAuthRefMap.items():
+                    for seqAuth in seqAuthRefMap:
+                        seqAuth[0] = str(len(rptRefL) + 1)
+                        rptRefL.append(tuple(seqAuth))
+                    #
+                #
+            #
+            dataBlock.append(self.__getEntitySourceCategory())
+            #
+            if len(rptCommentL) > 0:
+                dataBlock.append(
+                    self.__writeGeneralCifCategory("pdbx_seqtool_mapping_comment", ("ordinal", "entity_id", "entity_mon_id", "entity_seq_num", "comment"), rptCommentL)
+                )
+            #
+            if len(rptCommentModL) > 0:
+                dataBlock.append(
+                    self.__writeGeneralCifCategory(
+                        "pdbx_seqtool_mapping_modification_comment", ("ordinal", "entity_id", "entity_mon_id", "entity_seq_num", "comment"), rptCommentModL
+                    )
+                )
+            #
+            if len(rptDeleteL) > 0:
+                dataBlock.append(
+                    self.__writeGeneralCifCategory(
+                        "pdbx_seqtool_ref_deletions", ("ordinal", "entity_id", "part_id", "db_name", "db_accession", "db_isoform", "ref_mon_id", "ref_mon_num"), rptDeleteL
+                    )
+                )
+            #
+            if len(rptRefL) > 0:
+                dataBlock.append(
+                    self.__writeGeneralCifCategory(
+                        "pdbx_seqtool_mapping_ref",
+                        ("ordinal", "entity_id", "entity_mon_id", "entity_seq_num", "auth_asym_id", "ref_mon_id", "ref_mon_num", "entity_part_id"),
+                        rptRefL,
+                    )
+                )
+            #
+            if len(rptXyzL) > 0:
+                dataBlock.append(
+                    self.__writeGeneralCifCategory(
+                        "pdbx_seqtool_mapping_xyz",
+                        ("ordinal", "entity_id", "entity_mon_id", "entity_seq_num", "auth_asym_id", "pdb_mon_id", "pdb_mon_num", "pdb_ins_code", "hetero_flag", "org_mon_id"),
+                        rptXyzL,
+                    )
+                )
+            #
+            blockList.append(dataBlock)
+            pdbxW = PdbxWriter(ofh)
+            pdbxW.write(blockList)
+            ofh.close()
+        except:  # noqa: E722 pylint: disable=bare-except
+            if self.__verbose:
+                self.__lfh.write("+SequenceDataExport.__exportSeqMapping() saving export mapping file failed %s\n" % self.__exportFilePathSession)
+                traceback.print_exc(file=self.__lfh)
+            return False, numConflicts, conflictList, warningMsg
 
-                if len(authRefAssignText) > 0:
-                    detailsD[ver][partId]["author"]["description"] += authRefAssignText
+        return True, numConflicts, conflictList, warningMsg
 
-        for ver in detailsD.keys():
-            np = 0
-            for partId in partIdList:
-                if partId in detailsD[ver]:
-                    np += 1
-            detailsD[ver]["numparts"] = np
-        if self.__debug:
-            self.__lfh.write("+SummaryView.__getAuthFeaturesAll() detailsD entity %r seqId %r partIdList %r\n" % (entityId, seqId0, partIdList))
-            fOut = FormatOut()
-            fOut.autoFormat("Summary Entity Details", detailsD, 3, 3)
-            fOut.writeStream(self.__lfh)
-            fOut.clear()
-        #
-        return detailsD, dbAccessionList
-
-    def __checkPolyAlaAssignment(self, seqId="", partId="1", altId=1, version="1"):
-        """Check if the sequence contains 10 or more consecutive ALA residues
-        """
-        authFObj = self.__sds.getFeatureObj(seqId, "auth", partId=partId, altId=altId, version=version)
-        if authFObj.getPolymerType() != "AA":
-            return 0, authFObj.getEntitySourceMethod(), authFObj.getPolymerLinkingType()
-        #
-        seqAuth = self.__sds.getSequence(seqId=seqId, seqType="auth", partId=partId, altId=altId, version=version)
+    def __checkPolyAlaAssignment(self, seqAuth):
+        """Check if the sequence contains 10 or more consecutive ALA residues"""
         has_consecutive_ALA = False
         count = 0
         for seqTupL in seqAuth:
             if seqTupL[0] == "ALA":
                 count += 1
             else:
                 if count > 9:
@@ -735,262 +605,188 @@
                 count = 0
             #
         #
         if count > 9:
             has_consecutive_ALA = True
         #
         if count == len(seqAuth):
-            return 1, authFObj.getEntitySourceMethod(), authFObj.getPolymerLinkingType()
+            return 1
         elif has_consecutive_ALA:
-            return 2, authFObj.getEntitySourceMethod(), authFObj.getPolymerLinkingType()
+            return 2
         #
-        return 0, authFObj.getEntitySourceMethod(), authFObj.getPolymerLinkingType()
+        return 0
 
-    def __getSummaryPageInfo(self, seqId="1", partIdList=None, altId=1):
-        """
-        """
-        if partIdList is None:
-            partIdList = []
-
-        infoKeys = ("ENTITY_DESCRIPTION", "ENTITY_DESCRIPTION_ORIG", "SOURCE_ORGANISM", "SOURCE_ORGANISM_ORIG", "SOURCE_TAXID", "SOURCE_TAXID_ORIG")
-        #
-        retValD = {}
-        for partId in partIdList:
-            verList = self.__sds.getVersionIds(seqId, partId=partId, altId=altId, dataType="sequence", seqType="auth")
-            valD = {}
-            if len(verList) > 0:
-                authFObj = self.__sds.getFeatureObj(seqId, "auth", partId=partId, altId=altId, version=verList[0])
-                mapD = authFObj.get()
-                for key in infoKeys:
-                    if (key in mapD) and mapD[key]:
-                        valD[key] = mapD[key]
-                        #
-                        additionlKey = ""
-                        if key == "SOURCE_ORGANISM":
-                            additionlKey = "SOURCE_STRAIN"
-                        elif key == "SOURCE_ORGANISM_ORIG":
-                            additionlKey = "SOURCE_STRAIN_ORIG"
-                        #
-                        if additionlKey and (additionlKey in mapD) and mapD[additionlKey]:
-                            valD[key] = mapD[key] + " " + mapD[additionlKey]
-                        #
-                    #
-                #
-            #
-            if ("SOURCE_TAXID" in valD) and ("SOURCE_TAXID_ORIG" in valD) and (valD["SOURCE_TAXID"] != valD["SOURCE_TAXID_ORIG"]):
-                for key in ("SOURCE_ORGANISM_ORIG", "SOURCE_TAXID_ORIG"):
-                    if (key in valD) and valD[key]:
-                        valD[key] = '<span style="color:red">' + valD[key] + '</span>'
-                    #
-                #
-            #
-            for key in infoKeys:
-                val = ""
-                if (key in valD) and valD[key]:
-                    val = valD[key]
-                #
-                if key in retValD:
-                    retValD[key].append(val)
-                else:
-                    retValD[key] = [val]
-                #
+    def __refDdReport(self, refFeatureD):
+        """Return a list of content rows for reference sequence database accession report --"""
+        rptRefDbL = []
+        irow = 1
+        for (gId, partId), tup in refFeatureD.items():
+            if (str(gId), str(partId)) in self.__selfReferenceEntityList:
+                continue
             #
-        #
-        return retValD
-
-    def __getAuthSection(self, seqId0, partId0, altId, verList, detailsD, partIdListLength):
-        """Assemble the data content for the author sequence summary view.
-
-        Returns: summaryDataObject)
+            # sId = tup[0]
+            fD = tup[2]
+            rptRefDbL.append(
+                [
+                    irow,
+                    gId,
+                    self.__srd.convertDbNameToResource(fD["DB_NAME"]),
+                    fD["DB_CODE"],
+                    fD["DB_ACCESSION"],
+                    fD["DB_ISOFORM"],
+                    fD["REF_MATCH_BEGIN"],
+                    fD["REF_MATCH_END"],
+                    partId,
+                ]
+            )
+            irow += 1
+        #
+        return rptRefDbL
+
+    # def __deletionReport(self, refFeatureD, allRefSeqIdxD):
+    #     """Return a list of content rows for the sequence deletion report."""
+    #     rptDeleteL = []
+    #     idel = 1
+    #     for (gId, partId), tup in refFeatureD.items():
+    #         if (str(gId), str(partId)) in self.__selfReferenceEntityList:
+    #             continue
+    #         #
+    #         sId = tup[0]
+    #         fD = tup[2]
+    #         if sId in allRefSeqIdxD:
+    #             if self.__verbose:
+    #                 self.__lfh.write("+SequenceDataExport.__exportSeqMapping() searching deletions in seqId %s\n" % sId)
+    #             #
+    #             refSeqIdx = allRefSeqIdxD[sId]
+    #             for sTup in refSeqIdx:
+    #                 if sTup[2] in ["Deletion", "deletion"]:
+    #                     if self.__verbose:
+    #                         self.__lfh.write("+SequenceDataExport.__exportSeqMapping() position %s comment %s\n" % (sTup[1], sTup[2]))
+    #                     #
+    #                     rptDeleteL.append([idel, gId, partId, self.__srd.convertDbNameToResource(fD["DB_NAME"]), fD["DB_ACCESSION"], fD["DB_ISOFORM"], sTup[0], sTup[1]])
+    #                     idel += 1
+    #                 #
+    #             #
+    #         else:
+    #             self.__lfh.write("+SequenceDataExport.__exportSeqMapping() delete scan missing reference sequence for seqId %s keys() %r\n" % (sId, allRefSeqIdxD.keys()))
+    #         #
+    #     #
+    #     return rptDeleteL
+
+    def __cifCatSelfReference(self, entityList):
+        """Update entities for self reference  ---"""
+        aCat = DataCategory("pdbx_seqtool_self_ref")
+        aCat.appendAttribute("entity_id")
+        aCat.appendAttribute("entity_part_id")
+        for eid, partId in entityList:
+            aCat.append([eid, partId])
+        return aCat
+
+    def __writeGeneralCifCategory(self, categoryName, categoryItems, dataList):
+        """Write pdbx_seqtool_db_ref, pdbx_seqtool_anno_db_ref, pdbx_seqtool_ref_deletions, pdbx_seqtool_mapping_ref, pdbx_seqtool_mapping_comment,
+        pdbx_seqtool_mapping_modification_comment, pdbx_seqtool_mapping_xyz categories
+        """
+        if len(dataList) < 1:
+            return None
+        #
+        aCat = DataCategory(categoryName)
+        for itemName in categoryItems:
+            aCat.appendAttribute(itemName)
+        #
+        rowCount = 0
+        for row in dataList:
+            rowCount += 1
+            row[0] = str(rowCount)
+            aCat.append(row)
+        #
+        return aCat
+
+    def __getEntitySourceCategory(self):
+        """Return category object of source details."""
+        itemTupList = [
+            ("ORDINAL", "ordinal"),
+            ("ENTITY_ID", "entity_id"),
+            ("AUTH_SEQ_PART_ID", "seq_part_id"),
+            ("AUTH_SEQ_NUM_BEGIN", "seq_part_beg"),
+            ("AUTH_SEQ_NUM_END", "seq_part_end"),
+            ("AUTH_SEQ_PART_TYPE", "seq_part_type"),
+            ("ENTITY_DESCRIPTION", "entity_description"),
+            ("ENTITY_SYNONYMS", "entity_synonyms"),
+            ("SOURCE_GENE_NAME", "gene_name"),
+            ("SOURCE_TAXID", "taxonomy_id"),
+            ("SOURCE_ORGANISM", "source_scientific_name"),
+            ("SOURCE_STRAIN", "source_strain"),
+            ("SOURCE_COMMON_NAME", "source_common_name"),
+            ("SOURCE_VARIANT", "variant"),
+            ("POLYMER_LINKING_TYPE", "entity_polymer_type"),
+            ("ENTITY_ENZYME_CLASS", "entity_enzyme_class"),
+            ("ENTITY_FRAGMENT_DETAILS", "entity_fragment_details"),
+            ("ENTITY_MUTATION_DETAILS", "entity_mutation_details"),
+            ("ENTITY_DETAILS", "entity_details"),
+            ("SOURCE_METHOD", "source_method"),
+            ("HOST_ORG_SOURCE", "host_org_scientific_name"),
+            ("HOST_ORG_STRAIN", "host_org_strain"),
+            ("HOST_ORG_TAXID", "host_org_taxonomy_id"),
+            ("HOST_ORG_VECTOR", "host_org_vector"),
+            ("HOST_ORG_VECTOR_TYPE", "host_org_vector_type"),
+            ("HOST_ORG_PLASMID", "host_org_plasmid"),
+            ("HOST_ORG_COMMON_NAME", "host_org_common_name"),
+            ("HOST_ORG_CELL_LINE", "host_org_cell_line"),
+            ("HOST_ORG_VARIANT", "host_org_variant"),
+        ]
 
-        ** Always show a single full sequence for each entity and store multi-part information as details
-
-        """
-        seqLabel = SequenceLabel()
-        #
-        rowIdList = []
-        rowStatusList = []
-        rowDataDictList = []
-        #
-        for ver in verList:
-            seqAuth = self.__sds.getSequence(seqId=seqId0, seqType="auth", partId=partId0, altId=altId, version=ver)
-            seqLabel.set(seqType="auth", seqInstId=seqId0, seqPartId=partId0, seqAltId=altId, seqVersion=ver)
-            seqAuthId = seqLabel.pack()
-            rowIdList.append(seqAuthId)
-            #
-            isSelected = seqAuthId in self.__summarySeqSelectList
-            isAligned = seqAuthId in self.__summarySeqAlignList
-            #
-            # if op == 'reload':
-            #     isSelected = (ver == max(verList))
-            #     isAligned = (ver == max(verList))
-            # #
-            #
-            rowStatusList.append((isSelected, isAligned))
-            #
-            rowDataDict = {}
-            rowDataDict["ROW_VERSION"] = ver
-            rowDataDict["ROW_SEQ_LENGTH"] = len(seqAuth)
-            rowDataDict["ROW_DETAIL_STRING"] = ""
-            rowDataDict.update(detailsD[ver])
-            rowDataDictList.append(rowDataDict)
-        #
-        dT = {}
-        dT["ROW_IDS"] = rowIdList
-        dT["ROW_STATUS"] = rowStatusList
-        dT["ROW_DATA_DICT"] = rowDataDictList
-        dT["ENTITY_NUM_PARTS"] = partIdListLength
-        #
-        return dT
-
-    def __markupAuthorAssignments(self, entityId):
-        """Markup the author provided reference assignments -"""
-        spStr = "<br />"
-        authRefAssignText = ""
-        dbAccessionList = []
-        dbAccessionMap = {}
-        depSeqAssignD = self.__sds.getDepositorReferenceAssignments()
-        sADep = SequenceAssignDepositor(verbose=self.__verbose, log=self.__lfh)
-        sADep.set(depSeqAssignD)
-        refSeqAssignL = sADep.getReferenceList(entityId)
-
-        if self.__debug:
-            self.__lfh.write("+SummaryView.__markupAuthorAssignments() for entityId %r author reference count is %d\n" % (entityId, sADep.getReferenceCount(entityId)))
-            sADep.printIt(log=self.__lfh)
-            for ii, rsa in enumerate(refSeqAssignL):
-                self.__lfh.write("+SummaryView.__markupAuthorAssignments() depositor reference  %d\n" % (ii + 1))
-                rsa.printIt(self.__lfh)
-        #
-
-        for rsa in refSeqAssignL:
-            dbName, dbCode, dbAccession = rsa.getDbReference()
-            if (len(dbAccession) > 0) and (dbAccession not in [".", "?"]):
-                if dbAccession not in dbAccessionList:
-                    dbAccessionList.append(dbAccession)
-                    if (dbAccession not in dbAccessionMap) and (len(dbName) > 0) and (dbName not in [".", "?"]):
-                        dbAccessionMap[dbAccession] = dbName.upper()
-                    #
-                #
-            #
-            if ((len(dbAccession) > 0) and (dbAccession not in [".", "?"])) or ((len(dbCode) > 0) and (dbCode not in [".", "?"])):
-                tRef = "<b>Depositor reference:&nbsp;</b> %s %s %s" % (dbName, dbAccession, dbCode)
-                sp = spStr if len(authRefAssignText) > 0 else ""
-                authRefAssignText += sp + tRef
-            #
-            refDetails = rsa.getDetails()
-            if len(refDetails) > 0 and refDetails not in [".", "?"]:
-                tDetails = "<b>Depositor details:&nbsp;</b> %s" % refDetails
-                sp = spStr if len(authRefAssignText) > 0 else ""
-                authRefAssignText += sp + tDetails
-            #
-        #
         if self.__verbose:
-            self.__lfh.write("+SummaryView.__markupAuthorAssignments() depositor reference assignments for entity %s : %s\n" % (entityId, authRefAssignText))
+            self.__lfh.write("+SequenceDataExport.__getSourceDetails() starting\n")
+            # self.printIt()
         #
-        if len(dbAccessionList) > 0:
-            dbAccTaxMap = {}
-            picklePath = os.path.join(self.__sessionPath, "dbAccTaxMap.pic")
-            if os.access(picklePath, os.F_OK):
-                fb = open(picklePath, "rb")
-                dbAccTaxMap = pickle.load(fb)
-                fb.close()
-            #
-            fetchSeqUtil = FetchSeqInfoUtils(siteId=str(self.__reqObj.getValue("WWPDB_SITE_ID")), verbose=self.__verbose, log=self.__lfh)
-            tmpList = []
-            for dbAccession in dbAccessionList:
-                if dbAccession in dbAccTaxMap:
-                    tmpList.append((dbAccession, dbAccTaxMap[dbAccession]))
-                    continue
-                #
-                if dbAccession not in dbAccessionMap:
-                    tmpList.append((dbAccession, ""))
-                    continue
+        rowList = []
+        entityIdList = self.__sds.getGroupIds()
+        iRow = 1
+        for entityId in entityIdList:
+            seqIds = self.__sds.getGroup(entityId)
+            if len(seqIds) < 1:
+                if self.__verbose:
+                    self.__lfh.write("+SequenceDataExport.__getSourceDetails() entityId %s is empty\n" % (entityId))
                 #
-                dbIsoform = ""
-                dbAccessionS = dbAccession
-                if dbAccessionMap[dbAccession] in ["UNP", "SP", "TR"]:
-                    tL = dbAccession.split("-")
-                    if len(tL) > 1:
-                        dbIsoform = dbAccession
-                        dbAccessionS = tL[0]
+                continue
+            #
+            seqId0 = entityId
+            partIdList = self.__sds.getPartIds(seqId0, dataType="sequence", seqType="auth")
+            #
+            for partId in partIdList:
+                if self.__verbose:
+                    self.__lfh.write("+SequenceDataExport.__getSourceDetails() entityId %r partId %r  __I  %r\n" % (entityId, partId, self.__I["auth"][seqId0][partId]))
+                # JDW
+                # altId,versionId=self.__I["auth"][seqId0][partId]
+                altId, versionId = self.__I["auth"][seqId0][1]
+                fD = self.__sds.getFeature(seqId0, seqType="auth", partId=partId, altId=altId, version=versionId)
+                d = {}
+                for itemTup in itemTupList:
+                    ky = itemTup[0]
+                    if ky in fD:
+                        d[ky] = fD[ky]
+                    else:
+                        d[ky] = ""
                     #
                 #
-                _accCode, refInfoD = fetchSeqUtil.getRefInfo(dbAccessionMap[dbAccession], dbAccessionS, dbIsoform, 0, 0, addMissingKeyFlag=False)
-                if ("taxonomy_id" in refInfoD) and refInfoD["taxonomy_id"]:
-                    tmpList.append((dbAccession, refInfoD["taxonomy_id"]))
-                    dbAccTaxMap[dbAccession] = refInfoD["taxonomy_id"]
-                else:
-                    tmpList.append((dbAccession, ""))
+                d["ORDINAL"] = iRow
+                d["ENTITY_ID"] = entityId
+                d["AUTH_SEQ_PART_ID"] = partId
+                rowList.append(d)
+                iRow += 1
                 #
             #
-            dbAccessionList = tmpList
-            #
-            fb = open(picklePath, "wb")
-            pickle.dump(dbAccTaxMap, fb)
-            fb.close()
-        #
-        return authRefAssignText, dbAccessionList
-
-    def __checkPartRange(self, entityId, partInfoList):
-        """Check part range definition and write out the warning message if there are errors"""
-        seqLength = 0
-        authVerList = self.__sds.getVersionIds(seqId=entityId, partId=1, altId=1, dataType="sequence", seqType="auth")
-        if len(authVerList) > 0:
-            seq = self.__sds.getSequence(seqId=entityId, seqType="auth", partId=1, altId=1, version=authVerList[0])
-            seqLength = len(seq)
-        #
-        if seqLength == 0:
-            return
         #
-        ok, partText = self.__checkPartRangeError(seqLength, partInfoList)
-        if ok:
-            return
+        aCat = DataCategory("pdbx_seqtool_entity_details")
+        for itemTup in itemTupList:
+            attribName = itemTup[1]
+            aCat.appendAttribute(attribName)
         #
-        if self.__partRangeErrorMsg:
-            self.__partRangeErrorMsg += "<br />\n"
-        #
-        self.__partRangeErrorMsg += "Entity '" + str(entityId) + "' (seq. length=" + str(seqLength) + ") : " + partText
-
-    def __checkPartRangeError(self, seqLength, partList):
-        """Check part range definition"""
-        if len(partList) < 1:
-            return False, "No part information defined."
-        #
-        try:
-            status = True
-            text = ""
-            for i in range(0, len(partList)):
-                if text:
-                    text += ", "
-                #
-                text += "Part '" + str(partList[i][0]) + "' - ( " + str(partList[i][1]) + ", " + str(partList[i][2]) + " )"
-                #
-                seqNumBeg = int(partList[i][1])
-                seqNumEnd = int(partList[i][2])
-                if seqNumEnd < seqNumBeg:
-                    status = False
-                if (i == 0) and (seqNumBeg != 1):
-                    status = False
-                if (i == (len(partList) - 1)) and (seqNumEnd != seqLength):
-                    status = False
-                if i > 0:
-                    prevNumEnd = int(partList[i - 1][2])
-                    if seqNumBeg != (prevNumEnd + 1):
-                        status = False
-                    #
-                #
+        for rD in rowList:
+            vL = []
+            for itemTup in itemTupList:
+                ky = itemTup[0]
+                vL.append(rD[ky])
             #
-            return status, text
-        except Exception as _e:  # noqa: F841
-            text = ""
-            for i in range(0, len(partList)):
-                if text:
-                    text += ", "
-                #
-                text += "Part '" + str(partList[i][0]) + "' - ( " + str(partList[i][1]) + ", " + str(partList[i][2]) + " )"
-            #
-            return False, text
+            aCat.append(vL)
         #
-
-
-if __name__ == "__main__":
-    pass
+        return aCat
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/AlignmentDataStore.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/AlignmentDataStore.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 ##
 # File:  AlignmentDataStore.py
 # Date:  25-Oct-2018
 #
-# Updates:
-#   27-Oct-2022 zf   add getSummaryPageInfo() method
-##
 """
 Provide a storage interface for recording sequence alignments.
 """
 __docformat__ = "restructuredtext en"
 __author__ = "Zukang Feng"
 __email__ = "zfeng@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
@@ -119,21 +116,14 @@
             self._addErrorMessage(traceback.format_exc())
         #
 
     def getErrorMessage(self):
         """Return error message"""
         return self.__errorMsg
 
-    def getSummaryPageInfo(self):
-        """Return summary page info map"""
-        if ("summary_page" in self._missingSeqMap) and self._missingSeqMap["summary_page"]:
-            return self._missingSeqMap["summary_page"]
-        #
-        return {}
-
     def serialize(self):
         """Write alignment pickle file"""
         try:
             fb = open(self.__filePath, "wb")
             pickle.dump(self._authLabel, fb)
             pickle.dump(self._hasAlignmentFlag, fb)
             pickle.dump(self._seqAlignLabelIndices, fb)
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/BlastPlusReader.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/BlastPlusReader.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 #
 #
 # Updates:
 #
 #  18-Apr-2013  jdw  modify to handle current conventions in UNP fasta files comment lines
 #                    Extract isoform information from comment lines --
 #  19-Apr-2013  jdw  remove any identity-based filtering of output
-#  24-Oct-2022  zf   added _getUniprotInfo() method to parse Uniprot information from "Hit_def" tag.
 ##
 
 
 from xml.dom import minidom
 import sys
 import traceback
 
@@ -108,56 +107,45 @@
         alignlist = []
         description = ""
         length = ""
         # _code = ""
         for node in nodelist:
             if node.nodeType != node.ELEMENT_NODE:
                 continue
-            #
+
             if node.tagName == "Hit_id":
                 dbName, dbCode, accCode, isoForm = self._parseID(node.firstChild.data)
                 if not accCode:
                     return resultList
-                #
             elif node.tagName == "Hit_accession":
                 _code = node.firstChild.data  # noqa: F841
             elif node.tagName == "Hit_def":
                 description = node.firstChild.data
             elif node.tagName == "Hit_len":
                 length = node.firstChild.data
             elif node.tagName == "Hit_hsps":
                 plist = self._ProcessHit_hspsTag(node.childNodes, length)
                 if plist:
                     for li in plist:
                         alignlist.append(li)
-                    #
-                #
-            #
-        #
+
         if not accCode or not alignlist:
             return resultList
-        #
-        desInfo = {}
-        if description and (dbName in ("SP", "TR", "UNP")):
-            desInfo = self._getUniprotInfo(description)
-        #
+
+        # dict={}
+
         for align in alignlist:
             align["db_name"] = dbName
             align["db_code"] = dbCode
             align["db_accession"] = accCode
             align["db_isoform"] = isoForm
             align["db_description"] = description
             align["db_length"] = length
-            if desInfo:
-                for key, val in desInfo.items():
-                    align[key] = val
-                #
-            #
             resultList.append(align)
-        #
+
         return resultList
 
     def _parseID(self, data):
         accCode = ""
         dbCode = ""
         dbName = ""
         isoForm = ""
@@ -172,126 +160,74 @@
                 if accCode is not None and (accCode.find("-") != -1):
                     tL = accCode.split("-")
                     if len(tL) > 1 and len(tL[1]) > 0:
                         #  Isoform is the acession + '-' + variant #
                         # isoForm=tL[1]
                         isoForm = accCode
                         accCode = tL[0]
-                    #
-                #
             elif f0 in ["GI"]:
                 dbName = str(dlist[2]).upper()
                 accCode = str(dlist[1])
                 dbCode = str(dlist[3])
-            #
-        #
+
         return dbName, dbCode, accCode, isoForm
 
     def _ProcessHit_hspsTag(self, nodelist, length):
         resultList = []
         for node in nodelist:
             if node.nodeType != node.ELEMENT_NODE:
                 continue
-            #
             if node.tagName != "Hsp":
                 continue
-            #
+
             adict = self._GetMatchAlignment(node.childNodes, length)
             if adict:
                 resultList.append(adict)
-            #
-        #
         return resultList
 
     def _GetMatchAlignment(self, nodelist, length):  # pylint: disable=unused-argument
         rdict = {}
         hsp_num = ""
         for node in nodelist:
             if node.nodeType != node.ELEMENT_NODE:
                 continue
-            #
+
             if node.tagName == "Hsp_identity":
                 rdict["identity"] = node.firstChild.data
             elif node.tagName == "Hsp_positive":
                 rdict["positive"] = node.firstChild.data
             elif node.tagName == "Hsp_gaps":
                 rdict["gaps"] = node.firstChild.data
             elif node.tagName == "Hsp_midline":
                 if self.__sequenceType == "polyribonucleotide":
                     rdict["midline"] = node.firstChild.data.replace("T", "U")
                 else:
                     rdict["midline"] = node.firstChild.data
-                #
             elif node.tagName == "Hsp_qseq":
                 if self.__sequenceType == "polyribonucleotide":
                     rdict["query"] = node.firstChild.data.replace("T", "U")
                 else:
                     rdict["query"] = node.firstChild.data
-                #
             elif node.tagName == "Hsp_query-from":
                 rdict["queryFrom"] = node.firstChild.data
             elif node.tagName == "Hsp_query-to":
                 rdict["queryTo"] = node.firstChild.data
             elif node.tagName == "Hsp_hseq":
                 if self.__sequenceType == "polyribonucleotide":
                     rdict["subject"] = node.firstChild.data.replace("T", "U")
                 else:
                     rdict["subject"] = node.firstChild.data
-                #
             elif node.tagName == "Hsp_hit-from":
                 rdict["hitFrom"] = node.firstChild.data
             elif node.tagName == "Hsp_hit-to":
                 rdict["hitTo"] = node.firstChild.data
             elif node.tagName == "Hsp_align-len":
                 rdict["alignLen"] = node.firstChild.data
                 rdict["match_length"] = node.firstChild.data
             elif node.tagName == "Hsp_num":
                 hsp_num = node.firstChild.data
-            #
+
         # only take the first alignment within the hit
         if str(hsp_num) != "1":
             rdict.clear()
-        #
-        return rdict
 
-    def _getUniprotInfo(self, description):
-        desInfo = {}
-        for tokenTupL in (("SV", ""), ("PE", ""), ("GN", "gene"), ("OX", "taxonomy_id"), ("OS", "source_scientific")):
-            idx = description.find(tokenTupL[0] + "=")
-            if idx < 0:
-                continue
-            #
-            val = description[idx + 3:].strip()
-            description = description[:idx].strip()
-            if tokenTupL[1] and val:
-                if tokenTupL[1] == "source_scientific":
-                    idx1 = val.find("(strain")
-                    if (val[-1] == ")") and idx1 >= 0:
-                        source_scientific = val[:idx1].strip()
-                        if source_scientific:
-                            desInfo[tokenTupL[1]] = source_scientific
-                        #
-                        strain = val[idx1 + 7:-1].strip()
-                        if strain:
-                            desInfo["strain"] = strain
-                        #
-                    else:
-                        desInfo[tokenTupL[1]] = val
-                #
-                elif tokenTupL[1] == "taxonomy_id":
-                    if val.isnumeric():
-                        desInfo[tokenTupL[1]] = val
-                    #
-                else:
-                    desInfo[tokenTupL[1]] = val
-                #
-            #
-        #
-        if description:
-            wList = description.split(" ")
-            if (len(wList) > 3) and (wList[0] == "Isoform") and wList[1].isnumeric() and (wList[2] == "of"):
-                desInfo["name"] = " ".join(wList[3:])
-            else:
-                desInfo["name"] = description
-            #
-        #
-        return desInfo
+        return rdict
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/ModelSequenceUtils.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/ModelSequenceUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/ModelSequenceUtilsTests.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/ModelSequenceUtilsTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/PdbxIoUtils.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/PdbxIoUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/SequenceDataExportTests.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/SequenceDataExportTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/SequenceDataExport_v2.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/control/SummaryView_v2.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,599 +1,576 @@
 ##
-# File:  SequenceDataExport_v2.py
-# Date:  14-Feb-2010
-#
+# File:    SummaryView.py
+# Date:    19-Jan-2010
 # Updates:
-#   20-Apr-2010 jdw Ported to module seqmodule.
-#   23-Apr-2010 jdw Added method for self-references.
-#   02-May-2010 jdw Add file path to constructor, move makeDefaultSelection() to SequenceSelection class.
-#                   Add handling of self-references...
-#  01-Mar-2013  jdw remove SiteInterface -
-#  08-Mar-2013  jdw adpot the standard file name conventions.
-#  08-Mar-2013  jdw add support use of sequence parts.
-#  07-Apr-2013  jdw add support for isoforms/filter self references from db references
-#  23-Apr-2013  jdw add separate category for export of modified residues
-#  05-May-2013  jdw filter gap residues from author/xyz mapping list
-#  20-Sep-2013  jdw fix filter for mapping from auth/xyz mapping
-#  14-Nov-2013  jdw add new entity details export
-#  18-Dec-2013  jdw adjust conflict array lengths after alignment --
-#  19-Jan-2014  jdw "HOST_ORG_CELL_LINE"
-#  27-Apr-2014  jdw working on fix to source detail export -
-#  28-Apr-2014  jdw verify that updateArchive=False is default --
-#                   Changes will always be applied to the first model in the session  --
-#
-# 19-May-2014   jdw refactor to better reuse new stored alignment data -
-# 22-May-2014   jdw add output conflict list
-#  3-Jun-2014   jdw fix self-reference issue
-# 16-Oct-2014   jdw add explicit flag for sequence heterogeneity
-# 22-Oct-2014   jdw add combination microheterogeneity/modified residue
-# 01-Feb-2015   jdw add host org variant
-# 01-Feb-2016   jdw change file handling for model merge -
-# 07-Sep-2017   zf  add __cifCatAnnoDbRef() to export annotator's editing db reference information
-# 31-Oct-2018   zf  split orignial SequenceDataExport into SequenceDataExport_v2 & AlignmentExport
+# 09-Feb-2010  jdw Adopt SequenceFeature() to access to feature dictionaries.
+# 12-Feb-2010  jdw Move example data loader to the SequenceDataImportExample class.
+# 14-Feb-2010  jdw Add statistics updater after primary sequence data load.
+# 20-Apr-2010  jdw Ported to module seqmodule
+# 27-Apr-2010  jdw Add row-level data dictionary to the summary data object.
+# 02-May-2010  jdw Add SequenceSelection()
+# 09-Aug-2010  rps __loadSummary() --> Highest numbered version of coordinate sequence to be selected by default in "SELECT" column of UI
+# 08-Jan-2013  jdw Select higher version of author sequence in reload operations
+# 03-Mar-2013  jdw Refactor -
+# 05-Mar-2013  jdw Move default sequence selection from SequenceSelection()
+#                  Add default self-reference selections
+#                  Implement stored sorting order for reference sequeneces --
+#                  Limit reference sequence to maxRefAlign --
+# 12-Mar-2013  jdw adjust the assembly of author sequence details -
+# 13-Apr-2013  jdw change self reference identifiers
+# 15-Nov-2013  jdw major overhaul to support expanded author content display and entity review
+# 12-Dec-2013  jdw make default alignment selections.
+# 19-Dec-2013  jdw select any added or edited reference sequence by default
+# 15-May-2014  jdw add status field for instance id with xyz sequence groups
+# 22-May-2014  jdw add method to provide entry details --
+# 30-Aug-2017  zf  change self.__reqObj.getSummaryAlignList & self.__reqObj.getSummarySelectList to use latest UI input values
+# 29-Jun-2021  zf  added self.__checkPolyAlaAssignment()
 ##
 """
-Export sequence and alignment details to production RCSB pipeline.
+Controlling class for the production of data for the summary sequence view.
 
 """
 __docformat__ = "restructuredtext en"
 __author__ = "John Westbrook"
 __email__ = "jwest@rcsb.rutgers.edu"
 __license__ = "Creative Commons Attribution 3.0 Unported"
-__version__ = "V0.07"
+__version__ = "V0.08"
 
-import os
 import sys
 import traceback
 
-from mmcif.api.DataCategory import DataCategory
-from mmcif.api.PdbxContainers import DataContainer
-from mmcif.io.PdbxWriter import PdbxWriter
-
-#
-from wwpdb.apps.seqmodule.align.AlignmentExport import AlignmentExport
 from wwpdb.apps.seqmodule.io.SequenceDataStore import SequenceDataStore
-from wwpdb.apps.seqmodule.util.SequenceReferenceData import SequenceReferenceData
-from wwpdb.apps.seqmodule.util.SequenceLabel import SequenceLabel
-from wwpdb.apps.seqmodule.util.Autodict import Autodict
+from wwpdb.apps.seqmodule.util.SequenceLabel import SequenceLabel, SequenceFeature
+from wwpdb.apps.seqmodule.util.SequenceFeatureDepict import SequenceFeatureDepict
+
+from wwpdb.apps.seqmodule.util.SequenceAssign import SequenceAssignDepositor
+from wwpdb.apps.seqmodule.update.UpdatePolymerEntitySourceDetails import UpdatePolymerEntitySourceDetails
 
-#
 from wwpdb.io.misc.FormatOut import FormatOut
-from wwpdb.io.locator.PathInfo import PathInfo
-from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
 
 
-class SequenceDataExport(object):
-    """
-    This class encapsulates all of the data export operations
-    of sequence and other data to the RCSB/WF data pipeline.
+class SummaryView(object):
+    """Controlling class for the production of data for the summary sequence view.
+
+    Supported operations:
+
+     load             = load summary from current sequence data store using default sequence selection.
+     reload           = reload summary using current sequence data and current user selections.
 
-    Storage model - exported data is loaded from the sequence data store
-                    where it is managed by the SequenceDataStore() class.
     """
 
-    def __init__(self, reqObj=None, exportList=None, verbose=False, log=sys.stderr):
+    def __init__(self, reqObj=None, maxRefAlign=100, verbose=False, log=sys.stderr):
         self.__verbose = verbose
+        self.__debug = False
         self.__reqObj = reqObj
         self.__lfh = log
-        if exportList is None:
-            exportList = []
-        self.__debug = False
-        self.__sessionObj = None
-        self.__sessionPath = "."
+        self.__maxRefAlign = maxRefAlign
         #
-        # This is the setting for all selected sequences to be exported -
-        #
-        self.__summarySeqSelectList = exportList
-        self.__selfRefList = []
+        # placeholders for sequence identifiers picked on the summary page as selected and/or to be aligned.
+        self.__summarySeqAlignList = []
+        self.__summarySeqSelectList = ""
+        #
+        self.__natureSourceTaxIds = {}
+        self.__partRangeErrorMsg = ""
+        self.__sds = None
+
         self.__setup()
 
     def __setup(self):
         try:
             self.__sessionObj = self.__reqObj.getSessionObj()
-            self.__sessionPath = self.__sessionObj.getPath()
-
-            self.__siteId = self.__reqObj.getValue("WWPDB_SITE_ID")
-            self.__identifier = self.__reqObj.getValue("identifier")
-
-            self.__srd = SequenceReferenceData(verbose=self.__verbose, log=self.__lfh)
-
-            self.__pI = PathInfo(siteId=self.__siteId, sessionPath=self.__sessionPath, verbose=self.__verbose, log=self.__lfh)
-            self.__exportFilePathSession = self.__pI.getSequenceAssignmentFilePath(self.__identifier, fileSource="session", versionId="next")
-            if self.__verbose:
-                self.__lfh.write("+SequenceDataExport.__setup() session assignment file path %s\n" % self.__exportFilePathSession)
-            #
+            # self.__sessionPath = self.__sessionObj.getPath()
             self.__sds = SequenceDataStore(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
-            if self.__debug:
-                self.__sds.dump(self.__lfh)
+            self.__sdu = UpdatePolymerEntitySourceDetails(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
             #
-            if not self.__summarySeqSelectList:
-                self.__summarySeqSelectList = self.__sds.getSelectedIds()
+            # Selections coming from the the web request --
             #
-            self.__selfReferenceEntityList = []
-            self.__trueSelfReferenceEntityList = []
-            self.__annoRefDbL = []
-            self.__annoSeqAuthRefMap = {}
-            self.__I = self.__makeExportIndex(self.__summarySeqSelectList)
-            self.__makeSelfReferenceIndex(self.__summarySeqSelectList)
+            # self.__summarySeqAlignList = self.__reqObj.getSummaryAlignList(usingRevAllAlignIds=False)
+            # self.__summarySeqSelectList = self.__reqObj.getSummarySelectList(usingRevSlectIds=False)
+            self.__summarySeqAlignList = str(self.__reqObj.getValue("allalignids")).split(",")
+            self.__summarySeqSelectList = str(self.__reqObj.getValue("selectids")).split(",")
+            self.__updateSelectList()
             if self.__verbose:
-                self.__lfh.write("+SequenceDataExport.__setup() incoming selected id list %r\n" % (self.__summarySeqSelectList))
-                self.__lfh.write("+SequenceDataExport.__setup() self reference list %r\n" % self.__selfReferenceEntityList)
+                self.__lfh.write("+SummaryView.__setup() request input align list  %r\n" % (self.__summarySeqAlignList))
+                self.__lfh.write("+SummaryView._setup()  request input select list %r\n" % (self.__summarySeqSelectList))
             #
-        except:  # noqa: E722 pylint: disable=bare-except
-            self.__lfh.write("+SequenceDataExport.__setup() failed for entry id %s\n" % (self.__identifier))
-            traceback.print_exc(file=self.__lfh)
-        #
-
-    def exportAssignments(self):
-        """Export assign file and associated updated model data file --"""
-        numConflicts = 0
-        conflictList = []
-        try:
-            ok, numConflicts, conflictList, warningMsg = self.__exportSeqMapping()
-            return ok, numConflicts, conflictList, warningMsg
-        except:  # noqa: E722 pylint: disable=bare-except
+            # Reset any newly loaded reference sequence id as it is included above --
+            self.__reqObj.setNewRefId("")
+        except Exception as _e:  # noqa: F841
             if self.__verbose:
-                self.__lfh.write("+SequenceDataExport.exportAssignments() failed for entry id %s\n" % (self.__identifier))
+                self.__lfh.write("+SummaryView.__setup() sessionId %s failed\n" % (self.__sessionObj.getId()))
                 traceback.print_exc(file=self.__lfh)
-            #
-        #
-        return False, numConflicts, conflictList, ""
-
-    def getAllEntityIdList(self):
-        """Interface to get all entity Id list from SequenceDataStore"""
-        return self.__sds.getGroupIds()
 
-    def applyAssignmentsToModel(self):
-        """Create an updated model file in the current session --"""
-        try:
-            #  ----------------
-            # Changes will always be applied to the earliest model in the current session  --
+    def __updateSelectList(self):
+        """ """
+        updatedids = str(self.__reqObj.getValue("updatedids"))
+        if not updatedids:
+            return
+        #
+        updatedList = updatedids.split(",")
+        #
+        entityId = str(self.__reqObj.getValue("activegroupid"))
+        chainIdList = self.__sds.getGroup(entityId)
+        for seqId in self.__summarySeqSelectList:
+            tL = str(seqId).strip().split("_")
+            if len(tL) < 3:
+                continue
             #
-            for v in ["1", "2", "3", "4"]:
-                pdbxPath = self.__pI.getModelPdbxFilePath(self.__identifier, fileSource="session", versionId=v)
-                self.__lfh.write("\n+SequenceDataExport.applyAssignmentsToModel() verifying starting model target path %s\n" % pdbxPath)
-                if os.access(pdbxPath, os.R_OK):
-                    break
-                #
-            #
-            pdbxPathNext = self.__pI.getModelPdbxFilePath(self.__identifier, fileSource="session", versionId="next")
-            logPath = os.path.join(self.__sessionPath, "annot-seqmod-merge.log")
-            if os.access(logPath, os.R_OK):
-                os.remove(logPath)
-            #
-            self.__lfh.write("\n+SequenceDataExport.applyAssignmentsToModel() starting model target path %s\n" % pdbxPath)
-            self.__lfh.write("+SequenceDataExport.applyAssignmentsToModel() model output path %s\n" % pdbxPathNext)
-            self.__lfh.write("+SequenceDataExport.applyAssignmentsToModel() assignment file path %s\n" % self.__exportFilePathSession)
-
-            dp = RcsbDpUtility(tmpPath=self.__sessionPath, siteId=self.__siteId, verbose=self.__verbose, log=self.__lfh)
-            dp.setDebugMode()
-            dp.imp(pdbxPath)
-            dp.addInput(name="seqmod_assign_file_path", value=self.__exportFilePathSession, type="file")
-            dp.op("annot-merge-sequence-data")
-            dp.exp(pdbxPathNext)
-            dp.expLog(logPath)
-            # dp.cleanup()
-            if not os.access(pdbxPathNext, os.R_OK):
-                return False
+            elif (tL[0] in ("selfref", "auth", "ref")) and (tL[1] == entityId):
+                continue
+            elif (tL[0] == "xyz") and (tL[1] in chainIdList):
+                continue
             #
-        except:  # noqa: E722 pylint: disable=bare-except
-            if self.__verbose:
-                self.__lfh.write("+SequenceDataExport.applyAssignmentsToModel() model update failed for assignment file  %s\n" % self.__exportFilePathSession)
-                traceback.print_exc(file=self.__lfh)
-            return False
+            updatedList.append(seqId)
         #
-        return True
+        self.__summarySeqSelectList = updatedList
 
-    def printIt(self):
-        fOut = FormatOut()
-        fOut.autoFormat("Summary Selection List", self.__summarySeqSelectList, 3, 3)
-        fOut.autoFormat("Self Reference List", self.__selfReferenceEntityList, 3, 3)
-        fOut.autoFormat("Selection Index", self.__I, 3, 3)
-        fOut.writeStream(self.__lfh)
-        fOut.clear()
-
-    def __makeExportIndex(self, selectIdList):
-        """Return an index dictionary for the input sequence id list -
-
-        The sequence labels  have the format:
-
-        seqType + "_" + seqInstId + "_" + seqPartId + "_" + seqAltId  + "_" + seqVersion
-
-        or, for the special case of a self reference --
-
-        "selfref"  "_"  entityId  "_"  partId
-        """
-        if self.__verbose:
-            self.__lfh.write("+SequenceDataExport.__makeExportIndex() selected sequence id list %r\n" % selectIdList)
-        #
-        I = Autodict()  # noqa: E741
+    def __finish(self):
         try:
-            for seqId in selectIdList:
-                tup = seqId.strip().split("_")
-                # Skip self reference ids
-                if str(tup[0]).strip() == "selfref":
-                    self.__selfRefList.append(seqId)
-                    continue
-                #
-                I[tup[0]][tup[1]][int(tup[2])] = (int(tup[3]), int(tup[4]))
-            #
-        except:  # noqa: E722 pylint: disable=bare-except
+            # Persist the current summary selection list --
+            self.__reqObj.setSummarySelectList(self.__summarySeqSelectList)
+            self.__reqObj.setSummaryAlignList(self.__summarySeqAlignList)
+            self.__sds.setSelectedIds(idList=self.__summarySeqSelectList)
+            self.__sds.serialize()
+        except Exception as _e:  # noqa: F841
             if self.__verbose:
-                self.__lfh.write("+SequenceDataExport.__makeExportIndex() failed \n")
+                self.__lfh.write("+SummaryView.__finish() sessionId %s failed\n" % (self.__sessionObj.getId()))
                 traceback.print_exc(file=self.__lfh)
-            #
-        #
-        return I
-
-    def __makeSelfReferenceIndex(self, selectIdList):
-        """Return the list self referenced entities for the input sequence id list -
 
-        The sequence labels  have the format:
+    def getEntryDetails(self, kyList=None):
+        if kyList is None:
+            kyList = ["STRUCT_TITLE", "CITATION_TITLE", "PDB_ID"]
+
+        eD = {}
+        for ky in kyList:
+            eD[ky] = self.__sds.getEntryDetail(detailKey=ky)
+        #
+        return eD
+
+    def loadSummary(self, operation="load"):
+        """Create the data structure to populate the HTML pages containing alignment summary --
+
+        Options for operation:
+        + load   - Performs a default selection of the best matching reference sequences then
+                   creates the summary data structure.
+        + reload - reloads current data from the sequence and alignment data stores.
+        """
+        if self.__verbose:
+            self.__lfh.write("+SummaryView.loadSummary() operation %s : sessionId %s\n" % (operation, self.__sessionObj.getId()))
+            self.__lfh.write("+SummaryView.loadSummary() request input align list  %r\n" % (self.__summarySeqAlignList))
+            self.__lfh.write("+SummaryView.loadSummary() request input select list %r\n" % (self.__summarySeqSelectList))
+        if operation == "load":
+            # Using coming from persisted data only here
+            #  -- ignore user selections from web context as these may not exist or may need to be overridden --
+            self.__summarySeqSelectList = self.__sds.getSelectedIds()
+        #
+        self.__summarySeqAlignList = self.__summarySeqSelectList
+
+        self.__sdu.updateAuthEntityDetails(selectIdList=self.__summarySeqSelectList)
+        self.__sds = SequenceDataStore(reqObj=self.__reqObj, verbose=self.__verbose, log=self.__lfh)
+        return self.__loadSummary(op=operation)
 
-        seqType + "_" + seqInstId + "_" + seqPartId + "_" + seqAltId  + "_" + seqVersion
+    def getGroupIdList(self):
+        return self.__sds.getGroupIds()
 
-        or, for the special case of a self reference --
+    def __loadSummary(self, op="load"):
+        """Assemble the data for sequence summary view using current contents of the session sequence data store.
 
-        "selfref"  "_"  entityId  "_"  partId
+        Returns:  summaryDataObj [<entity/groupId>]  ['auth'|'xyz'] ->  {data dict}
+                                                     ['ref']        -> [(partId,{data dict}),(partId,{data dict}),...]
+                               {data dict}  with keys
+
+                               dT['ROW_IDS']       =rowIdList
+                               dT['ROW_STATUS']    =rowStatusList
+                               dT['ROW_DATA_DICT'] =rowDataDictList
+                               dT['SELF_REFERENCE_FLAG']=Boolean
         """
-        if self.__verbose:
-            self.__lfh.write("+SequenceDataExport.__makeSelfReferenceIndex() selected sequence id list %r\n" % selectIdList)
-        #
-        try:
-            for seqId in selectIdList:
-                tup = seqId.strip().split("_")
-                if str(tup[0]).strip() == "selfref":
-                    if self.__verbose:
-                        self.__lfh.write("+SequenceDataExport.__makeSelfReferenceIndex() - assigning reference for sequence entity %s part %s (%s)\n" % (tup[1], tup[2], tup[0]))
-                    #
-                    seqId = str(tup[1]).strip()
-                    partId = str(tup[2]).strip()
-                    self.__selfReferenceEntityList.append((seqId, partId))
-                    foundAnnInputRefInfo = False
-                    if (seqId in self.__I["auth"]) and (int(partId) in self.__I["auth"][seqId]):
-                        altId = self.__I["auth"][seqId][int(partId)][0]
-                        verId = self.__I["auth"][seqId][int(partId)][1]
-                        seqAuthFD = self.__sds.getFeature(seqId=seqId, seqType="auth", partId=int(partId), altId=altId, version=verId)
-                        row = []
-                        row.append(len(self.__annoRefDbL) + 1)
-                        row.append(seqId)
-                        for item in ("ANNO_EDIT_DB_NAME", "ANNO_EDIT_DB_CODE", "ANNO_EDIT_DB_ACCESSION", "ANNO_EDIT_DB_ALIGN_BEGIN", "ANNO_EDIT_DB_ALIGN_END"):
-                            if (item in seqAuthFD) and seqAuthFD[item]:
-                                row.append(seqAuthFD[item])
-                            else:
-                                break
-                            #
-                        #
-                        if len(row) == 7:
-                            seqAuthRefMap = []
-                            if (seqId in self.__annoSeqAuthRefMap) and self.__annoSeqAuthRefMap[seqId]:
-                                seqAuthRefMap = self.__annoSeqAuthRefMap[seqId]
-                            else:
-                                seqAuthIdx = self.__sds.getSequence(seqId=seqId, seqType="auth", partId=int(partId), altId=altId, version=verId)
-                                idx = 1
-                                for seqAuth in seqAuthIdx:
-                                    seqAuthRefMap.append([".", seqId, seqAuth[0], str(idx), seqId, ".", ".", "."])
-                                    idx += 1
-                                #
-                            #
-                            if seqAuthRefMap:
-                                authFObj = self.__sds.getFeatureObj(seqId, "auth", partId=int(partId), altId=altId, version=verId)
-                                _authPartId, authSeqBeg, authSeqEnd, _authSeqPartType = authFObj.getAuthPartDetails()
-                                partBeg = int(authSeqBeg)
-                                partEnd = int(authSeqEnd)
-                                foundMap = False
-                                startNum = int(row[5])
-                                for seqAuth in seqAuthRefMap:
-                                    idx = int(seqAuth[3])
-                                    if (idx >= partBeg) and (idx <= partEnd):
-                                        if idx > partBeg:
-                                            startNum += 1
-                                        #
-                                        seqAuth[5] = seqAuth[2]
-                                        seqAuth[6] = str(startNum)
-                                        seqAuth[7] = str(partId)
-                                        foundMap = True
-                                    #
-                                #
-                                if foundMap:
-                                    row.append(partId)
-                                    self.__annoRefDbL.append(row)
-                                    foundAnnInputRefInfo = True
-                                    self.__annoSeqAuthRefMap[seqId] = seqAuthRefMap
-                                #
-                            #
-                        #
-                    #
-                    if not foundAnnInputRefInfo:
-                        self.__trueSelfReferenceEntityList.append((seqId, partId))
-                    #
-                #
-            #
-        except:  # noqa: E722 pylint: disable=bare-except
-            if self.__verbose:
-                self.__lfh.write("+SequenceDataExport.__makeSelfReferenceIndex() failed \n")
-                traceback.print_exc(file=self.__lfh)
-            #
         #
+        if self.__verbose:
+            self.__lfh.write("+SummaryView.__loadSummary() with sessionId %s\n" % self.__sessionObj.getId())
 
-    def __exportSeqMapping(self):
-        """Export worker function -"""
         #
-        # Get entry ids
-        depDataSetId = self.__sds.getEntryDetail("DEPOSITION_DATA_SET_ID")
-        # pdbId = self.__sds.getEntryDetail("PDB_ID")
-        #
-        # Get the entity group list -
+        summaryDataObj = {}
+
         gIdList = self.__sds.getGroupIds()
-        if len(gIdList) < 1:
-            if self.__verbose:
-                self.__lfh.write("+SequenceDataExport.__exportSeqMapping() for data set %s group list is empty\n" % depDataSetId)
-            #
-        #
+
         if self.__verbose:
-            self.__lfh.write("+SequenceDataExport.__exportSeqMapping() number of groups %d depDataSetId %s\n" % (len(gIdList), depDataSetId))
+            self.__lfh.write("+SummaryView.__loadSummary() group list is %r\n" % gIdList)
+            self.__lfh.write("+SummaryView.__loadSummary() starting selection list %r\n" % self.__summarySeqSelectList)
+            self.__lfh.write("+SummaryView.__loadSummary() starting alignment list %r\n" % self.__summarySeqAlignList)
         #
 
-        seqLabel = SequenceLabel()
-        refFeatureD = {}
-        rptRefL = []
-        rptXyzL = []
-        rptCommentL = []
-        rptCommentModL = []
-        rptDeleteL = []
-        allRefSeqIdxD = {}
-        numConflicts = 0
-        conflictList = []
-        warningMsg = ""
-        natureSourceTaxIds = {}
-        #
         polyAlaCaseList = []
         for gId in gIdList:
             #
-            # Get seqIds in group -
-            #
-            seqIdList = self.__sds.getGroup(gId)
-            if len(seqIdList) < 1:
-                if self.__verbose:
-                    self.__lfh.write("+SequenceDataExport.__exportSeqMapping() skipping entity group %s which has no instances\n" % (gId))
-                #
-                continue
-            #
-            if self.__verbose:
-                self.__lfh.write("+SequenceDataExport.__exportSeqMapping() group %s sequence list %r\n" % (gId, seqIdList))
-            #
-            # Author sequence -
-            #
-            sourceInfo = ""
-            idAuthSeq = ""
-            first = True
-            if gId in self.__I["auth"]:
-                if self.__verbose:
-                    self.__lfh.write("+SequenceDataExport.__exportSeqMapping() entity group %s author sequence s list %r\n" % (gId, list(self.__I["auth"][gId].items())))
-                #
-                for partId, (altId, ver) in self.__I["auth"][gId].items():
-                    fD = self.__sds.getFeature(gId, seqType="auth", partId=partId, altId=altId, version=ver)
-                    if ("SOURCE_METHOD" in fD) and fD["SOURCE_METHOD"].upper() == "NAT":
-                        sourceInfo = "NAT"
-                        if ("SOURCE_TAXID" in fD) and fD["SOURCE_TAXID"]:
-                            if fD["SOURCE_TAXID"] in natureSourceTaxIds:
-                                if gId not in natureSourceTaxIds[fD["SOURCE_TAXID"]]:
-                                    natureSourceTaxIds[fD["SOURCE_TAXID"]].append(gId)
-                                #
-                            else:
-                                natureSourceTaxIds[fD["SOURCE_TAXID"]] = [gId]
-                            #
-                        #
-                    #
-                    seqLabel.set(seqType="auth", seqInstId=gId, seqPartId=partId, seqAltId=altId, seqVersion=ver)
-                    idAuthSeq = seqLabel.pack()
-                    if self.__verbose:
-                        self.__lfh.write("+SequenceDataExport.__exportSeqMapping() from entity group %s exporting author sequence %s\n" % (gId, idAuthSeq))
-                    #
-                    if first and ("POLYMER_TYPE" in fD) and (fD["POLYMER_TYPE"] == "AA"):
-                        seqAuth = self.__sds.getSequence(seqId=gId, seqType="auth", partId=partId, altId=altId, version=ver)
-                        polyALA_assignment = self.__checkPolyAlaAssignment(seqAuth)
-                        if polyALA_assignment > 0:
-                            polyAlaCaseList.append((gId, polyALA_assignment))
-                        #
-                    #
-                    first = False
-                #
-            #
-            if not idAuthSeq:
-                # report missing author sequence
-                if self.__verbose:
-                    self.__lfh.write("+SequenceDataExport.__exportSeqMapping() missing author sequence from entity group %s\n" % gId)
-                #
-                continue
-            #
-            # Reference sequences -
-            #
-            idListRef = []
-            if gId in self.__I["ref"]:
-                for partId, (altId, ver) in self.__I["ref"][gId].items():
-                    seqRefIdx = self.__sds.getSequence(seqId=gId, seqType="ref", partId=partId, altId=altId, version=ver)
-                    seqRefFD = self.__sds.getFeature(seqId=gId, seqType="ref", partId=partId, altId=altId, version=ver)
-                    seqLabel.set(seqType="ref", seqInstId=gId, seqPartId=partId, seqAltId=altId, seqVersion=ver)
-                    idRefSeq = seqLabel.pack()
-                    idListRef.append(idRefSeq)
-                    #
-                    refFeatureD[(gId, partId)] = (idRefSeq, altId, seqRefFD, partId)
-                    allRefSeqIdxD[idRefSeq] = seqRefIdx
-                    #
-                    if self.__verbose:
-                        self.__lfh.write("+SequenceDataExport.__exportSeqMapping() from entity group %s part %s exporting reference sequence %s\n" % (gId, partId, idRefSeq))
-                    #
-                #
-            else:
-                # report missing reference sequence
-                if self.__verbose:
-                    self.__lfh.write("+SequenceDataExport.__exportSeqMapping() missing reference sequence from group %s\n" % gId)
-                #
-            #
-            # Coordinate sequences -
-            #
-            idListXyz = []
-            for seqId in seqIdList:
-                if seqId in self.__I["xyz"]:
-                    for partId, (altId, ver) in self.__I["xyz"][seqId].items():
-                        seqLabel.set(seqType="xyz", seqInstId=seqId, seqPartId=partId, seqAltId=altId, seqVersion=ver)
-                        idXyzSeq = seqLabel.pack()
-                        idListXyz.append(idXyzSeq)
-                    #
-                else:
-                    # report missing coordinate sequence
-                    pass
-                #
-            #
-            if (len(idListRef) < 1) and (len(idListXyz) < 1):
-                continue
-            #
-            alignExport = AlignmentExport(reqObj=self.__reqObj, entityId=gId, pathInfo=self.__pI, seqDataStore=self.__sds, verbose=self.__verbose, log=self.__lfh)
-            localRptRefL, localRptCommentL, localRptCommentModL, localRptDeleteL, localRptXyzL, message, numC = alignExport.doExport(
-                idAuthSeq, idListRef, idListXyz, self.__selfRefList, sourceInfo
-            )
-            if self.__verbose:
-                errMsg = alignExport.getErrorMessage()
-                if errMsg:
-                    self.__lfh.write("\nError message for entity '%s'\n%s\n" % (gId, errMsg))
-                #
-            #
-            if len(localRptRefL) > 0:
-                rptRefL.extend(localRptRefL)
+            summaryDataObj[gId] = {}
             #
-            if len(localRptCommentL) > 0:
-                rptCommentL.extend(localRptCommentL)
+            dT, polyALA_assignment = self.__buildAuthSection(groupId=gId, op=op)
+            if polyALA_assignment > 0:
+                polyAlaCaseList.append((gId, polyALA_assignment))
             #
-            if len(localRptCommentModL) > 0:
-                rptCommentModL.extend(localRptCommentModL)
-            #
-            if len(localRptDeleteL) > 0:
-                rptDeleteL.extend(localRptDeleteL)
-            #
-            if len(localRptXyzL) > 0:
-                rptXyzL.extend(localRptXyzL)
-            #
-            if message:
-                warningMsg += message
-            #
-            if numC > 0:
-                numConflicts += numC
-                conflictList.append((gId, numC))
-            #
-        #  END of iteration over  --- gId  ----
+            summaryDataObj[gId]["auth"] = dT
+
+            rL = self.__buildReferenceSection(groupId=gId)
+            summaryDataObj[gId]["ref"] = rL
+
+            summaryDataObj[gId]["xyz"] = self.__buildCoordinateSection(groupId=gId)
         #
-        if len(natureSourceTaxIds) > 1:
+        self.__finish()
+        #
+        warningMsg = ""
+        if len(self.__natureSourceTaxIds) > 1:
             warningMsg += "Entry contains multiple natural sources:<br />\n"
-            for k, v in natureSourceTaxIds.items():
+            for k, v in self.__natureSourceTaxIds.items():
                 if len(v) > 1:
                     warningMsg += "Entities '" + "', '".join(v) + "' have "
                 else:
                     warningMsg += "Entity '" + "', '".join(v) + "' has "
                 #
                 warningMsg += "source taxonomy Id '" + k + "'.<br />\n"
             #
         #
+        if self.__partRangeErrorMsg != "":
+            if warningMsg:
+                warningMsg += "<br />\n"
+            #
+            warningMsg += "Part range errors:<br />\n" + self.__partRangeErrorMsg
+        #
         if polyAlaCaseList:
             for polyAlaCaseTupL in polyAlaCaseList:
                 if warningMsg:
                     warningMsg += "<br />\n"
                 #
                 warningMsg += "Entity [" + polyAlaCaseTupL[0] + "]"
                 if polyAlaCaseTupL[1] == 1:
                     warningMsg += " is composed only of poly-ALA.<br />\n"
                 else:
                     warningMsg += " has stretches of poly-ALA.<br />\n"
                 #
             #
-        # ref FeatureD ---
-        rptRefDbL = self.__refDdReport(refFeatureD)
-        # rptDeleteL = self.__deletionReport(refFeatureD, allRefSeqIdxD)
+        #
+        return summaryDataObj, warningMsg
 
-        try:
-            # Make a local copy of the mapping file in the session directory and then copy the file as needed.
+    def __buildAuthSection(self, groupId=None, op="load"):
+        """Assemble the data content for the author sequence summary view.
+
+        Returns: summaryDataObject)
+
+        ** Always show a single full sequence for each entity and store multi-part information as details
+
+        """
+
+        seqLabel = SequenceLabel()
+
+        rowIdList = []
+        rowStatusList = []
+        rowDataDictList = []
+        #
+        # Each author entity sequence is shown once and is labeled by its first instance in the group.
+        #
+        seqId0 = groupId
+
+        if self.__verbose:
+            self.__lfh.write("SummaryView.__buildAuthSection() groupId %r op %s \n" % (groupId, op))
+        #
+        altId = 1
+        partIdList = self.__sds.getPartIds(seqId0, dataType="sequence", seqType="auth")
+        partId0 = partIdList[0]
+        detailsD = self.__getAuthFeaturesAll(groupId, seqId0, partIdList)
+
+        verList = self.__sds.getVersionIds(seqId0, partId=partId0, altId=altId, dataType="sequence", seqType="auth")
+
+        first = True
+        polyALA_assignment = 0
+        for ver in verList:
+            seqAuth = self.__sds.getSequence(seqId=seqId0, seqType="auth", partId=partId0, altId=altId, version=ver)
+            if first:
+                authFObj = self.__sds.getFeatureObj(seqId0, "auth", partId=partId0, altId=altId, version=ver)
+                polymerTypeCode = authFObj.getPolymerType()
+                if polymerTypeCode == "AA":
+                    polyALA_assignment = self.__checkPolyAlaAssignment(seqAuth)
+                #
+            #
+            seqLabel.set(seqType="auth", seqInstId=seqId0, seqPartId=partId0, seqAltId=altId, seqVersion=ver)
+            seqAuthId = seqLabel.pack()
+            rowIdList.append(seqAuthId)
+            #
+            isSelected = seqAuthId in self.__summarySeqSelectList
+            isAligned = seqAuthId in self.__summarySeqAlignList
+            #
             #
-            blockList = []
-            ofh = open(self.__exportFilePathSession, "w")
-            dataBlock = DataContainer(depDataSetId)
-            if len(self.__trueSelfReferenceEntityList) > 0:
-                dataBlock.append(self.__cifCatSelfReference(self.__trueSelfReferenceEntityList))
-            #
-            if len(rptRefDbL) > 0:
-                dataBlock.append(
-                    self.__writeGeneralCifCategory(
-                        "pdbx_seqtool_db_ref", ("ordinal", "entity_id", "db_name", "db_code", "db_accession", "db_isoform", "match_begin", "match_end", "entity_part_id"), rptRefDbL
-                    )
-                )
-            #
-            if len(self.__annoRefDbL) > 0:
-                dataBlock.append(
-                    self.__writeGeneralCifCategory(
-                        "pdbx_seqtool_anno_db_ref", ("ordinal", "entity_id", "db_name", "db_code", "db_accession", "match_begin", "match_end", "entity_part_id"), self.__annoRefDbL
-                    )
-                )
-                #
-                for k, seqAuthRefMap in self.__annoSeqAuthRefMap.items():
-                    for seqAuth in seqAuthRefMap:
-                        seqAuth[0] = str(len(rptRefL) + 1)
-                        rptRefL.append(tuple(seqAuth))
+            # if op == 'reload':
+            #     isSelected = (ver == max(verList))
+            #     isAligned = (ver == max(verList))
+            # #
+            #
+            rowStatusList.append((isSelected, isAligned))
+            #
+            rowDataDict = {}
+            rowDataDict["ROW_VERSION"] = ver
+            rowDataDict["ROW_SEQ_LENGTH"] = len(seqAuth)
+            rowDataDict["ROW_DETAIL_STRING"] = ""
+            rowDataDict.update(detailsD[ver])
+            rowDataDictList.append(rowDataDict)
+            first = False
+        #
+        dT = {}
+        dT["ROW_IDS"] = rowIdList
+        dT["ROW_STATUS"] = rowStatusList
+        dT["ROW_DATA_DICT"] = rowDataDictList
+        dT["ENTITY_NUM_PARTS"] = len(partIdList)
+        #
+        return dT, polyALA_assignment
+
+    def __buildCoordinateSection(self, groupId=None):
+        """Assemble the data content for the coordinate sequence summary view.
+
+        Returns: summaryDataObject
+
+        """
+        seqLabel = SequenceLabel()
+        seqFeature = SequenceFeature()
+
+        #
+        # For each coordinate sequence -
+        #
+        seqIdList = self.__sds.getGroup(groupId)
+
+        rowIdList = []
+        rowStatusList = []
+        rowDataDictList = []
+        #
+        partId = 1
+        altId = 1
+        for seqId in seqIdList:
+            verList = self.__sds.getVersionIds(seqId=seqId, partId=partId, altId=altId, dataType="sequence", seqType="xyz")
+            if len(verList) < 1:
+                continue
+            maxVrsnNum = verList[0]
+            seqLabel.set(seqType="xyz", seqInstId=seqId, seqPartId=partId, seqAltId=altId, seqVersion=maxVrsnNum)
+            maxSeqXyzId = seqLabel.pack()
+
+            # select the highest version sequence
+            if not (maxSeqXyzId in self.__summarySeqSelectList):
+                self.__summarySeqSelectList.append(maxSeqXyzId)
+                self.__summarySeqAlignList.append(maxSeqXyzId)
+
+            for ver in verList:
+                seqXyz = self.__sds.getSequence(seqId, "xyz", partId=partId, altId=altId, version=ver)
+                seqXyzFD = self.__sds.getFeature(seqId, "xyz", partId=partId, altId=altId, version=ver)
+                seqLabel.set(seqType="xyz", seqInstId=seqId, seqPartId=partId, seqAltId=altId, seqVersion=ver)
+                seqXyzId = seqLabel.pack()
+                #
+                seqFeature.set(seqXyzFD)
+                sfd = SequenceFeatureDepict(sfObj=seqFeature, verbose=self.__verbose, log=self.__lfh)
+                detailString = sfd.markupXyzFeatures()
+                #
+                rowLabel = seqId
+                rowIdList.append(seqXyzId)
+                #
+                # unselect any selected lower version for this sequence -
+                if (ver < maxVrsnNum) and (seqXyzId in self.__summarySeqSelectList):
+                    self.__summarySeqSelectList.remove(seqXyzId)
+                    if seqXyzId in self.__summarySeqAlignList:
+                        self.__summarySeqAlignList.remove(seqXyzId)
+                #
+                isSelected = seqXyzId in self.__summarySeqSelectList
+                isAligned = seqXyzId in self.__summarySeqAlignList
+                # JDW add instance here to provide a selection group
+                if ver == maxVrsnNum:
+                    rowStatusList.append((isSelected, isAligned, seqId, "maxver"))
+                else:
+                    rowStatusList.append((isSelected, isAligned, seqId, ""))
+                #
+                rowDataDict = {}
+                rowDataDict["ROW_ID_CODE"] = rowLabel
+                rowDataDict["ROW_VERSION"] = ver
+                rowDataDict["ROW_SEQ_LENGTH"] = len(seqXyz)
+                rowDataDict["ROW_DETAIL_STRING"] = detailString
+                rowDataDict.update(seqXyzFD)
+                rowDataDictList.append(rowDataDict)
+        #
+        dT = {}
+        dT["ROW_IDS"] = rowIdList
+        dT["ROW_STATUS"] = rowStatusList
+        dT["ROW_DATA_DICT"] = rowDataDictList
+        return dT
+
+    def __buildReferenceSection(self, groupId=None):
+        """Assemble the data content for the reference sequence summary view.
+
+        Returns: [(partId,summaryDataObject),]
+
+               where:
+                  partId is the integer identifier for pieces of a multipart entity sequence
+                  summaryDataObject contains the 'ref' sequence summary data for the input groupId.
+        """
+        rL = []
+        seqLabel = SequenceLabel()
+        seqFeature = SequenceFeature()
+        #
+        # use the leading sequence Id in the group as the id for the reference -
+        #
+        seqIdRef = groupId
+        #
+        partInfoList = []
+        partIdList = self.__sds.getPartIds(seqIdRef, dataType="sequence", seqType="auth")
+        for partId in partIdList:
+            #
+            authVerList = self.__sds.getVersionIds(seqId=seqIdRef, partId=partId, altId=1, dataType="feature", seqType="auth")
+            # Changed to original tax ID ( DAOTHER-6126 )
+            OrigTaxId = ""
+            skipPart = False
+            if len(authVerList) > 0:
+                authFObj = self.__sds.getFeatureObj(seqIdRef, "auth", partId=partId, altId=1, version=authVerList[0])
+                sourceInfo = authFObj.getEntitySourceMethod().upper()
+                OrigTaxId = authFObj.getSourceTaxIdOrig()
+                TaxId = authFObj.getSourceTaxId()
+                if (sourceInfo == "NAT") and TaxId:
+                    if TaxId in self.__natureSourceTaxIds:
+                        self.__natureSourceTaxIds[TaxId].append(groupId)
+                    else:
+                        self.__natureSourceTaxIds[TaxId] = [groupId]
                     #
                 #
+                authPartId, authSeqBeg, authSeqEnd, authSeqPartType = authFObj.getAuthPartDetails()
+                partInfoList.append((authPartId, authSeqBeg, authSeqEnd))
+                skipPart = len(authSeqPartType) > 1 and authSeqPartType.lower() != "biological sequence"
             #
-            dataBlock.append(self.__getEntitySourceCategory())
+            if skipPart:
+                self.__lfh.write("+SummaryView.__buildReferenceSection() entity %s skipping part %s type %s\n" % (groupId, partId, authSeqPartType))
+                continue
             #
-            if len(rptCommentL) > 0:
-                dataBlock.append(
-                    self.__writeGeneralCifCategory("pdbx_seqtool_mapping_comment", ("ordinal", "entity_id", "entity_mon_id", "entity_seq_num", "comment"), rptCommentL)
-                )
-            #
-            if len(rptCommentModL) > 0:
-                dataBlock.append(
-                    self.__writeGeneralCifCategory(
-                        "pdbx_seqtool_mapping_modification_comment", ("ordinal", "entity_id", "entity_mon_id", "entity_seq_num", "comment"), rptCommentModL
-                    )
-                )
-            #
-            if len(rptDeleteL) > 0:
-                dataBlock.append(
-                    self.__writeGeneralCifCategory(
-                        "pdbx_seqtool_ref_deletions", ("ordinal", "entity_id", "part_id", "db_name", "db_accession", "db_isoform", "ref_mon_id", "ref_mon_num"), rptDeleteL
-                    )
-                )
-            #
-            if len(rptRefL) > 0:
-                dataBlock.append(
-                    self.__writeGeneralCifCategory(
-                        "pdbx_seqtool_mapping_ref",
-                        ("ordinal", "entity_id", "entity_mon_id", "entity_seq_num", "auth_asym_id", "ref_mon_id", "ref_mon_num", "entity_part_id"),
-                        rptRefL,
-                    )
-                )
-            #
-            if len(rptXyzL) > 0:
-                dataBlock.append(
-                    self.__writeGeneralCifCategory(
-                        "pdbx_seqtool_mapping_xyz",
-                        ("ordinal", "entity_id", "entity_mon_id", "entity_seq_num", "auth_asym_id", "pdb_mon_id", "pdb_mon_num", "pdb_ins_code", "hetero_flag", "org_mon_id"),
-                        rptXyzL,
-                    )
-                )
-            #
-            blockList.append(dataBlock)
-            pdbxW = PdbxWriter(ofh)
-            pdbxW.write(blockList)
-            ofh.close()
-        except:  # noqa: E722 pylint: disable=bare-except
-            if self.__verbose:
-                self.__lfh.write("+SequenceDataExport.__exportSeqMapping() saving export mapping file failed %s\n" % self.__exportFilePathSession)
-                traceback.print_exc(file=self.__lfh)
-            return False, numConflicts, conflictList, warningMsg
+            rowIdList = []
+            rowStatusList = []
+            rowDataDictList = []
+            # List of reference sequences for this group only for the leading sequence -
+            #
+            altIdList = self.__sds.getAlternativeIds(seqIdRef, dataType="sequence", seqType="ref", partId=partId)
+
+            srId = "selfref_" + str(groupId) + "_" + str(partId)
+            if srId in self.__summarySeqSelectList:
+                if self.__verbose:
+                    self.__lfh.write("+SummaryView.__buildReferenceSection() using self-refereence for entity %s part %s\n" % (groupId, partId))
+                selfRefFlag = True
+            else:
+                selfRefFlag = False
+            #
+            for altId in altIdList[: self.__maxRefAlign]:
+                #
+                verList = self.__sds.getVersionIds(seqId=seqIdRef, partId=partId, altId=altId, dataType="sequence", seqType="ref")
+                for ver in verList:
+                    #
+                    seqRefFD = self.__sds.getFeature(seqIdRef, "ref", partId=partId, altId=altId, version=ver)
+                    seqFeature.set(seqRefFD)
+                    seqLabel.set(seqType="ref", seqInstId=seqIdRef, seqPartId=partId, seqAltId=altId, seqVersion=ver)
+                    seqRefId = seqLabel.pack()
+                    #
+                    taxIdWarningFlag = False
+                    RefTaxId = seqFeature.getSourceTaxId()
+                    if OrigTaxId and RefTaxId and (OrigTaxId != RefTaxId):
+                        taxIdWarningFlag = True
+                    #
+                    isSelected = seqRefId in self.__summarySeqSelectList
+                    isAligned = seqRefId in self.__summarySeqAlignList
+                    rowStatusList.append((isSelected, isAligned))
+                    #
+                    sfd = SequenceFeatureDepict(sfObj=seqFeature, verbose=self.__verbose, log=self.__lfh)
+                    detailString = sfd.markupReferenceAlignmentFeatures()
+                    featureString = sfd.markupReferenceFeatures()
+                    rowLabel = sfd.markupDatabaseReferenceWithUrl(altId)
+                    rowIdList.append(seqRefId)
+
+                    lengthRefSeq = seqFeature.getMatchLength()
+                    # authSimWithGaps = seqFeature.getAuthRefSimWithGaps()
+                    #
+                    #
+                    rowDataDict = {}
+                    rowDataDict["ROW_ID_CODE"] = rowLabel
+                    rowDataDict["ROW_VERSION"] = ver
+                    rowDataDict["ROW_SEQ_LENGTH"] = lengthRefSeq
+                    # rowDataDict['ROW_AUTH_REF_SIM'] = "%.3f" % authSimWithGaps
+                    rowDataDict["ROW_AUTH_REF_SIM"] = sfd.markupReferenceSimilarttFeatures()
+                    rowDataDict["ROW_DETAIL_STRING"] = detailString
+                    rowDataDict["ROW_FEATURE_STRING"] = featureString
+                    rowDataDict["ROW_IS_SELECTED"] = isSelected
+                    rowDataDict["ROW_IS_ALIGNED"] = isAligned
+                    # rowDataDict.update(seqRefFD)
+                    for key, _val in seqRefFD.items():
+                        if (key == "SOURCE_TAXID") and taxIdWarningFlag:
+                            rowDataDict[key] = '<span style="color:red">' + seqRefFD[key] + "</span>"
+                        else:
+                            rowDataDict[key] = seqRefFD[key]
+                        #
+                    #
+                    rowDataDictList.append(rowDataDict)
+            #
+            dT = {}
+            dT["ROW_IDS"] = rowIdList
+            dT["ROW_STATUS"] = rowStatusList
+            dT["ROW_DATA_DICT"] = rowDataDictList
+            dT["SELF_REFERENCE_FLAG"] = selfRefFlag
+            rL.append((partId, dT))
+        #
+        self.__checkPartRange(groupId, partInfoList)
+        #
+        return rL
+
+    def __getAuthFeaturesAll(self, entityId, seqId0, partIdList):
+        """Consolidate the feature data for the author sequences entity sequence respecting
+        potential mutiple source details.
+
+        Original and current features are assembled.
+
+        Returns a dictionaries of features for each sequence version.
+
+        Details[ver][partId]['current']={'partdetails','sourceAndStrain','description','hostorg'}
+        Details[ver][partId]['author']={'partdetails','sourceAndStrain','description','hostorg'}
+        """
+        if self.__verbose:
+            self.__lfh.write("+SummaryView.__getAuthFeaturesAll() entityId %r seqId0 %r partIdList %r\n" % (entityId, seqId0, partIdList))
+
+        #
+        authRefAssignText = self.__markupAuthorAssignments(entityId)
+        #
+        #
+        altId = 1
+        detailsD = {}
+        for partId in partIdList:
+            verList = self.__sds.getVersionIds(seqId0, partId=partId, altId=altId, dataType="sequence", seqType="auth")
+            for ver in verList:
+                if ver not in detailsD:
+                    detailsD[ver] = {}
+
+                sfObj = self.__sds.getFeatureObj(seqId=seqId0, seqType="auth", partId=partId, altId=altId, version=ver)
+                sfd = SequenceFeatureDepict(sfObj=sfObj, verbose=self.__verbose, log=self.__lfh)
 
-        return True, numConflicts, conflictList, warningMsg
+                if partId not in detailsD[ver]:
+                    detailsD[ver][partId] = {}
+
+                detailsD[ver][partId]["current"] = sfd.markupCurrentEntityDetails()
+                detailsD[ver][partId]["author"] = sfd.markupAuthorEntityDetails()
+
+                if len(authRefAssignText) > 0:
+                    detailsD[ver][partId]["author"]["description"] += authRefAssignText
+
+        for ver in detailsD.keys():
+            np = 0
+            for partId in partIdList:
+                if partId in detailsD[ver]:
+                    np += 1
+            detailsD[ver]["numparts"] = np
+        if self.__debug:
+            self.__lfh.write("+SummaryView.__getAuthFeaturesAll() detailsD entity %r seqId %r partIdList %r\n" % (entityId, seqId0, partIdList))
+            fOut = FormatOut()
+            fOut.autoFormat("Summary Entity Details", detailsD, 3, 3)
+            fOut.writeStream(self.__lfh)
+            fOut.clear()
+        #
+        return detailsD
 
     def __checkPolyAlaAssignment(self, seqAuth):
         """Check if the sequence contains 10 or more consecutive ALA residues"""
         has_consecutive_ALA = False
         count = 0
         for seqTupL in seqAuth:
             if seqTupL[0] == "ALA":
@@ -611,182 +588,106 @@
         if count == len(seqAuth):
             return 1
         elif has_consecutive_ALA:
             return 2
         #
         return 0
 
-    def __refDdReport(self, refFeatureD):
-        """Return a list of content rows for reference sequence database accession report --"""
-        rptRefDbL = []
-        irow = 1
-        for (gId, partId), tup in refFeatureD.items():
-            if (str(gId), str(partId)) in self.__selfReferenceEntityList:
-                continue
-            #
-            # sId = tup[0]
-            fD = tup[2]
-            rptRefDbL.append(
-                [
-                    irow,
-                    gId,
-                    self.__srd.convertDbNameToResource(fD["DB_NAME"]),
-                    fD["DB_CODE"],
-                    fD["DB_ACCESSION"],
-                    fD["DB_ISOFORM"],
-                    fD["REF_MATCH_BEGIN"],
-                    fD["REF_MATCH_END"],
-                    partId,
-                ]
-            )
-            irow += 1
-        #
-        return rptRefDbL
-
-    # def __deletionReport(self, refFeatureD, allRefSeqIdxD):
-    #     """Return a list of content rows for the sequence deletion report."""
-    #     rptDeleteL = []
-    #     idel = 1
-    #     for (gId, partId), tup in refFeatureD.items():
-    #         if (str(gId), str(partId)) in self.__selfReferenceEntityList:
-    #             continue
-    #         #
-    #         sId = tup[0]
-    #         fD = tup[2]
-    #         if sId in allRefSeqIdxD:
-    #             if self.__verbose:
-    #                 self.__lfh.write("+SequenceDataExport.__exportSeqMapping() searching deletions in seqId %s\n" % sId)
-    #             #
-    #             refSeqIdx = allRefSeqIdxD[sId]
-    #             for sTup in refSeqIdx:
-    #                 if sTup[2] in ["Deletion", "deletion"]:
-    #                     if self.__verbose:
-    #                         self.__lfh.write("+SequenceDataExport.__exportSeqMapping() position %s comment %s\n" % (sTup[1], sTup[2]))
-    #                     #
-    #                     rptDeleteL.append([idel, gId, partId, self.__srd.convertDbNameToResource(fD["DB_NAME"]), fD["DB_ACCESSION"], fD["DB_ISOFORM"], sTup[0], sTup[1]])
-    #                     idel += 1
-    #                 #
-    #             #
-    #         else:
-    #             self.__lfh.write("+SequenceDataExport.__exportSeqMapping() delete scan missing reference sequence for seqId %s keys() %r\n" % (sId, allRefSeqIdxD.keys()))
-    #         #
-    #     #
-    #     return rptDeleteL
-
-    def __cifCatSelfReference(self, entityList):
-        """Update entities for self reference  ---"""
-        aCat = DataCategory("pdbx_seqtool_self_ref")
-        aCat.appendAttribute("entity_id")
-        aCat.appendAttribute("entity_part_id")
-        for eid, partId in entityList:
-            aCat.append([eid, partId])
-        return aCat
-
-    def __writeGeneralCifCategory(self, categoryName, categoryItems, dataList):
-        """Write pdbx_seqtool_db_ref, pdbx_seqtool_anno_db_ref, pdbx_seqtool_ref_deletions, pdbx_seqtool_mapping_ref, pdbx_seqtool_mapping_comment,
-        pdbx_seqtool_mapping_modification_comment, pdbx_seqtool_mapping_xyz categories
-        """
-        if len(dataList) < 1:
-            return None
+    def __markupAuthorAssignments(self, entityId):
+        """Markup the author provided reference assignments -"""
+        spStr = "<br />"
+        authRefAssignText = ""
+        depSeqAssignD = self.__sds.getDepositorReferenceAssignments()
+        sADep = SequenceAssignDepositor(verbose=self.__verbose, log=self.__lfh)
+        sADep.set(depSeqAssignD)
+        refSeqAssignL = sADep.getReferenceList(entityId)
+
+        if self.__debug:
+            self.__lfh.write("+SummaryView.__markupAuthorAssignments() for entityId %r author reference count is %d\n" % (entityId, sADep.getReferenceCount(entityId)))
+            sADep.printIt(log=self.__lfh)
+            for ii, rsa in enumerate(refSeqAssignL):
+                self.__lfh.write("+SummaryView.__markupAuthorAssignments() depositor reference  %d\n" % (ii + 1))
+                rsa.printIt(self.__lfh)
+        #
+
+        for rsa in refSeqAssignL:
+            dbName, dbCode, dbAccession = rsa.getDbReference()
+            if (len(dbAccession) > 0 and (dbAccession not in [".", "?"])) or (len(dbCode) > 0 and (dbCode not in [".", "?"])):
+                tRef = "Depositor reference: %s %s %s" % (dbName, dbAccession, dbCode)
+                sp = spStr if len(authRefAssignText) > 0 else ""
+                authRefAssignText += sp + tRef
+
+            refDetails = rsa.getDetails()
+            if len(refDetails) > 0 and refDetails not in [".", "?"]:
+                tDetails = "Depositor details: %s" % refDetails
+                sp = spStr if len(authRefAssignText) > 0 else ""
+                authRefAssignText += sp + tDetails
         #
-        aCat = DataCategory(categoryName)
-        for itemName in categoryItems:
-            aCat.appendAttribute(itemName)
-        #
-        rowCount = 0
-        for row in dataList:
-            rowCount += 1
-            row[0] = str(rowCount)
-            aCat.append(row)
-        #
-        return aCat
-
-    def __getEntitySourceCategory(self):
-        """Return category object of source details."""
-        itemTupList = [
-            ("ORDINAL", "ordinal"),
-            ("ENTITY_ID", "entity_id"),
-            ("AUTH_SEQ_PART_ID", "seq_part_id"),
-            ("AUTH_SEQ_NUM_BEGIN", "seq_part_beg"),
-            ("AUTH_SEQ_NUM_END", "seq_part_end"),
-            ("AUTH_SEQ_PART_TYPE", "seq_part_type"),
-            ("ENTITY_DESCRIPTION", "entity_description"),
-            ("ENTITY_SYNONYMS", "entity_synonyms"),
-            ("SOURCE_GENE_NAME", "gene_name"),
-            ("SOURCE_TAXID", "taxonomy_id"),
-            ("SOURCE_ORGANISM", "source_scientific_name"),
-            ("SOURCE_STRAIN", "source_strain"),
-            ("SOURCE_COMMON_NAME", "source_common_name"),
-            ("SOURCE_VARIANT", "variant"),
-            ("POLYMER_LINKING_TYPE", "entity_polymer_type"),
-            ("ENTITY_ENZYME_CLASS", "entity_enzyme_class"),
-            ("ENTITY_FRAGMENT_DETAILS", "entity_fragment_details"),
-            ("ENTITY_MUTATION_DETAILS", "entity_mutation_details"),
-            ("ENTITY_DETAILS", "entity_details"),
-            ("SOURCE_METHOD", "source_method"),
-            ("HOST_ORG_SOURCE", "host_org_scientific_name"),
-            ("HOST_ORG_STRAIN", "host_org_strain"),
-            ("HOST_ORG_TAXID", "host_org_taxonomy_id"),
-            ("HOST_ORG_VECTOR", "host_org_vector"),
-            ("HOST_ORG_VECTOR_TYPE", "host_org_vector_type"),
-            ("HOST_ORG_PLASMID", "host_org_plasmid"),
-            ("HOST_ORG_COMMON_NAME", "host_org_common_name"),
-            ("HOST_ORG_CELL_LINE", "host_org_cell_line"),
-            ("HOST_ORG_VARIANT", "host_org_variant"),
-        ]
-
         if self.__verbose:
-            self.__lfh.write("+SequenceDataExport.__getSourceDetails() starting\n")
-            # self.printIt()
+            self.__lfh.write("+SummaryView.__markupAuthorAssignments() depositor reference assignments for entity %s : %s\n" % (entityId, authRefAssignText))
         #
-        rowList = []
-        entityIdList = self.__sds.getGroupIds()
-        iRow = 1
-        for entityId in entityIdList:
-            seqIds = self.__sds.getGroup(entityId)
-            if len(seqIds) < 1:
-                if self.__verbose:
-                    self.__lfh.write("+SequenceDataExport.__getSourceDetails() entityId %s is empty\n" % (entityId))
+        return authRefAssignText
+
+    def __checkPartRange(self, entityId, partInfoList):
+        """Check part range definition and write out the warning message if there are errors"""
+        seqLength = 0
+        authVerList = self.__sds.getVersionIds(seqId=entityId, partId=1, altId=1, dataType="sequence", seqType="auth")
+        if len(authVerList) > 0:
+            seq = self.__sds.getSequence(seqId=entityId, seqType="auth", partId=1, altId=1, version=authVerList[0])
+            seqLength = len(seq)
+        #
+        if seqLength == 0:
+            return
+        #
+        ok, partText = self.__checkPartRangeError(seqLength, partInfoList)
+        if ok:
+            return
+        #
+        if self.__partRangeErrorMsg:
+            self.__partRangeErrorMsg += "<br />\n"
+        #
+        self.__partRangeErrorMsg += "Entity '" + str(entityId) + "' (seq. length=" + str(seqLength) + ") : " + partText
+
+    def __checkPartRangeError(self, seqLength, partList):
+        """Check part range definition"""
+        if len(partList) < 1:
+            return False, "No part information defined."
+        #
+        try:
+            status = True
+            text = ""
+            for i in range(0, len(partList)):
+                if text:
+                    text += ", "
                 #
-                continue
-            #
-            seqId0 = entityId
-            partIdList = self.__sds.getPartIds(seqId0, dataType="sequence", seqType="auth")
-            #
-            for partId in partIdList:
-                if self.__verbose:
-                    self.__lfh.write("+SequenceDataExport.__getSourceDetails() entityId %r partId %r  __I  %r\n" % (entityId, partId, self.__I["auth"][seqId0][partId]))
-                # JDW
-                # altId,versionId=self.__I["auth"][seqId0][partId]
-                altId, versionId = self.__I["auth"][seqId0][1]
-                fD = self.__sds.getFeature(seqId0, seqType="auth", partId=partId, altId=altId, version=versionId)
-                d = {}
-                for itemTup in itemTupList:
-                    ky = itemTup[0]
-                    if ky in fD:
-                        d[ky] = fD[ky]
-                    else:
-                        d[ky] = ""
-                    #
+                text += "Part '" + str(partList[i][0]) + "' - ( " + str(partList[i][1]) + ", " + str(partList[i][2]) + " )"
                 #
-                d["ORDINAL"] = iRow
-                d["ENTITY_ID"] = entityId
-                d["AUTH_SEQ_PART_ID"] = partId
-                rowList.append(d)
-                iRow += 1
+                seqNumBeg = int(partList[i][1])
+                seqNumEnd = int(partList[i][2])
+                if seqNumEnd < seqNumBeg:
+                    status = False
+                if (i == 0) and (seqNumBeg != 1):
+                    status = False
+                if (i == (len(partList) - 1)) and (seqNumEnd != seqLength):
+                    status = False
+                if i > 0:
+                    prevNumEnd = int(partList[i - 1][2])
+                    if seqNumBeg != (prevNumEnd + 1):
+                        status = False
+                    #
                 #
             #
-        #
-        aCat = DataCategory("pdbx_seqtool_entity_details")
-        for itemTup in itemTupList:
-            attribName = itemTup[1]
-            aCat.appendAttribute(attribName)
-        #
-        for rD in rowList:
-            vL = []
-            for itemTup in itemTupList:
-                ky = itemTup[0]
-                vL.append(rD[ky])
+            return status, text
+        except Exception as _e:  # noqa: F841
+            text = ""
+            for i in range(0, len(partList)):
+                if text:
+                    text += ", "
+                #
+                text += "Part '" + str(partList[i][0]) + "' - ( " + str(partList[i][1]) + ", " + str(partList[i][2]) + " )"
             #
-            aCat.append(vL)
+            return False, text
         #
-        return aCat
+
+
+if __name__ == "__main__":
+    pass
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/SequenceDataStore.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/SequenceDataStore.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/SequenceDataStoreTests.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/SequenceDataStoreTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/SequenceEditStore.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/SequenceEditStore.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/SequenceEditStoreTests.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/SequenceEditStoreTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/TaxonomyDbUtils.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/TaxonomyDbUtils.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/TaxonomyUtils.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/TaxonomyUtils.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 # File:  TaxonomyIoUtils.py
 # Date:  23-Feb-2013
 #
 # Updates:
 #   24-Feb-2013  jdw add serialization
 #   25-Feb-2013  jdw replace dependency request object with siteId on the request object
 #   20-Mar-2013  jdw add method to lookup organism name from taxid
-#   17-Oct-2022   zf add checking if pickle file exists
 ##
 """
 Accessors for NCBI taxonomy names and organizational data hierarchy.
 
 Python style serialization and deserialization of taxonomy data structures is provided
 and coordinated within the project reference data storage model.
 
@@ -80,143 +79,118 @@
     def __serialize(self, d, fn):
         try:
             fb = open(fn, "wb")
             pickle.dump(d, fb, self.__pickleProtocol)
             fb.close()
         except:  # noqa: E722 pylint: disable=bare-except
             pass
-        #
 
     def __deserialize(self, fn):
         try:
-            if os.access(fn, os.F_OK):
-                fb = open(fn, "rb")
-                d = pickle.load(fb)
-                fb.close()
-                if self.__verbose:
-                    self.__lfh.write("+TaxonomyUtils.__deserialize() return %d records for file %s\n" % (len(d), fn))
-                return d
-            else:
-                return {}
-            #
+            fb = open(fn, "rb")
+            d = pickle.load(fb)
+            fb.close()
+            if self.__verbose:
+                self.__lfh.write("+TaxonomyUtils.__deserialize() return %d records for file %s\n" % (len(d), fn))
+            return d
         except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
                 self.__lfh.write("+TaxonomyUtils.__deserialize() failed for file %s\n" % fn)
-            #
             return {}
-        #
 
     def readTaxonomyNodeData(self, serialize=False):
         """Read the NCBI taxonomy data file 'nodes.dmp' and
         return a dictionary of parent taxonomy id's.
 
         d[tax_id]=parent_tax_id
         """
         d = {}
         try:
             fn = os.path.join(self.__taxPath, "nodes.dmp")
-            if os.access(fn, os.F_OK):
-                ifh = open(fn, "r")
-                for line in ifh:
-                    if not line:
-                        continue
-                    #
-                    fields = line.split("\t|\t")
-                    d[str(fields[0]).strip()] = str(fields[1]).strip()
+            ifh = open(fn, "r")
+            for line in ifh:
+                if not line:
+                    continue
                 #
-                ifh.close()
-                if serialize:
-                    self.__serialize(d, self.__nodesPicPath)
-                #
-            #
+                fields = line.split("\t|\t")
+                d[str(fields[0]).strip()] = str(fields[1]).strip()
+            ifh.close()
+            if serialize:
+                self.__serialize(d, self.__nodesPicPath)
         except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
                 traceback.print_exc(file=self.__lfh)
-            #
             self.__lfh.write("+TaxonomyUtils.readTaxonomyNodeData() failed to read taxonomy data file %s\n" % fn)
-        #
+
         return d
 
     def readTaxonomyNameData(self, serialize=False):
         """Read the NCBI taxonomy data file 'names.dmp' and
         return a dictionary of taxonomy names and synonyms.
 
         d[tax_id]=(name: [] , synoynm: [])
 
         """
         d = {}
         orgD = {}
         try:
             fn = os.path.join(self.__taxPath, "names.dmp")
-            if os.access(fn, os.F_OK):
-                ifh = open(fn, "r")
-                for line in ifh:
-                    if line is None or len(line) < 1:
-                        continue
-                    #
-                    fields = line[:-1].split("\t|")
-                    taxId = str(fields[0]).strip()
-                    name = str(fields[1]).strip()
-                    nType = str(fields[3]).strip()
-                    #
-                    if taxId not in d:
-                        d[taxId] = {}
-                        d[taxId]["name"] = []
-                        d[taxId]["synonym"] = []
-                    #
-                    if nType in ["scientific name"]:
-                        d[taxId]["name"].append(name)
-                        orgD[name] = name
-                    elif nType in ["synonym", "equivalent name"]:
-                        d[taxId]["synonym"].append(name)
-                    #
+            ifh = open(fn, "r")
+            for line in ifh:
+                if line is None or len(line) < 1:
+                    continue
+                fields = line[:-1].split("\t|")
+                taxId = str(fields[0]).strip()
+                name = str(fields[1]).strip()
+                nType = str(fields[3]).strip()
                 #
-                ifh.close()
-                if serialize:
-                    self.__serialize(d, self.__namesPicPath)
-                    self.__serialize(sorted(orgD.keys()), self.__orgNameListPicPath)
-                #
-            #
+                if taxId not in d:
+                    d[taxId] = {}
+                    d[taxId]["name"] = []
+                    d[taxId]["synonym"] = []
+                if nType in ["scientific name"]:
+                    d[taxId]["name"].append(name)
+                    orgD[name] = name
+                elif nType in ["synonym", "equivalent name"]:
+                    d[taxId]["synonym"].append(name)
+            ifh.close()
+            if serialize:
+                self.__serialize(d, self.__namesPicPath)
+                self.__serialize(sorted(orgD.keys()), self.__orgNameListPicPath)
         except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
                 traceback.print_exc(file=self.__lfh)
-            #
             self.__lfh.write("+TaxonomyUtils.readTaxonomyNameData() failed to read taxonomy data file %s\n" % fn)
-        #
         return d
 
     def getAncestors(self, taxId):
         """Fetch the ancestors for the input taxId.
 
         Return ancestors dictionary containing keys:
 
                 id    - input TaxId
                 p_id  - parent TaxId
                gp_id  - grand parent TaxId
         """
         if not self.__nodes:
             self.__nodes = self.__deserialize(self.__nodesPicPath)
-        #
+
         anD = {}
         if taxId is None or len(taxId) < 1:
             return anD
-        #
         try:
             sTaxId = str(taxId).strip()
             anD["id"] = sTaxId
             if self.__nodes:
                 if sTaxId in self.__nodes:
                     parent_id = self.__nodes[sTaxId]
                     anD["p_id"] = parent_id
                     if parent_id in self.__nodes:
                         gparent_id = self.__nodes[parent_id]
                         anD["gp_id"] = gparent_id
-                    #
-                #
-            #
         except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
                 self.__lfh.write("+TaxonomyUtils.getAncestos() failed for input taxId %s\n" % taxId)
                 traceback.print_exc(file=self.__lfh)
-            #
+
         #
         return anD
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/TaxonomyUtilsTests.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/TaxonomyUtilsTests.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/io/testAuto.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/io/testAuto.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/link/PolymerLinkageDepict.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/link/PolymerLinkageDepict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/update/UpdatePolymerEntityPartitions.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/update/UpdatePolymerEntityPartitions.py`

 * *Files 0% similar despite different names*

```diff
@@ -214,17 +214,14 @@
                 self.__updateGroupInstances(entityId, mergeEntityId)
 
             #
             pD = {}
             # for partId in range(1, numParts + 8):
             for partId in range(1, totalNumParts + 1):
                 taxId = self.__reqObj.getValue("p_%d_taxid" % partId)
-                if (taxId is None) or (taxId == self.__placeHolderValue):
-                    taxId = ""
-                #
                 seqBegin = self.__reqObj.getValue("p_%d_seqbegin" % partId)
                 seqEnd = self.__reqObj.getValue("p_%d_seqend" % partId)
                 seqPartType = self.__reqObj.getValue("p_%d_seqtype" % partId)
                 if (
                     (not seqPartType)
                     or (seqPartType == self.__placeHolderValue)
                     or (not seqBegin)
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/update/UpdatePolymerEntityReference_v2.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/update/UpdatePolymerEntityReference_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,15 +70,17 @@
             <tr>
                <th>Reference Resource</th>
                <th>Accession Code</th>
                <th>Seq Begin</th>
                <th>Seq End</th>
              </tr>
             <tr>
-            <td><span id="dbname"      class="ief %(dbname_css)s" data-ief-edittype="select" data-ief-selectvalues='[{"value":"UNP","label":"UNP","selected":false},{"value":"GB","label":"GB","selected":false}]'>%(dbname)s</span></td>
+            <td><span id="dbname"      class="ief %(dbname_css)s" data-ief-edittype="select"
+                                       data-ief-selectvalues='[{"value":"UNP","label":"UNP","selected":false},{"value":"GB","label":"GB","selected":false}]'>
+                                       %(dbname)s</span></td>
             <td><span id="dbaccession" class="ief %(dbaccession_css)s">%(dbaccession)s</span></td>
             <td><span id="dbseqbegin"  class="ief %(dbseqbegin_css)s">%(dbseqbegin)s</span></td>
             <td><span id="dbseqend"    class="ief %(dbseqend_css)s">%(dbseqend)s</span></td>
             </tr>
             </table>
             <input type="submit" name="submit" value="Submit" class="disableonclick submitparentform" />
             <!-- <input type="reset" name="reset" value="Reset" /> -->
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/update/UpdatePolymerEntitySourceDetails.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/update/UpdatePolymerEntitySourceDetails.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,16 @@
                 <td class="bgcolcurrent"><span id="HOST_ORG_VARIANT" class="ief my-editable-cell %(HOST_ORG_VARIANT_CSS)s">%(HOST_ORG_VARIANT)s</span></td>
                 <td></td>
                 <td class="bgcolauthor"><span id="HOST_ORG_VARIANT_ORIG" class="my-cell-static">%(HOST_ORG_VARIANT_ORIG)s</span></td>
              </tr>
 
              <tr>
                 <td>Source Method</td>
-                <td class="bgcolcurrent"><span id="SOURCE_METHOD" class="ief my-editable-cell" data-ief-edittype="select"  data-ief-selectvalues='%(SOURCE_METHOD_SELECT)s'>%(SOURCE_METHOD)s</span></td>
+                <td class="bgcolcurrent"><span id="SOURCE_METHOD" class="ief my-editable-cell" data-ief-edittype="select"  data-ief-selectvalues='%(SOURCE_METHOD_SELECT)s'>
+                       %(SOURCE_METHOD)s</span></td>
                 <td></td>
                 <td class="bgcolauthor"><span id="SOURCE_METHOD_ORIG" class="my-cell-static">%(SOURCE_METHOD_ORIG)s</span></td>
              <tr>
             </table>
             <input type="submit" name="submit" value="%(savebuttontext)s" class="disableonclick submitparentform fltrgt" />
             <!-- <input type="reset" name="reset" value="Reset" /> -->
         </form>
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/Autodict.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/Autodict.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/GetSameSeqAnnotationWithTaxIdOnly.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/GetSameSeqAnnotationWithTaxIdOnly.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 ##
 # File:  GetSameSeqAnnotation.py
 # Date:  23-Mar-2018
 # Updates:
-#
-# 19-Oct-2022 zf add author provided reference sequence information
-#
 ##
 """
 
 This software was developed as part of the World Wide Protein Data Bank
 Common Deposition and Annotation System Project
 
 Copyright (c) 2018 wwPDB
@@ -27,15 +24,15 @@
 import sys
 import traceback
 from operator import itemgetter
 
 from wwpdb.io.locator.PathInfo import PathInfo
 from wwpdb.io.file.mmCIFUtil import mmCIFUtil
 from wwpdb.apps.seqmodule.align.AlignmentToolUtils import codeIndex
-from wwpdb.apps.seqmodule.io.FetchSeqInfoUtils import FetchSeqInfoUtils
+from wwpdb.apps.seqmodule.io.FetchSeqInfoUtils import fetchNcbiGi, fetchUniProt
 from wwpdb.apps.seqmodule.util.SequenceReferenceData import SequenceReferenceData
 
 
 class GetSameSeqAnnotation(object):
     def __init__(self, siteId=None, sessionPath=None, pathInfo=None, verbose=False, log=sys.stderr):
         """ """
         self.__siteId = siteId
@@ -55,15 +52,15 @@
     def setEntitySeq(self, seq="", polyTypeCode="AA"):
         """Set three letter sequence from input one letter seq"""
         if (not seq) or (len(seq) < 1):
             return
         #
         (self.__oneLetterCodeSeqList, self.__threeLetterCodeSeqList) = self.__srd.cnv1ListPlus3List(seq, polyTypeCode)
 
-    def getSeqAnnotationFromAssignFile(self, retList=None, authPartsTaxIdInfoList=None, authRefList=None, includeSelfRef=False):
+    def getSeqAnnotationFromAssignFile(self, retList=None, authPartsTaxIdInfoList=None, includeSelfRef=False):
         """retList[][0]: depID, retList[][1]: entityID, retList[][2]: pdbID, retList[][3]: AnnInitial, retList[][4]: statusCode,
         retList[][5]: date_begin_processing
         """
         if (not retList) or (not authPartsTaxIdInfoList):
             return {}
         #
         if len(authPartsTaxIdInfoList) == 1:
@@ -86,34 +83,21 @@
         #
         if not assignFileList:
             return {}
         #
         if len(assignFileList) > 1:
             assignFileList.sort(key=itemgetter(7), reverse=True)
         #
-        autoMatchList = []
-        otherMatchList = []
         for entityTup in assignFileList:
-            annInfoMap = self.__getSeqAnnotationFromAssignFile(entityTup, authPartsTaxIdInfoList, authRefList, includeSelfRef)
-            if not annInfoMap:
-                continue
-            #
-            if ("auto_match_status" in annInfoMap) and annInfoMap["auto_match_status"]:
-                autoMatchList.append(annInfoMap)
-            else:
-                otherMatchList.append(annInfoMap)
+            annInfoMap = self.__getSeqAnnotationFromAssignFile(entityTup, authPartsTaxIdInfoList, includeSelfRef)
+            if annInfoMap:
+                return annInfoMap
             #
         #
-        if len(autoMatchList) > 0:
-            return autoMatchList[0]
-        elif len(otherMatchList) > 0:
-            return otherMatchList[0]
-        else:
-            return {}
-        #
+        return {}
 
     def testGetSeqAnnotationFromAssignFile(self, assignFile, entityId, authPartsTaxIdInfoList):
         """ """
         try:
             cifObj = mmCIFUtil(filePath=assignFile)
             seqAnntationInfoMap, partsTaxIdInfo = self.__getEntityDetailsMap(cifObj, entityId, authPartsTaxIdInfoList)
             self.__lfh.write("seqAnntationInfoMap=%d\n" % len(seqAnntationInfoMap))
@@ -142,40 +126,36 @@
             #
         except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
                 traceback.print_exc(file=self.__lfh)
             #
         #
 
-    def __getSeqAnnotationFromAssignFile(self, entityInfo, authPartsTaxIdInfoList, authRefList, includeSelfRef):
+    def __getSeqAnnotationFromAssignFile(self, entityInfo, authPartsTaxIdInfoList, includeSelfRef):
         """ """
         try:
             cifObj = mmCIFUtil(filePath=entityInfo[6])
             seqAnntationInfoMap, partsTaxIdInfo = self.__getEntityDetailsMap(cifObj, entityInfo[1], authPartsTaxIdInfoList)
             if not seqAnntationInfoMap:
                 return seqAnntationInfoMap
             #
             alignmentMap = self.__getAlignmentMap(cifObj, entityInfo[1], partsTaxIdInfo)
             #           if not alignmentMap:
             #               return {}
             #           #
-            dbRefMap = self.__getDbRefMap(cifObj, entityInfo[1], authRefList)
+            dbRefMap = self.__getDbRefMap(cifObj, entityInfo[1])
             selfRefmap = self.__getSelfRefmap(cifObj, entityInfo[1], includeSelfRef)
-            auto_match_status = True
             for partId, infoD in seqAnntationInfoMap.items():
                 if partId in selfRefmap:
                     infoD["selfref"] = True
                     continue
                 #
                 if partId not in dbRefMap:
                     return {}
                 #
-                if "auto_match_status" not in dbRefMap[partId]:
-                    auto_match_status = False
-                #
                 for k, v in dbRefMap[partId].items():
                     infoD[k] = v
                 #
                 if partId not in alignmentMap:
                     return {}
                 #
                 infoD["alignment"] = alignmentMap[partId][0]
@@ -186,17 +166,14 @@
                 #
                 infoD["REF_ENTRY_ID"] = entityInfo[0]
                 infoD["REF_ENTRY_ENTITY_ID"] = entityInfo[1]
                 infoD["REF_PDB_ID"] = entityInfo[2]
                 infoD["REF_ENTRY_STATUS"] = entityInfo[4]
                 infoD["REF_ENTRY_ANN"] = entityInfo[3]
             #
-            if auto_match_status:
-                seqAnntationInfoMap["auto_match_status"] = True
-            #
             return seqAnntationInfoMap
         except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
                 traceback.print_exc(file=self.__lfh)
             #
         #
         return {}
@@ -382,30 +359,25 @@
                 if not alignList[refMap[retDic["ref_mon_id"] + "_" + retDic["ref_mon_num"] + "_" + retDic["part_id"]]][5]:
                     alignList[refMap[retDic["ref_mon_id"] + "_" + retDic["ref_mon_num"] + "_" + retDic["part_id"]]][5] = "deletion"
                 #
             #
         #
         return self.__getAuthRefAlignmentMap(alignList, partsTaxIdInfo)
 
-    def __getDbRefMap(self, cifObj, entityId, authRefList=None):
-        """
-        """
+    def __getDbRefMap(self, cifObj, entityId):
+        """ """
         itemList = (
             ("db_name", "db_name"),
             ("db_code", "db_code"),
             ("db_accession", "db_accession"),
             ("db_isoform", "db_isoform"),
             ("match_begin", "hitFrom"),
             ("match_end", "hitTo"),
         )
         #
-        __authRefList = []
-        if authRefList:
-            __authRefList = authRefList[0]
-        #
         unpIdList = []
         gbIdList = []
         dbRefMap = {}
         retList = cifObj.GetValue("pdbx_seqtool_db_ref")
         for retDic in retList:
             if ("entity_id" not in retDic) or (retDic["entity_id"] != entityId) or ("entity_part_id" not in retDic) or (not retDic["entity_part_id"]):
                 continue
@@ -414,28 +386,14 @@
             for itemTup in itemList:
                 if (itemTup[0] in retDic) and retDic[itemTup[0]]:
                     infoDic[itemTup[1]] = retDic[itemTup[0]]
                 else:
                     infoDic[itemTup[1]] = ""
                 #
             #
-            auto_match_status = False
-            if __authRefList:
-                if (("db_accession" in infoDic) and (infoDic["db_accession"] in __authRefList)) or \
-                   (("db_isoform" in infoDic) and (infoDic["db_isoform"] in __authRefList)):
-                    auto_match_status = True
-                    infoDic["author_provided_id"] = True
-                #
-            else:
-                auto_match_status = True
-            #
-            if auto_match_status:
-                infoDic["auto_match_status"] = True
-            #
-
             if "db_name" in infoDic:
                 if infoDic["db_name"] == "UNP":
                     try:
                         start = int(str(infoDic["hitFrom"]))
                     except:  # noqa: E722 pylint: disable=bare-except
                         start = 0
                     #
@@ -456,24 +414,23 @@
                 #
             #
             infoDic["id"] = 101
             infoDic["sort_order"] = 101
             #
             dbRefMap[retDic["entity_part_id"]] = infoDic
         #
-        fetchSeqUtil = FetchSeqInfoUtils(siteId=self.__siteId, seqReferenceData=self.__srd, verbose=self.__verbose, log=self.__lfh)
         unpD = {}
         gbD = {}
         if len(unpIdList) > 0:
-            unpD = fetchSeqUtil.fetchUniProt(idTupleList=unpIdList)
+            unpD = fetchUniProt(idTupleList=unpIdList, verbose=self.__verbose, log=self.__lfh)
         elif len(gbIdList) > 0:
             gbIdList = list(set(gbIdList))
             for idCode in gbIdList:
                 # No need to rate limit here as this fetches the whole entry - is likely a genome and takes seconds.
-                gbD[idCode] = fetchSeqUtil.fetchNcbiGi(idCode)
+                gbD[idCode] = fetchNcbiGi(idCode, siteId=self.__siteId)
             #
         #
         for _partId, infoDic in dbRefMap.items():
             dbDic = {}
             if "db_name" in infoDic:
                 if infoDic["db_name"] == "UNP":
                     try:
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/LocalBlastSearchUtils.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/LocalBlastSearchUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 #                  nucleotide search
 # 04-Nov-2013  jdw update sort score
 # 15-Dec-2013  jdw trap cases missing taxonomy in either input or in returned reference list
 # 27-Jun-2014  jdw overhaul the runBlastLocal() and optimize for children of taxId 562.
 #                  reduce the number of id lookups and try to find distant matching SP entries.
 #  1-Aug-2014  jdw update handling of annotation fetch failures
 #  8-Dec-2015  jdw change isoform annoation processing -
-#  3-Oct-2022  zf  update __runBlastSearch() & __fetchAuthProvidedRefSequence() methods for better handling author provided
-#                  reference sequence cases.
+# 24-Aug-2018  zf
 ##
 """
 Methods to manage local and sequence search services and package matching reference sequence data.
 
 """
 __docformat__ = "restructuredtext en"
 __author__ = "John Westbrook"
@@ -39,15 +38,15 @@
 import os
 import sys
 import time
 import traceback
 from operator import itemgetter
 
 from wwpdb.apps.seqmodule.io.BlastPlusReader import BlastPlusReader
-from wwpdb.apps.seqmodule.io.FetchSeqInfoUtils import FetchSeqInfoUtils
+from wwpdb.apps.seqmodule.io.FetchSeqInfoUtils import fetchNcbiSummary, fetchUniProt
 from wwpdb.apps.seqmodule.io.TaxonomyUtils import TaxonomyUtils
 from wwpdb.apps.seqmodule.util.FetchReferenceSequenceUtils import FetchReferenceSequenceUtils
 from wwpdb.apps.seqmodule.util.SequenceReferenceData import SequenceReferenceData
 from rcsb.utils.multiproc.MultiProcUtil import MultiProcUtil
 from wwpdb.io.locator.PathInfo import PathInfo
 from wwpdb.utils.dp.RcsbDpUtility import RcsbDpUtility
 
@@ -135,24 +134,24 @@
         if authRefList:
             self.__authRefIdList = authRefList[0]
             self.__authRefDataList = authRefList[1]
         #
         if (not self.__dataSetId) or (not self.__entityD):
             return {}
         #
-        autoMatchStatus, rD = self.__getExistingSearchResult()
+        rD = self.__getExistingSearchResult()
         if rD:
-            return autoMatchStatus, rD
+            return rD
         #
-        autoMatchStatus, rD = self.__runBlastSearch()
+        rD = self.__runBlastSearch()
         if rD:
             self.__writeSearchResult(rD)
             # self.__writeBlastSearchResultCifFile(rD)
         #
-        return autoMatchStatus, rD
+        return rD
 
     def __getExistingSearchResult(self):
         """Get prvious blast search result"""
         self.__entityId = self.__entityD["ENTITY_ID"]
         currSeq = self.__entityD["SEQ_ENTITY_1"]
         self.__entitySeq = currSeq.replace(" ", "").replace("\n", "").replace("\t", "")
         self.__blastResultFile = self.__pI.getFilePath(self.__dataSetId, contentType="seqdb-match", formatType="pic", fileSource="session", partNumber=self.__entityId)
@@ -174,55 +173,47 @@
             if (
                 ("sequence" not in pickleObj)
                 or ("part_info" not in pickleObj)
                 or ("ref_data" not in pickleObj)
                 or (self.__entitySeq != pickleObj["sequence"])
                 or (len(self.__entityD["PART_LIST"]) != len(pickleObj["part_info"]))
             ):
-                return False, {}
+                return {}
             #
             for partNum, fD in enumerate(self.__entityD["PART_LIST"], start=1):
                 if (
                     (partNum not in pickleObj["part_info"])
                     or (fD["SEQ_NUM_BEG"] != pickleObj["part_info"][partNum][0])
                     or (fD["SEQ_NUM_END"] != pickleObj["part_info"][partNum][1])
                 ):
-                    return False, {}
+                    return {}
                 #
             #
             if self.__verbose:
                 self.__lfh.write("+LocalBlastSearchUtils.__getExistingSearchResult() using previous search result for entity id %s\n" % self.__entityId)
             #
             return self.__getReSortHitInfo(pickleObj["ref_data"])
         #
-        return False, {}
+        return {}
 
     def __getReSortHitInfo(self, inD):
         """ """
         try:
-            autoMatchList = []
             outD = {}
             for partNum, fD in enumerate(self.__entityD["PART_LIST"], start=1):
                 partId = str(partNum)
                 if partId not in inD:
                     continue
                 #
                 _start_index, hitList = self.__sortHitList(inD[partId], fD["SOURCE_TAXID"], False)
                 outD[partId] = hitList
-                if (len(hitList) == 1) and ("auto_match_status" in hitList[0]) and hitList[0]["auto_match_status"]:
-                    autoMatchList.append(True)
-                #
-            #
-            autoMatchStatus = False
-            if (len(autoMatchList) > 0) and (len(autoMatchList) == len(self.__entityD["PART_LIST"])):
-                autoMatchStatus = True
             #
-            return autoMatchStatus, outD
+            return outD
         except:  # noqa: E722 pylint: disable=bare-except
-            return False, {}
+            return {}
         #
 
     def __runBlastSearch(self):
         """Perform sequence search for each entity part in the input feature list described in the input dictionary."""
         oneLetterCodeSeq = str(self.__entityD["SEQ_ENTITY_1_CAN"]).strip().upper()
         #
         if "SEQ_ENTITY_1_SEARCH" in self.__entityD:
@@ -235,19 +226,18 @@
         self.__seqType = self.__entityD["POLYMER_LINKING_TYPE"]
         #
         if self.__verbose:
             self.__lfh.write("\n+LocalBlastSearchUtils.__runBlastSearch() STARTING with polymer type  %s sequence = %s\n" % (self.__seqType, oneLetterCodeSeq))
         #
         authRefD = {}
         if not self.__checkPartRange(len(self.__fullOneLetterSeq), self.__entityD["PART_LIST"]):
-            return False, authRefD
+            return authRefD
         #
-        foundPerfectMatch = True
+        partIdList = []
         partDataList = []
-        blastDataList = []
         for partNum, fD in enumerate(self.__entityD["PART_LIST"], start=1):
             seqPartType = fD["SEQ_PART_TYPE"]
             seqPartId = fD["SEQ_PART_ID"]
             if not str(seqPartType).lower().startswith("biol"):
                 if self.__verbose:
                     self.__lfh.write("+LocalBlastSearchUtils.__runBlastSearch() skipping sequence entity %r part %r type %r\n" % (self.__entityId, seqPartId, seqPartType))
                 #
@@ -260,105 +250,67 @@
                     self.__lfh.write(
                         "+LocalBlastSearchUtils.__runBlastSearch() skipping sequence entity %r part %r type %r BegNum %r EndNum %r\n"
                         % (self.__entityId, seqPartId, seqPartType, seqNumBeg, seqNumEnd)
                     )
                 #
                 continue
             #
-            # Skip blast search for poly-UNK/ALA sequence (DAOTHER-3639 & DAOTHER-8135)
+            # Skip blast search for UNK sequence DAOTHER-3639
             countUNK = 0
-            countALA = 0
             countTotal = 0
             for oneLetterCode in self.__fullOneLetterSeq[(int(seqNumBeg) - 1) : int(seqNumEnd)]:
                 if oneLetterCode == "X":
                     countUNK += 1
-                elif oneLetterCode == "A":
-                    countALA += 1
                 #
                 countTotal += 1
             #
-            if ((10 * countUNK) > (9 * countTotal)) or (self.__seqType.startswith("polypeptide") and ((10 * countALA) > (9 * countTotal))):
+            if (10 * countUNK) > (9 * countTotal):
                 if self.__verbose:
-                    self.__lfh.write("+LocalBlastSearchUtils.__runBlastSearch() skipping unknown/poly-ALA sequence part %r type %r BegNum %r EndNum %r\n" %
-                                     (seqPartId, seqPartType, seqNumBeg, seqNumEnd))
-                    self.__lfh.flush()
-                #
-                if self.__seqType.startswith("polypeptide") and ((10 * countALA) > (9 * countTotal)):
-                    foundPerfectMatch = False
+                    self.__lfh.write(
+                        "+LocalBlastSearchUtils.__runBlastSearch() skipping unknown sequence part %r type %r BegNum %r EndNum %r\n" % (seqPartId, seqPartType, seqNumBeg, seqNumEnd)
+                    )
                 #
                 continue
             #
+            partIdList.append(str(partNum))
+            #
             taxId = fD["SOURCE_TAXID"]
+            sequence = oneLetterCodeSeq[(int(seqNumBeg) - 1) : int(seqNumEnd)]
             searchSequence = oneLetterSearchSeq[(int(seqNumBeg) - 1) : int(seqNumEnd)]
             #
-            xmlFilePath = os.path.join(self.__sessionPath, self.__dataSetId + "_blast-match_E" + self.__entityId + "_P" + str(partNum) + ".xml")
-            if os.access(xmlFilePath, os.F_OK):
-                os.remove(xmlFilePath)
-            #
-            partDataList.append((str(partNum), searchSequence, seqNumBeg, seqNumEnd, taxId, xmlFilePath))
-            #
-            mutationList = []
-            if ("MUTATION_DETAILS" in self.__entityD) and self.__entityD["MUTATION_DETAILS"]:
-                for val in self.__entityD["MUTATION_DETAILS"].strip().upper().replace(",", " ").split(" "):
-                    if (not val) or (len(val) < 3) or (not val[0].isalpha()) or (not val[len(val) - 1].isalpha()):
-                        continue
-                    #
-                    hasDigit = False
-                    allDigit = True
-                    for i in range(1, len(val) - 1):
-                        if val[i].isdigit():
-                            hasDigit = True
-                        else:
-                            allDigit = False
-                        #
-                    #
-                    if hasDigit and allDigit:
-                        mutationList.append(val)
-                    #
-                #
-            #
-            autoMatchStatus, authHitList = self.__fetchAuthProvidedRefSequence(searchSequence, seqNumBeg, seqNumEnd, str(partNum), taxId, mutationList,
-                                                                               len(self.__entityD["PART_LIST"]))
-            if not autoMatchStatus:
-                foundPerfectMatch = False
-            #
+            authHitList = self.__fetchAuthProvidedRefSequence(sequence, seqNumBeg, seqNumEnd, str(partNum))
             if authHitList:
                 authRefD[str(partNum)] = authHitList
-                # Skip blast search if found perfect author provided reference sequence match
-                if autoMatchStatus:
-                    continue
-                #
-                # Skip blast search for short sequence
-                if len(searchSequence) <= self.__shortSequenceLengthLimit:
+                if len(sequence) <= self.__shortSequenceLengthLimit:
                     continue
                 #
-            else:
-                foundPerfectMatch = False
             #
-            blastDataList.append((str(partNum), searchSequence, seqNumBeg, seqNumEnd, taxId, xmlFilePath))
+            xmlFilePath = os.path.join(self.__sessionPath, self.__dataSetId + "_blast-match_E" + self.__entityId + "_P" + str(partNum) + ".xml")
+            if os.access(xmlFilePath, os.F_OK):
+                os.remove(xmlFilePath)
+            #
+            partDataList.append((str(partNum), searchSequence, seqNumBeg, seqNumEnd, taxId, xmlFilePath))
         #
         if not partDataList:
-            return foundPerfectMatch, authRefD
+            return authRefD
         #
         rD = {}
         try:
-            if blastDataList:
-                numProc = int(multiprocessing.cpu_count() / 2)
-                mpu = MultiProcUtil(verbose=True)
-                mpu.set(workerObj=self, workerMethod="runMultiLocalBlasts")
-                mpu.setWorkingDir(self.__sessionPath)
-                mpu.setOptions({"ncbilock": self.__ncbilock})
-                _ok, _failList, _retLists, _diagList = mpu.runMulti(dataList=blastDataList, numProc=numProc, numResults=1)
-            #
+            numProc = int(multiprocessing.cpu_count() / 2)
+            mpu = MultiProcUtil(verbose=True)
+            mpu.set(workerObj=self, workerMethod="runMultiLocalBlasts")
+            mpu.setWorkingDir(self.__sessionPath)
+            mpu.setOptions({"ncbilock": self.__ncbilock})
+            _ok, _failList, _retLists, _diagList = mpu.runMulti(dataList=partDataList, numProc=numProc, numResults=1)
             id_count = 1
             for partTup in partDataList:
-                hitList = []
-                if os.access(partTup[5], os.F_OK):
-                    hitList = self.__readBlastResultXmlFile(seqNumBeg=partTup[2], seqNumEnd=partTup[3], seqPartId=partTup[0], authTaxId=partTup[4],
-                                                            blastResultXmlPath=partTup[5])
+                if not os.access(partTup[5], os.F_OK):
+                    continue
+                #
+                hitList = self.__readBlastResultXmlFile(seqNumBeg=partTup[2], seqNumEnd=partTup[3], seqPartId=partTup[0], authTaxId=partTup[4], blastResultXmlPath=partTup[5])
                 #
                 if hitList:
                     SeqAlignmentMap = self.__getRefSeqAlignments(hitList)
                     for hit in hitList:
                         if not hit["sort_order"] in SeqAlignmentMap:
                             continue
                         #
@@ -380,76 +332,61 @@
                         if partTup[0] in rD:
                             rD[partTup[0]].append(hit)
                         else:
                             rD[partTup[0]] = [hit]
                         #
                     #
                 #
-                # Merge author provided reference sequence match result
-                #
-                if (partTup[0] in authRefD) and authRefD[partTup[0]]:
-                    if partTup[0] not in rD:
-                        rD[partTup[0]] = authRefD[partTup[0]]
-                    else:
-                        rD[partTup[0]] = self.__mergeAuthorProvidedRefSeqMath(rD[partTup[0]], authRefD[partTup[0]], partTup[4])
-                    #
-                #
             #
             if self.__verbose:
                 self.__lfh.write("+LocalBlastSearchUtils.__runBlastSearch() COMPLETED search for entity %r\n" % self.__entityId)
-            #
+        #
         except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
                 traceback.print_exc(file=self.__lfh)
                 self.__lfh.write("+LocalBlastSearchUtils.__runBlastSearch() search for entity %r failed\n" % self.__entityId)
             #
         #
-        return foundPerfectMatch, rD
-
-    def __fetchAuthProvidedRefSequence(self, sequence, seqNumBeg, seqNumEnd, seqPartId, taxId, mutationList, partNumbers):
-        """Fetch reference sequence based on author provided ref IDs"""
-        if (not self.__authRefDataList) or (len(self.__authRefDataList) > partNumbers):
-            return False, []
+        # Merge author provided short sequence reference match result
         #
-        refData = []
-        if partNumbers > 1:
-            for aRefData in self.__authRefDataList:
-                if aRefData[3] and aRefData[4] and (int(seqNumBeg) <= int(aRefData[3])) and (int(seqNumEnd) >= int(aRefData[4])):
-                    refData = aRefData
-                    break
-                #
+        for partId in partIdList:
+            if (partId in authRefD) and (partId not in rD):
+                rD[partId] = authRefD[partId]
             #
-        else:
-            refData = self.__authRefDataList[0]
         #
-        if not refData:
-            return False, []
+        return rD
+
+    def __fetchAuthProvidedRefSequence(self, sequence, seqNumBeg, seqNumEnd, seqPartId):
+        """Fetch reference sequence based on author provided ref IDs"""
+        if not self.__authRefDataList:
+            return []
         #
         fetchUtil = FetchReferenceSequenceUtils(siteId=self.__siteId, seqReferenceData=self.__srd, verbose=self.__verbose, log=self.__lfh)
-        autoMatchStatus, hitD = fetchUtil.fetchReferenceSequenceWithSeqMatch(refData[0], refData[1], refData[2], taxId, sequence, seqNumBeg, mutationList)
-        if hitD:
-            hitD["beg_seq_num"] = seqNumBeg
-            hitD["end_seq_num"] = seqNumEnd
-            hitD["fragment_id"] = seqPartId
-            #
-            alignIndex, sTup3L, alignLength, seqSim, seqSimWithGaps, error = self.__getSeqAlignIndex(hitD)
-            if not error:
+        #
+        for refIDList in self.__authRefDataList:
+            for accession in refIDList[1:]:
+                hitD = fetchUtil.fetchReferenceSequenceWithSeqMatch(refIDList[0], accession, sequence)
+                if not hitD:
+                    continue
+                #
+                hitD["beg_seq_num"] = seqNumBeg
+                hitD["end_seq_num"] = seqNumEnd
+                hitD["fragment_id"] = seqPartId
+                #
+                alignIndex, sTup3L, alignLength, seqSim, seqSimWithGaps, error = self.__getSeqAlignIndex(hitD)
+                if error:
+                    break
+                #
                 hitD["alignment"] = alignIndex
                 hitD["seq_tup_list"] = sTup3L
                 hitD["statistics"] = (alignLength, seqSim, seqSimWithGaps)
-                hitD["author_provided_id"] = True
-                if autoMatchStatus:
-                    hitD["auto_match_status"] = True
-                #
-                return autoMatchStatus, [hitD]
-            else:
-                self.__lfh.write("+LocalBlastSearchUtils.__fetchAuthProvidedRefSequence() get sequence alignment index error: %s\n" % error)
+                return [hitD]
             #
         #
-        return False, []
+        return []
 
     def __writeSearchResult(self, rD):
         """Write out the current search result pickle file"""
         partInfoD = {}
         for partNum, fD in enumerate(self.__entityD["PART_LIST"], start=1):
             partInfoD[partNum] = (fD["SEQ_NUM_BEG"], fD["SEQ_NUM_END"])
         #
@@ -532,34 +469,28 @@
         #
         if self.__seqType in ["polypeptide(L)", "polypeptide(D)", "polypeptide"]:
             dp = RcsbDpUtility(tmpPath=tmpPathAbs, siteId=self.__siteId, verbose=True)
             dp.addInput(name="one_letter_code_sequence", value=oneLetterCodeSeq)
             dp.addInput(name="db_name", value="my_uniprot_all")
             dp.addInput(name="num_threads", value="4")
             dp.addInput(name="max_hits", value=self.__maxHitsSearch)
-            if taxId:
-                dp.addInput(name="tax_id", value=taxId)
-            #
             dp.op("seq-blastp")
             dp.exp(resultPath)
             if self.__cleanUp and not self.__debug:
                 dp.cleanup()
             #
         # elif self.__seqType == 'polyribonucleotide':
         # for DAOTHER-6304
         elif self.__seqType in ["polydeoxyribonucleotide", "polyribonucleotide"]:
             if len(oneLetterCodeSeq) > self.__minRnaSequenceSearchLength:
                 dp = RcsbDpUtility(tmpPath=tmpPathAbs, siteId=self.__siteId, verbose=True)
                 dp.addInput(name="one_letter_code_sequence", value=oneLetterCodeSeq)
                 dp.addInput(name="db_name", value="my_ncbi_nt")
                 dp.addInput(name="num_threads", value="4")
                 dp.addInput(name="max_hits", value=self.__maxHitsSearch)
-                if taxId:
-                    dp.addInput(name="tax_id", value=taxId)
-                #
                 dp.op("seq-blastn")
                 dp.exp(resultPath)
                 if self.__cleanUp and not self.__debug:
                     dp.cleanup()
                 #
             #
         else:
@@ -574,18 +505,16 @@
 
     def __readBlastResultXmlFile(self, seqNumBeg, seqNumEnd, seqPartId, authTaxId, blastResultXmlPath):
         """Read blast result"""
         hitList = []
         bpr = BlastPlusReader(verbose=self.__verbose, log=self.__lfh)
         if self.__seqType == "polyribonucleotide":
             bpr.setSequenceType(self.__seqType)
-        #
         searchHitList = bpr.readFile(filePath=blastResultXmlPath)
         #
-        fetchSeqUtil = FetchSeqInfoUtils(siteId=self.__siteId, seqReferenceData=self.__srd, verbose=self.__verbose, log=self.__lfh)
         if self.__seqType in ["polypeptide(L)", "polypeptide(D)", "polypeptide"]:
             idCodeList = []
             for hit in searchHitList:
                 hit["non_isoform_score"] = 1
                 if "db_accession" in hit and "db_name" in hit:
                     try:
                         start = int(str(hit["hitFrom"]))
@@ -605,22 +534,16 @@
                 #
             #
             # Incorporate non-overlapping additional details about each matching sequence entry.
             #   ( Still using the REST API to get the entry information )
             #
             if self.__verbose:
                 self.__lfh.write("+LocalBlastSearchUtils.__readBlastResultXmlFile() Fetch sequence database entries for %d filtered reference idcodes\n" % len(idCodeList))
-            #
             if len(idCodeList) > 0:
-                try:
-                    unpD = fetchSeqUtil.fetchUniProt(idTupleList=idCodeList)
-                except:  # noqa: E722 pylint: disable=bare-except
-                    traceback.print_exc(file=self.__lfh)
-                    self.__lfh.flush()
-                #
+                unpD = fetchUniProt(idTupleList=idCodeList, verbose=self.__verbose, log=self.__lfh)
                 for hit in searchHitList:
                     acId = None
                     isIso = False
                     if "db_isoform" in hit and (len(hit["db_isoform"]) > 0) and (hit["db_isoform"] not in [".", "?"]):
                         acId = hit["db_isoform"]
                         hit["non_isoform_score"] = 0
                         isIso = True
@@ -640,19 +563,17 @@
                         #
                         dd = {}
                         if (acId, start, end) in unpD:
                             dd = unpD[(acId, start, end)]
                         elif isIso and ((hit["db_accession"], start, end) in unpD):
                             dd = unpD[(hit["db_accession"], start, end)]
                         #
-                        if dd:
-                            for (k, v) in dd.items():
-                                if (k != "sequence") and ((k not in hit) or (v and (k in ("name", "source_scientific", "strain", "taxonomy_id", "gene")))):
-                                    hit[k] = v
-                                #
+                        for (k, v) in dd.items():
+                            if (k != "sequence") and (k not in hit):
+                                hit[k] = v
                             #
                         #
                         hitList.append(hit)
                     #
                 #
             #
         # elif self.__seqType == 'polyribonucleotide':
@@ -672,16 +593,16 @@
             #
             if len(idCodeList) > 0:
                 giD = {}
                 for idCode in idCodeList:
                     # Ensure do not max out request rate
                     if self.__ncbilock:
                         self.__ncbilock.waitnext()
-                    #
-                    giD[idCode] = fetchSeqUtil.fetchNcbiSummary(idCode)
+
+                    giD[idCode] = fetchNcbiSummary(idCode, siteId=self.__siteId)
                 #
                 for hit in hitList:
                     if "db_accession" in hit:
                         acId = hit["db_accession"]
                         if acId in giD:
                             dd = giD[acId]
                             for (k, v) in dd.items():
@@ -740,15 +661,14 @@
         authAncestorD = self.__taxUtils.getAncestors(authTaxId)
         if self.__debug:
             self.__lfh.write("+LocalBlastSearchUtils.__sortHitList() length %d authTaxId %s authAncestorD %r\n" % (len(hitList), authTaxId, authAncestorD.items()))
         #
         highest_identity_score_with_taxid_match = 0
         lowest_identity_score_with_taxid_match = 101
         lowest_identity_score_with_refid_match = 101
-        has_author_provided_id = False
         for i, hit in enumerate(hitList):
             if "non_isoform_score" not in hit:
                 hit["non_isoform_score"] = 1
             #
             if fullScoreFlag or ("identity_score" not in hit):
                 hit["identity_score"] = (float(hit["identity"]) - float(hit["gaps"])) * 100.0 / float(hit["query_length"])
                 if self.__debug:
@@ -759,28 +679,25 @@
                     #
                 if hit["db_name"] == "SP":
                     hit["db_score"] = 1
                 else:
                     hit["db_score"] = 0
                 #
             #
-            if self.__authRefIdList and ((hit["db_code"].strip().upper() in self.__authRefIdList) or (hit["db_accession"].strip().upper() in
-               self.__authRefIdList) or (hit["db_isoform"].strip().upper() in self.__authRefIdList)):
+            if self.__authRefIdList and ((hit["db_code"].strip().upper() in self.__authRefIdList) or (hit["db_accession"].strip().upper() in self.__authRefIdList)):
                 if hit["identity_score"] < lowest_identity_score_with_refid_match:
                     lowest_identity_score_with_refid_match = hit["identity_score"]
                 #
-                hit["author_provided_id"] = True
-                has_author_provided_id = True
                 hit["code_score"] = 1
             else:
                 hit["code_score"] = 0
             #
             targetAncestorD = {}
             taxonomy_id = ""
-            if ("taxonomy_id" in hit) and hit["taxonomy_id"]:
+            if "taxonomy_id" in hit:
                 taxonomy_id = hit["taxonomy_id"]
                 targetAncestorD = self.__taxUtils.getAncestors(hit["taxonomy_id"])
             #
             taxidMatch = 0
             if authAncestorD and targetAncestorD and "id" in authAncestorD and "id" in targetAncestorD:
                 if authAncestorD["id"] == targetAncestorD["id"]:
                     taxidMatch = 3
@@ -814,48 +731,30 @@
                     self.__lfh.write(
                         "+ReferencSequenceUtils.__sortHitList() taxidMatch %d  authAncestorD[id] %s targetAncestorD[id] %s final score %r\n"
                         % (taxidMatch, authAncestorD["id"], targetAncestorD["id"], hit["sort_metric"])
                     )
                 #
             #
         #
+        start_index = 0
         cutoff_identity_score = 0
         if highest_identity_score_with_taxid_match > 0:
             cutoff_identity_score = 0.85 * highest_identity_score_with_taxid_match
-            if lowest_identity_score_with_refid_match < cutoff_identity_score:
-                cutoff_identity_score = lowest_identity_score_with_refid_match - 0.1
+            if lowest_identity_score_with_taxid_match < cutoff_identity_score:
+                cutoff_identity_score = lowest_identity_score_with_taxid_match
             #
             if lowest_identity_score_with_taxid_match < cutoff_identity_score:
-                cutoff_identity_score = lowest_identity_score_with_taxid_match - 0.1
+                cutoff_identity_score = lowest_identity_score_with_taxid_match
             #
         #
-        # The highest score hit is at the bottom of the list.
-        #
         hitList.sort(key=itemgetter("identity_score", "taxid_match", "code_score", "db_score", "non_isoform_score"))
         #
-        # reorder list if found author provided reference id
-        #
-        if has_author_provided_id and (len(hitList) > 2):
-            idx = -1
-            for i, hit in enumerate(hitList):
-                if ("author_provided_id" in hit) and hit["author_provided_id"]:
-                    idx = i
-                #
-            #
-            if (idx >= 0) and (idx < (len(hitList) - 2)):
-                hitList.insert(-1, hitList.pop(idx))
-            #
-        #
-        start_index = 0
         first = True
         for i, hit in enumerate(hitList):
             hit["sort_order"] = str(i + 1)
-            if ("author_provided_id" in hit) and hit["author_provided_id"]:
-                continue
-            #
             if first and (hit["identity_score"] > cutoff_identity_score):
                 start_index = i
                 first = False
             #
         #
         if self.__debug:
             self.__lfh.write("ReferencSequenceUtils.__sortHitList() hitList=%d maxHitsSave=%d\n" % (len(hitList), self.__maxHitsSave))
@@ -895,42 +794,14 @@
         except:  # noqa: E722 pylint: disable=bare-except
             if self.__verbose:
                 traceback.print_exc(file=self.__lfh)
             #
         #
         return alignMap
 
-    def __mergeAuthorProvidedRefSeqMath(self, blastHitList, authHitList, authTaxId):
-        """ Merge author provided reference sequence match with blast search match(es)
-            See ticket DAOTHER-7903 the rule for displaying row(s)
-        """
-        mergedHitList = []
-        for authD in authHitList:
-            found = False
-            for blastD in blastHitList:
-                if ("db_accession" in authD) and ("db_isoform" in authD) and ("db_accession" in blastD) and ("db_isoform" in blastD) and \
-                   (authD["db_accession"] == blastD["db_accession"]) and (authD["db_isoform"] == blastD["db_isoform"]):
-                    if ("auto_match_status" in authD) and authD["auto_match_status"]:
-                        blastD["auto_match_status"] = True
-                    #
-                    found = True
-                    break
-                #
-            #
-            if not found:
-                mergedHitList.append(authD)
-            #
-        #
-        if not mergedHitList:
-            return blastHitList
-        #
-        mergedHitList.extend(blastHitList)
-        _start_index, finalList = self.__sortHitList(mergedHitList, authTaxId, True)
-        return finalList
-
     def getMultiSeqAlignmentProcess(self, dataList, procName, optionsD, workingDir):  # pylint: disable=unused-argument
         """Get Auth/Ref sequence alignments MultiProcUtil API"""
         rList = []
         eList = []
         for hitD in dataList:
             alignIndex, sTup3L, alignLength, seqSim, seqSimWithGaps, error = self.__getSeqAlignIndex(hitD)
             if error:
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/MultiProcLimit.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/MultiProcLimit.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/SearchEntityPolySeqs.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/SearchEntityPolySeqs.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/SeqReferenceSearchUtils.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/SeqReferenceSearchUtils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,12 @@
 ##
 # File:  SeqReferenceSearchUtils.py
 # Date:  22-Nov-2018
 #
 # Updates:
-#
-# 19-Oct-2022 zf add author provided reference sequence information
-#
 ##
 """
 Wrap class for blast sequence search and 100% matched previous processed sequence search
 """
 __docformat__ = "restructuredtext en"
 __author__ = "Zukang Feng"
 __email__ = "zfeng@rcsb.rutgers.edu"
@@ -38,28 +35,28 @@
         self.__ncbilock = ncbilock
 
     def run(self, dataSetId, eD, authDefinedRefList, refRefSearchFlag, forceBlastSearchFlag):
         """ """
         sasUtil = SeqAnnotationSearchUtils(
             siteId=self.__siteId, sessionPath=self.__sessionPath, searchUtil=self.__sepsUtil, pathInfo=self.__pI, verbose=self.__verbose, log=self.__lfh
         )
-        selfRefD, sameSeqRefD = sasUtil.getSameSeqRefInfo(dataSetId, eD, authDefinedRefList)
+        selfRefD, sameSeqRefD = sasUtil.getSameSeqRefInfo(dataSetId, eD)
         #
         eRefD = {}
         if (len(selfRefD) == 0) or forceBlastSearchFlag:
             lbsUtil = LocalBlastSearchUtils(
                 siteId=self.__siteId,
                 sessionPath=self.__sessionPath,
                 pathInfo=self.__pI,
                 doRefSearchFlag=refRefSearchFlag,
                 verbose=self.__verbose,
                 log=self.__lfh,
                 ncbilock=self.__ncbilock,
             )
-            _autoMatchStatus, eRefD = lbsUtil.searchSeqReference(dataSetId=dataSetId, entityD=eD, authRefList=authDefinedRefList)
+            eRefD = lbsUtil.searchSeqReference(dataSetId=dataSetId, entityD=eD, authRefList=authDefinedRefList)
         #
         return eRefD, selfRefD, sameSeqRefD
 
 
 class SeqAnnotationSearchUtils(object):
     """ """
 
@@ -72,42 +69,39 @@
         self.__verbose = verbose
         self.__lfh = log
         #
         if not self.__sepsUtil:
             self.__sepsUtil = SearchEntityPolySeqs(siteId=self.__siteId, sessionPath=self.__sessionPath, verbose=self.__verbose, log=self.__lfh)
         #
 
-    def getSameSeqRefInfo(self, dataSetId, eD, authRefList):
+    def getSameSeqRefInfo(self, dataSetId, eD):
         """ """
         if not eD:
             return {}, {}
         #
         try:
             selfList, sameSeqEntryList = self.__sepsUtil.searchSameSequenceEntity(entryId=dataSetId, seq=eD["SEQ_ENTITY_1"])
             selfInfoMap = {}
             sameSeqInfoMap = {}
             if (len(selfList) > 0) or (len(sameSeqEntryList) > 0):
                 partsTaxIdInfoList = []
                 for (partNo, pD) in enumerate(eD["PART_LIST"], start=1):
-                    if ("SOURCE_TAXID" in pD) and pD["SOURCE_TAXID"] and ("SEQ_NUM_BEG" in pD) and pD["SEQ_NUM_BEG"] and \
-                       ("SEQ_NUM_END" in pD) and pD["SEQ_NUM_END"]:
+                    if ("SOURCE_TAXID" in pD) and pD["SOURCE_TAXID"] and ("SEQ_NUM_BEG" in pD) and pD["SEQ_NUM_BEG"] and ("SEQ_NUM_END" in pD) and pD["SEQ_NUM_END"]:
                         partsTaxIdInfoList.append([str(partNo), pD["SEQ_NUM_BEG"], pD["SEQ_NUM_END"], "", pD["SOURCE_TAXID"]])
                     elif (len(eD["PART_LIST"]) == 1) and ("SOURCE_TAXID" in pD) and pD["SOURCE_TAXID"]:
                         partsTaxIdInfoList.append([str(partNo), "", "", "", pD["SOURCE_TAXID"]])
                     #
                 #
                 annObj = GetSameSeqAnnotation(siteId=self.__siteId, sessionPath=self.__sessionPath, pathInfo=self.__pI, verbose=self.__verbose, log=self.__lfh)
                 annObj.setEntitySeq(seq=eD["SEQ_ENTITY_1"], polyTypeCode=eD["POLYMER_TYPE_CODE"])
                 if len(selfList) > 0:
-                    selfInfoMap = annObj.getSeqAnnotationFromAssignFile(retList=selfList, authPartsTaxIdInfoList=partsTaxIdInfoList,
-                                                                        authRefList=authRefList, includeSelfRef=True)
+                    selfInfoMap = annObj.getSeqAnnotationFromAssignFile(retList=selfList, authPartsTaxIdInfoList=partsTaxIdInfoList, includeSelfRef=True)
                 #
                 if len(sameSeqEntryList) > 0:
-                    sameSeqInfoMap = annObj.getSeqAnnotationFromAssignFile(retList=sameSeqEntryList, authPartsTaxIdInfoList=partsTaxIdInfoList,
-                                                                           authRefList=authRefList)
+                    sameSeqInfoMap = annObj.getSeqAnnotationFromAssignFile(retList=sameSeqEntryList, authPartsTaxIdInfoList=partsTaxIdInfoList)
                 #
             #
             return selfInfoMap, sameSeqInfoMap
         except:  # noqa: E722 pylint: disable=bare-except
             traceback.print_exc(file=self.__lfh)
             return {}, {}
         #
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/SequenceAssign.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/SequenceAssign.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/SequenceExamples.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/SequenceExamples.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/SequenceFeatureDepict.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/SequenceFeatureDepict.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 ##
 # File:    SequenceFeatureDepict.py
 # Date:    03-Mar-2013
 #
 # Updates:
 # 10-Nov-2013  -- Add entity detail dictionary markup
-# 19-Oct-2022  zf add author provided reference sequence information
-#
 ##
 """
 Convenience methods to markup sequence features.
 
 """
 __docformat__ = "restructuredtext en"
 __author__ = "John Westbrook"
@@ -37,40 +35,30 @@
             dbAccession=self.__fD["DB_ACCESSION"],
             dbIsoForm=self.__fD["DB_ISOFORM"],
             seqAltId=seqAltId,
             entryId=self.__fD["REF_ENTRY_ID"],
             entityId=self.__fD["REF_ENTRY_ENTITY_ID"],
             statusCode=self.__fD["REF_ENTRY_STATUS"],
             annInitial=self.__fD["REF_ENTRY_ANN"],
-            isAuthProvidedId=self.__fD["IS_AUTH_PROVIDED_ID"]
         )
 
     def __markupDatabaseReferenceWithUrl(
-        self, dbName, dbAccession, dbIsoForm="", seqAltId=0, entryId="", entityId="", statusCode="", annInitial="", isAuthProvidedId=False
+        self, dbName, dbAccession, dbIsoForm="", seqAltId=0, entryId="", entityId="", statusCode="", annInitial=""
     ):  # pylint: disable=unused-argument
 
-        style = ""
-        span_start = ""
-        span_end = ""
-        if isAuthProvidedId:
-            style = 'style="color:green;"'
-            span_start = '<span style="color:green;">'
-            span_end = '</span>'
-        #
         displayCode = dbAccession
         if len(dbIsoForm) > 0:
             displayCode = dbIsoForm
         #
         if dbName in ["UNP", "SP", "TR"]:
-            lab = '<a href="http://www.uniprot.org/uniprot/%s" target="blank"><span %s class="nowrap">%s</span></a>' \
-                  % (dbAccession, style, dbName + ":" + displayCode)
-#       elif dbName in ["GENBANK", "GB"]:
-#           lab = dbName + ":" + displayCode
+            lab = '<a href="http://www.uniprot.org/uniprot/%s" target="blank"><span class="nowrap">%s</span></a>' % (dbAccession, dbName + ":" + displayCode)
+        elif dbName in ["GENBANK", "GB"]:
+            lab = dbName + ":" + displayCode
         else:
-            lab = span_start + dbName + ":" + displayCode + span_end
+            lab = dbName + ":" + displayCode
         #
         if entryId:
             lab += "<br/><br/>From:<br/>DepID:" + entryId + "<br/>EntityID:" + entityId + "<br/>Status:" + statusCode + "<br/>Ann:" + annInitial
         #
         return lab
 
     # def markupAuthorFeatures(self):
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/SequenceLabel.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/SequenceLabel.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,14 @@
 #  10-Sep-2014 jdw add  method getPartInfo()
 #  25-Nov-2014 jdw return source + strain from __getstrain()
 #  01-Feb-2015 jdw add host org variant
 #  07-Sep-2017 zf  add ALIGN_LENGTH, ANNO_EDIT_DB_NAME, ANNO_EDIT_DB_CODE, ANNO_EDIT_DB_ACCESSION, ANNO_EDIT_DB_ALIGN_BEGIN,
 #                  ANNO_EDIT_DB_ALIGN_END
 #                  updated updateAuth() to keep original author's molecular name for DNA/RNA entities if existing
 #  02-Sep-2020 zf  Excluded 'Uncharacterized protein' molecule name from Uniprot
-#  03-Oct-2022 zf  Excluded "SOURCE_STRAIN" from updateAuth() method.
-#                  add IS_AUTH_PROVIDED_ID
 ##
 """
 Containers for sequence and residue labels/features used as identifiers and classifiers
 of aligned sequence data.
 
 """
 __docformat__ = "restructuredtext en"
@@ -69,15 +67,15 @@
         """Map editable reference values to current author values --"""
         mapTupList = [
             ("ENTITY_DESCRIPTION", "DB_MOLECULE_NAME"),
             ("ENTITY_SYNONYMS", "DB_MOLECULE_SYNONYMS"),
             ("SOURCE_GENE_NAME", "DB_GENE_NAME"),
             # ('SOURCE_TAXID', 'SOURCE_TAXID'),
             # ('SOURCE_ORGANISM', 'SOURCE_ORGANISM'),
-            # ("SOURCE_STRAIN", "SOURCE_STRAIN"),
+            ("SOURCE_STRAIN", "SOURCE_STRAIN"),
             # ('SOURCE_COMMON_NAME', 'SOURCE_COMMON_NAME'),
             ("ENTITY_ENZYME_CLASS", "DB_MOLECULE_EC"),
         ]
         if self.__debug:
             for mapTup in mapTupList:
                 self.__lfh.write("++++Before Mapping %30s : %-40r  %30s:  %r\n" % (mapTup[0], authFD[mapTup[0]], mapTup[1], refFD[mapTup[0]]))
         #
@@ -260,15 +258,15 @@
             "AUTH_SEQ_NUM_END_ORIG",
             "AUTH_SEQ_PART_ID",
             "REF_SORT_ORDER_INDEX",
             "AUTH_SEQ_PART_ID_ORIG",
         ]
 
         self.__fListFloat = ["AUTH_XYZ_SEQ_SIM", "AUTH_XYZ_SEQ_SIM_WITH_GAPS", "AUTH_REF_SEQ_SIM", "AUTH_REF_SEQ_SIM_WITH_GAPS", "AUTH_REF_SEQ_SIM_BLAST", "REF_SORT_METRIC"]
-        self.__fListBool = ["HAS_MANUAL_EDIT", "IS_AUTH_PROVIDED_ID"]
+        self.__fListBool = ["HAS_MANUAL_EDIT"]
 
         # self.__fIndex={k:k for k in  self.__fListStr + self.__fListInt + self.__fListBool}
         self.__fD = {}
         self.__reset()
 
     def __reset(self):
         self.__fD = {}
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/SequenceReferenceData.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/SequenceReferenceData.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/util/UpdateSequenceDataStoreUtils.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/util/UpdateSequenceDataStoreUtils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 ##
 # File:  UpdateSequenceDataStoreUtils.py
 # Date:  23-Nov-2018
 #
-# Updates:
-#  03-Oct-2022 zf  improve the handling for author provided reference sequence information
-#
 ##
 """
 Wrap class to update SequenceDataStore storage
 
 """
 __docformat__ = "restructuredtext en"
 __author__ = "Zukang Feng"
@@ -20,15 +17,15 @@
 import os
 import sys
 import traceback
 
 from wwpdb.apps.seqmodule.io.SequenceDataStore import SequenceDataStore
 from wwpdb.apps.seqmodule.util.SequenceLabel import SequenceLabel, SequenceFeature
 from wwpdb.io.file.mmCIFUtil import mmCIFUtil
-from wwpdb.io.locator.ChemRefPathInfo import ChemRefPathInfo
+from wwpdb.utils.config.ConfigInfoApp import ConfigInfoAppCommon
 
 
 class UpdateSequenceDataStoreUtils(object):
     """ """
 
     def __init__(self, reqObj=None, seqDataStore=None, verbose=False, log=sys.stderr):
         """ """
@@ -183,29 +180,30 @@
         """
         entityD = {}
         verList = self.getVersionIdList("auth", entityId, 1, 1)
         if len(verList) == 0:
             return "", entityD
         #
         siteId = str(self._reqObj.getValue("WWPDB_SITE_ID"))
+        cICommon = ConfigInfoAppCommon(siteId)
+        ccPath = cICommon.get_site_cc_cvs_path()
         #
         sTupL = self.getSequence("auth", entityId, 1, 1, verList[0])
         r1L = []
         r1L_CAN = []
         r1L_SEARCH = []
         for sTup in sTupL:
             r1L_CAN.append(sTup[4])
             if sTup[4] == "X":
                 r1L.append("(" + sTup[0] + ")")
                 #
                 ccCode = ""
                 ccId = sTup[0].upper()
-                crpi = ChemRefPathInfo(siteId=siteId, verbose=self._verbose, log=self._lfh)
-                ccFilePath = crpi.getFilePath(ccId, "CC")
-                if ccFilePath and os.access(ccFilePath, os.F_OK):
+                ccFilePath = os.path.join(ccPath, ccId[0], ccId, ccId + ".cif")
+                if os.access(ccFilePath, os.F_OK):
                     cifObj = mmCIFUtil(filePath=ccFilePath)
                     ccCode = cifObj.GetSingleValue("chem_comp", "one_letter_code")
                 #
                 if ccCode:
                     r1L_SEARCH.append(ccCode)
                 else:
                     r1L_SEARCH.append(sTup[4])
@@ -374,50 +372,28 @@
     def setSingleEntityRefSequenceInfo(self, eId, eD, eRefD, ownRefD, eSSRefD):
         """Load reference sequence(s) and features for single entity"""
         ref_label = {}
         ref_align_index = {}
         sId = eD["ENTITY_ID"]
         for (partNo, pD) in enumerate(eD["PART_LIST"], start=1):
             rList = []
-            autoList = []
             selfRefFlag = False
             if (eId in eRefD) and eRefD[eId] and (str(partNo) in eRefD[eId]) and eRefD[eId][str(partNo)]:
                 rList = eRefD[eId][str(partNo)]
-#               for refD in eRefD[eId][str(partNo)]:
-#                   if ("auto_match_status" in refD) and refD["auto_match_status"]:
-#                       autoList.append(refD)
-#                   else:
-#                       rList.append(refD)
-#                   #
-#               #
             #
             if (eId in eSSRefD) and eSSRefD[eId] and (str(partNo) in eSSRefD[eId]) and eSSRefD[eId][str(partNo)] and ("selfref" not in eSSRefD[eId][str(partNo)]):
-                # rList.append(eSSRefD[eId][str(partNo)])
-                if ("auto_match_status" in eSSRefD[eId][str(partNo)]) and eSSRefD[eId][str(partNo)]["auto_match_status"]:
-                    autoList.append(eSSRefD[eId][str(partNo)])
-                else:
-                    rList.append(eSSRefD[eId][str(partNo)])
-                #
+                rList.append(eSSRefD[eId][str(partNo)])
             #
             if (eId in ownRefD) and ownRefD[eId] and (str(partNo) in ownRefD[eId]) and ownRefD[eId][str(partNo)]:
                 if ("selfref" in ownRefD[eId][str(partNo)]) and ownRefD[eId][str(partNo)]["selfref"]:
                     selfRefFlag = True
                 else:
-                    # rList.append(ownRefD[eId][str(partNo)])
-                    if ("auto_match_status" in ownRefD[eId][str(partNo)]) and ownRefD[eId][str(partNo)]["auto_match_status"]:
-                        autoList.append(ownRefD[eId][str(partNo)])
-                    else:
-                        rList.append(ownRefD[eId][str(partNo)])
-                    #
+                    rList.append(ownRefD[eId][str(partNo)])
                 #
             #
-            # put auto_match_status=True references at the bottom
-            if len(autoList) > 0:
-                rList.extend(autoList)
-            #
             if (len(rList) > 0) and (not selfRefFlag):
                 if ("statistics" in rList[-1]) and (rList[-1]["statistics"][2] > 0.899999):
                     self.__seqLabel.set(seqType="ref", seqInstId=sId, seqPartId=partNo, seqAltId=len(rList), seqVersion=1)
                     self.__defSelList.append(self.__seqLabel.pack())
                     ref_label[partNo] = [self.__seqLabel.pack()]
                     self._entityAlignInfoMap[sId]["alignids"].append(self.__seqLabel.pack())
                 else:
@@ -577,17 +553,14 @@
         # For 100% sequence match previous processed entry
         #
         for item in ("REF_ENTRY_ID", "REF_ENTRY_ENTITY_ID", "REF_ENTRY_STATUS", "REF_ENTRY_ANN"):
             if item in rD:
                 self.__seqFeature.setItem(item, rD[item])
             #
         #
-        if "author_provided_id" in rD:
-            self.__seqFeature.setItem("IS_AUTH_PROVIDED_ID", rD["author_provided_id"])
-        #
         return self.__seqFeature
 
     def mergePartialAnnotatedResult(self, newOldEntityIdMap, dataStoreFile):
         """Merge previous partial SequenceDataStore object values into current SequenceDataStore object"""
         if (not newOldEntityIdMap) or (not dataStoreFile) or (not os.access(dataStoreFile, os.R_OK)):
             return
         #
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/view3d/ModelViewer3D.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/view3d/ModelViewer3D.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/webapp/SeqModWebApp_v2.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/webapp/SeqModWebApp_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -43,15 +43,14 @@
 # 20-Apr-2014  jdw update input export file copy operations -
 # 28-Apr-2014  jdw retire DataImporter.updateData*  modules
 # 14-May-2014  jdw assign any missing aligntag to the current entity group
 # 22-May-2014  jdw new alignment protocol -- push entry details in summary update response
 #  8-Jul-2014  jdw export group id list in the summary view return object
 #  2-Dec-2014  jdw capture updates in selection and alignment id lists after alignment edits --
 # 24-Aug-2017  zf  add '/service/sequence_editor/rerun_blast/start' & _reRunBlastOp for rerun blast search
-# 19-Oct-2022  zf  add __getSummaryPageContent() method
 ##
 #    WF Testing entry points -
 #
 #   /service/sequence_editor/new_session/wf?classID=AnnMod&identifier=D_1000000000&filesource=wf-archive&instance=W_000
 #   /service/sequence_editor/new_session/wf?classID=AnnMod&identifier=D_1000000001&filesource=wf-archive&instance=W_000
 ##
 """
@@ -947,18 +946,14 @@
                         warningMsg += "Sequences not matched to existing entries in entity: " + warningD["not_found_existing_match"][0]
                     #
                 #
                 if warningMsg:
                     rC.set("entrywarningmessage", warningMsg)
                 #
             #
-            # Set summary page content
-            #
-            rC.set("summaryinfo", self.__getSummaryPageContent(sV.getSummaryPageObj()))
-            #
             #  Reset --
             #
             self.__reqObj.setNewRefId("")
         except:  # noqa: E722 pylint: disable=bare-except
             rC.setError(errMsg="Sequence alignment summary preparation has failed.")
             rC.setStatusCode("failed")
             if self.__verbose:
@@ -1007,61 +1002,14 @@
             if outputText:
                 outputText += "</br>\n"
             #
             outputText += inputText[rangeTup[0] : rangeTup[1]]
         #
         return outputText
 
-    def __getSummaryPageContent(self, spObj):
-        """ Generate summary page content
-        """
-        columnNameKeyList = (("Entity", "entity_id"), ("Chain", "chain_ids"), ("Type", "entity_types"),
-                             ("Molecule name<br/>(Depositor-provided name)", "mol_names"),
-                             ("Source name/strain<br/>(Depositor-provided source name)", "source_names"),
-                             ("Source TaxID<br/>(Depositor-provided TaxID)", "tax_ids"),
-                             ("Scores", "identity_scores"),
-                             ("Top hit ID [TaxID]<br/>(Depositor-provided ID)", "ref_db_ids"),
-                             ("Mismatch and differences", "warn_err_msgs"))
-        #
-        oL = []
-        oL.append('<table class="summary_table">\n')
-        oL.append("<thead>\n")
-        oL.append("<tr>")
-        for columnNameKeTuple in columnNameKeyList:
-            oL.append("<th>%s</th>" % columnNameKeTuple[0])
-        #
-        oL.append("</tr>\n")
-        oL.append("</thead>\n")
-        oL.append("<tbody>\n")
-        #
-        gIdList = list(spObj.keys())
-        gIdList.sort(key=int)
-        oddEven = True
-        for gId in gIdList:
-            gObj = spObj[gId]
-            if oddEven:
-                oL.append('<tr class="odd">')
-                oddEven = False
-            else:
-                oL.append('<tr class="even">')
-                oddEven = True
-            #
-            for columnNameKeTuple in columnNameKeyList:
-                if columnNameKeTuple[1] in gObj:
-                    oL.append("<td>%s</td>" % gObj[columnNameKeTuple[1]])
-                else:
-                    oL.append("<td>-</td>")
-                #
-            #
-            oL.append("</tr>\n")
-        #
-        oL.append("</tbody>\n")
-        oL.append("</table>\n")
-        return "".join(oL)
-
     def __storeAlignmentStart(self):
         """Launch a subprocess to compute, store and render the aligned input sequence list."""
         #
         self.__getSession(useContext=True)
         _sessionId = self.__reqObj.getSessionId()  # noqa: F841
         alignTag = self.__reqObj.getValue("aligntag")
         operation = self.__reqObj.getValue("operation")
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb/apps/seqmodule/webapp/SeqModWebRequest.py` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb/apps/seqmodule/webapp/SeqModWebRequest.py`

 * *Files identical despite different names*

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb.apps.seqmodule.egg-info/PKG-INFO` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb.apps.seqmodule.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.apps.seqmodule
-Version: 0.24.9.dev1
+Version: 0.24.dev1
 Summary: wwPDB sequence module
 Home-page: https://github.com/wwPDB/py-wwpdb_apps_seqmodule
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.apps.seqmodule-0.24.9.dev1/wwpdb.apps.seqmodule.egg-info/SOURCES.txt` & `wwpdb.apps.seqmodule-0.24.dev1/wwpdb.apps.seqmodule.egg-info/SOURCES.txt`

 * *Files identical despite different names*

