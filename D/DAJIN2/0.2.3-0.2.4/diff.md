# Comparing `tmp/DAJIN2-0.2.3.tar.gz` & `tmp/DAJIN2-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DAJIN2-0.2.3.tar", last modified: Tue Jun  6 00:10:51 2023, max compression
+gzip compressed data, was "DAJIN2-0.2.4.tar", last modified: Tue Jun 13 04:33:34 2023, max compression
```

## Comparing `DAJIN2-0.2.3.tar` & `DAJIN2-0.2.4.tar`

### file list

```diff
@@ -1,67 +1,66 @@
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:51.170600 DAJIN2-0.2.3/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1069 2023-06-04 20:44:56.000000 DAJIN2-0.2.3/LICENSE
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       90 2023-06-04 20:44:56.000000 DAJIN2-0.2.3/MANIFEST.in
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3406 2023-06-06 00:10:51.164599 DAJIN2-0.2.3/PKG-INFO
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2918 2023-06-04 20:44:56.000000 DAJIN2-0.2.3/README.md
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       38 2023-06-06 00:10:51.171599 DAJIN2-0.2.3/setup.cfg
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1078 2023-06-06 00:09:45.000000 DAJIN2-0.2.3/setup.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:49.622909 DAJIN2-0.2.3/src/
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:49.889693 DAJIN2-0.2.3/src/DAJIN2/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 08:26:28.000000 DAJIN2-0.2.3/src/DAJIN2/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3832 2023-06-05 08:08:39.000000 DAJIN2-0.2.3/src/DAJIN2/batch.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:50.080675 DAJIN2-0.2.3/src/DAJIN2/core/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/__init__.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:50.179232 DAJIN2-0.2.3/src/DAJIN2/core/classification/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      124 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/classification/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3076 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/classification/classify.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      509 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/classification/detect_sv.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:50.336219 DAJIN2-0.2.3/src/DAJIN2/core/clustering/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      147 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/clustering/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6938 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/clustering/clustering.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2791 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/clustering/make_score.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1566 2023-06-04 20:45:00.000000 DAJIN2-0.2.3/src/DAJIN2/core/clustering/merge_clusters.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4239 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/clustering/return_labels.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:50.443841 DAJIN2-0.2.3/src/DAJIN2/core/consensus/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      311 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/consensus/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5873 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/consensus/consensus.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      312 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/consensus/subset.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10880 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/core_execute.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:50.849408 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      472 2023-06-05 05:23:44.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4912 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/call_midsv.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7398 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/correct_knockin.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    10324 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/correct_sequence_error.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6054 2023-06-05 08:50:22.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1109 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/extract_knockin_loci.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7561 2023-06-05 08:52:41.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/extract_mutation_loci.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4356 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/format_inputs.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3755 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/mappy_align.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1787 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/replace_NtoD.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5139 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/preprocess/validate_inputs.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:50.957549 DAJIN2-0.2.3/src/DAJIN2/core/report/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       39 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/report/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    12958 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/report/report_bam.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1156 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/core/report/report_files.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2883 2023-06-05 08:39:04.000000 DAJIN2-0.2.3/src/DAJIN2/gui.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11054 2023-06-06 00:10:07.000000 DAJIN2-0.2.3/src/DAJIN2/main.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:51.015606 DAJIN2-0.2.3/src/DAJIN2/postprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/postprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2347 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/postprocess/report.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:51.072154 DAJIN2-0.2.3/src/DAJIN2/preprocess/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 08:06:47.000000 DAJIN2-0.2.3/src/DAJIN2/preprocess/__init__.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5436 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/preprocess/validate_inputs.py
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1127 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/single.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:49.691078 DAJIN2-0.2.3/src/DAJIN2/static/
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:51.104815 DAJIN2-0.2.3/src/DAJIN2/static/css/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       27 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/static/css/style.css
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1901 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/template_igvjs.html
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:51.135942 DAJIN2-0.2.3/src/DAJIN2/templates/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1777 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/templates/index.html
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2797 2023-06-04 20:45:01.000000 DAJIN2-0.2.3/src/DAJIN2/view.py
-drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-06 00:10:50.028115 DAJIN2-0.2.3/src/DAJIN2.egg-info/
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3406 2023-06-06 00:10:49.000000 DAJIN2-0.2.3/src/DAJIN2.egg-info/PKG-INFO
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1743 2023-06-06 00:10:49.000000 DAJIN2-0.2.3/src/DAJIN2.egg-info/SOURCES.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        1 2023-06-06 00:10:49.000000 DAJIN2-0.2.3/src/DAJIN2.egg-info/dependency_links.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)       47 2023-06-06 00:10:49.000000 DAJIN2-0.2.3/src/DAJIN2.egg-info/entry_points.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)      237 2023-06-06 00:10:49.000000 DAJIN2-0.2.3/src/DAJIN2.egg-info/requires.txt
--rwxrwxrwx   0 kuno      (1000) kuno      (1000)        7 2023-06-06 00:10:49.000000 DAJIN2-0.2.3/src/DAJIN2.egg-info/top_level.txt
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:34.150776 DAJIN2-0.2.4/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1069 2023-06-04 20:44:56.000000 DAJIN2-0.2.4/LICENSE
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       90 2023-06-04 20:44:56.000000 DAJIN2-0.2.4/MANIFEST.in
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3767 2023-06-13 04:33:34.147775 DAJIN2-0.2.4/PKG-INFO
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3199 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/README.md
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       38 2023-06-13 04:33:34.150776 DAJIN2-0.2.4/setup.cfg
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1150 2023-06-13 04:32:42.000000 DAJIN2-0.2.4/setup.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:32.471855 DAJIN2-0.2.4/src/
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:32.739585 DAJIN2-0.2.4/src/DAJIN2/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 08:26:28.000000 DAJIN2-0.2.4/src/DAJIN2/__init__.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:32.950507 DAJIN2-0.2.4/src/DAJIN2/core/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/__init__.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:33.060284 DAJIN2-0.2.4/src/DAJIN2/core/classification/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      124 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/classification/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3076 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/classification/classify.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      509 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/classification/detect_sv.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:33.246900 DAJIN2-0.2.4/src/DAJIN2/core/clustering/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      147 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/clustering/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6938 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/clustering/clustering.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2791 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/clustering/make_score.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1566 2023-06-04 20:45:00.000000 DAJIN2-0.2.4/src/DAJIN2/core/clustering/merge_clusters.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3824 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/src/DAJIN2/core/clustering/return_labels.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:33.396723 DAJIN2-0.2.4/src/DAJIN2/core/consensus/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      409 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/src/DAJIN2/core/consensus/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5930 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/src/DAJIN2/core/consensus/consensus.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2513 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/src/DAJIN2/core/consensus/extract_mutation_loci_by_labels.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      312 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/core/consensus/subset.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11018 2023-06-12 07:18:55.000000 DAJIN2-0.2.4/src/DAJIN2/core/core_execute.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:33.740810 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      367 2023-06-12 07:12:52.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5418 2023-06-12 07:18:55.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/call_midsv.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      917 2023-06-12 07:02:39.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/check_caches.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     6116 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1109 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/extract_knockin_loci.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     7157 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/extract_mutation_loci.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     4437 2023-06-08 03:17:27.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/format_inputs.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3755 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/mappy_align.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1787 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/core/preprocess/replace_NtoD.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:33.927117 DAJIN2-0.2.4/src/DAJIN2/core/report/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       86 2023-06-07 21:49:16.000000 DAJIN2-0.2.4/src/DAJIN2/core/report/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5125 2023-06-08 04:18:39.000000 DAJIN2-0.2.4/src/DAJIN2/core/report/remove_microhomology.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     8324 2023-06-12 07:18:55.000000 DAJIN2-0.2.4/src/DAJIN2/core/report/report_bam.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1156 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/core/report/report_files.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1565 2023-06-07 21:55:43.000000 DAJIN2-0.2.4/src/DAJIN2/core/report/reverse_sam.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2883 2023-06-05 08:39:04.000000 DAJIN2-0.2.4/src/DAJIN2/gui.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)    11137 2023-06-12 07:09:09.000000 DAJIN2-0.2.4/src/DAJIN2/main.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:33.992717 DAJIN2-0.2.4/src/DAJIN2/postprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/postprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2347 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/postprocess/report.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:34.053552 DAJIN2-0.2.4/src/DAJIN2/preprocess/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-05 08:06:47.000000 DAJIN2-0.2.4/src/DAJIN2/preprocess/__init__.py
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     5440 2023-06-12 03:47:36.000000 DAJIN2-0.2.4/src/DAJIN2/preprocess/validate_inputs.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:32.557038 DAJIN2-0.2.4/src/DAJIN2/static/
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:34.086588 DAJIN2-0.2.4/src/DAJIN2/static/css/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       27 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/static/css/style.css
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1901 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/template_igvjs.html
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:34.121250 DAJIN2-0.2.4/src/DAJIN2/templates/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1777 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/templates/index.html
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     2797 2023-06-04 20:45:01.000000 DAJIN2-0.2.4/src/DAJIN2/view.py
+drwxrwxrwx   0 kuno      (1000) kuno      (1000)        0 2023-06-13 04:33:32.890881 DAJIN2-0.2.4/src/DAJIN2.egg-info/
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     3767 2023-06-13 04:33:31.000000 DAJIN2-0.2.4/src/DAJIN2.egg-info/PKG-INFO
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)     1746 2023-06-13 04:33:32.000000 DAJIN2-0.2.4/src/DAJIN2.egg-info/SOURCES.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        1 2023-06-13 04:33:31.000000 DAJIN2-0.2.4/src/DAJIN2.egg-info/dependency_links.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)       47 2023-06-13 04:33:31.000000 DAJIN2-0.2.4/src/DAJIN2.egg-info/entry_points.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)      237 2023-06-13 04:33:31.000000 DAJIN2-0.2.4/src/DAJIN2.egg-info/requires.txt
+-rwxrwxrwx   0 kuno      (1000) kuno      (1000)        7 2023-06-13 04:33:31.000000 DAJIN2-0.2.4/src/DAJIN2.egg-info/top_level.txt
```

### Comparing `DAJIN2-0.2.3/LICENSE` & `DAJIN2-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.3/PKG-INFO` & `DAJIN2-0.2.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: DAJIN2
-Version: 0.2.3
-Summary: One-step genotyping tools for Nanopore amplicon sequencing
+Version: 0.2.4
+Summary: One-step genotyping tools for Targeted long-read sequencing
 Home-page: https://github.com/akikuno/DAJIN2
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![License](https://img.shields.io/badge/License-MIT-9cf.svg?style=flat-square)](https://choosealicense.com/licenses/mit/)
 [![PyPI](https://img.shields.io/pypi/v/DAJIN2.svg?label=PyPI&color=orange&style=flat-square)](https://pypi.org/project/DAJIN2/)
+[![Python](https://img.shields.io/pypi/pyversions/DAJIN2.svg?label=Python&color=blue&style=flat-square)](https://pypi.org/project/DAJIN2/)
 
 ⚠️ DAJIN2 is currently under development ⚠️
 
 Expected to be available the stable version in August 2023 🤞
 
 ## Installation (alpha-version)
 
@@ -76,15 +78,15 @@
 # 2023-06-04 11:35:01: Consensus calling single/barcode25.fq.gz...
 # 2023-06-04 11:35:08: 🍵 single/barcode25.fq.gz is finished!
 # 🎉 Finished! Open DAJINResults/stx2-deletion to see the report.
 ```
 
 ### Batch-mode
 
-DAJIN2 can handle multiple FASTQ files via `batch` subcommand.
+DAJIN2 can handle multiple FASTQ files using the `batch' subcommand.
 
 ```bash
 DAJIN2 batch [-h] -f FILE [-t THREADS]
 
 options:
   -h, --help            Show this help message and exit
   -f FILE, --file FILE  CSV or Excel file
@@ -92,10 +94,23 @@
                         Number of threads [default: 1]
 ```
 
 #### Example
 
 🚧 Working in progress 🚧
 
-## Reference
+### GUI-mode
 
-Kuno A, Ikeda Y, Ayabe S, Kato K, Sakamoto K, et al. (2022) DAJIN enables multiplex genotyping to simultaneously validate intended and unintended target genome editing outcomes. PLOS Biology 20(1): e3001507. https://doi.org/10.1371/journal.pbio.3001507
+You can use DAJIN2 with a graphical user interface (GUI) via the `gui` subcommand.
+
+```bash
+DAJIN2 gui
+```
+
+#### Example
+
+🚧 Working in progress 🚧
+
+
+## References
+
+[Kuno A, et al. (2022) DAJIN enables multiplex genotyping to simultaneously validate intended and unintended target genome editing outcomes. *PLoS Biology* 20(1): e3001507.](https://doi.org/10.1371/journal.pbio.3001507)
```

### Comparing `DAJIN2-0.2.3/README.md` & `DAJIN2-0.2.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 [![License](https://img.shields.io/badge/License-MIT-9cf.svg?style=flat-square)](https://choosealicense.com/licenses/mit/)
 [![PyPI](https://img.shields.io/pypi/v/DAJIN2.svg?label=PyPI&color=orange&style=flat-square)](https://pypi.org/project/DAJIN2/)
+[![Python](https://img.shields.io/pypi/pyversions/DAJIN2.svg?label=Python&color=blue&style=flat-square)](https://pypi.org/project/DAJIN2/)
 
 ⚠️ DAJIN2 is currently under development ⚠️
 
 Expected to be available the stable version in August 2023 🤞
 
 ## Installation (alpha-version)
 
@@ -61,15 +62,15 @@
 # 2023-06-04 11:35:01: Consensus calling single/barcode25.fq.gz...
 # 2023-06-04 11:35:08: 🍵 single/barcode25.fq.gz is finished!
 # 🎉 Finished! Open DAJINResults/stx2-deletion to see the report.
 ```
 
 ### Batch-mode
 
-DAJIN2 can handle multiple FASTQ files via `batch` subcommand.
+DAJIN2 can handle multiple FASTQ files using the `batch' subcommand.
 
 ```bash
 DAJIN2 batch [-h] -f FILE [-t THREADS]
 
 options:
   -h, --help            Show this help message and exit
   -f FILE, --file FILE  CSV or Excel file
@@ -77,10 +78,23 @@
                         Number of threads [default: 1]
 ```
 
 #### Example
 
 🚧 Working in progress 🚧
 
-## Reference
+### GUI-mode
 
-Kuno A, Ikeda Y, Ayabe S, Kato K, Sakamoto K, et al. (2022) DAJIN enables multiplex genotyping to simultaneously validate intended and unintended target genome editing outcomes. PLOS Biology 20(1): e3001507. https://doi.org/10.1371/journal.pbio.3001507
+You can use DAJIN2 with a graphical user interface (GUI) via the `gui` subcommand.
+
+```bash
+DAJIN2 gui
+```
+
+#### Example
+
+🚧 Working in progress 🚧
+
+
+## References
+
+[Kuno A, et al. (2022) DAJIN enables multiplex genotyping to simultaneously validate intended and unintended target genome editing outcomes. *PLoS Biology* 20(1): e3001507.](https://doi.org/10.1371/journal.pbio.3001507)
```

### Comparing `DAJIN2-0.2.3/setup.py` & `DAJIN2-0.2.4/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,30 @@
 long_description = (this_directory / "README.md").read_text()
 
 with open("requirements.txt") as requirements_file:
     install_requirements = requirements_file.read().splitlines()
 
 setuptools.setup(
     name="DAJIN2",
-    version="0.2.3",
+    version="0.2.4",
     author="Akihiro Kuno",
     author_email="akuno@md.tsukuba.ac.jp",
-    description="One-step genotyping tools for Nanopore amplicon sequencing",
+    description="One-step genotyping tools for Targeted long-read sequencing",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/akikuno/DAJIN2",
     install_requires=install_requirements,
     packages=setuptools.find_packages(
         where="src",
     ),
     package_dir={"": "src"},
     entry_points={"console_scripts": ["DAJIN2=DAJIN2.main:execute"]},
     include_package_data=True,
     classifiers=[
-        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
         "License :: OSI Approved :: MIT License",
         "Operating System :: POSIX",
         "Development Status :: 3 - Alpha",
     ],
-    python_requires=">=3.7",
 )
```

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/classification/classify.py` & `DAJIN2-0.2.4/src/DAJIN2/core/classification/classify.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/clustering/clustering.py` & `DAJIN2-0.2.4/src/DAJIN2/core/clustering/clustering.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/clustering/make_score.py` & `DAJIN2-0.2.4/src/DAJIN2/core/clustering/make_score.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/clustering/merge_clusters.py` & `DAJIN2-0.2.4/src/DAJIN2/core/clustering/merge_clusters.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/clustering/return_labels.py` & `DAJIN2-0.2.4/src/DAJIN2/core/clustering/return_labels.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 ###############################################################################
 # Dimension reduction
 ###############################################################################
 
 
 def reduce_dimension(scores_sample: Generator[list], scores_control: Generator[list]) -> np.array:
     scores = list(chain(scores_sample, scores_control))
-    pca = PCA(n_components=20).fit(scores)
+    pca = PCA(n_components=min(20, len(scores))).fit(scores)
     return pca.transform(scores)
 
 
 def optimize_labels(X: np.array, coverage_sample, coverage_control) -> list[int]:
     n_components = min(20, coverage_sample + coverage_control)
     for i in range(1, n_components):
         np.random.seed(seed=1)
@@ -69,38 +69,28 @@
 
 
 ###############################################################################
 # main
 ###############################################################################
 
 
+def get_label_most(labels: list[int]) -> int:
+    return Counter(labels).most_common()[0][0]
+
+
+def subset_scores(labels: list[int], scores: list[int], label_most: int, length: int = 1000) -> list[int]:
+    subset = [score for label, score in zip(labels, scores) if label == label_most]
+    return subset[:length]
+
+
 def return_labels(path_score_sample: Path | str, path_score_control: Path | str) -> list[int]:
     np.random.seed(seed=1)
-    # Remove abnormal minor reads from control
     X_control = reduce_dimension([], read_json(path_score_control))
+    # subset to 1000 reads of controls in the most common cluster to remove outliers and reduce computation time
     labels = GaussianMixture(n_components=2, random_state=1).fit_predict(X_control)
-    label_most = Counter(labels).most_common()[0][0]
-    # Subset control to 1000 reads
-    scores_control_subset = []
-    count = 0
-    for label, score in zip(labels, read_json(path_score_control)):
-        if label == label_most:
-            scores_control_subset.append(score)
-            count += 1
-        if count == 1000:
-            break
+    label_most = get_label_most(labels)
+    scores_control_subset = subset_scores(labels, read_json(path_score_control), label_most, 1000)
     X = reduce_dimension(read_json(path_score_sample), scores_control_subset)
     coverage_sample = count_newlines(path_score_sample)
     coverage_control = len(scores_control_subset)
     labels = optimize_labels(X, coverage_sample, coverage_control)
     return labels
-
-
-# def return_labels(scores_sample: Generator[list[float]], scores_control: Generator[list[float]]) -> list[int]:
-#     np.random.seed(seed=1)
-#     X_control = reduce_dimension([], scores_control)
-#     labels = GaussianMixture(n_components=2, random_state=1).fit_predict(X_control)
-#     label_most = Counter(labels).most_common()[0][0]
-#     scores_control_subset = [s for label, s in zip(labels, scores_control) if label == label_most][:1000]
-#     X = reduce_dimension(scores_sample, scores_control_subset)
-#     labels = optimize_labels(X, scores_sample, scores_control_subset)
-#     return labels
```

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/consensus/consensus.py` & `DAJIN2-0.2.4/src/DAJIN2/core/consensus/consensus.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,26 +92,27 @@
 
 
 ###########################################################
 # main
 ###########################################################
 
 
-def call_consensus(clust_sample: list[dict], MUTATION_LOCI_ALLELES) -> tuple[defaultdict[list], defaultdict[str]]:
+def call_consensus(clust_sample: list[dict], MUTATION_LOCI_LABELS) -> tuple[defaultdict[list], defaultdict[str]]:
     cons_percentage = defaultdict(list)
     cons_sequence = defaultdict(str)
     clust_sample.sort(key=lambda x: x["LABEL"])
-    for _, group in groupby(clust_sample, key=lambda x: x["LABEL"]):
+    for label, group in groupby(clust_sample, key=lambda x: x["LABEL"]):
         clust = list(group)
         keys = (
             clust[0]["ALLELE"],
             clust[0]["LABEL"],
             clust[0]["PERCENT"],
         )
-        mutation_loci = MUTATION_LOCI_ALLELES[clust[0]["ALLELE"]]
+        # mutation_loci = MUTATION_LOCI_ALLELES[clust[0]["ALLELE"]]
+        mutation_loci = MUTATION_LOCI_LABELS[label]
         cssplits = [cs["CSSPLIT"].split(",") for cs in clust]
         cons_per = _call_percentage(cssplits, mutation_loci)
         cons_per = _replace_percentage(cons_per)
         cons_seq = _call_sequence(cons_per)
         cons_percentage[keys] = cons_per
         cons_sequence[keys] = cons_seq
     return cons_percentage, cons_sequence
```

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/core_execute.py` & `DAJIN2-0.2.4/src/DAJIN2/core/core_execute.py`

 * *Files 4% similar despite different names*

```diff
@@ -46,19 +46,19 @@
     FASTA_ALLELES: dict = preprocess.format_inputs.dictionize_allele(ALLELE)
 
     TEMPDIR = Path("DAJINResults", ".tempdir", NAME)
     SUBDIRS = ["cache", "fasta", "sam", "midsv", "clustering", "report", "result", "mutation_loci"]
     SUBDIRS_REPORT = ["HTML", "FASTA", "BAM", ".igvjs"]
     preprocess.format_inputs.make_directories(TEMPDIR, SUBDIRS, SUBDIRS_REPORT, SAMPLE_NAME, CONTROL_NAME)
 
-    IS_CACHE_CONTROL = preprocess.validate_inputs.exists_cached_control(CONTROL, TEMPDIR)
-    IS_CACHE_GENOME = preprocess.validate_inputs.exists_cached_genome(GENOME, TEMPDIR, IS_CACHE_CONTROL)
+    IS_CACHE_CONTROL = preprocess.check_caches.exists_cached_control(CONTROL, TEMPDIR)
+    IS_CACHE_GENOME = preprocess.check_caches.exists_cached_genome(GENOME, TEMPDIR, IS_CACHE_CONTROL)
     if GENOME:
         if not IS_CACHE_GENOME:
-            GENOME_COODINATES = preprocess.format_inputs.fetch_coodinate(GENOME, URL_UCSC, FASTA_ALLELES["control"])
+            GENOME_COODINATES = preprocess.format_inputs.fetch_coordinate(GENOME, URL_UCSC, FASTA_ALLELES["control"])
             CHROME_SIZE = preprocess.format_inputs.fetch_chrom_size(GENOME_COODINATES["chr"], GENOME, URL_GOLDENPATH)
             preprocess.format_inputs.cache_coodinates_and_chromsize(TEMPDIR, GENOME, GENOME_COODINATES, CHROME_SIZE)
         else:
             GENOME_COODINATES = json.loads(Path(TEMPDIR, "cache", "genome_coodinates.jsonl").read_text())
             CHROME_SIZE = int(Path(TEMPDIR, "cache", "chrome_size.txt").read_text())
     return SAMPLE_NAME, CONTROL_NAME, FASTA_ALLELES, TEMPDIR, GENOME_COODINATES, CHROME_SIZE, THREADS
 
@@ -69,64 +69,65 @@
 
 def execute_control(arguments: dict):
     print(f"{_dtnow()}: {arguments['control']} is now processing...", file=sys.stderr)
     ###########################################################
     # Preprocess
     ###########################################################
     SAMPLE, CONTROL, ALLELE, NAME, THREADS, GENOME, _, _ = _parse_arguments(arguments)
-    # preprocess.validate_inputs.check_files(SAMPLE, CONTROL, ALLELE)
     _, CONTROL_NAME, FASTA_ALLELES, TEMPDIR, GENOME_COODINATES, CHROME_SIZE, THREADS = _format_inputs(arguments)
     ###########################################################
-    # Save Caches
+    # Check caches
     ###########################################################
     if Path(TEMPDIR, "report", "BAM", CONTROL_NAME, f"{CONTROL_NAME}.bam").exists():
         print(
             f"{arguments['control']} is already preprocessed and reuse the results for the current run...",
             file=sys.stderr,
         )
         return
     print(f"{_dtnow()}: Preprocess {arguments['control']}...", file=sys.stderr)
+    ###########################################################
+    # Mapping
+    ###########################################################
     # ============================================================
     # Export fasta files as single-FASTA format
     # ============================================================
     for identifier, sequence in FASTA_ALLELES.items():
         contents = "\n".join([">" + identifier, sequence]) + "\n"
         output_fasta = Path(TEMPDIR, "fasta", f"{identifier}.fasta")
         output_fasta.write_text(contents)
-    print(f"{_dtnow()}: Mapping {arguments['control']}...", file=sys.stderr)
     # ============================================================
     # Mapping using mappy
     # ============================================================
     for path_fasta in Path(TEMPDIR, "fasta").glob("*.fasta"):
         name_fasta = path_fasta.stem
         preprocess.mappy_align.output_sam(TEMPDIR, path_fasta, name_fasta, CONTROL, CONTROL_NAME, threads=THREADS)
         preprocess.mappy_align.output_sam(
             TEMPDIR, path_fasta, name_fasta, CONTROL, CONTROL_NAME, preset="splice", threads=THREADS
         )
-    # ============================================================
+    ###########################################################
     # MIDSV conversion
-    # ============================================================
-    print(f"{_dtnow()}: Call MIDSV {arguments['control']}...", file=sys.stderr)
+    ###########################################################
     preprocess.call_midsv(TEMPDIR, FASTA_ALLELES, CONTROL_NAME)
     ###########################################################
-    # Save MIDSV and BAM
+    # Output BAM
     ###########################################################
-    # with open(Path(TEMPDIR, "midsv", f"{arguments['control']}.plk"), 'wb') as p:
-    #     pickle.dump(midsv_control_alleles, p)
+    print(f"{_dtnow()}: Output BAM files of {arguments['control']}...", file=sys.stderr)
     report.report_bam.output_bam_control(TEMPDIR, CONTROL_NAME, GENOME, GENOME_COODINATES, CHROME_SIZE, THREADS)
+    ###########################################################
+    # Finish call
+    ###########################################################
     print(f"{_dtnow()}: \N{teacup without handle} {arguments['control']} is finished!", file=sys.stderr)
 
 
 def execute_sample(arguments: dict):
     print(f"{_dtnow()}: {arguments['sample']} is now processing...", file=sys.stderr)
     ###########################################################
     # Preprocess
     ###########################################################
     SAMPLE, CONTROL, ALLELE, NAME, THREADS, GENOME, _, _ = _parse_arguments(arguments)
-    # preprocess.validate_inputs.check_files(SAMPLE, CONTROL, ALLELE)
     SAMPLE_NAME, CONTROL_NAME, FASTA_ALLELES, TEMPDIR, GENOME_COODINATES, CHROME_SIZE, THREADS = _format_inputs(
         arguments
     )
     print(f"{_dtnow()}: Preprocess {arguments['sample']}...", file=sys.stderr)
     # ============================================================
     # Mapping with mappy
     # ============================================================
@@ -140,21 +141,17 @@
     # MIDSV conversion
     # ============================================================
     preprocess.call_midsv(TEMPDIR, FASTA_ALLELES, SAMPLE_NAME)
     # ============================================================
     # Extract mutation loci
     # ============================================================
     MUTATION_LOCI_ALLELES = preprocess.extract_mutation_loci(TEMPDIR, FASTA_ALLELES, SAMPLE_NAME, CONTROL_NAME)
+    KNOCKIN_LOCI_ALLELES = preprocess.extract_knockin_loci(TEMPDIR)
     with open(Path(TEMPDIR, "mutation_loci", f"{SAMPLE_NAME}.plk"), "wb") as p:
         pickle.dump(MUTATION_LOCI_ALLELES, p)
-    KNOCKIN_LOCI_ALLELES = preprocess.extract_knockin_loci(TEMPDIR)
-    # ============================================================
-    # CSSPLITS Error Correction
-    # ============================================================
-    # preprocess.correct_knockin.execute(TEMPDIR, FASTA_ALLELES, CONTROL_NAME, SAMPLE_NAME)
     ########################################################################
     # Classify alleles
     ########################################################################
     print(f"{_dtnow()}: Classify {arguments['sample']}...", file=sys.stderr)
     classif_sample = classification.classify_alleles(TEMPDIR, FASTA_ALLELES, SAMPLE_NAME)
     ########################################################################
     # Clustering
@@ -162,29 +159,33 @@
     print(f"{_dtnow()}: Clustering {arguments['sample']}...", file=sys.stderr)
     clust_sample = clustering.add_labels(
         classif_sample, TEMPDIR, SAMPLE_NAME, CONTROL_NAME, MUTATION_LOCI_ALLELES, KNOCKIN_LOCI_ALLELES, THREADS
     )
     clust_sample = clustering.add_readnum(clust_sample)
     clust_sample = clustering.add_percent(clust_sample)
     clust_sample = clustering.update_labels(clust_sample)
+    with open(Path(TEMPDIR, "clustering", f"{SAMPLE_NAME}.plk"), "wb") as p:
+        pickle.dump(clust_sample, p)
     ########################################################################
     # Consensus call
     ########################################################################
-    print(f"{_dtnow()}: Consensus calling {arguments['sample']}...", file=sys.stderr)
+    print(f"{_dtnow()}: Consensus calling of {arguments['sample']}...", file=sys.stderr)
     # Downsampling to 1000 reads in each LABEL
     clust_subset_sample = consensus.subset_clust(clust_sample, 1000)
-    cons_percentage, cons_sequence = consensus.call_consensus(clust_subset_sample, MUTATION_LOCI_ALLELES)
+    MUTATION_LOCI_LABELS = consensus.extract_mutation_loci_by_labels(clust_sample, TEMPDIR, FASTA_ALLELES, CONTROL_NAME)
+    cons_percentage, cons_sequence = consensus.call_consensus(clust_subset_sample, MUTATION_LOCI_LABELS)
     allele_names = consensus.call_allele_name(cons_sequence, cons_percentage, FASTA_ALLELES)
     cons_percentage = consensus.update_key_by_allele_name(cons_percentage, allele_names)
     cons_sequence = consensus.update_key_by_allele_name(cons_sequence, allele_names)
     RESULT_SAMPLE = consensus.add_key_by_allele_name(clust_sample, allele_names)
     RESULT_SAMPLE.sort(key=lambda x: x["LABEL"])
     ########################################################################
-    # Output Report：RESULT/FASTA/HTML/BAM/VCF
+    # Output Report：RESULT/FASTA/HTML/BAM
     ########################################################################
+    print(f"{_dtnow()}: Output reports of {arguments['sample']}...", file=sys.stderr)
     # RESULT
     midsv.write_jsonl(RESULT_SAMPLE, Path(TEMPDIR, "result", f"{SAMPLE_NAME}.jsonl"))
     # FASTA
     for header, cons_seq in cons_sequence.items():
         cons_fasta = report.report_files.to_fasta(header, cons_seq)
         Path(TEMPDIR, "report", "FASTA", SAMPLE_NAME, f"{SAMPLE_NAME}_{header}.fasta").write_text(cons_fasta)
     # HTML
@@ -195,8 +196,11 @@
     report.report_bam.output_bam_sample(
         TEMPDIR, RESULT_SAMPLE, SAMPLE_NAME, GENOME, GENOME_COODINATES, CHROME_SIZE, THREADS
     )
     for path_bam_igvjs in Path(TEMPDIR, "cache", ".igvjs").glob(f"{CONTROL_NAME}_control.bam*"):
         shutil.copy(path_bam_igvjs, Path(TEMPDIR, "report", ".igvjs", SAMPLE_NAME))
     # VCF
     # working in progress
+    ###########################################################
+    # Finish call
+    ###########################################################
     print(f"{_dtnow()}: \N{teacup without handle} {arguments['sample']} is finished!", file=sys.stderr)
```

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/call_midsv.py` & `DAJIN2-0.2.4/src/DAJIN2/core/preprocess/call_midsv.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,17 +4,15 @@
 import re
 from itertools import chain, groupby
 from pathlib import Path
 from typing import Generator
 
 import midsv
 
-
-def _load_sam(path_sam: str | Path) -> Generator[list[str]]:
-    return midsv.read_sam(path_sam)
+from DAJIN2.core.report.report_bam import remove_overlapped_reads
 
 
 def _split_cigar(CIGAR: str) -> list[str]:
     cigar = re.split(r"([MIDNSH=X])", CIGAR)
     n = len(cigar)
     cigar_split = []
     for i, j in zip(range(0, n, 2), range(1, n, 2)):
@@ -42,15 +40,15 @@
             is_splice = True
             break
         else:
             is_insertion = False
     return is_splice
 
 
-def _extract_qname_of_map_ont(sam_ont: Generator[list[str]], sam_splice: Generator[list[str]]) -> set():
+def extract_qname_of_map_ont(sam_ont: Generator[list[str]], sam_splice: Generator[list[str]]) -> set():
     """Extract qname of reads from `map-ont` when:
     - no inversion signal in `splice` alignment (insertion + deletion)
     - single read
     - long alignment length
     """
     dict_alignments_splice = {s[0]: s for s in sam_splice if not s[0].startswith("@")}
     alignments_ont = [s for s in sam_ont if not s[0].startswith("@")]
@@ -71,32 +69,32 @@
         alignment_length_ont = _call_alignment_length(alignment_ont[5])
         alignment_length_splice = _call_alignment_length(alignment_splice[5])
         if alignment_length_ont >= alignment_length_splice:
             qname_of_map_ont.add(qname_ont)
     return qname_of_map_ont
 
 
-def _extract_sam(sam: Generator[list[str]], qname_of_map_ont: set, preset: str = "map-ont") -> Generator[list[str]]:
+def extract_sam(sam: Generator[list[str]], qname_of_map_ont: set, preset: str = "map-ont") -> Generator[list[str]]:
     for alignment in sam:
         if alignment[0].startswith("@"):
             yield alignment
         if preset == "map-ont":
             if alignment[0] in qname_of_map_ont:
                 yield alignment
         else:
             if alignment[0] not in qname_of_map_ont:
                 yield alignment
 
 
-def _midsv_transform(sam: Generator[list[str]]) -> Generator[list[str]]:
+def midsv_transform(sam: Generator[list[str]]) -> Generator[list[str]]:
     for midsv_sample in midsv.transform(sam, midsv=False, cssplit=True, qscore=False):
         yield midsv_sample
 
 
-def _replaceNtoD(midsv_sample: Generator[list[str]], sequence: str) -> Generator[dict[str, str]]:
+def replaceNtoD(midsv_sample: Generator[list[str]], sequence: str) -> Generator[dict[str, str]]:
     for samp in midsv_sample:
         qname = samp["QNAME"]
         cssplits = samp["CSSPLIT"].split(",")
         # extract right/left index of the end of sequential Ns
         left_idx_n = 0
         for cs in cssplits:
             if cs != "N":
@@ -111,21 +109,31 @@
         # replace sequential Ns within the sequence
         for j, (cs, seq) in enumerate(zip(cssplits, sequence)):
             if left_idx_n <= j <= right_idx_n and cs == "N":
                 cssplits[j] = f"-{seq}"
         yield {"QNAME": qname, "CSSPLIT": ",".join(cssplits)}
 
 
+###########################################################
+# main
+###########################################################
+
+
 def call_midsv(TEMPDIR: Path | str, FASTA_ALLELES: dict, SAMPLE_NAME: str) -> None:
     for allele, sequence in FASTA_ALLELES.items():
         path_ont = Path(TEMPDIR, "sam", f"{SAMPLE_NAME}_map-ont_{allele}.sam")
         path_splice = Path(TEMPDIR, "sam", f"{SAMPLE_NAME}_splice_{allele}.sam")
-        qname_of_map_ont = _extract_qname_of_map_ont(_load_sam(path_ont), _load_sam(path_splice))
-        sam_of_map_ont = _extract_sam(_load_sam(path_ont), qname_of_map_ont, preset="map-ont")
-        sam_of_splice = _extract_sam(_load_sam(path_splice), qname_of_map_ont, preset="splice")
+        sam_ont = remove_overlapped_reads(list(midsv.read_sam(path_ont)))
+        sam_splice = remove_overlapped_reads(list(midsv.read_sam(path_splice)))
+        qname_of_map_ont = extract_qname_of_map_ont(sam_ont, sam_splice)
+        sam_of_map_ont = extract_sam(sam_ont, qname_of_map_ont, preset="map-ont")
+        sam_of_splice = extract_sam(sam_splice, qname_of_map_ont, preset="splice")
+        # qname_of_map_ont = extract_qname_of_map_ont(midsv.read_sam(path_ont), midsv.read_sam(path_splice))
+        # sam_of_map_ont = extract_sam(midsv.read_sam(path_ont), qname_of_map_ont, preset="map-ont")
+        # sam_of_splice = extract_sam(midsv.read_sam(path_splice), qname_of_map_ont, preset="splice")
         sam_chained = chain(sam_of_map_ont, sam_of_splice)
-        midsv_chaind = _midsv_transform(sam_chained)
-        midsv_sample = _replaceNtoD(midsv_chaind, sequence)
+        midsv_chaind = midsv_transform(sam_chained)
+        midsv_sample = replaceNtoD(midsv_chaind, sequence)
         filepath = Path(TEMPDIR, "midsv", f"{SAMPLE_NAME}_{allele}.json")
         with open(filepath, "wt", encoding="utf-8") as f:
             for data in midsv_sample:
                 f.write(json.dumps(data) + "\n")
```

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py` & `DAJIN2-0.2.4/src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 import re
 from collections import defaultdict
 import numpy as np
 import scipy
 from statsmodels.nonparametric.smoothers_lowess import lowess as sm_lowess
 
 
-def get_repeat_regions(sequence: str, candidates: set(int)) -> list[tuple[int, int]]:
+def get_repeat_regions(sequence: str, candidate_loci: set(int)) -> list[tuple[int, int]]:
     """
     Find homopolymers in the sequence but discard them that
     are adjacent to candidate mutation loci because they are
     likely to be covered by the real mutations
     """
     pattern = r"A{4,}|C{4,}|G{4,}|T{4,}|N{4,}"
     repeat_regions = []
     for start, end in (match.span() for match in re.finditer(pattern, sequence)):
-        if not (start - 1 in candidates and end + 1 in candidates):
+        if not (start - 1 in candidate_loci and end + 1 in candidate_loci):
             repeat_regions.append((start, end))
     return repeat_regions
 
 
 def get_counts_homopolymer(indels_sample_mut, indels_control_mut, repeat_regions):
     # Initialize default dictionaries to hold counts
     mutation_counts = defaultdict(list)
@@ -120,13 +120,15 @@
 ###########################################################
 # main
 ###########################################################
 
 
 def extract_errors_in_homopolymer(indels_sample_mut, indels_control_mut, sequence, candidate_loci) -> set(int):
     repeat_regions = get_repeat_regions(sequence, candidate_loci)
+    if repeat_regions == []:
+        return set()
     mutation_counts, mutation_counts_regions = get_counts_homopolymer(
         indels_sample_mut, indels_control_mut, repeat_regions
     )
     thresholds = return_thresholds(mutation_counts)
     errors_in_homopolyer = get_errors_in_homopolyer(mutation_counts_regions, thresholds)
     return errors_in_homopolyer
```

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/extract_knockin_loci.py` & `DAJIN2-0.2.4/src/DAJIN2/core/preprocess/extract_knockin_loci.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/extract_mutation_loci.py` & `DAJIN2-0.2.4/src/DAJIN2/core/preprocess/extract_mutation_loci.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,39 +4,38 @@
 from collections import defaultdict
 import json
 import numpy as np
 from pathlib import Path
 from typing import Generator
 from scipy import stats
 from scipy.spatial import distance
-from sklearn.neighbors import LocalOutlierFactor
+import pickle
+
+# from sklearn.neighbors import LocalOutlierFactor
 from DAJIN2.core.preprocess.extract_errors_in_homopolymer import extract_errors_in_homopolymer
 
 
 def read_midsv(filepath) -> Generator[dict[str, str]]:
     with open(filepath, "r") as f:
         for line in f:
             yield json.loads(line)
 
 
-def _make_gen(reader):
-    while True:
-        b = reader(2**16)
-        if not b:
-            break
-        yield b
-
-
-def count_newlines(filepath):
-    with open(filepath, "rb") as f:
-        count = sum(buf.count(b"\n") for buf in _make_gen(f.raw.read))
-    return count
+def call_coverage_on_each_base(midsv_sample: Generator[dict], sequence: str) -> list[int]:
+    coverages = [1] * len(sequence)
+    for cont in midsv_sample:
+        cssplits = cont["CSSPLIT"].split(",")
+        for i, cssplit in enumerate(cssplits):
+            if cssplit == "N":
+                continue
+            coverages[i] += 1
+    return coverages
 
 
-def _count_indels(midsv_sample, len_sequence: int) -> dict[str, list[int]]:
+def count_indels(midsv_sample, len_sequence: int) -> dict[str, list[int]]:
     count = {"+": [0] * len_sequence, "-": [0] * len_sequence, "*": [0] * len_sequence}
     for samp in midsv_sample:
         for i, cs in enumerate(samp["CSSPLIT"].split(",")):
             if cs.startswith("=") or cs == "N" or re.search(r"a|c|g|t|n", cs):
                 continue
             if cs.startswith("+"):
                 # count["+"][i] += len(cs.split("|"))
@@ -44,94 +43,75 @@
             elif cs.startswith("-"):
                 count["-"][i] += 1
             elif cs.startswith("*"):
                 count["*"][i] += 1
     return count
 
 
-def _normalize_indels(count: dict[str, list[int]], coverage: int) -> dict[str, np.array]:
+def normalize_indels(count: dict[str, list[int]], coverages: list[int]) -> dict[str, np.array]:
     count_normalized = dict()
+    coverages = np.array(coverages)
     for mut in count:
         counts = np.array(count[mut])
-        counts_norm = (counts / coverage) * 10**6
-        count_normalized[mut] = counts_norm.astype("uint32")
+        count_normalized[mut] = counts / coverages
     return count_normalized
 
 
-def _split_kmer(indels: dict[str, np.array], kmer: int = 10) -> dict[str, np.array]:
+def split_kmer(indels: dict[str, np.array], kmer: int = 10) -> dict[str, np.array]:
     results = defaultdict(list)
     center = kmer // 2
     for mut, value in indels.items():
         for i in range(len(value)):
             if center <= i <= len(value) - center:
                 start = i - center
                 if kmer % 2 == 0:
                     end = i + center
                 else:
                     end = i + center + 1
                 results[mut].append(value[start:end])
             else:
-                results[mut].append(np.array([0] * kmer, dtype="uint32"))
+                results[mut].append(np.array([0] * kmer))
     return results
 
 
-def _extract_anomaly_loci(indels_kmer_sample: dict, indels_kmer_control: dict) -> dict[str, set[int]]:
-    anomaly_loci = dict()
-    clf = LocalOutlierFactor(novelty=True, n_neighbors=5)
-    for mut in indels_kmer_sample.keys():
-        loci = set()
-        values_control = indels_kmer_control[mut]
-        values_sample = indels_kmer_sample[mut]
-        index = -1
-        for i, (value_control, value_sample) in enumerate(zip(values_control, values_sample)):
-            if i == index:
-                continue
-            clf.fit(value_control.reshape(-1, 1))
-            pred = clf.predict(value_sample.reshape(-1, 1))
-            if pred[5] == -1:
-                loci.add(i)
-            # If the next base is not -1, do not validate the next base because the next base is not an outlier.
-            if pred[6] == 1:
-                index = i + 1
-        anomaly_loci.update({mut: loci})
-    return anomaly_loci
-
-
-def _extract_dissimilar_loci(indels_kmer_sample: dict, indels_kmer_control: dict) -> dict[str, set]:
+def extract_dissimilar_loci(indels_kmer_sample: dict, indels_kmer_control: dict) -> dict[str, set]:
     """
     Comparing Sample and Control, the 1. 'high similarity',  2. 'similar mean' and
     3. 'similar variance' are considered as sequence errors.
     """
     results = dict()
     for mut in indels_kmer_sample:
         values_sample = indels_kmer_sample[mut]
         values_control = indels_kmer_control[mut]
         # Calculate cosine similarity: 1 means exactly same, 0 means completely different.
         # When calculating cossim, uint32 returns inaccurate results so convert to float64
-        cossim = [
-            1 - distance.cosine(x.astype("float64"), y.astype("float64")) for x, y in zip(values_sample, values_control)
-        ]
+        cossim = [1 - distance.cosine(x, y) for x, y in zip(values_sample, values_control)]
         # Perform T-test: nan means exactly same, p > 0.05 means similar in average.
         t_pvalues = [stats.ttest_ind(x, y, equal_var=False)[1] for x, y in zip(values_sample, values_control)]
         t_pvalues = [1 if np.isnan(t) else t for t in t_pvalues]
         # Perform F-test: p > 0.05 means similar in variance.
         f_pvalues = [stats.bartlett(x, y)[1] for x, y in zip(values_sample, values_control)]
         # if pvalue == nan or pval > 0.05, samples and controls are similar.
         dissimilar_loci = set()
         for i, (sim, t_pval, f_pval) in enumerate(zip(cossim, t_pvalues, f_pvalues)):
-            flag_seqerror = False
-            if sim > 0.90 and t_pval > 0.05 and f_pval > 0.05:
-                flag_seqerror = True
-            if flag_seqerror is False:
+            if not (sim > 0.90 and t_pval > 0.05 and f_pval > 0.05):
                 dissimilar_loci.add(i)
-        results.update({mut: dissimilar_loci})
+        results[mut] = dissimilar_loci
     return results
 
 
-def _transpose_mutation_loci(mutation_loci, len_sequence):
+def discard_errors_in_homopolymer(dissimilar_loci, errors_in_homopolymer) -> dict[str, set]:
+    mutation_loci = dict()
+    for mut in ["+", "-", "*"]:
+        error_loci = errors_in_homopolymer[mut]
+        mutation_loci[mut] = dissimilar_loci[mut] - error_loci
+    return mutation_loci
+
+
+def transpose_mutation_loci(mutation_loci: set[int], len_sequence: int) -> list[set]:
     mutation_loci_transposed = [set() for _ in range(len_sequence)]
     for mut, idx_mutation in mutation_loci.items():
         for i, loci in enumerate(mutation_loci_transposed):
             if i in idx_mutation:
                 loci.add(mut)
     return mutation_loci_transposed
 
@@ -144,34 +124,36 @@
 def extract_mutation_loci(
     TEMPDIR: Path, FASTA_ALLELES: dict, SAMPLE_NAME: str, CONTROL_NAME: str
 ) -> dict[str, list[set[str]]]:
     MUTATION_LOCI_ALLELES = dict()
     for allele, sequence in FASTA_ALLELES.items():
         filepath_sample = Path(TEMPDIR, "midsv", f"{SAMPLE_NAME}_{allele}.json")
         filepath_control = Path(TEMPDIR, "midsv", f"{CONTROL_NAME}_{allele}.json")
-        coverage_sample = count_newlines(filepath_sample)
-        coverage_control = count_newlines(filepath_control)
-        indels_sample = _count_indels(read_midsv(filepath_sample), len(sequence))
-        indels_control = _count_indels(read_midsv(filepath_control), len(sequence))
-        indels_sample_normalized = _normalize_indels(indels_sample, coverage_sample)
-        indels_control_normalized = _normalize_indels(indels_control, coverage_control)
-        indels_kmer_sample = _split_kmer(indels_sample_normalized, kmer=10)
-        indels_kmer_control = _split_kmer(indels_control_normalized, kmer=10)
-        anomaly_loci = _extract_anomaly_loci(indels_kmer_sample, indels_kmer_control)
-        dissimilar_loci = _extract_dissimilar_loci(indels_kmer_sample, indels_kmer_control)
+        indels_sample = count_indels(read_midsv(filepath_sample), len(sequence))
+        indels_control = count_indels(read_midsv(filepath_control), len(sequence))
+        coverages_sample = call_coverage_on_each_base(read_midsv(filepath_sample), sequence)
+        coverages_control = call_coverage_on_each_base(read_midsv(filepath_control), sequence)
+        indels_sample_normalized = normalize_indels(indels_sample, coverages_sample)
+        indels_control_normalized = normalize_indels(indels_control, coverages_control)
+        indels_kmer_sample = split_kmer(indels_sample_normalized, kmer=10)
+        indels_kmer_control = split_kmer(indels_control_normalized, kmer=10)
+        # anomaly_loci = _extract_anomaly_loci(indels_kmer_sample, indels_kmer_control)
+        dissimilar_loci = extract_dissimilar_loci(indels_kmer_sample, indels_kmer_control)
         # Extract error loci in homopolymer regions
-        error_loci_homopolymer = dict()
-        for mut in ["+", "-", "*"]:
-            candidate_loci = anomaly_loci[mut] & dissimilar_loci[mut]
-            indels_sample_mut = indels_sample[mut]
-            indels_control_mut = indels_control[mut]
-            error_loci = extract_errors_in_homopolymer(indels_sample_mut, indels_control_mut, sequence, candidate_loci)
-            error_loci_homopolymer.update({mut: error_loci})
-        mutation_loci = dict()
+        errors_in_homopolymer = dict()
         for mut in ["+", "-", "*"]:
-            candidate_loci = anomaly_loci[mut] & dissimilar_loci[mut]
-            error_loci = error_loci_homopolymer[mut]
-            # Discard error loci in homopolymer regions
-            mutation_loci.update({mut: candidate_loci - error_loci})
-        mutation_loci_transposed = _transpose_mutation_loci(mutation_loci, len(sequence))
-        MUTATION_LOCI_ALLELES.update({allele: mutation_loci_transposed})
+            indels_sample_mut = indels_sample_normalized[mut]
+            indels_control_mut = indels_control_normalized[mut]
+            candidate_loci = dissimilar_loci[mut]
+            # candidate_loci = anomaly_loci[mut] & dissimilar_loci[mut]
+            errors_in_homopolymer[mut] = extract_errors_in_homopolymer(
+                indels_sample_mut, indels_control_mut, sequence, candidate_loci
+            )
+        mutation_loci = discard_errors_in_homopolymer(dissimilar_loci, errors_in_homopolymer)
+        mutation_loci_transposed = transpose_mutation_loci(mutation_loci, len(sequence))
+        MUTATION_LOCI_ALLELES[allele] = mutation_loci_transposed
+        # Save indels_control_normalized and indels_kmer_control as pickle to reuse in consensus calling
+        with open(Path(TEMPDIR, "mutation_loci", f"{CONTROL_NAME}_{allele}_normalized.pkl"), "wb") as f:
+            pickle.dump(indels_control_normalized, f)
+        with open(Path(TEMPDIR, "mutation_loci", f"{CONTROL_NAME}_{allele}_kmer.pkl"), "wb") as f:
+            pickle.dump(indels_kmer_control, f)
     return MUTATION_LOCI_ALLELES
```

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/format_inputs.py` & `DAJIN2-0.2.4/src/DAJIN2/core/preprocess/format_inputs.py`

 * *Files 18% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 ########################################################################
 
 
 def convert_to_posix_path(path: str) -> str:
     try:
         path = wslPath.toPosix(path)
     except ValueError:
+        # This is already a posix path, so just pass
         pass
     return str(path)
 
 
 ########################################################################
 # Extract basename
 ########################################################################
@@ -65,52 +66,50 @@
         name = re.sub(r'[\\|/|:|?|.|,|\'|"|<|>|\| |]', "-", name)
         header.append(name)
         sequence.append(seq.upper())
     return {h: s for h, s in zip(header, sequence)}
 
 
 ########################################################################
-# Update threads
-########################################################################
-
-
-def update_threads(threads):
-    threads_updated = min(int(threads), os.cpu_count() - 1)
-    threads_updated = max(1, threads_updated)
-    return threads_updated
-
-
-########################################################################
 # Fetch genome coodinate and chrom size
 ########################################################################
 
 
-# TODO TEST
-def fetch_coodinate(genome: str, ucsc_url: str, seq: str) -> dict:
-    ucsc_blat = f"{ucsc_url}/cgi-bin/hgBlat?db={genome}&type=BLAT&userSeq={seq}"
-    request = urlopen(ucsc_blat).read().decode("utf8").split("\n")
-    coodinate = [x for x in request if x.count("100.0%")]
-    if not coodinate:
-        raise AttributeError(f"{seq} is not found in {genome}")
+def fetch_coordinate(genome: str, ucsc_url: str, seq: str) -> dict:
+    def _fetch_seq(seq: str):
+        url_blat = f"{ucsc_url}/cgi-bin/hgBlat?db={genome}&type=BLAT&userSeq={seq}"
+        request = urlopen(url_blat).read().decode("utf8").split("\n")
+        matches = [x for x in request if "100.0%" in x]
+        if not matches:
+            raise AttributeError(f"{seq} is not found in {genome}")
+        return matches[0].split()[-5:-1]
+
+    seq_start, seq_end = seq[:1000], seq[-1000:]
+    coordinate_start, coordinate_end = _fetch_seq(seq_start), _fetch_seq(seq_end)
+
+    chromosome, strand = coordinate_start[0], coordinate_start[1]
+    if strand == "+":
+        start, end = int(coordinate_start[2]), int(coordinate_end[3])
     else:
-        coodinate = coodinate[0].split()
-        return {"chr": coodinate[-5], "start": int(coodinate[-3]), "end": int(coodinate[-2]), "strand": coodinate[-4]}
+        start, end = int(coordinate_end[2]), int(coordinate_start[3])
+
+    return {"chr": chromosome, "start": start, "end": end, "strand": strand}
 
 
 def fetch_chrom_size(chrom: str, genome: str, goldenpath_url: str) -> int:
     url = f"{goldenpath_url}/{genome}/bigZips/{genome}.chrom.sizes"
     request = urlopen(url).read().decode("utf8").split("\n")
     for req in request:
         req = req.split("\t")
         if chrom == req[0]:
             chrom_size = int(req[1])
     return chrom_size
 
 
-def cache_coodinates_and_chromsize(TEMPDIR, GENOME, GENOME_COODINATES, CHROME_SIZE):
+def cache_coodinates_and_chromsize(TEMPDIR, GENOME, GENOME_COODINATES, CHROME_SIZE) -> None:
     """
     Save (1) genome_symbol.txt, (2) genome_coodinates.jsonl, (3) chrome_size.txt
     """
     # Save info to the cache directory
     Path(TEMPDIR, "cache", "genome_symbol.txt").write_text(GENOME + "\n")
     midsv.write_jsonl([GENOME_COODINATES], Path(TEMPDIR, "cache", "genome_coodinates.jsonl"))
     Path(TEMPDIR, "cache", "chrome_size.txt").write_text(str(CHROME_SIZE))
```

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/mappy_align.py` & `DAJIN2-0.2.4/src/DAJIN2/core/preprocess/mappy_align.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/replace_NtoD.py` & `DAJIN2-0.2.4/src/DAJIN2/core/preprocess/replace_NtoD.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/preprocess/validate_inputs.py` & `DAJIN2-0.2.4/src/DAJIN2/preprocess/validate_inputs.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,64 +5,66 @@
 from pathlib import Path
 from urllib.error import URLError
 from urllib.request import urlopen
 
 import mappy
 
 
-def exists(input_file: str):
+def _exist_file(input_file: str):
     if not Path(input_file).exists():
         raise FileNotFoundError(f"{input_file} is not found")
 
 
 ########################################################################
 # Check if the sample is in the proper format.
 ########################################################################
 
 
-def fastq_extension(fastq_path: str):
+def _fastq_extension(fastq_path: str):
     if not re.search(r".fastq$|.fastq.gz$|.fq$|.fq.gz$", fastq_path):
         raise AttributeError(f"{fastq_path} requires extensions either 'fastq', 'fastq.gz', 'fq' or 'fq.gz'")
 
 
-# File content
-def fastq_content(fastq_path: str):
+# Varidate if the file is in the proper format. See top 100 lines
+def _fastq_content(fastq_path: str):
     name, seq, qual = [], [], []
-    for n, s, q in mappy.fastx_read(fastq_path):
+    for i, (n, s, q) in enumerate(mappy.fastx_read(fastq_path)):
         name.append(n)
         seq.append(s)
         qual.append(q)
+        if i == 100:
+            break
     if not (len(name) == len(seq) == len(qual) > 0):
         raise AttributeError(f"{fastq_path} is not a FASTQ format")
 
 
-def fasta_content(fasta_path: str):
+def _fasta_content(fasta_path: str):
     name, seq = [], []
     for n, s, _ in mappy.fastx_read(fasta_path):
         name.append(n)
         seq.append(s)
     if not len(name) == len(seq) > 0:
         raise AttributeError(f"{fasta_path} is not a FASTA format")
     if len(name) > len(set(name)):
         raise AttributeError(f"{fasta_path} must include unique identifiers")
     if len(seq) > len(set(seq)):
         raise AttributeError(f"{fasta_path} must include unique DNA sequences")
     if name.count("control") == 0:
         raise AttributeError(f"One of the headers in the {fasta_path} must be '>control'")
 
 
-def check_files(SAMPLE: str, CONTROL: str, ALLELE: str) -> None:
-    exists(CONTROL)
-    exists(SAMPLE)
-    exists(ALLELE)
-    fastq_extension(CONTROL)
-    fastq_content(CONTROL)
-    fastq_extension(SAMPLE)
-    fastq_content(SAMPLE)
-    fasta_content(ALLELE)
+def validate_files(SAMPLE: str, CONTROL: str, ALLELE: str) -> None:
+    _exist_file(CONTROL)
+    _exist_file(SAMPLE)
+    _exist_file(ALLELE)
+    _fastq_extension(CONTROL)
+    _fastq_content(CONTROL)
+    _fastq_extension(SAMPLE)
+    _fastq_content(SAMPLE)
+    _fasta_content(ALLELE)
 
 
 ########################################################################
 # Check Cache
 ########################################################################
 
 
@@ -93,58 +95,56 @@
 
 
 def _check_url_availabilities(urls: list[str]) -> list[bool]:
     availabilities = []
     for url in urls:
         try:
             _ = urlopen(url, timeout=10)
-        except URLError:
+        except TimeoutError:
             availabilities.append(False)
         else:
             availabilities.append(True)
     return availabilities
 
 
 def _extract_available_urls(urls: list[str], availabilities: list[bool]) -> list[str]:
     available_urls = []
     for url, flag in zip(urls, availabilities):
         if flag:
             available_urls.append(url)
     return available_urls
 
 
-def _is_listed(genome: str, ucsc_url: str) -> None:
+def _is_genome_listed_in_UCSC(genome: str, ucsc_url: str) -> None:
     url = f"{ucsc_url}/cgi-bin/das/{genome}/dna?segment=1:1,10"
     response = urlopen(url, timeout=10)
     content = response.read()
     response.close()
     if not content:
         raise AttributeError(
-            f"{genome} is not listed in UCSC genome browser. Available genomes are in {ucsc_url}/cgi-bin/das/dsn"
+            f"{genome} is not listed in UCSC genome browser. Available genomes are listed in {ucsc_url}/cgi-bin/das/dsn"
         )
 
 
-def check_and_fetch_genome(GENOME: str) -> tuple[str, str]:
-    # Check UCSC Server
-    UCSC_URLS = [
+def validate_genome_and_fetch_urls(GENOME: str) -> dict[str, str]:
+    # Check UCSC Server is available
+    URLS_UCSC = [
         "https://genome.ucsc.edu/",
         "https://genome-asia.ucsc.edu/",
         "https://genome-euro.ucsc.edu/",
     ]
-    url_availabilities = _check_url_availabilities(UCSC_URLS)
+    url_availabilities = _check_url_availabilities(URLS_UCSC)
     if not any(url_availabilities):
         raise URLError("All servers of UCSC Genome Browsers are currently down. Please wait for a while and try again.")
-
-    UCSC_URL = _extract_available_urls(UCSC_URLS, url_availabilities)[0]
-
-    # Check UCSC Download Server
-    GOLDENPATH_URLS = [
+    URL_UCSC_AVAILABLE = _extract_available_urls(URLS_UCSC, url_availabilities)[0]
+    # Check UCSC Download Server is available
+    URLS_GOLDENPATH = [
         "https://hgdownload.cse.ucsc.edu/goldenPath",
         "http://hgdownload-euro.soe.ucsc.edu/goldenPath",
     ]
-    url_availabilities = _check_url_availabilities(UCSC_URLS)
+    url_availabilities = _check_url_availabilities(URLS_UCSC)
     if not any(url_availabilities):
         raise URLError("All servers of UCSC GoldenPath are currently down. Please wait for a while and try again.")
-    GOLDENPATH_URL = _extract_available_urls(GOLDENPATH_URLS, url_availabilities)[0]
-    # Check input genome
-    _is_listed(GENOME, UCSC_URL)
-    return UCSC_URL, GOLDENPATH_URL
+    URL_GOLDENPATH_AVAILABLE = _extract_available_urls(URLS_GOLDENPATH, url_availabilities)[0]
+    # Check input genome is listed in UCSC
+    _is_genome_listed_in_UCSC(GENOME, URL_UCSC_AVAILABLE)
+    return {"ucsc": URL_UCSC_AVAILABLE, "goldenpath": URL_GOLDENPATH_AVAILABLE}
```

### Comparing `DAJIN2-0.2.3/src/DAJIN2/core/report/report_files.py` & `DAJIN2-0.2.4/src/DAJIN2/core/report/report_files.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.3/src/DAJIN2/gui.py` & `DAJIN2-0.2.4/src/DAJIN2/gui.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.3/src/DAJIN2/main.py` & `DAJIN2-0.2.4/src/DAJIN2/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,24 +2,25 @@
 
 import os
 import argparse
 import multiprocessing
 import sys
 from itertools import groupby, islice
 from pathlib import Path
+import csv
 
 import pandas as pd
 import wslPath
 
 from DAJIN2 import gui, view
 from DAJIN2.core import core_execute
 from DAJIN2.postprocess import report
 from DAJIN2.preprocess.validate_inputs import validate_files, validate_genome_and_fetch_urls
 
-VERSION = "0.2.3"
+VERSION = "0.2.4"
 
 # prevent BLAS from using all cores
 os.environ["OMP_NUM_THREADS"] = "1"
 os.environ["OPENBLAS_NUM_THREADS"] = "1"
 os.environ["MKL_NUM_THREADS"] = "1"
 os.environ["VECLIB_MAXIMUM_THREADS"] = "1"
 os.environ["NUMEXPR_NUM_THREADS"] = "1"
@@ -28,30 +29,30 @@
 def execute_single_mode(arguments: dict[str]):
     ################################################################################
     # Validate contents
     ################################################################################
     validate_files(arguments["sample"], arguments["control"], arguments["allele"])
     URLS_GENOME: dict[str, dict[str, str]] = dict()
     if "genome" in arguments:
-        URLS_GENOME.update({arguments["genome"]: validate_genome_and_fetch_urls(arguments["genome"])})
+        URLS_GENOME[arguments["genome"]] = validate_genome_and_fetch_urls(arguments["genome"])
         arguments.update(URLS_GENOME[arguments["genome"]])
     ##############################################################################
     # Perform DAJIN2
     ##############################################################################
     core_execute.execute_control(arguments)
     core_execute.execute_sample(arguments)
     name = arguments["name"]
     report.report(name)
     print(
         f"\N{party popper} Finished! Open DAJINResults/{name} to see the report.",
         file=sys.stderr,
     )
 
 
-def _update_threads(threads) -> int:
+def _update_threads(threads: int) -> int:
     threads_updated = min(int(threads), os.cpu_count() - 1)
     threads_updated = max(1, threads_updated)
     return threads_updated
 
 
 def _extract_unique_contents(list: list) -> list:
     list_unique = []
@@ -97,21 +98,25 @@
     # Check file exists
     # ----------------------------------------------------------
     if not Path(path_batchfile).exists():
         raise FileNotFoundError(f"'{path_batchfile}' does not exist.")
     # ----------------------------------------------------------
     # Load the file
     # ----------------------------------------------------------
+    # From Excel file
     try:
         df_batchfile = pd.read_excel(path_batchfile)
         inputs = []
         inputs.append(df_batchfile.columns.to_list())
         inputs += df_batchfile.values.tolist()
     except ValueError:
-        inputs = [s.split(",") for s in Path(path_batchfile).read_text().strip().split("\n")]
+        # From CSV file
+        with open(path_batchfile) as f:
+            inputs = [row for row in csv.reader(f, skipinitialspace=True, delimiter=",")]
+
     ################################################################################
     # Validate Column of the batch file
     ################################################################################
     columns = inputs[0]
     if not {"sample", "control", "allele", "name"}.issubset(set(columns)):
         raise ValueError(f"{path_batchfile} must contain 'sample', 'control', and 'allele' in the header")
     if not set(columns).issubset({"sample", "control", "allele", "name", "genome"}):
@@ -126,15 +131,15 @@
     contents.sort(key=lambda x: x[index_name])
     for _, groups in groupby(contents, key=lambda x: x[index_name]):
         for group in groups:
             args = {h: g for h, g in zip(columns, group)}
             validate_files(args["sample"], args["control"], args["allele"])
             URLS_GENOME: dict[str, dict[str, str]] = dict()
             if "genome" in args and not args["genome"] in URLS_GENOME:
-                URLS_GENOME.update({args["genome"]: validate_genome_and_fetch_urls(args["genome"])})
+                URLS_GENOME[args["genome"]] = validate_genome_and_fetch_urls(args["genome"])
     ##############################################################################
     # Perform DAJIN2
     ##############################################################################
     num_workers = _update_threads(arguments["threads"])
     index_name = columns.index("name")
     contents.sort(key=lambda x: x[index_name])
     contents_sample = []
```

### Comparing `DAJIN2-0.2.3/src/DAJIN2/postprocess/report.py` & `DAJIN2-0.2.4/src/DAJIN2/postprocess/report.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.3/src/DAJIN2/template_igvjs.html` & `DAJIN2-0.2.4/src/DAJIN2/template_igvjs.html`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.3/src/DAJIN2/templates/index.html` & `DAJIN2-0.2.4/src/DAJIN2/templates/index.html`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.3/src/DAJIN2/view.py` & `DAJIN2-0.2.4/src/DAJIN2/view.py`

 * *Files identical despite different names*

### Comparing `DAJIN2-0.2.3/src/DAJIN2.egg-info/PKG-INFO` & `DAJIN2-0.2.4/src/DAJIN2.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 Metadata-Version: 2.1
 Name: DAJIN2
-Version: 0.2.3
-Summary: One-step genotyping tools for Nanopore amplicon sequencing
+Version: 0.2.4
+Summary: One-step genotyping tools for Targeted long-read sequencing
 Home-page: https://github.com/akikuno/DAJIN2
 Author: Akihiro Kuno
 Author-email: akuno@md.tsukuba.ac.jp
-Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX
 Classifier: Development Status :: 3 - Alpha
-Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 [![License](https://img.shields.io/badge/License-MIT-9cf.svg?style=flat-square)](https://choosealicense.com/licenses/mit/)
 [![PyPI](https://img.shields.io/pypi/v/DAJIN2.svg?label=PyPI&color=orange&style=flat-square)](https://pypi.org/project/DAJIN2/)
+[![Python](https://img.shields.io/pypi/pyversions/DAJIN2.svg?label=Python&color=blue&style=flat-square)](https://pypi.org/project/DAJIN2/)
 
 ⚠️ DAJIN2 is currently under development ⚠️
 
 Expected to be available the stable version in August 2023 🤞
 
 ## Installation (alpha-version)
 
@@ -76,15 +78,15 @@
 # 2023-06-04 11:35:01: Consensus calling single/barcode25.fq.gz...
 # 2023-06-04 11:35:08: 🍵 single/barcode25.fq.gz is finished!
 # 🎉 Finished! Open DAJINResults/stx2-deletion to see the report.
 ```
 
 ### Batch-mode
 
-DAJIN2 can handle multiple FASTQ files via `batch` subcommand.
+DAJIN2 can handle multiple FASTQ files using the `batch' subcommand.
 
 ```bash
 DAJIN2 batch [-h] -f FILE [-t THREADS]
 
 options:
   -h, --help            Show this help message and exit
   -f FILE, --file FILE  CSV or Excel file
@@ -92,10 +94,23 @@
                         Number of threads [default: 1]
 ```
 
 #### Example
 
 🚧 Working in progress 🚧
 
-## Reference
+### GUI-mode
 
-Kuno A, Ikeda Y, Ayabe S, Kato K, Sakamoto K, et al. (2022) DAJIN enables multiplex genotyping to simultaneously validate intended and unintended target genome editing outcomes. PLOS Biology 20(1): e3001507. https://doi.org/10.1371/journal.pbio.3001507
+You can use DAJIN2 with a graphical user interface (GUI) via the `gui` subcommand.
+
+```bash
+DAJIN2 gui
+```
+
+#### Example
+
+🚧 Working in progress 🚧
+
+
+## References
+
+[Kuno A, et al. (2022) DAJIN enables multiplex genotyping to simultaneously validate intended and unintended target genome editing outcomes. *PLoS Biology* 20(1): e3001507.](https://doi.org/10.1371/journal.pbio.3001507)
```

### Comparing `DAJIN2-0.2.3/src/DAJIN2.egg-info/SOURCES.txt` & `DAJIN2-0.2.4/src/DAJIN2.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 LICENSE
 MANIFEST.in
 README.md
 setup.py
 src/DAJIN2/__init__.py
-src/DAJIN2/batch.py
 src/DAJIN2/gui.py
 src/DAJIN2/main.py
-src/DAJIN2/single.py
 src/DAJIN2/template_igvjs.html
 src/DAJIN2/view.py
 src/DAJIN2.egg-info/PKG-INFO
 src/DAJIN2.egg-info/SOURCES.txt
 src/DAJIN2.egg-info/dependency_links.txt
 src/DAJIN2.egg-info/entry_points.txt
 src/DAJIN2.egg-info/requires.txt
@@ -23,28 +21,29 @@
 src/DAJIN2/core/clustering/__init__.py
 src/DAJIN2/core/clustering/clustering.py
 src/DAJIN2/core/clustering/make_score.py
 src/DAJIN2/core/clustering/merge_clusters.py
 src/DAJIN2/core/clustering/return_labels.py
 src/DAJIN2/core/consensus/__init__.py
 src/DAJIN2/core/consensus/consensus.py
+src/DAJIN2/core/consensus/extract_mutation_loci_by_labels.py
 src/DAJIN2/core/consensus/subset.py
 src/DAJIN2/core/preprocess/__init__.py
 src/DAJIN2/core/preprocess/call_midsv.py
-src/DAJIN2/core/preprocess/correct_knockin.py
-src/DAJIN2/core/preprocess/correct_sequence_error.py
+src/DAJIN2/core/preprocess/check_caches.py
 src/DAJIN2/core/preprocess/extract_errors_in_homopolymer.py
 src/DAJIN2/core/preprocess/extract_knockin_loci.py
 src/DAJIN2/core/preprocess/extract_mutation_loci.py
 src/DAJIN2/core/preprocess/format_inputs.py
 src/DAJIN2/core/preprocess/mappy_align.py
 src/DAJIN2/core/preprocess/replace_NtoD.py
-src/DAJIN2/core/preprocess/validate_inputs.py
 src/DAJIN2/core/report/__init__.py
+src/DAJIN2/core/report/remove_microhomology.py
 src/DAJIN2/core/report/report_bam.py
 src/DAJIN2/core/report/report_files.py
+src/DAJIN2/core/report/reverse_sam.py
 src/DAJIN2/postprocess/__init__.py
 src/DAJIN2/postprocess/report.py
 src/DAJIN2/preprocess/__init__.py
 src/DAJIN2/preprocess/validate_inputs.py
 src/DAJIN2/static/css/style.css
 src/DAJIN2/templates/index.html
```

