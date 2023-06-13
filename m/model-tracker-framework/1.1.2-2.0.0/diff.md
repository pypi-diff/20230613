# Comparing `tmp/model_tracker_framework-1.1.2.tar.gz` & `tmp/model_tracker_framework-2.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/model-tracker-framework/model-tracker-framework/dist/.tmp-g3ci9qva/model_tracker_framework-1.1.2.tar", last modified: Tue Jun 13 15:40:41 2023, max compression
+gzip compressed data, was "model_tracker_framework-2.0.0.tar", last modified: Tue Apr 19 09:16:58 2022, max compression
```

## Comparing `model_tracker_framework-1.1.2.tar` & `model_tracker_framework-2.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:40:41.000000 model_tracker_framework-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-13 15:40:41.000000 model_tracker_framework-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4416 2023-06-13 15:40:29.000000 model_tracker_framework-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 15:40:41.000000 model_tracker_framework-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-13 15:40:29.000000 model_tracker_framework-1.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:40:41.000000 model_tracker_framework-1.1.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:40:41.000000 model_tracker_framework-1.1.2/src/model_tracker_framework/
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 15:40:29.000000 model_tracker_framework-1.1.2/src/model_tracker_framework/MTFSupporting.py
--rw-r--r--   0 runner    (1001) docker     (123)    12600 2023-06-13 15:40:29.000000 model_tracker_framework-1.1.2/src/model_tracker_framework/ModelExperimentBase.py
--rw-r--r--   0 runner    (1001) docker     (123)     9791 2023-06-13 15:40:29.000000 model_tracker_framework-1.1.2/src/model_tracker_framework/ModelTracker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-06-13 15:40:29.000000 model_tracker_framework-1.1.2/src/model_tracker_framework/SupervisedModelExperiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-06-13 15:40:29.000000 model_tracker_framework-1.1.2/src/model_tracker_framework/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 15:40:41.000000 model_tracker_framework-1.1.2/src/model_tracker_framework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-06-13 15:40:41.000000 model_tracker_framework-1.1.2/src/model_tracker_framework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      509 2023-06-13 15:40:41.000000 model_tracker_framework-1.1.2/src/model_tracker_framework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 15:40:41.000000 model_tracker_framework-1.1.2/src/model_tracker_framework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 15:40:41.000000 model_tracker_framework-1.1.2/src/model_tracker_framework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 15:40:41.000000 model_tracker_framework-1.1.2/src/model_tracker_framework.egg-info/top_level.txt
+drwxr-xr-x   0 joshuaspear   (501) staff       (20)        0 2022-04-19 09:16:58.623422 model_tracker_framework-2.0.0/
+-rw-r--r--   0 joshuaspear   (501) staff       (20)     4834 2022-04-19 09:16:58.623296 model_tracker_framework-2.0.0/PKG-INFO
+-rw-r--r--   0 joshuaspear   (501) staff       (20)     4416 2022-01-04 15:56:10.000000 model_tracker_framework-2.0.0/README.md
+-rw-r--r--   0 joshuaspear   (501) staff       (20)       38 2022-04-19 09:16:58.623466 model_tracker_framework-2.0.0/setup.cfg
+-rw-r--r--   0 joshuaspear   (501) staff       (20)      766 2022-04-19 09:07:40.000000 model_tracker_framework-2.0.0/setup.py
+drwxr-xr-x   0 joshuaspear   (501) staff       (20)        0 2022-04-19 09:16:58.621715 model_tracker_framework-2.0.0/src/
+drwxr-xr-x   0 joshuaspear   (501) staff       (20)        0 2022-04-19 09:16:58.622526 model_tracker_framework-2.0.0/src/model_tracker_framework/
+-rw-r--r--   0 joshuaspear   (501) staff       (20)      449 2022-03-22 16:28:07.000000 model_tracker_framework-2.0.0/src/model_tracker_framework/MTFSupporting.py
+-rw-r--r--   0 joshuaspear   (501) staff       (20)    13815 2022-04-19 08:59:29.000000 model_tracker_framework-2.0.0/src/model_tracker_framework/ModelExperimentBase.py
+-rw-r--r--   0 joshuaspear   (501) staff       (20)     8399 2022-04-19 08:49:23.000000 model_tracker_framework-2.0.0/src/model_tracker_framework/ModelTracker.py
+-rw-r--r--   0 joshuaspear   (501) staff       (20)     1583 2022-04-19 08:58:53.000000 model_tracker_framework-2.0.0/src/model_tracker_framework/SupervisedModelExperiment.py
+-rw-r--r--   0 joshuaspear   (501) staff       (20)      366 2022-01-04 15:56:10.000000 model_tracker_framework-2.0.0/src/model_tracker_framework/__init__.py
+drwxr-xr-x   0 joshuaspear   (501) staff       (20)        0 2022-04-19 09:16:58.623111 model_tracker_framework-2.0.0/src/model_tracker_framework.egg-info/
+-rw-r--r--   0 joshuaspear   (501) staff       (20)     4834 2022-04-19 09:16:58.000000 model_tracker_framework-2.0.0/src/model_tracker_framework.egg-info/PKG-INFO
+-rw-r--r--   0 joshuaspear   (501) staff       (20)      509 2022-04-19 09:16:58.000000 model_tracker_framework-2.0.0/src/model_tracker_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 joshuaspear   (501) staff       (20)        1 2022-04-19 09:16:58.000000 model_tracker_framework-2.0.0/src/model_tracker_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 joshuaspear   (501) staff       (20)        7 2022-04-19 09:16:58.000000 model_tracker_framework-2.0.0/src/model_tracker_framework.egg-info/requires.txt
+-rw-r--r--   0 joshuaspear   (501) staff       (20)       24 2022-04-19 09:16:58.000000 model_tracker_framework-2.0.0/src/model_tracker_framework.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `model_tracker_framework-1.1.2/PKG-INFO` & `model_tracker_framework-2.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: model_tracker_framework
-Version: 1.1.2
+Version: 2.0.0
 Summary: An object-orientated framework for tracking machine learning projects.
-Home-page: https://gitlab.com/kaggle-tings/mtf
+Home-page: https://github.com/joshuaspear/model-tracker-framework
 Author: Joshua Spear
 Author-email: josh.spear9@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # model_tracker_framework
 
 An object-orientated framework for tracking machine learning projects. The framework aims to make building and tracking the results of experiments easier. 
 
 Key features:
@@ -61,7 +62,8 @@
 
 ### MTFSupporting 
 MTFSupporting contains exception classes and the ExperimentOption class. The ExperimentOption should be used when specifying the "dupe_model_nms" parameter for the self.run_experiment method. This class is an attempt to enforce soem static typing in Python cos statically typed > dynamically typed.  
 
 
 ### SupervisedModelExperiment
 The SupervisedModelExperiment class inherits from ModelExperimentBase and provides exactly the same functionilty but provides some attributes which may be useful for running supervised machine learning experiments.
+
```

