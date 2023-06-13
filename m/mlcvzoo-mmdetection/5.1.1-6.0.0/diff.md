# Comparing `tmp/mlcvzoo_mmdetection-5.1.1.tar.gz` & `tmp/mlcvzoo_mmdetection-6.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_mmdetection-5.1.1.tar", max compression
+gzip compressed data, was "mlcvzoo_mmdetection-6.0.0.tar", max compression
```

## Comparing `mlcvzoo_mmdetection-5.1.1.tar` & `mlcvzoo_mmdetection-6.0.0.tar`

### file list

```diff
@@ -1,16 +1,13 @@
--rw-r--r--   0        0        0      423 2023-05-22 10:51:20.525114 mlcvzoo_mmdetection-5.1.1/README.md
--rw-r--r--   0        0        0      177 2023-05-22 10:51:20.525114 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/__init__.py
--rw-r--r--   0        0        0     5279 2023-05-23 07:13:04.241771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/configuration.py
--rw-r--r--   0        0        0     8133 2023-05-23 07:13:04.241771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py
--rw-r--r--   0        0        0    15578 2023-05-23 07:13:04.245771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/model.py
--rw-r--r--   0        0        0     6835 2023-05-23 07:13:04.245771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/object_detection_model.py
--rw-r--r--   0        0        0      154 2023-05-22 10:51:20.525114 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/py.typed
--rw-r--r--   0        0        0     9744 2023-05-23 08:40:45.799876 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/segmentation_model.py
--rw-r--r--   0        0        0    11398 2023-05-23 07:13:04.245771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/third_party/LICENSE
--rw-r--r--   0        0        0      109 2023-05-23 07:13:04.245771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/third_party/README.md
--rw-r--r--   0        0        0      154 2023-05-23 07:13:04.245771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/third_party/__init__.py
--rw-r--r--   0        0        0     2590 2023-05-23 07:13:04.245771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/third_party/mmdetection.py
--rw-r--r--   0        0        0     2643 2023-05-23 07:13:04.245771 mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/utils.py
--rw-r--r--   0        0        0     4014 2023-05-23 09:26:31.124042 mlcvzoo_mmdetection-5.1.1/pyproject.toml
--rw-r--r--   0        0        0     1648 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-5.1.1/setup.py
--rw-r--r--   0        0        0     2078 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-5.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11412 2023-06-12 09:08:46.196127 mlcvzoo_mmdetection-6.0.0/LICENSE
+-rw-r--r--   0        0        0      423 2023-06-12 09:08:46.196127 mlcvzoo_mmdetection-6.0.0/README.md
+-rw-r--r--   0        0        0      244 2023-06-13 14:54:27.168223 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/__init__.py
+-rw-r--r--   0        0        0     5716 2023-06-13 09:14:59.550114 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/configuration.py
+-rw-r--r--   0        0        0     6817 2023-06-13 09:14:59.550114 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/mlcvzoo_mmdet_dataset.py
+-rw-r--r--   0        0        0    13641 2023-06-13 09:14:59.550114 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/model.py
+-rw-r--r--   0        0        0     7394 2023-06-12 09:08:46.196127 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/object_detection_model.py
+-rw-r--r--   0        0        0      196 2023-06-12 09:08:46.196127 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/py.typed
+-rw-r--r--   0        0        0    10928 2023-06-13 09:14:59.550114 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/segmentation_model.py
+-rw-r--r--   0        0        0     1938 2023-06-13 09:14:59.550114 mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/utils.py
+-rw-r--r--   0        0        0     4294 2023-06-13 14:54:27.172223 mlcvzoo_mmdetection-6.0.0/pyproject.toml
+-rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-6.0.0/setup.py
+-rw-r--r--   0        0        0     2081 1970-01-01 00:00:00.000000 mlcvzoo_mmdetection-6.0.0/PKG-INFO
```

### Comparing `mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/configuration.py` & `mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/configuration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,18 +1,20 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Definition of the MMDetectionConfig that is used to configure the MMDetectionModel.
 """
 
 import logging
-from typing import Any, Dict, List, Optional
+import os
+from typing import Any, Dict, Optional
 
 import related
 from attr import define
 from config_builder import BaseConfigClass
 from mlcvzoo_base.api.configuration import InferenceConfig, ModelConfiguration
 from mlcvzoo_base.configuration.class_mapping_config import ClassMappingConfig
 from mlcvzoo_base.configuration.reduction_mapping_config import ReductionMappingConfig
@@ -28,80 +30,92 @@
     def check_values(self) -> bool:
         return self.num_classes >= 1
 
 
 @define
 class MMDetectionTrainArgparseConfig(BaseConfigClass):
     __related_strict__ = True
-    # argparse parameter from mmdetection:
+    # Gathering of all argparse parameter mmdetection/tools/train.py:
 
     # train config file path
     config: str = related.StringField()
     # the dir to save logs and models
     work_dir: str = related.StringField()
-    # the checkpoint file to resume from
-    resume_from: Optional[str] = related.ChildField(
-        cls=str, required=False, default=None
-    )
-    # whether not to evaluate the checkpoint during training
-    no_validate: bool = related.BooleanField(required=False, default=False)
+    # enable automatic-mixed-precision training
+    amp: bool = related.BooleanField(default=False)
     # enable automatically scaling LR
     auto_scale_lr: bool = related.BooleanField(required=False, default=False)
-    # resume from the latest checkpoint automatically
-    auto_resume: bool = related.BooleanField(required=False, default=False)
-    # whether to set deterministic options for CUDNN backend.
-    deterministic: bool = related.BooleanField(required=False, default=False)
-    # random seed
-    seed: Optional[int] = related.IntegerField(required=False, default=None)
-    # Whether to set different seeds for different ranks
-    diff_seed: bool = related.BooleanField(required=False, default=False)
-    # number of gpus to use
-    gpus: Optional[int] = related.IntegerField(required=False, default=None)
-    # ids of gpus to use
-    gpu_ids: Optional[List[int]] = related.ChildField(
-        cls=list, required=False, default=None
-    )
-    # override some settings in the used config, the key-value pair '
-    # 'in xxx=yyy format will be merged into config file (deprecate), '
-    # 'change to --cfg-options instead.
-    options: Optional[Dict[str, Any]] = related.ChildField(
-        cls=dict, default=None, required=False
-    )
     # override some settings in the used config, the key-value pair '
     # 'in xxx=yyy format will be merged into config file. If the value to '
     # 'be overwritten is a list, it should be like key="[a,b]" or key=a,b '
     # 'It also allows nested list/tuple values, e.g. key="[(a,b),(c,d)]" '
     # 'Note that the quotation marks are necessary and that no white space '
     # 'is allowed.
     cfg_options: Optional[Dict[str, Any]] = related.ChildField(
         cls=dict, default=None, required=False
     )
     # job launcher
-    launcher: str = related.StringField(default="none")
+    launcher: str = related.StringField(default="none", required=False)
 
-    def check_values(self) -> bool:
-        if self.gpus is not None:
-            logger.warning(
-                "DEPRECATED: 'gpus' config attributes is deprecated "
-                "because mmdet only supports single GPU mode in non-distributed "
-                "training, use gpu_id instead"
-            )
+    # ======================================================================================
+    # Parameters of the mmdetection/tools/train.py that are not used in mlcvzoo-mmdetection:
+    #
+    # If specify checkpoint path, resume from it, while if not
+    # specify, try to auto resume from the latest checkpoint
+    # in the work directory:
+    # resume: str
+    #
+    # NOTE: The local_rank parameter will be set via the argparse argument
+    #       in the training scripts.
+    # When using PyTorch version >= 2.0.0, the `torch.distributed.launch`
+    # will pass the `--local-rank` parameter to `tools/train.py` instead
+    # of `--local_rank`:
+    #
+    # local_rank: int
 
+    def check_values(self) -> bool:
         return self.launcher in ["none", "pytorch", "slurm", "mpi"]
 
 
 @define
 class MMDetectionDistributedTrainConfig(BaseConfigClass):
+    """
+    Definition of attributes needed to start a distributed training on multiple GPUs.
+    It is leaned against the documentation of mmdetection:
+    https://mmdetection.readthedocs.io/en/dev-3.x/user_guides/train.html?highlight=gpu
+
+
+    TODO: Add this to the arc42 Documentation
+    Launch multiple jobs simultaneously
+    If you would like to launch multiple jobs on a single machine, e.g., 2 jobs of 4-GPU training
+    on a machine with 8 GPUs, you need to specify different ports (29500 by default) for each job
+    to avoid communication conflict.
+
+    If you use dist_train.sh to launch training jobs, you can set the port in the commands.
+
+    CUDA_VISIBLE_DEVICES=0,1,2,3 PORT=29500 ./tools/dist_train.sh ${CONFIG_FILE} 4
+    CUDA_VISIBLE_DEVICES=4,5,6,7 PORT=29501 ./tools/dist_train.sh ${CONFIG_FILE} 4
+    """
+
     __related_strict__ = True
-    # CUDA device IDs that are visible during the training.
-    # This will be used to set the os environment variable: CUDA_VISIBLE_DEVICES
-    cuda_visible_devices: str = related.StringField()
 
-    # synchronisation port for interprocess communication
-    multi_gpu_sync_port: int = related.IntegerField(default=29500)
+    # Number of nodes, or the range of nodes in form <minimum_nodes>:<maximum_nodes>
+    nnodes: str = related.StringField(default="1:1")
+
+    # Number of workers per node; supported values: [auto, cpu, gpu, int]
+    nproc_per_node = related.StringField(default="auto")
+
+    # Rank of the node for multi-node distributed training.
+    node_rank: int = related.IntegerField(default=0)
+
+    # Synchronisation port for interprocess communication
+    master_port: int = related.IntegerField(default=29500)
+
+    # Synchronisation URI for interprocess communication
+    master_address: str = related.StringField(default="localhost")
 
 
 @define
 class MMDetectionTrainConfig(BaseConfigClass):
     """
     argparse parameter from mmdetection/tools/train.py
     """
@@ -109,24 +123,25 @@
     __related_strict__ = True
 
     argparse_config: MMDetectionTrainArgparseConfig = related.ChildField(
         cls=MMDetectionTrainArgparseConfig
     )
 
     multi_gpu_config: Optional[MMDetectionDistributedTrainConfig] = related.ChildField(
-        cls=MMDetectionDistributedTrainConfig, required=False, default=None
+        cls=MMDetectionDistributedTrainConfig,
+        required=False,
     )
 
 
 @define
 class MMDetectionInferenceConfig(InferenceConfig):
     __related_strict__ = True
 
     config_path: str = related.StringField()
-    device_string: str = related.StringField(default="cuda:0")
+    device_string: Optional[str] = related.StringField(required=False, default=None)
 
     reduction_class_mapping: Optional[ReductionMappingConfig] = related.ChildField(
         cls=ReductionMappingConfig, required=False, default=None
     )
 
     def check_values(self) -> bool:
         return 0.0 <= self.score_threshold <= 1.0
```

### Comparing `mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/model.py` & `mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/model.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,48 @@
-# Copyright 2021 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Model that wraps all objection detection models of mmdetection
 """
