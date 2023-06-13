# Comparing `tmp/nlpipes-0.1.8.tar.gz` & `tmp/nlpipes-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nlpipes-0.1.8.tar", max compression
+gzip compressed data, was "nlpipes-0.1.9.tar", max compression
```

## Comparing `nlpipes-0.1.8.tar` & `nlpipes-0.1.9.tar`

### file list

```diff
@@ -1,85 +1,36 @@
--rw-r--r--   0        0        0     4039 2023-03-01 13:45:32.044264 nlpipes-0.1.8/README.md
--rw-r--r--   0        0        0       30 2023-02-28 13:21:04.473570 nlpipes-0.1.8/nlpipes/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     6456 2023-03-01 13:58:08.254813 nlpipes-0.1.8/nlpipes/.ipynb_checkpoints/auto_model-checkpoint.py
--rw-r--r--   0        0        0       30 2023-02-28 13:31:06.873730 nlpipes-0.1.8/nlpipes/__init__.py
--rw-r--r--   0        0        0     6456 2023-03-01 14:01:00.674888 nlpipes-0.1.8/nlpipes/auto_model.py
--rw-r--r--   0        0        0    19792 2023-03-01 13:38:18.723851 nlpipes-0.1.8/nlpipes/callbacks/.ipynb_checkpoints/callbacks-checkpoint.py
--rw-r--r--   0        0        0        1 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/callbacks/__init__.py
--rw-r--r--   0        0        0      138 2023-02-27 15:44:03.469432 nlpipes-0.1.8/nlpipes/callbacks/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0    19832 2023-03-01 13:38:26.408568 nlpipes-0.1.8/nlpipes/callbacks/__pycache__/callbacks.cpython-37.pyc
--rw-r--r--   0        0        0    19792 2023-03-01 13:45:32.068266 nlpipes-0.1.8/nlpipes/callbacks/callbacks.py
--rw-r--r--   0        0        0     1606 2023-02-27 15:44:03.541437 nlpipes-0.1.8/nlpipes/configurations/__pycache__/bert_config.cpython-37.pyc
--rw-r--r--   0        0        0     1903 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/configurations/bert_config.py
--rw-r--r--   0        0        0      283 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/configurations/card_config.py
--rw-r--r--   0        0        0     1922 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/data/.ipynb_checkpoints/data_loaders-checkpoint.py
--rw-r--r--   0        0        0     4842 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/data/.ipynb_checkpoints/data_processors-checkpoint.py
--rw-r--r--   0        0        0     6301 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/data/.ipynb_checkpoints/data_selectors-checkpoint.py
--rw-r--r--   0        0        0     1418 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/data/.ipynb_checkpoints/data_splitters-checkpoint.py
--rw-r--r--   0        0        0     8587 2023-02-27 16:41:49.053512 nlpipes-0.1.8/nlpipes/data/.ipynb_checkpoints/data_types-checkpoint.py
--rw-r--r--   0        0        0     2599 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/data/.ipynb_checkpoints/data_utils-checkpoint.py
--rw-r--r--   0        0        0        1 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/data/__init__.py
--rw-r--r--   0        0        0      133 2023-02-27 15:44:03.441430 nlpipes-0.1.8/nlpipes/data/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     5828 2023-02-27 15:44:03.485433 nlpipes-0.1.8/nlpipes/data/__pycache__/data_augmentors.cpython-37.pyc
--rw-r--r--   0        0        0      703 2023-02-27 15:44:03.489434 nlpipes-0.1.8/nlpipes/data/__pycache__/data_cleaners.cpython-37.pyc
--rw-r--r--   0        0        0     1885 2023-02-27 15:44:03.481433 nlpipes-0.1.8/nlpipes/data/__pycache__/data_loaders.cpython-37.pyc
--rw-r--r--   0        0        0     4536 2023-02-27 15:44:03.481433 nlpipes-0.1.8/nlpipes/data/__pycache__/data_processors.cpython-37.pyc
--rw-r--r--   0        0        0     5606 2023-02-27 15:44:03.485433 nlpipes-0.1.8/nlpipes/data/__pycache__/data_selectors.cpython-37.pyc
--rw-r--r--   0        0        0    10709 2023-02-27 16:45:29.321026 nlpipes-0.1.8/nlpipes/data/__pycache__/data_types.cpython-37.pyc
--rw-r--r--   0        0        0     3371 2023-02-27 15:44:03.533437 nlpipes-0.1.8/nlpipes/data/__pycache__/data_utils.cpython-37.pyc
--rw-r--r--   0        0        0     6638 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/data/data_augmentors.py
--rw-r--r--   0        0        0      656 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/data/data_cleaners.py
--rw-r--r--   0        0        0     1922 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/data/data_loaders.py
--rw-r--r--   0        0        0     4842 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/data/data_processors.py
--rw-r--r--   0        0        0     6301 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/data/data_selectors.py
--rw-r--r--   0        0        0     1418 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/data/data_splitters.py
--rw-r--r--   0        0        0     8587 2023-02-27 16:41:49.053512 nlpipes-0.1.8/nlpipes/data/data_types.py
--rw-r--r--   0        0        0     2599 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/data/data_utils.py
--rw-r--r--   0        0        0    14393 2023-02-27 15:44:03.541437 nlpipes-0.1.8/nlpipes/layers/__pycache__/bert_layers.cpython-37.pyc
--rw-r--r--   0        0        0    19444 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/layers/bert_layers.py
--rw-r--r--   0        0        0      233 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/losses/.ipynb_checkpoints/losses-checkpoint.py
--rw-r--r--   0        0        0      428 2023-02-27 15:44:03.477433 nlpipes-0.1.8/nlpipes/losses/__pycache__/losses.cpython-37.pyc
--rw-r--r--   0        0        0      233 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/losses/losses.py
--rw-r--r--   0        0        0     4194 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/metrics/.ipynb_checkpoints/confusion-checkpoint.py
--rw-r--r--   0        0        0     3876 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/metrics/.ipynb_checkpoints/diversity-checkpoint.py
--rw-r--r--   0        0        0     4436 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/metrics/.ipynb_checkpoints/similarity-checkpoint.py
--rw-r--r--   0        0        0      141 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/metrics/__init__.py
--rw-r--r--   0        0        0      315 2023-02-27 15:44:03.485433 nlpipes-0.1.8/nlpipes/metrics/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     3919 2023-02-27 15:44:03.541437 nlpipes-0.1.8/nlpipes/metrics/__pycache__/confusion.cpython-37.pyc
--rw-r--r--   0        0        0     4080 2023-02-27 15:44:03.485433 nlpipes-0.1.8/nlpipes/metrics/__pycache__/diversity.cpython-37.pyc
--rw-r--r--   0        0        0     4331 2023-02-27 15:44:03.485433 nlpipes-0.1.8/nlpipes/metrics/__pycache__/similarity.cpython-37.pyc
--rw-r--r--   0        0        0     4194 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/metrics/confusion.py
--rw-r--r--   0        0        0     3876 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/metrics/diversity.py
--rw-r--r--   0        0        0     4436 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/metrics/similarity.py
--rw-r--r--   0        0        0      650 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/models/.ipynb_checkpoints/language_modeling-checkpoint.py
--rw-r--r--   0        0        0     4318 2023-02-27 13:45:56.768770 nlpipes-0.1.8/nlpipes/models/.ipynb_checkpoints/sequence_classification-checkpoint.py
--rw-r--r--   0        0        0     1052 2023-02-27 15:44:03.541437 nlpipes-0.1.8/nlpipes/models/__pycache__/language_modeling.cpython-37.pyc
--rw-r--r--   0        0        0     3402 2023-02-27 15:44:03.537437 nlpipes-0.1.8/nlpipes/models/__pycache__/sequence_classification.cpython-37.pyc
--rw-r--r--   0        0        0      650 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/models/language_modeling.py
--rw-r--r--   0        0        0     4318 2023-02-27 13:45:56.768770 nlpipes-0.1.8/nlpipes/models/sequence_classification.py
--rw-r--r--   0        0        0     4878 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/optimization/.ipynb_checkpoints/optimizers-checkpoint.py
--rw-r--r--   0        0        0      739 2023-02-27 16:41:42.541053 nlpipes-0.1.8/nlpipes/optimization/.ipynb_checkpoints/schedulers-checkpoint.py
--rw-r--r--   0        0        0     4878 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/optimization/optimizers.py
--rw-r--r--   0        0        0      739 2023-02-27 16:41:42.541053 nlpipes-0.1.8/nlpipes/optimization/schedulers.py
--rw-r--r--   0        0        0        0 2023-02-27 15:29:38.640510 nlpipes-0.1.8/nlpipes/pipelines/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0       74 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/pipelines/.ipynb_checkpoints/base-checkpoint.py
--rw-r--r--   0        0        0     6278 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/pipelines/.ipynb_checkpoints/language_modeling-checkpoint.py
--rw-r--r--   0        0        0     7588 2023-02-27 09:43:09.162520 nlpipes-0.1.8/nlpipes/pipelines/.ipynb_checkpoints/sequence_classification-checkpoint.py
--rw-r--r--   0        0        0        0 2023-02-27 15:29:38.640510 nlpipes-0.1.8/nlpipes/pipelines/__init__.py
--rw-r--r--   0        0        0      138 2023-02-27 15:37:03.355838 nlpipes-0.1.8/nlpipes/pipelines/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     4822 2023-02-27 17:04:31.457467 nlpipes-0.1.8/nlpipes/pipelines/__pycache__/auto_pipeline.cpython-37.pyc
--rw-r--r--   0        0        0      336 2023-02-27 15:44:03.445430 nlpipes-0.1.8/nlpipes/pipelines/__pycache__/base.cpython-37.pyc
--rw-r--r--   0        0        0     4746 2023-02-27 15:44:03.449431 nlpipes-0.1.8/nlpipes/pipelines/__pycache__/language_modeling.cpython-37.pyc
--rw-r--r--   0        0        0     5618 2023-02-27 15:44:03.481433 nlpipes-0.1.8/nlpipes/pipelines/__pycache__/pipeline_utils.cpython-37.pyc
--rw-r--r--   0        0        0     6238 2023-02-27 15:44:03.533437 nlpipes-0.1.8/nlpipes/pipelines/__pycache__/sequence_classification.cpython-37.pyc
--rw-r--r--   0        0        0       74 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/pipelines/base.py
--rw-r--r--   0        0        0     6278 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/pipelines/language_modeling.py
--rw-r--r--   0        0        0     5421 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/pipelines/pipeline_utils.py
--rw-r--r--   0        0        0     7588 2023-02-27 09:43:09.162520 nlpipes-0.1.8/nlpipes/pipelines/sequence_classification.py
--rw-r--r--   0        0        0     1888 2023-02-27 09:39:51.531828 nlpipes-0.1.8/nlpipes/trainers/.ipynb_checkpoints/trainers-checkpoint.py
--rw-r--r--   0        0        0        1 2023-02-23 17:48:35.809060 nlpipes-0.1.8/nlpipes/trainers/__init__.py
--rw-r--r--   0        0        0      137 2023-02-27 15:44:03.449431 nlpipes-0.1.8/nlpipes/trainers/__pycache__/__init__.cpython-37.pyc
--rw-r--r--   0        0        0     1798 2023-02-27 15:44:03.469432 nlpipes-0.1.8/nlpipes/trainers/__pycache__/trainers.cpython-37.pyc
--rw-r--r--   0        0        0     1888 2023-02-27 09:39:51.531828 nlpipes-0.1.8/nlpipes/trainers/trainers.py
--rw-r--r--   0        0        0      668 2023-03-01 14:01:00.678888 nlpipes-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     5491 1970-01-01 00:00:00.000000 nlpipes-0.1.8/setup.py
--rw-r--r--   0        0        0     4962 1970-01-01 00:00:00.000000 nlpipes-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     4076 2023-03-03 06:56:48.815501 nlpipes-0.1.9/README.md
+-rw-r--r--   0        0        0       30 2023-02-28 13:31:06.873730 nlpipes-0.1.9/nlpipes/__init__.py
+-rw-r--r--   0        0        0     6456 2023-03-01 14:01:00.674888 nlpipes-0.1.9/nlpipes/auto_model.py
+-rw-r--r--   0        0        0        1 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/callbacks/__init__.py
+-rw-r--r--   0        0        0    20375 2023-03-03 06:53:25.020812 nlpipes-0.1.9/nlpipes/callbacks/callbacks.py
+-rw-r--r--   0        0        0     1903 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/configurations/bert_config.py
+-rw-r--r--   0        0        0      283 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/configurations/card_config.py
+-rw-r--r--   0        0        0        1 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/data/__init__.py
+-rw-r--r--   0        0        0     6638 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/data/data_augmentors.py
+-rw-r--r--   0        0        0      656 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/data/data_cleaners.py
+-rw-r--r--   0        0        0     1930 2023-03-03 06:53:25.020812 nlpipes-0.1.9/nlpipes/data/data_loaders.py
+-rw-r--r--   0        0        0     4842 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/data/data_processors.py
+-rw-r--r--   0        0        0     6301 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/data/data_selectors.py
+-rw-r--r--   0        0        0     1392 2023-03-03 06:53:25.020812 nlpipes-0.1.9/nlpipes/data/data_splitters.py
+-rw-r--r--   0        0        0     8587 2023-02-27 16:41:49.053512 nlpipes-0.1.9/nlpipes/data/data_types.py
+-rw-r--r--   0        0        0     2572 2023-03-03 06:53:25.020812 nlpipes-0.1.9/nlpipes/data/data_utils.py
+-rw-r--r--   0        0        0    19444 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/layers/bert_layers.py
+-rw-r--r--   0        0        0      233 2023-03-02 09:16:32.532156 nlpipes-0.1.9/nlpipes/losses/losses.py
+-rw-r--r--   0        0        0      141 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/metrics/__init__.py
+-rw-r--r--   0        0        0     4194 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/metrics/confusion.py
+-rw-r--r--   0        0        0     3876 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/metrics/diversity.py
+-rw-r--r--   0        0        0     4436 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/metrics/similarity.py
+-rw-r--r--   0        0        0      650 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/models/language_modeling.py
+-rw-r--r--   0        0        0     4318 2023-02-27 13:45:56.768770 nlpipes-0.1.9/nlpipes/models/sequence_classification.py
+-rw-r--r--   0        0        0     4878 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/optimization/optimizers.py
+-rw-r--r--   0        0        0      739 2023-02-27 16:41:42.541053 nlpipes-0.1.9/nlpipes/optimization/schedulers.py
+-rw-r--r--   0        0        0        0 2023-02-27 15:29:38.640510 nlpipes-0.1.9/nlpipes/pipelines/__init__.py
+-rw-r--r--   0        0        0       74 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/pipelines/base.py
+-rw-r--r--   0        0        0     6279 2023-03-03 06:53:25.020812 nlpipes-0.1.9/nlpipes/pipelines/language_modeling.py
+-rw-r--r--   0        0        0     5471 2023-03-03 06:53:25.020812 nlpipes-0.1.9/nlpipes/pipelines/pipeline_utils.py
+-rw-r--r--   0        0        0     7656 2023-03-03 06:53:25.020812 nlpipes-0.1.9/nlpipes/pipelines/sequence_classification.py
+-rw-r--r--   0        0        0        1 2023-02-23 17:48:35.809060 nlpipes-0.1.9/nlpipes/trainers/__init__.py
+-rw-r--r--   0        0        0     2019 2023-03-03 06:53:25.020812 nlpipes-0.1.9/nlpipes/trainers/trainers.py
+-rw-r--r--   0        0        0      668 2023-03-03 06:57:27.971092 nlpipes-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     5180 1970-01-01 00:00:00.000000 nlpipes-0.1.9/setup.py
+-rw-r--r--   0        0        0     4999 1970-01-01 00:00:00.000000 nlpipes-0.1.9/PKG-INFO
```

### Comparing `nlpipes-0.1.8/README.md` & `nlpipes-0.1.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
   <h3>Text Classification with Transformers</h3>
 </div>
 
 <div align="center">
     <a href="https://opensource.org/licenses/Apache-2.0">
        <img alt="Licence" src="https://img.shields.io/badge/License-Apache_2.0-blue.svg">
     </a>
