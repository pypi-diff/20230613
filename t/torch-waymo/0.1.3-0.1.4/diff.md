# Comparing `tmp/torch_waymo-0.1.3.tar.gz` & `tmp/torch_waymo-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch_waymo-0.1.3.tar", last modified: Thu Apr 27 02:05:45 2023, max compression
+gzip compressed data, was "torch_waymo-0.1.4.tar", last modified: Tue Jun 13 14:54:00 2023, max compression
```

## Comparing `torch_waymo-0.1.3.tar` & `torch_waymo-0.1.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-04-27 02:05:45.263885 torch_waymo-0.1.3/
--rw-r--r--   0 william   (1000) william   (1000)     1078 2023-01-31 16:43:26.000000 torch_waymo-0.1.3/LICENSE
--rw-r--r--   0 william   (1000) william   (1000)     2076 2023-04-27 02:05:45.263885 torch_waymo-0.1.3/PKG-INFO
--rw-r--r--   0 william   (1000) william   (1000)     1507 2023-01-31 18:53:42.000000 torch_waymo-0.1.3/README.md
--rw-r--r--   0 william   (1000) william   (1000)      847 2023-04-27 02:05:26.000000 torch_waymo-0.1.3/pyproject.toml
--rw-r--r--   0 william   (1000) william   (1000)       38 2023-04-27 02:05:45.263885 torch_waymo-0.1.3/setup.cfg
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-04-27 02:05:45.260552 torch_waymo-0.1.3/src/
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-04-27 02:05:45.260552 torch_waymo-0.1.3/src/torch_waymo/
--rw-r--r--   0 william   (1000) william   (1000)      102 2023-01-31 18:05:50.000000 torch_waymo-0.1.3/src/torch_waymo/__init__.py
--rw-r--r--   0 william   (1000) william   (1000)     3449 2023-01-31 18:19:13.000000 torch_waymo-0.1.3/src/torch_waymo/convert_waymo.py
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-04-27 02:05:45.260552 torch_waymo-0.1.3/src/torch_waymo/dataset/
--rw-r--r--   0 william   (1000) william   (1000)        0 2023-01-11 14:53:42.000000 torch_waymo-0.1.3/src/torch_waymo/dataset/__init__.py
--rw-r--r--   0 william   (1000) william   (1000)      355 2023-01-31 18:09:13.000000 torch_waymo-0.1.3/src/torch_waymo/dataset/simplified_frame.py
--rw-r--r--   0 william   (1000) william   (1000)     1296 2023-01-31 18:09:13.000000 torch_waymo-0.1.3/src/torch_waymo/dataset/waymo_dataset.py
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-04-27 02:05:45.263885 torch_waymo-0.1.3/src/torch_waymo/protocol/
--rw-r--r--   0 william   (1000) william   (1000)        0 2023-01-10 18:59:44.000000 torch_waymo-0.1.3/src/torch_waymo/protocol/__init__.py
--rw-r--r--   0 william   (1000) william   (1000)     4456 2023-01-31 18:09:13.000000 torch_waymo-0.1.3/src/torch_waymo/protocol/dataset_proto.py
--rw-r--r--   0 william   (1000) william   (1000)     1753 2023-01-31 18:09:13.000000 torch_waymo-0.1.3/src/torch_waymo/protocol/keypoint_proto.py
--rw-r--r--   0 william   (1000) william   (1000)     1647 2023-01-31 18:09:13.000000 torch_waymo-0.1.3/src/torch_waymo/protocol/label_proto.py
--rw-r--r--   0 william   (1000) william   (1000)      281 2023-01-24 23:52:49.000000 torch_waymo-0.1.3/src/torch_waymo/protocol/utils.py
-drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-04-27 02:05:45.260552 torch_waymo-0.1.3/src/torch_waymo.egg-info/
--rw-r--r--   0 william   (1000) william   (1000)     2076 2023-04-27 02:05:45.000000 torch_waymo-0.1.3/src/torch_waymo.egg-info/PKG-INFO
--rw-r--r--   0 william   (1000) william   (1000)      646 2023-04-27 02:05:45.000000 torch_waymo-0.1.3/src/torch_waymo.egg-info/SOURCES.txt
--rw-r--r--   0 william   (1000) william   (1000)        1 2023-04-27 02:05:45.000000 torch_waymo-0.1.3/src/torch_waymo.egg-info/dependency_links.txt
--rw-r--r--   0 william   (1000) william   (1000)       71 2023-04-27 02:05:45.000000 torch_waymo-0.1.3/src/torch_waymo.egg-info/entry_points.txt
--rw-r--r--   0 william   (1000) william   (1000)       71 2023-04-27 02:05:45.000000 torch_waymo-0.1.3/src/torch_waymo.egg-info/requires.txt
--rw-r--r--   0 william   (1000) william   (1000)       12 2023-04-27 02:05:45.000000 torch_waymo-0.1.3/src/torch_waymo.egg-info/top_level.txt
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-06-13 14:54:00.250399 torch_waymo-0.1.4/
+-rw-r--r--   0 william   (1000) william   (1000)     1078 2023-06-13 12:38:59.000000 torch_waymo-0.1.4/LICENSE
+-rw-r--r--   0 william   (1000) william   (1000)     2076 2023-06-13 14:54:00.250399 torch_waymo-0.1.4/PKG-INFO
+-rw-r--r--   0 william   (1000) william   (1000)     1507 2023-06-13 12:38:59.000000 torch_waymo-0.1.4/README.md
+-rw-r--r--   0 william   (1000) william   (1000)      894 2023-06-13 14:53:15.000000 torch_waymo-0.1.4/pyproject.toml
+-rw-r--r--   0 william   (1000) william   (1000)       38 2023-06-13 14:54:00.250399 torch_waymo-0.1.4/setup.cfg
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-06-13 14:54:00.247066 torch_waymo-0.1.4/src/
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-06-13 14:54:00.247066 torch_waymo-0.1.4/src/torch_waymo/
+-rw-r--r--   0 william   (1000) william   (1000)      102 2023-06-13 12:38:59.000000 torch_waymo-0.1.4/src/torch_waymo/__init__.py
+-rw-r--r--   0 william   (1000) william   (1000)     3535 2023-06-13 12:38:59.000000 torch_waymo-0.1.4/src/torch_waymo/convert_waymo.py
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-06-13 14:54:00.250399 torch_waymo-0.1.4/src/torch_waymo/dataset/
+-rw-r--r--   0 william   (1000) william   (1000)        0 2023-06-13 12:38:59.000000 torch_waymo-0.1.4/src/torch_waymo/dataset/__init__.py
+-rw-r--r--   0 william   (1000) william   (1000)      355 2023-06-13 12:38:59.000000 torch_waymo-0.1.4/src/torch_waymo/dataset/simplified_frame.py
+-rw-r--r--   0 william   (1000) william   (1000)     1297 2023-06-13 14:47:34.000000 torch_waymo-0.1.4/src/torch_waymo/dataset/waymo_dataset.py
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-06-13 14:54:00.250399 torch_waymo-0.1.4/src/torch_waymo/protocol/
+-rw-r--r--   0 william   (1000) william   (1000)        0 2023-06-13 12:38:59.000000 torch_waymo-0.1.4/src/torch_waymo/protocol/__init__.py
+-rw-r--r--   0 william   (1000) william   (1000)     4422 2023-06-13 12:38:59.000000 torch_waymo-0.1.4/src/torch_waymo/protocol/dataset_proto.py
+-rw-r--r--   0 william   (1000) william   (1000)     1753 2023-06-13 12:38:59.000000 torch_waymo-0.1.4/src/torch_waymo/protocol/keypoint_proto.py
+-rw-r--r--   0 william   (1000) william   (1000)     1647 2023-06-13 12:38:59.000000 torch_waymo-0.1.4/src/torch_waymo/protocol/label_proto.py
+-rw-r--r--   0 william   (1000) william   (1000)      281 2023-06-13 12:38:59.000000 torch_waymo-0.1.4/src/torch_waymo/protocol/utils.py
+drwxr-xr-x   0 william   (1000) william   (1000)        0 2023-06-13 14:54:00.250399 torch_waymo-0.1.4/src/torch_waymo.egg-info/
+-rw-r--r--   0 william   (1000) william   (1000)     2076 2023-06-13 14:54:00.000000 torch_waymo-0.1.4/src/torch_waymo.egg-info/PKG-INFO
+-rw-r--r--   0 william   (1000) william   (1000)      646 2023-06-13 14:54:00.000000 torch_waymo-0.1.4/src/torch_waymo.egg-info/SOURCES.txt
+-rw-r--r--   0 william   (1000) william   (1000)        1 2023-06-13 14:54:00.000000 torch_waymo-0.1.4/src/torch_waymo.egg-info/dependency_links.txt
+-rw-r--r--   0 william   (1000) william   (1000)       71 2023-06-13 14:54:00.000000 torch_waymo-0.1.4/src/torch_waymo.egg-info/entry_points.txt
+-rw-r--r--   0 william   (1000) william   (1000)       71 2023-06-13 14:54:00.000000 torch_waymo-0.1.4/src/torch_waymo.egg-info/requires.txt
+-rw-r--r--   0 william   (1000) william   (1000)       12 2023-06-13 14:54:00.000000 torch_waymo-0.1.4/src/torch_waymo.egg-info/top_level.txt
```

### Comparing `torch_waymo-0.1.3/LICENSE` & `torch_waymo-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torch_waymo-0.1.3/PKG-INFO` & `torch_waymo-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch_waymo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Load Waymo Open Dataset in PyTorch
 Author-email: William Guimont-Martin <william.guimont-martin.1@ulaval.ca>
 Project-URL: Homepage, https://github.com/willGuimont/torch_waymo
 Project-URL: Bug Tracker, https://github.com/willGuimont/torch_waymo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `torch_waymo-0.1.3/README.md` & `torch_waymo-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `torch_waymo-0.1.3/pyproject.toml` & `torch_waymo-0.1.4/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "torch_waymo"
