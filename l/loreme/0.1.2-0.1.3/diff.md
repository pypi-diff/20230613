# Comparing `tmp/loreme-0.1.2.tar.gz` & `tmp/loreme-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loreme-0.1.2.tar", last modified: Fri Jun  9 16:52:50 2023, max compression
+gzip compressed data, was "loreme-0.1.3.tar", last modified: Tue Jun 13 17:06:24 2023, max compression
```

## Comparing `loreme-0.1.2.tar` & `loreme-0.1.3.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-09 16:52:50.621053 loreme-0.1.2/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-05 04:30:20.000000 loreme-0.1.2/LICENSE
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2882 2023-06-09 16:52:50.620607 loreme-0.1.2/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2367 2023-06-05 20:21:59.000000 loreme-0.1.2/README.md
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-09 16:52:50.572999 loreme-0.1.2/loreme.egg-info/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2882 2023-06-09 16:52:50.000000 loreme-0.1.2/loreme.egg-info/PKG-INFO
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      717 2023-06-09 16:52:50.000000 loreme-0.1.2/loreme.egg-info/SOURCES.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-06-09 16:52:50.000000 loreme-0.1.2/loreme.egg-info/dependency_links.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-06-09 16:52:50.000000 loreme-0.1.2/loreme.egg-info/entry_points.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-06-09 16:52:50.000000 loreme-0.1.2/loreme.egg-info/requires.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-06-09 16:52:50.000000 loreme-0.1.2/loreme.egg-info/top_level.txt
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-06-09 16:51:40.000000 loreme-0.1.2/pyproject.toml
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-06-09 16:52:50.621205 loreme-0.1.2/setup.cfg
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-09 16:52:50.520907 loreme-0.1.2/src/
-drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-09 16:52:50.620009 loreme-0.1.2/src/loreme/
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1512 2023-06-05 20:07:53.000000 loreme-0.1.2/src/loreme/__init__.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/check_gpu_availability.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3119 2023-06-08 08:55:56.000000 loreme-0.1.2/src/loreme/dorado.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5227 2023-06-08 08:59:20.000000 loreme-0.1.2/src/loreme/download.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3336 2023-06-08 09:00:46.000000 loreme-0.1.2/src/loreme/env.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/export_bedgraph.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/gene_body_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/intersect.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)    33071 2023-06-09 16:49:10.000000 loreme-0.1.2/src/loreme/loreme.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5191 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/mean.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/merge.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/methylation_hist.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/parse_gff.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2610 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/pbcpg.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     6487 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/plot.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     2440 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/plot_bedtools.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/plot_genes.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/plot_repeats.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-05 04:30:20.000000 loreme-0.1.2/src/loreme/promoter_methylation.py
--rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-06-09 16:51:24.000000 loreme-0.1.2/src/loreme/version.py
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-13 17:06:24.342747 loreme-0.1.3/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1520 2023-06-05 04:30:20.000000 loreme-0.1.3/LICENSE
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5166 2023-06-13 17:06:24.342137 loreme-0.1.3/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4651 2023-06-13 17:03:35.000000 loreme-0.1.3/README.md
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-13 17:06:24.306628 loreme-0.1.3/loreme.egg-info/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5166 2023-06-13 17:06:24.000000 loreme-0.1.3/loreme.egg-info/PKG-INFO
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      763 2023-06-13 17:06:24.000000 loreme-0.1.3/loreme.egg-info/SOURCES.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        1 2023-06-13 17:06:24.000000 loreme-0.1.3/loreme.egg-info/dependency_links.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       46 2023-06-13 17:06:24.000000 loreme-0.1.3/loreme.egg-info/entry_points.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       77 2023-06-13 17:06:24.000000 loreme-0.1.3/loreme.egg-info/requires.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)        7 2023-06-13 17:06:24.000000 loreme-0.1.3/loreme.egg-info/top_level.txt
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      918 2023-06-10 09:03:08.000000 loreme-0.1.3/pyproject.toml
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       38 2023-06-13 17:06:24.342878 loreme-0.1.3/setup.cfg
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-13 17:06:24.297881 loreme-0.1.3/src/
+drwxr-xr-x   0 anthonyaylward   (501) staff       (20)        0 2023-06-13 17:06:24.340872 loreme-0.1.3/src/loreme/
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1623 2023-06-10 18:11:11.000000 loreme-0.1.3/src/loreme/__init__.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2645 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/check_gpu_availability.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      396 2023-06-10 18:19:42.000000 loreme-0.1.3/src/loreme/check_tags.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3631 2023-06-13 05:56:48.000000 loreme-0.1.3/src/loreme/dorado.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5921 2023-06-10 17:32:09.000000 loreme-0.1.3/src/loreme/download.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3602 2023-06-10 17:30:49.000000 loreme-0.1.3/src/loreme/env.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1496 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/export_bedgraph.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3440 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/gene_body_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1144 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/intersect.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)    37354 2023-06-13 05:58:08.000000 loreme-0.1.3/src/loreme/loreme.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5191 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/mean.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     1690 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/merge.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      940 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/methylation_hist.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)      376 2023-06-10 17:48:02.000000 loreme-0.1.3/src/loreme/modkit.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3054 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/parse_gff.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2219 2023-06-10 18:20:20.000000 loreme-0.1.3/src/loreme/pbcpg.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     6487 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/plot.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     2440 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/plot_bedtools.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     5087 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/plot_genes.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     4327 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/plot_repeats.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)     3433 2023-06-05 04:30:20.000000 loreme-0.1.3/src/loreme/promoter_methylation.py
+-rw-r--r--   0 anthonyaylward   (501) staff       (20)       90 2023-06-10 09:03:11.000000 loreme-0.1.3/src/loreme/version.py
```

### Comparing `loreme-0.1.2/LICENSE` & `loreme-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `loreme-0.1.2/loreme.egg-info/SOURCES.txt` & `loreme-0.1.3/loreme.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -5,24 +5,26 @@
 loreme.egg-info/SOURCES.txt
 loreme.egg-info/dependency_links.txt
 loreme.egg-info/entry_points.txt
 loreme.egg-info/requires.txt
 loreme.egg-info/top_level.txt
 src/loreme/__init__.py
 src/loreme/check_gpu_availability.py
+src/loreme/check_tags.py
 src/loreme/dorado.py
 src/loreme/download.py
 src/loreme/env.py
 src/loreme/export_bedgraph.py
 src/loreme/gene_body_methylation.py
 src/loreme/intersect.py
 src/loreme/loreme.py
 src/loreme/mean.py
 src/loreme/merge.py
 src/loreme/methylation_hist.py
+src/loreme/modkit.py
 src/loreme/parse_gff.py
 src/loreme/pbcpg.py
 src/loreme/plot.py
 src/loreme/plot_bedtools.py
 src/loreme/plot_genes.py
 src/loreme/plot_repeats.py
 src/loreme/promoter_methylation.py
```

