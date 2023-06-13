# Comparing `tmp/TSInterpret-0.2.8.tar.gz` & `tmp/TSInterpret-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TSInterpret-0.2.8.tar", last modified: Tue Jun 13 12:52:26 2023, max compression
+gzip compressed data, was "TSInterpret-0.2.9.tar", last modified: Tue Jun 13 14:47:08 2023, max compression
```

## Comparing `TSInterpret-0.2.8.tar` & `TSInterpret-0.2.9.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.726975 TSInterpret-0.2.8/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.710975 TSInterpret-0.2.8/ClassificationModels/
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/CNN.py
--rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/CNN_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/DecisionTree.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/LSTM.py
--rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/LSTM_T.py
--rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/ResNet.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/ClassificationModels/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-13 12:52:26.726975 TSInterpret-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.714975 TSInterpret-0.2.8/TSInterpret/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.714975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/
--rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/FeatureAttribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.714975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/GradCam/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/GradCam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/InstanceBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.714975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/
--rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
--rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
--rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/TSR.py
--rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.722975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/
--rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
--rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/CF.py
--rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.722975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
--rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
--rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.722975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.722975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/
--rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.722975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
--rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
--rw-r--r--   0 runner    (1001) docker     (123)     7179 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/leftist.py
--rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/neighbors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.722975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.722975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
--rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.726975 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
--rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
--rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
--rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.726975 TSInterpret-0.2.8/TSInterpret/Models/
--rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/Models/PyTorchModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/Models/SklearnModel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/Models/TensorflowModel.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/Models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/Models/base_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/TSInterpret/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:52:26.714975 TSInterpret-0.2.8/TSInterpret.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-13 12:52:26.000000 TSInterpret-0.2.8/TSInterpret.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-13 12:52:26.000000 TSInterpret-0.2.8/TSInterpret.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:52:26.000000 TSInterpret-0.2.8/TSInterpret.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-13 12:52:26.000000 TSInterpret-0.2.8/TSInterpret.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 12:52:26.000000 TSInterpret-0.2.8/TSInterpret.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 12:52:26.726975 TSInterpret-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-13 12:52:09.000000 TSInterpret-0.2.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.229413 TSInterpret-0.2.9/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.221413 TSInterpret-0.2.9/ClassificationModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-13 14:46:55.000000 TSInterpret-0.2.9/ClassificationModels/CNN.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12183 2023-06-13 14:46:55.000000 TSInterpret-0.2.9/ClassificationModels/CNN_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3320 2023-06-13 14:46:55.000000 TSInterpret-0.2.9/ClassificationModels/DecisionTree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-06-13 14:46:55.000000 TSInterpret-0.2.9/ClassificationModels/LSTM.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3334 2023-06-13 14:46:55.000000 TSInterpret-0.2.9/ClassificationModels/LSTM_T.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6886 2023-06-13 14:46:55.000000 TSInterpret-0.2.9/ClassificationModels/ResNet.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:46:55.000000 TSInterpret-0.2.9/ClassificationModels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/ClassificationModels/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-13 14:47:08.229413 TSInterpret-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7038 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.221413 TSInterpret-0.2.9/TSInterpret/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.221413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/
+-rw-r--r--   0 runner    (1001) docker     (123)     5893 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/FeatureAttribution.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.221413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/GradCam/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/GradCam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/InstanceBase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/InterpretabilityBase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.221413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/
+-rw-r--r--   0 runner    (1001) docker     (123)    16172 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9389 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/TSR.py
+-rw-r--r--   0 runner    (1001) docker     (123)      155 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.225413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/
+-rw-r--r--   0 runner    (1001) docker     (123)    22784 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/Ates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10737 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/CF.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11302 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.225413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/
+-rw-r--r--   0 runner    (1001) docker     (123)     7746 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11874 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.225413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.225413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/
+-rw-r--r--   0 runner    (1001) docker     (123)    10469 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5575 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.225413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)     4432 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10995 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      838 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7359 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/leftist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2256 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/neighbors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.225413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.229413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1765 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.229413 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/
+-rw-r--r--   0 runner    (1001) docker     (123)      301 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3075 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4556 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1913 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1633 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3841 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py
+-rw-r--r--   0 runner    (1001) docker     (123)      759 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py
+-rw-r--r--   0 runner    (1001) docker     (123)      983 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.229413 TSInterpret-0.2.9/TSInterpret/Models/
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/Models/PyTorchModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      907 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/Models/SklearnModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/Models/TensorflowModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/Models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/Models/base_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/TSInterpret/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:47:08.221413 TSInterpret-0.2.9/TSInterpret.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7909 2023-06-13 14:47:08.000000 TSInterpret-0.2.9/TSInterpret.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3981 2023-06-13 14:47:08.000000 TSInterpret-0.2.9/TSInterpret.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:47:08.000000 TSInterpret-0.2.9/TSInterpret.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-13 14:47:08.000000 TSInterpret-0.2.9/TSInterpret.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 14:47:08.000000 TSInterpret-0.2.9/TSInterpret.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:47:08.229413 TSInterpret-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3894 2023-06-13 14:46:56.000000 TSInterpret-0.2.9/setup.py
```

### Comparing `TSInterpret-0.2.8/ClassificationModels/CNN.py` & `TSInterpret-0.2.9/ClassificationModels/CNN.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/ClassificationModels/CNN_T.py` & `TSInterpret-0.2.9/ClassificationModels/CNN_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/ClassificationModels/DecisionTree.py` & `TSInterpret-0.2.9/ClassificationModels/DecisionTree.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/ClassificationModels/LSTM.py` & `TSInterpret-0.2.9/ClassificationModels/LSTM.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/ClassificationModels/LSTM_T.py` & `TSInterpret-0.2.9/ClassificationModels/LSTM_T.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/ClassificationModels/ResNet.py` & `TSInterpret-0.2.9/ClassificationModels/ResNet.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/ClassificationModels/utils.py` & `TSInterpret-0.2.9/ClassificationModels/utils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/LICENSE` & `TSInterpret-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/PKG-INFO` & `TSInterpret-0.2.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.2.8
+Version: 0.2.9
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
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.8 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.9 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
```

### Comparing `TSInterpret-0.2.8/README.md` & `TSInterpret-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/FeatureAttribution.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/FeatureAttribution.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/GradCam/GradCam_1D.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/InterpretabilityBase.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/InterpretabilityBase.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_PTY.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/SaliencyMethods_TF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/Saliency_Base.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/Saliency/TSR.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/Saliency/TSR.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/Ates.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/Ates.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/CF.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/CF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/NativeGuideCF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Evo.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/EvoUtils.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvo/Problem.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/counterfactual/TSEvoCF.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/LIME_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/SHAP_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/LIME_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/SHAP_neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/neighbors_generator/neighbors_generator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/learning_process/utils_learning_process.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/leftist.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/leftist.py`

 * *Files 6% similar despite different names*

```diff
@@ -41,37 +41,42 @@
         data=None,
         mode="time",
         backend="F",
         transform_name="straight",
         segmentator_name="uniform",
         learning_process_name="Lime",
         nb_interpretable_feature=10,
