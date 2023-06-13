# Comparing `tmp/taskcluster-taskgraph-5.3.0.tar.gz` & `tmp/taskcluster-taskgraph-5.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/taskcluster-taskgraph-5.3.0.tar", last modified: Thu Jun  8 20:00:01 2023, max compression
+gzip compressed data, was "taskcluster-taskgraph-5.4.0.tar", last modified: Tue Jun 13 13:57:11 2023, max compression
```

## Comparing `taskcluster-taskgraph-5.3.0.tar` & `taskcluster-taskgraph-5.4.0.tar`

### file list

```diff
@@ -1,146 +1,146 @@
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/
--rw-r--r--   0 ahal      (1000) ahal      (1000)    16725 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/LICENSE
--rw-r--r--   0 ahal      (1000) ahal      (1000)      175 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/MANIFEST.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3659 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/README.rst
--rw-r--r--   0 ahal      (1000) ahal      (1000)      602 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.3.0/pyproject.toml
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/requirements/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      191 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/requirements/base.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)    20557 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/requirements/base.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       22 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/requirements/dev.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1281 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.3.0/requirements/dev.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       58 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.3.0/requirements/test.in
--rw-r--r--   0 ahal      (1000) ahal      (1000)     8476 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/requirements/test.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       38 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/setup.cfg
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1555 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/setup.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      665 2023-06-08 20:00:00.000000 taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3977 2023-06-08 20:00:00.000000 taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)        1 2023-06-08 20:00:00.000000 taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       50 2023-06-08 20:00:00.000000 taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)      215 2023-06-08 20:00:00.000000 taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/requires.txt
--rw-r--r--   0 ahal      (1000) ahal      (1000)       10 2023-06-08 20:00:00.000000 taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/top_level.txt
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      729 2023-06-08 19:59:10.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/__init__.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      416 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1831 2022-06-10 19:06:39.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/add_new_jobs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1309 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/cancel.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1941 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/cancel_all.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1086 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/rebuild_cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    13113 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/registry.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9382 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/retrigger.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/actions/util.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4583 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/config.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5184 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/create.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12882 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7834 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2793 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/files_changed.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      866 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/filter_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    15585 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/generator.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4667 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/graph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/loader/
--rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/loader/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1185 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/loader/default.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2147 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/loader/transform.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    26201 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/main.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9192 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/morph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/optimize/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      123 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/optimize/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    18341 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/optimize/base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2380 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/optimize/strategies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    11906 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/parameters.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)    29990 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/fetch-content
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)      896 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/hgrc
--rw-r--r--   0 ahal      (1000) ahal      (1000)    30243 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/robustcheckout.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)    44960 2023-06-08 19:59:10.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/run-task
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3324 2023-04-03 20:22:29.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/target_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3132 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2397 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/taskgraph.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/
--rw-r--r--   0 ahal      (1000) ahal      (1000)      110 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5285 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2607 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      707 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/code_review.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7606 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/docker_image.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10443 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/fetch.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6647 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/from_deps.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/
--rw-r--r--   0 ahal      (1000) ahal      (1000)    17271 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6826 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/common.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1220 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/index_search.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     9800 2023-06-08 14:51:23.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6015 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/toolchain.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6019 2023-03-09 21:54:49.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/notify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    51243 2023-06-08 14:51:24.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/task.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/
--rw-r--r--   0 ahal      (1000) ahal      (1000)        0 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/__init__.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2855 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/archive.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2964 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/attributes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3406 2023-06-02 18:49:13.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2433 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2502 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/dependencies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    11690 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1661 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/hash.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3419 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/keyed_by.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1331 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/memoize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3184 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/parameterization.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4466 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1576 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/python_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      787 2022-04-07 15:42:51.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/readonlydict.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     8323 2023-04-18 14:17:54.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/schema.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1317 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/shell.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12445 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/taskcluster.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1969 2023-03-01 18:52:59.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/taskgraph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1417 2022-05-30 14:06:28.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/templates.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3390 2023-03-01 18:54:05.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/time.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2687 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/treeherder.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    18534 2023-05-25 14:50:00.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/vcs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     8827 2023-06-08 14:51:24.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/verify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2494 2023-06-08 14:51:24.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/workertypes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1029 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/src/taskgraph/util/yaml.py
-drwxr-xr-x   0 ahal      (1000) ahal      (1000)        0 2023-06-08 20:00:01.000000 taskcluster-taskgraph-5.3.0/test/
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1584 2023-03-10 16:40:34.000000 taskcluster-taskgraph-5.3.0/test/test_actions_rebuild_cached_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1670 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_actions_registry.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3654 2023-03-09 21:40:30.000000 taskcluster-taskgraph-5.3.0/test/test_create.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7688 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_decision.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3505 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_files_changed.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7588 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_generator.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7063 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_graph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7940 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.3.0/test/test_main.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2701 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_morph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    15584 2023-06-08 02:55:35.000000 taskcluster-taskgraph-5.3.0/test/test_optimize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1727 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_optimize_strategies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    13921 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_parameters.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2491 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_scripts_fetch_content.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12257 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.3.0/test/test_scripts_run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    12046 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_target_tasks.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3759 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_taskgraph.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1812 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_transform_docker_image.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      874 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_base.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1527 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_fetch.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5880 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_from_deps.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5181 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_job.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6291 2023-04-19 14:40:27.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_job_run_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7131 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_job_toolchain.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6948 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_notify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    23573 2023-05-25 15:00:02.000000 taskcluster-taskgraph-5.3.0/test/test_transforms_task.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     3596 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_attributes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1120 2023-06-08 14:52:02.000000 taskcluster-taskgraph-5.3.0/test/test_util_dependencies.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10212 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_docker.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     2340 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_memoize.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     7556 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_util_parameterization.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     5906 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1045 2023-03-09 21:27:25.000000 taskcluster-taskgraph-5.3.0/test/test_util_python_path.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1234 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_readonlydict.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     6961 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_schema.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    10115 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_util_taskcluster.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)     1677 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_templates.py
--rwxr-xr-x   0 ahal      (1000) ahal      (1000)     2239 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_time.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      913 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_treeherder.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)    14739 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_util_vcs.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     4981 2023-03-09 21:35:48.000000 taskcluster-taskgraph-5.3.0/test/test_util_verify.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)      942 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_util_workertypes.py
--rw-r--r--   0 ahal      (1000) ahal      (1000)     1591 2023-04-19 14:40:20.000000 taskcluster-taskgraph-5.3.0/test/test_util_yaml.py
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.762659 taskcluster-taskgraph-5.4.0/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    16725 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/LICENSE
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      175 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/MANIFEST.in
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      665 2023-06-13 13:57:11.758659 taskcluster-taskgraph-5.4.0/PKG-INFO
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3659 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/README.rst
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      602 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/pyproject.toml
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.738659 taskcluster-taskgraph-5.4.0/requirements/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      177 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/requirements/base.in
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    20339 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/requirements/base.txt
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)       22 2023-01-24 13:47:12.000000 taskcluster-taskgraph-5.4.0/requirements/dev.in
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1281 2023-06-08 13:35:32.000000 taskcluster-taskgraph-5.4.0/requirements/dev.txt
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)       58 2023-01-24 13:47:12.000000 taskcluster-taskgraph-5.4.0/requirements/test.in
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     9241 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/requirements/test.txt
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)       38 2023-06-13 13:57:11.762659 taskcluster-taskgraph-5.4.0/setup.cfg
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1555 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/setup.py
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.734659 taskcluster-taskgraph-5.4.0/src/
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.738659 taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      665 2023-06-13 13:57:11.000000 taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/PKG-INFO
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3977 2023-06-13 13:57:11.000000 taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)        1 2023-06-13 13:57:11.000000 taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/dependency_links.txt
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)       50 2023-06-13 13:57:11.000000 taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/entry_points.txt
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      201 2023-06-13 13:57:11.000000 taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/requires.txt
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)       10 2023-06-13 13:57:11.000000 taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/top_level.txt
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.738659 taskcluster-taskgraph-5.4.0/src/taskgraph/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      729 2023-06-13 09:06:43.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/__init__.py
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.742659 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      416 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/__init__.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1836 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/add_new_jobs.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1309 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/cancel.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1941 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/cancel_all.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1086 2022-11-29 10:00:19.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/rebuild_cached_tasks.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    13113 2023-03-08 13:37:12.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/registry.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     9387 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/retrigger.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    10661 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/actions/util.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4611 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/config.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5184 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/create.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    12882 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/decision.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7834 2023-02-24 15:00:45.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/docker.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2793 2022-08-29 09:00:10.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/files_changed.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      866 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/filter_tasks.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    15541 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/generator.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4680 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/graph.py
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.742659 taskcluster-taskgraph-5.4.0/src/taskgraph/loader/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)        0 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/loader/__init__.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1185 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/loader/default.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2147 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/loader/transform.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    26201 2023-06-08 13:35:32.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/main.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     9192 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/morph.py
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.742659 taskcluster-taskgraph-5.4.0/src/taskgraph/optimize/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      123 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/optimize/__init__.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    18341 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/optimize/base.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2380 2023-02-24 15:00:45.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/optimize/strategies.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    11906 2022-11-08 15:09:41.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/parameters.py
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.742659 taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/
+-rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)    29990 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/fetch-content
+-rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)      896 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/hgrc
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    30243 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/robustcheckout.py
+-rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)    44960 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/run-task
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3324 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/target_tasks.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3240 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/task.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2434 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/taskgraph.py
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.746659 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      110 2022-11-29 10:00:19.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/__init__.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5146 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/base.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2607 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/cached_tasks.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      707 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/code_review.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7606 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/docker_image.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    10479 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/fetch.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6647 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/from_deps.py
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.746659 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    17271 2022-12-19 12:50:27.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/__init__.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6826 2022-10-13 13:09:44.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/common.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1220 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/index_search.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     9814 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/run_task.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6015 2023-02-24 15:00:45.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/toolchain.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6019 2022-11-29 10:00:19.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/notify.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    51279 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/task.py
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.750659 taskcluster-taskgraph-5.4.0/src/taskgraph/util/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)        0 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/__init__.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2855 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/archive.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2964 2023-06-08 13:35:32.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/attributes.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3406 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/cached_tasks.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2433 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/decision.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2502 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/dependencies.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    11690 2023-03-08 13:37:12.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/docker.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1661 2023-01-24 13:47:12.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/hash.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3419 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/keyed_by.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1331 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/memoize.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3184 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/parameterization.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4466 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/path.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1576 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/python_path.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      787 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/readonlydict.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     8323 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/schema.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1317 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/shell.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    12445 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/taskcluster.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1969 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/taskgraph.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1417 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/templates.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3390 2022-08-26 12:55:10.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/time.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2687 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/treeherder.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    18534 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/vcs.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     8947 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/verify.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2498 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/workertypes.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1029 2023-03-08 13:37:12.000000 taskcluster-taskgraph-5.4.0/src/taskgraph/util/yaml.py
+drwxr-xr-x   0 jcristau  (1000) jcristau  (1000)        0 2023-06-13 13:57:11.758659 taskcluster-taskgraph-5.4.0/test/
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1584 2022-11-29 10:00:19.000000 taskcluster-taskgraph-5.4.0/test/test_actions_rebuild_cached_tasks.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1670 2022-09-07 16:01:21.000000 taskcluster-taskgraph-5.4.0/test/test_actions_registry.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3654 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/test/test_create.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7688 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/test/test_decision.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3505 2022-08-29 09:00:10.000000 taskcluster-taskgraph-5.4.0/test/test_files_changed.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7588 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/test/test_generator.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7063 2023-02-24 15:00:45.000000 taskcluster-taskgraph-5.4.0/test/test_graph.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7940 2023-06-08 13:35:32.000000 taskcluster-taskgraph-5.4.0/test/test_main.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2701 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/test/test_morph.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    15584 2023-06-08 13:35:32.000000 taskcluster-taskgraph-5.4.0/test/test_optimize.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1727 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_optimize_strategies.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    13921 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/test/test_parameters.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2491 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/test/test_scripts_fetch_content.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    12257 2023-06-08 13:35:32.000000 taskcluster-taskgraph-5.4.0/test/test_scripts_run_task.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    12046 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_target_tasks.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3759 2023-02-24 15:00:45.000000 taskcluster-taskgraph-5.4.0/test/test_taskgraph.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1812 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/test/test_transform_docker_image.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      874 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_base.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1527 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_fetch.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5880 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_from_deps.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5181 2023-01-24 13:47:12.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_job.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6291 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_job_run_task.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7131 2023-02-24 15:00:45.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_job_toolchain.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6948 2022-11-29 10:00:19.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_notify.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    23573 2023-06-08 13:35:29.000000 taskcluster-taskgraph-5.4.0/test/test_transforms_task.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     3596 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_attributes.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1120 2023-06-13 07:43:16.000000 taskcluster-taskgraph-5.4.0/test/test_util_dependencies.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    10212 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_docker.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     2340 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_memoize.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     7556 2023-01-24 13:47:12.000000 taskcluster-taskgraph-5.4.0/test/test_util_parameterization.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     5906 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_path.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1045 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_python_path.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1234 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_readonlydict.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     6961 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_schema.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    10115 2023-02-24 15:00:45.000000 taskcluster-taskgraph-5.4.0/test/test_util_taskcluster.py
+-rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)     1677 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_templates.py
+-rwxr-xr-x   0 jcristau  (1000) jcristau  (1000)     2239 2022-09-07 16:01:29.000000 taskcluster-taskgraph-5.4.0/test/test_util_time.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      913 2022-07-27 13:56:11.000000 taskcluster-taskgraph-5.4.0/test/test_util_treeherder.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)    14739 2023-04-27 13:22:14.000000 taskcluster-taskgraph-5.4.0/test/test_util_vcs.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     4981 2022-08-23 14:06:09.000000 taskcluster-taskgraph-5.4.0/test/test_util_verify.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)      942 2023-03-08 13:37:12.000000 taskcluster-taskgraph-5.4.0/test/test_util_workertypes.py
+-rw-r--r--   0 jcristau  (1000) jcristau  (1000)     1591 2023-03-08 13:37:12.000000 taskcluster-taskgraph-5.4.0/test/test_util_yaml.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `taskcluster-taskgraph-5.3.0/LICENSE` & `taskcluster-taskgraph-5.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/PKG-INFO` & `taskcluster-taskgraph-5.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.3.0
+Version: 5.4.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `taskcluster-taskgraph-5.3.0/README.rst` & `taskcluster-taskgraph-5.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/pyproject.toml` & `taskcluster-taskgraph-5.4.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/requirements/base.txt` & `taskcluster-taskgraph-5.4.0/requirements/base.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,22 @@
-# SHA1:a199a11be56ce347d10dd1fce8de55752b42b141
+# SHA1:23064426a438219fd274b6a954a7740f27c6a978
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 appdirs==1.4.4 \
     --hash=sha256:7d5d0167b2b1ba821647616af46a749d1c653740dd0d2415100fe26e27afdf41 \
     --hash=sha256:a841dacd6b99318a741b166adb07e19ee71a274450e68237b4650ca1055ab128
     # via -r requirements/base.in
 arrow==1.2.3 \
     --hash=sha256:3934b30ca1b9f292376d9db15b19446088d12ec58629bc3f0da28fd55fb633a1 \
     --hash=sha256:5a49ab92e3b7b71d96cd6bfcc4df14efefc9dfa96ea19045815914a6ab6b1fe2
     # via jinja2-time