### Comparing `model_tracker_framework-1.1.2/README.md` & `model_tracker_framework-2.0.0/README.md`

 * *Files identical despite different names*

### Comparing `model_tracker_framework-1.1.2/setup.py` & `model_tracker_framework-2.0.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,23 +5,23 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name='model_tracker_framework',
-    version='1.1.2',
+    version='2.0.0',
     description="An object-orientated framework for tracking machine learning projects.",
     long_description=README,
     packages=setuptools.find_packages(where="src"),
     author="Joshua Spear",
     author_email="josh.spear9@gmail.com",
     long_description_content_type="text/markdown",
-    url="https://gitlab.com/kaggle-tings/mtf",
+    url="https://github.com/joshuaspear/model-tracker-framework",
     license='MIT',
     classifiers=[
         "License :: OSI Approved :: MIT License",
     ],
     package_dir={"": "src"},
-    python_requires=">=3.7",
+    python_requires=">=3.6",
     install_requires=["pandas"]
 )
```

### Comparing `model_tracker_framework-1.1.2/src/model_tracker_framework/ModelExperimentBase.py` & `model_tracker_framework-2.0.0/src/model_tracker_framework/ModelExperimentBase.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+from datetime import datetime
+import logging
 import os
 import shutil
 import time
-
-from datetime import datetime
-import logging
+from typing import Dict
 
 from .MTFSupporting import ModelExperimentBaseError, ExperimentOption
 from .ModelTracker import ModelTracker
 
 logger = logging.getLogger("mtf_logger")
 
-
+# TODO: Midway through converting all params to class definition
 class ModelExperimentBase(ModelTracker):
 
