# Comparing `tmp/tuned-lens-0.1.0.tar.gz` & `tmp/tuned-lens-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuned-lens-0.1.0.tar", last modified: Tue May  2 01:29:34 2023, max compression
+gzip compressed data, was "tuned-lens-0.1.1.tar", last modified: Tue Jun 13 16:09:59 2023, max compression
```

## Comparing `tuned-lens-0.1.0.tar` & `tuned-lens-0.1.1.tar`

### file list

```diff
@@ -1,58 +1,58 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2115 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.905034 tuned-lens-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2533 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.905034 tuned-lens-0.1.0/tests/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      815 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/scripts/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_lenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_load_artifact.py
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_model_surgery.py
--rw-r--r--   0 runner    (1001) docker     (123)      612 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_subspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_unembed.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.905034 tuned-lens-0.1.0/tuned_lens/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/tuned_lens/causal/
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/causal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/causal/ablation.py
--rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/causal/subspaces.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/causal/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/data.py
--rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/load_artifacts.py
--rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/model_surgery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/tuned_lens/nn/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/nn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/nn/lenses.py
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/nn/unembed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/tuned_lens/plotting/
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/plotting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/plotting/prediction_trajectory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/plotting/token_formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/plotting/trajectory_plotting.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/tuned_lens/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7905 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/scripts/eval_loop.py
--rw-r--r--   0 runner    (1001) docker     (123)    11206 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/scripts/ingredients.py
--rw-r--r--   0 runner    (1001) docker     (123)    12607 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/scripts/train_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.909034 tuned-lens-0.1.0/tuned_lens/stats/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/stats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/stats/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/stats/logit_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     7536 2023-05-02 01:29:25.000000 tuned-lens-0.1.0/tuned_lens/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 01:29:34.905034 tuned-lens-0.1.0/tuned_lens.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-02 01:29:34.000000 tuned-lens-0.1.0/tuned_lens.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-02 01:29:34.000000 tuned-lens-0.1.0/tuned_lens.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 01:29:34.000000 tuned-lens-0.1.0/tuned_lens.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-02 01:29:34.000000 tuned-lens-0.1.0/tuned_lens.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-02 01:29:34.000000 tuned-lens-0.1.0/tuned_lens.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 01:29:34.000000 tuned-lens-0.1.0/tuned_lens.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.974218 tuned-lens-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-13 16:09:59.974218 tuned-lens-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3774 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:09:59.974218 tuned-lens-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.962218 tuned-lens-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2608 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.962218 tuned-lens-0.1.1/tests/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1122 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/scripts/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3842 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_lenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_load_artifact.py
+-rw-r--r--   0 runner    (1001) docker     (123)      870 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_model_surgery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      612 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_subspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_unembed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.966218 tuned-lens-0.1.1/tuned_lens/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.966218 tuned-lens-0.1.1/tuned_lens/causal/
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/causal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/causal/ablation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9031 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/causal/subspaces.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/causal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2895 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/load_artifacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6576 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/model_surgery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.970218 tuned-lens-0.1.1/tuned_lens/nn/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/nn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10172 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/nn/lenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6897 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/nn/unembed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.970218 tuned-lens-0.1.1/tuned_lens/plotting/
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/plotting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15742 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/plotting/prediction_trajectory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/plotting/token_formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/plotting/trajectory_plotting.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.970218 tuned-lens-0.1.1/tuned_lens/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12070 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/scripts/eval_loop.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13264 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/scripts/ingredients.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16609 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/scripts/train_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.974218 tuned-lens-0.1.1/tuned_lens/stats/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/stats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1857 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/stats/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4121 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/stats/logit_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7974 2023-06-13 16:09:46.000000 tuned-lens-0.1.1/tuned_lens/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:09:59.966218 tuned-lens-0.1.1/tuned_lens.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4224 2023-06-13 16:09:59.000000 tuned-lens-0.1.1/tuned_lens.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-13 16:09:59.000000 tuned-lens-0.1.1/tuned_lens.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:09:59.000000 tuned-lens-0.1.1/tuned_lens.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 16:09:59.000000 tuned-lens-0.1.1/tuned_lens.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-13 16:09:59.000000 tuned-lens-0.1.1/tuned_lens.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 16:09:59.000000 tuned-lens-0.1.1/tuned_lens.egg-info/top_level.txt
```

### Comparing `tuned-lens-0.1.0/LICENSE` & `tuned-lens-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/PKG-INFO` & `tuned-lens-0.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: tuned-lens
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for understanding how transformer predictions are built layer-by-layer
 License: MIT License
 Keywords: nlp,interpretability,language-models,explainable-ai
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
+Provides-Extra: slow_tokenizers
 Provides-Extra: notebooks
+Provides-Extra: 8bit
 License-File: LICENSE
 
 # Tuned Lens 🔎
 <a target="_blank" href="https://colab.research.google.com/github/AlignmentResearch/tuned-lens/blob/main/notebooks/interactive.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 <a target="_blank" href="https://huggingface.co/spaces/AlignmentResearch/tuned-lens">
```

### Comparing `tuned-lens-0.1.0/README.md` & `tuned-lens-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/pyproject.toml` & `tuned-lens-0.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -9,23 +9,23 @@
 requires-python = ">=3.9"
 keywords = ["nlp", "interpretability", "language-models", "explainable-ai"]
 license = {text = "MIT License"}
 dependencies = [
     "accelerate",
     "datasets",
     "plotly>=5.13.1",
-    "scikit-learn",
-    "zstandard",
+    "torchdata>=0.6.0",
     "torch>=1.13.0",
     "transformers>=4.28.1",
     "huggingface_hub>=0.12.1",
     "simple-parsing>=0.1.1",
+    "flatten-dict>=0.4.1",
     "wandb>=0.15.0",
 ]
-version = "0.1.0"
+version = "0.1.1"
 
 [project.optional-dependencies]
 dev = [
     "pre-commit",
     "bump2version",
     "pytest-skip-slow",
     "pytest",
@@ -35,23 +35,30 @@
     "myst-parser",
     "sphinx",
     "sphinx-autodoc-typehints",
     "sphinx-rtd-theme",
     "nbsphinx",
 ]
 test = [
+    "sentencepiece>=0.1.99",
     "pytest-skip-slow",
     "pytest-cov",
     "nbmake",
     "pytest",
     "mock",
 ]
+slow_tokenizers = [
+    "sentencepiece>=0.1.99"
+]
 notebooks = [
     "ipywidgets",
 ]
