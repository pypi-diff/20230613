# Comparing `tmp/janis-pipelines.bioinformatics-0.9.8.tar.gz` & `tmp/janis-pipelines.bioinformatics-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/janis-pipelines.bioinformatics-0.9.8.tar", last modified: Wed Apr 22 06:49:03 2020, max compression
+gzip compressed data, was "dist/janis-pipelines.bioinformatics-0.9.9.tar", last modified: Fri Apr 24 00:05:34 2020, max compression
```

## Comparing `janis-pipelines.bioinformatics-0.9.8.tar` & `janis-pipelines.bioinformatics-0.9.9.tar`

### file list

```diff
@@ -1,363 +1,367 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3233 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     2305 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_pipelines.bioinformatics.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3233 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_pipelines.bioinformatics.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_pipelines.bioinformatics.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       21 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_pipelines.bioinformatics.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_pipelines.bioinformatics.egg-info/not-zip-safe
--rw-rw-r--   0 travis    (2000) travis    (2000)    14922 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_pipelines.bioinformatics.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       29 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_pipelines.bioinformatics.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      180 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_pipelines.bioinformatics.egg-info/entry_points.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      326 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)     1420 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/
--rw-rw-r--   0 travis    (2000) travis    (2000)      541 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/cram.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      304 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/sam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      334 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/bai.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      538 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/bam.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1435 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/vcf.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      465 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/bed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2740 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/fastq.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      298 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/crai.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3148 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/fasta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      177 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      100 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/__meta__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v98_3/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4449 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v98_3/cache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    43400 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v98_3/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      350 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v98_3/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v98_3/database.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v96_3/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3317 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v96_3/basedatabase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4430 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v96_3/basecache.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    22269 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v96_3/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      358 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v96_3/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      113 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/latest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       19 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vardict/
--rw-rw-r--   0 travis    (2000) travis    (2000)    18271 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vardict/vardictgermline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18114 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vardict/vardictgermline_compressed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18408 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vardict/vardictsomatic_compressed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18655 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vardict/vardictsomatic.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      518 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vardict/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      835 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vardict/vardict.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/papenfuss/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/papenfuss/gridss/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1430 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/papenfuss/gridss/gridss.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8782 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/papenfuss/gridss/base_2_2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/papenfuss/gridss/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4657 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/papenfuss/gridss/base_2_4.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       29 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/papenfuss/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/parsefastqc/
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/parsefastqc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5120 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/parsefastqc/v0_1_0.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/trimiupac/
--rw-rw-r--   0 travis    (2000) travis    (2000)      356 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/trimiupac/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1917 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/trimiupac/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/trimiupac/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      543 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      126 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/combinevariants/
--rw-rw-r--   0 travis    (2000) travis    (2000)      404 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/combinevariants/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5210 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/combinevariants/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/combinevariants/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/multiqc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      206 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/multiqc/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11590 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/multiqc/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/multiqc/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cellranger/
--rw-rw-r--   0 travis    (2000) travis    (2000)      140 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cellranger/cellranger.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cellranger/mkfastq/
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cellranger/mkfastq/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10209 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cellranger/mkfastq/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cellranger/mkfastq/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       32 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cellranger/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/freebayes/
--rw-rw-r--   0 travis    (2000) travis    (2000)      437 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/freebayes/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25243 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/freebayes/base_1_2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/freebayes/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25593 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/freebayes/base_1_3.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/annotate/
--rw-rw-r--   0 travis    (2000) travis    (2000)      317 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/annotate/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10387 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/annotate/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/annotate/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/sort/
--rw-rw-r--   0 travis    (2000) travis    (2000)      182 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/sort/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3003 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/sort/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/sort/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/index/
--rw-rw-r--   0 travis    (2000) travis    (2000)      222 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/index/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3452 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/index/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/index/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      261 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/bcftoolstoolbase.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/norm/
--rw-rw-r--   0 travis    (2000) travis    (2000)      289 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/norm/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9893 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/norm/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/norm/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/view/
--rw-rw-r--   0 travis    (2000) travis    (2000)      289 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/view/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12050 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/view/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/view/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      191 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/bcftools_1_5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      480 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/concat/
--rw-rw-r--   0 travis    (2000) travis    (2000)      227 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/concat/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6885 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/concat/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/concat/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      137 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/bcftools_1_9.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cutadapt/
--rw-rw-r--   0 travis    (2000) travis    (2000)    19657 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cutadapt/base_2.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      880 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cutadapt/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    18177 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cutadapt/base_1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       24 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cutadapt/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/
--rw-rw-r--   0 travis    (2000) travis    (2000)      225 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/htslib_1_9.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      182 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/htslib_1_2_1.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/tabix/
--rw-rw-r--   0 travis    (2000) travis    (2000)      115 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/tabix/tabix_1_9.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      123 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/tabix/tabix_1_2_1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6705 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/tabix/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/tabix/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      178 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/tabix/latest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/bgzip/
--rw-rw-r--   0 travis    (2000) travis    (2000)      184 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/bgzip/bgzip_1_2_1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      115 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/bgzip/bgzip_1_9.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5551 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/bgzip/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/bgzip/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      178 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/bgzip/latest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      200 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/htslibbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      242 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       68 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/latest.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/mergeandmark/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1469 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/mergeandmark/mergeandmark_4_0.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/mergeandmark/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1480 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/mergeandmark/mergeandmark_4_1_3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2701 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/bwaaligner.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7238 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/splitmultiallele.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    17733 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/bwamem_samtoolsview.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/indexfasta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      302 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/io_lib/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/io_lib/scramble/
--rw-rw-r--   0 travis    (2000) travis    (2000)      236 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/io_lib/scramble/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6135 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/io_lib/scramble/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/io_lib/scramble/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      227 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/io_lib/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       33 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/io_lib/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/validation/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1501 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/validation/performancevalidator.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       61 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/validation/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/star/
--rw-rw-r--   0 travis    (2000) travis    (2000)      305 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/star/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6448 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/star/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       59 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/star/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      456 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bioinformaticstoolbase.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/filtermutectcalls/
--rw-rw-r--   0 travis    (2000) travis    (2000)      513 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/filtermutectcalls/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4974 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/filtermutectcalls/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/filtermutectcalls/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1201 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/gatk4toolbase.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergesamfiles/
--rw-rw-r--   0 travis    (2000) travis    (2000)      564 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergesamfiles/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8084 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergesamfiles/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergesamfiles/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/createsequencedictionary/
--rw-rw-r--   0 travis    (2000) travis    (2000)      601 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/createsequencedictionary/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/createsequencedictionary/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/createsequencedictionary/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/applybqsr/
--rw-rw-r--   0 travis    (2000) travis    (2000)      449 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/applybqsr/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5294 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/applybqsr/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/applybqsr/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/fastqtosam/
--rw-rw-r--   0 travis    (2000) travis    (2000)      569 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/fastqtosam/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11393 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/fastqtosam/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/fastqtosam/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/markduplicates/
--rw-rw-r--   0 travis    (2000) travis    (2000)      576 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/markduplicates/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10961 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/markduplicates/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/markduplicates/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/sortsam/
--rw-rw-r--   0 travis    (2000) travis    (2000)      492 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/sortsam/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7047 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/sortsam/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/sortsam/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/printreads/
--rw-rw-r--   0 travis    (2000) travis    (2000)      528 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/printreads/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2708 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/printreads/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/printreads/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/splitreads/
--rw-rw-r--   0 travis    (2000) travis    (2000)      442 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/splitreads/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    21881 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/splitreads/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/splitreads/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/calculatecontaminations/
--rw-rw-r--   0 travis    (2000) travis    (2000)      563 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/calculatecontaminations/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5608 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/calculatecontaminations/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/calculatecontaminations/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergebamalignment/
--rw-rw-r--   0 travis    (2000) travis    (2000)      653 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergebamalignment/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13809 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergebamalignment/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergebamalignment/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/baserecalibrator/
--rw-rw-r--   0 travis    (2000) travis    (2000)      600 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/baserecalibrator/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6489 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/baserecalibrator/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/baserecalibrator/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      926 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/versions.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/genotypeconcordance/
--rw-rw-r--   0 travis    (2000) travis    (2000)      636 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/genotypeconcordance/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12401 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/genotypeconcordance/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/genotypeconcordance/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/getpileupsummaries/
--rw-rw-r--   0 travis    (2000) travis    (2000)      523 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/getpileupsummaries/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4078 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/getpileupsummaries/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/getpileupsummaries/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/haplotypecaller/
--rw-rw-r--   0 travis    (2000) travis    (2000)      588 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/haplotypecaller/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19836 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/haplotypecaller/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/haplotypecaller/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mutect2/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6313 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mutect2/base_4_0.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    46730 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mutect2/base_4_1.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      553 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mutect2/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mutect2/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/learnreadorientationmodel/
--rw-rw-r--   0 travis    (2000) travis    (2000)      624 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/learnreadorientationmodel/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3415 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/learnreadorientationmodel/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/learnreadorientationmodel/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergemutectstats/
--rw-rw-r--   0 travis    (2000) travis    (2000)      503 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergemutectstats/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2940 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergemutectstats/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergemutectstats/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/gathervcfs/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6891 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/gathervcfs/base_compressed.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      962 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/gathervcfs/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6824 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/gathervcfs/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/gathervcfs/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/babrahambioinformatics/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/babrahambioinformatics/fastqc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      317 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/babrahambioinformatics/fastqc/fastqc_0_11_5.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9497 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/babrahambioinformatics/fastqc/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/babrahambioinformatics/fastqc/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      136 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/babrahambioinformatics/fastqc/latest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      250 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/babrahambioinformatics/fastqc/fastqc_0_11_8.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       89 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/babrahambioinformatics/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/biobambam/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/biobambam/bamsormadup/
--rw-rw-r--   0 travis    (2000) travis    (2000)      254 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/biobambam/bamsormadup/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4958 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/biobambam/bamsormadup/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/biobambam/bamsormadup/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      220 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/biobambam/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       36 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/biobambam/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ucsf/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ucsf/cnvkit/
--rw-rw-r--   0 travis    (2000) travis    (2000)      238 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ucsf/cnvkit/cnvkit_0_9_6.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5750 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ucsf/cnvkit/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ucsf/cnvkit/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       60 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ucsf/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/
--rw-rw-r--   0 travis    (2000) travis    (2000)      134 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcflib_1_0_1.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfallelicprimitives/
--rw-rw-r--   0 travis    (2000) travis    (2000)      226 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfallelicprimitives/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1935 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfallelicprimitives/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfallelicprimitives/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      230 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcflibtoolbase.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcffixup/
--rw-rw-r--   0 travis    (2000) travis    (2000)      166 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcffixup/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1431 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcffixup/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcffixup/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfroc/
--rw-rw-r--   0 travis    (2000) travis    (2000)      156 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfroc/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2012 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfroc/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfroc/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfuniqalleles/
--rw-rw-r--   0 travis    (2000) travis    (2000)      196 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfuniqalleles/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1321 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfuniqalleles/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfuniqalleles/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      451 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfrandomsample/
--rw-rw-r--   0 travis    (2000) travis    (2000)      201 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfrandomsample/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1857 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfrandomsample/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfrandomsample/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfuniq/
--rw-rw-r--   0 travis    (2000) travis    (2000)      161 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfuniq/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1298 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfuniq/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfuniq/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bwa/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bwa/index/
--rw-rw-r--   0 travis    (2000) travis    (2000)      160 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bwa/index/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2290 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bwa/index/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bwa/index/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      139 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bwa/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       58 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bwa/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bwa/mem/
--rw-rw-r--   0 travis    (2000) travis    (2000)      212 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bwa/mem/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11588 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bwa/mem/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bwa/mem/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      466 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/
--rw-rw-r--   0 travis    (2000) travis    (2000)      237 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/strelka_2_9_9.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/strelkasomatic/
--rw-rw-r--   0 travis    (2000) travis    (2000)    15671 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/strelkasomatic/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/strelkasomatic/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      439 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/strelkasomatic/strelkasomatic.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/strelkagermline/
--rw-rw-r--   0 travis    (2000) travis    (2000)      447 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/strelkagermline/strelkagermline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    14522 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/strelkagermline/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/strelkagermline/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/manta/
--rw-rw-r--   0 travis    (2000) travis    (2000)      461 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/manta/manta.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11152 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/manta/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/manta/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      274 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/strelka_2_9_10.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      208 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/illuminabase.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/happy/
--rw-rw-r--   0 travis    (2000) travis    (2000)    20508 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/happy/happybase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      292 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/happy/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/happy/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      441 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/gatk/
--rw-rw-r--   0 travis    (2000) travis    (2000)     3945 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/gatk/gatksomatic_variants_4_0_12.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3083 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/gatk/gatkgermline_variants_4_0_12.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3996 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/gatk/gatksomatic_variants_4_1_3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3289 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/gatk/gatkgermline_variants_4_1_3.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      292 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/gatk/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1311 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/gridssgermline.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2358 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/vardictgermline_variants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2406 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/vardictsomatic_variants.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2107 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/illuminagermline_strelka.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2230 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/illuminasomatic_strelka.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      155 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/
--rw-rw-r--   0 travis    (2000) travis    (2000)      143 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/samtools_1_7.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      157 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/samtools_1_9.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/sort/
--rw-rw-r--   0 travis    (2000) travis    (2000)     7225 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/sort/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      289 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/sort/sort.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/sort/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/index/
--rw-rw-r--   0 travis    (2000) travis    (2000)      365 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/index/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1713 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/index/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10698 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/index/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/faidx/
--rw-rw-r--   0 travis    (2000) travis    (2000)      365 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/faidx/versions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1205 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/faidx/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/faidx/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-22 06:49:03.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/view/
--rw-rw-r--   0 travis    (2000) travis    (2000)      289 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/view/view.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    11157 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/view/base.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/view/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      334 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2368 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/samtoolstoolbase.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      151 2020-04-22 06:48:48.000000 janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3233 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2305 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_pipelines.bioinformatics.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3233 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_pipelines.bioinformatics.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_pipelines.bioinformatics.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       21 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_pipelines.bioinformatics.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_pipelines.bioinformatics.egg-info/not-zip-safe
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15092 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_pipelines.bioinformatics.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       29 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_pipelines.bioinformatics.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      180 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_pipelines.bioinformatics.egg-info/entry_points.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      326 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1420 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      541 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/cram.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      304 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/sam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      334 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/bai.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      538 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/bam.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1435 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/vcf.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      465 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/bed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2740 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/fastq.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      298 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/crai.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3148 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/fasta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      177 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      100 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/__meta__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v98_3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4449 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v98_3/cache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    43400 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v98_3/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      350 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v98_3/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3414 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v98_3/database.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v96_3/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3317 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v96_3/basedatabase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4430 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v96_3/basecache.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    22269 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v96_3/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      358 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v96_3/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      113 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/latest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       19 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vardict/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18271 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vardict/vardictgermline.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18114 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vardict/vardictgermline_compressed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18408 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vardict/vardictsomatic_compressed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18655 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vardict/vardictsomatic.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      518 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vardict/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      835 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vardict/vardict.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/papenfuss/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/papenfuss/gridss/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1430 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/papenfuss/gridss/gridss.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8782 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/papenfuss/gridss/base_2_2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/papenfuss/gridss/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4657 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/papenfuss/gridss/base_2_4.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       29 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/papenfuss/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/parsefastqc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/parsefastqc/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5120 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/parsefastqc/v0_1_0.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/trimiupac/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      356 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/trimiupac/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1917 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/trimiupac/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/trimiupac/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      543 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      126 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/combinevariants/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      404 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/combinevariants/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5210 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/combinevariants/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/combinevariants/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/multiqc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      206 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/multiqc/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11590 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/multiqc/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/multiqc/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cellranger/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      140 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cellranger/cellranger.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cellranger/mkfastq/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cellranger/mkfastq/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10209 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cellranger/mkfastq/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cellranger/mkfastq/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       32 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cellranger/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/freebayes/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      437 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/freebayes/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25243 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/freebayes/base_1_2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       68 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/freebayes/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25593 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/freebayes/base_1_3.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/annotate/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      317 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/annotate/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10387 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/annotate/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/annotate/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/sort/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      182 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/sort/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3003 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/sort/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/sort/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/index/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      222 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/index/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3452 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/index/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/index/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      261 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/bcftoolstoolbase.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/norm/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      289 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/norm/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9893 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/norm/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/norm/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/view/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      289 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/view/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12050 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/view/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/view/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      191 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/bcftools_1_5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      480 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/concat/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      227 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/concat/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6885 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/concat/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/concat/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      137 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/bcftools_1_9.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cutadapt/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19657 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cutadapt/base_2.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      880 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cutadapt/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    18177 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cutadapt/base_1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       24 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cutadapt/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      225 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/htslib_1_9.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      182 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/htslib_1_2_1.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/tabix/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      115 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/tabix/tabix_1_9.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      123 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/tabix/tabix_1_2_1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6705 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/tabix/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/tabix/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      178 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/tabix/latest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/bgzip/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      184 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/bgzip/bgzip_1_2_1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      115 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/bgzip/bgzip_1_9.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5551 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/bgzip/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/bgzip/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      178 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/bgzip/latest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      200 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/htslibbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      242 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       68 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/latest.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/mergeandmark/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1469 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/mergeandmark/mergeandmark_4_0.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/mergeandmark/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1480 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/mergeandmark/mergeandmark_4_1_3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2701 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/bwaaligner.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7238 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/splitmultiallele.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    17733 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/bwamem_samtoolsview.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1243 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/indexfasta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      302 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/io_lib/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/io_lib/scramble/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      236 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/io_lib/scramble/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6135 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/io_lib/scramble/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/io_lib/scramble/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      227 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/io_lib/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       33 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/io_lib/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/validation/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1501 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/validation/performancevalidator.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       61 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/validation/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/star/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      305 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/star/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6448 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/star/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       59 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/star/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      456 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bioinformaticstoolbase.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/filtermutectcalls/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      513 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/filtermutectcalls/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4974 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/filtermutectcalls/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/filtermutectcalls/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1201 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/gatk4toolbase.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergesamfiles/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      564 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergesamfiles/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8084 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergesamfiles/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergesamfiles/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/createsequencedictionary/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      601 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/createsequencedictionary/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2336 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/createsequencedictionary/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/createsequencedictionary/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/applybqsr/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      449 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/applybqsr/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5294 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/applybqsr/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/applybqsr/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/fastqtosam/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      569 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/fastqtosam/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11393 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/fastqtosam/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/fastqtosam/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/markduplicates/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      576 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/markduplicates/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10961 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/markduplicates/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/markduplicates/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/sortsam/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      492 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/sortsam/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7047 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/sortsam/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/sortsam/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/printreads/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      528 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/printreads/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2708 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/printreads/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/printreads/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/splitreads/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      442 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/splitreads/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    21881 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/splitreads/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/splitreads/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/calculatecontaminations/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      563 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/calculatecontaminations/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5608 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/calculatecontaminations/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/calculatecontaminations/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergebamalignment/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      653 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergebamalignment/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13809 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergebamalignment/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergebamalignment/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/baserecalibrator/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      600 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/baserecalibrator/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6489 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/baserecalibrator/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/baserecalibrator/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      926 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/versions.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/genotypeconcordance/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      636 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/genotypeconcordance/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12401 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/genotypeconcordance/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/genotypeconcordance/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/getpileupsummaries/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      523 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/getpileupsummaries/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4078 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/getpileupsummaries/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/getpileupsummaries/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/haplotypecaller/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      588 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/haplotypecaller/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19836 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/haplotypecaller/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/haplotypecaller/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mutect2/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6313 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mutect2/base_4_0.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    46730 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mutect2/base_4_1.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      553 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mutect2/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mutect2/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/learnreadorientationmodel/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      624 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/learnreadorientationmodel/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3415 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/learnreadorientationmodel/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/learnreadorientationmodel/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3215 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergemutectstats/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      503 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergemutectstats/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2940 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergemutectstats/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergemutectstats/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/gathervcfs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6891 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/gathervcfs/base_compressed.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      962 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/gathervcfs/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6824 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/gathervcfs/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/gathervcfs/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/babrahambioinformatics/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/babrahambioinformatics/fastqc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      317 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/babrahambioinformatics/fastqc/fastqc_0_11_5.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9497 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/babrahambioinformatics/fastqc/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/babrahambioinformatics/fastqc/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      136 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/babrahambioinformatics/fastqc/latest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      250 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/babrahambioinformatics/fastqc/fastqc_0_11_8.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       89 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/babrahambioinformatics/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/biobambam/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/biobambam/bamsormadup/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      254 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/biobambam/bamsormadup/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4958 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/biobambam/bamsormadup/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/biobambam/bamsormadup/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      220 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/biobambam/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       36 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/biobambam/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ucsf/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ucsf/cnvkit/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      238 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ucsf/cnvkit/cnvkit_0_9_6.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5750 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ucsf/cnvkit/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ucsf/cnvkit/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       60 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ucsf/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      134 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcflib_1_0_1.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfallelicprimitives/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      226 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfallelicprimitives/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1935 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfallelicprimitives/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfallelicprimitives/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      230 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcflibtoolbase.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcffixup/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      166 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcffixup/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1431 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcffixup/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcffixup/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfroc/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      156 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfroc/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2012 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfroc/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfroc/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfuniqalleles/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      196 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfuniqalleles/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1321 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfuniqalleles/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfuniqalleles/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      451 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfrandomsample/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      201 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfrandomsample/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1857 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfrandomsample/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfrandomsample/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfuniq/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      161 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfuniq/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1298 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfuniq/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfuniq/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bwa/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bwa/index/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      160 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bwa/index/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2290 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bwa/index/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bwa/index/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      139 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bwa/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       58 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bwa/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bwa/mem/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      212 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bwa/mem/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11588 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bwa/mem/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bwa/mem/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      466 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      237 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/strelka_2_9_9.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/strelkasomatic/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15671 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/strelkasomatic/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/strelkasomatic/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      439 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/strelkasomatic/strelkasomatic.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/strelkagermline/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      447 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/strelkagermline/strelkagermline.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    14522 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/strelkagermline/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/strelkagermline/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/manta/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      461 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/manta/manta.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11152 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/manta/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/manta/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      274 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/strelka_2_9_10.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      208 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/illuminabase.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/bcl2fastq/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      278 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/bcl2fastq/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7294 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/bcl2fastq/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/bcl2fastq/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:33.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/happy/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20508 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/happy/happybase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/happy/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/happy/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      476 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/gatk/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3945 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/gatk/gatksomatic_variants_4_0_12.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3083 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/gatk/gatkgermline_variants_4_0_12.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3996 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/gatk/gatksomatic_variants_4_1_3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3289 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/gatk/gatkgermline_variants_4_1_3.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      292 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/gatk/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1311 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/gridssgermline.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2358 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/vardictgermline_variants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2406 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/vardictsomatic_variants.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2107 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/illuminagermline_strelka.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2230 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/illuminasomatic_strelka.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      155 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      143 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/samtools_1_7.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      157 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/samtools_1_9.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/sort/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7225 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/sort/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      289 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/sort/sort.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/sort/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/index/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      365 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/index/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1713 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/index/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10698 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/index/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/faidx/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      365 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/faidx/versions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1205 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/faidx/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/faidx/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:34.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/view/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      289 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/view/view.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    11157 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/view/base.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/view/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      334 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2368 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/samtoolstoolbase.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      151 2020-04-24 00:05:18.000000 janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/__init__.py
```

### Comparing `janis-pipelines.bioinformatics-0.9.8/PKG-INFO` & `janis-pipelines.bioinformatics-0.9.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janis-pipelines.bioinformatics
-Version: 0.9.8
+Version: 0.9.9
 Summary: Bioinformatics tools for Janis; the Pipeline creation helper
 Home-page: https://github.com/PMCC-BioinformaticsCore/janis-bioinformatics
 Author: Michael Franklin, Evan Thomas, Mohammad Bhuyan
 Author-email: michael.franklin@petermac.org
 License: GNU
 Description: # Janis - Bioinformatics Toolbox
