# Comparing `tmp/foundation_cancer_image_biomarker-0.0.1a3.tar.gz` & `tmp/foundation_cancer_image_biomarker-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation_cancer_image_biomarker-0.0.1a3.tar", max compression
+gzip compressed data, was "foundation_cancer_image_biomarker-0.0.1a4.tar", max compression
```

## Comparing `foundation_cancer_image_biomarker-0.0.1a3.tar` & `foundation_cancer_image_biomarker-0.0.1a4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1076 2023-06-04 18:03:55.694363 foundation_cancer_image_biomarker-0.0.1a3/LICENSE
--rw-r--r--   0        0        0    27254 2023-06-09 09:53:08.816608 foundation_cancer_image_biomarker-0.0.1a3/README.md
--rw-r--r--   0        0        0       23 2023-06-09 09:55:32.943580 foundation_cancer_image_biomarker-0.0.1a3/fmcib/__init__.py
--rw-r--r--   0        0        0       45 2023-06-09 08:53:45.238232 foundation_cancer_image_biomarker-0.0.1a3/fmcib/callbacks/__init__.py
--rw-r--r--   0        0        0     2188 2023-06-09 07:25:30.580753 foundation_cancer_image_biomarker-0.0.1a3/fmcib/callbacks/prediction_saver.py
--rw-r--r--   0        0        0      403 2023-06-09 07:24:26.381203 foundation_cancer_image_biomarker-0.0.1a3/fmcib/callbacks/utils.py
--rw-r--r--   0        0        0       54 2023-06-09 09:10:44.118566 foundation_cancer_image_biomarker-0.0.1a3/fmcib/datasets/__init__.py
--rw-r--r--   0        0        0     5353 2023-06-09 05:43:21.136415 foundation_cancer_image_biomarker-0.0.1a3/fmcib/datasets/ssl_radiomics_dataset.py
--rw-r--r--   0        0        0     2365 2023-06-08 04:18:19.159890 foundation_cancer_image_biomarker-0.0.1a3/fmcib/datasets/utils.py
--rw-r--r--   0        0        0       31 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a3/fmcib/models/__init__.py
--rw-r--r--   0        0        0      767 2023-06-09 06:28:56.871613 foundation_cancer_image_biomarker-0.0.1a3/fmcib/models/resnet50.py
--rw-r--r--   0        0        0     1437 2023-06-06 01:43:30.521334 foundation_cancer_image_biomarker-0.0.1a3/fmcib/preprocessing/__init__.py
--rw-r--r--   0        0        0     4283 2023-06-06 01:43:30.549334 foundation_cancer_image_biomarker-0.0.1a3/fmcib/preprocessing/seed_based_crop.py
--rw-r--r--   0        0        0      943 2023-06-06 01:43:30.505334 foundation_cancer_image_biomarker-0.0.1a3/fmcib/run.py
--rw-r--r--   0        0        0        0 2023-06-08 02:44:13.386481 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/__init__.py
--rw-r--r--   0        0        0       54 2023-06-08 02:48:18.036638 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/losses/__init__.py
--rw-r--r--   0        0        0     3348 2023-06-08 02:44:38.830290 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/losses/ntxent_mined_loss.py
--rw-r--r--   0        0        0       96 2023-06-08 05:19:10.855520 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/models/__init__.py
--rw-r--r--   0        0        0      671 2023-06-08 02:45:52.657736 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/models/exneg_simclr.py
--rw-r--r--   0        0        0     2074 2023-06-09 09:04:10.961477 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/models/load_pretrained_resnet.py
--rw-r--r--   0        0        0       22 2023-06-08 02:45:31.477895 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/optimizers/__init__.py
--rw-r--r--   0        0        0     5397 2023-06-08 02:45:31.565894 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/optimizers/lars.py
--rw-r--r--   0        0        0       85 2023-06-08 04:47:26.794430 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/transforms/__init__.py
--rw-r--r--   0        0        0     1414 2023-06-08 04:47:13.370533 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/transforms/duplicate.py
--rw-r--r--   0        0        0     1313 2023-06-08 04:44:35.583740 foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/transforms/random_resized_crop.py
--rw-r--r--   0        0        0       67 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a3/fmcib/utils/__init__.py
--rw-r--r--   0        0        0      367 2023-06-06 01:43:30.485334 foundation_cancer_image_biomarker-0.0.1a3/fmcib/utils/download_utils.py
--rw-r--r--   0        0        0     3419 2023-06-09 09:21:27.165850 foundation_cancer_image_biomarker-0.0.1a3/fmcib/utils/idc_helper.py
--rw-r--r--   0        0        0       44 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a3/fmcib/visualization/__init__.py
--rw-r--r--   0        0        0      499 2023-06-06 01:41:36.682184 foundation_cancer_image_biomarker-0.0.1a3/fmcib/visualization/verify_io.py
--rw-r--r--   0        0        0     4201 2023-06-09 09:55:32.875581 foundation_cancer_image_biomarker-0.0.1a3/pyproject.toml
--rw-r--r--   0        0        0    28631 1970-01-01 00:00:00.000000 foundation_cancer_image_biomarker-0.0.1a3/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-04 18:03:55.694363 foundation_cancer_image_biomarker-0.0.1a4/LICENSE
+-rw-r--r--   0        0        0    28582 2023-06-12 21:55:26.988316 foundation_cancer_image_biomarker-0.0.1a4/README.md
+-rw-r--r--   0        0        0       24 2023-06-13 02:05:01.956824 foundation_cancer_image_biomarker-0.0.1a4/fmcib/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-13 02:03:39.397472 foundation_cancer_image_biomarker-0.0.1a4/fmcib/callbacks/__init__.py
+-rw-r--r--   0        0        0     2159 2023-06-13 02:03:53.085364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/callbacks/prediction_saver.py
+-rw-r--r--   0        0        0      406 2023-06-13 02:03:53.089364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/callbacks/utils.py
+-rw-r--r--   0        0        0      619 2023-06-13 02:03:53.093364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/datasets/__init__.py
+-rw-r--r--   0        0        0     5184 2023-06-13 02:03:53.093364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/datasets/ssl_radiomics_dataset.py
+-rw-r--r--   0        0        0     2151 2023-06-13 02:03:53.097364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/datasets/utils.py
+-rw-r--r--   0        0        0      257 2023-06-13 02:03:53.033365 foundation_cancer_image_biomarker-0.0.1a4/fmcib/models/__init__.py
+-rw-r--r--   0        0        0      767 2023-06-09 10:06:02.963848 foundation_cancer_image_biomarker-0.0.1a4/fmcib/models/resnet50.py
+-rw-r--r--   0        0        0     1437 2023-06-13 01:00:24.547870 foundation_cancer_image_biomarker-0.0.1a4/fmcib/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4283 2023-06-06 01:43:30.549334 foundation_cancer_image_biomarker-0.0.1a4/fmcib/preprocessing/seed_based_crop.py
+-rw-r--r--   0        0        0      943 2023-06-13 01:00:06.900032 foundation_cancer_image_biomarker-0.0.1a4/fmcib/run.py
+-rw-r--r--   0        0        0        0 2023-06-08 02:44:13.386481 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/__init__.py
+-rw-r--r--   0        0        0       55 2023-06-13 02:03:39.437472 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/losses/__init__.py
+-rw-r--r--   0        0        0     3259 2023-06-13 02:03:53.061365 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/losses/ntxent_mined_loss.py
+-rw-r--r--   0        0        0       97 2023-06-13 02:03:39.437472 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/models/__init__.py
+-rw-r--r--   0        0        0      656 2023-06-13 02:03:53.041365 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/models/exneg_simclr.py
+-rw-r--r--   0        0        0     2212 2023-06-13 02:03:53.045365 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/models/load_pretrained_resnet.py
+-rw-r--r--   0        0        0       23 2023-06-13 02:03:39.453472 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/optimizers/__init__.py
+-rw-r--r--   0        0        0     5399 2023-06-13 02:03:39.525471 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/optimizers/lars.py
+-rw-r--r--   0        0        0       86 2023-06-13 02:03:53.065364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/transforms/__init__.py
+-rw-r--r--   0        0        0     1376 2023-06-13 02:03:53.065364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/transforms/duplicate.py
+-rw-r--r--   0        0        0     1301 2023-06-13 02:03:53.069364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/transforms/random_resized_crop.py
+-rw-r--r--   0        0        0       67 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a4/fmcib/utils/__init__.py
+-rw-r--r--   0        0        0      367 2023-06-13 02:03:39.465471 foundation_cancer_image_biomarker-0.0.1a4/fmcib/utils/download_utils.py
+-rw-r--r--   0        0        0     5378 2023-06-13 02:03:53.105364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/utils/idc_helper.py
+-rw-r--r--   0        0        0       44 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a4/fmcib/visualization/__init__.py
+-rw-r--r--   0        0        0      499 2023-06-06 01:41:36.682184 foundation_cancer_image_biomarker-0.0.1a4/fmcib/visualization/verify_io.py
+-rw-r--r--   0        0        0     4201 2023-06-13 02:05:01.888824 foundation_cancer_image_biomarker-0.0.1a4/pyproject.toml
+-rw-r--r--   0        0        0    29959 1970-01-01 00:00:00.000000 foundation_cancer_image_biomarker-0.0.1a4/PKG-INFO
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/LICENSE` & `foundation_cancer_image_biomarker-0.0.1a4/LICENSE`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/README.md` & `foundation_cancer_image_biomarker-0.0.1a4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -11,22 +11,24 @@
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/releases)
 [![License](https://img.shields.io/github/license/foundation_image_biomarker/foundation-image-biomarker)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/blob/master/LICENSE)
 ![Coverage Report](assets/images/coverage.svg)
 
 </div> -->
 
-## Overview
 This is the the official repository for the paper <i> Foundation Models for Quantitative Biomarker Discovery for Cancer Imaging </i> <br/>
 Suraj Pai, Dennis Bontempi, Vasco Prudente, Ibrahim Hadzic, Mateo Sokač, Tafadzwa L. Chaunzwa, Simon Bernatz, Ahmed Hosny, Raymond H Mak, Nicolai J Birkbak, Hugo JWL Aerts
 
-<div style="display: flex; justify-content: center"><img src="assets/images/overview_v5.png" width=550 /></div>
+&emsp;
+## Overview
+<div style="display: flex; justify-content: center"><img src="assets/images/overview_v5.png" width=600 /></div>
 
- <b>General overview of the study.</b><b> a. Foundation model pre-training.</b> A foundation model, specifically a deep convolutional encoder model, was pre-trained by contrasting volumes with and without lesions. <b> b. </b> Clinical application of the foundation model. The foundation model was used to extract biomarkers and then evaluated for three classification tasks on diverse datasets. <b>c. Foundation model implementation approaches </b>  The foundation model was adapted to specific use cases by extracting features or through fine-tuning (left). <b> d. Evaluation against supervised models with selected performance metrics. </b> We compared the performance of the foundation models against conventional supervised implementations, trained from scratch (left) and fine-tuned from a different task (right). The comparison was made through several criteria for the different use cases, including quantitative performance, stability, and biological analysis. Biological, clinical, and stability analyses are limited to use case 2 due to the availability of associated data. 
+ <b>General overview of the study.</b><b> a. Foundation model pre-training.</b> A foundation model, specifically a deep convolutional encoder model, was pre-trained by contrasting volumes with and without lesions. <b> b.  Clinical application of the foundation model.</b> The foundation model was used to extract biomarkers and then evaluated for three classification tasks on diverse datasets. <b>c. Foundation model implementation approaches </b>  The foundation model was adapted to specific use cases by extracting features or through fine-tuning (left). <b> d. Evaluation against supervised models with selected performance metrics. </b> We compared the performance of the foundation models against conventional supervised implementations, trained from scratch (left) and fine-tuned from a different task (right). The comparison was made through several criteria for the different use cases, including quantitative performance, stability, and biological analysis. Biological, clinical, and stability analyses are limited to use case 2 due to the availability of associated data. 
 
+&emsp;
 ## Table of Contents
 
 - [Repository Structure](#repository-structure)
 - [Quick Start](#quick-start)
 - [Data](#data)
   - [Downloading the datasets](#downloading-the-datasets)
   - [Preprocessing the datasets](#preprocessing-the-datasets)
@@ -44,31 +46,34 @@
   - [Predictions pipeline](#predictions-pipeline)
 - [Analysis](#analysis)
 - [License](#🛡-license)
 - [Acknowledgement](#acknowledgements)
 - [Disclaimer](#disclaimer)
 - [Code Citation](#📃-code-citation)
 
+<div style="page-break-after: always;"></div>
+
 ## Repository Structure
 
-This code repository includes the Python package `fmcib`, as well as the code to reproduce experiments and analyses presented in our paper.
+This code repository includes the Python package containing all our source code: `fmcib`, as well as the code to reproduce experiments and analyses presented in our paper. The pipelines to reproduce our experiments and analyses are independent of the python package and will be shared to the public upon publication.
 
 Here is the structure of the repository:
 
 ```
 ├── fmcib/          # The main Python package
 ├── data/           # Downloading and preprocessing data
 ├── experiments/    # Reproduce paper experiments
 ├── models/         # Download and test final models
 ├── outputs/        # Outputs from pipelines in the study
 ├── analysis/       # Reproducible analysis for statistics
 ├── additional_requirements.txt
 └── README.pdf
 ```
 
+&emsp;
 ## Quick Start
 
 We recommend using **Python 3.8** on a Linux machine since that is the environment we have tested on. However, the use of Poetry for managing dependencies should make it compatible with Python versions above 3.8 on all platforms. We suggest using Conda to create an isolated virtual environment for the project dependencies. To download Conda, follow the instructions here: https://conda.io/projects/conda/en/latest/user-guide/install/index.html
 
 After downloading and activating Conda, create and activate a virtual environment with the following commands:
 
 ```python
