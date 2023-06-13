# Comparing `tmp/pyrlprob-2.0.3.tar.gz` & `tmp/pyrlprob-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrlprob-2.0.3.tar", last modified: Tue Apr 25 19:26:18 2023, max compression
+gzip compressed data, was "pyrlprob-2.0.4.tar", last modified: Tue Jun 13 12:12:11 2023, max compression
```

## Comparing `pyrlprob-2.0.3.tar` & `pyrlprob-2.0.4.tar`

### file list

```diff
@@ -1,74 +1,73 @@
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.626211 pyrlprob-2.0.3/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1073 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/LICENSE.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      301 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/MANIFEST.in
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2322 2023-04-25 19:26:18.625215 pyrlprob-2.0.3/PKG-INFO
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1803 2023-03-08 19:07:40.000000 pyrlprob-2.0.3/README.md
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      103 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyproject.toml
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.343208 pyrlprob-2.0.3/pyrlprob/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      250 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1157 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/__main__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)    15337 2023-04-21 21:39:44.000000 pyrlprob-2.0.3/pyrlprob/base_funs.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      661 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/commands.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.277208 pyrlprob-2.0.3/pyrlprob/include/
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.370209 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2938 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/binding.cpp
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     5140 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/mdp.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     3818 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/mdp_vec.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     4114 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/include/pyrlprob/py_mdp.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     7448 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/mdp.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)    12688 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/problem.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.447207 pyrlprob-2.0.3/pyrlprob/tests/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      477 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/__init__.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.527209 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      210 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      390 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/binding.cpp
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     6849 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.cpp
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2063 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1830 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.py
--rwx------   0 lorenzof (1001204911) domain users (1000000513)   463776 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      696 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d_dyn.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1405 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/rk4.h
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1282 2023-03-08 18:08:23.000000 pyrlprob-2.0.3/pyrlprob/tests/landing1d_cpp.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1574 2023-04-21 21:36:35.000000 pyrlprob-2.0.3/pyrlprob/tests/landing1d_load.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1266 2023-04-21 21:39:57.000000 pyrlprob-2.0.3/pyrlprob/tests/landing1d_py.yaml
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.539206 pyrlprob-2.0.3/pyrlprob/tests/py_tests/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      190 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     4713 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      974 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d_dyn.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     6161 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d_gym.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.611210 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      428 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      691 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      331 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      560 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1064 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      496 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      433 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_DQN.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      713 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      520 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      456 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      582 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      732 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      639 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      497 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_A2C.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      432 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PG.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      558 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      714 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      615 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     5273 2023-04-21 21:13:31.000000 pyrlprob-2.0.3/pyrlprob/tests/test_landing1d.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2813 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/tests/test_multiple_gym.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.623205 pyrlprob-2.0.3/pyrlprob/utils/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      546 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/utils/__init__.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     3183 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/utils/auxiliary.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     4637 2023-04-25 19:25:53.000000 pyrlprob-2.0.3/pyrlprob/utils/callbacks.py
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     3036 2022-11-23 23:28:53.000000 pyrlprob-2.0.3/pyrlprob/utils/plots.py
-drwx------   0 lorenzof (1001204911) domain users (1000000513)        0 2023-04-25 19:26:18.357207 pyrlprob-2.0.3/pyrlprob.egg-info/
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2322 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/PKG-INFO
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     2454 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/SOURCES.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)        1 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/dependency_links.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)      194 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/requires.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)        9 2023-04-25 19:26:18.000000 pyrlprob-2.0.3/pyrlprob.egg-info/top_level.txt
--rw-------   0 lorenzof (1001204911) domain users (1000000513)       38 2023-04-25 19:26:18.627209 pyrlprob-2.0.3/setup.cfg
--rw-------   0 lorenzof (1001204911) domain users (1000000513)     1242 2023-04-25 19:25:59.000000 pyrlprob-2.0.3/setup.py
+drwxr-xr-x   0 lorenzofederici   (501) staff       (20)        0 2023-06-13 12:12:11.523850 pyrlprob-2.0.4/
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     1073 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/LICENSE.txt
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      301 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/MANIFEST.in
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     2285 2023-06-13 12:12:11.523697 pyrlprob-2.0.4/PKG-INFO
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     1803 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/README.md
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      103 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyproject.toml
+drwxr-xr-x   0 lorenzofederici   (501) staff       (20)        0 2023-06-13 12:12:11.512679 pyrlprob-2.0.4/pyrlprob/
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      250 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/__init__.py
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     1157 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/__main__.py
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)    15337 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/base_funs.py
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      661 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/commands.py
+drwxr-xr-x   0 lorenzofederici   (501) staff       (20)        0 2023-06-13 12:12:11.510368 pyrlprob-2.0.4/pyrlprob/include/
+drwxr-xr-x   0 lorenzofederici   (501) staff       (20)        0 2023-06-13 12:12:11.513964 pyrlprob-2.0.4/pyrlprob/include/pyrlprob/
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     2938 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/include/pyrlprob/binding.cpp
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     5140 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/include/pyrlprob/mdp.h
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     3818 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/include/pyrlprob/mdp_vec.h
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     4114 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/include/pyrlprob/py_mdp.h
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     7448 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/mdp.py
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)    12688 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/problem.py
+drwxr-xr-x   0 lorenzofederici   (501) staff       (20)        0 2023-06-13 12:12:11.515130 pyrlprob-2.0.4/pyrlprob/tests/
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      477 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/__init__.py
+drwxr-xr-x   0 lorenzofederici   (501) staff       (20)        0 2023-06-13 12:12:11.517560 pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      210 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/__init__.py
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      390 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/binding.cpp
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     6849 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/landing1d.cpp
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     2063 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/landing1d.h
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     1830 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/landing1d.py
+-rwxr-xr-x   0 lorenzofederici   (501) staff       (20)   463776 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      696 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/landing1d_dyn.h
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     1405 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/rk4.h
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     1282 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/landing1d_cpp.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     1266 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/landing1d_py.yaml
+drwxr-xr-x   0 lorenzofederici   (501) staff       (20)        0 2023-06-13 12:12:11.518231 pyrlprob-2.0.4/pyrlprob/tests/py_tests/
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      190 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/__init__.py
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     4713 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/landing1d.py
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      974 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/landing1d_dyn.py
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     6161 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/landing1d_gym.py
+drwxr-xr-x   0 lorenzofederici   (501) staff       (20)        0 2023-06-13 12:12:11.522865 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      428 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_A2C.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      691 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      331 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PG.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      560 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     1064 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      496 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_A2C.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      433 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_DQN.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      432 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PG.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      558 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      713 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      520 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      456 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PG.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      582 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      732 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      639 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      497 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_A2C.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      432 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PG.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      558 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      714 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      615 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     5273 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/test_landing1d.py
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     2813 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/tests/test_multiple_gym.py
+drwxr-xr-x   0 lorenzofederici   (501) staff       (20)        0 2023-06-13 12:12:11.523477 pyrlprob-2.0.4/pyrlprob/utils/
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      546 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/utils/__init__.py
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     3183 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/utils/auxiliary.py
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     4637 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/utils/callbacks.py
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     3036 2023-06-13 11:56:45.000000 pyrlprob-2.0.4/pyrlprob/utils/plots.py
+drwxr-xr-x   0 lorenzofederici   (501) staff       (20)        0 2023-06-13 12:12:11.513421 pyrlprob-2.0.4/pyrlprob.egg-info/
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     2285 2023-06-13 12:12:11.000000 pyrlprob-2.0.4/pyrlprob.egg-info/PKG-INFO
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     2419 2023-06-13 12:12:11.000000 pyrlprob-2.0.4/pyrlprob.egg-info/SOURCES.txt
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)        1 2023-06-13 12:12:11.000000 pyrlprob-2.0.4/pyrlprob.egg-info/dependency_links.txt
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)      194 2023-06-13 12:12:11.000000 pyrlprob-2.0.4/pyrlprob.egg-info/requires.txt
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)        9 2023-06-13 12:12:11.000000 pyrlprob-2.0.4/pyrlprob.egg-info/top_level.txt
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)       38 2023-06-13 12:12:11.523893 pyrlprob-2.0.4/setup.cfg
+-rw-r--r--   0 lorenzofederici   (501) staff       (20)     1242 2023-06-13 12:05:36.000000 pyrlprob-2.0.4/setup.py
```

### Comparing `pyrlprob-2.0.3/LICENSE.txt` & `pyrlprob-2.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/PKG-INFO` & `pyrlprob-2.0.4/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pyrlprob
-Version: 2.0.3
+Version: 2.0.4
 Summary: Train Gym-derived environments in Python/C++ through Ray RLlib
 Home-page: https://github.com/LorenzoFederici/pyrlprob
 Author: Lorenzo Federici
 Author-email: federicilorenzo94@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -56,9 +54,7 @@
 ## Credits
 pyRLprob has been created by [Lorenzo Federici](https://github.com/LorenzoFederici) in 2021.
 For any problem, clarification or suggestion, you can contact the author at [lorenzof@arizona.edu](mailto:lorenzof@arizona.edu).
 
 ## License
 The package is under the [MIT](https://choosealicense.com/licenses/mit/) license.
 
-
-
```

### Comparing `pyrlprob-2.0.3/README.md` & `pyrlprob-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/__main__.py` & `pyrlprob-2.0.4/pyrlprob/__main__.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/base_funs.py` & `pyrlprob-2.0.4/pyrlprob/base_funs.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/commands.py` & `pyrlprob-2.0.4/pyrlprob/commands.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/include/pyrlprob/binding.cpp` & `pyrlprob-2.0.4/pyrlprob/include/pyrlprob/binding.cpp`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/include/pyrlprob/mdp.h` & `pyrlprob-2.0.4/pyrlprob/include/pyrlprob/mdp.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/include/pyrlprob/mdp_vec.h` & `pyrlprob-2.0.4/pyrlprob/include/pyrlprob/mdp_vec.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/include/pyrlprob/py_mdp.h` & `pyrlprob-2.0.4/pyrlprob/include/pyrlprob/py_mdp.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/mdp.py` & `pyrlprob-2.0.4/pyrlprob/mdp.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/problem.py` & `pyrlprob-2.0.4/pyrlprob/problem.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.cpp` & `pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/landing1d.cpp`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.h` & `pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/landing1d.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d.py` & `pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so` & `pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/landing1d_cpp.cpython-39-x86_64-linux-gnu.so`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/landing1d_dyn.h` & `pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/landing1d_dyn.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/cpp_tests/rk4.h` & `pyrlprob-2.0.4/pyrlprob/tests/cpp_tests/rk4.h`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/landing1d_cpp.yaml` & `pyrlprob-2.0.4/pyrlprob/tests/landing1d_cpp.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/landing1d_load.yaml` & `pyrlprob-2.0.4/pyrlprob/tests/landing1d_py.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,69 @@
+run: ppo
+stop:
+  training_iteration: 50
+custom_metrics:
+- cstr_viol
+postproc_data:
+  episode_step_data: 
+  - h
+  - v
+  - m
+  - t
+  - T
+num_eval_episodes: 10
+eval_env_config:
+  env_config:
+    prng_seed: 0
 config:
+  num_workers: 2
+  num_envs_per_worker: 5
+  num_gpus: 0
+  num_cpus_per_worker: 1
+  num_gpus_per_worker: 0
+  num_cpus_for_driver: 1
+  create_env_on_driver: False
+  remote_worker_envs: False
+  rollout_fragment_length: 40
   batch_mode: complete_episodes
-  callbacks: TrainingCallbacks
+  train_batch_size: 400
+  model:
+    fcnet_hiddens: [64, 64]
+    fcnet_activation: tanh
+    vf_share_layers: False
+    free_log_std: True
+  gamma: 1.
+  log_level: INFO
+  framework: tf
+  explore: True
+  ignore_worker_failures: True
+  evaluation_interval: 1
+  evaluation_num_episodes: 2
+  evaluation_config:
+    explore: False
+  evaluation_num_workers: 2
+  use_critic: True
+  use_gae: True
+  lambda: 1.
+  kl_coeff: 0.
+  sgd_minibatch_size: 160
+  shuffle_sequences: True
+  num_sgd_iter: 10
+  lr: 1.0e-04
+  vf_loss_coeff: 0.5
   clip_param: 0.2
-  create_env_on_driver: false
+  callbacks:
+    TrainingCallbacks
   env: pyrlprob.tests.py_tests.pyLanding1DEnv
   env_config:
     H: 40
-    Tmax: 1.227
-    c: 2.349
-    g: 1.0
-    h0_max: 1.2
     h0_min: 0.8
-    hf: 0.0
+    h0_max: 1.2
+    v0_min: -0.85
+    v0_max: -0.75
     m0: 1.0
     tf: 1.397
-    v0_max: -0.75
-    v0_min: -0.85
+    hf: 0.0
     vf: 0.0
-  evaluation_config:
-    explore: false
-  evaluation_interval: 1
-  evaluation_num_episodes: 2
-  evaluation_num_workers: 2
-  explore: true
-  framework: tf
-  gamma: 1.0
-  ignore_worker_failures: true
-  kl_coeff: 0.0
-  lambda: 1.0
-  log_level: INFO
-  lr: 0.0001
-  model:
-    fcnet_activation: tanh
-    fcnet_hiddens:
-    - 64
-    - 64
-    free_log_std: true
-    vf_share_layers: false
-  num_cpus_for_driver: 1
-  num_cpus_per_worker: 1
-  num_envs_per_worker: 5
-  num_gpus: 0
-  num_gpus_per_worker: 0
-  num_sgd_iter: 10
-  num_workers: 2
-  remote_worker_envs: false
-  rollout_fragment_length: 40
-  sgd_minibatch_size: 160
-  shuffle_sequences: true
-  train_batch_size: 400
-  use_critic: true
-  use_gae: true
-  vf_loss_coeff: 0.5
-custom_metrics:
-- cstr_viol
-eval_env_config:
-  env_config:
-    prng_seed: 0
-load:
-  prev_exp_dirs:
-  - /home/lorenzof/Documents/Python_codes/pyrlprob/results/PPO_2023-04-21_14-36-15/PPO_pyrlprob.tests.py_tests.pyLanding1DEnv_8b2d9_00000_0_2023-04-21_14-36-15/
-  prev_last_cps:
-  - 1
-  trainer_dir: /home/lorenzof/Documents/Python_codes/pyrlprob/results/PPO_2023-04-21_14-36-15/
-num_eval_episodes: 28
-postproc_data:
-  episode_step_data:
-  - h
-  - v
-  - m
-  - t
-  - T
-run: ppo
-stop:
-  training_iteration: 2
+    Tmax: 1.227
+    c: 2.349
+    g: 1.0
```

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d.py` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d_dyn.py` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/landing1d_dyn.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/landing1d_gym.py` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/landing1d_gym.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_DQN.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Breakout-v0_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/CartPole-v1_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_A2C.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Landing1D_TD3.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_PPO.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_SAC.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml` & `pyrlprob-2.0.4/pyrlprob/tests/py_tests/tuned_examples/Pendulum-v1_TD3.yaml`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/test_landing1d.py` & `pyrlprob-2.0.4/pyrlprob/tests/test_landing1d.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/tests/test_multiple_gym.py` & `pyrlprob-2.0.4/pyrlprob/tests/test_multiple_gym.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/utils/__init__.py` & `pyrlprob-2.0.4/pyrlprob/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/utils/auxiliary.py` & `pyrlprob-2.0.4/pyrlprob/utils/auxiliary.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/utils/callbacks.py` & `pyrlprob-2.0.4/pyrlprob/utils/callbacks.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob/utils/plots.py` & `pyrlprob-2.0.4/pyrlprob/utils/plots.py`

 * *Files identical despite different names*

### Comparing `pyrlprob-2.0.3/pyrlprob.egg-info/PKG-INFO` & `pyrlprob-2.0.4/pyrlprob.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: pyrlprob
-Version: 2.0.3
+Version: 2.0.4
 Summary: Train Gym-derived environments in Python/C++ through Ray RLlib
 Home-page: https://github.com/LorenzoFederici/pyrlprob
 Author: Lorenzo Federici
 Author-email: federicilorenzo94@gmail.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
@@ -56,9 +54,7 @@
 ## Credits
 pyRLprob has been created by [Lorenzo Federici](https://github.com/LorenzoFederici) in 2021.
 For any problem, clarification or suggestion, you can contact the author at [lorenzof@arizona.edu](mailto:lorenzof@arizona.edu).
 
 ## License
 The package is under the [MIT](https://choosealicense.com/licenses/mit/) license.
 
-
-
```

### Comparing `pyrlprob-2.0.3/pyrlprob.egg-info/SOURCES.txt` & `pyrlprob-2.0.4/pyrlprob.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 pyrlprob.egg-info/top_level.txt
 pyrlprob/include/pyrlprob/binding.cpp
 pyrlprob/include/pyrlprob/mdp.h
 pyrlprob/include/pyrlprob/mdp_vec.h
 pyrlprob/include/pyrlprob/py_mdp.h
 pyrlprob/tests/__init__.py
 pyrlprob/tests/landing1d_cpp.yaml
-pyrlprob/tests/landing1d_load.yaml
 pyrlprob/tests/landing1d_py.yaml
 pyrlprob/tests/test_landing1d.py
 pyrlprob/tests/test_multiple_gym.py
 pyrlprob/tests/cpp_tests/__init__.py
 pyrlprob/tests/cpp_tests/binding.cpp
 pyrlprob/tests/cpp_tests/landing1d.cpp
 pyrlprob/tests/cpp_tests/landing1d.h
```

### Comparing `pyrlprob-2.0.3/setup.py` & `pyrlprob-2.0.4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 from pathlib import Path
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(name='pyrlprob',
-    version='2.0.3',
+    version='2.0.4',
     author='Lorenzo Federici',
     author_email = 'federicilorenzo94@gmail.com',
     description = 'Train Gym-derived environments in Python/C++ through Ray RLlib',
     long_description = long_description,
     long_description_content_type = 'text/markdown',
     url = 'https://github.com/LorenzoFederici/pyrlprob',
     classifiers = [
@@ -22,15 +22,15 @@
         'gym==0.15.3',
         'lz4',
         'matplotlib',
         'numpy',
         'pandas',
         'pybind11',
         'pytest',
-        'ray==1.6.0',
+        'ray==1.8.0',
         'scipy',
         'scikit-image',
         'opencv-python; platform_machine=="x86_64"',
         'tabulate',
         'tensorflow',
         'tensorboardx; platform_machine=="x86_64"',
         'torch',
```

