# Comparing `tmp/cami-opal-1.0.8.post0.tar.gz` & `tmp/cami-opal-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cami-opal-1.0.8.post0.tar", last modified: Mon Aug 10 09:28:22 2020, max compression
+gzip compressed data, was "dist/cami-opal-1.0.9.tar", last modified: Mon Feb  1 12:36:41 2021, max compression
```

## Comparing `cami-opal-1.0.8.post0.tar` & `cami-opal-1.0.9.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2020-08-10 09:28:22.000000 cami-opal-1.0.8.post0/
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    11357 2020-06-23 16:04:33.000000 cami-opal-1.0.8.post0/LICENSE
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       39 2020-08-10 09:15:55.000000 cami-opal-1.0.8.post0/MANIFEST.in
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      546 2020-08-10 09:28:22.000000 cami-opal-1.0.8.post0/PKG-INFO
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    10361 2020-06-26 13:00:15.000000 cami-opal-1.0.8.post0/README.md
-drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2020-08-10 09:28:22.000000 cami-opal-1.0.8.post0/cami_opal.egg-info/
--rwxrwxrwx   0 fmeyer    (1000) fmeyer    (1000)      546 2020-08-10 09:28:22.000000 cami-opal-1.0.8.post0/cami_opal.egg-info/PKG-INFO
--rwxrwxrwx   0 fmeyer    (1000) fmeyer    (1000)      642 2020-08-10 09:28:22.000000 cami-opal-1.0.8.post0/cami_opal.egg-info/SOURCES.txt
--rwxrwxrwx   0 fmeyer    (1000) fmeyer    (1000)        1 2020-08-10 09:28:22.000000 cami-opal-1.0.8.post0/cami_opal.egg-info/dependency_links.txt
--rwxrwxrwx   0 fmeyer    (1000) fmeyer    (1000)      136 2020-08-10 09:28:22.000000 cami-opal-1.0.8.post0/cami_opal.egg-info/requires.txt
--rwxrwxrwx   0 fmeyer    (1000) fmeyer    (1000)        4 2020-08-10 09:28:22.000000 cami-opal-1.0.8.post0/cami_opal.egg-info/top_level.txt
--rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)    18923 2020-07-26 10:34:17.000000 cami-opal-1.0.8.post0/opal.py
--rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)     3737 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/opal_stats.py
--rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)     6724 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/opal_workflow.py
-drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2020-08-10 09:28:22.000000 cami-opal-1.0.8.post0/requirements/
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      136 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/requirements/default.txt
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       50 2020-06-23 19:40:57.000000 cami-opal-1.0.8.post0/requirements/development.txt
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       71 2020-08-10 09:28:22.000000 cami-opal-1.0.8.post0/setup.cfg
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     1063 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/setup.py
-drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2020-08-10 09:28:22.000000 cami-opal-1.0.8.post0/src/
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)        0 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/src/__init__.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    10103 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/src/binary_metrics.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      836 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/src/braycurtis.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    32859 2020-06-28 08:14:14.000000 cami-opal-1.0.8.post0/src/html_opal.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     2620 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/src/l1norm.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    31880 2020-08-10 09:27:41.000000 cami-opal-1.0.8.post0/src/plots.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     3213 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/src/rankings.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     1781 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/src/shannon.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     2458 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/src/tsv2biom.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     2954 2020-07-26 10:34:17.000000 cami-opal-1.0.8.post0/src/unifrac_distance.py
-drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2020-08-10 09:28:22.000000 cami-opal-1.0.8.post0/src/utils/
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     2251 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/src/utils/EMDUnifrac.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    23525 2020-07-26 10:34:17.000000 cami-opal-1.0.8.post0/src/utils/ProfilingTools.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)        0 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/src/utils/__init__.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     3274 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/src/utils/constants.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     8665 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/src/utils/load_data.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     3333 2020-06-26 13:00:16.000000 cami-opal-1.0.8.post0/src/utils/spider_plot_functions.py
--rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       28 2020-08-10 09:19:02.000000 cami-opal-1.0.8.post0/version.py
+drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2021-02-01 12:36:41.000000 cami-opal-1.0.9/
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    11357 2021-02-01 12:34:57.000000 cami-opal-1.0.9/LICENSE
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       39 2021-02-01 12:34:57.000000 cami-opal-1.0.9/MANIFEST.in
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      540 2021-02-01 12:36:41.000000 cami-opal-1.0.9/PKG-INFO
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    10673 2021-02-01 12:34:57.000000 cami-opal-1.0.9/README.md
+drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2021-02-01 12:36:41.000000 cami-opal-1.0.9/cami_opal.egg-info/
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      540 2021-02-01 12:36:41.000000 cami-opal-1.0.9/cami_opal.egg-info/PKG-INFO
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      642 2021-02-01 12:36:41.000000 cami-opal-1.0.9/cami_opal.egg-info/SOURCES.txt
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)        1 2021-02-01 12:36:41.000000 cami-opal-1.0.9/cami_opal.egg-info/dependency_links.txt
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      136 2021-02-01 12:36:41.000000 cami-opal-1.0.9/cami_opal.egg-info/requires.txt
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)        4 2021-02-01 12:36:41.000000 cami-opal-1.0.9/cami_opal.egg-info/top_level.txt
+-rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)    18842 2021-02-01 12:34:58.000000 cami-opal-1.0.9/opal.py
+-rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)     3737 2021-02-01 12:34:58.000000 cami-opal-1.0.9/opal_stats.py
+-rwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)     6724 2021-02-01 12:34:58.000000 cami-opal-1.0.9/opal_workflow.py
+drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2021-02-01 12:36:41.000000 cami-opal-1.0.9/requirements/
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      136 2021-02-01 12:34:58.000000 cami-opal-1.0.9/requirements/default.txt
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       50 2021-02-01 12:34:58.000000 cami-opal-1.0.9/requirements/development.txt
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       71 2021-02-01 12:36:41.000000 cami-opal-1.0.9/setup.cfg
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     1063 2021-02-01 12:34:58.000000 cami-opal-1.0.9/setup.py
+drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2021-02-01 12:36:41.000000 cami-opal-1.0.9/src/
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)        0 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/__init__.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    10103 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/binary_metrics.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)      836 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/braycurtis.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    32238 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/html_opal.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     2620 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/l1norm.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    32040 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/plots.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     3213 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/rankings.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     1781 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/shannon.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     2458 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/tsv2biom.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     2954 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/unifrac_distance.py
+drwxrwxr-x   0 fmeyer    (1000) fmeyer    (1000)        0 2021-02-01 12:36:41.000000 cami-opal-1.0.9/src/utils/
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     2251 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/utils/EMDUnifrac.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)    23525 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/utils/ProfilingTools.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)        0 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/utils/__init__.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     3274 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/utils/constants.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     8665 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/utils/load_data.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)     3333 2021-02-01 12:34:58.000000 cami-opal-1.0.9/src/utils/spider_plot_functions.py
+-rw-rw-r--   0 fmeyer    (1000) fmeyer    (1000)       22 2021-02-01 12:34:58.000000 cami-opal-1.0.9/version.py
```

### Comparing `cami-opal-1.0.8.post0/LICENSE` & `cami-opal-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/PKG-INFO` & `cami-opal-1.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cami-opal
-Version: 1.0.8.post0
+Version: 1.0.9
 Summary: OPAL: Open-community Profiling Assessment tooL
 Home-page: http://cami-challenge.org
 Author: CAMI
 Author-email: support@cami-challenge.org
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `cami-opal-1.0.8.post0/README.md` & `cami-opal-1.0.9/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 * Shannon diversity and equitability indices
 * Bray–Curtis distance
 
 **Example pages produced by OPAL**
 * [CAMI I high complexity challenge dataset](https://cami-challenge.github.io/OPAL/cami_i_hc/)
 * [CAMI II mouse gut toy dataset](https://cami-challenge.github.io/OPAL/cami_ii_mg/)
 * [CAMI II mouse gut toy dataset (using parameter --filter 1)](https://cami-challenge.github.io/OPAL/cami_ii_mg_filter1/)
-* [CAMI II mouse gut toy dataset (using parameters --filter 1 --no_normalization)](https://cami-challenge.github.io/OPAL/cami_ii_mg_filter1_nonormalization/)
+* [CAMI II mouse gut toy dataset (using parameters --filter 1 --normalize)](https://cami-challenge.github.io/OPAL/cami_ii_mg_filter1_normalized)
 * [Human Microbiome Project Mock Community dataset](https://cami-challenge.github.io/OPAL/hmp_mc/)
 
 **See also**
 * [Assessments of profiling submissions to the 1st CAMI Challenge](https://cami-challenge.github.io/OPAL/cami_i_challenge_submissions/)
 
 # User Guide
 
@@ -89,29 +89,29 @@
 * RANK: taxonomic rank
 * TAXPATH and TAXPATHSN: path from the root of the taxonomy to the respective current taxon, including the current taxon, separated by a `|`. TAXPATH and TAXPATHSN contain identifiers and plain names, respectively, of the taxonomies. For more details and examples, see [CAMI profiling Bioboxes format](https://github.com/bioboxes/rfc/tree/master/data-format).
 
 ## Running _opal.py_
 ~~~BASH
 usage: opal.py -g GOLD_STANDARD_FILE -o OUTPUT_DIR [-n] [-f FILTER] [-p]
                [-l LABELS] [-t TIME] [-m MEMORY] [-d DESC] [-r RANKS]
-               [--metrics_plot METRICS_PLOT] [--silent] [-v] [-h]
+               [--metrics_plot_rel METRICS_PLOT_REL]
+               [--metrics_plot_abs METRICS_PLOT_ABS] [--silent] [-v] [-h]
                profiles_files [profiles_files ...]
 
 OPAL: Open-community Profiling Assessment tooL
 
 required arguments:
   profiles_files        Files of profiles
   -g GOLD_STANDARD_FILE, --gold_standard_file GOLD_STANDARD_FILE
                         Gold standard file
   -o OUTPUT_DIR, --output_dir OUTPUT_DIR
                         Directory to write the results to
 
 optional arguments:
-  -n, --no_normalization
-                        Do not normalize samples
+  -n, --normalize       Normalize samples
   -f FILTER, --filter FILTER
                         Filter out the predictions with the smallest relative
                         abundances summing up to [FILTER]% within a rank
                         (affects only precision, default: 0)
   -p, --plot_abundances
                         Plot abundances in the gold standard (can take some
                         minutes)
@@ -122,20 +122,25 @@
                         Comma-separated memory usages in gigabytes
   -d DESC, --desc DESC  Description for HTML page
   -r RANKS, --ranks RANKS
                         Highest and lowest taxonomic ranks to consider in
                         performance rankings, comma-separated. Valid ranks:
                         superkingdom, phylum, class, order, family, genus,
                         species, strain (default:superkingdom,species)
-  --metrics_plot METRICS_PLOT
+  --metrics_plot_rel METRICS_PLOT_REL
                         Metrics for spider plot of relative performances,
                         first character, comma-separated. Valid metrics:
-                        w:weighted Unifrac, l:L1 norm, c:completeness,
-                        p:purity, f:false positives, t:true positives
-                        (default: w,l,c,p,f)
+                        c:completeness, p:purity, l:L1 norm, w:weighted
+                        Unifrac, f:false positives, t:true positives (default:
+                        c,p,l,w)
+  --metrics_plot_abs METRICS_PLOT_ABS
+                        Metrics for spider plot of absolute performances,
+                        first character, comma-separated. Valid metrics:
+                        c:completeness, p:purity, b:Bray-Curtis (default:
+                        c,p,b)
   --silent              Silent mode
   -v, --version         show program's version number and exit
   -h, --help            Show this help message and exit
 ~~~
 **Example:** To run the example, please download the files given in the [_data_](https://github.com/CAMI-challenge/OPAL/tree/master/data) directory.
 ~~~BASH
 python3 opal.py -g data/goldstandard_low_1.bin \
```