-attrs==23.1.0 \
-    --hash=sha256:1f28b4522cdc2fb4256ac1a020c78acf9cba2c6b461ccd2c126f3aa8e8335d04 \
-    --hash=sha256:6279836d581513a26f1bf235f9acd333bc9115683f14f7e8fae46c98fc50e015
-    # via -r requirements/base.in
 binaryornot==0.4.4 \
     --hash=sha256:359501dfc9d40632edc9fac890e19542db1a287bbcfa58175b66658392018061 \
     --hash=sha256:b8b71173c917bddcd2c16070412e369c3ed7f0528926f70cac18a6c97fd563e4
     # via cookiecutter
 certifi==2023.5.7 \
     --hash=sha256:0f0d56dc5a6ad56fd4ba36484d6cc34451e1c6548c61daad8c320169f91eddc7 \
     --hash=sha256:c6c2e98f5c7869efca1f8916fed228dd91539f9f1b444c314c06eef02980c716
@@ -138,65 +134,65 @@
     --hash=sha256:d14eaa4d315e7688daa4969f616f226614350c48730bfa1692d2caebd8c90d40 \
     --hash=sha256:d3eab6605e3ec8b7a0863df09cc1d23714908fa61aa6986a845c20ba488b4efa
     # via cookiecutter
 json-e==4.5.2 \
     --hash=sha256:0d1203645a5753dec2da1ceab279f82169023948eff858b87968117e8a592e10 \
     --hash=sha256:b1c82e79ec232b8a86393488b39aa086f8c098cf67fa190ac03517daf0e51aed
     # via -r requirements/base.in