-    def __init__(self, model_name:str, debug_skips_preprop_steps:bool):
+    def __init__(self, model_name:str, debug_skips_preprop_steps:bool, 
+                 existing_tracker_path:str, exp_description:str, 
+                 parent_sv_dir:str, prev_run_notes:str="", 
+                 preprop_kwargs:Dict ={}, preprop_debug_kwargs:Dict={},
+                 train_kwargs:Dict={}, updt_kwargs: dict = {}, 
+                 debug_sv_dir:str=None, force_columns:bool=False):
         """ModelExperimentBase contains keys methods for running experiments and updating an underlying model tracker.
         An experiment is defined as a single observation in the model tracker. 
         The class has been designed such that a (or multiple) "ProjectModelExperiment" class(es) is (are) defined which implement 
         generic sections of the model development process such as the preprocessing stages and evaluation stages. Individual 
         experiments can subsiquently inherit from the "ProjectModelExperiment", implementing experiment specific changes whilst still 
         ultimately updating the same underlying model tracker.
         self.results is utilised by self.run_experiment and can be updated by any method. It is intended to hold model evaluation 
@@ -27,20 +32,44 @@
         _create_output_sub_loc
 
         Args:
             model_name (str): Name of the experiment. If inheriting this class, this variable should not be perminently defined.
             debug_skips_preprop_steps (bool): Defines whether self.preprocessing_debug replaces self.preprocessing_steps or follows it 
             when running in debug model. If set to True, the self.preprocessing_debug will replace self.preprocessing_steps. 
             This attribute is designed to be perminently set wherever the preprocessing steps are defined.
+            existing_tracker_path (str): Location of existing json tracker to update. 
+            exp_description (str): A description of the experiment. 
+            parent_sv_dir (str): The location of the parent directory where the subdirectory should be made to store any 
+            outputs such as graphs.. 
+            prev_run_notes (str, optional): A description of the differences compared to a previous experiment. Defaults to "".
+            preprop_kwargs (dict, optional): kwargs relating to the self.preprocessing_steps
+            preprop_debug_kwargs (dict, optional): kwargs relating to the self.preprocessing_debug
+            train_kwargs (dict, optional): kwargs relating to self.train_model. Defaults to {}.
+            debug_sv_dir (str): Assigns location to model_save_loc if the debug option is selected
+            force_columns (bool): Option to force new columns into the tracker
+            updt_kwargs (dict, optional): kwargs relating to self.import_existing_json_tracker. See ModelTracker for more 
+            info. Defaults to {}.
         """
         super().__init__() 
+        print("ModelExperimentBase init")
+        print(existing_tracker_path)
         self.debug_skips_preprop_steps = debug_skips_preprop_steps
         self.model_name = model_name
         self.results = {}
         self.model_sv_loc = None
+        self.existing_tracker_path = existing_tracker_path
+        self.exp_description = exp_description 
+        self.parent_sv_dir = parent_sv_dir 
+        self.prev_run_notes = prev_run_notes 
+        self.preprop_kwargs = preprop_kwargs
+        self.preprop_debug_kwargs = preprop_debug_kwargs 
+        self.train_kwargs = train_kwargs
+        self.updt_kwargs = updt_kwargs 
+        self.debug_sv_dir = debug_sv_dir 
+        self.force_columns = force_columns
 
 
     def _create_output_sub_loc(self, parent_loc:str, sub_dir_nm: str = None):
         """Creates directory within the parent_loc directory with the model_name as the directory name
 
         Args:
             parent_loc (str): Location of in which the subdirectory should be set. It is advised to set this at a project level
@@ -54,18 +83,18 @@
         sub_loc_path = os.path.join(parent_loc, sub_dir_nm)
         os.mkdir(sub_loc_path)
         self.model_sv_loc = sub_loc_path
 
     def evaluate_model(self):
         raise NotImplementedError("evaluate_model method should be implemented on a experiment type basis or pass if not required.")
     
-    def preprocessing_steps(self):
+    def preprocessing_steps(self, **kwargs):
         raise NotImplementedError("preprocessing_steps method should be implemented on a experiment type basis or pass if not required.")
 
-    def preprocessing_debug(self):
+    def preprocessing_debug(self, **kwargs):
         # Note: If the debug_skips_preprop_steps attribute is set to True, this behaves as an alternate set of preprocessing steps 
         # to preprocessing_steps i.e. if a different dataset should be imported. 
         # If debug_skips_preprop_steps is set to False, this behaves as a postprocessing to the preprocessing_steps i.e. it could sample 
         # from a dataset generated by preprocessing_steps
         raise NotImplementedError("preprocessing_debug method should be implemented on a experiment type basis or pass if not required.")
 
     def preprocessing(self, debug: bool=False):
@@ -73,140 +102,130 @@
 
         Args:
             debug (bool, optional): Specifies whether the preprocessing should be run in debug mode. Refer to self.run_experiment
             for more information. Defaults to False.
         """
         if debug:
             if not self.debug_skips_preprop_steps:
-                self.preprocessing_steps()
+                self.preprocessing_steps(**self.preprop_kwargs)
             try:
-                self.preprocessing_debug()
+                self.preprocessing_debug(**self.preprop_debug_kwargs)
             except NotImplementedError:
                 logger.warning("preprocessing_debug not implemented however skipping error.")
         else:
-            self.preprocessing_steps()
+            self.preprocessing_steps(**self.preprop_kwargs)
 
-    def train_model(self):
+    def train_model(self, **kwargs):
         raise NotImplementedError("train_model method should be implemented on a per experiment basis")
 
-    def run_experiment(self, existing_tracker_path:str, exp_description:str, 
-                       parent_sv_dir:str, prev_run_notes:str="", 
-                       train_kwargs: dict = {}, updt_kwargs: dict = {}, 
-                       dupe_model_nms: ExperimentOption = ExperimentOption(None), 
-                       debug=False, debug_sv_dir:str=None, 
-                       force_columns:bool=False):
+    def run_experiment(self, debug=False, 
+                       dupe_model_nms: ExperimentOption = ExperimentOption(
+                           None)):
         """Runs an experiment in either 'normal' or debug mode specified by the debug parameter. 
         An experiment in 'normal' mode consists of the following:
         1. Create or import an existing tracker from json. If the tracker is imported, check whether an entry with the same 
         self.model_name exists. If it does, handle depending on what is specified by dupe_model_nms
         2. If preprocessing steps have been implemented in self.preprocessing_steps run them
         3. Train the model using self.train_model
         4. Evaluate the model outputs using self.evaluate_model 
         5. Update the tracker and re-save the json
 
         If run in debug mode. No results will be saved and self.preprocessing will be run in debug mode. Refer to 
         self.preprocessing_debug for more information on how self.preprocessing is effected by debug mode
         
 
         Args:
-            existing_tracker_path (str): Location of existing json tracker to update. 
-            exp_description (str): A description of the experiment. 
-            parent_sv_dir (str): The location of the parent directory where the subdirectory should be made to store any 
-            outputs such as graphs.. 
-            prev_run_notes (str, optional): A description of the differences compared to a previous experiment. Defaults to "".
-            train_kwargs (dict, optional): kwargs relating to self.train_model. Defaults to {}.
-            updt_kwargs (dict, optional): kwargs relating to self.import_existing_json_tracker. See ModelTracker for more 
-            info. Defaults to {}.
             dupe_model_nms (ExperimentOption, optional): Defines what action should be taken if an experiment with the same 
             self.model_name is found in the tracker. 
             ExperimentOption('overwrite') will overwrite the previous experiment. 
             ExperimentOption('duplicate') will add both experiments and will append _1 to the new experiment (note if self.model_name_1 also exists, _2 
             will be used etc)
-            ExperimentOption('None') will raise an exception. Defaults to ExperimentOption(None).
             debug (bool, optional): Defines whether the experiment should be run in debug mode. Defaults to False.
-            debug_sv_dir (str): Assigns location to model_save_loc if the debug option is selected
-            force_columns (bool): Option to force new columns into the tracker
         """
-        # TODO: Move parent_sv_dir to an attribute of the class such that it can be set by parent classes
-
         if debug:
             logger.info(" ***** Running in debug mode ***** ")
             logger.info("""No results will be captured in debug mode. 
             If preprocessing method has been defined with debug facilities, this will also run.""")
-            self.model_sv_loc = debug_sv_dir
+            self.model_sv_loc = self.debug_sv_dir
             try:
                 self.preprocessing(debug=True)
             except NotImplementedError:
                 logger.warning("preprocessing_steps not implemented however skipping error.")
-            self.train_model(**train_kwargs)
+            self.train_model(**self.train_kwargs)
 
         else:
             logger.info(" ***** Importing existing tracker ***** ")
-            if self.check_tracker_exists(existing_tracker_path=existing_tracker_path):
+            if self.check_tracker_exists(existing_tracker_path=
+                                         self.existing_tracker_path):
                 logger.info("Tracker identified. Importing...")
                 # TODO: Implement the ability to specify what type of tracker to import i.e. dataframe/csv/json etc
-                self.import_existing_json_tracker(existing_tracker_path, 
-                                                  **updt_kwargs)
+                self.import_existing_json_tracker(self.existing_tracker_path, 
+                                                  **self.updt_kwargs)
             else:
                 logger.info("Could not find tracker at location, creating new tracker")
 
             logger.info(" ***** Checking whether model exists in tracker ***** ")
             curr_model_nms = [rw["model_name"] for rw in self.rows]
             if self.model_name in curr_model_nms:
                 logger.info("{} run already exists".format(self.model_name))
                 if dupe_model_nms.exp_option == "overwrite":
                     logger.info("Overwriting previous run")
                     # Cannot just use index incase duplicates have already slipped through!
                     dupe_indices = [idx for idx, mdl_nm in enumerate(curr_model_nms) if mdl_nm == self.model_name]
                     dupe_indices.sort(reverse=True)
                     for idx in dupe_indices:
                         del self.rows[idx]
