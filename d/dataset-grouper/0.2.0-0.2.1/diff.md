# Comparing `tmp/dataset_grouper-0.2.0.tar.gz` & `tmp/dataset_grouper-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataset_grouper-0.2.0.tar", last modified: Mon Jun 12 21:55:22 2023, max compression
+gzip compressed data, was "dataset_grouper-0.2.1.tar", last modified: Tue Jun 13 02:36:15 2023, max compression
```

## Comparing `dataset_grouper-0.2.0.tar` & `dataset_grouper-0.2.1.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxr-x---   0 zachcharles (709374) primarygroup (89939)        0 2023-06-12 21:55:22.404136 dataset_grouper-0.2.0/
-drwxr-x---   0 zachcharles (709374) primarygroup (89939)        0 2023-06-12 21:55:22.400136 dataset_grouper-0.2.0/.github/
-drwxr-x---   0 zachcharles (709374) primarygroup (89939)        0 2023-06-12 21:55:22.400136 dataset_grouper-0.2.0/.github/workflows/
--rw-r-----   0 zachcharles (709374) primarygroup (89939)      758 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/.github/workflows/pytest_and_autopublish.yml
--rw-r-----   0 zachcharles (709374) primarygroup (89939)      721 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/.gitignore
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     1155 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/CHANGELOG.md
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     1103 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/CONTRIBUTING.md
--rw-r-----   0 zachcharles (709374) primarygroup (89939)    11357 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/LICENSE
--rw-r-----   0 zachcharles (709374) primarygroup (89939)    14604 2023-06-12 21:55:22.404136 dataset_grouper-0.2.0/PKG-INFO
--rw-r-----   0 zachcharles (709374) primarygroup (89939)      901 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/README.md
-drwxr-x---   0 zachcharles (709374) primarygroup (89939)        0 2023-06-12 21:55:22.400136 dataset_grouper-0.2.0/dataset_grouper/
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     1092 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/dataset_grouper/__init__.py
-drwxr-x---   0 zachcharles (709374) primarygroup (89939)        0 2023-06-12 21:55:22.404136 dataset_grouper-0.2.0/dataset_grouper/core/
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     4509 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/dataset_grouper/core/beam_transforms.py
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     8461 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/dataset_grouper/core/beam_transforms_test.py
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     2323 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/dataset_grouper/core/count_utils.py
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     2979 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/dataset_grouper/core/count_utils_test.py
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     5171 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/dataset_grouper/core/data_loaders.py
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     2082 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/dataset_grouper/core/serialization.py
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     2427 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/dataset_grouper/core/serialization_test.py
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     2137 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/dataset_grouper/core/tf_utils.py
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     4222 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/dataset_grouper/core/tf_utils_test.py
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     5440 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/dataset_grouper/core/tfds_pipelines.py
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     1039 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/dataset_grouper/core/types.py
-drwxr-x---   0 zachcharles (709374) primarygroup (89939)        0 2023-06-12 21:55:22.400136 dataset_grouper-0.2.0/dataset_grouper.egg-info/
--rw-r-----   0 zachcharles (709374) primarygroup (89939)    14604 2023-06-12 21:55:22.000000 dataset_grouper-0.2.0/dataset_grouper.egg-info/PKG-INFO
--rw-r-----   0 zachcharles (709374) primarygroup (89939)      759 2023-06-12 21:55:22.000000 dataset_grouper-0.2.0/dataset_grouper.egg-info/SOURCES.txt
--rw-r-----   0 zachcharles (709374) primarygroup (89939)        1 2023-06-12 21:55:22.000000 dataset_grouper-0.2.0/dataset_grouper.egg-info/dependency_links.txt
--rw-r-----   0 zachcharles (709374) primarygroup (89939)      120 2023-06-12 21:55:22.000000 dataset_grouper-0.2.0/dataset_grouper.egg-info/requires.txt
--rw-r-----   0 zachcharles (709374) primarygroup (89939)       16 2023-06-12 21:55:22.000000 dataset_grouper-0.2.0/dataset_grouper.egg-info/top_level.txt
--rw-r-----   0 zachcharles (709374) primarygroup (89939)     1559 2023-06-12 21:51:05.000000 dataset_grouper-0.2.0/pyproject.toml
--rw-r-----   0 zachcharles (709374) primarygroup (89939)       38 2023-06-12 21:55:22.404136 dataset_grouper-0.2.0/setup.cfg
+drwxr-x---   0 zachcharles (709374) primarygroup (89939)        0 2023-06-13 02:36:15.464492 dataset_grouper-0.2.1/
+drwxr-x---   0 zachcharles (709374) primarygroup (89939)        0 2023-06-13 02:36:15.460492 dataset_grouper-0.2.1/.github/
+drwxr-x---   0 zachcharles (709374) primarygroup (89939)        0 2023-06-13 02:36:15.460492 dataset_grouper-0.2.1/.github/workflows/
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)      758 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/.github/workflows/pytest_and_autopublish.yml
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)      721 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/.gitignore
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     1365 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/CHANGELOG.md
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     1103 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/CONTRIBUTING.md
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)    11357 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/LICENSE
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)    14604 2023-06-13 02:36:15.464492 dataset_grouper-0.2.1/PKG-INFO
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)      901 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/README.md
+drwxr-x---   0 zachcharles (709374) primarygroup (89939)        0 2023-06-13 02:36:15.460492 dataset_grouper-0.2.1/dataset_grouper/
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     1092 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/dataset_grouper/__init__.py
+drwxr-x---   0 zachcharles (709374) primarygroup (89939)        0 2023-06-13 02:36:15.464492 dataset_grouper-0.2.1/dataset_grouper/core/
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     4509 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/dataset_grouper/core/beam_transforms.py
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     8461 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/dataset_grouper/core/beam_transforms_test.py
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     2323 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/dataset_grouper/core/count_utils.py
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     2979 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/dataset_grouper/core/count_utils_test.py
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     5171 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/dataset_grouper/core/data_loaders.py
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     2249 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/dataset_grouper/core/integration_test.py
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     2082 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/dataset_grouper/core/serialization.py
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     2427 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/dataset_grouper/core/serialization_test.py
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     2137 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/dataset_grouper/core/tf_utils.py
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     4222 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/dataset_grouper/core/tf_utils_test.py
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     5410 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/dataset_grouper/core/tfds_pipelines.py
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     1039 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/dataset_grouper/core/types.py
+drwxr-x---   0 zachcharles (709374) primarygroup (89939)        0 2023-06-13 02:36:15.460492 dataset_grouper-0.2.1/dataset_grouper.egg-info/
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)    14604 2023-06-13 02:36:15.000000 dataset_grouper-0.2.1/dataset_grouper.egg-info/PKG-INFO
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)      800 2023-06-13 02:36:15.000000 dataset_grouper-0.2.1/dataset_grouper.egg-info/SOURCES.txt
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)        1 2023-06-13 02:36:15.000000 dataset_grouper-0.2.1/dataset_grouper.egg-info/dependency_links.txt
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)      120 2023-06-13 02:36:15.000000 dataset_grouper-0.2.1/dataset_grouper.egg-info/requires.txt
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)       16 2023-06-13 02:36:15.000000 dataset_grouper-0.2.1/dataset_grouper.egg-info/top_level.txt
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)     1559 2023-06-13 02:35:01.000000 dataset_grouper-0.2.1/pyproject.toml
+-rw-r-----   0 zachcharles (709374) primarygroup (89939)       38 2023-06-13 02:36:15.464492 dataset_grouper-0.2.1/setup.cfg
```

### Comparing `dataset_grouper-0.2.0/.github/workflows/pytest_and_autopublish.yml` & `dataset_grouper-0.2.1/.github/workflows/pytest_and_autopublish.yml`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/.gitignore` & `dataset_grouper-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/CHANGELOG.md` & `dataset_grouper-0.2.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -19,20 +19,25 @@
   `[2.0.0]: https://github.com/google-research/dataset_grouper/compare/v1.0.0...v2.0.0`
   * Update the `[Unreleased]` url: `v1.0.0...HEAD` -> `v2.0.0...HEAD`
 
 -->
 
 ## [Unreleased]
 