### Comparing `loreme-0.1.2/pyproject.toml` & `loreme-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "loreme"
-version = "0.1.2" # Don't forget to match with version.py and docs/source/conf.py
+version = "0.1.3" # Don't forget to match with version.py and docs/source/conf.py
 authors = [
     { name="Anthony Aylward", email="aaylward@salk.edu" },
 ]
 description = "Extract Methylation calls from ONT or PB long read data"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `loreme-0.1.2/src/loreme/__init__.py` & `loreme-0.1.3/src/loreme/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,24 +4,26 @@
 long read sequencing data.
 
 It consists of an API and CLI for three distinct applications:
 
 1. Pacific Biosciences data processing. PB reads in SAM/BAM format are aligned
 to a reference genome with the special-purpose aligner `pbmm2 <https://github.com/PacificBiosciences/pbmm2>`_ ,
 a modified version of `minimap2 <https://lh3.github.io/minimap2/>`_ .
-Methylation calls are then extracted from the aligned reads by `pb-CpG-tools <https://github.com/PacificBiosciences/pb-CpG-tools>`_ .
+Methylation calls are then piled up from the aligned reads with `pb-CpG-tools <https://github.com/PacificBiosciences/pb-CpG-tools>`_ .
 
 2. Oxford nanopore basecalling. ONT reads are optionally converted from FAST5
 to `POD5 <https://github.com/nanoporetech/pod5-file-format>`_ format, then
-basecalled and aligned to a reference with `dorado <https://github.com/nanoporetech/dorado>`_ .
-(dorado alignment also uses minimap2 under the hood).
+basecalled and aligned to a reference with `dorado <https://github.com/nanoporetech/dorado>`_ 
+(dorado alignment also uses minimap2 under the hood), and finally piled up with
+`modkit <https://github.com/nanoporetech/modkit/>`_ .
 
 3. Postprocessing and QC of methylation calls. Several functions are available
 to generate diagnostic statistics and plots.
 """
 
 from loreme.version import __version__
 from loreme.env import PBCPG_MODEL
 from loreme.download import download_pbcpg, download_dorado
-from loreme.pbcpg import pbcpg_check_tags, pbcpg_align_bam, pbcpg_align_bams, pbcpg_extract
 from loreme.check_gpu_availability import check_gpu_availability
-from loreme.dorado import dorado
+from loreme.check_tags import check_tags
+from loreme.pbcpg import pbcpg_align_bam, pbcpg_align_bams, pbcpg_pileup
+from loreme.dorado import dorado_basecall
```

### Comparing `loreme-0.1.2/src/loreme/check_gpu_availability.py` & `loreme-0.1.3/src/loreme/check_gpu_availability.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.2/src/loreme/dorado.py` & `loreme-0.1.3/src/loreme/dorado.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 import itertools
 import os
 import os.path
 import subprocess
-
+import pysam
+import multiprocessing
 from loreme.env import DORADO_PATH, DORADO_PATH_024, DORADO_MODEL_DIR, DORADO_PLATFORM
 
+CPU_COUNT = multiprocessing.cpu_count()
+
 def fast5_to_pod5(*input_fast5, output_pod5: str, threads: int = 1):
     """Convert FAST5 files to POD5 files
 
     Parameters
     ----------
     *input_fast5
         fast5 files or directories containing fast5s
@@ -19,17 +22,17 @@
     parsed_fast5 = itertools.chain.from_iterable(
         ([os.path.join(f, f5) for f5 in os.listdir(f) if f5.endswith('.fast5')]
          if os.path.isdir(f) else [f]) for f in input_fast5)
     subprocess.run(('pod5', 'convert', 'fast5', *parsed_fast5,
                     '--output', output_pod5, '--threads', str(threads)))
 
 
