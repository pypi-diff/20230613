# Comparing `tmp/Navix-0.1.0.tar.gz` & `tmp/Navix-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Navix-0.1.0.tar", last modified: Tue Jun 13 20:40:17 2023, max compression
+gzip compressed data, was "Navix-0.1.1.tar", last modified: Tue Jun 13 21:19:10 2023, max compression
```

## Comparing `Navix-0.1.0.tar` & `Navix-0.1.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:40:17.532035 Navix-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:40:17.528035 Navix-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:40:17.528035 Navix-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 20:40:00.000000 Navix-0.1.0/.github/workflows/CD.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-13 20:40:00.000000 Navix-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 20:40:00.000000 Navix-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 20:40:00.000000 Navix-0.1.0/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 20:40:00.000000 Navix-0.1.0/COPYRIGHT
--rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-13 20:40:00.000000 Navix-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 20:40:00.000000 Navix-0.1.0/NOTICE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:40:17.532035 Navix-0.1.0/Navix.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-06-13 20:40:17.000000 Navix-0.1.0/Navix.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 20:40:17.000000 Navix-0.1.0/Navix.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:40:17.000000 Navix-0.1.0/Navix.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 20:40:17.000000 Navix-0.1.0/Navix.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 20:40:17.000000 Navix-0.1.0/Navix.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16411 2023-06-13 20:40:17.532035 Navix-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-06-13 20:40:00.000000 Navix-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:40:17.532035 Navix-0.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-06-13 20:40:00.000000 Navix-0.1.0/docs/profiling.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:40:17.532035 Navix-0.1.0/navix/
--rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-13 20:40:00.000000 Navix-0.1.0/navix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2241 2023-06-13 20:40:00.000000 Navix-0.1.0/navix/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-06-13 20:40:00.000000 Navix-0.1.0/navix/components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:40:17.532035 Navix-0.1.0/navix/environments/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-13 20:40:00.000000 Navix-0.1.0/navix/environments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2858 2023-06-13 20:40:00.000000 Navix-0.1.0/navix/environments/environment.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-06-13 20:40:00.000000 Navix-0.1.0/navix/environments/room.py
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-13 20:40:00.000000 Navix-0.1.0/navix/grid.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-13 20:40:00.000000 Navix-0.1.0/navix/observations.py
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-06-13 20:40:00.000000 Navix-0.1.0/navix/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)      540 2023-06-13 20:40:00.000000 Navix-0.1.0/navix/termination.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 20:40:00.000000 Navix-0.1.0/navix/transitions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2470 2023-06-13 20:40:00.000000 Navix-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 20:40:00.000000 Navix-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:40:17.532035 Navix-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:40:17.532035 Navix-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-13 20:40:00.000000 Navix-0.1.0/tests/test_environment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.142311 Navix-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.138311 Navix-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.138311 Navix-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2012 2023-06-13 21:18:58.000000 Navix-0.1.1/.github/workflows/CD.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-06-13 21:18:58.000000 Navix-0.1.1/.github/workflows/CI.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 21:18:58.000000 Navix-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 21:18:58.000000 Navix-0.1.1/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 21:18:58.000000 Navix-0.1.1/COPYRIGHT
+-rw-r--r--   0 runner    (1001) docker     (123)    11349 2023-06-13 21:18:58.000000 Navix-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 21:18:58.000000 Navix-0.1.1/NOTICE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.138311 Navix-0.1.1/Navix.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    18017 2023-06-13 21:19:10.000000 Navix-0.1.1/Navix.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      585 2023-06-13 21:19:10.000000 Navix-0.1.1/Navix.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 21:19:10.000000 Navix-0.1.1/Navix.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 21:19:10.000000 Navix-0.1.1/Navix.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-13 21:19:10.000000 Navix-0.1.1/Navix.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18017 2023-06-13 21:19:10.142311 Navix-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-13 21:18:58.000000 Navix-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.138311 Navix-0.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-06-13 21:18:58.000000 Navix-0.1.1/docs/profiling.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.138311 Navix-0.1.1/navix/
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.142311 Navix-0.1.1/navix/environments/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/environments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/environments/environment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1912 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/environments/room.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/observations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/termination.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-06-13 21:18:58.000000 Navix-0.1.1/navix/transitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2471 2023-06-13 21:18:58.000000 Navix-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 21:18:58.000000 Navix-0.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 21:19:10.142311 Navix-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 21:19:10.142311 Navix-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1317 2023-06-13 21:18:58.000000 Navix-0.1.1/tests/test_environment.py
```

### Comparing `Navix-0.1.0/.github/workflows/CD.yml` & `Navix-0.1.1/.github/workflows/CD.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.1.0/.github/workflows/CI.yml` & `Navix-0.1.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `Navix-0.1.0/.gitignore` & `Navix-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `Navix-0.1.0/COPYRIGHT` & `Navix-0.1.1/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `Navix-0.1.0/LICENSE` & `Navix-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `Navix-0.1.0/Navix.egg-info/PKG-INFO` & `Navix-0.1.1/Navix.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.1.0
+Version: 0.1.1
 Summary: Gridworld navigation for Reinforcement Learning with JAX
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -240,43 +240,86 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 License-File: AUTHORS
 
