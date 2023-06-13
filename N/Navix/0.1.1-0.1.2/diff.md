# Comparing `tmp/Navix-0.1.1.tar.gz` & `tmp/Navix-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Navix-0.1.1.tar", last modified: Tue Jun 13 21:19:10 2023, max compression
+gzip compressed data, was "Navix-0.1.2.tar", last modified: Tue Jun 13 21:32:18 2023, max compression
```

## Comparing `Navix-0.1.1.tar` & `Navix-0.1.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.142311 Navix-0.1.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.138311 Navix-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.138311 Navix-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 21:18:58.000000 Navix-0.1.1/.github/workflows/CD.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-13 21:18:58.000000 Navix-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 21:18:58.000000 Navix-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 21:18:58.000000 Navix-0.1.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 21:18:58.000000 Navix-0.1.1/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-13 21:18:58.000000 Navix-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 21:18:58.000000 Navix-0.1.1/NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.138311 Navix-0.1.1/Navix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    18017 2023-06-13 21:19:10.000000 Navix-0.1.1/Navix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 21:19:10.000000 Navix-0.1.1/Navix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:19:10.000000 Navix-0.1.1/Navix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 21:19:10.000000 Navix-0.1.1/Navix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 21:19:10.000000 Navix-0.1.1/Navix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    18017 2023-06-13 21:19:10.142311 Navix-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-13 21:18:58.000000 Navix-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.138311 Navix-0.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-13 21:18:58.000000 Navix-0.1.1/docs/profiling.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.138311 Navix-0.1.1/navix/
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.142311 Navix-0.1.1/navix/environments/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/environments/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/environments/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/termination.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/transitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-13 21:18:58.000000 Navix-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 21:18:58.000000 Navix-0.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:19:10.142311 Navix-0.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.142311 Navix-0.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-13 21:18:58.000000 Navix-0.1.1/tests/test_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.872310 Navix-0.1.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.864310 Navix-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.868310 Navix-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 21:32:08.000000 Navix-0.1.2/.github/workflows/CD.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-13 21:32:08.000000 Navix-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 21:32:08.000000 Navix-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 21:32:08.000000 Navix-0.1.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 21:32:08.000000 Navix-0.1.2/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-13 21:32:08.000000 Navix-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 21:32:08.000000 Navix-0.1.2/NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.868310 Navix-0.1.2/Navix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17993 2023-06-13 21:32:18.000000 Navix-0.1.2/Navix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 21:32:18.000000 Navix-0.1.2/Navix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:32:18.000000 Navix-0.1.2/Navix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 21:32:18.000000 Navix-0.1.2/Navix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 21:32:18.000000 Navix-0.1.2/Navix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    17993 2023-06-13 21:32:18.872310 Navix-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2959 2023-06-13 21:32:08.000000 Navix-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.868310 Navix-0.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-13 21:32:08.000000 Navix-0.1.2/docs/profiling.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.872310 Navix-0.1.2/navix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.872310 Navix-0.1.2/navix/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/environments/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/environments/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/termination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 21:32:08.000000 Navix-0.1.2/navix/transitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-13 21:32:08.000000 Navix-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 21:32:08.000000 Navix-0.1.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:32:18.872310 Navix-0.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:32:18.872310 Navix-0.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-13 21:32:08.000000 Navix-0.1.2/tests/test_environment.py
```

### Comparing `Navix-0.1.1/.github/workflows/CD.yml` & `Navix-0.1.2/.github/workflows/CD.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/.github/workflows/CI.yml` & `Navix-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/.gitignore` & `Navix-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/COPYRIGHT` & `Navix-0.1.2/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/LICENSE` & `Navix-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/Navix.egg-info/PKG-INFO` & `Navix-0.1.2/Navix.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.1.1
-Summary: Gridworld navigation for Reinforcement Learning with JAX
+Version: 0.1.2
+Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -255,37 +255,36 @@
 
 ## What is NAVIX?
 NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **~2000x** faster with Autograd and XLA support.
 You can see a superficial performance comparison [here](docs/profiling.ipynb).
 
 
 ## Installation