-def dorado(input_dir, output, speed: int = 400, accuracy: str ='fast',
+def dorado_basecall(input_dir, output, speed: int = 400, accuracy: str ='fast',
            frequency: str = '4kHz', modified_bases: str = '5mCG_5hmCG',
-           reference=None):
+           no_mod: bool = False, reference=None):
     """Run dorado basecaller
 
     Parameters
     ----------
     input_dir : str
         directory containing POD5 or Fast5 files
     output : str
@@ -58,29 +61,34 @@
     if speed == 260 and frequency != '4kHz':
         raise RuntimeError('260bps speed only available at 4kHz frequency')
     if frequency == '4kHz' and modified_bases != '5mCG_5hmCG':
         raise RuntimeError('the only modified base model at 4kHz frequency is 5mCG_5hmCG')
     model = f"dna_r10.4.1_e8.2_{speed}bps_{accuracy}@v4.{1+(frequency=='5kHz')}.0"
     with open(output, 'wb') as f:
         subprocess.run((DORADO_PATH_024[DORADO_PLATFORM], 'basecaller',
-                        os.path.join(DORADO_MODEL_DIR, model), input_dir,
-                        '--modified-bases', modified_bases)
+                        os.path.join(DORADO_MODEL_DIR, model), input_dir)
+                        + (not no_mod) * ('--modified-bases', modified_bases)
                         + bool(reference) * ('--reference', reference),
                        stdout=f)
 
 
-def dorado_align(index: str, reads: str, output: str):
-    """Run dorado aligner
+def dorado_align(reference_index: str, input_reads: str, output_bam: str,
+                 threads: int = CPU_COUNT, mem_per_thread_mb: int = 768):
+    """Run dorado aligner, sorting and indexing the output
 
     Parameters
     ----------
-    index : str
+    reference_index : str
         path to reference index
-    reads : str
+    input_reads : str
         path to input reads
-    output : str
+    output_bam : str
         path to output BAM file
     """
 
-    with open(output, 'wb') as f:
-        subprocess.run((DORADO_PATH[DORADO_PLATFORM], 'aligner', index,
-                        reads), stdout=f)
+    with open(output_bam, 'wb') as f, \
+        subprocess.Popen((DORADO_PATH[DORADO_PLATFORM], 'aligner',
+            reference_index, input_reads), stdout=subprocess.PIPE) as aligner:
+        subprocess.run(('samtools', 'sort', '-@', str(threads),
+                        '-m', f'{mem_per_thread_mb}M'),
+                       stdin=aligner.stdout, stdout=f)
+    pysam.index(output_bam)
```

### Comparing `loreme-0.1.2/src/loreme/download.py` & `loreme-0.1.3/src/loreme/download.py`

 * *Files 7% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import ftplib
 import gzip
 import tarfile
 import subprocess
 from itertools import product
 from loreme.env import (PBCPG_URL, PBCPG_DIR, EXAMPLE_DATA_URLS, EXAMPLE_DATA_DIR, HG38_FTP,
                        HG38_GENOME_PATH, HG38_ANNOT_PATH, DORADO_DIR, DORADO_URL, DORADO_URL_024,
-                       DORADO_MODEL_DIR, DORADO_PATH_024)
+                       DORADO_MODEL_DIR, DORADO_PATH_024, MODKIT_URL, MODKIT_DIR)
 
 def download_pbcpg(directory: str = PBCPG_DIR):
     """Download pb-CpG-tools
 
     Parameters
     ----------
     directory : str
@@ -113,7 +113,26 @@
     #     subprocess.run((DORADO_PATH[pfm], 'download', '--directory', model_dir,
     #         '--model', f'dna_r10.4.1_e8.2_400bps_{accuracy}@v4.2.0'))
     #     subprocess.run((DORADO_PATH[pfm], 'download', '--directory', model_dir,
     #         '--model', f'dna_r10.4.1_e8.2_400bps_{accuracy}@v4.2.0_5mCG_5hmCG@v2'))
     # for modified_bases in '5mC', '6mA':
     #     subprocess.run((DORADO_PATH[pfm], 'download', '--directory', model_dir,
     #         '--model', f'dna_r10.4.1_e8.2_400bps_sup@v4.2.0_{modified_bases}@v2'))
+
+def download_modkit(directory: str = MODKIT_DIR):
+    """Download pb-CpG-tools
+
+    Parameters
+    ----------
+    directory : str
+        Destination directory for pb-CpG-tools
+    """
+
+    dest_tarfile = os.path.join(directory, 'modkit_v0.1.8_centos7_x86_64.tar.gz')
+    print(f'downloading to {dest_tarfile}')
+    if os.path.exists(dest_tarfile):
+        raise RuntimeError(f'a file already exists at {dest_tarfile}')
+    http = urllib3.PoolManager()
+    with http.request('GET', MODKIT_URL, preload_content=False) as r, open(dest_tarfile, 'wb') as f:
+        shutil.copyfileobj(r, f)
+    with tarfile.open(dest_tarfile) as tar:
+        tar.extractall(path=directory)
```

### Comparing `loreme-0.1.2/src/loreme/env.py` & `loreme-0.1.3/src/loreme/env.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,7 +44,11 @@
     'linux-x64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.2.4-linux-x64.tar.gz',
     'linux-arm64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.2.4-linux-arm64.tar.gz',
     'osx-arm64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.2.4-osx-arm64.tar.gz',
     'win64': 'https://cdn.oxfordnanoportal.com/software/analysis/dorado-0.2.4-win64.zip'
 }
 DORADO_MODEL_DIR = os.environ.get('LOREME_DORADO_MODEL_DIR',
     os.path.join(os.path.dirname(__file__)))