-                    if os.path.exists(os.path.join(parent_sv_dir, self.model_name)):
-                        shutil.rmtree(os.path.join(parent_sv_dir, self.model_name))
+                    if os.path.exists(os.path.join(self.parent_sv_dir, 
+                                                   self.model_name)):
+                        shutil.rmtree(os.path.join(self.parent_sv_dir, 
+                                                   self.model_name))
                         dir_not_rmved = True
                         while(dir_not_rmved):
                             time.sleep(1)
                             dir_not_rmved = os.path.exists(os.path.join(
-                                parent_sv_dir, self.model_name))
-                    self._create_output_sub_loc(parent_sv_dir)
+                                self.parent_sv_dir, self.model_name))
+                    self._create_output_sub_loc(self.parent_sv_dir)
                 elif dupe_model_nms.exp_option == "duplicate":
                     logger.info("Keeping both runs")
                     avail_loc = False
                     sup_dir_idx = 1
                     # Loop through adding 1 to the end each time to find available name to save model 
                     while avail_loc == False:
                         sup_dir = "{}_{}".format(self.model_name, sup_dir_idx)
-                        if not os.path.exists(os.path.join(parent_sv_dir, sup_dir)):
+                        if not os.path.exists(os.path.join(self.parent_sv_dir, 
+                                                           sup_dir)):
                             avail_loc = True
-                            self._create_output_sub_loc(parent_sv_dir, sup_dir)
+                            self._create_output_sub_loc(self.parent_sv_dir, 
+                                                        sup_dir)
                         sup_dir_idx  =+ 1
                 elif dupe_model_nms.exp_option == None:
                     raise ModelExperimentBaseError(
                 "Run with model name {} already exists therefore duplicate or overwrite must be specified in the dupe_model_nms option".format(self.model_name))
             else:
-                self._create_output_sub_loc(parent_sv_dir)
+                self._create_output_sub_loc(self.parent_sv_dir)
 
             logger.info(" **** Training model ***** ")
             train_time_strt = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
             try:
                 self.preprocessing()
             except NotImplementedError:
                 logger.warning("preprocessing_steps not implemented however skipping error.")
-            self.train_model(**train_kwargs)
+            self.train_model(**self.train_kwargs)
             train_time_end = datetime.now().strftime("%d/%m/%Y %H:%M:%S")
             logger.info(" ***** Evaluating model ***** ")
             self.evaluate_model()
             new_tracker_line = {**self.results,
                                 "model_name": self.model_name,
-                                "experiment_description": exp_description,
-                                "prev_run_notes": prev_run_notes,
+                                "experiment_description": self.exp_description,
+                                "prev_run_notes": self.prev_run_notes,
                                 "train_time_strt": train_time_strt,
                                 "train_time_end": train_time_end,
-                                "output_save_location": self.model_sv_loc
+                                "output_save_location": self.model_sv_loc,
+                                **self.train_kwargs, **self.preprop_kwargs
                                 }
             logger.info(" ***** Updating tracker ***** ")
             self.update_tracker_w_dict(new_tracker_line, 
-                                       force_columns=force_columns)
+                                       force_columns=self.force_columns)
             logger.info(" ***** Updating json ***** ")
-            self.tracker_to_json(json_dir=existing_tracker_path)
+            self.tracker_to_json(json_dir=self.existing_tracker_path)
```

### Comparing `model_tracker_framework-1.1.2/src/model_tracker_framework/ModelTracker.py` & `model_tracker_framework-2.0.0/src/model_tracker_framework/ModelTracker.py`

 * *Files 17% similar despite different names*

```diff
@@ -4,43 +4,36 @@
 import pandas as pd
 
 logger = logging.getLogger("mtf_logger")
 
 
 class ModelTracker:
     
-    def __init__(self, u_id:str="model_name"):
+    def __init__(self):
         """Class representing a 'model tracker'. 
-        self.rows is a list dictionaries where each dictionary is of the form 
-        {column_name: value} and each dictionary represents an individual 
-        experiment
+        self.rows is a list dictionaries where each dictionary is of the form {column_name: value} and each dictionary represents an 
+        individual experiment
         self.column_names is a list of unique column_name value from self.rows
         
         """
         self.rows = []
         self.column_names = []
-        self.u_id = u_id
 
