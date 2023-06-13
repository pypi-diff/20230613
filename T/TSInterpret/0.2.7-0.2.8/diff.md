# Comparing `tmp/TSInterpret-0.2.7.tar.gz` & `tmp/TSInterpret-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSInterpret-0.2.7.tar", last modified: Tue Jun 13 07:01:45 2023, max compression
+gzip compressed data, was "TSInterpret-0.2.8.tar", last modified: Tue Jun 13 12:52:26 2023, max compression
```

## Comparing `TSInterpret-0.2.7.tar` & `TSInterpret-0.2.8.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.341606 TSInterpret-0.2.7/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.329606 TSInterpret-0.2.7/ClassificationModels/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/CNN.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/CNN_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/DecisionTree.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/LSTM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/LSTM_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/ClassificationModels/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-13 07:01:45.341606 TSInterpret-0.2.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.329606 TSInterpret-0.2.7/TSInterpret/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.329606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/FeatureAttribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.329606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/GradCam/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/GradCam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/InstanceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.333606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/TSR.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.333606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (123)    22782 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10504 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/CF.py
--rw-r--r--   0 runner    (1001) docker     (123)    11329 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.333606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.333606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.337606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.337606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7228 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/leftist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/neighbors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.337606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.337606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.337606 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.341606 TSInterpret-0.2.7/TSInterpret/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/Models/PyTorchModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/Models/SklearnModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/Models/TensorflowModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/Models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/TSInterpret/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:01:45.329606 TSInterpret-0.2.7/TSInterpret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-13 07:01:45.000000 TSInterpret-0.2.7/TSInterpret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-13 07:01:45.000000 TSInterpret-0.2.7/TSInterpret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:01:45.000000 TSInterpret-0.2.7/TSInterpret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-13 07:01:45.000000 TSInterpret-0.2.7/TSInterpret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 07:01:45.000000 TSInterpret-0.2.7/TSInterpret.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:01:45.341606 TSInterpret-0.2.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-13 07:01:35.000000 TSInterpret-0.2.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.726975 TSInterpret-0.2.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.710975 TSInterpret-0.2.8/ClassificationModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/CNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/CNN_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/DecisionTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/LSTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/LSTM_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-13 12:52:26.726975 TSInterpret-0.2.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.714975 TSInterpret-0.2.8/TSInterpret/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.714975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/FeatureAttribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.714975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/GradCam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/GradCam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/InstanceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.714975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/TSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.722975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/CF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.722975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.722975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.722975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.722975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/leftist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/neighbors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.722975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.722975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.726975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.726975 TSInterpret-0.2.8/TSInterpret/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/Models/PyTorchModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/Models/SklearnModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/Models/TensorflowModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/Models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.714975 TSInterpret-0.2.8/TSInterpret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-13 12:52:26.000000 TSInterpret-0.2.8/TSInterpret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-13 12:52:26.000000 TSInterpret-0.2.8/TSInterpret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:52:26.000000 TSInterpret-0.2.8/TSInterpret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-13 12:52:26.000000 TSInterpret-0.2.8/TSInterpret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 12:52:26.000000 TSInterpret-0.2.8/TSInterpret.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 12:52:26.726975 TSInterpret-0.2.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/setup.py
```

### Comparing `TSInterpret-0.2.7/ClassificationModels/CNN.py` & `TSInterpret-0.2.8/ClassificationModels/CNN.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/ClassificationModels/CNN_T.py` & `TSInterpret-0.2.8/ClassificationModels/CNN_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/ClassificationModels/DecisionTree.py` & `TSInterpret-0.2.8/ClassificationModels/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/ClassificationModels/LSTM.py` & `TSInterpret-0.2.8/ClassificationModels/LSTM.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/ClassificationModels/LSTM_T.py` & `TSInterpret-0.2.8/ClassificationModels/LSTM_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/ClassificationModels/ResNet.py` & `TSInterpret-0.2.8/ClassificationModels/ResNet.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/ClassificationModels/utils.py` & `TSInterpret-0.2.8/ClassificationModels/utils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/LICENSE` & `TSInterpret-0.2.8/LICENSE`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/PKG-INFO` & `TSInterpret-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.2.7
+Version: 0.2.8
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
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.7 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.8 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
```

### Comparing `TSInterpret-0.2.7/README.md` & `TSInterpret-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/FeatureAttribution.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/FeatureAttribution.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/InterpretabilityBase.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/InterpretabilityBase.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/Saliency/TSR.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/TSR.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/Ates.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/Ates.py`

 * *Files 1% similar despite different names*