### Comparing `cami-opal-1.0.8.post0/cami_opal.egg-info/PKG-INFO` & `cami-opal-1.0.9/cami_opal.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cami-opal
-Version: 1.0.8.post0
+Version: 1.0.9
 Summary: OPAL: Open-community Profiling Assessment tooL
 Home-page: http://cami-challenge.org
 Author: CAMI
 Author-email: support@cami-challenge.org
 License: UNKNOWN
 Description: UNKNOWN
 Platform: UNKNOWN
```

### Comparing `cami-opal-1.0.8.post0/cami_opal.egg-info/SOURCES.txt` & `cami-opal-1.0.9/cami_opal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/opal.py` & `cami-opal-1.0.9/opal.py`

 * *Files 1% similar despite different names*

```diff
@@ -128,17 +128,15 @@
 
     # Bray-Curtis
     braycurtis = bc.braycurtis(gs_rank_to_taxid_to_percentage, rank_to_taxid_to_percentage)
 
     return unifrac, shannon, l1norm, binary_metrics, braycurtis
 
 
-def load_profiles(gold_standard_file, profiles_files, no_normalization):
-    normalize = False if no_normalization else True
-
+def load_profiles(gold_standard_file, profiles_files, normalize):
     gs_samples_list = load_data.open_profile(gold_standard_file, normalize)
     sample_ids_list = []
     for sample in gs_samples_list:
         sample_id, sample_metadata, profile = sample
         sample_ids_list.append(sample_id)
 
     profiles_list_to_samples_list = []