+8bit = [
+    "bitsandbytes",
+]
 
 [project.scripts]
 tuned-lens = "tuned_lens.__main__:main"
 
 [tool.setuptools.packages.find]
 namespaces = false
```

### Comparing `tuned-lens-0.1.0/tests/conftest.py` & `tuned-lens-0.1.1/tests/conftest.py`

 * *Files 11% similar despite different names*

```diff
@@ -76,17 +76,20 @@
     config = tr.AutoConfig.from_pretrained("facebook/opt-125m")
     model = tr.AutoModelForCausalLM.from_config(config)
     model.eval()
     return model
 
 
 @pytest.fixture(scope="module")
-def gpt2_random_model_local_path(
+def gpt2_tiny_random_model_local_path(
     tmpdir_factory, gpt2_tokenizer: tr.PreTrainedTokenizerBase
 ):
     config = tr.AutoConfig.from_pretrained("gpt2")
+    config.n_heads = 2
+    config.n_embed = 8
+    config.n_layers = 2
     model = tr.AutoModelForCausalLM.from_config(config)
     assert isinstance(model, tr.PreTrainedModel)
     tmp_path = tmpdir_factory.mktemp("gpt2_random_model_local")
     model.save_pretrained(tmp_path)
     gpt2_tokenizer.save_pretrained(tmp_path)
     return tmp_path
```

### Comparing `tuned-lens-0.1.0/tests/test_data.py` & `tuned-lens-0.1.1/tests/test_data.py`

 * *Files 16% similar despite different names*

```diff
@@ -18,14 +18,30 @@
     )
 
     length = min(small_model_tokenizer.model_max_length, max_length)
     for i in range(len(chunked)):
         assert len(chunked[i]["input_ids"]) == length
 
 
+def test_chunk_and_tokenize_slow(text_dataset: Dataset):
+    tokenizer = tr.AutoTokenizer.from_pretrained("gpt2", use_fast=False)
+
+    max_length = 128
+    chunked, _ = data.chunk_and_tokenize(
+        text_dataset,
+        tokenizer,
+        load_from_cache_file=False,
+        max_length=max_length,
+    )
+
+    length = min(tokenizer.model_max_length, max_length)
+    for i in range(len(chunked)):
+        assert len(chunked[i]["input_ids"]) == length
+
+
 def test_compute_nats_to_bpb_ratio(
     text_dataset: Dataset, gpt2_tokenizer: tr.PreTrainedTokenizerBase
 ):
     max_length = 128
     _, ratio = data.chunk_and_tokenize(
         text_dataset, gpt2_tokenizer, load_from_cache_file=True, max_length=max_length
     )
```

### Comparing `tuned-lens-0.1.0/tests/test_distance.py` & `tuned-lens-0.1.1/tests/test_distance.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tests/test_lenses.py` & `tuned-lens-0.1.1/tests/test_lenses.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 
 @pytest.fixture
 def unembed():
     mock_unembed = mock.MagicMock(Unembed)
     W = th.randn(100, 128)
     mock_unembed.forward = lambda x: th.matmul(x, W.T)
+    mock_unembed.unembedding = th.nn.Linear(128, 100)
     mock_unembed.unembedding_hash.return_value = 42
     return mock_unembed
 
 
 @pytest.fixture
 def logit_lens(unembed):
     logit_lens = LogitLens(unembed)
```

### Comparing `tuned-lens-0.1.0/tests/test_model_surgery.py` & `tuned-lens-0.1.1/tests/test_model_surgery.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tests/test_stats.py` & `tuned-lens-0.1.1/tests/test_stats.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tests/test_subspaces.py` & `tuned-lens-0.1.1/tests/test_subspaces.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tests/test_unembed.py` & `tuned-lens-0.1.1/tests/test_unembed.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tuned_lens/__main__.py` & `tuned-lens-0.1.1/tuned_lens/__main__.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tuned_lens/causal/ablation.py` & `tuned-lens-0.1.1/tuned_lens/causal/ablation.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tuned_lens/causal/subspaces.py` & `tuned-lens-0.1.1/tuned_lens/causal/subspaces.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tuned_lens/causal/utils.py` & `tuned-lens-0.1.1/tuned_lens/causal/utils.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tuned_lens/data.py` & `tuned-lens-0.1.1/tuned_lens/data.py`

 * *Files 8% similar despite different names*

```diff
@@ -53,21 +53,28 @@
             joined_text,  # start with an eos token
             max_length=chunk_size,
             return_attention_mask=False,
             return_overflowing_tokens=True,
             truncation=True,
         )
 
+        if overflow := output.pop("overflowing_tokens", None):
+            # Slow Tokenizers return unnested lists of ints
+            assert isinstance(output["input_ids"][0], int)
+
+            # Chunk the overflow into batches of size `chunk_size`
+            chunks = [output["input_ids"]] + [
+                overflow[i * chunk_size : (i + 1) * chunk_size]
+                for i in range(math.ceil(len(overflow) / chunk_size))
+            ]
+            output = {"input_ids": chunks}
+
         total_tokens = sum(len(ids) for ids in output["input_ids"])
         total_bytes = len(joined_text.encode("utf-8"))
 
-        assert (
-            "overflowing_tokens" not in output
-        ), "We should not have any overflowing tokens."
-
         if not return_final_batch:
             # We know that the last sample will almost always be less than the max
             # number of tokens, and we don't want to pad, so we just drop it.
             output = {k: v[:-1] for k, v in output.items()}
 
         output_batch_size = len(output["input_ids"])
