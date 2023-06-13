# Comparing `tmp/foundation_cancer_image_biomarker-0.0.1a4.tar.gz` & `tmp/foundation_cancer_image_biomarker-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "foundation_cancer_image_biomarker-0.0.1a4.tar", max compression
+gzip compressed data, was "foundation_cancer_image_biomarker-0.0.1a5.tar", max compression
```

## Comparing `foundation_cancer_image_biomarker-0.0.1a4.tar` & `foundation_cancer_image_biomarker-0.0.1a5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1076 2023-06-04 18:03:55.694363 foundation_cancer_image_biomarker-0.0.1a4/LICENSE
--rw-r--r--   0        0        0    28582 2023-06-12 21:55:26.988316 foundation_cancer_image_biomarker-0.0.1a4/README.md
--rw-r--r--   0        0        0       24 2023-06-13 02:05:01.956824 foundation_cancer_image_biomarker-0.0.1a4/fmcib/__init__.py
--rw-r--r--   0        0        0       48 2023-06-13 02:03:39.397472 foundation_cancer_image_biomarker-0.0.1a4/fmcib/callbacks/__init__.py
--rw-r--r--   0        0        0     2159 2023-06-13 02:03:53.085364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/callbacks/prediction_saver.py
--rw-r--r--   0        0        0      406 2023-06-13 02:03:53.089364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/callbacks/utils.py
--rw-r--r--   0        0        0      619 2023-06-13 02:03:53.093364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/datasets/__init__.py
--rw-r--r--   0        0        0     5184 2023-06-13 02:03:53.093364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/datasets/ssl_radiomics_dataset.py
--rw-r--r--   0        0        0     2151 2023-06-13 02:03:53.097364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/datasets/utils.py
--rw-r--r--   0        0        0      257 2023-06-13 02:03:53.033365 foundation_cancer_image_biomarker-0.0.1a4/fmcib/models/__init__.py
--rw-r--r--   0        0        0      767 2023-06-09 10:06:02.963848 foundation_cancer_image_biomarker-0.0.1a4/fmcib/models/resnet50.py
--rw-r--r--   0        0        0     1437 2023-06-13 01:00:24.547870 foundation_cancer_image_biomarker-0.0.1a4/fmcib/preprocessing/__init__.py
--rw-r--r--   0        0        0     4283 2023-06-06 01:43:30.549334 foundation_cancer_image_biomarker-0.0.1a4/fmcib/preprocessing/seed_based_crop.py
--rw-r--r--   0        0        0      943 2023-06-13 01:00:06.900032 foundation_cancer_image_biomarker-0.0.1a4/fmcib/run.py
--rw-r--r--   0        0        0        0 2023-06-08 02:44:13.386481 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/__init__.py
--rw-r--r--   0        0        0       55 2023-06-13 02:03:39.437472 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/losses/__init__.py
--rw-r--r--   0        0        0     3259 2023-06-13 02:03:53.061365 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/losses/ntxent_mined_loss.py
--rw-r--r--   0        0        0       97 2023-06-13 02:03:39.437472 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/models/__init__.py
--rw-r--r--   0        0        0      656 2023-06-13 02:03:53.041365 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/models/exneg_simclr.py
--rw-r--r--   0        0        0     2212 2023-06-13 02:03:53.045365 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/models/load_pretrained_resnet.py
--rw-r--r--   0        0        0       23 2023-06-13 02:03:39.453472 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/optimizers/__init__.py
--rw-r--r--   0        0        0     5399 2023-06-13 02:03:39.525471 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/optimizers/lars.py
--rw-r--r--   0        0        0       86 2023-06-13 02:03:53.065364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/transforms/__init__.py
--rw-r--r--   0        0        0     1376 2023-06-13 02:03:53.065364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/transforms/duplicate.py
--rw-r--r--   0        0        0     1301 2023-06-13 02:03:53.069364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/transforms/random_resized_crop.py
--rw-r--r--   0        0        0       67 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a4/fmcib/utils/__init__.py
--rw-r--r--   0        0        0      367 2023-06-13 02:03:39.465471 foundation_cancer_image_biomarker-0.0.1a4/fmcib/utils/download_utils.py
--rw-r--r--   0        0        0     5378 2023-06-13 02:03:53.105364 foundation_cancer_image_biomarker-0.0.1a4/fmcib/utils/idc_helper.py
--rw-r--r--   0        0        0       44 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a4/fmcib/visualization/__init__.py
--rw-r--r--   0        0        0      499 2023-06-06 01:41:36.682184 foundation_cancer_image_biomarker-0.0.1a4/fmcib/visualization/verify_io.py
--rw-r--r--   0        0        0     4201 2023-06-13 02:05:01.888824 foundation_cancer_image_biomarker-0.0.1a4/pyproject.toml
--rw-r--r--   0        0        0    29959 1970-01-01 00:00:00.000000 foundation_cancer_image_biomarker-0.0.1a4/PKG-INFO
+-rw-r--r--   0        0        0     1076 2023-06-04 18:03:55.694363 foundation_cancer_image_biomarker-0.0.1a5/LICENSE
+-rw-r--r--   0        0        0    28582 2023-06-12 21:55:26.988316 foundation_cancer_image_biomarker-0.0.1a5/README.md
+-rw-r--r--   0        0        0       24 2023-06-13 15:29:06.135943 foundation_cancer_image_biomarker-0.0.1a5/fmcib/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-13 02:03:39.397472 foundation_cancer_image_biomarker-0.0.1a5/fmcib/callbacks/__init__.py
+-rw-r--r--   0        0        0     2159 2023-06-13 02:03:53.085364 foundation_cancer_image_biomarker-0.0.1a5/fmcib/callbacks/prediction_saver.py
+-rw-r--r--   0        0        0      406 2023-06-13 02:03:53.089364 foundation_cancer_image_biomarker-0.0.1a5/fmcib/callbacks/utils.py
+-rw-r--r--   0        0        0     2363 2023-06-13 15:04:42.507085 foundation_cancer_image_biomarker-0.0.1a5/fmcib/datasets/__init__.py
+-rw-r--r--   0        0        0     5184 2023-06-13 02:03:53.093364 foundation_cancer_image_biomarker-0.0.1a5/fmcib/datasets/ssl_radiomics_dataset.py
+-rw-r--r--   0        0        0     2151 2023-06-13 02:03:53.097364 foundation_cancer_image_biomarker-0.0.1a5/fmcib/datasets/utils.py
+-rw-r--r--   0        0        0      257 2023-06-13 02:03:53.033365 foundation_cancer_image_biomarker-0.0.1a5/fmcib/models/__init__.py
+-rw-r--r--   0        0        0      767 2023-06-09 10:06:02.963848 foundation_cancer_image_biomarker-0.0.1a5/fmcib/models/resnet50.py
+-rw-r--r--   0        0        0     1430 2023-06-13 14:31:47.554595 foundation_cancer_image_biomarker-0.0.1a5/fmcib/preprocessing/__init__.py
+-rw-r--r--   0        0        0     4283 2023-06-06 01:43:30.549334 foundation_cancer_image_biomarker-0.0.1a5/fmcib/preprocessing/seed_based_crop.py
+-rw-r--r--   0        0        0      889 2023-06-13 14:31:03.962933 foundation_cancer_image_biomarker-0.0.1a5/fmcib/run.py
+-rw-r--r--   0        0        0        0 2023-06-08 02:44:13.386481 foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/__init__.py
+-rw-r--r--   0        0        0       55 2023-06-13 02:03:39.437472 foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/losses/__init__.py
+-rw-r--r--   0        0        0     3259 2023-06-13 02:03:53.061365 foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/losses/ntxent_mined_loss.py
+-rw-r--r--   0        0        0       97 2023-06-13 02:03:39.437472 foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/models/__init__.py
+-rw-r--r--   0        0        0      656 2023-06-13 02:03:53.041365 foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/models/exneg_simclr.py
+-rw-r--r--   0        0        0     2212 2023-06-13 02:03:53.045365 foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/models/load_pretrained_resnet.py
+-rw-r--r--   0        0        0       23 2023-06-13 02:03:39.453472 foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/optimizers/__init__.py
+-rw-r--r--   0        0        0     5399 2023-06-13 02:03:39.525471 foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/optimizers/lars.py
+-rw-r--r--   0        0        0       86 2023-06-13 02:03:53.065364 foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/transforms/__init__.py
+-rw-r--r--   0        0        0     1376 2023-06-13 02:03:53.065364 foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/transforms/duplicate.py
+-rw-r--r--   0        0        0     1301 2023-06-13 02:03:53.069364 foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/transforms/random_resized_crop.py
+-rw-r--r--   0        0        0       67 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a5/fmcib/utils/__init__.py
+-rw-r--r--   0        0        0      367 2023-06-13 02:03:39.465471 foundation_cancer_image_biomarker-0.0.1a5/fmcib/utils/download_utils.py
+-rw-r--r--   0        0        0     5378 2023-06-13 02:03:53.105364 foundation_cancer_image_biomarker-0.0.1a5/fmcib/utils/idc_helper.py
+-rw-r--r--   0        0        0       44 2023-06-06 01:43:30.477335 foundation_cancer_image_biomarker-0.0.1a5/fmcib/visualization/__init__.py
+-rw-r--r--   0        0        0      499 2023-06-06 01:41:36.682184 foundation_cancer_image_biomarker-0.0.1a5/fmcib/visualization/verify_io.py
+-rw-r--r--   0        0        0     4201 2023-06-13 15:29:06.067943 foundation_cancer_image_biomarker-0.0.1a5/pyproject.toml
+-rw-r--r--   0        0        0    29959 1970-01-01 00:00:00.000000 foundation_cancer_image_biomarker-0.0.1a5/PKG-INFO
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/LICENSE` & `foundation_cancer_image_biomarker-0.0.1a5/LICENSE`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/README.md` & `foundation_cancer_image_biomarker-0.0.1a5/README.md`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/fmcib/callbacks/prediction_saver.py` & `foundation_cancer_image_biomarker-0.0.1a5/fmcib/callbacks/prediction_saver.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/fmcib/datasets/ssl_radiomics_dataset.py` & `foundation_cancer_image_biomarker-0.0.1a5/fmcib/datasets/ssl_radiomics_dataset.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/fmcib/datasets/utils.py` & `foundation_cancer_image_biomarker-0.0.1a5/fmcib/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/fmcib/models/resnet50.py` & `foundation_cancer_image_biomarker-0.0.1a5/fmcib/models/resnet50.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/fmcib/preprocessing/__init__.py` & `foundation_cancer_image_biomarker-0.0.1a5/fmcib/preprocessing/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import monai
 import torchvision
 from loguru import logger
 from monai import transforms as monai_transforms
 
 from .seed_based_crop import SeedBasedPatchCropd
 