@@ -291,24 +289,24 @@
 def main():
     parser = argparse.ArgumentParser(description='OPAL: Open-community Profiling Assessment tooL', add_help=False)
     group1 = parser.add_argument_group('required arguments')
     group1.add_argument('profiles_files', nargs='+', help='Files of profiles')
     group1.add_argument('-g', '--gold_standard_file', help='Gold standard file', required=True)
     group1.add_argument('-o', '--output_dir', help='Directory to write the results to', required=True)
     group2 = parser.add_argument_group('optional arguments')
-    group2.add_argument('-n', '--no_normalization', help='Do not normalize samples', action='store_true')
+    group2.add_argument('-n', '--normalize', help='Normalize samples', action='store_true')
     group2.add_argument('-f', '--filter', help='Filter out the predictions with the smallest relative abundances summing up to [FILTER]%% within a rank (affects only precision, default: 0)', type=float)
     group2.add_argument('-p', '--plot_abundances', help='Plot abundances in the gold standard (can take some minutes)', action='store_true')
     group2.add_argument('-l', '--labels', help='Comma-separated profiles names', required=False)
     group2.add_argument('-t', '--time', help='Comma-separated runtimes in hours', required=False)
     group2.add_argument('-m', '--memory', help='Comma-separated memory usages in gigabytes', required=False)
     group2.add_argument('-d', '--desc', help='Description for HTML page', required=False)
     group2.add_argument('-r', '--ranks', help='Highest and lowest taxonomic ranks to consider in performance rankings, comma-separated. Valid ranks: superkingdom, phylum, class, order, family, genus, species, strain (default:superkingdom,species)', required=False)