```

### Comparing `janis-pipelines.bioinformatics-0.9.8/README.md` & `janis-pipelines.bioinformatics-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_pipelines.bioinformatics.egg-info/PKG-INFO` & `janis-pipelines.bioinformatics-0.9.9/janis_pipelines.bioinformatics.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janis-pipelines.bioinformatics
-Version: 0.9.8
+Version: 0.9.9
 Summary: Bioinformatics tools for Janis; the Pipeline creation helper
 Home-page: https://github.com/PMCC-BioinformaticsCore/janis-bioinformatics
 Author: Michael Franklin, Evan Thomas, Mohammad Bhuyan
 Author-email: michael.franklin@petermac.org
 License: GNU
 Description: # Janis - Bioinformatics Toolbox
```

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_pipelines.bioinformatics.egg-info/SOURCES.txt` & `janis-pipelines.bioinformatics-0.9.9/janis_pipelines.bioinformatics.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -165,14 +165,17 @@
 janis_bioinformatics/tools/htslib/tabix/latest.py
 janis_bioinformatics/tools/htslib/tabix/tabix_1_2_1.py
 janis_bioinformatics/tools/htslib/tabix/tabix_1_9.py
 janis_bioinformatics/tools/illumina/__init__.py
 janis_bioinformatics/tools/illumina/illuminabase.py
 janis_bioinformatics/tools/illumina/strelka_2_9_10.py
 janis_bioinformatics/tools/illumina/strelka_2_9_9.py
+janis_bioinformatics/tools/illumina/bcl2fastq/__init__.py
+janis_bioinformatics/tools/illumina/bcl2fastq/base.py
+janis_bioinformatics/tools/illumina/bcl2fastq/versions.py
 janis_bioinformatics/tools/illumina/happy/__init__.py
 janis_bioinformatics/tools/illumina/happy/happybase.py
 janis_bioinformatics/tools/illumina/happy/versions.py
 janis_bioinformatics/tools/illumina/manta/__init__.py
 janis_bioinformatics/tools/illumina/manta/base.py
 janis_bioinformatics/tools/illumina/manta/manta.py
 janis_bioinformatics/tools/illumina/strelkagermline/__init__.py
```

