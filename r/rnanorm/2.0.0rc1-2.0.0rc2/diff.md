# Comparing `tmp/rnanorm-2.0.0rc1.tar.gz` & `tmp/rnanorm-2.0.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rnanorm-2.0.0rc1.tar", last modified: Mon Jun 12 08:22:10 2023, max compression
+gzip compressed data, was "rnanorm-2.0.0rc2.tar", last modified: Tue Jun 13 13:52:51 2023, max compression
```

## Comparing `rnanorm-2.0.0rc1.tar` & `rnanorm-2.0.0rc2.tar`

### file list

```diff
@@ -1,59 +1,60 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.215154 rnanorm-2.0.0rc1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.207154 rnanorm-2.0.0rc1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.211154 rnanorm-2.0.0rc1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/.github/workflows/build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-12 08:22:10.215154 rnanorm-2.0.0rc1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.211154 rnanorm-2.0.0rc1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/docs/guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/docs/ref.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1770 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-12 08:22:10.215154 rnanorm-2.0.0rc1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.211154 rnanorm-2.0.0rc1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.211154 rnanorm-2.0.0rc1/src/rnanorm/
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5152 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.211154 rnanorm-2.0.0rc1/src/rnanorm/files/
--rw-r--r--   0 runner    (1001) docker     (123)    74590 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/files/gencode.v26.annotation.chr21.gtf.gz
--rw-r--r--   0 runner    (1001) docker     (123)    23755 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/files/gtex_lung.first30.chr21.csv.gz
--rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/files/prepare_gtex.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.215154 rnanorm-2.0.0rc1/src/rnanorm/methods/
--rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/methods/between_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/methods/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5762 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/methods/within_sample.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/src/rnanorm/typing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.211154 rnanorm-2.0.0rc1/src/rnanorm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-12 08:22:10.000000 rnanorm-2.0.0rc1/src/rnanorm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1159 2023-06-12 08:22:10.000000 rnanorm-2.0.0rc1/src/rnanorm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 08:22:10.000000 rnanorm-2.0.0rc1/src/rnanorm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-12 08:22:10.000000 rnanorm-2.0.0rc1/src/rnanorm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-12 08:22:10.000000 rnanorm-2.0.0rc1/src/rnanorm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 08:22:10.000000 rnanorm-2.0.0rc1/src/rnanorm.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.215154 rnanorm-2.0.0rc1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 08:22:10.215154 rnanorm-2.0.0rc1/tests/files/
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/files/gtex.lung.30.chr21.tmm_factors_edgeR.tsv
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/files/gtex.lung.30.chr21.uq_factors_edgeR.tsv
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_annotation.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_cpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_ctf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_cuf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_datasets.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_fpkm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_library_size.py
--rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_tmm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_tpm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tests/test_uq.py
--rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-12 08:21:56.000000 rnanorm-2.0.0rc1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:52:51.690254 rnanorm-2.0.0rc2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:52:51.686254 rnanorm-2.0.0rc2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      215 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:52:51.686254 rnanorm-2.0.0rc2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/.github/workflows/build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-13 13:52:51.690254 rnanorm-2.0.0rc2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3524 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:52:51.686254 rnanorm-2.0.0rc2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1487 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2230 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/docs/guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/docs/ref.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1900 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-13 13:52:51.690254 rnanorm-2.0.0rc2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:52:51.686254 rnanorm-2.0.0rc2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:52:51.686254 rnanorm-2.0.0rc2/src/rnanorm/
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/src/rnanorm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/src/rnanorm/annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6311 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/src/rnanorm/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4073 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/src/rnanorm/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:52:51.690254 rnanorm-2.0.0rc2/src/rnanorm/files/
+-rw-r--r--   0 runner    (1001) docker     (123)    74590 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/src/rnanorm/files/gencode.v26.annotation.chr21.gtf.gz
+-rw-r--r--   0 runner    (1001) docker     (123)    23755 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/src/rnanorm/files/gtex_lung.first30.chr21.csv.gz
+-rw-r--r--   0 runner    (1001) docker     (123)     2685 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/src/rnanorm/files/prepare_gtex.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:52:51.690254 rnanorm-2.0.0rc2/src/rnanorm/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/src/rnanorm/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15954 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/src/rnanorm/methods/between_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/src/rnanorm/methods/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/src/rnanorm/methods/within_sample.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/src/rnanorm/typing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:52:51.690254 rnanorm-2.0.0rc2/src/rnanorm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-06-13 13:52:51.000000 rnanorm-2.0.0rc2/src/rnanorm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-06-13 13:52:51.000000 rnanorm-2.0.0rc2/src/rnanorm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:52:51.000000 rnanorm-2.0.0rc2/src/rnanorm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-06-13 13:52:51.000000 rnanorm-2.0.0rc2/src/rnanorm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-13 13:52:51.000000 rnanorm-2.0.0rc2/src/rnanorm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 13:52:51.000000 rnanorm-2.0.0rc2/src/rnanorm.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:52:51.690254 rnanorm-2.0.0rc2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:52:51.690254 rnanorm-2.0.0rc2/tests/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tests/files/gtex.lung.30.chr21.tmm_factors_edgeR.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tests/files/gtex.lung.30.chr21.uq_factors_edgeR.tsv
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tests/test_annotation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tests/test_cpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tests/test_ctf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tests/test_cuf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1240 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tests/test_datasets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tests/test_fpkm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tests/test_library_size.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2084 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tests/test_tmm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tests/test_tpm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2106 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tests/test_uq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-13 13:52:41.000000 rnanorm-2.0.0rc2/tox.ini
```

### Comparing `rnanorm-2.0.0rc1/.github/workflows/build.yml` & `rnanorm-2.0.0rc2/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/LICENSE` & `rnanorm-2.0.0rc2/LICENSE`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/PKG-INFO` & `rnanorm-2.0.0rc2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rnanorm
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Common RNAseq normalization methods
 Author: Genialis, Inc.
 Author-email: dev-team@genialis.com
 License: Proprietary
 Project-URL: repository, https://github.com/genialis/RNAnorm
 Keywords: bio,bioinformatics,data science,machine learning,artificial intelligence,python,genialis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rnanorm-2.0.0rc1/README.rst` & `rnanorm-2.0.0rc2/README.rst`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/docs/conf.py` & `rnanorm-2.0.0rc2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/docs/contributing.rst` & `rnanorm-2.0.0rc2/docs/contributing.rst`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/pyproject.toml` & `rnanorm-2.0.0rc2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -79,7 +79,14 @@
 
 [tool.isort]
 profile = "black"
 
 [tool.pydocstyle]
 add-select = "D404"
 add-ignore = "D202"
+
+[tool.mypy]
+ignore_missing_imports = true
+strict = true
+pretty = true
+no_warn_return_any = true
+disallow_subclassing_any = false
```