-     <a href="https://opensource.org/licenses/Apache-2.0">
+     <a href="https://pypi.org/project/nlpipes/">
        <img alt="PyPi Version" src="https://img.shields.io/pypi/pyversions/nlpipes">
     </a> 
     <a href="https://pypi.org/project/nlpipes/">
         <img alt="PyPi Package Version" src="https://img.shields.io/pypi/v/nlpipes">
     </a>
     <!--
     <a href="https://pepy.tech/project/nlpipes/">
@@ -62,14 +62,14 @@
 
 #### Examples
 
 Here are some use-cases with `NLPipes` on real datasets:
 
 Name|Notebook|Description|Task|Size|Memory| 
 ----|-----------|-----|---------|---------|---------|
-GooglePlay Sentiment Detection|[Link]("")|Train a model to label reviews from the GooglePlay store reviews|Single-label classification|  |  
+GooglePlay Sentiment Detection|[Link]("/notebooks/googleplay_sentiment_labeling.ipynb")|Train a model to label reviews from the GooglePlay store reviews|Single-label classification|  |  
 StackOverflow tags Detection|Coming soon|Train a model to detect tags from the StackOverFlow questions |Multiple-labels classification|  | 
 GooglePlay Aspect and Sentiment Detection|Coming soon|Train a model for aspect based sentiment detection to detect the aspects mentionned in GooglePlay reviews along his assocated sentiment polarity |Aspect-based classification|  | 
 
 
 ## Notice
 `NLPipes` is still in its early stage and is not yet suitable for production usage. Proceed with caution and use it at your own risk. The library comes with no warranty and future releases could bring substantial API and behavior changes.