-markupsafe==2.1.2 \
-    --hash=sha256:0576fe974b40a400449768941d5d0858cc624e3249dfd1e0c33674e5c7ca7aed \
-    --hash=sha256:085fd3201e7b12809f9e6e9bc1e5c96a368c8523fad5afb02afe3c051ae4afcc \
-    --hash=sha256:090376d812fb6ac5f171e5938e82e7f2d7adc2b629101cec0db8b267815c85e2 \
-    --hash=sha256:0b462104ba25f1ac006fdab8b6a01ebbfbce9ed37fd37fd4acd70c67c973e460 \
-    --hash=sha256:137678c63c977754abe9086a3ec011e8fd985ab90631145dfb9294ad09c102a7 \
-    --hash=sha256:1bea30e9bf331f3fef67e0a3877b2288593c98a21ccb2cf29b74c581a4eb3af0 \
-    --hash=sha256:22152d00bf4a9c7c83960521fc558f55a1adbc0631fbb00a9471e097b19d72e1 \
-    --hash=sha256:22731d79ed2eb25059ae3df1dfc9cb1546691cc41f4e3130fe6bfbc3ecbbecfa \
-    --hash=sha256:2298c859cfc5463f1b64bd55cb3e602528db6fa0f3cfd568d3605c50678f8f03 \
-    --hash=sha256:28057e985dace2f478e042eaa15606c7efccb700797660629da387eb289b9323 \
-    --hash=sha256:2e7821bffe00aa6bd07a23913b7f4e01328c3d5cc0b40b36c0bd81d362faeb65 \
-    --hash=sha256:2ec4f2d48ae59bbb9d1f9d7efb9236ab81429a764dedca114f5fdabbc3788013 \
-    --hash=sha256:340bea174e9761308703ae988e982005aedf427de816d1afe98147668cc03036 \
-    --hash=sha256:40627dcf047dadb22cd25ea7ecfe9cbf3bbbad0482ee5920b582f3809c97654f \
-    --hash=sha256:40dfd3fefbef579ee058f139733ac336312663c6706d1163b82b3003fb1925c4 \
-    --hash=sha256:4cf06cdc1dda95223e9d2d3c58d3b178aa5dacb35ee7e3bbac10e4e1faacb419 \
-    --hash=sha256:50c42830a633fa0cf9e7d27664637532791bfc31c731a87b202d2d8ac40c3ea2 \
-    --hash=sha256:55f44b440d491028addb3b88f72207d71eeebfb7b5dbf0643f7c023ae1fba619 \
-    --hash=sha256:608e7073dfa9e38a85d38474c082d4281f4ce276ac0010224eaba11e929dd53a \
-    --hash=sha256:63ba06c9941e46fa389d389644e2d8225e0e3e5ebcc4ff1ea8506dce646f8c8a \
-    --hash=sha256:65608c35bfb8a76763f37036547f7adfd09270fbdbf96608be2bead319728fcd \
-    --hash=sha256:665a36ae6f8f20a4676b53224e33d456a6f5a72657d9c83c2aa00765072f31f7 \
-    --hash=sha256:6d6607f98fcf17e534162f0709aaad3ab7a96032723d8ac8750ffe17ae5a0666 \
-    --hash=sha256:7313ce6a199651c4ed9d7e4cfb4aa56fe923b1adf9af3b420ee14e6d9a73df65 \
-    --hash=sha256:7668b52e102d0ed87cb082380a7e2e1e78737ddecdde129acadb0eccc5423859 \
-    --hash=sha256:7df70907e00c970c60b9ef2938d894a9381f38e6b9db73c5be35e59d92e06625 \
-    --hash=sha256:7e007132af78ea9df29495dbf7b5824cb71648d7133cf7848a2a5dd00d36f9ff \
-    --hash=sha256:835fb5e38fd89328e9c81067fd642b3593c33e1e17e2fdbf77f5676abb14a156 \
-    --hash=sha256:8bca7e26c1dd751236cfb0c6c72d4ad61d986e9a41bbf76cb445f69488b2a2bd \
-    --hash=sha256:8db032bf0ce9022a8e41a22598eefc802314e81b879ae093f36ce9ddf39ab1ba \
-    --hash=sha256:99625a92da8229df6d44335e6fcc558a5037dd0a760e11d84be2260e6f37002f \
-    --hash=sha256:9cad97ab29dfc3f0249b483412c85c8ef4766d96cdf9dcf5a1e3caa3f3661cf1 \
-    --hash=sha256:a4abaec6ca3ad8660690236d11bfe28dfd707778e2442b45addd2f086d6ef094 \
-    --hash=sha256:a6e40afa7f45939ca356f348c8e23048e02cb109ced1eb8420961b2f40fb373a \
-    --hash=sha256:a6f2fcca746e8d5910e18782f976489939d54a91f9411c32051b4aab2bd7c513 \
-    --hash=sha256:a806db027852538d2ad7555b203300173dd1b77ba116de92da9afbc3a3be3eed \
-    --hash=sha256:abcabc8c2b26036d62d4c746381a6f7cf60aafcc653198ad678306986b09450d \
-    --hash=sha256:b8526c6d437855442cdd3d87eede9c425c4445ea011ca38d937db299382e6fa3 \
-    --hash=sha256:bb06feb762bade6bf3c8b844462274db0c76acc95c52abe8dbed28ae3d44a147 \
-    --hash=sha256:c0a33bc9f02c2b17c3ea382f91b4db0e6cde90b63b296422a939886a7a80de1c \
-    --hash=sha256:c4a549890a45f57f1ebf99c067a4ad0cb423a05544accaf2b065246827ed9603 \
-    --hash=sha256:ca244fa73f50a800cf8c3ebf7fd93149ec37f5cb9596aa8873ae2c1d23498601 \
-    --hash=sha256:cf877ab4ed6e302ec1d04952ca358b381a882fbd9d1b07cccbfd61783561f98a \
-    --hash=sha256:d9d971ec1e79906046aa3ca266de79eac42f1dbf3612a05dc9368125952bd1a1 \
-    --hash=sha256:da25303d91526aac3672ee6d49a2f3db2d9502a4a60b55519feb1a4c7714e07d \
-    --hash=sha256:e55e40ff0cc8cc5c07996915ad367fa47da6b3fc091fdadca7f5403239c5fec3 \
-    --hash=sha256:f03a532d7dee1bed20bc4884194a16160a2de9ffc6354b3878ec9682bb623c54 \
-    --hash=sha256:f1cd098434e83e656abf198f103a8207a8187c0fc110306691a2e94a78d0abb2 \
-    --hash=sha256:f2bfb563d0211ce16b63c7cb9395d2c682a23187f54c3d79bfec33e6705473c6 \
-    --hash=sha256:f8ffb705ffcf5ddd0e80b65ddf7bed7ee4f5a441ea7d3419e861a12eaf41af58
+markupsafe==2.1.3 \
+    --hash=sha256:05fb21170423db021895e1ea1e1f3ab3adb85d1c2333cbc2310f2a26bc77272e \
+    --hash=sha256:0a4e4a1aff6c7ac4cd55792abf96c915634c2b97e3cc1c7129578aa68ebd754e \
+    --hash=sha256:10bbfe99883db80bdbaff2dcf681dfc6533a614f700da1287707e8a5d78a8431 \
+    --hash=sha256:134da1eca9ec0ae528110ccc9e48041e0828d79f24121a1a146161103c76e686 \
+    --hash=sha256:1577735524cdad32f9f694208aa75e422adba74f1baee7551620e43a3141f559 \
+    --hash=sha256:1b40069d487e7edb2676d3fbdb2b0829ffa2cd63a2ec26c4938b2d34391b4ecc \
+    --hash=sha256:282c2cb35b5b673bbcadb33a585408104df04f14b2d9b01d4c345a3b92861c2c \
+    --hash=sha256:2c1b19b3aaacc6e57b7e25710ff571c24d6c3613a45e905b1fde04d691b98ee0 \
+    --hash=sha256:2ef12179d3a291be237280175b542c07a36e7f60718296278d8593d21ca937d4 \
+    --hash=sha256:338ae27d6b8745585f87218a3f23f1512dbf52c26c28e322dbe54bcede54ccb9 \
+    --hash=sha256:3c0fae6c3be832a0a0473ac912810b2877c8cb9d76ca48de1ed31e1c68386575 \
+    --hash=sha256:3fd4abcb888d15a94f32b75d8fd18ee162ca0c064f35b11134be77050296d6ba \
+    --hash=sha256:42de32b22b6b804f42c5d98be4f7e5e977ecdd9ee9b660fda1a3edf03b11792d \
+    --hash=sha256:504b320cd4b7eff6f968eddf81127112db685e81f7e36e75f9f84f0df46041c3 \
+    --hash=sha256:525808b8019e36eb524b8c68acdd63a37e75714eac50e988180b169d64480a00 \
+    --hash=sha256:56d9f2ecac662ca1611d183feb03a3fa4406469dafe241673d521dd5ae92a155 \
+    --hash=sha256:5bbe06f8eeafd38e5d0a4894ffec89378b6c6a625ff57e3028921f8ff59318ac \
+    --hash=sha256:65c1a9bcdadc6c28eecee2c119465aebff8f7a584dd719facdd9e825ec61ab52 \
+    --hash=sha256:68e78619a61ecf91e76aa3e6e8e33fc4894a2bebe93410754bd28fce0a8a4f9f \
+    --hash=sha256:69c0f17e9f5a7afdf2cc9fb2d1ce6aabdb3bafb7f38017c0b77862bcec2bbad8 \
+    --hash=sha256:6b2b56950d93e41f33b4223ead100ea0fe11f8e6ee5f641eb753ce4b77a7042b \
+    --hash=sha256:787003c0ddb00500e49a10f2844fac87aa6ce977b90b0feaaf9de23c22508b24 \
+    --hash=sha256:7ef3cb2ebbf91e330e3bb937efada0edd9003683db6b57bb108c4001f37a02ea \
+    --hash=sha256:8023faf4e01efadfa183e863fefde0046de576c6f14659e8782065bcece22198 \
+    --hash=sha256:8758846a7e80910096950b67071243da3e5a20ed2546e6392603c096778d48e0 \
+    --hash=sha256:8afafd99945ead6e075b973fefa56379c5b5c53fd8937dad92c662da5d8fd5ee \
+    --hash=sha256:8c41976a29d078bb235fea9b2ecd3da465df42a562910f9022f1a03107bd02be \
+    --hash=sha256:8e254ae696c88d98da6555f5ace2279cf7cd5b3f52be2b5cf97feafe883b58d2 \
+    --hash=sha256:9402b03f1a1b4dc4c19845e5c749e3ab82d5078d16a2a4c2cd2df62d57bb0707 \
+    --hash=sha256:962f82a3086483f5e5f64dbad880d31038b698494799b097bc59c2edf392fce6 \
+    --hash=sha256:9dcdfd0eaf283af041973bff14a2e143b8bd64e069f4c383416ecd79a81aab58 \
+    --hash=sha256:aa7bd130efab1c280bed0f45501b7c8795f9fdbeb02e965371bbef3523627779 \
+    --hash=sha256:ab4a0df41e7c16a1392727727e7998a467472d0ad65f3ad5e6e765015df08636 \
+    --hash=sha256:ad9e82fb8f09ade1c3e1b996a6337afac2b8b9e365f926f5a61aacc71adc5b3c \
+    --hash=sha256:af598ed32d6ae86f1b747b82783958b1a4ab8f617b06fe68795c7f026abbdcad \
+    --hash=sha256:b076b6226fb84157e3f7c971a47ff3a679d837cf338547532ab866c57930dbee \
+    --hash=sha256:b7ff0f54cb4ff66dd38bebd335a38e2c22c41a8ee45aa608efc890ac3e3931bc \
+    --hash=sha256:bfce63a9e7834b12b87c64d6b155fdd9b3b96191b6bd334bf37db7ff1fe457f2 \
+    --hash=sha256:c011a4149cfbcf9f03994ec2edffcb8b1dc2d2aede7ca243746df97a5d41ce48 \
+    --hash=sha256:c9c804664ebe8f83a211cace637506669e7890fec1b4195b505c214e50dd4eb7 \
+    --hash=sha256:ca379055a47383d02a5400cb0d110cef0a776fc644cda797db0c5696cfd7e18e \
+    --hash=sha256:cb0932dc158471523c9637e807d9bfb93e06a95cbf010f1a38b98623b929ef2b \
+    --hash=sha256:cd0f502fe016460680cd20aaa5a76d241d6f35a1c3350c474bac1273803893fa \
+    --hash=sha256:ceb01949af7121f9fc39f7d27f91be8546f3fb112c608bc4029aef0bab86a2a5 \
+    --hash=sha256:d080e0a5eb2529460b30190fcfcc4199bd7f827663f858a226a81bc27beaa97e \
+    --hash=sha256:dd15ff04ffd7e05ffcb7fe79f1b98041b8ea30ae9234aed2a9168b5797c3effb \
+    --hash=sha256:df0be2b576a7abbf737b1575f048c23fb1d769f267ec4358296f31c2479db8f9 \
+    --hash=sha256:e09031c87a1e51556fdcb46e5bd4f59dfb743061cf93c4d6831bf894f125eb57 \
+    --hash=sha256:e4dd52d80b8c83fdce44e12478ad2e85c64ea965e75d66dbeafb0a3e77308fcc \
+    --hash=sha256:fec21693218efe39aa7f8599346e90c705afa52c5b31ae019b2e57e8f6542bb2
     # via jinja2
 mozilla-repo-urls==0.1.1 \
     --hash=sha256:30510d3519479aa70211145d0ac9cf6e2fadcb8d30fa3b196bb957bd773502ba \
     --hash=sha256:7364da790751db2a060eb45adbf1d7db89a145ed279ba235f3425db9dd255915
     # via -r requirements/base.in
 python-dateutil==2.8.2 \
     --hash=sha256:0123cacc1627ae19ddf3c27a5de5bd67ee4586fbdd6440d9748f8abb483d3e86 \