-    group2.add_argument('--metrics_plot_rel', help='Metrics for spider plot of relative performances, first character, comma-separated. Valid metrics: w:weighted Unifrac, l:L1 norm, c:completeness, p:purity, f:false positives, t:true positives (default: w,l,c,p,f)', required=False)
-    group2.add_argument('--metrics_plot_abs', help='Metrics for spider plot of absolute performances, first character, comma-separated. Valid metrics: c:completeness, p:purity, b:Bray-Curtis (default: c,p)', required=False)
+    group2.add_argument('--metrics_plot_rel', help='Metrics for spider plot of relative performances, first character, comma-separated. Valid metrics: c:completeness, p:purity, l:L1 norm, w:weighted Unifrac, f:false positives, t:true positives (default: c,p,l,w)', required=False)
+    group2.add_argument('--metrics_plot_abs', help='Metrics for spider plot of absolute performances, first character, comma-separated. Valid metrics: c:completeness, p:purity, b:Bray-Curtis (default: c,p,b)', required=False)
     group2.add_argument('--silent', help='Silent mode', action='store_true')
     group2.add_argument('-v', '--version', action='version', version='%(prog)s ' + __version__)
     group2.add_argument('-h', '--help', action='help', help='Show this help message and exit')
     args = parser.parse_args()
     output_dir = os.path.abspath(args.output_dir)
     make_sure_path_exists(output_dir)
     labels = get_labels(args.labels, args.profiles_files)
@@ -316,15 +314,15 @@
     create_output_directories(output_dir, labels)
 
     logger = get_logger(args.output_dir, args.silent)
 
     logger.info('Loading profiles...')
     sample_ids_list, gs_samples_list, profiles_list_to_samples_list = load_profiles(args.gold_standard_file,
                                                                                     args.profiles_files,
-                                                                                    args.no_normalization)
+                                                                                    args.normalize)
     logger.info('done')
 
     plots_list = []
     if args.plot_abundances:
         logger.info('Plotting gold standard abundances...')
         plots_list += pl.plot_samples_hist(gs_samples_list, sample_ids_list, output_dir)
         logger.info('done')
