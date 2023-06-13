# Comparing `tmp/ai2_kit-0.1.0.tar.gz` & `tmp/ai2_kit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai2_kit-0.1.0.tar", max compression
+gzip compressed data, was "ai2_kit-0.2.0.tar", max compression
```

## Comparing `ai2_kit-0.1.0.tar` & `ai2_kit-0.2.0.tar`

### file list

```diff
@@ -1,25 +1,37 @@
--rw-r--r--   0        0        0     2312 2023-02-06 09:01:07.346349 ai2_kit-0.1.0/README.md
--rw-r--r--   0        0        0        0 2022-12-05 07:55:59.399408 ai2_kit-0.1.0/ai2_kit/__init__.py
--rw-r--r--   0        0        0        0 2022-12-05 07:55:59.399408 ai2_kit-0.1.0/ai2_kit/core/__init__.py
--rw-r--r--   0        0        0      473 2023-02-06 08:57:34.086411 ai2_kit-0.1.0/ai2_kit/core/artifact.py
--rw-r--r--   0        0        0     3116 2023-02-06 08:57:34.086411 ai2_kit-0.1.0/ai2_kit/core/checkpoint.py
--rw-r--r--   0        0        0     5766 2023-02-06 08:57:34.086411 ai2_kit-0.1.0/ai2_kit/core/connector.py
--rw-r--r--   0        0        0     6714 2023-02-06 08:57:34.086411 ai2_kit-0.1.0/ai2_kit/core/executor.py
--rw-r--r--   0        0        0     3988 2023-02-06 08:57:34.086411 ai2_kit-0.1.0/ai2_kit/core/job.py
--rw-r--r--   0        0        0      118 2023-01-12 06:31:12.298011 ai2_kit-0.1.0/ai2_kit/core/log.py
--rw-r--r--   0        0        0     8346 2023-02-06 08:57:34.086411 ai2_kit-0.1.0/ai2_kit/core/queue_system.py
--rw-r--r--   0        0        0     2358 2023-02-06 08:57:34.086411 ai2_kit-0.1.0/ai2_kit/core/script.py
--rw-r--r--   0        0        0     1377 2023-02-06 08:57:34.086411 ai2_kit-0.1.0/ai2_kit/core/util.py
--rw-r--r--   0        0        0        0 2022-12-09 08:45:06.073203 ai2_kit-0.1.0/ai2_kit/domain/__init__.py
--rw-r--r--   0        0        0      341 2023-02-06 08:57:34.086411 ai2_kit-0.1.0/ai2_kit/domain/constant.py
--rw-r--r--   0        0        0     8718 2023-02-06 08:57:34.086411 ai2_kit-0.1.0/ai2_kit/domain/cp2k.py
--rw-r--r--   0        0        0     5008 2023-02-06 08:57:34.086411 ai2_kit-0.1.0/ai2_kit/domain/deepmd.py
--rw-r--r--   0        0        0    12950 2023-02-06 08:57:34.086411 ai2_kit-0.1.0/ai2_kit/domain/lammps.py
--rw-r--r--   0        0        0     2234 2023-02-06 08:57:34.096411 ai2_kit-0.1.0/ai2_kit/domain/selector.py
--rw-r--r--   0        0        0      649 2023-02-06 08:57:34.096411 ai2_kit-0.1.0/ai2_kit/main.py
--rw-r--r--   0        0        0        0 2022-12-09 08:45:06.073203 ai2_kit-0.1.0/ai2_kit/workflow/__init__.py
--rw-r--r--   0        0        0     6054 2023-02-06 08:57:34.096411 ai2_kit-0.1.0/ai2_kit/workflow/cll_mlp.py
--rw-r--r--   0        0        0     7712 2023-02-06 08:57:34.096411 ai2_kit-0.1.0/ai2_kit/workflow/fep.py
--rw-r--r--   0        0        0      779 2023-02-06 08:57:34.096411 ai2_kit-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     3362 1970-01-01 00:00:00.000000 ai2_kit-0.1.0/setup.py
--rw-r--r--   0        0        0     3168 1970-01-01 00:00:00.000000 ai2_kit-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-02-07 08:30:11.900671 ai2_kit-0.2.0/LICENSE
+-rw-r--r--   0        0        0     1170 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.2.0/ai2_kit/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/ai2_kit/algorithm/__init__.py
+-rw-r--r--   0        0        0    12100 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/ai2_kit/algorithm/proton_transfer.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.2.0/ai2_kit/core/__init__.py
+-rw-r--r--   0        0        0     1884 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/core/artifact.py
+-rw-r--r--   0        0        0     3327 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/core/checkpoint.py
+-rw-r--r--   0        0        0      169 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/ai2_kit/core/cmd.py
+-rw-r--r--   0        0        0     5766 2023-02-06 09:01:27.000000 ai2_kit-0.2.0/ai2_kit/core/connector.py
+-rw-r--r--   0        0        0     7717 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/core/executor.py
+-rw-r--r--   0        0        0     1074 2023-02-22 05:58:23.102960 ai2_kit-0.2.0/ai2_kit/core/future.py
+-rw-r--r--   0        0        0     2995 2023-02-17 02:09:28.820341 ai2_kit-0.2.0/ai2_kit/core/job.py
+-rw-r--r--   0        0        0      118 2023-02-06 09:01:27.000000 ai2_kit-0.2.0/ai2_kit/core/log.py
+-rw-r--r--   0        0        0     8346 2023-03-02 05:16:23.680695 ai2_kit-0.2.0/ai2_kit/core/queue_system.py
+-rw-r--r--   0        0        0     2315 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/core/resource_manager.py
+-rw-r--r--   0        0        0     2358 2023-02-27 06:41:41.002117 ai2_kit-0.2.0/ai2_kit/core/script.py
+-rw-r--r--   0        0        0     1949 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/core/util.py
+-rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/ai2_kit/dflow/__init__.py
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.2.0/ai2_kit/domain/__init__.py
+-rw-r--r--   0        0        0     2232 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/domain/cll.py
+-rw-r--r--   0        0        0      341 2023-02-27 08:58:57.520622 ai2_kit-0.2.0/ai2_kit/domain/constant.py
+-rw-r--r--   0        0        0     8122 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/domain/cp2k.py
+-rw-r--r--   0        0        0     4121 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/domain/data_helper.py
+-rw-r--r--   0        0        0     6523 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/domain/deepmd.py
+-rw-r--r--   0        0        0    15627 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/domain/lammps.py
+-rw-r--r--   0        0        0     3173 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/domain/selector.py
+-rw-r--r--   0        0        0      183 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/domain/updater.py
+-rw-r--r--   0        0        0      949 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/ai2_kit/main.py
+-rw-r--r--   0        0        0        0 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/ai2_kit/tools/__init__.py
+-rw-r--r--   0        0        0      239 2023-06-13 03:47:09.348444 ai2_kit-0.2.0/ai2_kit/tools/demo.yaml
+-rw-r--r--   0        0        0        0 2023-02-06 09:01:27.000000 ai2_kit-0.2.0/ai2_kit/workflow/__init__.py
+-rw-r--r--   0        0        0     7426 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/workflow/cll_mlp.py
+-rw-r--r--   0        0        0     7755 2023-03-22 04:23:44.538179 ai2_kit-0.2.0/ai2_kit/workflow/ec_fep.py
+-rw-r--r--   0        0        0      821 2023-06-13 03:51:03.222343 ai2_kit-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 ai2_kit-0.2.0/setup.py
+-rw-r--r--   0        0        0     2154 1970-01-01 00:00:00.000000 ai2_kit-0.2.0/PKG-INFO
```

### Comparing `ai2_kit-0.1.0/ai2_kit/core/connector.py` & `ai2_kit-0.2.0/ai2_kit/core/connector.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.1.0/ai2_kit/core/executor.py` & `ai2_kit-0.2.0/ai2_kit/core/executor.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,51 +1,60 @@
 from .queue_system import QueueSystemConfig, BaseQueueSystem, Slrum, Lsf