### Comparing `rnanorm-2.0.0rc1/src/rnanorm/annotation.py` & `rnanorm-2.0.0rc2/src/rnanorm/annotation.py`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/src/rnanorm/cli.py` & `rnanorm-2.0.0rc2/src/rnanorm/cli.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,49 +1,64 @@
 """Command line interface."""
 import functools
 import io
 import sys
 from pathlib import Path
-from typing import Any, Callable, Type, Union
+from typing import Any, Callable, Optional, Type, Union
 
 import click
 import pandas as pd
 
 from rnanorm import CPM, CTF, CUF, FPKM, TMM, TPM, UQ
 
 method_type = Type[Union[CPM, FPKM, TMM, TPM, UQ]]
-out_type = Union[io.TextIOWrapper, Path]
+file_type = Union[io.TextIOWrapper, Path]
 
 
 class CLWrapper:
     """Input / output wrapper around normalization methods."""
 
     def __init__(self, method: method_type, **kwargs: Any) -> None:
         """Initialize class."""
         self.method = method
         self.kwargs = kwargs
 
-    def handle(self, exp: pd.DataFrame, out: out_type, force: bool) -> None:
-        """Parse, tranasform and write out the results.."""
+    def handle(self, exp: file_type, out: file_type, force: bool) -> None:
+        """Parse, transform and write out the results."""
         X = self.parse_exp(exp)
