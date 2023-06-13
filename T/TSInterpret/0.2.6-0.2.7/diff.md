# Comparing `tmp/TSInterpret-0.2.6.tar.gz` & `tmp/TSInterpret-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSInterpret-0.2.6.tar", last modified: Mon Jun 12 13:03:13 2023, max compression
+gzip compressed data, was "TSInterpret-0.2.7.tar", last modified: Tue Jun 13 07:01:45 2023, max compression
```

## Comparing `TSInterpret-0.2.6.tar` & `TSInterpret-0.2.7.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.816234 TSInterpret-0.2.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.808234 TSInterpret-0.2.6/ClassificationModels/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/ClassificationModels/CNN.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/ClassificationModels/CNN_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/ClassificationModels/DecisionTree.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/ClassificationModels/LSTM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/ClassificationModels/LSTM_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/ClassificationModels/ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/ClassificationModels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/ClassificationModels/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-12 13:03:13.816234 TSInterpret-0.2.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.808234 TSInterpret-0.2.6/TSInterpret/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.812234 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/FeatureAttribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.812234 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/GradCam/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/GradCam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/InstanceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.812234 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/Saliency/
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/Saliency/TSR.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/Saliency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.812234 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10517 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/CF.py
--rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.812234 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.812234 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.816234 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.816234 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/leftist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/neighbors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.816234 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.816234 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.816234 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.816234 TSInterpret-0.2.6/TSInterpret/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/Models/PyTorchModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/Models/SklearnModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/Models/TensorflowModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/Models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/TSInterpret/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 13:03:13.812234 TSInterpret-0.2.6/TSInterpret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-12 13:03:13.000000 TSInterpret-0.2.6/TSInterpret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-12 13:03:13.000000 TSInterpret-0.2.6/TSInterpret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 13:03:13.000000 TSInterpret-0.2.6/TSInterpret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-12 13:03:13.000000 TSInterpret-0.2.6/TSInterpret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-12 13:03:13.000000 TSInterpret-0.2.6/TSInterpret.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 13:03:13.816234 TSInterpret-0.2.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-12 13:03:03.000000 TSInterpret-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.341606 TSInterpret-0.2.7/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.329606 TSInterpret-0.2.7/ClassificationModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/CNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/CNN_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/DecisionTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/LSTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/LSTM_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-13 07:01:45.341606 TSInterpret-0.2.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.329606 TSInterpret-0.2.7/TSInterpret/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.329606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/FeatureAttribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.329606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/GradCam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/GradCam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/InstanceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.333606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/TSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.333606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/CF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.333606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.333606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.337606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.337606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/leftist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/neighbors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.337606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.337606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.337606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.341606 TSInterpret-0.2.7/TSInterpret/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/Models/PyTorchModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/Models/SklearnModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/Models/TensorflowModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/Models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.329606 TSInterpret-0.2.7/TSInterpret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-13 07:01:45.000000 TSInterpret-0.2.7/TSInterpret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-13 07:01:45.000000 TSInterpret-0.2.7/TSInterpret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:01:45.000000 TSInterpret-0.2.7/TSInterpret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-13 07:01:45.000000 TSInterpret-0.2.7/TSInterpret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 07:01:45.000000 TSInterpret-0.2.7/TSInterpret.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:01:45.341606 TSInterpret-0.2.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/setup.py
```

### Comparing `TSInterpret-0.2.6/ClassificationModels/CNN.py` & `TSInterpret-0.2.7/ClassificationModels/CNN.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/ClassificationModels/CNN_T.py` & `TSInterpret-0.2.7/ClassificationModels/CNN_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/ClassificationModels/DecisionTree.py` & `TSInterpret-0.2.7/ClassificationModels/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/ClassificationModels/LSTM.py` & `TSInterpret-0.2.7/ClassificationModels/LSTM.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/ClassificationModels/LSTM_T.py` & `TSInterpret-0.2.7/ClassificationModels/LSTM_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/ClassificationModels/ResNet.py` & `TSInterpret-0.2.7/ClassificationModels/ResNet.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/ClassificationModels/utils.py` & `TSInterpret-0.2.7/ClassificationModels/utils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/LICENSE` & `TSInterpret-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/PKG-INFO` & `TSInterpret-0.2.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.2.6
+Version: 0.2.7
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.6 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.7 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
```

### Comparing `TSInterpret-0.2.6/README.md` & `TSInterpret-0.2.7/README.md`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/FeatureAttribution.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/FeatureAttribution.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/InterpretabilityBase.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/InterpretabilityBase.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/Saliency/TSR.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/TSR.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/Ates.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/Ates.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/CF.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/CF.py`

 * *Files 1% similar despite different names*

```diff
@@ -173,15 +173,15 @@
             org_label int: originally predicted label.
             exp np.array: returned explanation. Shape: `mode = time` -> `(time, feat)` or `mode = time` -> `(feat, time)`
             cf_label int: lebel of returned instance.
             figsize Tuple: Size of Figure (x,y).
             save_fig str: Path to Save the figure.
         """
         if self.mode == "time":
-            item = item.reshape(item.shape[0], item.shape[2], item.shape[1])
+            item = item.reshape(item.shape[-1], item.shape[-2])
         # TODO This is new and needs to be testes
         ind = ""
         # print("Item Shape", item.shape[-2])
         if item.shape[-2] > 1:
 
             res = (item != exp).any(-1)
             # print(res)
```

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,14 +34,15 @@
         neighborhood,
         window,
         channels,
         backend,
         transformer="authentic_opposing_information",
         epochs=500,
         verbose=0,