@@ -278,23 +274,23 @@
     --hash=sha256:b25e122ecec249c4299ac7b20b08db76e3e2025bdaeb699a9d444556de5fd367 \
     --hash=sha256:f66dcbd6572a6216ab65949f0fa0b91f2df647918028436c384e6af5cd12ae2b
     # via -r requirements/base.in
 text-unidecode==1.3 \
     --hash=sha256:1311f10e8b895935241623731c2ba64f4c455287888b18189350b67134a822e8 \
     --hash=sha256:bad6603bb14d279193107714b288be206cac565dfa49aa5b105294dd5c4aab93
     # via python-slugify
-typing-extensions==4.6.2 \
-    --hash=sha256:06006244c70ac8ee83fa8282cb188f697b8db25bc8b4df07be1873c43897060c \
-    --hash=sha256:3a8b36f13dd5fdc5d1b16fe317f5668545de77fa0b8e02006381fd49d731ab98
+typing-extensions==4.6.3 \
+    --hash=sha256:88a4153d8505aabbb4e13aacb7c486c2b4a33ca3b3f807914a9b4c844c471c26 \
+    --hash=sha256:d91d5919357fe7f681a9f2b5b4cb2a5f1ef0a1e9f59c4d8ff0d3491e05c0ffd5
     # via
     #   arrow
     #   importlib-metadata
-urllib3==2.0.2 \
-    --hash=sha256:61717a1095d7e155cdb737ac7bb2f4324a858a1e2e6466f6d03ff630ca68d3cc \
-    --hash=sha256:d055c2f9d38dc53c808f6fdc8eab7360b6fdbbde02340ed25cfbcd817c62469e
+urllib3==2.0.3 \
+    --hash=sha256:48e7fafa40319d358848e1bc6809b208340fafe2096f1725d05d67443d0483d1 \
+    --hash=sha256:bee28b5e56addb8226c96f7f13ac28cb4c301dd5ea8a6ca179c0b9835e032825
     # via requests
 voluptuous==0.13.1 \
     --hash=sha256:4b838b185f5951f2d6e8752b68fcf18bd7a9c26ded8f143f92d6d28f3921a3e6 \
     --hash=sha256:e8d31c20601d6773cb14d4c0f42aee29c6821bbd1018039aac7ac5605b489723
     # via -r requirements/base.in
 zipp==3.15.0 \
     --hash=sha256:112929ad649da941c23de50f356a2b5570c954b65150642bccdd66bf194d224b \
```

### Comparing `taskcluster-taskgraph-5.3.0/requirements/dev.txt` & `taskcluster-taskgraph-5.4.0/requirements/dev.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/requirements/test.txt` & `taskcluster-taskgraph-5.4.0/requirements/test.txt`

 * *Files 16% similar despite different names*

```diff
@@ -2,74 +2,83 @@
 #
 # This file is autogenerated by pip-compile-multi
 # To update, run:
 #
 #    pip-compile-multi
 #
 -r base.txt
-cachetools==5.3.0 \
-    --hash=sha256:13dfddc7b8df938c21a940dfa6557ce6e94a2f1cdfa58eb90c805721d58f2c14 \
-    --hash=sha256:429e1a1e845c008ea6c85aa35d4b98b65d6a9763eeef3e37e92728a12d1de9d4
+cachetools==5.3.1 \
+    --hash=sha256:95ef631eeaea14ba2e36f06437f36463aac3a096799e876ee55e5cdccb102590 \
+    --hash=sha256:dce83f2d9b4e1f732a8cd44af8e8fab2dbe46201467fc98b3ef8f269092bf62b
     # via tox
 colorama==0.4.6 \
     --hash=sha256:08695f5cb7ed6e0531a20572697297273c47b8cae5a63ffc6d6ed5c201be6e44 \
     --hash=sha256:4f1d9991f5acc0ca119f9d443620b77f9d6b33703e51011c16baf57afb285fc6
     # via tox