-We currently support the OSs that are supported by JAX does.
-Please follow the [JAX installation guide](https://github.com/google/jax#installation) to install the correct version of JAX for your OS.
+We currently support the OSs supported by JAX.
+You can find a description [here](https://github.com/google/jax#installation).
 
-You might want to follow the same guide to use your faviourite accelerator
+You might want to follow the same guide to install jax for your faviourite accelerator
 (e.g. [CPU](https://github.com/google/jax#pip-installation-cpu),
 [GPU](https://github.com/google/jax#pip-installation-gpu-cuda-installed-locally-harder), or
 [TPU](https://github.com/google/jax#pip-installation-colab-tpu)
 ).
 
-Then, install `navix` with:
-
+Then, install `navix` and its dependencies with:
 ```bash
 pip install navix
 ```
 
 ---
 ## Examples
 
 ### XLA compilation
 One straightforward use case is to accelerate the computation of the environment with XLA compilation.
-For example, here we compile a full training run, and we vectorise the environment to run multiple environments in parallel.
+For example, here we vectorise the environment to run multiple environments in parallel, and compile **the full training run**.
 
-You can find a superficial performance comparison with [minigrid](https://github.com/Farama-Foundation/Minigrid) in the [docs](docs/profiling.ipynb).
+You can find a partial performance comparison with [minigrid](https://github.com/Farama-Foundation/Minigrid) in the [docs](docs/profiling.ipynb).
 
 ```python
 import jax
 import navix as nx
 
 
 def run(seed)
@@ -310,16 +309,16 @@
 TODO(epignatelli): add example.
 
 
 ## Cite
 If you use `helx` please consider citing it as:
 
 ```bibtex
-@misc{helx,
+@misc{pignatelli2023navix,
   author = {Pignatelli, Eduardo},
-  title = {Navix: Reinforcement Learning navigation with Autograd and XLA},
+  title = {Navix: Accelerated gridworld navigation with JAX},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/epignatelli/navix}}
   }
 ```
```

### Comparing `Navix-0.1.1/Navix.egg-info/SOURCES.txt` & `Navix-0.1.2/Navix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/PKG-INFO` & `Navix-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.1.1
-Summary: Gridworld navigation for Reinforcement Learning with JAX
+Version: 0.1.2
+Summary: Accelerated gridworld navigation with JAX for deep reinforcement learning
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -255,37 +255,36 @@
 
 ## What is NAVIX?
 NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **~2000x** faster with Autograd and XLA support.
 You can see a superficial performance comparison [here](docs/profiling.ipynb).
 
 
 ## Installation
-We currently support the OSs that are supported by JAX does.
-Please follow the [JAX installation guide](https://github.com/google/jax#installation) to install the correct version of JAX for your OS.
+We currently support the OSs supported by JAX.
+You can find a description [here](https://github.com/google/jax#installation).
 
-You might want to follow the same guide to use your faviourite accelerator
+You might want to follow the same guide to install jax for your faviourite accelerator
 (e.g. [CPU](https://github.com/google/jax#pip-installation-cpu),
 [GPU](https://github.com/google/jax#pip-installation-gpu-cuda-installed-locally-harder), or
 [TPU](https://github.com/google/jax#pip-installation-colab-tpu)
 ).
 
-Then, install `navix` with:
-
+Then, install `navix` and its dependencies with:
 ```bash
 pip install navix
 ```
 
 ---
 ## Examples
 
 ### XLA compilation
 One straightforward use case is to accelerate the computation of the environment with XLA compilation.
-For example, here we compile a full training run, and we vectorise the environment to run multiple environments in parallel.
+For example, here we vectorise the environment to run multiple environments in parallel, and compile **the full training run**.
 
-You can find a superficial performance comparison with [minigrid](https://github.com/Farama-Foundation/Minigrid) in the [docs](docs/profiling.ipynb).
+You can find a partial performance comparison with [minigrid](https://github.com/Farama-Foundation/Minigrid) in the [docs](docs/profiling.ipynb).
 
 ```python
 import jax
 import navix as nx
 
 
 def run(seed)
@@ -310,16 +309,16 @@
 TODO(epignatelli): add example.
 
 
 ## Cite
 If you use `helx` please consider citing it as:
 
 ```bibtex
-@misc{helx,
+@misc{pignatelli2023navix,
   author = {Pignatelli, Eduardo},
-  title = {Navix: Reinforcement Learning navigation with Autograd and XLA},
+  title = {Navix: Accelerated gridworld navigation with JAX},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/epignatelli/navix}}
   }
 ```
```

### Comparing `Navix-0.1.1/README.md` & `Navix-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -9,37 +9,36 @@
 
 ## What is NAVIX?
 NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **~2000x** faster with Autograd and XLA support.
 You can see a superficial performance comparison [here](docs/profiling.ipynb).
 
 
 ## Installation
-We currently support the OSs that are supported by JAX does.
-Please follow the [JAX installation guide](https://github.com/google/jax#installation) to install the correct version of JAX for your OS.
+We currently support the OSs supported by JAX.
+You can find a description [here](https://github.com/google/jax#installation).
 
-You might want to follow the same guide to use your faviourite accelerator
+You might want to follow the same guide to install jax for your faviourite accelerator
 (e.g. [CPU](https://github.com/google/jax#pip-installation-cpu),
 [GPU](https://github.com/google/jax#pip-installation-gpu-cuda-installed-locally-harder), or
 [TPU](https://github.com/google/jax#pip-installation-colab-tpu)
 ).
 
-Then, install `navix` with:
-
+Then, install `navix` and its dependencies with:
 ```bash
 pip install navix
 ```
 
 ---
 ## Examples
 
 ### XLA compilation
 One straightforward use case is to accelerate the computation of the environment with XLA compilation.
-For example, here we compile a full training run, and we vectorise the environment to run multiple environments in parallel.
+For example, here we vectorise the environment to run multiple environments in parallel, and compile **the full training run**.
 
-You can find a superficial performance comparison with [minigrid](https://github.com/Farama-Foundation/Minigrid) in the [docs](docs/profiling.ipynb).
+You can find a partial performance comparison with [minigrid](https://github.com/Farama-Foundation/Minigrid) in the [docs](docs/profiling.ipynb).
 
 ```python
 import jax
 import navix as nx
 
 
 def run(seed)
@@ -64,16 +63,16 @@
 TODO(epignatelli): add example.
 
 
 ## Cite
 If you use `helx` please consider citing it as:
 
 ```bibtex
-@misc{helx,
+@misc{pignatelli2023navix,
   author = {Pignatelli, Eduardo},
-  title = {Navix: Reinforcement Learning navigation with Autograd and XLA},
+  title = {Navix: Accelerated gridworld navigation with JAX},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/epignatelli/navix}}
   }
 ```
```

### Comparing `Navix-0.1.1/docs/profiling.ipynb` & `Navix-0.1.2/docs/profiling.ipynb`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/navix/__init__.py` & `Navix-0.1.2/navix/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 
 
 from __future__ import annotations
 
-__version__ = "0.1.1"
+__version__ = "0.1.2"
 __version_info__ = tuple(int(i) for i in __version__.split(".") if i.isdigit())
 
 
 from . import (
     actions,
     components,
     grid,
```

### Comparing `Navix-0.1.1/navix/actions.py` & `Navix-0.1.2/navix/actions.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/navix/components.py` & `Navix-0.1.2/navix/components.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/navix/environments/__init__.py` & `Navix-0.1.2/navix/environments/__init__.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/navix/environments/environment.py` & `Navix-0.1.2/navix/environments/environment.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/navix/environments/room.py` & `Navix-0.1.2/navix/environments/room.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/navix/grid.py` & `Navix-0.1.2/navix/grid.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/navix/observations.py` & `Navix-0.1.2/navix/observations.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/navix/tasks.py` & `Navix-0.1.2/navix/tasks.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/navix/termination.py` & `Navix-0.1.2/navix/termination.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/navix/transitions.py` & `Navix-0.1.2/navix/transitions.py`

 * *Files identical despite different names*

### Comparing `Navix-0.1.1/pyproject.toml` & `Navix-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 [build-system]
 build-backend = "setuptools.build_meta"
 requires = ["setuptools >= 50", "setuptools-scm[toml]>=6.2", "wheel"]
 
 [project]
 name = "Navix"
 dynamic = ["version", "dependencies"]
-description = "Gridworld navigation for Reinforcement Learning with JAX"
+description = "Accelerated gridworld navigation with JAX for deep reinforcement learning"
 requires-python = ">=3.9"
 readme = "README.md"
 license = {file = "LICENSE", name = "Apache-2.0"}
 authors = [
   {name = "Eduardo Pignatelli", email = "edu.pignatelli@gmail.com"},
 ]
 maintainers = [
```

### Comparing `Navix-0.1.1/tests/test_environment.py` & `Navix-0.1.2/tests/test_environment.py`

 * *Files identical despite different names*

