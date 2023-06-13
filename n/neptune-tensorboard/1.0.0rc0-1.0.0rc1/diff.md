# Comparing `tmp/neptune_tensorboard-1.0.0rc0.tar.gz` & `tmp/neptune_tensorboard-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neptune_tensorboard-1.0.0rc0.tar", max compression
+gzip compressed data, was "neptune_tensorboard-1.0.0rc1.tar", max compression
```

## Comparing `neptune_tensorboard-1.0.0rc0.tar` & `neptune_tensorboard-1.0.0rc1.tar`

### file list

```diff
@@ -1,9 +1,11 @@
--rw-r--r--   0        0        0      416 2023-05-24 14:17:24.834326 neptune_tensorboard-1.0.0rc0/CHANGELOG.md
--rw-r--r--   0        0        0    11357 2023-05-24 14:17:24.834326 neptune_tensorboard-1.0.0rc0/LICENSE
--rw-r--r--   0        0        0     3420 2023-05-24 14:17:24.834326 neptune_tensorboard-1.0.0rc0/README.md
--rw-r--r--   0        0        0     2639 2023-05-24 14:17:38.422524 neptune_tensorboard-1.0.0rc0/pyproject.toml
--rw-r--r--   0        0        0      750 2023-05-24 14:17:24.834326 neptune_tensorboard-1.0.0rc0/src/neptune_tensorboard/__init__.py
--rw-r--r--   0        0        0     1960 2023-05-24 14:17:24.834326 neptune_tensorboard-1.0.0rc0/src/neptune_tensorboard/integration/__init__.py
--rw-r--r--   0        0        0     3232 2023-05-24 14:17:24.834326 neptune_tensorboard-1.0.0rc0/src/neptune_tensorboard/integration/tensorflow_integration.py
--rw-r--r--   0        0        0      742 2023-05-24 14:17:24.834326 neptune_tensorboard-1.0.0rc0/src/neptune_tensorboard/integration/version.py
--rw-r--r--   0        0        0     5399 1970-01-01 00:00:00.000000 neptune_tensorboard-1.0.0rc0/PKG-INFO
+-rw-r--r--   0        0        0      589 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/CHANGELOG.md
+-rw-r--r--   0        0        0    11357 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     3420 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/README.md
+-rw-r--r--   0        0        0     2736 2023-06-13 10:38:12.895124 neptune_tensorboard-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0      820 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/__init__.py
+-rw-r--r--   0        0        0     3557 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/__init__.py
+-rw-r--r--   0        0        0     5605 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/pytorch_integration.py
+-rw-r--r--   0        0        0     3563 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/tensorflow_integration.py
+-rw-r--r--   0        0        0      292 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/utils.py
+-rw-r--r--   0        0        0      742 2023-06-13 10:37:59.850755 neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/version.py
+-rw-r--r--   0        0        0     5456 1970-01-01 00:00:00.000000 neptune_tensorboard-1.0.0rc1/PKG-INFO
```

### Comparing `neptune_tensorboard-1.0.0rc0/LICENSE` & `neptune_tensorboard-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `neptune_tensorboard-1.0.0rc0/README.md` & `neptune_tensorboard-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `neptune_tensorboard-1.0.0rc0/pyproject.toml` & `neptune_tensorboard-1.0.0rc1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -10,21 +10,23 @@
 
 [tool.poetry.dependencies]
 python = "^3.7"
 
 # Python lack of functionalities from future versions
 importlib-metadata = { version = "*", python = "<3.8" }
 tensorflow = { version = ">=2.0.0", optional = true }
+torch = { version = ">=1.9.0", optional = true }
 
 # dev
 pre-commit = { version = "*", optional = true }
 pytest = { version = ">=5.0", optional = true }
 pytest-cov = { version = "2.10.1", optional = true }
 pytest-xdist = { version = "*", optional = true }
 pydot = { version = "*", optional = true }