+from __future__ import annotations
 
+import argparse
 import copy
+import inspect
 import logging
 import os
 import shlex
 import subprocess
 import sys
-import time
 from abc import ABC
-from typing import Any, Callable, Dict, Optional, Tuple, TypeVar
+from threading import Thread
+from typing import IO, Any, Callable, Dict, Optional, TypeVar
 
 import torch
 import torch.nn
-from config_builder.replacement_map import get_current_replacement_map
+import yaml
 from mlcvzoo_base.api.interfaces import NetBased, Trainable
 from mlcvzoo_base.api.model import Model
-from mlcvzoo_base.configuration.class_mapping_config import ClassMappingConfig
-from mlcvzoo_base.configuration.reduction_mapping_config import ReductionMappingConfig
-from mlcvzoo_base.data_preparation.annotation_handler import AnnotationHandler
-from mmcv import Config, runner
-from mmcv.runner import get_dist_info, init_dist, load_checkpoint, set_random_seed
-from mmcv.utils import Registry
-from mmdet.utils import replace_cfg_vals, setup_multi_processes, update_data_root
+from mmdet.apis.det_inferencer import DetInferencer
+from mmdet.registry import DATASETS
+from mmdet.utils import setup_cache_size_limit_of_dynamo
+from mmengine.config import Config
+from mmengine.runner import Runner, load_checkpoint
 from nptyping import Int, NDArray, Shape
 
 from mlcvzoo_mmdetection.configuration import (
     MMDetectionConfig,
-    MMDetectionDistributedTrainConfig,
     MMDetectionInferenceConfig,
-    MMDetectionTrainArgparseConfig,
 )
 from mlcvzoo_mmdetection.mlcvzoo_mmdet_dataset import MLCVZooMMDetDataset
-from mlcvzoo_mmdetection.third_party.mmdetection import (
-    create_meta_dict,
-    create_random_seed,
-    init_work_dir,
-    set_checkpoint_config,
-)
-from mlcvzoo_mmdetection.utils import init_mmdetection_config
+from mlcvzoo_mmdetection.utils import init_mmdetection_config, modify_config
 
 logger = logging.getLogger(__name__)
 
 ImageType = NDArray[Shape["Height, Width, Any"], Int]
 
 MMDetectionInferenceConfigType = TypeVar(
     "MMDetectionInferenceConfigType", bound=MMDetectionInferenceConfig
@@ -70,23 +64,38 @@
         from_yaml: Optional[str] = None,
         configuration: Optional[MMDetectionConfig] = None,
         string_replacement_map: Optional[Dict[str, str]] = None,
         init_for_inference: bool = False,
         is_multi_gpu_instance: bool = False,
     ) -> None:
         self.net: Optional[torch.nn.Module] = None
+        self.inferencer: Optional[DetInferencer] = None
 
         self.yaml_config_path: Optional[str] = from_yaml
         self.is_multi_gpu_instance: bool = is_multi_gpu_instance
 
         self.configuration: MMDetectionConfig = self.create_configuration(
             from_yaml=from_yaml,
             configuration=configuration,
             string_replacement_map=string_replacement_map,
         )
+        self._register_dataset()
+
+        config_path = self.configuration.train_config.argparse_config.config
+        if string_replacement_map is not None:
+            config_path = modify_config(
+                config_path=config_path, string_replacement_map=string_replacement_map
+            )
+        self.cfg = init_mmdetection_config(
+            config_path=config_path,
+            cfg_options=self.configuration.train_config.argparse_config.cfg_options,
+        )
+        self.configuration.inference_config.config_path = config_path
+        self.configuration.train_config.argparse_config.config = config_path
+        self.__init_dataloader()
         Model.__init__(
             self,
             configuration=self.configuration,
             init_for_inference=init_for_inference,
         )
         NetBased.__init__(self, net=self.net)
         Trainable.__init__(self)
@@ -94,98 +103,87 @@
     def get_checkpoint_filename_suffix(self) -> str:
         return ".pth"
 
     def get_training_output_dir(self) -> str:
         return self.configuration.train_config.argparse_config.work_dir
 
     @staticmethod
-    def _get_framework_imports() -> (
-        Tuple[  # type: ignore[type-arg]
-            Callable,
-            Callable,
-            Callable,
-            Callable,
-            Callable,
-            Callable,
-        ]
-    ):
-        from mmdet.apis import init_detector, init_random_seed, train_detector
-        from mmdet.datasets import build_dataset
-        from mmdet.models import build_detector
-        from mmdet.utils import collect_env
-
-        return (
-            init_detector,
-            init_random_seed,
-            train_detector,
-            build_dataset,
-            build_detector,
-            collect_env,
-        )
-
-    @staticmethod
     def _get_dataset_type() -> str:
         return "MLCVZooMMDetDataset"
 
-    @staticmethod
-    def _get_framework_version() -> Any:
-        from mmdet import __version__ as framework_version
-
-        return framework_version
-
-    def _build_val_dataset(self, cfg: Config) -> Any:
-        (
-            _,
-            _,
-            _,
-            build_dataset,
-            _,
-            _,
-        ) = self._get_framework_imports()
-
-        val_dataset = copy.deepcopy(cfg.data.val)
-        val_dataset.pipeline = cfg.data.train.pipeline
-        return build_dataset(val_dataset)
-
     def get_net(self) -> Optional[torch.nn.Module]:
         return self.net
 
-    def _init_inference_model(self) -> None:
-        (
-            init_detector,
-            _,
-            _,
-            _,
-            _,
-            _,
-        ) = self._get_framework_imports()
+    def __init_dataloader(self) -> None:
+        dataset_type = self._get_dataset_type()
+        # TODO: Handle ConcatDataset => More than one dataset
+        for data_loader in ["train_dataloader", "val_dataloader", "test_dataloader"]:
+            if (
+                data_loader in self.cfg
+                and self.cfg[data_loader] is not None
+                and self.cfg[data_loader].dataset.type == dataset_type
+            ):
+                if self.configuration.class_mapping is not None:
+                    self.cfg[
+                        data_loader
+                    ].dataset.class_mapping_config = (
+                        self.configuration.class_mapping.to_dict()
+                    )
 
+    def _init_inference_model(self) -> None:
         if self.net is None:
