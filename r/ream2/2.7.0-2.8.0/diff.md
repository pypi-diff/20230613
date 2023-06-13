# Comparing `tmp/ream2-2.7.0.tar.gz` & `tmp/ream2-2.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ream2-2.7.0.tar", max compression
+gzip compressed data, was "ream2-2.8.0.tar", max compression
```

## Comparing `ream2-2.7.0.tar` & `ream2-2.8.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1064 2023-06-11 20:53:06.663041 ream2-2.7.0/LICENSE
--rw-r--r--   0        0        0     5267 2023-06-11 20:53:06.663041 ream2-2.7.0/README.md
--rw-r--r--   0        0        0      763 2023-06-11 20:53:06.663041 ream2-2.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/__init__.py
--rw-r--r--   0        0        0    14886 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actor_graph.py
--rw-r--r--   0        0        0     2197 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actor_state.py
--rw-r--r--   0        0        0     2040 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actor_version.py
--rw-r--r--   0        0        0        0 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actors/__init__.py
--rw-r--r--   0        0        0     3815 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actors/base.py
--rw-r--r--   0        0        0     1155 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actors/dsid.py
--rw-r--r--   0        0        0      976 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actors/enum.py
--rw-r--r--   0        0        0      363 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/actors/interface.py
--rw-r--r--   0        0        0    37569 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/cache_helper.py
--rw-r--r--   0        0        0     3393 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/cli_helper.py
--rw-r--r--   0        0        0    34210 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/data_model_helper.py
--rw-r--r--   0        0        0    14434 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/dataset_helper.py
--rw-r--r--   0        0        0     9838 2023-06-11 20:53:06.663041 ream2-2.7.0/ream/fs.py
--rw-r--r--   0        0        0     6636 2023-06-11 20:53:06.667041 ream2-2.7.0/ream/helper.py
--rw-r--r--   0        0        0     5684 2023-06-11 20:53:06.667041 ream2-2.7.0/ream/params_helper.py
--rw-r--r--   0        0        0     1090 2023-06-11 20:53:06.667041 ream2-2.7.0/ream/prelude.py
--rw-r--r--   0        0        0     2248 2023-06-11 20:53:06.667041 ream2-2.7.0/ream/workspace.py
--rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.7.0/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-06-13 06:02:33.452605 ream2-2.8.0/LICENSE
+-rw-r--r--   0        0        0     5267 2023-06-13 06:02:33.452605 ream2-2.8.0/README.md
+-rw-r--r--   0        0        0      763 2023-06-13 06:02:33.452605 ream2-2.8.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/__init__.py
+-rw-r--r--   0        0        0    14886 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actor_graph.py
+-rw-r--r--   0        0        0     2197 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actor_state.py
+-rw-r--r--   0        0        0     2040 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actor_version.py
+-rw-r--r--   0        0        0        0 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actors/__init__.py
+-rw-r--r--   0        0        0     4115 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actors/base.py
+-rw-r--r--   0        0        0     1155 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actors/dsid.py
+-rw-r--r--   0        0        0     1332 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actors/enum.py
+-rw-r--r--   0        0        0      363 2023-06-13 06:02:33.452605 ream2-2.8.0/ream/actors/interface.py
+-rw-r--r--   0        0        0    37569 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/cache_helper.py
+-rw-r--r--   0        0        0     3393 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/cli_helper.py
+-rw-r--r--   0        0        0    34210 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/data_model_helper.py
+-rw-r--r--   0        0        0    14434 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/dataset_helper.py
+-rw-r--r--   0        0        0     9838 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/fs.py
+-rw-r--r--   0        0        0     6636 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/helper.py
+-rw-r--r--   0        0        0     5684 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/params_helper.py
+-rw-r--r--   0        0        0     1090 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/prelude.py
+-rw-r--r--   0        0        0     2248 2023-06-13 06:02:33.456605 ream2-2.8.0/ream/workspace.py
+-rw-r--r--   0        0        0     6352 1970-01-01 00:00:00.000000 ream2-2.8.0/PKG-INFO
```

### Comparing `ream2-2.7.0/LICENSE` & `ream2-2.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/README.md` & `ream2-2.8.0/README.md`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/pyproject.toml` & `ream2-2.8.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ream2"
-version = "2.7.0"
+version = "2.8.0"
 description = "An actor architecture for research software"
 authors = ["Binh Vu <binh@toan2.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/binh-vu/ream"
 repository = "https://github.com/binh-vu/ream"
 packages = [
```

### Comparing `ream2-2.7.0/ream/actor_graph.py` & `ream2-2.8.0/ream/actor_graph.py`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/ream/actor_state.py` & `ream2-2.8.0/ream/actor_state.py`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/ream/actor_version.py` & `ream2-2.8.0/ream/actor_version.py`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/ream/actors/base.py` & `ream2-2.8.0/ream/actors/base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,40 @@
 from __future__ import annotations