```

### Comparing `tuned-lens-0.1.0/tuned_lens/load_artifacts.py` & `tuned-lens-0.1.1/tuned_lens/load_artifacts.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tuned_lens/model_surgery.py` & `tuned-lens-0.1.1/tuned_lens/model_surgery.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tuned_lens/nn/lenses.py` & `tuned-lens-0.1.1/tuned_lens/nn/lenses.py`

 * *Files 5% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     # The number of layers in the base model.
     num_hidden_layers: int
     # whether to use a bias in the linear translators.
     bias: bool = True
     # The revision of the base model this lens was tuned for.
     base_model_revision: Optional[str] = None
     # The hash of the base's unembed model this lens was tuned for.
-    unemebd_hash: Optional[str] = None
+    unembed_hash: Optional[str] = None
     # The name of the lens type.
     lens_type: str = "linear_tuned_lens"
 
     def to_dict(self):
         """Convert this config to a dictionary."""
         return asdict(self)
 
@@ -145,17 +145,23 @@
             unembed: The unembed operation to use.
             config: The configuration for this lens.
         """
         super().__init__(unembed)
 
         self.config = config
         unembed_hash = unembed.unembedding_hash()
-        config.unemebd_hash = unembed_hash
+        config.unembed_hash = unembed_hash
 
-        translator = th.nn.Linear(config.d_model, config.d_model, bias=config.bias)
+        # The unembedding might be int8 if we're using bitsandbytes
+        w = unembed.unembedding.weight
+        dtype = w.dtype if th.is_floating_point(w) else th.float16
+
+        translator = th.nn.Linear(
+            config.d_model, config.d_model, bias=config.bias, dtype=dtype
+        )
         translator.weight.data.zero_()
         translator.bias.data.zero_()
 
         # Don't include the final layer since it does not need a translator
         self.layer_translators = th.nn.ModuleList(
             [deepcopy(translator) for _ in range(self.config.num_hidden_layers)]
         )
@@ -251,15 +257,15 @@
             **{k: v for k, v in kwargs.items() if k in load_artifact_varnames},
         )
 
         with open(config_path, "r") as f:
             config = TunedLensConfig.from_dict(json.load(f))
 
         # validate the unembed is the same as the one used to train the lens
-        if config.unemebd_hash and unembed.unembedding_hash() != config.unemebd_hash:
+        if config.unembed_hash and unembed.unembedding_hash() != config.unembed_hash:
             warning(
                 "The unembeding matrix hash does not match the lens' hash."
                 "This lens may have been trained with a different unembedding."
             )
 
         # Create the lens
         lens = cls(unembed, config)
```

### Comparing `tuned-lens-0.1.0/tuned_lens/nn/unembed.py` & `tuned-lens-0.1.1/tuned_lens/nn/unembed.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,15 +50,15 @@
         self.unembedding = copy.deepcopy(unembeding_matrix)
 
         # In general we don't want to finetune the unembed operation.
         self.requires_grad_(False)
 
     def unembedding_hash(self) -> str:
         """Hash the unmbedding matrix to identify the model."""