-            (
-                cfg,
-                self.configuration.inference_config.config_path,
-            ) = init_mmdetection_config(
-                config_path=self.configuration.inference_config.config_path,
-                string_replacement_map=self.configuration.string_replacement_map,
+            self.inferencer = DetInferencer(
+                self.cfg,
+                weights=None,
+                device=self.configuration.inference_config.device_string,
             )
+            self.net = self.inferencer.model
 
-            if self.configuration.train_config.argparse_config.cfg_options is not None:
-                cfg.merge_from_dict(
-                    self.configuration.train_config.argparse_config.cfg_options
+            if self.configuration.inference_config.checkpoint_path != "":
+                self.restore(
+                    checkpoint_path=self.configuration.inference_config.checkpoint_path
                 )
 
-            self.net = init_detector(
-                config=cfg,
-                checkpoint=None,
-                device=self.configuration.inference_config.device_string,
-            )
+    def _init_training_model(self) -> None:
+        # load config
+        self.cfg.launcher = self.configuration.train_config.argparse_config.launcher
+        self.cfg.experiment_name = self.unique_name
+        # We always define the work_dir in the configuration file
+        self.cfg.work_dir = self.configuration.train_config.argparse_config.work_dir
+
+        # enable automatic-mixed-precision training
+        if self.configuration.train_config.argparse_config.amp is True:
+            optim_wrapper = self.cfg.optim_wrapper.type
+            if optim_wrapper == "AmpOptimWrapper":
+                logger.warning(
+                    "AMP training is already enabled in your config.",
+                )
+            else:
+                assert optim_wrapper == "OptimWrapper", (
+                    "`--amp` is only supported when the optimizer wrapper type is "
+                    f"`OptimWrapper` but got {optim_wrapper}."
+                )
+                self.cfg.optim_wrapper.type = "AmpOptimWrapper"
+                self.cfg.optim_wrapper.loss_scale = "dynamic"
 
-            self.restore(
-                checkpoint_path=self.configuration.inference_config.checkpoint_path
-            )
+        # enable automatically scaling LR
+        if self.configuration.train_config.argparse_config.auto_scale_lr:
+            if (
+                "auto_scale_lr" in self.cfg
+                and "enable" in self.cfg.auto_scale_lr
+                and "base_batch_size" in self.cfg.auto_scale_lr
+            ):
+                self.cfg.auto_scale_lr.enable = True
+            else:
+                raise RuntimeError(
+                    'Can not find "auto_scale_lr" or '
+                    '"auto_scale_lr.enable" or '
+                    '"auto_scale_lr.base_batch_size" in your'
+                    " configuration file."
+                )
 
     def store(self, checkpoint_path: str) -> None:
         pass
 
     def restore(self, checkpoint_path: str) -> None:
         if self.net is None:
             raise ValueError(
@@ -216,262 +214,171 @@
         anymore. Therefore, it keeps the weights and meta information of the source checkpoint.
 
         Args:
             input_checkpoint_path: Path to source checkpoint file
             output_checkpoint_path: Path to where the checkpoint is saved
         """
 
-        (
-            init_detector,
-            _,
-            _,
-            _,
-            _,
-            _,
-        ) = self._get_framework_imports()
-
-        # loading config of current model
-        cfg, _ = init_mmdetection_config(
-            config_path=self.configuration.inference_config.config_path,
-            string_replacement_map=self.configuration.string_replacement_map,
-        )
-
-        # load checkpoint from source directory to a model
-        model = init_detector(
-            config=cfg,
-            checkpoint=input_checkpoint_path,
-            device=self.configuration.inference_config.device_string,
-        )
+        runner = MMDetectionModel._build_runner(cfg=self.cfg)
 
         # Load input checkpoint dict from and extract the metadata for the output checkpoint.
         # Save reduced checkpoint with metadata of full checkpoint to target directory.
-        runner.checkpoint.save_checkpoint(
-            model,
-            output_checkpoint_path,
-            meta=runner.load_checkpoint(
-                model, input_checkpoint_path, map_location="cpu"
-            )["meta"],
+        runner.save_checkpoint(
+            out_dir=os.path.dirname(output_checkpoint_path),
+            filename=os.path.basename(output_checkpoint_path),
+            save_optimizer=False,
+            save_param_scheduler=False,
+            meta=runner.load_checkpoint(filename=input_checkpoint_path)["meta"],
         )
 
         logger.info(
             "Saved checkpoint from '%s' in a reduced version to '%s'.",
             input_checkpoint_path,
             output_checkpoint_path,
         )
 
     def train(self) -> None:
-        if self.configuration.train_config.argparse_config.launcher == "none":
-            self._train(
-                argparse_config=self.configuration.train_config.argparse_config,
-                string_replacement_map=self.configuration.string_replacement_map,
-                class_mapping_config=self.configuration.class_mapping,
-                reduction_mapping_config=self.configuration.inference_config.reduction_class_mapping,
-            )
+        if (
+            self.configuration.train_config.multi_gpu_config is None
+            or "LOCAL_RANK" in os.environ
+        ):
+            # Don't start a distributed training if called without a multi GPU config,
+            # or run as a worker via torch.distributed as indicated by the presence of a local rank
+            logger.info("Training model")
+            self._train()
         else:
-            if self.configuration.train_config.multi_gpu_config is None:
-                raise ValueError(
-                    "In order to run a multi GPU training, "
-                    "the config attribute train_config.multi_gpu_config has to be provided"
-                )
-
-            self._train_multi_gpu(
-                argparse_config=self.configuration.train_config.argparse_config,
-                multi_gpu_config=self.configuration.train_config.multi_gpu_config,
-                string_replacement_map=self.configuration.string_replacement_map,
-            )
+            logger.info("Training distributed model")
+            self._train_multi_gpu()
 
     @staticmethod
     def _register_dataset() -> None:
         """
         Register the custom dataset of the MLCVZoo in the registry of mmcv
 
         Returns:
             None
         """
-        mmdet_registry = Registry("dataset")
-        mmdet_registry.register_module(MLCVZooMMDetDataset.__name__)
+        DATASETS.register_module(
+            MLCVZooMMDetDataset.__name__, module=MLCVZooMMDetDataset, force=True
+        )
 
-    @staticmethod
     def _train_multi_gpu(
-        argparse_config: MMDetectionTrainArgparseConfig,
-        multi_gpu_config: MMDetectionDistributedTrainConfig,
-        string_replacement_map: Dict[str, str],
+        self,
     ) -> None:
         """
         Run mmdet multi-gpu/distributed training.
 
         Returns:
             None
         """
+        if self.configuration.train_config.multi_gpu_config is None:
+            raise RuntimeError("No multi GPU config provided")
 
-        if argparse_config.gpu_ids is None:
-            raise ValueError("argparse_config.gpus_ids is None")
-
-        env = os.environ.copy()
-        env[
-            "PYTHONPATH"
-        ] = f"{os.environ.get('PYTHONPATH') if os.environ.get('PYTHONPATH') is not None else ''}"
-
-        env["cuda_visible_devices"] = multi_gpu_config.cuda_visible_devices
-
-        for key, value in get_current_replacement_map().items():
-            env[key] = value
+        self.cfg = init_mmdetection_config(
+            config_path=self.configuration.train_config.argparse_config.config,
+        )
 
-        _, new_config_path = init_mmdetection_config(
-            config_path=argparse_config.config,
-            string_replacement_map=string_replacement_map,
+        distributed_model_config_path = os.path.join(
+            self.get_training_output_dir(),
+            "{}-worker.yaml".format(self.configuration.unique_name),
         )
+        os.makedirs(os.path.dirname(distributed_model_config_path), exist_ok=True)
+        with open(distributed_model_config_path, "w+") as yaml_file:
+            self.configuration.to_yaml(
+                yaml_package=yaml, dumper_cls=yaml.Dumper, stream=yaml_file
+            )
 
         command = (
-            f"-m torch.distributed.run "
-            f"--nproc_per_node={len(argparse_config.gpu_ids)} "
-            f"--master_port={multi_gpu_config.multi_gpu_sync_port} "
-            f"{__file__} "
-            f"{new_config_path} "
+            f"{sys.executable} -u "
+            "-m torch.distributed.run "
+            f"--nproc_per_node={self.configuration.train_config.multi_gpu_config.nproc_per_node} "
+            f"--master_port={self.configuration.train_config.multi_gpu_config.master_port} "
+            f"--master_addr={self.configuration.train_config.multi_gpu_config.master_address} "
+            f"--nnodes={self.configuration.train_config.multi_gpu_config.nnodes} "
+            f"--node_rank={self.configuration.train_config.multi_gpu_config.node_rank} "
+            f"{inspect.getfile(self.__class__)} "
+            f"{distributed_model_config_path} "
         )
 
-        logger.debug("Run command: %s", command)
+        subproc_env = dict(os.environ.copy())
+        subproc_env["LOGLEVEL"] = "INFO"
 
-        command_split = [sys.executable]
-        command_split.extend(shlex.split(command))
-        result = subprocess.run(args=command_split, env=env, check=False)
+        logger.debug("Run command: %s", command)
+        result = subprocess.Popen(
+            shlex.split(command),
+            env=subproc_env,
+            stdout=subprocess.PIPE,
+            stderr=subprocess.STDOUT,
+            text=False,
+        )
+        Thread(
+            target=self.__pipe_to_log, args=[result.stdout, logging.INFO], daemon=True
+        ).start()
+        result.wait()
 
         if result.returncode:
             logger.error(
                 "Command '%s' returned with exit code %i", command, result.returncode
             )
             raise RuntimeError(
                 f"Distributed training exited with exitcode != 0, "
                 f"exitcode: {result.returncode}"
             )
 
-    def _train_pre_init(self, cfg: Config) -> Config:
-        # replace the ${key} with the value of cfg.key
-        cfg = replace_cfg_vals(cfg)
-        # update data root according to MMDET_DATASETS
-        update_data_root(cfg)
+    @staticmethod
+    def __pipe_to_log(pipe: IO[bytes], level: int) -> None:
+        with pipe:
+            for line in iter(pipe.readline, b""):  # b'\n'-separated lines
+                logger.log(level, "Subprocess: %r", line.decode("utf-8").strip())
+
+    @staticmethod
+    def _build_runner(cfg: Config) -> Runner:
+        from mmengine.registry import RUNNERS
+
+        # build the runner from config
+        if "runner_type" not in cfg:
+            # build the default runner
+            runner = Runner.from_cfg(cfg)
+        else:
+            # build customized runner from the registry
+            # if 'runner_type' is set in the cfg
+            runner = RUNNERS.build(cfg)
 
-        return cfg
+        return runner
 
     def _train(
         self,
-        argparse_config: MMDetectionTrainArgparseConfig,
-        string_replacement_map: Dict[str, str],
-        class_mapping_config: Optional[ClassMappingConfig] = None,
-        reduction_mapping_config: Optional[ReductionMappingConfig] = None,
     ) -> None:
-        (
-            _,
-            init_random_seed,
-            train_detector,
-            build_dataset,
-            build_detector,
-            collect_env,
-        ) = self._get_framework_imports()
-
-        self._register_dataset()
-
-        _, new_config_path = init_mmdetection_config(
-            config_path=argparse_config.config,
-            string_replacement_map=string_replacement_map,
-        )
+        # Reduce the number of repeated compilations and improve
+        # training speed.
+        setup_cache_size_limit_of_dynamo()
 
-        cfg = Config.fromfile(new_config_path)
+        runner = MMDetectionModel._build_runner(cfg=self.cfg)
 
-        cfg = self._train_pre_init(cfg=cfg)
+        # start training
+        runner.train()
 
-        cfg.merge_from_dict(argparse_config.cfg_options)
-        # set multi-process settings
-        setup_multi_processes(cfg)
-
-        cfg.work_dir = argparse_config.work_dir
-        if argparse_config.resume_from:
-            cfg.resume_from = argparse_config.resume_from
-        cfg.auto_resume = argparse_config.auto_resume
-
-        # set cudnn_benchmark
-        if cfg.get("cudnn_benchmark", False):
-            torch.backends.cudnn.benchmark = True
-
-        cfg.gpu_ids = argparse_config.gpu_ids
-        distributed = False
-        if not cfg.gpu_ids:
-            # TODO: cpu use-case currently broken => fix in mmdet
-            cfg.device = "cpu"
-        # init distributed env first, since logger depends on the dist info.
-        elif argparse_config.launcher == "none":
-            cfg.device = "cuda"
-            cfg.gpu_ids = [cfg.gpu_ids[0]]
-        else:
-            cfg.device = "mlu"
-            distributed = True
-            init_dist(
-                argparse_config.launcher,
-                **cfg.dist_params,
-            )
-            # re-set gpu_ids with distributed training mode
-            _, world_size = get_dist_info()
-
-        init_work_dir(cfg=cfg, config_path=new_config_path)
-
-        cfg = create_random_seed(
-            argparse_config=argparse_config,
-            cfg=cfg,
-            init_random_seed=init_random_seed,
-            set_random_seed=set_random_seed,
-        )
-
-        logger.debug(f"Config:\n{cfg.pretty_text}")
+    @staticmethod
+    def run(model_class: Callable) -> None:  # type: ignore[type-arg]
+        """
+        Run training with given model subclass, reading a config from file.
+        This function is intended to be called during torch.distributed.run via subclass main
+        functions. It expects a single command line parameter called "yaml_config_path" pointing
+        to a valid YAML configuration file for the given model subclass.
 
-        model = build_detector(
-            cfg.model, train_cfg=cfg.get("train_cfg"), test_cfg=cfg.get("test_cfg")
+        Args:
+            model_class: the subclass of model.MMDetectionModel to train
+        """
+        parser: argparse.ArgumentParser = argparse.ArgumentParser()
+        parser.add_argument(
+            "yaml_config_path",
+            help="Load all parameters from the given yaml configuration file",
+            type=str,
         )
-        model.init_weights()
-
-        dataset_type = self._get_dataset_type()
-        for data_type in ["train", "test", "val"]:
-            if cfg.data[data_type].type == dataset_type:
-                annotation_handler_config = AnnotationHandler.create_configuration(
-                    from_yaml=cfg.data[data_type].annotation_handler_config_path,
-                    string_replacement_map=string_replacement_map,
-                )
-
-                if class_mapping_config is None:
-                    raise ValueError(
-                        "In order to use MLCVZooMMDetDataset as valid "
-                        "class_mapping_config has to be provided, "
-                        "class_mapping_config=None"
-                    )
 
-                annotation_handler_config.class_mapping = class_mapping_config
-                annotation_handler_config.reduction_class_mapping = (
-                    reduction_mapping_config
-                )
+        args = parser.parse_args()
 
-                cfg.data[
-                    data_type
-                ].annotation_handler_config_dict = annotation_handler_config.to_dict()
-
-        datasets = [build_dataset(cfg.data.train)]
-
-        if len(cfg.workflow) == 2:
-            datasets.append(self._build_val_dataset(cfg=cfg))
-
-        cfg = set_checkpoint_config(
-            cfg=cfg,
-            framework_version=self._get_framework_version(),
-            classes=datasets[0].CLASSES,
-            model=model,
-        )
-
-        timestamp = time.strftime("%Y%m%d_%H%M%S", time.localtime())
-        train_detector(
-            model,
-            datasets,
-            cfg,
-            distributed=distributed,
-            validate=(not argparse_config.no_validate),
-            timestamp=timestamp,
-            meta=create_meta_dict(
-                cfg=cfg, collect_env=collect_env, exp_name=self.unique_name
-            ),
+        mmdet_model = model_class(
+            from_yaml=args.yaml_config_path,
+            init_for_inference=False,
         )
+        mmdet_model.train()
```

### Comparing `mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/object_detection_model.py` & `mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/object_detection_model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-# Copyright 2022 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Model that wraps all objection detection models of mmdetection
 """
-
 import logging
 import typing
 from typing import Dict, List, Optional, Tuple, Union
 
 import numpy as np
 import torch.nn
 from mlcvzoo_base.api.data.annotation_class_mapper import AnnotationClassMapper
@@ -18,28 +18,28 @@
 from mlcvzoo_base.api.data.class_identifier import ClassIdentifier
 from mlcvzoo_base.api.interfaces import NetBased, Trainable
 from mlcvzoo_base.api.model import ObjectDetectionModel
 from mlcvzoo_base.configuration.structs import ObjectDetectionBBoxFormats
 from mlcvzoo_base.configuration.utils import (
     create_configuration as create_basis_configuration,
 )
-from mmdet.apis import inference_detector
+from mmdet.structures.det_data_sample import DetDataSample
 
 from mlcvzoo_mmdetection.configuration import (
     MMDetectionConfig,
     MMDetectionInferenceConfig,
 )
-from mlcvzoo_mmdetection.model import MMDetectionModel
+from mlcvzoo_mmdetection.model import ImageType, MMDetectionModel
 
 logger = logging.getLogger(__name__)
 
 
 class MMObjectDetectionModel(
     MMDetectionModel[MMDetectionInferenceConfig],
-    ObjectDetectionModel[MMDetectionConfig, Union[str, np.ndarray]],  # type: ignore[type-arg]
+    ObjectDetectionModel[MMDetectionConfig, Union[str, ImageType]],
     NetBased[torch.nn.Module, MMDetectionInferenceConfig],
     Trainable,
 ):
     """
     Class for wrapping mmdetection models
     """
 
@@ -49,16 +49,17 @@
         configuration: Optional[MMDetectionConfig] = None,
         string_replacement_map: Optional[Dict[str, str]] = None,
         init_for_inference: bool = False,
         is_multi_gpu_instance: bool = False,
     ) -> None:
         MMDetectionModel.__init__(
             self,
-            from_yaml=from_yaml,
-            configuration=configuration,
+            configuration=self.create_configuration(
+                from_yaml, configuration, string_replacement_map
+            ),
             string_replacement_map=string_replacement_map,
             init_for_inference=init_for_inference,
             is_multi_gpu_instance=is_multi_gpu_instance,
         )
         ObjectDetectionModel.__init__(
             self,
             configuration=self.configuration,
@@ -90,103 +91,116 @@
     @property
     def num_classes(self) -> int:
         return self.mapper.num_classes
 
     def get_classes_id_dict(self) -> Dict[int, str]:
         return self.mapper.annotation_class_id_to_model_class_name_map
 
-    def __decode_mmdet_result(
-        self, model_result: List[np.ndarray]  # type: ignore[type-arg]
-    ) -> List[BoundingBox]:
+    def __decode_mmdet_result(self, prediction: DetDataSample) -> List[BoundingBox]:
         """
         Decode output of an object detection model from mmdetection
 
         Args:
-            model_result: The result that the model has predicted
+            prediction: The result that the model has predicted
 
         Returns:
-            The model_result as list of bounding boxes in MLCVZoo format
+            The decoded prediction as list of bounding boxes in MLCVZoo format
         """
 
         bounding_boxes: List[BoundingBox] = list()
-
-        np_bounding_boxes = np.vstack(model_result)
-        assert np_bounding_boxes.shape[1] == 5
-
-        # Create numpy array containing all class ids
-        class_id_list = []
-        for index, box in enumerate(model_result):
-            class_id_list.append(np.full(box.shape[0], index, dtype=np.int32))
-        np_class_id_array = np.concatenate(class_id_list)
-
-        # Get relevant indices that do match a given threshold
-        np_scores = np_bounding_boxes[:, -1]
-        valid_indices = np_scores > self.configuration.inference_config.score_threshold
+        valid_indices = (
+            prediction.pred_instances.scores
+            > self.configuration.inference_config.score_threshold
+        )
 
         # Filter results according to the determined valid indices
-        np_bounding_boxes = np_bounding_boxes[valid_indices, :]
-        np_class_id_array = np_class_id_array[valid_indices]
-        np_scores = np_scores[valid_indices]
+        valid_bounding_boxes = prediction.pred_instances.bboxes[valid_indices]
+        valid_class_ids = prediction.pred_instances.labels[valid_indices]
+        valid_scores = prediction.pred_instances.scores[valid_indices]
 
         for bbox, class_id, score in zip(
-            np_bounding_boxes, np_class_id_array, np_scores
+            valid_bounding_boxes, valid_class_ids, valid_scores
         ):
-            bbox_int = bbox.astype(np.int32)
+            bbox_int = bbox.cpu().numpy().astype(np.int32)
+            class_id_int = int(class_id.cpu())
 
             bounding_boxes.extend(
                 self.build_bounding_boxes(
                     box_format=ObjectDetectionBBoxFormats.XYXY,
                     box_list=(bbox_int[0:4]),
                     class_identifiers=self.mapper.map_model_class_id_to_output_class_identifier(
-                        class_id=class_id
+                        class_id=class_id_int
                     ),
                     model_class_identifier=ClassIdentifier(
-                        class_id=class_id,
+                        class_id=class_id_int,
                         class_name=self.mapper.map_annotation_class_id_to_model_class_name(
-                            class_id=class_id
+                            class_id=class_id_int
                         ),
                     ),
-                    score=float(score),
+                    score=float(score.cpu()),
                     difficult=False,
                     occluded=False,
                     content="",
                 )
             )
 
         return bounding_boxes
 
     def predict(
-        self, data_item: Union[str, np.ndarray]  # type: ignore[type-arg]
-    ) -> Tuple[Union[str, np.ndarray], List[BoundingBox]]:  # type: ignore[type-arg]
-        """
-        Predicts objects for given data_item
-
-        Args:
-            data_item: Object on which a prediction is to be executed
+        self, data_item: Union[str, ImageType]
+    ) -> Tuple[Union[str, ImageType], List[BoundingBox]]:
+        if self.net is None:
+            raise ValueError(
+                "The 'net' attribute is not initialized, "
+                "make sure to instantiate with init_for_inference=True"
+            )
+        if self.inferencer is None:
+            raise ValueError(
+                "The 'inferencer' attribute is not initialized, "
+                "make sure to instantiate with init_for_inference=True"
+            )
 
-        Returns:
-            Data_item which served as input
-            List of BoundingBox objects containing bounding box information for every prediction
-            made by the model. Only contains bounding boxes which are above the score threshold
-            specified in configuration file.
-        """
+        # For a single data_item we only have one prediction
+        return data_item, self.__decode_mmdet_result(
+            prediction=self.inferencer(
+                inputs=data_item, return_datasample=True, batch_size=1
+            )["predictions"][0]
+        )
 
+    def predict_many(
+        self, data_items: List[Union[str, ImageType]]
+    ) -> List[Tuple[Union[str, ImageType], List[BoundingBox]]]:
         if self.net is None:
             raise ValueError(
-                "MMDetectionModel is not initialized for inference! "
-                "Please set the parameter 'init_for_inference=True'"
+                "The 'net' attribute is not initialized, "
+                "make sure to instantiate with init_for_inference=True"
+            )
+        if self.inferencer is None:
+            raise ValueError(
+                "The 'inferencer' attribute is not initialized, "
+                "make sure to instantiate with init_for_inference=True"
             )
 
-        result = inference_detector(model=self.net, imgs=data_item)
+        prediction_list: List[Tuple[Union[str, ImageType], List[BoundingBox]]] = []
 
-        # Check if model output is only bbox head, or if the model has other heads:
-        # tuple => bbox-head + mask-head
-        if isinstance(result, tuple):
-            model_result = result[0]
+        # TODO: add batch-size as parameter
+        predictions: List[DetDataSample] = self.inferencer(
+            inputs=data_items,
+            return_datasample=True,
+            batch_size=len(data_items),
+        )["predictions"]
+
+        for data_item, prediction in zip(data_items, predictions):
+            segmentations = self.__decode_mmdet_result(prediction=prediction)
+
+            prediction_list.append(
+                (
+                    data_item,
+                    segmentations,
+                )
+            )
 
-        # type is list => bbox-head only
-        else:
-            model_result = result
+        return prediction_list
 
-        bounding_boxes = self.__decode_mmdet_result(model_result=model_result)
 
-        return data_item, bounding_boxes
+if __name__ == "__main__":
+    MMDetectionModel.run(MMObjectDetectionModel)
```

### Comparing `mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/segmentation_model.py` & `mlcvzoo_mmdetection-6.0.0/mlcvzoo_mmdetection/segmentation_model.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,35 +1,34 @@
-# Copyright 2023 Open Logistics Foundation
+# Copyright Open Logistics Foundation
 #
-# Licensed under the Open Logistics License 1.0.
+# Licensed under the Open Logistics Foundation License 1.3.
 # For details on the licensing terms, see the LICENSE file.
+# SPDX-License-Identifier: OLFL-1.3
 
 """
 Model that wraps all segmentation models of mmdetection
 """
-
 import logging
 from typing import Any, Dict, List, Optional, Tuple, Union, cast
 
-import mmcv
 import numpy as np
 import torch.nn
 from mlcvzoo_base.api.data.annotation_class_mapper import AnnotationClassMapper
 from mlcvzoo_base.api.data.box import Box
 from mlcvzoo_base.api.data.class_identifier import ClassIdentifier
 from mlcvzoo_base.api.data.segmentation import PolygonType, Segmentation
 from mlcvzoo_base.api.interfaces import NetBased, Trainable
 from mlcvzoo_base.api.model import SegmentationModel
 from mlcvzoo_base.configuration.structs import ObjectDetectionBBoxFormats
 from mlcvzoo_base.configuration.utils import (
     create_configuration as create_basis_configuration,
 )
-from mmdet.apis import inference_detector
-from mmdet.core import INSTANCE_OFFSET
-from mmdet.core.mask.structures import bitmap_to_polygon
+from mmdet.evaluation import INSTANCE_OFFSET
+from mmdet.structures.det_data_sample import DetDataSample
+from mmdet.structures.mask.structures import bitmap_to_polygon
 from nptyping import Int, NDArray, Shape
 
 from mlcvzoo_mmdetection.configuration import (
     MMDetectionConfig,
     MMDetectionInferenceConfig,
 )
 from mlcvzoo_mmdetection.model import MMDetectionModel
@@ -55,16 +54,17 @@
         configuration: Optional[MMDetectionConfig] = None,
         string_replacement_map: Optional[Dict[str, str]] = None,
         init_for_inference: bool = False,
         is_multi_gpu_instance: bool = False,
     ) -> None:
         MMDetectionModel.__init__(
             self,
-            from_yaml=from_yaml,
-            configuration=configuration,
+            configuration=self.create_configuration(
+                from_yaml, configuration, string_replacement_map
+            ),
             string_replacement_map=string_replacement_map,
             init_for_inference=init_for_inference,
             is_multi_gpu_instance=is_multi_gpu_instance,
         )
         SegmentationModel.__init__(
             self,
             configuration=self.configuration,
@@ -96,31 +96,31 @@
     @property
     def num_classes(self) -> int:
         return self.mapper.num_classes
 
     def get_classes_id_dict(self) -> Dict[int, str]:
         return self.mapper.annotation_class_id_to_model_class_name_map
 
-    def __decode_mmdet_result(self, model_result: Any) -> List[Segmentation]:
+    def __decode_mmdet_result(self, prediction: Any) -> List[Segmentation]:
         """
         Decode output of an object detection model from mmdetection
 
         Args:
-            model_result: The result that the model has predicted
+            prediction: The result that the model has predicted
 
         Returns:
-            The model_result as list of bounding boxes in MLCVZoo format
+            The prediction as list of bounding boxes in MLCVZoo format
         """
 
         segmentations: List[Segmentation] = []
 
-        if isinstance(model_result, dict):
+        if hasattr(prediction, "pred_panoptic_seg"):
             # Have a shape of (IMAGE_HEIGHT, IMAGE_WIDTH) with each pixel
             # stating the class of the segmentation
-            pan_results = model_result["pan_results"]
+            pan_results = prediction.pred_panoptic_seg.sem_seg.cpu().numpy()[0]
             # Get the classes that are contained in this panoptic segmentation
             valid_indices = np.unique(pan_results)[::-1]
             # Since the panoptic result has an INSTANCE_OFFSET, we need to make
             # sure not to get the class-id which is equal to the number of classes
             legal_indices = valid_indices != self.num_classes
             valid_indices = valid_indices[legal_indices]
             pan_class_ids = np.array(
@@ -156,99 +156,121 @@
                         difficult=False,
                         occluded=False,
                         content="",
                         box=None,
                     )
                 )
         else:
-            bbox_result, segm_result = model_result
-            if isinstance(segm_result, tuple):
-                segm_result = segm_result[0]
-
-            np_bounding_boxes = np.vstack(bbox_result)
-
-            # Create numpy array containing all class ids
-            class_id_list = []
-            for index, box in enumerate(bbox_result):
-                class_id_list.append(np.full(box.shape[0], index, dtype=np.int32))
-            np_class_id_array = np.concatenate(class_id_list)
-
-            # Get relevant indices that do match a given threshold
-            np_scores = np_bounding_boxes[:, -1]
             valid_indices = (
-                np_scores > self.configuration.inference_config.score_threshold
+                prediction.pred_instances.scores
+                > self.configuration.inference_config.score_threshold
             )
 
             # Filter results according to the determined valid indices
-            np_bounding_boxes = np_bounding_boxes[valid_indices, :]
-            np_class_id_array = np_class_id_array[valid_indices]
-            np_scores = np_scores[valid_indices]
-
-            mmdet_segmentations = mmcv.concat_list(segm_result)
-            if isinstance(mmdet_segmentations[0], torch.Tensor):
-                mmdet_segmentations = (
-                    torch.stack(mmdet_segmentations, dim=0).detach().cpu().numpy()
-                )
-            else:
-                mmdet_segmentations = np.stack(mmdet_segmentations, axis=0)
+            valid_masks = prediction.pred_instances.masks[valid_indices]
+            valid_bounding_boxes = prediction.pred_instances.bboxes[valid_indices]
+            valid_class_ids = prediction.pred_instances.labels[valid_indices]
+            valid_scores = prediction.pred_instances.scores[valid_indices]
+
+            for i, (bbox, mask, class_id, score) in enumerate(
+                zip(valid_bounding_boxes, valid_masks, valid_class_ids, valid_scores)
+            ):
+                np_mask = np.stack(mask.detach().cpu().numpy(), axis=0)
+                contours, with_hole = bitmap_to_polygon(np_mask)
 
-            mmdet_segmentations = mmdet_segmentations[valid_indices, ...]
+                np_bbox = bbox.cpu().numpy().astype(np.int32)
+                class_id_int = int(class_id.cpu())
 
-            for i, (bbox, mmdet_segmentation, class_id, score) in enumerate(
-                zip(
-                    np_bounding_boxes, mmdet_segmentations, np_class_id_array, np_scores
+                # TODO: Add the 'box' parameter to build_segmentations to simplify the
+                #       instantiation of the segmentations per class_identifier
+                class_identifiers = (
+                    self.mapper.map_model_class_id_to_output_class_identifier(
+                        class_id=class_id_int
+                    )
                 )
-            ):
-                contours, with_hole = bitmap_to_polygon(mmdet_segmentation)
 
-                bbox_int = bbox.astype(np.int32)
-                # TODO: Multiple class-identifiers
-                segmentations.append(
-                    Segmentation(
-                        class_identifier=ClassIdentifier(
-                            class_id=class_id,
-                            class_name=self.mapper.map_annotation_class_id_to_model_class_name(
-                                class_id=class_id
+                model_class_identifier = ClassIdentifier(
+                    class_id=class_id_int,
+                    class_name=self.mapper.map_annotation_class_id_to_model_class_name(
+                        class_id=class_id_int
+                    ),
+                )
+
+                for class_identifier in class_identifiers:
+                    segmentations.append(
+                        Segmentation(
+                            class_identifier=class_identifier,
+                            model_class_identifier=model_class_identifier,
+                            score=float(score),
+                            # For now, we only take the first contour and don't expect
+                            # segmentations to be split into multiple parts
+                            polygon=cast(PolygonType, contours[0]),
+                            difficult=False,
+                            occluded=False,
+                            content="",
+                            box=Box.init_format_based(
+                                box_format=ObjectDetectionBBoxFormats.XYXY,
+                                box_list=(np_bbox[0:4]),
                             ),
-                        ),
-                        score=score,
-                        # For now, we only take the first contour and don't expect
-                        # segmentations to be split into multiple parts
-                        polygon=cast(PolygonType, contours[0]),
-                        difficult=False,
-                        occluded=False,
-                        content="",
-                        box=Box.init_format_based(
-                            box_format=ObjectDetectionBBoxFormats.XYXY,
-                            box_list=(bbox_int[0:4]),
-                        ),
+                        )
                     )
-                )
 
         return segmentations
 
     def predict(
         self, data_item: Union[str, ImageType]
     ) -> Tuple[Union[str, ImageType], List[Segmentation]]:
-        """
-        Predicts objects for given data_item
-
-        Args:
-            data_item: Object on which a prediction is to be executed
+        if self.net is None:
+            raise ValueError(
+                "The 'net' attribute is not initialized, "
+                "make sure to instantiate with init_for_inference=True"
+            )
+        if self.inferencer is None:
+            raise ValueError(
+                "The 'inferencer' attribute is not initialized, "
+                "make sure to instantiate with init_for_inference=True"
+            )
 
-        Returns:
-            TODO
-        """
+        return data_item, self.__decode_mmdet_result(
+            prediction=self.inferencer(
+                inputs=data_item, return_datasample=True, batch_size=1
+            )["predictions"][0]
+        )
 
+    def predict_many(
+        self, data_items: List[Union[str, ImageType]]
+    ) -> List[Tuple[Union[str, ImageType], List[Segmentation]]]:
         if self.net is None:
             raise ValueError(
-                "MMDetectionModel is not initialized for inference! "
-                "Please set the parameter 'init_for_inference=True'"
+                "The 'net' attribute is not initialized, "
+                "make sure to instantiate with init_for_inference=True"
+            )
+        if self.inferencer is None:
+            raise ValueError(
+                "The 'inferencer' attribute is not initialized, "
+                "make sure to instantiate with init_for_inference=True"
             )
 
-        result = inference_detector(model=self.net, imgs=data_item)
+        prediction_list: List[Tuple[Union[str, ImageType], List[Segmentation]]] = []
+
+        # TODO: add batch-size as parameter
+        predictions: List[DetDataSample] = self.inferencer(
+            inputs=data_items,
+            return_datasample=True,
+            batch_size=len(data_items),
+        )["predictions"]
+
+        for data_item, prediction in zip(data_items, predictions):
+            segmentations = self.__decode_mmdet_result(prediction=prediction)
+
+            prediction_list.append(
+                (
+                    data_item,
+                    segmentations,
+                )
+            )
+
+        return prediction_list
 
-        segmentations: List[Segmentation] = self.__decode_mmdet_result(
-            model_result=result
-        )
 
-        return data_item, segmentations
+if __name__ == "__main__":
+    MMDetectionModel.run(MMSegmentationModel)
```

### Comparing `mlcvzoo_mmdetection-5.1.1/mlcvzoo_mmdetection/third_party/LICENSE` & `mlcvzoo_mmdetection-6.0.0/LICENSE`

 * *Files 22% similar despite different names*

```diff
@@ -1,203 +1,220 @@
-Copyright 2018-2023 OpenMMLab. All rights reserved.
+Open Logistics Foundation License
+Version 1.3, January 2023
+https://www.openlogisticsfoundation.org/licenses/
+
+TERMS AND CONDITIONS FOR USE, REPRODUCTION AND DISTRIBUTION
+
+§1 Definitions
+
+(1) "Subject Matter of the License" shall mean the works of software components
+in Source or Object form as well as any other components protected under
+copyright, design and/or patent law which are made available under this License.
+
+(2) "License" shall mean the terms and conditions for the use, reproduction and
+distribution of the Subject Matter of the License in accordance with the
+provisions of this document.
+
+(3) "Licensor(s)" shall mean the copyright holder(s) or the entity authorized by
+law or contract by the copyright holder(s) to grant the License.
+
+(4) "You" (or "Your") shall mean a natural or legal person exercising the
+permissions granted by this License.
+
+(5) "Source" form shall mean the preferred form for making modifications,
+including but not limited to software source code, documentation source, and
+configuration files.
+
+(6) "Object" form shall mean any form resulting from mechanical transformation
+or translation of a Source form, including but not limited to compiled object
+code, generated documentation, and conversions to other media types.
+
+(7) "Derivative Works" shall mean any work, whether in Source or Object form or
+any other form, that is based on (or derived from) the Subject Matter of the
+License and for which the editorial revisions, annotations, elaborations, or
+other modifications represent, as a whole, an original work of authorship. For
+the purposes of this License, Derivative Works shall not include works that
+remain separable from, or merely link (or bind by name) to the interfaces of,
+the Subject Matter of the License and Derivative Works thereof.
+
+(8) "Contribution" shall mean any proprietary work, including the original
+version of the Subject Matter of the License and any changes or additions to
+such work, or Derivative Works of such work, that the rights holder, or a
+natural or legal person authorized to make submissions, intentionally submits to
+a Licensor to be incorporated into the Subject Matter of the License. For the
+purposes of this definition, "submit" shall mean any form of electronic or
+written communication which is sent to a Licensor or its representatives for the
+purpose of discussing or improving the Subject Matter of the License, including
+but not limited to communications sent via electronic mailing lists, source code
+control systems and issue tracking systems; however, communications that are
+clearly marked by the copyright holder as "not a contribution" or otherwise
+identified as such in writing are excluded.
+
+(9) "Contributor" shall mean the Licensor(s) and/or any natural or legal person
+on whose behalf the Licensor(s) receive(s) any Contribution subsequently
+incorporated into the Subject Matter of the License.
+
+§2 Grant of usage rights
+
+Subject to the terms and conditions of this License and compliance with the
+provisions of this License, You are hereby granted by each Contributor, insofar
+as applicable to the respective Subject Matter of the License the
+
+- royalty-free and non-exclusive,
+- sub-licensable for commercial and non-commercial purposes,
+- worldwide and perpetual,
+- irrevocable and non-terminable
+
+right to reproduce, prepare Derivative Works of, publicly display, publicly
+perform, and distribute the Subject Matter of the License and such Derivative
+Works in any form. This right of use includes but is not limited to the right
+
+- to use the Subject Matter of the License in any hardware and software
+  environment (with regard to the software and data components), in particular
+  to store or load it permanently or temporarily, to display it and run it,
+  including to the extent reproductions are necessary to that end,
+- to otherwise modify, interpret, edit or redesign it,
+- to store, reproduce, exhibit, publish, distribute it in tangible or intangible
+  form, on any medium or in any other way, for commercial and non-commercial
+  purposes, in particular to communicate it privately or publicly, including via
+  image, audio and other information carriers, irrespective of whether by wire
+  or wireless means,
+- to use it in databases, data networks and online services, including the right
+  to make the software and data components of the Subject Matter of the License
+  available in Source or Object form to users of the aforementioned databases,
+  networks and online services for research and retrieval purposes,
+- to allow third parties to use or operate it,
+- to use it for own purposes but also to provide services to third parties,
+- to distribute it
+
+in its original or modified, interpreted, edited or redesigned form.
+
+The foregoing right of use relates to the Subject Matter of the License, in
+particular to its Source and Object form of software components (including
+design rights, where applicable).
+
+§3 Grant of patent license
+
+Subject to the terms and conditions of this License and compliance with the
+provisions of this License, You are hereby granted by each Contributor a
+- royalty-free and non-exclusive,
+- worldwide and perpetual,
+- irrevocable (with the exception of the restrictions set out in this Section 3)
+
+patent license in all rights deriving from the patents, owned and licensable by
+the Contributor at the time of the submission of the Contribution, to
+
+- produce,
+- have produced,
+- use,
+- offer for sale,
+- sell,
+- import and otherwise transfer
+
+the Subject Matter of the License.
+
+However, said patent license shall cover only those rights deriving from the
+patents of the respective Contributors which are indispensable in order not to
+infringe that patent and only to the extent that the use of the Contributor’s
+respective Contributions, whether alone or in combination with other
+Contributions of the Contributors or any third parties together with the Subject
+Matter of the License for which these Contributions were submitted, would
+otherwise infringe that patent. The grant of license shall not include rights
+deriving from the patents which may in future become necessary for their lawful
+use due to subsequent modifications to the Subject Matter or Contributions made
+by third parties after the original submission.
+
+In the event that You institute patent litigation against any entity or person
+(including a counterclaim or countersuit in a legal action), alleging that the
+Subject Matter of the License or a Contribution incorporated or contained
+therein constitutes patent infringement or indirect infringement, all patent
+licenses which have been granted to You under this License for the Subject
+Matter of the License as well as this License itself shall be deemed terminated
+as of the date on which the action is filed.
+
+§4 Distribution
+
+You may reproduce and distribute copies of the Subject Matter of the License or
+Derivative Works on any medium, with or without modifications (with regard to
+software components in Source or Object form), provided that You comply with
+the following rules:
+
+- You must provide all other recipients of the Subject Matter of the License or
+  of Derivative Works with a copy of this License and inform them that the
+  Subject Matter of the License was originally licensed under this License.
+- You must ensure that modified files contain prominent notices indicating that
+  You have modified the files.
+- You must retain all copyright, patent, trademark and attribution notices in
+  the Subject Matter of the License in the Source form of any Derivative Works
+  You distribute, with the exception of those notices that do not pertain to any
+  part of the Derivative Works.
+
+You may add Your own copyright notices to Your modifications and state any
+additional or different license conditions and conditions for the use,
+reproduction or distribution of Your modifications or for those Derivative Works
+as a whole, provided that Your use, reproduction and distribution of the work
+complies with the terms and conditions set out in this License in all other
+respects.
+
+§5 Submission of Contributions
+
+Unless expressly stated otherwise, every Contribution that You have
+intentionally submitted for inclusion in the Subject Matter of the License is
+subject to this License without any additional terms or conditions applying.
+Irrespective of the above, none of the terms or conditions contained herein may
+be interpreted to supersede or modify the terms or conditions of any separate
+licensing agreement that You may have concluded with a Licensor for such
+Contributions, such as a so-called "Contributor License Agreement" (CLA).
+
+§6 Trademarks
+
+This License does not grant permission to use the trade names, trademarks,
+service marks or product names of the Licensor(s) or of a Contributor.
+
+§7 Limited warranty
+
+This License is granted free of charge and thus constitutes a gift. Accordingly,
+any warranty is excluded. The Subject Matter of the License is a work in
+progress; it is constantly being improved by countless Contributors. The Subject
+Matter of the License is not complete and may therefore contain errors ("bugs")
+or additional patents of Contributors or third parties, as is inherent in this
+type of development.
+
+§8 Limitation of liability
+
+Except in cases of intentional and grossly negligent conduct, the Contributors,
+their legal representatives, trustees, officers and employees shall not be
+liable for direct or indirect, material or immaterial loss or damage of any kind
+arising from the License or the use of the Subject Matter of the License; this
+applies, among other things, but not exclusively, to loss of goodwill, loss of
+production, computer failures or errors, loss of data or economic loss or
+damage, even if the Contributor has been notified of the possibility of such
+loss or damage. Irrespective of the above, the Licensor shall only be liable
+within the scope of statutory product liability to the extent that the
+respective provisions are applicable to the Subject Matter of the License or the
+Contribution.
+
+Except in cases of intentional conduct, the Contributors, their legal
+representatives, trustees, officers and employees shall not be liable for any
+infringement of third-party patent or intellectual property rights arising from
+the Contributions nor do they warrant that the Contributions are accurate,
+devoid of mistakes, complete and/or fit for any particular purpose.
+
+§9 Provision of warranties or assumption of additional liability in the event of
+distribution of the Subject Matter of the License
+
+In the event of distribution of the Subject Matter of the License or Derivative
+Works, You are free to accept support, warranty, indemnity or other liability
+obligations and/or rights consistent with this License and to charge a fee in
+return. However, in accepting such obligations, You may act only on Your own
+behalf and on Your sole responsibility, not on behalf of any other Contributor,
+and You hereby agree to indemnify, defend, and hold each Contributor harmless
+for any liability incurred by, or claims asserted against, such Contributor by
+reason of Your accepting any such warranty or additional liability.
+
+§10 Applicable law
+
+This License is governed by German law, excluding its conflict of laws
+provisions and the provisions of the UN Convention on Contracts for the
+International Sale of Goods (CISG).
 
-                                 Apache License
-                           Version 2.0, January 2004
-                        http://www.apache.org/licenses/
-
-   TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
-
-   1. Definitions.
-
-      "License" shall mean the terms and conditions for use, reproduction,
-      and distribution as defined by Sections 1 through 9 of this document.
-
-      "Licensor" shall mean the copyright owner or entity authorized by
-      the copyright owner that is granting the License.
-
-      "Legal Entity" shall mean the union of the acting entity and all
-      other entities that control, are controlled by, or are under common
-      control with that entity. For the purposes of this definition,
-      "control" means (i) the power, direct or indirect, to cause the
-      direction or management of such entity, whether by contract or
-      otherwise, or (ii) ownership of fifty percent (50%) or more of the
-      outstanding shares, or (iii) beneficial ownership of such entity.
-
-      "You" (or "Your") shall mean an individual or Legal Entity
-      exercising permissions granted by this License.
-
-      "Source" form shall mean the preferred form for making modifications,
-      including but not limited to software source code, documentation
-      source, and configuration files.
-
-      "Object" form shall mean any form resulting from mechanical
-      transformation or translation of a Source form, including but
-      not limited to compiled object code, generated documentation,
-      and conversions to other media types.
-
-      "Work" shall mean the work of authorship, whether in Source or
-      Object form, made available under the License, as indicated by a
-      copyright notice that is included in or attached to the work
-      (an example is provided in the Appendix below).
-
-      "Derivative Works" shall mean any work, whether in Source or Object
-      form, that is based on (or derived from) the Work and for which the
-      editorial revisions, annotations, elaborations, or other modifications
-      represent, as a whole, an original work of authorship. For the purposes
-      of this License, Derivative Works shall not include works that remain
-      separable from, or merely link (or bind by name) to the interfaces of,
-      the Work and Derivative Works thereof.
-
-      "Contribution" shall mean any work of authorship, including
-      the original version of the Work and any modifications or additions
-      to that Work or Derivative Works thereof, that is intentionally
-      submitted to Licensor for inclusion in the Work by the copyright owner
-      or by an individual or Legal Entity authorized to submit on behalf of
-      the copyright owner. For the purposes of this definition, "submitted"
-      means any form of electronic, verbal, or written communication sent
-      to the Licensor or its representatives, including but not limited to
-      communication on electronic mailing lists, source code control systems,
-      and issue tracking systems that are managed by, or on behalf of, the
-      Licensor for the purpose of discussing and improving the Work, but
-      excluding communication that is conspicuously marked or otherwise
-      designated in writing by the copyright owner as "Not a Contribution."
-
-      "Contributor" shall mean Licensor and any individual or Legal Entity
-      on behalf of whom a Contribution has been received by Licensor and
-      subsequently incorporated within the Work.
-
-   2. Grant of Copyright License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      copyright license to reproduce, prepare Derivative Works of,
-      publicly display, publicly perform, sublicense, and distribute the
-      Work and such Derivative Works in Source or Object form.
-
-   3. Grant of Patent License. Subject to the terms and conditions of
-      this License, each Contributor hereby grants to You a perpetual,
-      worldwide, non-exclusive, no-charge, royalty-free, irrevocable
-      (except as stated in this section) patent license to make, have made,
-      use, offer to sell, sell, import, and otherwise transfer the Work,
-      where such license applies only to those patent claims licensable
-      by such Contributor that are necessarily infringed by their
-      Contribution(s) alone or by combination of their Contribution(s)
-      with the Work to which such Contribution(s) was submitted. If You
-      institute patent litigation against any entity (including a
-      cross-claim or counterclaim in a lawsuit) alleging that the Work
-      or a Contribution incorporated within the Work constitutes direct
-      or contributory patent infringement, then any patent licenses
-      granted to You under this License for that Work shall terminate
-      as of the date such litigation is filed.
-
-   4. Redistribution. You may reproduce and distribute copies of the
-      Work or Derivative Works thereof in any medium, with or without
-      modifications, and in Source or Object form, provided that You
-      meet the following conditions:
-
-      (a) You must give any other recipients of the Work or
-          Derivative Works a copy of this License; and
-
-      (b) You must cause any modified files to carry prominent notices
-          stating that You changed the files; and
-
-      (c) You must retain, in the Source form of any Derivative Works
-          that You distribute, all copyright, patent, trademark, and
-          attribution notices from the Source form of the Work,
-          excluding those notices that do not pertain to any part of
-          the Derivative Works; and
-
-      (d) If the Work includes a "NOTICE" text file as part of its
-          distribution, then any Derivative Works that You distribute must
-          include a readable copy of the attribution notices contained
-          within such NOTICE file, excluding those notices that do not
-          pertain to any part of the Derivative Works, in at least one
-          of the following places: within a NOTICE text file distributed
-          as part of the Derivative Works; within the Source form or
-          documentation, if provided along with the Derivative Works; or,
-          within a display generated by the Derivative Works, if and
-          wherever such third-party notices normally appear. The contents
-          of the NOTICE file are for informational purposes only and
-          do not modify the License. You may add Your own attribution
-          notices within Derivative Works that You distribute, alongside
-          or as an addendum to the NOTICE text from the Work, provided
-          that such additional attribution notices cannot be construed
-          as modifying the License.
-
-      You may add Your own copyright statement to Your modifications and
-      may provide additional or different license terms and conditions
-      for use, reproduction, or distribution of Your modifications, or
-      for any such Derivative Works as a whole, provided Your use,
-      reproduction, and distribution of the Work otherwise complies with
-      the conditions stated in this License.
-
-   5. Submission of Contributions. Unless You explicitly state otherwise,
-      any Contribution intentionally submitted for inclusion in the Work
-      by You to the Licensor shall be under the terms and conditions of
-      this License, without any additional terms or conditions.
-      Notwithstanding the above, nothing herein shall supersede or modify
-      the terms of any separate license agreement you may have executed
-      with Licensor regarding such Contributions.
-
-   6. Trademarks. This License does not grant permission to use the trade
-      names, trademarks, service marks, or product names of the Licensor,
-      except as required for reasonable and customary use in describing the
-      origin of the Work and reproducing the content of the NOTICE file.
-
-   7. Disclaimer of Warranty. Unless required by applicable law or
-      agreed to in writing, Licensor provides the Work (and each
-      Contributor provides its Contributions) on an "AS IS" BASIS,
-      WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
-      implied, including, without limitation, any warranties or conditions
-      of TITLE, NON-INFRINGEMENT, MERCHANTABILITY, or FITNESS FOR A
-      PARTICULAR PURPOSE. You are solely responsible for determining the
-      appropriateness of using or redistributing the Work and assume any
-      risks associated with Your exercise of permissions under this License.
-
-   8. Limitation of Liability. In no event and under no legal theory,
-      whether in tort (including negligence), contract, or otherwise,
-      unless required by applicable law (such as deliberate and grossly
-      negligent acts) or agreed to in writing, shall any Contributor be
-      liable to You for damages, including any direct, indirect, special,
-      incidental, or consequential damages of any character arising as a
-      result of this License or out of the use or inability to use the
-      Work (including but not limited to damages for loss of goodwill,
-      work stoppage, computer failure or malfunction, or any and all
-      other commercial damages or losses), even if such Contributor
-      has been advised of the possibility of such damages.
-
-   9. Accepting Warranty or Additional Liability. While redistributing
-      the Work or Derivative Works thereof, You may choose to offer,
-      and charge a fee for, acceptance of support, warranty, indemnity,
-      or other liability obligations and/or rights consistent with this
-      License. However, in accepting such obligations, You may act only
-      on Your own behalf and on Your sole responsibility, not on behalf
-      of any other Contributor, and only if You agree to indemnify,
-      defend, and hold each Contributor harmless for any liability
-      incurred by, or claims asserted against, such Contributor by reason
-      of your accepting any such warranty or additional liability.
-
-   END OF TERMS AND CONDITIONS
-
-   APPENDIX: How to apply the Apache License to your work.
-
-      To apply the Apache License to your work, attach the following
-      boilerplate notice, with the fields enclosed by brackets "[]"
-      replaced with your own identifying information. (Don't include
-      the brackets!)  The text should be enclosed in the appropriate
-      comment syntax for the file format. We also recommend that a
-      file or class name and description of purpose be included on the
-      same "printed page" as the copyright notice for easier
-      identification within third-party archives.
-
-   Copyright 2018-2023 OpenMMLab.
-
-   Licensed under the Apache License, Version 2.0 (the "License");
-   you may not use this file except in compliance with the License.
-   You may obtain a copy of the License at
-
-       http://www.apache.org/licenses/LICENSE-2.0
-
-   Unless required by applicable law or agreed to in writing, software
-   distributed under the License is distributed on an "AS IS" BASIS,
-   WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
-   See the License for the specific language governing permissions and
-   limitations under the License.
+END OF TERMS AND CONDITIONS
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `mlcvzoo_mmdetection-5.1.1/pyproject.toml` & `mlcvzoo_mmdetection-6.0.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "mlcvzoo_mmdetection"
-version = "5.1.1"
-license = "Open Logistics License Version 1.0"
 description = "MLCVZoo MMDetection Package"
+version = "6.0.0"
+license = "Open Logistics Foundation License 1.3"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
@@ -32,20 +32,21 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 
 yaml-config-builder = { version = "^8" }
 related-mltoolbox = { version = "^1" }
 mlcvzoo_base = { version = "^5" }
 
-attrs = { version = ">=20" }
 # 4.6.0.66 leads to errors when building mmcv-full
-opencv-python = { version = "^4.5,!=4.5.5.64,!=4.6.0.66" }
-opencv-contrib-python = { version = "^4.5,!=4.5.5.64,!=4.6.0.66" }
-mmdet = { version="^2.14.0" }
-mmcv-full = { version="^1.3,!=1.3.18" }
+opencv-python = { version = ">=4.5,!=4.5.5.64,!=4.6.0.66" }
+opencv-contrib-python = { version = ">=4.5,!=4.5.5.64,!=4.6.0.66" }
+attrs = { version = ">=20" }
+mmcv = { version = "^2" }
+mmengine = { version= "^0.7" }
+mmdet = { version = "^3" }
 pycocotools = { version=">=2.0.2", markers = "platform_machine == 'x86_64'" }
 # 1.19.2 is oldest available on aarch64 but 1.19.5 leads to unbuildable pytorch there, all is well on amd64
 numpy = { version = ">=1.19.2,!=1.19.5" }
 nptyping = { version = ">=2.0" }
 # torch 2.0.1 has missing cuda dependencies https://github.com/pytorch/pytorch/issues/100974
 torch = { version = ">=1.9,!=2.0.1" }
 torchvision = { version = ">=0.10" }
@@ -53,16 +54,19 @@
 [tool.poetry.dev-dependencies]
 mock = { version = ">=4.0" }
 pytest = { version = ">=7.0" }
 pytest-cov = { version = ">=3.0.0" }
 black = { version = ">=22" }
 mypy = { version = ">=0.961" }
 pylint = { version = ">=2.9.6" }
-isort = { version = ">=5.9" }
-pytest-mock = ">=3.7"
+# Isort guarantees formatting results for 5.X
+isort = { version = "^5.0" }
+pytest-mock = { version = ">=3.7" }
+# Needed by mmdetection but currently only used in unit tests
+panopticapi = { git = "https://github.com/cocodataset/panopticapi.git", rev = "7bb4655548f98f3fedc07bf37e9040a992b054b0"}
 
 [build-system]
 # NOTE: Don't remove setuptools, therefore require it from the build system
 requires = ["setuptools", "poetry_core>=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
@@ -112,14 +116,15 @@
 module = [
     "cv2", # https://github.com/opencv/opencv/issues/14590
     "keras.*",
     "imageio.*",
     "keras_preprocessing.*",
     "mlflow.*",
     "mmcv.*",
+    "mmengine.*",
     "mmdet.*",
     "mmocr.*",
     "numpy.*",
     "pandas.*",
     "PIL.*",
     "related.*",
     "scipy.*",
```

### Comparing `mlcvzoo_mmdetection-5.1.1/setup.py` & `mlcvzoo_mmdetection-6.0.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # -*- coding: utf-8 -*-
 from setuptools import setup
 
 packages = \
-['mlcvzoo_mmdetection', 'mlcvzoo_mmdetection.third_party']
+['mlcvzoo_mmdetection']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['attrs>=20',
  'mlcvzoo_base>=5,<6',
- 'mmcv-full>=1.3,<2.0,!=1.3.18',
- 'mmdet>=2.14.0,<3.0.0',
+ 'mmcv>=2,<3',
+ 'mmdet>=3,<4',
+ 'mmengine>=0.7,<0.8',
  'nptyping>=2.0',
  'numpy>=1.19.2,!=1.19.5',
- 'opencv-contrib-python>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66',
- 'opencv-python>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66',
+ 'opencv-contrib-python>=4.5,!=4.5.5.64,!=4.6.0.66',
+ 'opencv-python>=4.5,!=4.5.5.64,!=4.6.0.66',
  'related-mltoolbox>=1,<2',
  'torch>=1.9,!=2.0.1',
  'torchvision>=0.10',
  'yaml-config-builder>=8,<9']
 
 extras_require = \
 {':platform_machine == "x86_64"': ['pycocotools>=2.0.2']}
 
 setup_kwargs = {
     'name': 'mlcvzoo-mmdetection',
-    'version': '5.1.1',
+    'version': '6.0.0',
     'description': 'MLCVZoo MMDetection Package',
     'long_description': '# MLCVZoo MMDetection\n\nThe MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)\ncomputer vision algorithms. The package **mlcvzoo_mmdetection** is the wrapper module for\nthe [mmdetection framework](https://github.com/open-mmlab/mmdetection).\n\nFurther information about the MLCVZoo can be found [here](../README.md).\n\n## Install\n`\npip install mlcvzoo-mmdetection\n`\n\n## Technology stack\n\n- Python\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo',
```

### Comparing `mlcvzoo_mmdetection-5.1.1/PKG-INFO` & `mlcvzoo_mmdetection-6.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,33 +1,34 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-mmdetection
-Version: 5.1.1
+Version: 6.0.0
 Summary: MLCVZoo MMDetection Package
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
-License: Open Logistics License Version 1.0
+License: Open Logistics Foundation License 1.3
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: attrs (>=20)
 Requires-Dist: mlcvzoo_base (>=5,<6)
-Requires-Dist: mmcv-full (>=1.3,<2.0,!=1.3.18)
-Requires-Dist: mmdet (>=2.14.0,<3.0.0)
+Requires-Dist: mmcv (>=2,<3)
+Requires-Dist: mmdet (>=3,<4)
+Requires-Dist: mmengine (>=0.7,<0.8)
 Requires-Dist: nptyping (>=2.0)
 Requires-Dist: numpy (>=1.19.2,!=1.19.5)
-Requires-Dist: opencv-contrib-python (>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66)
-Requires-Dist: opencv-python (>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66)
+Requires-Dist: opencv-contrib-python (>=4.5,!=4.5.5.64,!=4.6.0.66)
+Requires-Dist: opencv-python (>=4.5,!=4.5.5.64,!=4.6.0.66)
 Requires-Dist: pycocotools (>=2.0.2) ; platform_machine == "x86_64"
 Requires-Dist: related-mltoolbox (>=1,<2)
 Requires-Dist: torch (>=1.9,!=2.0.1)
 Requires-Dist: torchvision (>=0.10)
 Requires-Dist: yaml-config-builder (>=8,<9)
 Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc
 Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
```

