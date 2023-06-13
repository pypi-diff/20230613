# Comparing `tmp/torchtime-0.5.1.tar.gz` & `tmp/torchtime-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchtime-0.5.1.tar", max compression
+gzip compressed data, was "torchtime-0.6.0.tar", max compression
```

## Comparing `torchtime-0.5.1.tar` & `torchtime-0.6.0.tar`

### file list

```diff
@@ -1,11 +1,10 @@
--rwxr-xr-x   0        0        0     1071 2022-08-03 09:47:34.817864 torchtime-0.5.1/LICENSE
--rw-r--r--   0        0        0     8211 2022-08-03 09:47:34.817864 torchtime-0.5.1/README.md
--rw-r--r--   0        0        0     1078 2022-08-03 09:47:34.821864 torchtime-0.5.1/pyproject.toml
--rw-r--r--   0        0        0       75 2022-08-03 09:47:34.821864 torchtime-0.5.1/src/torchtime/__init__.py
--rw-r--r--   0        0        0     4851 2022-08-03 09:47:34.821864 torchtime-0.5.1/src/torchtime/collate.py
--rw-r--r--   0        0        0     1943 2022-08-03 09:47:34.821864 torchtime-0.5.1/src/torchtime/constants.py
--rw-r--r--   0        0        0    57401 2022-08-03 09:47:34.821864 torchtime-0.5.1/src/torchtime/data.py
--rw-r--r--   0        0        0     4539 2022-08-03 09:47:34.821864 torchtime-0.5.1/src/torchtime/impute.py
--rw-r--r--   0        0        0     8461 2022-08-03 09:47:34.821864 torchtime-0.5.1/src/torchtime/utils.py
--rw-r--r--   0        0        0     9217 2022-08-03 09:50:01.995739 torchtime-0.5.1/setup.py
--rw-r--r--   0        0        0     9074 2022-08-03 09:50:01.996374 torchtime-0.5.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1071 2023-06-12 18:49:08.012030 torchtime-0.6.0/LICENSE
+-rw-r--r--   0        0        0     8415 2023-06-12 18:49:08.012030 torchtime-0.6.0/README.md
+-rw-r--r--   0        0        0     1073 2023-06-12 18:50:35.348596 torchtime-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0       75 2023-06-12 18:49:08.012030 torchtime-0.6.0/src/torchtime/__init__.py
+-rw-r--r--   0        0        0     4851 2023-06-12 18:49:08.012030 torchtime-0.6.0/src/torchtime/collate.py
+-rw-r--r--   0        0        0     1943 2023-06-12 18:49:08.012030 torchtime-0.6.0/src/torchtime/constants.py
+-rw-r--r--   0        0        0    57401 2023-06-12 18:49:08.012030 torchtime-0.6.0/src/torchtime/data.py
+-rw-r--r--   0        0        0     4539 2023-06-12 18:49:08.012030 torchtime-0.6.0/src/torchtime/impute.py
+-rw-r--r--   0        0        0     8461 2023-06-12 18:49:08.012030 torchtime-0.6.0/src/torchtime/utils.py
+-rw-r--r--   0        0        0     9313 1970-01-01 00:00:00.000000 torchtime-0.6.0/PKG-INFO
```

### Comparing `torchtime-0.5.1/LICENSE` & `torchtime-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtime-0.5.1/README.md` & `torchtime-0.6.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -16,18 +16,28 @@
 ## Why use `torchtime`?
 
 1. Saves time. You don't have to write your own PyTorch data classes.
 2. Better research. Use common, reproducible implementations of data sets for a level playing field when evaluating models.
 
 ## Installation
 
+Install PyTorch followed by `torchtime`:
+
 ```bash
 $ pip install torchtime
 ```
 