-from .job import JobState
+from .job import JobFuture
 from .artifact import Artifact
 from .connector import SshConfig, BaseConnector, SshConnector, LocalConnector
+from .util import s_uuid
+from .log import get_logger
+
+logger = get_logger(__name__)
 
 from pydantic import BaseModel
-from typing import Optional, Dict, List, TypeVar, Callable
+from typing import Optional, Dict, List, TypeVar, Callable, Mapping
 from abc import ABC, abstractmethod
 from invoke import Result
 import os
 import shlex
 import base64
+import bz2
 import cloudpickle
 
 
 class BaseExecutorConfig(BaseModel):
     ssh: Optional[SshConfig]
     queue_system: QueueSystemConfig
     work_dir: str
     python_cmd: str = 'python'
 
+ExecutorMap = Mapping[str, BaseExecutorConfig]
+
 FnType = TypeVar('FnType', bound=Callable)
 
 class Executor(ABC):
 
     name: str
+    work_dir: str
+    tmp_dir: str
+    python_cmd: str
+
+    def init(self):
+        ...
 
     @abstractmethod
     def mkdir(self, path: str):
         ...
 
     @abstractmethod
     def run_python_script(self, script: str, python_cmd=None):
         ...
 
     @abstractmethod
     def run_python_fn(self, fn: FnType, python_cmd=None) -> FnType:
         ...
 
     @abstractmethod
-    def get_full_path(self, path: str) -> str:
-        ...
-
-    @abstractmethod
     def dump_text(self, text: str, path: str):
         ...
 
     @abstractmethod
     def load_text(self, path: str) -> str:
         ...
 
@@ -54,33 +63,35 @@
         ...
 
     @abstractmethod
     def run(self, script: str, **kwargs) -> Result:
         ...
 
     @abstractmethod
-    def submit(self, script: str, **kwargs) -> JobState:
+    def submit(self, script: str, **kwargs) -> JobFuture:
         ...
 
     @abstractmethod
     def upload(self, from_artifact: Artifact, to_dir: str) -> Artifact:
         ...
 
     @abstractmethod
     def download(self, from_artifact: Artifact, to_dir: str) -> Artifact:
         ...
 
     @abstractmethod
-    def sym_link(self, from_artifact: Artifact, to_dir: str) -> Artifact:
-        ...
-
-    @abstractmethod
-    def unpack_artifact(self, artifact: Artifact) -> List[str]:
+    def resolve_artifact(self, artifact: Artifact) -> List[str]:
         ...
 
+    def setup_workspace(self, workspace_dir: str, dirs: List[str]):
+        paths = [os.path.join(workspace_dir, dir) for dir in dirs]
+        for path in paths :
+            self.mkdir(path)
+            logger.info('create path: %s', path)
+        return paths
 
 class HpcExecutor(Executor):
 
     @classmethod
     def from_config(cls, config: BaseExecutorConfig, name: str):
         if config.ssh:
             connector = SshConnector.from_config(config.ssh)
@@ -104,17 +115,19 @@
 
     def __init__(self, connector: BaseConnector, queue_system: BaseQueueSystem, work_dir: str, python_cmd: str, name: str):
         self.name = name
         self.connector = connector
         self.queue_system = queue_system
         self.work_dir = work_dir
         self.python_cmd = python_cmd
+        self.tmp_dir = os.path.join(self.work_dir, '.tmp')  # TODO: make it configurable
 
-    def get_full_path(self, path: str):
-        return os.path.join(self.work_dir, path)
+    def init(self):
+        self.mkdir(self.work_dir)
+        self.mkdir(self.tmp_dir)
 
     def mkdir(self, path: str):
         return self.connector.run('mkdir -p {}'.format(shlex.quote(path)))
 
     def dump_text(self, text: str, path: str):
         return self.connector.dump_text(text, path)
 
@@ -124,34 +137,46 @@
 
     def glob(self, pattern: str):
         return self.connector.glob(pattern)
 
     def run(self, script: str, **kwargs):
         return self.connector.run(script, **kwargs)
 
-    def run_python_script(self, script: str, python_cmd=None):
+    def run_python_script(self, script: str, python_cmd=None, cwd=None):
         if python_cmd is None:
             python_cmd = self.python_cmd
-        return self.connector.run('{} -c {}'.format(python_cmd, shlex.quote(script)))
+        if cwd is None:
+            cwd = self.work_dir
+        cd_cwd = f'cd {shlex.quote(cwd)}  &&'
+        script_len = len(script)
+        logger.info('the size of generated python script is %s', script_len)
+        if script_len < 100_000: # ssh connection will be closed of the size of command is too large
+            return self.connector.run(f'{cd_cwd} {python_cmd} -c {shlex.quote(script)}', hide=True)
+        else:
+            script_path = os.path.join(self.tmp_dir, f'run_python_script_{s_uuid()}.py')
+            self.dump_text(script, script_path)
+            ret = self.connector.run(f'{cd_cwd} {python_cmd} {shlex.quote(script_path)}', hide=True)
+            self.connector.run(f'rm {shlex.quote(script_path)}')
+            return ret
 
-    def run_python_fn(self, fn: FnType, python_cmd=None) -> FnType:
+    def run_python_fn(self, fn: FnType, python_cmd=None, cwd=None) -> FnType:
         def remote_fn(*args, **kwargs):
             script = fn_to_script(lambda: fn(*args, **kwargs), delimiter='@')
-            ret = self.run_python_script(script=script, python_cmd=python_cmd)
+            ret = self.run_python_script(script=script, python_cmd=python_cmd, cwd=None)
             _, r = ret.stdout.rsplit('@')
-            return cloudpickle.loads(base64.b64decode(r))
+            return cloudpickle.loads(bz2.decompress(base64.b64decode(r)))
         return remote_fn  # type: ignore
 
     def submit(self, script: str, cwd: str, **kwargs):
         return self.queue_system.submit(script, cwd=cwd, **kwargs)
 
-    def unpack_artifact(self, artifact: Artifact) -> List[str]:
-        if artifact.glob is None:
+    def resolve_artifact(self, artifact: Artifact) -> List[str]:
+        if artifact.includes is None:
             return [artifact.url]