+
+        # Turn ``--gene-lengths`` (CLI option, a file object) into
+        # ``gene_lengths`` (TPM / FPKM method argument, a Series)
+        if self.kwargs.get("gene_lengths", None) is not None:
+            self.kwargs["gene_lengths"] = self.parse_gene_lengths(self.kwargs["gene_lengths"])
+
         normalization = self.method(**self.kwargs).set_output(transform="pandas")
         result = normalization.fit_transform(X)
         self.write_out(out, result, force)
 
-    def parse_exp(self, exp: pd.DataFrame) -> pd.DataFrame:
+    def parse_exp(self, exp: file_type) -> pd.DataFrame:
         """Parse expression matrix into a DataFrame."""
         if exp.name != "<stdin>":
             if not Path(exp.name).exists():
                 raise ValueError(f"File {exp.name} does not exist.")
             if not Path(exp.name).is_file():
                 raise ValueError(f"File {exp.name} is not a file.")
 
         return pd.read_csv(exp, index_col=0)
 
-    def write_out(self, out: out_type, result: pd.DataFrame, force: bool = False) -> None:
+    def parse_gene_lengths(self, gene_lengths_file: file_type) -> pd.DataFrame:
+        """Parse gene lengths file into a Series object."""
+        if not Path(gene_lengths_file.name).exists():
+            raise ValueError(f"File {gene_lengths_file.name} does not exist.")
+        if not Path(gene_lengths_file.name).is_file():
+            raise ValueError(f"File {gene_lengths_file.name} is not a file.")
+
+        return pd.read_csv(gene_lengths_file, index_col=0).iloc[:, 0]
+
+    def write_out(self, out: file_type, result: pd.DataFrame, force: bool = False) -> None:
         """Write the resulting DataFrame to a file or stdout."""
         if out.name != "<stdout>":
             if Path(out.name).is_dir():
                 raise ValueError(f"File {out.name} is a directory.")
             elif Path(out.name).exists() and not force:
                 raise ValueError(
                     f"File {out.name} already exists. Use --force parameter to overwrite"
@@ -75,17 +90,23 @@
 
 def gtf_param(func: Callable[..., Any]) -> Callable[..., Any]:
     """Set parameters for normalization methods that require a GTF file."""
 
     @click.option(
         "--gtf",
         type=click.File("r"),
-        required=True,
+        required=False,
         help="Compute gene lengths from this GTF file",
     )
+    @click.option(
+        "--gene-lengths",
+        type=click.File("r"),
+        required=False,
+        help="File with gene lengths",
+    )
     @functools.wraps(func)
     def wrapper(*args: Any, **kwargs: Any) -> Callable[..., Any]:
         return func(*args, **kwargs)
 
     return wrapper
 
 
@@ -99,61 +120,73 @@
         return func(*args, **kwargs)
 
     return wrapper
 
 
 @click.command()
 @common_params
-def cpm(exp: pd.DataFrame, out: out_type, force: bool) -> None:
+def cpm(exp: pd.DataFrame, out: file_type, force: bool) -> None:
     """Compute CPM."""
     CLWrapper(CPM).handle(exp, out, force)
 
 
 @click.command()
 @common_params
 @gtf_param
-def fpkm(exp: pd.DataFrame, out: out_type, force: bool, gtf: io.TextIOWrapper) -> None:
+def fpkm(
+    exp: pd.DataFrame,
+    out: file_type,
+    force: bool,
+    gtf: Optional[io.TextIOWrapper] = None,
+    gene_lengths: Optional[io.TextIOWrapper] = None,
+) -> None:
     """Compute FPKM."""
-    CLWrapper(FPKM, gtf=gtf).handle(exp, out, force)
+    CLWrapper(FPKM, gtf=gtf, gene_lengths=gene_lengths).handle(exp, out, force)
 
 
 @click.command()
 @common_params
 @gtf_param
-def tpm(exp: pd.DataFrame, out: out_type, force: bool, gtf: io.TextIOWrapper) -> None:
+def tpm(
+    exp: pd.DataFrame,
+    out: file_type,
+    force: bool,
+    gtf: Optional[io.TextIOWrapper] = None,
+    gene_lengths: Optional[io.TextIOWrapper] = None,
+) -> None:
     """Compute TPM."""
-    CLWrapper(TPM, gtf=gtf).handle(exp, out, force)
+    CLWrapper(TPM, gtf=gtf, gene_lengths=gene_lengths).handle(exp, out, force)
 
 
 @click.command()
 @common_params
-def uq(exp: pd.DataFrame, out: out_type, force: bool) -> None:
+def uq(exp: pd.DataFrame, out: file_type, force: bool) -> None:
     """Compute UQ."""
     CLWrapper(UQ).handle(exp, out, force)
 
 
 @click.command()
 @common_params
-def cuf(exp: pd.DataFrame, out: out_type, force: bool) -> None:
+def cuf(exp: pd.DataFrame, out: file_type, force: bool) -> None:
     """Compute CUF."""
     CLWrapper(CUF).handle(exp, out, force)
 
 
 @click.command()
 @common_params
 @tmm_params
-def tmm(exp: pd.DataFrame, out: out_type, force: bool, m_trim: float, a_trim: float) -> None:
+def tmm(exp: pd.DataFrame, out: file_type, force: bool, m_trim: float, a_trim: float) -> None:
     """Compute TMM."""
     CLWrapper(TMM, m_trim=m_trim, a_trim=a_trim).handle(exp, out, force)
 
 
 @click.command()
 @common_params
 @tmm_params
-def ctf(exp: pd.DataFrame, out: out_type, force: bool, m_trim: float, a_trim: float) -> None:
+def ctf(exp: pd.DataFrame, out: file_type, force: bool, m_trim: float, a_trim: float) -> None:
     """Compute CTF."""
     CLWrapper(CTF, m_trim=m_trim, a_trim=a_trim).handle(exp, out, force)
 
 
 @click.group()
 def main() -> None:
     """Define main entry point for CLI."""
```

### Comparing `rnanorm-2.0.0rc1/src/rnanorm/datasets.py` & `rnanorm-2.0.0rc2/src/rnanorm/datasets.py`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/src/rnanorm/files/gencode.v26.annotation.chr21.gtf.gz` & `rnanorm-2.0.0rc2/src/rnanorm/files/gencode.v26.annotation.chr21.gtf.gz`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/src/rnanorm/files/gtex_lung.first30.chr21.csv.gz` & `rnanorm-2.0.0rc2/src/rnanorm/files/gtex_lung.first30.chr21.csv.gz`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/src/rnanorm/files/prepare_gtex.py` & `rnanorm-2.0.0rc2/src/rnanorm/files/prepare_gtex.py`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/src/rnanorm/methods/between_sample.py` & `rnanorm-2.0.0rc2/src/rnanorm/methods/between_sample.py`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/src/rnanorm/methods/utils.py` & `rnanorm-2.0.0rc2/src/rnanorm/methods/utils.py`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/src/rnanorm/methods/within_sample.py` & `rnanorm-2.0.0rc2/src/rnanorm/methods/within_sample.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Within sample normalization: CPM, FPKM and TPM."""
 import warnings
 from pathlib import Path
-from typing import Union
+from typing import Optional, Union
 
 import numpy as np
+import pandas as pd
 from sklearn.preprocessing import FunctionTransformer
 
 from ..annotation import GTF
 from ..typing import Numeric1D, Numeric2D
 from .utils import LibrarySize
 
 
@@ -73,30 +74,55 @@
             kwargs["force_all_finite"] = "allow-nan"
         return self._validate_data(X, reset=reset, **kwargs)
 
 
 class BaseNormalizationWithGTF(FunctionTransformer):
     """Normalize raw counts."""
 
-    def __init__(self, gtf: Union[str, Path]) -> None:
+    def __init__(
+        self,
+        gtf: Optional[Union[str, Path]] = None,
+        gene_lengths: Optional[pd.Series] = None,
+    ) -> None:
         """Initialize class."""
+        if (gtf is None and gene_lengths is None) or (
+            gtf is not None and gene_lengths is not None
+        ):
+            raise ValueError("One and only one of gtf or gene_lengths should be provided")
+        self.gene_lengths = gene_lengths
         self.gtf = gtf
         super().__init__(
             func=self._func,
             validate=True,
             feature_names_out="one-to-one",
         )
 
     def _get_gene_lengths(self, X: Numeric2D) -> Numeric1D:
         """Check and correct X and gene lengths."""
-        # gene_lengths is a pandas.Series object
-        gene_lengths = GTF(self.gtf).length
+        # gene_lengths should be a pandas.Series object with gene ID's in index
+        # and gene lengths in values.
+        if self.gtf:
+            gene_lengths = GTF(self.gtf).length
+        else:
+            # Validate gene lengths
+            if not isinstance(self.gene_lengths, pd.Series):
+                raise ValueError("gene_lengths should be a pandas.Series object")
+            if not self.gene_lengths.index.is_unique:
+                raise ValueError("gene_lengths should have unique index")
+            if not self.gene_lengths.ge(0).all():
+                raise ValueError("gene_lengths should only contain positive numbers")
+            if not (self.gene_lengths - self.gene_lengths.astype(int)).sum() == 0:
+                raise ValueError("gene_lengths should only contain integers")
+            gene_lengths = self.gene_lengths
 
         missing = set(self.feature_names_in_) - set(gene_lengths.index)
         if missing:
+            if len(missing) == len(self.feature_names_in_):
+                container = "gtf" if self.gtf is not None else "gene_lengths"
+                raise ValueError(f"None of the genes in X are in {container}.")
             warnings.warn(
                 f"X contains {len(missing)} genes that are not in GTF "
                 f"{self.gtf}. This will result in NaN values for missing "
                 "genes in the output."
             )
 
         return gene_lengths.reindex(index=self.feature_names_in_).to_numpy()
```

### Comparing `rnanorm-2.0.0rc1/src/rnanorm.egg-info/PKG-INFO` & `rnanorm-2.0.0rc2/src/rnanorm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rnanorm
-Version: 2.0.0rc1
+Version: 2.0.0rc2
 Summary: Common RNAseq normalization methods
 Author: Genialis, Inc.
 Author-email: dev-team@genialis.com
 License: Proprietary
 Project-URL: repository, https://github.com/genialis/RNAnorm
 Keywords: bio,bioinformatics,data science,machine learning,artificial intelligence,python,genialis
 Classifier: Development Status :: 4 - Beta
```

### Comparing `rnanorm-2.0.0rc1/src/rnanorm.egg-info/SOURCES.txt` & `rnanorm-2.0.0rc2/src/rnanorm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 .readthedocs.yaml
 LICENSE
 MANIFEST.in
 README.rst
 pyproject.toml
 setup.cfg
 tox.ini
+.github/dependabot.yml
 .github/workflows/build.yml
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/guide.rst
 docs/index.rst
 docs/ref.rst
```

### Comparing `rnanorm-2.0.0rc1/tests/conftest.py` & `rnanorm-2.0.0rc2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/tests/files/gtex.lung.30.chr21.tmm_factors_edgeR.tsv` & `rnanorm-2.0.0rc2/tests/files/gtex.lung.30.chr21.tmm_factors_edgeR.tsv`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/tests/files/gtex.lung.30.chr21.uq_factors_edgeR.tsv` & `rnanorm-2.0.0rc2/tests/files/gtex.lung.30.chr21.uq_factors_edgeR.tsv`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/tests/test_cli.py` & `rnanorm-2.0.0rc2/tests/test_cli.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
+import os
 import subprocess
 from io import StringIO
 
 import pandas as pd
 import pytest
 
 from rnanorm import CPM, CTF, CUF, FPKM, TMM, TPM, UQ
+from rnanorm.annotation import GTF
 
 
 @pytest.fixture
 def exp_path(tmp_path, exp):
     exp_path = tmp_path / "exp.csv"
 
     # This si to prevent warnings for missing gene in TPM / FPKM
@@ -22,14 +24,22 @@
 def out_path(tmp_path):
     out_path = tmp_path / "out.csv"
     yield out_path
     # Remove file after test
     out_path.unlink(missing_ok=True)
 
 
+@pytest.fixture
+def gene_lengths_file(tmp_path, gtf_file):
+    out_path = tmp_path / "gene_lengths.csv"
+    gene_lengths = GTF(gtf_file).length
+    gene_lengths.to_csv(out_path)
+    return out_path
+
+
 def test_files_in_out(exp_path, out_path):
     assert not out_path.is_file()
     cp = subprocess.run(["rnanorm", "cpm", str(exp_path), "--out", str(out_path)])
     assert out_path.is_file()
     assert cp.returncode == 0
 
 
@@ -62,40 +72,84 @@
     assert cp.returncode == 0
     pd.testing.assert_frame_equal(
         pd.read_csv(out_path, index_col=0),
         CPM().set_output(transform="pandas").fit_transform(exp),
     )
 
 
-def test_fpkm(exp, exp_path, gtf_file, out_path):
+def test_fpkm(exp, exp_path, gtf_file, out_path, gene_lengths_file):
     assert not out_path.is_file()
 
     cp = subprocess.run(
         ["rnanorm", "fpkm", str(exp_path), "--out", str(out_path), "--gtf", str(gtf_file)]
     )
     assert out_path.is_file()
     assert cp.returncode == 0
     pd.testing.assert_frame_equal(
         pd.read_csv(out_path, index_col=0),
         FPKM(gtf=gtf_file).set_output(transform="pandas").fit_transform(exp),
     )
 
+    # Test also with gene lengths file
+    os.remove(out_path)
+    assert not out_path.is_file()
+
+    cp = subprocess.run(
+        [
+            "rnanorm",
+            "fpkm",
+            str(exp_path),
+            "--out",
+            str(out_path),
+            "--gene-lengths",
+            str(gene_lengths_file),
+        ]
+    )
+    assert out_path.is_file()
+    assert cp.returncode == 0
+    pd.testing.assert_frame_equal(
+        pd.read_csv(out_path, index_col=0),
+        FPKM(gtf=gtf_file).set_output(transform="pandas").fit_transform(exp),
+    )
 
-def test_tpm(exp, exp_path, gtf_file, out_path):
+
+def test_tpm(exp, exp_path, gtf_file, out_path, gene_lengths_file):
     assert not out_path.is_file()
 
     cp = subprocess.run(
         ["rnanorm", "tpm", str(exp_path), "--out", str(out_path), "--gtf", str(gtf_file)]
     )
     assert out_path.is_file()
     assert cp.returncode == 0
     pd.testing.assert_frame_equal(
         pd.read_csv(out_path, index_col=0),
         TPM(gtf=gtf_file).set_output(transform="pandas").fit_transform(exp),
     )
+
+    # Test also with gene lengths file
+    os.remove(out_path)
+    assert not out_path.is_file()
+
+    cp = subprocess.run(
+        [
+            "rnanorm",
+            "tpm",
+            str(exp_path),
+            "--out",
+            str(out_path),
+            "--gene-lengths",
+            str(gene_lengths_file),
+        ]
+    )
+    assert out_path.is_file()
+    assert cp.returncode == 0
+    pd.testing.assert_frame_equal(
+        pd.read_csv(out_path, index_col=0),
+        TPM(gtf=gtf_file).set_output(transform="pandas").fit_transform(exp),
+    )
 
 
 def test_uq(exp, exp_path, out_path):
     assert not out_path.is_file()
 
     cp = subprocess.run(["rnanorm", "uq", str(exp_path), "--out", str(out_path)])
     assert out_path.is_file()
```

### Comparing `rnanorm-2.0.0rc1/tests/test_cpm.py` & `rnanorm-2.0.0rc2/tests/test_cpm.py`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/tests/test_ctf.py` & `rnanorm-2.0.0rc2/tests/test_ctf.py`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/tests/test_cuf.py` & `rnanorm-2.0.0rc2/tests/test_cuf.py`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/tests/test_datasets.py` & `rnanorm-2.0.0rc2/tests/test_datasets.py`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/tests/test_fpkm.py` & `rnanorm-2.0.0rc2/tests/test_fpkm.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pandas as pd
 import pytest
 
 from rnanorm import FPKM
+from rnanorm.annotation import GTF
 
 
 @pytest.fixture
 def expected(exp):
     return pd.DataFrame(
         [
             [100000, 100000, 100000, 200000, np.nan],
@@ -36,7 +37,20 @@
     assert isinstance(exp_normalized, pd.DataFrame)
     pd.testing.assert_frame_equal(exp_normalized, expected)
 
     # Validation refuses nan values
     exp.iloc[0, 0] = np.nan
     with pytest.raises(ValueError, match="Input X contains NaN."):
         transformer.fit_transform(exp)
+
+
+def test_fpkm_gene_lengths(exp, expected, gtf_file):
+    gene_lengths = GTF(gtf=gtf_file).length
+
+    transformer = FPKM(gene_lengths=gene_lengths)
+    transformer.set_output(transform="pandas")
+
+    with pytest.warns(UserWarning, match=r"X contains .* genes that are not ."):
+        exp_normalized = transformer.fit_transform(exp)
+
+    assert isinstance(exp_normalized, pd.DataFrame)
+    pd.testing.assert_frame_equal(exp_normalized, expected)
```

### Comparing `rnanorm-2.0.0rc1/tests/test_library_size.py` & `rnanorm-2.0.0rc2/tests/test_library_size.py`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/tests/test_tmm.py` & `rnanorm-2.0.0rc2/tests/test_tmm.py`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/tests/test_tpm.py` & `rnanorm-2.0.0rc2/tests/test_tpm.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import numpy as np
 import pandas as pd
 import pytest
 
 from rnanorm import TPM
+from rnanorm.annotation import GTF
 
 
 @pytest.fixture
 def expected(exp):
     return pd.DataFrame(
         [
             [200000, 200000, 200000, 400000, np.nan],
@@ -36,7 +37,20 @@
     assert isinstance(exp_normalized, pd.DataFrame)
     pd.testing.assert_frame_equal(exp_normalized, expected)
 
     # Validation refuses nan values
     exp.iloc[0, 0] = np.nan
     with pytest.raises(ValueError, match="Input X contains NaN."):
         transformer.fit_transform(exp)
+
+
+def test_tpm_gene_lengths(exp, expected, gtf_file):
+    gene_lengths = GTF(gtf=gtf_file).length
+
+    transformer = TPM(gene_lengths=gene_lengths)
+    transformer.set_output(transform="pandas")
+
+    with pytest.warns(UserWarning, match=r"X contains .* genes that are not ."):
+        exp_normalized = transformer.fit_transform(exp)
+
+    assert isinstance(exp_normalized, pd.DataFrame)
+    pd.testing.assert_frame_equal(exp_normalized, expected)
```

### Comparing `rnanorm-2.0.0rc1/tests/test_uq.py` & `rnanorm-2.0.0rc2/tests/test_uq.py`

 * *Files identical despite different names*

### Comparing `rnanorm-2.0.0rc1/tox.ini` & `rnanorm-2.0.0rc2/tox.ini`

 * *Files identical despite different names*