-version = "0.1.3"
+version = "0.1.4"
 authors = [
     { name = "William Guimont-Martin", email = "william.guimont-martin.1@ulaval.ca" },
 ]
 description = "Load Waymo Open Dataset in PyTorch"
 readme = "README.md"
 requires-python = ">=3.7"
-dependencies = [
-    'tqdm',
-    'torch',
-    'numpy',
-]
+dependencies = ["tqdm", "torch", "numpy"]
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 [project.optional-dependencies]
 waymo = ["waymo-open-dataset-tf-2-6-0", "protobuf==3.20.0"]
 [project.urls]
 "Homepage" = "https://github.com/willGuimont/torch_waymo"
 "Bug Tracker" = "https://github.com/willGuimont/torch_waymo/issues"
 [project.scripts]
 torch-waymo-convert = "torch_waymo.convert_waymo:main"
+[tool.black]
+line-length = 120
+[tool.isort]
+profile = "black"
```

### Comparing `torch_waymo-0.1.3/src/torch_waymo/convert_waymo.py` & `torch_waymo-0.1.4/src/torch_waymo/convert_waymo.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,92 +2,115 @@
 import pathlib
 import pickle
 
 import tensorflow.compat.v1 as tf
 
 tf.enable_eager_execution()
 import tqdm