-    def _get_check_consistent_col_names(self, new_row_col_names:list, 
-                                        force_columns:bool=False) -> set:
-        """Method is used check whether the column names provided in 
-        new_row_col_names are consistent with the current names housed in 
-        self.column_names. The method raises an exception if the new column 
-        names don't align unless force_columns is set to True, in which case a 
-        warning is provided.
+    def _get_check_consistent_col_names(self, new_row_col_names:list, force_columns:bool=False) -> set:
+        """Method is used check whether the column names provided in new_row_col_names are consistent with the current 
+        names housed in self.column_names. The method raises an exception if the new column names don't align unless 
+        force_columns is set to True, in which case a warning is provided.
         
 
         Args:
             new_row_col_names (list): List of column names to check
-            force_columns (bool, optional): Option to force new column names in 
-            and avoid exception. Defaults to False.
+            force_columns (bool, optional): Option to force new column names in and avoid exception. Defaults to False.
 
         Returns:
-            set: The column names provided in new_row_col_names that are not 
-            already in self.column_names
+            set: The column names provided in new_row_col_names that are not already in self.column_names
         """
         miss_frm_exst_col = set(self.column_names) - set(new_row_col_names)
         miss_frm_exst_col_wrn = "Column names {} already exist in the tracker however are missing from the new row".format(miss_frm_exst_col)
         nw_col_names = set(new_row_col_names) - set(self.column_names)
         nw_col_names_wrn = "{} are new column names in the row that are not already in the tracker".format(nw_col_names)
         if len(self.column_names) > 0:
             # Only check if column names are not empty
@@ -51,170 +44,120 @@
                     logger.warning(nw_col_names_wrn)
             else:
                 assert(len(miss_frm_exst_col) == 0), miss_frm_exst_col_wrn
                 assert(len(nw_col_names) == 0), nw_col_names_wrn
         return nw_col_names
 
     def update_tracker_w_dict(self, row_dict:dict, force_columns:bool=False):
-        """Updates the self.rows and self.column_names with the new values 
-        provided in row_dict
+        """Updates the self.rows and self.column_names with the new values provided in row_dict
 
         Args:
-            row_dict (dict): dictionary containing {column:values} to be added 
-            to the tracker
-            force_columns (bool, optional): Option to force new column names in 
-            and avoid exception. Defaults to False.
-        """
-        try:
-            row_idx = self.get_cur_row_index(u_id=row_dict[self.u_id])
-            logger.warn(
-                "Model already exists in tracker, overwriting relevant values")
-            old_row = self.rows.pop(row_idx)
-            for i in row_dict:
-                old_row[i] = row_dict[i]
-            row_dict = old_row
-        except KeyError as e:
-            pass     
+            row_dict (dict): dictionary containing {column:values} to be added to the tracker
+            force_columns (bool, optional): Option to force new column names in and avoid exception. Defaults to False.
+        """
+
         new_row_col_names = [col for col in row_dict.keys()]
-        nw_col_names = self._get_check_consistent_col_names(
-            new_row_col_names=new_row_col_names, force_columns=force_columns)
+        nw_col_names = self._get_check_consistent_col_names(new_row_col_names=new_row_col_names,
+                                                            force_columns=force_columns)
         if len(nw_col_names) > 0:
             self.column_names += nw_col_names
         self.rows.append(row_dict)
-        
-    def check_model_exists(self, u_id:str):
-        curr_model_nms = [rw[u_id] for rw in self.rows]
-        res = u_id in curr_model_nms
-        return res
-    
-    def get_cur_row_index(self, u_id:str):
-        for idx, rw in enumerate(self.rows):
-            if rw[self.u_id] == u_id:
-                return idx
-        raise KeyError("Model does not exist in tracker")
 
     def tracker_to_pandas_df(self)->pd.DataFrame:
-        """Converts the values stored in self.rows and returns in the form of a 
-        dataframe
+        """Converts the values stored in self.rows and returns in the form of a dataframe
 
         Returns:
             pd.DataFrame: Dataframe containing the values in self.rows
         """
         dict_df = pd.DataFrame.from_dict(self.rows)
         return dict_df
-    
-    
 
     def tracker_to_csv(self, csv_dir:str, **kwargs):