@@ -91,16 +96,16 @@
 ```
 
 You can verify if the dependencies are installed by: 
 ```bash
 python -c "import fmcib; print(fmcib.__version__)"
 ```
 
-This should work without error and show you a version string as the results. Once completed, you can run each of the provided pipelines to reproduce experiments and analyses. These pipelines are not part of the Python package (which mostly contains code to load models and ssl training specific code) and will be shared publicly upon publication.
 
+<div style="page-break-after: always;"></div>
 
 ## Data
 The majority of the datasets utilized in this study are openly accessible for both training and validation purposes: 
 1.  DeepLesion (https://nihcc.app.box.com/v/DeepLesion/): DeepLesion is a dataset comprising 32,735 lesions from 10,594 studies of 4,427 unique patients collected over two decades from the National Institute of Health Clinical Center PACS server. Various lesions, including kidney, bone, and liver lesions - as well as enlarged lymph nodes and lung nodules, are annotated. The lesions are identified through radiologist-bookmarked RECIST diameters across 32,120 CT slice . In our study we use this dataset both for our pre-training and use-case 1 
 
 
 2.  LUNA16 (https://luna16.grand-challenge.org/Data/): LUNA16 is a curated version of the LIDC-IDRI dataset of 888 diagnostic and lung cancer screening thoracic CT scans obtained from seven academic centers and eight medical imaging companies comprising 1,186 nodules. The nodules are accompanied by annotations agreed upon by at least 3 out of 4 radiologists. Alongside nodule location annotations, radiologists also noted various observed attributes like internal composition, calcification, malignancy, suspiciousness, and more. We use this dataset to develop and validate our diagnostic image biomarker
@@ -124,15 +129,14 @@
 
 For DeepLesion,
 ```
 cd data/download
 bash deeplesion.sh <path_to_download>
 ```
 
-
 For LUNA16,
 ```
 cd data/download
 bash luna16.sh <path_to_download>
 ```
 <b> Downloading the LUNG1 and RADIO datasets </b>
 Refer to [Google colab notebook](https://colab.research.google.com/drive/1Svk8VaZHWAYdZHE45DNdWXVqhe7v9sFR#scrollTo=okx0n73EI11u) that contains information on how this data can be downloaded and pre-processed.
@@ -140,30 +144,36 @@
 ### Preprocessing the datasets
 We provide simple linux shell scripts to reproduce the pre-processing pipeline. Incase, you have a different operating system, simply run the python scripts in these shell scripts individually in your environment.
 
 <b> Pre-processing the DeepLesion dataset </b>
 Note: Conda is required to perform this
 ```
 cd data/preprocessing/deeplesion