+from waymo_open_dataset import dataset_pb2 as open_dataset
+from waymo_open_dataset.utils import frame_utils
 
 from . import SimplifiedFrame
 from .protocol import dataset_proto
 from .protocol.dataset_proto import Frame
 
-from waymo_open_dataset import dataset_pb2 as open_dataset
-from waymo_open_dataset.utils import frame_utils
-
 
 def generate_cache(root_path: pathlib.Path, split: str):
     split_path = root_path.joinpath(split)
-    split_cache_path = root_path.joinpath('converted').joinpath(split)
+    split_cache_path = root_path.joinpath("converted").joinpath(split)
 
     split_path.mkdir(parents=True, exist_ok=True)
     split_cache_path.mkdir(parents=True, exist_ok=True)
 
     # Cache sequence lengths
     sequence_paths = sorted(list(split_path.iterdir()))
     seq_lens = _cache_seq_lens(sequence_paths, split_cache_path)
 
     # Generate the new dataset
     frame_count = 0
     for seq_idx, seq_len in tqdm.tqdm(enumerate(seq_lens), total=len(seq_lens)):
         seq_path = sequence_paths[seq_idx]
-        seq = tf.data.TFRecordDataset(seq_path, compression_type='')
+        seq = tf.data.TFRecordDataset(seq_path, compression_type="")
         for data in seq:
-            frame_path = split_cache_path.joinpath(f'{frame_count}.pkl')
+            frame_path = split_cache_path.joinpath(f"{frame_count}.pkl")
             frame_count += 1
             if not frame_path.exists():
                 simple_frame = _load_frame(data)
-                with open(frame_path, 'wb') as f:
+                with open(frame_path, "wb") as f:
                     pickle.dump(simple_frame, f)
 
 
 def _cache_seq_lens(sequence_paths, split_cache_path):