-from dataclasses import is_dataclass
+
 import os
-from typing import (
-    Optional,
-    List,
-    Type,
-    TypeVar,
-    Generic,
-)
+from dataclasses import is_dataclass
+from typing import TYPE_CHECKING, Generic, List, Optional, Protocol, Type, TypeVar
+
+from loguru import logger
+
 from ream.actor_state import ActorState
+from ream.actors.interface import Actor
+from ream.fs import FS
 from ream.helper import resolve_type_arguments
 from ream.params_helper import EnumParams
-from ream.fs import FS
 from ream.workspace import ReamWorkspace
-from loguru import logger
-from ream.actors.interface import Actor
 
-P = TypeVar("P")
+if TYPE_CHECKING:
+    from loguru import Logger
+
+P = TypeVar("P", covariant=True)
+
+
+class BaseActorProtocol(Protocol[P]):
+    @property
+    def params(self) -> P:
+        ...
+
+    @property
+    def logger(self) -> Logger:
+        ...
+
+    @property
+    def dep_actors(self) -> list[BaseActorProtocol]:
+        ...
 
 
 class BaseActor(Actor, Generic[P]):
     """A based for parameterized actor that its output is always determisitic given: the input, actor's state, and actor's provenance.
 
     The actor's provenance is an optional mechanism to provide additional guarantee to always have deterministic output if
     the combination of input and actor's state is not sufficient. For example, training a model with a random seed and the store the model
```

### Comparing `ream2-2.7.0/ream/actors/dsid.py` & `ream2-2.8.0/ream/actors/dsid.py`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/ream/actors/enum.py` & `ream2-2.8.0/ream/actors/enum.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,27 +1,46 @@
 from __future__ import annotations
-from typing import Generic, TypeVar
+
+from abc import ABC, abstractmethod
+from typing import Generic, List, Optional, TypeVar, cast
+
 from ream.actor_state import ActorState
 from ream.actors.base import BaseActor, P
 from ream.params_helper import EnumParams
 
+
+class EnumInterface(ABC):
+    @abstractmethod
+    def exec(self, *args, **kwargs):
+        pass
+
+    def get_provenance(self) -> str:
+        return ""
+
+
 EP = TypeVar("EP", bound=EnumParams)
+EI = TypeVar("EI", bound=EnumInterface)  # enum interface
 
 
-class EnumActor(BaseActor[EP]):
-    def get_actor_state(self) -> ActorState:
-        deps = [actor.get_actor_state() for actor in self.dep_actors]
+class EnumActor(Generic[EP, EI], BaseActor[EP]):
+    def __init__(self, params: EP, dep_actors: Optional[List[BaseActor]] = None):
+        super().__init__(params, dep_actors)
 
+        # extract the method
         enum_fields = self.params.get_method_fields()
-        if not len(enum_fields) != 1:
+        if len(enum_fields) != 1:
             raise ValueError(
                 f"EnumActor must have exactly one method field, got {len(enum_fields)}"
             )
 
         enum_field = enum_fields[0]
         cls = self.params.get_method_class(enum_field)
         params = self.params.get_method_params(enum_field)
-        if params is None:
-            raise ValueError(
-                f"Parameter for an enum variant {cls} must be provided, got None"
-            )
-        return ActorState.create(cls, params, dependencies=deps)
+
+        # construct the selected method
+        self.method = cast(EI, cls(params))
+
+    def get_provenance(self):
+        return self.method.get_provenance()
+
+    def exec(self, *args, **kwargs):
+        return self.method.exec(*args, **kwargs)
```

### Comparing `ream2-2.7.0/ream/cache_helper.py` & `ream2-2.8.0/ream/cache_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/ream/cli_helper.py` & `ream2-2.8.0/ream/cli_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/ream/data_model_helper.py` & `ream2-2.8.0/ream/data_model_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/ream/dataset_helper.py` & `ream2-2.8.0/ream/dataset_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/ream/fs.py` & `ream2-2.8.0/ream/fs.py`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/ream/helper.py` & `ream2-2.8.0/ream/helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/ream/params_helper.py` & `ream2-2.8.0/ream/params_helper.py`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/ream/prelude.py` & `ream2-2.8.0/ream/prelude.py`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/ream/workspace.py` & `ream2-2.8.0/ream/workspace.py`

 * *Files identical despite different names*

### Comparing `ream2-2.7.0/PKG-INFO` & `ream2-2.8.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ream2
-Version: 2.7.0
+Version: 2.8.0
 Summary: An actor architecture for research software
 Home-page: https://github.com/binh-vu/ream
 License: MIT
 Author: Binh Vu
 Author-email: binh@toan2.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