```

### Comparing `cami-opal-1.0.8.post0/opal_stats.py` & `cami-opal-1.0.9/opal_stats.py`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/opal_workflow.py` & `cami-opal-1.0.9/opal_workflow.py`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/setup.py` & `cami-opal-1.0.9/setup.py`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/src/binary_metrics.py` & `cami-opal-1.0.9/src/binary_metrics.py`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/src/braycurtis.py` & `cami-opal-1.0.9/src/braycurtis.py`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/src/html_opal.py` & `cami-opal-1.0.9/src/html_opal.py`

 * *Files 4% similar despite different names*

```diff
@@ -112,76 +112,50 @@
         if rank == 'rank independent':
             rank_to_sample_pd[rank][sample] = rank_to_sample_pd[rank][sample].drop(c.ALL_METRICS[2:])
     return rank_to_sample_pd
 
 
 def get_formatted_pd_rankings(pd_rankings, labels):
     df_list = []
-    df_list_unsorted_pos = []
-    metrics_list = []
     for metric, g in pd_rankings.groupby(level=0):
-        metrics_list.append(metric)
         df = g.reset_index().sort_values('position')
-        df2 = g.reset_index()
         df_list.append(pd.DataFrame({metric: df['tool'].tolist(), 'score' + metric: df['position'].tolist()}))
-        df_list_unsorted_pos.append(pd.DataFrame({metric: df2['tool'].tolist(), 'score' + metric: df2['position'].tolist()}))
-
     df_sum = pd_rankings.groupby(['tool'])['position'].sum().reset_index().sort_values('position')
-    df_sum_unsorted_pos = pd_rankings.groupby(['tool'])['position'].sum().loc[labels].reset_index()
-
     df_list.append(
         pd.DataFrame({SUM_OF_SCORES: df_sum['tool'].tolist(), 'score' + SUM_OF_SCORES: df_sum['position'].tolist()}))
-    df_list_unsorted_pos.append(
-        pd.DataFrame({SUM_OF_SCORES: df_sum_unsorted_pos['tool'].tolist(), 'score' + SUM_OF_SCORES: df_sum_unsorted_pos['position'].tolist()}))
-
     pd_show = pd.concat(df_list, axis=1)
-    pd_show_unsorted_pos = pd.concat(df_list_unsorted_pos, axis=1)
-    return pd_show, pd_show_unsorted_pos
 
+    pd_plot = pd_rankings.reset_index().pivot(index='tool', columns='metric')
+    pd_plot[SUM_OF_SCORES] = pd_plot.sum(axis=1)
+    pd_plot = pd_plot.reindex(labels)
+    return pd_show, pd_plot
 
-def create_rankings_html(pd_rankings, ranks_scored, labels):
-    pd_show, pd_show_unsorted_pos = get_formatted_pd_rankings(pd_rankings, labels)
 
-    table_source = ColumnDataSource(pd_show)
-
-    columns = [
-        TableColumn(field=SUM_OF_SCORES, title=SUM_OF_SCORES, sortable=False),
-        TableColumn(field='score' + SUM_OF_SCORES, title='', width=50),
-        TableColumn(field=c.RECALL, title=c.RECALL, sortable=False),
-        TableColumn(field='score' + c.RECALL, title='', width=50),
-        TableColumn(field=c.PRECISION, title=c.PRECISION, sortable=False),
-        TableColumn(field='score' + c.PRECISION, title='', width=50),
-        TableColumn(field=c.L1NORM, title=c.L1NORM, sortable=False),
-        TableColumn(field='score' + c.L1NORM, title='', width=50),
-        TableColumn(field=c.UNIFRAC, title=c.UNIFRAC, sortable=False),
-        TableColumn(field='score' + c.UNIFRAC, title='', width=50),
-    ]
-    data_table = DataTable(source=table_source, columns=columns, width=800, height=25 + len(pd_show) * 25)
+def create_rankings_html(pd_rankings, ranks_scored, labels):
+    pd_show, pd_plot = get_formatted_pd_rankings(pd_rankings, labels)
 
-    top = [float(x) for x in pd_show_unsorted_pos['score' + SUM_OF_SCORES]]
-    source = ColumnDataSource(data=dict(x=pd_show_unsorted_pos[SUM_OF_SCORES].tolist(),
-                                        top=top,
-                                        recall=pd_show_unsorted_pos['score' + c.RECALL],
-                                        precision=pd_show_unsorted_pos['score' + c.PRECISION],
-                                        l1norm=pd_show_unsorted_pos['score' + c.L1NORM],
-                                        unifrac=pd_show_unsorted_pos['score' + c.UNIFRAC]))
+    source = ColumnDataSource(data=dict(x=labels,
+                                        top=pd_plot[SUM_OF_SCORES],
+                                        recall=pd_plot['position', c.RECALL],
+                                        precision=pd_plot['position', c.PRECISION],
+                                        l1norm=pd_plot['position', c.L1NORM],
+                                        unifrac=pd_plot['position', c.UNIFRAC]))
 
     callback = CustomJS(args=dict(source=source), code="""
         var data = source.data;
         var wrecall = weight_recall.value;
         var wprecision = weight_precision.value;
         var wl1norm = weight_l1norm.value;
         var wunifrac = weight_unifrac.value;
         topx = data['top'];
         recall = data['recall'];
         precision = data['precision'];
         l1norm = data['l1norm'];
         unifrac = data['unifrac'];
         
-        
         for (i = 0; i < topx.length; i++) {
             topx[i] = recall[i] * wrecall + precision[i] * wprecision + l1norm[i] * wl1norm + unifrac[i] * wunifrac;
         }
         
         source.change.emit();
     """)
 
@@ -193,17 +167,31 @@
 
     weight_l1norm = Slider(start=0, end=10, value=1, step=.1, title=c.L1NORM + " weight", callback=callback)
     callback.args["weight_l1norm"] = weight_l1norm
 
     weight_unifrac = Slider(start=0, end=10, value=1, step=.1, title=c.UNIFRAC + " weight", callback=callback)
     callback.args["weight_unifrac"] = weight_unifrac
 
-    p = figure(x_range=pd_show_unsorted_pos[SUM_OF_SCORES].tolist(), plot_width=800, plot_height=400, title=SUM_OF_SCORES + " - lower is better")
+    p = figure(x_range=pd_plot.index.to_list(), plot_width=1200, plot_height=400, title=SUM_OF_SCORES + " - lower is better")
     p.vbar(x='x', top='top', source=source, width=0.5, bottom=0, color="firebrick")
 
+    table_source = ColumnDataSource(pd_show)
+    columns = [
+        TableColumn(field=SUM_OF_SCORES, title=SUM_OF_SCORES, sortable=False),
+        TableColumn(field='score' + SUM_OF_SCORES, title='', width=50),
+        TableColumn(field=c.RECALL, title=c.RECALL, sortable=False),
+        TableColumn(field='score' + c.RECALL, title='', width=50),
+        TableColumn(field=c.PRECISION, title=c.PRECISION, sortable=False),
+        TableColumn(field='score' + c.PRECISION, title='', width=50),
+        TableColumn(field=c.L1NORM, title=c.L1NORM, sortable=False),
+        TableColumn(field='score' + c.L1NORM, title='', width=50),
+        TableColumn(field=c.UNIFRAC, title=c.UNIFRAC, sortable=False),
+        TableColumn(field='score' + c.UNIFRAC, title='', width=50),
+    ]
+    data_table = DataTable(source=table_source, columns=columns, width=800, height=25 + len(pd_show) * 25)
     col_rankings = column([Div(text="<font color='navy'><u>Hint 1:</u> click on the columns of scores for sorting.</font>", style={"width": "600px", "margin-bottom": "0px"}),
                            Div(text="Taxonomic ranks scored: " + ", ".join(ranks_scored), style={"width": "600px", "margin-bottom": "0px"}),
                            data_table,
                            Div(text="<font color='navy'><u>Hint 2:</u> slide the bars to change the weight of the metrics.</font>", style={"width": "500px", "margin-top": "18px"}),
                            row(weight_recall, weight_precision),
                            row(weight_l1norm, weight_unifrac),
                            p], css_classes=['bk-padding-top'])
```