```diff
@@ -565,15 +565,15 @@
      2021 International Conference on Applied Artificial Intelligence (ICAPAI). IEEE, 2021.
     ----------
     """
 
     def __init__(
         self,
         model,
-        ref,
+        data,
         backend,
         mode,
         method="opt",
         number_distractors=2,
         max_attempts=1000,
         max_iter=1000,
         silent=False,
@@ -587,15 +587,15 @@
             method str : 'opt' if optimized calculation, 'brute' for Brute Force
             number_distractors int: number of distractore to be used
             silent bool: logging.
 
         """
         super().__init__(model, mode)
         self.backend = backend
-        test_x, test_y = ref
+        test_x, test_y = data
         shape = test_x.shape
         if mode == "time":
             # Parse test data into (1, feat, time):
             change = True
             self.ts_length = shape[-2]
             test_x = test_x.reshape(test_x.shape[0], test_x.shape[2], test_x.shape[1])
         elif mode == "feat":
```

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/CF.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/CF.py`

 * *Files 3% similar despite different names*

```diff
@@ -174,33 +174,38 @@
             exp np.array: returned explanation. Shape: `mode = time` -> `(time, feat)` or `mode = time` -> `(feat, time)`
             cf_label int: lebel of returned instance.
             figsize Tuple: Size of Figure (x,y).
             save_fig str: Path to Save the figure.
         """
         if self.mode == "time":
             item = item.reshape(item.shape[-1], item.shape[-2])
+            exp = exp.reshape(item.shape[-1], item.shape[-2])
+        else:
+            item = item.reshape(item.shape[-2], item.shape[-1])
+            exp = exp.reshape(item.shape[-2], item.shape[-1])
+
         # TODO This is new and needs to be testes
         ind = ""
         # print("Item Shape", item.shape[-2])
         if item.shape[-2] > 1:
-
             res = (item != exp).any(-1)
             # print(res)
             ind = np.where(res)
             # print(ind)
             if len(ind[0]) == 0:
                 print("Items are identical")
                 return
             elif len(ind[0]) > 1:
                 self.plot_multi(
                     item, org_label, exp, cf_label, figsize=figsize, save_fig=save_fig
                 )
                 return
             else:
                 item = item[ind]
+                exp = exp[ind]
 
         plt.style.use("classic")
         colors = [
             "#08F7FE",  # teal/cyan
             "#FE53BB",  # pink
             "#F5D300",  # yellow
             "#00ff41",  # matrix green
```

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,38 +30,38 @@
     ----------
     """
 
     def __init__(
         self,
         model,
         shape,
-        reference_set,
+        data,
         backend="PYT",
         mode="feat",
         method="NUN-CF",
         distance_measure="dtw",
         n_neighbors=1,
         max_iter=500,
     ) -> None:
         """
         In this case differentiation between time & feat not necessary as implicitly given by CNN. Only works for CNNs due to the attribution methods.
         Arguments:
             model [torch.nn.Module, Callable, tf.keras.model]: classification model to explain
             shape Tuple: input shape
-            reference_set Tuple: reference set as tuple (x,y)
+            data Tuple: reference set as tuple (x,y)
             backend str: 'PYT' or  'TF'
             mode str: model either 'time' or 'feat'. `time` -> `(-1, time, feature)` or `feat` -> `(-1, feature, time)`
             method str: 'Nun_CF', 'dtw_bary_center' or 'native_guide'.
             distance_measure str: sklearn appreviation for distance of knn.
             n_neighbore int: # neighbors to select from.
             max_iter int : max number of runs
         """
         super().__init__(model, mode)
         self.backend = backend
-        test_x, test_y = reference_set
+        test_x, test_y = data
         test_x = np.array(test_x)  # , dtype=np.float32)
 
         if mode == "time":
             # Parse test data into (1, feat, time):
             self.ts_length = shape[-2]
             test_x = test_x.reshape(test_x.shape[0], test_x.shape[2], test_x.shape[1])
         elif mode == "feat":
```

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/leftist.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/leftist.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,38 +33,38 @@
     [1] Guillemé, Maël, et al. "Agnostic local explanation for time series classification."
     2019 IEEE 31st International Conference on Tools with Artificial Intelligence (ICTAI). IEEE, 2019.
     ----------
     """
 
     def __init__(
         self,
-        model_to_explain,
-        reference_set=None,
+        model,
+        data=None,
         mode="time",
         backend="F",
         transform_name="straight",
         segmentator_name="uniform",
         learning_process_name="Lime",
         nb_interpretable_feature=10,
     ) -> None:
         """Initization.
         Arguments:
            model_to_explain [torch.nn.Module, Callable, tf.keras.model]: classification model to explain.
-           reference_set Tuple: Reference Dataset as Tuple (x,y).
+           data Tuple: Reference Dataset as Tuple (x,y).
            mode str: Name of second dimension: `time` -> `(-1, time, feature)` or `feat` -> `(-1, feature, time)`
            backend str: TF, PYT or SK
            transform_name str: Name of transformer
            learning_process_name str: 'Lime' or 'Shap'
            nb_interpretable_feature int: number of desired features
         """
-        super().__init__(model_to_explain, mode)
+        super().__init__(model, mode)
 
         self.neighbors = None
 
-        self.test_x, _ = reference_set
+        self.test_x, _ = data
         self.backend = backend
         self.mode = mode
         self.change = False
         self.transform_name = transform_name
         self.segmentator_name = segmentator_name
         self.learning_process_name = learning_process_name
         self.nb_interpretable_feature = nb_interpretable_feature
```

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/neighbors.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/neighbors.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/InterpretabilityModels/leftist/transform.py` & `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/Models/PyTorchModel.py` & `TSInterpret-0.2.8/TSInterpret/Models/PyTorchModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/Models/SklearnModel.py` & `TSInterpret-0.2.8/TSInterpret/Models/SklearnModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/Models/TensorflowModel.py` & `TSInterpret-0.2.8/TSInterpret/Models/TensorflowModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret/Models/base_model.py` & `TSInterpret-0.2.8/TSInterpret/Models/base_model.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret.egg-info/PKG-INFO` & `TSInterpret-0.2.8/TSInterpret.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.2.7
+Version: 0.2.8
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
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.7 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.8 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
```

### Comparing `TSInterpret-0.2.7/TSInterpret.egg-info/SOURCES.txt` & `TSInterpret-0.2.8/TSInterpret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/TSInterpret.egg-info/requires.txt` & `TSInterpret-0.2.8/TSInterpret.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.7/setup.py` & `TSInterpret-0.2.8/setup.py`

 * *Files identical despite different names*