-        """Saves the tracker i.e. values in self.rows as a csv. This is performed 
-        via pandas. kwargs should contain options defined in 
-        pd.DataFrame.to_csv()
+        """Saves the tracker i.e. values in self.rows as a csv. This is performed via pandas.
+        kwargs should contain options defined in pd.DataFrame.to_csv()
         
 
         Args:
             csv_dir (str): File location of where to save the output csv
         """
         dict_df = self.tracker_to_pandas_df()
         dict_df.to_csv(csv_dir, **kwargs)
 
     def import_existing_pandas_df_tracker(self, exstng_track_df:pd.DataFrame, **kwargs):
-        """Takes as an input a dataframe representing and model tracker and 
-        updates self with values from the dataframe. kwargs should refer to 
-        updating options defined in self.update_tracker_w_dict
+        """Takes as an input a dataframe representing and model tracker and updates self with values from the dataframe.
+        kwargs should refer to updating options defined in self.update_tracker_w_dict
         
 
         Args:
-            exstng_track_df (pd.DataFrame): Pandas dataframe representing a 
-            model tracker
+            exstng_track_df (pd.DataFrame): Pandas dataframe representing a model tracker
         """
         exstng_track_dict = exstng_track_df.to_dict("records")
         for row in exstng_track_dict:
             self.update_tracker_w_dict(row, **kwargs)
 
     def import_existing_csv_tracker(self, existing_tracker_path:str, imprt_kwargs:dict = {}, rd_csv_kwargs:dict = {}):
-        """Takes as an input a csv representing and model tracker and updates 
-        self with values from the csv. This is performed via pandas. 
+        """Takes as an input a csv representing and model tracker and updates self with values from the csv. 
+        This is performed via pandas. 
 
         Args:
             existing_tracker_path (str): File location of the csv tracker
-            imprt_kwargs (dict): kwargs to provide to 
-            self.import_existing_pandas_df_tracker. Defaults to {}.
-            rd_csv_kwargs (dict): kwargs to provide to pd.read_csv. 
-            Defaults to {}.
+            imprt_kwargs (dict): kwargs to provide to self.import_existing_pandas_df_tracker. Defaults to {}.
+            rd_csv_kwargs (dict): kwargs to provide to pd.read_csv. Defaults to {}.
         """
         exstng_track_df = pd.read_csv(existing_tracker_path, **rd_csv_kwargs)
         self.import_existing_pandas_df_tracker(exstng_track_df, **imprt_kwargs)
 
-    def update_existing_csv_tracker(self, existing_tracker_path:str, 
-                                    imprt_kwargs:dict = {}, 
-                                    rd_csv_kwargs:dict = {}, 
-                                    wrt_csv_kwargs:dict = {}):
-        """Imports a csv file representing a model tracker, updates it with the 
-        observations captured in self and re-writes the csv
+    def update_existing_csv_tracker(self, existing_tracker_path:str, imprt_kwargs:dict = {}, rd_csv_kwargs:dict = {}, 
+    wrt_csv_kwargs:dict = {}):
+        """Imports a csv file representing a model tracker, updates it with the observations captured in self and re-writes the csv
 
         Args:
             existing_tracker_path (str): File location of the csv tracker
-            imprt_kwargs (dict, optional): kwargs to provide to 
-            self.import_existing_pandas_df_tracker. Defaults to {}.
-            rd_csv_kwargs (dict, optional): kwargs to provide to pd.read_csv. 
-            Defaults to {}.
-            wrt_csv_kwargs (dict, optional): kwargs to provide to 
-            pd.DataFrame.to_csv. Defaults to {}.
-        """
-        self.import_existing_csv_tracker(
-            existing_tracker_path=existing_tracker_path, 
-            imprt_kwargs=imprt_kwargs, rd_csv_kwargs=rd_csv_kwargs)
-        self.tracker_to_csv(existing_tracker_path, index=False, 
-                            **wrt_csv_kwargs)
+            imprt_kwargs (dict, optional): kwargs to provide to self.import_existing_pandas_df_tracker. Defaults to {}.
+            rd_csv_kwargs (dict, optional): kwargs to provide to pd.read_csv. Defaults to {}.
+            wrt_csv_kwargs (dict, optional): kwargs to provide to pd.DataFrame.to_csv. Defaults to {}.
+        """
+        self.import_existing_csv_tracker(existing_tracker_path=existing_tracker_path, imprt_kwargs=imprt_kwargs, 
+        rd_csv_kwargs=rd_csv_kwargs)
+        self.tracker_to_csv(existing_tracker_path, index=False, **wrt_csv_kwargs)
 
     def tracker_to_json(self, json_dir:str, **kwargs):
-        """Saves the tracker i.e. values in self.rows as a json. This is 
-        performed via pandas. kwargs should contain options defined in 
-        pd.DataFrame.to_json()
+        """Saves the tracker i.e. values in self.rows as a json. This is performed via pandas.
+        kwargs should contain options defined in pd.DataFrame.to_json()
 
         Args:
             json_dir (str): File location of where to save the output json
         """
         dict_df = self.tracker_to_pandas_df()
         dict_df.to_json(json_dir, **kwargs)
 