+MODKIT_URL = 'https://github.com/nanoporetech/modkit/releases/download/v0.1.8/modkit_v0.1.8_centos7_x86_64.tar.gz'
+MODKIT_DIR = os.environ.get('LOREME_MODKIT_DIR',
+    os.path.join(os.path.dirname(__file__)))
+MODKIT_PATH = os.path.join(MODKIT_DIR, 'dist', 'modkit')
```

### Comparing `loreme-0.1.2/src/loreme/export_bedgraph.py` & `loreme-0.1.3/src/loreme/export_bedgraph.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.2/src/loreme/gene_body_methylation.py` & `loreme-0.1.3/src/loreme/gene_body_methylation.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.2/src/loreme/intersect.py` & `loreme-0.1.3/src/loreme/intersect.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.2/src/loreme/loreme.py` & `loreme-0.1.3/src/loreme/loreme.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,22 +8,26 @@
 
 
 # Imports ======================================================================
 
 import argparse
 import os.path
 import platform
+import shutil
 from math import floor
 from loreme.env import (PBCPG_DIR, PBCPG_MODEL, EXAMPLE_DATA_DIR, DORADO_DIR,
-                       DORADO_MODEL_DIR)
+                       DORADO_MODEL_DIR, DORADO_PLATFORM, MODKIT_DIR)
 from loreme.version import __version__
-from loreme.download import download_pbcpg, download_example, download_dorado
-from loreme.pbcpg import pbcpg_check_tags, pbcpg_align_bams, pbcpg_extract
+from loreme.download import (download_pbcpg, download_example, download_dorado,
+                             download_modkit)
+from loreme.check_tags import check_tags
 from loreme.check_gpu_availability import check_gpu_availability
-from loreme.dorado import fast5_to_pod5, dorado, dorado_align
+from loreme.pbcpg import pbcpg_align_bams, pbcpg_pileup
+from loreme.dorado import CPU_COUNT, fast5_to_pod5, dorado_basecall, dorado_align
+from loreme.modkit import modkit_pileup
 from loreme.mean import calculate_mean, calculate_total_mean
 from loreme.gene_body_methylation import gene_body_methylation
 from loreme.promoter_methylation import promoter_methylation
 from loreme.plot import plot, COLOR_PALETTE
 from loreme.plot_genes import plot_genes
 from loreme.plot_repeats import plot_repeats
 from loreme.merge import merge_bedmethyl
@@ -95,74 +99,84 @@
 
 
 def _download_dorado(args):
     download_dorado(args.platform, directory=args.directory,
                     model_dir=args.model_dir)
 
 
-def _pbcpg_check_tags(args):
-    if pbcpg_check_tags(args.bam, n_reads=args.n_reads):
+def _download_modkit(args):
+    download_modkit(directory=args.directory)
+
+
+def _check_tags(args):
+    if check_tags(args.bam, n_reads=args.n_reads):
         print('MM/ML tags found')
     else:
         raise RuntimeError('MM/ML tags not found in BAM file')
 
 
+def _check_gpu_availability(args):
+    if check_gpu_availability(args.devices, gpu_load=args.gpu_load,
+                           gpu_mem=args.gpu_mem):
+        print('GPU is available')
+
+
 def _pbcpg_align(args):
     pbcpg_align_bams(args.fasta, args.bam, args.aligned_bam,
         threads=max(1, args.threads-1),
         memory_mb=max(floor(args.memory/args.threads), 1))
 
 