-coverage==7.2.6 \
-    --hash=sha256:004948e296149644d208964300cb3d98affc5211e9e490e9979af4030b0d6473 \
-    --hash=sha256:13cde6bb0e58fb67d09e2f373de3899d1d1e866c5a9ff05d93615f2f54fbd2bb \
-    --hash=sha256:1c9e4a5eb1bbc3675ee57bc31f8eea4cd7fb0cbcbe4912cf1cb2bf3b754f4a80 \
-    --hash=sha256:2025f913f2edb0272ef15d00b1f335ff8908c921c8eb2013536fcaf61f5a683d \
-    --hash=sha256:25bad4196104761bc26b1dae9b57383826542ec689ff0042f7f4f4dd7a815cba \
-    --hash=sha256:2692306d3d4cb32d2cceed1e47cebd6b1d2565c993d6d2eda8e6e6adf53301e6 \
-    --hash=sha256:272ab31228a9df857ab5df5d67936d8861464dc89c5d3fab35132626e9369379 \
-    --hash=sha256:2e8c0e79820cdd67978e1120983786422d279e07a381dbf89d03bbb23ec670a6 \
-    --hash=sha256:3062fd5c62df988cea9f2972c593f77fed1182bfddc5a3b12b1e606cb7aba99e \
-    --hash=sha256:3436927d1794fa6763b89b60c896f9e3bd53212001026ebc9080d23f0c2733c1 \
-    --hash=sha256:35db06450272473eab4449e9c2ad9bc6a0a68dab8e81a0eae6b50d9c2838767e \
-    --hash=sha256:392154d09bd4473b9d11351ab5d63391f3d5d24d752f27b3be7498b0ee2b5226 \
-    --hash=sha256:3cff6980fe7100242170092bb40d2b1cdad79502cd532fd26b12a2b8a5f9aee0 \
-    --hash=sha256:42c692b55a647a832025a4c048007034fe77b162b566ad537ce65ad824b12a84 \
-    --hash=sha256:44c9b9f1a245f3d0d202b1a8fa666a80b5ecbe4ad5d0859c0fb16a52d9763224 \
-    --hash=sha256:496b86f1fc9c81a1cd53d8842ef712e950a4611bba0c42d33366a7b91ba969ec \
-    --hash=sha256:4bbd58eb5a2371bf160590f4262109f66b6043b0b991930693134cb617bc0169 \
-    --hash=sha256:4e3783a286d5a93a2921396d50ce45a909aa8f13eee964465012f110f0cbb611 \
-    --hash=sha256:4f3c7c19581d471af0e9cb49d928172cd8492cd78a2b7a4e82345d33662929bb \
-    --hash=sha256:52c139b7ab3f0b15f9aad0a3fedef5a1f8c0b2bdc291d88639ca2c97d3682416 \
-    --hash=sha256:541280dde49ce74a4262c5e395b48ea1207e78454788887118c421cb4ffbfcac \
-    --hash=sha256:5906f6a84b47f995cd1bf0aca1c72d591c55ee955f98074e93660d64dfc66eb9 \
-    --hash=sha256:6284a2005e4f8061c58c814b1600ad0074ccb0289fe61ea709655c5969877b70 \
-    --hash=sha256:6727a0d929ff0028b1ed8b3e7f8701670b1d7032f219110b55476bb60c390bfb \
-    --hash=sha256:697f4742aa3f26c107ddcb2b1784a74fe40180014edbd9adaa574eac0529914c \
-    --hash=sha256:6b9f64526286255735847aed0221b189486e0b9ed943446936e41b7e44b08783 \
-    --hash=sha256:6babcbf1e66e46052442f10833cfc4a0d3554d8276aa37af8531a83ed3c1a01d \
-    --hash=sha256:6e7f1a8328eeec34c54f1d5968a708b50fc38d31e62ca8b0560e84a968fbf9a9 \
-    --hash=sha256:71f739f97f5f80627f1fee2331e63261355fd1e9a9cce0016394b6707ac3f4ec \
-    --hash=sha256:76d06b721c2550c01a60e5d3093f417168658fb454e5dfd9a23570e9bffe39a1 \
-    --hash=sha256:77a04b84d01f0e12c66f16e69e92616442dc675bbe51b90bfb074b1e5d1c7fbd \
-    --hash=sha256:97729e6828643f168a2a3f07848e1b1b94a366b13a9f5aba5484c2215724edc8 \
-    --hash=sha256:9a8723ccec4e564d4b9a79923246f7b9a8de4ec55fa03ec4ec804459dade3c4f \
-    --hash=sha256:a5ffd45c6b93c23a8507e2f436983015c6457aa832496b6a095505ca2f63e8f1 \
-    --hash=sha256:a6f03f87fea579d55e0b690d28f5042ec1368650466520fbc400e7aeaf09e995 \
-    --hash=sha256:aac1d5fdc5378f6bac2c0c7ebe7635a6809f5b4376f6cf5d43243c1917a67087 \
-    --hash=sha256:ae82c5f168d2a39a5d69a12a69d4dc23837a43cf2ca99be60dfe59996ea6b113 \
-    --hash=sha256:bc7b667f8654376e9353dd93e55e12ce2a59fb6d8e29fce40de682273425e044 \
-    --hash=sha256:c1d7a31603c3483ac49c1726723b0934f88f2c011c660e6471e7bd735c2fa110 \
-    --hash=sha256:c534431153caffc7c495c3eddf7e6a6033e7f81d78385b4e41611b51e8870446 \
-    --hash=sha256:c93d52c3dc7b9c65e39473704988602300e3cc1bad08b5ab5b03ca98bbbc68c1 \
-    --hash=sha256:cbcc874f454ee51f158afd604a315f30c0e31dff1d5d5bf499fc529229d964dd \
-    --hash=sha256:d3cacc6a665221108ecdf90517a8028d07a2783df3417d12dcfef1c517e67478 \
-    --hash=sha256:d712cefff15c712329113b01088ba71bbcef0f7ea58478ca0bbec63a824844cb \
-    --hash=sha256:d7786b2fa7809bf835f830779ad285215a04da76293164bb6745796873f0942d \
-    --hash=sha256:dc11b42fa61ff1e788dd095726a0aed6aad9c03d5c5984b54cb9e1e67b276aa5 \
-    --hash=sha256:dc4d5187ef4d53e0d4c8eaf530233685667844c5fb0b855fea71ae659017854b \
-    --hash=sha256:f5440cdaf3099e7ab17a5a7065aed59aff8c8b079597b61c1f8be6f32fe60636 \
-    --hash=sha256:fa079995432037b5e2ef5ddbb270bcd2ded9f52b8e191a5de11fe59a00ea30d8 \
-    --hash=sha256:fbe6e8c0a9a7193ba10ee52977d4d5e7652957c1f56ccefed0701db8801a2a3b \
-    --hash=sha256:fde5c7a9d9864d3e07992f66767a9817f24324f354caa3d8129735a3dc74f126
+coverage==7.2.7 \
+    --hash=sha256:06a9a2be0b5b576c3f18f1a241f0473575c4a26021b52b2a85263a00f034d51f \
+    --hash=sha256:06fb182e69f33f6cd1d39a6c597294cff3143554b64b9825d1dc69d18cc2fff2 \
+    --hash=sha256:0a5f9e1dbd7fbe30196578ca36f3fba75376fb99888c395c5880b355e2875f8a \
+    --hash=sha256:0e1f928eaf5469c11e886fe0885ad2bf1ec606434e79842a879277895a50942a \
+    --hash=sha256:171717c7cb6b453aebac9a2ef603699da237f341b38eebfee9be75d27dc38e01 \
+    --hash=sha256:1e9d683426464e4a252bf70c3498756055016f99ddaec3774bf368e76bbe02b6 \
+    --hash=sha256:201e7389591af40950a6480bd9edfa8ed04346ff80002cec1a66cac4549c1ad7 \
+    --hash=sha256:245167dd26180ab4c91d5e1496a30be4cd721a5cf2abf52974f965f10f11419f \
+    --hash=sha256:2aee274c46590717f38ae5e4650988d1af340fe06167546cc32fe2f58ed05b02 \
+    --hash=sha256:2e07b54284e381531c87f785f613b833569c14ecacdcb85d56b25c4622c16c3c \
+    --hash=sha256:31563e97dae5598556600466ad9beea39fb04e0229e61c12eaa206e0aa202063 \
+    --hash=sha256:33d6d3ea29d5b3a1a632b3c4e4f4ecae24ef170b0b9ee493883f2df10039959a \
+    --hash=sha256:3d376df58cc111dc8e21e3b6e24606b5bb5dee6024f46a5abca99124b2229ef5 \
+    --hash=sha256:419bfd2caae268623dd469eff96d510a920c90928b60f2073d79f8fe2bbc5959 \
+    --hash=sha256:48c19d2159d433ccc99e729ceae7d5293fbffa0bdb94952d3579983d1c8c9d97 \
+    --hash=sha256:49969a9f7ffa086d973d91cec8d2e31080436ef0fb4a359cae927e742abfaaa6 \
+    --hash=sha256:52edc1a60c0d34afa421c9c37078817b2e67a392cab17d97283b64c5833f427f \
+    --hash=sha256:537891ae8ce59ef63d0123f7ac9e2ae0fc8b72c7ccbe5296fec45fd68967b6c9 \
+    --hash=sha256:54b896376ab563bd38453cecb813c295cf347cf5906e8b41d340b0321a5433e5 \
+    --hash=sha256:58c2ccc2f00ecb51253cbe5d8d7122a34590fac9646a960d1430d5b15321d95f \
+    --hash=sha256:5b7540161790b2f28143191f5f8ec02fb132660ff175b7747b95dcb77ac26562 \
+    --hash=sha256:5baa06420f837184130752b7c5ea0808762083bf3487b5038d68b012e5937dbe \
+    --hash=sha256:5e330fc79bd7207e46c7d7fd2bb4af2963f5f635703925543a70b99574b0fea9 \
+    --hash=sha256:61b9a528fb348373c433e8966535074b802c7a5d7f23c4f421e6c6e2f1697a6f \
+    --hash=sha256:63426706118b7f5cf6bb6c895dc215d8a418d5952544042c8a2d9fe87fcf09cb \
+    --hash=sha256:6d040ef7c9859bb11dfeb056ff5b3872436e3b5e401817d87a31e1750b9ae2fb \
+    --hash=sha256:6f48351d66575f535669306aa7d6d6f71bc43372473b54a832222803eb956fd1 \
+    --hash=sha256:7ee7d9d4822c8acc74a5e26c50604dff824710bc8de424904c0982e25c39c6cb \
+    --hash=sha256:81c13a1fc7468c40f13420732805a4c38a105d89848b7c10af65a90beff25250 \
+    --hash=sha256:8d13c64ee2d33eccf7437961b6ea7ad8673e2be040b4f7fd4fd4d4d28d9ccb1e \
+    --hash=sha256:8de8bb0e5ad103888d65abef8bca41ab93721647590a3f740100cd65c3b00511 \
+    --hash=sha256:8fa03bce9bfbeeef9f3b160a8bed39a221d82308b4152b27d82d8daa7041fee5 \
+    --hash=sha256:924d94291ca674905fe9481f12294eb11f2d3d3fd1adb20314ba89e94f44ed59 \
+    --hash=sha256:975d70ab7e3c80a3fe86001d8751f6778905ec723f5b110aed1e450da9d4b7f2 \
+    --hash=sha256:976b9c42fb2a43ebf304fa7d4a310e5f16cc99992f33eced91ef6f908bd8f33d \
+    --hash=sha256:9e31cb64d7de6b6f09702bb27c02d1904b3aebfca610c12772452c4e6c21a0d3 \
+    --hash=sha256:a342242fe22407f3c17f4b499276a02b01e80f861f1682ad1d95b04018e0c0d4 \
+    --hash=sha256:a3d33a6b3eae87ceaefa91ffdc130b5e8536182cd6dfdbfc1aa56b46ff8c86de \
+    --hash=sha256:a895fcc7b15c3fc72beb43cdcbdf0ddb7d2ebc959edac9cef390b0d14f39f8a9 \
+    --hash=sha256:afb17f84d56068a7c29f5fa37bfd38d5aba69e3304af08ee94da8ed5b0865833 \
+    --hash=sha256:b1c546aca0ca4d028901d825015dc8e4d56aac4b541877690eb76490f1dc8ed0 \
+    --hash=sha256:b29019c76039dc3c0fd815c41392a044ce555d9bcdd38b0fb60fb4cd8e475ba9 \
+    --hash=sha256:b46517c02ccd08092f4fa99f24c3b83d8f92f739b4657b0f146246a0ca6a831d \
+    --hash=sha256:b7aa5f8a41217360e600da646004f878250a0d6738bcdc11a0a39928d7dc2050 \
+    --hash=sha256:b7b4c971f05e6ae490fef852c218b0e79d4e52f79ef0c8475566584a8fb3e01d \
+    --hash=sha256:ba90a9563ba44a72fda2e85302c3abc71c5589cea608ca16c22b9804262aaeb6 \
+    --hash=sha256:cb017fd1b2603ef59e374ba2063f593abe0fc45f2ad9abdde5b4d83bd922a353 \
+    --hash=sha256:d22656368f0e6189e24722214ed8d66b8022db19d182927b9a248a2a8a2f67eb \
+    --hash=sha256:d2c2db7fd82e9b72937969bceac4d6ca89660db0a0967614ce2481e81a0b771e \
+    --hash=sha256:d39b5b4f2a66ccae8b7263ac3c8170994b65266797fb96cbbfd3fb5b23921db8 \
+    --hash=sha256:d62a5c7dad11015c66fbb9d881bc4caa5b12f16292f857842d9d1871595f4495 \
+    --hash=sha256:e7d9405291c6928619403db1d10bd07888888ec1abcbd9748fdaa971d7d661b2 \
+    --hash=sha256:e84606b74eb7de6ff581a7915e2dab7a28a0517fbe1c9239eb227e1354064dcd \
+    --hash=sha256:eb393e5ebc85245347950143969b241d08b52b88a3dc39479822e073a1a8eb27 \
+    --hash=sha256:ebba1cd308ef115925421d3e6a586e655ca5a77b5bf41e02eb0e4562a111f2d1 \
+    --hash=sha256:ee57190f24fba796e36bb6d3aa8a8783c643d8fa9760c89f7a98ab5455fbf818 \
+    --hash=sha256:f2f67fe12b22cd130d34d0ef79206061bfb5eda52feb6ce0dba0644e20a03cf4 \
+    --hash=sha256:f6951407391b639504e3b3be51b7ba5f3528adbf1a8ac3302b687ecababf929e \
+    --hash=sha256:f75f7168ab25dd93110c8a8117a22450c19976afbc44234cbf71481094c1b850 \
+    --hash=sha256:fdec9e8cbf13a5bf63290fc6013d216a4c7232efb51548594ca3631a7f13c3a3
     # via -r requirements/test.in
 distlib==0.3.6 \
     --hash=sha256:14bad2d9b04d3a36127ac97f30b12a19268f211063d8f8ee4f47108896e11b46 \
     --hash=sha256:f35c4b692542ca110de7ef0bea44d73981caeb34ca0b9b6b2e6d7790dda8f80e
     # via virtualenv
 exceptiongroup==1.1.1 \
     --hash=sha256:232c37c63e4f682982c8b6459f33a8981039e5fb8756b2074364e5055c498c9e \