-        parameter = self.unembedding.weight.data.detach().cpu().numpy()
+        parameter = self.unembedding.weight.data.detach().cpu().float().numpy()
         return tensor_hash(parameter)
 
     def forward(self, h: th.Tensor) -> th.Tensor:
         """Convert hidden states into logits."""
         return self.unembedding(self.final_norm(h))
 
     def invert(
```

### Comparing `tuned-lens-0.1.0/tuned_lens/plotting/prediction_trajectory.py` & `tuned-lens-0.1.1/tuned_lens/plotting/prediction_trajectory.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tuned_lens/plotting/token_formatter.py` & `tuned-lens-0.1.1/tuned_lens/plotting/token_formatter.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tuned_lens/plotting/trajectory_plotting.py` & `tuned-lens-0.1.1/tuned_lens/plotting/trajectory_plotting.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tuned_lens/scripts/ingredients.py` & `tuned-lens-0.1.1/tuned_lens/scripts/ingredients.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Shared configuration for the scripts."""
 import enum
 import os
 from dataclasses import dataclass
+from datetime import timedelta
 from functools import partial
 from typing import Optional, Union
 
 import torch as th
 import torch.distributed as dist
 from datasets import Dataset, DatasetDict, load_dataset
 from simple_parsing import field
@@ -13,29 +14,32 @@
     CPUOffload,
     FullyShardedDataParallel,
     MixedPrecision,
 )
 from torch.distributed.fsdp.wrap import transformer_auto_wrap_policy
 from torch.distributed.optim import ZeroRedundancyOptimizer
 from torch.nn.parallel import DistributedDataParallel as DDP
+from torchdata import dataloader2, datapipes
 from transformers import (
     AutoModelForCausalLM,
     AutoTokenizer,
     PreTrainedModel,
     PreTrainedTokenizerBase,
     get_linear_schedule_with_warmup,
 )
+from typing_extensions import Literal
 
 from tuned_lens.data import (
     chunk_and_tokenize,
 )
 from tuned_lens.model_surgery import get_transformer_layers
 from tuned_lens.nn.lenses import Lens
 from tuned_lens.utils import (
     TreeType,
+    handle_name_conflicts,
     send_to_device,
 )
 
 
 @dataclass
 class Data:
     """Configuration for the dataset."""
@@ -67,15 +71,18 @@
             dataset = load_dataset(*self.name, split=self.split, revision=self.revision)
             if not isinstance(dataset, (Dataset, DatasetDict)):
                 raise ValueError(
                     "Only Dataset and DatasetDict instances are supported."
                 )
 
         processed, nats_to_bpb = chunk_and_tokenize(
-            dataset, tokenizer, text_key=self.text_column, max_length=self.max_length
+            dataset,
+            tokenizer,
+            text_key=self.text_column,
+            max_length=self.max_length,
         )
 
         print(f"Using nats per token to bits per byte ratio: {nats_to_bpb}")
 
         assert isinstance(processed, Dataset)
 
         return processed, nats_to_bpb
@@ -84,14 +91,17 @@
 @dataclass
 class Model:
     """Configuration for the model and tokenizer."""
 
     name: str
     """Name of model to use in the Huggingface Hub."""
 
+    precision: Literal["auto", "bfloat16", "float16", "float32", "int8"] = "auto"
+    """Precision in which to load the model weights."""
+
     revision: str = "main"
     """Git revision to use for pretrained models."""
 
     slow_tokenizer: bool = field(action="store_true")
     """Use a slow tokenizer."""
 
     tokenizer: Optional[str] = None
@@ -99,37 +109,59 @@
     AutoTokenizer.from_pretrained('<model name>')."""
 
     tokenizer_type: Optional[str] = None
     """Name of tokenizer class to use. If None, will use AutoTokenizer."""
 
     def load_tokenizer(self, must_use_cache: bool = False) -> PreTrainedTokenizerBase:
         """Load the tokenizer from huggingface hub."""
-        tokenizer = AutoTokenizer.from_pretrained(
-            self.tokenizer or self.name,
-            revision=self.revision,
-            use_fast=not self.slow_tokenizer,
-            tokenizer_type=self.tokenizer_type,
-            local_files_only=must_use_cache,
-        )
+        with handle_name_conflicts():
+            tokenizer = AutoTokenizer.from_pretrained(
+                self.tokenizer or self.name,
+                revision=self.revision,
+                use_fast=not self.slow_tokenizer,
+                tokenizer_type=self.tokenizer_type,
+                local_files_only=must_use_cache,
+            )
 
         assert isinstance(tokenizer, PreTrainedTokenizerBase)
         return tokenizer
 
     def load(
-        self, must_use_cache: bool = False
+        self, device: Optional[th.device], must_use_cache: bool = False
     ) -> tuple[PreTrainedModel, PreTrainedTokenizerBase]:
-        """Load the model and tokenizer."""
+        """Load the model and tokenizer.
+
+        Args:
+            device: The device to load the model on. Implemented with the `device_map`
+                argument of `AutoModelForCausalLM.from_pretrained`.
+            must_use_cache: If True, will raise an error if the model is not cached.
+        """
         print(f"Loading pretrained weights for '{self.name}'...")
-        model = AutoModelForCausalLM.from_pretrained(  # type: ignore
-            self.name,
-            low_cpu_mem_usage=True,
-            revision=self.revision,
-            torch_dtype="auto",
-            local_files_only=must_use_cache,
-        )
+        try:
+            dtype = {
+                "auto": "auto",
+                "bfloat16": th.bfloat16,
+                "float16": th.float16,
+                "float32": th.float32,
+                # `bitsandbytes` requires weights to initially be in fp16
+                "int8": th.float16,
+            }[self.precision]
+        except KeyError as e:
+            raise ValueError(f"Unknown precision: {self.precision}") from e
+
+        with handle_name_conflicts():
+            model = AutoModelForCausalLM.from_pretrained(  # type: ignore
+                self.name,
+                device_map={"": device} if device is not None else None,
+                load_in_8bit=self.precision == "int8",
+                low_cpu_mem_usage=True,
+                revision=self.revision,
+                torch_dtype=dtype,
+                local_files_only=must_use_cache,
+            )
 
         assert isinstance(model, PreTrainedModel)
         model.eval()
         model.requires_grad_(False)
 
         return model, self.load_tokenizer(must_use_cache=must_use_cache)
 
@@ -213,25 +245,35 @@
         if self.zero:
             opt = ZeroRedundancyOptimizer(params, optimizer_class=opt_class, **config)
         else:
             opt = opt_class(params, **config)  # type: ignore[call-arg]
 
         return opt
 
+    def per_parameter_optim_state_size(self) -> int:
+        """The number of elements in the optimizer state per parameter."""
+        return 2 if self.optimizer == OptimizerOption.ADAM else 1
+
 
 @dataclass
 class Distributed:
     """Configuration and utilities for distributing the model."""
 
     fsdp: bool = field(action="store_true")
     """Run the model with Fully Sharded Data Parallelism."""
 
     cpu_offload: bool = field(action="store_true")
     """Use CPU offloading. Must be combined with fsdp"""
 
+    nccl_timeout: int = 1200  # 20 minutes
+    """Timeout for NCCL operations in seconds."""
+
+    per_gpu_batch_size: int = 1
+    """The batch size per GPU."""
+
     @property
     def rank(self) -> int:
         """The rank of this process.
 
         Note that in general this is not the same as the local rank.
         However, for single-node training, the local rank is the same as the
         global rank.
@@ -252,20 +294,24 @@
     def primary(self) -> bool:
         """Whether this is the rank 0 process."""
         return self.rank == 0
 
     @property
     def device(self) -> th.device:
         """The device associated with this process."""
-        return th.device("cuda") if th.cuda.is_available() else th.device("cpu")
+        return (
+            th.device("cuda", self.local_rank)
+            if th.cuda.is_available()
+            else th.device("cpu")
+        )
 
     def shard_model(
         self, model: PreTrainedModel
     ) -> Union[FullyShardedDataParallel, PreTrainedModel]:
-        """Shard the model using Fully Sharded Data Parallelism."""
+        """Shard the model using Fully Sharded Data Parallelism if needed."""
         if self.fsdp:
             _, layers = get_transformer_layers(model)
             layer_cls = type(layers[0])
             print(f"Using '{layer_cls.__name__}' for transformer_auto_wrap_policy.")
             return FullyShardedDataParallel(
                 model,
                 auto_wrap_policy=partial(
@@ -280,37 +326,49 @@
                     reduce_dtype=th.float16,
                     buffer_dtype=th.float16,
                 ),
             )
         elif self.cpu_offload:
             raise ValueError("CPU offload requires FSDP.")
         else:
-            model.to(self.device)
             return model
 
     def distribute_lens(self, lens: Lens) -> Union[DDP, Lens]:
         """Distribute the lens using DistributedDataParallel and send lens to device."""
         if self.world_size > 1:
             lens.to(self.device)
             return DDP(lens, device_ids=[self.local_rank], find_unused_parameters=True)
         else:
             return lens.to(self.device)
 
-    def shard_dataset(self, dataset: Dataset) -> Dataset:
+    def data_loader(
+        self,
+        dataset: Dataset,
+    ) -> dataloader2.DataLoader2:
         """Shard the dataset based on local rank."""
-        if dist.is_initialized():
-            dataset = dataset.shard(self.world_size, self.rank)
-        return dataset
+        dp = datapipes.iter.IterableWrapper(dataset)
+        if self.world_size > 1:
+            rs = dataloader2.DistributedReadingService()
+        else:
+            rs = None
+
+        dp = dp.shuffle()
+        dp = dp.sharding_filter()
+        dp = dp.batch(self.per_gpu_batch_size)
+        dp = dp.collate()
+        return dataloader2.DataLoader2(dp, reading_service=rs)
 
-    def init(self) -> None:
+    def init(self):
         """Initialize distributed process group if started with elastic launch."""
         # Support both distributed and non-distributed training
         local_rank = os.environ.get("LOCAL_RANK")
         if local_rank is not None:
-            dist.init_process_group("nccl")
+            dist.init_process_group(
+                "nccl", timeout=timedelta(seconds=self.nccl_timeout)
+            )
             assert (
                 th.cuda.is_available()
             ), "CUDA must be available for distributed training"
             th.cuda.set_device(self.local_rank)
 
     def barrier(self) -> None:
         """Barrier for all processes."""
```

### Comparing `tuned-lens-0.1.0/tuned_lens/scripts/train_loop.py` & `tuned-lens-0.1.1/tuned_lens/scripts/eval_loop.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,344 +1,324 @@
-"""Training loop for training a TunedLens model against a transformer on a dataset."""
-import dataclasses
-import enum
+"""Evaluation loop for the tuned lens model."""
+import json
 from collections import defaultdict
 from dataclasses import dataclass
 from itertools import islice
 from pathlib import Path
-from typing import Optional
+from typing import Literal, Optional
 
 import torch as th
 from simple_parsing import field
-from torch.utils.data import DataLoader
 from tqdm.auto import tqdm
 from transformers import PreTrainedModel
 
-from tuned_lens import TunedLens
+from tuned_lens.nn.lenses import Lens, LogitLens, TunedLens
 from tuned_lens.scripts.ingredients import (
     Data,
     Distributed,
     Model,
-    Optimizer,
 )
-from tuned_lens.utils import maybe_all_reduce, shift_labels, shift_preds
+from tuned_lens.stats import LogitStats
+from tuned_lens.utils import (
+    maybe_all_reduce,
+    pytree_map,
+    pytree_stack,
+    shift_labels,
+    shift_preds,
+)
 
+LensType = Literal["logit", "tuned"]
 
-class LossChoice(enum.Enum):
-    """Options of what loss to select when training the model."""
 
-    CE = "ce"
-    KL = "kl"
+def _nested_dict():
+    return defaultdict(_nested_dict)
 
 
 @dataclass
-class Train:
-    """Training loop for the tuned lens."""
-
-    model: Model
-    """Model configuration."""
+class Eval:
+    """Type hinting for CLI args."""
 
     data: Data
-    """Data configuration."""
 
-    opt: Optimizer
-    """Optimizer configuration."""
+    model: Model
 
     dist: Distributed
-    """Configuration for how to distribute the training."""
-
-    seed: int = 42
-    """Random seed for data shuffling."""
-
-    lens_name_or_path: Optional[str] = field(alias=["-l"], default=None)
-
-    constant: Optional[bool] = field(action="store_true")
-    """Train only the bias term."""
-
-    num_steps: int = 250
-    """Number of training steps."""
-
-    output: Optional[Path] = field(alias=["-o"], default=None)
-    """File to save the lenses to. Defaults to the model name."""
 
-    pre_ln: Optional[bool] = field(action="store_true")
-    """Apply layer norm before, and not after, each probe."""
+    output: Path = field(alias=["-o"])
+    """Folder to save the eval results to."""
 
-    separate_unembeddings: Optional[bool] = field(action="store_true")
-    """Learn a separate unembedding for each layer."""
+    lens_name: Optional[str] = field(alias=["-l"], default=None)
+    """Path to the tuned lens model."""
 
-    tokens_per_step: int = 2**18
-    """Number of tokens per step."""
+    lens_types: list[LensType] = field(default_factory=lambda: ["logit"])
+    """Types of lenses to evaluate can be a combination of (logit|tuned)."""
 
-    wandb: Optional[str] = None
-    """Name of run in Weights & Biases."""
+    seed: int = 42
+    """Random seed used for data shuffling."""
 
-    wandb_upload_checkpoints: Optional[bool] = field(action="store_true")
-    """Upload checkpoints to Weights & Biases."""
+    tokens: Optional[int] = None
+    """Number of tokens to evaluate on. If None, will use the entire dataset."""
 
-    token_shift: Optional[int] = None
+    token_shift: int = field(default=1)
     """How to shift the labels wrt the input tokens (1 = next token, 0 = current token,
     -1 = previous token, etc.)"""
 
     per_gpu_batch_size: int = 1
     """Number of samples to try to fit on a GPU at once."""
 
-    loss: LossChoice = LossChoice.KL
-    """Loss function to use."""
+    layer_transfer: bool = field(action="store_true")
+    """Evaluate the transfer of the lens to different layers of the transformer."""
 
-    def get_lens(self, model: PreTrainedModel) -> TunedLens:
-        """Load or create a TunedLens model."""
-        if self.lens_name_or_path is None:
-            lens = TunedLens.from_model(model)
-        else:
-            lens = TunedLens.from_model_and_pretrained(model, self.lens_name_or_path)
+    record_logit_stats: bool = field(action="store_true")
+    """Record the statistics of the marginal token distribution at each layer."""
 
-        lens_size = sum(p.numel() * p.element_size() for p in lens.parameters())
-        print(f"Tuned lens parameter memory usage: {lens_size / 2 ** 20:.2f} MB")
+    def load_lens(self, model: PreTrainedModel) -> dict[str, Lens]:
+        """Load the tuned lens model."""
+        lenses = {}
+        for lens_type in self.lens_types:
+            if lens_type == "logit":
+                lenses["logit"] = LogitLens.from_model(model)
+            elif lens_type == "tuned":
+                if self.lens_name is None:
+                    raise ValueError(
+                        "Must specify a lens name when evaluating a tuned lens."
+                    )
+                lenses["tuned"] = TunedLens.from_model_and_pretrained(
+                    model, self.lens_name
+                )
+            else:
+                raise ValueError(f"Unknown lens type: {lens_type}")
+        return lenses
 
-        if self.constant:
-            for probe in lens:
-                probe.weight.requires_grad_(False)
+    def calculate_batch_limit(self, tokens_per_sample: int):
+        """Calculate the total number of batches to evaluate on."""
+        assert self.tokens is not None
+        global_batch_size = self.dist.world_size * self.per_gpu_batch_size
+        tokens_per_batch = global_batch_size * tokens_per_sample
+        return self.tokens // tokens_per_batch
 
-        return lens
+    def _initialize_logit_stats_recorders(
+        self, lenses: dict[str, Lens], total_layers: int
+    ):
+        if self.record_logit_stats:
+            self.logit_stats_recorders = {
+                lens_type: {f"layer_{i}": LogitStats() for i in range(total_layers)}
+                for lens_type in lenses.keys()
+            }
+            self.logit_stats_recorder_final = LogitStats()
+        else:
+            self.logit_stats_recorders = None
+            self.logit_stats_recorder_final = None
 
-    def _init_logging(self, model_name: str, lens: TunedLens):
-        """Initialize logging to weights and biases."""
-        if not self.dist.primary or not self.wandb:
-            return
+    def _record_logit_stats(self, logp: th.Tensor, layer: int, lens_type: str):
+        if self.logit_stats_recorders is not None:
+            self.logit_stats_recorders[lens_type][f"layer_{layer}"].update(
+                logp, assume_normalized=True
+            )
 
-        import wandb
+    def _record_logit_stats_final(self, logp: th.Tensor):
+        if self.logit_stats_recorder_final is not None:
+            self.logit_stats_recorder_final.update(logp, assume_normalized=True)
+
+    def _save_logit_stats(self) -> defaultdict:
+        logit_stats = _nested_dict()
+        if self.logit_stats_recorders is not None:
+            for lens_type, recorders in self.logit_stats_recorders.items():
+                for layer, recorder in recorders.items():
+                    recorder.all_reduce_()
+                    logit_stats[lens_type]["logit_stats"][layer] = (
+                        recorder.marginal_probs.cpu().numpy().tolist()
+                    )
+
+        if self.logit_stats_recorder_final is not None:
+            self.logit_stats_recorder_final.all_reduce_()
+            logit_stats["baseline"]["logit_stats"]["final"] = (
+                self.logit_stats_recorder_final.marginal_probs.cpu().numpy().tolist()
+            )
 
-        wandb.init(
-            config=dataclasses.asdict(self),
-            group=model_name,
-            name=self.wandb,
-        )
-        wandb.watch(lens)
+        return logit_stats
 
-    def _log(
+    def _evaluate_lenses_on_hidden(
         self,
-        opt: th.optim.Optimizer,
-        step: int,
-        losses: dict[str, list[float]],
-        tuned_lens: TunedLens,
-        nats_to_bpb: float,
+        lenses: dict[str, Lens],
+        hidden: th.Tensor,
+        layer: int,
+        final_probs: th.Tensor,
+        final_lps: th.Tensor,
+        labels: th.Tensor,
+        batch_output: defaultdict,
+        total_layers: int,
     ):
-        """Log statistics about the training process to weights and biases."""
-        if not self.dist.primary or not self.wandb:
-            return
-
-        import wandb
-
-        log_dict = {}
-        log_dict.update(
-            {f"loss/{k}": th.tensor(v).mean() * nats_to_bpb for k, v in losses.items()}
-        )
-
-        # Log statistics about optimizer & probes
-        for i, probe in enumerate(tuned_lens):
-            name = "input" if i == 0 else f"{i - 1}.ffn"
-            states = [opt.state[p] for p in probe.parameters()]
-
-            # Approximate the true grad norm using the optimizer's moving
-            # avg
-            corr = 1 - self.opt.momentum**step
-            if self.opt.optimizer == "sgd" and not self.opt.zero:
-                log_dict["grad_norm/" + name] = th.cat(
-                    [
-                        # Undo PyTorch's scaling of the gradient by
-                        # 1 / (1 - β)
-                        (1 - self.opt.momentum) * s["momentum_buffer"].flatten() / corr
-                        for s in states
-                    ]
-                ).norm()
-            elif self.opt.optimizer == "adam" and not self.opt.zero:
-                log_dict["grad_norm/" + name] = th.cat(
-                    [s["exp_avg"].flatten() / corr for s in states]
-                ).norm()
-
-            if isinstance(probe, th.nn.Linear):
-                log_dict["bias_norm/" + name] = probe.bias.data.norm()
-                log_dict["weight_norm/" + name] = probe.weight.data.norm()
-
-        wandb.log(log_dict)
-
-    def _save_model(self, tuned_lens: TunedLens, model_name: str):
-        """Save the model to disk and try to upload to wandb if enabled."""
-        if not self.dist.primary:
-            return
+        """Evaluate a lens at a given layer. Batch output is modified in place.
 
-        assert model_name is not None
-        output = model_name if self.output is None else self.output
-        print(f"Saving lens to {output}")
-        tuned_lens.save(output)
-
-        if self.wandb and self.wandb_upload_checkpoints:
-            import wandb
-
-            artifact = wandb.Artifact(
-                name="final_checkpoint",
-                type="checkpoint",
-                description="A trained lens.",
+        Args:
+            lenses: The dictionary of lenses to evaluate on this hidden state.
+            hidden: (batch x seq x d_model) The hidden states of the transformer.
+            layer: The layer this hidden state is from.
+            final_probs: (batch x seq x vocab) The final probabilities of
+                the transformer.
+            final_lps: (batch x seq x vocab) The final log probabilities
+                of the transformer.
+            labels: (batch x seq) The labels for the transformer.
+            batch_output: Where to store the logging results.
+            total_layers: The total number of layers in the transformer.
+            logp_stats: where to record the logging results.
+        """
+        for lens_type, lens in lenses.items():
+            layer_name = f"layer_{layer}"
+            lens_lps = lens(hidden, idx=layer).log_softmax(dim=-1)
+            lens_probs = lens_lps.exp()
+
+            self._record_logit_stats(lens_lps, layer, lens_type)
+
+            batch_output[lens_type]["ce"][layer_name] = th.nn.functional.cross_entropy(
+                shift_preds(lens_lps, self.token_shift).flatten(0, 1),
+                labels.flatten(),
+                reduction="none",
             )
-            artifact.add_dir(output)
-            wandb.log_artifact(artifact)
 
-    def calculate_gradient_accumulation_steps(self, tokens_per_sample: int) -> int:
-        """Calculate the number of batches of data to process before taking a step."""
-        # chunk_and_tokenize ensures the samples are all the same length
-        samples_per_step, rem = divmod(self.tokens_per_step, tokens_per_sample)
-        if rem:
-            raise ValueError(
-                f"Number of tokens per step ({self.tokens_per_step:_}) must be "
-                f"divisible by the number of tokens per sample ({tokens_per_sample})."
+            batch_output[lens_type]["entropy"][layer_name] = th.sum(
+                -lens_probs * lens_lps, dim=-1
             )
 
-        global_batch_size = self.per_gpu_batch_size * self.dist.world_size
-        grad_acc_steps, rem = divmod(samples_per_step, global_batch_size)
-        if rem:
-            # If the number of samples per step isn't divisible by the global batch
-            # size, use ceil division and let the user know about it.
-            grad_acc_steps += 1
-            adjusted_count = grad_acc_steps * global_batch_size * tokens_per_sample
-            print(
-                f"Note: Increasing grad acc steps from {grad_acc_steps - 1} to "
-                f"{grad_acc_steps} to maintain load balance across "
-                f"{self.dist.world_size} GPUs."
+            batch_output[lens_type]["kl"][layer_name] = th.sum(
+                final_probs * (final_lps - lens_lps), dim=-1
             )
-            print(
-                f"Using {adjusted_count:_} tokens per training step "
-                f"({self.tokens_per_step:_} requested)."
-            )
-        else:
-            print(f"Gradient accumulation steps: {grad_acc_steps}")
-            print(f"Using {self.tokens_per_step:_} tokens per training step.")
-        return grad_acc_steps
 
+            if self.layer_transfer:
+                for i in range(total_layers):
+                    trans_name = f"layer_{i}"
+                    transfer_lps = lens(hidden, idx=i).log_softmax(dim=-1)
+                    batch_output[lens_type]["layer_transfer"]["ce"][trans_name][
+                        layer_name
+                    ] = th.nn.functional.cross_entropy(
+                        shift_preds(transfer_lps, self.token_shift).flatten(0, 1),
+                        labels.flatten(),
+                    )
+                    batch_output[lens_type]["layer_transfer"]["kl"][trans_name][
+                        layer_name
+                    ] = th.sum(lens_probs * (lens_lps - transfer_lps), dim=-1).mean()
+
+    @th.autocast("cuda", enabled=th.cuda.is_available())
+    @th.no_grad()
     def execute(self):
-        """Trains a TunedLens model against a transformer on a dataset."""
+        """Evaluates a TunedLens model against a transformer on a dataset."""
         # Load model, tokenizer, data, and lens
         self.dist.init()
-        model = tokenizer = data = lens = nats_to_bpb = model_name = None
+        model = tokenizer = data = lenses = nats_to_bpb = None
+
+        # See comment in train_loop.py for why we do this
+        load_device = self.dist.device if not self.dist.fsdp else None
         if self.dist.primary:
             # Let the primary processes populate the cache
-            model, tokenizer = self.model.load()
+            model, tokenizer = self.model.load(load_device)
             data, nats_to_bpb = self.data.load(tokenizer)
-            lens = self.get_lens(model)
-
-            *_, model_name = model.config.name_or_path.split("/")
-            self._init_logging(model_name, lens)
+            lenses = self.load_lens(model)
 
         self.dist.barrier()  # Wait for primary to finish filling the cache
 
         if not self.dist.primary:
             # Let the non-primary processes load from the cache
-            model, tokenizer = self.model.load(must_use_cache=True)
+            model, tokenizer = self.model.load(load_device, must_use_cache=True)
             data, nats_to_bpb = self.data.load(tokenizer)
-            lens = self.get_lens(model)
+            lenses = self.load_lens(model)
 
-        assert model and tokenizer and data and lens and nats_to_bpb
+        assert model and tokenizer and data and lenses and nats_to_bpb
 
-        # Shard the model using fully shared data parallel
         model = self.dist.shard_model(model)
-        # Distribute the lens across the GPUS using distributed data parallel
-        ddp_lens = self.dist.distribute_lens(lens)
-        # Shard the dataset for use with distributed data parallel
-        data = self.dist.shard_dataset(data)
-
-        dl = DataLoader(
-            data.shuffle(seed=self.seed),  # type: ignore[arg-type]
-            batch_size=self.per_gpu_batch_size,
-        )
-
-        # Don't train the unembedding matrix or final layer norm
-        params = [p for p in ddp_lens.parameters() if p.requires_grad]
+        # Note since we are not training we can just move the lens to the device.
+        # No need to use DDP
+        lenses = {name: lens.to(self.dist.device) for name, lens in lenses.items()}
+        dl = self.dist.data_loader(data)
+        dl.seed(self.seed)
+
+        for lens in lenses.values():
+            lens.eval()
+
+        if self.tokens is not None:
+            tokens_per_sample = len(data[0]["input_ids"])
+            batch_limit = self.calculate_batch_limit(tokens_per_sample)
+            assert batch_limit > 0, "Batch limit must be positive."
+            dl = islice(dl, batch_limit)
+            total = batch_limit
+        else:
+            total = len(data) // self.dist.world_size
 
-        # Create the optimizer and scheduler
-        opt = self.opt.create_optim(params)
-        scheduler = self.opt.create_scheduler(opt, self.num_steps)
+        L = model.config.num_hidden_layers
 
-        tokens_per_sample = len(data[0]["input_ids"])
+        self._initialize_logit_stats_recorders(lenses, L)
 
-        grad_acc_steps = self.calculate_gradient_accumulation_steps(tokens_per_sample)
+        root_dir = self.output
 
-        if self.dist.cpu_offload and grad_acc_steps > 1:
-            raise ValueError("CPU offloading cannot be used with gradient accumulation")
+        root_dir.mkdir(exist_ok=True, parents=True)
 
-        losses = defaultdict(list)
-        total_batches = self.num_steps * grad_acc_steps
+        batches = []
 
-        # Wait for all processes to finish setup
         self.dist.barrier()
-        print("All processes have completed setup. Starting training.")
+        print(f"All processes initialized. Running evaluation on {total} batches.")
 
-        # Main training loop
-        pbar = tqdm(islice(dl, total_batches), desc="Training", total=total_batches)
-        for batch_idx, batch in enumerate(pbar, start=1):
-            assert isinstance(batch, dict)
+        pbar = tqdm(dl, desc="Evaluating", position=self.dist.rank, total=total)
+        for batch in pbar:
             batch = self.dist.send_to_device(batch)
-            with th.no_grad():
-                output = model(**batch, output_hidden_states=True)
+            output = model(**batch, output_hidden_states=True)
 
-            final_logits = output.logits
-            hidden_stats = output.hidden_states[:-1]
+            hidden_states = output.hidden_states[:-1]
 
-            shift = self.token_shift
-            if self.loss == LossChoice.CE:
-                labels = batch["input_ids"]
-
-                # Predict the *next* token by default w/ cross entropy
-                if shift is None:
-                    shift = 1
-            elif self.loss == LossChoice.KL:
-                labels = final_logits.log_softmax(dim=-1)
-
-                # Match the *current* token distribution by default
-                if shift is None:
-                    shift = 0
-            else:
-                raise NotImplementedError(f"Unknown loss {self.loss}")
+            final_lps = output.logits.log_softmax(dim=-1)
 
-            labels = shift_labels(labels, shift)
+            final_probs = final_lps.exp()
+            assert not th.isnan(output.logits).any(), "Logits are NaN"
 
-            # We do this sequentially to save VRAM
-            for i, h in enumerate(hidden_stats):
-                # bfloat16 has larger dynamic range than float16 and seems to be better
-                # for computing log softmax & KL loss
-                with th.autocast(self.dist.device.type, dtype=th.bfloat16):
-                    logits = shift_preds(ddp_lens(h, idx=i), shift)
-
-                    if self.loss == LossChoice.CE:
-                        loss = th.nn.functional.cross_entropy(
-                            logits.flatten(0, -2), labels.flatten()
-                        )
-                    elif self.loss == LossChoice.KL:
-                        loss = th.sum(
-                            labels.exp() * (labels - logits.log_softmax(-1)), dim=-1
-                        ).mean()
-                    else:
-                        raise NotImplementedError
-
-                    # Log the loss *before* LASSO regularization
-                    logging_loss = loss.detach()
-                    logging_loss = maybe_all_reduce(logging_loss).item()
-                    if self.dist.primary:
-                        losses[f"translator_{i}"].append(logging_loss)
-
-                    scaled_loss = loss / grad_acc_steps
-
-                scaled_loss.backward()
-
-            step, rem = divmod(batch_idx, grad_acc_steps)
-            if rem == 0:
-                th.nn.utils.clip_grad_norm_(lens.parameters(), 1.0)
-                opt.step()
-                opt.zero_grad(set_to_none=False)
-                scheduler.step()
-                self._log(opt, step, losses, lens, nats_to_bpb)
-                losses.clear()
+            labels = shift_labels(batch["input_ids"], self.token_shift)
+
+            batch_output = _nested_dict()
+
+            # Compute tuned lens eval and statistics if applicable
+            for j, h in zip(range(L), hidden_states):
+                self._evaluate_lenses_on_hidden(
+                    lenses=lenses,
+                    hidden=h,
+                    layer=j,
+                    final_probs=final_probs,
+                    final_lps=final_lps,
+                    labels=labels,
+                    batch_output=batch_output,
+                    total_layers=L,
+                )
+
+            batch_output["baseline"]["ce"]["final"] = th.nn.functional.cross_entropy(
+                shift_preds(final_lps, self.token_shift).flatten(0, 1),
+                labels.flatten(),
+                reduction="none",
+            )
+            batch_output["baseline"]["entropy"]["final"] = th.sum(
+                -final_probs * final_lps, dim=-1
+            )
+
+            batches.append(pytree_map(th.mean, batch_output))  # type: ignore[arg-type]
+
+            self._record_logit_stats_final(final_lps)
+
+        pbar.close()
+        agg = pytree_map(lambda x: nats_to_bpb * x.mean(), pytree_stack(batches))
+        agg = pytree_map(lambda x: maybe_all_reduce(x), agg)
+        agg = pytree_map(lambda x: x.cpu().numpy().item(), agg)
+
+        assert isinstance(agg, dict)
+
+        batches = pytree_map(lambda x: nats_to_bpb * x, batches)
+        batches = pytree_map(lambda x: maybe_all_reduce(x), batches)
+        batches = pytree_map(lambda x: x.cpu().item(), batches)
+        assert isinstance(batches, list)
+
+        logit_stats = self._save_logit_stats()
 
         if self.dist.primary:
-            assert model_name is not None
-            output = model_name if self.output is None else self.output
-            print(f"Saving lens to {output}")
-            lens.save(output)
+            with (root_dir / "batches.jsonl").open("w") as f:
+                json.dump(batches, f)
+
+            with (root_dir / "aggregate_metrics.json").open("w") as f:
+                json.dump(agg, f)
+
+            if self.record_logit_stats:
+                with (root_dir / "logit_stats.json").open("w") as f:
+                    json.dump(logit_stats, f)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tuned-lens-0.1.0/tuned_lens/stats/distance.py` & `tuned-lens-0.1.1/tuned_lens/stats/distance.py`

 * *Files identical despite different names*

### Comparing `tuned-lens-0.1.0/tuned_lens/utils.py` & `tuned-lens-0.1.1/tuned_lens/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 """Utilities for distributed training and handling nested collections of tensors."""
 
 import hashlib
+from contextlib import contextmanager
 from itertools import islice
 from typing import Any, Callable, Iterable, Sequence, Type, TypeVar, Union, cast
 
 import numpy as np
 import torch as th
 import torch.distributed as dist
 from numpy.typing import NDArray
@@ -107,14 +108,27 @@
 
 # Backported from Python 3.10
 def pairwise(it: Iterable[T]) -> Iterable[tuple[T, T]]:
     """Iterate over pairs of elements in an iterable."""
     yield from zip(it, islice(it, 1, None))
 
 
+@contextmanager
+def handle_name_conflicts():
+    """Provide better error messages."""
+    try:
+        yield
+    except OSError as e:
+        raise RuntimeError(
+            "HuggingFace is throwing an error during a `from_pretrained` call. Check "
+            "your CWD to ensure there are no folders with names that may conflict "
+            "with the model name you provided."
+        ) from e
+
+
 # Define pytree type recursively- this works for Pylance but unfortunately not MyPy
 AnyTree = Union[th.Tensor, dict[Any, "AnyTree"], list["AnyTree"], tuple["AnyTree", ...]]
 TreeType = TypeVar("TreeType", bound=AnyTree)
 
 
 def pytree_flatten(tree: AnyTree) -> Iterable[th.Tensor]:
     """Recursively iterate over all tensors in a pytree, in topological order."""
```

### Comparing `tuned-lens-0.1.0/tuned_lens.egg-info/PKG-INFO` & `tuned-lens-0.1.1/tuned_lens.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: tuned-lens
-Version: 0.1.0
+Version: 0.1.1
 Summary: Tools for understanding how transformer predictions are built layer-by-layer
 License: MIT License
 Keywords: nlp,interpretability,language-models,explainable-ai
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: docs
 Provides-Extra: test
+Provides-Extra: slow_tokenizers
 Provides-Extra: notebooks
+Provides-Extra: 8bit
 License-File: LICENSE
 
 # Tuned Lens 🔎
 <a target="_blank" href="https://colab.research.google.com/github/AlignmentResearch/tuned-lens/blob/main/notebooks/interactive.ipynb">
   <img src="https://colab.research.google.com/assets/colab-badge.svg" alt="Open In Colab"/>
 </a>
 <a target="_blank" href="https://huggingface.co/spaces/AlignmentResearch/tuned-lens">
```

### Comparing `tuned-lens-0.1.0/tuned_lens.egg-info/SOURCES.txt` & `tuned-lens-0.1.1/tuned_lens.egg-info/SOURCES.txt`

 * *Files identical despite different names*