+monai.data.set_track_meta(True)
+
 T = monai_transforms.Compose(
     [
-        monai_transforms.LoadImaged(keys=["image_path"], image_only=True, reader="ITKReader"),
-        monai_transforms.EnsureChannelFirstd(keys=["image_path"]),
+        monai_transforms.LoadImaged(keys=["image_path"], image_only=True, reader="ITKReader", ensure_channel_first=True),
         monai_transforms.Spacingd(keys=["image_path"], pixdim=1, mode="bilinear", align_corners=True, diagonal=True),
         monai_transforms.ScaleIntensityRanged(keys=["image_path"], a_min=-1024, a_max=3072, b_min=0.0, b_max=1.0, clip=True),
         monai_transforms.Orientationd(keys=["image_path"], axcodes="LPS"),
         SeedBasedPatchCropd(keys=["image_path"], roi_size=(50, 50, 50), coord_orientation="LPS", global_coordinates=True),
         monai_transforms.Transposed(keys=["image_path"], indices=(0, 3, 2, 1)),
         monai_transforms.SpatialPadd(keys=["image_path"], spatial_size=(50, 50, 50)),
         torchvision.transforms.Lambda(lambda x: x["image_path"].as_tensor()),
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/fmcib/preprocessing/seed_based_crop.py` & `foundation_cancer_image_biomarker-0.0.1a5/fmcib/preprocessing/seed_based_crop.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/fmcib/run.py` & `foundation_cancer_image_biomarker-0.0.1a5/fmcib/run.py`

 * *Files 7% similar despite different names*

```diff
@@ -18,17 +18,14 @@
     feature_list = []
     logger.info("Running inference over batches ...")
 
     for batch in tqdm(dataloader, total=len(dataloader)):
         feature = model(batch.to(device)).detach().cpu().numpy()
         feature_list.append(feature)
 
-        if len(feature_list) == 1:
-            break
-
     features = np.concatenate(feature_list, axis=0)
     # Flatten features into a list
     features = features.reshape(-1, 4096)
 
     # Add the features to the dataframe
     df = pd.concat([df, pd.DataFrame(features)], axis=1)
     return df
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/losses/ntxent_mined_loss.py` & `foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/losses/ntxent_mined_loss.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/models/exneg_simclr.py` & `foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/models/exneg_simclr.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/models/load_pretrained_resnet.py` & `foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/models/load_pretrained_resnet.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/optimizers/lars.py` & `foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/optimizers/lars.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/transforms/duplicate.py` & `foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/transforms/duplicate.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/fmcib/ssl/transforms/random_resized_crop.py` & `foundation_cancer_image_biomarker-0.0.1a5/fmcib/ssl/transforms/random_resized_crop.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/fmcib/utils/idc_helper.py` & `foundation_cancer_image_biomarker-0.0.1a5/fmcib/utils/idc_helper.py`

 * *Files identical despite different names*

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/pyproject.toml` & `foundation_cancer_image_biomarker-0.0.1a5/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Poetry pyproject.toml: https://python-poetry.org/docs/pyproject/
 [build-system]
 requires = ["poetry_core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "foundation-cancer-image-biomarker"
-version = "0.0.1a4"
+version = "0.0.1a5"
 description = "Official repo for Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging [INSERT DOI]"
 readme = "README.md"
 authors = ["Suraj Pai <bspai@bwh.harvard.edu>"]
 license = "MIT"
 repository = "https://github.com/AIM-Harvard/foundation-cancer-image-biomarker"
 homepage = "https://aim.hms.harvard.edu/foundation-cancer-image-biomarker"
 
@@ -31,15 +31,15 @@
   "Programming Language :: Python :: 3.9",
 ]
 
 
 
 [tool.poetry.dependencies]
 python = "^3.8"
-project-lighter = {version = "^0.0.2a2", allow-prereleases = true}
+project-lighter = {version = "^0.0.2a5", allow-prereleases = true}
 wget = "^3.2"
 google-cloud-storage = "^2.9.0"
 thedicomsort = "^1.0.1"
 dcmrtstruct2nii = "^5"
 nibabel = "^5.1.0"
 matplotlib = "^3.7.1"
 platipy = "0.4.1"
```

### Comparing `foundation_cancer_image_biomarker-0.0.1a4/PKG-INFO` & `foundation_cancer_image_biomarker-0.0.1a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: foundation-cancer-image-biomarker
-Version: 0.0.1a4
+Version: 0.0.1a5
 Summary: Official repo for Foundation Models for Quantitative Biomarker Discovery in Cancer Imaging [INSERT DOI]
 Home-page: https://aim.hms.harvard.edu/foundation-cancer-image-biomarker
 License: MIT
 Author: Suraj Pai
 Author-email: bspai@bwh.harvard.edu
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
@@ -18,15 +18,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: dcmrtstruct2nii (>=5,<6)
 Requires-Dist: google-cloud-storage (>=2.9.0,<3.0.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: nibabel (>=5.1.0,<6.0.0)
 Requires-Dist: platipy (==0.4.1)
-Requires-Dist: project-lighter (>=0.0.2a2,<0.0.3)
+Requires-Dist: project-lighter (>=0.0.2a5,<0.0.3)
 Requires-Dist: pynrrd (>=1.0.0,<2.0.0)
 Requires-Dist: thedicomsort (>=1.0.1,<2.0.0)
 Requires-Dist: wget (>=3.2,<4.0)
 Project-URL: Repository, https://github.com/AIM-Harvard/foundation-cancer-image-biomarker
 Description-Content-Type: text/markdown
 
 # Foundation Models for Quantitative Imaging Biomarker Discovery in Cancer Imaging
```