### Comparing `janis-pipelines.bioinformatics-0.9.8/setup.py` & `janis-pipelines.bioinformatics-0.9.9/setup.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/cram.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/cram.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/bam.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/bam.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/vcf.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/vcf.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/fastq.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/fastq.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/data_types/fasta.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/data_types/fasta.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v98_3/cache.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v98_3/cache.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v98_3/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v98_3/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v98_3/database.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v98_3/database.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v96_3/basedatabase.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v96_3/basedatabase.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v96_3/basecache.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v96_3/basecache.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ensembl/vep/v96_3/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ensembl/vep/v96_3/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vardict/vardictgermline.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vardict/vardictgermline.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vardict/vardictgermline_compressed.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vardict/vardictgermline_compressed.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vardict/vardictsomatic_compressed.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vardict/vardictsomatic_compressed.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vardict/vardictsomatic.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vardict/vardictsomatic.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vardict/__init__.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vardict/__init__.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vardict/vardict.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vardict/vardict.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/papenfuss/gridss/gridss.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/papenfuss/gridss/gridss.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/papenfuss/gridss/base_2_2.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/papenfuss/gridss/base_2_2.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/papenfuss/gridss/base_2_4.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/papenfuss/gridss/base_2_4.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/parsefastqc/v0_1_0.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/parsefastqc/v0_1_0.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/trimiupac/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/trimiupac/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/pmac/combinevariants/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/pmac/combinevariants/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/multiqc/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/multiqc/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cellranger/mkfastq/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cellranger/mkfastq/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/freebayes/base_1_2.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/freebayes/base_1_2.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/freebayes/base_1_3.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/freebayes/base_1_3.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/annotate/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/annotate/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/sort/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/sort/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/index/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/index/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/norm/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/norm/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/view/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/view/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bcftools/concat/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bcftools/concat/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cutadapt/base_2.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cutadapt/base_2.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cutadapt/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cutadapt/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/cutadapt/base_1.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/cutadapt/base_1.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/tabix/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/tabix/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/htslib/bgzip/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/htslib/bgzip/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/mergeandmark/mergeandmark_4_0.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/mergeandmark/mergeandmark_4_0.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/mergeandmark/mergeandmark_4_1_3.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/mergeandmark/mergeandmark_4_1_3.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/bwaaligner.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/bwaaligner.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/splitmultiallele.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/splitmultiallele.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/bwamem_samtoolsview.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/bwamem_samtoolsview.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/common/indexfasta.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/common/indexfasta.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/io_lib/scramble/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/io_lib/scramble/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/validation/performancevalidator.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/validation/performancevalidator.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/star/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/star/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/filtermutectcalls/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/filtermutectcalls/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/filtermutectcalls/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/filtermutectcalls/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/gatk4toolbase.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/gatk4toolbase.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergesamfiles/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergesamfiles/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergesamfiles/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergesamfiles/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/createsequencedictionary/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/createsequencedictionary/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/createsequencedictionary/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/createsequencedictionary/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/applybqsr/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/applybqsr/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/fastqtosam/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/fastqtosam/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/fastqtosam/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/fastqtosam/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/markduplicates/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/markduplicates/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/markduplicates/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/markduplicates/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/sortsam/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/sortsam/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/printreads/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/printreads/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/printreads/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/printreads/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/splitreads/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/splitreads/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/calculatecontaminations/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/calculatecontaminations/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/calculatecontaminations/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/calculatecontaminations/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergebamalignment/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergebamalignment/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergebamalignment/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergebamalignment/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/baserecalibrator/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/baserecalibrator/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/baserecalibrator/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/baserecalibrator/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/genotypeconcordance/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/genotypeconcordance/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/genotypeconcordance/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/genotypeconcordance/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/getpileupsummaries/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/getpileupsummaries/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/getpileupsummaries/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/getpileupsummaries/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/haplotypecaller/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/haplotypecaller/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/haplotypecaller/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/haplotypecaller/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mutect2/base_4_0.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mutect2/base_4_0.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mutect2/base_4_1.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mutect2/base_4_1.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mutect2/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mutect2/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/learnreadorientationmodel/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/learnreadorientationmodel/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/learnreadorientationmodel/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/learnreadorientationmodel/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/__init__.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/__init__.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/mergemutectstats/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/mergemutectstats/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/gathervcfs/base_compressed.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/gathervcfs/base_compressed.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/gathervcfs/versions.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/gathervcfs/versions.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/gatk4/gathervcfs/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/gatk4/gathervcfs/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/babrahambioinformatics/fastqc/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/babrahambioinformatics/fastqc/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/biobambam/bamsormadup/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/biobambam/bamsormadup/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/ucsf/cnvkit/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/ucsf/cnvkit/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfallelicprimitives/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfallelicprimitives/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcffixup/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcffixup/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfroc/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfroc/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfuniqalleles/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfuniqalleles/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfrandomsample/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfrandomsample/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/vcflib/vcfuniq/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/vcflib/vcfuniq/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bwa/index/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bwa/index/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/bwa/mem/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/bwa/mem/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/strelkasomatic/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/strelkasomatic/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/strelkagermline/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/strelkagermline/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/manta/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/manta/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/illumina/happy/happybase.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/illumina/happy/happybase.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/gatk/gatksomatic_variants_4_0_12.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/gatk/gatksomatic_variants_4_0_12.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/gatk/gatkgermline_variants_4_0_12.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/gatk/gatkgermline_variants_4_0_12.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/gatk/gatksomatic_variants_4_1_3.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/gatk/gatksomatic_variants_4_1_3.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/gatk/gatkgermline_variants_4_1_3.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/gatk/gatkgermline_variants_4_1_3.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/gridssgermline.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/gridssgermline.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/vardictgermline_variants.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/vardictgermline_variants.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/vardictsomatic_variants.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/vardictsomatic_variants.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/illuminagermline_strelka.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/illuminagermline_strelka.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/variantcallers/illuminasomatic_strelka.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/variantcallers/illuminasomatic_strelka.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/sort/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/sort/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/index/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/index/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/index/__init__.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/index/__init__.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/faidx/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/faidx/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/view/base.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/view/base.py`

 * *Files identical despite different names*

### Comparing `janis-pipelines.bioinformatics-0.9.8/janis_bioinformatics/tools/samtools/samtoolstoolbase.py` & `janis-pipelines.bioinformatics-0.9.9/janis_bioinformatics/tools/samtools/samtoolstoolbase.py`

 * *Files identical despite different names*