@@ -129,17 +138,17 @@
 tomli==2.0.1 \
     --hash=sha256:939de3e7a6161af0c887ef91b7d41a53e7c5a1ca976325f429cb46ea9bc30ecc \
     --hash=sha256:de526c12914f0c550d15924c62d72abc48d6fe7364aa87328337a31007fe8a4f
     # via
     #   pyproject-api
     #   pytest
     #   tox
-tox==4.5.1 \
-    --hash=sha256:5a2eac5fb816779dfdf5cb00fecbc27eb0524e4626626bb1de84747b24cacc56 \
-    --hash=sha256:d25a2e6cb261adc489604fafd76cd689efeadfa79709965e965668d6d3f63046
+tox==4.6.0 \
+    --hash=sha256:4874000453e637a87ca892f9744a2ab9a7d24064dad1b0ecbf5a4c3c146cc732 \
+    --hash=sha256:954f1f647f67f481d239a193288983242a6152b67503c4a56b19a4aafaa29736
     # via -r requirements/test.in
 types-pyyaml==6.0.12.10 \
     --hash=sha256:662fa444963eff9b68120d70cda1af5a5f2aa57900003c2006d7626450eaae5f \
     --hash=sha256:ebab3d0700b946553724ae6ca636ea932c1b0868701d4af121630e78d695fc97
     # via responses
 virtualenv==20.23.0 \
     --hash=sha256:6abec7670e5802a528357fdc75b26b9f57d5d92f29c5462ba0fbe45feacc685e \
```

### Comparing `taskcluster-taskgraph-5.3.0/setup.py` & `taskcluster-taskgraph-5.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/PKG-INFO` & `taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: taskcluster-taskgraph
-Version: 5.3.0
+Version: 5.4.0
 Summary: Build taskcluster taskgraphs
 Home-page: https://github.com/taskcluster/taskgraph
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: Mozilla Public License 2.0 (MPL 2.0)
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt` & `taskcluster-taskgraph-5.4.0/src/taskcluster_taskgraph.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/__init__.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-__version__ = "5.3.0"
+__version__ = "5.4.0"
 
 # Maximum number of dependencies a single task can have
 # https://docs.taskcluster.net/reference/platform/taskcluster-queue/references/api#createTask
 # specifies 100, but we also optionally add the decision task id as a dep in
 # taskgraph.create, so let's set this to 99.
 MAX_DEPENDENCIES = 99
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/actions/add_new_jobs.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/actions/add_new_jobs.py`

 * *Files 8% similar despite different names*

```diff
@@ -55,10 +55,10 @@
         create_tasks(
             graph_config,
             to_run,
             full_task_graph,
             label_to_taskid,
             parameters,
             decision_task_id,
-            i,
+            f"{i}",
         )
     combine_task_graph_files(list(range(times)))
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/actions/cancel.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/actions/cancel.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/actions/cancel_all.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/actions/cancel_all.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/actions/rebuild_cached_tasks.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/actions/rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/actions/registry.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/actions/registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/actions/retrigger.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/actions/retrigger.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,15 +172,15 @@
         create_tasks(
             graph_config,
             to_run,
             full_task_graph,
             label_to_taskid,
             parameters,
             decision_task_id,
-            i,
+            f"{i}",
         )
 
         logger.info(f"Scheduled {label}{with_downstream}(time {i + 1}/{times})")
     combine_task_graph_files(list(range(times)))
 
 
 @register_callback_action(
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/actions/util.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/actions/util.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/config.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/config.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,17 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 import logging
 import os
 import sys
+from dataclasses import dataclass
+from typing import Dict
 
-import attr
 from voluptuous import All, Any, Extra, Length, Optional, Required
 
 from .util import path
 from .util.python_path import find_object
 from .util.schema import Schema, optionally_keyed_by, validate_schema
 from .util.yaml import load_yaml
 
@@ -74,18 +75,18 @@
         },
         Extra: object,
     }
 )
 """Schema for GraphConfig"""
 
 
-@attr.s(frozen=True, cmp=False)
+@dataclass(frozen=True, eq=False)
 class GraphConfig:
-    _config = attr.ib()
-    root_dir = attr.ib()
+    _config: Dict
+    root_dir: str
 
     _PATH_MODIFIED = False
 
     def __getitem__(self, name):
         return self._config[name]
 
     def __contains__(self, name):
@@ -133,8 +134,8 @@
     if not os.path.exists(config_yml):
         raise Exception(f"Couldn't find taskgraph configuration: {config_yml}")
 
     logger.debug(f"loading config from `{config_yml}`")
     config = load_yaml(config_yml)
 
     validate_graph_config(config)
-    return GraphConfig(config=config, root_dir=root_dir)
+    return GraphConfig(config, root_dir=root_dir)
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/create.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/decision.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/docker.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/files_changed.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/filter_tasks.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/filter_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/generator.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 import copy
 import logging
 import os
-from typing import AnyStr
-
-import attr
+from dataclasses import dataclass
+from typing import Dict
 
 from . import filter_tasks
 from .config import GraphConfig, load_graph_config
 from .graph import Graph
 from .morph import morph
 from .optimize.base import optimize_task_graph
 from .parameters import parameters_loader
@@ -27,20 +26,20 @@
 
 class KindNotFound(Exception):
     """
     Raised when trying to load kind from a directory without a kind.yml.
     """
 
 
-@attr.s(frozen=True)
+@dataclass(frozen=True)
 class Kind:
-    name = attr.ib(type=AnyStr)
-    path = attr.ib(type=AnyStr)
-    config = attr.ib(type=dict)
-    graph_config = attr.ib(type=GraphConfig)
+    name: str
+    path: str
+    config: Dict
+    graph_config: GraphConfig
 
     def _get_loader(self):
         try:
             loader = self.config["loader"]
         except KeyError:
             loader = "taskgraph.loader.default:loader"
         return find_object(loader)
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/graph.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/graph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 import collections
+from dataclasses import dataclass
+from typing import FrozenSet
 
-import attr
 
-
-@attr.s(frozen=True)
+@dataclass(frozen=True)
 class Graph:
     """Generic representation of a directed acyclic graph with labeled edges
     connecting the nodes. Graph operations are implemented in a functional
     manner, so the data structure is immutable.
 
     It permits at most one edge of a given name between any set of nodes.  The
     graph is not checked for cycles, and methods may hang or otherwise fail if
@@ -20,16 +20,16 @@
 
     The `nodes` and `edges` attributes may be accessed in a read-only fashion.
     The `nodes` attribute is a set of node names, while `edges` is a set of
     `(left, right, name)` tuples representing an edge named `name` going from
     node `left` to node `right`..
     """
 