+        nb_neighbors=1000,
+        explanation_size=1,
     ) -> None:
         """Initization.
         Arguments:
            model_to_explain [torch.nn.Module, Callable, tf.keras.model]: classification model to explain.
            data Tuple: Reference Dataset as Tuple (x,y).
            mode str: Name of second dimension: `time` -> `(-1, time, feature)` or `feat` -> `(-1, feature, time)`
            backend str: TF, PYT or SK
            transform_name str: Name of transformer
            learning_process_name str: 'Lime' or 'Shap'
            nb_interpretable_feature int: number of desired features
+            nb_neighbors int: number of neighbors to generate.
+            explanation_size int: number of feature to use for the explanations
         """
         super().__init__(model, mode)
 
         self.neighbors = None
-
+        self.nb_neighbors = nb_neighbors
         self.test_x, _ = data
         self.backend = backend
         self.mode = mode
         self.change = False
         self.transform_name = transform_name
         self.segmentator_name = segmentator_name
         self.learning_process_name = learning_process_name
         self.nb_interpretable_feature = nb_interpretable_feature
+        self.explanation_size = explanation_size
         if mode == "feat":
             self.change = True
             self.test_x = self.test_x.reshape(
                 -1, self.test_x.shape[-1], self.test_x.shape[-2]
             )
 
         if backend == "PYT":