+## [0.2.1] - 2023-06-12
+
+* Fixed bug where beam pipelines would not work with datasets that were not globally prepared.
+
 ## [0.2.0] - 2023-06-12
 
 * Improved parallelism in Beam pipelines to speed up dataset grouping.
 * Updated pyproject.toml file for initial PyPI release.
 * Added more detailed README file.
 
 ## [0.1.0] - 2023-05-31
 
 * Initial release
 
-[Unreleased]: https://github.com/google-research/dataset_grouper/compare/v0.2.0...HEAD
+[Unreleased]: https://github.com/google-research/dataset_grouper/compare/v0.2.1...HEAD
+[0.2.1]: https://github.com/google-research/dataset_grouper/releases/tag/v0.2.0...v0.2.1
 [0.2.0]: https://github.com/google-research/dataset_grouper/releases/tag/v0.1.0...v0.2.0
 [0.1.0]: https://github.com/google-research/dataset_grouper/releases/tag/v0.1.0
```

### Comparing `dataset_grouper-0.2.0/CONTRIBUTING.md` & `dataset_grouper-0.2.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/LICENSE` & `dataset_grouper-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/PKG-INFO` & `dataset_grouper-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset_grouper
-Version: 0.2.0
+Version: 0.2.1
 Summary: Dataset Grouper - A library for datasets with group-level structure.
 Author-email: Dataset Grouper Team <dataset-grouper-dev@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `dataset_grouper-0.2.0/README.md` & `dataset_grouper-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/dataset_grouper/__init__.py` & `dataset_grouper-0.2.1/dataset_grouper/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Dataset Grouper API."""
 
 # A new PyPI release will be pushed everytime `__version__` is increased
 # When changing this, also move the unreleased changes in CHANGELOG.md to the
 # associated version.
-__version__ = '0.2.0'
+__version__ = '0.2.1'
 
 
 from dataset_grouper.core.data_loaders import PartitionedDataset
 from dataset_grouper.core.tfds_pipelines import tfds_group_counts
 from dataset_grouper.core.tfds_pipelines import tfds_to_tfrecords
 from dataset_grouper.core.types import Example
 from dataset_grouper.core.types import GetKeyFn
```