-    nodes = attr.ib(converter=frozenset)
-    edges = attr.ib(converter=frozenset)
+    nodes: FrozenSet
+    edges: FrozenSet
 
     def transitive_closure(self, nodes, reverse=False):
         """Return the transitive closure of <nodes>: the graph containing all
         specified nodes as well as any nodes reachable from them, and any
         intervening edges.
 
         If `reverse` is true, the "reachability" will be reversed and this
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/loader/default.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/loader/default.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/loader/transform.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/loader/transform.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/main.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/morph.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/optimize/base.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/optimize/base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/optimize/strategies.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/optimize/strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/parameters.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/fetch-content` & `taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/fetch-content`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/hgrc` & `taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/hgrc`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/robustcheckout.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/robustcheckout.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/run-task/run-task` & `taskcluster-taskgraph-5.4.0/src/taskgraph/run-task/run-task`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/target_tasks.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/task.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/task.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
+from dataclasses import dataclass, field
+from typing import Any, Dict, List, Union
 
-import attr
 
-
-@attr.s
+@dataclass
 class Task:
     """
     Representation of a task in a TaskGraph.  Each Task has, at creation:
 
     - kind: the name of the task kind
     - label; the label for this task
     - attributes: a dictionary of attributes for this task (used for filtering)
@@ -27,26 +27,26 @@
 
     - task_id -- TaskCluster taskId under which this task will be created
 
     This class is just a convenience wrapper for the data type and managing
     display, comparison, serialization, etc. It has no functionality of its own.
     """
 
-    kind = attr.ib()
-    label = attr.ib()
-    attributes = attr.ib()
-    task = attr.ib()
-    description = attr.ib(default="")
-    task_id = attr.ib(default=None, init=False)
-    optimization = attr.ib(default=None)
-    dependencies = attr.ib(factory=dict)
-    soft_dependencies = attr.ib(factory=list)
-    if_dependencies = attr.ib(factory=list)
+    kind: str
+    label: str
+    attributes: Dict
+    task: Dict
+    description: str = ""
+    task_id: Union[str, None] = field(default=None, init=False)
+    optimization: Union[Dict[str, Any], None] = field(default=None)
+    dependencies: Dict = field(default_factory=dict)
+    soft_dependencies: List = field(default_factory=list)
+    if_dependencies: List = field(default_factory=list)
 
-    def __attrs_post_init__(self):
+    def __post_init__(self):
         self.attributes["kind"] = self.kind
 
     def to_json(self):
         rv = {
             "kind": self.kind,
             "label": self.label,
             "description": self.description,
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/taskgraph.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/taskgraph.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-
-import attr
+from dataclasses import dataclass
+from typing import List
 
 from .graph import Graph
 from .task import Task
 
 
-@attr.s(frozen=True)
+@dataclass(frozen=True)
 class TaskGraph:
     """
     Representation of a task graph.
 
     A task graph is a combination of a Graph and a dictionary of tasks indexed
     by label. TaskGraph instances should be treated as immutable.
 
     In the graph, tasks are said to "link to" their dependencies. Whereas
     tasks are "linked from" their dependents.
     """
 
-    tasks = attr.ib()
-    graph = attr.ib()
+    tasks: List[Task]
+    graph: Graph
 
-    def __attrs_post_init__(self):
+    def __post_init__(self):
         assert set(self.tasks) == self.graph.nodes
 
     def for_each_task(self, f, *args, **kwargs):
         for task_label in self.graph.visit_postorder():
             task = self.tasks[task_label]
             f(task, self, *args, **kwargs)
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/base.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/base.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,65 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 import re
-from typing import AnyStr
+from dataclasses import dataclass, field
+from typing import Dict, List, Union
 
-import attr
+from taskgraph.task import Task
 
 from ..config import GraphConfig
 from ..parameters import Parameters
 from ..util.memoize import memoize
 from ..util.schema import Schema, validate_schema
 
 
-@attr.s(frozen=True)
+@dataclass(frozen=True)
 class RepoConfig:
-    prefix = attr.ib(type=str)
-    name = attr.ib(type=str)
-    base_repository = attr.ib(type=str)
-    head_repository = attr.ib(type=str)
-    head_ref = attr.ib(type=str)
-    type = attr.ib(type=str)
-    path = attr.ib(type=str, default="")
-    head_rev = attr.ib(type=str, default=None)
-    ssh_secret_name = attr.ib(type=str, default=None)
+    prefix: str
+    name: str
+    base_repository: str
+    head_repository: str
+    head_ref: str
+    type: str
+    path: str = ""
+    head_rev: Union[str, None] = None
+    ssh_secret_name: Union[str, None] = None
 
 
-@attr.s(frozen=True, cmp=False)
+@dataclass(frozen=True, eq=False)
 class TransformConfig:
     """
     A container for configuration affecting transforms.  The `config` argument
     to transforms is an instance of this class.
     """
 
     # the name of the current kind
-    kind = attr.ib()
+    kind: str
 
     # the path to the kind configuration directory
-    path = attr.ib(type=AnyStr)
+    path: str
 
     # the parsed contents of kind.yml
-    config = attr.ib(type=dict)
+    config: Dict
 
     # the parameters for this task-graph generation run
-    params = attr.ib(type=Parameters)
+    params: Parameters
 
     # a dict of all the tasks associated with the kind dependencies of the
     # current kind
-    kind_dependencies_tasks = attr.ib(type=dict)
+    kind_dependencies_tasks: Dict[str, Task]
 
     # Global configuration of the taskgraph
-    graph_config = attr.ib(type=GraphConfig)
+    graph_config: GraphConfig
 
     # whether to write out artifacts for the decision task
-    write_artifacts = attr.ib(type=bool)
+    write_artifacts: bool
 
     @property
     @memoize
     def repo_configs(self):
         repositories = self.graph_config["taskgraph"]["repositories"]
         if len(repositories) == 1:
             current_prefix = list(repositories.keys())[0]
@@ -102,27 +103,27 @@
                     for (repo_prefix, repo) in repositories.items()
                     if repo_prefix != current_prefix
                 }
             )
         return repo_configs
 
 
-@attr.s()
+@dataclass()
 class TransformSequence:
     """
     Container for a sequence of transforms.  Each transform is represented as a
     callable taking (config, items) and returning a generator which will yield
     transformed items.  The resulting sequence has the same interface.
 
     This is convenient to use in a file full of transforms, as it provides a
     decorator, @transforms.add, that will add the decorated function to the
     sequence.
     """
 
-    _transforms = attr.ib(factory=list)
+    _transforms: List = field(default_factory=list)
 
     def __call__(self, config, items):
         for xform in self._transforms:
             items = xform(config, items)
             if items is None:
                 raise Exception(f"Transform {xform} is not a generator")
         return items
@@ -131,17 +132,17 @@
         self._transforms.append(func)
         return func
 
     def add_validate(self, schema):
         self.add(ValidateSchema(schema))
 
 
-@attr.s
+@dataclass
 class ValidateSchema:
-    schema = attr.ib(type=Schema)
+    schema: Schema
 
     def __call__(self, config, tasks):
         for task in tasks:
             if "name" in task:
                 error = "In {kind} kind task {name!r}:".format(
                     kind=config.kind, name=task["name"]
                 )
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/cached_tasks.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/code_review.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/code_review.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/docker_image.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/fetch.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/fetch.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,16 +4,17 @@
 
 # Support for running tasks that download remote content and re-export
 # it as task artifacts.
 
 
 import os
 import re
+from dataclasses import dataclass
+from typing import Callable
 
-import attr
 from voluptuous import Extra, Optional, Required
 
 import taskgraph
 
 from ..util import path
 from ..util.cached_tasks import add_optimization
 from ..util.schema import Schema, validate_schema
@@ -52,18 +53,18 @@
 )
 
 
 # define a collection of payload builders, depending on the worker implementation
 fetch_builders = {}
 
 
-@attr.s(frozen=True)
+@dataclass(frozen=True)
 class FetchBuilder:
-    schema = attr.ib(type=Schema)
-    builder = attr.ib()
+    schema: Schema
+    builder: Callable
 
 
 def fetch_builder(name, schema):
     schema = Schema({Required("type"): name}).extend(schema)
 
     def wrap(func):
         fetch_builders[name] = FetchBuilder(schema, func)
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/from_deps.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/from_deps.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/__init__.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/__init__.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/common.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/common.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/index_search.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/index_search.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/run_task.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/run_task.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 """
 Support for running jobs that are invoked via the `run-task` script.
 """
 
-
+import dataclasses
 import os
 
-import attr
 from voluptuous import Any, Extra, Optional, Required
 
 from taskgraph.transforms.job import run_job_using
 from taskgraph.transforms.job.common import support_vcs_checkout
 from taskgraph.transforms.task import taskref_or_string
 from taskgraph.util import path, taskcluster
 from taskgraph.util.schema import Schema
@@ -74,15 +73,15 @@
     run = job["run"]
     if run["checkout"]:
         repo_configs = config.repo_configs
         if len(repo_configs) > 1 and run["checkout"] is True:
             raise Exception("Must explicitly specify checkouts with multiple repos.")
         elif run["checkout"] is not True:
             repo_configs = {
-                repo: attr.evolve(repo_configs[repo], **config)
+                repo: dataclasses.replace(repo_configs[repo], **config)
                 for (repo, config) in run["checkout"].items()
             }
 
         support_vcs_checkout(
             config,
             job,
             taskdesc,
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/job/toolchain.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/job/toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/notify.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/transforms/task.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/transforms/task.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,16 +10,17 @@
 
 
 import hashlib
 import os
 import re
 import time
 from copy import deepcopy
+from dataclasses import dataclass
+from typing import Callable
 
-import attr
 from voluptuous import All, Any, Extra, NotIn, Optional, Required
 
 from taskgraph import MAX_DEPENDENCIES
 from taskgraph.transforms.base import TransformSequence
 from taskgraph.util.hash import hash_path
 from taskgraph.util.keyed_by import evaluate_keyed_by
 from taskgraph.util.memoize import memoize
@@ -220,18 +221,18 @@
     )
 
 
 # define a collection of payload builders, depending on the worker implementation
 payload_builders = {}
 
 
-@attr.s(frozen=True)
+@dataclass(frozen=True)
 class PayloadBuilder:
-    schema = attr.ib(type=Schema)
-    builder = attr.ib()
+    schema: Schema
+    builder: Callable
 
 
 def payload_builder(name, schema):
     schema = Schema({Required("implementation"): name, Optional("os"): str}).extend(
         schema
     )
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/archive.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/archive.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/attributes.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/cached_tasks.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/decision.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/dependencies.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/docker.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/hash.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/hash.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/keyed_by.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/keyed_by.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/memoize.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/parameterization.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/path.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/python_path.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/readonlydict.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/schema.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/shell.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/shell.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/taskcluster.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/taskgraph.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/templates.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/time.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/treeherder.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/vcs.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/verify.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/verify.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,48 +2,48 @@
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
 
 import logging
 import sys
 from abc import ABC, abstractmethod
-
-import attr
+from dataclasses import dataclass, field
+from typing import Callable, Dict, List, Union
 
 from taskgraph.config import GraphConfig
 from taskgraph.parameters import Parameters
 from taskgraph.taskgraph import TaskGraph
 from taskgraph.util.attributes import match_run_on_projects
 from taskgraph.util.treeherder import join_symbol
 
 logger = logging.getLogger(__name__)
 
 
-@attr.s(frozen=True)
+@dataclass(frozen=True)
 class Verification(ABC):
-    func = attr.ib()
+    func: Callable
 
     @abstractmethod
     def verify(self, **kwargs) -> None:
         pass
 
 
-@attr.s(frozen=True)
+@dataclass(frozen=True)
 class InitialVerification(Verification):
     """Verification that doesn't depend on any generation state."""
 
     def verify(self):
         self.func()
 
 
