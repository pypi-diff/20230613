# Comparing `tmp/evox-0.1.0.tar.gz` & `tmp/evox-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evox-0.1.0.tar", last modified: Tue Jun  6 13:16:17 2023, max compression
+gzip compressed data, was "evox-0.2.0.tar", last modified: Tue Jun 13 07:04:20 2023, max compression
```

## Comparing `evox-0.1.0.tar` & `evox-0.2.0.tar`

### file list

```diff
@@ -1,120 +1,119 @@
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.900022 evox-0.1.0/
--rw-r--r--   0 bill      (1000) users      (100)     1546 2022-11-22 16:31:12.000000 evox-0.1.0/LICENSE
--rw-r--r--   0 bill      (1000) users      (100)     4801 2023-06-06 13:16:17.900022 evox-0.1.0/PKG-INFO
--rw-r--r--   0 bill      (1000) users      (100)     2302 2023-06-06 13:11:57.000000 evox-0.1.0/README.md
--rw-r--r--   0 bill      (1000) users      (100)     1185 2023-06-06 13:10:46.000000 evox-0.1.0/pyproject.toml
--rw-r--r--   0 bill      (1000) users      (100)       38 2023-06-06 13:16:17.900022 evox-0.1.0/setup.cfg
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.890022 evox-0.1.0/src/
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.892022 evox-0.1.0/src/evox/
--rw-r--r--   0 bill      (1000) users      (100)      240 2022-10-21 09:22:33.000000 evox-0.1.0/src/evox/__init__.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.892022 evox-0.1.0/src/evox/algorithms/
--rw-r--r--   0 bill      (1000) users      (100)      197 2023-02-09 12:37:43.000000 evox-0.1.0/src/evox/algorithms/__init__.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.893022 evox-0.1.0/src/evox/algorithms/containers/
--rw-r--r--   0 bill      (1000) users      (100)      173 2023-02-28 03:20:59.000000 evox-0.1.0/src/evox/algorithms/containers/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     5518 2023-03-06 02:25:38.000000 evox-0.1.0/src/evox/algorithms/containers/clustered_algorithm.py
--rw-r--r--   0 bill      (1000) users      (100)     7625 2023-03-29 08:40:11.000000 evox-0.1.0/src/evox/algorithms/containers/coevolution.py
--rw-r--r--   0 bill      (1000) users      (100)     1632 2023-04-23 13:21:16.000000 evox-0.1.0/src/evox/algorithms/containers/tree_algorithm.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.893022 evox-0.1.0/src/evox/algorithms/mo/
--rw-r--r--   0 bill      (1000) users      (100)       96 2022-10-21 09:22:33.000000 evox-0.1.0/src/evox/algorithms/mo/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     3388 2023-02-02 13:10:39.000000 evox-0.1.0/src/evox/algorithms/mo/ibea.py
--rw-r--r--   0 bill      (1000) users      (100)     6247 2023-02-02 13:11:05.000000 evox-0.1.0/src/evox/algorithms/mo/moead.py
--rw-r--r--   0 bill      (1000) users      (100)     3117 2023-02-02 13:11:15.000000 evox-0.1.0/src/evox/algorithms/mo/nsga2.py
--rw-r--r--   0 bill      (1000) users      (100)     4270 2023-02-02 13:11:49.000000 evox-0.1.0/src/evox/algorithms/mo/rvea.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.894022 evox-0.1.0/src/evox/algorithms/so/
--rw-r--r--   0 bill      (1000) users      (100)      183 2023-02-02 12:50:02.000000 evox-0.1.0/src/evox/algorithms/so/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     8254 2023-03-30 08:15:51.000000 evox-0.1.0/src/evox/algorithms/so/cma_es.py
--rw-r--r--   0 bill      (1000) users      (100)     2878 2023-03-06 07:47:48.000000 evox-0.1.0/src/evox/algorithms/so/cso.py
--rw-r--r--   0 bill      (1000) users      (100)     4989 2023-03-01 13:30:16.000000 evox-0.1.0/src/evox/algorithms/so/de.py
--rw-r--r--   0 bill      (1000) users      (100)     6758 2023-02-08 16:28:36.000000 evox-0.1.0/src/evox/algorithms/so/nes.py
--rw-r--r--   0 bill      (1000) users      (100)     2431 2023-02-02 13:07:57.000000 evox-0.1.0/src/evox/algorithms/so/open_es.py
--rw-r--r--   0 bill      (1000) users      (100)     3927 2023-03-30 08:13:48.000000 evox-0.1.0/src/evox/algorithms/so/pgpe.py
--rw-r--r--   0 bill      (1000) users      (100)     3349 2023-03-30 07:15:54.000000 evox-0.1.0/src/evox/algorithms/so/pso.py
--rw-r--r--   0 bill      (1000) users      (100)      267 2022-10-21 09:22:33.000000 evox-0.1.0/src/evox/algorithms/so/sort_utils.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.895022 evox-0.1.0/src/evox/core/
--rw-r--r--   0 bill      (1000) users      (100)     1056 2023-02-15 09:45:58.000000 evox-0.1.0/src/evox/core/algorithm.py
--rw-r--r--   0 bill      (1000) users      (100)     6286 2023-03-06 02:50:05.000000 evox-0.1.0/src/evox/core/module.py
--rw-r--r--   0 bill      (1000) users      (100)      255 2023-02-15 09:46:19.000000 evox-0.1.0/src/evox/core/operator.py
--rw-r--r--   0 bill      (1000) users      (100)      600 2023-02-15 09:46:26.000000 evox-0.1.0/src/evox/core/problem.py
--rw-r--r--   0 bill      (1000) users      (100)     7168 2023-03-06 02:50:12.000000 evox-0.1.0/src/evox/core/state.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.895022 evox-0.1.0/src/evox/metrics/
--rw-r--r--   0 bill      (1000) users      (100)       57 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/metrics/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     1287 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/metrics/hypervolume.py
--rw-r--r--   0 bill      (1000) users      (100)      274 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/metrics/igd.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.895022 evox-0.1.0/src/evox/monitors/
--rw-r--r--   0 bill      (1000) users      (100)      105 2023-01-04 08:43:02.000000 evox-0.1.0/src/evox/monitors/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     1719 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/monitors/fitness.py
--rw-r--r--   0 bill      (1000) users      (100)     4531 2023-01-04 08:46:06.000000 evox-0.1.0/src/evox/monitors/gym.py
--rw-r--r--   0 bill      (1000) users      (100)     2666 2022-10-21 09:22:33.000000 evox-0.1.0/src/evox/monitors/population.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.895022 evox-0.1.0/src/evox/operators/
--rw-r--r--   0 bill      (1000) users      (100)      128 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/operators/__init__.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.896022 evox-0.1.0/src/evox/operators/crossover/
--rw-r--r--   0 bill      (1000) users      (100)      212 2022-10-21 09:22:33.000000 evox-0.1.0/src/evox/operators/crossover/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     1492 2023-02-02 13:15:24.000000 evox-0.1.0/src/evox/operators/crossover/differential_evolution.py
--rw-r--r--   0 bill      (1000) users      (100)     1185 2023-02-02 13:15:34.000000 evox-0.1.0/src/evox/operators/crossover/one_point.py
--rw-r--r--   0 bill      (1000) users      (100)     2133 2023-02-02 13:15:42.000000 evox-0.1.0/src/evox/operators/crossover/sbx.py
--rw-r--r--   0 bill      (1000) users      (100)     1709 2023-02-02 13:15:52.000000 evox-0.1.0/src/evox/operators/crossover/simulated_binary.py
--rw-r--r--   0 bill      (1000) users      (100)     1072 2023-02-02 13:15:59.000000 evox-0.1.0/src/evox/operators/crossover/uniform.py
--rw-r--r--   0 bill      (1000) users      (100)     1876 2023-02-15 09:46:32.000000 evox-0.1.0/src/evox/operators/crowding_distance_sort.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.896022 evox-0.1.0/src/evox/operators/mutation/
--rw-r--r--   0 bill      (1000) users      (100)      112 2022-11-22 16:33:53.000000 evox-0.1.0/src/evox/operators/mutation/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)      778 2023-02-02 13:16:07.000000 evox-0.1.0/src/evox/operators/mutation/bitflip.py
--rw-r--r--   0 bill      (1000) users      (100)      439 2023-02-02 13:16:14.000000 evox-0.1.0/src/evox/operators/mutation/gaussian.py
--rw-r--r--   0 bill      (1000) users      (100)     1869 2023-02-02 13:16:20.000000 evox-0.1.0/src/evox/operators/mutation/pm_mutation.py
--rw-r--r--   0 bill      (1000) users      (100)     2581 2023-02-02 13:17:19.000000 evox-0.1.0/src/evox/operators/non_dominated_sort.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.897022 evox-0.1.0/src/evox/operators/sampling/
--rw-r--r--   0 bill      (1000) users      (100)       88 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/operators/sampling/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)      592 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/operators/sampling/latin_hypercude.py
--rw-r--r--   0 bill      (1000) users      (100)     1408 2023-01-31 04:52:29.000000 evox-0.1.0/src/evox/operators/sampling/uniform.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.897022 evox-0.1.0/src/evox/operators/selection/
--rw-r--r--   0 bill      (1000) users      (100)      154 2022-10-21 09:22:33.000000 evox-0.1.0/src/evox/operators/selection/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     1917 2023-02-02 13:16:50.000000 evox-0.1.0/src/evox/operators/selection/rvea_selection.py
--rw-r--r--   0 bill      (1000) users      (100)     1579 2023-02-02 13:16:59.000000 evox-0.1.0/src/evox/operators/selection/tournament.py
--rw-r--r--   0 bill      (1000) users      (100)      459 2023-02-02 13:17:07.000000 evox-0.1.0/src/evox/operators/selection/uniform_random.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.897022 evox-0.1.0/src/evox/pipelines/
--rw-r--r--   0 bill      (1000) users      (100)      430 2023-03-28 15:25:39.000000 evox-0.1.0/src/evox/pipelines/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     8175 2023-02-15 09:43:08.000000 evox-0.1.0/src/evox/pipelines/distributed.py
--rw-r--r--   0 bill      (1000) users      (100)     1312 2023-01-04 08:43:02.000000 evox-0.1.0/src/evox/pipelines/gym.py
--rw-r--r--   0 bill      (1000) users      (100)     5308 2023-04-07 02:08:06.000000 evox-0.1.0/src/evox/pipelines/multidevice.py
--rw-r--r--   0 bill      (1000) users      (100)     1574 2023-03-24 02:21:20.000000 evox-0.1.0/src/evox/pipelines/standard.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.897022 evox-0.1.0/src/evox/problems/
--rw-r--r--   0 bill      (1000) users      (100)       99 2023-02-09 12:38:26.000000 evox-0.1.0/src/evox/problems/__init__.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.898022 evox-0.1.0/src/evox/problems/classic/
--rw-r--r--   0 bill      (1000) users      (100)      284 2022-10-21 09:22:33.000000 evox-0.1.0/src/evox/problems/classic/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)      523 2023-03-24 03:21:45.000000 evox-0.1.0/src/evox/problems/classic/ackley.py
--rw-r--r--   0 bill      (1000) users      (100)    10161 2023-02-02 12:54:06.000000 evox-0.1.0/src/evox/problems/classic/dtlz.py
--rw-r--r--   0 bill      (1000) users      (100)      321 2023-02-02 12:54:20.000000 evox-0.1.0/src/evox/problems/classic/griewank.py
--rw-r--r--   0 bill      (1000) users      (100)      284 2023-02-02 12:54:28.000000 evox-0.1.0/src/evox/problems/classic/rastrigin.py
--rw-r--r--   0 bill      (1000) users      (100)      331 2023-02-02 12:54:35.000000 evox-0.1.0/src/evox/problems/classic/rosenbrock.py
--rw-r--r--   0 bill      (1000) users      (100)      278 2023-02-02 12:54:40.000000 evox-0.1.0/src/evox/problems/classic/sphere.py
--rw-r--r--   0 bill      (1000) users      (100)     2010 2023-02-15 09:46:35.000000 evox-0.1.0/src/evox/problems/classic/zdt.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.898022 evox-0.1.0/src/evox/problems/neuroevolution/
--rw-r--r--   0 bill      (1000) users      (100)      355 2023-01-31 14:32:11.000000 evox-0.1.0/src/evox/problems/neuroevolution/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)    11631 2023-04-23 13:21:16.000000 evox-0.1.0/src/evox/problems/neuroevolution/torchvision_dataset.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.899022 evox-0.1.0/src/evox/problems/rl/
--rw-r--r--   0 bill      (1000) users      (100)      543 2023-03-23 07:57:10.000000 evox-0.1.0/src/evox/problems/rl/__init__.py
--rw-r--r--   0 bill      (1000) users      (100)     3427 2023-03-30 06:51:16.000000 evox-0.1.0/src/evox/problems/rl/brax.py
--rw-r--r--   0 bill      (1000) users      (100)    12332 2023-02-15 09:47:00.000000 evox-0.1.0/src/evox/problems/rl/gym.py
--rw-r--r--   0 bill      (1000) users      (100)    11621 2023-02-15 09:46:53.000000 evox-0.1.0/src/evox/problems/rl/gym_mo.py
--rw-r--r--   0 bill      (1000) users      (100)        0 2023-03-13 02:52:06.000000 evox-0.1.0/src/evox/problems/rl/gymnasium.py
--rw-r--r--   0 bill      (1000) users      (100)     5106 2023-03-06 02:03:16.000000 evox-0.1.0/src/evox/utils.py
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.892022 evox-0.1.0/src/evox.egg-info/
--rw-r--r--   0 bill      (1000) users      (100)     4801 2023-06-06 13:16:17.000000 evox-0.1.0/src/evox.egg-info/PKG-INFO
--rw-r--r--   0 bill      (1000) users      (100)     3175 2023-06-06 13:16:17.000000 evox-0.1.0/src/evox.egg-info/SOURCES.txt
--rw-r--r--   0 bill      (1000) users      (100)        1 2023-06-06 13:16:17.000000 evox-0.1.0/src/evox.egg-info/dependency_links.txt
--rw-r--r--   0 bill      (1000) users      (100)      255 2023-06-06 13:16:17.000000 evox-0.1.0/src/evox.egg-info/requires.txt
--rw-r--r--   0 bill      (1000) users      (100)        5 2023-06-06 13:16:17.000000 evox-0.1.0/src/evox.egg-info/top_level.txt
-drwxr-xr-x   0 bill      (1000) users      (100)        0 2023-06-06 13:16:17.900022 evox-0.1.0/tests/
--rw-r--r--   0 bill      (1000) users      (100)     1699 2023-02-02 12:57:14.000000 evox-0.1.0/tests/test_classic_problems.py
--rw-r--r--   0 bill      (1000) users      (100)     5036 2023-04-04 08:37:26.000000 evox-0.1.0/tests/test_containers.py
--rw-r--r--   0 bill      (1000) users      (100)     3649 2022-10-21 09:22:33.000000 evox-0.1.0/tests/test_crowding_distance.py
--rw-r--r--   0 bill      (1000) users      (100)     1072 2023-01-31 15:16:22.000000 evox-0.1.0/tests/test_distributed_pipeline.py
--rw-r--r--   0 bill      (1000) users      (100)     1855 2023-01-31 15:16:48.000000 evox-0.1.0/tests/test_gym.py
--rw-r--r--   0 bill      (1000) users      (100)     1004 2023-02-02 13:09:47.000000 evox-0.1.0/tests/test_ibea.py
--rw-r--r--   0 bill      (1000) users      (100)      929 2023-02-02 13:14:09.000000 evox-0.1.0/tests/test_moead.py
--rw-r--r--   0 bill      (1000) users      (100)     3464 2023-01-31 04:52:29.000000 evox-0.1.0/tests/test_neuroevolution.py
--rw-r--r--   0 bill      (1000) users      (100)      556 2022-10-21 09:22:33.000000 evox-0.1.0/tests/test_non_dominated_sort.py
--rw-r--r--   0 bill      (1000) users      (100)     1017 2023-02-02 13:14:28.000000 evox-0.1.0/tests/test_nsga2.py
--rw-r--r--   0 bill      (1000) users      (100)      914 2023-02-02 13:14:16.000000 evox-0.1.0/tests/test_rvea.py
--rw-r--r--   0 bill      (1000) users      (100)     3029 2023-02-02 13:08:59.000000 evox-0.1.0/tests/test_single_objective_algorithms.py
--rw-r--r--   0 bill      (1000) users      (100)     2766 2023-03-06 02:25:38.000000 evox-0.1.0/tests/test_state.py
--rw-r--r--   0 bill      (1000) users      (100)     1016 2022-10-21 09:22:33.000000 evox-0.1.0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.348936 evox-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1546 2023-06-13 07:04:09.000000 evox-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-13 07:04:20.348936 evox-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2302 2023-06-13 07:04:09.000000 evox-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1165 2023-06-13 07:04:09.000000 evox-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:04:20.348936 evox-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.324936 evox-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.328935 evox-0.2.0/src/evox/
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.328935 evox-0.2.0/src/evox/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.332936 evox-0.2.0/src/evox/algorithms/containers/
+-rw-r--r--   0 runner    (1001) docker     (123)      173 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/containers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5518 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/containers/clustered_algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7625 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/containers/coevolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/containers/tree_algorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.332936 evox-0.2.0/src/evox/algorithms/mo/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/mo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3388 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/mo/ibea.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6247 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/mo/moead.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/mo/nsga2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4270 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/mo/rvea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.332936 evox-0.2.0/src/evox/algorithms/so/
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/cma_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/cso.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4989 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/de.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6758 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/nes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/open_es.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3927 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/pgpe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/pso.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/algorithms/so/sort_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.336936 evox-0.2.0/src/evox/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/core/algorithm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/core/module.py
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/core/operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      600 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/core/problem.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7168 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/core/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.336936 evox-0.2.0/src/evox/metrics/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/metrics/hypervolume.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/metrics/igd.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.336936 evox-0.2.0/src/evox/monitors/
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/monitors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/monitors/fitness.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4788 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/monitors/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/monitors/population.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/monitors/std_mo_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3351 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/monitors/std_so_monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.336936 evox-0.2.0/src/evox/operators/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.336936 evox-0.2.0/src/evox/operators/crossover/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/crossover/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1492 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/crossover/differential_evolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/crossover/one_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/crossover/sbx.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/crossover/simulated_binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/crossover/uniform.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1876 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/crowding_distance_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.340936 evox-0.2.0/src/evox/operators/mutation/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/mutation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/mutation/bitflip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/mutation/gaussian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/mutation/pm_mutation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/non_dominated_sort.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.340936 evox-0.2.0/src/evox/operators/sampling/
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/sampling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/sampling/latin_hypercude.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/sampling/uniform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.340936 evox-0.2.0/src/evox/operators/selection/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/selection/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1917 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/selection/rvea_selection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1579 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/selection/tournament.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/operators/selection/uniform_random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.340936 evox-0.2.0/src/evox/pipelines/
+-rw-r--r--   0 runner    (1001) docker     (123)      430 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/pipelines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8085 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/pipelines/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1312 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/pipelines/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5249 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/pipelines/multidevice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1511 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/pipelines/standard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.340936 evox-0.2.0/src/evox/problems/
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.344936 evox-0.2.0/src/evox/problems/classic/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/ackley.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10161 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/dtlz.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/griewank.py
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/rastrigin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      331 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/rosenbrock.py
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/sphere.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/classic/zdt.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.344936 evox-0.2.0/src/evox/problems/neuroevolution/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/neuroevolution/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11631 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/neuroevolution/torchvision_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.344936 evox-0.2.0/src/evox/problems/rl/
+-rw-r--r--   0 runner    (1001) docker     (123)      543 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/rl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3427 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/rl/brax.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12332 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/rl/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11621 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/problems/rl/gym_mo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5106 2023-06-13 07:04:09.000000 evox-0.2.0/src/evox/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.328935 evox-0.2.0/src/evox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4801 2023-06-13 07:04:20.000000 evox-0.2.0/src/evox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3199 2023-06-13 07:04:20.000000 evox-0.2.0/src/evox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:04:20.000000 evox-0.2.0/src/evox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      242 2023-06-13 07:04:20.000000 evox-0.2.0/src/evox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 07:04:20.000000 evox-0.2.0/src/evox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:04:20.348936 evox-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_classic_problems.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5009 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_containers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3649 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_crowding_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_distributed_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2560 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_monitors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_multi_objective_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_neuroevolution.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_non_dominated_sort.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_single_objective_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-13 07:04:09.000000 evox-0.2.0/tests/test_utils.py
```

### Comparing `evox-0.1.0/LICENSE` & `evox-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/PKG-INFO` & `evox-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evox
-Version: 0.1.0
+Version: 0.2.0
 Summary: evox
 Author-email: Bill Huang <bill.huang2001@gmail.com>, Christina Lee <1315552992@qq.com>, Zhenyu Liang <zhenyuliang97@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, EMI-Group
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evox Version: 0.1.0 Summary: evox Author-email:
+Metadata-Version: 2.1 Name: evox Version: 0.2.0 Summary: evox Author-email:
 Bill Huang
 huang2001@gmail.com>, Christina Lee <1315552992@qq.com>, Zhenyu Liang
 gmail.com> License: BSD 3-Clause License Copyright (c) 2022, EMI-Group All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