+or
+
+```bash
+$ conda install torchtime -c conda-forge
+```
+
+There is currently no Windows build for `conda`. Feedback is welcome from `conda` users in particular.
+
 ## Getting started
 
 Data classes have a common API. The `split` argument determines whether training ("*train*"), validation ("*val*") or test ("*test*") data are returned. The size of the splits are controlled with the `train_prop` and (optional) `val_prop` arguments.
 
 ### PhysioNet data sets
 
 Three [PhysioNet](https://physionet.org/) data sets are currently supported:
```

### Comparing `torchtime-0.5.1/src/torchtime/collate.py` & `torchtime-0.6.0/src/torchtime/collate.py`

 * *Files identical despite different names*

### Comparing `torchtime-0.5.1/src/torchtime/constants.py` & `torchtime-0.6.0/src/torchtime/constants.py`

 * *Files identical despite different names*

### Comparing `torchtime-0.5.1/src/torchtime/data.py` & `torchtime-0.6.0/src/torchtime/data.py`

 * *Files identical despite different names*

### Comparing `torchtime-0.5.1/src/torchtime/impute.py` & `torchtime-0.6.0/src/torchtime/impute.py`

 * *Files identical despite different names*

### Comparing `torchtime-0.5.1/src/torchtime/utils.py` & `torchtime-0.6.0/src/torchtime/utils.py`

 * *Files identical despite different names*

### Comparing `torchtime-0.5.1/setup.py` & `torchtime-0.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,39 +1,181 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: torchtime
+Version: 0.6.0
+Summary: Benchmark time series data sets for PyTorch
+Home-page: https://philipdarke.com/torchtime
+License: MIT
+Author: Philip Darke
+Author-email: hello@philipdarke.com
+Requires-Python: >=3.8.1,<3.12
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: numpy (>=1.21,<2.0)
+Requires-Dist: requests (>=2.27.1,<3.0.0)
+Requires-Dist: scikit-learn (>=1.1,<2.0)
+Requires-Dist: sktime (>=0.17,<0.19)
+Requires-Dist: torch (==1.12.0)
+Requires-Dist: tqdm (>=4.64.0,<5.0.0)
+Project-URL: Documentation, https://philipdarke.com/torchtime
+Project-URL: Repository, https://github.com/philipdarke/torchtime
+Description-Content-Type: text/markdown
 
-package_dir = \
-{'': 'src'}
+# Benchmark time series data sets for PyTorch
 
-packages = \
-['torchtime']
+[![PyPi](https://img.shields.io/pypi/v/torchtime)](https://pypi.org/project/torchtime)
+[![Build status](https://img.shields.io/github/workflow/status/philipdarke/torchtime/build.svg)](https://github.com/philipdarke/torchtime/actions/workflows/build.yml)
+![Coverage](https://philipdarke.com/torchtime/assets/coverage-badge.svg?dummy=8484744)
+[![License](https://img.shields.io/github/license/philipdarke/torchtime.svg)](https://github.com/philipdarke/torchtime/blob/main/LICENSE)
+[![DOI](https://img.shields.io/badge/DOI-10.48550%2FarXiv.2207.12503-blue)](https://doi.org/10.48550/arXiv.2207.12503)
 
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['numpy>=1.21.0,<2.0.0',
- 'requests>=2.27.1,<3.0.0',
- 'scikit-learn>=1.1.1,<2.0.0',
- 'sktime>=0.12.1,<0.13.0',
- 'torch>=1.11.0,<2.0.0',
- 'tqdm>=4.64.0,<5.0.0']
-
-setup_kwargs = {
-    'name': 'torchtime',
-    'version': '0.5.1',
-    'description': 'Benchmark time series data sets for PyTorch',
-    'long_description': '# Benchmark time series data sets for PyTorch\n\n[![PyPi](https://img.shields.io/pypi/v/torchtime)](https://pypi.org/project/torchtime)\n[![Build status](https://img.shields.io/github/workflow/status/philipdarke/torchtime/build.svg)](https://github.com/philipdarke/torchtime/actions/workflows/build.yml)\n![Coverage](https://philipdarke.com/torchtime/assets/coverage-badge.svg?dummy=8484744)\n[![License](https://img.shields.io/github/license/philipdarke/torchtime.svg)](https://github.com/philipdarke/torchtime/blob/main/LICENSE)\n[![DOI](https://img.shields.io/badge/DOI-10.48550%2FarXiv.2207.12503-blue)](https://doi.org/10.48550/arXiv.2207.12503)\n\nPyTorch data sets for supervised time series classification and prediction problems, including:\n\n* All UEA/UCR classification repository data sets\n* PhysioNet Challenge 2012 (in-hospital mortality)\n* PhysioNet Challenge 2019 (sepsis prediction)\n* A binary prediction variant of the 2019 PhysioNet Challenge\n\n## Why use `torchtime`?\n\n1. Saves time. You don\'t have to write your own PyTorch data classes.\n2. Better research. Use common, reproducible implementations of data sets for a level playing field when evaluating models.\n\n## Installation\n\n```bash\n$ pip install torchtime\n```\n\n## Getting started\n\nData classes have a common API. The `split` argument determines whether training ("*train*"), validation ("*val*") or test ("*test*") data are returned. The size of the splits are controlled with the `train_prop` and (optional) `val_prop` arguments.\n\n### PhysioNet data sets\n\nThree [PhysioNet](https://physionet.org/) data sets are currently supported:\n\n* [`torchtime.data.PhysioNet2012`](https://philipdarke.com/torchtime/api/data.html#torchtime.data.PhysioNet2012) returns the 2012 challenge (in-hospital mortality) [[link]](https://physionet.org/content/challenge-2012/1.0.0/).\n* [`torchtime.data.PhysioNet2019`](https://philipdarke.com/torchtime/api/data.html#torchtime.data.PhysioNet2019) returns the 2019 challenge (sepsis prediction) [[link]](https://physionet.org/content/challenge-2019/1.0.0/).\n* [`torchtime.data.PhysioNet2019Binary`](https://philipdarke.com/torchtime/api/data.html#torchtime.data.PhysioNet2019Binary) returns a binary prediction variant of the 2019 challenge.\n\nFor example, to load training data for the 2012 challenge with a 70/30% training/validation split and create a [DataLoader](https://pytorch.org/docs/stable/data.html#torch.utils.data.DataLoader) for model training:\n\n```python\nfrom torch.utils.data import DataLoader\nfrom torchtime.data import PhysioNet2012\n\nphysionet2012 = PhysioNet2012(\n    split="train",\n    train_prop=0.7,\n)\ndataloader = DataLoader(physionet2012, batch_size=32)\n```\n\n### UEA/UCR repository data sets\n\nThe [`torchtime.data.UEA`](https://philipdarke.com/torchtime/api/data.html#torchtime.data.UEA) class returns the [UEA/UCR repository](https://www.timeseriesclassification.com/) data set specified by the `dataset` argument, for example:\n\n```python\nfrom torch.utils.data import DataLoader\nfrom torchtime.data import UEA\n\narrowhead = UEA(\n    dataset="ArrowHead",\n    split="train",\n    train_prop=0.7,\n)\ndataloader = DataLoader(arrowhead, batch_size=32)\n```\n\n### Using the DataLoader\n\nBatches are dictionaries of tensors `X`, `y` and `length`:\n\n* `X` are the time series data. The package follows the *batch first* convention therefore `X` has shape (*n*, *s*, *c*) where *n* is batch size, *s* is (longest) trajectory length and *c* is the number of channels. By default, the first channel is a time stamp.\n* `y` are one-hot encoded labels of shape (*n*, *l*) where *l* is the number of classes.\n* `length` are the length of each trajectory (before padding if sequences are of irregular length) i.e. a tensor of shape (*n*).\n\nFor example, ArrowHead is a univariate time series therefore `X` has two channels, the time stamp followed by the time series (*c* = 2). Each series has 251 observations (*s* = 251) and there are three classes (*l* = 3). For a batch size of 32:\n\n```python\nnext_batch = next(iter(dataloader))\nnext_batch["X"].shape       # torch.Size([32, 251, 2])\nnext_batch["y"].shape       # torch.Size([32, 3])\nnext_batch["length"].shape  # torch.Size([32])\n```\n\nSee [Using DataLoaders](https://philipdarke.com/torchtime/tutorials/getting_started.html#using-dataloaders) for more information.\n\n## Advanced options\n\n* Missing data can be imputed by setting `impute` to *mean* (replace with training data channel means) or *forward* (replace with previous observation). Alternatively a custom imputation function can be passed to the `impute` argument.\n* A time stamp (added by default), missing data mask and the time since previous observation can be appended with the boolean arguments ``time``, ``mask`` and ``delta`` respectively.\n* Time series data are standardised using the `standardise` boolean argument.\n* The location of cached data can be changed with the ``path`` argument, for example to share a single cache location across projects.\n* For reproducibility, an optional random `seed` can be specified.\n* Missing data can be simulated using the `missing` argument to drop data at random from UEA/UCR data sets.\n\nSee the [tutorials](https://philipdarke.com/torchtime/tutorials/) and [API](https://philipdarke.com/torchtime/api/) for more information.\n\n## Other resources\n\nIf you\'re looking for the TensorFlow equivalent for PhysioNet data sets try [medical_ts_datasets](https://github.com/ExpectationMax/medical_ts_datasets).\n\n## Acknowledgements\n\n`torchtime` uses some of the data processing ideas in Kidger et al, 2020 [[1]](https://arxiv.org/abs/2005.08926) and Che et al, 2018 [[2]](https://doi.org/10.1038/s41598-018-24271-9).\n\nThis work is supported by the Engineering and Physical Sciences Research Council, Centre for Doctoral Training in Cloud Computing for Big Data, Newcastle University (grant number EP/L015358/1).\n\n## Citing `torchtime`\n\nIf you use this software, please cite the [paper](https://doi.org/10.48550/arXiv.2207.12503):\n\n```\n@software{darke_torchtime_2022,\n    author = Darke, Philip and Missier, Paolo and Bacardit, Jaume,\n    title = "Benchmark time series data sets for {PyTorch} - the torchtime package",\n    month = July,\n    year = 2022,\n    publisher={arXiv},\n    doi = 10.48550/arXiv.2207.12503,\n    url = https://doi.org/10.48550/arXiv.2207.12503,\n}\n```\n\nDOIs are also available for each version of the package [here](https://doi.org/10.5281/zenodo.6402406).\n\n## References\n\n1. Kidger, P, Morrill, J, Foster, J, *et al*. Neural Controlled Differential Equations for Irregular Time Series. *arXiv* 2005.08926 (2020). [[arXiv]](https://arxiv.org/abs/2005.08926)\n\n1. Che, Z, Purushotham, S, Cho, K, *et al*. Recurrent Neural Networks for Multivariate Time Series with Missing Values. *Sci Rep* 8, 6085 (2018). [[doi]](https://doi.org/10.1038/s41598-018-24271-9)\n\n1. Silva, I, Moody, G, Scott, DJ, *et al*. Predicting In-Hospital Mortality of ICU Patients: The PhysioNet/Computing in Cardiology Challenge 2012. *Comput Cardiol* 2012;39:245-248 (2010). [[hdl]](http://hdl.handle.net/1721.1/93166)\n\n1. Reyna, M, Josef, C, Jeter, R, *et al*. Early Prediction of Sepsis From Clinical Data: The PhysioNet/Computing in Cardiology Challenge. *Critical Care Medicine* 48 2: 210-217 (2019). [[doi]](https://doi.org/10.1097/CCM.0000000000004145)\n\n1. Reyna, M, Josef, C, Jeter, R, *et al*. Early Prediction of Sepsis from Clinical Data: The PhysioNet/Computing in Cardiology Challenge 2019 (version 1.0.0). *PhysioNet* (2019). [[doi]](https://doi.org/10.13026/v64v-d857)\n\n1. Goldberger, A, Amaral, L, Glass, L, *et al*. PhysioBank, PhysioToolkit, and PhysioNet: Components of a new research resource for complex physiologic signals. *Circulation* 101 (23), pp. e215–e220 (2000). [[doi]](https://doi.org/10.1161/01.cir.101.23.e215)\n\n1. Löning, M, Bagnall, A, Ganesh, S, *et al*. sktime: A Unified Interface for Machine Learning with Time Series. *Workshop on Systems for ML at NeurIPS 2019* (2019). [[doi]](https://doi.org/10.5281/zenodo.3970852)\n\n1. Löning, M, Bagnall, A, Middlehurst, M, *et al*. alan-turing-institute/sktime: v0.10.1 (v0.10.1). *Zenodo* (2022). [[doi]](https://doi.org/10.5281/zenodo.6191159)\n\n## License\n\nReleased under the MIT license.\n',
-    'author': 'Philip Darke',
-    'author_email': 'hello@philipdarke.com',
-    'maintainer': None,
-    'maintainer_email': None,
-    'url': 'https://philipdarke.com/torchtime',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.10',
+PyTorch data sets for supervised time series classification and prediction problems, including:
+
+* All UEA/UCR classification repository data sets
+* PhysioNet Challenge 2012 (in-hospital mortality)
+* PhysioNet Challenge 2019 (sepsis prediction)
+* A binary prediction variant of the 2019 PhysioNet Challenge
+
+## Why use `torchtime`?
+
+1. Saves time. You don't have to write your own PyTorch data classes.
+2. Better research. Use common, reproducible implementations of data sets for a level playing field when evaluating models.
+
+## Installation
+
+Install PyTorch followed by `torchtime`:
+
+```bash
+$ pip install torchtime
+```
+
+or
+
+```bash
+$ conda install torchtime -c conda-forge
+```
+
+There is currently no Windows build for `conda`. Feedback is welcome from `conda` users in particular.
+
+## Getting started
+
+Data classes have a common API. The `split` argument determines whether training ("*train*"), validation ("*val*") or test ("*test*") data are returned. The size of the splits are controlled with the `train_prop` and (optional) `val_prop` arguments.
+
+### PhysioNet data sets
+
+Three [PhysioNet](https://physionet.org/) data sets are currently supported:
+
+* [`torchtime.data.PhysioNet2012`](https://philipdarke.com/torchtime/api/data.html#torchtime.data.PhysioNet2012) returns the 2012 challenge (in-hospital mortality) [[link]](https://physionet.org/content/challenge-2012/1.0.0/).
+* [`torchtime.data.PhysioNet2019`](https://philipdarke.com/torchtime/api/data.html#torchtime.data.PhysioNet2019) returns the 2019 challenge (sepsis prediction) [[link]](https://physionet.org/content/challenge-2019/1.0.0/).
+* [`torchtime.data.PhysioNet2019Binary`](https://philipdarke.com/torchtime/api/data.html#torchtime.data.PhysioNet2019Binary) returns a binary prediction variant of the 2019 challenge.
+
+For example, to load training data for the 2012 challenge with a 70/30% training/validation split and create a [DataLoader](https://pytorch.org/docs/stable/data.html#torch.utils.data.DataLoader) for model training:
+
+```python
+from torch.utils.data import DataLoader
+from torchtime.data import PhysioNet2012
+
+physionet2012 = PhysioNet2012(
+    split="train",
+    train_prop=0.7,
+)
+dataloader = DataLoader(physionet2012, batch_size=32)
+```
+
+### UEA/UCR repository data sets
+
+The [`torchtime.data.UEA`](https://philipdarke.com/torchtime/api/data.html#torchtime.data.UEA) class returns the [UEA/UCR repository](https://www.timeseriesclassification.com/) data set specified by the `dataset` argument, for example:
+
+```python
+from torch.utils.data import DataLoader
+from torchtime.data import UEA
+
+arrowhead = UEA(
+    dataset="ArrowHead",
+    split="train",
+    train_prop=0.7,
+)
+dataloader = DataLoader(arrowhead, batch_size=32)
+```
+
+### Using the DataLoader
+
+Batches are dictionaries of tensors `X`, `y` and `length`:
+
+* `X` are the time series data. The package follows the *batch first* convention therefore `X` has shape (*n*, *s*, *c*) where *n* is batch size, *s* is (longest) trajectory length and *c* is the number of channels. By default, the first channel is a time stamp.
+* `y` are one-hot encoded labels of shape (*n*, *l*) where *l* is the number of classes.
+* `length` are the length of each trajectory (before padding if sequences are of irregular length) i.e. a tensor of shape (*n*).
+
+For example, ArrowHead is a univariate time series therefore `X` has two channels, the time stamp followed by the time series (*c* = 2). Each series has 251 observations (*s* = 251) and there are three classes (*l* = 3). For a batch size of 32:
+
+```python
+next_batch = next(iter(dataloader))
+next_batch["X"].shape       # torch.Size([32, 251, 2])
+next_batch["y"].shape       # torch.Size([32, 3])
+next_batch["length"].shape  # torch.Size([32])
+```
+
+See [Using DataLoaders](https://philipdarke.com/torchtime/tutorials/getting_started.html#using-dataloaders) for more information.
+
+## Advanced options
+
+* Missing data can be imputed by setting `impute` to *mean* (replace with training data channel means) or *forward* (replace with previous observation). Alternatively a custom imputation function can be passed to the `impute` argument.
+* A time stamp (added by default), missing data mask and the time since previous observation can be appended with the boolean arguments ``time``, ``mask`` and ``delta`` respectively.
+* Time series data are standardised using the `standardise` boolean argument.
+* The location of cached data can be changed with the ``path`` argument, for example to share a single cache location across projects.
+* For reproducibility, an optional random `seed` can be specified.
+* Missing data can be simulated using the `missing` argument to drop data at random from UEA/UCR data sets.
+
+See the [tutorials](https://philipdarke.com/torchtime/tutorials/) and [API](https://philipdarke.com/torchtime/api/) for more information.
+
+## Other resources
+
+If you're looking for the TensorFlow equivalent for PhysioNet data sets try [medical_ts_datasets](https://github.com/ExpectationMax/medical_ts_datasets).
+
+## Acknowledgements
+
+`torchtime` uses some of the data processing ideas in Kidger et al, 2020 [[1]](https://arxiv.org/abs/2005.08926) and Che et al, 2018 [[2]](https://doi.org/10.1038/s41598-018-24271-9).
+
+This work is supported by the Engineering and Physical Sciences Research Council, Centre for Doctoral Training in Cloud Computing for Big Data, Newcastle University (grant number EP/L015358/1).
+
+## Citing `torchtime`
+
+If you use this software, please cite the [paper](https://doi.org/10.48550/arXiv.2207.12503):
+
+```
+@software{darke_torchtime_2022,
+    author = Darke, Philip and Missier, Paolo and Bacardit, Jaume,
+    title = "Benchmark time series data sets for {PyTorch} - the torchtime package",
+    month = July,
+    year = 2022,
+    publisher={arXiv},
+    doi = 10.48550/arXiv.2207.12503,
+    url = https://doi.org/10.48550/arXiv.2207.12503,
 }
+```
+
+DOIs are also available for each version of the package [here](https://doi.org/10.5281/zenodo.6402406).
+
+## References
+
+1. Kidger, P, Morrill, J, Foster, J, *et al*. Neural Controlled Differential Equations for Irregular Time Series. *arXiv* 2005.08926 (2020). [[arXiv]](https://arxiv.org/abs/2005.08926)
+
+1. Che, Z, Purushotham, S, Cho, K, *et al*. Recurrent Neural Networks for Multivariate Time Series with Missing Values. *Sci Rep* 8, 6085 (2018). [[doi]](https://doi.org/10.1038/s41598-018-24271-9)
+
+1. Silva, I, Moody, G, Scott, DJ, *et al*. Predicting In-Hospital Mortality of ICU Patients: The PhysioNet/Computing in Cardiology Challenge 2012. *Comput Cardiol* 2012;39:245-248 (2010). [[hdl]](http://hdl.handle.net/1721.1/93166)
+
+1. Reyna, M, Josef, C, Jeter, R, *et al*. Early Prediction of Sepsis From Clinical Data: The PhysioNet/Computing in Cardiology Challenge. *Critical Care Medicine* 48 2: 210-217 (2019). [[doi]](https://doi.org/10.1097/CCM.0000000000004145)
+
+1. Reyna, M, Josef, C, Jeter, R, *et al*. Early Prediction of Sepsis from Clinical Data: The PhysioNet/Computing in Cardiology Challenge 2019 (version 1.0.0). *PhysioNet* (2019). [[doi]](https://doi.org/10.13026/v64v-d857)
+
+1. Goldberger, A, Amaral, L, Glass, L, *et al*. PhysioBank, PhysioToolkit, and PhysioNet: Components of a new research resource for complex physiologic signals. *Circulation* 101 (23), pp. e215–e220 (2000). [[doi]](https://doi.org/10.1161/01.cir.101.23.e215)
+
+1. Löning, M, Bagnall, A, Ganesh, S, *et al*. sktime: A Unified Interface for Machine Learning with Time Series. *Workshop on Systems for ML at NeurIPS 2019* (2019). [[doi]](https://doi.org/10.5281/zenodo.3970852)
+
+1. Löning, M, Bagnall, A, Middlehurst, M, *et al*. alan-turing-institute/sktime: v0.10.1 (v0.10.1). *Zenodo* (2022). [[doi]](https://doi.org/10.5281/zenodo.6191159)
+
+## License
 
+Released under the MIT license.
 
-setup(**setup_kwargs)
```