+        mode="feat",
     ):
         """
         Initialization of Optimization Algorithm
         Args:
             model: Keras or Tensorflow Model.
             original_x (np.array): Original instance.
             original_y (np.array): Classification Probability of instance.
@@ -63,25 +64,27 @@
         # self.LAMBDA = 200
         # prob that an offspring produced by crossover
         self.CXPB = 0.9
         # prob that an offspring produced by mutation
         self.MUTPB = 0.6  # 0.6
         # print('Create MOP')
         # self.neighborhood=neighborhood
+
         self.verbose = verbose
         self.mop = MultiObjectiveCounterfactuals(
             model,
             observation_x,
             original_y,
             target_y,
             reference_set,
             neighborhood,
             window,
             backend,
             channels,
+            mode=mode,
         )
         # print('Finished Create MOP')
         """Create types"""
         creator.create("FitnessMin", base.Fitness, weights=(-1.0, -1.0, -1.0))
         # print('Channels', channels)
         if channels == 1:
             creator.create(
```

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,20 +16,21 @@
         original_y,
         target,
         reference_set,
         neighborhood,
         window,
         backend="torch",
         channels=1,
+        mode="feat",
     ):
 
         super().__init__(n_var=channels, n_obj=3, n_constr=0, evaluation_of="auto")
 
         self.model = model
-
+        self.mode = mode
         self.window = window
         self.observation = observation
         print(self.observation.shape)
         self.target = target
         self.original_y = original_y
         if len(original_y) > 1:
             self.original_label = np.argmax(original_y, axis=1)[0]
@@ -99,17 +100,24 @@
         return np.sum(np.abs(first - second)) / (first.shape[-1] * first.shape[-2])
 
     def get_prediction_torch(
         self,
         individual,
         full=False,
     ):
-
+        if self.mode == "time":
+            individual = individual.reshape(
+                1, individual.shape[-1], individual.shape[-2]
+            )
+        else:
+            individual = individual.reshape(
+                1, individual.shape[-2], individual.shape[-1]
+            )
         individual = np.array(individual.tolist(), dtype=np.float64)
-        input_ = torch.from_numpy(individual).float().reshape(1, -1, self.window)
+        input_ = torch.from_numpy(individual).float()  # .reshape(1, -1, self.window)
 
         with torch.no_grad():
             output = torch.nn.functional.softmax(self.model(input_)).detach().numpy()
 
         idx = output.argmax()
 
         if full:
@@ -123,15 +131,23 @@
 
         if full:
             return idx, output[0]
         return idx, output[0][idx]
 
     def get_prediction_target_torch(self, individual, full=False, binary=False):
         individual = np.array(individual.tolist(), dtype=np.float64)
-        input_ = torch.from_numpy(individual).float().reshape(1, -1, self.window)
+        if self.mode == "time":
+            individual = individual.reshape(
+                1, individual.shape[-1], individual.shape[-2]
+            )
+        else:
+            individual = individual.reshape(
+                1, individual.shape[-2], individual.shape[-1]
+            )
+        input_ = torch.from_numpy(individual).float()  # .reshape(1, -1, self.window)
         output = torch.nn.functional.softmax(self.model(input_)).detach().numpy()
         idx = output.argmax()
         if full:
             return idx, output[0]
         return idx, output[0][idx]
 
     def get_prediction_target_tensorflow(self, individual, full=False):
```

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py`

 * *Files 1% similar despite different names*

```diff
@@ -112,10 +112,11 @@
             neighborhood,
             window,
             channels,
             self.backend,
             transformer,
             verbose=self.verbose,
             epochs=epochs,
+            mode=self.mode,
         )
         ep, output = e.run()
         return np.array(ep)[0], output
```

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/leftist.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/leftist.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/neighbors.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/neighbors.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/InterpretabilityModels/leftist/transform.py` & `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/Models/PyTorchModel.py` & `TSInterpret-0.2.7/TSInterpret/Models/PyTorchModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/Models/SklearnModel.py` & `TSInterpret-0.2.7/TSInterpret/Models/SklearnModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/Models/TensorflowModel.py` & `TSInterpret-0.2.7/TSInterpret/Models/TensorflowModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret/Models/base_model.py` & `TSInterpret-0.2.7/TSInterpret/Models/base_model.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret.egg-info/PKG-INFO` & `TSInterpret-0.2.7/TSInterpret.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.2.6
+Version: 0.2.7
 Summary: todo
 Home-page: https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries
 Author: Jacqueline Hoellig
 Author-email: hoellig@fzi.de
 License: BSD-3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.6 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.7 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
```

### Comparing `TSInterpret-0.2.6/TSInterpret.egg-info/SOURCES.txt` & `TSInterpret-0.2.7/TSInterpret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/TSInterpret.egg-info/requires.txt` & `TSInterpret-0.2.7/TSInterpret.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.6/setup.py` & `TSInterpret-0.2.7/setup.py`

 * *Files identical despite different names*