-bash run.sh
+bash run.sh <path_to_download>
 ```
 
 Once you run this successfully, you should see a file `data/processing/deeplesion/annotations/deeplesion_training_annotations.csv`. At this point you can run the notebook `data/processing/deeplesion/Process_Dataset.ipynb` to get the splits we use in our paper. For reference, we have already provided splits for comparison as generated by us.
 
+NOTE: The pre-processing extracts the image files from zip files. Please delete the zip files from the path `<path_to_download>/DeepLesion/Images_png` using `rm <path_to_download>/DeepLesion/Images_png/*.zip`  path after these scripts are successfully run to not inflate your disk space.
+
+
 <b> Pre-processing the LUNA16 dataset </b>
 ```
 cd data/preprocessing/luna16
-bash run.sh
+bash run.sh <path_to_download>
 ```
 
+NOTE: The pre-processing extracts the image files from zip files. Please delete the zip files from the path `<path_to_download>/LUNA16` using `rm <path_to_download>/LUNA16/*.zip` after these scripts are successfully run to not inflate your disk space.
+
 Once you run this successfully, you should see a file `data/processing/deeplesion/annotations/luna16_training_annotations.csv`. At this point you can run the notebook `data/processing/deeplesion/Process_Dataset.ipynb` to get the splits we use in our paper. For reference, we have already provided splits for comparison as generated by us.
 
 <b> Pre-processing the LUNG1 and RADIO dataset </b>
-Refer to [our Google Colab reprocible notebooks](https://colab.research.google.com/drive/1Svk8VaZHWAYdZHE45DNdWXVqhe7v9sFR#scrollTo=okx0n73EI11u) that also contains information on how this data can be downloaded and pre-processed
+Refer to [our Google Colab reproducible notebooks](https://colab.research.google.com/drive/1Svk8VaZHWAYdZHE45DNdWXVqhe7v9sFR#scrollTo=okx0n73EI11u) that also contains information on how this data can be accessed
 
+<div style="page-break-after: always;"></div>
 
 ## Model
 All our models are will be made available to the public through Zenodo upon publication. Currently, we release these using Dropbox for the reviewers to use and test. Scripts for downloading these models are present under `models`. 
 
 As part of our study we develop and share the following,
 
 ### Self-supervised pre-training model:
@@ -182,42 +192,47 @@
 
 The pre-trained model is implemented on downstreams task using supervised training or linear evaluation approaches. For these we develop,
 
 ### Supervised models:
 
 We developed three supervised training approaches,
  - Supervised model trained from random initialization
+<br>
+<div style="display: flex; justify-content: center"><img src="assets/images/implementation1.png" width=400 /></div>
+
 
  - Fine-tuning a trained supervised model
+<br>
+<div style="display: flex; justify-content: center"><img src="assets/images/implementation2.png" width=400 /></div>
 
  - Fine-tuning a pre-trained foundation model
+<br>
+<div style="display: flex; justify-content: center"><img src="assets/images/implementation3.png" width=400 /></div>
 
 
-<br>
-<div style="display: flex; justify-content: center"><img src="assets/images/supervised_models.png" width=400 /></div>
 
 To download these models run,
 ````bash
 cd models
 bash download_supervised_models.sh
 ````
 
 
 ### Linear (Logistic Regression) models:
 Our linear model takes features extracted from the pre-trained foundation model and builds a logistic regression classifer to predict outcome. 
 <div style="display: flex; justify-content: center"><img src="assets/images/linear_model.png" width=400 /></div>
 
+&emsp;
 To download these models run,
 ````bash
 cd models
 bash download_linear_models.sh
 ````
 
-These models can also be found at this [link](https://www.dropbox.com/scl/fo/brhqokhzn839zez15erzf/h?dl=0&rlkey=wzvgrobl8p3v49ettm16uxbyy)
-In addition to providing our models, we also provide comprehensive documentation and ongoing support to users through [project-lighter](https://zenodo.org/record/8007711) to reproduce our results and workflows.
+These models can also be found at this [link](https://www.dropbox.com/scl/fo/brhqokhzn839zez15erzf/h?dl=0&rlkey=wzvgrobl8p3v49ettm16uxbyy). In addition to providing our models, we also provide comprehensive documentation and ongoing support to users through [project-lighter](https://zenodo.org/record/8007711) to reproduce our results and workflows.
 
 
 ### Data setup for the models
 Make sure you download all the datasets before starting to train. The datasets are provided as CSV files to the training pipelines with `image_path` column providing location of the image to be used, `coordX`, `coordY` and `coordZ` providing the global coordinates of the seed point around which a patch is cropped. We crop a [50, 50, 50] patch around the seed point. Please refer to our paper for more details on this. Along with these columns, label columns are needed for supervised training. Labels for each task are as follows,
 ```
 Task 1: Coarse_lesion_type
 Task 2: malignancy
@@ -252,14 +267,16 @@
 ```yaml
 train_dataset:
   _target_: fmcib.ssl.datasets.SSLRadiomicsDataset
   path: "your_pretrain_set_path_goes_here"
 ```
 
 Now you can start training by running this in the root code folder,
+
+
 ```bash
 lighter fit --config_file ./experiments/pretraining/simclr_pretrain.yaml
 ```
 
 
 ### Reproducing our supervised training
 As mentioned in [section](#supervised-models), we have three different supervised training implementations. Similar to the foundation pre-training, we use YAML files to maintain the configurations of these implementations. 
@@ -273,14 +290,15 @@
 lighter fit --config_file ./experiments/supervised_training/supervised_random_init.yaml
 ```
 
 <b> Fine-tuning a trained supervised model </b>
 
 The YAML configuration at `experiments/supervised_training/supervised_finetune.yaml` describes how you can fine-tune an already trained supervised model. Note that this is possible only for Task 2 and Task 3 as we used the supervised model trained in Task 1 to load weights from. Make sure you download the weights for Task 1 supervised models. You can follow instructions [here](#model) 
 
+
 You can start training by running this in the root code folder,
 ```bash
 lighter fit --config_file ./experiments/supervised_training/supervised_finetune.yaml
 ```
 
 <b> Fine-tuning a pre-trained foundation model </b>
 
@@ -322,16 +340,27 @@
 
 The <label> corresponds to the column in the csv files that contains the supervised label to predict. For example, in use-case 2 the label is `malignancy`. 
 
 You can also provide scoring metrics, for instance,  using `--scoring roc_auc` where the scoring metric is a sklearn scorer. You can also provide the number of trials the optimization framework needs to be run for using `--trials`. 
 
 The features folder is provided under `outputs/foundation_features` to try our the modelling process. Refer [here](#feature-extaction-pipeline)
 
+<div style="page-break-after: always;"></div>
+
 ## Outputs
-The `outputs` folder contains outputs from several pipelines used in our study. 
+The `outputs` folder contains outputs from several pipelines used in our study. To download all the outputs, you can run
+
+
+```bash
+cd outputs
+bash download_outputs.sh
+```
+
+
+The script contains several dropbox links. You can also manually download them and place them in the right location. 
 
 ### Feature extaction pipeline
 The `foundation_features` folders contains features extracted from the pre-trained foundation model for Task 1, 2 and 3. The features are stored in `csv` files with column names `feature_x` corresponding to the dimension `x` of the feature. The total dimensionality of the features is 4096. Below is the structure of the folder,
 ```bash
 outputs
 └── foundation_features
     └── task1
@@ -365,52 +394,57 @@
         └── RADIO
             └── *.csv 
 ```
 For Task 1 and Task 2, we store predictions extracted over a range of different percentages of data used during the model training process (100%, 50%, 20%, and 10%). Predictions are saved for each of the implementation approaches. To differentiate between the predictions based on limited data percentages, we have appended a suffix `_x_percent.cs`, where 'x' represents the data percentage used
 
 For Task 3, we provide predictions for each of the different implementation approaches when tested on the LUNG1 and RADIO datasets. Validation predictions of the HarvardRT for computing Kaplan Meier curves as presented in [analysis](#analysis) notebooks are also provided.
 
+<div style="page-break-after: always;"></div>
+
 ## Analysis
 To support complete transparency of our work and allow you to have a better understanding of our analysis pipelines, the provided notebooks, with detailed walk-throughs, will help explore our analysis as well as reproduce the figures that are included in our research paper. The predictions extracted are described [here](#predictions-extracted).
 
 The analysis notebooks are organized as follows,
 
 ```bash
 analysis
 └── task1.ipynb
 └── task2.ipynb
 └── task3.ipynb
 └── stability.ipynb
 ```
 
-Detailed walk-throughs are provided in the notebooks. These notebooks reproduce Figures 2, 3, 4 and Extended Data Figure 3. Please ensure you download additional dependenices as described in the [quickstart](#quick-start)
+Detailed walk-throughs are provided in the notebooks. These notebooks reproduce Figures 2, 3, 4 and Extended Data Figure 3. Please ensure you download additional dependenices as described in the [quickstart](#quick-start) and that you have downloaded all the outputs from our pipelines.
 
 Shown below are samples from the analysis notebooks
 <div style="display: flex; justify-content: center"><img src="assets/analysis_1.png" width=300 /><img src="assets/analysis_2.png" width=200 /></div>
 
 <div style="display: flex; justify-content: center"><img src="assets/analysis_3.png" width=300 /><img src="assets/analysis_4.png" width=300 /></div>
 
-## 🛡 License
+<div style="page-break-after: always;"></div>
 
-This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/AIM-Harvard/foundation-cancer-image-biomarker/blob/master/LICENSE) for more details.
+&emsp;
+## License
 
+This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/AIM-Harvard/foundation-cancer-image-biomarker/blob/master/LICENSE) for more details.
 
+&emsp;
 ## Acknowledgements
 Code development, testing, and documentation: Suraj Pai
 Framework used for building the code: project-lighter (https://github.com/project-lighter/lighter)
 
+project-lighter was developed internally within our lab by Ibrahim Hadzic and Suraj Pai. 
+
+&emsp;
 ## Disclaimer
 The code and data of this repository are provided to promote reproducible research. They are not intended for clinical care or
-commercial use.
-The software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of
-merchantability, fitness for a particular purpose and noninfringement. In no event shall the authors or copyright holders be liable
-for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection
-with the software or the use or other dealings in the software.
+commercial use. The software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software or the use or other dealings in the software.
 
-## 📃 Code Citation
+&emsp;
+## Code Citation
 Will be updated to reflect a Zenodo DOI upon publication
 ```bibtex
 @misc{foundation-cancer-image-biomarker,
   author = {AIM-Harvard},
   title = {Official repo for "Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging"},
   year = {2023},
   publisher = {GitHub},
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/fmcib/callbacks/prediction_saver.py` & `foundation_cancer_image_biomarker-0.0.1a4/fmcib/callbacks/prediction_saver.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,52 +1,53 @@
-from pytorch_lightning.callbacks import BasePredictionWriter
+from typing import Any, List
+
+from pathlib import Path
+
+import pandas as pd
 import torchvision
 from loguru import logger
+from pytorch_lightning.callbacks import BasePredictionWriter
+
 from .utils import decollate
-import pandas as pd
-from pathlib import Path
-from typing import List, Any
+
 
 def handle_image(image):
     image = image.squeeze()
     if image.dim() == 3:
-        return image[image.shape[0]//2]
+        return image[image.shape[0] // 2]
     else:
         return image
 
+
 class SavePredictions(BasePredictionWriter):
     def __init__(self, path: str, save_preview: bool = False):
         super().__init__("epoch")
         self.output_csv = Path(path)
         self.save_preview = save_preview
         self.output_csv.parent.mkdir(parents=True, exist_ok=True)
         self.df = pd.DataFrame()
 
-
     def save_previews(self, dataset):
         logger.info("Saving image previews")
         self.output_dir = self.output_csv.parent / "previews"
         self.output_dir.mkdir(parents=True, exist_ok=True)
         for idx, data_item in enumerate(iter(dataset)):
             image, _ = data_item
             image = handle_image(image)
             fp = self.output_dir / f"{idx}.png"
             torchvision.utils.save_image(image, fp)
 
-    def write_on_epoch_end(
-        self, trainer, pl_module: 'LightningModule', predictions: List[Any], batch_indices: List[Any]
-    ):
+    def write_on_epoch_end(self, trainer, pl_module: "LightningModule", predictions: List[Any], batch_indices: List[Any]):
         assert getattr(pl_module, "predict_dataset"), "`predict_dataset` not defined"
         dataset = pl_module.predict_dataset
 
         if self.save_preview:
             self.save_previews(dataset)
 
-        assert getattr(dataset, "get_rows"), \
-            "The dataset must have `get_image_paths` defined for predict functionality"
+        assert getattr(dataset, "get_rows"), "The dataset must have `get_image_paths` defined for predict functionality"
         rows = dataset.get_rows()
 
         out = decollate(predictions)
         assert len(out) == len(rows), "Length of image_paths and predictions do not match"
 
         for pred, row in zip(out, rows):
             # Handle multiple output cases (features and multi-class)
@@ -54,9 +55,9 @@
                 for idx, v in enumerate(pred):
                     row[f"pred_{idx}"] = v
             # Single class case
             else:
                 row["pred"] = pred
 
             self.df = self.df.append(row, ignore_index=True)
-        
-        self.df.to_csv(self.output_csv)
+
+        self.df.to_csv(self.output_csv)
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/fmcib/datasets/ssl_radiomics_dataset.py` & `foundation_cancer_image_biomarker-0.0.1a4/fmcib/datasets/ssl_radiomics_dataset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,32 +1,36 @@
+import faulthandler
+import signal
 from pathlib import Path
 
+import monai
 import numpy as np
 import pandas as pd
 import SimpleITK as sitk
-import monai
 from loguru import logger
 from torch.utils.data import Dataset
-from .utils import resample_image_to_spacing, slice_image, is_overlapping
 
-import faulthandler
-import signal
+from .utils import is_overlapping, resample_image_to_spacing, slice_image
+
 faulthandler.register(signal.SIGUSR1.value)
 monai.data.set_track_meta(False)
 sitk.ProcessObject.SetGlobalDefaultNumberOfThreads(1)
 
+
 class SSLRadiomicsDataset(Dataset):
     """
     add documentation on how this dataset works
 
     Args:
         add docstrings for the parameters
     """
 
-    def __init__(self, path, label=None, radius=25, orient=False, resample_spacing=None, enable_negatives=True, transform=None):
+    def __init__(
+        self, path, label=None, radius=25, orient=False, resample_spacing=None, enable_negatives=True, transform=None
+    ):
         super(SSLRadiomicsDataset, self).__init__()
         self._path = Path(path)
 
         self.radius = radius
         self.orient = orient
         self.resample_spacing = resample_spacing
         self.label = label
@@ -59,42 +63,35 @@
         """
         Extract a negative sample from the image backgroundwith no overlap to the positive sample
 
         image: Image to extract sample
         positive_patch_idx: Index of the positive patch in [(xmin, xmax), (ymin, ymax), (zmin, zmax)]
 
         """
-        positive_patch_size = [self.radius*2] * 3
-        valid_patch_size = monai.data.utils.get_valid_patch_size(
-            image.GetSize(), positive_patch_size
-        )
-        
+        positive_patch_size = [self.radius * 2] * 3
+        valid_patch_size = monai.data.utils.get_valid_patch_size(image.GetSize(), positive_patch_size)
+
         def get_random_patch():
             random_patch_idx = [
-                [x.start, x.stop]
-                for x in monai.data.utils.get_random_patch(
-                    image.GetSize(), valid_patch_size
-                )
+                [x.start, x.stop] for x in monai.data.utils.get_random_patch(image.GetSize(), valid_patch_size)
             ]
             return random_patch_idx
 
         random_patch_idx = get_random_patch()
 
         # escape_count = 0
         # while is_overlapping(positive_patch_idx, random_patch_idx):
         #     if escape_count >= 3:
         #         logger.warning("Random patch has overlap with positive patch")
         #         return None
 
         #     random_patch_idx = get_random_patch()
         #     escape_count += 1
-            
-        random_patch = slice_image(
-            image, random_patch_idx
-        )
+
+        random_patch = slice_image(image, random_patch_idx)
 
         random_patch = sitk.DICOMOrient(random_patch, "LPS")
         negative_array = sitk.GetArrayFromImage(random_patch)
 
         negative_tensor = negative_array if self.transform is None else self.transform(negative_array)
         return negative_tensor
 
@@ -104,16 +101,15 @@
         from your data source
         """
 
         # Get a row from the CSV file
         row = self.annotations.iloc[idx]
         image_path = row["image_path"]
         image = sitk.ReadImage(str(image_path))
-        image = resample_image_to_spacing(image, self.resample_spacing, -1024) \
-                if self.resample_spacing is not None else image
+        image = resample_image_to_spacing(image, self.resample_spacing, -1024) if self.resample_spacing is not None else image
 
         centroid = (row["coordX"], row["coordY"], row["coordZ"])
         centroid = image.TransformPhysicalPointToContinuousIndex(centroid)
         centroid = [int(d) for d in centroid]
 
         # Orient all images to LPI orientation
         image = sitk.DICOMOrient(image, "LPI") if self.orient else image
@@ -124,35 +120,32 @@
         patch_image = sitk.DICOMOrient(patch_image, "LPS")
 
         array = sitk.GetArrayFromImage(patch_image)
         tensor = array if self.transform is None else self.transform(array)
         target = int(row[self.label]) if self.label is not None else False
 
         if self.enable_negatives:
-            return  {
-                "positive": tensor, 
-                "negative": self.get_negative_sample(image)
-                }, target
+            return {"positive": tensor, "negative": self.get_negative_sample(image)}, target
 
         return tensor, target
 
 
 if __name__ == "__main__":
     from pathlib import Path
+
     # Test pytorch dataset
     print("Test pytorch dataset")
     dataset = SSLRadiomicsDataset(
         "/home/suraj/Repositories/cancer-imaging-ssl/src/pretraining/data_csv/deeplesion/train.csv",
         orient=True,
-        resample_spacing=[1, 1, 1]
+        resample_spacing=[1, 1, 1],
     )
 
     # Visualize item from dataset
     item = dataset[0]
 
-
     positive = sitk.GetImageFromArray(item[0][0])
     negative = sitk.GetImageFromArray(item[0][1])
     current_dir = Path(__file__).parent.resolve()
 
     sitk.WriteImage(positive, f"{str(current_dir)}/tests/positive.nrrd")
     sitk.WriteImage(negative, f"{str(current_dir)}/tests/negative.nrrd")
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/fmcib/datasets/utils.py` & `foundation_cancer_image_biomarker-0.0.1a4/fmcib/datasets/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,62 +1,61 @@
-import SimpleITK as sitk
 from pathlib import Path
 
 import numpy as np
+import SimpleITK as sitk
 
 # https://github.com/SimpleITK/SlicerSimpleFilters/blob/master/SimpleFilters/SimpleFilters.py
 SITK_INTERPOLATOR_DICT = {
-    'nearest': sitk.sitkNearestNeighbor,
-    'linear': sitk.sitkLinear,
-    'gaussian': sitk.sitkGaussian,
-    'label_gaussian': sitk.sitkLabelGaussian,
-    'bspline': sitk.sitkBSpline,
-    'hamming_sinc': sitk.sitkHammingWindowedSinc,
-    'cosine_windowed_sinc': sitk.sitkCosineWindowedSinc,
-    'welch_windowed_sinc': sitk.sitkWelchWindowedSinc,
-    'lanczos_windowed_sinc': sitk.sitkLanczosWindowedSinc
+    "nearest": sitk.sitkNearestNeighbor,
+    "linear": sitk.sitkLinear,
+    "gaussian": sitk.sitkGaussian,
+    "label_gaussian": sitk.sitkLabelGaussian,
+    "bspline": sitk.sitkBSpline,
+    "hamming_sinc": sitk.sitkHammingWindowedSinc,
+    "cosine_windowed_sinc": sitk.sitkCosineWindowedSinc,
+    "welch_windowed_sinc": sitk.sitkWelchWindowedSinc,
+    "lanczos_windowed_sinc": sitk.sitkLanczosWindowedSinc,
 }
 
-def resample_image_to_spacing(image, new_spacing, default_value, interpolator='linear'):
-    """Resample an image to a new spacing.
-    """    
-    assert interpolator in SITK_INTERPOLATOR_DICT, \
-        (f"Interpolator '{interpolator}' not part of SimpleITK. " 
-         f"Please choose one of the following {list(SITK_INTERPOLATOR_DICT.keys())}.")
-    
-    assert image.GetDimension() == len(new_spacing), \
-        (f"Input is {image.GetDimension()}-dimensional while "
-         f"the new spacing is {len(new_spacing)}-dimensional.")  
-    
+
+def resample_image_to_spacing(image, new_spacing, default_value, interpolator="linear"):
+    """Resample an image to a new spacing."""
+    assert interpolator in SITK_INTERPOLATOR_DICT, (
+        f"Interpolator '{interpolator}' not part of SimpleITK. "
+        f"Please choose one of the following {list(SITK_INTERPOLATOR_DICT.keys())}."
+    )
+
+    assert image.GetDimension() == len(new_spacing), (
+        f"Input is {image.GetDimension()}-dimensional while " f"the new spacing is {len(new_spacing)}-dimensional."
+    )
 
     interpolator = SITK_INTERPOLATOR_DICT[interpolator]
     spacing = image.GetSpacing()
     size = image.GetSize()
     new_size = [int(round(siz * spac / n_spac)) for siz, spac, n_spac in zip(size, spacing, new_spacing)]
-    return sitk.Resample(image,
-                         new_size,             # size
-                         sitk.Transform(),     # transform
-                         interpolator,         # interpolator
-                         image.GetOrigin(),    # outputOrigin
-                         new_spacing,          # outputSpacing
-                         image.GetDirection(), # outputDirection
-                         default_value,        # defaultPixelValue
-                         image.GetPixelID())   # outputPixelType
+    return sitk.Resample(
+        image,
+        new_size,  # size
+        sitk.Transform(),  # transform
+        interpolator,  # interpolator
+        image.GetOrigin(),  # outputOrigin
+        new_spacing,  # outputSpacing
+        image.GetDirection(),  # outputDirection
+        default_value,  # defaultPixelValue
+        image.GetPixelID(),
+    )  # outputPixelType
 
 
 def slice_image(image, patch_idx):
-    """Slice an image.
-    """
+    """Slice an image."""
 
     start, stop = zip(*patch_idx)
     slice_filter = sitk.SliceImageFilter()
     slice_filter.SetStart(start)
     slice_filter.SetStop(stop)
     return slice_filter.Execute(image)
 
 
 def is_overlapping(patch1, patch2):
+    overlap_by_axis = [max(axis1[0], axis2[0]) < min(axis1[1], axis2[1]) for axis1, axis2 in zip(patch1, patch2)]
 
-    overlap_by_axis = [max(axis1[0], axis2[0]) < min(axis1[1], axis2[1]) \
-                            for axis1, axis2 in zip(patch1, patch2)]
-
-    return np.all(overlap_by_axis)
+    return np.all(overlap_by_axis)
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/fmcib/models/resnet50.py` & `foundation_cancer_image_biomarker-0.0.1a4/fmcib/models/resnet50.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/fmcib/preprocessing/__init__.py` & `foundation_cancer_image_biomarker-0.0.1a4/fmcib/preprocessing/__init__.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/fmcib/preprocessing/seed_based_crop.py` & `foundation_cancer_image_biomarker-0.0.1a4/fmcib/preprocessing/seed_based_crop.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/fmcib/run.py` & `foundation_cancer_image_biomarker-0.0.1a4/fmcib/run.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/losses/ntxent_mined_loss.py` & `foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/losses/ntxent_mined_loss.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 """ Contrastive Loss Functions """
 
 # Copyright (c) 2020. Lightly AG and its affiliates.
 # All Rights Reserved
 
 # Modified to function for explicitly selected negatives
 
+from typing import Dict
+
 import torch
+from lightly.utils import dist
 from torch import nn
 
-from lightly.utils import dist
-from typing import Dict
 
 class NTXentNegativeMinedLoss(torch.nn.Module):
     """
     NTXentNegativeMinedLoss:
     NTXentLoss with explicitly mined negatives
     """
 
-    def __init__(self,
-                 temperature: float = 0.1,
-                 gather_distributed: bool = False):
+    def __init__(self, temperature: float = 0.1, gather_distributed: bool = False):
         super(NTXentNegativeMinedLoss, self).__init__()
         self.temperature = temperature
         self.gather_distributed = gather_distributed
         self.cross_entropy = nn.CrossEntropyLoss(reduction="mean")
         self.eps = 1e-8
 
         if abs(self.temperature) < self.eps:
-            raise ValueError('Illegal temperature: abs({}) < 1e-8'
-                             .format(self.temperature))
+            raise ValueError("Illegal temperature: abs({}) < 1e-8".format(self.temperature))
 
     def forward(self, out: Dict):
         """Forward pass through Negative mining contrastive Cross-Entropy Loss.
 
         Args:
             out: Dictionary with `positive` and `negative` key to represent
             positive selected and negative selected samples
@@ -53,41 +51,39 @@
 
         # normalize the output to length 1
         pos0 = nn.functional.normalize(pos0, dim=1)
         pos1 = nn.functional.normalize(pos1, dim=1)
         neg0 = nn.functional.normalize(neg0, dim=1)
         neg1 = nn.functional.normalize(neg1, dim=1)
 
-
         if self.gather_distributed and dist.world_size() > 1:
             # gather hidden representations from other processes
             pos0_large = torch.cat(dist.gather(pos0), 0)
             pos1_large = torch.cat(dist.gather(pos1), 0)
             neg0_large = torch.cat(dist.gather(neg0), 0)
-            neg1_large = torch.cat(dist.gather(neg1), 0)            
+            neg1_large = torch.cat(dist.gather(neg1), 0)
             diag_mask = dist.eye_rank(batch_size, device=pos0.device)
 
         else:
-             # gather hidden representations from other processes
+            # gather hidden representations from other processes
             pos0_large = pos0
             pos1_large = pos1
             neg0_large = neg0
             neg1_large = neg1
             diag_mask = torch.eye(batch_size, device=pos0.device, dtype=torch.bool)
-    
 
-        logits_00 = torch.einsum('nc,mc->nm', pos0, neg0_large) / self.temperature
-        logits_01 = torch.einsum('nc,mc->nm', pos0, pos1_large) / self.temperature
-        logits_10 = torch.einsum('nc,mc->nm', pos1, pos0_large) / self.temperature
-        logits_11 = torch.einsum('nc,mc->nm', pos1, neg1_large) / self.temperature
-        
+        logits_00 = torch.einsum("nc,mc->nm", pos0, neg0_large) / self.temperature
+        logits_01 = torch.einsum("nc,mc->nm", pos0, pos1_large) / self.temperature
+        logits_10 = torch.einsum("nc,mc->nm", pos1, pos0_large) / self.temperature
+        logits_11 = torch.einsum("nc,mc->nm", pos1, neg1_large) / self.temperature
+
         logits_01 = logits_01[diag_mask].view(batch_size, -1)
         logits_10 = logits_10[diag_mask].view(batch_size, -1)
 
         logits_0100 = torch.cat([logits_01, logits_00], dim=1)
         logits_1011 = torch.cat([logits_10, logits_11], dim=1)
         logits = torch.cat([logits_0100, logits_1011], dim=0)
 
         labels = torch.zeros(logits.shape[0], device=device, dtype=torch.long)
         loss = self.cross_entropy(logits, labels)
 
-        return loss
+        return loss
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/models/exneg_simclr.py` & `foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/models/exneg_simclr.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-from typing import Union, Dict
+from typing import Dict, Union
+
 import torch
 import torch.nn as nn
 from lightly.models import SimCLR
 
+
 class ExNegSimCLR(SimCLR):
     def __init__(self, backbone: nn.Module, num_ftrs: int = 32, out_dim: int = 128) -> None:
         print(backbone)
         super().__init__(backbone, num_ftrs, out_dim)
 
     def forward(self, x: Union[Dict, torch.Tensor], return_features: bool = False):
         assert isinstance(x, dict), "Input to forward must be a `dict` for ExNegSimCLR"
         out = {}
         for key, value in x.items():
             if isinstance(value, list):
                 out[key] = super().forward(*value, return_features)
 
         return out
-
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/models/load_pretrained_resnet.py` & `foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/models/load_pretrained_resnet.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,35 +1,38 @@
 import monai
-from torch import nn
-from monai.networks.nets.resnet import ResNetBottleneck as Bottleneck
 import torch
 from loguru import logger
+from monai.networks.nets.resnet import ResNetBottleneck as Bottleneck
+from torch import nn
+
 
 class LoadPretrainedResnet3D(nn.Module):
     def __init__(self, pretrained=None, vissl=False, heads=[]) -> None:
         super().__init__()
         self.trunk = monai.networks.nets.resnet.ResNet(
             block=Bottleneck,
             layers=(3, 4, 6, 3),
             block_inplanes=(64, 128, 256, 512),
             spatial_dims=3,
             n_input_channels=1,
             conv1_t_stride=2,
             conv1_t_size=7,
             widen_factor=2,
-            num_classes=400
+            num_classes=400,
         )
         self.trunk.fc = nn.Identity()
 
         head_layers = []
         for idx in range(len(heads) - 1):
-            head_layers.append(nn.Linear(heads[idx], heads[idx+1], bias=True))
+            current_layers = []
+            current_layers.append(nn.Linear(heads[idx], heads[idx + 1], bias=True))
 
             if idx != len(heads) - 1:
-                head_layers.append(nn.ReLU(inplace=True))
+                current_layers.append(nn.ReLU(inplace=True))
+            head_layers.append(nn.Sequential(*current_layers))
 
         if len(head_layers):
             self.heads = nn.Sequential(*head_layers)
         else:
             self.heads = nn.Identity()
 
         if pretrained is not None:
@@ -40,21 +43,22 @@
         out = self.heads(out)
         return out
 
     def load(self, pretrained):
         pretrained_model = torch.load(pretrained)
 
         # Load trained trunk
-        trained_trunk = pretrained_model['trunk_state_dict']
+        trained_trunk = pretrained_model["trunk_state_dict"]
         msg = self.trunk.load_state_dict(trained_trunk, strict=False)
-        logger.warning(f'Missing keys: {msg[0]} and unexpected keys: {msg[1]}')
+        logger.warning(f"Missing keys: {msg[0]} and unexpected keys: {msg[1]}")
 
         # Load trained heads
         if "head_state_dict" in pretrained_model:
-            trained_heads = pretrained_model['head_state_dict']
+            trained_heads = pretrained_model["head_state_dict"]
+
             try:
                 msg = self.heads.load_state_dict(trained_heads, strict=False)
-            except:
-                logger.error("Failed to load trained heads. This is expected if the models do not match!")
-            logger.warning(f'Missing keys: {msg[0]} and unexpected keys: {msg[1]}')
+            except Exception as e:
+                logger.error(f"Failed to load trained heads with error {e}. This is expected if the models do not match!")
+            logger.warning(f"Missing keys: {msg[0]} and unexpected keys: {msg[1]}")
 
-        logger.info(f'Loaded pretrained model weights \n')
+        logger.info(f"Loaded pretrained model weights \n")
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/optimizers/lars.py` & `foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/optimizers/lars.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 References:
     - https://arxiv.org/pdf/1708.03888.pdf
     - https://github.com/pytorch/pytorch/blob/1.6/torch/optim/sgd.py
 """
 import torch
 from torch.optim.optimizer import Optimizer, required
 
+
 class LARS(Optimizer):
     """Extends SGD in PyTorch with LARS scaling from the paper
     `Large batch training of Convolutional Networks <https://arxiv.org/pdf/1708.03888.pdf>`_.
     Args:
         params (iterable): iterable of parameters to optimize or dicts defining
             parameter groups
         lr (float): learning rate
@@ -140,8 +141,8 @@
                     if nesterov:
                         d_p = d_p.add(buf, alpha=momentum)
                     else:
                         d_p = buf
 
                 p.add_(d_p, alpha=-group["lr"])
 
-        return loss
+        return loss
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/transforms/duplicate.py` & `foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/transforms/duplicate.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,18 @@
+from typing import Any, Callable, List, Optional, Tuple
+
 from copy import deepcopy
-from typing import Any, Callable, Optional, Tuple, List
 
 import torch
 
 
 class Duplicate:
-    """Duplicate an input and apply two different transforms. Used for SimCLR primarily.
-    """
+    """Duplicate an input and apply two different transforms. Used for SimCLR primarily."""
 
-    def __init__(self,
-                 transforms1: Optional[Callable] = None,
-                 transforms2: Optional[Callable] = None):
+    def __init__(self, transforms1: Optional[Callable] = None, transforms2: Optional[Callable] = None):
         """Duplicates an input and applies the given transformations to each copy separately.
 
         Args:
             transforms1 (Optional[Callable], optional): _description_. Defaults to None.
             transforms2 (Optional[Callable], optional): _description_. Defaults to None.
         """
         # Wrapped into a list if it isn't one already to allow both a
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/fmcib/ssl/transforms/random_resized_crop.py` & `foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/transforms/random_resized_crop.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
-import torch
 from typing import Any, Dict, List
 
+import torch
 from monai.transforms import RandScaleCrop, Resize, Transform
 
+
 class RandomResizedCrop3D(Transform):
     """
     Combines monai's random spatial crop followed by resize to the desired size.
 
-    Modification: 
-    1. The spatial crop is done with same dimensions for all the axes 
-    2. Handles cases where the image_size is less than the crop_size by choosing 
+    Modification:
+    1. The spatial crop is done with same dimensions for all the axes
+    2. Handles cases where the image_size is less than the crop_size by choosing
         the smallest dimension as the random scale.
 
     """
 
     def __init__(self, prob: float = 1, size: int = 50, scale: List[float] = [0.5, 1.0]):
         """
         Args:
@@ -21,19 +22,17 @@
              before resizing. The scale is defined with respect to the area of the original image.
         """
         super().__init__()
         self.prob = prob
         self.scale = scale
         self.size = [size] * 3
 
-
     def __call__(self, image):
         if torch.rand(1) < self.prob:
             random_scale = torch.empty(1).uniform_(*self.scale).item()
             rand_cropper = RandScaleCrop(random_scale, random_size=False)
             resizer = Resize(self.size, mode="trilinear")
 
             for transform in [rand_cropper, resizer]:
                 image = transform(image)
 
         return image
-
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/pyproject.toml` & `foundation_cancer_image_biomarker-0.0.1a4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "foundation-cancer-image-biomarker"
-version = "0.0.1a3"
+version = "0.0.1a4"
 description = "Official repo for Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging [INSERT DOI]"
 readme = "README.md"
 authors = ["Suraj Pai <bspai@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/AIM-Harvard/foundation-cancer-image-biomarker"
 homepage = "https://aim.hms.harvard.edu/foundation-cancer-image-biomarker"
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a3/PKG-INFO` & `foundation_cancer_image_biomarker-0.0.1a4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundation-cancer-image-biomarker
-Version: 0.0.1a3
+Version: 0.0.1a4
 Summary: Official repo for Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging [INSERT DOI]
 Home-page: https://aim.hms.harvard.edu/foundation-cancer-image-biomarker
 License: MIT
 Author: Suraj Pai
 Author-email: bspai@bwh.harvard.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -42,22 +42,24 @@
 [![Pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/blob/master/.pre-commit-config.yaml)
 [![Semantic Versions](https://img.shields.io/badge/%20%20%F0%9F%93%A6%F0%9F%9A%80-semantic--versions-e10079.svg)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/releases)
 [![License](https://img.shields.io/github/license/foundation_image_biomarker/foundation-image-biomarker)](https://github.com/foundation_image_biomarker/foundation-image-biomarker/blob/master/LICENSE)
 ![Coverage Report](assets/images/coverage.svg)
 
 </div> -->
 
-## Overview
 This is the the official repository for the paper <i> Foundation Models for Quantitative Biomarker Discovery for Cancer Imaging </i> <br/>
 Suraj Pai, Dennis Bontempi, Vasco Prudente, Ibrahim Hadzic, Mateo Sokač, Tafadzwa L. Chaunzwa, Simon Bernatz, Ahmed Hosny, Raymond H Mak, Nicolai J Birkbak, Hugo JWL Aerts
 
-<div style="display: flex; justify-content: center"><img src="assets/images/overview_v5.png" width=550 /></div>
+&emsp;
+## Overview
+<div style="display: flex; justify-content: center"><img src="assets/images/overview_v5.png" width=600 /></div>
 
- <b>General overview of the study.</b><b> a. Foundation model pre-training.</b> A foundation model, specifically a deep convolutional encoder model, was pre-trained by contrasting volumes with and without lesions. <b> b. </b> Clinical application of the foundation model. The foundation model was used to extract biomarkers and then evaluated for three classification tasks on diverse datasets. <b>c. Foundation model implementation approaches </b>  The foundation model was adapted to specific use cases by extracting features or through fine-tuning (left). <b> d. Evaluation against supervised models with selected performance metrics. </b> We compared the performance of the foundation models against conventional supervised implementations, trained from scratch (left) and fine-tuned from a different task (right). The comparison was made through several criteria for the different use cases, including quantitative performance, stability, and biological analysis. Biological, clinical, and stability analyses are limited to use case 2 due to the availability of associated data. 
+ <b>General overview of the study.</b><b> a. Foundation model pre-training.</b> A foundation model, specifically a deep convolutional encoder model, was pre-trained by contrasting volumes with and without lesions. <b> b.  Clinical application of the foundation model.</b> The foundation model was used to extract biomarkers and then evaluated for three classification tasks on diverse datasets. <b>c. Foundation model implementation approaches </b>  The foundation model was adapted to specific use cases by extracting features or through fine-tuning (left). <b> d. Evaluation against supervised models with selected performance metrics. </b> We compared the performance of the foundation models against conventional supervised implementations, trained from scratch (left) and fine-tuned from a different task (right). The comparison was made through several criteria for the different use cases, including quantitative performance, stability, and biological analysis. Biological, clinical, and stability analyses are limited to use case 2 due to the availability of associated data. 
 
+&emsp;
 ## Table of Contents
 
 - [Repository Structure](#repository-structure)
 - [Quick Start](#quick-start)
 - [Data](#data)
   - [Downloading the datasets](#downloading-the-datasets)
   - [Preprocessing the datasets](#preprocessing-the-datasets)
@@ -75,31 +77,34 @@
   - [Predictions pipeline](#predictions-pipeline)
 - [Analysis](#analysis)
 - [License](#🛡-license)
 - [Acknowledgement](#acknowledgements)
 - [Disclaimer](#disclaimer)
 - [Code Citation](#📃-code-citation)
 
+<div style="page-break-after: always;"></div>
+
 ## Repository Structure
 
-This code repository includes the Python package `fmcib`, as well as the code to reproduce experiments and analyses presented in our paper.
+This code repository includes the Python package containing all our source code: `fmcib`, as well as the code to reproduce experiments and analyses presented in our paper. The pipelines to reproduce our experiments and analyses are independent of the python package and will be shared to the public upon publication.
 
 Here is the structure of the repository:
 
 ```
 ├── fmcib/          # The main Python package
 ├── data/           # Downloading and preprocessing data
 ├── experiments/    # Reproduce paper experiments
 ├── models/         # Download and test final models
 ├── outputs/        # Outputs from pipelines in the study
 ├── analysis/       # Reproducible analysis for statistics
 ├── additional_requirements.txt
 └── README.pdf
 ```
 
+&emsp;
 ## Quick Start
 
 We recommend using **Python 3.8** on a Linux machine since that is the environment we have tested on. However, the use of Poetry for managing dependencies should make it compatible with Python versions above 3.8 on all platforms. We suggest using Conda to create an isolated virtual environment for the project dependencies. To download Conda, follow the instructions here: https://conda.io/projects/conda/en/latest/user-guide/install/index.html
 
 After downloading and activating Conda, create and activate a virtual environment with the following commands:
 
 ```python
@@ -122,16 +127,16 @@
 ```
 
 You can verify if the dependencies are installed by: 
 ```bash
 python -c "import fmcib; print(fmcib.__version__)"
 ```
 
-This should work without error and show you a version string as the results. Once completed, you can run each of the provided pipelines to reproduce experiments and analyses. These pipelines are not part of the Python package (which mostly contains code to load models and ssl training specific code) and will be shared publicly upon publication.
 
+<div style="page-break-after: always;"></div>
 
 ## Data
 The majority of the datasets utilized in this study are openly accessible for both training and validation purposes: 
 1.  DeepLesion (https://nihcc.app.box.com/v/DeepLesion/): DeepLesion is a dataset comprising 32,735 lesions from 10,594 studies of 4,427 unique patients collected over two decades from the National Institute of Health Clinical Center PACS server. Various lesions, including kidney, bone, and liver lesions - as well as enlarged lymph nodes and lung nodules, are annotated. The lesions are identified through radiologist-bookmarked RECIST diameters across 32,120 CT slice . In our study we use this dataset both for our pre-training and use-case 1 
 
 
 2.  LUNA16 (https://luna16.grand-challenge.org/Data/): LUNA16 is a curated version of the LIDC-IDRI dataset of 888 diagnostic and lung cancer screening thoracic CT scans obtained from seven academic centers and eight medical imaging companies comprising 1,186 nodules. The nodules are accompanied by annotations agreed upon by at least 3 out of 4 radiologists. Alongside nodule location annotations, radiologists also noted various observed attributes like internal composition, calcification, malignancy, suspiciousness, and more. We use this dataset to develop and validate our diagnostic image biomarker
@@ -155,15 +160,14 @@
 
 For DeepLesion,
 ```
 cd data/download
 bash deeplesion.sh <path_to_download>
 ```
 
-
 For LUNA16,
 ```
 cd data/download
 bash luna16.sh <path_to_download>
 ```
 <b> Downloading the LUNG1 and RADIO datasets </b>
 Refer to [Google colab notebook](https://colab.research.google.com/drive/1Svk8VaZHWAYdZHE45DNdWXVqhe7v9sFR#scrollTo=okx0n73EI11u) that contains information on how this data can be downloaded and pre-processed.
@@ -171,30 +175,36 @@
 ### Preprocessing the datasets
 We provide simple linux shell scripts to reproduce the pre-processing pipeline. Incase, you have a different operating system, simply run the python scripts in these shell scripts individually in your environment.
 
 <b> Pre-processing the DeepLesion dataset </b>
 Note: Conda is required to perform this
 ```
 cd data/preprocessing/deeplesion
-bash run.sh
+bash run.sh <path_to_download>
 ```
 
 Once you run this successfully, you should see a file `data/processing/deeplesion/annotations/deeplesion_training_annotations.csv`. At this point you can run the notebook `data/processing/deeplesion/Process_Dataset.ipynb` to get the splits we use in our paper. For reference, we have already provided splits for comparison as generated by us.
 
+NOTE: The pre-processing extracts the image files from zip files. Please delete the zip files from the path `<path_to_download>/DeepLesion/Images_png` using `rm <path_to_download>/DeepLesion/Images_png/*.zip`  path after these scripts are successfully run to not inflate your disk space.
+
+
 <b> Pre-processing the LUNA16 dataset </b>
 ```
 cd data/preprocessing/luna16
-bash run.sh
+bash run.sh <path_to_download>
 ```
 
+NOTE: The pre-processing extracts the image files from zip files. Please delete the zip files from the path `<path_to_download>/LUNA16` using `rm <path_to_download>/LUNA16/*.zip` after these scripts are successfully run to not inflate your disk space.
+
 Once you run this successfully, you should see a file `data/processing/deeplesion/annotations/luna16_training_annotations.csv`. At this point you can run the notebook `data/processing/deeplesion/Process_Dataset.ipynb` to get the splits we use in our paper. For reference, we have already provided splits for comparison as generated by us.
 
 <b> Pre-processing the LUNG1 and RADIO dataset </b>
-Refer to [our Google Colab reprocible notebooks](https://colab.research.google.com/drive/1Svk8VaZHWAYdZHE45DNdWXVqhe7v9sFR#scrollTo=okx0n73EI11u) that also contains information on how this data can be downloaded and pre-processed
+Refer to [our Google Colab reproducible notebooks](https://colab.research.google.com/drive/1Svk8VaZHWAYdZHE45DNdWXVqhe7v9sFR#scrollTo=okx0n73EI11u) that also contains information on how this data can be accessed
 
+<div style="page-break-after: always;"></div>
 
 ## Model
 All our models are will be made available to the public through Zenodo upon publication. Currently, we release these using Dropbox for the reviewers to use and test. Scripts for downloading these models are present under `models`. 
 
 As part of our study we develop and share the following,
 
 ### Self-supervised pre-training model:
@@ -213,42 +223,47 @@
 
 The pre-trained model is implemented on downstreams task using supervised training or linear evaluation approaches. For these we develop,
 
 ### Supervised models:
 
 We developed three supervised training approaches,
  - Supervised model trained from random initialization
+<br>
+<div style="display: flex; justify-content: center"><img src="assets/images/implementation1.png" width=400 /></div>
+
 
  - Fine-tuning a trained supervised model
+<br>
+<div style="display: flex; justify-content: center"><img src="assets/images/implementation2.png" width=400 /></div>
 
  - Fine-tuning a pre-trained foundation model
+<br>
+<div style="display: flex; justify-content: center"><img src="assets/images/implementation3.png" width=400 /></div>
 
 
-<br>
-<div style="display: flex; justify-content: center"><img src="assets/images/supervised_models.png" width=400 /></div>
 
 To download these models run,
 ````bash
 cd models
 bash download_supervised_models.sh
 ````
 
 
 ### Linear (Logistic Regression) models:
 Our linear model takes features extracted from the pre-trained foundation model and builds a logistic regression classifer to predict outcome. 
 <div style="display: flex; justify-content: center"><img src="assets/images/linear_model.png" width=400 /></div>
 
+&emsp;
 To download these models run,
 ````bash
 cd models
 bash download_linear_models.sh
 ````
 
-These models can also be found at this [link](https://www.dropbox.com/scl/fo/brhqokhzn839zez15erzf/h?dl=0&rlkey=wzvgrobl8p3v49ettm16uxbyy)
-In addition to providing our models, we also provide comprehensive documentation and ongoing support to users through [project-lighter](https://zenodo.org/record/8007711) to reproduce our results and workflows.
+These models can also be found at this [link](https://www.dropbox.com/scl/fo/brhqokhzn839zez15erzf/h?dl=0&rlkey=wzvgrobl8p3v49ettm16uxbyy). In addition to providing our models, we also provide comprehensive documentation and ongoing support to users through [project-lighter](https://zenodo.org/record/8007711) to reproduce our results and workflows.
 
 
 ### Data setup for the models
 Make sure you download all the datasets before starting to train. The datasets are provided as CSV files to the training pipelines with `image_path` column providing location of the image to be used, `coordX`, `coordY` and `coordZ` providing the global coordinates of the seed point around which a patch is cropped. We crop a [50, 50, 50] patch around the seed point. Please refer to our paper for more details on this. Along with these columns, label columns are needed for supervised training. Labels for each task are as follows,
 ```
 Task 1: Coarse_lesion_type
 Task 2: malignancy
@@ -283,14 +298,16 @@
 ```yaml
 train_dataset:
   _target_: fmcib.ssl.datasets.SSLRadiomicsDataset
   path: "your_pretrain_set_path_goes_here"
 ```
 
 Now you can start training by running this in the root code folder,
+
+
 ```bash
 lighter fit --config_file ./experiments/pretraining/simclr_pretrain.yaml
 ```
 
 
 ### Reproducing our supervised training
 As mentioned in [section](#supervised-models), we have three different supervised training implementations. Similar to the foundation pre-training, we use YAML files to maintain the configurations of these implementations. 
@@ -304,14 +321,15 @@
 lighter fit --config_file ./experiments/supervised_training/supervised_random_init.yaml
 ```
 
 <b> Fine-tuning a trained supervised model </b>
 
 The YAML configuration at `experiments/supervised_training/supervised_finetune.yaml` describes how you can fine-tune an already trained supervised model. Note that this is possible only for Task 2 and Task 3 as we used the supervised model trained in Task 1 to load weights from. Make sure you download the weights for Task 1 supervised models. You can follow instructions [here](#model) 
 
+
 You can start training by running this in the root code folder,
 ```bash
 lighter fit --config_file ./experiments/supervised_training/supervised_finetune.yaml
 ```
 
 <b> Fine-tuning a pre-trained foundation model </b>
 
@@ -353,16 +371,27 @@
 
 The <label> corresponds to the column in the csv files that contains the supervised label to predict. For example, in use-case 2 the label is `malignancy`. 
 
 You can also provide scoring metrics, for instance,  using `--scoring roc_auc` where the scoring metric is a sklearn scorer. You can also provide the number of trials the optimization framework needs to be run for using `--trials`. 
 
 The features folder is provided under `outputs/foundation_features` to try our the modelling process. Refer [here](#feature-extaction-pipeline)
 
+<div style="page-break-after: always;"></div>
+
 ## Outputs
-The `outputs` folder contains outputs from several pipelines used in our study. 
+The `outputs` folder contains outputs from several pipelines used in our study. To download all the outputs, you can run
+
+
+```bash
+cd outputs
+bash download_outputs.sh
+```
+
+
+The script contains several dropbox links. You can also manually download them and place them in the right location. 
 
 ### Feature extaction pipeline
 The `foundation_features` folders contains features extracted from the pre-trained foundation model for Task 1, 2 and 3. The features are stored in `csv` files with column names `feature_x` corresponding to the dimension `x` of the feature. The total dimensionality of the features is 4096. Below is the structure of the folder,
 ```bash
 outputs
 └── foundation_features
     └── task1
@@ -396,52 +425,57 @@
         └── RADIO
             └── *.csv 
 ```
 For Task 1 and Task 2, we store predictions extracted over a range of different percentages of data used during the model training process (100%, 50%, 20%, and 10%). Predictions are saved for each of the implementation approaches. To differentiate between the predictions based on limited data percentages, we have appended a suffix `_x_percent.cs`, where 'x' represents the data percentage used
 
 For Task 3, we provide predictions for each of the different implementation approaches when tested on the LUNG1 and RADIO datasets. Validation predictions of the HarvardRT for computing Kaplan Meier curves as presented in [analysis](#analysis) notebooks are also provided.
 
+<div style="page-break-after: always;"></div>
+
 ## Analysis
 To support complete transparency of our work and allow you to have a better understanding of our analysis pipelines, the provided notebooks, with detailed walk-throughs, will help explore our analysis as well as reproduce the figures that are included in our research paper. The predictions extracted are described [here](#predictions-extracted).
 
 The analysis notebooks are organized as follows,
 
 ```bash
 analysis
 └── task1.ipynb
 └── task2.ipynb
 └── task3.ipynb
 └── stability.ipynb
 ```
 
-Detailed walk-throughs are provided in the notebooks. These notebooks reproduce Figures 2, 3, 4 and Extended Data Figure 3. Please ensure you download additional dependenices as described in the [quickstart](#quick-start)
+Detailed walk-throughs are provided in the notebooks. These notebooks reproduce Figures 2, 3, 4 and Extended Data Figure 3. Please ensure you download additional dependenices as described in the [quickstart](#quick-start) and that you have downloaded all the outputs from our pipelines.
 
 Shown below are samples from the analysis notebooks
 <div style="display: flex; justify-content: center"><img src="assets/analysis_1.png" width=300 /><img src="assets/analysis_2.png" width=200 /></div>
 
 <div style="display: flex; justify-content: center"><img src="assets/analysis_3.png" width=300 /><img src="assets/analysis_4.png" width=300 /></div>
 
-## 🛡 License
+<div style="page-break-after: always;"></div>
 
-This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/AIM-Harvard/foundation-cancer-image-biomarker/blob/master/LICENSE) for more details.
+&emsp;
+## License
 
+This project is licensed under the terms of the `MIT` license. See [LICENSE](https://github.com/AIM-Harvard/foundation-cancer-image-biomarker/blob/master/LICENSE) for more details.
 
+&emsp;
 ## Acknowledgements
 Code development, testing, and documentation: Suraj Pai
 Framework used for building the code: project-lighter (https://github.com/project-lighter/lighter)
 
+project-lighter was developed internally within our lab by Ibrahim Hadzic and Suraj Pai. 
+
+&emsp;
 ## Disclaimer
 The code and data of this repository are provided to promote reproducible research. They are not intended for clinical care or
-commercial use.
-The software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of
-merchantability, fitness for a particular purpose and noninfringement. In no event shall the authors or copyright holders be liable
-for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection
-with the software or the use or other dealings in the software.
+commercial use. The software is provided "as is", without warranty of any kind, express or implied, including but not limited to the warranties of merchantability, fitness for a particular purpose and noninfringement. In no event shall the authors or copyright holders be liable for any claim, damages or other liability, whether in an action of contract, tort or otherwise, arising from, out of or in connection with the software or the use or other dealings in the software.
 
-## 📃 Code Citation
+&emsp;
+## Code Citation
 Will be updated to reflect a Zenodo DOI upon publication
 ```bibtex
 @misc{foundation-cancer-image-biomarker,
   author = {AIM-Harvard},
   title = {Official repo for "Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging"},
   year = {2023},
   publisher = {GitHub},
```