-        pattern = os.path.join(artifact.url, artifact.glob)
+        pattern = os.path.join(artifact.url, artifact.includes)
         return self.glob(pattern)
 
     def upload(self, from_artifact: Artifact, to_dir: str) -> Artifact:
         dest_path = self.connector.upload(from_artifact.url, to_dir)
         return Artifact(
             executor=self.name,
             url=dest_path,
@@ -161,31 +186,23 @@
     def download(self, from_artifact: Artifact, to_dir: str) -> Artifact:
         dest_path = self.connector.download(from_artifact.url, to_dir)
         return Artifact(
             url=dest_path,
             attrs=from_artifact.attrs,
         ) # type: ignore
 
-    def sym_link(self, from_artifact: Artifact, to_dir: str) -> Artifact:
-        dest_path = self.connector.sym_link(from_artifact.url, to_dir)
-        return Artifact(
-            executor=from_artifact.executor,
-            url=dest_path,
-            attrs=from_artifact.attrs,
-        ) # type: ignore
-
 
 def create_executor(config: BaseExecutorConfig, name: str) -> Executor:
     if config.queue_system is not None:
         return HpcExecutor.from_config(config, name)
     raise RuntimeError('The executor configuration is not supported!')
 
 
 class ExecutorManager:
-    def __init__(self, executor_configs: Dict[str, BaseExecutorConfig]):
+    def __init__(self, executor_configs: Mapping[str, BaseExecutorConfig]):
         self._executor_configs = executor_configs
         self._executors: Dict[str, Executor] = dict()
 
     def get_executor(self, name: str):
         config = self._executor_configs.get(name)
         if config is None:
             raise ValueError(
@@ -195,14 +212,16 @@
             executor = create_executor(config, name)
             self._executors[name] = executor
 
         return self._executors[name]
 
 
 def fn_to_script(fn: Callable, delimiter='@'):
-    dumped_fn = base64.b64encode(cloudpickle.dumps(fn, protocol=cloudpickle.DEFAULT_PROTOCOL))
+    dumped_fn = base64.b64encode(bz2.compress(cloudpickle.dumps(fn, protocol=cloudpickle.DEFAULT_PROTOCOL), 5))
     script = [
-        f'''import base64,cloudpickle as cp''',
-        f'''r=cp.loads(base64.b64decode({repr(dumped_fn)}))()''',
-        f'''print({repr(delimiter)}+base64.b64encode(cp.dumps(r, protocol=cp.DEFAULT_PROTOCOL)).decode('ascii'))''',
+        f'''import base64,bz2,sys,cloudpickle as cp''',
+        f'''r=cp.loads(bz2.decompress(base64.b64decode({repr(dumped_fn)})))()''',
+        f'''sys.stdout.flush()''',  # avoid overlapping
+        f'''print({repr(delimiter)}+base64.b64encode(bz2.compress(cp.dumps(r, protocol=cp.DEFAULT_PROTOCOL),5)).decode('ascii'))''',
+        f'''sys.stdout.flush()''',  # ensure all output is printed
     ]
     return ';'.join(script)
```

### Comparing `ai2_kit-0.1.0/ai2_kit/core/queue_system.py` & `ai2_kit-0.2.0/ai2_kit/core/queue_system.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.1.0/ai2_kit/core/script.py` & `ai2_kit-0.2.0/ai2_kit/core/script.py`

 * *Files identical despite different names*

### Comparing `ai2_kit-0.1.0/ai2_kit/core/util.py` & `ai2_kit-0.2.0/ai2_kit/core/util.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,25 +1,33 @@
 from ruamel.yaml import YAML
 from pathlib import Path
-from typing import Tuple
+from typing import Tuple, List, TypeVar
+from dataclasses import field
+from cp2k_input_tools.parser import CP2KInputParserSimplified
+
 import shortuuid
 import copy
-from dataclasses import field
+import os
+import io
+
+from .log import get_logger
+
+logger = get_logger(__name__)
 
 def default_mutable_field(obj):
     return field(default_factory=lambda: copy.copy(obj))
 
 def __merge_dict():
-    """
-    merge two dict, the left dict will be overridden
-    this method won't merge list
-
-    cloudpickle compatible: https://stackoverflow.com/questions/75292769
-    """
+    """cloudpickle compatible: https://stackoverflow.com/questions/75292769"""
     def merge_dict(lo: dict, ro: dict, path=None):
+        """
+        merge two dict, the left dict will be overridden
+
+        this method won't merge list
+        """
         if path is None:
             path = []
 
         for key, value in ro.items():
             if key in lo:
                 current_path = path + [ str(key) ]
                 if isinstance(lo[key], dict) and isinstance(value, dict):
@@ -40,13 +48,29 @@
     return yaml.load(path)
 
 
 def load_yaml_files(*paths: Tuple[Path]):
     d = {}
     for path in paths:
         print('load yaml file: ', path)
-        d = merge_dict(d, load_yaml_file(Path(path)))
+        d = merge_dict(d, load_yaml_file(Path(path)))  # type: ignore
     return d
 
 
-def tmpfile_name():
+def s_uuid():
+    """short uuid"""
     return shortuuid.uuid()
+
+
+def parse_cp2k_input(text: str):
+    parser = CP2KInputParserSimplified()
+    return parser.parse(io.StringIO(text))
+
+
+def sort_unique_str_list(l: List[str]) -> List[str]:
+    """remove duplicate str and sort"""
+    return list(sorted(set(l)))
+
+
+T = TypeVar('T')
+def flatten(l: List[List[T]]) -> List[T]:
+    return [item for sublist in l for item in sublist]
```

### Comparing `ai2_kit-0.1.0/ai2_kit/domain/cp2k.py` & `ai2_kit-0.2.0/ai2_kit/domain/cp2k.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,250 +1,224 @@
-from ai2_kit.core.executor import Executor
 from ai2_kit.core.artifact import Artifact
 from ai2_kit.core.script import BashScript, BashStep, BashTemplate
-from ai2_kit.core.job import GatherJobsFuture, MapFuture, retry_fn, DummyFuture, IFuture
+from ai2_kit.core.job import GatherJobsFuture, retry_fn
 
-from ai2_kit.core.util import merge_dict
-from ai2_kit.core.log import get_logger
+from ai2_kit.core.future import DummyFuture, IFuture, map_future
 
+from ai2_kit.core.util import merge_dict, parse_cp2k_input
+from ai2_kit.core.log import get_logger
 
-from typing import List, Optional
+from typing import List, Union
 from pydantic import BaseModel
 from dataclasses import dataclass
 
 import copy
 import os
 
-from .constant import (
-    LAMMPS_TRAJ_DIR,
-    LAMMPS_TRAJ_SUFFIX,
-)
+from .data_helper import LammpsOutputHelper, XyzHelper, Cp2kOutputHelper, ase_atoms_to_cp2k_input_data
+from .cll import ICllLabelInput, ICllLabelOutput, BaseCllContext
 
 logger = get_logger(__name__)
 
-class GeneralCp2kInputConfig(BaseModel):
-    max_candidates: int = 50
-    input_template: dict
-    basic_set_file: Optional[str]
-    potential_file: Optional[str]
+class GenericCp2kInputConfig(BaseModel):
+    init_system_files: List[str] = []
+    limit: int = 50
+    input_template: Union[dict, str]
+    """
+    Input template for cp2k. Could be a dict or content of a cp2k input file.
+
+    Note:
+    If you are using files in input templates, it is recommended to use artifact name instead of literal path.
+    String starts with '@' will be treated as artifact name.
+    For examples, FORCE_EVAL/DFT/BASIS_SET_FILE_NAME = @cp2k/basic_set.
+    You can still use literal path, but it is not recommended.
+    """
 
-class GeneralCp2kContextConfig(BaseModel):
+class GenericCp2kContextConfig(BaseModel):
     script_template: BashTemplate
     cp2k_cmd: str = 'cp2k'
     concurrency: int = 5
 
 @dataclass
-class GeneralCp2kInput:
-    config: GeneralCp2kInputConfig
-    candidates: List[Artifact]
+class GenericCp2kInput(ICllLabelInput):
+
+    config: GenericCp2kInputConfig
+    system_files: List[Artifact]
     type_map: List[str]
+    initiated: bool = False
+
+    def set_systems(self, systems: List[Artifact]):
+        self.system_files = systems
 
-    basic_set_file: Optional[Artifact] = None
-    potential_file: Optional[Artifact] = None
 
 @dataclass
-class GeneralCp2kContext:
-    config: GeneralCp2kContextConfig
-    executor: Executor
-    path_prefix: str
+class GenericCp2kContext(BaseCllContext):
+    config: GenericCp2kContextConfig
+
 
 @dataclass
-class GeneralCp2kOutput:
-    dp_data_sets: List[Artifact]
+class GenericCp2kOutput(ICllLabelOutput):
     cp2k_outputs: List[Artifact]
 
-def general_cp2k(input: GeneralCp2kInput, ctx: GeneralCp2kContext) -> IFuture[GeneralCp2kOutput]:
-    # setup dirs
-    work_dir = ctx.executor.get_full_path(ctx.path_prefix)
-    ctx.executor.mkdir(work_dir)
-    logger.info('work_dir is %s', work_dir)
-
-    tasks_dir = os.path.join(work_dir, 'tasks')
-    ctx.executor.mkdir(tasks_dir)
-    logger.info('tasks_dir is %s', tasks_dir)
-
-    dp_data_dir = os.path.join(work_dir, 'output_dp_data')
-    ctx.executor.mkdir(dp_data_dir)
-    logger.info('dp_data_dir is %s', dp_data_dir)
-
-    # resolve input template
-    input_template = copy.deepcopy(input.config.input_template)
-    # FIXME: potential_file and basic_set_file should be list
-    if input.basic_set_file is not None:
-        merge_dict(input_template,  {
-            'FORCE_EVAL': {
-                'DFT': {
-                    'BASIS_SET_FILE_NAME': input.basic_set_file.url,
-                }
-            }
-        })
-    if input.potential_file is not None:
-        merge_dict(input_template,  {
-            'FORCE_EVAL': {
-                'DFT': {
-                    'POTENTIAL_FILE_NAME': input.potential_file.url,
-                }
-            }
-        })
+    def get_labeled_system_dataset(self):
+        return self.cp2k_outputs
 
-    # resolve candidate files
-    lammps_traj_files = []
 
-    for candidate in input.candidates:
-        by = candidate.attrs['by']
-        if by == 'lammps':
-            traj_files = [os.path.join(candidate.url, LAMMPS_TRAJ_DIR, f'{i}{LAMMPS_TRAJ_SUFFIX}') for i in candidate.attrs['passed']]
-            lammps_traj_files.extend(traj_files)
-        else:
-            logger.warn('skip unsupported data source: %s, generated by: %s', candidate.url, by)
-            continue
+def generic_cp2k(input: GenericCp2kInput, ctx: GenericCp2kContext) -> IFuture[GenericCp2kOutput]:
+
+    executor = ctx.resource_manager.default_executor
+
+    # For the first round
+    if not input.initiated:
+        input.system_files += ctx.resource_manager.get_artifacts(input.config.init_system_files)
+
+    # setup workspace
+    work_dir = os.path.join(executor.work_dir, ctx.path_prefix)
+    [tasks_dir] = executor.setup_workspace(work_dir, ['tasks'])
 
-    # limit max_candidates
-    # TODO: allow user to choose random sample
-    lammps_traj_files = lammps_traj_files[:input.config.max_candidates]
+    # prepare input template
+    if isinstance(input.config.input_template, str):
+        input_template = parse_cp2k_input(input.config.input_template)
+    else:
+        input_template = copy.deepcopy(input.config.input_template)
+
+    # resolve artifacts resources in the input template
+    basic_set_file: str = input_template['FORCE_EVAL']['DFT']['BASIS_SET_FILE_NAME']
+    if basic_set_file.startswith('@'):
+        logger.info(f'resolve artifact {basic_set_file}')
+        input_template['FORCE_EVAL']['DFT']['BASIS_SET_FILE_NAME'] = \
+            ctx.resource_manager.resolve_artifact(basic_set_file[1:])[0].url
+
+    potential_file: str = input_template['FORCE_EVAL']['DFT']['POTENTIAL_FILE_NAME']
+    if potential_file.startswith('@'):
+        logger.info(f'resolve artifact {potential_file}')
+        input_template['FORCE_EVAL']['DFT']['POTENTIAL_FILE_NAME'] = \
+            ctx.resource_manager.resolve_artifact(potential_file[1:])[0].url
+
+    # resolve data files
+    lammps_dump_files: List[Artifact] = []
+    xyz_files: List[Artifact] = []
+
+    # TODO: support POSCAR in the future
+    # TODO: refactor the way of handling different file formats
+    for system_file in input.system_files:
+        if LammpsOutputHelper.is_match(system_file):
+            lammps_out = LammpsOutputHelper(system_file)
+            lammps_dump_files.extend(lammps_out.get_passed_dump_files())
+        elif XyzHelper.is_match(system_file):
+            xyz_files.append(system_file)
+        else:
+            raise ValueError(f'unsupported format {system_file.url}: {system_file.format}')
 
     # create task dirs and prepare input files
     cp2k_task_dirs = []
-    if lammps_traj_files:
-        cp2k_task_dirs = [
-            os.path.join(tasks_dir, str(i).zfill(6))
-            for i in range(len(lammps_traj_files))
-        ]
-        ctx.executor.run_python_fn(make_cp2k_task_dirs)(
-            task_dirs=cp2k_task_dirs,
-            traj_files=lammps_traj_files,
-            traj_fmt='lammps/dump',
+    if lammps_dump_files or xyz_files:
+        cp2k_task_dirs = executor.run_python_fn(make_cp2k_task_dirs)(
+            lammps_dump_files=[a.url for a in lammps_dump_files],
+            xyz_files=[a.url for a in xyz_files],
             type_map=input.type_map,
+            base_dir=tasks_dir,
             input_template=input_template,
+            limit=input.config.limit,
         )
     else:
-        logger.warn('no available candidates')
-        return DummyFuture(GeneralCp2kOutput(dp_data_sets=[], cp2k_outputs=[]))
+        logger.warn('no available candidates, skip')
+        return DummyFuture(GenericCp2kOutput(cp2k_outputs=[]))
 
-    # run cp2k tasks
-    # group tasks by concurrency
+    # group cp2k tasks by concurrency
     concurrency = ctx.config.concurrency
     steps_group = [list() for _ in range(concurrency)]
     for i, cp2k_task_dir in enumerate(cp2k_task_dirs):
         steps = steps_group[i % concurrency]
         step = BashStep(
             cwd=cp2k_task_dir,
             cmd=[ctx.config.cp2k_cmd, '-i input.inp 1>> output 2>> output'],
             checkpoint='cp2k',
         )
         steps.append(step)
 
+    # run tasks
     jobs = []
     for steps in steps_group:
         if not steps:
             continue
         script = BashScript(
             template=ctx.config.script_template,
             steps=steps,
         )
-        job = ctx.executor.submit(script.render(), cwd=tasks_dir)
+        job = executor.submit(script.render(), cwd=tasks_dir)
         jobs.append(job)
 
     future = GatherJobsFuture(jobs, done_fn=retry_fn(max_tries=2), raise_exception=True)
 
-    # TODO: use a common intermediate data format instead of deepmd/npy
-    # ref: https://www.reddit.com/r/comp_chem/comments/10q0isd/whats_the_best_data_format_to_transfer/
-    def convert_to_dp_data(_):
-        ctx.executor.run_python_fn(cp2k_output_to_dp_data)(
-            task_dirs=cp2k_task_dirs,
-            output_dir=dp_data_dir,
-            type_map=input.type_map)
-        dp_data_sets =[
-            Artifact(
-                executor=ctx.executor.name,
-                url=dp_data_dir,
-                attrs=dict(fmt='deepmd', set_size=len(cp2k_task_dirs))
-            ), # type: ignore
-        ]
-        cp2k_outputs = [
-            Artifact(
-                executor=ctx.executor.name,
-                url=task_dir,
-                attrs=dict(fmt='cp2k')
-            )  for task_dir in cp2k_task_dirs  # type: ignore
-        ]
-        return GeneralCp2kOutput(dp_data_sets=dp_data_sets, cp2k_outputs=cp2k_outputs)
-    return MapFuture(future, convert_to_dp_data)
+    cp2k_outputs = [Artifact.of(
+        url=url,
+        format=Cp2kOutputHelper.format,
+        executor=executor.name,
+        attrs=dict(),  # TODO: success from input
+    ) for url in cp2k_task_dirs]
+
+    return map_future(future, GenericCp2kOutput(cp2k_outputs=cp2k_outputs))
 
 
 def __make_cp2k_task_dirs():
-    """cloudpickle compatible: https://stackoverflow.com/questions/75292769"""
-    def make_cp2k_task_dirs(traj_files: List[str],
-                            task_dirs: List[str],
+    def make_cp2k_task_dirs(lammps_dump_files: List[str],
+                            xyz_files: List[str],
                             type_map: List[str],
-                            traj_fmt: str,
                             input_template: dict,
+                            base_dir: str,
+                            limit: int = 0,
                             input_file_name: str = 'input.inp',
-                            ):
-        import dpdata
-        import numpy as np
+                            ) -> List[str]:
+        """Generate CP2K input files from LAMMPS dump files or XYZ files."""
+
+        # TODO: pymatgen has a better support for cp2k input, replace cp2k_input_tools with pymatgen in the future
+        # https://pymatgen.org/pymatgen.io.cp2k.inputs.html#pymatgen.io.cp2k.inputs.Cp2kInput
         from cp2k_input_tools import DEFAULT_CP2K_INPUT_XML
         from cp2k_input_tools.generator import CP2KInputGenerator
 
-        assert len(traj_files) == len(task_dirs), 'len(input_files) != len(task_dirs)'
+        import ase.io
+        from ase import Atoms
 
         cp2k_generator = CP2KInputGenerator(DEFAULT_CP2K_INPUT_XML)
+        task_dirs = []
+        atoms_list: List[Atoms] = []
 
-        for i in range(len(traj_files)):
-            traj_file = traj_files[i]
-            task_dir = task_dirs[i]
-
+        # read atoms
+        for dump_file in lammps_dump_files:
+            atoms_list += ase.io.read(dump_file, ':', format='lammps-dump-text', order=False, specorder=type_map)  # type: ignore
+        for xyz_file in xyz_files:
+            atoms_list += ase.io.read(xyz_file, ':', format='extxyz', order=False)  # type: ignore
+
+        if limit > 0:
+            atoms_list = atoms_list[:limit]
+
+        for i, atoms in enumerate(atoms_list):
+            # create task dir
+            task_dir = os.path.join(base_dir, f'{str(i).zfill(6)}')
             os.makedirs(task_dir, exist_ok=True)
-            input_data = copy.deepcopy(input_template)
-            system = dpdata.System(traj_file, fmt=traj_fmt, type_map=type_map)
-
-            # format coords
-            atom_names = np.array(system['atom_names'])  # type: ignore
-            atom_types = system['atom_types']  # type: ignore
-            coord_arr = system['coords'][0]  # type: ignore
-            kind_arr = atom_names[atom_types]  # type: ignore
-            coords = [ str(k) + ' ' + ' '.join(str(x) for x in c)  for k, c in zip(kind_arr, coord_arr) ] # type: ignore
-
-            # format cell
-            cell = system['cells'][0]
-            cell = np.reshape(cell, [3,3])
 
-            # override input_data
+            # create input file
+            input_data = copy.deepcopy(input_template)
+            coords, cell = ase_atoms_to_cp2k_input_data(atoms)
             merge_dict(input_data, {
                 'FORCE_EVAL': {
                     'SUBSYS': {
                         'COORD': {
                             '*': coords
                         },
                         'CELL': {
-                            'A': list(cell[0, :]),
-                            'B': list(cell[1, :]),
-                            'C': list(cell[2, :]),
+                            'A': cell[0],
+                            'B': cell[1],
+                            'C': cell[2],
                         }
                     }
                 }
             })
             input_text = '\n'.join(cp2k_generator.line_iter(input_data))
             with open(os.path.join(task_dir, input_file_name), 'w') as f:
                 f.write(input_text)
+            task_dirs.append(task_dir)
+        return task_dirs
 
     return make_cp2k_task_dirs
 make_cp2k_task_dirs = __make_cp2k_task_dirs()
-
-
-def __cp2k_output_to_dp_data():
-    """cloudpickle compatible: https://stackoverflow.com/questions/75292769"""
-    def cp2k_output_to_dp_data(task_dirs: List[str], output_dir: str, type_map: List[str]):
-        import dpdata
-        system = None
-        for task_dir in task_dirs:
-            _system = dpdata.LabeledSystem(os.path.join(task_dir, 'output'), fmt='cp2k/output', type_map=type_map)
-            if system is None:
-                system = _system
-            else:
-                system.append(_system)
-        assert system, 'system should not be None, check if task_dirs is empty'
-        system.to_deepmd_raw(output_dir)  # type: ignore
-        system.to_deepmd_npy(output_dir, set_size = len(system))  # type: ignore
-
-    return cp2k_output_to_dp_data
-cp2k_output_to_dp_data = __cp2k_output_to_dp_data()
```

### Comparing `ai2_kit-0.1.0/ai2_kit/workflow/cll_mlp.py` & `ai2_kit-0.2.0/ai2_kit/workflow/cll_mlp.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,72 +1,84 @@
-from ai2_kit.core.executor import BaseExecutorConfig, ExecutorManager
+from ai2_kit.core.executor import BaseExecutorConfig
 from ai2_kit.core.artifact import ArtifactMap
 from ai2_kit.core.log import get_logger
-from ai2_kit.core.util import load_yaml_files
-from ai2_kit.domain import deepmd
-from ai2_kit.domain import lammps
-from ai2_kit.domain import selector
-from ai2_kit.domain import cp2k
-from ai2_kit.domain import constant as const
+from ai2_kit.core.util import load_yaml_files, merge_dict
+from ai2_kit.core.resource_manager import ResourceManager
+from ai2_kit.domain import (
+    deepmd,
+    lammps,
+    selector,
+    cp2k,
+    constant as const,
+    updater,
+    cll,
+)
 
 from pydantic import BaseModel
-from typing import Dict, List, Optional
+from typing import Dict, List, Optional, Any
 from fire import Fire
 
+import itertools
+import copy
 import os
 
 logger = get_logger(__name__)
 
 
 class CllWorkflowExecutorConfig(BaseExecutorConfig):
     class Context(BaseModel):
         class Train(BaseModel):
-            deepmd: deepmd.GeneralDeepmdContextConfig
+            deepmd: deepmd.GenericDeepmdContextConfig
 
         class Explore(BaseModel):
-            lammps: lammps.GeneralLammpsContextConfig
+            lammps: lammps.GenericLammpsContextConfig
 
         class Label(BaseModel):
-            cp2k: cp2k.GeneralCp2kContextConfig
+            cp2k: cp2k.GenericCp2kContextConfig
 
         train: Train
         explore: Explore
         label: Label
 
     context: Context
 
 
-class CllWorkflowConfig(BaseModel):
-    class Workflow(BaseModel):
-        class General(BaseModel):
-            type_map: List[str]
-            mass_map: List[float]
-            max_iters: int = 10
-
-        class Train(BaseModel):
-            deepmd: deepmd.GeneralDeepmdInputConfig
-
-        class Explore(BaseModel):
-            lammps: lammps.GeneralLammpsInputConfig
-
-        class Select(BaseModel):
-            threshold: selector.GeneralThresholdInputConfig
+class WorkflowConfig(BaseModel):
+    class General(BaseModel):
+        type_map: List[str]
+        mass_map: List[float]
+        max_iters: int = 10
+
+    class Label(BaseModel):
+        cp2k: cp2k.GenericCp2kInputConfig
+
+    class Train(BaseModel):
+        deepmd: deepmd.GenericDeepmdInputConfig
+
+    class Explore(BaseModel):
+        lammps: lammps.GenericLammpsInputConfig
+
+    class Select(BaseModel):
+        by_threshold: selector.ThresholdSelectorInputConfig
+
+    class Update(BaseModel):
+        walkthrough: updater.WalkthroughUpdaterInputConfig
+
+    general: General
+    train: Train
+    explore: Explore
+    select: Select
+    label: Label
+    update: Update
 
-        class Label(BaseModel):
-            cp2k: cp2k.GeneralCp2kInputConfig
-
-        general: General
-        train: Train
-        explore: Explore
-        select: Select
-        label: Label
+class CllWorkflowConfig(BaseModel):
 
     executors: Dict[str, CllWorkflowExecutorConfig]
     artifacts: ArtifactMap
-    workflow: Workflow
+    workflow: Any  # Keep it raw here, it should be parsed later in iteration
 
 
 def cll_train_mlp(*config_files, executor: Optional[str] = None, path_prefix: Optional[str] = None):
     """
     Run Closed-Loop Learning (CLL) workflow to train Machine Learning Potential (MLP) models.
     """
 
@@ -74,102 +86,132 @@
     config = CllWorkflowConfig.parse_obj(config_data)
 
     if executor not in config.executors:
         raise ValueError(f'executor {executor} is not found')
     if path_prefix is None:
         raise ValueError('path_prefix should not be empty')
 
-    executor_manager = ExecutorManager(config.executors)  # type: ignore
-    default_executor = executor_manager.get_executor(executor)
+    resource_manager = ResourceManager(
+        executor_configs=config.executors,
+        artifacts=config.artifacts,
+        default_executor=executor,
+    )
 
-    context_cfg = config.executors[executor].context
+    context_config = config.executors[executor].context
+    raw_workflow_config = copy.deepcopy(config.workflow)
 
-    type_map = config.workflow.general.type_map
-    mass_map = config.workflow.general.mass_map
+    # output of each step
+    label_output: Optional[cll.ICllLabelOutput] = None
+    selector_output: Optional[cll.ICllSelectorOutput] = None
+    train_output: Optional[cll.ICllTrainOutput] = None
+    explore_output: Optional[cll.ICllExploreOutput] = None
 
-    # Init Setting
-    deepmd_input = deepmd.GeneralDeepmdInput(
-        config=config.workflow.train.deepmd,
-        type_map=type_map,
-        old_data=[],
-        new_data=[config.artifacts[key] for key in config.workflow.train.deepmd.init_data],
-    )
-    deepmd_context = deepmd.GeneralDeepmdContext(
-        path_prefix='',
-        executor=default_executor,
-        config=context_cfg.train.deepmd,
-    )
+
+    # cursor of update table
+    update_cursor = 0
 
     # Start iteration
-    for i in range(config.workflow.general.max_iters):
-        # update path prefix for each iteration
+    for i in itertools.count(0):
+
+        # parse workflow config
+        workflow_config = WorkflowConfig.parse_obj(raw_workflow_config)
+        if i >= workflow_config.general.max_iters:
+            logger.info(f'Iteration {i} exceeds max_iters, stop iteration.')
+            break
+
+        # shortcut for type_map and mass_map
+        type_map = workflow_config.general.type_map
+        mass_map = workflow_config.general.mass_map
+
+        # decide path prefix for each iteration
         iter_path_prefix = os.path.join(path_prefix, f'iters-{str(i).zfill(3)}')
 
-        # TODO: change order to: label -> train -> explore -> select
-        # TODO: support more tools
-        # TODO: support more options
+        # label
+        if workflow_config.label.cp2k:
+            cp2k_input = cp2k.GenericCp2kInput(
+                config=workflow_config.label.cp2k,
+                type_map=type_map,
+                system_files=[] if selector_output is None else selector_output.get_model_devi_dataset(),
+                initiated= i > 0,
+            )
+            cpk2_context = cp2k.GenericCp2kContext(
+                config=context_config.label.cp2k,
+                path_prefix=os.path.join(iter_path_prefix, 'label-cp2k'),
+                resource_manager=resource_manager,
+            )
+            label_output = cp2k.generic_cp2k(cp2k_input, cpk2_context).result()
+        else:
+            raise ValueError('No label method is specified')
 
         # train
-        deepmd_context.path_prefix = os.path.join(iter_path_prefix, 'train-deepmd')
-        deepmd_output = deepmd.general_deepmd(deepmd_input, deepmd_context).result()
+        if workflow_config.train.deepmd:
+            deepmd_input = deepmd.GenericDeepmdInput(
+                config=workflow_config.train.deepmd,
+                type_map=type_map,
+                old_dataset=[] if train_output is None else train_output.get_training_dataset(),
+                new_dataset=label_output.get_labeled_system_dataset(),
+                initiated= i > 0,
+            )
+            deepmd_context = deepmd.GenericDeepmdContext(
+                path_prefix=os.path.join(iter_path_prefix, 'train-deepmd'),
+                config=context_config.train.deepmd,
+                resource_manager=resource_manager,
+            )
+            train_output = deepmd.generic_deepmd(deepmd_input, deepmd_context).result()
+        else:
+            raise ValueError('No train method is specified')
 
         # explore
-        models = [a.output_dir.join(a.output_dir.attrs['frozen_model']) for a in deepmd_output.results]
-        lammps_iters = config.workflow.explore.lammps.iters
-        md_vars = lammps_iters[ i if i < len(lammps_iters) else (len(lammps_iters) - 1) ]
-
-        lammps_input = lammps.GeneralLammpsInput(
-            config=config.workflow.explore.lammps,
-            type_map=type_map,
-            mass_map=mass_map,
-            md_vars=md_vars,
-            system_vars=[config.artifacts[key] for key in md_vars.system_vars],
-            md_options=lammps.GeneralLammpsInput.MdOptions(models=models)
-        )
-        lammps_context = lammps.GeneralLammpsContext(
-            config=context_cfg.explore.lammps,
-            path_prefix=os.path.join(iter_path_prefix, 'explore-lammps'),
-            executor=default_executor,
-        )
-        lammps_output = lammps.general_lammps(lammps_input, lammps_context).result()
+        if workflow_config.explore.lammps:
+            md_options = lammps.GenericLammpsInput.MdOptions(
+                models=train_output.get_mlp_models(),
+            )
+            lammps_input = lammps.GenericLammpsInput(
+                config=workflow_config.explore.lammps,
+                type_map=type_map,
+                mass_map=mass_map,
+                md_options=md_options,
+            )
+            lammps_context = lammps.GenericLammpsContext(
+                path_prefix=os.path.join(iter_path_prefix, 'explore-lammps'),
+                config=context_config.explore.lammps,
+                resource_manager=resource_manager,
+            )
+            explore_output = lammps.generic_lammps(lammps_input, lammps_context).result()
+        else:
+            raise ValueError('No explore method is specified')
 
         # select
-        selector_input = selector.LammpsGeneralThresholdInput(
-            config=config.workflow.select.threshold,
-            candidates=lammps_output.candidates,
-            model_devi_out_file=const.MODEL_DEVI_OUT,
-        )
-        selector_context = selector.GeneralThresholdContext(
-            executor=default_executor,
-        )
-        selector_output = selector.lammps_general_threshold(selector_input, selector_context).result()
-
-        # label
-        cp2k_input = cp2k.GeneralCp2kInput(
-            config=config.workflow.label.cp2k,
-            type_map=config.workflow.general.type_map,
-            candidates=selector_output.candidates,
-            basic_set_file=config.artifacts.get(config.workflow.label.cp2k.basic_set_file or ''),
-            potential_file=config.artifacts.get(config.workflow.label.cp2k.potential_file or ''),
-        )
-        cp2k_context = cp2k.GeneralCp2kContext(
-            config=context_cfg.label.cp2k,
-            path_prefix=os.path.join(iter_path_prefix, 'label-cp2k'),
-            executor=default_executor,
-        )
-        cp2k_output = cp2k.general_cp2k(cp2k_input, cp2k_context).result()
-
-        # update input for the next round
-        deepmd_input.old_data.extend(deepmd_input.new_data)
-        deepmd_input.new_data = cp2k_output.dp_data_sets
-
-        # deepmd_input, lammps_input, selector_input, cp2k_input = smart_update(
-        #     i,
-        #     deepmd_output, lammps_output, selector_output, cp2k_output,
-        #     deepmd_input, lammps_input, selector_input, cp2k_input,
-        # )
-
+        if workflow_config.select.by_threshold:
+            selector_input = selector.ThresholdSelectorInput(
+                config=workflow_config.select.by_threshold,
+                model_devi_data=explore_output.get_model_devi_dataset(),
+                model_devi_out_filename=const.MODEL_DEVI_OUT,
+            )
+            selector_context = selector.ThresholdSelectorContext(
+                path_prefix=os.path.join(iter_path_prefix, 'selector-threshold'),
+                resource_manager=resource_manager,
+            )
+            selector_output = selector.threshold_selector(selector_input, selector_context).result()
+        else:
+            raise ValueError('No select method is specified')
+
+        # Update
+        update_config = workflow_config.update.walkthrough
+
+        # nothing to update because the table is empty
+        if not update_config.table:
+            continue
+        # keep using the latest config when it reach the end of table
+        if update_cursor >= len(update_config.table):
+            continue
+
+        # move cursor to next row if passing rate pass threshold
+        if selector_output.get_passing_rate() > update_config.passing_rate_threshold:
+            raw_workflow_config = merge_dict(copy.deepcopy(
+                config.workflow), update_config.table[update_cursor])
+            update_cursor += 1
 
 
 if __name__ == '__main__':
-    # for test, e.g:
+    # use python-fire to parse command line arguments
     Fire(cll_train_mlp)
```

### Comparing `ai2_kit-0.1.0/ai2_kit/workflow/fep.py` & `ai2_kit-0.2.0/ai2_kit/workflow/ec_fep.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,37 +16,37 @@
 
 logger = get_logger(__name__)
 
 
 class FepExecutorConfig(BaseExecutorConfig):
     class Context(BaseModel):
 
-        deepmd: deepmd.GeneralDeepmdContextConfig
-        lammps: lammps.GeneralLammpsContextConfig
-        cp2k: cp2k.GeneralCp2kContextConfig
+        deepmd: deepmd.GenericDeepmdContextConfig
+        lammps: lammps.GenericLammpsContextConfig
+        cp2k: cp2k.GenericCp2kContextConfig
 
     context: Context
 
 
 class FepConfig(BaseModel):
     class Workflow(BaseModel):
         class General(BaseModel):
             type_map: List[str]
             mass_map: List[float]
             max_iters: int = 10
 
         class Branch(BaseModel):
-            deepmd: deepmd.GeneralDeepmdInputConfig
-            cp2k: cp2k.GeneralCp2kInputConfig
-            threshold: selector.GeneralThresholdInputConfig
+            deepmd: deepmd.GenericDeepmdInputConfig
+            cp2k: cp2k.GenericCp2kInputConfig
+            threshold: selector.ThresholdSelectorInputConfig
 
         general: General
         neu: Branch
         red: Branch
-        lammps: lammps.GeneralLammpsInputConfig
+        lammps: lammps.GenericLammpsInputConfig
 
     executors: Dict[str, FepExecutorConfig]
     artifacts: ArtifactMap
     workflow: Workflow
 
 def fep_train_mlp(*config_files, executor: Optional[str] = None, path_prefix: Optional[str] = None):
     """
@@ -66,135 +66,135 @@
 
     context_cfg = config.executors[executor].context
 
     type_map = config.workflow.general.type_map
     mass_map = config.workflow.general.mass_map
 
     # Init Setting
-    neu_deepmd_input = deepmd.GeneralDeepmdInput(
+    neu_deepmd_input = deepmd.GenericDeepmdInput(
         config=config.workflow.neu.deepmd,
         type_map=type_map,
-        old_data=[],
-        new_data=[config.artifacts[key] for key in config.workflow.neu.deepmd.init_data],
+        old_dataset=[],
+        new_dataset=[config.artifacts[key] for key in config.workflow.neu.deepmd.init_dataset],
     )
-    neu_deepmd_context = deepmd.GeneralDeepmdContext(
+    neu_deepmd_context = deepmd.GenericDeepmdContext(
         path_prefix='',
         executor=default_executor,
         config=context_cfg.deepmd,
     )
 
-    red_deepmd_input = deepmd.GeneralDeepmdInput(
+    red_deepmd_input = deepmd.GenericDeepmdInput(
         config=config.workflow.red.deepmd,
         type_map=type_map,
-        old_data=[],
-        new_data=[config.artifacts[key] for key in config.workflow.red.deepmd.init_data],
+        old_dataset=[],
+        new_dataset=[config.artifacts[key] for key in config.workflow.red.deepmd.init_dataset],
     )
-    red_deepmd_context = deepmd.GeneralDeepmdContext(
+    red_deepmd_context = deepmd.GenericDeepmdContext(
         path_prefix='',
         executor=default_executor,
         config=context_cfg.deepmd,
     )
 
     # Start iteration
     for i in range(config.workflow.general.max_iters):
         # update path prefix for each iteration
         iter_path_prefix = os.path.join(path_prefix, f'iters-{str(i).zfill(3)}')
 
         # train
         neu_deepmd_context.path_prefix = os.path.join(iter_path_prefix, 'train-neu-deepmd')
-        neu_deepmd_output_future = deepmd.general_deepmd(neu_deepmd_input, neu_deepmd_context)
+        neu_deepmd_output_future = deepmd.generic_deepmd(neu_deepmd_input, neu_deepmd_context)
 
         red_deepmd_context.path_prefix = os.path.join(iter_path_prefix, 'train-red-deepmd')
-        red_deepmd_output_future = deepmd.general_deepmd(red_deepmd_input, red_deepmd_context)
+        red_deepmd_output_future = deepmd.generic_deepmd(red_deepmd_input, red_deepmd_context)
 
         neu_deepmd_output, red_deepmd_output = neu_deepmd_output_future.result(), red_deepmd_output_future.result()
 
         # explore
         neu_models = [a.output_dir.join(a.output_dir.attrs['frozen_model']) for a in neu_deepmd_output.results]
         red_models = [a.output_dir.join(a.output_dir.attrs['frozen_model']) for a in red_deepmd_output.results]
 
         lammps_iters = config.workflow.lammps.iters
         md_vars = lammps_iters[i % len(lammps_iters)]
 
-        lammps_input = lammps.GeneralLammpsInput(
+        lammps_input = lammps.GenericLammpsInput(
             config=config.workflow.lammps,
             type_map=type_map,
             mass_map=mass_map,
             md_vars=md_vars,
             system_vars=[config.artifacts[key] for key in md_vars.system_vars],
-            fep_options=lammps.GeneralLammpsInput.FepOptions(red_models=red_models, neu_models=neu_models)
+            fep_options=lammps.GenericLammpsInput.FepOptions(red_models=red_models, neu_models=neu_models)
         )
-        lammps_context = lammps.GeneralLammpsContext(
+        lammps_context = lammps.GenericLammpsContext(
             config=context_cfg.lammps,
             path_prefix=os.path.join(iter_path_prefix, 'explore-lammps'),
             executor=default_executor,
         )
-        lammps_output = lammps.general_lammps(lammps_input, lammps_context).result()
+        lammps_output = lammps.generic_lammps(lammps_input, lammps_context).result()
 
         # select
-        neu_selector_input = selector.LammpsGeneralThresholdInput(
+        neu_selector_input = selector.ThresholdSelectorInput(
             config=config.workflow.neu.threshold,
-            candidates=lammps_output.candidates,
-            model_devi_out_file=const.MODEL_DEVI_NEU_OUT,
+            model_devi_data=lammps_output.systems,
+            model_devi_out_filename=const.MODEL_DEVI_NEU_OUT,
         )
-        neu_selector_context = selector.GeneralThresholdContext(
+        neu_selector_context = selector.ThresholdSelectorContext(
             executor=default_executor,
         )
 
-        red_selector_input = selector.LammpsGeneralThresholdInput(
+        red_selector_input = selector.ThresholdSelectorInput(
             config=config.workflow.red.threshold,
-            candidates=lammps_output.candidates,
-            model_devi_out_file=const.MODEL_DEVI_RED_OUT,
+            model_devi_data=lammps_output.systems,
+            model_devi_out_filename=const.MODEL_DEVI_RED_OUT,
         )
-        red_selector_context = selector.GeneralThresholdContext(
+        red_selector_context = selector.ThresholdSelectorContext(
             executor=default_executor,
         )
 
-        neu_selector_output_future = selector.lammps_general_threshold(neu_selector_input, neu_selector_context)
-        red_selector_output_future = selector.lammps_general_threshold(red_selector_input, red_selector_context)
+        neu_selector_output_future = selector.threshold_selector(neu_selector_input, neu_selector_context)
+        red_selector_output_future = selector.threshold_selector(red_selector_input, red_selector_context)
 
         neu_selector_output, red_selector_output = neu_selector_output_future.result(), red_selector_output_future.result()
 
         # label
-        neu_cp2k_input = cp2k.GeneralCp2kInput(
+        neu_cp2k_input = cp2k.GenericCp2kInput(
             config=config.workflow.neu.cp2k,
             type_map=config.workflow.general.type_map,
-            candidates=neu_selector_output.candidates,
+            system_files=neu_selector_output.model_devi_data,
             basic_set_file=config.artifacts.get(config.workflow.neu.cp2k.basic_set_file or ''),
             potential_file=config.artifacts.get(config.workflow.neu.cp2k.potential_file or ''),
         )
-        neu_cp2k_context = cp2k.GeneralCp2kContext(
+        neu_cp2k_context = cp2k.GenericCp2kContext(
             config=context_cfg.cp2k,
             path_prefix=os.path.join(iter_path_prefix, 'label-neu-cp2k'),
             executor=default_executor,
         )
 
-        red_cp2k_input = cp2k.GeneralCp2kInput(
+        red_cp2k_input = cp2k.GenericCp2kInput(
             config=config.workflow.red.cp2k,
             type_map=config.workflow.general.type_map,
-            candidates=red_selector_output.candidates,
+            system_files=red_selector_output.model_devi_data,
             basic_set_file=config.artifacts.get(config.workflow.red.cp2k.basic_set_file or ''),
             potential_file=config.artifacts.get(config.workflow.red.cp2k.potential_file or ''),
         )
-        red_cp2k_context = cp2k.GeneralCp2kContext(
+        red_cp2k_context = cp2k.GenericCp2kContext(
             config=context_cfg.cp2k,
             path_prefix=os.path.join(iter_path_prefix, 'label-red-cp2k'),
             executor=default_executor,
         )
 
-        neu_cp2k_output_future = cp2k.general_cp2k(neu_cp2k_input, neu_cp2k_context)
-        red_cp2k_output_future = cp2k.general_cp2k(red_cp2k_input, red_cp2k_context)
+        neu_cp2k_output_future = cp2k.generic_cp2k(neu_cp2k_input, neu_cp2k_context)
+        red_cp2k_output_future = cp2k.generic_cp2k(red_cp2k_input, red_cp2k_context)
 
         neu_cp2k_output, red_cp2k_output = neu_cp2k_output_future.result(), red_cp2k_output_future.result()
 
         # update input for the next round
-        neu_deepmd_input.old_data.extend(neu_deepmd_input.new_data)
-        neu_deepmd_input.new_data = neu_cp2k_output.dp_data_sets
+        neu_deepmd_input.old_dataset.extend(neu_deepmd_input.new_dataset)
+        neu_deepmd_input.new_dataset = neu_cp2k_output.dp_data_sets
 
-        red_deepmd_input.old_data.extend(red_deepmd_input.new_data)
-        red_deepmd_input.new_data = red_cp2k_output.dp_data_sets
+        red_deepmd_input.old_dataset.extend(red_deepmd_input.new_dataset)
+        red_deepmd_input.new_dataset = red_cp2k_output.dp_data_sets
 
 
 if __name__ == '__main__':
     # for test, e.g:
     # python -m ai2_kit.workflow.fep fep_config.yaml --executor=hpc01 --path-prefix=fep-test
     Fire(fep_train_mlp)
```

### Comparing `ai2_kit-0.1.0/pyproject.toml` & `ai2_kit-0.2.0/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai2-kit"
-version = "0.1.0"
+version = "0.2.0"
 description = ""
 authors = ["weihong.xu <xuweihong.cn@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ai2_kit"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
@@ -14,27 +14,29 @@
 invoke = "^1.7.3"
 ruamel-yaml = "^0.17.21"
 cloudpickle = "^2.2.0"
 shortuuid = "^1.0.11"
 dpdata = "^0.2.13"
 pandas = "^1.5.3"
 cp2k-input-tools = "^0.8.2"
+ase = "^3.22.1"
+pymatgen = "^2023.2.22"
+mdanalysis = "^2.4.3"
 
 
 [[tool.poetry.source]]
 name = "ustc"
 url = "https://pypi.mirrors.ustc.edu.cn/simple/"
 default = true
 secondary = false
 
 
 [tool.poetry.group.dev.dependencies]
 autopep8 = "^2.0.0"
 pytest = "^7.2.0"
-pylint = "^2.15.10"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry.scripts]
 ai2-kit= "ai2_kit.main:main"
```