### Comparing `dataset_grouper-0.2.0/dataset_grouper/core/beam_transforms.py` & `dataset_grouper-0.2.1/dataset_grouper/core/beam_transforms.py`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/dataset_grouper/core/beam_transforms_test.py` & `dataset_grouper-0.2.1/dataset_grouper/core/beam_transforms_test.py`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/dataset_grouper/core/count_utils.py` & `dataset_grouper-0.2.1/dataset_grouper/core/count_utils.py`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/dataset_grouper/core/count_utils_test.py` & `dataset_grouper-0.2.1/dataset_grouper/core/count_utils_test.py`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/dataset_grouper/core/data_loaders.py` & `dataset_grouper-0.2.1/dataset_grouper/core/data_loaders.py`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/dataset_grouper/core/serialization.py` & `dataset_grouper-0.2.1/dataset_grouper/core/serialization.py`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/dataset_grouper/core/serialization_test.py` & `dataset_grouper-0.2.1/dataset_grouper/core/serialization_test.py`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/dataset_grouper/core/tf_utils.py` & `dataset_grouper-0.2.1/dataset_grouper/core/tf_utils.py`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/dataset_grouper/core/tf_utils_test.py` & `dataset_grouper-0.2.1/dataset_grouper/core/tf_utils_test.py`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/dataset_grouper/core/tfds_pipelines.py` & `dataset_grouper-0.2.1/dataset_grouper/core/tfds_pipelines.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,49 +19,48 @@
 from dataset_grouper.core import beam_transforms
 from dataset_grouper.core import types
 import tensorflow as tf
 import tensorflow_datasets as tfds
 
 
 def tfds_to_tfrecords(
-    dataset_name: str,
+    dataset_builder: tfds.core.DatasetBuilder,
     split: str,
     file_path_prefix: str,
     get_key_fn: types.GetKeyFn,
     file_name_suffix: str = '',
     num_shards: Optional[int] = None,
 ) -> beam.Pipeline:
   """Builds a Beam pipeline that partitions a TFDS partitions to TFRecords.
 
   The pipeline will partition the dataset across groups. Each group corresponds
   to a distinct output of the `get_key_fn`, which is applied to each tensor of
   the TFDS dataset specified. The TFDS examples for each group are serialized
   in a single `tf.train.SequenceExample`, and written to TFRecords.
 
   Args:
-    dataset_name: The name of the TFDS dataset to partition.
+    dataset_builder: A `tfds.core.DatasetBuilder` to get examples from.
     split: Which split of the dataset should be used.
     file_path_prefix: The file path to write to. The TFRecords files written
       will begin with this prefix, followed by a shard identifier, and a common
       extension (if `file_name_suffix` is provided).
     get_key_fn: A function that takes as input an example from the TFDS dataset
       specified, and that returns bytes identifying the group it belongs to.
     file_name_suffix: A common suffix for the files written.
     num_shards: The number of files (shards) used for output. If not set, the
       number of shards will be automatically set.
 
   Returns:
     A `beam.Pipeline`.
   """
