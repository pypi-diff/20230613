# Comparing `tmp/anacore-2.9.0.tar.gz` & `tmp/anacore-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/anacore-2.9.0.tar", last modified: Sat May  1 14:51:48 2021, max compression
+gzip compressed data, was "anacore-3.0.0.tar", last modified: Tue Jun 13 16:22:13 2023, max compression
```

## Comparing `anacore-2.9.0.tar` & `anacore-3.0.0.tar`

### file list

```diff
@@ -1,47 +1,78 @@
-drwxrwxr-x   0 fescudie  (1000) fescudie  (1000)        0 2021-05-01 14:51:48.097463 anacore-2.9.0/
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)      324 2021-05-01 14:51:48.097463 anacore-2.9.0/PKG-INFO
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)      880 2021-04-28 13:28:26.110516 anacore-2.9.0/README.md
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     3203 2021-04-28 13:28:26.110516 anacore-2.9.0/RELEASES_NOTES.md
-drwxrwxr-x   0 fescudie  (1000) fescudie  (1000)        0 2021-05-01 14:51:48.093462 anacore-2.9.0/anacore/
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     4680 2021-01-29 16:47:20.359155 anacore-2.9.0/anacore/STARLog.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)        0 2021-01-29 16:47:20.359155 anacore-2.9.0/anacore/__init__.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     3783 2021-01-29 16:47:20.359155 anacore-2.9.0/anacore/abstractFile.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     5967 2021-04-28 13:28:26.110516 anacore-2.9.0/anacore/annotVcf.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    12006 2021-01-29 16:47:20.371161 anacore-2.9.0/anacore/bed.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    15230 2021-01-29 16:47:20.371161 anacore-2.9.0/anacore/filters.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    64945 2021-04-28 13:28:26.110516 anacore-2.9.0/anacore/fusion.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    23681 2021-04-28 13:28:26.110516 anacore-2.9.0/anacore/genomicRegion.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    11007 2021-01-29 16:47:20.371161 anacore-2.9.0/anacore/gff.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    12155 2021-01-29 16:47:20.371161 anacore-2.9.0/anacore/gtf.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    35925 2021-04-28 13:28:26.118516 anacore-2.9.0/anacore/hgvs.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    23192 2021-04-28 13:28:26.118516 anacore-2.9.0/anacore/illumina.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     2792 2021-01-29 16:47:20.371161 anacore-2.9.0/anacore/maf.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     2576 2021-01-29 16:47:20.371161 anacore-2.9.0/anacore/matrix.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    37945 2021-01-29 16:47:20.371161 anacore-2.9.0/anacore/msi.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     4695 2021-01-29 16:47:20.371161 anacore-2.9.0/anacore/msiannot.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     7041 2021-01-29 16:47:20.371161 anacore-2.9.0/anacore/msings.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    10431 2021-01-29 16:47:20.371161 anacore-2.9.0/anacore/node.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     6027 2021-04-28 13:28:26.118516 anacore-2.9.0/anacore/picardIO.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    22413 2021-04-28 13:28:26.118516 anacore-2.9.0/anacore/region.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     8140 2021-04-28 13:28:26.118516 anacore-2.9.0/anacore/sequence.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    23107 2021-04-28 13:28:26.118516 anacore-2.9.0/anacore/sequenceIO.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     8946 2021-04-28 13:28:26.118516 anacore-2.9.0/anacore/sv.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     1772 2021-01-29 16:47:20.371161 anacore-2.9.0/anacore/tophatFusion.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    69027 2021-04-28 13:28:26.122516 anacore-2.9.0/anacore/vcf.py
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)       46 2021-04-28 13:28:26.206516 anacore-2.9.0/requirements.txt
--rw-rw-r--   0 fescudie  (1000) fescudie  (1000)       40 2021-01-29 16:47:20.543247 anacore-2.9.0/setup.cfg
--rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)     1259 2021-01-29 16:47:20.543247 anacore-2.9.0/setup.py
-drwxrwxr-x   0 fescudie  (1000) fescudie  (1000)        0 2021-05-01 14:51:48.097463 anacore-2.9.0/test/
--rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    11159 2021-01-29 16:47:20.543247 anacore-2.9.0/test/test_filters.py
--rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    83924 2021-04-28 13:28:26.206516 anacore-2.9.0/test/test_fusion.py
--rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    36421 2021-04-28 13:28:26.206516 anacore-2.9.0/test/test_genomicRegion.py
--rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)     5497 2021-01-29 16:47:20.543247 anacore-2.9.0/test/test_gff.py
--rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    41488 2021-01-29 16:47:20.543247 anacore-2.9.0/test/test_gtf.py
--rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    21546 2021-04-28 13:28:26.206516 anacore-2.9.0/test/test_hgvs.py
--rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    33675 2021-04-28 13:28:26.206516 anacore-2.9.0/test/test_illumina.py
--rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    17689 2021-04-28 13:28:26.206516 anacore-2.9.0/test/test_picardIO.py
--rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    33543 2021-04-28 13:28:26.206516 anacore-2.9.0/test/test_region.py
--rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)     4392 2021-04-28 13:28:26.210516 anacore-2.9.0/test/test_sequence.py
--rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    21240 2021-04-28 13:28:26.210516 anacore-2.9.0/test/test_sequenceIO.py
--rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    16865 2021-04-28 13:28:26.210516 anacore-2.9.0/test/test_sv.py
--rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    56017 2021-04-28 13:28:26.210516 anacore-2.9.0/test/test_vcf.py
+drwxrwxr-x   0 fescudie  (1000) fescudie  (1000)        0 2023-06-13 16:22:13.242614 anacore-3.0.0/
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    34494 2021-01-29 16:47:20.000000 anacore-3.0.0/LICENSE.txt
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)      290 2023-06-13 16:18:40.000000 anacore-3.0.0/MANIFEST.in
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)      362 2023-06-13 16:22:13.242614 anacore-3.0.0/PKG-INFO
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)      961 2023-06-13 16:18:40.000000 anacore-3.0.0/README.md
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     7807 2023-06-13 16:18:40.000000 anacore-3.0.0/RELEASES_NOTES.md
+drwxrwxr-x   0 fescudie  (1000) fescudie  (1000)        0 2023-06-13 16:22:13.214600 anacore-3.0.0/anacore/
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     4680 2021-01-29 16:47:20.000000 anacore-3.0.0/anacore/STARLog.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)        0 2021-01-29 16:47:20.000000 anacore-3.0.0/anacore/__init__.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     3783 2021-01-29 16:47:20.000000 anacore-3.0.0/anacore/abstractFile.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     9274 2021-09-28 10:01:20.000000 anacore-3.0.0/anacore/annotVcf.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    15046 2021-09-28 10:01:20.000000 anacore-3.0.0/anacore/bed.py
+drwxrwxr-x   0 fescudie  (1000) fescudie  (1000)        0 2023-06-13 16:22:13.218603 anacore-3.0.0/anacore/db/
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)        0 2021-09-28 10:01:20.000000 anacore-3.0.0/anacore/db/__init__.py
+drwxrwxr-x   0 fescudie  (1000) fescudie  (1000)        0 2023-06-13 16:22:13.218603 anacore-3.0.0/anacore/db/homo_sapiens/
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)        0 2021-09-28 10:01:20.000000 anacore-3.0.0/anacore/db/homo_sapiens/__init__.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     8460 2021-09-28 10:01:20.000000 anacore-3.0.0/anacore/db/homo_sapiens/accession.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    29631 2023-06-13 16:18:40.000000 anacore-3.0.0/anacore/filters.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    67727 2023-06-13 16:18:40.000000 anacore-3.0.0/anacore/fusion.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    23669 2021-09-28 10:01:20.000000 anacore-3.0.0/anacore/genomicRegion.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    13785 2023-06-13 16:18:40.000000 anacore-3.0.0/anacore/getterPath.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    11007 2021-01-29 16:47:20.000000 anacore-3.0.0/anacore/gff.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    12155 2021-01-29 16:47:20.000000 anacore-3.0.0/anacore/gtf.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    35925 2021-04-28 13:28:26.000000 anacore-3.0.0/anacore/hgvs.py
+drwxrwxr-x   0 fescudie  (1000) fescudie  (1000)        0 2023-06-13 16:22:13.218603 anacore-3.0.0/anacore/illumina/
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)        0 2023-06-13 16:18:40.000000 anacore-3.0.0/anacore/illumina/__init__.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     4820 2023-06-13 16:18:40.000000 anacore-3.0.0/anacore/illumina/base.py
+drwxrwxr-x   0 fescudie  (1000) fescudie  (1000)        0 2023-06-13 16:22:13.218603 anacore-3.0.0/anacore/illumina/demultiplex/
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     1977 2023-06-13 16:19:38.000000 anacore-3.0.0/anacore/illumina/demultiplex/__init__.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     4085 2023-06-13 16:18:40.000000 anacore-3.0.0/anacore/illumina/demultiplex/base.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     5499 2023-06-13 16:18:40.000000 anacore-3.0.0/anacore/illumina/demultiplex/bcl2fastq.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     6719 2023-06-13 16:18:40.000000 anacore-3.0.0/anacore/illumina/demultiplex/bclconvert.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    17621 2023-06-13 16:18:40.000000 anacore-3.0.0/anacore/illumina/run.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    24288 2023-06-13 16:18:40.000000 anacore-3.0.0/anacore/illumina/samplesheet.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     2792 2021-01-29 16:47:20.000000 anacore-3.0.0/anacore/maf.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     2576 2021-01-29 16:47:20.000000 anacore-3.0.0/anacore/matrix.py
+drwxrwxr-x   0 fescudie  (1000) fescudie  (1000)        0 2023-06-13 16:22:13.222604 anacore-3.0.0/anacore/msi/
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)        0 2022-09-06 14:11:15.000000 anacore-3.0.0/anacore/msi/__init__.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     4694 2022-09-06 14:11:15.000000 anacore-3.0.0/anacore/msi/annot.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    12498 2022-10-01 08:37:24.000000 anacore-3.0.0/anacore/msi/base.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    12212 2023-06-13 16:18:40.000000 anacore-3.0.0/anacore/msi/hubble.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    11249 2022-09-06 14:11:15.000000 anacore-3.0.0/anacore/msi/locus.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     9267 2022-09-06 14:11:15.000000 anacore-3.0.0/anacore/msi/msings.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    22704 2022-09-06 14:11:15.000000 anacore-3.0.0/anacore/msi/msisensorpro.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     2444 2022-09-06 14:11:15.000000 anacore-3.0.0/anacore/msi/reportIO.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    12939 2022-10-01 13:54:36.000000 anacore-3.0.0/anacore/msi/sample.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    10431 2021-01-29 16:47:20.000000 anacore-3.0.0/anacore/node.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     6027 2021-04-28 13:28:26.000000 anacore-3.0.0/anacore/picardIO.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    22413 2021-04-28 13:28:26.000000 anacore-3.0.0/anacore/region.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     8896 2022-09-06 14:11:15.000000 anacore-3.0.0/anacore/sequence.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    23301 2022-09-06 14:11:15.000000 anacore-3.0.0/anacore/sequenceIO.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     8946 2021-04-28 13:28:26.000000 anacore-3.0.0/anacore/sv.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     1772 2021-01-29 16:47:20.000000 anacore-3.0.0/anacore/tophatFusion.py
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)    82690 2023-06-13 16:18:40.000000 anacore-3.0.0/anacore/vcf.py
+drwxrwxr-x   0 fescudie  (1000) fescudie  (1000)        0 2023-06-13 16:22:13.218603 anacore-3.0.0/anacore.egg-info/
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)      362 2023-06-13 16:22:12.000000 anacore-3.0.0/anacore.egg-info/PKG-INFO
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)     1506 2023-06-13 16:22:13.000000 anacore-3.0.0/anacore.egg-info/SOURCES.txt
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)        1 2023-06-13 16:22:12.000000 anacore-3.0.0/anacore.egg-info/dependency_links.txt
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)       44 2023-06-13 16:22:13.000000 anacore-3.0.0/anacore.egg-info/requires.txt
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)        8 2023-06-13 16:22:13.000000 anacore-3.0.0/anacore.egg-info/top_level.txt
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)       47 2022-03-10 14:32:28.000000 anacore-3.0.0/requirements.txt
+-rw-rw-r--   0 fescudie  (1000) fescudie  (1000)       79 2023-06-13 16:22:13.242614 anacore-3.0.0/setup.cfg
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)     1275 2021-11-28 16:57:20.000000 anacore-3.0.0/setup.py
+drwxrwxr-x   0 fescudie  (1000) fescudie  (1000)        0 2023-06-13 16:22:13.238613 anacore-3.0.0/test/
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)     8204 2021-09-28 10:01:20.000000 anacore-3.0.0/test/test_bed.py
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    21718 2023-06-13 16:18:40.000000 anacore-3.0.0/test/test_filters.py
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    83924 2021-04-28 13:28:26.000000 anacore-3.0.0/test/test_fusion.py
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    36421 2021-04-28 13:28:26.000000 anacore-3.0.0/test/test_genomicRegion.py
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    16504 2023-06-13 16:18:40.000000 anacore-3.0.0/test/test_getterPath.py
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)     5497 2021-01-29 16:47:20.000000 anacore-3.0.0/test/test_gff.py
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    41488 2021-01-29 16:47:20.000000 anacore-3.0.0/test/test_gtf.py
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    21546 2021-04-28 13:28:26.000000 anacore-3.0.0/test/test_hgvs.py
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    17689 2021-04-28 13:28:26.000000 anacore-3.0.0/test/test_picardIO.py
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    33543 2021-04-28 13:28:26.000000 anacore-3.0.0/test/test_region.py
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)     5076 2022-09-06 14:11:15.000000 anacore-3.0.0/test/test_sequence.py
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    21720 2022-09-06 14:11:15.000000 anacore-3.0.0/test/test_sequenceIO.py
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    16865 2021-04-28 13:28:26.000000 anacore-3.0.0/test/test_sv.py
+-rwxrwxr-x   0 fescudie  (1000) fescudie  (1000)    71155 2023-06-13 16:18:40.000000 anacore-3.0.0/test/test_vcf.py
```

### Comparing `anacore-2.9.0/README.md` & `anacore-3.0.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# AnaCore
+# AnaCore <img src="doc/img/logo/anacore_logo_40deg.png" alt="logo" width=60 rotate="60"/>
+
 
 ![license](https://img.shields.io/badge/license-GPLv3-blue)
-![coverage](https://img.shields.io/badge/coverage-64%25-yellow)
+![coverage](https://img.shields.io/badge/coverage-82%25-green)
 
 ## Description
 Anapath Core is a package containing libraries for managing standard file
 formats (BED, fasta, gff, gtf, MAF, newick, VCF, ...) and objects from NGS.
 
 ## Installation
 ### From PyPI
```

### Comparing `anacore-2.9.0/anacore/STARLog.py` & `anacore-3.0.0/anacore/STARLog.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/anacore/abstractFile.py` & `anacore-3.0.0/anacore/abstractFile.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/anacore/bed.py` & `anacore-3.0.0/anacore/bed.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,107 @@
 # -*- coding: utf-8 -*-
-"""Classes and functions for reading/writing/processing BED files."""
+"""
+Classes and functions for reading/writing/processing BED files.
+
+:Code example:
+
+    Test if a file is a BED file
+
+    .. highlight:: python
+    .. code-block:: python
+
+        from anacore.bed import BEDIO
+
+        if BEDIO.isValid("test.txt.gz"):
+            print("The file is a BED file")
+
+        # Result>
+        # The file is a BED file
+
+    Read BED file by line
+
+    .. highlight:: python
+    .. code-block:: python
+
+        from anacore.bed import BEDIO
+
+        with BEDIO("test.bed.gz") as reader:
+            print("Region", "Name", sep="\\t")
+            for record in reader:
+                print(
+                    "{}:{}-{}({})".format(
+                        record.reference.name,
+                        record.start,
+                        record.end
+                        record.strand
+                    ),
+                    record.name,
+                    sep="\\t"
+                )
+
+        # Result>
+        # Region\tName
+        # chr1:158-367(-)\ttarget_01
+        # chr1:54899-54999(+)\ttarget_02
+
+    Read whole BED file and store by region
+
+    .. highlight:: python
+    .. code-block:: python
+
+        from anacore.bed import getSortedAreasByChr
+
+        areas_by_chr = getSortedAreasByChr("test.bed.gz")
+        print("Region", "Name", sep="\\t")
+        for chrom, areas_on_curr_chr in areas_by_chr.items():
+            for curr_area in areas_on_curr_chr:
+                print(
+                    "{}:{}-{}({})".format(
+                        curr_area.reference.name,
+                        curr_area.start,
+                        curr_area.end
+                        curr_area.strand
+                    ),
+                    curr_area.name,
+                    sep="\\t"
+                )
+
+        # Result>
+        # Region\tName
+        # chr1:158-367(-)\ttarget_01
+        # chr1:54899-54999(+)\ttarget_02
+
+    Write BED file from regions
+
+    .. highlight:: python
+    .. code-block:: python
+
+        from anacore.bed import BEDIO, BEDRecord
+        from anacore.region import Region
+
+        regions = [
+            Region(158, 367, "-", "chr1", "target_01"),
+            Region(54899, 54999, "+", "chr1", "target_02"),
+        ]
+
+        with BEDIO("test.bed.gz", "w", 6) as writer:  # Write BED file with 6 columns
+            for curr_region in regions:
+                writer.write(
+                    BEDRecord.recFromRegion(curr_region)
+                )
+
+        # Result>
+        # chr1\t157\t367\ttarget_01\t.\t-
+        # chr1\t54898\t54999\ttarget_02\t.\t+
+"""
 
 __author__ = 'Frederic Escudie'
 __copyright__ = 'Copyright (C) 2017 IUCT-O'
 __license__ = 'GNU General Public License'
-__version__ = '1.5.0'
+__version__ = '1.5.1'
 __email__ = 'escudie.frederic@iuct-oncopole.fr'
 __status__ = 'prod'
 
 from anacore.region import Region, RegionList
 from anacore.abstractFile import AbstractFile
 
 
@@ -123,15 +216,15 @@
             (record.start - 1),
             record.end,
             ("." if record.name is None else record.name),
             ("." if record.score is None else str(record.score)),
             ("." if record.strand is None else record.strand),
             ("." if record.thickStart is None else str(record.thickStart - 1)),
             ("." if record.thickEnd is None else str(record.thickEnd)),
-            ("." if record.itemRgb is None else ",".join(record.itemRgb)),
+            ("." if record.itemRgb is None else ",".join(map(str, record.itemRgb))),
             ("." if record.blockCount is None else str(record.blockCount)),
             ("." if record.blockSizes is None else ",".join(map(str, record.blockSizes))),
             ("." if record.blockStarts is None else ",".join(map(str, record.blockStarts)))
         )
         return line
 
     def isRecordLine(self, line):
@@ -154,31 +247,33 @@
         Return True if the file can be a BED file.
 
         :return: True if the file can be a BED file.
         :rtype: bool
         """
         is_valid = False
         try:
-            with BEDIO(filepath) as FH_in:
+            with BEDIO(filepath) as reader:
                 record_idx = 0
-                for record in FH_in:
+                for record in reader:
                     if record_idx >= 10:
                         break
-                    if record.strand is not None and record.strand not in ["+", "-", "."]:  # Check strand
+                    # Check strand
+                    if record.strand is not None and record.strand not in {"+", "-", "."}:
+                        raise IOError(
+                            "Invalid strand value in {} from file {}.".format(
+                                reader.current_line_nb, reader.filepath
+                            )
+                        )
+                    # Check RGB
+                    if record.itemRgb is not None and len(record.itemRgb) != 3:
                         raise IOError(
-                            "The line {} in \"{}\" cannot be parsed by {}.\nLine content: {}".format(
-                                FH_in.current_line_nb, FH_in.filepath, FH_in.__class__.__name__, FH_in.current_line
+                            "Invalid RGB code in {} from file {}.".format(
+                                reader.current_line_nb, reader.filepath
                             )
                         )
-                    # if record.itemRgb is not None and len(record.itemRgb.split(",")) != 3:
-                    #     raise IOError(
-                    #         "The line {} in \"{}\" cannot be parsed by {}.\nLine content: {}".format(
-                    #             FH_in.current_line_nb, FH_in.filepath, FH_in.__class__.__name__, FH_in.current_line
-                    #         )
-                    #     )
                     record_idx += 1
                 is_valid = True
         except Exception:
             pass
         return is_valid
 
     def _parseLine(self):
@@ -188,26 +283,32 @@
         :return: The record defined by the current line.
         :rtype: BEDrecord
         """
         fields = [elt.strip() for elt in self.current_line.split('\t')]
         fields[1] = int(fields[1]) + 1  # Start in BED is 0-based
         fields[2] = int(fields[2])
         nb_col = len(fields)
-        if nb_col >= 5:
-            fields[4] = None if fields[4] == "." else int(fields[4])  # A score between 0 and 1000. If the track line useScore attribute is set to 1 for this annotation data set, the score value will determine the level of gray in which this feature is displayed (higher numbers = darker gray).
-            if nb_col >= 7:
-                fields[6] = int(fields[6]) + 1  # The starting position at which the feature is drawn thickly (for example, the start codon in gene displays). When there is no thick part, thickStart and thickEnd are usually set to the chromStart position.
-                if nb_col >= 8:
-                    fields[7] = int(fields[7])  # The ending position at which the feature is drawn thickly (for example the stop codon in gene displays).
-                    if nb_col >= 10:
-                        fields[9] = int(fields[9])  # The number of blocks (exons) in the BED line.
-                        if nb_col >= 11:
-                            fields[10] = [int(block) for block in fields[10].split(",")]  # A comma-separated list of the block sizes. The number of items in this list should correspond to blockCount.
-                            if nb_col >= 12:
-                                fields[11] = [int(block) for block in fields[11].split(",")]  # A comma-separated list of block starts. All of the blockStart positions should be calculated relative to chromStart. The number of items in this list should correspond to blockCount.
+        if nb_col > 3:
+            fields[3] = None if fields[3] == "." else fields[3]
+            if nb_col > 4:
+                fields[4] = None if fields[4] == "." else int(fields[4])  # A score between 0 and 1000. If the track line useScore attribute is set to 1 for this annotation data set, the score value will determine the level of gray in which this feature is displayed (higher numbers = darker gray).
+                if nb_col > 5:
+                    fields[5] = None if fields[5] == "." else fields[5]
+                    if nb_col > 6:
+                        fields[6] = None if fields[6] == "." else int(fields[6]) + 1  # The starting position at which the feature is drawn thickly (for example, the start codon in gene displays). When there is no thick part, thickStart and thickEnd are usually set to the chromStart position.
+                        if nb_col > 7:
+                            fields[7] = None if fields[7] == "." else int(fields[7])  # The ending position at which the feature is drawn thickly (for example the stop codon in gene displays).
+                            if nb_col > 8:
+                                fields[8] = None if fields[8] in {".", "0"} else [int(color) for color in fields[8].split(",")]  # An RGB value of the form R,G,B (e.g. 255,0,0).
+                                if nb_col > 9:
+                                    fields[9] = None if fields[9] == "." else int(fields[9])  # The number of blocks (exons) in the BED line.
+                                    if nb_col > 10:
+                                        fields[10] = None if fields[10] == "." else [int(block) for block in fields[10].split(",")]  # A comma-separated list of the block sizes. The number of items in this list should correspond to blockCount.
+                                        if nb_col > 11:
+                                            fields[11] = None if fields[11] == "." else [int(block) for block in fields[11].split(",")]  # A comma-separated list of block starts. All of the blockStart positions should be calculated relative to chromStart. The number of items in this list should correspond to blockCount.
         return BEDRecord(*fields)
 
     def write(self, record):
         """
         Write record line in file.
 
         :param bed: The record to write.
```

### Comparing `anacore-2.9.0/anacore/fusion.py` & `anacore-3.0.0/anacore/fusion.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,75 @@
 # -*- coding: utf-8 -*-
-"""Classes and functions for reading/writing fusions callers's output and VCF containing fusions. Each record is converted to VCFRecord."""
+"""
+Classes and functions for reading/writing fusions callers's output and VCF containing fusions. Each record is converted to VCFRecord.
+
+:Example:
+
+    Read results form STAR-Fusion
+
+    .. highlight:: python
+    .. code-block:: python
+
+        # File content>
+        # #FusionName	JunctionReadCount	SpanningFragCount	SpliceType	LeftGene	LeftBreakpoint	RightGene	RightBreakpoint	LargeAnchorSupport	FFPM	LeftBreakDinuc	LeftBreakEntropy	RightBreakDinuc	RightBreakEntropy	annots
+        # MN1--BEND2	90	39	ONLY_REF_SPLICE	MN1^ENSG00000169184.6	chr22:27796763:-	BEND2^ENSG00000177324.14	chrX:18195442:-	YES_LDAS	38.9246	GT	1.9656	AG	1.7232	["INTERCHROMOSOMAL[chr22--chr9]"]
+
+        from anacore.fusion import FusionFileReader
+
+        spl_name = "spl1"
+        print("Breakpoint_1\\tGene_brkpt_1\\tBreakpoint_2\\tGene_brkpt_2\\tSpanning_pair\\tSplit_read")
+        with FusionFileReader.factory("test.tsv", sample_name=spl_name, annot_field="ANN") as reader:
+            for first, second in reader:
+                print(
+                    "{}:{}".format(first.chrom, frist.pos),
+                    ",".join([elt["SYMBOL"] for elt in first.info["ANN"]]),
+                    "{}:{}".format(second.chrom, second.pos),
+                    ",".join([elt["SYMBOL"] for elt in second.info["ANN"]]),
+                    first.samples[spl_name]["PR"],
+                    first.samples[spl_name]["SR"],
+                    sep="\\t"
+                )
+
+        # Result>
+        # Breakpoint_1\tGene_brkpt_1\tBreakpoint_2\tGene_brkpt_2\tSpanning_pair\tSplit_read
+        # chr22:27796763\tMN1\tchrX:18195442\tBEND2\t39\t99
+
+    Read VCF
+
+    .. highlight:: python
+    .. code-block:: python
+
+        from anacore.fusion import FusionFileReader
+
+        # File content>
+        # ##fileformat=VCFv4.3
+        # ##INFO=<ID=MATEID,Number=A,Type=String,Description="ID of mate breakend.">
+        # ##INFO=<ID=SVTYPE,Number=1,Type=String,Description="Type of structural variant.">
+        # #CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO
+        # 2	321682	bnd_V	T	]13:123456]T	6	PASS	SVTYPE=BND;MATEID=bnd_U
+        # 4	888888	.	T	G	.	PASS	.
+        # 13	123456	bnd_U	C	C[2:321682[,C[17:198983[	6	PASS	SVTYPE=BND;MATEID=bnd_V,bnd_Z
+        # 17	198983	bnd_Z	A	]13:123456]A	6	PASS	SVTYPE=BND;MATEID=bnd_U
+
+        print("Breakpoint_1\\tBreakpoint_1_name\\tBreakpoint_2\\tBreakpoint_2_name")
+        with FusionFileReader.factory("test.vcf") as reader:
+            for first, second in reader:
+                print(
+                    "{}:{}".format(first.chrom, frist.pos),
+                    first.id,
+                    "{}:{}".format(second.chrom, second.pos),
+                    second.id,
+                    sep="\\t"
+                )
+
+        # Result>
+        # Breakpoint_1\tBreakpoint_1_name\tBreakpoint_2\tBreakpoint_2_name
+        # 2:321682\tbnd_V\t13:123456\tbnd_U_0
+        # 13:123456\tbnd_U_1\t17:198983\tbnd_Z
+"""
 """
 Alt representation in VCF specification:
 
     First in RNA and strand + => alt: N|
                     ------>
                            |
         >>>>>>>>>>>>>>     |     >>>>>>>>>>>>
```

### Comparing `anacore-2.9.0/anacore/genomicRegion.py` & `anacore-3.0.0/anacore/genomicRegion.py`

 * *Files 0% similar despite different names*

```diff
@@ -187,20 +187,18 @@
                     found = True
                 else:  # In previous intron
                     raise Exception("Position {}:{} is in intron of {}.".format(self.reference.name, chr_pos, self))
         return transcript_pos
 
     def getSubFromRegionPos(self, transcript_pos):
         """
-        Return exon and coordinate on his from the coordinate on transcript.
+        Return exon and coordinate on its from coordinate on transcript. Coordinate on exon is stranded:
 
-        Coordinate on exon is stranded:
-
-        - pos 2 in region test:10-20(+) correspond to ref position 12
-        - pos 2 in region test:10-20(-) correspond to ref position 18
+            * pos 2 in region test:10-20(+) correspond to ref position 12
+            * pos 2 in region test:10-20(-) correspond to ref position 18
 
         :param transcript_pos: The coordinate on transcript (1-based).
         :type transcript_pos: int
         :return: Exon and coordinate on exon (1-based).
         :rtype: (genomicRegion.Exon, int)
         """
         if transcript_pos > self.length():
@@ -421,18 +419,18 @@
                     chained_cds_pos += cds[cds_idx].length()
                     cds_idx += 1
                 chained_cds_pos += cds[cds_idx].end - chr_pos + 1
         return chained_cds_pos
 
     def getSubFromRegionPos(self, protein_pos, codon_pos):
         """
-        Return CDS and coordinate on his from the coordinate on protein.
-        The coordinate on CDS is stranded:
-            With region test:10-20(+) the pos 2 correspond to ref position 12
-            With region test:10-20(-) the pos 2 correspond to ref position 18
+        Return CDS and coordinate on its from coordinate on protein. The coordinate on CDS is stranded:
+
+            * With region test:10-20(+) the pos 2 correspond to ref position 12
+            * With region test:10-20(-) the pos 2 correspond to ref position 18
 
         :param protein_pos: Coordinate of the amino acid on protein (1-based).
         :type protein_pos: int.
         :param codon_pos: Coordinate on the codon (1-based).
         :type codon_pos: int.
         :return: CDS and coordinate on CDS (1-based).
         :rtype: genomicRegion.CDS, int
```

### Comparing `anacore-2.9.0/anacore/gff.py` & `anacore-3.0.0/anacore/gff.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/anacore/gtf.py` & `anacore-3.0.0/anacore/gtf.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/anacore/hgvs.py` & `anacore-3.0.0/anacore/hgvs.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/anacore/illumina.py` & `anacore-3.0.0/anacore/illumina/samplesheet.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,571 +1,593 @@
 # -*- coding: utf-8 -*-
-"""Classes and functions for reading Illumina's files (samplesheet, runInfo, runParameters, ...) and parsing header, filenames and run folder informations."""
+"""
+Classes and functions for reading Illumina's samplesheet.
+
+:Code example:
+
+    List samples and index from the samplesheet
+
+    .. highlight:: python
+    .. code-block:: python
+
+        from anacore.illumina.samplesheet import SampleSheetFactory
+
+        samplesheet = SampleSheetFactory.get("my_run/SampleSheet.csv"):
+        print("Samples:")
+        for spl in samplesheet.samples:
+            print("", spl.library_basename, spl.barcodes)
+
+        # Result>
+        # Samples:
+        #  sapmleA_S1 {"index": "TATCTTCAGC", "index2": "CGAATATTGG"}
+        #  sampleB_S2 {"index": "TGCACGGATA", "index2": "GTTGTCTGCG"}
+        #  sampleC_S3 {"index": "GGTTGATAGA", "index2": "TCTGCTCCGA"}
+"""
 
 __author__ = 'Frederic Escudie'
-__copyright__ = 'Copyright (C) 2017 IUCT-O'
+__copyright__ = 'Copyright (C) 2017 CHU Toulouse'
 __license__ = 'GNU General Public License'
-__version__ = '1.19.0'
+__version__ = '2.0.0'
 __email__ = 'escudie.frederic@iuct-oncopole.fr'
 __status__ = 'prod'
 
+from anacore.illumina.base import getIlluminaName
+import glob
 import os
 import re
-import glob
-import datetime
-import xml.etree.ElementTree as ET
 
 
-class SampleSheetIO(object):
-    """Reader for SampleSheet.csv."""
+class AbstractSampleSheet(object):
+    """Abstract reader for SampleSheet.csv."""
 
-    SECTIONS = ["Header", "Manifests", "Reads", "Settings", "Data"]
+    # REQUIRED_SECTIONS = {"Header", "Reads", "Settings", "Data"}
+    # DEMULTIPLEX_SECTION = "Reads"
+    # SAMPLES_SECTION = "Data"
 
     def __init__(self, path):
+        """
+        Build and return an instance of AbstractSampleSheet.
+
+        :param path: Path to samplesheet (format: CSV).
+        :type path: str
+        :return: The new instance.
+        :rtype: AbstractSampleSheet
+        """
+        self.extra = None
         self.filepath = path
-        self.run = None
-        self.samples = None
         self.header = None
         self.manifests = None
+        self.reads = None
+        self.samples = None
         self._parse()
 
-    def _parse(self):
-        # Retrieve information by section
-        with open(self.filepath) as FH_sheet:
+    @staticmethod
+    def cleanedEnd(value):
+        """
+        Return line without ending empty CSV fields. This method can be used to removes invalid comma used in CSV to obtain the same number of columns in whole file.
+
+        :param value: Line to clean.
+        :type value: str
+        :return: Line without ending empty CSV fields.
+        :rtype: str
+        """
+        value = value.strip()
+        while value.endswith(","):
+            value = value[:-1].strip()
+        return value
+
+    def _getInfoFromSection(self, section):
+        """
+        Return keys and values contained in section.
+
+        :param section: Lines from section. Each row contains one key and corresponding value.
+        :type section: list
+        :return: Keys and values contained in section.
+        :rtype: dict
+        """
+        info = dict()
+        for line in section:
+            key, value = [field.strip() for field in line.split(",", 1)]
+            value = AbstractSampleSheet.cleanedEnd(value)
+            info[key] = value
+        return info
+
+    def _getInfoFromTitledSection(self, section):
+        """
+        Return titles and list of entries (Keys and values for one element).
+
+        :param section: Lines from section with a titles row. Each row contains one entry where columns correspond to key and cells to values.
+        :type section: list
+        :return: Titles and list of entries (Keys and values for one element).
+        :rtype: (list, list)
+        """
+        titles_line = AbstractSampleSheet.cleanedEnd(section[0])
+        titles = titles_line.split(",")
+        rows = list()
+        for line in section[1:]:
+            fields = [elt.strip() for elt in line.split(",")]
+            while len(fields) < len(titles):
+                fields.append("")
+            rows.append(
+                {title: fields[idx] for idx, title in enumerate(titles)}
+            )
+        return titles, rows
+
+    def _getReads(self, reads_section):
+        """
+        Returns reads phase(s). Each phase is described by its type (is_index) and by its number of cycles (nb_cycles).
+
+        :param reads_section: Lines from desction "Reads".
+        :type reads_section: list
+        :return: Reads phase(s). Each phase is described by its type (is_index) and by its number of cycles (nb_cycles).
+        :rtype: list
+        """
+        raise NotImplementedError
+
+    def _getSamplesFromData(self, data_section):
+        """
+        Return samples list containing for each: keys and values from data section as dict.
+
+        :param section: Lines from section with a titles row. Each row contains one entry where columns correspond to key and cells to values.
+        :type section: list
+        :return: Samples list as anacore.illumina.samplesheet.Sample.
+        :rtype: list
+        """
+        samples_obj = list()
+        titles, samples = self._getInfoFromTitledSection(data_section)
+        protected_fields = {"sample_id", "sample_description", "description", "index", "index2"}
+        spl_idx = 1  # Index come from position in Data (for V1) or BCLConvert_Data (for V3) list afterremove same Sample_ID
+        spl_idx_by_id = dict()
+        lib_by_barcode = dict()
+        for spl in samples:
+            spl_id = spl["Sample_ID"]
+            barcodes = dict()
+            if "index" in spl:
+                barcodes["index"] = spl["index"]
+            if "index2" in spl:
+                if "index" not in spl:
+                    barcodes["index"] = ""
+                barcodes["index2"] = spl["index2"]
+            barcodes_str = "+".join([str(val) for key, val in sorted(barcodes.items())])
+            if barcodes_str in lib_by_barcode:  # Same lib on multiple lanes
+                if "Lane" in spl:
+                    lib_by_barcode[barcodes_str].metadata["Lane"] += "," + spl["Lane"]
+                else:
+                    raise Exception("Sample {} is repeated with same barcodes: {}".format(spl_id, barcodes_str))
+            else:  # New library
+                # Get description
+                description = None
+                if "Sample_Description" in spl:
+                    description = spl["Sample_Description"]
+                elif "Description" in spl:
+                    description = spl["Description"]
+                # Get metadata
+                meta = dict()
+                for key, val in spl.items():
+                    lower_key = key.lower()
+                    if lower_key not in protected_fields:
+                        meta[key] = val
+                # Store library
+                lib_spl_idx = spl_idx
+                if spl_id in spl_idx_by_id:  # Different libraries with same sample ID
+                    lib_spl_idx = spl_idx_by_id[spl_id]  # Libraries with same sample ID keep the same S{idx}
+                else:  # New sample
+                    spl_idx_by_id[spl_id] = lib_spl_idx
+                    spl_idx += 1
+                lib_obj = Sample(lib_spl_idx, spl_id, barcodes, description, meta)
+                samples_obj.append(lib_obj)
+                lib_by_barcode[barcodes_str] = lib_obj
+        return samples_obj
+
+    def _getSections(self):
+        """
+        Read file content and return by section its lines.
+
+        :return: By section title its content as list of rows.
+        :rtype: dict
+        """
+        sections_by_title = dict()
+        with open(self.filepath) as reader:
             sections_by_title = dict()
             section_title = None
-            for line in FH_sheet:
+            for line in reader:
                 striped_line = line.strip()
-                if any([re.fullmatch("\[" + elt + "\],*", striped_line) for elt in SampleSheetIO.SECTIONS]):
-                    while striped_line.endswith(","):  # Removes invalid comma used in CSV to obtain the same number of columns in whole file
-                        striped_line = striped_line[:-1]
+                if re.fullmatch(r"\[[^]]+\],*", striped_line):  # New section
+                    striped_line = AbstractSampleSheet.cleanedEnd(striped_line)
                     section_title = striped_line[1:-1]
                     sections_by_title[section_title] = list()
-                elif re.fullmatch(",*", striped_line):
+                elif re.fullmatch(r",*", striped_line):  # Empty line
                     section_title = None
-                else:
+                else:  # Section content
                     sections_by_title[section_title].append(striped_line)
+        return sections_by_title
+
+    def _parse(self):
+        """Read file content and store information on the instance's attributes."""
+        # Retrieve information by section
+        sections_by_title = self._getSections()
         # Process information
-        self.samples = self._getSamplesFromData(sections_by_title["Data"])
-        self.header = self._getInfoFromSection(sections_by_title["Header"])
-        self.manifests = self._getInfoFromSection(sections_by_title["Manifests"]) if "Manifests" in sections_by_title else dict()
-        self.run = self._getRunFromHeaderAndReads(sections_by_title["Header"], sections_by_title["Reads"])
+        cls = self.__class__
+        self.header = self._getInfoFromSection(
+            sections_by_title["Header"]
+        )
+        self.manifests = dict()
+        if "Manifests" in sections_by_title:
+            self.manifests = self._getInfoFromSection(sections_by_title["Manifests"])
+        self.samples = self._getSamplesFromData(
+            sections_by_title[cls.SAMPLES_SECTION]
+        )
+        self.reads = self._getReads(
+            sections_by_title[cls.DEMULTIPLEX_SECTION]
+        )
+        self.extra = dict()
+        for title, data in sections_by_title.items():
+            if title not in cls.REQUIRED_SECTIONS and title != "Manifests":
+                if title.endswith("_Data") or title.endswith("_Settings"):
+                    title, sub_title = title.rsplit("_", 1)
+                    sub_title = sub_title.lower()
+                    if title not in self.extra:
+                        self.extra[title] = dict()
+                    if sub_title == "data":
+                        self.extra[title][sub_title] = self._getInfoFromTitledSection(data)[1]
+                    else:
+                        self.extra[title][sub_title] = self._getInfoFromSection(data)
+                else:
+                    self.extra[title] = self._getInfoFromSection(data)
+        # Post process
+        if "Description" not in self.header:
+            self.header["Description"] = ""
 
-    def _getSamplesFromData(self, data_section):
-        samples = list()
-        data_titles = [field.strip() for field in data_section[0].split(",")]
-        for spl_idx, line in enumerate(data_section[1:]):
-            spl = {data_titles[idx]: field.strip() for idx, field in enumerate(line.split(","))}
-            spl["Sample_Basename"] = getIlluminaName(spl["Sample_ID"])
-            spl["Library_Basename"] = spl["Sample_Basename"] + "_S" + str(spl_idx + 1)
-            samples.append(spl)
-        return samples
 
-    def _getInfoFromSection(self, section):
-        info = dict()
-        for line in section:
-            key, value = [field.strip() for field in line.split(",", 1)]
-            while value.endswith(","):  # Removes invalid comma used in CSV to obtain the same number of columns in whole file
-                value = value[:-1]
-            info[key] = value
-        return info
+class Sample:
+    """Class to manage a sample from sample sheet. One sample could represent several libraries if they are the same sample ID."""
 
-    def _getRunFromHeaderAndReads(self, header_section, reads_section):
-        run = dict()
-        # Header
-        for line in header_section:
-            key, value = line.split(",", 1)
-            while value.endswith(","):  # Removes invalid comma used in CSV to obtain the same number of columns in whole file
-                value = value[:-1]
-            run[key] = value
-        # Reads
-        read_idx = 1
-        for line in reads_section:
-            striped_line = line.strip()
-            while striped_line.endswith(","):  # Removes invalid comma used in CSV to obtain the same number of columns in whole file
-                striped_line = striped_line[:-1]
-            run["nb_cycles_R" + str(read_idx)] = int(striped_line)
-            read_idx += 1
-        return run
+    def __init__(self, sheet_index, id, barcodes=None, description=None, metadata=None):
+        """
+        Build and return an instance of Sample.
 
+        :param sheet_index: Index of sample in samplesheet (start from 1). This element is used for library name: <splID>_S<splSheetIndex>.
+        :type sheet_index: int
+        :param id: Sample ID (example: splA).
+        :type id: str
+        :param barcodes: Sample molecular index used in demultiplex. Example:
+            * For single-end: {"index": "ATGC"}
+            * For paired-end: {"index": "ATGC", "index2": "CGCA"}
+            * For paired-end with skipped index 1: {"index": "", "index2": "CGCA"}
+        :type barcodes: dict
+        :param description: Sample description.
+        :type description: str
+        :param metadata: Additional data on sample (example: {"panel": "Enrich_Soli-Tumor_V3", "project": "Rimo"}). These data come from additional column in section Data.
+        :type metadata: dict
+        :return: The new instance.
+        :rtype: Sample
+        """
+        self.barcodes = dict() if barcodes is None else barcodes
+        self.description = description
+        self.id = id
+        self.sheet_index = sheet_index
+        self.metadata = dict() if metadata is None else metadata
 
-class ADSSampleSheetIO(SampleSheetIO):
-    """Reader for SampleSheet.csv designed for AmpliconDS analysis."""
+    @property
+    def basename(self):
+        """
+        Return the start of file basename corresponding to the sample (example: splA).
 
-    def _getSamplesFromData(self, data_section):
-        samples = super()._getSamplesFromData(data_section)
-        for spl_idx, spl in enumerate(samples):
-            spl["Sample_Basename"] = getIlluminaName(spl["Sample_Name"])
-            spl["Library_Basename"] = spl["Sample_Basename"] + "_S" + str(spl_idx + 1)
-        return samples
+        :return: Sample basename.
+        :rtype: str
+        """
+        return getIlluminaName(self.id)
 
-    def filterPanels(self, selected_manifests):
+    @property
+    def library_basename(self):
         """
-        Filter samples and manifests on their panel.
+        Return the start of file basename corresponding to the library (example: splA_S3).
 
-        :param selected_manifests: The manifests corresponding to the selected panel.
-        :type selected_manifests: list
+        :return: Library basename.
+        :rtype: str
         """
-        # Get kept
-        new_manifests = {}
-        new_by_old_id = {}
-        new_idx = 0
-        for manifest_id in sorted(self.manifests):
-            manifest_file = self.manifests[manifest_id]
-            if manifest_file in selected_manifests:
-                new_manifest_id = chr(ord("A") + new_idx)
-                new_by_old_id[manifest_id] = new_manifest_id
-                new_manifests[new_manifest_id] = self.manifests[manifest_id]
-                new_idx += 1
-        # Update manifests
-        self.manifests = new_manifests
-        # Update samples
-        new_spl = list()
-        for spl in self.samples:
-            if spl["Manifest"] in new_by_old_id:
-                if spl["Sample_ID"].endswith("_" + spl["Manifest"]):
-                    spl["Sample_ID"] = spl["Sample_ID"].rsplit("_" + spl["Manifest"], 1)[0]
-                    spl["Sample_ID"] += "_" + new_by_old_id[spl["Manifest"]]
-                spl["Manifest"] = new_by_old_id[spl["Manifest"]]
-                new_spl.append(spl)
-        self.samples = new_spl
+        return "{}_S{}".format(self.basename, self.sheet_index)
+
+    def toDict(self):
+        """
+        Return dict representation of the instance.
+
+        :return: Dict representation of the instance.
+        :rtype: dict
+        """
+        res = self.__dict__
+        res["basename"] = self.basename
+        res["library_basename"] = self.library_basename
+        return res
+
+
+class SampleADS(Sample):
+    """Class to manage an amplicon double strand sample from sample sheet. One sample could represent several libraries if they are the same sample ID."""
+
+    @property
+    def basename(self):
+        """
+        Return the start of file basename corresponding to the sample (example: splA).
+
+        :return: Sample basename.
+        :rtype: str
+        """
+        return getIlluminaName(self.metadata["Sample_Name"])
 
     def findSplFiles(self, directory, end_pattern, subject="library"):
         """
-        Return by sample name or library name all the files in directory corresponding to the subject.
+        Return paths to files in directory corresponding to the subject.
 
         :param directory: The path to the directory where the files names are evaluated.
         :type directory: str
-        :param end_pattern: File pattern added at the end of each sample basename or library basename to select files.
+        :param end_pattern: File pattern added at the end of sample basename or library basename to select files.
         :type end_pattern: str
         :param subject: "library" or "sample" to select files corresponding to libraries or corresponding to samples.
         :type subject: str
-        :return: By subject the pathes of the corresponding files.
-        :rtype: dict
+        :return: Paths of the corresponding files.
+        :rtype: list
         """
-        subject_start_tag = subject.capitalize()
-        files_by_elt = {}
-        for spl in self.samples:
-            if subject == "library" or spl["Sample_Name"] not in files_by_elt:  # The subject is the library or the subject is the sample and no library has been already processed for this sample
-                files_by_elt[spl[subject_start_tag + "_Name"]] = sorted(glob.glob(
-                    os.path.join(directory, spl[subject_start_tag + "_Basename"] + end_pattern)
-                ))
-        return files_by_elt
+        selector = self.libray_basename if subject == "library" else self.basename
+        return sorted(
+            glob.glob(
+                os.path.join(directory, selector + end_pattern)
+            )
+        )
 
     def setSplFiles(self, tag, directory, end_pattern, subject="library"):
         """
         Add the files in directory corresponding to the subject. These information are keyed by provided tag for each element of self.samples.
 
-        :param tag: The attribute used in self.sample to store the files pathes.
+        :param tag: The attribute used in self.sample to store the files paths.
         :type tag: str
         :param directory: The path to the directory where the files names are evaluated.
         :type directory: str
         :param end_pattern: File pattern added at the end of each sample basename or library basename to select files.
         :type end_pattern: str
         :param subject: "library" or "sample" to select files corresponding to libraries or corresponding to samples.
         :type subject: str
         """
-        subject_tag = subject.capitalize() + "_Name"
-        files_by_spl = self.findSplFiles(directory, end_pattern, subject)
-        for spl in self.samples:
-            spl[tag] = files_by_spl[spl[subject_tag]]
+        self.metadata[tag] = self.findSplFiles(directory, end_pattern, subject)
 
 
-class RTAComplete(object):
-    """Reader for RTAComplete.txt."""
+class SampleSheetFactory(object):
+    """Factory to identify and return version compliant handler to SampleSheet."""
 
-    def __init__(self, path):
-        self.filepath = path
-        self.end_date = None
-        self.RTA_version = None
-        self._parse()
+    @staticmethod
+    def get(filepath, *args, **kwargs):
+        """
+        Return instance of SampleSheet corresponding to the file.
 
-    def _parse(self):
-        with open(self.filepath) as FH_in:
-            content = FH_in.read().strip()
-            match = re.fullmatch("(.+/.+/.+,.+),Illumina RTA (.+)", content)
-            if match:  # 11/1/2017,15:11:43.174,Illumina RTA 1.18.54
-                date_str, self.RTA_version = match.groups()
-                if "." in date_str and ".":
-                    date_str = date_str.split(".")[0]
-                self.end_date = datetime.datetime.strptime(date_str, '%m/%d/%Y,%H:%M:%S')
-            else:
-                match = re.fullmatch("RTA (.+) completed on (.+/.+/.+ .+:.+:.+ ..)", content)
-                if match:  # RTA 2.4.11 completed on 11/14/2019 4:56:45 AM
-                    self.RTA_version, date_str = match.groups()
-                    self.end_date = datetime.datetime.strptime(date_str, '%m/%d/%Y %I:%M:%S %p')
-                else:
-                    raise Exception('"{}" in {} cannot be parsed by {}.'.format(content, self.filepath, self.__class__.__name__))
+        :param filepath: Path to the samplesheet (format: CSV).
+        :type filepath: str
+        :return: Instance of SampleSheet corresponding to the file.
+        :rtype: AbstractSampleSheet
+        """
+        if SampleSheetV2.isValid(filepath):
+            return SampleSheetV2(filepath, *args, **kwargs)
+        elif SampleSheetADS.isValid(filepath):
+            return SampleSheetADS(filepath, *args, **kwargs)
+        elif SampleSheetV1.isValid(filepath):
+            return SampleSheetV1(filepath, *args, **kwargs)
+        else:
+            raise IOError("The file {} does not have a valid format for SampleSheetReader.".format(filepath))
 
 
-class RunInfo(object):
-    """Reader for RunInfo.xml."""
+class SampleSheetV1(AbstractSampleSheet):
+    """Reader for SampleSheet.csv in V1 format (see: https://www.illumina.com/content/dam/illumina-marketing/documents/products/technotes/sequencing-sheet-format-specifications-technical-note-970-2017-004.pdf)."""
 
-    def __init__(self, path):
-        self.filepath = path
-        self.flowcell = None  # {'id': 'HN33VBGX5', 'layout': {'LaneCount': '4', 'SurfaceCount': '2', 'SwathCount': '3', 'TileCount': '12', 'SectionPerLane': '3', 'LanePerSection': '2'}}
-        self.instrument = None  # {'id': 'NS500523', 'platform': 'NextSeq'}
-        self.reads_phases = None  # [{'is_index': False, 'nb_cycles': 151}, {'is_index': True, 'nb_cycles': 8}, {'is_index': True, 'nb_cycles': 8}, {'is_index': False, 'nb_cycles': 151}]
-        self.run = None  # {'number': '133', 'id': '180406_NS500523_0133_AHN33VBGX5', 'start_date': datetime.datetime(2018, 4, 6, 0, 0)}
-        self._parse()
+    REQUIRED_SECTIONS = {"Header", "Reads", "Settings", "Data"}
+    DEMULTIPLEX_SECTION = "Reads"
+    SAMPLES_SECTION = "Data"
 
-    def _parse(self):
-        # Retrieve information by section
-        tree = ET.parse(self.filepath)
-        run = tree.getroot().find("Run")
-        # Process information
-        self.instrument = self._getInstrumentFromRun(run)
-        self.reads_phases = self._getReadsFromRun(run.find("Reads"))
-        self.run = self._getRunFromRun(run)
-        self.flowcell = self._getFlowcellFromRun(run)
-
-    def _getReadsFromRun(self, reads_tree):
-        reads = list()
-        for child in reads_tree:
-            reads.append({
-                "is_index": (child.get("IsIndexedRead") == "Y"),
-                "nb_cycles": int(child.get("NumCycles"))
-            })
-        return reads
-
-    def _getInstrumentFromRun(self, run_tree):
-        serial_number = run_tree.find("Instrument").text
-        return {
-            "id": serial_number,
-            "platform": platformFromInstrumentSerialNumber(serial_number)
-        }
-
-    def _getRunFromRun(self, run_tree):
-        date_str = run_tree.find("Date").text
-        start_date = None
-        if len(date_str) == 6:
-            start_date = datetime.datetime.strptime(date_str, '%y%m%d')
-        elif len(date_str) == 8:
-            start_date = datetime.datetime.strptime(date_str, '%Y%m%d')
-        else:
-            start_date = datetime.datetime.strptime(date_str, '%m/%d/%Y %I:%M:%S %p')
-        return {
-            "number": run_tree.attrib["Number"],
-            "id": run_tree.attrib["Id"],
-            "start_date": start_date
-        }
-
-    def _getFlowcellFromRun(self, run_tree):
-        return {
-            "id": run_tree.find("Flowcell").text,
-            "layout": run_tree.find("FlowcellLayout").attrib
-        }
+    def _getReads(self, reads_section):
+        """
+        Returns number of cycles in reads phase(s). Index cycles are ignored.
 
+        :param reads_section: Lines from desction "Reads".
+        :type reads_section: list
+        :return: Number of cycles in reads phase(s). Index cycles are ignored.
+        :rtype: dict
+        """
+        cycles = dict()
+        read_idx = 1
+        for line in reads_section:
+            striped_line = AbstractSampleSheet.cleanedEnd(line)
+            cycles["R{}".format(read_idx)] = int(striped_line)
+            read_idx += 1
+        return {"nb_cycles": cycles}
 
-class RunParameters(object):
-    """Reader for runParameters.xml."""
+    @staticmethod
+    def isValid(filepath):
+        """
+        Return true if the file is in SamplSheet V1 format.
 
-    def __init__(self, path):
-        self.filepath = path
-        self.kit = None  # {"flowcell_id": "H14U5BGXX", "reagent_kit_id": "NS2044178-REAGT"}
-        self.instrument = None  # {"id": "NS500413", "platform": "NextSeq"}
-        self.reads_phases = None  # [{'is_index': False, 'nb_cycles': 151}, {'is_index': True, 'nb_cycles': 8}, {'is_index': True, 'nb_cycles': 8}, {'is_index': False, 'nb_cycles': 151}]
-        self.run = None  # {"number": "0033", "id": "141107_NS500413_0033_H14U5BGXX", "start_date": datetime}
-        self.post_process = None  # "GenerateFASTQ"
-        self.software = None  # {"RTA": "2.11.3", "CS": "4.0.1.41"}
-        self._parse()
+        :param filepath: The file path.
+        :type filepath: str
+        :return: True if the file is in SamplSheet V1 format.
+        :rtype: bool
+        """
+        is_valid = False
+        try:
+            sections = set()
+            with open(filepath) as reader:
+                for line in reader:
+                    striped_line = line.strip()
+                    if re.fullmatch(r"\[[^]]+\],*", striped_line):
+                        title = AbstractSampleSheet.cleanedEnd(striped_line)[1:-1]
+                        sections.add(title)
+                    elif striped_line.startswith("FileFormatVersion,"):
+                        if striped_line.split(",")[1] != "1":
+                            raise Exception('Invalid format declaration.')
+            if len(SampleSheetV1.REQUIRED_SECTIONS - sections) != 0:
+                raise Exception('Missing core sections: {}.'.format(SampleSheetV1.REQUIRED_SECTIONS - sections))
+            is_valid = True
+        except FileNotFoundError:
+            raise
+        except Exception:
+            pass
+        return is_valid
+
+
+class SampleSheetV2(AbstractSampleSheet):
+    """Reader for SampleSheet.csv in V2 format (see: https://sapac.support.illumina.com/content/dam/illumina-support/documents/documentation/system_documentation/NextSeq2000/SampleSheet_v2_template.csv)."""
+
+    REQUIRED_SECTIONS = {"Header", "Reads", "BCLConvert_Data", "BCLConvert_Settings"}
+    DEMULTIPLEX_SECTION = "Reads"
+    SAMPLES_SECTION = "BCLConvert_Data"
+
+    def _getReads(self, reads_section):
+        """
+        Returns reads phase(s). Each phase is described by its type (is_index) and by its number of cycles (nb_cycles).
+
+        :param reads_section: Lines from desction "Reads".
+        :type reads_section: list
+        :return: Reads phase(s). Each phase is described by its type (is_index) and by its number of cycles (nb_cycles).
+        :rtype: list
+        """
+        reads_info = self._getInfoFromSection(reads_section)
+        reads_phases = list()
+        for phase in ["Read1Cycles", "Index1Cycles", "Index2Cycles", "Read2Cycles"]:
+            if phase in reads_info:
+                reads_phases.append(
+                    {'is_index': phase.startswith("Index"), 'nb_cycles': int(reads_info[phase])}
+                )
+        return {"phases": reads_phases}
 
     def _parse(self):
-        # Retrieve information by section
-        tree = ET.parse(self.filepath)
-        root = tree.getroot()
-        if {"Version", "Setup"} == {child.tag for child in root}:  # For HiSeq information are all in <Setup> under <RunParameters>
-            root = [child for child in root if child.tag == "Setup"][0]
-        # Process information
-        self.instrument = self._getInstrumentFromRoot(root)
-        reads_subtree = root.find("Reads")
-        if reads_subtree is not None:
-            self.reads_phases = self._getReadsFromSection(reads_subtree)
-        else:
-            self.reads_phases = self._getReadsFromSetup(root.find("Setup"))
-        self.run = self._getRunFromRoot(root)
-        self.kit = self._getKitFromRoot(root)
-        self.post_process = self._getPostProcessFromRoot(root)
-        self.software = self._getSoftwareFromRoot(root)
-
-    def _getReadsFromSetup(self, subtree):
-        reads = list()
-        indices = list()
-        for child in subtree:
-            if child.tag.startswith("Read"):
-                reads.append({
-                    "is_index": False,
-                    "nb_cycles": int(child.text)
-                })
-            elif child.tag.startswith("Index"):
-                indices.append({
-                    "is_index": True,
-                    "nb_cycles": int(child.text)
-                })
-        phases = [reads[0]]
-        for curr in indices:
-            phases.append(curr)
-        for curr in reads[1:]:
-            phases.append(curr)
-        return phases
-
-    def _getReadsFromSection(self, subtree):
-        reads = list()
-        for child in subtree:
-            reads.append({
-                "is_index": (child.get("IsIndexedRead") == "Y"),
-                "nb_cycles": int(child.get("NumCycles"))
-            })
-        return reads
-
-    def _getInstrumentFromRoot(self, root):
-        serial_number = root.find("ScannerID")
-        if serial_number is None:
-            serial_number = root.find("InstrumentID")
-        serial_number = serial_number.text
-        return {
-            "id": serial_number,
-            "platform": platformFromInstrumentSerialNumber(serial_number)
-        }
-
-    def _getRunFromRoot(self, root):
-        run_number = root.find("RunNumber")
-        if run_number is None:
-            run_number = root.find("ScanNumber")
-        run_number = run_number.text.lstrip("0")
-        return {
-            "number": run_number,
-            "id": root.find("RunID").text,
-            "start_date": datetime.datetime.strptime(root.find("RunStartDate").text, '%y%m%d')
-        }
-
-    def _getPostProcessFromRoot(self, root):
-        workflow = root.find("AnalysisWorkflowType")  # NextSeq style
-        if workflow is None:
-            workflow_markup = root.find("Workflow")  # MiSeq style
-            if workflow_markup is not None:
-                workflow = workflow_markup.find("Analysis")
-            # Else HiSeq does not process any post-processing
-        if workflow is not None:
-            workflow = None if workflow.text == "" else workflow.text
-        return workflow
-
-    def _getKitFromRoot(self, root):
-        # Flowcell ID
-        flowcell_id = root.find("FlowCellSerial")  # NextSeq style
-        if flowcell_id is not None:
-            flowcell_id = flowcell_id.text
-        else:
-            flowcell_markup = root.find("FlowcellRFIDTag")  # MiSeq style
-            if flowcell_markup is not None:
-                flowcell_id = flowcell_markup.find("SerialNumber").text
-            else:
-                flowcell_id = root.find("Barcode")  # HiSeq style
-                if flowcell_id is not None:
-                    flowcell_id = flowcell_id.text
-                else:
-                    flowcell_id = self.run["id"].rsplit("_", 1)[1]
-        # Reagent kit ID
-        reagent_kit_id = root.find("ReagentKitBarcode")
-        if reagent_kit_id is None:
-            reagent_kit_id = root.find("ReagentKitSerial")
-        if reagent_kit_id is not None:
-            reagent_kit_id = reagent_kit_id.text
-        return {
-            "flowcell_id": flowcell_id,
-            "reagent_kit_id": reagent_kit_id
-        }
-
-    def _getSoftwareFromRoot(self, root):
-        cs_root_markup = root.find("Setup")
-        if cs_root_markup is None:
-            cs_root_markup = root
-        return {
-            "RTA": root.find("RTAVersion").text,
-            "CS": cs_root_markup.find("ApplicationVersion").text
-        }
+        """Read file content and store information on the instance's attributes."""
+        super()._parse()
+        # Add samples data from software data to self.samples like in V1 format
+        spl_by_id = dict()
+        for spl in self.samples:
+            if spl.id not in spl_by_id:
+                spl_by_id[spl.id] = list()
+            spl_by_id[spl.id].append(spl)
+        for title, curr_extra in self.extra.items():
+            if "data" in curr_extra and isinstance(curr_extra["data"], list):
+                if len(curr_extra["data"]) != 0:
+                    lower_keys = [key.lower() for key in curr_extra["data"][0].keys()]
+                    if "sample_id" in lower_keys:  # Section contains data by sample
+                        for spl_metadata in curr_extra["data"]:
+                            spl_id = [val for key, val in spl_metadata.items() if key.lower() == "sample_id"][0]
+                            for key, val in spl_metadata.items():
+                                lower_key = key.lower()
+                                if lower_key != "sample_id":
+                                    if lower_key in {"sample_description", "description"}:
+                                        for curr_spl in spl_by_id[spl_id]:
+                                            curr_spl.description = val
+                                    else:
+                                        for curr_spl in spl_by_id[spl_id]:
+                                            curr_spl.metadata[key] = val
 
+    @staticmethod
+    def isValid(filepath):
+        """
+        Return true if the file is in SamplSheet V2 format.
 
-class CompletedJobInfo(object):
-    """Reader for CompletedJobInfo.xml."""
+        :param filepath: The file path.
+        :type filepath: str
+        :return: True if the file is in SamplSheet V2 format.
+        :rtype: bool
+        """
+        is_valid = False
+        try:
+            format_declaration = None
+            sections = set()
+            with open(filepath) as reader:
+                for line in reader:
+                    striped_line = line.strip()
+                    if re.fullmatch(r"\[[^]]+\],*", striped_line):
+                        title = AbstractSampleSheet.cleanedEnd(striped_line)[1:-1]
+                        sections.add(title)
+                    elif striped_line.startswith("FileFormatVersion,2"):
+                        format_declaration = striped_line
+            if format_declaration is None:
+                raise Exception('Invalid format declaration.')
+            if len(SampleSheetV2.REQUIRED_SECTIONS - sections) != 0:
+                raise Exception('Missing core sections: {}.'.format(SampleSheetV2.REQUIRED_SECTIONS - sections))
+            for extra_section in sections - SampleSheetV2.REQUIRED_SECTIONS:
+                if not extra_section.endswith("_Data") and not extra_section.endswith("_Settings"):
+                    raise Exception('Section "{}" is invalid.'.fomat(extra_section))
+            is_valid = True
+        except FileNotFoundError:
+            raise
+        except Exception:
+            pass
+        return is_valid
 
-    def __init__(self, path, date_format='%Y-%m-%dT%H:%M:%S'):
-        self.filepath = path
-        self.date_format = date_format
-        self.start_datetime = None
-        self.end_datetime = None
-        self.version = None
-        self.workflow_name = None
-        self.parameters = None
-        self._parse()
 
-    def _parse(self):
-        # Retrieve information by section
-        tree = ET.parse(self.filepath)
-        root = tree.getroot()
-        # Process information
-        self.end_datetime = root.find("CompletionTime").text  # 2017-11-23T17:19:55.0941558+01:00
-        self.end_datetime = self.end_datetime.split(".")[0]
-        self.end_datetime = datetime.datetime.strptime(self.end_datetime, self.date_format)
-        self.start_datetime = root.find("StartTime").text  # 2017-11-23T17:19:55.0941558+01:00
-        self.start_datetime = self.start_datetime.split(".")[0]
-        self.start_datetime = datetime.datetime.strptime(self.start_datetime, self.date_format)
-        self.version = root.find("Workflow").find("WorkflowVersion").text
-        self.workflow_name = root.find("Workflow").find("Analysis").text
-        workflow_param = etreeToDict(root.find("Workflow").find("WorkflowSettings"))
-        self.parameters = {"WorkflowSettings": workflow_param}
-        if self.workflow_name == "Amplicon - DS":
-            self.parameters["AmpliconSettings"] = etreeToDict(root.find("Workflow").find("AmpliconSettings"))
-
-
-def etreeToDict(node):
-    data = {"key": node.tag}
-    # Attributes
-    if len(node.attrib):
-        data["attributes"] = node.attrib
-    # Children
-    children = list()
-    for child in node:
-        children.append(etreeToDict(child))
-    if len(children):
-        data["children"] = children
-    else:
-        data["val"] = node.text
-    # Return
-    return data
-
-
-def getIlluminaName(name):
-    """
-    Return sample name used by Illumina in filename.
-
-    :param name: The name provided to Illumina process (for example in samplesheet).
-    :type name: str
-    :return: The sample name used by Illumina as part of filename.
-    :rtype: str
-    """
-    return name.replace("_", "-").replace(" ", "-").replace(".", "-").replace("+", "")
-
-
-def getLibNameFromReadsPath(seq_path):
-    """
-    Return library name from the path of the sequences file.
-
-    :param seq_path: The path of the sequences file.
-    :type seq_path: str
-    :return: The library name.
-    :rtype: str
-    """
-    library_name, extensions = os.path.basename(seq_path).split(".", 1)
-    for curr_ext in extensions.split("."):
-        if curr_ext not in ["fq", "fastq", "fasta", "fa", "gz", "bz", "bz2", "lz", "zip"]:
-            raise Exception('The file "{}" cannot be processed by getLibNameFromReadsPath because the extension "{}" is not managed.'.format(seq_path, curr_ext))
-    if re.search('_[rR][1-2]$', library_name):
-        library_name = library_name[:-3]
-    elif re.search('_[rR][1-2]_\d\d\d$', library_name):
-        library_name = library_name[:-7]
-    return library_name
-
-
-def getInfFromSeqID(seq_id):
-    """
-    Return sequencer id, run id, flowcell id and position of the sequence on the sequencer flowcell.
-
-    :param sequence: The ID of the sequence provided by the sequencer.
-    :type sequence: str
-    :return: The sequencer id, run id, flowcell id and position of the sequence on the sequencer flowcell.
-    :rtype: dict
-    """
-    fields = seq_id.split(":")
-    if len(fields) == 7:  # Illumina's ID: EAS139:136:FC706VJ:2:2104:15343:197393
-        fields.append(None)
-    # else  Illumina's ID: EAS139:136:FC706VJ:2:2104:15343:197393:ATGCATA+CTAGC
-    return {
-        "sequencer_id": fields[0],
-        "run_id": fields[1],
-        "flowcell_id": fields[2],
-        "lane_id": int(fields[3]),
-        "tile_id": int(fields[4]),
-        "x_pos": int(fields[5]),
-        "y_pos": int(fields[6]),
-        "umi": fields[7]
-    }
-
-
-def getInfFromSeqDesc(seq_desc):
-    """
-    Return sequencer id, run id, flowcell id and position of the sequence on the sequencer flowcell.
-
-    :param sequence: The ID of the sequence provided by the sequencer.
-    :type sequence: str
-    :return: The sequencer id, run id, flowcell id and position of the sequence on the sequencer flowcell.
-    :rtype: dict
-    """
-    # Illumina's description: 1:Y:18:ATCACG
-    reads_phases, kept_status, control_bits, barcode = seq_desc.split(":")
-    return {
-        "reads_phases": int(reads_phases),
-        "is_kept": kept_status == "N",
-        "control_bits": None if control_bits == "0" else int(control_bits),
-        "barcode": None if barcode == "" else barcode
-    }
-
-
-def platformFromInstrumentSerialNumber(instrument_id):
-    """
-    Return platform name from instrument ID.
-
-    :param instrument_id: The instrument serial number.
-    :type instrument_id: str
-    :return: The platform name (Hiseq or NextSeq or ...).
-    :rtype: str
-    """
-    platform_by_re = {
-        # "?": "iSeq",
-        "^MN[0-9]{5}$": "MiniSeq",
-        "^ML-..-[0-9]{2}$": "MiniSeq",
-        "^M[0-9]{5}$": "MiSeq",
-        "^N[SB][0-9]{6}$": "NextSeq",
-        "^NDX[0-9]{6}": "NextSeq",
-        "^[CDJKE][0-9]{5}$": "HiSeq",
-        "^A[0-9]{5}$": "NovaSeq"
-    }
-    if instrument_id.startswith("HWI"):
-        instrument_id = instrument_id[3:]
-    platform = None
-    for curr_re, curr_instru in platform_by_re.items():
-        if platform is None:
-            if re.search(curr_re, instrument_id):
-                platform = curr_instru
-    return platform
-
-
-def getRunFolderInfo(run_folder):
-    """
-    Return run information (instrument, run configuration, samples, ...) coming from several file in run folder.
-
-    :param run_folder: Path to the run folder.
-    :type run_folder: str
-    :return: Run information.
-    :rtype: dict
-    """
-    # RunInfo
-    run_info_path = os.path.join(run_folder, "RunInfo.xml")
-    run_info = RunInfo(run_info_path)
-    run = {
-        "reads_phases": run_info.reads_phases,
-        "flowcell": run_info.flowcell,
-        "instrument": run_info.instrument,
-        "info": run_info.run,
-        "samples": None
-    }
-    run["info"]["end_date"] = None
-    # RTAComplete
-    rta_complete_path = os.path.join(run_folder, "RTAComplete.txt")
-    if os.path.exists(rta_complete_path):
-        rta_complete = RTAComplete(rta_complete_path)
-        run["info"]["end_date"] = rta_complete.end_date
-    # SampleSheet
-    samplesheet_path = os.path.join(run_folder, "SampleSheet.csv")
-    if os.path.exists(samplesheet_path):
-        run["samples"] = SampleSheetIO(samplesheet_path).samples
-    return run
+class SampleSheetADS(SampleSheetV1):
+    """Reader for SampleSheet.csv designed for AmpliconDS analysis."""
+
+    def _getSamplesFromData(self, data_section):
+        """
+        Return samples list containing for each: keys and values from data section as dict.
+
+        :param section: Lines from section with a titles row. Each row contains one entry where columns correspond to key and cells to values.
+        :type section: list
+        :return: Samples list as anacore.illumina.samplesheet.SampleADS.
+        :rtype: list
+        """
+        samples = super()._getSamplesFromData(data_section)
+        return [
+            SampleADS(spl.sheet_index, spl.id, spl.barcodes, spl.description, spl.metadata)
+            for spl in samples
+        ]
+
+    @staticmethod
+    def isValid(filepath):
+        """
+        Return true if the file is in SamplSheet Amplicon Double Strand format.
+
+        :param filepath: The file path.
+        :type filepath: str
+        :return: True if the file is in SamplSheet Amplicon Double Strand format.
+        :rtype: bool
+        """
+        is_valid = False
+        if SampleSheetV1.isValid(filepath):
+            try:
+                samplesheet = SampleSheetV1(filepath)
+                if "Application" in samplesheet.header and \
+                   samplesheet.header["Application"] == "Amplicon - DS" and \
+                   len(samplesheet.manifests) != 0:
+                    if len(samplesheet.samples) == 0:
+                        is_valid = True
+                    elif "Manifest" in samplesheet.samples[0].metadata:
+                        is_valid = True
+            except FileNotFoundError:
+                raise
+            except Exception:
+                pass
+        return is_valid
+
+    def filterPanels(self, selected_manifests):
+        """
+        Filter samples and manifests on their panel.
+
+        :param selected_manifests: The manifests corresponding to the selected panel.
+        :type selected_manifests: list
+        """
+        # Get kept
+        new_manifests = {}
+        new_by_old_id = {}
+        new_idx = 0
+        for manifest_id in sorted(self.manifests):
+            manifest_file = self.manifests[manifest_id]
+            if manifest_file in selected_manifests:
+                new_manifest_id = chr(ord("A") + new_idx)
+                new_by_old_id[manifest_id] = new_manifest_id
+                new_manifests[new_manifest_id] = self.manifests[manifest_id]
+                new_idx += 1
+        # Update manifests
+        self.manifests = new_manifests
+        # Update samples
+        new_spl = list()
+        for spl in self.samples:
+            if spl.metadata["Manifest"] in new_by_old_id:
+                if spl.id.endswith("_" + spl.metadata["Manifest"]):
+                    spl.id = spl.id.rsplit("_" + spl.metadata["Manifest"], 1)[0]
+                    spl.id += "_" + new_by_old_id[spl.metadata["Manifest"]]
+                spl.metadata["Manifest"] = new_by_old_id[spl.metadata["Manifest"]]
+                new_spl.append(spl)
+        self.samples = new_spl
```

### Comparing `anacore-2.9.0/anacore/maf.py` & `anacore-3.0.0/anacore/maf.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/anacore/matrix.py` & `anacore-3.0.0/anacore/matrix.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/anacore/msiannot.py` & `anacore-3.0.0/anacore/msi/annot.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 # -*- coding: utf-8 -*-
 """Classes and functions for reading/writing MSI annotations files."""
 
 __author__ = 'Frederic Escudie'
-__copyright__ = 'Copyright (C) 2018 IUCT-O'
+__copyright__ = 'Copyright (C) 2018 CHU Toulouse'
 __license__ = 'GNU General Public License'
 __version__ = '1.0.1'
 __email__ = 'escudie.frederic@iuct-oncopole.fr'
 __status__ = 'prod'
 
 import json
 from anacore.sv import HashedSVIO
-from anacore.msi import Status, LocusRes, MSILocus
+from anacore.msi.base import Status
+from anacore.msi.locus import Locus, LocusRes
 
 
 class MSIAnnot(HashedSVIO):
     def __init__(self, filepath, mode="r"):
         """
         Build and return an instance of HashedSVIO.
 
@@ -101,31 +102,31 @@
                 data_by_res[record["method_id"]] = dict()
             data_by_key = data_by_res[record["method_id"]]
             # Add data
             data_by_key[record["key"]] = record["value"]
     return data_by_spl
 
 
-def addLociResToSpl(msi_spl, data_by_locus, res_cls=LocusRes):
+def addLociResToSpl(msi_spl, data_by_locus):
     for locus_id, data_by_res in data_by_locus.items():
         # Add locus
         if locus_id not in msi_spl.loci:
             msi_spl.addLocus(
-                MSILocus(locus_id)
+                Locus(locus_id)
             )
         msi_locus = msi_spl.loci[locus_id]
         # Add result and data
-        addLociResult(msi_locus, data_by_res, res_cls)
+        addLociResult(msi_locus, data_by_res)
 
 
-def addLociResult(msi_locus, data_by_res, res_cls):
+def addLociResult(msi_locus, data_by_res):
     for result_id, data_by_key in data_by_res.items():
         # Add result
         if result_id not in msi_locus.results:
-            msi_locus.results[result_id] = res_cls(Status.none)
+            msi_locus.results[result_id] = LocusRes(Status.none)
         locus_res = msi_locus.results[result_id]
         # Add data
         for key, value in data_by_key.items():
             if key != "result_id":
                 if key in locus_res.__dict__ and key != "data":  # The key correspond to an attibute
                     setattr(locus_res, key, value)
                 else:  # The key correspond to a data
```

### Comparing `anacore-2.9.0/anacore/msings.py` & `anacore-3.0.0/anacore/msi/msings.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # -*- coding: utf-8 -*-
-"""Classes and functions for reading/writing mSINGS's outputs."""
+"""Classes and functions to predict with mSINGS's algorithm and to read/write mSINGS binaries outputs."""
 
 __author__ = 'Frederic Escudie'
 __copyright__ = 'Copyright (C) 2018 IUCT-O'
 __license__ = 'GNU General Public License'
-__version__ = '1.3.0'
+__version__ = '1.5.0'
 __email__ = 'escudie.frederic@iuct-oncopole.fr'
 __status__ = 'prod'
 
 import gzip
 from anacore.abstractFile import isGzip
+from anacore.msi.base import Status
+from anacore.msi.locus import Locus, LocusRes
+from anacore.msi.sample import MSISample, MSISplRes
 from anacore.sv import HashedSVIO
-from anacore.msi import MSILocus, LocusRes, MSISample, MSISplRes, Status
+from numpy import average, std
 
 
-class MSINGSAnalysis(HashedSVIO):
+class MSINGSAnalysisIO(HashedSVIO):
     """Manage output file produced by the command "msi analyzer" of mSINGS (https://bitbucket.org/uwlabmed/msings)."""
 
     def __init__(self, filepath, mode="r"):
         """
         Return the new instance of MSINGSAnalysis.
 
         :param filepath: The filepath.
@@ -31,100 +34,144 @@
             self.titles = ["Position", "Name", "Average_Depth", "Number_of_Peaks", "Standard_Deviation", "IndelLength:AlleleFraction:SupportingCalls"]
 
     def _parseLine(self):
         """
         Return a structured record from the current line.
 
         :return: The record described by the current line.
-        :rtype: MSILocus
+        :rtype: anacore.msi.base.Locus
         """
         record = super()._parseLine()
+        locus_len = int(record["Position"].rsplit("-", 1)[1]) - int(record["Position"].rsplit(":", 1)[1].rsplit("-", 1)[0])
         peaks = record["IndelLength:AlleleFraction:SupportingCalls"].split(" ")
         nb_by_length = {}
-        if len(peaks) == 1 and peaks[0] == "0:0.0:0":
-            peaks = []
-        else:
-            for idx, curr_peak in enumerate(peaks):
-                indel_length, AF, DP = curr_peak.split(":")
-                peaks[idx] = {
-                    "indel_length": int(indel_length),
-                    "AF": float(AF),
-                    "DP": int(DP)
-                }
-                nb_by_length[int(indel_length)] = int(DP)
-
-        return MSILocus.fromDict({
+        for idx, curr_peak in enumerate(peaks):
+            indel_length, AF, DP = curr_peak.split(":")
+            if DP != "0":
+                nb_by_length[int(indel_length) + locus_len] = int(DP)
+        return Locus.fromDict({
             "position": record["Position"],
             "name": record["Name"],
             "results": {
-                "MSINGS": {
-                    "_class": "LocusResDistrib",
+                "mSINGS": {
                     "status": Status.undetermined,
                     "data": {
-                        "avg_depth": record["Average_Depth"],
-                        "nb_peaks": record["Number_of_Peaks"],
-                        "peaks": peaks,
-                        "std_dev": record["Standard_Deviation"],
-                        "nb_by_length": nb_by_length
+                        "avg_depth": int(record["Average_Depth"]),
+                        "nb_peaks": int(record["Number_of_Peaks"]),
+                        "std_dev": float(record["Standard_Deviation"]),
+                        "lengths": {"ct_by_len": nb_by_length}
                     }
                 }
             }
         })
 
     def recordToLine(self, record):
         """
         Return the record in SV format.
 
         :param record: The record containing a result coming from mSINGS.
-        :type record: MSILocus
+        :type record: anacore.msi.base.Locus
         :return: The SV line corresponding to the record.
         :rtype: str
         """
         formatted_record = {
             "Position": record.position,
             "Name": record.name,
-            "Average_Depth": record.results["MSINGS"].data["avg_depth"],
-            "Number_of_Peaks": record.results["MSINGS"].data["nb_peaks"],
-            "Standard_Deviation": record.results["MSINGS"].data["std_dev"]
+            "Average_Depth": record.results["mSINGS"].data["avg_depth"],
+            "Number_of_Peaks": record.results["mSINGS"].data["nb_peaks"],
+            "Standard_Deviation": record.results["mSINGS"].data["std_dev"]
         }
-        formatted_record["IndelLength:AlleleFraction:SupportingCalls"] = " ".join(
-            ["{}:{}:{}".format(curr_peak["indel_length"], curr_peak["AF"], curr_peak["DP"]) for curr_peak in record.results["MSINGS"].data["peaks"]]
-        )
+        ct_by_len = record.results["mSINGS"].data["lengths"]
+        max_ct = ct_by_len.getMostRepresented()["count"]
+        if max_ct == 0:
+            formatted_record["IndelLength:AlleleFraction:SupportingCalls"] = "0:0.0000000:0"
+        else:
+            locus_ref_len = record.length
+            locus_min_len = ct_by_len.getMinLength()
+            formatted_record["IndelLength:AlleleFraction:SupportingCalls"] = " ".join(
+                [
+                    "{}:{:.7f}:{}".format((locus_min_len + idx) - locus_ref_len, ct / max_ct, ct)
+                    for idx, ct in enumerate(ct_by_len.getDenseCount())
+                ]
+            )
         return super().recordToLine(formatted_record)
 
 
+class MSINGSEval:
+    """Provides utils to predict with mSINGS: calculate feature and determine feature threshold."""
+
+    @staticmethod
+    def getNbPeaks(locus_distrib, highest_peak_ratio=0.05):
+        """
+        Return feature used to predict stability status by mSINGS: the number of peaks with height >= peak_height_cutoff * highest_peak_height.
+
+        :param locus_distrib: Lengths distribution of microsatellite.
+        :type locus_distrib: anacore.msi.locus.LocusDataDistrib
+        :param highest_peak_ratio: Minimum rate of highest peak height to consider a peak.
+        :type highest_peak_ratio: float
+        :return: Feature used to predict stability status by mSINGS: the number of peaks with height >= peak_height_cutoff * highest_peak_height.
+        :rtype: int
+        """
+        highest_peak = locus_distrib.getMostRepresented()
+        min_peak_height = highest_peak_ratio * highest_peak["count"]
+        return locus_distrib.getNbPeaks(min_peak_height)
+
+    @staticmethod
+    def getThresholdFromNbPeaks(models_nb_peaks, std_dev_rate=2.0):
+        """
+        Return minimum number of peaks to tag distribution as unstable.
+
+        :param models_nb_peaks: Number of peaks in stable population (see MSINGSEval.getNbPeaks).
+        :type models_nb_peaks: list
+        :param std_dev_rate: Number of standard deviation authorized around average number of peaks in stable population.
+        :type std_dev_rate: float
+        :return: Minimum number of peaks to tag distribution as unstable.
+        :rtype: float
+        """
+        return average(models_nb_peaks) + std(models_nb_peaks) * std_dev_rate
+
+
 class MSINGSReport(object):
     """Manage output file produced by the command "msi count_msi_samples" of mSINGS (https://bitbucket.org/uwlabmed/msings)."""
 
     def __init__(self, filepath):
         """
         Return the new instance of MSINGSReport.
 
         :param filepath: The filepath.
         :type filepath: str
         """
         self.filepath = filepath
         self.samples = dict()
         self.loci = list()
-        self.method_name = "MSINGS"
-        self.parse()
+        self.method_name = "mSINGS"
+        self._parse()
+
+    def _parse(self):
+        """Parse file and store information in self."""
+        if isGzip(self.filepath):
+            with gzip.open(self.filepath, "rt") as FH:
+                self._parseFileHandle(FH)
+        else:
+            with open(self.filepath, "r") as FH:
+                self._parseFileHandle(FH)
 
     def _parseFileHandle(self, FH):
         """
         Parse file referenced by the file handle FH and store information in self.
 
         :param FH: The file handle for the filepath.
         :type FH: TextIOWrapper
         """
         # Parse general information
         samples = [elt.strip() for elt in FH.readline().split("\t")[1:]]
         nb_unstable = [int(elt.strip()) for elt in FH.readline().split("\t")[1:]]
         nb_evaluated = [int(elt.strip()) for elt in FH.readline().split("\t")[1:]]
         line = FH.readline()
-        if not line.startswith("msing_score"):
+        if not line.startswith("msings_score"):
             scores = [None for curr_spl in samples]
         else:
             scores = [elt.strip() for elt in line.split("\t")][1:]
             for idx, elt in enumerate(scores):
                 curr_score = None
                 if elt != "":
                     curr_score = float(elt)
@@ -157,23 +204,16 @@
             curr_locus = fields[0]
             self.loci.append(curr_locus)
             for idx, curr_val in enumerate(fields[1:]):
                 curr_spl = samples[idx]
                 loci_res = None
                 if curr_val == "":
                     loci_res = LocusRes(Status.undetermined)
-                elif curr_val == "1":
+                elif curr_val == "1" or curr_val == "Unstable":
                     loci_res = LocusRes(Status.unstable)
-                else:
+                elif curr_val == "0" or curr_val == "Stable":
                     loci_res = LocusRes(Status.stable)
+                else:
+                    raise Exception("{} cannot be parsed by {}.".format(self.filepath, self.__class__.__name__,))
                 self.samples[curr_spl].addLocus(
-                    MSILocus(curr_locus, None, {self.method_name: loci_res})
+                    Locus(curr_locus, None, {self.method_name: loci_res})
                 )
-
-    def parse(self):
-        """Parse file and store information in self."""
-        if isGzip(self.filepath):
-            with gzip.open(self.filepath, "rt") as FH:
-                self._parseFileHandle(FH)
-        else:
-            with open(self.filepath, "r") as FH:
-                self._parseFileHandle(FH)
```

### Comparing `anacore-2.9.0/anacore/node.py` & `anacore-3.0.0/anacore/node.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/anacore/picardIO.py` & `anacore-3.0.0/anacore/picardIO.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/anacore/region.py` & `anacore-3.0.0/anacore/region.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/anacore/sequence.py` & `anacore-3.0.0/anacore/sequence.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Classes and functions for manipulating/processing sequences."""
 
 __author__ = 'Frederic Escudie'
 __copyright__ = 'Copyright (C) 2021 IUCT-O'
 __license__ = 'GNU General Public License'
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 __email__ = 'escudie.frederic@iuct-oncopole.fr'
 __status__ = 'prod'
 
 from textwrap import wrap
 
 
 class Alphabet:
@@ -185,14 +185,35 @@
         :type seq: str
         :return: The reverse complement.
         :rtype: str
         """
         return "".join([__class__.complement[base] for base in seq[::-1]])
 
 
+def getShortestRepeatUnit(seq):
+    """
+    Return the shortest repeat unit that can be used to reproduce the entire sequence or None if it does not exist.
+
+    :param str: Complete sequence.
+    :type seq: str
+    :return: The shortest repeat unit that can be used to reproduce the entire sequence or None if it does not exist.
+    :rtype: str
+    """
+    uc_seq = seq.upper()
+    seq_len = len(seq)
+    repeat_unit = None
+    for unit_size in range(1, int(seq_len / 2) + 1):
+        if repeat_unit is None and seq_len % unit_size == 0:
+            eval_unit = seq[:unit_size]
+            chunks = {chunk for chunk in wrap(uc_seq, unit_size)}
+            if len(chunks - {eval_unit}) == 0:
+                repeat_unit = eval_unit
+    return repeat_unit
+
+
 class RNAAlphabet(Alphabet):
     """Static methods and attributes to manage RNA alphabet."""
     complement = {
         'A': 'U', 'T': 'A', 'G': 'C', 'C': 'G', 'U': 'A', 'N': 'N',
         'a': 'u', 't': 'a', 'g': 'c', 'c': 'g', 'u': 'a', 'n': 'n',
         'W': 'W', 'S': 'S', 'M': 'K', 'K': 'M', 'R': 'Y', 'Y': 'R', 'B': 'V', 'V': 'B', 'D': 'H', 'H': 'D',
         'w': 'w', 's': 's', 'm': 'k', 'k': 'm', 'r': 'y', 'y': 'r', 'b': 'v', 'v': 'b', 'd': 'h', 'h': 'd'
```

### Comparing `anacore-2.9.0/anacore/sequenceIO.py` & `anacore-3.0.0/anacore/sequenceIO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # -*- coding: utf-8 -*-
 """Classes and functions for reading/writing sequence files and their indices."""
 
 __author__ = 'Frederic Escudie - Plateforme bioinformatique Toulouse'
 __copyright__ = 'Copyright (C) 2015 INRA'
 __license__ = 'GNU General Public License'
-__version__ = '2.5.0'
+__version__ = '2.6.0'
 __email__ = 'escudie.frederic@iuct-oncopole.fr'
 __status__ = 'prod'
 
 from anacore.abstractFile import isGzip
 from anacore.sequence import Sequence, DNAAlphabet
 from anacore.sv import SVIO
 import gzip
@@ -564,31 +564,34 @@
 
     def _setIndex(self):
         """Set self.index with content of self.fai_path."""
         self.index = Faidx(self.fai_path).readById()
 
     def getSub(self, id, start, end=None):
         """
-        Return the selected sub of the sequence from file.
+        Return the selected sub of the sequence from file. Return empty sequence if start position is out. Return fitted sequence if end is out.
 
         :param id: The sequence ID.
         :type id: str
         :param start: The start position of the selected sub-sequence (1-based).
         :type start: int
         :param end: The end position of the selected sub-sequence (1-based). Default: The end of the sequence.
         :type end: int
         :return: The sequence selected.
         :rtype: str
         """
+        if start > self.index[id].length + 1:
+            return ""
         endline_marker_len = self.index[id].line_width - self.index[id].line_bases
         # Start position
         start_line_idx = int((start - 1) / self.index[id].line_bases)
         read_start = self.index[id].offset + start - 1 + start_line_idx * endline_marker_len
         # End position
-        end = self.index[id].length if end is None else end
+        if end is None or end > self.index[id].length + 1:
+             end = self.index[id].length
         end_line_idx = int((end - 1) / self.index[id].line_bases)
         read_end = self.index[id].offset + end - 1 + end_line_idx * endline_marker_len
         # Get sequence
         self.file_handle.seek(read_start)
         seq = self.file_handle.read(read_end - read_start + 1).replace("\n", "").replace("\r", "")
         return seq
```

### Comparing `anacore-2.9.0/anacore/sv.py` & `anacore-3.0.0/anacore/sv.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/anacore/tophatFusion.py` & `anacore-3.0.0/anacore/tophatFusion.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/anacore/vcf.py` & `anacore-3.0.0/anacore/vcf.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,89 @@
 # -*- coding: utf-8 -*-
-"""Classes and functions for reading/writing/processing VCF."""
+"""
+Classes and functions for reading/writing/processing VCF.
+
+:Example:
+
+    Read VCF by line
+
+    .. highlight:: python
+    .. code-block:: python
+
+        from anacore.vcf import VCFIO
+
+        with VCFIO("test.vcf.gz") as reader:
+            print("Variant", "\\t".join(reader.samples), sep="\\t")
+            for record in reader:
+                alt_freq = [str(record.getAF(curr_spl)) for curr_spl in reader.samples]
+                print(record.getName(), "\\t".join(alt_freq), sep="\\t")
+
+        # Result>
+        # Variant\tN01\tN02\tN03
+        # chr1:35-35=A/T\t0.3\t0.4\t0.1
+        # chr1:128-128=G/A\t0.1\t0.6\t0.05
+
+    Read VCF by coordinate
+
+    .. highlight:: python
+    .. code-block:: python
+
+        from anacore.vcf import VCFIO
+
+        with VCFIO("test.vcf.gz", "i") as reader:
+            for record in reader.getSub("chr1", 10, 100):
+                print(record.getName())
+
+        # Result>
+        # chr1:35-35=A/T
+
+    Write VCF
+
+    .. highlight:: python
+    .. code-block:: python
+
+        from anacore.vcf import VCFIO
+
+        with VCFIO("test.vcf.gz", "w") as writer:
+            # Header
+            writer.samples = ["my_sample"]
+            writer.filter = [
+                {"q10": HeaderFilterAttr("q10", "Quality below 10")}
+            ]
+            self.info = {
+                "DB": HeaderInfoAttr("DB", "dbSNP membership, build 129", "Flag", 0)
+            }
+            self.format = {
+                "AF": HeaderFormatAttr("AF", "Allele Frequency", "Float", "A")
+            }
+            writer.extra_header = [
+                "##source=myImputationProgramV3.1",
+                "##phasing=partial"
+            ]
+            writer.writeHeader()
+            # Record
+            for record in vcf_record_list:
+                writer.write(record)
+
+        # Result>
+        # ##fileformat=VCFv4.3
+        # ##source=myImputationProgramV3.1
+        # ##phasing=partial
+        # ##INFO=<ID=DB,Number=0,Type=Flag,Description="dbSNP membership, build 129">
+        # ##FILTER=<ID=q10,Description="Quality below 10">
+        # ##FORMAT=<ID=AF,Number=A,Type=Float,Description="Allele Frequency">
+        # #CHROM\tPOS\tID\tREF\tALT\tQUAL\tFILTER\tINFO\tFORMAT\tmy_sample
+        # chr1\t35\t.\tA\tT.\tPASS\tDB\tAF\t0.1
+        # ...
+"""
 
 __author__ = 'Frederic Escudie'
-__copyright__ = 'Copyright (C) 2017 IUCT-O'
+__copyright__ = 'Copyright (C) 2017 CHU Toulouse'
 __license__ = 'GNU General Public License'
-__version__ = '1.31.0'
+__version__ = '1.34.0'
 __email__ = 'escudie.frederic@iuct-oncopole.fr'
 __status__ = 'prod'
 
 from anacore.abstractFile import AbstractFile
 from copy import deepcopy
 from pysam import TabixFile
 import sys
@@ -778,33 +853,35 @@
         Return the reference allele depth for the population (it is composed by all samples).
 
         :return: The reference allele population depth.
         :rtype: int
         """
         ref_pop_AD = None
         if "AD" in self.info and len(self.info["AD"]) == len(self.alt) + 1:  # INFO.AD contains ref allele
-            ref_pop_AD = self.info["AD"]
+            ref_pop_AD = self.info["AD"][0]
         elif "AF" in self.info and "DP" in self.info and len(self.info["AF"]) == len(self.alt) + 1:  # INFO.AF contains ref allele and INFO.DP exists
             ref_pop_AD = int(self.info["AF"][0] * self.info["DP"])
         elif len(self.samples) != 0:  # Must be processed by samples data
-            first_spl = self.samples.keys()[0]
-            if "AD" in self.format and len(first_spl["AD"]) == len(self.alt) + 1:  # AD contains ref allele
-                try:
-                    ref_pop_AD = 0
-                    for spl_name, spl_data in self.samples.items():  # Sum ref AD for all samples
-                        ref_pop_AD += spl_data["AD"][0]
-                except Exception:
-                    ref_pop_AD = None
-            if ref_pop_AD is None and "AF" in self.format and "DP" in self.format and len(first_spl["AF"]) == len(self.alt) + 1:  # AF contains ref allele
-                try:
-                    ref_pop_AD = 0
-                    for spl_name, spl_data in self.samples.items():  # Sum ref AD for all samples
-                        ref_pop_AD += spl_data["AF"][0] * spl_data["DP"]
-                except Exception:
-                    ref_pop_AD = None
+            if self.format:  # Counts are present by samples
+                first_spl = list(self.samples.values())[0]
+                if "AD" in self.format and len(first_spl["AD"]) == len(self.alt) + 1:  # AD contains ref allele
+                    try:
+                        ref_pop_AD = 0
+                        for spl_name, spl_data in self.samples.items():  # Sum ref AD for all samples
+                            ref_pop_AD += spl_data["AD"][0]
+                    except Exception:
+                        ref_pop_AD = None
+                if ref_pop_AD is None and "AF" in self.format and "DP" in self.format and len(first_spl["AF"]) == len(self.alt) + 1:  # AF contains ref allele
+                    try:
+                        ref_pop_AD = 0
+                        for spl_name, spl_data in self.samples.items():  # Sum ref AD for all samples
+                            ref_pop_AD += spl_data["AF"][0] * spl_data["DP"]
+                        ref_pop_AD = int(ref_pop_AD)
+                    except Exception:
+                        ref_pop_AD = None
         if ref_pop_AD is None:  # Erroneous when several variants exist on position and are line splitted
             if "AD" in self.info:  # INFO.AD does not contain ref
                 ref_pop_AD = self.getPopDP() - sum(self.info["AD"])
             elif "AF" in self.info and "DP" in self.info:  # INFO.AF does not contain ref and INFO.DP exists
                 ref_pop_AD = int((1 - sum(self.info["AF"])) * self.info["DP"])
             else:  # Must be processed by samples data
                 alt_pop_AD = sum(self.getPopAltAD())
@@ -860,39 +937,40 @@
         Return the reference allele frequency for the population (it is composed by all samples).
 
         :return: The reference allele population frequency.
         :rtype: int
         """
         ref_pop_AF = None
         if "AF" in self.info and len(self.info["AF"]) == len(self.alt) + 1:  # INFO.AF contains ref allele
-            ref_pop_AF = self.info["AF"]
+            ref_pop_AF = self.info["AF"][0]
         elif "AD" in self.info and "DP" in self.info and len(self.info["AD"]) == len(self.alt) + 1:  # INFO.AD contains ref allele and INFO.DP exists
             ref_pop_AF = self.info["AD"][0] / self.info["DP"]
         elif len(self.samples) != 0:  # Must be processed by samples data
-            first_spl = self.samples.keys()[0]
-            if "AD" in self.format and "DP" in self.format and len(first_spl["AD"]) == len(self.alt) + 1:  # AD contains ref allele
-                try:
-                    ref_pop_AD = 0
-                    pop_DP = 0
-                    for spl_name, spl_data in self.samples.items():  # Sum ref AD for all samples
-                        pop_DP += spl_data["DP"]
-                        ref_pop_AD += spl_data["AD"][0]
-                    ref_pop_AF = ref_pop_AD / pop_DP
-                except Exception:
-                    ref_pop_AF = None
-            if ref_pop_AF is None and "AF" in self.format and "DP" in self.format and len(first_spl["AF"]) == len(self.alt) + 1:  # AF contains ref allele
-                try:
-                    ref_pop_AD = 0
-                    pop_DP = 0
-                    for spl_name, spl_data in self.samples.items():  # Sum ref AF for all samples
-                        pop_DP += spl_data["DP"]
-                        ref_pop_AD += spl_data["AF"][0] * spl_data["DP"]
-                    ref_pop_AF = ref_pop_AD / pop_DP
-                except Exception:
-                    ref_pop_AF = None
+            if self.format:  # Counts are present by samples
+                first_spl = list(self.samples.values())[0]
+                if "AD" in self.format and "DP" in self.format and len(first_spl["AD"]) == len(self.alt) + 1:  # AD contains ref allele
+                    try:
+                        ref_pop_AD = 0
+                        pop_DP = 0
+                        for spl_name, spl_data in self.samples.items():  # Sum ref AD for all samples
+                            pop_DP += spl_data["DP"]
+                            ref_pop_AD += spl_data["AD"][0]
+                        ref_pop_AF = ref_pop_AD / pop_DP
+                    except Exception:
+                        ref_pop_AF = None
+                if ref_pop_AF is None and "AF" in self.format and "DP" in self.format and len(first_spl["AF"]) == len(self.alt) + 1:  # AF contains ref allele
+                    try:
+                        ref_pop_AD = 0
+                        pop_DP = 0
+                        for spl_name, spl_data in self.samples.items():  # Sum ref AF for all samples
+                            pop_DP += spl_data["DP"]
+                            ref_pop_AD += spl_data["AF"][0] * spl_data["DP"]
+                        ref_pop_AF = ref_pop_AD / pop_DP
+                    except Exception:
+                        ref_pop_AF = None
         if ref_pop_AF is None:  # Erroneous when several variants exist on position and are line splitted
             if "AF" in self.info:  # INFO.AF does not contain ref
                 ref_pop_AF = 1 - sum(self.info["AF"])
             elif "AD" in self.info and "DP" in self.info:  # INFO.AD does not contain ref and INFO.DP exists
                 ref_pop_AF = (self.info["DP"] - sum(self.info["AD"])) / self.info["DP"]
             else:  # Must be processed by samples data
                 alt_pop_AF = sum(self.getPopAltAF())
@@ -1132,14 +1210,275 @@
             else:  # AD does not contain reference AD and AF is missing to calculate DP
                 raise Exception('The depth cannot be retrieved in variant "' + self.chrom + ":" + str(self.pos) + '".')
         else:  # AD is missing to calculate DP
             raise Exception('The depth cannot be retrieved in variant "' + self.chrom + ":" + str(self.pos) + '".')
         return DP
 
 
+class VCFSymbAltRecord(VCFRecord):
+    """Class to manage a variant record with symbolic alternative like <DUP>, <DEL>, etc."""
+
+    def __setattr__(self, name, value):
+        """
+        Assign value to the attribute.
+
+        :param name: The attribute name.
+        :type name: str
+        :param value: The value to be assigned to the attribute.
+        :type value: *
+        """
+        if name == "alt":
+            for alt in value:
+                if not alt.startswith("<"):
+                    raise Exception("Alternative allele {} is not a symbolic allele.".format(alt))
+                if alt.startswith("<BND"):
+                    raise Exception("BND are not managed by {}.".format(self.__class__.__name__))
+        super().__setattr__(name, value)
+
+    def containsIndel(self):
+        """
+        Return True if the variant contains an allele corresponding to an insertion or a deletion.
+
+        :return: True if the variant contains an allele corresponding to an insertion or a deletion.
+        :rtype: bool
+        """
+        raise NotImplementedError("Method 'containsIndel' is not implemented for {}.".format(self.__class__.__name__))
+
+    @property
+    def end(self):
+        """
+        Return end position of the variant (1-based).
+
+        :return: End position of the variant (1-based). This position correspond to the last reference nt implicated in variant. For example, in DUP, the position correspond to last duplicated nt on reference.
+        :rtype: int | None
+        :warnings: This method can only be used on record with only one alternative allele.
+        """
+        if len(self.alt) > 1:
+            raise Exception("The attribute 'end' cannot be used on multi-allelic variant {}.".format(VCFRecord.getName(self)))
+        end = None
+        if "END" in self.info:
+            end = self.info["END"]
+            if isinstance(end, (list, tuple)):
+                end = end[0]
+        elif self.alt[0].startswith("<INS"):  # INS
+            end = self.pos
+        elif "SVLEN" in self.info:  # CNV or DEL or DUP or INV
+            end = self.pos + abs(self.sv_len)
+        return end
+
+    def fastDownstreamed(self, seq_handler, padding=500):
+        raise NotImplementedError("Method 'fastDownstreamed' is not implemented for {}.".format(self.__class__.__name__))
+
+    def fastStandardize(self, seq_handler, padding=500):
+        raise NotImplementedError("Method 'fastStandardize' is not implemented for {}.".format(self.__class__.__name__))
+
+    @staticmethod
+    def fromStdRecord(record):
+        """
+        Build and return an instance of VCFSymbAltRecord from VCFRecord.
+
+        :param record: Initial VCFRecord.
+        :type record: VCFRecord
+        :return: The new instance.
+        :rtype: VCFSymbAltRecord
+        """
+        return VCFSymbAltRecord(
+            record.chrom,
+            record.pos,
+            record.id,
+            record.ref,
+            record.alt,
+            record.qual,
+            record.filter,
+            record.info,
+            record.format,
+            record.samples
+        )
+
+    def getMostUpstream(self, ref_seq):
+        raise NotImplementedError("Method 'getMostUpstream' is not implemented for {}.".format(self.__class__.__name__))
+
+    def getMostDownstream(self, ref_seq):
+        raise NotImplementedError("Method 'getMostDownstream' is not implemented for {}.".format(self.__class__.__name__))
+
+    def getName(self):
+        """
+        Return an unique name to identified the variant.
+
+        :return: The variant name.
+        :rtype: str
+        :warnings: This name can be not uniq for two insertions on same position and with same length.
+        """
+        return "{}:{}[{}]={}/{}".format(
+            self.chrom,
+            self.pos,
+            self.sv_len if self.sv_len else "",
+            self.ref,
+            "/".join(self.alt)
+        )
+
+    def isDeletion(self):
+        """
+        Return True if the variant is a deletion.
+
+        :return: True if the variant is a deletion.
+        :rtype: bool
+        :warnings: This method can only be used on record with only one alternative allele.
+        """
+        if len(self.alt) > 1:
+            raise Exception("The function 'isDeletion' cannot be used on multi-allelic variant {}.".format(VCFRecord.getName(self)))
+        is_deletion = False
+        if self.alt[0].startswith("<DEL"):
+            is_deletion = True
+        elif self.alt[0].startswith("<CNV"):
+            if "SVLEN" in self.info:
+                sv_len = self.info["SVLEN"]
+                if isinstance(sv_len, (list, tuple)):
+                    sv_len = sv_len[0]
+                if sv_len < 0:
+                    is_deletion = True
+            else:
+                raise Exception("CNV can be deletion or insertion on variant {}.".format(VCFRecord.getName(self)))
+        return is_deletion
+
+    def isIndel(self):
+        """
+        Return True if the variant is an insertion or a deletion.
+
+        :return: True if the variant is an insertion or a deletion.
+        :rtype: bool
+        :warnings: This method can only be used on record with only one alternative allele.
+        """
+        if len(self.alt) > 1:
+            raise Exception("The function 'isIndel' cannot be used on multi-allelic variant {}.".format(VCFRecord.getName(self)))
+        return self.isDeletion() or self.isInsertion() or self.alt[0].startswith("<CNV")  # CNV may be both deletion and duplication
+
+    def isInsAndDel(self):
+        """
+        Return True if the variant is an insertion and also a deletion.
+
+        :return: True if the variant is an insertion and also a deletion.
+        :rtype: bool
+        :warnings: This method can only be used on record with only one alternative allele.
+        """
+        if len(self.alt) > 1:
+            raise Exception("The function 'isInsAndDel' cannot be used on multi-allelic variant {}.".format(VCFRecord.getName(self)))
+        return False
+
+    def isInsertion(self):
+        """
+        Return True if the variant is an insertion.
+
+        :return: True if the variant is an insertion.
+        :rtype: bool
+        :warnings: This method can only be used on record with only one alternative allele.
+        """
+        if len(self.alt) > 1:
+            raise Exception("The function 'isInsertion' cannot be used on multi-allelic variant {}.".format(VCFRecord.getName(self)))
+        is_insertion = False
+        if self.alt[0].startswith("<DUP") or self.alt[0].startswith("<INS"):
+            is_insertion = True
+        elif self.alt[0].startswith("<CNV"):
+            if "SVLEN" in self.info:
+                sv_len = self.info["SVLEN"]
+                if isinstance(sv_len, (list, tuple)):
+                    sv_len = sv_len[0]
+                if sv_len >= 0:
+                    is_insertion = True
+                # else: is_insertion = False
+            else:
+                raise Exception("CNV can be deletion or insertion on variant {}.".format(VCFRecord.getName(self)))
+        return is_insertion
+
+    def isInversion(self):
+        """
+        Return True if the variant is a deletion.
+
+        :return: True if the variant is a deletion.
+        :rtype: bool
+        :warnings: This method can only be used on record with only one alternative allele.
+        """
+        if len(self.alt) > 1:
+            raise Exception("The function 'isInversion' cannot be used on multi-allelic variant {}.".format(VCFRecord.getName(self)))
+        is_inversion = False
+        if self.alt[0].startswith("<INV"):
+            is_inversion = True
+        return is_inversion
+
+    def normalizeSingleAllele(self):
+        raise NotImplementedError("Method 'normalizeSingleAllele' is not implemented for {}.".format(self.__class__.__name__))
+
+    def refEnd(self):
+        """
+        Return the last position on reference affected by the alternative allele (1-based).
+
+        :return: The last position on reference affected by the alternative allele (1-based). For an insertion between two nucleotids the value will be: first nucleotids pos + 0.5.
+        :rtype: float | None
+        :warnings: This method can only be used on record with only one alternative allele.
+        """
+        end = self.end
+        if self.isInsertion():  # DUP or INS or CNV representing INS
+            end = self.pos + 0.5
+        return end
+
+    def refStart(self):
+        """
+        Return the first position on reference affected by the alternative allele (1-based).
+
+        :return: The first position on reference affected by the alternative allele (1-based). For an insertion between two nucleotids the value will be: first nucleotids pos + 0.5.
+        :rtype: float | None
+        :warnings: This method can only be used on record with only one alternative allele.
+        """
+        start = None  # CNV
+        if self.isInsertion():  # DUP or INS or CNV representing INS
+            start = self.pos + 0.5
+        elif not self.alt[0].startswith("<CNV"):  # DEL or INV
+            start = self.pos + 1
+        return start
+
+    @property
+    def sv_len(self):
+        """
+        Return difference in length between REF and ALT alleles.
+
+        :return: Difference in length between REF and ALT alleles. Longer ALT alleles (e.g. insertions) have positive values, shorter ALT alleles (e.g. deletions) have negative values.
+        :rtype: int | None
+        :warnings: This method can only be used on record with only one alternative allele.
+        """
+        if len(self.alt) > 1:
+            raise Exception("The attribute 'sv_len' cannot be used on multi-allelic variant {}.".format(VCFRecord.getName(self)))
+        sv_len = None
+        if "SVLEN" in self.info:
+            sv_len = self.info["SVLEN"]
+            if isinstance(sv_len, (list, tuple)):
+                sv_len = sv_len[0]
+        elif "END" in self.info:
+            try:
+                if self.isDeletion():  # DEL
+                    sv_len = - (self.end - self.pos)
+                elif not self.alt[0].startswith("<INS"):  # CNV or DUP or INV (Exclude INS because length is unknown)
+                    sv_len = (self.end - self.pos)
+            except Exception:
+                pass  # CNV with unknown type del or ins
+        return sv_len
+
+    def type(self):
+        """
+        Return the variant type.
+
+        :return: 'indel' or 'inv'.
+        :rtype: str
+        :warnings: This method can only be used on record with only one alternative allele.
+        """
+        record_type = "indel"
+        if self.alt[0].startswith("<INV"):
+            record_type = "inv"
+        return record_type
+
+
 class VCFIO(AbstractFile):
     """Manage VCF file."""
 
     def __init__(self, filepath, mode="r"):
         """
         Return instance of VCFIO.
 
@@ -1271,20 +1610,23 @@
                 info = dict()
                 for tag_and_value in fields[7].split(';'):
                     if "=" not in tag_and_value:  # The field is a flag (self.info[tag]._number == 0)
                         info[tag_and_value] = True
                     else:
                         tag, value = tag_and_value.split('=', 1)
                         if self.info[tag]._number == 1:  # The field contains an unique value
-                            info[tag] = self.info[tag]._type(value)
-                            if self.info[tag].type == "String":
-                                info[tag] = decodeInfoValue(info[tag])
+                            if value != ".":  # Exclude key None value
+                                info[tag] = self.info[tag]._type(value)
+                                if self.info[tag].type == "String":
+                                    info[tag] = decodeInfoValue(info[tag])
                         else:  # The field contains a list (self.info[tag]._number is None or self.info[tag]._number > 1)
                             if value == "":
                                 info[tag] = []
+                            elif value == ".":
+                                pass  # Exclude key with None list
                             elif self.info[tag].type == "String":
                                 info[tag] = [decodeInfoValue(self.info[tag]._type(list_elt)) for list_elt in value.split(",")]
                             else:
                                 info[tag] = [self.info[tag]._type(list_elt) for list_elt in value.split(",")]
                 variation.info = info
 
             if len(fields) >= 9:
@@ -1326,14 +1668,17 @@
                                     if self.format[field_id].type == "String":
                                         spl_data[field_id] = decodeInfoValue(spl_data[field_id])
                             else:  # Number == 0
                                 spl_data[field_id] = True
                     data_by_spl[self.samples[spl_idx]] = spl_data
                 variation.samples = data_by_spl
 
+        if variation.alt[0].startswith("<"):
+            variation = VCFSymbAltRecord.fromStdRecord(variation)
+
         return variation
 
     def write(self, record):
         """
         Write variant record in VCF.
 
         :param record: The variant record.
@@ -1444,22 +1789,27 @@
         self.file_handle.write(last_header_line + "\n")
 
 
 def getAlleleRecord(FH_vcf, record, idx_alt):
     """
     Return the record corresponding to the specified allele in variant.
 
+    :param FH_vcf: Handler on record source file.
+    :type FH_vcf: anacore.vcf.VCFIO
     :param record: The variant record.
-    :type record: VCFRecord
+    :type record: anacore.vcf.VCFRecord
     :param idx_alt: The index of the allele in alt attribute.
     :type idx_alt: int
     :return: The record corresponding to the specified allele in variant.
-    :rtype: VCFRecord
+    :rtype: anacore.vcf.VCFRecord
     """
-    new_record = VCFRecord(
+    new_class = VCFRecord
+    if record.alt[idx_alt].startswith("<"):
+        new_class = VCFSymbAltRecord
+    new_record = new_class(
         region=record.chrom,
         position=record.pos,
         knownSNPId=record.id,
         refAllele=record.ref.upper(),  ########################### pb transfo
         altAlleles=[record.alt[idx_alt].upper()],  ########################### pb transfo
         qual=record.qual,
         pFilter=deepcopy(record.filter),
```

### Comparing `anacore-2.9.0/setup.py` & `anacore-3.0.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #!/usr/bin/env python
 import os
 import re
-from distutils.core import setup
+from setuptools import find_packages, setup
 
 
 def get_long_description():
     content = ""
     with open("README.md", encoding='utf-8') as FH:
         content = FH.read()
     return content
@@ -13,15 +13,15 @@
 
 def get_version():
     version = None
     notes_filepath = "RELEASES_NOTES.md"
     if os.path.exists(notes_filepath):
         with open(notes_filepath) as FH:
             first_line = FH.readline()
-            version = re.search("^\#\s+.+\s+(.+)\s+\[", first_line).groups()[0]  # Example: "# v2.5.0 [DEV]"
+            version = re.search(r"^\#\s+.+\s+(.+)\s+\[", first_line).groups()[0]  # Example: "# v2.5.0 [DEV]"
     return version
 
 
 def load_requirements(path):
     requirements = []
     with open(path) as FH:
         requirements = [elt.strip().replace(" ", "") for elt in FH]
@@ -31,15 +31,15 @@
 setup(
     name='anacore',
     version=get_version(),
     description='Libraries for managing standard file formats and objects from NGS.',
     author='Frederic Escudie',
     author_email='escudie.frederic@iuct-oncopole.fr',
     license='GNU GPL v3',
-    packages=["anacore"],
+    packages=find_packages(),
     install_requires=load_requirements("requirements.txt"),
     url='https://github.com/bialimed/anacore',
     python_requires='>=3.5',
     keywords='bio NGS',
     #long_description_content_type='text/markdown',
     #long_description=get_long_description()
 )
```

### Comparing `anacore-2.9.0/test/test_fusion.py` & `anacore-3.0.0/test/test_fusion.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/test/test_genomicRegion.py` & `anacore-3.0.0/test/test_genomicRegion.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/test/test_gff.py` & `anacore-3.0.0/test/test_gff.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/test/test_gtf.py` & `anacore-3.0.0/test/test_gtf.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/test/test_hgvs.py` & `anacore-3.0.0/test/test_hgvs.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/test/test_picardIO.py` & `anacore-3.0.0/test/test_picardIO.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/test/test_region.py` & `anacore-3.0.0/test/test_region.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/test/test_sequence.py` & `anacore-3.0.0/test/test_sequence.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 #!/usr/bin/env python3
 
 __author__ = 'Frederic Escudie'
 __copyright__ = 'Copyright (C) 2021 IUCT-O'
 __license__ = 'GNU General Public License'
-__version__ = '1.0.0'
+__version__ = '1.1.0'
 __email__ = 'escudie.frederic@iuct-oncopole.fr'
 __status__ = 'prod'
 
 import os
 import sys
 import unittest
 
 TEST_DIR = os.path.dirname(os.path.abspath(__file__))
 PACKAGE_DIR = os.path.dirname(TEST_DIR)
 sys.path.append(PACKAGE_DIR)
 
-from anacore.sequence import AA3LettersAlphabet, CodonAlphabet, DNAAlphabet, RNAAlphabet, Sequence
+from anacore.sequence import AA3LettersAlphabet, CodonAlphabet, DNAAlphabet, getShortestRepeatUnit, RNAAlphabet, Sequence
 
 
 ########################################################################
 #
 # FUNCTIONS
 #
 ########################################################################
@@ -67,14 +67,42 @@
             DNAAlphabet.revCom("GCCGGGATCTGM"),
             "KCAGATCCCGGC"
         )
         with self.assertRaises(Exception):
             DNAAlphabet.revCom("GCCGUGAICTGA")  # Invalid nt
 
 
+class TestGetShortestRepeatUnit(unittest.TestCase):
+    def test(self):
+        self.assertEqual(
+            getShortestRepeatUnit("A"),
+            None
+        )
+        self.assertEqual(
+            getShortestRepeatUnit("AA"),
+            "A"
+        )
+        self.assertEqual(
+            getShortestRepeatUnit("ATATATAT"),
+            "AT"
+        )
+        self.assertEqual(
+            getShortestRepeatUnit("AAAAA"),
+            "A"
+        )
+        self.assertEqual(
+            getShortestRepeatUnit("ATCGAATCGA"),
+            "ATCGA"
+        )
+        self.assertEqual(
+            getShortestRepeatUnit("ATATATAG"),
+            None
+        )
+
+
 class TestRNAAlphabet(unittest.TestCase):
     def testIsValid(self):
         self.assertTrue(RNAAlphabet.isValid("GCCGGGAUCUGM"))
         self.assertFalse(RNAAlphabet.isValid("GCCGIGAUCUGA"))  # Invalid nt
 
     def testRevCom(self):
         self.assertEqual(
```

### Comparing `anacore-2.9.0/test/test_sequenceIO.py` & `anacore-3.0.0/test/test_sequenceIO.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 __author__ = 'Frederic Escudie'
 __copyright__ = 'Copyright (C) 2019 IUCT-O'
 __license__ = 'GNU General Public License'
-__version__ = '1.6.0'
+__version__ = '1.7.0'
 __email__ = 'escudie.frederic@iuct-oncopole.fr'
 __status__ = 'prod'
 
 import os
 import sys
 import gzip
 import uuid
@@ -489,14 +489,29 @@
                 FH.getSub("one", 58, 63)
             )
             # nt on first, second and third line
             self.assertEqual(
                 self.expected_rec["one"].string[29:63],
                 FH.getSub("one", 30, 63)
             )
+            # End of first
+            self.assertEqual(
+                self.expected_rec["one"].string[63:66],
+                FH.getSub("one", 64, 66)
+            )
+            # Ends out of first
+            self.assertEqual(
+                self.expected_rec["one"].string[63:66],
+                FH.getSub("one", 64, 80)
+            )
+            # Starts out of first
+            self.assertEqual(
+                "",
+                FH.getSub("one", 67, 80)
+            )
 
 
 class TestUtils(unittest.TestCase):
     def setUp(self):
         tmp_folder = tempfile.gettempdir()
         unique_id = str(uuid.uuid1())
```

### Comparing `anacore-2.9.0/test/test_sv.py` & `anacore-3.0.0/test/test_sv.py`

 * *Files identical despite different names*

### Comparing `anacore-2.9.0/test/test_vcf.py` & `anacore-3.0.0/test/test_vcf.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python3
 
 __author__ = 'Frederic Escudie'
-__copyright__ = 'Copyright (C) 2017 IUCT-O'
+__copyright__ = 'Copyright (C) 2017 CHU Toulouse'
 __license__ = 'GNU General Public License'
-__version__ = '1.12.0'
+__version__ = '1.15.0'
 __email__ = 'escudie.frederic@iuct-oncopole.fr'
 __status__ = 'prod'
 
 from anacore.sequenceIO import IdxFastaIO
 import os
 import pysam
 import sys
@@ -15,22 +15,235 @@
 import unittest
 import uuid
 
 TEST_DIR = os.path.dirname(os.path.abspath(__file__))
 PACKAGE_DIR = os.path.dirname(TEST_DIR)
 sys.path.append(PACKAGE_DIR)
 
-from anacore.vcf import VCFRecord, VCFIO, getHeaderAttr, HeaderInfoAttr
+from anacore.vcf import getHeaderAttr, HeaderInfoAttr, VCFIO, VCFRecord, VCFSymbAltRecord
 
 
 ########################################################################
 #
 # FUNCTIONS
 #
 ########################################################################
+class TestVCFHeader(unittest.TestCase):
+    def setUp(self):
+        tmp_folder = tempfile.gettempdir()
+        unique_id = str(uuid.uuid1())
+
+        # Temporary files
+        self.tmp_in_variants = os.path.join(tmp_folder, unique_id + "_in.vcf")
+        self.tmp_out_variants = os.path.join(tmp_folder, unique_id + "_out.vcf")
+        content = """##fileformat=VCFv4.3
+##fileDate=20090805
+##source=myImputationProgramV3.1
+##reference=file:///seq/references/1000GenomesPilot-NCBI36.fasta
+##contig=<ID=20,length=62435964,assembly=B36,md5=f126cdf8a6e0c7f379d618ff66beb2da,species="Homo sapiens",taxonomy=x>
+##phasing=partial
+##SAMPLE=<ID=NA00001,Assay="WholeGenome",Description="Patient germline genome from unaffected",Disease="None",DOI="url",Ethnicity="AFR">
+##SAMPLE=<ID=NA00002,Assay="Exome",Description="European patient exome from breast cancer",Disease="Cancer",Ethnicity="CEU",Tissue="Breast">
+##PEDIGREE=<ID=TumourSample,Original=GermlineID>
+##PEDIGREE=<ID=SomaticNonTumour,Original=GermlineID>
+##PEDIGREE=<ID=ChildID,Father=FatherID,Mother=MotherID>
+##PEDIGREE=<ID=SampleID,Name_1=Ancestor_1,Name_N=Ancestor_N>
+##INFO=<ID=NS,Number=1,Type=Integer,Description="Number of Samples With Data",Source="myImputationProgram",Version="3.1">
+##INFO=<ID=DP,Number=1,Type=Integer,Description="Total Depth">
+##INFO=<ID=AF,Number=A,Type=Float,Description="Allele Frequency">
+##INFO=<ID=SRC,Number=.,Type=String,Description="Caller source">
+##INFO=<ID=AA,Number=1,Type=String,Description="Ancestral Allele">
+##INFO=<ID=DB,Number=0,Type=Flag,Description="dbSNP membership",Version="129">
+##INFO=<ID=H2,Number=0,Type=Flag,Description="HapMap2 membership">
+##FILTER=<ID=q10,Description="Quality below 10">
+##FILTER=<ID=s50,Description="Less than 50% of samples have data">
+##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype \\"test\\"">
+##FORMAT=<ID=GQ,Number=1,Type=Integer,Description="Genotype Quality">
+##FORMAT=<ID=DP,Number=1,Type=Integer,Description="Read Depth">
+##FORMAT=<ID=HQ,Number=2,Type=Integer,Description="Haplotype Quality">
+#CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO	FORMAT	NA00001	NA00002	NA00003
+"""
+        with open(self.tmp_in_variants, "w") as FH_variants:
+            FH_variants.write(content)
+
+    def tearDown(self):
+        # Clean temporary files
+        for curr_file in [self.tmp_in_variants, self.tmp_out_variants]:
+            if os.path.exists(curr_file):
+                os.remove(curr_file)
+
+    def testReadWriteHeader(self):
+        with VCFIO(self.tmp_in_variants) as FH_in:
+            with VCFIO(self.tmp_out_variants, "w") as FH_out:
+                FH_out.copyHeader(FH_in)
+                FH_out.writeHeader()
+        expected = None
+        with open(self.tmp_in_variants) as FH_exp:
+            expected = FH_exp.readlines()
+        observed = None
+        with open(self.tmp_out_variants) as FH_obs:
+            observed = FH_obs.readlines()
+        self.assertTrue(len(expected) != 0)
+        self.assertEqual(sorted(expected), sorted(observed))
+
+    def testHeaderAttrDel(self):
+        data = HeaderInfoAttr(
+            id="NS",
+            number="1",
+            type="Integer",
+            description="Number of Samples With Data",
+            source="myImputationProgram",
+            version="3.1"
+        )
+        del(data.source)
+        expected = {"id": "NS", "number": "1", "type": "Integer", "description": "Number of Samples With Data", "version": "3.1"}
+        self.assertEqual(expected, data.datastore)
+
+    def testHeaderAttrKeys(self):
+        data = HeaderInfoAttr(
+            id="NS",
+            number="1",
+            type="Integer",
+            description="Number of Samples With Data",
+            source="myImputationProgram",
+            version="3.1"
+        )
+        expected = sorted(["id", "number", "type", "description", "source", "version"])
+        self.assertEqual(expected, sorted(data.keys()))
+
+    def testHeaderAttrStr(self):
+        data = HeaderInfoAttr(
+            id="NS",
+            number="1",
+            type="Integer",
+            description="Number of Samples With Data",
+            source="myImputationProgram",
+            version="3.1"
+        )
+        expected = '<ID=NS,Number=1,Type=Integer,Description="Number of Samples With Data",Source="myImputationProgram",Version="3.1">'
+        self.assertEqual(expected, str(data))
+
+    def testGetHeaderAttr(self):
+        data = [
+            {
+                "text": '##INFO=<ID=NS,Number=1,Type=Integer,Description="Number of Samples With Data",Source="myImputationProgram",Version="3.1">',
+                "expected_dict": {"id": "NS", "number": "1", "type": "Integer", "description": "Number of Samples With Data", "source": "myImputationProgram", "version": "3.1"},
+                "expected_cls": "HeaderInfoAttr"
+            },
+            {
+                "text": '##INFO=<ID=DP,Number=1,Type=Integer,Description="Total Depth">',
+                "expected_dict": {"id": "DP", "number": "1", "type": "Integer", "description": "Total Depth"},
+                "expected_cls": "HeaderInfoAttr"
+            },
+            {
+                "text": '##INFO=<ID=AF,Number=A,Type=Float,Description="Allele Frequency">',
+                "expected_dict": {"id": "AF", "number": "A", "type": "Float", "description": "Allele Frequency"},
+                "expected_cls": "HeaderInfoAttr"
+            },
+            {
+                "text": '##INFO=<ID=SRC,Number=.,Type=String,Description="Caller source">',
+                "expected_dict": {"id": "SRC", "number": ".", "type": "String", "description": "Caller source"},
+                "expected_cls": "HeaderInfoAttr"
+            },
+            {
+                "text": '##INFO=<ID=DB,Number=0,Type=Flag,Description="dbSNP membership, 2018-01",Version="129">',
+                "expected_dict": {"id": "DB", "number": "0", "type": "Flag", "description": "dbSNP membership, 2018-01", "version": "129"},
+                "expected_cls": "HeaderInfoAttr"
+            },
+            {
+                "text": '##FILTER=<ID=q10,Description="Quality below 10",Source="myImputationProgram",Version=10>',
+                "expected_dict": {"id": "q10", "description": "Quality below 10", "source": "myImputationProgram", "version": "10"},
+                "expected_cls": "HeaderFilterAttr"
+            },
+            {
+                "text": '##FILTER=<ID=s50,Description="Less than 50% of samples have data">',
+                "expected_dict": {"id": "s50", "description": "Less than 50% of samples have data"},
+                "expected_cls": "HeaderFilterAttr"
+            },
+            {
+                "text": '##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">',
+                "expected_dict": {"id": "GT", "number": "1", "type": "String", "description": "Genotype"},
+                "expected_cls": "HeaderFormatAttr"
+            },
+            {
+                "text": '##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype \\"test\\"">',
+                "expected_dict": {"id": "GT", "number": "1", "type": "String", "description": 'Genotype "test"'},
+                "expected_cls": "HeaderFormatAttr"
+            }
+        ]
+        for curr in data:
+            attr = getHeaderAttr(curr["text"])
+            self.assertEqual(curr["expected_dict"], attr.datastore)
+            self.assertEqual(curr["expected_cls"], attr.__class__.__name__)
+
+
+class TestNoneInfo(unittest.TestCase):
+    def setUp(self):
+        tmp_folder = tempfile.gettempdir()
+        unique_id = str(uuid.uuid1())
+        self.tmp_in = os.path.join(tmp_folder, unique_id + "_in.vcf")
+        self.tmp_out = os.path.join(tmp_folder, unique_id + "_out.vcf")
+        with open(self.tmp_in, "w") as FH_variants:
+            FH_variants.write("""##fileformat=VCFv4.3
+##INFO=<ID=AF,Number=A,Type=Float,Description="Allele Frequency">
+##INFO=<ID=DP,Number=1,Type=Integer,Description="Total Depth">
+##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">
+#CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO	FORMAT	NA00001	NA00002	NA00003
+20	14370	.	G	A	29.0	PASS	DP=.;AF=.	GT	0|0	1|0	1/1
+20	14371	.	T	A	29.0	PASS	.	GT	0|0	1|0	1/1
+20	14372	.	C	A	29.0	PASS	DP=300;AF=.	GT	0|0	1|0	1/1
+20	14373	.	C	A	29.0	PASS	DP=300	GT	0|0	1|0	1/1
+20	14374	.	G	A	29.0	PASS	DP=.;AF=0.5	GT	0|0	1|0	1/1
+20	14375	.	T	A	29.0	PASS	AF=0.5	GT	0|0	1|0	1/1
+20	14376	.	C	A	29.0	PASS	DP=300;AF=0.5	GT	0|0	1|0	1/1""")
+
+    def tearDown(self):
+        for curr_file in [self.tmp_in, self.tmp_out]:
+            if os.path.exists(curr_file):
+                os.remove(curr_file)
+
+    def testRecord(self):
+        with VCFIO(self.tmp_in) as reader:
+            for record in reader:
+                if record.pos in {14374, 14375, 14376}:
+                    self.assertTrue("AF" in record.info and record.info["AF"] == [0.5])
+                else:
+                    self.assertTrue("AF" not in record.info)
+                if record.pos in {14372, 14373, 14376}:
+                    self.assertTrue("DP" in record.info and record.info["DP"] == 300)
+                else:
+                    self.assertTrue("DP" not in record.info)
+
+    def testWrite(self):
+        expected_content = """##fileformat=VCFv4.3
+##INFO=<ID=AF,Number=A,Type=Float,Description="Allele Frequency">
+##INFO=<ID=DP,Number=1,Type=Integer,Description="Total Depth">
+##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">
+#CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO	FORMAT	NA00001	NA00002	NA00003
+20	14370	.	G	A	29.0	PASS	.	GT	0|0	1|0	1/1
+20	14371	.	T	A	29.0	PASS	.	GT	0|0	1|0	1/1
+20	14372	.	C	A	29.0	PASS	DP=300	GT	0|0	1|0	1/1
+20	14373	.	C	A	29.0	PASS	DP=300	GT	0|0	1|0	1/1
+20	14374	.	G	A	29.0	PASS	AF=0.5	GT	0|0	1|0	1/1
+20	14375	.	T	A	29.0	PASS	AF=0.5	GT	0|0	1|0	1/1
+20	14376	.	C	A	29.0	PASS	AF=0.5;DP=300	GT	0|0	1|0	1/1"""
+        # Read and write VCF
+        with VCFIO(self.tmp_in) as reader:
+            with VCFIO(self.tmp_out, "w") as writer:
+                writer.copyHeader(reader)
+                writer.writeHeader()
+                for record in reader:
+                    writer.write(record)
+        # Compare input content with output
+        observed_content = None
+        with open(self.tmp_out) as reader:
+            observed_content = "".join(reader.readlines()).strip()
+        self.assertEqual(observed_content, expected_content)
+
+
 class TestVCFIO(unittest.TestCase):
     def setUp(self):
         tmp_folder = tempfile.gettempdir()
         unique_id = str(uuid.uuid1())
 
         # Temporary files
         self.tmp_in_variants = os.path.join(tmp_folder, unique_id + "_in.vcf")
@@ -391,49 +604,61 @@
 ##FORMAT=<ID=AF,Number=R,Type=Float,Description="Allele Frequency">
 ##FORMAT=<ID=DP,Number=1,Type=Integer,Description="Total Depth">
 #CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO	FORMAT	splA	splB
 11	1	two_spl_rAD_aAF_1	A	T	29	PASS	expModel=model_4	AD:DP	2:50	8:50
 11	2	two_spl_rAD_aAF_2	A	T	29	PASS	expModel=model_4	AF:AD	0.96,0.04:2	0.84,0.16:8
 11	3	two_spl_rAD_aAF_3	A	T	29	PASS	expModel=model_4	AF:DP	0.96,0.04:50	0.84,0.16:50
 11	1	two_spl_rAD_aAF_4	A	T,G	29	PASS	expModel=model_5	AD:DP	2,5:50	8,1:50
-11	2	two_spl_rAD_aAF_5	A	T,G	29	PASS	expModel=model_5	AF:AD	0.96,0.04,0.1:2,5	0.84,0.16,0.02:8,1
-11	3	two_spl_rAD_aAF_6	A	T,G	29	PASS	expModel=model_5	AF:DP	0.96,0.04,0.1:50	0.84,0.16,0.02:50"""
+11	2	two_spl_rAD_aAF_5	A	T,G	29	PASS	expModel=model_5	AF:AD	0.86,0.04,0.1:2,5	0.82,0.16,0.02:8,1
+11	3	two_spl_rAD_aAF_6	A	T,G	29	PASS	expModel=model_5	AF:DP	0.86,0.04,0.1:50	0.82,0.16,0.02:50"""
         self.freq_expected = {
             "model_0": {
-                "AF": {"pop": [0.1]},
-                "AD": {"pop": [10]},
+                "AF": {"pop": [0.1], "pop_ref": 0.9},
+                "AD": {"pop": [10], "pop_ref": 90},
                 "DP": {"pop": 100}
             },
             "model_1": {
-                "AF": {"pop": [0.1, 0.05]},
-                "AD": {"pop": [10, 5]},
+                "AF": {"pop": [0.1, 0.05], "pop_ref": 0.85},
+                "AD": {"pop": [10, 5], "pop_ref": 85},
                 "DP": {"pop": 100}
             },
             "model_2": {
-                "AF": {"splA": [0.1], "pop": [0.1]},
-                "AD": {"splA": [10], "pop": [10]},
+                "AF": {"splA": [0.1], "pop": [0.1], "pop_ref": 0.9},
+                "AD": {"splA": [10], "pop": [10], "pop_ref": 90},
                 "DP": {"splA": 100, "pop": 100}
             },
             "model_3": {
-                "AF": {"splA": [0.1, 0.05], "pop": [0.1, 0.05]},
-                "AD": {"splA": [10, 5], "pop": [10, 5]},
+                "AF": {"splA": [0.1, 0.05], "pop": [0.1, 0.05], "pop_ref": 0.85},
+                "AD": {"splA": [10, 5], "pop": [10, 5], "pop_ref": 85},
                 "DP": {"splA": 100, "pop": 100}
             },
             "model_4": {
-                "AF": {"splA": [0.04], "splB": [0.16], "pop": [0.1]},
-                "AD": {"splA": [2], "splB": [8], "pop": [10]},
+                "AF": {"splA": [0.04], "splB": [0.16], "pop": [0.1], "pop_ref": 0.9},
+                "AD": {"splA": [2], "splB": [8], "pop": [10], "pop_ref": 90},
                 "DP": {"splA": 50, "splB": 50, "pop": 100}
             },
             "model_5": {
-                "AF": {"splA": [0.04, 0.1], "splB": [0.16, 0.02], "pop": [0.1, 0.06]},
-                "AD": {"splA": [2, 5], "splB": [8, 1], "pop": [10, 6]},
+                "AF": {"splA": [0.04, 0.1], "splB": [0.16, 0.02], "pop": [0.1, 0.06], "pop_ref": 0.84},
+                "AD": {"splA": [2, 5], "splB": [8, 1], "pop": [10, 6], "pop_ref": 84},
                 "DP": {"splA": 50, "splB": 50, "pop": 100}
             }
         }
 
+    def testContainsIndel(self):
+        data = [
+            {"variant": VCFRecord("chr1", 2, None, "A", ["T"]), "expected": False},
+            {"variant": VCFRecord("chr1", 2, None, "A", ["AT"]), "expected": True},
+            {"variant": VCFRecord("chr1", 1, None, "CA", ["C"]), "expected": True},
+            {"variant": VCFRecord("chr1", 15, None, "CA", ["GT"]), "expected": False},
+            {"variant": VCFRecord("chr1", 15, None, "CA", ["GTT"]), "expected": True},
+            {"variant": VCFRecord("chr1", 15, None, "CAC", ["GT"]), "expected": True}
+        ]
+        for curr in data:
+            self.assertEqual(curr["variant"].containsIndel(), curr["expected"])
+
     def tearDown(self):
         # Clean temporary files
         for curr_file in [self.tmp_fa, self.tmp_fai, self.tmp_variants]:
             if os.path.exists(curr_file):
                 os.remove(curr_file)
 
     def testGetAltAF(self):
@@ -561,14 +786,54 @@
                         expected_records.append("{} {}".format(variant.id, expected_DP))
                         observed_records.append("{} {}".format(variant.id, variant.getPopDP()))
                     except Exception:
                         raise Exception('Error in TestVCFRecord.testGetPopDP() for variant "' + variant.id + '".')
             # Assert
             self.assertEqual(expected_records, observed_records)
 
+    def testGetPopRefAD(self):
+        for curr_dataset in sorted(self.freq_data):
+            # Write test data
+            content = self.freq_data[curr_dataset]
+            with open(self.tmp_variants, "w") as FH_variants:
+                FH_variants.write(content)
+            # Parse
+            expected_records = list()
+            observed_records = list()
+            with VCFIO(self.tmp_variants) as FH_vcf:
+                for variant in FH_vcf:
+                    try:
+                        expected_AD = self.freq_expected[variant.info["expModel"]]["AD"]["pop_ref"]
+                        expected_records.append("{} {}".format(variant.id, expected_AD))
+                        observed_records.append("{} {}".format(variant.id, variant.getPopRefAD()))
+                    except Exception:
+                        raise Exception('Error in TestVCFRecord.testGetPopRefAD() for variant "{}".'.format(variant.id))
+            # Assert
+            self.assertEqual(expected_records, observed_records)
+
+    def testGetPopRefAF(self):
+        for curr_dataset in sorted(self.freq_data):
+            # Write test data
+            content = self.freq_data[curr_dataset]
+            with open(self.tmp_variants, "w") as FH_variants:
+                FH_variants.write(content)
+            # Parse
+            expected_records = list()
+            observed_records = list()
+            with VCFIO(self.tmp_variants) as FH_vcf:
+                for variant in FH_vcf:
+                    try:
+                        expected_AF = self.freq_expected[variant.info["expModel"]]["AF"]["pop_ref"]
+                        expected_records.append("{} {}".format(variant.id, expected_AF))
+                        observed_records.append("{} {}".format(variant.id, variant.getPopRefAF()))
+                    except Exception:
+                        raise Exception('Error in TestVCFRecord.testGetPopRefAF() for variant "{}".'.format(variant.id))
+            # Assert
+            self.assertEqual(expected_records, observed_records)
+
     def testNormalizeSingleAllele(self):
         # Test substitution one nt
         substitution = VCFRecord("artificial_1", 18, None, "TC", ["TA"], 230)
         substitution.normalizeSingleAllele()
         self.assertTrue(substitution.ref == "C" and substitution.alt[0] == "A" and substitution.pos == 19)
         # Test substitution multi nt
         substitution = VCFRecord("artificial_1", 18, None, "TCtgA", ["TaGCc"], 230)
@@ -821,162 +1086,209 @@
             {"variant": VCFRecord("chr1", 15, None, "CA", ["GT"]), "expected": False},
             {"variant": VCFRecord("chr1", 15, None, "CA", ["GTT"]), "expected": True},
             {"variant": VCFRecord("chr1", 15, None, "CAC", ["GT"]), "expected": False}
         ]
         for curr in data:
             self.assertEqual(curr["variant"].isInsertion(), curr["expected"])
 
+    def testType(self):
+        data = [
+            {"variant": VCFRecord("chr1", 2, None, "A", ["T"]), "expected": "snp"},
+            {"variant": VCFRecord("chr1", 2, None, "A", ["AT"]), "expected": "indel"},
+            {"variant": VCFRecord("chr1", 1, None, "CA", ["C"]), "expected": "indel"},
+            {"variant": VCFRecord("chr1", 15, None, "CA", ["GT"]), "expected": "variation"},
+            {"variant": VCFRecord("chr1", 15, None, "CA", ["GTT"]), "expected": "indel"},
+            {"variant": VCFRecord("chr1", 15, None, "CAC", ["GT"]), "expected": "indel"}
+        ]
+        for curr in data:
+            self.assertEqual(curr["variant"].type(), curr["expected"])
 
-class TestVCFHeader(unittest.TestCase):
+
+class TestVCFSymbAltRecord(unittest.TestCase):
     def setUp(self):
         tmp_folder = tempfile.gettempdir()
         unique_id = str(uuid.uuid1())
-
-        # Temporary files
-        self.tmp_in_variants = os.path.join(tmp_folder, unique_id + "_in.vcf")
-        self.tmp_out_variants = os.path.join(tmp_folder, unique_id + "_out.vcf")
-        content = """##fileformat=VCFv4.3
-##fileDate=20090805
-##source=myImputationProgramV3.1
-##reference=file:///seq/references/1000GenomesPilot-NCBI36.fasta
-##contig=<ID=20,length=62435964,assembly=B36,md5=f126cdf8a6e0c7f379d618ff66beb2da,species="Homo sapiens",taxonomy=x>
-##phasing=partial
-##SAMPLE=<ID=NA00001,Assay="WholeGenome",Description="Patient germline genome from unaffected",Disease="None",DOI="url",Ethnicity="AFR">
-##SAMPLE=<ID=NA00002,Assay="Exome",Description="European patient exome from breast cancer",Disease="Cancer",Ethnicity="CEU",Tissue="Breast">
-##PEDIGREE=<ID=TumourSample,Original=GermlineID>
-##PEDIGREE=<ID=SomaticNonTumour,Original=GermlineID>
-##PEDIGREE=<ID=ChildID,Father=FatherID,Mother=MotherID>
-##PEDIGREE=<ID=SampleID,Name_1=Ancestor_1,Name_N=Ancestor_N>
-##INFO=<ID=NS,Number=1,Type=Integer,Description="Number of Samples With Data",Source="myImputationProgram",Version="3.1">
-##INFO=<ID=DP,Number=1,Type=Integer,Description="Total Depth">
-##INFO=<ID=AF,Number=A,Type=Float,Description="Allele Frequency">
-##INFO=<ID=SRC,Number=.,Type=String,Description="Caller source">
-##INFO=<ID=AA,Number=1,Type=String,Description="Ancestral Allele">
-##INFO=<ID=DB,Number=0,Type=Flag,Description="dbSNP membership",Version="129">
-##INFO=<ID=H2,Number=0,Type=Flag,Description="HapMap2 membership">
-##FILTER=<ID=q10,Description="Quality below 10">
-##FILTER=<ID=s50,Description="Less than 50% of samples have data">
-##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype \\"test\\"">
-##FORMAT=<ID=GQ,Number=1,Type=Integer,Description="Genotype Quality">
-##FORMAT=<ID=DP,Number=1,Type=Integer,Description="Read Depth">
-##FORMAT=<ID=HQ,Number=2,Type=Integer,Description="Haplotype Quality">
-#CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO	FORMAT	NA00001	NA00002	NA00003
-"""
-        with open(self.tmp_in_variants, "w") as FH_variants:
-            FH_variants.write(content)
+        self.tmp_variants = os.path.join(tmp_folder, unique_id + ".vcf")
+        with open(self.tmp_variants, "w") as writer:
+            writer.write("""##fileformat=VCFv4.3
+##fileDate=20100501
+##reference=1000GenomesPilot-NCBI36
+##assembly=ftp://ftp-trace.ncbi.nih.gov/1000genomes/ftp/release/sv/breakpoint_assemblies.fasta
+##INFO=<ID=BKPTID,Number=.,Type=String,Description="ID of the assembled alternate allele in the assembly file">
+##INFO=<ID=CIEND,Number=2,Type=Integer,Description="Confidence interval around END for imprecise variants">
+##INFO=<ID=CIPOS,Number=2,Type=Integer,Description="Confidence interval around POS for imprecise variants">
+##INFO=<ID=END,Number=1,Type=Integer,Description="End position of the variant described in this record">
+##INFO=<ID=HOMLEN,Number=.,Type=Integer,Description="Length of base pair identical micro-homology at event breakpoints">
+##INFO=<ID=HOMSEQ,Number=.,Type=String,Description="Sequence of base pair identical micro-homology at event breakpoints">
+##INFO=<ID=SVLEN,Number=.,Type=Integer,Description="Difference in length between REF and ALT alleles">
+##INFO=<ID=SVTYPE,Number=1,Type=String,Description="Type of structural variant">
+##ALT=<ID=DEL,Description="Deletion">
+##ALT=<ID=DEL:ME:ALU,Description="Deletion of ALU element">
+##ALT=<ID=DEL:ME:L1,Description="Deletion of L1 element">
+##ALT=<ID=DUP,Description="Duplication">
+##ALT=<ID=DUP:TANDEM,Description="Tandem Duplication">
+##ALT=<ID=INS,Description="Insertion of novel sequence">
+##ALT=<ID=INS:ME:ALU,Description="Insertion of ALU element">
+##ALT=<ID=INS:ME:L1,Description="Insertion of L1 element">
+##ALT=<ID=INV,Description="Inversion">
+##ALT=<ID=CNV,Description="Copy number variable region">
+##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">
+##FORMAT=<ID=GQ,Number=1,Type=Integer,Description="Genotype quality">
+##FORMAT=<ID=CN,Number=1,Type=Integer,Description="Copy number genotype for imprecise events">
+##FORMAT=<ID=CNQ,Number=1,Type=Float,Description="Copy number genotype quality for imprecise events">
+#CHROM	POS	ID	REF	ALT	QUAL	FILTER	INFO	FORMAT	NA00001
+1	100	cnv_notation	T	<CNV:TR>	.	.	END=130;SVLEN=30	GT	1/2
+1	2827694	rs2376870	CGTGGATGCGGGGAC	C	.	PASS	SVTYPE=DEL;END=2827708;HOMLEN=1;HOMSEQ=G;SVLEN=-14	GT:GQ	1/1:14
+2	321682	.	T	<DEL>	6	PASS	SVTYPE=DEL;END=321887;SVLEN=-205;CIPOS=-56,20;CIEND=-10,62	GT:GQ	0/1:12
+2	321682	INV0	T	<INV>	6	PASS	SVTYPE=INV;END=421681	.	.
+2	14477084	.	C	<DEL:ME:ALU>	12	PASS	SVTYPE=DEL;END=14477381;SVLEN=-297;CIPOS=-22,18;CIEND=-12,32	GT:GQ	0/1:12
+3	9425916	.	C	<INS:ME:L1>	23	PASS	SVTYPE=INS;END=9425916;SVLEN=6027;CIPOS=-16,22	GT:GQ	1/1:15
+3	12665100	.	A	<DUP>	14	PASS	SVTYPE=DUP;END=12686200;SVLEN=21100;CIPOS=-500,500;CIEND=-500,500	GT:GQ:CN:CNQ	./.:0:3:16.2
+4	18665128	.	T	<DUP:TANDEM>	11	PASS	SVTYPE=DUP;END=18665204;SVLEN=76;CIPOS=-10,10;CIEND=-10,10	GT:GQ:CN:CNQ	./.:0:5:8.3
+17	41242722	.	N	<DEL>	.	.	END=41246879	GT	./.""")
 
     def tearDown(self):
-        # Clean temporary files
-        for curr_file in [self.tmp_in_variants, self.tmp_out_variants]:
+        for curr_file in [self.tmp_variants]:
             if os.path.exists(curr_file):
                 os.remove(curr_file)
 
-    def testReadWriteHeader(self):
-        with VCFIO(self.tmp_in_variants) as FH_in:
-            with VCFIO(self.tmp_out_variants, "w") as FH_out:
-                FH_out.copyHeader(FH_in)
-                FH_out.writeHeader()
-        expected = None
-        with open(self.tmp_in_variants) as FH_exp:
-            expected = FH_exp.readlines()
-        observed = None
-        with open(self.tmp_out_variants) as FH_obs:
-            observed = FH_obs.readlines()
-        self.assertTrue(len(expected) != 0)
-        self.assertEqual(sorted(expected), sorted(observed))
+    def testEnd(self):
+        # With END
+        expected = [130, 321887, 421681, 14477381, 9425916, 12686200, 18665204, 41246879]
+        observed = list()
+        with VCFIO(self.tmp_variants) as reader:
+            for record in reader:
+                if record.__class__ is VCFSymbAltRecord:
+                    observed.append(record.end)
+        self.assertEqual(observed, expected)
+        # Without END
+        expected = [130, 321887, None, 14477381, 9425916, 12686200, 18665204, None]
+        observed = list()
+        with VCFIO(self.tmp_variants) as reader:
+            for record in reader:
+                if record.__class__ is VCFSymbAltRecord:
+                    if "END" in record.info:
+                        del record.info["END"]
+                    observed.append(record.end)
+        self.assertEqual(observed, expected)
 
-    def testHeaderAttrDel(self):
-        data = HeaderInfoAttr(
-            id="NS",
-            number="1",
-            type="Integer",
-            description="Number of Samples With Data",
-            source="myImputationProgram",
-            version="3.1"
-        )
-        del(data.source)
-        expected = {"id": "NS", "number": "1", "type": "Integer", "description": "Number of Samples With Data", "version": "3.1"}
-        self.assertEqual(expected, data.datastore)
+    def testGetName(self):
+        expected = [
+            "1:100[30]=T/<CNV:TR>",
+            "1:2827694=CGTGGATGCGGGGAC/C",
+            "2:321682[-205]=T/<DEL>",
+            "2:321682[99999]=T/<INV>",
+            "2:14477084[-297]=C/<DEL:ME:ALU>",
+            "3:9425916[6027]=C/<INS:ME:L1>",
+            "3:12665100[21100]=A/<DUP>",
+            "4:18665128[76]=T/<DUP:TANDEM>",
+            "17:41242722[-4157]=N/<DEL>"
+        ]
+        observed = list()
+        with VCFIO(self.tmp_variants) as reader:
+            for record in reader:
+                observed.append(record.getName())
+        self.assertEqual(observed, expected)
 
-    def testHeaderAttrKeys(self):
-        data = HeaderInfoAttr(
-            id="NS",
-            number="1",
-            type="Integer",
-            description="Number of Samples With Data",
-            source="myImputationProgram",
-            version="3.1"
-        )
-        expected = sorted(["id", "number", "type", "description", "source", "version"])
-        self.assertEqual(expected, sorted(data.keys()))
+    def testIsDeletion(self):
+        expected = [False, True, True, False, True, False, False, False, True]
+        observed = list()
+        with VCFIO(self.tmp_variants) as reader:
+            for record in reader:
+                observed.append(record.isDeletion())
+        self.assertEqual(observed, expected)
+
+    def testIsIndel(self):
+        expected = [True, True, True, False, True, True, True, True, True]
+        observed = list()
+        with VCFIO(self.tmp_variants) as reader:
+            for record in reader:
+                observed.append(record.isIndel())
+        self.assertEqual(observed, expected)
 
-    def testHeaderAttrStr(self):
-        data = HeaderInfoAttr(
-            id="NS",
-            number="1",
-            type="Integer",
-            description="Number of Samples With Data",
-            source="myImputationProgram",
-            version="3.1"
-        )
-        expected = '<ID=NS,Number=1,Type=Integer,Description="Number of Samples With Data",Source="myImputationProgram",Version="3.1">'
-        self.assertEqual(expected, str(data))
+    def testIsInsAndDel(self):
+        expected = [False, False, False, False, False, False, False, False, False]
+        observed = list()
+        with VCFIO(self.tmp_variants) as reader:
+            for record in reader:
+                observed.append(record.isInsAndDel())
+        self.assertEqual(observed, expected)
 
-    def testGetHeaderAttr(self):
-        data = [
-            {
-                "text": '##INFO=<ID=NS,Number=1,Type=Integer,Description="Number of Samples With Data",Source="myImputationProgram",Version="3.1">',
-                "expected_dict": {"id": "NS", "number": "1", "type": "Integer", "description": "Number of Samples With Data", "source": "myImputationProgram", "version": "3.1"},
-                "expected_cls": "HeaderInfoAttr"
-            },
-            {
-                "text": '##INFO=<ID=DP,Number=1,Type=Integer,Description="Total Depth">',
-                "expected_dict": {"id": "DP", "number": "1", "type": "Integer", "description": "Total Depth"},
-                "expected_cls": "HeaderInfoAttr"
-            },
-            {
-                "text": '##INFO=<ID=AF,Number=A,Type=Float,Description="Allele Frequency">',
-                "expected_dict": {"id": "AF", "number": "A", "type": "Float", "description": "Allele Frequency"},
-                "expected_cls": "HeaderInfoAttr"
-            },
-            {
-                "text": '##INFO=<ID=SRC,Number=.,Type=String,Description="Caller source">',
-                "expected_dict": {"id": "SRC", "number": ".", "type": "String", "description": "Caller source"},
-                "expected_cls": "HeaderInfoAttr"
-            },
-            {
-                "text": '##INFO=<ID=DB,Number=0,Type=Flag,Description="dbSNP membership, 2018-01",Version="129">',
-                "expected_dict": {"id": "DB", "number": "0", "type": "Flag", "description": "dbSNP membership, 2018-01", "version": "129"},
-                "expected_cls": "HeaderInfoAttr"
-            },
-            {
-                "text": '##FILTER=<ID=q10,Description="Quality below 10",Source="myImputationProgram",Version=10>',
-                "expected_dict": {"id": "q10", "description": "Quality below 10", "source": "myImputationProgram", "version": "10"},
-                "expected_cls": "HeaderFilterAttr"
-            },
-            {
-                "text": '##FILTER=<ID=s50,Description="Less than 50% of samples have data">',
-                "expected_dict": {"id": "s50", "description": "Less than 50% of samples have data"},
-                "expected_cls": "HeaderFilterAttr"
-            },
-            {
-                "text": '##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype">',
-                "expected_dict": {"id": "GT", "number": "1", "type": "String", "description": "Genotype"},
-                "expected_cls": "HeaderFormatAttr"
-            },
-            {
-                "text": '##FORMAT=<ID=GT,Number=1,Type=String,Description="Genotype \\"test\\"">',
-                "expected_dict": {"id": "GT", "number": "1", "type": "String", "description": 'Genotype "test"'},
-                "expected_cls": "HeaderFormatAttr"
-            }
+    def testIsInsertion(self):
+        expected = [True, False, False, False, False, True, True, True, False]
+        observed = list()
+        with VCFIO(self.tmp_variants) as reader:
+            for record in reader:
+                observed.append(record.isInsertion())
+        self.assertEqual(observed, expected)
+
+    def testIsInversion(self):
+        expected = [False, False, True, False, False, False, False, False]
+        observed = list()
+        with VCFIO(self.tmp_variants) as reader:
+            for record in reader:
+                if record.__class__ is VCFSymbAltRecord:
+                    observed.append(record.isInversion())
+        self.assertEqual(observed, expected)
+
+    def testParsingClass(self):
+        expected = [
+            VCFSymbAltRecord, VCFRecord, VCFSymbAltRecord, VCFSymbAltRecord,
+            VCFSymbAltRecord, VCFSymbAltRecord, VCFSymbAltRecord,
+            VCFSymbAltRecord, VCFSymbAltRecord
         ]
-        for curr in data:
-            attr = getHeaderAttr(curr["text"])
-            self.assertEqual(curr["expected_dict"], attr.datastore)
-            self.assertEqual(curr["expected_cls"], attr.__class__.__name__)
+        observed = list()
+        with VCFIO(self.tmp_variants) as reader:
+            for record in reader:
+                observed.append(record.__class__)
+        self.assertEqual(observed, expected)
+
+    def testRefEnd(self):
+        expected = [100.5, 2827708, 321887, 421681, 14477381, 9425916.5, 12665100.5, 18665128.5, 41246879]
+        observed = list()
+        with VCFIO(self.tmp_variants) as reader:
+            for record in reader:
+                observed.append(record.refEnd())
+        self.assertEqual(observed, expected)
+
+    def testRefStart(self):
+        expected = [100.5, 2827695, 321683, 321683, 14477085, 9425916.5, 12665100.5, 18665128.5, 41242723]
+        observed = list()
+        with VCFIO(self.tmp_variants) as reader:
+            for record in reader:
+                observed.append(record.refStart())
+        self.assertEqual(observed, expected)
+
+    def testSvLen(self):
+        # With SVLEN
+        expected = [30, -205, 99999, -297, 6027, 21100, 76, -4157]
+        observed = list()
+        with VCFIO(self.tmp_variants) as reader:
+            for record in reader:
+                if record.__class__ is VCFSymbAltRecord:
+                    observed.append(record.sv_len)
+        self.assertEqual(observed, expected)
+        # Without SVLEN
+        expected = [None, -205, 99999, -297, None, 21100, 76, -4157]
+        observed = list()
+        with VCFIO(self.tmp_variants) as reader:
+            for record in reader:
+                if record.__class__ is VCFSymbAltRecord:
+                    if "SVLEN" in record.info:
+                        del record.info["SVLEN"]
+                    observed.append(record.sv_len)
+        self.assertEqual(observed, expected)
+
+    def testType(self):
+        expected = ["indel", "indel", "indel", "inv", "indel", "indel", "indel", "indel", "indel"]
+        observed = list()
+        with VCFIO(self.tmp_variants) as reader:
+            for record in reader:
+                observed.append(record.type())
+        self.assertEqual(observed, expected)
 
 
 ########################################################################
 #
 # MAIN
 #
 ########################################################################
```

