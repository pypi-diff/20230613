# Comparing `tmp/DomiKnowS-0.536.dev0.tar.gz` & `tmp/DomiKnowS-0.537.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DomiKnowS-0.536.dev0.tar", last modified: Thu Jun  8 16:05:27 2023, max compression
+gzip compressed data, was "DomiKnowS-0.537.dev0.tar", last modified: Tue Jun 13 14:22:46 2023, max compression
```

## Comparing `DomiKnowS-0.536.dev0.tar` & `DomiKnowS-0.537.dev0.tar`

### file list

```diff
@@ -1,114 +1,114 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.272679 DomiKnowS-0.536.dev0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.260679 DomiKnowS-0.536.dev0/DomiKnowS.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-08 16:05:27.000000 DomiKnowS-0.536.dev0/DomiKnowS.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-08 16:05:27.000000 DomiKnowS-0.536.dev0/DomiKnowS.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-08 16:05:27.000000 DomiKnowS-0.536.dev0/DomiKnowS.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-08 16:05:27.000000 DomiKnowS-0.536.dev0/DomiKnowS.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-08 16:05:27.000000 DomiKnowS-0.536.dev0/DomiKnowS.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-08 16:05:27.272679 DomiKnowS-0.536.dev0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.264679 DomiKnowS-0.536.dev0/domiknows/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14139 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.264679 DomiKnowS-0.536.dev0/domiknows/compiler/
--rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/compiler/OntologyMLGraph.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/compiler/compiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.264679 DomiKnowS-0.536.dev0/domiknows/data/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.264679 DomiKnowS-0.536.dev0/domiknows/data/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/data/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/data/allennlp/reader.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/data/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.264679 DomiKnowS-0.536.dev0/domiknows/graph/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.264679 DomiKnowS-0.536.dev0/domiknows/graph/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/allennlp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/allennlp/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/allennlp/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/allennlp/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    14462 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/candidates.py
--rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/concept.py
--rw-r--r--   0 runner    (1001) docker     (123)   110657 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/dataNode.py
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/dataNodeConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    28639 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/logicalConstrain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/property.py
--rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/graph/trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.268679 DomiKnowS-0.536.dev0/domiknows/program/
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/batchprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/callbackprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/loss.py
--rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/lossprogram.py
--rw-r--r--   0 runner    (1001) docker     (123)     9249 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/metric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.268679 DomiKnowS-0.536.dev0/domiknows/program/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/model/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7775 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/model/gbi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1622 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/model/ilpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/model/iml.py
--rw-r--r--   0 runner    (1001) docker     (123)    11952 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/model/lossModel.py
--rw-r--r--   0 runner    (1001) docker     (123)    18964 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/model/pytorch.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/model/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/model_program.py
--rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/program.py
--rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/program/tracker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.268679 DomiKnowS-0.536.dev0/domiknows/sensor/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.268679 DomiKnowS-0.536.dev0/domiknows/sensor/allennlp/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/allennlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/allennlp/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/allennlp/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/allennlp/module.py
--rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/allennlp/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.268679 DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/learnerModels.py
--rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/learners.py
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/query_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/relation_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)    24604 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/sensors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.268679 DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/tokenizers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/tokenizers/spacy.py
--rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/tokenizers/transformers.py
--rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.268679 DomiKnowS-0.536.dev0/domiknows/sensor/torch/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/torch/learner.py
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/sensor/torch/sensor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.272679 DomiKnowS-0.536.dev0/domiknows/solver/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/allennlpInferenceSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/allennlplogInferenceSolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.272679 DomiKnowS-0.536.dev0/domiknows/solver/constructor/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/constructor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/constructor/constructor.py
--rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/dummyILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/gekkoILPBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)    38888 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/gekkoILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)    38785 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/gurobiILPBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)   103195 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/gurobiILPOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/ilpBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/ilpBooleanMethodsCalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/ilpConfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/ilpOntSolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/ilpOntSolverFactory.py
--rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/lcLossBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/lcLossSampleBooleanMethods.py
--rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/mini_solver_debug.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:27.272679 DomiKnowS-0.536.dev0/domiknows/solver/session/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/session/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/session/gurobi_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/session/solver_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/solver/solver.py
--rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/domiknows/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-08 16:05:27.272679 DomiKnowS-0.536.dev0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-08 16:05:15.000000 DomiKnowS-0.536.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.572652 DomiKnowS-0.537.dev0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.564653 DomiKnowS-0.537.dev0/DomiKnowS.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-13 14:22:46.000000 DomiKnowS-0.537.dev0/DomiKnowS.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3174 2023-06-13 14:22:46.000000 DomiKnowS-0.537.dev0/DomiKnowS.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:22:46.000000 DomiKnowS-0.537.dev0/DomiKnowS.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 14:22:46.000000 DomiKnowS-0.537.dev0/DomiKnowS.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 14:22:46.000000 DomiKnowS-0.537.dev0/DomiKnowS.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1327 2023-06-13 14:22:46.572652 DomiKnowS-0.537.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3740 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.564653 DomiKnowS-0.537.dev0/domiknows/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14139 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.564653 DomiKnowS-0.537.dev0/domiknows/compiler/
+-rw-r--r--   0 runner    (1001) docker     (123)     7701 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/compiler/OntologyMLGraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/compiler/compiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.564653 DomiKnowS-0.537.dev0/domiknows/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.564653 DomiKnowS-0.537.dev0/domiknows/data/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/data/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6617 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/data/allennlp/reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/data/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.568652 DomiKnowS-0.537.dev0/domiknows/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.568652 DomiKnowS-0.537.dev0/domiknows/graph/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18149 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/allennlp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11710 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/allennlp/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12506 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/allennlp/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19624 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/allennlp/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2446 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14462 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/candidates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12858 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/concept.py
+-rw-r--r--   0 runner    (1001) docker     (123)   112408 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/dataNode.py
+-rw-r--r--   0 runner    (1001) docker     (123)      305 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/dataNodeConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5133 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28639 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/logicalConstrain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2172 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/property.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4913 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/graph/trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.568652 DomiKnowS-0.537.dev0/domiknows/program/
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/batchprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/callbackprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14005 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/lossprogram.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9205 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/metric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.568652 DomiKnowS-0.537.dev0/domiknows/program/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/model/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7695 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/model/gbi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1580 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/model/ilpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1593 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/model/iml.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11860 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/model/lossModel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18834 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/model/pytorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/model/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/model_program.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14008 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/program.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2257 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/program/tracker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.568652 DomiKnowS-0.537.dev0/domiknows/sensor/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.568652 DomiKnowS-0.537.dev0/domiknows/sensor/allennlp/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/allennlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4857 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/allennlp/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7471 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/allennlp/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16060 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/allennlp/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/allennlp/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.568652 DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1784 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/learnerModels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4778 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/learners.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/query_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5723 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/relation_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24604 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/sensors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.568652 DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/tokenizers/spacy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      829 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/tokenizers/transformers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.568652 DomiKnowS-0.537.dev0/domiknows/sensor/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/torch/learner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/sensor/torch/sensor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.572652 DomiKnowS-0.537.dev0/domiknows/solver/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6595 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/allennlpInferenceSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6390 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/allennlplogInferenceSolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.572652 DomiKnowS-0.537.dev0/domiknows/solver/constructor/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/constructor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8745 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/constructor/constructor.py
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/dummyILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12465 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/gekkoILPBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38888 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/gekkoILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38785 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/gurobiILPBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)   100192 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/gurobiILPOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5219 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/ilpBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5834 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/ilpBooleanMethodsCalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/ilpConfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5721 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/ilpOntSolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5129 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/ilpOntSolverFactory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16520 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/lcLossBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7343 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/lcLossSampleBooleanMethods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4193 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/mini_solver_debug.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:46.572652 DomiKnowS-0.537.dev0/domiknows/solver/session/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/session/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1716 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/session/gurobi_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/session/solver_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/solver/solver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14524 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/domiknows/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 14:22:46.572652 DomiKnowS-0.537.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-06-13 14:22:34.000000 DomiKnowS-0.537.dev0/setup.py
```

### Comparing `DomiKnowS-0.536.dev0/DomiKnowS.egg-info/PKG-INFO` & `DomiKnowS-0.537.dev0/DomiKnowS.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DomiKnowS
-Version: 0.536.dev0
+Version: 0.537.dev0
 Summary: A library provides integration between Domain Knowledge and Deep Learning.
 Home-page: https://github.com/HLR/DomiKnowS
 Author: Andrzej Uszok
 Author-email: auszok@ihmc.org
 License: MIT
 Description: The library allows to specify a problem domain with a conceptual [graph](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#graph) including declarations of edges and nodes, as well as [logical constraints](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#constraints) on the graph concepts and relations. [Neural network](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/MODEL.md#model-declaration) outputs bounded to the graph edges and nodes. The logical constraints are converted to ILP and Gurobi Solver is used for inferring. This adds a relational overlay over elements in a network that relates physical concepts in applications. <br> <br> The example running in Google CoLab environment, presenting the usage of the library is [here](https://colab.research.google.com/drive/1FvdePHv3h3NDSTkBw1VKwAmaZFWuGgTi).
 Platform: UNKNOWN
```

### Comparing `DomiKnowS-0.536.dev0/DomiKnowS.egg-info/SOURCES.txt` & `DomiKnowS-0.537.dev0/DomiKnowS.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/PKG-INFO` & `DomiKnowS-0.537.dev0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DomiKnowS
-Version: 0.536.dev0
+Version: 0.537.dev0
 Summary: A library provides integration between Domain Knowledge and Deep Learning.
 Home-page: https://github.com/HLR/DomiKnowS
 Author: Andrzej Uszok
 Author-email: auszok@ihmc.org
 License: MIT
 Description: The library allows to specify a problem domain with a conceptual [graph](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#graph) including declarations of edges and nodes, as well as [logical constraints](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/KNOWLEDGE.md#constraints) on the graph concepts and relations. [Neural network](https://github.com/HLR/DomiKnowS/blob/main/docs/developer/MODEL.md#model-declaration) outputs bounded to the graph edges and nodes. The logical constraints are converted to ILP and Gurobi Solver is used for inferring. This adds a relational overlay over elements in a network that relates physical concepts in applications. <br> <br> The example running in Google CoLab environment, presenting the usage of the library is [here](https://colab.research.google.com/drive/1FvdePHv3h3NDSTkBw1VKwAmaZFWuGgTi).
 Platform: UNKNOWN
```

### Comparing `DomiKnowS-0.536.dev0/README.md` & `DomiKnowS-0.537.dev0/README.md`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/base.py` & `DomiKnowS-0.537.dev0/domiknows/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/compiler/OntologyMLGraph.py` & `DomiKnowS-0.537.dev0/domiknows/compiler/OntologyMLGraph.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/data/allennlp/reader.py` & `DomiKnowS-0.537.dev0/domiknows/data/allennlp/reader.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/data/reader.py` & `DomiKnowS-0.537.dev0/domiknows/data/reader.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/graph/__init__.py` & `DomiKnowS-0.537.dev0/domiknows/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/graph/allennlp/base.py` & `DomiKnowS-0.537.dev0/domiknows/graph/allennlp/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/graph/allennlp/metrics.py` & `DomiKnowS-0.537.dev0/domiknows/graph/allennlp/metrics.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/graph/allennlp/model.py` & `DomiKnowS-0.537.dev0/domiknows/graph/allennlp/model.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/graph/allennlp/utils.py` & `DomiKnowS-0.537.dev0/domiknows/graph/allennlp/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/graph/base.py` & `DomiKnowS-0.537.dev0/domiknows/graph/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/graph/candidates.py` & `DomiKnowS-0.537.dev0/domiknows/graph/candidates.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/graph/concept.py` & `DomiKnowS-0.537.dev0/domiknows/graph/concept.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/graph/dataNode.py` & `DomiKnowS-0.537.dev0/domiknows/graph/dataNode.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,45 +56,46 @@
 _DataNode__Logger.setLevel(logLevel)
 # Add ch to logger
 _DataNode__Logger.addHandler(ch)
 # Don't propagate
 _DataNode__Logger.propagate = False
         
 # --- Create loggers
-_DataNodeBulder__Logger  = logging.getLogger("dataNodeBuilder")
-_DataNodeBulder__Logger.setLevel(logLevel)
+_DataNodeBuilder__Logger  = logging.getLogger("dataNodeBuilder")
+_DataNodeBuilder__Logger.setLevel(logLevel)
 # Add ch to logger
-_DataNodeBulder__Logger.addHandler(ch)
+_DataNodeBuilder__Logger.addHandler(ch)
 # Don't propagate
-_DataNodeBulder__Logger.propagate = False
+_DataNodeBuilder__Logger.propagate = False
 
-_DataNodeBulder__Logger.info('--- Starting new run ---')
+_DataNodeBuilder__Logger.info('--- Starting new run ---')
 
 # Class representing single data instance with relation links to other data nodes
 class DataNode:
     def __init__(self, instanceID = None, instanceValue = None, ontologyNode = None, relationLinks = {}, attributes = {}):
 
         self.instanceID = instanceID                     # The data instance id (e.g. paragraph number, sentence number, phrase  number, image number, etc.)
         self.instanceValue = instanceValue               # Optional value of the instance (e.g. paragraph text, sentence text, phrase text, image bitmap, etc.)
         self.ontologyNode = ontologyNode                 # Reference to the node in the ontology graph (e.g. Concept) which is the type of this instance (e.g. paragraph, sentence, phrase, etc.)
         
         self.graph =  self.ontologyNode.sup
         if relationLinks:
-            self.relationLinks = relationLinks           # Dictionary mapping relation name to RealtionLinks
+            self.relationLinks = relationLinks           # Dictionary mapping relation name to RelationLinks
         else:
             self.relationLinks = {}
             
         self.impactLinks = {}                            # Dictionary with dataNodes impacting this dataNode by having it as a subject of its relation
         
         if attributes:
             self.attributes = attributes                 # Dictionary with node's attributes
         else:
             self.attributes = {}
             
         self.current_device = 'auto'
+        self.gurobiModel = None
         
         self.myLoggerTime = getRegrTimer_logger()
                      
     class DataNodeError(Exception):
         pass
     
     def __str__(self):
@@ -230,23 +231,23 @@
         for _, kConcept in enumerate(keys):
             if key != "":
                 key = key + "/"
                 keyBis = keyBis + "/"
                 
             # Handle different way of representing concept in the key list
             if isinstance(kConcept, str): # Concept name
-                cocneptForK = None
+                conceptForK = None
                 if not conceptFound:
-                    cocneptForK = self.findConcept(kConcept) # Find concept
+                    conceptForK = self.findConcept(kConcept) # Find concept
                 
-                if not conceptFound and cocneptForK is not None:  
+                if not conceptFound and conceptForK is not None:  
                     conceptFound = True
-                    if isinstance(cocneptForK, tuple):
-                        key = key + '<' + cocneptForK[0].name +'>'
-                        index = cocneptForK[2]
+                    if isinstance(conceptForK, tuple):
+                        key = key + '<' + conceptForK[0].name +'>'
+                        index = conceptForK[2]
                         keyBis = keyBis + kConcept
                     else:
                         key = key + '<' + kConcept +'>'
                         keyBis = keyBis + kConcept
                 else:
                     key = key + kConcept
                     keyBis = keyBis + kConcept
@@ -1024,15 +1025,15 @@
             if not dns:
                 continue
             
             vs = []
             
             for dn in dns:
                 keySoftmax = "<" + c[0].name + ">/local/softmax"
-                normalized_keys = set(["normalizedProb", "meanNormalizedProb", "normalizedProbAll"])
+                normalized_keys = set(["normalizedProb", "meanNormalizedProb", "normalizedProbAll", "meanNormalizedProbStd"])
                 if "softmax" in keys or normalized_keys.intersection(set(keys)):
                     keySoftmax = "<" + c[0].name + ">/local/softmax"
                     if not keySoftmax in dn.attributes: # Already calculated ?                    
                         v = dn.getAttribute(c[0])
                         
                         # check if v is None or not a tensor
                         if v is None or not torch.is_tensor(v):
@@ -1083,43 +1084,59 @@
 
                 if "normalizedProbAll" in keys:
                     keyNormalizedProb = "<" + c[0].name + ">/local/normalizedProbAll"
                     if not keyNormalizedProb in dn.attributes: # Already calculated ?   
                         vSoftmaxT = dn.attributes[keySoftmax]
 
                         # Clamps the softmax probabilities
-                        vector = torch.clamp(vSoftmaxT, min=1e-12, max=1 - 1e-12) 
+                        vector = torch.clamp(vSoftmaxT, min=1e-18, max=1 - 1e-18) 
                         
                         # Calculates their entropy;
                         entropy = torch.distributions.Categorical(torch.log(vector)).entropy() / vector.shape[0]
                         
                         signs = vector - torch.mean(vector)
                         signs[signs < 0] = -1
                         signs[signs >= 0] = +1
                         adjustment = signs * torch.pow(vector - torch.mean(vector), 4)
                         
                         # Multiplies the reverse of entropy to the vector divided by its mean value. P
                         vNormalizedProbT = (1/entropy.item()) * (vector/torch.mean(vector)) + adjustment
                         
                         dn.attributes[keyNormalizedProb] = vNormalizedProbT
+
+                if "meanNormalizedProbStd" in keys:
+                    keyNormalizedProb = "<" + c[0].name + ">/local/meanNormalizedProbStd"
+                    if not keyNormalizedProb in dn.attributes: # Already calculated ?   
+                        vSoftmaxT = dn.attributes[keySoftmax]
+
+                        vector = vSoftmaxT
+
+                        signs = vector - torch.mean(vector)
+                        signs[signs < 0] = -1
+                        signs[signs >= 0] = +1
+                        adjustment = signs * torch.pow(vector - torch.mean(vector), 2)
+                        
+                        # Multiplies the reverse of entropy to the vector divided by its mean value. P
+                        vNormalizedProbT = (adjustment/torch.pow(torch.mean(vector), 2))
+                        
+                        dn.attributes[keyNormalizedProb] = vNormalizedProbT
                 
                 if "argmax" in keys:
                     keyArgmax  = "<" + c[0].name + ">/local/argmax"
                     v = dn.getAttribute(c[0])
                     vArgmax = torch.clone(v)
                     vArgmaxIndex = torch.argmax(v).item()
                     
                     for i, _ in enumerate(v):
                         if i == vArgmaxIndex:
                             vArgmax[i] = 1
                         else:
                             vArgmax[i] = 0
                                     
                     dn.attributes[keyArgmax] = vArgmax
-                    
         
     # Calculate ILP prediction for data graph with this instance as a root based on the provided list of concepts and relations
     def inferILPResults(self, *_conceptsRelations, key = ("local" , "softmax"), fun=None, epsilon = 0.00001, minimizeObjective = False, ignorePinLCs = False):
         if len(_conceptsRelations) == 0:
             _DataNode__Logger.info('Called with empty list of concepts and relations for inference')
         else:
             _DataNode__Logger.info('Called with - %s - list of concepts and relations for inference'%([x.name if isinstance(x, Concept) else x for x in _conceptsRelations]))
@@ -1442,16 +1459,16 @@
     
 # Class constructing the data graph based on the sensors data during the model execution
 class DataNodeBuilder(dict):
     
     context = "build"
     def __init__(self, *args, **kwargs ):
         dict.__init__(self, *args, **kwargs )
-        _DataNodeBulder__Logger.info("")
-        _DataNodeBulder__Logger.info("Called")
+        _DataNodeBuilder__Logger.info("")
+        _DataNodeBuilder__Logger.info("Called")
         self.myLoggerTime = getRegrTimer_logger()
         
         from domiknows.utils import getDnSkeletonMode
         self.skeletonDataNode = getDnSkeletonMode()
         dict.__setitem__(self, "DataNodesConcepts", set())
 
     def __getitem__(self, key):
@@ -1498,27 +1515,27 @@
             
     # Add or increase sensor counter counting number of setitem calls with the given sensor key
     def __addSensorCounters(self, skey, value):
         _value = value
         if isinstance(value, list):
             _value = self.__changToTuple(_value)
             
-        counterNanme = 'Counter'
+        counterName = 'Counter'
         for s in skey: # skey[2:]:
-            counterNanme = counterNanme + '/' + s
+            counterName = counterName + '/' + s
             
-        if not dict.__contains__(self, counterNanme):
+        if not dict.__contains__(self, counterName):
             try:
-                dict.__setitem__(self, counterNanme, {_value : {"counter": 1, "recent" : True}})
+                dict.__setitem__(self, counterName, {_value : {"counter": 1, "recent" : True}})
             except TypeError:
                 return False
             
             return False
         else:
-            currentCounter =  dict.__getitem__(self, counterNanme)
+            currentCounter =  dict.__getitem__(self, counterName)
             
             if _value in currentCounter:
                 currentCounter[_value]["counter"] = currentCounter[_value]["counter"] + 1 
                 
                 if currentCounter[_value]["recent"]:
                     return True
                 else:
@@ -1540,45 +1557,23 @@
                     concept = subGraph.concepts[conceptNameItem]
                     
                     return concept
         return None 
         
     # Collect concept information defined in the graph
     def __findConceptInfo(self, usedGraph, concept):
-        conceptInfo = {}
-        
-        conceptInfo['concept'] = concept
-        
-        conceptInfo['relation'] = False
-        conceptInfo['relationAttrs'] = {}
-        for _, rel in enumerate(concept.has_a()): 
-            conceptInfo['relation'] = True
-            conceptName = rel.dst.name
-                            
-            conceptAttr = self.__findConcept(conceptName, usedGraph)
+        conceptInfo = {
+            'concept': concept,
+            'relation': bool(concept.has_a()),
+            'relationAttrs': {rel.name: self.__findConcept(rel.dst.name, usedGraph) for _, rel in enumerate(concept.has_a())},
+            'root': not ('contains' in concept._in),
+            'contains': [contain.dst for contain in concept._out.get('contains', [])],
+            'containedIn': [contain.src for contain in concept._in.get('contains', [])]
+        }
 
-            conceptInfo['relationAttrs'][rel.name] = conceptAttr
-            
-        conceptInfo['root'] = False
-        # Check if the concept is root concept 
-        if ('contains' not in concept._in):
-            conceptInfo['root'] = True
-          
-        conceptInfo['contains'] = []  
-        # Check if concept contains other concepts
-        if ('contains' in concept._out):
-            for _contain in concept._out['contains']:
-                conceptInfo['contains'].append(_contain.dst)
-                
-        conceptInfo['containedIn'] = []  
-        # Check if concept is contained in other concepts
-        if ('contains' in concept._in):
-            for _contain in concept._in['contains']:
-                conceptInfo['containedIn'].append(_contain.src)
-                           
         return conceptInfo
             
     def __updateConceptInfo(self,  usedGraph, conceptInfo, sensor):
         from domiknows.sensor.pytorch.relation_sensors import EdgeSensor
         conceptInfo["relationAttrData"] = False
         conceptInfo['label'] = False
         if hasattr(sensor, 'label') and sensor.label: 
@@ -1622,74 +1617,88 @@
                         break
                     
             if not isRoot:
                 break
             
         return isRoot
     
+    # Update root dataNodes list
     def __updateRootDataNodeList(self, *dns):
         if not dns:
             return
     
         # Get existing roots dataNodes
         if dict.__contains__(self, 'dataNode'):
             dnsRoots = dict.__getitem__(self, 'dataNode')
-            _DataNodeBulder__Logger.debug('Existing elements in the root dataNodes list - %s'%(dnsRoots))
+            _DataNodeBuilder__Logger.debug('Existing elements in the root dataNodes list - %s'%(dnsRoots))
         else:
             dnsRoots = []
-         
-        newDnsRoots = []
         
         # First flatten the list of new dataNodes
-        flattenDns = [] 
-        if isinstance(dns[0], list): 
-            for dList in dns:
-                flattenDns.extend(dList)
-                
-            if flattenDns and isinstance(flattenDns[0], list): 
-                _flattenDns = []
-                
-                for dList in flattenDns:
-                    _flattenDns.extend(dList)
-                    
-                flattenDns = _flattenDns  
-        else:
-            flattenDns = dns
+        def flatten(dns):
+            for dn in dns:
+                if isinstance(dn, list):
+                    yield from flatten(dn)
+                else:
+                    yield dn
+
+        # Flatten the list of new dataNodes
+        flattenDns = list(flatten(dns))
             
-        for fd in flattenDns:
-            if fd not in dnsRoots:
-                dnsRoots.append(fd)
+        # Create a set of all unique dataNodes in dnsRoots and flattenDns
+        allDns = set(dnsRoots)
+        allDns.update(flattenDns)
+                
+        # -- Update list of existing root dataNotes  
         
-        # Update list of existing root dataNotes     
-        for dnE in dnsRoots:            
-            if not dnE.impactLinks: #  Has not impact link
-                if dnE not in newDnsRoots: # Not yet in the new Root list
-                    newDnsRoots.append(dnE)  
-            else:
-                if self.__isRootDn(dnE, dnsRoots, visitedDns = None):
-                    newDnsRoots.append(dnE)  
+        # Will be used to store new root dataNodes
+        newDnsRoots = []
+        
+        # Loop over all known unique dataNodes
+        #for dnE in allDns:
+        # Check if the dataNode is a root dataNode because it has no impact link
+        # if not dnE.impactLinks: # Has no impact link
+        #     if dnE not in newDnsRoots: # Not yet in the new Root list
+        #         # Add it to the new Root list
+        #         newDnsRoots.append(dnE)
+        # else:
+        #     # Check if the current dataNode is still a root dataNode
+        #     if self.__isRootDn(dnE, dnsRoots, visitedDns = None):
+        #         newDnsRoots.append(dnE)
+        
+        # Count the number of incoming links for each dataNode
+        incomingLinks = {dn: 0 for dn in allDns}
+        for dn in allDns:
+            for il in dn.impactLinks:
+                if il in incomingLinks:
+                    incomingLinks[dn] += 1
+                else:
+                    incomingLinks[dn] = 1
+
+        # Find the root dataNodes which have no incoming links
+        newDnsRoots = [dn for dn in allDns if incomingLinks[dn] == 0 or not dn.impactLinks]
 
         # Set the updated root list 
-        _DataNodeBulder__Logger.info('Updated elements in the root dataNodes list - %s'%(newDnsRoots))
+        _DataNodeBuilder__Logger.info('Updated elements in the root dataNodes list - %s'%(newDnsRoots))
         dict.__setitem__(self, 'dataNode', newDnsRoots) # Updated the dict 
     
         return
     
     # Build or update relation dataNode in the data graph for a given key
     def __buildRelationLink(self, vInfo, conceptInfo, keyDataName):
         relationName = conceptInfo['concept'].name
          
         # Check if data graph started
         existingRootDns = dict.__getitem__(self, 'dataNode') # DataNodes roots
         
         if not existingRootDns:
-            _DataNodeBulder__Logger.error('No dataNode created yet - abandon processing relation link dataNode value for %s and attribute %s'%(relationName,keyDataName))
+            _DataNodeBuilder__Logger.error('No dataNode created yet - abandon processing relation link dataNode value for %s and attribute %s'%(relationName,keyDataName))
             return # No graph yet - information about relation should not be provided yet
         
-        # Find if DatnNodes for this relation have been created
+        # Find if DataNodes for this relation have been created
         existingDnsForRelation = self.findDataNodesInBuilder(select = relationName)
         
         existingDnsForRelationNotSorted = OrderedDict()
         for dn in existingDnsForRelation:
             existingDnsForRelationNotSorted[dn.getInstanceID()] = dn
                 
         existingDnsForRelationSorted = OrderedDict(sorted(existingDnsForRelationNotSorted.items()))
@@ -1703,15 +1712,15 @@
             
             if not dict.__contains__(self, relationAttrsCacheName):
                 dict.__setitem__(self, relationAttrsCacheName, {})
         
             relationAttrsCache =  dict.__getitem__(self, relationAttrsCacheName)
             relationAttrsCache[attrName] = vInfo.value
                 
-            _DataNodeBulder__Logger.info('Caching received data for %s related to relation %s dataNode, found %i existing dataNode of this type - provided value has length %i'
+            _DataNodeBuilder__Logger.info('Caching received data for %s related to relation %s dataNode, found %i existing dataNode of this type - provided value has length %i'
                                          %(keyDataName,relationName,len(existingDnsForRelation),vInfo.len))
             
             # Find if all the needed attribute were initialized
             allAttrInit = True
             for relationAttributeName, _ in conceptInfo['relationAttrsGraph'].items():
                 if relationAttributeName not in relationAttrsCache:
                     allAttrInit = False
@@ -1721,18 +1730,18 @@
                 # Find DataNodes connected by this relation based on graph definition
                 existingDnsForAttr = OrderedDict() # DataNodes for Attributes of the relation
                 for relationAttributeName, relationAttributeConcept in conceptInfo['relationAttrsGraph'].items():
                     _existingDnsForAttr = self.findDataNodesInBuilder(select = relationAttributeConcept.name)
                      
                     if _existingDnsForAttr:
                         existingDnsForAttr[relationAttributeName] = _existingDnsForAttr
-                        _DataNodeBulder__Logger.info('Found %i dataNodes of the attribute %s for concept %s'%(len(_existingDnsForAttr),relationAttributeName,relationAttributeConcept.name))
+                        _DataNodeBuilder__Logger.info('Found %i dataNodes of the attribute %s for concept %s'%(len(_existingDnsForAttr),relationAttributeName,relationAttributeConcept.name))
                     else:
                         existingDnsForAttr[relationAttributeName] = []
-                        _DataNodeBulder__Logger.warning('Not found dataNodes of the attribute %s for concept %s'%(relationAttributeName,relationAttributeConcept.name))
+                        _DataNodeBuilder__Logger.warning('Not found dataNodes of the attribute %s for concept %s'%(relationAttributeName,relationAttributeConcept.name))
                                     
                 attributeNames = [*existingDnsForAttr]
                 
                 # Create links between this relation and instance dataNode based on the candidate information provided by sensor for each relation attribute
                 for relationDnIndex, relationDn in existingDnsForRelationSorted.items():
                     for attributeIndex, attribute in enumerate(attributeNames):
                           
@@ -1747,116 +1756,116 @@
                             
                             if attributeIndex == 0:
                                 candidateDn.addRelationLink(attribute, relationDn)
                             
                             relationDn.addRelationLink(attribute, candidateDn)  
                             relationDn.attributes[keyDataName] = vInfo.value[relationDnIndex] # Add / /Update value of the attribute
                 
-                _DataNodeBulder__Logger.info('Create links between the relation %s and instance dataNode of types'%(conceptInfo['concept'].name))
+                _DataNodeBuilder__Logger.info('Create links between the relation %s and instance dataNode of types'%(conceptInfo['concept'].name))
             else:
                 # Just add the sensor value to relation DataNodes
                 if keyDataName in self:
-                    _DataNodeBulder__Logger.info('Updating attribute %s in relation link dataNodes %s'%(keyDataName,conceptInfo['concept'].name))
+                    _DataNodeBuilder__Logger.info('Updating attribute %s in relation link dataNodes %s'%(keyDataName,conceptInfo['concept'].name))
                 else:
-                    _DataNodeBulder__Logger.info('Adding attribute %s to relation link dataNodes %s'%(keyDataName,conceptInfo['concept'].name))
+                    _DataNodeBuilder__Logger.info('Adding attribute %s to relation link dataNodes %s'%(keyDataName,conceptInfo['concept'].name))
                     
                 for i, rDn in existingDnsForRelationSorted.items(): # Loop through all relation links dataNodes
                     rDn.attributes[keyDataName] = vInfo.value[i] # Add / /Update value of the attribute
 
             self.__updateRootDataNodeList(list(existingDnsForRelationSorted.values()))
         else:    
             # -- DataNode with this relation already created  - update it with new attribute value
             if keyDataName in self:
-                _DataNodeBulder__Logger.info('Updating attribute %s in relation link dataNodes %s'%(keyDataName,conceptInfo['concept'].name))
+                _DataNodeBuilder__Logger.info('Updating attribute %s in relation link dataNodes %s'%(keyDataName,conceptInfo['concept'].name))
             else:
-                _DataNodeBulder__Logger.info('Adding attribute %s to relation link dataNodes %s'%(keyDataName,conceptInfo['concept'].name))
+                _DataNodeBuilder__Logger.info('Adding attribute %s to relation link dataNodes %s'%(keyDataName,conceptInfo['concept'].name))
  
             if len(existingDnsForRelation) != vInfo.len:
-                _DataNodeBulder__Logger.error('Number of relations is %i and is different then the length of the provided tensor %i'%(len(existingDnsForRelation),vInfo.len))
+                _DataNodeBuilder__Logger.error('Number of relations is %i and is different then the length of the provided tensor %i'%(len(existingDnsForRelation),vInfo.len))
                 raise ValueError('Number of relations is %i and is different then the length of the provided tensor %i'%(len(existingDnsForRelation),vInfo.len))
  
             if len(existingDnsForRelationSorted) == 1:
                 if vInfo.dim == 0:
                     existingDnsForRelationSorted[0].attributes[keyDataName] = vInfo.value # Add / /Update value of the attribute
             elif vInfo.dim > 0:
                 for i, rDn in existingDnsForRelationSorted.items(): # Loop through all relations links dataNodes
                     rDn.attributes[keyDataName] = vInfo.value[i] # Add / /Update value of the attribute
             else:
                 pass
 
-    def __createInitialdDataNode(self, vInfo, conceptInfo, keyDataName):
+    def __createInitialDataNode(self, vInfo, conceptInfo, keyDataName):
         conceptName = conceptInfo['concept'].name
 
         dns = []
                    
-        _DataNodeBulder__Logger.info('Creating initial dataNode - provided value has length %i'%(vInfo.len))
+        _DataNodeBuilder__Logger.info('Creating initial dataNode - provided value has length %i'%(vInfo.len))
 
         if vInfo.len == 1: # Will use "READER" key as an id of the root dataNode
             instanceValue = ""
             
             if "READER" in self:
                 instanceID = dict.__getitem__(self, "READER")
             else:
                 instanceID = 0
                 
             _dn = DataNode(instanceID = instanceID, instanceValue = instanceValue, ontologyNode = conceptInfo['concept'])
             
             _dn.attributes[keyDataName] = vInfo.value
             
-            _DataNodeBulder__Logger.info('Created single dataNode with id %s of type %s'%(instanceID,conceptName))
+            _DataNodeBuilder__Logger.info('Created single dataNode with id %s of type %s'%(instanceID,conceptName))
             dns.append(_dn)
         elif vInfo.len > 1:
             for vIndex, v in enumerate(vInfo.value):
                 instanceValue = ""
                 instanceID = vIndex
                 _dn = DataNode(instanceID = instanceID, instanceValue = instanceValue, ontologyNode = conceptInfo['concept'])
                 
                 _dn.attributes[keyDataName] = v
                 
                 dns.append(_dn)
                         
-            _DataNodeBulder__Logger.info('Created %i dataNodes of type %s'%(len(dns),conceptName))
+            _DataNodeBuilder__Logger.info('Created %i dataNodes of type %s'%(len(dns),conceptName))
                     
         self.__updateRootDataNodeList(dns)
         
         return dns
     
     def __createSingleDataNode(self, vInfo, conceptInfo, keyDataName):
         conceptName = conceptInfo['concept'].name
-        _DataNodeBulder__Logger.info('Received information about dataNodes of type %s - value dim is %i and length is %i'%(conceptName,vInfo.dim,vInfo.len))
+        _DataNodeBuilder__Logger.info('Received information about dataNodes of type %s - value dim is %i and length is %i'%(conceptName,vInfo.dim,vInfo.len))
 
         # -- Create a single the new dataNode 
         instanceValue = ""
         instanceID = 0
         _dn = DataNode(instanceID = instanceID, instanceValue = instanceValue, ontologyNode = conceptInfo['concept'])
         _dn.attributes[keyDataName] = vInfo.value
                 
-        _DataNodeBulder__Logger.info('Single new dataNode %s created'%(_dn))
+        _DataNodeBuilder__Logger.info('Single new dataNode %s created'%(_dn))
 
         self.__updateRootDataNodeList(_dn)
                 
         return [_dn]
         
     def __createMultiplyDataNode(self, vInfo, conceptInfo, keyDataName):
         conceptName = conceptInfo['concept'].name
         
         # Master List of lists of created dataNodes - each list in the master list represent set of new dataNodes connected to the same parent dataNode 
         # (identified by the index in the master list)
         dns = [] 
                 
-        _DataNodeBulder__Logger.info('Received information about dataNodes of type %s - value dim is %i and length is %i'%(conceptName,vInfo.dim,vInfo.len))
+        _DataNodeBuilder__Logger.info('Received information about dataNodes of type %s - value dim is %i and length is %i'%(conceptName,vInfo.dim,vInfo.len))
 
         # --- Create dataNodes
         
         # Check the type of sensor data
         if vInfo.dim == 0: 
-            _DataNodeBulder__Logger.warning('Provided value is empty %s - abandon the update'%(vInfo.value))
+            _DataNodeBuilder__Logger.warning('Provided value is empty %s - abandon the update'%(vInfo.value))
             return
         elif vInfo.dim == 1: # List with indexes for new DataNodes and data for attribute
-            _DataNodeBulder__Logger.info('Adding %i new dataNodes of type %s'%(vInfo.len,conceptName))
+            _DataNodeBuilder__Logger.info('Adding %i new dataNodes of type %s'%(vInfo.len,conceptName))
 
             dns1 = []
             for vIndex, v in enumerate(vInfo.value):
                 instanceValue = ""
                 instanceID = vIndex
                 
                 # Create new DataNode
@@ -1872,33 +1881,33 @@
         elif vInfo.dim == 2: # Two dimensional relation information
             if "relationMode" in conceptInfo:
                 relatedDnsType = conceptInfo["relationAttrs"]['src']
                 relatedDns = self.findDataNodesInBuilder(select = relatedDnsType)
                 
                 if len(vInfo.value) > 0:
                     try:
-                        requiredLenOFReltedDns = len(vInfo.value[0])
+                        requiredLenOFRelatedDns = len(vInfo.value[0])
                     except IndexError:
-                        requiredLenOFReltedDns = 0
+                        requiredLenOFRelatedDns = 0
                 else:
-                    requiredLenOFReltedDns = 0
+                    requiredLenOFRelatedDns = 0
                     
-                if requiredLenOFReltedDns != len(relatedDns):
-                    _DataNodeBulder__Logger.warning('Value of %s expects %i related dataNode of type %s but the number of existing dataNodes is %i - abandon the update'
-                                                    %(conceptInfo['relationName'],requiredLenOFReltedDns,relatedDnsType,len(relatedDns)))
+                if requiredLenOFRelatedDns != len(relatedDns):
+                    _DataNodeBuilder__Logger.warning('Value of %s expects %i related dataNode of type %s but the number of existing dataNodes is %i - abandon the update'
+                                                    %(conceptInfo['relationName'],requiredLenOFRelatedDns,relatedDnsType,len(relatedDns)))
                     return
            
-                _DataNodeBulder__Logger.info('Create %i new dataNodes of type %s'%(vInfo.len,conceptName))
+                _DataNodeBuilder__Logger.info('Create %i new dataNodes of type %s'%(vInfo.len,conceptName))
                 
                 if not conceptInfo['relation']:
-                    _DataNodeBulder__Logger.info('It is a contain update of type - %s'%(conceptInfo["relationMode"]))
+                    _DataNodeBuilder__Logger.info('It is a contain update of type - %s'%(conceptInfo["relationMode"]))
                     if conceptInfo["relationMode"] == "forward":
-                        _DataNodeBulder__Logger.info('%s is contain in %s'%(conceptName, relatedDnsType))
+                        _DataNodeBuilder__Logger.info('%s is contain in %s'%(conceptName, relatedDnsType))
                     else:
-                        _DataNodeBulder__Logger.info('%s is contain in %s'%(relatedDnsType, conceptName))
+                        _DataNodeBuilder__Logger.info('%s is contain in %s'%(relatedDnsType, conceptName))
 
                 for i in range(0,vInfo.len):
                     instanceValue = ""
                     instanceID = i
                     _dn = DataNode(instanceID = instanceID, instanceValue = instanceValue, ontologyNode = conceptInfo['concept'])
                         
                     _dn.attributes[keyDataName] = vInfo.value[i]
@@ -1911,23 +1920,23 @@
                                 if isRelated == 1:
                                     relatedDns[index].addChildDataNode(_dn)                            
                         elif conceptInfo["relationMode"] == "backward":
                             for index, isRelated in enumerate(vInfo.value[i]):
                                 if isRelated == 1:
                                     _dn.addChildDataNode(relatedDns[index])  
             else:
-                _DataNodeBulder__Logger.info('Create %i new dataNodes of type %s'%(vInfo.len,conceptName))
+                _DataNodeBuilder__Logger.info('Create %i new dataNodes of type %s'%(vInfo.len,conceptName))
                 for i in range(0,vInfo.len):
                     instanceValue = ""
                     instanceID = i
                     _dn = DataNode(instanceID = instanceID, instanceValue = instanceValue, ontologyNode = conceptInfo['concept'])
                         
                     dns.append(_dn)
         else:
-            _DataNodeBulder__Logger.warning('It is an unsupported sensor input - %s'%(vInfo))
+            _DataNodeBuilder__Logger.warning('It is an unsupported sensor input - %s'%(vInfo))
                 
         self.__updateRootDataNodeList(dns)   
         return dns
             
     def __updateDataNodes(self, vInfo, conceptInfo, keyDataName):
         conceptName = conceptInfo['concept'].name
         existingDnsForConcept = self.findDataNodesInBuilder(select = conceptName) # Try to get DataNodes of the current concept
@@ -1935,20 +1944,20 @@
         if not existingDnsForConcept:
             existingDnsForConcept = self.findDataNodesInBuilder(select = conceptName)
             
         if not existingDnsForConcept:
             return
                                                                     
         if keyDataName in existingDnsForConcept[0].attributes:
-            _DataNodeBulder__Logger.info('Updating attribute %s in existing dataNodes - found %i dataNodes of type %s'%(keyDataName, len(existingDnsForConcept),conceptName))
+            _DataNodeBuilder__Logger.info('Updating attribute %s in existing dataNodes - found %i dataNodes of type %s'%(keyDataName, len(existingDnsForConcept),conceptName))
         else:
-            _DataNodeBulder__Logger.info('Adding attribute %s in existing dataNodes - found %i dataNodes of type %s'%(keyDataName, len(existingDnsForConcept),conceptName))
+            _DataNodeBuilder__Logger.info('Adding attribute %s in existing dataNodes - found %i dataNodes of type %s'%(keyDataName, len(existingDnsForConcept),conceptName))
         
         if len(existingDnsForConcept) > vInfo.len: # Not enough elements in the value 
-            _DataNodeBulder__Logger.warning('Provided value has length %i but found %i existing dataNode - abandon the update'%(vInfo.len,len(existingDnsForConcept)))
+            _DataNodeBuilder__Logger.warning('Provided value has length %i but found %i existing dataNode - abandon the update'%(vInfo.len,len(existingDnsForConcept)))
         elif len(existingDnsForConcept) == vInfo.len: # Number of  value elements matches the number of found dataNodes
             if len(existingDnsForConcept) == 0:
                 return
             elif vInfo.dim == 0:
                 if isinstance(vInfo.value, torch.Tensor):
                     if keyDataName[0] == '<' and keyDataName[-1] == '>':
                         existingDnsForConcept[0].attributes[keyDataName] = [1-vInfo.value.item(), vInfo.value.item()]
@@ -1957,47 +1966,47 @@
                 else:
                     existingDnsForConcept[0].attributes[keyDataName] = [vInfo.value]
             else:
                 for vIndex, v in enumerate(vInfo.value):
                     if isinstance(existingDnsForConcept[vIndex], DataNode): # Check if DataNode
                         existingDnsForConcept[vIndex].attributes[keyDataName] = v
                     else:
-                        _DataNodeBulder__Logger.error('Element %i in the list is not a dataNode - skipping it'%(vIndex))
+                        _DataNodeBuilder__Logger.error('Element %i in the list is not a dataNode - skipping it'%(vIndex))
                         raise ValueError('Element %i in the list is not a dataNode - skipping it'%(vIndex))
         
                 if keyDataName[0] == '<' and keyDataName[-1] == '>':
                     if "contains" in existingDnsForConcept[0].impactLinks:
                         dnParent = existingDnsForConcept[0].impactLinks["contains"][0]
                         dnParent.attributes[keyDataName] = vInfo.value
         elif len(existingDnsForConcept) < vInfo.len: # Too many elements in the value
-            _DataNodeBulder__Logger.warning('Provided value has length %i but found %i existing dataNode - abandon the update'%(vInfo.len,len(existingDnsForConcept)))
+            _DataNodeBuilder__Logger.warning('Provided value has length %i but found %i existing dataNode - abandon the update'%(vInfo.len,len(existingDnsForConcept)))
             
         # Check if this is the contain relation update or attribute update
         if "relationMode" in conceptInfo and  not conceptInfo["relation"]:
             relatedDnsType = conceptInfo["relationAttrs"]['src']
 
             relatedDns = self.findDataNodesInBuilder(select = relatedDnsType)
 
             if vInfo.dim:
-                requiredLenOFReltedDns = len(vInfo.value[0])
+                requiredLenOFRelatedDns = len(vInfo.value[0])
             else:
-                requiredLenOFReltedDns = len(vInfo.item())
+                requiredLenOFRelatedDns = len(vInfo.item())
             
-            if requiredLenOFReltedDns != len(relatedDns):
-                _DataNodeBulder__Logger.error('Provided value expected %i related dataNode of type %s but the number of existing dataNodes is %i - abandon the update'
-                                              %(requiredLenOFReltedDns,relatedDnsType,len(relatedDns)))
+            if requiredLenOFRelatedDns != len(relatedDns):
+                _DataNodeBuilder__Logger.error('Provided value expected %i related dataNode of type %s but the number of existing dataNodes is %i - abandon the update'
+                                              %(requiredLenOFRelatedDns,relatedDnsType,len(relatedDns)))
                 raise ValueError('Provided value expected %i related dataNode of type %s but the number of existing dataNodes is %i - abandon the update'
-                                              %(requiredLenOFReltedDns,relatedDnsType,len(relatedDns)))
+                                              %(requiredLenOFRelatedDns,relatedDnsType,len(relatedDns)))
 
                 
-            _DataNodeBulder__Logger.info('It is a contain update of type - %s'%(conceptInfo["relationMode"]))
+            _DataNodeBuilder__Logger.info('It is a contain update of type - %s'%(conceptInfo["relationMode"]))
             if conceptInfo["relationMode"] == "forward":
-                _DataNodeBulder__Logger.info('%s is contain in %s'%(conceptName, relatedDnsType))
+                _DataNodeBuilder__Logger.info('%s is contain in %s'%(conceptName, relatedDnsType))
             else:
-                _DataNodeBulder__Logger.info('%s is contain in %s'%(relatedDnsType, conceptName))
+                _DataNodeBuilder__Logger.info('%s is contain in %s'%(relatedDnsType, conceptName))
                 
             for i in range(0,vInfo.len):
                 _dn = existingDnsForConcept[i]
                     
                 if conceptInfo["relationMode"] == "forward":
                     for index, isRelated in enumerate(vInfo.value[i]):
                         if isRelated == 1:
@@ -2010,15 +2019,15 @@
             self.__updateRootDataNodeList(existingDnsForConcept)   
                       
     # Build or update dataNode in the data graph for a given relationAttributeConcept
     def __buildDataNode(self, vInfo, conceptInfo, keyDataName):
         conceptName = conceptInfo['concept'].name
        
         if not dict.__contains__(self, 'dataNode'):   # ------ No DataNode yet
-            return self.__createInitialdDataNode(vInfo, conceptInfo, keyDataName) # Done - End the method
+            return self.__createInitialDataNode(vInfo, conceptInfo, keyDataName) # Done - End the method
         else:
             # ---------- DataNodes already created
             existingDnsForConcept = self.findDataNodesInBuilder(select = conceptName) # Try to get DataNodes of the current concept
             
             if len(existingDnsForConcept) == 0:# Check if DataNode for this concept already created                    
                 # No DataNode of this concept created yet
     
@@ -2032,38 +2041,38 @@
                 
     def __addEquality(self, vInfo, conceptInfo, equalityConceptName, keyDataName):
         conceptName = conceptInfo['concept'].name
         existingDnsForConcept = self.findDataNodesInBuilder(select = conceptName)
         existingDnsForEqualityConcept = self.findDataNodesInBuilder(select = equalityConceptName)
         
         if not existingDnsForConcept and not existingDnsForEqualityConcept:
-            _DataNodeBulder__Logger.warning('No datNodes created for concept %s and equality concept %s'%(conceptName,equalityConceptName))
+            _DataNodeBuilder__Logger.warning('No datNodes created for concept %s and equality concept %s'%(conceptName,equalityConceptName))
             return
         
         if not existingDnsForConcept:
-            _DataNodeBulder__Logger.warning('No datNodes created for concept %s'%(conceptName))
+            _DataNodeBuilder__Logger.warning('No datNodes created for concept %s'%(conceptName))
             return
         
         if not existingDnsForEqualityConcept:
-            _DataNodeBulder__Logger.warning('No datNodes created for equality concept %s'%(equalityConceptName))
+            _DataNodeBuilder__Logger.warning('No datNodes created for equality concept %s'%(equalityConceptName))
             return
         
-        _DataNodeBulder__Logger.info('Added equality between dataNodes of types %s and %s'%(conceptName,equalityConceptName))
+        _DataNodeBuilder__Logger.info('Added equality between dataNodes of types %s and %s'%(conceptName,equalityConceptName))
 
         for conceptDn in existingDnsForConcept:
             for equalDn in existingDnsForEqualityConcept:
                 
                 if conceptDn.getInstanceID() >= vInfo.value.shape[0]:
                     continue
                 
                 if equalDn.getInstanceID() >= vInfo.value.shape[1]:
                     continue
                 
                 if vInfo.value[conceptDn.getInstanceID(), equalDn.getInstanceID()]:
-                    _DataNodeBulder__Logger.info('DataNodes of %s is equal to %s'%(conceptDn,equalDn))
+                    _DataNodeBuilder__Logger.info('DataNodes of %s is equal to %s'%(conceptDn,equalDn))
                     conceptDn.addEqualTo(equalDn)
 
     # Method processing value of the attribute - determining it it should be treated as a single element. 
     #     It returns a tuple with elements specifying the length of the first dimension of the value, 
     #     the number of dimensions of the value and the original value itself
     def __processAttributeValue(self, value, keyDataName):
         ValueInfo = namedtuple('ValueInfo', ["len", "value", 'dim'])
@@ -2099,120 +2108,118 @@
             if not isinstance(value[0], (torch.Tensor, list)) or (isinstance(value[0], torch.Tensor) and value[0].dim() == 0):
                 return ValueInfo(len = lenV, value = value, dim=1)
             elif not isinstance(value[0][0], (torch.Tensor, list)) or (isinstance(value[0][0], torch.Tensor) and value[0][0].dim() == 0):
                 return ValueInfo(len = lenV, value = value, dim=2)
             elif not isinstance(value[0][0][0], (torch.Tensor, list)) or (isinstance(value[0][0][0], torch.Tensor) and value[0][0][0].dim() == 0):
                 return ValueInfo(len = lenV, value = value, dim=3)
             else:
-                _DataNodeBulder__Logger.warning('Dimension of nested list value for key %s is more then 3 returning dimension 4'%(keyDataName))
+                _DataNodeBuilder__Logger.warning('Dimension of nested list value for key %s is more then 3 returning dimension 4'%(keyDataName))
                 return ValueInfo(len = lenV, value = value, dim=4)
 
         elif isinstance(value, torch.Tensor):
             return ValueInfo(len = lenV, value = value, dim=dimV)
     
     def collectTime(self, start):
         # Collect time used for __setitem__
         end = process_time_ns()
-        currenTime =  end - start
-        if not dict.__contains__(self, "DataNodeTime"):
-            dict.__setitem__(self, "DataNodeTime", [])
-
-        timeList = dict.__getitem__(self, "DataNodeTime")
-        timeList.append(currenTime)
+        currentTime =  end - start
+    
+        timeList = self.setdefault("DataNodeTime", [])
+        timeList.append(currentTime)
         
     # Overloaded __setitem Dictionary method - tracking sensor data and building corresponding data graph
     def __setitem__(self, _key, value):
         from ..sensor import Sensor
 
         start = process_time_ns()
         self.__addSetitemCounter()
         
         if isinstance(_key, (Sensor, Property, Concept)):
             key = _key.fullname
             if  isinstance(_key, Sensor) and not _key.build:
                 if isinstance(value, torch.Tensor):
-                    _DataNodeBulder__Logger.debug('No processing (because build is set to False) - key - %s, key type - %s, value - %s, shape %s'%(key,type(_key),type(value),value.shape))
+                    _DataNodeBuilder__Logger.debug('No processing (because build is set to False) - key - %s, key type - %s, value - %s, shape %s'%(key,type(_key),type(value),value.shape))
                 elif isinstance(value, list):
-                    _DataNodeBulder__Logger.debug('No processing (because build is set to False) - key - %s, key type - %s, value - %s, length %s'%(key,type(_key),type(value),len(value)))
+                    _DataNodeBuilder__Logger.debug('No processing (because build is set to False) - key - %s, key type - %s, value - %s, length %s'%(key,type(_key),type(value),len(value)))
                 else:
-                    _DataNodeBulder__Logger.debug('No processing (because build is set to False) - key - %s, key type - %s, value - %s'%(key,type(_key),type(value)))
+                    _DataNodeBuilder__Logger.debug('No processing (because build is set to False) - key - %s, key type - %s, value - %s'%(key,type(_key),type(value)))
 
                 self.collectTime(start)
                 return dict.__setitem__(self, _key, value)
             
             if  isinstance(_key, Property):
                 if isinstance(value, torch.Tensor):
-                    _DataNodeBulder__Logger.debug('No processing Property as key - key - %s, key type - %s, value - %s, shape %s'%(key,type(_key),type(value),value.shape))
+                    _DataNodeBuilder__Logger.debug('No processing Property as key - key - %s, key type - %s, value - %s, shape %s'%(key,type(_key),type(value),value.shape))
                 elif isinstance(value, list):
-                    _DataNodeBulder__Logger.debug('No processing Property as key - key - %s, key type - %s, value - %s, length %s'%(key,type(_key),type(value),len(value)))
+                    _DataNodeBuilder__Logger.debug('No processing Property as key - key - %s, key type - %s, value - %s, length %s'%(key,type(_key),type(value),len(value)))
                 else:
-                    _DataNodeBulder__Logger.debug('No processing Property as key - key - %s, key type - %s, value - %s'%(key,type(_key),type(value)))
+                    _DataNodeBuilder__Logger.debug('No processing Property as key - key - %s, key type - %s, value - %s'%(key,type(_key),type(value)))
 
                 self.collectTime(start)
                 return dict.__setitem__(self, _key, value)
         elif isinstance(_key, str):
             key = _key
         else:
-            _DataNodeBulder__Logger.error('key - %s, type %s is not supported'%(_key,type(_key)))
+            _DataNodeBuilder__Logger.error('key - %s, type %s is not supported'%(_key,type(_key)))
             self.collectTime(start)
             return
         
         skey = key.split('/')
         
         # Check if the key with this value has been set recently
         # If not create a new sensor for it
         # If yes stop __setitem__ and return - the same value for the key was added last time that key was set
         if not getProductionModeStatus() and self.__addSensorCounters(skey, value):
             self.myLoggerTime.info(f"DataNode Builder skipping repeated value for sensor  - {skey}")
             self.collectTime(start)
             return # Stop __setitem__ for repeated key value combination
         
         if isinstance(value, torch.Tensor):
-            _DataNodeBulder__Logger.info('key - %s, key type - %s, value - %s, shape %s'%(key,type(_key),type(value),value.shape))
+            _DataNodeBuilder__Logger.info('key - %s, key type - %s, value - %s, shape %s'%(key,type(_key),type(value),value.shape))
         elif isinstance(value, list):
-            _DataNodeBulder__Logger.info('key - %s, key type - %s, value - %s, length %s'%(key,type(_key),type(value),len(value)))
+            _DataNodeBuilder__Logger.info('key - %s, key type - %s, value - %s, length %s'%(key,type(_key),type(value),len(value)))
         else:
-            _DataNodeBulder__Logger.info('key - %s, key type - %s, value - %s'%(key,type(_key),type(value)))
+            _DataNodeBuilder__Logger.info('key - %s, key type - %s, value - %s'%(key,type(_key),type(value)))
 
         if value is None:
-            _DataNodeBulder__Logger.error('The value for the key %s is None - abandon the update'%(key))
+            _DataNodeBuilder__Logger.error('The value for the key %s is None - abandon the update'%(key))
             self.collectTime(start)
             return dict.__setitem__(self, _key, value)
                 
         if len(skey) < 2:            
-            _DataNodeBulder__Logger.error('The key %s has only two elements, needs at least three - abandon the update'%(key))
+            _DataNodeBuilder__Logger.error('The key %s has only two elements, needs at least three - abandon the update'%(key))
             self.collectTime(start)
             return dict.__setitem__(self, _key, value)
         
         usedGraph = dict.__getitem__(self, "graph")
 
         # Find if the key include concept from graph
         
         graphPathIndex = usedGraph.cutGraphName(skey)
         keyWithoutGraphName = skey[graphPathIndex:]
         graphPath =  ''.join(map(str, skey[:graphPathIndex])) 
        
         # Check if found concept in the key
         if not keyWithoutGraphName:
-            _DataNodeBulder__Logger.warning('key - %s has not concept part - returning'%(key))
+            _DataNodeBuilder__Logger.warning('key - %s has not concept part - returning'%(key))
             self.collectTime(start)
             return dict.__setitem__(self, _key, value)
             
         # Find description of the concept in the graph
         if isinstance(_key, Sensor):
             try:
                 conceptName = _key.concept.name 
             except TypeError as _:
                 conceptName = keyWithoutGraphName[0]
         else:
             conceptName = keyWithoutGraphName[0]
         concept = self.__findConcept(conceptName, usedGraph)
                 
         if not concept:
-            _DataNodeBulder__Logger.warning('conceptName - %s has not been found in the used graph %s - returning'%(conceptName,usedGraph.fullname))
+            _DataNodeBuilder__Logger.warning('conceptName - %s has not been found in the used graph %s - returning'%(conceptName,usedGraph.fullname))
             self.collectTime(start)
             return dict.__setitem__(self, _key, value)
         
         conceptInfo = self.__findConceptInfo(usedGraph, concept)
         
         if isinstance(_key, Sensor):
             self.__updateConceptInfo(usedGraph, conceptInfo, _key)
@@ -2232,44 +2239,60 @@
             vInfo = self.__processAttributeValue(value, keyDataName)
             
             # Decide if this is equality between concept data, dataNode creation or update for concept or relation link
             if keyDataName.find("_Equality_") > 0:
                 equalityConceptName = keyDataName[keyDataName.find("_Equality_") + len("_Equality_"):]
                 self.__addEquality(vInfo, conceptInfo, equalityConceptName, keyDataName)
             else:                       
-                _DataNodeBulder__Logger.debug('%s found in the graph; it is a concept'%(conceptName))
+                _DataNodeBuilder__Logger.debug('%s found in the graph; it is a concept'%(conceptName))
                 index = self.__buildDataNode(vInfo, conceptInfo, keyDataName)   # Build or update Data node
                 
                 if index:
-                    indexKey = graphPath  + '/' +conceptName + '/index'
+                    indexKey = graphPath  + '/' + conceptName + '/index'
                     dict.__setitem__(self, indexKey, index)
                     from collections.abc import Sequence
                     if self.skeletonDataNode:
-                        if "allDns" not in self:
-                            dict.__setitem__(self, "allDns", set())
-                        allDns = dict.__getitem__(self, "allDns")
+                        allDns = self.setdefault("allDns", set())
+
+                        # Add the index to the "allDns" set
                         try:
                             if isinstance(index[0], Sequence):
                                 index = index[0]
                             allDns.update(index)
                         except TypeError as ty:
                             pass
                 
                 if conceptInfo['relation']:
-                    _DataNodeBulder__Logger.debug('%s is a relation'%(conceptName))
+                    _DataNodeBuilder__Logger.debug('%s is a relation'%(conceptName))
                     self.__buildRelationLink(vInfo, conceptInfo, keyDataName) # Build or update relation link
-        else:
-            keyInRootDataNode = skey[-3] + "/" + skey[-2]
-            if conceptInfo['label']:
-                keyInRootDataNode += "/label"
-            if "<" in keyInRootDataNode:
-                self.__addVariableNameToSet((_key, keyInRootDataNode))
-            else:       
-                self.__addPropertyNameToSet((_key, keyInRootDataNode))
-        
+                    
+        if self.skeletonDataNode:
+            # Join the last third and second elements of the skey list to create the key in the root data node
+            #  keyInRootDataNode = skey[-3] + "/" + skey[-2]
+            # keyInRootDataNode = "/".join(skey[-3:-1])
+            if conceptName in skey:
+                # Find the index of "conceptName" in skey
+                index = skey.index(conceptName)
+
+                # Join "conceptName" with the next element in skey
+                keyInRootDataNode = "/".join(skey[index:index+2])
+           
+                # Add "/label" to the key if the concept has a label
+                if conceptInfo['label']:
+                    keyInRootDataNode += "/label"
+
+                # Check if the key contains "<" and add it to the variable set if it does, otherwise add it to the property set
+                if "<" in keyInRootDataNode:
+                    self.__addVariableNameToSet((_key, keyInRootDataNode))
+                else:
+                    self.__addPropertyNameToSet((_key, keyInRootDataNode))
+            else:
+                # throw an exception
+                raise Exception("The key does not contain conceptName")
+                    
         # Add value to the underling dictionary
         r = dict.__setitem__(self, _key, value)
         
         if not r:
             pass # Error when adding entry to dictionary ?
         
         self.collectTime(start)
@@ -2286,152 +2309,133 @@
         counterName = 'Counter' + 'GetDataNode'
         if not dict.__contains__(self, counterName):
             dict.__setitem__(self, counterName, 1)
         else:
             currentCounter =  dict.__getitem__(self, counterName)
             dict.__setitem__(self, counterName, currentCounter + 1)
             
-    def findDataNodesInBuilder(self, select = None, indexes = None):
+    def findDataNodesInBuilder(self, select=None, indexes=None):
         existingRootDns = dict.__getitem__(self, 'dataNode') # DataNodes roots
-        
+            
         if not existingRootDns:
             foundDns = []
         else:
-            foundDns = existingRootDns[0].findDatanodes(dns = existingRootDns, select = select, indexes = indexes) 
-        
-        return foundDns
-    
-    def needsBatchRootDN(self):
-        if dict.__contains__(self, 'dataNode'):
-            _dataNode = dict.__getitem__(self, 'dataNode')
+            foundDns = existingRootDns[0].findDatanodes(dns=existingRootDns, select=select, indexes=indexes)
             
-            if len(_dataNode) == 1:
-                return False
-            else:
-                typesInDNs = set()
-                for i, d in enumerate(_dataNode):
-                    if i == 0:
-                        continue
-                    
-                    typesInDNs.add(d.getOntologyNode().name)
-                
-                if len(typesInDNs) > 1:
-                    return False
-                
-            return True
-        else:
-            return False 
-    
-    def addBatchRootDN(self):
+        return foundDns
+        
+    def createBatchRootDN(self):
         if dict.__contains__(self, 'dataNode'):
             _dataNode = dict.__getitem__(self, 'dataNode')
-
-            supGraph = None
             if len(_dataNode) == 1:
                 rootDn = _dataNode[0]
-                _DataNodeBulder__Logger.warning('No new Batch Root DataNode created - DataNode Builder has single DataNode with id %s of type %s'
-                                                %(rootDn.instanceID,rootDn.getOntologyNode().name))
-            else:
-                typesInDNs = set()
-                for i, d in enumerate(_dataNode):
-                    if i == 0:
-                        continue
-                    
-                    typesInDNs.add(d.getOntologyNode().name)
-                    supGraph = d.getOntologyNode().sup
+                _DataNodeBuilder__Logger.info(f'No new Batch Root DataNode created - DataNode Builder already has single Root DataNode with id {rootDn.instanceID} of type {rootDn.getOntologyNode().name}')
+                return
                 
-                if len(typesInDNs) > 1:
-                    raise ValueError('Not able to create Batch Root DataNode - DataNode Builder has DataNodes of different types: %s'%(typesInDNs))  
+            # Check if there are more than one type of DataNodes in the builder
+            typesInDNs = set()
+            for i, d in enumerate(_dataNode):
+                if i == 0:
+                    continue
                 
-                if supGraph == None:
-                    raise ValueError('Not able to create Batch Root DataNode - existing DataNodes in the Builder have concept type %s not connected to any graph: %s'%(typesInDNs))  
+                typesInDNs.add(d.getOntologyNode().name)
+            
+            # If there are more than one type of DataNodes in the builder, then it is not possible to create new Batch Root DataNode
+            if len(typesInDNs) > 1:
+                raise ValueError('Not able to create Batch Root DataNode - DataNode Builder has DataNodes of different types: %s'%(typesInDNs))  
+        
+            # Create the Batch Root DataNode
+            supGraph = _dataNode[1].getOntologyNode().sup
+            if supGraph is None:
+                raise ValueError('Not able to create Batch Root DataNode - existing DataNodes in the Builder have concept type %s not connected to any graph: %s'%(typesInDNs))  
 
-                batchRootDNValue = ""
-                batchRootDNID = 0
-                batchRootDNOntologyNode = Concept(name='batch')
-                supGraph.attach(batchRootDNOntologyNode)
-                
-                batchRootDN= DataNode(instanceID = batchRootDNID, instanceValue = batchRootDNValue, ontologyNode = batchRootDNOntologyNode)
+            batchRootDNValue = ""
+            batchRootDNID = 0
+            batchRootDNOntologyNode = Concept(name='batch')
+            supGraph.attach(batchRootDNOntologyNode)
+            
+            batchRootDN = DataNode(instanceID = batchRootDNID, instanceValue = batchRootDNValue, ontologyNode = batchRootDNOntologyNode)
+        
+            for i, d in enumerate(_dataNode):
+                batchRootDN.addChildDataNode(d)  
             
-                for i, d in enumerate(_dataNode):
-                    batchRootDN.addChildDataNode(d)  
-                  
-                dns = []
-                dns.append(batchRootDN)  
-                self.__updateRootDataNodeList(dns)
+            # The new Root DataNode it the batch Root DataNode
+            self.__updateRootDataNodeList([batchRootDN])
 
-                _DataNodeBulder__Logger.info('Created single Batch Root DataNode with id %s of type %s'%(batchRootDNID,batchRootDNOntologyNode))
+            _DataNodeBuilder__Logger.info('Created single Batch Root DataNode with id %s of type %s'%(batchRootDNID,batchRootDNOntologyNode))
+            self.myLoggerTime.info('Created single Batch Root DataNode with id %s of type %s'%(batchRootDNID,batchRootDNOntologyNode))
         else:
-            raise ValueError('DataNode Builder has no DataNode started yet')   
+            raise ValueError('DataNode Builder has no DataNode started yet')
         
     # Method returning constructed DataNode - the fist in the list
     def getDataNode(self, context="interference", device='auto'):
         self.__addGetDataNodeCounter()
         
         if context=="interference":
             if self.skeletonDataNode:
                 self.myLoggerTime.info("DataNode Builder is using skeleton datanode mode")
             if 'Counter' + '_setitem' in self:
                 self.myLoggerTime.info("DataNode Builder the set method called - %i times"%(self['Counter' + '_setitem']))
             if 'DataNodeTime' in self:
                 elapsedInMsDataNodeBuilder = sum(self['DataNodeTime'])/1000000
                 self.myLoggerTime.info(f"DataNode Builder used - {elapsedInMsDataNodeBuilder:.8f}ms")
-        
+                
+        # If DataNode it created then return it
         if dict.__contains__(self, 'dataNode'):
             _dataNode = dict.__getitem__(self, 'dataNode')
             
-            if len(_dataNode) > 0:  
+            if len(_dataNode) != 0:
                 returnDn = _dataNode[0]
                 
                 # Set the torch device
                 returnDn.current_device = device
-                if returnDn.current_device=='auto': # if not set use cpu or cuda if available
+                if returnDn.current_device == 'auto': # if not set use cpu or cuda if available
                     returnDn.current_device = 'cpu'
                     if torch.cuda.is_available():
                         returnDn.current_device = 'cuda'
-                    
-                if len(_dataNode) == 1:
-                    _DataNodeBulder__Logger.info('Returning dataNode with id %s of type %s'%(returnDn.instanceID,returnDn.getOntologyNode().name))
-                else:
-                    typesInDNs = set()
-                    for i, d in enumerate(_dataNode):
-                        if i == 0:
-                            continue
                         
-                        typesInDNs.add(d.getOntologyNode().name)
-                        
-                    _DataNodeBulder__Logger.warning('Returning first dataNode with id %s of type %s - there are total %i dataNodes of types %s'
-                                                    %(returnDn.instanceID,returnDn.getOntologyNode(),len(_dataNode),typesInDNs))
-
+                if len(_dataNode) != 1:
+                    typesInDNs = {d.getOntologyNode().name for d in _dataNode[1:]}
+                    _DataNodeBuilder__Logger.warning(f'Returning first dataNode with id {returnDn.instanceID} of type {returnDn.getOntologyNode().name} - there are total {len(_dataNode)} dataNodes of types {typesInDNs}')
+                    self.myLoggerTime.info(f'Returning first dataNode with id {returnDn.instanceID} of type {returnDn.getOntologyNode().name} - there are total {len(_dataNode)} dataNodes of types {typesInDNs}')
+                else:
+                    _DataNodeBuilder__Logger.info(f'Returning dataNode with id {returnDn.instanceID} of type {returnDn.getOntologyNode().name}')
+                    self.myLoggerTime.info(f'Returning dataNode with id {returnDn.instanceID} of type {returnDn.getOntologyNode().name}')
+                    
                 if self.skeletonDataNode:
-                    variableSetName = 'variableSet'
-                    if dict.__contains__(self, variableSetName):
-                        variableSet = dict.__getitem__(self, variableSetName)
-                        returnDn.attributes[variableSetName] = {}
-                        for _k, k in variableSet:
-                            returnDn.attributes[variableSetName][k] = self[_k]
-                            
-                    propertySetName = 'propertySet'
-                    if dict.__contains__(self, variableSetName):
-                        propertySet = dict.__getitem__(self, propertySetName)
-                        returnDn.attributes[propertySetName] = {}
-                        for _k, k in propertySet:
-                            returnDn.attributes[propertySetName][k] = self[_k]
-                            
-                    allDnsName = 'allDns' 
-                    if dict.__contains__(self, allDnsName):
-                        allDns = dict.__getitem__(self, allDnsName)
-                        for dn in allDns:
-                            if dn == returnDn:
-                                continue
-                            dn.attributes["rootDataNode"] = returnDn
+                    # Get the "variableSet" dictionary from the data node, or create a new empty dictionary if it doesn't exist
+                    variableSet = self.get("variableSet", {})
+
+                    # Create a dictionary of the items in "variableSet" with the keys and values swapped
+                    variableSetDict = {k2: self[k1] for k1, k2 in dict(variableSet).items()}
+                    
+                    # Add the "variableSet" dictionary to the return data node attributes
+                    returnDn.attributes["variableSet"] = variableSetDict
+
+                    # Get the "propertySet" dictionary from the data node, or create a new empty dictionary if it doesn't exist
+                    propertySet = self.get("propertySet", {})
+
+                    # Create a dictionary of the items in "propertySet" 
+                    propertySetDict = {k2: self[k1] for k1, k2 in dict(propertySet).items()}
+
+                    # Add the "propertySet" dictionary to the return data node attributes
+                    returnDn.attributes["propertySet"] = propertySetDict
+
+                    # Get the "allDns" set from the data node, or create a new empty set if it doesn't exist
+                    allDns = self.get("allDns", set())
+
+                    # Iterate over the data nodes in "allDns" and add the "rootDataNode" attribute to them
+                    for dn in allDns:
+                        if dn == returnDn:
+                            continue
+                        dn.attributes["rootDataNode"] = returnDn
         
                 return returnDn
         
-        _DataNodeBulder__Logger.error('Returning None - there are no dataNode')
+        _DataNodeBuilder__Logger.error('Returning None - there are no dataNode')
         return None
     
     # Method returning all constructed DataNodes 
     def getBatchDataNodes(self):
         self.__addGetDataNodeCounter()
         
         if 'Counter' + '_setitem' in self:
@@ -2441,13 +2445,13 @@
             self.myLoggerTime.info(f"DataNode Builder used - {elapsedInMsDataNodeBuilder:.8f}ms")
         
         if dict.__contains__(self, 'dataNode'):
             _dataNode = dict.__getitem__(self, 'dataNode')
             
             if len(_dataNode) > 0:  
                 
-                _DataNodeBulder__Logger.info('Returning %i dataNodes - %s'%(len(_dataNode),_dataNode))
+                _DataNodeBuilder__Logger.info('Returning %i dataNodes - %s'%(len(_dataNode),_dataNode))
 
                 return _dataNode
         
-        _DataNodeBulder__Logger.error('Returning None - there are no dataNodes')
+        _DataNodeBuilder__Logger.error('Returning None - there are no dataNodes')
         return None
```

### Comparing `DomiKnowS-0.536.dev0/domiknows/graph/graph.py` & `DomiKnowS-0.537.dev0/domiknows/graph/graph.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/graph/logicalConstrain.py` & `DomiKnowS-0.537.dev0/domiknows/graph/logicalConstrain.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/graph/property.py` & `DomiKnowS-0.537.dev0/domiknows/graph/property.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/graph/relation.py` & `DomiKnowS-0.537.dev0/domiknows/graph/relation.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/graph/trial.py` & `DomiKnowS-0.537.dev0/domiknows/graph/trial.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/program/batchprogram.py` & `DomiKnowS-0.537.dev0/domiknows/program/batchprogram.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/program/callbackprogram.py` & `DomiKnowS-0.537.dev0/domiknows/program/callbackprogram.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/program/loss.py` & `DomiKnowS-0.537.dev0/domiknows/program/loss.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/program/lossprogram.py` & `DomiKnowS-0.537.dev0/domiknows/program/lossprogram.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/program/metric.py` & `DomiKnowS-0.537.dev0/domiknows/program/metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,15 @@
 
 class DatanodeCMMetric(torch.nn.Module):
     def __init__(self, inferType='ILP'):
         super().__init__()
         self.inferType = inferType
 
     def forward(self, input, target, data_item, prop, weight=None):
-        if (data_item.needsBatchRootDN()):
-            data_item.addBatchRootDN()
+        data_item.createBatchRootDN()
         datanode = data_item.getDataNode(context=self.inferType)
         result = datanode.getInferMetrics(prop.name, inferType=self.inferType)
         if len(result.keys())==2:
             if str(prop.name) in result:
                 val =  result[str(prop.name)]
                 return calc_TP_FP_TN_FN_for_single_class(val)
             else:
```

### Comparing `DomiKnowS-0.536.dev0/domiknows/program/model/gbi.py` & `DomiKnowS-0.537.dev0/domiknows/program/model/gbi.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,16 +104,15 @@
         """
         _, _, *output = model(data_item)
         node = detuple(*output[:1])
         return node, output[1]
     # ----
     
     def forward(self, builder, build=None):
-        if builder.needsBatchRootDN():
-            builder.addBatchRootDN()
+        builder.createBatchRootDN()
         datanode = builder.getDataNode(device=self.device)
 
         datanode.infer()
 
         # Get constraint satisfaction for the current DataNode
         num_satisfied, num_constraints = self.get_constraints_satisfaction(datanode)
 
@@ -187,16 +186,15 @@
             c_opt.step()
         
         return c_loss, datanode, builder # ? float("nan")
  
     def calculateGBISelection(self, builder, conceptsRelations):
         self.forward(builder)
         
-        if builder.needsBatchRootDN():
-            builder.addBatchRootDN()
+        builder.createBatchRootDN()
         datanode = builder.getDataNode(device=self.device)
         
         for c in conceptsRelations:
             cRoot = datanode.findRootConceptOrRelation(c[0])
             dns = datanode.findDatanodes(select = cRoot)
             
             keyArgmax  = "<" + c[0].name + ">/local/argmax"
```

### Comparing `DomiKnowS-0.536.dev0/domiknows/program/model/ilpu.py` & `DomiKnowS-0.537.dev0/domiknows/program/model/ilpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,16 +11,15 @@
         output_sensor, target_sensor = sensors
         logit = output_sensor(data_item)
         # labels = target_sensor(data_item)
         if len(logit) == 0:
             return None
 
         builder = data_item
-        if (builder.needsBatchRootDN()):
-            builder.addBatchRootDN()
+        builder.createBatchRootDN()
         datanode = builder.getDataNode(device=self.device)
         concept = prop.sup
         values = []
         try:
             for cdn in datanode.findDatanodes(select=concept):
                 value = cdn.getAttribute(f'<{prop.name}>/ILP')
                 if isinstance(prop.name, EnumConcept):
```

### Comparing `DomiKnowS-0.536.dev0/domiknows/program/model/iml.py` & `DomiKnowS-0.537.dev0/domiknows/program/model/iml.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,16 +11,15 @@
         output_sensor, target_sensor = sensors
         logit = output_sensor(data_item)
         labels = target_sensor(data_item)
         if len(logit) == 0:
             return None
 
         builder = data_item
-        if (builder.needsBatchRootDN()):
-            builder.addBatchRootDN()
+        builder.createBatchRootDN()
         datanode = builder.getDataNode(device=self.device)
         concept = prop.sup
         values = []
         try:
             for cdn in datanode.findDatanodes(select=concept):
                 value = cdn.getAttribute(f'<{prop.name}>/ILP')
                 if isinstance(prop.name, EnumConcept):
```

### Comparing `DomiKnowS-0.536.dev0/domiknows/program/model/lossModel.py` & `DomiKnowS-0.537.dev0/domiknows/program/model/lossModel.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,16 +64,15 @@
     def forward(self, builder, build=None):
         if build is None:
             build = self.build
             
         if not build and not isinstance(builder, DataNodeBuilder):
             raise ValueError('PrimalDualModel must be invoked with `build` on or with provided DataNode Builder.')
         
-        if (builder.needsBatchRootDN()):
-            builder.addBatchRootDN()
+        builder.createBatchRootDN()
         datanode = builder.getDataNode(device=self.device)
         
         # Call the loss calculation returns a dictionary, keys are matching the constraints
         constr_loss = datanode.calculateLcLoss(tnorm=self.tnorm, sample=self.sample, sampleSize = self.sampleSize)
 
         lmbd_loss = []
         if self.sampleGlobalLoss and constr_loss['globalLoss']:
@@ -158,17 +157,16 @@
         if build is None:
             build = self.build
         self.iter_step += 1
             
         if not build and not isinstance(builder, DataNodeBuilder):
             raise ValueError('PrimalDualModel must be invoked with `build` on or with provided DataNode Builder.')
         
-        if (builder.needsBatchRootDN()):
-            builder.addBatchRootDN()
-        
+        builder.createBatchRootDN()
+
 #       self.loss.reset()
 
         datanode = builder.getDataNode(device=self.device)
         
         # Call the loss calculation returns a dictionary, keys are matching the constraints
         constr_loss = datanode.calculateLcLoss(tnorm=self.tnorm, sample=self.sample, sampleSize = self.sampleSize, sampleGlobalLoss = self.sampleGlobalLoss)
         import math
```

### Comparing `DomiKnowS-0.536.dev0/domiknows/program/model/pytorch.py` & `DomiKnowS-0.537.dev0/domiknows/program/model/pytorch.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,16 +88,15 @@
             sensor.fill_hash(data_hash)
         for sensor in self.graph.get_sensors(ReaderSensor):
             sensor.fill_data(data_item)
         if build:
             data_item.update({"graph": self.graph, 'READER': 0})
             builder = DataNodeBuilder(data_item)
             *out, = self.populate(builder)
-            if (builder.needsBatchRootDN()):
-                builder.addBatchRootDN()
+            builder.createBatchRootDN()
             datanode = builder.getDataNode(context="build", device=self.device)
             return (*out, datanode, builder)
         else:
             *out, = self.populate(data_item)
             return (*out,)
 
     def populate(self):
@@ -237,16 +236,15 @@
 #             for output_sensor, target_sensor in self.find_sensors(prop):
 #             # make sure the sensors are evaluated
 #                 output = output_sensor(builder)
 #                 target = target_sensor(builder)
 #         print("Done with the computation")
 
         # Check if this is batch
-        if (builder.needsBatchRootDN()):
-            builder.addBatchRootDN()
+        builder.createBatchRootDN()
         datanode = builder.getDataNode(device=self.device)
         # trigger inference
 #         fun=lambda val: torch.tensor(val, dtype=float).softmax(dim=-1).detach().cpu().numpy().tolist()
         if datanode:
             for infertype in self.inferTypes:
                 {
                     'ILP': lambda :datanode.inferILPResults(*self.inference_with, key=self.probKey, fun=None, epsilon=None),
@@ -483,16 +481,15 @@
 #             for output_sensor, target_sensor in self.find_sensors(prop):
 #             # make sure the sensors are evaluated
 #                 output = output_sensor(builder)
 #                 target = target_sensor(builder)
 #         print("Done with the computation")
 
         # Check if this is batch
-        if (builder.needsBatchRootDN()):
-            builder.addBatchRootDN()
+        builder.createBatchRootDN()
         datanode = builder.getDataNode(device=self.device)
         # trigger inference
 #         fun=lambda val: torch.tensor(val, dtype=float).softmax(dim=-1).detach().cpu().numpy().tolist()
         for infertype in self.inferTypes:
             {
                 'ILP': lambda :datanode.inferILPResults(*self.inference_with, fun=None, epsilon=None),
                 'local/argmax': lambda :datanode.inferLocal(),
```

### Comparing `DomiKnowS-0.536.dev0/domiknows/program/model/torch.py` & `DomiKnowS-0.537.dev0/domiknows/program/model/torch.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/program/model_program.py` & `DomiKnowS-0.537.dev0/domiknows/program/model_program.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/program/program.py` & `DomiKnowS-0.537.dev0/domiknows/program/program.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/program/tracker.py` & `DomiKnowS-0.537.dev0/domiknows/program/tracker.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/allennlp/base.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/allennlp/base.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/allennlp/learner.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/allennlp/learner.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/allennlp/module.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/allennlp/module.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/allennlp/sensor.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/allennlp/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/learnerModels.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/learnerModels.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/learners.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/learners.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/query_sensor.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/query_sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/relation_sensors.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/relation_sensors.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/sensors.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/sensors.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/tokenizers/spacy.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/tokenizers/spacy.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/tokenizers/transformers.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/tokenizers/transformers.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/pytorch/utils.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/pytorch/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/sensor.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/torch/learner.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/torch/learner.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/sensor/torch/sensor.py` & `DomiKnowS-0.537.dev0/domiknows/sensor/torch/sensor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/allennlpInferenceSolver.py` & `DomiKnowS-0.537.dev0/domiknows/solver/allennlpInferenceSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/allennlplogInferenceSolver.py` & `DomiKnowS-0.537.dev0/domiknows/solver/allennlplogInferenceSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/constructor/constructor.py` & `DomiKnowS-0.537.dev0/domiknows/solver/constructor/constructor.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/dummyILPOntSolver.py` & `DomiKnowS-0.537.dev0/domiknows/solver/dummyILPOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/gekkoILPBooleanMethods.py` & `DomiKnowS-0.537.dev0/domiknows/solver/gekkoILPBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/gekkoILPOntSolver.py` & `DomiKnowS-0.537.dev0/domiknows/solver/gekkoILPOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/gurobiILPBooleanMethods.py` & `DomiKnowS-0.537.dev0/domiknows/solver/gurobiILPBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/gurobiILPOntSolver.py` & `DomiKnowS-0.537.dev0/domiknows/solver/gurobiILPOntSolver.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import math
 from time import process_time, process_time_ns
 from collections import OrderedDict
 import logging
 
 # pytorch
 import torch
 
@@ -19,14 +20,15 @@
 
 from domiknows.graph import LcElement, LogicalConstrain, V, fixedL, ifL, forAllL
 from domiknows.graph import CandidateSelection
 from domiknows.utils import getReuseModel
 
 from domiknows.graph.candidates import getCandidates
 
+
 class gurobiILPOntSolver(ilpOntSolver):
     ilpSolver = 'Gurobi'
 
     def __init__(self, graph, ontologiesTuple, _ilpConfig, reuse_model=False) -> None:
         super().__init__(graph, ontologiesTuple, _ilpConfig)
         self.myIlpBooleanProcessor = gurobiILPBooleanProcessor()
         self.myLcLossBooleanMethods = lcLossBooleanMethods()
@@ -47,239 +49,192 @@
         
     def get_logical_constraints(self, ):
         return self.logical_constraints
     
     def reset_logical_constraints(self, ):
         self.logical_constraints = self.myGraph[0].logicalConstrains ### Can myGraph really be multiple graphs?
         
-    def valueToBeSkipped(self, x):
-        return ( 
-                x != x or  # nan 
-                abs(x) == float('inf')  # inf 
-                ) 
+    def getConcept(self, concept):
+        return concept[0]
+    
+    def getConceptName(self, concept):
+        return concept[0].name
     
+    def conceptIsBinary(self, concept):
+        return concept[2] is None
+    
+    def conceptIsMultiClass(self, concept):
+        return concept[2] is not None
+    
+    # Check if value is NaN or if and has to be skipped
+    def valueToBeSkipped(self, x):
+        return math.isnan(x) or math.isinf(x)
+        
     # Get Ground Truth for provided concept
     def __getLabel(self, dn, conceptRelation, fun=None, epsilon = None):
         value = dn.getAttribute(conceptRelation, 'label')
-        
         return value
         
-    # Get and calculate probability for provided concept
+    # Get and tailor probability for provided concept and instance (represented as dn)
     def getProbability(self, dn, conceptRelation, key = ("local" , "softmax"), fun=None, epsilon = 0.00001):
-        if not dn:
-            valueI = None
+        valueI = dn.getAttribute(conceptRelation, *key) if dn else None
+        labelIndex = conceptRelation[2]
+        
+        if valueI is None:
+            value = None
         else:
-            valueI = dn.getAttribute(conceptRelation, *key)
+            labelIndex = conceptRelation[2]
+            # If value is for multi-class concept, then we need to convert it to binary
+            value = torch.zeros(2, dtype=torch.float) if self.conceptIsMultiClass(conceptRelation) else valueI
+            value[0] = 1 - valueI[labelIndex] if self.conceptIsMultiClass(conceptRelation) else value[0]
+            value[1] = valueI[labelIndex] if self.conceptIsMultiClass(conceptRelation) else value[1]
+            
+        # If softmax process probability through function and apply epsilon
+        if "softmax" in key and value is not None and not math.isnan(value[0]) and epsilon is not None:
+            value[0] = max(epsilon, min(1-epsilon, value[0]))
+            value[1] = max(epsilon, min(1-epsilon, value[1]))
                     
-        if conceptRelation[2] is not None: # This is mutliclass - need to convert it to binary for ILP 
-            value = torch.empty(2, dtype=torch.float)
-            
-            value[0] = 1 - valueI[conceptRelation[2]]
-            value[1] = valueI[conceptRelation[2]]
-        else: # This is binary 
-            value = valueI
-
-        # Process probability through function and apply epsilon
-        if epsilon is not None:
-            if value[0] > 1-epsilon:
-                value[0] = 1-epsilon
-            elif value[1] > 1-epsilon:
-                value[1] = 1-epsilon
-                
-            if value[0] < epsilon:
-                value[0] = epsilon
-            elif value[1] < epsilon:
-                value[1] = epsilon
-               
             # Apply fun on probabilities if defined
             if fun is not None:
                 value = fun(value)
-            
+        
         return value # Return probability
     
+    def createILPVariable(self, m, dn, currentConceptRelation, notV = False):
+        if notV:
+            xkey = '<' + self.getConceptName(currentConceptRelation) + '>/ILP/notx'
+        else:
+            xkey = '<' + self.getConceptName(currentConceptRelation) + '>/ILP/x'  
+
+        # Create a placeholder in Datanode for variable if it does not exist
+        currentConceptLabelLength =  currentConceptRelation[3]
+        dn.attributes.setdefault(xkey, [None] * currentConceptLabelLength)
+        
+        # Check Datanode if ILP variable is already created
+        if self.conceptIsMultiClass(currentConceptRelation):
+            xNew = dn.attributes[xkey][currentConceptRelation[2]]
+        else:
+            xNew =  dn.attributes[xkey][0]
+            
+        # Return ILP variable if it already exists
+        if xNew is not None:
+            return xNew
+            
+        # --- Else create ILP variable
+        currentLabel = currentConceptRelation[1]
+
+        if notV:
+            xVarName = "%s_%s_is_not_%s"%(dn.getOntologyNode(), dn.getInstanceID(), currentLabel)
+        else:
+            xVarName = "%s_%s_is_%s"%(dn.getOntologyNode(), dn.getInstanceID(), currentLabel)
+            
+        xNew = m.addVar(vtype=GRB.BINARY,name=xVarName) 
+
+        # Add ILP Variable to Datanode
+        if self.conceptIsMultiClass(currentConceptRelation):
+            dn.attributes[xkey][currentConceptRelation[2]] = xNew
+        else:
+            dn.attributes[xkey][0] = xNew
+        
+        return xNew
+        
+    def getDatanodesForConcept(self, rootDn, currentName, conceptToDNSCash=None):
+        if conceptToDNSCash is None or currentName is None:
+            conceptToDNSCash = {}
+           
+            if currentName is None:
+                return  # Just reset cash
+            
+        if currentName in conceptToDNSCash:
+            dns = conceptToDNSCash[currentName]
+        else:
+            rootConcept = rootDn.findRootConceptOrRelation(currentName)
+            dns = rootDn.findDatanodes(select=rootConcept)
+            conceptToDNSCash[currentName] = dns
+            
+        return dns
+    
+    # Count number of variables for logical constraints
     def countLCVariables(self, rootDn, *conceptsRelations):
-        # Collect LC variables 
         ilpVarCount = {}
-        conceptToDNSCash = {}
         
         for currentConceptRelation in conceptsRelations: 
-            currentName = currentConceptRelation[0].name
-            
-            if currentName in conceptToDNSCash:
-                dns = conceptToDNSCash[currentName]
-            else:
-                rootConcept = rootDn.findRootConceptOrRelation(currentName)
-                dns = rootDn.findDatanodes(select = rootConcept)
-                conceptToDNSCash[currentName] = dns
+            currentName = self.getConceptName(currentConceptRelation)
+            currentLabel = currentConceptRelation[1]
+
+            dns = self.getDatanodesForConcept(rootDn, currentName)
                 
-            currentConceptName = currentName + "_" + currentConceptRelation[1]
+            currentConceptName = currentName + "_" + currentLabel
             ilpVarCount[currentConceptName] = len(dns)
             
-            if currentConceptRelation[2] is None:
+            if self.conceptIsMultiClass(currentConceptName):
                 ilpVarCount[currentConceptName] += len(dns)
        
         return ilpVarCount
-    
-    def createObjective(self, xDict, rootDn, *conceptsRelations, key = ("local" , "softmax"), fun=None, epsilon = 0.00001):
-        Q = None
-        conceptToDNSCash = {}        
-        
-        x = list(xDict.values())
-        index = 0
-        for currentConceptRelation in conceptsRelations: 
-            currentName = currentConceptRelation[0]
-            
-            if currentName in conceptToDNSCash:
-                dns = conceptToDNSCash[currentName]
-            else:
-                rootConcept = rootDn.findRootConceptOrRelation(currentName)
-                dns = rootDn.findDatanodes(select = rootConcept)
-                conceptToDNSCash[currentName] = dns
-       
-            for dn in dns:
-                if x[index] == None:
-                    continue
-                
-                currentProbability = self.getProbability(dn, currentConceptRelation, key=key, fun=fun, epsilon=epsilon)
-                
-                if currentProbability == None or (torch.is_tensor(currentProbability) and currentProbability.dim() == 0) or len(currentProbability) < 2:
-                    self.myLogger.warning("Probability not provided for variable concept %s in dataNode %s - skipping it"%(currentName,dn.getInstanceID()))
-                    x[index] = None
-                
-                # Check if probability is NaN or if and has to be skipped
-                elif self.valueToBeSkipped(currentProbability[1]):
-                    self.myLogger.info("Probability is %f for concept %s and dataNode %s - skipping it"%(currentProbability[1],currentConceptRelation[1],dn.getInstanceID()))
-                    x[index] = None
-                else:
-                    if Q is None:
-                        Q = currentProbability[1] * x[index]
-                    else:
-                        Q += currentProbability[1] * x[index] 
-                    index += 1   
-                       
-                # Create negative variable for binary concept
-                if currentConceptRelation[2] is None: # ilpOntSolver.__negVarTrashhold:
-                    if x[index-1] == None:
-                        x[index] = None
-                        continue
-                    
-                    # Check if probability is NaN or if and has to be created based on positive value
-                    if self.valueToBeSkipped(currentProbability[0]):
-                        currentProbability[0] = 1 - currentProbability[1]
-                        self.myLogger.info("No ILP negative variable for concept %s and dataNode %s - created based on positive value %f"
-                                           %(dn.getInstanceID(), currentName, currentProbability[1]))
-                        
-                    Q += currentProbability[0] * x[index] 
-                    index += 1  
-           
-        return Q
-    
+  
+    # Create ILP variables for logical constraints and objective
     def createILPVariables(self, m, x, rootDn, *conceptsRelations, key = ("local" , "softmax"), fun=None, epsilon = 0.00001):
         Q = None
+        # Reset the cash for concept to datanodes
+        self.getDatanodesForConcept(rootDn, None)
         
         # Create ILP variables 
         for currentConceptRelation in conceptsRelations: 
-            rootConcept = rootDn.findRootConceptOrRelation(currentConceptRelation[0])
-            dns = rootDn.findDatanodes(select = rootConcept)
-            xkey = '<' + currentConceptRelation[0].name + '>/ILP/x'  
+            currentLabel = currentConceptRelation[1]
+            if self.conceptIsMultiClass(currentConceptRelation):
+                currentLabelIndex = currentConceptRelation[2]
+            else:
+                currentLabelIndex = 0
+            
+            if currentLabel is None:
+                self.myLogger.debug("Concept %s does not have label"%currentConceptRelation)
        
+            # Get datanodes for concept
+            dns = self.getDatanodesForConcept(rootDn, self.getConceptName(currentConceptRelation))
             for dn in dns:
-                # Init x to None
-                if currentConceptRelation[2] is not None:
-                    x[currentConceptRelation[0], currentConceptRelation[1], dn.getInstanceID(), currentConceptRelation[2]] = None
-                else:
-                    x[currentConceptRelation[0], currentConceptRelation[1], dn.getInstanceID(), 0] = None
+                xNew = x.get((self.getConcept(currentConceptRelation), currentLabel, dn.getInstanceID(), currentLabelIndex), None)
+                if xNew is None:
+                    # Create ILP variable
+                    xNew = self.createILPVariable(m, dn, currentConceptRelation)
+                    if self.conceptIsBinary(currentConceptRelation):
+                        xNotNew  = self.createILPVariable(m, dn, currentConceptRelation, notV=True)
+
+                # ---- Prepare ILP variables for constraints and objective for the current run
+                
+                # Create placeholder for variable in the current x set for run
+                x[self.getConcept(currentConceptRelation), currentLabel, dn.getInstanceID(), currentLabelIndex] = None
+                if self.conceptIsBinary(currentConceptRelation):
+                    x[self.getConcept(currentConceptRelation), 'Not_'+  currentLabel, dn.getInstanceID(), currentLabelIndex]  = None
                     
-                if currentConceptRelation[2] is None:
-                    if currentConceptRelation[2] is not None:
-                        x[currentConceptRelation[0], 'Not_'+currentConceptRelation[1], dn.getInstanceID(), currentConceptRelation[2]] = None
-                    else:
-                        x[currentConceptRelation[0], 'Not_'+currentConceptRelation[1], dn.getInstanceID(), 0] = None
-                        
+                # Get probability for variable in the current run
                 currentProbability = self.getProbability(dn, currentConceptRelation, key=key, fun=fun, epsilon=epsilon)
                 
+                # Skip variable for the current run if probability is None
                 if currentProbability == None or (torch.is_tensor(currentProbability) and currentProbability.dim() == 0) or len(currentProbability) < 2:
-                    self.myLogger.warning("Probability not provided for variable concept %s in dataNode %s - skipping it"%(currentConceptRelation[0].name,dn.getInstanceID()))
-                    continue
-                
-                # Check if probability is NaN or if and has to be skipped
-                if self.valueToBeSkipped(currentProbability[1]):
-                    self.myLogger.info("Probability is %f for concept %s and dataNode %s - skipping it"%(currentProbability[1],currentConceptRelation[1],dn.getInstanceID()))
-                    continue
-    
-                xNew = None
-                if currentConceptRelation[2] is not None:
-                    if (currentConceptRelation[0], currentConceptRelation[1], dn.getInstanceID(), currentConceptRelation[2]) in x:
-                        xNew = x[currentConceptRelation[0], currentConceptRelation[1], dn.getInstanceID(), currentConceptRelation[2]]
-                else:
-                    if (currentConceptRelation[0], currentConceptRelation[1], dn.getInstanceID(), 0) in x:
-                        xNew = x[currentConceptRelation[0], currentConceptRelation[1], dn.getInstanceID(), 0]
-                
-                if xkey not in dn.attributes:
-                    dn.attributes[xkey] = [None] * currentConceptRelation[3]
-                        
-                if xNew is None:
-                    # Create variable
-                    xVarName = "%s_%s_is_%s"%(dn.getOntologyNode(), dn.getInstanceID(), currentConceptRelation[1])
-                    xNew = m.addVar(vtype=GRB.BINARY,name=xVarName) 
-                    
-                    if currentConceptRelation[2] is not None:
-                        x[currentConceptRelation[0], currentConceptRelation[1], dn.getInstanceID(), currentConceptRelation[2]] = xNew
-                    else:
-                        x[currentConceptRelation[0], currentConceptRelation[1], dn.getInstanceID(), 0] = xNew
+                    self.myLogger.warning("Probability not provided for variable concept %s in dataNode %s - skipping it"%(self.getConceptName(currentConceptRelation),dn.getInstanceID()))
+                # Skip variable for the current run if probability is NaN or Inf
+                elif self.valueToBeSkipped(currentProbability[1]):
+                    self.myLogger.info("Probability is %f for concept %s and dataNode %s - skipping it"%(currentProbability[1],  currentLabel, dn.getInstanceID()))
+                else:    
+                    # Add variable to the x set for current run
+                    x[self.getConcept(currentConceptRelation),  currentLabel, dn.getInstanceID(), currentLabelIndex] = xNew
+                    if self.conceptIsBinary(currentConceptRelation):
+                        x[self.getConcept(currentConceptRelation), 'Not_' + currentLabel, dn.getInstanceID(), currentLabelIndex] = xNotNew
 
-                if currentConceptRelation[2] is not None:
-                    dn.attributes[xkey][currentConceptRelation[2]] = xNew
-                else:
-                    dn.attributes[xkey][0] = xNew
-                
-                if Q is None:
-                    Q = currentProbability[1] * xNew
-                else:
-                    Q += currentProbability[1] * xNew       
-    
-                # Check if probability is NaN or if and has to be created based on positive value
-                if self.valueToBeSkipped(currentProbability[0]):
-                    currentProbability[0] = 1 - currentProbability[1]
-                    self.myLogger.info("No ILP negative variable for concept %s and dataNode %s - created based on positive value %f"
-                                       %(dn.getInstanceID(), currentConceptRelation[0].name, currentProbability[1]))
-    
-                # Create negative variable for binary concept
-                if currentConceptRelation[2] is None: # ilpOntSolver.__negVarTrashhold:
-                    xNotNew  = None
-                    
-                    if currentConceptRelation[2] is not None:
-                        if (currentConceptRelation[0], 'Not_'+currentConceptRelation[1], dn.getInstanceID(), currentConceptRelation[2]) in x:
-                            xNotNew= x[currentConceptRelation[0], 'Not_'+currentConceptRelation[1], dn.getInstanceID(), currentConceptRelation[2]]
-                    else:
-                        if (currentConceptRelation[0], 'Not_'+currentConceptRelation[1], dn.getInstanceID(), 0) in x:
-                            xNotNew = x[currentConceptRelation[0], 'Not_'+currentConceptRelation[1], dn.getInstanceID(), 0]
-                    
-                    notxkey = '<' + currentConceptRelation[0].name + '>/ILP/notx'
-                
-                    if notxkey not in dn.attributes:
-                        dn.attributes[notxkey] = [None] * currentConceptRelation[3]
-                        
-                    if xNotNew is None:
-                        xNotVarName = "%s_%s_is_not_%s"%(dn.getOntologyNode(), dn.getInstanceID(), currentConceptRelation[1])
-                        xNotNew = m.addVar(vtype=GRB.BINARY,name=xNotVarName)
-                        if currentConceptRelation[2] is not None:
-                            x[currentConceptRelation[0], 'Not_'+currentConceptRelation[1], dn.getInstanceID(), currentConceptRelation[2]] = xNotNew
-                        else:
-                            x[currentConceptRelation[0], 'Not_'+currentConceptRelation[1], dn.getInstanceID(), 0] = xNotNew
-                        
-                    if currentConceptRelation[2] is not None:
-                        dn.attributes[notxkey][currentConceptRelation[2]] = xNotNew
+                    # Add variable to objective
+                    if Q is None:
+                        Q = currentProbability[1] * xNew
                     else:
-                        dn.attributes[notxkey][0] = xNotNew
-                                        
-                    Q += currentProbability[0] * xNotNew    
+                        Q += currentProbability[1] * xNew       
+                            
+                    if self.conceptIsBinary(currentConceptRelation): 
+                        Q += currentProbability[0] * xNotNew    
                 
-            if currentConceptRelation[2] is not None:
-                self.myLogger.debug("No creating ILP negative variables for multiclass concept %s"%( currentConceptRelation[1]))
+            if self.conceptIsMultiClass(currentConceptRelation):
+                self.myLogger.debug("No creating ILP negative variables for multiclass concept %s"%(currentLabel))
 
         m.update()
 
         if len(x):
             self.myLogger.info("Created %i ILP variables"%(len(x)))
         else:
             self.myLogger.warning("No ILP variables created")
@@ -1216,47 +1171,55 @@
             self.myLogger.warning('ILP solver not provided - returning')
             self.myLoggerTime.warning('ILP solver not provided - returning')
             
             return 
         
         self.current_device = dn.current_device
         
-        self.myLogger.info('Calculating ILP Inferencing ')
-        self.myLoggerTime.info('Calculating ILP Inferencing ')
+        self.myLogger.info('Calculating ILP Inference ')
+        self.myLoggerTime.info('Calculating ILP Inference ')
 
         start = process_time() # timer()
 
         gurobiEnv = Env("", empty=True)
         gurobiEnv.setParam('OutputFlag', 0)
         gurobiEnv.start()  
         
+        # Check if existing ILP model can be reuse without recreating ILP constraints
         try:
             # Find count of instance in each concept 
             ilpVarCount = self.countLCVariables(dn, *conceptsRelations)
 
             reusingModel = False
             if self.reuse_model:
-                # Find it there is saved model with this count of instances per concept
+                # Find it there is saved ILP model with this count of instances per concept
                 for modelDec in self.model:
                     if ilpVarCount == modelDec[0]:
                         m = modelDec[1]
                         x = modelDec[2]
                         reusingModel = True
                         break
                     
             if not reusingModel:
                 # If not reusing the model or if the right model was yet saved - create new Gurabi model
-                m = Model("decideOnClassificationResult" + str(start), gurobiEnv)
+                if dn.gurobiModel == None:
+                    m = Model("decideOnClassificationResult" + str(start), gurobiEnv)
+                    dn.gurobiModel = m
+                else:
+                    m = dn.gurobiModel
+                    m.reset()
+                    mConstr = m.getConstrs()
+                    m.remove(mConstr)
+                    m.update()
+                    
                 m.params.outputflag = 0
                 x = OrderedDict()
                 
-                # Create ILP Variables for concepts and objective
-                Q = self.createILPVariables(m, x, dn, *conceptsRelations, key=key, fun=fun, epsilon = epsilon)
-            else:
-                Q = self.createObjective(x, dn, *conceptsRelations, key=key, fun=fun, epsilon = epsilon)
+            # Handle ILP Variables for concepts and objective
+            Q = self.createILPVariables(m, x, dn, *conceptsRelations, key=key, fun=fun, epsilon = epsilon)
             
             endVariableInit = process_time() # timer()
             elapsedVariablesInMs = (endVariableInit - start) *1000
             self.myLoggerTime.info('ILP Variables Init - time: %ims'%(elapsedVariablesInMs))
 
             if not reusingModel:
                 # Add constraints based on ontology and graph definition
@@ -1346,15 +1309,15 @@
                                     continue
                                 
                                 xLen = len(dns[0].attributes[xkey])
                                 dns[0].attributes[xPkey][p] = [None] * xLen
                                 
                             dns[0].attributes[xPkey][p][_x[3]] = mP.getVarByName(x[_x].VarName)
                             
-                            pEnd= process_time() # timer()
+                            pEnd = process_time() # timer()
                             self.myLoggerTime.info('ILP Model init for p %i - time: %ims'%(p, (pEnd - pStart)*1000))
                 else:
                     mP = m
                     xP = x
                     
                     lckey = "/ILP/x"
             
@@ -1562,20 +1525,20 @@
             
         self.myLogger.info('')
 
         end = process_time() # timer()
         elapsedInS = end - start
         
         if elapsedInS > 1:
-            self.myLogger.info('End ILP Inferencing - total time: %fs'%(elapsedInS))
-            self.myLoggerTime.info('End ILP Inferencing - total time: %fs'%(elapsedInS))
+            self.myLogger.info('End ILP Inference - total time: %fs'%(elapsedInS))
+            self.myLoggerTime.info('End ILP Inference - total time: %fs'%(elapsedInS))
         else:
             elapsedInMs = elapsedInS *1000
-            self.myLogger.info('End ILP Inferencing - total time: %ims'%(elapsedInMs))
-            self.myLoggerTime.info('End ILP Inferencing - total time: %ims'%(elapsedInMs))
+            self.myLogger.info('End ILP Inference - total time: %ims'%(elapsedInMs))
+            self.myLoggerTime.info('End ILP Inference - total time: %ims'%(elapsedInMs))
             
         self.myLogger.info('')
         self.myLoggerTime.info('')
         
         # ----------- Return
         return
 
@@ -1668,29 +1631,29 @@
         
         # Collect master concepts with length of multiclass set
         masterConcepts = OrderedDict()
         productConcepts = []
         productSize = 1
         productArgs = []
         for currentConceptRelation in conceptsRelations:
-            currentConceptName = currentConceptRelation[0].name
+            currentConceptName = self.getConceptName(currentConceptRelation)
             
             if currentConceptName not in masterConcepts:
                 masterConcepts[currentConceptName] = OrderedDict()
                 
                 masterConcepts[currentConceptName]['e'] = []
                 masterConcepts[currentConceptName]['e'].append(currentConceptRelation)
                 
                 
                 rootConcept = rootDn.findRootConceptOrRelation(currentConceptName)
                 dns = rootDn.findDatanodes(select = rootConcept)
                 masterConcepts[currentConceptName]["dns"] = dns
                 
                 conceptRange = 2
-                if currentConceptRelation[2] is not None:
+                if self.conceptIsMultiClass(currentConceptRelation):
                     conceptRange = currentConceptRelation[3]
                 masterConcepts[currentConceptName]["range"] = [x for x in range(conceptRange)]
                 
                 masterConcepts[currentConceptName]['xkey'] = '<' + currentConceptName + '>/sample'
                  
                 if self.isConceptFixed(currentConceptName):
                     continue
```

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/ilpBooleanMethods.py` & `DomiKnowS-0.537.dev0/domiknows/solver/ilpBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/ilpBooleanMethodsCalculator.py` & `DomiKnowS-0.537.dev0/domiknows/solver/ilpBooleanMethodsCalculator.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/ilpOntSolver.py` & `DomiKnowS-0.537.dev0/domiknows/solver/ilpOntSolver.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/ilpOntSolverFactory.py` & `DomiKnowS-0.537.dev0/domiknows/solver/ilpOntSolverFactory.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/lcLossBooleanMethods.py` & `DomiKnowS-0.537.dev0/domiknows/solver/lcLossBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/lcLossSampleBooleanMethods.py` & `DomiKnowS-0.537.dev0/domiknows/solver/lcLossSampleBooleanMethods.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/mini_solver_debug.py` & `DomiKnowS-0.537.dev0/domiknows/solver/mini_solver_debug.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/session/gurobi_session.py` & `DomiKnowS-0.537.dev0/domiknows/solver/session/gurobi_session.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/solver/session/solver_session.py` & `DomiKnowS-0.537.dev0/domiknows/solver/session/solver_session.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/domiknows/utils.py` & `DomiKnowS-0.537.dev0/domiknows/utils.py`

 * *Files identical despite different names*

### Comparing `DomiKnowS-0.536.dev0/setup.py` & `DomiKnowS-0.537.dev0/setup.py`

 * *Files identical despite different names*