-    def import_existing_json_tracker(self, existing_tracker_path:str, 
-                                     imprt_kwargs:dict = {}, 
-                                     rd_json_kwargs:dict = {}):
-        """Takes as an input a json representing and model tracker and updates 
-        self with values from the json. This is performed via pandas.
+    def import_existing_json_tracker(self, existing_tracker_path:str, imprt_kwargs:dict = {}, rd_json_kwargs:dict = {}):
+        """Takes as an input a json representing and model tracker and updates self with values from the json. 
+        This is performed via pandas.
 
         Args:
             existing_tracker_path (str): File location of the csv tracker
-            imprt_kwargs (dict, optional): kwargs to provide to 
-            self.import_existing_pandas_df_tracker. Defaults to {}.
-            rd_json_kwargs (dict, optional): kwargs to provide to pd.read_json. 
-            Defaults to {}.
+            imprt_kwargs (dict, optional): kwargs to provide to self.import_existing_pandas_df_tracker. Defaults to {}.
+            rd_json_kwargs (dict, optional): kwargs to provide to pd.read_json. Defaults to {}.
         """
         exstng_track_df = pd.read_json(existing_tracker_path, **rd_json_kwargs)
         self.import_existing_pandas_df_tracker(exstng_track_df, **imprt_kwargs)
 
-    def update_existing_json_tracker(self, existing_tracker_path: str, 
-                                     imprt_kwargs: dict = {},
+    def update_existing_json_tracker(self, existing_tracker_path: str, imprt_kwargs: dict = {},
     rd_json_kwargs:dict = {}, wrt_json_kwargs: dict = {}):
-        """Imports a json file representing a model tracker, updates it with the 
-        observations captured in self and re-writes the json
+        """Imports a json file representing a model tracker, updates it with the observations captured in self and re-writes the json
 
         Args:
             existing_tracker_path (str): File location of the csv tracker
-            imprt_kwargs (dict, optional): kwargs to provide to 
-            self.import_existing_pandas_df_tracker. Defaults to {}.
-            rd_json_kwargs (dict, optional): kwargs to provide to pd.read_json. 
-            Defaults to {}.
-            wrt_json_kwargs (dict, optional): kwargs to provide to 
-            pd.DataFrame.to_json. Defaults to {}.
-        """
-        self.import_existing_json_tracker(
-            existing_tracker_path=existing_tracker_path, 
-            imprt_kwargs=imprt_kwargs, rd_json_kwargs=rd_json_kwargs)
+            imprt_kwargs (dict, optional): kwargs to provide to self.import_existing_pandas_df_tracker. Defaults to {}.
+            rd_json_kwargs (dict, optional): kwargs to provide to pd.read_json. Defaults to {}.
+            wrt_json_kwargs (dict, optional): kwargs to provide to pd.DataFrame.to_json. Defaults to {}.
+        """
+        self.import_existing_json_tracker(existing_tracker_path=existing_tracker_path, imprt_kwargs=imprt_kwargs, 
+        rd_json_kwargs=rd_json_kwargs)
         self.tracker_to_json(existing_tracker_path, **wrt_json_kwargs)
 
     @staticmethod
     def check_tracker_exists(existing_tracker_path: str) -> bool:
         """Confirms whether a file exists.
 
         Args:
```

### Comparing `model_tracker_framework-1.1.2/src/model_tracker_framework.egg-info/PKG-INFO` & `model_tracker_framework-2.0.0/src/model_tracker_framework.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: model-tracker-framework
-Version: 1.1.2
+Version: 2.0.0
 Summary: An object-orientated framework for tracking machine learning projects.
-Home-page: https://gitlab.com/kaggle-tings/mtf
+Home-page: https://github.com/joshuaspear/model-tracker-framework
 Author: Joshua Spear
 Author-email: josh.spear9@gmail.com
 License: MIT
+Platform: UNKNOWN
 Classifier: License :: OSI Approved :: MIT License
-Requires-Python: >=3.7
+Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # model_tracker_framework
 
 An object-orientated framework for tracking machine learning projects. The framework aims to make building and tracking the results of experiments easier. 
 
 Key features:
@@ -61,7 +62,8 @@
 
 ### MTFSupporting 
 MTFSupporting contains exception classes and the ExperimentOption class. The ExperimentOption should be used when specifying the "dupe_model_nms" parameter for the self.run_experiment method. This class is an attempt to enforce soem static typing in Python cos statically typed > dynamically typed.  
 
 
 ### SupervisedModelExperiment
 The SupervisedModelExperiment class inherits from ModelExperimentBase and provides exactly the same functionilty but provides some attributes which may be useful for running supervised machine learning experiments.
+
```

