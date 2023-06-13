# Comparing `tmp/lens_metric-0.1.0.tar.gz` & `tmp/lens_metric-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lens_metric-0.1.0.tar", last modified: Fri Mar  3 02:13:24 2023, max compression
+gzip compressed data, was "lens_metric-0.1.1.tar", last modified: Tue Jun 13 21:26:52 2023, max compression
```

## Comparing `lens_metric-0.1.0.tar` & `lens_metric-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,32 @@
-drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-03-03 02:13:24.503478 lens_metric-0.1.0/
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     9693 2023-03-02 20:35:12.000000 lens_metric-0.1.0/LICENSE
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      424 2023-03-03 02:13:24.508478 lens_metric-0.1.0/PKG-INFO
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     1665 2023-03-03 01:50:47.000000 lens_metric-0.1.0/README.md
-drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-03-03 02:13:24.402478 lens_metric-0.1.0/lens/
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)        0 2023-03-03 01:50:47.000000 lens_metric-0.1.0/lens/__init__.py
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     1169 2023-03-03 01:50:47.000000 lens_metric-0.1.0/lens/lens_score.py
-drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-03-03 02:13:24.487478 lens_metric-0.1.0/lens_metric.egg-info/
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      424 2023-03-03 02:13:24.000000 lens_metric-0.1.0/lens_metric.egg-info/PKG-INFO
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      246 2023-03-03 02:13:24.000000 lens_metric-0.1.0/lens_metric.egg-info/SOURCES.txt
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)        1 2023-03-03 02:13:24.000000 lens_metric-0.1.0/lens_metric.egg-info/dependency_links.txt
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      178 2023-03-03 02:13:24.000000 lens_metric-0.1.0/lens_metric.egg-info/requires.txt
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)        5 2023-03-03 02:13:24.000000 lens_metric-0.1.0/lens_metric.egg-info/top_level.txt
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)       79 2023-03-03 02:13:24.516479 lens_metric-0.1.0/setup.cfg
--rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      832 2023-03-03 02:11:50.000000 lens_metric-0.1.0/setup.py
+drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-06-13 21:26:52.777818 lens_metric-0.1.1/
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     9693 2023-06-13 21:20:38.000000 lens_metric-0.1.1/LICENSE
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      424 2023-06-13 21:26:52.780818 lens_metric-0.1.1/PKG-INFO
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     1677 2023-06-13 21:20:38.000000 lens_metric-0.1.1/README.md
+drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-06-13 21:26:52.350815 lens_metric-0.1.1/lens/
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)        0 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/__init__.py
+drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-06-13 21:26:52.427816 lens_metric-0.1.1/lens/encoders/
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      757 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/encoders/__init__.py
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     2959 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/encoders/base.py
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     3482 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/encoders/bert.py
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     2206 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/encoders/roberta.py
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     1169 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/lens_score.py
+drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-06-13 21:26:52.572817 lens_metric-0.1.1/lens/models/
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     1612 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/models/__init__.py
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)    22468 2023-06-13 21:20:38.000000 lens_metric-0.1.1/lens/models/base.py
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     8990 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/models/lru_cache.py
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     3703 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/models/metrics.py
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     2266 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/models/pooling_utils.py
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      599 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/models/predict_pbar.py
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)    12439 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/models/regression_metric_multi_ref.py
+drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-06-13 21:26:52.640817 lens_metric-0.1.1/lens/modules/
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      104 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/modules/__init__.py
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     2549 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/modules/feedforward.py
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)     5125 2023-06-13 21:20:39.000000 lens_metric-0.1.1/lens/modules/layerwise_attention.py
+drwxr-xr-x   0 mmaddela3 (448703) gtperson  (2626)        0 2023-06-13 21:26:52.759818 lens_metric-0.1.1/lens_metric.egg-info/
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      424 2023-06-13 21:26:51.000000 lens_metric-0.1.1/lens_metric.egg-info/PKG-INFO
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      622 2023-06-13 21:26:52.000000 lens_metric-0.1.1/lens_metric.egg-info/SOURCES.txt
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)        1 2023-06-13 21:26:52.000000 lens_metric-0.1.1/lens_metric.egg-info/dependency_links.txt
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      178 2023-06-13 21:26:52.000000 lens_metric-0.1.1/lens_metric.egg-info/requires.txt
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)        5 2023-06-13 21:26:52.000000 lens_metric-0.1.1/lens_metric.egg-info/top_level.txt
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)       79 2023-06-13 21:26:52.792818 lens_metric-0.1.1/setup.cfg
+-rw-r--r--   0 mmaddela3 (448703) gtperson  (2626)      855 2023-06-13 21:20:39.000000 lens_metric-0.1.1/setup.py
```

### Comparing `lens_metric-0.1.0/LICENSE` & `lens_metric-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lens_metric-0.1.0/README.md` & `lens_metric-0.1.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 We leveraged the code of [COMET metric](https://github.com/Unbabel/COMET) to implement LENS.
 
 ## Installation Instructions
 
 Install from pypi with pip by
 
 ```bash
-pip install lens
+pip install lens-metric
 ```
 
 Install it from the source by:
 
 ```bash
 git clone https://github.com/Yao-Dou/LENS.git
-cd lens
+cd LENS/lens
 pip install .
 ```
 
 ### Scoring within Python:
 Please download the model checkpoint from [here](https://drive.google.com/drive/folders/1unqQ_bpUjOdXcjTV6YmgCWF3l0sMcCvv), which corresponds to the LENS(k=3) metric in our paper.
 
 ```python
```

### Comparing `lens_metric-0.1.0/lens/lens_score.py` & `lens_metric-0.1.1/lens/lens_score.py`

 * *Files identical despite different names*

### Comparing `lens_metric-0.1.0/setup.py` & `lens_metric-0.1.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,19 +1,19 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 setup(
     name='lens_metric',
-    version='0.1.0',
+    version='0.1.1',
     description='A new metric for text simplification',
     author='Mounica Maddela',
     author_email='mmaddela3@gatech.edu',
     url='https://github.com/Yao-Dou/LENS',
-    download_url='https://github.com/Yao-Dou/LENS/archive/refs/tags/v0.1.0.tar.gz',
+    download_url='https://github.com/Yao-Dou/LENS/archive/refs/tags/v0.1.1.tar.gz',
     license='Apache license',
-    packages=['lens'],
+    packages=find_packages(),
     install_requires=[
         "sentencepiece==0.1.96",
         "pandas==1.1.5",
         "transformers>=4.8",
         "pytorch-lightning==1.6.0",
         "jsonargparse==3.13.1",
         "torch >=1.6.0,<2",
@@ -22,8 +22,8 @@
         "sacrebleu >= 2.0.0",
         "scipy >=1.5.4" ],
 
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
     ],
-)
+)
```