```

### Comparing `evox-0.1.0/README.md` & `evox-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/pyproject.toml` & `evox-0.2.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "evox"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
   { name = "Bill Huang", email = "bill.huang2001@gmail.com" },
   { name = "Christina Lee", email = "1315552992@qq.com" },
   { name = "Zhenyu Liang", email = "zhenyuliang97@gmail.com" },
 ]
 description = "evox"
 readme = "README.md"
@@ -21,15 +21,14 @@
   "Topic :: Scientific/Engineering :: Artificial Intelligence",
 ]
 
 dependencies = [
   "jax >= 0.3.0",
   "jaxlib >= 0.3.0",
   "optax >= 0.1.0",
-  "bokeh >= 2.4.0",
 ]
 
 [project.optional-dependencies]
 test = [
   "chex >= 0.1.0",
   "flax >= 0.5.0",
   "pytest >= 6.0.0",
```

### Comparing `evox-0.1.0/src/evox/algorithms/containers/clustered_algorithm.py` & `evox-0.2.0/src/evox/algorithms/containers/clustered_algorithm.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/algorithms/containers/coevolution.py` & `evox-0.2.0/src/evox/algorithms/containers/coevolution.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/algorithms/containers/tree_algorithm.py` & `evox-0.2.0/src/evox/algorithms/containers/tree_algorithm.py`

 * *Files 5% similar despite different names*

```diff
@@ -39,18 +39,7 @@
         return self.flatten_param.unflatten(params), state
 
     def tell(self, state, fitness):
         for inner_self in self.inner:
             state = self._base_algorithm.tell(inner_self, state, fitness)
 
         return state
-
-
-class TreeCC(Algorithm):
-    def __init__(self) -> None:
-        super().__init__()
-
-    def ask(self, state):
-        pass
-
-    def tell(self, state):
-        pass
```

### Comparing `evox-0.1.0/src/evox/algorithms/mo/ibea.py` & `evox-0.2.0/src/evox/algorithms/mo/ibea.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/algorithms/mo/moead.py` & `evox-0.2.0/src/evox/algorithms/mo/moead.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/algorithms/mo/nsga2.py` & `evox-0.2.0/src/evox/algorithms/mo/nsga2.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/algorithms/mo/rvea.py` & `evox-0.2.0/src/evox/algorithms/mo/rvea.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/algorithms/so/cma_es.py` & `evox-0.2.0/src/evox/algorithms/so/cma_es.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/algorithms/so/cso.py` & `evox-0.2.0/src/evox/algorithms/so/cso.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/algorithms/so/de.py` & `evox-0.2.0/src/evox/algorithms/so/de.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/algorithms/so/nes.py` & `evox-0.2.0/src/evox/algorithms/so/nes.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/algorithms/so/open_es.py` & `evox-0.2.0/src/evox/algorithms/so/open_es.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/algorithms/so/pgpe.py` & `evox-0.2.0/src/evox/algorithms/so/pgpe.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/algorithms/so/pso.py` & `evox-0.2.0/src/evox/algorithms/so/pso.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/core/algorithm.py` & `evox-0.2.0/src/evox/core/algorithm.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/core/module.py` & `evox-0.2.0/src/evox/core/module.py`

 * *Files 12% similar despite different names*

```diff
@@ -189,26 +189,35 @@
             warnings.warn(
                 "Trying to re-initialize a Stateful module that is already initialized"
             )
 
         self._node_id = node_id
 
         child_states = {}
+
+        # Find all submodules and sort them according to their name.
+        # Sorting is important because it makes sure that the node_id
+        # is deterministic across different runs.
+        submodules = []
         for attr_name in vars(self):
             attr = getattr(self, attr_name)
             if not attr_name.startswith("_") and isinstance(attr, Stateful):
-                if key is None:
-                    subkey = None
-                else:
-                    key, subkey = jax.random.split(key)
-                submodule_state, node_id = attr._recursive_init(subkey, node_id + 1)
-                assert isinstance(
-                    submodule_state, State
-                ), "setup method must return a State"
-                child_states[attr_name] = submodule_state
+                submodules.append((attr_name, attr))
+        submodules.sort()
+
+        for attr_name, attr in submodules:
+            if key is None:
+                subkey = None
+            else:
+                key, subkey = jax.random.split(key)
+            submodule_state, node_id = attr._recursive_init(subkey, node_id + 1)
+            assert isinstance(
+                submodule_state, State
+            ), "setup method must return a State"
+            child_states[attr_name] = submodule_state
 
         return (
             self.setup(key)
             ._set_state_id_mut(self._node_id)
             ._set_child_states_mut(child_states),
             node_id,
         )
```

### Comparing `evox-0.1.0/src/evox/core/problem.py` & `evox-0.2.0/src/evox/core/problem.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/core/state.py` & `evox-0.2.0/src/evox/core/state.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/metrics/hypervolume.py` & `evox-0.2.0/src/evox/metrics/hypervolume.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/monitors/gym.py` & `evox-0.2.0/src/evox/monitors/gym.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,70 @@
 import jax.numpy as jnp
 from evox.core.module import Stateful
 from evox.operators import non_dominated_sort, crowding_distance_sort
-import bokeh
-from bokeh.plotting import figure, show
-from bokeh.models import Spinner
 import time
 import os
 
+
 def initialize_log_dir(log_dir, env_name, mo=False, monitor_info=None):
     if log_dir is None:
-        current_time = time.strftime('%Y_%m_%d_%H_%M_%S', time.localtime(time.time()))
-        log_dir = os.path.join('logs')
+        current_time = time.strftime("%Y_%m_%d_%H_%M_%S", time.localtime(time.time()))
+        log_dir = os.path.join("logs")
         if env_name is not None:
             log_dir = os.path.join(log_dir, env_name)
         if monitor_info is not None:
             log_dir = os.path.join(log_dir, str(monitor_info))
         if mo:
-            log_dir = os.path.join(log_dir, 'mo')
-        
+            log_dir = os.path.join(log_dir, "mo")
+
         log_dir = os.path.join(log_dir, current_time)
 
     if not os.path.exists(log_dir):
         os.makedirs(log_dir)
     return log_dir
 
+
 def file_print(log_file, s):
-    with open(log_file, 'a+') as f:
+    with open(log_file, "a+") as f:
         print(s, file=f)
 
+
 class GymMonitor:
-    def __init__(self, need_save=True, log_dir=None, save_interval=50, env_name=None, mo_keys=None, monitor_info=None):
+    def __init__(
+        self,
+        need_save=True,
+        log_dir=None,
+        save_interval=50,
+        env_name=None,
+        mo_keys=None,
+        monitor_info=None,
+    ):
         self.iteration = 0
         self.need_save = need_save
         self.mo_keys = mo_keys
         if mo_keys is None:
             self.global_min_fitness = float("inf")
             if need_save:
-                self.log_dir = initialize_log_dir(log_dir, env_name, monitor_info=monitor_info)
+                self.log_dir = initialize_log_dir(
+                    log_dir, env_name, monitor_info=monitor_info
+                )
                 print(f"use {self.log_dir} as log directory.")
                 self.save_interval = save_interval
                 self.log_file = os.path.join(self.log_dir, "log.txt")
             else:
                 print(f"do not save models")
         else:
             if need_save:
                 self.log_dir = initialize_log_dir(log_dir, env_name, mo=True)
                 print(f"use {self.log_dir} as log directory.")
                 self.save_interval = save_interval
                 self.log_file = os.path.join(self.log_dir, "log.txt")
             else:
                 print(f"do not save models")
-        
+
     def update(self, state, problem, pop, fitness):
         self.iteration += 1
         if self.mo_keys is None:
             avg_fitness = jnp.average(fitness)
             min_index = jnp.argmin(fitness)
             min_fitness = fitness[min_index]
             max_fitness = jnp.max(fitness)
@@ -63,41 +73,55 @@
 
             if min_fitness < self.global_min_fitness:
                 self.global_min_fitness = min_fitness
                 if self.need_save:
                     self.save_agent("best_agent.npy", best_agent)
 
             if self.need_save:
-                file_print(self.log_file, f"it: {self.iteration}, min: {min_fitness}, max: {max_fitness}, mean: {avg_fitness}, var: {var_}, global_min: {self.global_min_fitness}")
+                file_print(
+                    self.log_file,
+                    f"it: {self.iteration}, min: {min_fitness}, max: {max_fitness}, mean: {avg_fitness}, var: {var_}, global_min: {self.global_min_fitness}",
+                )
 
                 if self.iteration % self.save_interval == 0:
                     self.save_agent(f"best_iteration{self.iteration}", best_agent)
-                
-            print(f"iteration: {self.iteration}, min_fitness {min_fitness}, avg_fitness: {avg_fitness}")
+
+            print(
+                f"iteration: {self.iteration}, min_fitness {min_fitness}, avg_fitness: {avg_fitness}"
+            )
         else:
             sum_fitness = jnp.asarray([jnp.sum(f) for f in fitness])
             min_fitness = jnp.min(sum_fitness)
             max_fitness = jnp.max(sum_fitness)
             avg_fitness = jnp.average(sum_fitness)
             var_ = jnp.var(sum_fitness)
             non_dominated_rank = non_dominated_sort(fitness)
             print(fitness)
             print(non_dominated_rank)
 
             pareto_front = non_dominated_rank == 0
             if self.need_save:
                 if self.iteration % self.save_interval == 0:
-                    new_folder_path = os.path.join(self.log_dir, f"iteration{self.iteration}")
+                    new_folder_path = os.path.join(
+                        self.log_dir, f"iteration{self.iteration}"
+                    )
                     os.makedirs(new_folder_path, exist_ok=True)
                     for idx, value in enumerate(pareto_front):
                         if value:
                             file_name = os.path.join(new_folder_path, f"agent{idx}.npy")
                             jnp.save(file_name, pop[idx])
-                    file_print(os.path.join(new_folder_path, "fitness.txt"), f"fitness: {fitness}, non_dominated_rank: {non_dominated_rank}")
-            
-            print(f"iteration: {self.iteration}, min_fitness {min_fitness}, avg_fitness: {avg_fitness}")
-            file_print(self.log_file, f"it: {self.iteration}, min: {min_fitness}, max: {max_fitness}, mean: {avg_fitness}, var: {var_}")
-
+                    file_print(
+                        os.path.join(new_folder_path, "fitness.txt"),
+                        f"fitness: {fitness}, non_dominated_rank: {non_dominated_rank}",
+                    )
+
+            print(
+                f"iteration: {self.iteration}, min_fitness {min_fitness}, avg_fitness: {avg_fitness}"
+            )
+            file_print(
+                self.log_file,
+                f"it: {self.iteration}, min: {min_fitness}, max: {max_fitness}, mean: {avg_fitness}, var: {var_}",
+            )
 
     def save_agent(self, name, agent):
         file_name = os.path.join(self.log_dir, name)
-        jnp.save(file_name, agent)
+        jnp.save(file_name, agent)
```

### Comparing `evox-0.1.0/src/evox/operators/crossover/differential_evolution.py` & `evox-0.2.0/src/evox/operators/crossover/differential_evolution.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/operators/crossover/one_point.py` & `evox-0.2.0/src/evox/operators/crossover/one_point.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/operators/crossover/sbx.py` & `evox-0.2.0/src/evox/operators/crossover/sbx.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/operators/crossover/simulated_binary.py` & `evox-0.2.0/src/evox/operators/crossover/simulated_binary.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/operators/crossover/uniform.py` & `evox-0.2.0/src/evox/operators/crossover/uniform.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/operators/crowding_distance_sort.py` & `evox-0.2.0/src/evox/operators/crowding_distance_sort.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/operators/mutation/bitflip.py` & `evox-0.2.0/src/evox/operators/mutation/bitflip.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/operators/mutation/pm_mutation.py` & `evox-0.2.0/src/evox/operators/mutation/pm_mutation.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/operators/sampling/latin_hypercude.py` & `evox-0.2.0/src/evox/operators/sampling/latin_hypercude.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/operators/sampling/uniform.py` & `evox-0.2.0/src/evox/operators/sampling/uniform.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/operators/selection/rvea_selection.py` & `evox-0.2.0/src/evox/operators/selection/rvea_selection.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/operators/selection/tournament.py` & `evox-0.2.0/src/evox/operators/selection/tournament.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/pipelines/distributed.py` & `evox-0.2.0/src/evox/pipelines/distributed.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import jax
 import jax.numpy as jnp
 import numpy as np
 import ray
 from jax.tree_util import tree_flatten
 
 from evox import Algorithm, Problem, State, Stateful
-from evox.monitors import FitnessMonitor, PopulationMonitor
 
 
 class WorkerPipeline(Stateful):
     def __init__(
         self,
         algorithm: Algorithm,
         problem: Problem,
@@ -64,19 +63,15 @@
 
     def sample(self, state: State):
         return self.algorithm.ask(state)
 
 
 @ray.remote
 class Worker:
-    def __init__(
-        self,
-        pipeline: WorkerPipeline,
-        worker_index: int
-    ):
+    def __init__(self, pipeline: WorkerPipeline, worker_index: int):
         self.pipeline = pipeline
         self.worker_index = worker_index
 
     def init(self, key: jax.Array):
         self.state = self.pipeline.init(key)
         self.initialized = True
```

### Comparing `evox-0.1.0/src/evox/pipelines/gym.py` & `evox-0.2.0/src/evox/pipelines/gym.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/pipelines/multidevice.py` & `evox-0.2.0/src/evox/pipelines/multidevice.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from typing import Callable, Optional, Tuple
 from functools import partial
 
 import jax
 import jax.numpy as jnp
 from jax import pmap
 
-from evox import Algorithm, Problem, State, Stateful, jit_method
-from evox.monitors import FitnessMonitor, PopulationMonitor
+from evox import Algorithm, Problem, State, Stateful
 
 
 class MultiDevicePipeline(Stateful):
     def __init__(
         self,
         algorithm: Algorithm,
         problem: Problem,
@@ -119,25 +118,26 @@
 
         return state.update(
             alg_states=alg_states,
             pro_states=pro_states,
         )
 
     def valid(self, state: State, metric: str = "loss") -> Tuple[jax.Array, State]:
-        new_pro_state = pmap(partial(self.problem.valid, metric=metric))(state.pro_states)
+        new_pro_state = pmap(partial(self.problem.valid, metric=metric))(
+            state.pro_states
+        )
         pop, new_state = self.pmap_alg_ask(new_state)
         if self.pop_transform is not None:
             pop = self.pop_transform(pop)
 
         new_state, fitness = self.pmap_pro_eval(new_pro_state, pop)
         return fitness, state
 
     def sample(self, state: State):
-        """Sample the algorithm but don't change it's state
-        """
+        """Sample the algorithm but don't change it's state"""
         sample_pop, state_ = self.pmap_alg_ask(state)
         if self.pop_transform is not None:
             sample_pop = self.pop_transform(sample_pop)
 
         # we have N copies of the population
         # just take one
         sample_pop = sample_pop[0]
```

### Comparing `evox-0.1.0/src/evox/pipelines/standard.py` & `evox-0.2.0/src/evox/pipelines/standard.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from evox import Stateful
 from evox import Algorithm, Problem
-from evox.monitors import FitnessMonitor, PopulationMonitor
 from typing import Optional, Callable
 
 
 class StdPipeline(Stateful):
     def __init__(
         self,
         algorithm: Algorithm,
         problem: Problem,
         pop_transform: Optional[Callable] = None,
-        fitness_transform: Optional[Callable] = None):
+        fitness_transform: Optional[Callable] = None,
+    ):
         self.algorithm = algorithm
         self.problem = problem
         self.pop_transform = pop_transform
         self.fitness_transform = fitness_transform
 
     def step(self, state):
         pop, state = self.algorithm.ask(state)
@@ -36,14 +36,13 @@
         if self.pop_transform is not None:
             pop = self.pop_transform(pop)
 
         new_state, fitness = self.problem.evaluate(new_state, pop)
         return fitness, state
 
     def sample(self, state):
-        """Sample the algorithm but don't change it's state
-        """
+        """Sample the algorithm but don't change it's state"""
         sample_pop, state_ = self.algorithm.ask(state)
         if self.pop_transform is not None:
             sample_pop = self.pop_transform(sample_pop)
 
         return sample_pop, state
```

### Comparing `evox-0.1.0/src/evox/problems/classic/ackley.py` & `evox-0.2.0/src/evox/problems/classic/ackley.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/problems/classic/dtlz.py` & `evox-0.2.0/src/evox/problems/classic/dtlz.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/problems/classic/zdt.py` & `evox-0.2.0/src/evox/problems/classic/zdt.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/problems/neuroevolution/torchvision_dataset.py` & `evox-0.2.0/src/evox/problems/neuroevolution/torchvision_dataset.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/problems/rl/__init__.py` & `evox-0.2.0/src/evox/problems/rl/__init__.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/problems/rl/brax.py` & `evox-0.2.0/src/evox/problems/rl/brax.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/problems/rl/gym.py` & `evox-0.2.0/src/evox/problems/rl/gym.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/problems/rl/gym_mo.py` & `evox-0.2.0/src/evox/problems/rl/gym_mo.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox/utils.py` & `evox-0.2.0/src/evox/utils.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/src/evox.egg-info/PKG-INFO` & `evox-0.2.0/src/evox.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evox
-Version: 0.1.0
+Version: 0.2.0
 Summary: evox
 Author-email: Bill Huang <bill.huang2001@gmail.com>, Christina Lee <1315552992@qq.com>, Zhenyu Liang <zhenyuliang97@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2022, EMI-Group
         All rights reserved.
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: evox Version: 0.1.0 Summary: evox Author-email:
+Metadata-Version: 2.1 Name: evox Version: 0.2.0 Summary: evox Author-email:
 Bill Huang
 huang2001@gmail.com>, Christina Lee <1315552992@qq.com>, Zhenyu Liang
 gmail.com> License: BSD 3-Clause License Copyright (c) 2022, EMI-Group All
 rights reserved. Redistribution and use in source and binary forms, with or
 without modification, are permitted provided that the following conditions are
 met: 1. Redistributions of source code must retain the above copyright notice,
 this list of conditions and the following disclaimer. 2. Redistributions in
```

### Comparing `evox-0.1.0/src/evox.egg-info/SOURCES.txt` & `evox-0.2.0/src/evox.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -35,14 +35,16 @@
 src/evox/metrics/__init__.py
 src/evox/metrics/hypervolume.py
 src/evox/metrics/igd.py
 src/evox/monitors/__init__.py
 src/evox/monitors/fitness.py
 src/evox/monitors/gym.py
 src/evox/monitors/population.py
+src/evox/monitors/std_mo_monitor.py
+src/evox/monitors/std_so_monitor.py
 src/evox/operators/__init__.py
 src/evox/operators/crowding_distance_sort.py
 src/evox/operators/non_dominated_sort.py
 src/evox/operators/crossover/__init__.py
 src/evox/operators/crossover/differential_evolution.py
 src/evox/operators/crossover/one_point.py
 src/evox/operators/crossover/sbx.py
@@ -75,22 +77,19 @@
 src/evox/problems/classic/zdt.py
 src/evox/problems/neuroevolution/__init__.py
 src/evox/problems/neuroevolution/torchvision_dataset.py
 src/evox/problems/rl/__init__.py
 src/evox/problems/rl/brax.py
 src/evox/problems/rl/gym.py
 src/evox/problems/rl/gym_mo.py
-src/evox/problems/rl/gymnasium.py
 tests/test_classic_problems.py
 tests/test_containers.py
 tests/test_crowding_distance.py
 tests/test_distributed_pipeline.py
 tests/test_gym.py
-tests/test_ibea.py
-tests/test_moead.py
+tests/test_monitors.py
+tests/test_multi_objective_algorithms.py
 tests/test_neuroevolution.py
 tests/test_non_dominated_sort.py
-tests/test_nsga2.py
-tests/test_rvea.py
 tests/test_single_objective_algorithms.py
 tests/test_state.py
 tests/test_utils.py
```

### Comparing `evox-0.1.0/tests/test_classic_problems.py` & `evox-0.2.0/tests/test_classic_problems.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/tests/test_containers.py` & `evox-0.2.0/tests/test_containers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,29 @@
-import evox as ex
 import jax
 import jax.numpy as jnp
 import pytest
 from evox import algorithms, pipelines, problems
-from evox.monitors import FitnessMonitor
-import chex
+from evox.monitors import StdSOMonitor
 
 
 @pytest.mark.skip(
     reason="a bit non-deterministic now, maybe due to the fact that eigen decomposition is unstable"
 )
 def test_clustered_cma_es():
     # create a pipeline
     init_mean = jnp.full((10,), fill_value=-20)
-    monitor = FitnessMonitor()
+    monitor = StdSOMonitor()
     pipeline = pipelines.StdPipeline(
         algorithms.ClusterdAlgorithm(
             base_algorithm=algorithms.CMAES(init_mean, init_stdev=10, pop_size=10),
             dim=40,
             num_cluster=4,
         ),
         problem=problems.classic.Ackley(),
-        fitness_transform=monitor.update,
+        fitness_transform=monitor.record_fit,
     )
     # init the pipeline
     key = jax.random.PRNGKey(42)
     state = pipeline.init(key)
 
     # run the pipeline for 10 steps
     for i in range(200):
@@ -34,29 +32,29 @@
     min_fitness = monitor.get_min_fitness()
     assert min_fitness < 2
 
 
 @pytest.mark.parametrize("random_subpop", [True, False])
 def test_vectorized_coevolution(random_subpop):
     # create a pipeline
-    monitor = FitnessMonitor()
+    monitor = StdSOMonitor()
     algorithm = algorithms.VectorizedCoevolution(
         base_algorithm=algorithms.CSO(
             lb=jnp.full(shape=(20,), fill_value=-32),
             ub=jnp.full(shape=(20,), fill_value=32),
             pop_size=30,
         ),
         dim=40,
         num_subpops=2,
         random_subpop=random_subpop,
     )
     pipeline = pipelines.StdPipeline(
         algorithm,
         problem=problems.classic.Ackley(),
-        fitness_transform=monitor.update,
+        fitness_transform=monitor.record_fit,
     )
     # init the pipeline
     key = jax.random.PRNGKey(42)
     state = pipeline.init(key)
 
     if not random_subpop:
         # test the population given by VectorizedCoevolution
@@ -98,30 +96,30 @@
 
 
 @pytest.mark.parametrize(
     "random_subpop, num_subpop_iter", [(True, 1), (False, 1), (True, 2), (False, 2)]
 )
 def test_coevolution(random_subpop, num_subpop_iter):
     # create a pipeline
-    monitor = FitnessMonitor()
+    monitor = StdSOMonitor()
     pipeline = pipelines.StdPipeline(
         algorithms.Coevolution(
             base_algorithm=algorithms.CSO(
                 lb=jnp.full(shape=(10,), fill_value=-32),
                 ub=jnp.full(shape=(10,), fill_value=32),
                 pop_size=20,
             ),
             dim=40,
             num_subpops=4,
             subpop_size=10,
             num_subpop_iter=num_subpop_iter,
             random_subpop=random_subpop,
         ),
         problem=problems.classic.Ackley(),
-        fitness_transform=monitor.update,
+        fitness_transform=monitor.record_fit,
     )
     # init the pipeline
     key = jax.random.PRNGKey(42)
     state = pipeline.init(key)
 
     for i in range(4 * 200):
         state = pipeline.step(state)
@@ -129,30 +127,30 @@
     min_fitness = monitor.get_min_fitness()
     assert min_fitness < 2
 
 
 @pytest.mark.skip(reason="currently random_mask is unstable")
 def test_random_mask_cso():
     # create a pipeline
-    monitor = FitnessMonitor()
+    monitor = StdSOMonitor()
     pipeline = pipelines.StdPipeline(
         algorithms.RandomMaskAlgorithm(
-            base_algorithm=ex.algorithms.CSO(
+            base_algorithm=algorithms.CSO(
                 lb=jnp.full(shape=(10,), fill_value=-32),
                 ub=jnp.full(shape=(10,), fill_value=32),
                 pop_size=100,
             ),
             dim=40,
             num_cluster=4,
             num_mask=2,
             change_every=10,
             pop_size=50,
         ),
         problem=problems.classic.Ackley(),
-        fitness_transform=monitor.update,
+        fitness_transform=monitor.record_fit,
     )
     # init the pipeline
     key = jax.random.PRNGKey(42)
     state = pipeline.init(key)
 
     # run the pipeline for 10 steps
     for i in range(10):
```

### Comparing `evox-0.1.0/tests/test_crowding_distance.py` & `evox-0.2.0/tests/test_crowding_distance.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/tests/test_distributed_pipeline.py` & `evox-0.2.0/tests/test_distributed_pipeline.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 import evox as ex
 from evox import pipelines, algorithms, problems
-from evox.monitors import FitnessMonitor
+from evox.monitors import StdSOMonitor
 import jax
 import jax.numpy as jnp
 import pytest
 
 
 def test_distributed_cso():
-    monitor = FitnessMonitor()
+    monitor = StdSOMonitor()
     # create a pipeline
     pipeline = pipelines.DistributedPipeline(
         algorithm=algorithms.CSO(
             lb=jnp.full(shape=(2,), fill_value=-32),
             ub=jnp.full(shape=(2,), fill_value=32),
             pop_size=20,
         ),
         problem=problems.classic.Ackley(),
         pop_size=10,
         num_workers=2,
-        global_fitness_transform=monitor.update,
-        options={
-            "num_cpus": 0.5, # just for testing purpose
-            "num_gpus": 0
-        }
+        global_fitness_transform=monitor.record_fit,
+        options={"num_cpus": 0.5, "num_gpus": 0},  # just for testing purpose
     )
     # init the pipeline
     key = jax.random.PRNGKey(42)
     state = pipeline.init(key)
 
     # run the pipeline for 100 steps
     for i in range(100):
```

### Comparing `evox-0.1.0/tests/test_gym.py` & `evox-0.2.0/tests/test_gym.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import evox as ex
 from evox import pipelines, algorithms, problems
-from evox.monitors import FitnessMonitor
+from evox.monitors import StdSOMonitor
 from evox.utils import TreeAndVector
 import jax
 import jax.numpy as jnp
 from flax import linen as nn
 import pytest
 
 
@@ -24,16 +24,16 @@
 def test_cartpole(batch_policy):
     key = jax.random.PRNGKey(42)
     model_key, pipeline_key = jax.random.split(key)
 
     model = CartpolePolicy()
     params = model.init(model_key, jnp.zeros((4,)))
     adapter = TreeAndVector(params)
-    monitor = FitnessMonitor()
-    problem = problems.neuroevolution.Gym(
+    monitor = StdSOMonitor()
+    problem = problems.rl.Gym(
         policy=jax.jit(model.apply),
         num_workers=4,
         env_per_worker=10,
         controller_options={
             "num_cpus": 0.25,
             "num_gpus": 0,
         },
@@ -46,15 +46,15 @@
         algorithm=algorithms.PGPE(
             optimizer="adam",
             center_init=center,
             pop_size=40,
         ),
         problem=problem,
         pop_transform=adapter.batched_to_tree,
-        fitness_transform=monitor.update,
+        fitness_transform=monitor.record_fit,
     )
     # init the pipeline
     state = pipeline.init(pipeline_key)
 
     # run the pipeline for 10 steps
     for i in range(10):
         print(monitor.get_min_fitness())
```

### Comparing `evox-0.1.0/tests/test_neuroevolution.py` & `evox-0.2.0/tests/test_neuroevolution.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,38 +2,37 @@
 
 import evox as ex
 import jax
 import jax.numpy as jnp
 import pytest
 from flax import linen as nn
 from evox import algorithms, pipelines, problems
-from evox.monitors import FitnessMonitor
-
+from evox.monitors import StdSOMonitor
 
 
 class PartialPGPE(ex.algorithms.PGPE):
     def __init__(self, center_init):
         super().__init__(
             100, center_init, "adam", center_learning_rate=0.01, stdev_init=0.01
         )
 
 
 class SimpleCNN(nn.Module):
     """A simple CNN model."""
 
     @nn.compact
     def __call__(self, x):
-        x = nn.Conv(features=6, kernel_size=(3, 3), padding='SAME')(x)
+        x = nn.Conv(features=6, kernel_size=(3, 3), padding="SAME")(x)
         x = nn.relu(x)
-        x = nn.Conv(features=16, kernel_size=(3, 3), padding='SAME')(x)
+        x = nn.Conv(features=16, kernel_size=(3, 3), padding="SAME")(x)
         x = nn.relu(x)
         x = nn.max_pool(x, window_shape=(2, 2), strides=(2, 2))
-        x = nn.Conv(features=16, kernel_size=(3, 3), padding='SAME')(x)
+        x = nn.Conv(features=16, kernel_size=(3, 3), padding="SAME")(x)
         x = nn.relu(x)
-        x = nn.Conv(features=16, kernel_size=(3, 3), padding='SAME')(x)
+        x = nn.Conv(features=16, kernel_size=(3, 3), padding="SAME")(x)
         x = nn.relu(x)
         x = nn.max_pool(x, window_shape=(2, 2), strides=(2, 2))
 
         x = x.reshape(x.shape[0], -1)
         x = nn.Dense(120)(x)
         x = nn.sigmoid(x)
         x = nn.Dense(10)(x)
@@ -41,15 +40,18 @@
 
 
 def init_problem_and_model(key):
     model = SimpleCNN()
     batch_size = 64
     initial_params = model.init(key, jnp.zeros((batch_size, 32, 32, 3)))
     problem = ex.problems.neuroevolution.TorchvisionDataset(
-        root="./datasets", batch_size=batch_size, forward_func=model.apply, dataset_name="cifar10"
+        root="./datasets",
+        batch_size=batch_size,
+        forward_func=model.apply,
+        dataset_name="cifar10",
     )
     return initial_params, problem
 
 
 @pytest.mark.skip(reason="time consuming")
 def test_neuroevolution_treemap():
     key = jax.random.PRNGKey(42)
@@ -58,19 +60,19 @@
     initial_params, problem = init_problem_and_model(model_init_key)
 
     start = time.perf_counter()
     center_init = jax.tree_util.tree_map(
         lambda x: x.reshape(-1),
         initial_params,
     )
-    monitor = FitnessMonitor()
+    monitor = StdSOMonitor()
     pipeline = pipelines.StdPipeline(
         algorithm=ex.algorithms.TreeAlgorithm(PartialPGPE, initial_params, center_init),
         problem=problem,
-        fitness_transform=monitor.update,
+        fitness_transform=monitor.record_fit,
     )
     # init the pipeline
     state = pipeline.init(pipeline_key)
 
     # run the pipeline for 100 steps
     for i in range(100):
         state = pipeline.step(state)
@@ -84,27 +86,27 @@
 def test_neuroevolution_adapter():
     key = jax.random.PRNGKey(42)
     pipeline_key, model_init_key = jax.random.split(key)
     initial_params, problem = init_problem_and_model(model_init_key)
 
     start = time.perf_counter()
     adapter = ex.utils.TreeAndVector(initial_params)
-    monitor = FitnessMonitor()
+    monitor = StdSOMonitor()
     algorithm = algorithms.PGPE(
         100,
         adapter.to_vector(initial_params),
         "adam",
         center_learning_rate=0.01,
         stdev_init=0.01,
     )
     pipeline = pipelines.StdPipeline(
         algorithm=algorithm,
         problem=problem,
         pop_transform=adapter.batched_to_tree,
-        fitness_transform=monitor.update,
+        fitness_transform=monitor.record_fit,
     )
     # init the pipeline
     state = pipeline.init(key)
 
     # run the pipeline for 100 steps
     for i in range(100):
         state = pipeline.step(state)
```

### Comparing `evox-0.1.0/tests/test_non_dominated_sort.py` & `evox-0.2.0/tests/test_non_dominated_sort.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/tests/test_nsga2.py` & `evox-0.2.0/tests/test_multi_objective_algorithms.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,39 +1,66 @@
-import sys
-sys.path.append("../src")
-
 from evox import pipelines, algorithms, problems
-from evox.monitors import FitnessMonitor
-from evox.metrics import HyperVolume, IGD
+from evox.monitors import StdMOMonitor
+from evox.metrics import IGD
 import jax
 import jax.numpy as jnp
-import pytest
 
 
-def test_nsga2():
-    monitor = FitnessMonitor(n_objects=3)
-    key = jax.random.PRNGKey(1234)
-    problem=problems.classic.DTLZ1(m=3)
+def run_moea(algorithm, problem=problems.classic.DTLZ1(m=3)):
+    key = jax.random.PRNGKey(123)
+    monitor = StdMOMonitor(record_pf=False)
+    problem = problems.classic.DTLZ1(m=3)
     pipeline = pipelines.StdPipeline(
-        algorithm=algorithms.NSGA2(
-            lb=jnp.full(shape=(3,), fill_value=0),
-            ub=jnp.full(shape=(3,), fill_value=1),
-            n_objs=3,
-            pop_size=100,
-        ),
-        # problem=ex.problems.classic.ZDT1(n=2),
+        algorithm=algorithm,
         problem=problem,
-        fitness_transform=monitor.update
+        fitness_transform=monitor.record_fit,
     )
     state = pipeline.init(key)
-    pf, state = problem.pf(state=state)
+    true_pf, state = problem.pf(state)
 
-    for i in range(100):
+    for i in range(10):
         state = pipeline.step(state)
 
-        objs = monitor.get_last()
-        # print(objs)
-        igd = IGD(pf, objs).calulate()
-        print("step", i)
-        # print(t1-t0)
-        print("igd", igd)
+    objs = monitor.get_last()
+    igd = IGD(true_pf, objs).calulate()
+    print("igd", igd)
+
+
+def test_ibea():
+    algorithm = algorithms.IBEA(
+        lb=jnp.full(shape=(3,), fill_value=0),
+        ub=jnp.full(shape=(3,), fill_value=1),
+        n_objs=3,
+        pop_size=100,
+    )
+    run_moea(algorithm)
+
+
+def test_moead():
+    algorithm = algorithms.MOEAD(
+        lb=jnp.full(shape=(3,), fill_value=0),
+        ub=jnp.full(shape=(3,), fill_value=1),
+        n_objs=3,
+        pop_size=100,
+        type=1,
+    )
+    run_moea(algorithm)
+
 
+def test_nsga2():
+    algorithm = algorithms.NSGA2(
+        lb=jnp.full(shape=(3,), fill_value=0),
+        ub=jnp.full(shape=(3,), fill_value=1),
+        n_objs=3,
+        pop_size=100,
+    )
+    run_moea(algorithm)
+
+
+def test_rvea():
+    algorithm = algorithms.RVEA(
+        lb=jnp.full(shape=(3,), fill_value=0),
+        ub=jnp.full(shape=(3,), fill_value=1),
+        n_objs=3,
+        pop_size=100,
+    )
+    run_moea(algorithm)
```

### Comparing `evox-0.1.0/tests/test_single_objective_algorithms.py` & `evox-0.2.0/tests/test_single_objective_algorithms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import jax
 import jax.numpy as jnp
 import pytest
 from evox import pipelines, problems
 from evox.algorithms import CMAES, SepCMAES, CSO, DE, PGPE, PSO, OpenES, xNES
-from evox.monitors import FitnessMonitor
+from evox.monitors import StdSOMonitor
 from evox.utils import compose, rank_based_fitness
 
 
 def run_single_objective_algorithm(
     algorithm, problem=problems.classic.Sphere(), num_iter=200, fitness_shaping=False
 ):
     key = jax.random.PRNGKey(42)
-    monitor = FitnessMonitor(keep_global_best=True)
+    monitor = StdSOMonitor()
     if fitness_shaping is True:
-        fitness_transform = compose(monitor.update, rank_based_fitness)
+        fitness_transform = compose(monitor.record_fit, rank_based_fitness)
     else:
-        fitness_transform = monitor.update
+        fitness_transform = monitor.record_fit
 
     pipeline = pipelines.StdPipeline(
         algorithm=algorithm,
         problem=problem,
         fitness_transform=fitness_transform,
     )
 
@@ -34,26 +34,29 @@
 def test_cso():
     lb = jnp.full((5,), -32.0)
     ub = jnp.full((5,), 32.0)
     algorithm = CSO(lb, ub, 100)
     fitness = run_single_objective_algorithm(algorithm)
     assert fitness < 0.1
 
+
 def test_cma_es():
     init_mean = jnp.array([5.0, -10, 15, -20, 25])
     algorithm = CMAES(init_mean, init_stdev=0.1, pop_size=10)
     fitness = run_single_objective_algorithm(algorithm)
     assert fitness < 0.1
 
+
 def test_sep_cma_es():
     init_mean = jnp.array([5.0, -10, 15, -20, 25])
     algorithm = SepCMAES(init_mean, init_stdev=0.1, pop_size=10)
     fitness = run_single_objective_algorithm(algorithm)
     assert fitness < 0.1
 
+
 def test_pso():
     lb = jnp.full((5,), -32.0)
     ub = jnp.full((5,), 32.0)
     algorithm = PSO(lb, ub, 100)
     fitness = run_single_objective_algorithm(algorithm)
     assert fitness < 0.1
 
@@ -75,15 +78,20 @@
 
 
 @pytest.mark.parametrize("optimizer", ["adam", None])
 def test_openes(optimizer):
     init_mean = jnp.array([5.0, -10, 15, -20, 25])
 
     algorithm = OpenES(
-        init_mean, 100, learning_rate=1, noise_stdev=3, optimizer=optimizer, mirrored_sampling=True
+        init_mean,
+        100,
+        learning_rate=1,
+        noise_stdev=3,
+        optimizer=optimizer,
+        mirrored_sampling=True,
     )
     fitness = run_single_objective_algorithm(
         algorithm, fitness_shaping=True, num_iter=1000
     )
     assert fitness < 1
```

### Comparing `evox-0.1.0/tests/test_state.py` & `evox-0.2.0/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `evox-0.1.0/tests/test_utils.py` & `evox-0.2.0/tests/test_utils.py`

 * *Files identical despite different names*