-    seq_len_cache_path = split_cache_path.joinpath('len.pkl')
+    seq_len_cache_path = split_cache_path.joinpath("len.pkl")
     if seq_len_cache_path.exists():
-        with open(seq_len_cache_path, 'rb') as f:
+        with open(seq_len_cache_path, "rb") as f:
             seq_lens = pickle.load(f)
     else:
-        print('Computing sequence lengths, might take a while')
-        seq_lens = list(
-            tqdm.tqdm((_get_size(s) for s in sequence_paths), total=len(sequence_paths)))
-        with open(seq_len_cache_path, 'wb') as f:
+        print("Computing sequence lengths, might take a while")
+        seq_lens = list(tqdm.tqdm((_get_size(s) for s in sequence_paths), total=len(sequence_paths)))
+        with open(seq_len_cache_path, "wb") as f:
             pickle.dump(seq_lens, f)
     return seq_lens
 
 
 def _get_size(s: pathlib.Path) -> int:
-    return sum(1 for _ in tf.data.TFRecordDataset(s, compression_type=''))
+    return sum(1 for _ in tf.data.TFRecordDataset(s, compression_type=""))
 
 
 def _load_frame(data):
     frame = open_dataset.Frame()
     frame.ParseFromString(bytearray(data.numpy()))
-    (range_images, camera_projections, _,
-     range_image_top_pose) = frame_utils.parse_range_image_and_camera_projection(frame)
+    (
+        range_images,
+        camera_projections,
+        _,
+        range_image_top_pose,
+    ) = frame_utils.parse_range_image_and_camera_projection(frame)
     points, cp_points = frame_utils.convert_range_image_to_point_cloud(
-        frame, range_images, camera_projections, range_image_top_pose)
+        frame, range_images, camera_projections, range_image_top_pose
+    )
     clean_frame = dataset_proto.from_data(Frame, frame)
-    simple_frame = SimplifiedFrame(clean_frame.context, clean_frame.timestamp_micros, clean_frame.pose,
-                                   clean_frame.laser_labels, clean_frame.no_label_zones, points)
+    simple_frame = SimplifiedFrame(
+        clean_frame.context,
+        clean_frame.timestamp_micros,
+        clean_frame.pose,
+        clean_frame.laser_labels,
+        clean_frame.no_label_zones,
+        points,
+    )
     return simple_frame
 
 
-SPLITS = ['training', 'validation', 'testing']
+SPLITS = ["training", "validation", "testing"]
 
 
 def main():
-    global parser, args, split
-    parser = argparse.ArgumentParser(prog='Convert Waymo',
-                                     description='Convert the Waymo Open Dataset to remove all dependencies to Tensorflow')
-    parser.add_argument('-d', '--dataset', type=str, required=True, help='Path to the Waymo Open Dataset')
-    parser.add_argument('-s', '--splits', type=str, choices=SPLITS,
-                        nargs='+', default=SPLITS, help='Specify the splits you want to process')
+    parser = argparse.ArgumentParser(
+        prog="Convert Waymo",
+        description="Convert the Waymo Open Dataset to remove all dependencies to Tensorflow",
+    )
+    parser.add_argument(
+        "-d",
+        "--dataset",
+        type=str,
+        required=True,
+        help="Path to the Waymo Open Dataset",
+    )
+    parser.add_argument(
+        "-s",
+        "--splits",
+        type=str,
+        choices=SPLITS,
+        nargs="+",
+        default=SPLITS,
+        help="Specify the splits you want to process",
+    )
     args = parser.parse_args()
     dataset_path = pathlib.Path(args.dataset)
     splits = args.splits
     for split in splits:
-        print(f'Processing {split}...')
+        print(f"Processing {split}...")
         generate_cache(dataset_path, split)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `torch_waymo-0.1.3/src/torch_waymo/dataset/waymo_dataset.py` & `torch_waymo-0.1.4/src/torch_waymo/dataset/waymo_dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,30 +10,30 @@
 class WaymoDataset(Dataset):
     def __init__(self, root_path: str, split: str, transform: Optional[Callable] = None):
         self._root_path = pathlib.Path(root_path).expanduser()
         self._split = split
         self._split_path = self._root_path.joinpath(split)
         self._transform = transform
 
-        self._seq_len_cache_path = self._split_path.joinpath('len.pkl')
+        self._seq_len_cache_path = self._split_path.joinpath("len.pkl")
         if self._seq_len_cache_path.exists():
-            with open(self._seq_len_cache_path, 'rb') as f:
+            with open(self._seq_len_cache_path, "rb") as f:
                 self._seq_lens = pickle.load(f)
         else:
-            raise RuntimeError(f'Could not find {self._seq_len_cache_path}')
+            raise RuntimeError(f"Could not find {self._seq_len_cache_path}")
 
     def __len__(self) -> int:
-        return self._seq_lens[-1]
+        return sum(self._seq_lens)
 
     def __getitem__(self, idx: int) -> SimplifiedFrame:
-        path = self._split_path.joinpath(f'{idx}.pkl')
+        path = self._split_path.joinpath(f"{idx}.pkl")
         if path.exists():
             return self._get_frame(path)
         else:
-            raise IndexError(f'Could not load frame at index {idx}')
+            raise IndexError(f"Could not load frame at index {idx}")
 
     def _get_frame(self, path):
-        with open(path, 'rb') as f:
+        with open(path, "rb") as f:
             x = pickle.load(f)
         if self._transform is not None:
             x = self._transform(x)
         return x
```

### Comparing `torch_waymo-0.1.3/src/torch_waymo/protocol/dataset_proto.py` & `torch_waymo-0.1.4/src/torch_waymo/protocol/dataset_proto.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,33 +5,39 @@
 from dataclasses import dataclass, fields, is_dataclass
 
 import numpy as np
 
 from .label_proto import Type, Label, Polygon2dProto
 from .utils import ReversibleIntEnum
 
-T = typing.TypeVar('T')
+T = typing.TypeVar("T")
 
 
 def fullname(o):
     klass = o.__class__
     module = klass.__module__
-    if module == 'builtins':
+    if module == "builtins":
         return klass.__qualname__  # avoid outputs like 'builtins.str'
-    return module + '.' + klass.__qualname__
+    return module + "." + klass.__qualname__
 
 
 def from_data(cls: typing.Type[T], data) -> T:
     from waymo_open_dataset import dataset_pb2
-    from google.protobuf.pyext._message import RepeatedCompositeContainer, RepeatedScalarContainer
+    from google.protobuf.pyext._message import (
+        RepeatedCompositeContainer,
+        RepeatedScalarContainer,
+    )
 
     if isinstance(data, dataset_pb2.Transform):
         return np.array(data.transform).reshape((4, 4))
-    if isinstance(data, list) or isinstance(data, RepeatedCompositeContainer) or isinstance(data,
-                                                                                            RepeatedScalarContainer):
+    if (
+        isinstance(data, list)
+        or isinstance(data, RepeatedCompositeContainer)
+        or isinstance(data, RepeatedScalarContainer)
+    ):
         return [from_data(cls[0], d) for d in data]
     if not is_dataclass(cls):
         return data
 
     field_names = [f.name for f in fields(cls)]
     field_types = {f.name: f.type for f in fields(cls)}
 
@@ -132,14 +138,15 @@
 
 
 @dataclass
 class RangeImage:
     """
     *_compressed are compressed using Zlib (val = ZlibDecompress(range_image_compressed))
     """
+
     range_image_compressed: np.ndarray
     camera_projection_compressed: np.ndarray
     range_image_pose_compressed: np.ndarray
     range_image_flow_compressed: np.ndarray
     segmentation_label_compressed: np.ndarray
```

### Comparing `torch_waymo-0.1.3/src/torch_waymo/protocol/keypoint_proto.py` & `torch_waymo-0.1.4/src/torch_waymo/protocol/keypoint_proto.py`

 * *Files identical despite different names*

### Comparing `torch_waymo-0.1.3/src/torch_waymo/protocol/label_proto.py` & `torch_waymo-0.1.4/src/torch_waymo/protocol/label_proto.py`

 * *Files identical despite different names*

### Comparing `torch_waymo-0.1.3/src/torch_waymo.egg-info/PKG-INFO` & `torch_waymo-0.1.4/src/torch_waymo.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-waymo
-Version: 0.1.3
+Version: 0.1.4
 Summary: Load Waymo Open Dataset in PyTorch
 Author-email: William Guimont-Martin <william.guimont-martin.1@ulaval.ca>
 Project-URL: Homepage, https://github.com/willGuimont/torch_waymo
 Project-URL: Bug Tracker, https://github.com/willGuimont/torch_waymo/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `torch_waymo-0.1.3/src/torch_waymo.egg-info/SOURCES.txt` & `torch_waymo-0.1.4/src/torch_waymo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