```

#### html2text {}

```diff
@@ -27,18 +27,18 @@
 www.tensorflow.org/): An end-to-end open source deep learning framework *
 [Transformers](https://huggingface.co/transformers/): An general-purpose open-
 sources library for transformers-based architectures ## Getting Started ####
 Installation 1. Create a virtual environment ```console python3 -m venv
 nlpipesenv source nlpipesenv/bin/activate ``` 2. Install the package ```console
 pip install nlpipes ``` #### Examples Here are some use-cases with `NLPipes` on
 real datasets: Name|Notebook|Description|Task|Size|Memory| ----|-----------|---
---|---------|---------|---------| GooglePlay Sentiment Detection|[Link]
-("")|Train a model to label reviews from the GooglePlay store reviews|Single-
-label classification| | StackOverflow tags Detection|Coming soon|Train a model
-to detect tags from the StackOverFlow questions |Multiple-labels
-classification| | GooglePlay Aspect and Sentiment Detection|Coming soon|Train a
-model for aspect based sentiment detection to detect the aspects mentionned in
-GooglePlay reviews along his assocated sentiment polarity |Aspect-based
-classification| | ## Notice `NLPipes` is still in its early stage and is not
-yet suitable for production usage. Proceed with caution and use it at your own
-risk. The library comes with no warranty and future releases could bring
-substantial API and behavior changes.
+--|---------|---------|---------| GooglePlay Sentiment Detection|[Link]("/
+notebooks/googleplay_sentiment_labeling.ipynb")|Train a model to label reviews
+from the GooglePlay store reviews|Single-label classification| | StackOverflow
+tags Detection|Coming soon|Train a model to detect tags from the StackOverFlow
+questions |Multiple-labels classification| | GooglePlay Aspect and Sentiment
+Detection|Coming soon|Train a model for aspect based sentiment detection to
+detect the aspects mentionned in GooglePlay reviews along his assocated
+sentiment polarity |Aspect-based classification| | ## Notice `NLPipes` is still
+in its early stage and is not yet suitable for production usage. Proceed with
+caution and use it at your own risk. The library comes with no warranty and
+future releases could bring substantial API and behavior changes.
```

### Comparing `nlpipes-0.1.8/nlpipes/.ipynb_checkpoints/auto_model-checkpoint.py` & `nlpipes-0.1.9/nlpipes/auto_model.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/callbacks/.ipynb_checkpoints/callbacks-checkpoint.py` & `nlpipes-0.1.9/nlpipes/callbacks/callbacks.py`

 * *Files 9% similar despite different names*

```diff
@@ -50,27 +50,27 @@
 
 class Callback(ABC):
     
     """ Abstract base class for callback objects. """
     
     def on_train_begin(self):
         """ Called at the beginning of the training. """
-     
+        
     def on_train_end(self):
         """ Called at the end of the training. """
-      
+        
     def on_test_begin(self):
         """ Called at the beginning of the evaluation. """
-     
+        
     def on_test_end(self):
         """ Called at the end of the evaluation. """
     
     def on_epoch_begin(self, *args):
         """ Called at the beginning of an epoch. """
-
+        
     def on_epoch_end(self, *args):
         """ Called at the end of an epoch. """
     
     def on_train_batch_begin(self, *args):
         """ Called at the beginning of a training batch. """
     
     def on_train_batch_end(self, *args):
@@ -93,15 +93,15 @@
            easily. For example, if we have three callbacks 
            that do something at the end of an epoch, then 
            callbacks.on_epoch_end() will call the three
            callback objects in order. 
     """
 
     callbacks: List[Callback]
-   
+    
     def on_train_begin(self, *args):
         for callback in self.callbacks:
             callback.on_train_begin(*args)
         
     def on_train_end(self, *args):
         for callback in self.callbacks:
             callback.on_train_end(*args)
@@ -143,158 +143,173 @@
 class TrainingStep(Callback):
     """ Callback that define the training step. The training step is
     a single iteration of the training process. It consists of a 
     forward pass (where the obj:`model` makes predictions based on
     the input data) and a backward pass (where the obj:`optimizer`
     updates the obj:`model` weights and biases based on the difference
     between the predicted output and the expected output as expressed
-    by the obj:`loss_finction`).
+    by the obj:`loss_function`).
     """
     
     name: str = 'TrainingStep'
     model: TFPreTrainedModel = None
     optimizer: tf.optimizers.Optimizer = None
     loss_function: tf.losses = None
     
-    def _train_step(self, features: InputFeatures):
+    def train_step(self, input_batch: InputFeatures):
         """ Train the obj:`model` on a single batch of examples. """
         
         with tf.GradientTape() as tape:
-            model_outputs = self.model.call(
-                input_ids=features.input_ids,
-                attention_mask=features.attention_mask,
-                token_type_ids=features.token_type_ids,
+            output_batch = self.model.call(
+                input_ids=input_batch.input_ids,
+                attention_mask=input_batch.attention_mask,
+                token_type_ids=input_batch.token_type_ids,
                 training=True,
             )
             
-            loss_values = self.loss_function(
-                features.label, model_outputs.logits
+            loss = self.loss_function(
+                input_batch.label, output_batch.logits
             )
             
-        trainable_variables = self.model.trainable_variables
-            
-        gradients = tape.gradient(loss_values, trainable_variables)
+        variables = self.model.trainable_variables
+        gradients = tape.gradient(loss, variables)
         
         self.optimizer.apply_gradients(
-            zip(gradients, trainable_variables)
+            zip(gradients, variables)
         )
         
-        output_batch = TFSequenceClassifierBatchOutput(
-            loss=loss_values,
-            logits=model_outputs.logits,
-            hidden_states=model_outputs.hidden_states,
-            attentions=model_outputs.attentions,
+        return TFSequenceClassifierBatchOutput(
+            loss=loss,
+            logits=output_batch.logits,
+            hidden_states=output_batch.hidden_states,
+            attentions=output_batch.attentions,
         )
-        
-        return output_batch
     
-    def _test_step(self, features: InputFeatures):
+    def test_step(self, input_batch: InputFeatures):
         """ Test the obj:`model` on a single batch of examples. """
         
-        model_outputs = self.model.call(
-                  input_ids=features.input_ids,
-                  attention_mask=features.attention_mask,
-                  token_type_ids=features.token_type_ids,
+        output_batch = self.model.call(
+                  input_ids=input_batch.input_ids,
+                  attention_mask=input_batch.attention_mask,
+                  token_type_ids=input_batch.token_type_ids,
                   training=False,
         )
         
-        loss_values = self.loss_function(
-            features.label, model_outputs.logits
+        loss = self.loss_function(
+            input_batch.label, output_batch.logits
         )
         
         return TFSequenceClassifierBatchOutput(
-            loss=loss_values,
-            logits=model_outputs.logits,
-            hidden_states=model_outputs.hidden_states,
-            attentions=model_outputs.attentions,
+            loss=loss,
+            logits=output_batch.logits,
+            hidden_states=output_batch.hidden_states,
+            attentions=output_batch.attentions,
         )
     
     def on_train_begin(self):
         message = self.model.summary()
-        logger.info(message)           
-     
-    def on_train_batch_begin(self, step: int, features: InputFeatures):
-        self.train_step_output = self._train_step(features)
+        logger.info(message)
+        
+    def on_train_batch_begin(self, step: int, batch: InputFeatures):
+        self.train_step_output = self.train_step(batch)
              
-    def on_test_batch_begin(self, step: int, features: InputFeatures):
-        self.test_step_output = self._test_step(features)
-
+    def on_test_batch_begin(self, step: int, batch: InputFeatures):
+        self.test_step_output = self.test_step(batch)
 
+        
 @dataclass
 class History(Callback):
     """ Callback that records the performance of the model 
     during training. It stores all the evaluation metrics 
     such as loss and accuracy at each training and testing
     steps. This allows to track the progress of the model
     over time, and can be used by other callbacks, e.g. to
     detect when the model has reached its optimal performance.
     """
     
     name: str = 'History'
     epoch: int = field(default_factory=int)
-    metric: Callable[[], tf.metrics.Metric] = None
+    loss_metric: Callable[[], tf.metrics.Metric] = None
+    acc_metric: Callable[[], tf.metrics.Metric] = None
     training_step: Callback = None
-    train: Dict = field(default_factory=lambda: defaultdict(dict))
-    test: Dict = field(default_factory=lambda: defaultdict(dict))
-    train_details: Dict = field(default_factory=lambda: defaultdict(dict))
-    test_details: Dict = field(default_factory=lambda: defaultdict(dict))
-
+    logs: Dict = field(default_factory=lambda: defaultdict(dict))
     
     def __post_init__(self):
-        self.train_metric = self.metric()
-        self.test_metric = self.metric()
+        """ """
+        self.loss_train_metric = self.loss_metric()
+        self.loss_test_metric = self.loss_metric()
+        self.acc_train_metric = self.acc_metric()
+        self.acc_test_metric = self.acc_metric()
+        
+    def on_train_begin(self):
+        """ """
+        self.logs['loss'] = {}
+        self.logs['acc'] = {}
+        self.logs['val_loss'] = {}
+        self.logs['val_acc'] = {}
     
     def on_epoch_begin(self, epoch: int):
         """ Resets all of the metric state variables """
+        
         self.epoch = epoch
-        self.train_metric.reset_states()
-        self.test_metric.reset_states()
+        '''
+        self.logs['loss'][epoch] = []
+        self.logs['acc'][epoch] = []
+        self.logs['val_loss'][epoch] = []
+        self.logs['val_acc'][epoch] = []
+        '''
+        self.loss_train_metric.reset_states()
+        self.loss_test_metric.reset_states()
+        self.acc_train_metric.reset_states()
+        self.acc_test_metric.reset_states()
         
-        self.train['loss'] = {}
-        self.train_details['loss'] = {}
-        self.test_details['loss'] = {}
-        self.train['loss'][epoch] = []
-        self.train_details['loss'][epoch] = []
-        self.test_details['loss'][epoch] = []
-        
-        self.test['accuracy'] = {}
-        self.train_details['accuracy'] = {}
-        self.test_details['accuracy'] = {}
-        self.test['accuracy'][epoch] = []
-        self.train_details['accuracy'][epoch] = []
-        self.test_details['accuracy'][epoch] = []
-    
     def on_epoch_end(self, epoch: int):
         """ Display the performance metrics after each epoch """
-        self.train['loss'][self.epoch] = self.train_metric.result()
-        self.test['loss'][self.epoch] = self.test_metric.result()
         
-        message = f'Epoch {self.epoch+1:4d} {self.name:10} ' \
-                  f'Train {self.train_metric.result():1.3f} ' \
-                  f'Test {self.test_metric.result():1.3f}'
+        message = f"Training loss:       {self.logs['loss'][epoch]:1.3f}" \
+                  f"Training accuracy:   {self.logs['acc'][epoch]:1.3f}" \
+                  f"Validation loss:     {self.logs['val_loss'][epoch]:1.3f}" \
+                  f"Validation accuracy: {self.logs['val_acc'][epoch]:1.3f}"
         
-        logger.info(message)
+        logger.info(message)     
+
+    def on_train_batch_end(self, step: int, input_batch: InputFeatures):
+        """ Compute the performance metrics for each training batch """
+        epoch = self.epoch
+        output_batch = self.training_step.train_step_output
 
-    def on_train_batch_end(self, step: int):
-        """ Compute the performance metrics after each training batch """
-        loss = self.training_step.train_step_output.loss
-        self.train_metric(loss)
-        self.train_details['loss'][self.epoch].extend(loss)
-        self.train['loss'][self.epoch] = self.train_metric.result()
-        
-    def on_test_batch_end(self, step: int):
-        """ Compute the performance metrics after each testing batch """
-        loss = self.training_step.test_step_output.loss
-        self.test_metric(loss)
-        self.test_details['loss'][self.epoch].extend(loss)
-        self.test['loss'][self.epoch] = self.test_metric.result()
+        labels = input_batch.label
+        logits = output_batch.logits
+        loss = output_batch.loss
+        
+        self.loss_train_metric.update_state(loss)
+        self.acc_train_metric.update_state(labels, logits)
+        
+        self.logs['loss'][epoch] = self.loss_train_metric.result()
+        self.logs['acc'][epoch] = self.acc_train_metric.result()
+        
+        
+    def on_test_batch_end(self, step: int, input_batch: InputFeatures):
+        """ Compute the performance metrics for each testing batch """
+        epoch = self.epoch
+        output_batch = self.training_step.test_step_output
+        
+        labels = input_batch.label
+        logits = output_batch.logits
+        loss = output_batch.loss
+        
+        self.loss_test_metric.update_state(loss)
+        self.acc_test_metric.update_state(labels, logits)
+        
+        self.logs['val_loss'][epoch] = self.loss_test_metric.result()
+        self.logs['val_acc'][epoch] = self.acc_test_metric.result()
         
     @property
     def best_result(self) -> float:
-        return min(self.test['loss'].values())
+        return min(self.logs['val_loss'].values())
     
 
 @dataclass
 class ModelCheckpoint(Callback):
     """ Callback that save the model weights and configuration 
     after each epoch and to keep track of the best model """
     
@@ -317,15 +332,15 @@
             abs_path = os.path.abspath(self.checkpoints_dir)
             text = f'Make a checkpoint directory: {abs_path}'
             logger.info(text)
             os.makedirs(self.checkpoints_dir)
 
     def on_epoch_end(self, epoch: int):
         """ Pass the obj:`ModelCheckpoint` callback after the obj:`History`. """
-        result = self.history.test['loss'][epoch]
+        result = self.history.logs['val_loss'][epoch]
         diff = self.best_result - result
         is_better = diff > 0 if self.direction == 'minimize' else diff < 0
         if is_better:
             name = f'epoch-{epoch:02d}-{result:.2f}'
             model_dir = os.path.join(self.checkpoints_dir, name)
             os.mkdir(model_dir)
             self.model.config.architectures = self.model.__class__.__name__
@@ -385,15 +400,15 @@
         if self.direction not in ['minimize', 'maximize']:
             raise ValueError
         if self.direction == 'maximize':
             self.best_result = 0
 
     def on_epoch_end(self, epoch: int):
         """ """
-        result = self.history.test['loss'][epoch]
+        result = self.history.logs['val_loss'][epoch]
         diff = self.best_result - result
         is_better = diff > self.min_delta if self.direction == 'minimize' \
             else diff < self.min_delta * -1
         if is_better:
             self.best_result = result
             self.current_patience = 0
             return
@@ -444,15 +459,15 @@
 @dataclass
 class ProgbarLogger(Callback):
     """ Callbacks to monitor the progress of a model's training, 
     and display the progress bar and performance metrics in the
     console. """ 
     
     name: str = 'ProgbarLogger'
-    history: List[History] = None
+    history: History = None
     metric: Callable = tf.metrics.Mean
     epoch: int = field(default_factory=int)
     num_samples: int = None
     num_epochs: int = None
     batch_size: int = None
     show_overall_progress: bool = False
     show_epoch_progress: bool = True
@@ -511,18 +526,18 @@
 
         if self.steps_so_far <= self.num_steps:  
             now = time.time()
             time_diff = now - self.last_update_time
             if self.show_epoch_progress and time_diff >= self.update_interval:
                 
                 self.epoch_progress_tqdm.desc = \
-                     f'loss: {self.train_logs["loss"]:04F} - ' \
-                     f'val_loss: {self.test_logs["loss"]:04F}'
-                     #f'acc: {self.logs["accuracy"]:04F} - ' \
-                     #f'val_acc: {self.logs["test_accuracy"]:04F}'
+                     f"loss: {self.train_logs['loss']:04F} - " \
+                     f"accuracy: {self.train_logs['acc']:04F} - " \
+                     f"val_loss: {self.test_logs['loss']:04F} - " \
+                     f"val_accuracy: {self.test_logs['acc']:04F}"
 
                 self.epoch_progress_tqdm.update(self.steps_to_update)
                 self.steps_to_update = 0
                 self.last_update_time = now
                 
     def _clean_up_progbar(self, hook):
         if self.show_epoch_progress:
@@ -543,29 +558,31 @@
     def on_test_begin(self):
         if not self.is_training:
             self._initialize_progbar("test", epoch=None)
             
     def on_test_end(self):
         if not self.is_training:
             self._clean_up_progbar("test")
-     
+            
     def on_epoch_begin(self, epoch: int):
         self.epoch = epoch
         self._initialize_progbar("train", epoch)
     
     def on_epoch_end(self, epoch: int):
         self._clean_up_progbar("train")
         if self.show_overall_progress:
             self.overall_progress_tqdm.update(1)
         self.epoch_progress_tqdm.close()
 
-    def on_train_batch_end(self, step: int):
+    def on_train_batch_end(self, step: int, input_batch: InputFeatures):
         train_logs = defaultdict(float)
-        train_logs["loss"] = self.history.train['loss'][self.epoch]
+        train_logs["loss"] = self.history.logs['loss'][self.epoch]
+        train_logs["acc"] = self.history.logs['acc'][self.epoch]
         self.train_logs = train_logs
         self._update_progbar()
         
-    def on_test_batch_end(self, step: int):
+    def on_test_batch_end(self, step: int, input_batch: InputFeatures):
         test_logs = defaultdict(float)
-        test_logs["loss"] = self.history.test['loss'][self.epoch]
+        test_logs["loss"] = self.history.logs['val_loss'][self.epoch]
+        test_logs["acc"] = self.history.logs['val_acc'][self.epoch]
         self.test_logs = test_logs 
         self._update_progbar()
```

### Comparing `nlpipes-0.1.8/nlpipes/configurations/bert_config.py` & `nlpipes-0.1.9/nlpipes/configurations/bert_config.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/data/.ipynb_checkpoints/data_loaders-checkpoint.py` & `nlpipes-0.1.9/nlpipes/data/data_loaders.py`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,15 @@
             batch_examples.append(example)
             
             if len(batch_examples) == self.batch_size:
                 batch_features = self.data_processor(batch_examples)
                 batch_examples.clear() 
                 yield batch_features
     
-    def __len__(self) -> int:
+    def num_batches(self) -> int:
         """ Number of batches per epoch. """
         return math.ceil(len(self.examples) / self.batch_size)
    
     def num_examples(self) -> int:
         """ Number of dataset examples. """
         return len(self.examples)
+
```

### Comparing `nlpipes-0.1.8/nlpipes/data/.ipynb_checkpoints/data_processors-checkpoint.py` & `nlpipes-0.1.9/nlpipes/data/data_processors.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/data/.ipynb_checkpoints/data_selectors-checkpoint.py` & `nlpipes-0.1.9/nlpipes/data/data_selectors.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/data/.ipynb_checkpoints/data_splitters-checkpoint.py` & `nlpipes-0.1.9/nlpipes/data/data_splitters.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,18 +9,17 @@
 from nlpipes.data.data_types import InputExample
 
 
 @dataclass
 class TrainTestSplitter:
     """ Splits input data into training/test set """
         
-    train_frac: float = 0.75
-    test_frac: float = 0.25
+    train_frac: float = None
+    test_frac: float = None
     shufffle: bool = True
-    random_seed: int = 69
 
     def __call__(self, examples: List[InputExample]
                 ) -> Iterable:
         """  """
         
         n_examples = len(examples)
         n_train = int(np.ceil(n_examples*self.train_frac))
```

### Comparing `nlpipes-0.1.8/nlpipes/data/.ipynb_checkpoints/data_types-checkpoint.py` & `nlpipes-0.1.9/nlpipes/data/data_types.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/data/.ipynb_checkpoints/data_utils-checkpoint.py` & `nlpipes-0.1.9/nlpipes/data/data_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -46,18 +46,17 @@
         examples = [InputExample(text=text) for text in texts]
         
     return examples
 
 
 def split_examples(
     examples: List[InputExample],
-    train_frac: float = 0.75,
-    test_frac: float = 0.25, 
+    train_frac: float = None,
+    test_frac: float = None, 
     shufffle: bool = True, 
-    random_seed: int = 69,
    ) -> Tuple[InputExample]:
     """  """
     
     n_examples = len(examples)
     n_train = int(np.ceil(n_examples*train_frac))
     n_test = int(np.ceil(n_examples*test_frac))
     n_total = n_train + n_test
```

### Comparing `nlpipes-0.1.8/nlpipes/data/data_augmentors.py` & `nlpipes-0.1.9/nlpipes/data/data_augmentors.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/data/data_cleaners.py` & `nlpipes-0.1.9/nlpipes/data/data_cleaners.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/data/data_processors.py` & `nlpipes-0.1.9/nlpipes/pipelines/pipeline_utils.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,190 +1,209 @@
-from typing import Callable
-from typing import List
+from typing import (
+    List,
+    Optional,
+)
 
 from dataclasses import dataclass
 
-import copy
-
-import numpy as np
 import tensorflow as tf
+import transformers
 
 from transformers import (
     PretrainedConfig,
-    PreTrainedTokenizer,
-    AutoTokenizer,
+    PreTrainedTokenizerFast,
+    TFPreTrainedModel,
 )
 
-from nlpipes.data.data_types import InputExample
-from nlpipes.data.data_types import InputFeatures
+from tokenizers.pre_tokenizers import Whitespace
 
+#from nlpipes.losses.losses import softmax_cross_entropy
 
-""" The data processor classes.
+from nlpipes.data.data_selectors import DataSelector
+from nlpipes.data.data_augmentors import VocabAugmentor
+from nlpipes.data.data_processors import DataProcessorForSequenceClassification
+from nlpipes.data.data_cleaners import clean
+from nlpipes.data.data_utils import chunk
+
+from nlpipes.data.data_types import (
+     Corpus,
+     Document,
+     Token,
+     InputExample,
+     InputTokens,
+     InputFeatures,
+     Predictions,
+     Outcomes,
+)
 
-The data processor encapsulates all the transformations
-needed to encode input examples into input features 
-expected by the model. """
-
-
-@dataclass
-class DataProcessorForLanguageModeling:
-    
-    """ 
-    Data processor for Masked Language Modeling:
-    80% MASK, 10% random, 10% original.
-    Inputs are dynamically padded to the maximum 
-    length of a batch if they are not all of the 
-    same length.
-    
-    Args
-    ----------
-
-    tokenizer (transformers.PreTrainedTokenizer):
-        The tokenizer used for encoding the data.
-
-    config (transformers.PreTrainedCOnfig):
-        The configuration of the model.
-
-    """
-    name: str = 'LanguageModelingProcessor'
-    tokenizer: PreTrainedTokenizer = None
-    config: PretrainedConfig = None
-    mlm_proba: float = None
-    
-    def __call__(self, 
-                 examples: List[InputExample],
-                ) -> InputFeatures:
-        
-        texts = [example.text for example in examples]
-        
-        inputs = self.tokenizer(
-            texts,
-            add_special_tokens=True,
-            padding=True,
-            truncation=True,
-            max_length=512,
-            is_split_into_words=False,
-            return_tensors='tf',
-        )
-        
-        input_ids = tf.identity(inputs.input_ids)
-        
-        mask = self.create_mask(
-            inputs=inputs.input_ids,
-            mask_frac=self.mlm_proba,
-            excluded=self.tokenizer.all_special_ids,
-        )
-        
-        inputs['input_ids'] = self.apply_mask(
-            inputs=inputs.input_ids,
-            mask=mask,
-            mask_token_id=self.tokenizer.mask_token_id,
-        )
-        
-        labels = self.apply_mask(
-            inputs=input_ids,
-            mask=~mask,
-            mask_token_id=-100,
-        )
-        
-        inputs['label'] = tf.one_hot(
-            [label for label in labels],
-            depth=len(self.tokenizer)
-        )
-        
-        input_features = InputFeatures(
-            input_ids=inputs['input_ids'],
-            attention_mask=inputs['attention_mask'],
-            token_type_ids=inputs['token_type_ids'],
-            label=inputs['label'],
-        )
-        
-        return input_features
-    
-    def create_mask(
-        self,
-        inputs: tf.Tensor,
-        mask_frac: float,
-        excluded: tf.Tensor,  
-    ) -> tf.Tensor:
-        """ Create the mask used for the masked 
-        language modeling """
-        
-        random = tf.random.uniform(inputs.shape)
-        
-        mask = tf.math.logical_and(
-            random < mask_frac, 
-            ~np.isin(inputs, excluded),
-        )
-        
-        return mask
-    
-    def apply_mask(
-        self,
-        inputs: tf.Tensor,
-        mask: tf.Tensor,
-        mask_token_id: int,
-    ) -> tf.Tensor:
-        """ Apply the mask to the given inputs """
-        
-        masked_inputs = tf.where(
-            condition=mask,
-            x=mask_token_id,
-            y=inputs,
-        )
-        
-        return masked_inputs
+def select_corpus(
+    corpus: Corpus,
+    tokenizer: PreTrainedTokenizerFast,
+    target_corpus_size: int,
+    similarity_metrics: List[str],
+    diversity_metrics: List[str],
+) -> Corpus :
+    """ """
+
+    data_selector = DataSelector(
+        name='DataSelection',
+        tokenizer=tokenizer,
+        target_corpus_size=target_corpus_size,
+        similarity_metrics=similarity_metrics,
+        diversity_metrics=diversity_metrics,
+    )
+
+    clean_corpus = [clean(text) for text in corpus]
+    sub_corpus= data_selector(clean_corpus)
+
+    return sub_corpus
+
+def augment_vocabulary(
+    corpus: Corpus,
+    tokenizer: PreTrainedTokenizerFast, 
+    target_vocab_size: int,
+) -> List[Token]:
+    """ """
+
+    vocab_augmentor = VocabAugmentor(
+        name='VocabAugmentation',
+        tokenizer=tokenizer,
+        target_vocab_size=target_vocab_size,
+        cased=False, 
+    )
+
+    new_tokens = vocab_augmentor.get_new_tokens(corpus)
+
+    return new_tokens
+
+def preprocess(texts: Corpus,
+               labels: Optional[str] = None,
+               chunk_text: Optional[bool] = False,
+              ) -> List[InputExample]:
+    """ Serialize each raw text into examples. Raw texts can 
+    eventually be chunked into spans. E.g., at inference time,
+    each span need to be chunked into sentences if the model 
+    has been trained at the sentence level. """
+
+    if labels is not None:
+        input_examples = [
+            InputExample(text=text, label=label)
+            for text, label in zip(texts, labels)
+        ]
+    else:
+        spans = chunk(text) if chunk_text == True else texts
+        input_examples = [
+            InputExample(span) for span in spans
+        ]
+
+    return input_examples
+
+def tokenize(examples: List[InputExample],
+             tokenizer: PreTrainedTokenizerFast,
+            ) -> InputTokens:
+    """ Convert examples into tokens. Tokens encapsulate both 
+    words, wordpieces and enriched wordpieces with the special
+    [CLS] and [SEP] tokens. """
+
+    texts = [example.text for example in examples]
+
+    words = [Whitespace().pre_tokenize_str(text) for text in texts]
+
+    wordpieces = [
+        encoding.tokens for encoding 
+        in tokenizer.backend_tokenizer.encode_batch(
+           texts, add_special_tokens=False
+        )
+    ]
+
+    tokens = [
+        encoding.tokens for encoding 
+        in tokenizer.backend_tokenizer.encode_batch(
+           texts, add_special_tokens=True
+        )
+    ]
+
+    input_tokens = InputTokens(
+        words=words,
+        wordpieces=wordpieces,
+        tokens=tokens,
+    )
+
+    return input_tokens
+
+def encode(tokens: InputTokens,
+           tokenizer: PreTrainedTokenizerFast,
+          ) -> InputFeatures: 
+    """ Encode human-readable wordpieces into encoded features
+    that can be use as input by the model. """
+
+    inputs = tokenizer(
+       tokens.wordpieces,
+       add_special_tokens=False,
+       padding=True,
+       truncation=True,
+       max_length=512,
+       is_split_into_words = True,
+       return_tensors='tf',
+    )
+
+    input_features = InputFeatures(
+       input_ids=inputs['input_ids'],
+       attention_mask=inputs['attention_mask'],
+       token_type_ids=inputs['token_type_ids'],
+    )
+
+    return input_features
+
+def estimate(features: InputFeatures,
+             model: TFPreTrainedModel,
+             config: PretrainedConfig,
+            ) -> Predictions:
+    """ Predict the label index matching the maximum prediction
+    score and compute the loss value associated with each
+    prediction."""
+
+    outputs = model.call(
+        input_ids=features.input_ids,
+        attention_mask=features.attention_mask,
+        token_type_ids=features.token_type_ids,
+    )
+
+    logits = outputs.logits
+    label = tf.argmax(logits, axis=-1)
+    label_onehot = tf.one_hot(label, config.num_labels)
+    scores = tf.nn.softmax(logits, axis=1)
+    losses = tf.nn.softmax_cross_entropy_with_logits(
+        label_onehot, logits, axis=-1, name='Loss')
+
+    predictions = Predictions(
+        label=label,
+        scores=scores,
+        losses=losses,
+    )
+
+    return predictions
+
+def postprocess(predictions: Predictions, 
+                config: PretrainedConfig,
+               ) -> Outcomes:
+    """ Convert outputs tensors into more handy numpy lists. """
+
+    indice = [label.numpy() for label in predictions.label]
+    scores = [
+        score.numpy().tolist() 
+        for score in predictions.scores
+    ] 
+    losses = [loss.numpy() for loss in predictions.losses]
+
+    label = [config.id2label[idx] for idx in indice]
+
+    outcomes = Outcomes(
+        indice=indice,
+        label=label,
+        scores=scores,
+        losses=losses,
+    )
+
+    return outcomes
 
 
-@dataclass
-class DataProcessorForSequenceClassification:
-    
-    """
-    Data Processor for Sequence Classification.
-    Inputs are dynamically padded to the maximum 
-    length of a batch if they are not all of the 
-    same length.
-    
-    Args
-    ----------
-
-    tokenizer (transformers.PreTrainedTokenizer):
-        The tokenizer used for encoding the data.
-
-    config (transformers.PreTrainedCOnfig):
-        The configuration of the model.
-
-    """
-    name: str = 'SequenceClassificationProcessor'
-    tokenizer: PreTrainedTokenizer = None
-    config: PretrainedConfig = None
-    
-    def __call__(self, 
-                 examples: List[InputExample],
-                ) -> InputFeatures:
-        
-        texts = [example.text for example in examples]
-        
-        inputs = self.tokenizer(
-            texts,
-            add_special_tokens=True,
-            padding=True,
-            truncation = True,
-            max_length=512,
-            is_split_into_words = False,
-            return_tensors='tf',
-        )
-        
-        inputs['label'] = tf.one_hot(
-            [example.label for example in examples],
-            depth=self.config.num_labels
-        )
-        
-        input_features = InputFeatures(
-            input_ids=inputs['input_ids'],
-            attention_mask=inputs['attention_mask'],
-            token_type_ids=inputs['token_type_ids'],
-            label=inputs['label'],
-        )
-        
-        return input_features
-
```

### Comparing `nlpipes-0.1.8/nlpipes/layers/bert_layers.py` & `nlpipes-0.1.9/nlpipes/layers/bert_layers.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/metrics/.ipynb_checkpoints/confusion-checkpoint.py` & `nlpipes-0.1.9/nlpipes/metrics/confusion.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/metrics/.ipynb_checkpoints/diversity-checkpoint.py` & `nlpipes-0.1.9/nlpipes/metrics/diversity.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/metrics/.ipynb_checkpoints/similarity-checkpoint.py` & `nlpipes-0.1.9/nlpipes/metrics/similarity.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/models/.ipynb_checkpoints/language_modeling-checkpoint.py` & `nlpipes-0.1.9/nlpipes/models/language_modeling.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/models/.ipynb_checkpoints/sequence_classification-checkpoint.py` & `nlpipes-0.1.9/nlpipes/models/sequence_classification.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/optimization/.ipynb_checkpoints/optimizers-checkpoint.py` & `nlpipes-0.1.9/nlpipes/optimization/optimizers.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/optimization/.ipynb_checkpoints/schedulers-checkpoint.py` & `nlpipes-0.1.9/nlpipes/optimization/schedulers.py`

 * *Files identical despite different names*

### Comparing `nlpipes-0.1.8/nlpipes/pipelines/.ipynb_checkpoints/language_modeling-checkpoint.py` & `nlpipes-0.1.9/nlpipes/pipelines/language_modeling.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
             patience=patience,
         )
         
         timed_stopping = TimedStopping(
             name='TimedStopping',
             time_limit=time_limit,
         )
-       
+        
         csv_logger = CSVLogger(
             name='CSVLogging',
             logs_dir=logs_dir,
         )
         
         progbar_logger = ProgbarLogger(
             name='ProgbarLogger',
```

### Comparing `nlpipes-0.1.8/nlpipes/pipelines/.ipynb_checkpoints/sequence_classification-checkpoint.py` & `nlpipes-0.1.9/nlpipes/pipelines/sequence_classification.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,15 +156,16 @@
             loss_function=softmax_cross_entropy,
             optimizer=tf.optimizers.Adam(lr),
         )
         
         history = History(
             name='History', 
             training_step=training_step,
-            metric=tf.metrics.Mean,
+            loss_metric = tf.metrics.Mean,
+            acc_metric = tf.metrics.CategoricalAccuracy,
         )
         
         model_checkpoint = ModelCheckpoint(
             name='ModelCheckpoint',
             model=self.model, 
             history=history,
             checkpoints_dir=checkpoints_dir,
@@ -178,15 +179,15 @@
             patience=patience,
         )
         
         timed_stopping = TimedStopping(
             name='TimedStopping',
             time_limit=time_limit,
         )
-       
+        
         csv_logger = CSVLogger(
             name='CSVLogging',
             logs_dir=logs_dir,
         )
         
         progbar_logger = ProgbarLogger(
             name='ProgbarLogger',
@@ -216,15 +217,15 @@
             num_epochs=num_epochs,
         )
         
         trainer.train()
         
         if keep_checkpoints == False:
             shutil.rmtree(checkpoints_dir)
-         
+            
         return history
     
     def evaluate(self,
                  X: List[str],
                  Y: List[str],
                  metric: tf.metrics.Metric,
                  batch_size: int = 32,
```

### Comparing `nlpipes-0.1.8/nlpipes/trainers/.ipynb_checkpoints/trainers-checkpoint.py` & `nlpipes-0.1.9/nlpipes/trainers/trainers.py`

 * *Files 14% similar despite different names*

```diff
@@ -36,28 +36,32 @@
         
         callbacks = CallbackList(self.callbacks)
         
         try:
             callbacks.on_train_begin()
             
             for epoch in range(self.num_epochs):
-                
                 callbacks.on_epoch_begin(epoch)
                 
                 for step, batch in enumerate(self.train_stream):
                     callbacks.on_train_batch_begin(step, batch)
-                    callbacks.on_train_batch_end(step)
+                    callbacks.on_train_batch_end(step, batch)
                     
                 if self.test_stream:
+                    callbacks.on_test_begin()
+                    
                     for step, batch in enumerate(self.test_stream):
                         callbacks.on_test_batch_begin(step, batch)
-                        callbacks.on_test_batch_end(step)
-                       
+                        callbacks.on_test_batch_end(step, batch)
+                        
+                    callbacks.on_test_end()
+                    
                 callbacks.on_epoch_end(epoch)
                 
             callbacks.on_train_end()
              
         except:
             message = 'Unexpected error during the training process.'
             logger.error(message)
             exit()
+
```

### Comparing `nlpipes-0.1.8/pyproject.toml` & `nlpipes-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "nlpipes"
-version = "0.1.8"
+version = "0.1.9"
 description = "Text Classification with Transformers"
 authors = ["Ayhan UYANIK <ayhan.uyanik@renault.com>"]
 license = "Apache 2.0"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.7,<4.0"
```

### Comparing `nlpipes-0.1.8/setup.py` & `nlpipes-0.1.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,31 +1,22 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
 ['nlpipes',
- 'nlpipes..ipynb_checkpoints',
  'nlpipes.callbacks',
- 'nlpipes.callbacks..ipynb_checkpoints',
  'nlpipes.configurations',
  'nlpipes.data',
- 'nlpipes.data..ipynb_checkpoints',
  'nlpipes.layers',
  'nlpipes.losses',
- 'nlpipes.losses..ipynb_checkpoints',
  'nlpipes.metrics',
- 'nlpipes.metrics..ipynb_checkpoints',
  'nlpipes.models',
- 'nlpipes.models..ipynb_checkpoints',
  'nlpipes.optimization',
- 'nlpipes.optimization..ipynb_checkpoints',
  'nlpipes.pipelines',
- 'nlpipes.pipelines..ipynb_checkpoints',
- 'nlpipes.trainers',
- 'nlpipes.trainers..ipynb_checkpoints']
+ 'nlpipes.trainers']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['ftfy>=6.1.1,<7.0.0',
  'numpy>=1.21.0,<2.0.0',
@@ -34,17 +25,17 @@
  'tensorflow>=2.11.0,<3.0.0',
  'tokenizers>=0.13.0,<0.14.0',
  'tqdm>=4.64.0,<5.0.0',
  'transformers>=4.24.0,<5.0.0']
 
 setup_kwargs = {
     'name': 'nlpipes',
-    'version': '0.1.8',
+    'version': '0.1.9',
     'description': 'Text Classification with Transformers',
-    'long_description': '<!-- PROJECT NAME -->\n<div align="center">\n  <h2>NLPIPES</h2>\n  <h3>Text Classification with Transformers</h3>\n</div>\n\n<div align="center">\n    <a href="https://opensource.org/licenses/Apache-2.0">\n       <img alt="Licence" src="https://img.shields.io/badge/License-Apache_2.0-blue.svg">\n    </a>\n     <a href="https://opensource.org/licenses/Apache-2.0">\n       <img alt="PyPi Version" src="https://img.shields.io/pypi/pyversions/nlpipes">\n    </a> \n    <a href="https://pypi.org/project/nlpipes/">\n        <img alt="PyPi Package Version" src="https://img.shields.io/pypi/v/nlpipes">\n    </a>\n    <!--\n    <a href="https://pepy.tech/project/nlpipes/">\n        <img alt="PyPi Downloads" src="https://static.pepy.tech/badge/nlpipes/month">\n    </a>\n    -->\n</div>\n\n<div align="center">\n    <a href=""><strong>Documentation</strong></a>\n    • <a href=""><strong>References</strong></a>\n</div>\n\n<div align="center">\n  <img src="https://raw.githubusercontent.com/uyanik/Images/dd6d7682a6b0e1bc504a5b9da1fe930e01a39aab/nlpipes_screenshot.png" alt="nlpipes_screenshot" title="nlpipes screenshot">\n</div>\n\n`NLPipes` provides an easy way to use Transformers-based models for training, evaluation and inference on a diversity of text classification tasks, including:\n\n* **Single-label classification**: Assign one label to each text. A typical use case is sentiment analysis where one want to detect the overall sentiment polarity (e.g., positive, neutral, negative) in a review.\n* **Multi-labels classification** [Not yet implemented]: Assign one or more label to each text from a list of possible labels. A typical use case is categories detection where one want to detect the multiple aspects mentionned in a review (e.g., #product_quality, #delivery_time, #price, ...).\n* **Aspect-based classification** [Not yet implemented]: Assign one label from a list of possible labels for each of a list of aspects. A typical use case is aspect based sentiment analysis where one want to detect each aspect mentionned in a review along his assocated sentiment polarity (e.g., #product_quality: neutral, #delivery_time: negative, #price: positive, ...).\n* **Zero-shot classification** [Not yet implemented]: Assign one or more label to each text from a list of possible labels without the requirement of an annotated training dataset.\n\n`NLPipes` expose a simple `Model` API that offers a common abstraction to run several text classification tasks. The `Model` encapsulate most of the complex code from the library and save having to deal with the complexity of transformers based algorithms.\n\n#### Built with\n`NLPipes` is built with TensorFlow and HuggingFace Transformers:\n* [TensorFlow](https://www.tensorflow.org/): An end-to-end open source deep learning framework\n* [Transformers](https://huggingface.co/transformers/): An general-purpose open-sources library for transformers-based architectures\n\n## Getting Started\n\n#### Installation\n1. Create a virtual environment\n\n ```console\n python3 -m venv nlpipesenv\n source nlpipesenv/bin/activate\n ```\n\n2. Install the package\n\n ```console\n pip install nlpipes\n ```\n\n#### Examples\n\nHere are some use-cases with `NLPipes` on real datasets:\n\nName|Notebook|Description|Task|Size|Memory| \n----|-----------|-----|---------|---------|---------|\nGooglePlay Sentiment Detection|[Link]("")|Train a model to label reviews from the GooglePlay store reviews|Single-label classification|  |  \nStackOverflow tags Detection|Coming soon|Train a model to detect tags from the StackOverFlow questions |Multiple-labels classification|  | \nGooglePlay Aspect and Sentiment Detection|Coming soon|Train a model for aspect based sentiment detection to detect the aspects mentionned in GooglePlay reviews along his assocated sentiment polarity |Aspect-based classification|  | \n\n\n## Notice\n`NLPipes` is still in its early stage and is not yet suitable for production usage. Proceed with caution and use it at your own risk. The library comes with no warranty and future releases could bring substantial API and behavior changes.\n',
+    'long_description': '<!-- PROJECT NAME -->\n<div align="center">\n  <h2>NLPIPES</h2>\n  <h3>Text Classification with Transformers</h3>\n</div>\n\n<div align="center">\n    <a href="https://opensource.org/licenses/Apache-2.0">\n       <img alt="Licence" src="https://img.shields.io/badge/License-Apache_2.0-blue.svg">\n    </a>\n     <a href="https://pypi.org/project/nlpipes/">\n       <img alt="PyPi Version" src="https://img.shields.io/pypi/pyversions/nlpipes">\n    </a> \n    <a href="https://pypi.org/project/nlpipes/">\n        <img alt="PyPi Package Version" src="https://img.shields.io/pypi/v/nlpipes">\n    </a>\n    <!--\n    <a href="https://pepy.tech/project/nlpipes/">\n        <img alt="PyPi Downloads" src="https://static.pepy.tech/badge/nlpipes/month">\n    </a>\n    -->\n</div>\n\n<div align="center">\n    <a href=""><strong>Documentation</strong></a>\n    • <a href=""><strong>References</strong></a>\n</div>\n\n<div align="center">\n  <img src="https://raw.githubusercontent.com/uyanik/Images/dd6d7682a6b0e1bc504a5b9da1fe930e01a39aab/nlpipes_screenshot.png" alt="nlpipes_screenshot" title="nlpipes screenshot">\n</div>\n\n`NLPipes` provides an easy way to use Transformers-based models for training, evaluation and inference on a diversity of text classification tasks, including:\n\n* **Single-label classification**: Assign one label to each text. A typical use case is sentiment analysis where one want to detect the overall sentiment polarity (e.g., positive, neutral, negative) in a review.\n* **Multi-labels classification** [Not yet implemented]: Assign one or more label to each text from a list of possible labels. A typical use case is categories detection where one want to detect the multiple aspects mentionned in a review (e.g., #product_quality, #delivery_time, #price, ...).\n* **Aspect-based classification** [Not yet implemented]: Assign one label from a list of possible labels for each of a list of aspects. A typical use case is aspect based sentiment analysis where one want to detect each aspect mentionned in a review along his assocated sentiment polarity (e.g., #product_quality: neutral, #delivery_time: negative, #price: positive, ...).\n* **Zero-shot classification** [Not yet implemented]: Assign one or more label to each text from a list of possible labels without the requirement of an annotated training dataset.\n\n`NLPipes` expose a simple `Model` API that offers a common abstraction to run several text classification tasks. The `Model` encapsulate most of the complex code from the library and save having to deal with the complexity of transformers based algorithms.\n\n#### Built with\n`NLPipes` is built with TensorFlow and HuggingFace Transformers:\n* [TensorFlow](https://www.tensorflow.org/): An end-to-end open source deep learning framework\n* [Transformers](https://huggingface.co/transformers/): An general-purpose open-sources library for transformers-based architectures\n\n## Getting Started\n\n#### Installation\n1. Create a virtual environment\n\n ```console\n python3 -m venv nlpipesenv\n source nlpipesenv/bin/activate\n ```\n\n2. Install the package\n\n ```console\n pip install nlpipes\n ```\n\n#### Examples\n\nHere are some use-cases with `NLPipes` on real datasets:\n\nName|Notebook|Description|Task|Size|Memory| \n----|-----------|-----|---------|---------|---------|\nGooglePlay Sentiment Detection|[Link]("/notebooks/googleplay_sentiment_labeling.ipynb")|Train a model to label reviews from the GooglePlay store reviews|Single-label classification|  |  \nStackOverflow tags Detection|Coming soon|Train a model to detect tags from the StackOverFlow questions |Multiple-labels classification|  | \nGooglePlay Aspect and Sentiment Detection|Coming soon|Train a model for aspect based sentiment detection to detect the aspects mentionned in GooglePlay reviews along his assocated sentiment polarity |Aspect-based classification|  | \n\n\n## Notice\n`NLPipes` is still in its early stage and is not yet suitable for production usage. Proceed with caution and use it at your own risk. The library comes with no warranty and future releases could bring substantial API and behavior changes.\n',
     'author': 'Ayhan UYANIK',
     'author_email': 'ayhan.uyanik@renault.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

#### html2text {}

```diff
@@ -1,23 +1,17 @@
 # -*- coding: utf-8 -*- from setuptools import setup packages = \ ['nlpipes',
-'nlpipes..ipynb_checkpoints', 'nlpipes.callbacks',
-'nlpipes.callbacks..ipynb_checkpoints', 'nlpipes.configurations',
-'nlpipes.data', 'nlpipes.data..ipynb_checkpoints', 'nlpipes.layers',
-'nlpipes.losses', 'nlpipes.losses..ipynb_checkpoints', 'nlpipes.metrics',
-'nlpipes.metrics..ipynb_checkpoints', 'nlpipes.models',
-'nlpipes.models..ipynb_checkpoints', 'nlpipes.optimization',
-'nlpipes.optimization..ipynb_checkpoints', 'nlpipes.pipelines',
-'nlpipes.pipelines..ipynb_checkpoints', 'nlpipes.trainers',
-'nlpipes.trainers..ipynb_checkpoints'] package_data = \ {'': ['*']}
-install_requires = \ ['ftfy>=6.1.1,<7.0.0', 'numpy>=1.21.0,<2.0.0',
-'pandas>=1.3.5,<2.0.0', 'scipy>=1.7.3,<2.0.0', 'tensorflow>=2.11.0,<3.0.0',
-'tokenizers>=0.13.0,<0.14.0', 'tqdm>=4.64.0,<5.0.0',
-'transformers>=4.24.0,<5.0.0'] setup_kwargs = { 'name': 'nlpipes', 'version':
-'0.1.8', 'description': 'Text Classification with Transformers',
-'long_description': '\n
+'nlpipes.callbacks', 'nlpipes.configurations', 'nlpipes.data',
+'nlpipes.layers', 'nlpipes.losses', 'nlpipes.metrics', 'nlpipes.models',
+'nlpipes.optimization', 'nlpipes.pipelines', 'nlpipes.trainers'] package_data =
+\ {'': ['*']} install_requires = \ ['ftfy>=6.1.1,<7.0.0',
+'numpy>=1.21.0,<2.0.0', 'pandas>=1.3.5,<2.0.0', 'scipy>=1.7.3,<2.0.0',
+'tensorflow>=2.11.0,<3.0.0', 'tokenizers>=0.13.0,<0.14.0',
+'tqdm>=4.64.0,<5.0.0', 'transformers>=4.24.0,<5.0.0'] setup_kwargs = { 'name':
+'nlpipes', 'version': '0.1.9', 'description': 'Text Classification with
+Transformers', 'long_description': '\n
                                       \n
                               ***** NLPIPES *****
                                       \n
                 **** Text Classification with Transformers ****
                                       \n
 \n\n
   \n \n_[Licence]\n\n \n_[PyPi_Version]\n \n \n_[PyPi_Package_Version]\n\n \n
@@ -50,22 +44,23 @@
 [Transformers](https://huggingface.co/transformers/): An general-purpose open-
 sources library for transformers-based architectures\n\n## Getting
 Started\n\n#### Installation\n1. Create a virtual environment\n\n ```console\n
 python3 -m venv nlpipesenv\n source nlpipesenv/bin/activate\n ```\n\n2. Install
 the package\n\n ```console\n pip install nlpipes\n ```\n\n#### Examples\n\nHere
 are some use-cases with `NLPipes` on real datasets:
 \n\nName|Notebook|Description|Task|Size|Memory| \n----|-----------|-----|------
----|---------|---------|\nGooglePlay Sentiment Detection|[Link]("")|Train a
-model to label reviews from the GooglePlay store reviews|Single-label
-classification| | \nStackOverflow tags Detection|Coming soon|Train a model to
-detect tags from the StackOverFlow questions |Multiple-labels classification| |
-\nGooglePlay Aspect and Sentiment Detection|Coming soon|Train a model for
-aspect based sentiment detection to detect the aspects mentionned in GooglePlay
-reviews along his assocated sentiment polarity |Aspect-based classification| |
-\n\n\n## Notice\n`NLPipes` is still in its early stage and is not yet suitable
-for production usage. Proceed with caution and use it at your own risk. The
-library comes with no warranty and future releases could bring substantial API
-and behavior changes.\n', 'author': 'Ayhan UYANIK', 'author_email':
+---|---------|---------|\nGooglePlay Sentiment Detection|[Link]("/notebooks/
+googleplay_sentiment_labeling.ipynb")|Train a model to label reviews from the
+GooglePlay store reviews|Single-label classification| | \nStackOverflow tags
+Detection|Coming soon|Train a model to detect tags from the StackOverFlow
+questions |Multiple-labels classification| | \nGooglePlay Aspect and Sentiment
+Detection|Coming soon|Train a model for aspect based sentiment detection to
+detect the aspects mentionned in GooglePlay reviews along his assocated
+sentiment polarity |Aspect-based classification| | \n\n\n## Notice\n`NLPipes`
+is still in its early stage and is not yet suitable for production usage.
+Proceed with caution and use it at your own risk. The library comes with no
+warranty and future releases could bring substantial API and behavior
+changes.\n', 'author': 'Ayhan UYANIK', 'author_email':
 'ayhan.uyanik@renault.com', 'maintainer': 'None', 'maintainer_email': 'None',
 'url': 'None', 'packages': packages, 'package_data': package_data,
 'install_requires': install_requires, 'python_requires': '>=3.7,<4.0', } setup
 (**setup_kwargs)
```

### Comparing `nlpipes-0.1.8/PKG-INFO` & `nlpipes-0.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlpipes
-Version: 0.1.8
+Version: 0.1.9
 Summary: Text Classification with Transformers
 License: Apache 2.0
 Author: Ayhan UYANIK
 Author-email: ayhan.uyanik@renault.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
@@ -29,15 +29,15 @@
   <h3>Text Classification with Transformers</h3>
 </div>
 
 <div align="center">
     <a href="https://opensource.org/licenses/Apache-2.0">
        <img alt="Licence" src="https://img.shields.io/badge/License-Apache_2.0-blue.svg">
     </a>
-     <a href="https://opensource.org/licenses/Apache-2.0">
+     <a href="https://pypi.org/project/nlpipes/">
        <img alt="PyPi Version" src="https://img.shields.io/pypi/pyversions/nlpipes">
     </a> 
     <a href="https://pypi.org/project/nlpipes/">
         <img alt="PyPi Package Version" src="https://img.shields.io/pypi/v/nlpipes">
     </a>
     <!--
     <a href="https://pepy.tech/project/nlpipes/">
@@ -87,15 +87,15 @@
 
 #### Examples
 
 Here are some use-cases with `NLPipes` on real datasets:
 
 Name|Notebook|Description|Task|Size|Memory| 
 ----|-----------|-----|---------|---------|---------|
-GooglePlay Sentiment Detection|[Link]("")|Train a model to label reviews from the GooglePlay store reviews|Single-label classification|  |  
+GooglePlay Sentiment Detection|[Link]("/notebooks/googleplay_sentiment_labeling.ipynb")|Train a model to label reviews from the GooglePlay store reviews|Single-label classification|  |  
 StackOverflow tags Detection|Coming soon|Train a model to detect tags from the StackOverFlow questions |Multiple-labels classification|  | 
 GooglePlay Aspect and Sentiment Detection|Coming soon|Train a model for aspect based sentiment detection to detect the aspects mentionned in GooglePlay reviews along his assocated sentiment polarity |Aspect-based classification|  | 
 
 
 ## Notice
 `NLPipes` is still in its early stage and is not yet suitable for production usage. Proceed with caution and use it at your own risk. The library comes with no warranty and future releases could bring substantial API and behavior changes.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nlpipes Version: 0.1.8 Summary: Text Classification
+Metadata-Version: 2.1 Name: nlpipes Version: 0.1.9 Summary: Text Classification
 with Transformers License: Apache 2.0 Author: Ayhan UYANIK Author-email:
 ayhan.uyanik@renault.com Requires-Python: >=3.7,<4.0 Classifier: License ::
 Other/Proprietary License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Requires-Dist: ftfy (>=6.1.1,<7.0.0) Requires-Dist:
@@ -40,18 +40,18 @@
 www.tensorflow.org/): An end-to-end open source deep learning framework *
 [Transformers](https://huggingface.co/transformers/): An general-purpose open-
 sources library for transformers-based architectures ## Getting Started ####
 Installation 1. Create a virtual environment ```console python3 -m venv
 nlpipesenv source nlpipesenv/bin/activate ``` 2. Install the package ```console
 pip install nlpipes ``` #### Examples Here are some use-cases with `NLPipes` on
 real datasets: Name|Notebook|Description|Task|Size|Memory| ----|-----------|---
---|---------|---------|---------| GooglePlay Sentiment Detection|[Link]
-("")|Train a model to label reviews from the GooglePlay store reviews|Single-
-label classification| | StackOverflow tags Detection|Coming soon|Train a model
-to detect tags from the StackOverFlow questions |Multiple-labels
-classification| | GooglePlay Aspect and Sentiment Detection|Coming soon|Train a
-model for aspect based sentiment detection to detect the aspects mentionned in
-GooglePlay reviews along his assocated sentiment polarity |Aspect-based
-classification| | ## Notice `NLPipes` is still in its early stage and is not
-yet suitable for production usage. Proceed with caution and use it at your own
-risk. The library comes with no warranty and future releases could bring
-substantial API and behavior changes.
+--|---------|---------|---------| GooglePlay Sentiment Detection|[Link]("/
+notebooks/googleplay_sentiment_labeling.ipynb")|Train a model to label reviews
+from the GooglePlay store reviews|Single-label classification| | StackOverflow
+tags Detection|Coming soon|Train a model to detect tags from the StackOverFlow
+questions |Multiple-labels classification| | GooglePlay Aspect and Sentiment
+Detection|Coming soon|Train a model for aspect based sentiment detection to
+detect the aspects mentionned in GooglePlay reviews along his assocated
+sentiment polarity |Aspect-based classification| | ## Notice `NLPipes` is still
+in its early stage and is not yet suitable for production usage. Proceed with
+caution and use it at your own risk. The library comes with no warranty and
+future releases could bring substantial API and behavior changes.
```