-def _pbcpg_extract(args):
-    pbcpg_extract(args.bam, args.output_prefix, hap_tag=args.hap_tag,
+def _pbcpg_pileup(args):
+    pbcpg_pileup(args.bam, args.output_prefix, hap_tag=args.hap_tag,
                   min_coverage=args.min_coverage,min_mapq=args.min_mapq,
                   model=args.model, threads=args.threads)
 
 
 def run_pbcpg(args):
     pbcpg_validate_args_pre_alignment(args)
     for bam in args.bam:
-        if not pbcpg_check_tags(bam, n_reads=args.n_reads):
+        if not check_tags(bam, n_reads=args.n_reads):
             raise RuntimeError('MM/ML tags not found in BAM file')
     aligned_bam = f'{args.output_prefix}.pbmm2.bam'
     pbcpg_align_bams(args.fasta, args.bam, aligned_bam,
         threads=max(1, args.threads-1),
         memory_mb = max(floor(args.memory/args.threads), 1))
     args.bam = aligned_bam
     pbcpg_validate_args_post_alignment(args)
-    _pbcpg_extract(args)
+    _pbcpg_pileup(args)
 
 
 def _fast5_to_pod5(args):
     fast5_to_pod5(*args.fast5, output_pod5=args.output, threads=args.threads)
 
 
-def _dorado_check_gpu(args):
-    if check_gpu_availability(args.devices, gpu_load=args.gpu_load,
-                           gpu_mem=args.gpu_mem):
-        print('GPU is available')
+def _dorado_align(args):
+    dorado_align(args.index, args.reads, args.output, threads=args.threads,
+                 mem_per_thread_mb=int(args.memory_mb/args.threads))
 
 
-def _dorado_align(args):
-    dorado_align(args.index, args.reads, args.output)
+def _modkit_pileup(args):
+    modkit_pileup(args.fasta, args.input, args.output, threads=args.threads)
 
 
-def run_dorado(args):
+def run_dorado_basecall(args):
     check_gpu_availability([0])
     if args.convert:
         pod5_dir = f'{args.output[:-4]}_pod5'
         pod5_base = f'{os.path.basename(args.output)[:-4]}.pod5'
         os.mkdir(pod5_dir)
         fast5_to_pod5(*args.reads,
                       output_pod5=os.path.join(pod5_dir, pod5_base),
                       threads=args.threads)
-        dorado(pod5_dir, args.output, speed=args.speed, accuracy=args.accuracy)
+        dorado_basecall(pod5_dir, args.output, speed=args.speed,
+                        accuracy=args.accuracy, no_mod=args.no_mod)
     elif len(args.reads) == 1 and os.path.isdir(args.reads[0]):
-        dorado(args.reads[0], args.output, speed=args.speed,
-               accuracy=args.accuracy)
+        dorado_basecall(args.reads[0], args.output, speed=args.speed,
+               accuracy=args.accuracy, no_mod=args.no_mod)
     else:
         raise RuntimeError('For running without --convert, supply only one input FAST5 or POD5 directory')
 
 
 
 def _calculate_mean(args):
     if args.total:
@@ -227,14 +241,41 @@
     intersect_bedmethyl(args.bedmethyl, chromosomes=args.chromosomes)
 
 
 def _export_bedgraph(args):
     export_bedgraph(args.bedmethyl, chromosomes=args.chromosomes,
                     coverage=args.coverage)
 
+def clean(args):
+    for root in args.dirs:
+        for file in ('pb-CpG-tools-v2.3.1-x86_64-unknown-linux-gnu.tar.gz',
+                     'dorado-0.2.4-linux-x64.tar.gz',
+                     'dorado-0.3.0-linux-x64.tar.gz',
+                     'modkit_v0.1.8_centos7_x86_64.tar.gz'):
+            if os.path.isfile(os.path.join(root, file)):
+                os.remove(os.path.join(root, file))
+        for directory in ('pb-CpG-tools-v2.3.1-x86_64-unknown-linux-gnu/',
+                          f'dorado-0.2.4-{DORADO_PLATFORM}/',
+                          f'dorado-0.3.0-{DORADO_PLATFORM}/',
+                          'dna_r10.4.1_e8.2_260bps_fast@v4.1.0/',
+                          'dna_r10.4.1_e8.2_260bps_hac@v4.1.0/',
+                          'dna_r10.4.1_e8.2_260bps_sup@v4.1.0/',
+                          'dna_r10.4.1_e8.2_400bps_fast@v4.1.0/',
+                          'dna_r10.4.1_e8.2_400bps_hac@v4.1.0/',
+                          'dna_r10.4.1_e8.2_400bps_sup@v4.1.0/',
+                          'dna_r10.4.1_e8.2_260bps_fast@v4.1.0_5mCG_5hmCG@v2/',
+                          'dna_r10.4.1_e8.2_260bps_hac@v4.1.0_5mCG_5hmCG@v2/',
+                          'dna_r10.4.1_e8.2_260bps_sup@v4.1.0_5mCG_5hmCG@v2/',
+                          'dna_r10.4.1_e8.2_400bps_fast@v4.1.0_5mCG_5hmCG@v2/',
+                          'dna_r10.4.1_e8.2_400bps_hac@v4.1.0_5mCG_5hmCG@v2/',
+                          'dna_r10.4.1_e8.2_400bps_sup@v4.1.0_5mCG_5hmCG@v2/',
+                          'dist'):
+            if os.path.exists(os.path.join(root, directory)):
+                shutil.rmtree(os.path.join(root, directory))
+
 
 def parse_arguments():
     parser = argparse.ArgumentParser(
         description="""Analysis of DNA methylation signals from `Pacific Biosciences <https://www.pacb.com/technology/hifi-sequencing/>`_
 or `Oxford Nanopore <https://nanoporetech.com/applications/dna-nanopore-sequencing>`_
 long read sequencing data.""")
     parser.add_argument('--version', action='version',
@@ -257,22 +298,49 @@
     parser_download_dorado.add_argument(
         '-d', '--directory', metavar='<directory/>', default=DORADO_DIR,
         help=f'destination directory for dorado (default: {DORADO_DIR})')
     parser_download_dorado.add_argument(
         '-m', '--model-dir', metavar='<directory/>', default=DORADO_MODEL_DIR,
         help=f'destination directory for dorado models (default: {DORADO_MODEL_DIR})')
 
+    parser_download_modkit = subparsers.add_parser('download-modkit',
+                                                  help='download modkit')
+    parser_download_modkit.set_defaults(func=_download_modkit)
+    parser_download_modkit.add_argument(
+        '-d', '--directory', metavar='<directory/>', default=MODKIT_DIR,
+        help=f'destination directory for pb-CpG-tools (default: {MODKIT_DIR})')
+
     parser_download_example = subparsers.add_parser('download-example',
         help='download an example dataset for pbcpg')
     parser_download_example.set_defaults(func=_download_example)
     parser_download_example.add_argument( '-d', '--directory', metavar='<directory/>',
         default=EXAMPLE_DATA_DIR, help='destination directory for example data')
     parser_download_example.add_argument('-n', '--n-samples', metavar='<int>',
         type=int, default=1, help='number of samples to download, max 4 (default: 1)')
 
+    parser_check_tags = subparsers.add_parser('check-tags', help='check BAM for MM/ML tags')
+    parser_check_tags.set_defaults(func=_check_tags)
+    parser_check_tags.add_argument("bam", metavar="<reads.bam>",
+        help="BAM file to check.")
+    parser_check_tags.add_argument('-n', '--n-reads', metavar="<int>",
+        type=int, default=1000, help="Number of reads to check (default: %(default)d].")
+
+    parser_check_gpu = subparsers.add_parser('check-gpu',
+        help='check GPU availability')
+    parser_check_gpu.set_defaults(func=_check_gpu_availability)
+    parser_check_gpu.add_argument('--devices', metavar='<int>', type=int,
+                                      nargs='+', default=[0],
+                                      help='GPUs to check')
+    parser_check_gpu.add_argument('--gpu-load', metavar='<float>', type=float,
+                                     default=0.9,
+                                     help='required available GPU load')
+    parser_check_gpu.add_argument('--gpu-mem', metavar='<float>', type=float,
+                                     default=0.9,
+                                     help='required available GPU memory')
+
     parser_pbcpg = subparsers.add_parser('pbcpg', help='run full pbcpg pipeline')
     parser_pbcpg.set_defaults(func=run_pbcpg)
     io_args = parser_pbcpg.add_argument_group('io args')
     io_args.add_argument("bam", metavar="<unaligned.bam>", nargs='+',
                         help="Unaligned BAM file.")
     io_args.add_argument("fasta", metavar="<ref.fasta>",
                         help="The reference fasta file.")
@@ -305,21 +373,14 @@
     resource_args = parser_pbcpg.add_argument_group('resource args')
     resource_args.add_argument("-t", "--threads", metavar="<int>", default=1,
                         type=int,
                         help="Number of threads for parallel processing. (default: %(default)d)")
     resource_args.add_argument("--memory", metavar="<int>", default=4_000,
                         type=int,
                         help="Memory for read alignment and sorting in megabytes. (default: %(default)d)")
-    
-    parser_pbcpg_check = subparsers.add_parser('pbcpg-check', help='check BAM for MM/ML tags')
-    parser_pbcpg_check.set_defaults(func=_pbcpg_check_tags)
-    parser_pbcpg_check.add_argument("bam", metavar="<reads.bam>",
-        help="BAM file to check.")
-    parser_pbcpg_check.add_argument('-n', '--n-reads', metavar="<int>",
-        type=int, default=1000, help="Number of reads to check (default: %(default)d].")
 
     parser_pbcpg_align = subparsers.add_parser('pbcpg-align', help='align BAM to reference')
     parser_pbcpg_align.set_defaults(func=_pbcpg_align)
     io_args = parser_pbcpg_align.add_argument_group('io args')
     io_args.add_argument("bam", metavar="<unaligned.bam>", nargs='+',
         help="Unaligned BAM file to read.")
     io_args.add_argument("fasta", metavar="<ref.fasta>",
@@ -330,24 +391,24 @@
     resource_args.add_argument("-t", "--threads", metavar="<int>", type=int,
         default=1,
         help="Number of threads for parallel processing. (default: %(default)d)")
     resource_args.add_argument("--memory", metavar="<int>", type=int,
         default=4_000,
         help="Memory for read alignment and sorting in megabytes. (default: %(default)d)")
 
-    parser_pbcpg_extract = subparsers.add_parser('pbcpg-extract', help='extract methylation calls from aligned PB reads')
-    parser_pbcpg_extract.set_defaults(func=pbcpg_extract)
-    io_args = parser_pbcpg_extract.add_argument_group('io args')
+    parser_pbcpg_pileup = subparsers.add_parser('pbcpg-pileup', help='pile up methylation calls from aligned PB reads')
+    parser_pbcpg_pileup.set_defaults(func=pbcpg_pileup)
+    io_args = parser_pbcpg_pileup.add_argument_group('io args')
     io_args.add_argument("bam", metavar="<aligned.bam>",
                         help="Aligned BAM file.")
     io_args.add_argument("fasta", metavar="<ref.fasta>",
                         help="The reference fasta file.")
     io_args.add_argument("output_prefix", metavar="<prefix>",
                         help="prefix for output files, which results in [prefix].bam/bed/bw.")
-    score_args = parser_pbcpg_extract.add_argument_group('score args')
+    score_args = parser_pbcpg_pileup.add_argument_group('score args')
     score_args.add_argument("--model", metavar="</path/to/model.tflite>",
                         default=PBCPG_MODEL,
                         help=f"Full path to the model (*.tflite files) to load. (default: {PBCPG_MODEL})")
     score_args.add_argument("--modsites", choices=["denovo", "reference"],
                         default="denovo",
                         help="Only output CG sites with a modification probability > 0 "
                              "(denovo), or output all CG sites based on the "
@@ -360,76 +421,83 @@
                         help="Ignore alignments with MAPQ < N. (default: %(default)d)")
     score_args.add_argument("-a", "--hap_tag", metavar="<TAG>", default="HP",
                         help="The SAM tag containing haplotype information. (default: %(default)s)")
     score_args.add_argument("-s", "--chunksize", metavar="<int>", default=500_000,
                         type=int,
                         help="Break reference regions into chunks "
                              "of this size for parallel processing. (default: %(default)d)")
-    resource_args = parser_pbcpg_extract.add_argument_group('resource args')
+    resource_args = parser_pbcpg_pileup.add_argument_group('resource args')
     resource_args.add_argument("-t", "--threads", metavar="<int>", default=1,
                         type=int,
                         help="Number of threads for parallel processing. (default: %(default)d)")
-    
-    parser_dorado = subparsers.add_parser('dorado',
+
+    parser_dorado_convert = subparsers.add_parser('dorado-convert',
+        help='convert FAST5 to POD5')
+    parser_dorado_convert.set_defaults(func=_fast5_to_pod5)
+    parser_dorado_convert.add_argument('fast5', metavar='<reads[.fast5]>', nargs='+',
+                               help='input FAST5 files, or direcories containing FAST5')
+    parser_dorado_convert.add_argument('output', metavar='<output.pod5>',
+                               help='path to output POD5 file')
+    parser_dorado_convert.add_argument("-t", "--threads", metavar="<int>",
+        type=int, default=1, help="Number of threads. (default: %(default)d)")
+
+    parser_dorado_basecall = subparsers.add_parser('dorado-basecall',
         help='run full dorado pipeline')
-    parser_dorado.set_defaults(func=run_dorado)
-    parser_dorado.add_argument('reads', metavar='<reads>', nargs='+',
+    parser_dorado_basecall.set_defaults(func=run_dorado_basecall)
+    parser_dorado_basecall.add_argument('reads', metavar='<reads>', nargs='+',
                                help='input FAST5 files, or single directory containing FAST5 or POD5 files')
-    parser_dorado.add_argument('output', metavar='<output.sam>',
+    parser_dorado_basecall.add_argument('output', metavar='<output.sam>',
                                help='path to output SAM file')
-    parser_dorado.add_argument('--convert', action='store_true',
+    parser_dorado_basecall.add_argument('--convert', action='store_true',
                                help='convert FAST5 to POD5 before basecalling')
-    parser_dorado.add_argument('--speed', type=int, choices=(260, 400),
+    parser_dorado_basecall.add_argument('--speed', type=int, choices=(260, 400),
                                default=400, help='pore speed (default: 400)')
-    parser_dorado.add_argument('--accuracy', choices=('fast', 'hac', 'sup'),
+    parser_dorado_basecall.add_argument('--accuracy', choices=('fast', 'hac', 'sup'),
                                default='fast', help='model accuracy (default: fast)')
-    # parser_dorado.add_argument('--frequency', choices=('4kHz', '5kHz'),
+    parser_dorado_basecall.add_argument('--no-mod', action='store_true',
+                               help='turn off modified basecalling')
+    # parser_dorado_basecall.add_argument('--frequency', choices=('4kHz', '5kHz'),
     #                            default='4kHz', help='(default: 4kHz)')
-    # parser_dorado.add_argument('--modified-bases',
+    # parser_dorado_basecall.add_argument('--modified-bases',
     #                            choices=('5mCG_5hmCG', '5mC', '6mA'),
     #                            default='5mCG_5hmCG',
     #                            help='Modified base model (default: 5mCG_5hmCG)')
-    # parser_dorado.add_argument('--reference', metavar='<index>',
+    # parser_dorado_basecall.add_argument('--reference', metavar='<index>',
     #                            help='map to a reference index (fastq/fasta/mmi)')
-    parser_dorado.add_argument("-t", "--threads", metavar="<int>",
+    parser_dorado_basecall.add_argument("-t", "--threads", metavar="<int>",
         type=int, default=1,
         help="Number of cpu threads. (default: %(default)d)")
-    
-    parser_dorado_check = subparsers.add_parser('dorado-check',
-        help='check GPU availability')
-    parser_dorado_check.set_defaults(func=_dorado_check_gpu)
-    parser_dorado_check.add_argument('--devices', metavar='<int>', type=int,
-                                      nargs='+', default=[0],
-                                      help='GPUs to check')
-    parser_dorado_check.add_argument('--gpu-load', metavar='<float>', type=float,
-                                     default=0.9,
-                                     help='required available GPU load')
-    parser_dorado_check.add_argument('--gpu-mem', metavar='<float>', type=float,
-                                     default=0.9,
-                                     help='required available GPU memory')
-
-    parser_dorado_convert = subparsers.add_parser('dorado-convert',
-        help='convert FAST5 to POD5')
-    parser_dorado_convert.set_defaults(func=_fast5_to_pod5)
-    parser_dorado_convert.add_argument('fast5', metavar='<reads[.fast5]>', nargs='+',
-                               help='input FAST5 files, or direcories containing FAST5')
-    parser_dorado_convert.add_argument('output', metavar='<output.pod5>',
-                               help='path to output POD5 file')
-    parser_dorado_convert.add_argument("-t", "--threads", metavar="<int>",
-        type=int, default=1, help="Number of threads. (default: %(default)d)")
 
     parser_dorado_align = subparsers.add_parser('dorado-align',
         help='align dorado basecalls')
     parser_dorado_align.set_defaults(func=_dorado_align)
     parser_dorado_align.add_argument('index', metavar='<index>',
                                      help='reference index for alignment')
     parser_dorado_align.add_argument('reads', metavar='<reads>',
                                      help='reads for alignment')
     parser_dorado_align.add_argument('output', metavar='<output.bam>',
                                      help='path to output BAM file')
+    parser_dorado_align.add_argument('--threads', metavar='<int>', type=int,
+                                     default=CPU_COUNT,
+                                     help=f'number of sorting threads (default: {CPU_COUNT})')
+    parser_dorado_align.add_argument('--memory-mb', metavar='<int>', type=int,
+                                     default=CPU_COUNT*768,
+                                     help=f'approximate sorting memory in MB (default: {CPU_COUNT*768})')
+    
+    parser_modkit_pileup = subparsers.add_parser('modkit-pileup',
+        help='pile up aligned dorado methylation calls')
+    parser_modkit_pileup.set_defaults(func=_modkit_pileup)
+    parser_modkit_pileup.add_argument('fasta', metavar='<reference.fasta>',
+        help='reference FASTA file')
+    parser_modkit_pileup.add_argument('input', metavar='<input.bam>',
+        help='input BAM file')
+    parser_modkit_pileup.add_argument('output', metavar='<output.bed>',
+        help='output BED file')
+    parser_modkit_pileup.add_argument("-t", "--threads", metavar="<int>",
+        type=int, default=1, help="Number of threads. (default: %(default)d)")
 
     parser_mean = subparsers.add_parser('mean',
         help='calculate average methylation across chromosomes or in total')
     parser_mean.set_defaults(func=_calculate_mean)
     parser_mean.add_argument('bedmethyl', metavar='<bedmethyl.bed>',
         nargs='+', help='bedMethyl file containing methylation data')
     parser_mean.add_argument('--plot', metavar='<output.{pdf,png,svg}>',
@@ -620,13 +688,20 @@
     parser_intersect.add_argument('bedmethyl', metavar='<bedmethyl.bed>',
         nargs='+', help='bedMethyl file containing methylation data')
     parser_intersect.add_argument('output_prefix', metavar='<output-prefix>',
         help='prefix for output files')
     parser_intersect.add_argument('--chromosomes', metavar='<X>',
         nargs='+', help='chromosomes to include')
 
+    parser_clean = subparsers.add_parser('clean',
+        help='clean up downloads for uninstall')
+    parser_clean.set_defaults(func=clean)
+    parser_clean.add_argument('--dirs', metavar='<directory/>',
+        nargs='+', default=[PBCPG_DIR, DORADO_DIR, DORADO_MODEL_DIR],
+        help=f"directories to clean up (default: {', '.join(set([PBCPG_DIR, DORADO_DIR, DORADO_MODEL_DIR]))})")
+
     return parser.parse_args()
 
 
 def main():
     args = parse_arguments()
     args.func(args)
```

### Comparing `loreme-0.1.2/src/loreme/mean.py` & `loreme-0.1.3/src/loreme/mean.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.2/src/loreme/merge.py` & `loreme-0.1.3/src/loreme/merge.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.2/src/loreme/methylation_hist.py` & `loreme-0.1.3/src/loreme/methylation_hist.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.2/src/loreme/parse_gff.py` & `loreme-0.1.3/src/loreme/parse_gff.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.2/src/loreme/pbcpg.py` & `loreme-0.1.3/src/loreme/pbcpg.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,12 @@
 import os
 import subprocess
 import pysam
-from itertools import islice
 from loreme.env import PBCPG_PATH, PBCPG_MODEL
 
-def pbcpg_check_tags(bam, n_reads: int = 1000):
-    samfile = pysam.AlignmentFile(bam, 'r', check_sq=False)
-    has_tags = any(((read.has_tag('MM') or read.has_tag('Mm'))
-                    and (read.has_tag('ML') or read.has_tag('Ml'))
-                    for read in islice(samfile.fetch(until_eof=True), n_reads)))
-    samfile.close()
-    return has_tags
-
-
 def pbcpg_align_bam(ref: str, in_bam: str, out_bam: str, threads: int = 1,
               memory_mb: int = 768):
     """Run pbmm2 to align a BAM file to a FASTA reference
 
     Parameters
     ----------
     ref : str
@@ -63,15 +53,15 @@
         pysam.merge('-o', out_bam,
                     *(f'{out_bam[:-4]}_{n}.bam' for n in range(len(in_bams))))
         pysam.index(out_bam)
         for n in range(len(in_bams)):
             os.remove(f'{out_bam[:-4]}_{n}.bam')
             os.remove(f'{out_bam[:-4]}_{n}.bam.bai')
 
-def pbcpg_extract(bam, output_prefix, hap_tag: str = 'HP',
+def pbcpg_pileup(bam, output_prefix, hap_tag: str = 'HP',
                   min_coverage: int = 4, min_mapq: int = 1,
                   model: str = PBCPG_MODEL, threads: int = 1):
     subprocess.run((PBCPG_PATH, '--bam', bam,
         '--output-prefix', output_prefix,
         '--hap-tag', hap_tag,
         '--min-coverage', str(min_coverage),
         '--min-mapq', str(min_mapq),
```

### Comparing `loreme-0.1.2/src/loreme/plot.py` & `loreme-0.1.3/src/loreme/plot.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.2/src/loreme/plot_bedtools.py` & `loreme-0.1.3/src/loreme/plot_bedtools.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.2/src/loreme/plot_genes.py` & `loreme-0.1.3/src/loreme/plot_genes.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.2/src/loreme/plot_repeats.py` & `loreme-0.1.3/src/loreme/plot_repeats.py`

 * *Files identical despite different names*

### Comparing `loreme-0.1.2/src/loreme/promoter_methylation.py` & `loreme-0.1.3/src/loreme/promoter_methylation.py`

 * *Files identical despite different names*

