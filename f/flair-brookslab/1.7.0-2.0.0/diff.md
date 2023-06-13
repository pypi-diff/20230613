# Comparing `tmp/flair-brookslab-1.7.0.tar.gz` & `tmp/flair-brookslab-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/hive/users/jeltje/flair/tmp/flair/dist/tmpei6zvpa6/flair-brookslab-1.7.0.tar", last modified: Thu Oct 27 20:14:18 2022, max compression
+gzip compressed data, was "/hive/users/jeltje/flair/master_flair/dist/tmpo3urlbdr/flair-brookslab-2.0.0.tar", last modified: Tue Jun 13 19:34:16 2023, max compression
```

## Comparing `flair-brookslab-1.7.0.tar` & `flair-brookslab-2.0.0.tar`

### file list

```diff
@@ -1,59 +1,63 @@
-drwxrwxr-x   0 jeltje   (30017) protein   (1304)        0 2022-10-27 20:14:18.000000 flair-brookslab-1.7.0/
--rw-rw-r--   0 jeltje   (30017) protein   (1304)     2904 2022-10-27 20:14:18.000000 flair-brookslab-1.7.0/PKG-INFO
-drwxrwxr-x   0 jeltje   (30017) protein   (1304)        0 2022-10-27 20:14:18.000000 flair-brookslab-1.7.0/bin/
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)    14469 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/bin/plot_isoform_usage
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)      792 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/bin/psl_to_bed
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     5062 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/bin/bam2Bed12
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     2423 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/bin/normalize_counts_matrix
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     7785 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/bin/mark_productivity
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1693 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/bin/bed_to_psl
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)    30976 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/bin/junctions_from_sam
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1380 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/bin/diffsplice_fishers_exact
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1070 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/bin/fasta_seq_lengths
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     2975 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/bin/mark_intron_retention
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     2892 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/bin/diff_iso_usage
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)    12153 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/bin/predictProductivity
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)      447 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/bin/sam_to_map
--rw-rw-r--   0 jeltje   (30017) protein   (1304)     1568 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/LICENSE.txt
--rw-rw-r--   0 jeltje   (30017) protein   (1304)     1131 2022-10-27 20:14:18.000000 flair-brookslab-1.7.0/setup.cfg
--rw-rw-r--   0 jeltje   (30017) protein   (1304)      753 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/README.md
--rw-rw-r--   0 jeltje   (30017) protein   (1304)       85 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/pyproject.toml
-drwxrwxr-x   0 jeltje   (30017) protein   (1304)        0 2022-10-27 20:14:18.000000 flair-brookslab-1.7.0/src/
-drwxrwxr-x   0 jeltje   (30017) protein   (1304)        0 2022-10-27 20:14:18.000000 flair-brookslab-1.7.0/src/flair/
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     7277 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/runDU.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1382 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/es_as_inc_excl_to_counts.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     8816 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/bed_to_sequence.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1996 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/match_counts.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)    53154 2022-10-27 19:59:07.000000 flair-brookslab-1.7.0/src/flair/flair.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     7711 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/filter_collapsed_isoforms.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1409 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/counts_to_tpm.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1329 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/pull_starts.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     5033 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/bed_to_gtf.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     2091 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/consolidate_isoforms.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)    14849 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/ssPrep.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     5592 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/identify_annotated_gene.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     5062 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/bam2Bed12.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)    26725 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/collapse_isoforms_precise.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)        0 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/__init__.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)    11489 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/filter_collapsed_isoforms_from_annotation.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)    13179 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/deFLAIR.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)    10607 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/runDS.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     6282 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/get_phase_sets.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     8268 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/samJuncs.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     9070 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/runDE.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)    16561 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/ssCorrect.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1325 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/subset_unassigned_reads.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     5341 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/es_as.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     9775 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/identify_gene_isoform.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)      537 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/select_from_bed.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1572 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/filter_isoforms_by_proportion_of_gene_expr.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     8344 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/call_diffsplice_events.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)    15324 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/count_sam_transcripts.py
--rwxrwxr-x   0 jeltje   (30017) protein   (1304)     5690 2022-10-27 19:57:11.000000 flair-brookslab-1.7.0/src/flair/gtf_to_bed.py
-drwxrwxr-x   0 jeltje   (30017) protein   (1304)        0 2022-10-27 20:14:18.000000 flair-brookslab-1.7.0/src/flair_brookslab.egg-info/
--rw-rw-r--   0 jeltje   (30017) protein   (1304)     1460 2022-10-27 20:14:18.000000 flair-brookslab-1.7.0/src/flair_brookslab.egg-info/SOURCES.txt
--rw-rw-r--   0 jeltje   (30017) protein   (1304)     2904 2022-10-27 20:14:18.000000 flair-brookslab-1.7.0/src/flair_brookslab.egg-info/PKG-INFO
--rw-rw-r--   0 jeltje   (30017) protein   (1304)        1 2022-10-27 20:14:18.000000 flair-brookslab-1.7.0/src/flair_brookslab.egg-info/dependency_links.txt
--rw-rw-r--   0 jeltje   (30017) protein   (1304)        6 2022-10-27 20:14:18.000000 flair-brookslab-1.7.0/src/flair_brookslab.egg-info/top_level.txt
--rw-rw-r--   0 jeltje   (30017) protein   (1304)       44 2022-10-27 20:14:18.000000 flair-brookslab-1.7.0/src/flair_brookslab.egg-info/entry_points.txt
--rw-rw-r--   0 jeltje   (30017) protein   (1304)       51 2022-10-27 20:14:18.000000 flair-brookslab-1.7.0/src/flair_brookslab.egg-info/requires.txt
+drwxrwxr-x   0 jeltje   (30017) protein   (1304)        0 2023-06-13 19:34:16.000000 flair-brookslab-2.0.0/
+-rw-rw-r--   0 jeltje   (30017) protein   (1304)     2903 2023-06-13 19:34:16.000000 flair-brookslab-2.0.0/PKG-INFO
+drwxrwxr-x   0 jeltje   (30017) protein   (1304)        0 2023-06-13 19:34:16.000000 flair-brookslab-2.0.0/bin/
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     5592 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/bin/identify_annotated_gene
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     9775 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/bin/identify_gene_isoform
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)    14469 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/bin/plot_isoform_usage
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)      792 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/bin/psl_to_bed
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     8094 2023-03-02 19:17:50.000000 flair-brookslab-2.0.0/bin/assign_variants_to_transcripts
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     9107 2023-03-02 19:11:15.000000 flair-brookslab-2.0.0/bin/bed_to_sequence
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     5020 2023-06-06 16:49:40.000000 flair-brookslab-2.0.0/bin/bam2Bed12
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     2423 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/bin/normalize_counts_matrix
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     7785 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/bin/mark_productivity
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1693 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/bin/bed_to_psl
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)    30976 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/bin/junctions_from_sam
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1380 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/bin/diffsplice_fishers_exact
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1070 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/bin/fasta_seq_lengths
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     2975 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/bin/mark_intron_retention
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     2885 2023-06-01 19:13:05.000000 flair-brookslab-2.0.0/bin/diff_iso_usage
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     5687 2023-03-02 19:34:05.000000 flair-brookslab-2.0.0/bin/gtf_to_bed
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)    12270 2023-03-02 19:33:34.000000 flair-brookslab-2.0.0/bin/predictProductivity
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)      447 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/bin/sam_to_map
+-rw-rw-r--   0 jeltje   (30017) protein   (1304)     1568 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/LICENSE.txt
+-rw-rw-r--   0 jeltje   (30017) protein   (1304)     1260 2023-06-13 19:34:16.000000 flair-brookslab-2.0.0/setup.cfg
+-rw-rw-r--   0 jeltje   (30017) protein   (1304)      752 2023-03-02 19:01:28.000000 flair-brookslab-2.0.0/README.md
+-rw-rw-r--   0 jeltje   (30017) protein   (1304)       85 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/pyproject.toml
+drwxrwxr-x   0 jeltje   (30017) protein   (1304)        0 2023-06-13 19:34:16.000000 flair-brookslab-2.0.0/src/
+drwxrwxr-x   0 jeltje   (30017) protein   (1304)        0 2023-06-13 19:34:16.000000 flair-brookslab-2.0.0/src/flair/
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     7277 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/runDU.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1382 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/es_as_inc_excl_to_counts.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     9107 2023-03-02 19:11:15.000000 flair-brookslab-2.0.0/src/flair/bed_to_sequence.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1996 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/match_counts.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)    52767 2023-06-13 19:20:58.000000 flair-brookslab-2.0.0/src/flair/flair.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     7711 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/filter_collapsed_isoforms.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1409 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/counts_to_tpm.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1329 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/pull_starts.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     5026 2023-06-01 19:17:29.000000 flair-brookslab-2.0.0/src/flair/bed_to_gtf.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     2091 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/consolidate_isoforms.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)    14849 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/ssPrep.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     5020 2023-06-06 16:49:40.000000 flair-brookslab-2.0.0/src/flair/bam2Bed12.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)    26725 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/collapse_isoforms_precise.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)        0 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/__init__.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)    11489 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/filter_collapsed_isoforms_from_annotation.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)    13179 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/deFLAIR.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)    10607 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/runDS.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     6282 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/get_phase_sets.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     8268 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/samJuncs.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     9070 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/runDE.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)    16561 2023-03-02 19:12:16.000000 flair-brookslab-2.0.0/src/flair/ssCorrect.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1283 2023-06-06 17:44:16.000000 flair-brookslab-2.0.0/src/flair/subset_unassigned_reads.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     5341 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/es_as.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     9775 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/identify_gene_isoform.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)      537 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/select_from_bed.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     1547 2023-06-09 19:26:05.000000 flair-brookslab-2.0.0/src/flair/filter_isoforms_by_proportion_of_gene_expr.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     8344 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/call_diffsplice_events.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)    15324 2023-03-02 18:24:36.000000 flair-brookslab-2.0.0/src/flair/count_sam_transcripts.py
+-rwxrwxr-x   0 jeltje   (30017) protein   (1304)     5687 2023-03-02 19:34:05.000000 flair-brookslab-2.0.0/src/flair/gtf_to_bed.py
+drwxrwxr-x   0 jeltje   (30017) protein   (1304)        0 2023-06-13 19:34:16.000000 flair-brookslab-2.0.0/src/flair_brookslab.egg-info/
+-rw-rw-r--   0 jeltje   (30017) protein   (1304)     1547 2023-06-13 19:34:16.000000 flair-brookslab-2.0.0/src/flair_brookslab.egg-info/SOURCES.txt
+-rw-rw-r--   0 jeltje   (30017) protein   (1304)     2903 2023-06-13 19:34:16.000000 flair-brookslab-2.0.0/src/flair_brookslab.egg-info/PKG-INFO
+-rw-rw-r--   0 jeltje   (30017) protein   (1304)        1 2023-06-13 19:34:16.000000 flair-brookslab-2.0.0/src/flair_brookslab.egg-info/dependency_links.txt
+-rw-rw-r--   0 jeltje   (30017) protein   (1304)        6 2023-06-13 19:34:16.000000 flair-brookslab-2.0.0/src/flair_brookslab.egg-info/top_level.txt
+-rw-rw-r--   0 jeltje   (30017) protein   (1304)       44 2023-06-13 19:34:16.000000 flair-brookslab-2.0.0/src/flair_brookslab.egg-info/entry_points.txt
+-rw-rw-r--   0 jeltje   (30017) protein   (1304)       51 2023-06-13 19:34:16.000000 flair-brookslab-2.0.0/src/flair_brookslab.egg-info/requires.txt
```

### Comparing `flair-brookslab-1.7.0/PKG-INFO` & `flair-brookslab-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flair-brookslab
-Version: 1.7.0
+Version: 2.0.0
 Summary: flair
 Home-page: https://github.com/BrooksLabUCSC/flair
 Author: Jeltje van Baren
 Author-email: jeltje.van.baren@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/BrooksLabUCSC/flair/issues
 Project-URL: repository, https://github.com/BrooksLabUCSC/flair
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # flair
-FLAIR (Full-Length Alternative Isoform analysis of RNA) for the correction, isoform definition, and alternative splicing analysis of noisy reads. FLAIR has primarily been used for nanopore cDNA, native RNA, and PacBio sequencing reads. 
+FLAIR (Full-Length Alternative Isoform analysis of RNA) for the correction, isoform definition, and alternative splicing analysis of noisy reads. FLAIR has primarily been used for nanopore cDNA, native RNA, and PacBio sequencing reads.
 
 The complete Flair manual is available via [readthedocs](https://flair.readthedocs.io/en/latest/)
 
 ## Cite FLAIR <a name="cite"></a>
 If you use or discuss FLAIR, please cite the following [paper](https://www.nature.com/articles/s41467-020-15171-6):
 >Tang, A.D., Soulette, C.M., van Baren, M.J. et al. Full-length transcript characterization of SF3B1 mutation in chronic lymphocytic leukemia reveals downregulation of retained introns. Nat Commun 11, 1438 (2020). https://doi.org/10.1038/s41467-020-15171-6
```

### Comparing `flair-brookslab-1.7.0/bin/plot_isoform_usage` & `flair-brookslab-2.0.0/bin/plot_isoform_usage`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/bin/psl_to_bed` & `flair-brookslab-2.0.0/bin/psl_to_bed`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/bin/bam2Bed12` & `flair-brookslab-2.0.0/bin/bam2Bed12`

 * *Files 3% similar despite different names*

```diff
@@ -125,21 +125,21 @@
     for num, readData in enumerate(sObj.readJuncs(),0):
         read, chrom, startPos, junctions, endPos, flags, tags, score = readData
         blocks, sizes, starts = juncsToBed12(startPos, endPos, junctions)
         flags = str(flags)
 
         if tags == "+":
 
-            print(chrom, startPos, endPos, read + ";" + flags, score, tags, startPos, endPos, positiveTxn, blocks,
+            print(chrom, startPos, endPos, read, score, tags, startPos, endPos, positiveTxn, blocks,
                 ",".join(str(x) for x in sizes) + ",", ",".join(str(x) for x in starts) + ",", sep="\t")
         elif tags == "-":
-            print(chrom, startPos, endPos, read + ";" + flags, score, tags, startPos, endPos, negativeTxn, blocks,
+            print(chrom, startPos, endPos, read, score, tags, startPos, endPos, negativeTxn, blocks,
                 ",".join(str(x) for x in sizes) + ",", ",".join(str(x) for x in starts) + ",", sep="\t")
 
         else:
             tags = "+" if flags == "0" else "-"
-            print(chrom, startPos, endPos, read + ";" + flags, score, tags, startPos, endPos, unknownTxn, blocks,
+            print(chrom, startPos, endPos, read, score, tags, startPos, endPos, unknownTxn, blocks,
             ",".join(str(x) for x in sizes) + ",", ",".join(str(x) for x in starts) + ",", sep="\t")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `flair-brookslab-1.7.0/bin/normalize_counts_matrix` & `flair-brookslab-2.0.0/bin/normalize_counts_matrix`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/bin/mark_productivity` & `flair-brookslab-2.0.0/bin/mark_productivity`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/bin/bed_to_psl` & `flair-brookslab-2.0.0/bin/bed_to_psl`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/bin/junctions_from_sam` & `flair-brookslab-2.0.0/bin/junctions_from_sam`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/bin/diffsplice_fishers_exact` & `flair-brookslab-2.0.0/bin/diffsplice_fishers_exact`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/bin/fasta_seq_lengths` & `flair-brookslab-2.0.0/bin/fasta_seq_lengths`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/bin/mark_intron_retention` & `flair-brookslab-2.0.0/bin/mark_intron_retention`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/bin/diff_iso_usage` & `flair-brookslab-2.0.0/bin/diff_iso_usage`

 * *Files 1% similar despite different names*

```diff
@@ -52,15 +52,15 @@
 
 
 counts = {}
 for line in counts_matrix:
 	line = line.rstrip().split('\t')
 	iso_gene, count1, count2 = line[0], float(line[col1]), float(line[col2])
 	if '_' not in iso_gene:
-		sys.stderr.write('Please run bin/identify_annotated_gene.py first so that isoforms\
+		sys.stderr.write('Please run identify_annotated_gene first so that isoforms\
 			can be grouped by their parent genes\n')
 		sys.exit(1)
 	iso, gene = split_iso_gene(iso_gene)
 	if gene not in counts:
 		counts[gene] = {}
 	counts[gene][iso] = [count1, count2]
```

### Comparing `flair-brookslab-1.7.0/bin/predictProductivity` & `flair-brookslab-2.0.0/bin/predictProductivity`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,17 @@
             chrom, c1, c2, strand = cols[0], int(cols[3])-1, int(cols[4]), cols[6]
             if cols[2] == "start_codon":
                 gene = cols[8][cols[8].find('gene_id')+len('gene_id')+2:]
                 gene = gene[:gene.find('"')]
                 # gene = re.search("(ENSG[^\.]+)", cols[-1]).group(1)
 
                 starts.append((chrom,c1,c2,gene,".",strand))
+    if (len(starts)) == 0:
+        sys.stderr.write('ERROR, no start codons were found in', gtf)
+        sys.exit(1)
     return starts
 
 
 def split_iso_gene(iso_gene):
     if '_chr' in iso_gene:
         splitchar = '_chr'
     elif '_XM' in iso_gene:
```

### Comparing `flair-brookslab-1.7.0/LICENSE.txt` & `flair-brookslab-2.0.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/setup.cfg` & `flair-brookslab-2.0.0/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = flair-brookslab
-version = 1.7.0
+version = 2.0.0
 author = Jeltje van Baren
 author_email = jeltje.van.baren@gmail.com
 description = flair
 long_description = file: README.md, LICENSE.txt
 long_description_content_type = text/markdown
 url = https://github.com/BrooksLabUCSC/flair
 project_urls = 
@@ -25,27 +25,32 @@
 	tqdm
 	ncls
 	pybedtools
 	mappy==2.24
 	pysam
 	scipy
 scripts = 
+	bin/assign_variants_to_transcripts
 	bin/junctions_from_sam
 	bin/mark_intron_retention
 	bin/mark_productivity
 	bin/normalize_counts_matrix
 	bin/bam2Bed12
 	bin/bed_to_psl
 	bin/diff_iso_usage
 	bin/diffsplice_fishers_exact
 	bin/plot_isoform_usage
 	bin/predictProductivity
 	bin/psl_to_bed
 	bin/sam_to_map
 	bin/fasta_seq_lengths
+	bin/gtf_to_bed
+	bin/bed_to_sequence
+	bin/identify_annotated_gene
+	bin/identify_gene_isoform
 
 [options.packages.find]
 where = src
 
 [options.entry_points]
 console_scripts = 
 	flair = flair.flair:main
```

### Comparing `flair-brookslab-1.7.0/README.md` & `flair-brookslab-2.0.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # flair
-FLAIR (Full-Length Alternative Isoform analysis of RNA) for the correction, isoform definition, and alternative splicing analysis of noisy reads. FLAIR has primarily been used for nanopore cDNA, native RNA, and PacBio sequencing reads. 
+FLAIR (Full-Length Alternative Isoform analysis of RNA) for the correction, isoform definition, and alternative splicing analysis of noisy reads. FLAIR has primarily been used for nanopore cDNA, native RNA, and PacBio sequencing reads.
 
 The complete Flair manual is available via [readthedocs](https://flair.readthedocs.io/en/latest/)
 
 ## Cite FLAIR <a name="cite"></a>
 If you use or discuss FLAIR, please cite the following [paper](https://www.nature.com/articles/s41467-020-15171-6):
 >Tang, A.D., Soulette, C.M., van Baren, M.J. et al. Full-length transcript characterization of SF3B1 mutation in chronic lymphocytic leukemia reveals downregulation of retained introns. Nat Commun 11, 1438 (2020). https://doi.org/10.1038/s41467-020-15171-6
```

### Comparing `flair-brookslab-1.7.0/src/flair/runDU.py` & `flair-brookslab-2.0.0/src/flair/runDU.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/es_as_inc_excl_to_counts.py` & `flair-brookslab-2.0.0/src/flair/es_as_inc_excl_to_counts.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/bed_to_sequence.py` & `flair-brookslab-2.0.0/bin/bed_to_sequence`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 #!/usr/bin/env python3
-import sys
-import csv
-import os
-import argparse
-import pysam
-import subprocess
+import sys, csv, os, argparse, pysam, subprocess
+from collections import namedtuple
+
 # from filter_collapsed_isoforms_from_annotation import split_iso_gene
 
 parser = argparse.ArgumentParser(description='options',
-	usage='bed_to_sequence.py psl|bed genome.fa outfilename [options]')
+	usage='python script.py psl|bed genome.fa outfilename [options]')
 parser.add_argument('psl', type=str,
 	action='store', help='isoforms in psl or bed format')
 parser.add_argument('genome', type=str,
 	action='store', help='genomic sequence')
 parser.add_argument('outfilename', type=str,
 	action='store', help='Name of output file')
+parser.add_argument('-v', '--vcf', action='store', dest='vcf',
+	type=str, help='vcf file with flair phased transcripts')
+# longshot phased arguments
 parser.add_argument('--isoform_haplotypes', action='store', dest='isoform_haplotypes',
 	type=str, help='isoform haplotype assignments')
-parser.add_argument('-v', '--vcf', action='store', dest='vcf',
-	type=str, help='vcf file')
 parser.add_argument('--vcf_out', action='store', dest='vcf_out', default='',
 	type=str, help='vcf output file name')
 parser.add_argument('--models_out', action='store', dest='models_out', default='', type=str,
 	help='isoform psl/bed out, will contain additional isoforms created from unphased variants')
 args = parser.parse_args()
 
 fastq = args.outfilename[-2:].lower() in ['fq', 'fastq']
@@ -96,129 +94,134 @@
 		blockstarts = [int(n) + start for n in entry[11].split(',')[:-1]]
 		blocksizes = [int(n) for n in entry[10].split(',')[:-1]]
 		strand = entry[5]
 	else:
 		blocksizes = [int(n) for n in entry[18].split(',')[:-1]]
 		blockstarts = [int(n) for n in entry[20].split(',')[:-1]]
 		strand = entry[8]
-	pulledseq = ''
+	pulled_seq = ''
 	for block in range(len(blockstarts)):
-		pulledseq += seq[blockstarts[block]:blockstarts[block]+blocksizes[block]]
+		pulled_seq += seq[blockstarts[block]:blockstarts[block]+blocksizes[block]]
 	if strand == '-':
-		pulledseq = revcomp(pulledseq)
-	return pulledseq
-
+		pulled_seq = revcomp(pulled_seq)
+	return pulled_seq
 
-def add_variants_to_seq(variant_list, no_variant_sequence, starts, sizes, iso_name):
+def add_variants_to_seq(variant_list, no_variant_sequence, starts, sizes, strand = '+', chrom='chr1', iso_name=''):
 	pulled_seq = ''
+
 	for block in range(len(starts)):
 		exon_seq = no_variant_sequence[starts[block]:starts[block]+sizes[block]]
-
 		for v in variant_list:
 			if v.pos > starts[block] and v.pos < starts[block]+sizes[block]:
 				if v.ref != exon_seq[v.pos-starts[block]-1]:
-					print('VCF ref {} does not match genome ref base {}'.format(v.ref,
-						exon_seq[v.pos-starts[block] - 2:v.pos-starts[block] + 2]))
+					print('VCF ref {} does not match genome ref base {}, at {}:{}'.format(v.ref, 
+						exon_seq[v.pos-starts[block] - 2:v.pos-starts[block] + 2], v.chrom, v.pos))
 				exon_seq = exon_seq[:v.pos-starts[block]-1] + v.alts[0] + exon_seq[v.pos-starts[block]:]
 
-				vstring = str(v)
-				if vstring not in variant_string_to_record:
-					variant_string_to_record[vstring] = v
+				if args.isoform_haplotypes:
+					vstring = str(v)
+					if vstring not in variant_string_to_record:
+						variant_string_to_record[vstring] = v
+
+
+						used_variants[vstring] = set()
 
-					used_variants[vstring] = set()
+					used_variants[vstring].add(iso_name)
 
-				used_variants[vstring].add(iso_name)
 		pulled_seq += exon_seq
+
 	return pulled_seq
 
 
-def get_sequence_with_variants(entry, seq, name):
+def get_sequence_with_variants(entry, seq):
+	''' Entry is the isoform model line, seq is the genomic sequence for this chromosome'''
 	if isbed:
 		start = int(entry[1])
 		blockstarts = [int(n) + start for n in entry[11].split(',')[:-1]]
 		blocksizes = [int(n) for n in entry[10].split(',')[:-1]]
 		strand = entry[5]
 		name = entry[3]
 	else:
 		blocksizes = [int(n) for n in entry[18].split(',')[:-1]]
 		blockstarts = [int(n) for n in entry[20].split(',')[:-1]]
 		strand = entry[8]
 		name = entry[9]
 
-	if chrom not in vcf.header.contigs:
-		variants = []
-	else:
-		variants = vcf.fetch(chrom, blockstarts[0], blockstarts[-1]+blocksizes[-1],reopen=True)
 
 	# get variants for this haplotype
-	v_to_add = []
-	v_to_add_alt = []
-	for v in variants:
-		sample_name = list(v.samples)[0]
-		variant_ps = v.samples[sample_name]['PS']
-		variant_gt = v.samples[sample_name]['GT']
-		variant_ac = v.info['AC']
-		if variant_gt == (1,1):
-			v_to_add += [v]
-			v_to_add_alt += [v]
+	if not args.isoform_haplotypes:
+		if name not in iso_to_variants:
+			return get_sequence(entry, seq)
+		v_to_add = iso_to_variants[name]
+		v_to_add.reverse()
+	else:
+		if chrom not in vcf.header.contigs:
+			variants = []
+		else:
+			variants = vcf.fetch(chrom, blockstarts[0], blockstarts[-1]+blocksizes[-1],reopen=True)
+		v_to_add = []
+		v_to_add_alt = []
+		for v in variants:
+			sample_name = list(v.samples)[0]
+			variant_ps = v.samples[sample_name]['PS']
+			variant_gt = v.samples[sample_name]['GT']
+			variant_ac = v.info['AC']
+			if variant_gt == (1,1):
+				v_to_add += [v]
+				v_to_add_alt += [v]
 
-		elif args.models_out and variant_gt == (0,1) and not variant_ps and \
+			elif args.models_out and variant_gt == (0,1) and not variant_ps and \
 			variant_ac[0] > unphased_variant_support and variant_ac[1] > unphased_variant_support:
 				print(entry[0], v.pos, variant_ps, variant_ac)
 				v_to_add_alt += [v]
 
-		elif name not in haplotype or variant_ps not in haplotype[name]:
+			elif name not in haplotype or variant_ps not in haplotype[name]:
 
-			continue
+				continue
+			else:
+				v_to_add += [v]
+				v_to_add_alt += [v]
+		v_to_add.reverse()  # add variants starting from the end in case of indels 
+		v_to_add_alt.reverse()
+
+		if len(v_to_add_alt) != len(v_to_add):
+			iso, gene = split_iso_gene(name)
+			name_ref, name_alt = '>' + iso+':0_'+gene, '>' + iso+':1_'+gene
 		else:
-			v_to_add += [v]
-			v_to_add_alt += [v]
-	v_to_add.reverse()  # add variants starting at the downstream coordinate
-	v_to_add_alt.reverse()
-
-	if len(v_to_add_alt) != len(v_to_add):
-		iso, gene = split_iso_gene(name)
-		name_ref, name_alt = '>' + iso+':0_'+gene, '>' + iso+':1_'+gene
+			name_ref = name
+	if not args.isoform_haplotypes:
+		pulled_seq = add_variants_to_seq(v_to_add, seq, blockstarts, blocksizes, strand, entry[0])#, name_ref)
 	else:
-		name_ref = name
-	pulled_seq = add_variants_to_seq(v_to_add, seq, blockstarts, blocksizes, name_ref)
+		pulled_seq = add_variants_to_seq(v_to_add, seq, blockstarts, blocksizes, strand, entry[0], iso_name=name_ref)
 
-	if strand == '-':
-		pulled_seq = revcomp(pulled_seq)
-	if not args.models_out or len(v_to_add_alt) == len(v_to_add):
-		return [pulled_seq]
 
-	alt_seq = add_variants_to_seq(v_to_add_alt, seq, blockstarts, blocksizes, name_alt)
 	if strand == '-':
-		alt_seq = revcomp(alt_seq)
-	return name_ref, pulled_seq, name_alt, alt_seq
+		pulled_seq = revcomp(pulled_seq)
+	if args.isoform_haplotypes:
+		if not args.models_out or len(v_to_add_alt) == len(v_to_add):
+			return pulled_seq
+
+		alt_seq = add_variants_to_seq(v_to_add_alt, seq, blockstarts, blocksizes, iso_name=name_alt)
+		if strand == '-':
+			alt_seq = revcomp(alt_seq)
+		return name_ref, pulled_seq, name_alt, alt_seq
+	else:
+		return pulled_seq
 
 
 def write_sequences(chrom):
 
 	models = []
 	for entry in psldata[chrom]:
 
 		name = entry[3] if isbed else entry[9]
 		if args.vcf:
 			pulled_seqs = get_sequence_with_variants(entry, seq, name)
-			if len(pulled_seqs) > 1:
-				writer.writerow(['>' + pulled_seqs[0]])
-				writer.writerow([pulled_seqs[1]])
-				entry[3] = pulled_seqs[0]
-				entry_ref = tuple(entry)
-				writer.writerow(['>' + pulled_seqs[2]])
-				writer.writerow([pulled_seqs[3]])
-				entry[3] = pulled_seqs[2]
-				entry_alt = tuple(entry)
-				models += [entry_ref, entry_alt]
-			else:
-				writer.writerow(['>' + name])
-				writer.writerow([pulled_seqs[0]])
-				models += [entry]
+			writer.writerow(['>' + name])
+			writer.writerow([pulled_seq])
 
 		else:
 			if fastq:
 				writer.writerow(['@' + name])
 			else:
 				writer.writerow(['>' + name])
 			pulled_seq = get_sequence(entry, seq)
@@ -250,33 +253,33 @@
 	for line in open(args.genome):
 		line = line.rstrip()
 		if line.startswith('>'):
 			if not chrom:
 				chrom = line.split()[0][1:]
 				continue
 			if chrom in psldata:  # or bed
-				models_to_write += write_sequences(chrom)
+				write_sequences(chrom)
 
 			chrom = line.split()[0][1:]
 			ignore = chrom not in psldata
 			seq = ''
 		elif not ignore:
 			seq += line.upper()
 
 	if chrom in psldata:  # last chromosome
-		models_to_write += write_sequences(chrom)
+		write_sequences(chrom)
 
 
 if args.models_out:
 	with open(args.models_out, 'wt') as outfile:
 		writer = csv.writer(outfile, delimiter='\t', lineterminator=os.linesep)
 		for entry in models_to_write:
 			writer.writerow(entry)
 
-if args.vcf:
+if args.vcf and args.isoform_haplotypes:
 	header = vcf.header
 	header.add_meta('FORMAT', items=[('ID',"ISO"), ('Number',1), ('Type','String'),
 		('Description','Isoforms')])
 	if not args.vcf_out:
 		args.vcf_out = args.vcf[:-3]+'used_variants.vcf'
 	vcf_outfile = pysam.VariantFile(args.vcf_out, 'w', header=vcf.header)
 	for v in used_variants:
```

### Comparing `flair-brookslab-1.7.0/src/flair/match_counts.py` & `flair-brookslab-2.0.0/src/flair/match_counts.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/flair.py` & `flair-brookslab-2.0.0/src/flair/flair.py`

 * *Files 1% similar despite different names*

```diff
@@ -362,17 +362,14 @@
 	# other
 	parser.add_argument('--temp_dir', default='', action='store', dest='temp_dir',
 		help='directory for temporary files. use "./" to indicate current directory (default: python tempfile directory)')
 	parser.add_argument('--keep_intermediate', default=False, action='store_true', dest='keep_intermediate',
 		help='''specify if intermediate and temporary files are to be kept for debugging.
 		Intermediate files include: promoter-supported reads file,
 		read assignments to firstpass isoforms''')
-	parser.add_argument('--fusion_dist', default=0, type=int, action='store', dest='fusion_dist',
-			help='''minimium distance between separate read alignments on the same chromosome to be
-			considered a fusion, otherwise no reads will be assumed to be fusions''')
 	parser.add_argument('--mm2_args', action='store', dest='mm2_args',
 		type=str, default=[], help='''additional minimap2 arguments when aligning reads first-pass transcripts;
 		separate args by commas, e.g. --mm2_args=-I8g,--MD ''')
 	parser.add_argument('--quiet', default=False, action='store_true', dest='quiet',
 			help='''Suppress progress statements from being printed''')
 	parser.add_argument('--annotated_bed', default=False, action='store', dest='annotated_bed',
 		help='''annotation_reliant also requires a bedfile of annotated isoforms; if this isn't provided,
@@ -408,16 +405,14 @@
 		args.o = args.temp_dir+run_id
 		args.q = args.temp_dir+run_id+'.sorted.bed.gz'
 		args.quiet = True
 
 	args.quality = '0' if args.trust_ends else args.quality
 	args.o += '.'
 	min_reads = float(args.s) if float(args.s) >= 1 else 3
-	if args.fusion_dist:
-		args.trust_ends = True
 
 	if ',' in args.r[0]:
 		args.r = args.r[0].split(',')
 	for rfile in args.r:
 		if not os.path.exists(rfile):
 			sys.stderr.write(f'Read file path does not exist: {rfile}\n')
 			return 1
@@ -576,15 +571,15 @@
 		collapse_cmd += ['-i']
 	if args.quiet:
 		collapse_cmd += ['--quiet']
 
 	if subprocess.call(collapse_cmd):
 		return 1
 
-	# filtering out subset isoforms with insuficient support
+	# filtering out subset isoforms with insufficient support
 	filter_cmd = [sys.executable, path+'filter_collapsed_isoforms.py',
 		args.o+'firstpass.unfiltered.bed', args.filter, args.o+'firstpass.bed', str(args.w)]
 	if float(args.s) < 1:
 		filter_cmd += ['keep']
 
 	if subprocess.call(filter_cmd):
 		return 1
@@ -631,16 +626,14 @@
 		count_cmd += ['--check_splice']
 	if args.check_splice or args.stringent:
 		count_cmd += ['-i', args.o+'firstpass.bed']
 	if args.trust_ends:
 		count_cmd += ['--trust_ends']
 	if args.generate_map:
 		count_cmd += ['--generate_map', args.o+'isoform.read.map.txt']
-	if args.fusion_dist:
-		count_cmd += ['--fusion_dist', str(args.fusion_dist)]
 	if subprocess.call(count_cmd, stdin=ps.stdout):
 		sys.stderr.write('Failed at counting step for isoform read support\n')
 		return 1
 
 	if not args.quiet:
 		sys.stderr.write('Filtering isoforms by read coverage\n')
 	match_count_cmd = [sys.executable, path+'match_counts.py', count_file,
@@ -1093,12 +1086,12 @@
 			sys.exit(1)
 		else:
 			status = diffSplice()
 		if status == 1:
 			sys.exit(1)
 
 	if mode == '--version':
-		sys.stderr.write('FLAIR v1.7.0\n')
+		sys.stderr.write('FLAIR v2.0.0\n')
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `flair-brookslab-1.7.0/src/flair/filter_collapsed_isoforms.py` & `flair-brookslab-2.0.0/src/flair/filter_collapsed_isoforms.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/counts_to_tpm.py` & `flair-brookslab-2.0.0/src/flair/counts_to_tpm.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/pull_starts.py` & `flair-brookslab-2.0.0/src/flair/pull_starts.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/bed_to_gtf.py` & `flair-brookslab-2.0.0/src/flair/bed_to_gtf.py`

 * *Files 1% similar despite different names*

```diff
@@ -51,15 +51,15 @@
 		chrom, strand, score, name, start = line[13], line[8], line[0], line[9], int(line[15])
 		tstarts = [int(n) for n in line[20].split(',')[:-1]]  # target starts
 		bsizes = [int(n) for n in line[18].split(',')[:-1]]  # block sizes
 
 	if '_' not in name and not args.force:
 		sys.stderr.write('Entry name should contain underscore-delimited transcriptid and geneid like so:\
 		 ENST00000318842.11_ENSG00000156313.12 or a4bab8a3-1d28_chr8:232000\n')
-		sys.stderr.write('So no GTF conversion was done. Please run bin/identify_gene_isoform.py first\n')
+		sys.stderr.write('So no GTF conversion was done. Please run identify_gene_isoform first\n')
 		sys.stderr.write('for best results, or run with --force\n')
 		sys.exit(1)
 
 	if ';' in name:
 		name = name.replace(';', ':')
 
 	if args.force:
```

### Comparing `flair-brookslab-1.7.0/src/flair/consolidate_isoforms.py` & `flair-brookslab-2.0.0/src/flair/consolidate_isoforms.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/ssPrep.py` & `flair-brookslab-2.0.0/src/flair/ssPrep.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/identify_annotated_gene.py` & `flair-brookslab-2.0.0/bin/identify_annotated_gene`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/bam2Bed12.py` & `flair-brookslab-2.0.0/src/flair/bam2Bed12.py`

 * *Files 3% similar despite different names*

```diff
@@ -125,21 +125,21 @@
     for num, readData in enumerate(sObj.readJuncs(),0):
         read, chrom, startPos, junctions, endPos, flags, tags, score = readData
         blocks, sizes, starts = juncsToBed12(startPos, endPos, junctions)
         flags = str(flags)
 
         if tags == "+":
 
-            print(chrom, startPos, endPos, read + ";" + flags, score, tags, startPos, endPos, positiveTxn, blocks,
+            print(chrom, startPos, endPos, read, score, tags, startPos, endPos, positiveTxn, blocks,
                 ",".join(str(x) for x in sizes) + ",", ",".join(str(x) for x in starts) + ",", sep="\t")
         elif tags == "-":
-            print(chrom, startPos, endPos, read + ";" + flags, score, tags, startPos, endPos, negativeTxn, blocks,
+            print(chrom, startPos, endPos, read, score, tags, startPos, endPos, negativeTxn, blocks,
                 ",".join(str(x) for x in sizes) + ",", ",".join(str(x) for x in starts) + ",", sep="\t")
 
         else:
             tags = "+" if flags == "0" else "-"
-            print(chrom, startPos, endPos, read + ";" + flags, score, tags, startPos, endPos, unknownTxn, blocks,
+            print(chrom, startPos, endPos, read, score, tags, startPos, endPos, unknownTxn, blocks,
             ",".join(str(x) for x in sizes) + ",", ",".join(str(x) for x in starts) + ",", sep="\t")
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `flair-brookslab-1.7.0/src/flair/collapse_isoforms_precise.py` & `flair-brookslab-2.0.0/src/flair/collapse_isoforms_precise.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/filter_collapsed_isoforms_from_annotation.py` & `flair-brookslab-2.0.0/src/flair/filter_collapsed_isoforms_from_annotation.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/deFLAIR.py` & `flair-brookslab-2.0.0/src/flair/deFLAIR.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/runDS.py` & `flair-brookslab-2.0.0/src/flair/runDS.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/get_phase_sets.py` & `flair-brookslab-2.0.0/src/flair/get_phase_sets.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/samJuncs.py` & `flair-brookslab-2.0.0/src/flair/samJuncs.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/runDE.py` & `flair-brookslab-2.0.0/src/flair/runDE.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/ssCorrect.py` & `flair-brookslab-2.0.0/src/flair/ssCorrect.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/subset_unassigned_reads.py` & `flair-brookslab-2.0.0/src/flair/subset_unassigned_reads.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 headers_keep = set()
 isbed = sys.argv[2][-3:].lower() != 'psl'
 with open(sys.argv[4], 'wt') as outfile:
     writer = csv.writer(outfile, delimiter='\t', lineterminator=os.linesep)
     for line in open(sys.argv[2]):  # bed
         line = line.rstrip().split('\t')
         if isbed:
-            name = line[3][:line[3].rfind(';')]
+            name = line[3]
         else:
-            name = line[9][:line[9].rfind(';')]
+            name = line[9]
 
         if name not in assigned_names:
             writer.writerow(line)
             headers_keep.add(name)
 
 headers_used = set()
 for fle in sys.argv[5:]:
```

### Comparing `flair-brookslab-1.7.0/src/flair/es_as.py` & `flair-brookslab-2.0.0/src/flair/es_as.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/identify_gene_isoform.py` & `flair-brookslab-2.0.0/bin/identify_gene_isoform`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/select_from_bed.py` & `flair-brookslab-2.0.0/src/flair/select_from_bed.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/filter_isoforms_by_proportion_of_gene_expr.py` & `flair-brookslab-2.0.0/src/flair/filter_isoforms_by_proportion_of_gene_expr.py`

 * *Files 5% similar despite different names*

```diff
@@ -46,19 +46,18 @@
 		name = line[3]
 	else:
 		name = line[9]
 	iso, gene = split_iso_gene(name)
 	if gene not in genes:
 		genes[gene] = set()
 	genes[gene].add(tuple(line))
-	# print(tuple(line))
 
 with open(outfilename, 'wt') as outfile:
 	writer = csv.writer(outfile, delimiter='\t', lineterminator=os.linesep)
 	for gene in genes:
-		gene_total = float(sum([float(iso[0][-1]) for iso in genes[gene]]))
+		gene_total = float(sum([float(iso[-1]) for iso in genes[gene]]))
 		if gene_total == 0:
 			continue
 		for iso in genes[gene]:
 			if float(iso[0][-1])/gene_total >= s:
 				writer.writerow(iso)
```

### Comparing `flair-brookslab-1.7.0/src/flair/call_diffsplice_events.py` & `flair-brookslab-2.0.0/src/flair/call_diffsplice_events.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/count_sam_transcripts.py` & `flair-brookslab-2.0.0/src/flair/count_sam_transcripts.py`

 * *Files identical despite different names*

### Comparing `flair-brookslab-1.7.0/src/flair/gtf_to_bed.py` & `flair-brookslab-2.0.0/bin/gtf_to_bed`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import sys
 import csv
 import os
 import argparse
 
 parser = argparse.ArgumentParser(description='''converts a gtf to a bed or psl, depending on the output filename extension;
 	gtf exons need to be grouped by transcript and sorted by coordinate w/in a transcript''',
-	usage='gtf_to_psl.py in.gtf out.psl|bed [options]')
+	usage='gtf_to_bed in.gtf out.psl|bed [options]')
 required = parser.add_argument_group('required named arguments')
 required.add_argument('gtf', action='store',
 	type=str, help='annotated gtf')
 required.add_argument('psl', action='store',
 	type=str, help='psl or bed file')
 parser.add_argument('--include_gene', action='store_true', dest='include_gene',
 	required=False, help='''Include gene name in the isoform name''')
```

### Comparing `flair-brookslab-1.7.0/src/flair_brookslab.egg-info/SOURCES.txt` & `flair-brookslab-2.0.0/src/flair_brookslab.egg-info/SOURCES.txt`

 * *Files 26% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 LICENSE.txt
 README.md
 pyproject.toml
 setup.cfg
+bin/assign_variants_to_transcripts
 bin/bam2Bed12
 bin/bed_to_psl
+bin/bed_to_sequence
 bin/diff_iso_usage
 bin/diffsplice_fishers_exact
 bin/fasta_seq_lengths
+bin/gtf_to_bed
+bin/identify_annotated_gene
+bin/identify_gene_isoform
 bin/junctions_from_sam
 bin/mark_intron_retention
 bin/mark_productivity
 bin/normalize_counts_matrix
 bin/plot_isoform_usage
 bin/predictProductivity
 bin/psl_to_bed
@@ -29,15 +34,14 @@
 src/flair/es_as_inc_excl_to_counts.py
 src/flair/filter_collapsed_isoforms.py
 src/flair/filter_collapsed_isoforms_from_annotation.py
 src/flair/filter_isoforms_by_proportion_of_gene_expr.py
 src/flair/flair.py
 src/flair/get_phase_sets.py
 src/flair/gtf_to_bed.py
-src/flair/identify_annotated_gene.py
 src/flair/identify_gene_isoform.py
 src/flair/match_counts.py
 src/flair/pull_starts.py
 src/flair/runDE.py
 src/flair/runDS.py
 src/flair/runDU.py
 src/flair/samJuncs.py
```

### Comparing `flair-brookslab-1.7.0/src/flair_brookslab.egg-info/PKG-INFO` & `flair-brookslab-2.0.0/src/flair_brookslab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flair-brookslab
-Version: 1.7.0
+Version: 2.0.0
 Summary: flair
 Home-page: https://github.com/BrooksLabUCSC/flair
 Author: Jeltje van Baren
 Author-email: jeltje.van.baren@gmail.com
 License: UNKNOWN
 Project-URL: Bug Tracker, https://github.com/BrooksLabUCSC/flair/issues
 Project-URL: repository, https://github.com/BrooksLabUCSC/flair
@@ -13,15 +13,15 @@
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # flair
-FLAIR (Full-Length Alternative Isoform analysis of RNA) for the correction, isoform definition, and alternative splicing analysis of noisy reads. FLAIR has primarily been used for nanopore cDNA, native RNA, and PacBio sequencing reads. 
+FLAIR (Full-Length Alternative Isoform analysis of RNA) for the correction, isoform definition, and alternative splicing analysis of noisy reads. FLAIR has primarily been used for nanopore cDNA, native RNA, and PacBio sequencing reads.
 
 The complete Flair manual is available via [readthedocs](https://flair.readthedocs.io/en/latest/)
 
 ## Cite FLAIR <a name="cite"></a>
 If you use or discuss FLAIR, please cite the following [paper](https://www.nature.com/articles/s41467-020-15171-6):
 >Tang, A.D., Soulette, C.M., van Baren, M.J. et al. Full-length transcript characterization of SF3B1 mutation in chronic lymphocytic leukemia reveals downregulation of retained introns. Nat Commun 11, 1438 (2020). https://doi.org/10.1038/s41467-020-15171-6
```