-  tfds_builder = tfds.builder(dataset_name)
-  features_dict = tfds_builder.info.features
+  features_dict = dataset_builder.info.features
 
   def pipeline(root) -> None:
     examples = root | 'ReadTFDS' >> tfds.beam.ReadFromTFDS(
-        tfds_builder, split=split
+        dataset_builder, split=split
     )
     keyed_sequence_examples = beam_transforms.to_keyed_sequence_examples(
         examples, get_key_fn, features_dict
     )
     sequence_examples = keyed_sequence_examples | 'RemoveKey' >> beam.Map(
         lambda x: x[1]
     )
@@ -76,15 +75,15 @@
         )
     )
 
   return pipeline
 
 
 def tfds_group_counts(
-    dataset_name: str,
+    dataset_builder: tfds.core.DatasetBuilder,
     split: str,
     file_path_prefix: str,
     get_key_fn: types.GetKeyFn,
     file_name_suffix: str = '',
     num_shards: Optional[int] = None,
     delimiter: str = ',',
 ) -> beam.Pipeline:
@@ -103,15 +102,15 @@
   only consider string-valued features when computing this statistic, and assume
   that words are separated by ' '.
 
   Note that you can delimit statistics by something other than a comma via the
   `delimiter` argument.
 
   Args:
-    dataset_name: The name of the TFDS dataset to partition.
+    dataset_builder: A `tfds.core.DatasetBuilder`.
     split: Which split of the dataset should be used.
     file_path_prefix: The file path to write to. The output files written will
       begin with this prefix, followed by a shard identifier, and a common
       extension (if `file_name_suffix` is provided).
     get_key_fn: A function that takes as input an example from the TFDS dataset
       specified, and that returns bytes identifying the group it belongs to.
     file_name_suffix: A common suffix for the files written.
@@ -119,20 +118,19 @@
       number of shards will be automatically set.
     delimiter: A string representing the delimiter to use when writing the
       statistics of a group.
 
   Returns:
     A `beam.Pipeline`.
   """
-  tfds_builder = tfds.builder(dataset_name)
   header = 'group_id,num_examples,num_bytes,num_words'
 
   def pipeline(root) -> None:
     examples = root | 'ReadTFDS' >> tfds.beam.ReadFromTFDS(
-        tfds_builder, split=split
+        dataset_builder, split=split
     )
     formatted_group_counts = beam_transforms.compute_group_counts(
         examples, get_key_fn, delimiter=delimiter
     )
     _ = formatted_group_counts | 'WriteToText' >> beam.io.WriteToText(
         file_path_prefix=file_path_prefix,
         file_name_suffix=file_name_suffix,
```

### Comparing `dataset_grouper-0.2.0/dataset_grouper/core/types.py` & `dataset_grouper-0.2.1/dataset_grouper/core/types.py`

 * *Files identical despite different names*

### Comparing `dataset_grouper-0.2.0/dataset_grouper.egg-info/PKG-INFO` & `dataset_grouper-0.2.1/dataset_grouper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataset-grouper
-Version: 0.2.0
+Version: 0.2.1
 Summary: Dataset Grouper - A library for datasets with group-level structure.
 Author-email: Dataset Grouper Team <dataset-grouper-dev@google.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `dataset_grouper-0.2.0/dataset_grouper.egg-info/SOURCES.txt` & `dataset_grouper-0.2.1/dataset_grouper.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,13 +12,14 @@
 dataset_grouper.egg-info/requires.txt
 dataset_grouper.egg-info/top_level.txt
 dataset_grouper/core/beam_transforms.py
 dataset_grouper/core/beam_transforms_test.py
 dataset_grouper/core/count_utils.py
 dataset_grouper/core/count_utils_test.py
 dataset_grouper/core/data_loaders.py
+dataset_grouper/core/integration_test.py
 dataset_grouper/core/serialization.py
 dataset_grouper/core/serialization_test.py
 dataset_grouper/core/tf_utils.py
 dataset_grouper/core/tf_utils_test.py
 dataset_grouper/core/tfds_pipelines.py
 dataset_grouper/core/types.py
```

### Comparing `dataset_grouper-0.2.0/pyproject.toml` & `dataset_grouper-0.2.1/pyproject.toml`

 * *Files identical despite different names*

