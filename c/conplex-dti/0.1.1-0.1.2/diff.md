# Comparing `tmp/conplex_dti-0.1.1.tar.gz` & `tmp/conplex_dti-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conplex_dti-0.1.1.tar", max compression
+gzip compressed data, was "conplex_dti-0.1.2.tar", max compression
```

## Comparing `conplex_dti-0.1.1.tar` & `conplex_dti-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1074 2023-03-11 16:53:19.162872 conplex_dti-0.1.1/LICENSE
--rw-r--r--   0        0        0     3544 2023-04-27 21:09:41.869490 conplex_dti-0.1.1/README.md
--rw-r--r--   0        0        0     3510 2023-04-27 20:13:59.889524 conplex_dti-0.1.1/conplex_dti/MAIN_OLD.txt
--rw-r--r--   0        0        0      399 2023-06-12 15:18:13.332699 conplex_dti-0.1.1/conplex_dti/__init__.py
--rw-r--r--   0        0        0     1070 2023-06-12 15:38:30.887853 conplex_dti-0.1.1/conplex_dti/__main__.py
--rw-r--r--   0        0        0    23714 2023-04-27 20:13:59.892315 conplex_dti-0.1.1/conplex_dti/architectures.py
--rw-r--r--   0        0        0      166 2023-04-27 20:13:59.893555 conplex_dti-0.1.1/conplex_dti/cli/__init__.py
--rw-r--r--   0        0        0     1316 2023-04-27 20:13:59.894669 conplex_dti-0.1.1/conplex_dti/cli/download.py
--rw-r--r--   0        0        0    19418 2023-06-12 15:34:12.673595 conplex_dti-0.1.1/conplex_dti/cli/train.py
--rw-r--r--   0        0        0      171 2023-04-27 20:13:59.897366 conplex_dti-0.1.1/conplex_dti/dataset/__init__.py
--rw-r--r--   0        0        0    24290 2023-04-27 21:07:43.467420 conplex_dti-0.1.1/conplex_dti/dataset/datamodules.py
--rw-r--r--   0        0        0      421 2023-04-27 20:13:59.900173 conplex_dti-0.1.1/conplex_dti/featurizer/__init__.py
--rw-r--r--   0        0        0     7731 2023-04-27 20:13:59.901288 conplex_dti-0.1.1/conplex_dti/featurizer/base.py
--rw-r--r--   0        0        0    11422 2023-04-27 20:13:59.902654 conplex_dti-0.1.1/conplex_dti/featurizer/molecule.py
--rw-r--r--   0        0        0    11493 2023-04-27 21:09:39.865982 conplex_dti-0.1.1/conplex_dti/featurizer/protein.py
--rw-r--r--   0        0        0        0 2023-04-27 20:13:59.904417 conplex_dti-0.1.1/conplex_dti/model/__init__.py
--rw-r--r--   0        0        0    23789 2023-04-27 20:13:59.906381 conplex_dti-0.1.1/conplex_dti/model/architectures.py
--rw-r--r--   0        0        0     2125 2023-04-27 20:13:59.907393 conplex_dti-0.1.1/conplex_dti/model/margin.py
--rw-r--r--   0        0        0     4022 2023-04-27 20:13:59.908432 conplex_dti-0.1.1/conplex_dti/utils.py
--rw-r--r--   0        0        0     4177 2023-06-12 15:17:57.003372 conplex_dti-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5146 1970-01-01 00:00:00.000000 conplex_dti-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-03-11 16:53:19.162872 conplex_dti-0.1.2/LICENSE
+-rw-r--r--   0        0        0     3723 2023-06-12 16:38:19.603868 conplex_dti-0.1.2/README.md
+-rw-r--r--   0        0        0     3510 2023-04-27 20:13:59.889524 conplex_dti-0.1.2/conplex_dti/MAIN_OLD.txt
+-rw-r--r--   0        0        0      399 2023-06-12 16:38:19.605660 conplex_dti-0.1.2/conplex_dti/__init__.py
+-rw-r--r--   0        0        0     1070 2023-06-12 16:38:19.607396 conplex_dti-0.1.2/conplex_dti/__main__.py
+-rw-r--r--   0        0        0    23714 2023-04-27 20:13:59.892315 conplex_dti-0.1.2/conplex_dti/architectures.py
+-rw-r--r--   0        0        0      166 2023-04-27 20:13:59.893555 conplex_dti-0.1.2/conplex_dti/cli/__init__.py
+-rw-r--r--   0        0        0     1316 2023-04-27 20:13:59.894669 conplex_dti-0.1.2/conplex_dti/cli/download.py
+-rw-r--r--   0        0        0    19492 2023-06-13 20:17:18.168303 conplex_dti-0.1.2/conplex_dti/cli/train.py
+-rw-r--r--   0        0        0      171 2023-04-27 20:13:59.897366 conplex_dti-0.1.2/conplex_dti/dataset/__init__.py
+-rw-r--r--   0        0        0    24290 2023-06-12 16:38:19.611383 conplex_dti-0.1.2/conplex_dti/dataset/datamodules.py
+-rw-r--r--   0        0        0      421 2023-04-27 20:13:59.900173 conplex_dti-0.1.2/conplex_dti/featurizer/__init__.py
+-rw-r--r--   0        0        0     7731 2023-04-27 20:13:59.901288 conplex_dti-0.1.2/conplex_dti/featurizer/base.py
+-rw-r--r--   0        0        0    11422 2023-04-27 20:13:59.902654 conplex_dti-0.1.2/conplex_dti/featurizer/molecule.py
+-rw-r--r--   0        0        0    11493 2023-04-27 21:09:39.865982 conplex_dti-0.1.2/conplex_dti/featurizer/protein.py
+-rw-r--r--   0        0        0        0 2023-04-27 20:13:59.904417 conplex_dti-0.1.2/conplex_dti/model/__init__.py
+-rw-r--r--   0        0        0    23789 2023-04-27 20:13:59.906381 conplex_dti-0.1.2/conplex_dti/model/architectures.py
+-rw-r--r--   0        0        0     2125 2023-04-27 20:13:59.907393 conplex_dti-0.1.2/conplex_dti/model/margin.py
+-rw-r--r--   0        0        0     4022 2023-04-27 20:13:59.908432 conplex_dti-0.1.2/conplex_dti/utils.py
+-rw-r--r--   0        0        0     4177 2023-06-13 20:17:36.998182 conplex_dti-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5325 1970-01-01 00:00:00.000000 conplex_dti-0.1.2/PKG-INFO
```

### Comparing `conplex_dti-0.1.1/LICENSE` & `conplex_dti-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.1/README.md` & `conplex_dti-0.1.2/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-# 🚧🚧 Currently under construction 🚧🚧
-
 # ConPLex
 
 ![ConPLex Schematic](assets/images/Fig2_Schematic.png)
 
 [![ConPLex Releases](https://img.shields.io/github/v/release/samsledje/ConPLex?include_prereleases)](https://github.com/samsledje/ConPLex/releases)
 [![PyPI](https://img.shields.io/pypi/v/conplex-dti)](https://pypi.org/project/conplex-dti/)
 [![Documentation Status](https://readthedocs.org/projects/conplex/badge/?version=main)](https://conplex.readthedocs.io/en/main/?badge=main)
 [![License](https://img.shields.io/github/license/samsledje/ConPLex)](https://github.com/samsledje/ConPLex/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-- [Homepage](http://conplex.csail.mit.edu)
-- [Documentation](https://d-script.readthedocs.io/en/main/)
+🚧🚧 Please note that ConPLex v0.1.0 is currently a pre-release and is actively being developed. For the code used to generate our PNAS results, see the [manuscript code](https://github.com/samsledje/ConPLex_dev) 🚧🚧
+
+ - [Homepage](http://conplex.csail.mit.edu)
+ - [Documentation](https://d-script.readthedocs.io/en/main/)
 
 ## Abstract
 
 Sequence-based prediction of drug-target interactions has the potential to accelerate drug discovery by complementing experimental screens. Such computational prediction needs to be generalizable and scalable while remaining sensitive to subtle variations in the inputs. However, current computational techniques fail to simultaneously meet these goals, often sacrificing performance on one to achieve the others. We develop a deep learning model, ConPLex, successfully leveraging the advances in pre-trained protein language models ("PLex") and employing  a novel  protein-anchored contrastive co-embedding ("Con") to outperform state-of-the-art approaches. ConPLex achieves high accuracy, broad adaptivity to unseen data, and specificity against decoy compounds. It makes predictions of binding based on the distance between learned representations, enabling predictions at the scale of massive compound libraries and the human proteome. Experimental testing of 19 kinase-drug interaction predictions validated 12 interactions, including four with sub-nanomolar affinity, plus a novel strongly-binding EPHB1 inhibitor ($K_D = 1.3nM$). Furthermore, ConPLex embeddings are interpretable, which enables us to visualize the drug-target embedding space and use embeddings to characterize the function of human cell-surface proteins. We anticipate ConPLex will facilitate novel drug discovery by making highly sensitive in-silico drug screening feasible at genome scale.
 
 ## Installation
```

### Comparing `conplex_dti-0.1.1/conplex_dti/MAIN_OLD.txt` & `conplex_dti-0.1.2/conplex_dti/MAIN_OLD.txt`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.1/conplex_dti/__main__.py` & `conplex_dti-0.1.2/conplex_dti/__main__.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.1/conplex_dti/architectures.py` & `conplex_dti-0.1.2/conplex_dti/architectures.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.1/conplex_dti/cli/download.py` & `conplex_dti-0.1.2/conplex_dti/cli/download.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.1/conplex_dti/cli/train.py` & `conplex_dti-0.1.2/conplex_dti/cli/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -327,19 +327,19 @@
     training_generator = datamodule.train_dataloader()
     validation_generator = datamodule.val_dataloader()
     testing_generator = datamodule.test_dataloader()
 
     if config.contrastive:
         logg.info("Loading contrastive data (DUDE)")
         dude_drug_featurizer = get_featurizer(
-            config.drug_featurizer, save_dir=get_task_dir("DUDe")
+            config.drug_featurizer, save_dir=get_task_dir("DUDe", database_root=config.data_cache_dir)
         )
 
         dude_target_featurizer = get_featurizer(
-            config.target_featurizer, save_dir=get_task_dir("DUDe")
+            config.target_featurizer, save_dir=get_task_dir("DUDe", database_root=config.data_cache_dir)
         )
 
         contrastive_datamodule = DUDEDataModule(
             config.contrastive_split,
             dude_drug_featurizer,
             dude_target_featurizer,
             device=device,
```

### Comparing `conplex_dti-0.1.1/conplex_dti/dataset/datamodules.py` & `conplex_dti-0.1.2/conplex_dti/dataset/datamodules.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.1/conplex_dti/featurizer/base.py` & `conplex_dti-0.1.2/conplex_dti/featurizer/base.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.1/conplex_dti/featurizer/molecule.py` & `conplex_dti-0.1.2/conplex_dti/featurizer/molecule.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.1/conplex_dti/featurizer/protein.py` & `conplex_dti-0.1.2/conplex_dti/featurizer/protein.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.1/conplex_dti/model/architectures.py` & `conplex_dti-0.1.2/conplex_dti/model/architectures.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.1/conplex_dti/model/margin.py` & `conplex_dti-0.1.2/conplex_dti/model/margin.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.1/conplex_dti/utils.py` & `conplex_dti-0.1.2/conplex_dti/utils.py`

 * *Files identical despite different names*

### Comparing `conplex_dti-0.1.1/pyproject.toml` & `conplex_dti-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "conplex-dti"
-version = "0.1.1"
+version = "0.1.2"
 description = "Adapting protein language models and contrastive learning for DTI prediction."
 readme = "README.md"
 authors = ["samsledje <samsl@mit.edu>"]
 license = "MIT"
 repository = "https://github.com/samsledje/ConPLex"
 homepage = "https://github.com/samsledje/ConPLex"
```

### Comparing `conplex_dti-0.1.1/PKG-INFO` & `conplex_dti-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conplex-dti
-Version: 0.1.1
+Version: 0.1.2
 Summary: Adapting protein language models and contrastive learning for DTI prediction.
 Home-page: https://github.com/samsledje/ConPLex
 License: MIT
 Keywords: protein language models,contrastive learning,drug target interaction,DTI
 Author: samsledje
 Author-email: samsl@mit.edu
 Requires-Python: >=3.9,<4.0
@@ -32,28 +32,28 @@
 Requires-Dist: tqdm (>=4.62,<5.0)
 Requires-Dist: transformers (>=4.26.1,<5.0.0)
 Requires-Dist: typer[all] (>=0.4.0,<0.5.0)
 Requires-Dist: wandb (>=0.13,<0.14)
 Project-URL: Repository, https://github.com/samsledje/ConPLex
 Description-Content-Type: text/markdown
 
-# 🚧🚧 Currently under construction 🚧🚧
-
 # ConPLex
 
 ![ConPLex Schematic](assets/images/Fig2_Schematic.png)
 
 [![ConPLex Releases](https://img.shields.io/github/v/release/samsledje/ConPLex?include_prereleases)](https://github.com/samsledje/ConPLex/releases)
 [![PyPI](https://img.shields.io/pypi/v/conplex-dti)](https://pypi.org/project/conplex-dti/)
 [![Documentation Status](https://readthedocs.org/projects/conplex/badge/?version=main)](https://conplex.readthedocs.io/en/main/?badge=main)
 [![License](https://img.shields.io/github/license/samsledje/ConPLex)](https://github.com/samsledje/ConPLex/blob/main/LICENSE)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
-- [Homepage](http://conplex.csail.mit.edu)
-- [Documentation](https://d-script.readthedocs.io/en/main/)
+🚧🚧 Please note that ConPLex v0.1.0 is currently a pre-release and is actively being developed. For the code used to generate our PNAS results, see the [manuscript code](https://github.com/samsledje/ConPLex_dev) 🚧🚧
+
+ - [Homepage](http://conplex.csail.mit.edu)
+ - [Documentation](https://d-script.readthedocs.io/en/main/)
 
 ## Abstract
 
 Sequence-based prediction of drug-target interactions has the potential to accelerate drug discovery by complementing experimental screens. Such computational prediction needs to be generalizable and scalable while remaining sensitive to subtle variations in the inputs. However, current computational techniques fail to simultaneously meet these goals, often sacrificing performance on one to achieve the others. We develop a deep learning model, ConPLex, successfully leveraging the advances in pre-trained protein language models ("PLex") and employing  a novel  protein-anchored contrastive co-embedding ("Con") to outperform state-of-the-art approaches. ConPLex achieves high accuracy, broad adaptivity to unseen data, and specificity against decoy compounds. It makes predictions of binding based on the distance between learned representations, enabling predictions at the scale of massive compound libraries and the human proteome. Experimental testing of 19 kinase-drug interaction predictions validated 12 interactions, including four with sub-nanomolar affinity, plus a novel strongly-binding EPHB1 inhibitor ($K_D = 1.3nM$). Furthermore, ConPLex embeddings are interpretable, which enables us to visualize the drug-target embedding space and use embeddings to characterize the function of human cell-surface proteins. We anticipate ConPLex will facilitate novel drug discovery by making highly sensitive in-silico drug screening feasible at genome scale.
 
 ## Installation
```