### Comparing `cami-opal-1.0.8.post0/src/l1norm.py` & `cami-opal-1.0.9/src/l1norm.py`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/src/plots.py` & `cami-opal-1.0.9/src/plots.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from mpl_toolkits.mplot3d import Axes3D
 from matplotlib.lines import Line2D
 from src import braycurtis as bc
 from src.utils import spider_plot_functions as spl
 from src.utils import constants as c
 from src.utils import load_data
 import scipy.special
+import seaborn as sns
 
 
 def create_colors_list():
     colors_list = []
     for color in plt.cm.tab10(np.linspace(0, 1, 10))[:-1]:
         colors_list.append(tuple(color))
     colors_list.append("black")
@@ -352,15 +353,15 @@
 
 def spider_plot(metrics, labels, rank_to_metric_to_toolvalues, output_dir, file_name, colors, grid_points=None, fill=False, absolute=False):
     N = len(labels)
     if N < 3:
         return []
     theta = spl.radar_factory(N, frame='polygon')
     fig, axes = plt.subplots(figsize=(9, 9), nrows=2, ncols=3, subplot_kw=dict(projection='radar'))
-    fig.subplots_adjust(wspace=.5, hspace=0.3, top=0.87, bottom=0.45)
+    fig.subplots_adjust(wspace=1.0, hspace=0.0, top=0.87, bottom=0.45)
 
     for ax, rank in zip(axes.flat, c.PHYLUM_SPECIES):
         if grid_points:
             ax.set_rgrids(grid_points, fontsize='xx-small')
         else:
             ax.set_rgrids([0.2, 0.4, 0.6, 0.8], ('', '', '', ''))  # get rid of the labels of the grid points
         ax.set_title(rank, weight='bold', size=9, position=(0.5, 1.1),
@@ -397,15 +398,15 @@
             elif 0 < angle < np.pi:
                 label.set_horizontalalignment('right')
             else:
                 label.set_horizontalalignment('left')
 
         # move tick labels closer to plot and set font size
         for xticklabel in xticklabels:
-            xticklabel.set_position((0,.20))
+            xticklabel.set_position((0,.21))
             xticklabel.set_fontsize('x-small')
 
     if absolute:
         metrics = [metric[:-8] for metric in metrics]
 
     ax = axes[0, 0]
     ax.legend(metrics, loc=(2.0 - 0.353 * len(metrics), 1.25), labelspacing=0.1, fontsize='small', ncol=len(metrics), frameon=False)
@@ -456,25 +457,25 @@
     metrics_list = []
 
     if not absolute:
         initial_to_metric = {'w':c.UNIFRAC, 'l':c.L1NORM, 'c':c.RECALL, 'p':c.PRECISION, 'f':c.FP, 't':c.TP}
         for initial in metrics_initial:
             if initial not in initial_to_metric:
                 logging.getLogger('opal').warning('Invalid metric initial {} provided with option --metrics_plot_rel. Defaults will be used.'.format(initial))
-                return [c.UNIFRAC, c.L1NORM, c.RECALL, c.PRECISION, c.FP]
-            else:
+                return [c.RECALL, c.PRECISION, c.L1NORM, c.UNIFRAC]
+            elif initial_to_metric[initial] not in metrics_list:
                 metrics_list.append(initial_to_metric[initial])
         return metrics_list
 
     initial_to_metric = {'c':c.RECALL+'absolute', 'p':c.PRECISION+'absolute', 'b':c.BRAY_CURTIS+'absolute'}
     for initial in metrics_initial:
         if initial not in initial_to_metric:
             logging.getLogger('opal').warning('Invalid metric initial {} provided with option --metrics_plot_abs. Defaults will be used.'.format(initial))
-            return [c.RECALL+'absolute', c.PRECISION+'absolute']
-        else:
+            return [c.RECALL+'absolute', c.PRECISION+'absolute', c.BRAY_CURTIS+'absolute']
+        elif initial_to_metric[initial] not in metrics_list:
             metrics_list.append(initial_to_metric[initial])
     return metrics_list
 
 
 def plot_purity_completeness_per_tool_and_rank(pd_grouped, pd_mean, output_dir):
     ranks = c.ALL_RANKS[0:-1]
     ranks_range = range(len(ranks))
@@ -598,45 +599,45 @@
     cols = pd_grouped.columns
     pd_mean = pd_grouped.groupby(['rank', 'tool'], sort=False)[cols].mean()
 
     plot_purity_completeness_per_tool_and_rank(pd_grouped, pd_mean, output_dir)
 
     tool_to_rank_to_metric_to_value = spider_plot_preprocess_metrics(pd_mean, labels)
 
-    metrics_for_plot_rel = get_metrics_for_spider_plot(metrics_plot_rel, absolute=False) if metrics_plot_rel else [c.UNIFRAC, c.L1NORM, c.RECALL, c.PRECISION, c.FP]
-    metrics_for_plot_abs = get_metrics_for_spider_plot(metrics_plot_abs, absolute=True) if metrics_plot_abs else [c.RECALL+'absolute', c.PRECISION+'absolute']
+    metrics_for_plot_rel = get_metrics_for_spider_plot(metrics_plot_rel, absolute=False) if metrics_plot_rel else [c.RECALL, c.PRECISION, c.L1NORM, c.UNIFRAC]
+    metrics_for_plot_abs = get_metrics_for_spider_plot(metrics_plot_abs, absolute=True) if metrics_plot_abs else [c.RECALL+'absolute', c.PRECISION+'absolute', c.BRAY_CURTIS+'absolute']
 
     present_labels = []
     for label in labels:
         if label not in tool_to_rank_to_metric_to_value:
             continue
         else:
             present_labels.append(label)
         for rank in c.PHYLUM_SPECIES:
             for metric in metrics_for_plot_rel + metrics_for_plot_abs:
                 if metric in tool_to_rank_to_metric_to_value[label][rank]:
                     rank_to_metric_to_toolvalues[rank][metric].append(tool_to_rank_to_metric_to_value[label][rank][metric])
             rank_to_metric_to_toolvalues[rank][c.UNIFRAC].append(tool_to_rank_to_metric_to_value[label]['rank independent'][c.UNIFRAC])
 
-    colors = [plt.cm.tab10(2), plt.cm.tab10(0), plt.cm.tab10(3), 'k', 'm', 'y']
-    colors2 = ['r', 'k', 'olive']
+    colors = [sns.color_palette('colorblind')[x] for x in [0, 1, 2, 4, 7, 8]]
 
     plots_list = spider_plot(metrics_for_plot_rel,
                              present_labels,
                              rank_to_metric_to_toolvalues,
                              output_dir,
                              'spider_plot_relative',
-                             colors[:len(metrics_for_plot_rel)])
+                             colors[:len(metrics_for_plot_rel)],
+                             fill=True)
 
     plots_list += spider_plot(metrics_for_plot_abs,
                               present_labels,
                               rank_to_metric_to_toolvalues,
                               output_dir,
                               'spider_plot_absolute',
-                              colors2[:len(metrics_for_plot_abs)],
+                              colors[:len(metrics_for_plot_abs)],
                               grid_points=[0.2, 0.4, 0.6, 0.8, 1.0],
                               fill=True,
                               absolute=True)
 
     # compute average shannon for gold standard
     pd_shannon_equit = pd_metrics[pd_metrics['metric'] == c.SHANNON_EQUIT]
     table1 = pd_shannon_equit[pd_shannon_equit['tool'] == c.GS][['rank', 'value']]
```

### Comparing `cami-opal-1.0.8.post0/src/rankings.py` & `cami-opal-1.0.9/src/rankings.py`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/src/shannon.py` & `cami-opal-1.0.9/src/shannon.py`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/src/tsv2biom.py` & `cami-opal-1.0.9/src/tsv2biom.py`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/src/unifrac_distance.py` & `cami-opal-1.0.9/src/unifrac_distance.py`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/src/utils/EMDUnifrac.py` & `cami-opal-1.0.9/src/utils/EMDUnifrac.py`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/src/utils/ProfilingTools.py` & `cami-opal-1.0.9/src/utils/ProfilingTools.py`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/src/utils/constants.py` & `cami-opal-1.0.9/src/utils/constants.py`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/src/utils/load_data.py` & `cami-opal-1.0.9/src/utils/load_data.py`

 * *Files identical despite different names*

### Comparing `cami-opal-1.0.8.post0/src/utils/spider_plot_functions.py` & `cami-opal-1.0.9/src/utils/spider_plot_functions.py`

 * *Files identical despite different names*