-# Navix
+# NAVIX
 
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 [![CI](https://github.com/epignatelli/navix/actions/workflows/CI.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CI.yml)
 [![CD](https://github.com/epignatelli/navix/actions/workflows/CD.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CD.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/epignatelli/navix?color=%23216477&label=Release)
 
 **[Quickstart](#what-is-navix)** | **[Installation](#installation)** | **[Examples](#examples)** | **[Cite](#cite)**
 
-## What is Navix?
-Navix is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, with Autograd and XLA support.
+## What is NAVIX?
+NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **~2000x** faster with Autograd and XLA support.
 You can see a superficial performance comparison [here](docs/profiling.ipynb).
 
 
 ## Installation
+We currently support the OSs that are supported by JAX does.
+Please follow the [JAX installation guide](https://github.com/google/jax#installation) to install the correct version of JAX for your OS.
+
+You might want to follow the same guide to use your faviourite accelerator
+(e.g. [CPU](https://github.com/google/jax#pip-installation-cpu),
+[GPU](https://github.com/google/jax#pip-installation-gpu-cuda-installed-locally-harder), or
+[TPU](https://github.com/google/jax#pip-installation-colab-tpu)
+).
+
+Then, install `navix` with:
+
 ```bash
-pip install git+https://github.com/epignatelli/navix
+pip install navix
 ```
 
 ---
 ## Examples
-TODO
+
+### XLA compilation
+One straightforward use case is to accelerate the computation of the environment with XLA compilation.
+For example, here we compile a full training run, and we vectorise the environment to run multiple environments in parallel.
+
+You can find a superficial performance comparison with [minigrid](https://github.com/Farama-Foundation/Minigrid) in the [docs](docs/profiling.ipynb).
+
+```python
+import jax
+import navix as nx
+
+
+def run(seed)
+  env = nx.environments.Room(16, 16, 8)
+  key = jax.random.PRNGKey(seed)
+  timestep = env.reset(key)
+  actions = jax.random.randint(key, (N_TIMESTEPS,), 0, 6)
+
+  def body_fun(timestep, action):
+      timestep = env.step(timestep, jnp.asarray(action))
+      return timestep, ()
+
+  return jax.lax.scan(body_fun, timestep, jnp.asarray(actions, dtype=jnp.int32))[0]
+
+final_timestep = jax.jit(jax.vmap(run))(jax.numpy.arange(1000))
+```
+
+### Backpropagation through the environment
+
+Another use case it to backpropagate through the environment transition function, for example to learn a world model.
+
+TODO(epignatelli): add example.
+
 
 ## Cite
 If you use `helx` please consider citing it as:
 
 ```bibtex
 @misc{helx,
   author = {Pignatelli, Eduardo},
-  title = {Navix: Gridworld navigation with Autograd and XLA},
+  title = {Navix: Reinforcement Learning navigation with Autograd and XLA},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/epignatelli/navix}}
   }
 ```
```

### Comparing `Navix-0.1.0/Navix.egg-info/SOURCES.txt` & `Navix-0.1.1/Navix.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Navix-0.1.0/PKG-INFO` & `Navix-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Navix
-Version: 0.1.0
+Version: 0.1.1
 Summary: Gridworld navigation for Reinforcement Learning with JAX
 Author-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 Maintainer-email: Eduardo Pignatelli <edu.pignatelli@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -240,43 +240,86 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 License-File: NOTICE
 License-File: AUTHORS
 
-# Navix
+# NAVIX
 
 [![Project Status: WIP – Initial development is in progress, but there has not yet been a stable, usable release suitable for the public.](https://www.repostatus.org/badges/latest/wip.svg)](https://www.repostatus.org/#wip)
 [![CI](https://github.com/epignatelli/navix/actions/workflows/CI.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CI.yml)
 [![CD](https://github.com/epignatelli/navix/actions/workflows/CD.yml/badge.svg)](https://github.com/epignatelli/navix/actions/workflows/CD.yml)
 ![GitHub release (latest by date)](https://img.shields.io/github/v/release/epignatelli/navix?color=%23216477&label=Release)
 
 **[Quickstart](#what-is-navix)** | **[Installation](#installation)** | **[Examples](#examples)** | **[Cite](#cite)**
 
-## What is Navix?
-Navix is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, with Autograd and XLA support.
+## What is NAVIX?
+NAVIX is [minigrid](https://github.com/Farama-Foundation/Minigrid) in JAX, **~2000x** faster with Autograd and XLA support.
 You can see a superficial performance comparison [here](docs/profiling.ipynb).
 
 
 ## Installation
+We currently support the OSs that are supported by JAX does.
+Please follow the [JAX installation guide](https://github.com/google/jax#installation) to install the correct version of JAX for your OS.
+
+You might want to follow the same guide to use your faviourite accelerator
+(e.g. [CPU](https://github.com/google/jax#pip-installation-cpu),
+[GPU](https://github.com/google/jax#pip-installation-gpu-cuda-installed-locally-harder), or
+[TPU](https://github.com/google/jax#pip-installation-colab-tpu)
+).
+
+Then, install `navix` with:
+
 ```bash
-pip install git+https://github.com/epignatelli/navix
+pip install navix
 ```
 
 ---
 ## Examples
-TODO
+
+### XLA compilation
+One straightforward use case is to accelerate the computation of the environment with XLA compilation.
+For example, here we compile a full training run, and we vectorise the environment to run multiple environments in parallel.
+
+You can find a superficial performance comparison with [minigrid](https://github.com/Farama-Foundation/Minigrid) in the [docs](docs/profiling.ipynb).
+
+```python
+import jax
+import navix as nx
+
+
+def run(seed)
+  env = nx.environments.Room(16, 16, 8)
+  key = jax.random.PRNGKey(seed)
+  timestep = env.reset(key)
+  actions = jax.random.randint(key, (N_TIMESTEPS,), 0, 6)
+
+  def body_fun(timestep, action):
+      timestep = env.step(timestep, jnp.asarray(action))
+      return timestep, ()
+
+  return jax.lax.scan(body_fun, timestep, jnp.asarray(actions, dtype=jnp.int32))[0]
+
+final_timestep = jax.jit(jax.vmap(run))(jax.numpy.arange(1000))
+```
+
+### Backpropagation through the environment
+
+Another use case it to backpropagate through the environment transition function, for example to learn a world model.
+
+TODO(epignatelli): add example.
+
 
 ## Cite
 If you use `helx` please consider citing it as:
 
 ```bibtex
 @misc{helx,
   author = {Pignatelli, Eduardo},
-  title = {Navix: Gridworld navigation with Autograd and XLA},
+  title = {Navix: Reinforcement Learning navigation with Autograd and XLA},
   year = {2023},
   publisher = {GitHub},
   journal = {GitHub repository},
   howpublished = {\url{https://github.com/epignatelli/navix}}
   }
 ```
```

### Comparing `Navix-0.1.0/docs/profiling.ipynb` & `Navix-0.1.1/docs/profiling.ipynb`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999255952380952%*

 * *Differences: {"'cells'": "{2: {'source': {insert: [(13, '\\n')]}}}"}*

```diff
@@ -56,14 +56,15 @@
                 "\n",
                 "\n",
                 "def profile_navix(seed):\n",
                 "    env = nx.environments.Room(16, 16, 8)\n",
                 "    key = jax.random.PRNGKey(seed)\n",
                 "    timestep = env.reset(key)\n",
                 "    actions = jax.random.randint(key, (N_TIMESTEPS,), 0, 6)\n",
+                "\n",
                 "    def body_fun(carry, x):\n",
                 "        timestep = carry\n",
                 "        action = x\n",
                 "        timestep = env.step(timestep, jnp.asarray(action))\n",
                 "        return timestep, ()\n",
                 "\n",
                 "    return jax.lax.scan(body_fun, timestep, jnp.asarray(actions, dtype=jnp.int32))[0]\n",
```

### Comparing `Navix-0.1.0/navix/environments/environment.py` & `Navix-0.1.1/navix/environments/environment.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,28 @@
-from __future__ import annotations
+# Copyright 2023 The Navix Authors.
+
+# Licensed to the Apache Software Foundation (ASF) under one
+# or more contributor license agreements.  See the NOTICE file
+# distributed with this work for additional information
+# regarding copyright ownership.  The ASF licenses this file
+# to you under the Apache License, Version 2.0 (the
+# "License"); you may not use this file except in compliance
+# with the License.  You may obtain a copy of the License at
+
+#   http://www.apache.org/licenses/LICENSE-2.0
 
+# Unless required by applicable law or agreed to in writing,
+# software distributed under the License is distributed on an
+# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
+# KIND, either express or implied.  See the License for the
+# specific language governing permissions and limitations
+# under the License.
+
+
+from __future__ import annotations
 
 import abc
 from typing import Callable
 import jax
 import jax.numpy as jnp
 from jax.random import KeyArray
 from chex import Array
```

### Comparing `Navix-0.1.0/pyproject.toml` & `Navix-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -67,9 +67,10 @@
 exclude = ["test", "examples"]
 
 
 [tool.distutils.bdist_wheel]
 universal = true
 
 
+
 [tool.black]
 line-length = 88
```

### Comparing `Navix-0.1.0/tests/test_environment.py` & `Navix-0.1.1/tests/test_environment.py`

 * *Files identical despite different names*