-@attr.s(frozen=True)
+@dataclass(frozen=True)
 class GraphVerification(Verification):
     """Verification for a TaskGraph object."""
 
-    run_on_projects = attr.ib(default=None)
+    run_on_projects: Union[List, None] = field(default=None)
 
     def verify(
         self, graph: TaskGraph, graph_config: GraphConfig, parameters: Parameters
     ):
         if self.run_on_projects and not match_run_on_projects(
             parameters["project"], self.run_on_projects
         ):
@@ -61,41 +61,41 @@
             graph,
             scratch_pad=scratch_pad,
             graph_config=graph_config,
             parameters=parameters,
         )
 
 
-@attr.s(frozen=True)
+@dataclass(frozen=True)
 class ParametersVerification(Verification):
     """Verification for a set of parameters."""
 
     def verify(self, parameters: Parameters):
         self.func(parameters)
 
 
-@attr.s(frozen=True)
+@dataclass(frozen=True)
 class KindsVerification(Verification):
     """Verification for kinds."""
 
     def verify(self, kinds: dict):
         self.func(kinds)
 
 
-@attr.s(frozen=True)
+@dataclass(frozen=True)
 class VerificationSequence:
     """
     Container for a sequence of verifications over a TaskGraph. Each
     verification is represented as a callable taking (task, taskgraph,
     scratch_pad), called for each task in the taskgraph, and one more
     time with no task but with the taskgraph and the same scratch_pad
     that was passed for each task.
     """
 
-    _verifications = attr.ib(factory=dict)
+    _verifications: Dict = field(default_factory=dict)
     _verification_types = {
         "graph": GraphVerification,
         "initial": InitialVerification,
         "kinds": KindsVerification,
         "parameters": ParametersVerification,
     }
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/workertypes.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/workertypes.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # This Source Code Form is subject to the terms of the Mozilla Public
 # License, v. 2.0. If a copy of the MPL was not distributed with this
 # file, You can obtain one at http://mozilla.org/MPL/2.0/.
 
-
-import attr
+from dataclasses import dataclass
 
 from .keyed_by import evaluate_keyed_by
 from .memoize import memoize
 
 
-@attr.s
+@dataclass
 class _BuiltinWorkerType:
-    provisioner = attr.ib(str)
-    worker_type = attr.ib(str)
+    provisioner: str
+    worker_type: str
 
     @property
     def implementation(self):
         """
         Since the list of built-in worker-types is small and fixed, we can get
         away with punning the implementation name (in
         `taskgraph.transforms.task`) and the worker_type.
```

### Comparing `taskcluster-taskgraph-5.3.0/src/taskgraph/util/yaml.py` & `taskcluster-taskgraph-5.4.0/src/taskgraph/util/yaml.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_actions_rebuild_cached_tasks.py` & `taskcluster-taskgraph-5.4.0/test/test_actions_rebuild_cached_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_actions_registry.py` & `taskcluster-taskgraph-5.4.0/test/test_actions_registry.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_create.py` & `taskcluster-taskgraph-5.4.0/test/test_create.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_decision.py` & `taskcluster-taskgraph-5.4.0/test/test_decision.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_files_changed.py` & `taskcluster-taskgraph-5.4.0/test/test_files_changed.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_generator.py` & `taskcluster-taskgraph-5.4.0/test/test_generator.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_graph.py` & `taskcluster-taskgraph-5.4.0/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_main.py` & `taskcluster-taskgraph-5.4.0/test/test_main.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_morph.py` & `taskcluster-taskgraph-5.4.0/test/test_morph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_optimize.py` & `taskcluster-taskgraph-5.4.0/test/test_optimize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_optimize_strategies.py` & `taskcluster-taskgraph-5.4.0/test/test_optimize_strategies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_parameters.py` & `taskcluster-taskgraph-5.4.0/test/test_parameters.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_scripts_fetch_content.py` & `taskcluster-taskgraph-5.4.0/test/test_scripts_fetch_content.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_scripts_run_task.py` & `taskcluster-taskgraph-5.4.0/test/test_scripts_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_target_tasks.py` & `taskcluster-taskgraph-5.4.0/test/test_target_tasks.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_taskgraph.py` & `taskcluster-taskgraph-5.4.0/test/test_taskgraph.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_transform_docker_image.py` & `taskcluster-taskgraph-5.4.0/test/test_transform_docker_image.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_transforms_base.py` & `taskcluster-taskgraph-5.4.0/test/test_transforms_base.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_transforms_fetch.py` & `taskcluster-taskgraph-5.4.0/test/test_transforms_fetch.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_transforms_from_deps.py` & `taskcluster-taskgraph-5.4.0/test/test_transforms_from_deps.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_transforms_job.py` & `taskcluster-taskgraph-5.4.0/test/test_transforms_job.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_transforms_job_run_task.py` & `taskcluster-taskgraph-5.4.0/test/test_transforms_job_run_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_transforms_job_toolchain.py` & `taskcluster-taskgraph-5.4.0/test/test_transforms_job_toolchain.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_transforms_notify.py` & `taskcluster-taskgraph-5.4.0/test/test_transforms_notify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_transforms_task.py` & `taskcluster-taskgraph-5.4.0/test/test_transforms_task.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_attributes.py` & `taskcluster-taskgraph-5.4.0/test/test_util_attributes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_dependencies.py` & `taskcluster-taskgraph-5.4.0/test/test_util_dependencies.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_docker.py` & `taskcluster-taskgraph-5.4.0/test/test_util_docker.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_memoize.py` & `taskcluster-taskgraph-5.4.0/test/test_util_memoize.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_parameterization.py` & `taskcluster-taskgraph-5.4.0/test/test_util_parameterization.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_path.py` & `taskcluster-taskgraph-5.4.0/test/test_util_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_python_path.py` & `taskcluster-taskgraph-5.4.0/test/test_util_python_path.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_readonlydict.py` & `taskcluster-taskgraph-5.4.0/test/test_util_readonlydict.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_schema.py` & `taskcluster-taskgraph-5.4.0/test/test_util_schema.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_taskcluster.py` & `taskcluster-taskgraph-5.4.0/test/test_util_taskcluster.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_templates.py` & `taskcluster-taskgraph-5.4.0/test/test_util_templates.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_time.py` & `taskcluster-taskgraph-5.4.0/test/test_util_time.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_treeherder.py` & `taskcluster-taskgraph-5.4.0/test/test_util_treeherder.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_vcs.py` & `taskcluster-taskgraph-5.4.0/test/test_util_vcs.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_verify.py` & `taskcluster-taskgraph-5.4.0/test/test_util_verify.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_workertypes.py` & `taskcluster-taskgraph-5.4.0/test/test_util_workertypes.py`

 * *Files identical despite different names*

### Comparing `taskcluster-taskgraph-5.3.0/test/test_util_yaml.py` & `taskcluster-taskgraph-5.4.0/test/test_util_yaml.py`

 * *Files identical despite different names*