@@ -87,33 +92,30 @@
             # Assumption this is already a predict Function
             print("The Predict Function was given directly")
             self.predict = self.model
 
     def explain(
         self,
         instance,
-        nb_neighbors,
         idx_label=None,
-        explanation_size=None,
         random_state=0,
     ):
         """
         Compute the explanation.
 
         Arguments:
             instance np.array: item to be explained. Shape : `mode = time` -> `(1,time, feat)` or `mode = time` -> `(1,feat, time)`
-            nb_neighbors int: number of neighbors to generate.
             idx_label int: index of label to explain. If None, return an explanation for each label.
-            explanation_size int: number of feature to use for the explanations
             random_state int: fixes seed
 
         Returns:
             List: Attribution weight `mode = time` -> `(explanation_size,time, feat)` or `mode = time` -> `(explanation_size,feat, time)`
         """
-
+        nb_neighbors = self.nb_neighbors
+        explanation_size = self.explanation_size
         if self.segmentator_name == "uniform":
             self.segmentator = UniformSegmentator(self.nb_interpretable_feature)
 
         if self.mode == "feat":
             instance = instance.reshape(instance.shape[-1], instance.shape[-2])
         if self.transform_name == "mean":
             self.transform = MeanTransform(instance)
```

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/neighbors.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/neighbors.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/provided_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/segmentator/uniform_segmentator.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/all_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/mean_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_background_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/rand_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/transform_function/straightline_transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/timeseries/utils_timeseries.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/InterpretabilityModels/leftist/transform.py` & `TSInterpret-0.2.9/TSInterpret/InterpretabilityModels/leftist/transform.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/Models/PyTorchModel.py` & `TSInterpret-0.2.9/TSInterpret/Models/PyTorchModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/Models/SklearnModel.py` & `TSInterpret-0.2.9/TSInterpret/Models/SklearnModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/Models/TensorflowModel.py` & `TSInterpret-0.2.9/TSInterpret/Models/TensorflowModel.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret/Models/base_model.py` & `TSInterpret-0.2.9/TSInterpret/Models/base_model.py`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret.egg-info/PKG-INFO` & `TSInterpret-0.2.9/TSInterpret.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TSInterpret
-Version: 0.2.8
+Version: 0.2.9
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
-Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.8 Summary: todo Home-page:
+Metadata-Version: 2.1 Name: TSInterpret Version: 0.2.9 Summary: todo Home-page:
 https://ipe-wim-gitlab.fzi.de/hoellig/interpretabilitytimeseries Author:
 Jacqueline Hoellig Author-email: hoellig@fzi.de License: BSD-3 Classifier:
 License :: OSI Approved :: BSD License Classifier: Programming Language ::
 Python Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.7 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python ::
```

### Comparing `TSInterpret-0.2.8/TSInterpret.egg-info/SOURCES.txt` & `TSInterpret-0.2.9/TSInterpret.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/TSInterpret.egg-info/requires.txt` & `TSInterpret-0.2.9/TSInterpret.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `TSInterpret-0.2.8/setup.py` & `TSInterpret-0.2.9/setup.py`

 * *Files identical despite different names*