+matplotlib = { version = "*", optional = true }
 neptune = { version = ">=1.0.1", optional = true }
 
 [tool.poetry.extras]
 dev = [
     "pre-commit",
     "pytest",
     "pytest-cov",
@@ -38,15 +40,15 @@
 repository = "https://github.com/neptune-ai/neptune-tensorboard"
 homepage = "https://neptune.ai/"
 documentation = "https://docs.neptune.ai/integrations-and-supported-tools/model-training/tensorboard"
 include = ["CHANGELOG.md"]
 license = "Apache License 2.0"
 name = "neptune-tensorboard"
 readme = "README.md"
-version = "1.0.0-pre.0"
+version = "1.0.0-pre.1"
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Natural Language :: English",
```

### Comparing `neptune_tensorboard-1.0.0rc0/src/neptune_tensorboard/__init__.py` & `neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -9,13 +9,14 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__all__ = ["enable_tensorboard_logging", "__version__"]
+__all__ = ["enable_tensorboard_logging", "enable_tensorboard_logging_ctx", "__version__"]
 
 from neptune_tensorboard.integration import (
     __version__,
     enable_tensorboard_logging,
+    enable_tensorboard_logging_ctx,
 )
```

### Comparing `neptune_tensorboard-1.0.0rc0/src/neptune_tensorboard/integration/tensorflow_integration.py` & `neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/tensorflow_integration.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,35 +9,37 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
+import contextlib
 import warnings
-from functools import wraps
 from importlib.util import find_spec
 
 import tensorflow as tf
 from neptune.types import File
 
+from neptune_tensorboard.integration.utils import register_pre_hook
+
 IS_GRAPHLIB_AVAILABLE = find_spec("tfgraphviz")
 if IS_GRAPHLIB_AVAILABLE:
     import tfgraphviz as tfg
 
 _integrated_with_tensorflow = False
 
-__all__ = ["patch_tensorflow"]
+__all__ = ["patch_tensorflow", "NeptuneTensorflowTracker"]
 
 
 def patch_tensorflow(run, base_namespace):
     global _integrated_with_tensorflow
 
     if not _integrated_with_tensorflow:
-        patch_tensorflow_2x(run, base_namespace)
+        NeptuneTensorflowTracker(run, base_namespace)
         _integrated_with_tensorflow = True
 
 
 def track_scalar(name, data, step=None, description=None, run=None, base_namespace=None):
     run[base_namespace]["scalar"][name].append(data)
 
 
@@ -63,29 +65,32 @@
         png_bytes = graph.pipe(format="png")
         # There is only one graph
         run[base_namespace]["graph"].upload(File.from_content(png_bytes, extension="png"))
     else:
         warnings.warn("Skipping model visualization because no tfgraphviz installation was found.")
 
 
-def register_pre_hook(original, neptune_hook, run, base_namespace):
-    @wraps(original)
-    def wrapper(*args, **kwargs):
-        neptune_hook(*args, **kwargs, run=run, base_namespace=base_namespace)
-        return original(*args, **kwargs)
-
-    return wrapper
-
-
-def patch_tensorflow_2x(run, base_namespace):
-    tf.summary.scalar = register_pre_hook(
-        original=tf.summary.scalar, neptune_hook=track_scalar, run=run, base_namespace=base_namespace
-    )
-    tf.summary.image = register_pre_hook(
-        original=tf.summary.image, neptune_hook=track_image, run=run, base_namespace=base_namespace
-    )
-    tf.summary.text = register_pre_hook(
-        original=tf.summary.text, neptune_hook=track_text, run=run, base_namespace=base_namespace
-    )
-    tf.summary.graph = register_pre_hook(
-        original=tf.summary.graph, neptune_hook=track_graph, run=run, base_namespace=base_namespace
-    )
+class NeptuneTensorflowTracker(contextlib.AbstractContextManager):
+    def __init__(self, run, base_namespace):
+        self.org_scalar = tf.summary.scalar
+        self.org_image = tf.summary.image
+        self.org_text = tf.summary.text
+        self.org_graph = tf.summary.graph
+
+        tf.summary.scalar = register_pre_hook(
+            original=tf.summary.scalar, neptune_hook=track_scalar, run=run, base_namespace=base_namespace
+        )
+        tf.summary.image = register_pre_hook(
+            original=tf.summary.image, neptune_hook=track_image, run=run, base_namespace=base_namespace
+        )
+        tf.summary.text = register_pre_hook(
+            original=tf.summary.text, neptune_hook=track_text, run=run, base_namespace=base_namespace
+        )
+        tf.summary.graph = register_pre_hook(
+            original=tf.summary.graph, neptune_hook=track_graph, run=run, base_namespace=base_namespace
+        )
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        tf.summary.scalar = self.org_scalar
+        tf.summary.image = self.org_image
+        tf.summary.text = self.org_text
+        tf.summary.graph = self.org_graph
```

### Comparing `neptune_tensorboard-1.0.0rc0/src/neptune_tensorboard/integration/version.py` & `neptune_tensorboard-1.0.0rc1/src/neptune_tensorboard/integration/version.py`

 * *Files identical despite different names*

### Comparing `neptune_tensorboard-1.0.0rc0/PKG-INFO` & `neptune_tensorboard-1.0.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neptune-tensorboard
-Version: 1.0.0rc0
+Version: 1.0.0rc1
 Summary: Neptune.ai Tensorboard integration library
 Home-page: https://neptune.ai/
 License: Apache-2.0
 Keywords: MLOps,ML Experiment Tracking,ML Model Registry,ML Model Store,ML Metadata Store
 Author: neptune.ai
 Author-email: contact@neptune.ai
 Requires-Python: >=3.7,<4.0
@@ -25,21 +25,23 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: dev
 Requires-Dist: importlib-metadata ; python_version < "3.8"
+Requires-Dist: matplotlib
 Requires-Dist: neptune (>=1.0.1) ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: pydot ; extra == "dev"
 Requires-Dist: pytest (>=5.0) ; extra == "dev"
 Requires-Dist: pytest-cov (==2.10.1) ; extra == "dev"
 Requires-Dist: pytest-xdist
 Requires-Dist: tensorflow (>=2.0.0)
+Requires-Dist: torch (>=1.9.0)
 Project-URL: Documentation, https://docs.neptune.ai/integrations-and-supported-tools/model-training/tensorboard
 Project-URL: Repository, https://github.com/neptune-ai/neptune-tensorboard
 Project-URL: Tracker, https://github.com/neptune-ai/neptune-tensorboard/issues
 Description-Content-Type: text/markdown
 
 # neptune-tensorboard
```

