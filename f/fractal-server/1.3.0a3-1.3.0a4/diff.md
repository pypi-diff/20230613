# Comparing `tmp/fractal_server-1.3.0a3.tar.gz` & `tmp/fractal_server-1.3.0a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fractal_server-1.3.0a3.tar", max compression
+gzip compressed data, was "fractal_server-1.3.0a4.tar", max compression
```

## Comparing `fractal_server-1.3.0a3.tar` & `fractal_server-1.3.0a4.tar`

### file list

```diff
@@ -1,135 +1,135 @@
--rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.3.0a3/LICENSE
--rw-r--r--   0        0        0     2209 2023-02-24 07:28:35.026213 fractal_server-1.3.0a3/README.md
--rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.3.0a3/fractal_server/.gitignore
--rw-r--r--   0        0        0       24 2023-06-12 06:37:28.730485 fractal_server-1.3.0a3/fractal_server/__init__.py
--rw-r--r--   0        0        0     2202 2023-05-25 12:06:55.503794 fractal_server-1.3.0a3/fractal_server/__main__.py
--rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.3.0a3/fractal_server/alembic.ini
--rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.3.0a3/fractal_server/app/__init__.py
--rw-r--r--   0        0        0      952 2023-05-12 06:48:40.382595 fractal_server-1.3.0a3/fractal_server/app/api/__init__.py
--rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.3.0a3/fractal_server/app/api/v1/__init__.py
--rw-r--r--   0        0        0     6314 2023-05-12 06:48:40.382595 fractal_server-1.3.0a3/fractal_server/app/api/v1/_aux_functions.py
--rw-r--r--   0        0        0     7624 2023-05-23 13:25:45.067972 fractal_server-1.3.0a3/fractal_server/app/api/v1/dataset.py
--rw-r--r--   0        0        0     4817 2023-05-15 12:45:48.614516 fractal_server-1.3.0a3/fractal_server/app/api/v1/job.py
--rw-r--r--   0        0        0     8880 2023-05-15 09:02:05.627121 fractal_server-1.3.0a3/fractal_server/app/api/v1/project.py
--rw-r--r--   0        0        0    15343 2023-06-07 12:54:11.623397 fractal_server-1.3.0a3/fractal_server/app/api/v1/task.py
--rw-r--r--   0        0        0    12501 2023-05-29 15:02:27.725371 fractal_server-1.3.0a3/fractal_server/app/api/v1/workflow.py
--rw-r--r--   0        0        0     3081 2023-05-12 06:48:40.382595 fractal_server-1.3.0a3/fractal_server/app/db/__init__.py
--rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.3.0a3/fractal_server/app/models/__init__.py
--rw-r--r--   0        0        0     3412 2023-05-29 08:51:11.986940 fractal_server-1.3.0a3/fractal_server/app/models/job.py
--rw-r--r--   0        0        0      309 2023-05-12 06:48:40.382595 fractal_server-1.3.0a3/fractal_server/app/models/linkuserproject.py
--rw-r--r--   0        0        0     2355 2023-05-29 08:51:11.986940 fractal_server-1.3.0a3/fractal_server/app/models/project.py
--rw-r--r--   0        0        0     2563 2023-05-29 09:51:02.494983 fractal_server-1.3.0a3/fractal_server/app/models/security.py
--rw-r--r--   0        0        0     1119 2023-05-29 08:51:11.986940 fractal_server-1.3.0a3/fractal_server/app/models/state.py
--rw-r--r--   0        0        0     1591 2023-06-08 09:21:57.166713 fractal_server-1.3.0a3/fractal_server/app/models/task.py
--rw-r--r--   0        0        0     5948 2023-06-08 09:22:21.105956 fractal_server-1.3.0a3/fractal_server/app/models/workflow.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a3/fractal_server/app/runner/.gitignore
--rw-r--r--   0        0        0     8969 2023-05-15 10:36:57.758906 fractal_server-1.3.0a3/fractal_server/app/runner/__init__.py
--rw-r--r--   0        0        0    19523 2023-06-08 09:22:21.105956 fractal_server-1.3.0a3/fractal_server/app/runner/_common.py
--rw-r--r--   0        0        0     5464 2023-05-12 12:34:32.122055 fractal_server-1.3.0a3/fractal_server/app/runner/_local/__init__.py
--rw-r--r--   0        0        0     3273 2023-04-17 13:34:24.748408 fractal_server-1.3.0a3/fractal_server/app/runner/_local/_local_config.py
--rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.3.0a3/fractal_server/app/runner/_local/_submit_setup.py
--rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.3.0a3/fractal_server/app/runner/_local/executor.py
--rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/.gitignore
--rw-r--r--   0        0        0     3839 2023-05-12 12:34:32.122055 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/__init__.py
--rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_batching.py
--rw-r--r--   0        0        0     4331 2023-05-15 10:36:57.758906 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_executor_wait_thread.py
--rw-r--r--   0        0        0    19861 2023-05-12 06:48:40.382595 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_slurm_config.py
--rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_submit_setup.py
--rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
--rw-r--r--   0        0        0    42200 2023-05-18 09:57:35.703959 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/executor.py
--rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/remote.py
--rw-r--r--   0        0        0     7900 2023-06-08 08:33:26.930560 fractal_server-1.3.0a3/fractal_server/app/runner/common.py
--rw-r--r--   0        0        0    11324 2023-05-12 06:48:40.382595 fractal_server-1.3.0a3/fractal_server/app/security/__init__.py
--rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.3.0a3/fractal_server/common/.git
--rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/.github/workflows/ci.yml
--rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.3.0a3/fractal_server/common/.github/workflows/project-management.yml
--rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/.gitignore
--rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.3.0a3/fractal_server/common/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/README.md
--rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.3.0a3/fractal_server/common/__init__.py
--rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.3.0a3/fractal_server/common/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.3.0a3/fractal_server/common/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0       57 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/requirements.txt
--rw-r--r--   0        0        0      614 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/schemas/__init__.py
--rw-r--r--   0        0        0      425 2023-05-26 06:49:50.432129 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
--rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
--rw-r--r--   0        0        0     1624 2023-05-26 06:49:50.432129 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
--rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
--rw-r--r--   0        0        0     4082 2023-06-06 13:10:35.738263 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
--rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
--rw-r--r--   0        0        0     3551 2023-05-26 06:49:50.436129 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
--rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
--rw-r--r--   0        0        0     1179 2023-05-26 06:49:50.444129 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
--rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0     2719 2023-06-06 13:10:35.746263 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
--rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
--rw-r--r--   0        0        0     3112 2023-05-26 06:49:50.448129 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
--rw-r--r--   0        0        0     1216 2023-05-26 06:49:50.448129 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
--rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
--rw-r--r--   0        0        0     3896 2023-05-26 06:49:50.452129 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
--rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
--rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/schemas/_validators.py
--rw-r--r--   0        0        0     1117 2023-05-26 06:47:44.353797 fractal_server-1.3.0a3/fractal_server/common/schemas/applyworkflow.py
--rw-r--r--   0        0        0     3479 2023-06-06 13:04:16.393219 fractal_server-1.3.0a3/fractal_server/common/schemas/manifest.py
--rw-r--r--   0        0        0     2483 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/schemas/project.py
--rw-r--r--   0        0        0      673 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/schemas/state.py
--rw-r--r--   0        0        0     2578 2023-06-06 13:04:16.393219 fractal_server-1.3.0a3/fractal_server/common/schemas/task.py
--rw-r--r--   0        0        0     2741 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/schemas/task_collection.py
--rw-r--r--   0        0        0     1216 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/schemas/user.py
--rw-r--r--   0        0        0     2457 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/schemas/workflow.py
--rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0      620 2023-05-09 18:15:54.737187 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1255 2023-06-06 07:10:27.608505 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2806 2023-05-26 06:49:50.864124 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1238 2023-05-26 06:49:50.868124 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2685 2023-05-26 06:49:50.868124 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
--rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
--rw-r--r--   0        0        0     2925 2023-05-09 18:15:54.765188 fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
--rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/tests/conftest.py
--rw-r--r--   0        0        0      298 2023-05-09 11:24:30.681084 fractal_server-1.3.0a3/fractal_server/common/tests/test_applyworkflow.py
--rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/tests/test_dataset.py
--rw-r--r--   0        0        0     1420 2023-06-06 07:08:01.329849 fractal_server-1.3.0a3/fractal_server/common/tests/test_manifest.py
--rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/tests/test_project.py
--rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.3.0a3/fractal_server/common/tests/test_state.py
--rw-r--r--   0        0        0     1190 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/tests/test_task.py
--rw-r--r--   0        0        0      773 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/tests/test_task_collection.py
--rw-r--r--   0        0        0     1499 2023-05-26 06:41:57.297956 fractal_server-1.3.0a3/fractal_server/common/tests/test_user.py
--rw-r--r--   0        0        0     2596 2023-05-09 11:24:30.681084 fractal_server-1.3.0a3/fractal_server/common/tests/test_workflow.py
--rw-r--r--   0        0        0    12164 2023-05-12 12:34:32.122055 fractal_server-1.3.0a3/fractal_server/config.py
--rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.3.0a3/fractal_server/logger.py
--rw-r--r--   0        0        0     5849 2023-05-26 06:42:41.017595 fractal_server-1.3.0a3/fractal_server/main.py
--rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.3.0a3/fractal_server/migrations/README
--rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.3.0a3/fractal_server/migrations/env.py
--rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.3.0a3/fractal_server/migrations/script.py.mako
--rw-r--r--   0        0        0      954 2023-06-08 09:21:57.166713 fractal_server-1.3.0a3/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
--rw-r--r--   0        0        0     8770 2023-05-29 15:02:27.725371 fractal_server-1.3.0a3/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
--rw-r--r--   0        0        0      746 2023-06-08 09:21:57.166713 fractal_server-1.3.0a3/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
--rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.3.0a3/fractal_server/py.typed
--rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.3.0a3/fractal_server/syringe.py
--rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.3.0a3/fractal_server/tasks/__init__.py
--rw-r--r--   0        0        0    15725 2023-06-12 06:36:49.598978 fractal_server-1.3.0a3/fractal_server/tasks/collection.py
--rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.3.0a3/fractal_server/utils.py
--rw-r--r--   0        0        0     2689 2023-06-12 06:37:28.726485 fractal_server-1.3.0a3/pyproject.toml
--rw-r--r--   0        0        0     3631 1970-01-01 00:00:00.000000 fractal_server-1.3.0a3/PKG-INFO
+-rw-r--r--   0        0        0     1576 2022-09-07 11:17:53.820970 fractal_server-1.3.0a4/LICENSE
+-rw-r--r--   0        0        0     2092 2023-06-12 14:11:09.525929 fractal_server-1.3.0a4/README.md
+-rw-r--r--   0        0        0       69 2022-09-07 11:17:53.836969 fractal_server-1.3.0a4/fractal_server/.gitignore
+-rw-r--r--   0        0        0       24 2023-06-12 14:14:41.047872 fractal_server-1.3.0a4/fractal_server/__init__.py
+-rw-r--r--   0        0        0     2202 2023-05-25 12:06:55.503794 fractal_server-1.3.0a4/fractal_server/__main__.py
+-rw-r--r--   0        0        0     3153 2023-02-22 13:06:13.003243 fractal_server-1.3.0a4/fractal_server/alembic.ini
+-rw-r--r--   0        0        0        0 2022-09-07 11:17:53.836969 fractal_server-1.3.0a4/fractal_server/app/__init__.py
+-rw-r--r--   0        0        0      952 2023-05-12 06:48:40.382595 fractal_server-1.3.0a4/fractal_server/app/api/__init__.py
+-rw-r--r--   0        0        0       24 2023-02-22 13:06:13.003243 fractal_server-1.3.0a4/fractal_server/app/api/v1/__init__.py
+-rw-r--r--   0        0        0     6314 2023-05-12 06:48:40.382595 fractal_server-1.3.0a4/fractal_server/app/api/v1/_aux_functions.py
+-rw-r--r--   0        0        0     7624 2023-05-23 13:25:45.067972 fractal_server-1.3.0a4/fractal_server/app/api/v1/dataset.py
+-rw-r--r--   0        0        0     4817 2023-05-15 12:45:48.614516 fractal_server-1.3.0a4/fractal_server/app/api/v1/job.py
+-rw-r--r--   0        0        0     8880 2023-05-15 09:02:05.627121 fractal_server-1.3.0a4/fractal_server/app/api/v1/project.py
+-rw-r--r--   0        0        0    15343 2023-06-07 12:54:11.623397 fractal_server-1.3.0a4/fractal_server/app/api/v1/task.py
+-rw-r--r--   0        0        0    12501 2023-05-29 15:02:27.725371 fractal_server-1.3.0a4/fractal_server/app/api/v1/workflow.py
+-rw-r--r--   0        0        0     3081 2023-05-12 06:48:40.382595 fractal_server-1.3.0a4/fractal_server/app/db/__init__.py
+-rw-r--r--   0        0        0      372 2023-03-16 13:58:42.445129 fractal_server-1.3.0a4/fractal_server/app/models/__init__.py
+-rw-r--r--   0        0        0     3412 2023-05-29 08:51:11.986940 fractal_server-1.3.0a4/fractal_server/app/models/job.py
+-rw-r--r--   0        0        0      309 2023-05-12 06:48:40.382595 fractal_server-1.3.0a4/fractal_server/app/models/linkuserproject.py
+-rw-r--r--   0        0        0     2355 2023-05-29 08:51:11.986940 fractal_server-1.3.0a4/fractal_server/app/models/project.py
+-rw-r--r--   0        0        0     2563 2023-05-29 09:51:02.494983 fractal_server-1.3.0a4/fractal_server/app/models/security.py
+-rw-r--r--   0        0        0     1119 2023-05-29 08:51:11.986940 fractal_server-1.3.0a4/fractal_server/app/models/state.py
+-rw-r--r--   0        0        0     1591 2023-06-08 09:21:57.166713 fractal_server-1.3.0a4/fractal_server/app/models/task.py
+-rw-r--r--   0        0        0     5948 2023-06-08 09:22:21.105956 fractal_server-1.3.0a4/fractal_server/app/models/workflow.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a4/fractal_server/app/runner/.gitignore
+-rw-r--r--   0        0        0     8969 2023-05-15 10:36:57.758906 fractal_server-1.3.0a4/fractal_server/app/runner/__init__.py
+-rw-r--r--   0        0        0    19523 2023-06-08 09:22:21.105956 fractal_server-1.3.0a4/fractal_server/app/runner/_common.py
+-rw-r--r--   0        0        0     5464 2023-05-12 12:34:32.122055 fractal_server-1.3.0a4/fractal_server/app/runner/_local/__init__.py
+-rw-r--r--   0        0        0     3273 2023-04-17 13:34:24.748408 fractal_server-1.3.0a4/fractal_server/app/runner/_local/_local_config.py
+-rw-r--r--   0        0        0     1631 2023-04-17 13:34:24.748408 fractal_server-1.3.0a4/fractal_server/app/runner/_local/_submit_setup.py
+-rw-r--r--   0        0        0     3620 2023-04-17 13:34:24.748408 fractal_server-1.3.0a4/fractal_server/app/runner/_local/executor.py
+-rw-r--r--   0        0        0       16 2023-04-11 12:05:21.017629 fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/.gitignore
+-rw-r--r--   0        0        0     3839 2023-05-12 12:34:32.122055 fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/__init__.py
+-rw-r--r--   0        0        0     8840 2023-04-14 12:55:14.842206 fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/_batching.py
+-rw-r--r--   0        0        0     4331 2023-05-15 10:36:57.758906 fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/_executor_wait_thread.py
+-rw-r--r--   0        0        0    19861 2023-05-12 06:48:40.382595 fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/_slurm_config.py
+-rw-r--r--   0        0        0     2942 2023-04-11 12:05:21.021629 fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/_submit_setup.py
+-rw-r--r--   0        0        0     4534 2023-05-03 10:33:21.774484 fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py
+-rw-r--r--   0        0        0    42200 2023-05-18 09:57:35.703959 fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/executor.py
+-rw-r--r--   0        0        0     5852 2023-04-14 08:31:16.571080 fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/remote.py
+-rw-r--r--   0        0        0     7900 2023-06-08 08:33:26.930560 fractal_server-1.3.0a4/fractal_server/app/runner/common.py
+-rw-r--r--   0        0        0    11324 2023-05-12 06:48:40.382595 fractal_server-1.3.0a4/fractal_server/app/security/__init__.py
+-rw-r--r--   0        0        0       49 2023-02-22 11:04:15.289972 fractal_server-1.3.0a4/fractal_server/common/.git
+-rw-r--r--   0        0        0      717 2023-05-08 12:01:46.018194 fractal_server-1.3.0a4/fractal_server/common/.github/workflows/ci.yml
+-rw-r--r--   0        0        0      364 2023-02-22 11:04:15.289972 fractal_server-1.3.0a4/fractal_server/common/.github/workflows/project-management.yml
+-rw-r--r--   0        0        0       34 2023-05-08 12:01:46.018194 fractal_server-1.3.0a4/fractal_server/common/.gitignore
+-rw-r--r--   0        0        0      620 2023-02-22 11:04:15.289972 fractal_server-1.3.0a4/fractal_server/common/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1964 2023-05-08 12:01:46.018194 fractal_server-1.3.0a4/fractal_server/common/README.md
+-rw-r--r--   0        0        0        0 2023-02-22 11:04:15.289972 fractal_server-1.3.0a4/fractal_server/common/__init__.py
+-rw-r--r--   0        0        0      163 2023-02-22 12:30:35.511172 fractal_server-1.3.0a4/fractal_server/common/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      179 2023-02-23 12:52:36.416846 fractal_server-1.3.0a4/fractal_server/common/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0       57 2023-05-26 06:41:57.297956 fractal_server-1.3.0a4/fractal_server/common/requirements.txt
+-rw-r--r--   0        0        0      614 2023-05-26 06:41:57.297956 fractal_server-1.3.0a4/fractal_server/common/schemas/__init__.py
+-rw-r--r--   0        0        0      425 2023-05-26 06:49:50.432129 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0      593 2023-02-23 12:52:36.416846 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0      504 2023-03-03 14:24:46.376001 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/_validator.cpython-310.pyc
+-rw-r--r--   0        0        0     1767 2023-05-08 12:02:12.593892 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc
+-rw-r--r--   0        0        0     1624 2023-06-12 09:13:31.352825 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc
+-rw-r--r--   0        0        0     2325 2023-02-23 12:52:36.416846 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc
+-rw-r--r--   0        0        0     4082 2023-06-12 09:13:31.356825 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc
+-rw-r--r--   0        0        0     4433 2023-02-23 12:52:36.420846 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc
+-rw-r--r--   0        0        0     3551 2023-05-26 06:49:50.436129 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc
+-rw-r--r--   0        0        0     5221 2023-02-23 12:52:36.420846 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc
+-rw-r--r--   0        0        0     1179 2023-05-26 06:49:50.444129 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc
+-rw-r--r--   0        0        0     1877 2023-02-23 12:52:36.428846 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc
+-rw-r--r--   0        0        0     2719 2023-06-12 09:13:31.364825 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc
+-rw-r--r--   0        0        0     6570 2023-02-23 12:52:36.428846 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc
+-rw-r--r--   0        0        0     3306 2023-06-12 09:13:31.368826 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc
+-rw-r--r--   0        0        0     1216 2023-05-26 06:49:50.448129 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc
+-rw-r--r--   0        0        0     1200 2023-02-23 12:52:36.432846 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc
+-rw-r--r--   0        0        0     3896 2023-05-26 06:49:50.452129 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc
+-rw-r--r--   0        0        0     4596 2023-02-23 12:52:36.432846 fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc
+-rw-r--r--   0        0        0     1616 2023-05-08 12:01:46.018194 fractal_server-1.3.0a4/fractal_server/common/schemas/_validators.py
+-rw-r--r--   0        0        0     1117 2023-06-12 09:12:04.406676 fractal_server-1.3.0a4/fractal_server/common/schemas/applyworkflow.py
+-rw-r--r--   0        0        0     3479 2023-06-12 09:12:04.406676 fractal_server-1.3.0a4/fractal_server/common/schemas/manifest.py
+-rw-r--r--   0        0        0     2483 2023-05-26 06:41:57.297956 fractal_server-1.3.0a4/fractal_server/common/schemas/project.py
+-rw-r--r--   0        0        0      673 2023-05-26 06:41:57.297956 fractal_server-1.3.0a4/fractal_server/common/schemas/state.py
+-rw-r--r--   0        0        0     2578 2023-06-12 09:12:04.406676 fractal_server-1.3.0a4/fractal_server/common/schemas/task.py
+-rw-r--r--   0        0        0     2935 2023-06-12 09:12:04.406676 fractal_server-1.3.0a4/fractal_server/common/schemas/task_collection.py
+-rw-r--r--   0        0        0     1216 2023-05-26 06:41:57.297956 fractal_server-1.3.0a4/fractal_server/common/schemas/user.py
+-rw-r--r--   0        0        0     2457 2023-05-26 06:41:57.297956 fractal_server-1.3.0a4/fractal_server/common/schemas/workflow.py
+-rw-r--r--   0        0        0      429 2023-03-09 14:38:27.388159 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      429 2023-03-24 12:58:52.898563 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      429 2023-05-08 12:02:12.937888 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/conftest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-09 14:38:27.444159 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1592 2023-03-24 12:58:52.954562 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0      620 2023-05-09 18:15:54.737187 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-15 08:26:08.661090 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3396 2023-03-24 12:58:52.978562 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     3396 2023-05-08 12:02:13.009887 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-09 14:38:27.472158 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0      873 2023-03-24 12:58:52.978562 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1255 2023-06-06 07:10:27.608505 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1272 2023-03-15 08:26:08.665089 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1178 2023-04-06 08:33:24.349041 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1178 2023-05-08 12:02:13.013887 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-09 14:38:27.476158 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     1777 2023-03-24 12:58:52.982562 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     1777 2023-05-08 12:02:13.013887 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-09 14:38:27.480158 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2236 2023-03-24 12:58:52.982562 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2806 2023-05-26 06:49:50.864124 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1238 2023-05-26 06:49:50.868124 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     1331 2023-03-09 14:38:27.480158 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     2227 2023-04-06 08:33:24.353041 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2685 2023-05-26 06:49:50.868124 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0     2593 2023-03-09 14:38:27.480158 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc
+-rw-r--r--   0        0        0     3046 2023-03-24 12:58:52.986562 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc
+-rw-r--r--   0        0        0     2925 2023-05-09 18:15:54.765188 fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc
+-rw-r--r--   0        0        0      139 2023-05-08 12:01:46.018194 fractal_server-1.3.0a4/fractal_server/common/tests/conftest.py
+-rw-r--r--   0        0        0      298 2023-05-09 11:24:30.681084 fractal_server-1.3.0a4/fractal_server/common/tests/test_applyworkflow.py
+-rw-r--r--   0        0        0     2144 2023-05-08 12:01:46.018194 fractal_server-1.3.0a4/fractal_server/common/tests/test_dataset.py
+-rw-r--r--   0        0        0     1420 2023-06-12 09:12:04.406676 fractal_server-1.3.0a4/fractal_server/common/tests/test_manifest.py
+-rw-r--r--   0        0        0      525 2023-05-08 12:01:46.018194 fractal_server-1.3.0a4/fractal_server/common/tests/test_project.py
+-rw-r--r--   0        0        0      551 2023-05-08 12:01:46.018194 fractal_server-1.3.0a4/fractal_server/common/tests/test_state.py
+-rw-r--r--   0        0        0     1190 2023-05-26 06:41:57.297956 fractal_server-1.3.0a4/fractal_server/common/tests/test_task.py
+-rw-r--r--   0        0        0      968 2023-06-12 09:12:04.410676 fractal_server-1.3.0a4/fractal_server/common/tests/test_task_collection.py
+-rw-r--r--   0        0        0     1499 2023-05-26 06:41:57.297956 fractal_server-1.3.0a4/fractal_server/common/tests/test_user.py
+-rw-r--r--   0        0        0     2596 2023-05-09 11:24:30.681084 fractal_server-1.3.0a4/fractal_server/common/tests/test_workflow.py
+-rw-r--r--   0        0        0    12164 2023-05-12 12:34:32.122055 fractal_server-1.3.0a4/fractal_server/config.py
+-rw-r--r--   0        0        0     4562 2023-04-14 12:55:14.846206 fractal_server-1.3.0a4/fractal_server/logger.py
+-rw-r--r--   0        0        0     5849 2023-05-26 06:42:41.017595 fractal_server-1.3.0a4/fractal_server/main.py
+-rw-r--r--   0        0        0       59 2022-09-08 11:49:20.993046 fractal_server-1.3.0a4/fractal_server/migrations/README
+-rw-r--r--   0        0        0     2330 2023-02-22 13:06:13.007243 fractal_server-1.3.0a4/fractal_server/migrations/env.py
+-rw-r--r--   0        0        0      550 2022-09-08 11:49:30.768918 fractal_server-1.3.0a4/fractal_server/migrations/script.py.mako
+-rw-r--r--   0        0        0      954 2023-06-08 09:21:57.166713 fractal_server-1.3.0a4/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py
+-rw-r--r--   0        0        0     8770 2023-05-29 15:02:27.725371 fractal_server-1.3.0a4/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py
+-rw-r--r--   0        0        0      746 2023-06-08 09:21:57.166713 fractal_server-1.3.0a4/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py
+-rw-r--r--   0        0        0        0 2022-11-02 11:51:16.322067 fractal_server-1.3.0a4/fractal_server/py.typed
+-rw-r--r--   0        0        0     2786 2023-04-11 12:05:21.021629 fractal_server-1.3.0a4/fractal_server/syringe.py
+-rw-r--r--   0        0        0       72 2023-04-11 12:05:21.021629 fractal_server-1.3.0a4/fractal_server/tasks/__init__.py
+-rw-r--r--   0        0        0    17581 2023-06-12 14:10:58.230055 fractal_server-1.3.0a4/fractal_server/tasks/collection.py
+-rw-r--r--   0        0        0     2115 2023-05-03 10:43:26.232421 fractal_server-1.3.0a4/fractal_server/utils.py
+-rw-r--r--   0        0        0     2689 2023-06-12 14:14:41.047872 fractal_server-1.3.0a4/pyproject.toml
+-rw-r--r--   0        0        0     3514 1970-01-01 00:00:00.000000 fractal_server-1.3.0a4/PKG-INFO
```

### Comparing `fractal_server-1.3.0a3/LICENSE` & `fractal_server-1.3.0a4/LICENSE`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/README.md` & `fractal_server-1.3.0a4/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -30,10 +30,8 @@
 [@sampsyo](https://github.com/sampsyo) and collaborators, and it is released
 under the terms of the MIT license.
 
 Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute
 for Biomedical Research and in the Pelkmans Lab at the University of Zurich
 (both in Switzerland). The project lead is with
 [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi).
-The core development is done under contract by
-[@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa)
-& [@japs](https://github.com/japs) of [eXact lab S.r.l.](exact-lab.it).
+The core development is done under contract by [eXact lab S.r.l.](exact-lab.it).
```

### Comparing `fractal_server-1.3.0a3/fractal_server/__main__.py` & `fractal_server-1.3.0a4/fractal_server/__main__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/alembic.ini` & `fractal_server-1.3.0a4/fractal_server/alembic.ini`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/api/__init__.py` & `fractal_server-1.3.0a4/fractal_server/app/api/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/api/v1/_aux_functions.py` & `fractal_server-1.3.0a4/fractal_server/app/api/v1/_aux_functions.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/api/v1/dataset.py` & `fractal_server-1.3.0a4/fractal_server/app/api/v1/dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/api/v1/job.py` & `fractal_server-1.3.0a4/fractal_server/app/api/v1/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/api/v1/project.py` & `fractal_server-1.3.0a4/fractal_server/app/api/v1/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/api/v1/task.py` & `fractal_server-1.3.0a4/fractal_server/app/api/v1/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/api/v1/workflow.py` & `fractal_server-1.3.0a4/fractal_server/app/api/v1/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/db/__init__.py` & `fractal_server-1.3.0a4/fractal_server/app/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/models/job.py` & `fractal_server-1.3.0a4/fractal_server/app/models/job.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/models/project.py` & `fractal_server-1.3.0a4/fractal_server/app/models/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/models/security.py` & `fractal_server-1.3.0a4/fractal_server/app/models/security.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/models/state.py` & `fractal_server-1.3.0a4/fractal_server/app/models/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/models/task.py` & `fractal_server-1.3.0a4/fractal_server/app/models/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/models/workflow.py` & `fractal_server-1.3.0a4/fractal_server/app/models/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/__init__.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/_common.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/_common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/_local/__init__.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/_local/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/_local/_local_config.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/_local/_local_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/_local/_submit_setup.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/_local/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/_local/executor.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/_local/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/__init__.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_batching.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/_batching.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_executor_wait_thread.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/_executor_wait_thread.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_slurm_config.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/_slurm_config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_submit_setup.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/_submit_setup.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/_subprocess_run_as_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/executor.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/executor.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/_slurm/remote.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/_slurm/remote.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/runner/common.py` & `fractal_server-1.3.0a4/fractal_server/app/runner/common.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/app/security/__init__.py` & `fractal_server-1.3.0a4/fractal_server/app/security/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/.github/workflows/ci.yml` & `fractal_server-1.3.0a4/fractal_server/common/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/.pre-commit-config.yaml` & `fractal_server-1.3.0a4/fractal_server/common/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/README.md` & `fractal_server-1.3.0a4/fractal_server/common/README.md`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__init__.py` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/__init__.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/_validators.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 26 06:47:44 2023 UTC, .py size: 1117 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 1056 7064 5d04 0000  o........Vpd]...
+00000000: 6f0d 0d0a 0000 0000 64e1 8664 5d04 0000  o.......d..d]...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 7400 0000 6400  .....@...st...d.
 00000030: 6401 6c00 6d00 5a00 0100 6400 6402 6c01  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6405  ..d.d.l.m.Z...d.
 00000060: 6406 6c06 6d07 5a07 0100 6407 5a08 4700  d.l.m.Z...d.Z.G.
 00000070: 6408 6409 8400 6409 6504 8303 5a09 4700  d.d...d.e...Z.G.
```

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/applyworkflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/manifest.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun  6 13:04:16 2023 UTC, .py size: 3479 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 d02e 7f64 970d 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 64e1 8664 970d 0000  o.......d..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 a800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c00 6d03 5a03  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c04 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c04 6d06 5a06 0100 6400 6406 6c04  d.l.m.Z...d.d.l.
 00000070: 6d07 5a07 0100 6400 6407 6c04 6d08 5a08  m.Z...d.d.l.m.Z.
```

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/manifest.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/project.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/project.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/state.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/state.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/task.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Tue Jun  6 13:04:16 2023 UTC, .py size: 2578 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 d02e 7f64 120a 0000  o..........d....
+00000000: 6f0d 0d0a 0000 0000 64e1 8664 120a 0000  o.......d..d....
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 b000 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c00  d.l.m.Z...d.d.l.
 00000040: 6d02 5a02 0100 6400 6403 6c03 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c03 6d05 5a05 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c03 6d06 5a06 0100 6406 6407 6c07  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6408 5a09 4700 6409 640a  m.Z...d.Z.G.d.d.
```

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/task.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/task_collection.cpython-310.pyc`

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.10, timestamp-based, .py timestamp: Fri May 26 06:41:57 2023 UTC, .py size: 2741 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-00000000: 6f0d 0d0a 0000 0000 b554 7064 b50a 0000  o........Tpd....
+00000000: 6f0d 0d0a 0000 0000 64e1 8664 770b 0000  o.......d..dw...
 00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
 00000020: 0004 0000 0040 0000 0073 9800 0000 6400  .....@...s....d.
 00000030: 6401 6c00 6d01 5a01 0100 6400 6402 6c02  d.l.m.Z...d.d.l.
 00000040: 6d03 5a03 0100 6400 6403 6c02 6d04 5a04  m.Z...d.d.l.m.Z.
 00000050: 0100 6400 6404 6c05 6d06 5a06 0100 6400  ..d.d.l.m.Z...d.
 00000060: 6405 6c05 6d07 5a07 0100 6400 6406 6c05  d.l.m.Z...d.d.l.
 00000070: 6d08 5a08 0100 6407 6408 6c09 6d0a 5a0a  m.Z...d.d.l.m.Z.
@@ -30,166 +30,178 @@
 000001d0: 4672 6163 7461 6c2f 6672 6163 7461 6c2d  Fractal/fractal-
 000001e0: 7365 7276 6572 2f66 7261 6374 616c 5f73  server/fractal_s
 000001f0: 6572 7665 722f 636f 6d6d 6f6e 2f73 6368  erver/common/sch
 00000200: 656d 6173 2f74 6173 6b5f 636f 6c6c 6563  emas/task_collec
 00000210: 7469 6f6e 2e70 7972 0d00 0000 1200 0000  tion.pyr........
 00000220: 7304 0000 0008 0004 0172 0d00 0000 6300  s........r....c.
 00000230: 0000 0000 0000 0000 0000 0000 0000 0004  ................
-00000240: 0000 0040 0000 0073 9600 0000 6500 5a01  ...@...s....e.Z.
+00000240: 0000 0040 0000 0073 ae00 0000 6500 5a01  ...@...s....e.Z.
 00000250: 6400 5a02 5500 6401 5a03 6504 6505 6402  d.Z.U.d.Z.e.e.d.
 00000260: 3c00 6403 5a06 6507 6504 1900 6505 6404  <.d.Z.e.e...e.d.
 00000270: 3c00 6403 5a08 6507 6504 1900 6505 6405  <.d.Z.e.e...e.d.
 00000280: 3c00 6403 5a09 6507 6504 1900 6505 6406  <.d.Z.e.e...e.d.
-00000290: 3c00 650a 6404 6407 6408 8d02 650b 6404  <.e.d.d.d...e.d.
-000002a0: 8301 8301 5a0c 650a 6405 6407 6408 8d02  ....Z.e.d.d.d...
-000002b0: 650b 6405 8301 8301 5a0d 650a 6406 6407  e.d.....Z.e.d.d.
-000002c0: 6408 8d02 650b 6406 8301 8301 5a0e 650a  d...e.d.....Z.e.
-000002d0: 6402 8301 6409 640a 8400 8301 5a0f 6403  d...d.d.....Z.d.
-000002e0: 5300 290b 720b 0000 0061 e002 0000 0a20  S.).r....a..... 
-000002f0: 2020 2054 6173 6b43 6f6c 6c65 6374 5069     TaskCollectPi
-00000300: 7020 636c 6173 730a 0a20 2020 2054 6869  p class..    Thi
-00000310: 7320 636c 6173 7320 6f6e 6c79 2065 6e63  s class only enc
-00000320: 6f64 6573 2074 6865 2061 7474 7269 6275  odes the attribu
-00000330: 7465 7320 7265 7175 6972 6564 2074 6f20  tes required to 
-00000340: 7472 6967 6765 7220 610a 2020 2020 7461  trigger a.    ta
-00000350: 736b 2d63 6f6c 6c65 6374 696f 6e20 6f70  sk-collection op
-00000360: 6572 6174 696f 6e2e 204f 7468 6572 2061  eration. Other a
-00000370: 7474 7269 6275 7465 7320 2874 6861 7420  ttributes (that 
-00000380: 6172 6520 6173 7369 676e 6564 202a 6475  are assigned *du
-00000390: 7269 6e67 2a0a 2020 2020 7461 736b 2063  ring*.    task c
-000003a0: 6f6c 6c65 6374 696f 6e29 2061 7265 2064  ollection) are d
-000003b0: 6566 696e 6564 2061 7320 7061 7274 206f  efined as part o
-000003c0: 6620 6672 6163 7461 6c2d 7365 7276 6572  f fractal-server
-000003d0: 2e0a 0a20 2020 2054 776f 2063 6173 6573  ...    Two cases
-000003e0: 2061 7265 2073 7570 706f 7274 6564 3a0a   are supported:.
-000003f0: 0a20 2020 2020 2020 2031 2e20 6070 6163  .        1. `pac
-00000400: 6b61 6765 6020 6973 2074 6865 2070 6174  kage` is the pat
-00000410: 6820 6f66 2061 206c 6f63 616c 2077 6865  h of a local whe
-00000420: 656c 2066 696c 653b 0a20 2020 2020 2020  el file;.       
-00000430: 2032 2e20 6070 6163 6b61 6765 6020 6973   2. `package` is
-00000440: 2074 6865 206e 616d 6520 6f66 2061 2070   the name of a p
-00000450: 6163 6b61 6765 2074 6861 7420 6361 6e20  ackage that can 
-00000460: 6265 2069 6e73 7461 6c6c 6564 2076 6961  be installed via
-00000470: 2060 7069 7060 2e0a 0a0a 2020 2020 4174   `pip`....    At
-00000480: 7472 6962 7574 6573 3a0a 2020 2020 2020  tributes:.      
-00000490: 2020 7061 636b 6167 653a 0a20 2020 2020    package:.     
-000004a0: 2020 2020 2020 2054 6865 206e 616d 6520         The name 
-000004b0: 6f66 2061 2060 7069 7060 2d69 6e73 7461  of a `pip`-insta
-000004c0: 6c6c 6162 6c65 2070 6163 6b61 6765 2c20  llable package, 
-000004d0: 6f72 2074 6865 2070 6174 6820 746f 2061  or the path to a
-000004e0: 206c 6f63 616c 0a20 2020 2020 2020 2020   local.         
-000004f0: 2020 2077 6865 656c 2066 696c 652e 0a20     wheel file.. 
-00000500: 2020 2020 2020 2070 6163 6b61 6765 5f76         package_v
-00000510: 6572 7369 6f6e 3a20 5665 7273 696f 6e20  ersion: Version 
-00000520: 6f66 2074 6865 2070 6163 6b61 6765 0a20  of the package. 
-00000530: 2020 2020 2020 2070 6163 6b61 6765 5f65         package_e
-00000540: 7874 7261 733a 2050 6163 6b61 6765 2065  xtras: Package e
-00000550: 7874 7261 7320 746f 2069 6e63 6c75 6465  xtras to include
-00000560: 2069 6e20 7468 6520 6070 6970 2069 6e73   in the `pip ins
-00000570: 7461 6c6c 6020 636f 6d6d 616e 640a 2020  tall` command.  
-00000580: 2020 2020 2020 7079 7468 6f6e 5f76 6572        python_ver
-00000590: 7369 6f6e 3a20 5079 7468 6f6e 2076 6572  sion: Python ver
-000005a0: 7369 6f6e 2074 6f20 696e 7374 616c 6c20  sion to install 
-000005b0: 616e 6420 7275 6e20 7468 6520 7061 636b  and run the pack
-000005c0: 6167 6520 7461 736b 730a 2020 2020 da07  age tasks.    ..
-000005d0: 7061 636b 6167 654e da0f 7061 636b 6167  packageN..packag
-000005e0: 655f 7665 7273 696f 6eda 0e70 6163 6b61  e_version..packa
-000005f0: 6765 5f65 7874 7261 73da 0e70 7974 686f  ge_extras..pytho
-00000600: 6e5f 7665 7273 696f 6e54 2901 da0b 616c  n_versionT)...al
-00000610: 6c6f 775f 7265 7573 6563 0200 0000 0000  low_reusec......
-00000620: 0000 0000 0000 0200 0000 0400 0000 4300  ..............C.
-00000630: 0000 7342 0000 0064 017c 0176 0072 1f7c  ..sB...d.|.v.r.|
-00000640: 01a0 0064 02a1 0173 1174 0164 037c 019b  ...d...s.t.d.|..
-00000650: 0064 049d 0383 0182 0174 027c 0183 01a0  .d.......t.|....
-00000660: 03a1 0073 1f74 0164 057c 019b 0064 049d  ...s.t.d.|...d..
-00000670: 0383 0182 017c 0153 0029 064e fa01 2f7a  .....|.S.).N../z
-00000680: 042e 7768 6c7a 2f4c 6f63 616c 2d70 6163  ..whlz/Local-pac
-00000690: 6b61 6765 2070 6174 6820 6d75 7374 2062  kage path must b
-000006a0: 6520 6120 7768 6565 6c20 6669 6c65 2028  e a wheel file (
-000006b0: 6769 7665 6e20 7a02 292e 7a2c 4c6f 6361  given z.).z,Loca
-000006c0: 6c2d 7061 636b 6167 6520 7061 7468 206d  l-package path m
-000006d0: 7573 7420 6265 2061 6273 6f6c 7574 653a  ust be absolute:
-000006e0: 2028 6769 7665 6e20 2904 da08 656e 6473   (given )...ends
-000006f0: 7769 7468 da0a 5661 6c75 6545 7272 6f72  with..ValueError
-00000700: 7202 0000 00da 0b69 735f 6162 736f 6c75  r......is_absolu
-00000710: 7465 2902 da03 636c 73da 0576 616c 7565  te)...cls..value
-00000720: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
-00000730: 1170 6163 6b61 6765 5f76 616c 6964 6174  .package_validat
-00000740: 6f72 3c00 0000 7318 0000 0008 020a 0102  or<...s.........
-00000750: 0102 0102 0106 ff04 ff0c 0402 010a 0104  ................
-00000760: ff04 037a 2054 6173 6b43 6f6c 6c65 6374  ...z TaskCollect
-00000770: 5069 702e 7061 636b 6167 655f 7661 6c69  Pip.package_vali
-00000780: 6461 746f 7229 1072 0e00 0000 720f 0000  dator).r....r...
-00000790: 0072 1000 0000 da07 5f5f 646f 635f 5fda  .r......__doc__.
-000007a0: 0373 7472 da0f 5f5f 616e 6e6f 7461 7469  .str..__annotati
-000007b0: 6f6e 735f 5f72 1400 0000 7204 0000 0072  ons__r....r....r
-000007c0: 1500 0000 7216 0000 0072 0700 0000 7209  ....r....r....r.
-000007d0: 0000 00da 105f 7061 636b 6167 655f 7665  ....._package_ve
-000007e0: 7273 696f 6eda 0f5f 7061 636b 6167 655f  rsion.._package_
-000007f0: 6578 7472 6173 da0f 5f70 7974 686f 6e5f  extras.._python_
-00000800: 7665 7273 696f 6e72 1e00 0000 7211 0000  versionr....r...
-00000810: 0072 1100 0000 7211 0000 0072 1200 0000  .r....r....r....
-00000820: 720b 0000 0016 0000 0073 2200 0000 0a00  r........s".....
-00000830: 0401 0816 1001 1001 1001 0a02 0601 04ff  ................
-00000840: 0a03 0601 04ff 0a03 0601 04ff 0604 0e01  ................
-00000850: 720b 0000 0063 0000 0000 0000 0000 0000  r....c..........
-00000860: 0000 0000 0000 0300 0000 4000 0000 7368  ..........@...sh
-00000870: 0000 0065 005a 0164 005a 0255 0064 015a  ...e.Z.d.Z.U.d.Z
-00000880: 0365 0464 0219 0065 0564 033c 0065 0665  .e.d...e.d.<.e.e
-00000890: 0564 043c 0065 0765 0564 053c 0065 0867  .d.<.e.e.d.<.e.g
-000008a0: 0064 068d 015a 0965 0a65 0b65 0c19 0019  .d...Z.e.e.e....
-000008b0: 0065 0564 073c 0065 0a65 0619 0065 0564  .e.d.<.e.e...e.d
-000008c0: 083c 0065 0a65 0619 0065 0564 093c 0064  .<.e.e...e.d.<.d
-000008d0: 0a64 0b84 005a 0d64 0c53 0029 0d72 0c00  .d...Z.d.S.).r..
-000008e0: 0000 7aac 0a20 2020 2054 6173 6b43 6f6c  ..z..    TaskCol
-000008f0: 6c65 6374 5374 6174 7573 2063 6c61 7373  lectStatus class
-00000900: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
-00000910: 3a0a 2020 2020 2020 2020 7374 6174 7573  :.        status
-00000920: 3a20 5442 440a 2020 2020 2020 2020 7061  : TBD.        pa
-00000930: 636b 6167 653a 2054 4244 0a20 2020 2020  ckage: TBD.     
-00000940: 2020 2076 656e 765f 7061 7468 3a20 5442     venv_path: TB
-00000950: 440a 2020 2020 2020 2020 7461 736b 5f6c  D.        task_l
-00000960: 6973 743a 2054 4244 0a20 2020 2020 2020  ist: TBD.       
-00000970: 206c 6f67 3a20 5442 440a 2020 2020 2020   log: TBD.      
-00000980: 2020 696e 666f 3a20 5442 440a 2020 2020    info: TBD.    
-00000990: 2905 da07 7065 6e64 696e 67da 0a69 6e73  )...pending..ins
-000009a0: 7461 6c6c 696e 67da 0a63 6f6c 6c65 6374  talling..collect
-000009b0: 696e 67da 0466 6169 6cda 024f 4bda 0673  ing..fail..OK..s
-000009c0: 7461 7475 7372 1300 0000 da09 7665 6e76  tatusr......venv
-000009d0: 5f70 6174 6829 01da 0764 6566 6175 6c74  _path)...default
-000009e0: da09 7461 736b 5f6c 6973 74da 036c 6f67  ..task_list..log
-000009f0: da04 696e 666f 6301 0000 0000 0000 0000  ..infoc.........
-00000a00: 0000 0002 0000 0003 0000 0043 0000 0073  ...........C...s
-00000a10: 1a00 0000 7c00 a000 a100 7d01 7401 7c00  ....|.....}.t.|.
-00000a20: 6a02 8301 7c01 6401 3c00 7c01 5300 2902  j...|.d.<.|.S.).
-00000a30: 7a51 0a20 2020 2020 2020 2052 6574 7572  zQ.        Retur
-00000a40: 6e20 6073 656c 662e 6469 6374 2829 6020  n `self.dict()` 
-00000a50: 6166 7465 7220 6361 7374 696e 6720 6073  after casting `s
-00000a60: 656c 662e 7665 6e76 5f70 6174 6860 2074  elf.venv_path` t
-00000a70: 6f20 6120 7374 7269 6e67 0a20 2020 2020  o a string.     
-00000a80: 2020 2072 2b00 0000 2903 da04 6469 6374     r+...)...dict
-00000a90: 7220 0000 0072 2b00 0000 2902 da04 7365  r ...r+...)...se
-00000aa0: 6c66 da01 6472 1100 0000 7211 0000 0072  lf..dr....r....r
-00000ab0: 1200 0000 da0e 7361 6e69 7469 7365 645f  ......sanitised_
-00000ac0: 6469 6374 5f00 0000 7306 0000 0008 040e  dict_...s.......
-00000ad0: 0104 017a 2054 6173 6b43 6f6c 6c65 6374  ...z TaskCollect
-00000ae0: 5374 6174 7573 2e73 616e 6974 6973 6564  Status.sanitised
-00000af0: 5f64 6963 744e 290e 720e 0000 0072 0f00  _dictN).r....r..
-00000b00: 0000 7210 0000 0072 1f00 0000 7203 0000  ..r....r....r...
-00000b10: 0072 2100 0000 7220 0000 0072 0200 0000  .r!...r ...r....
-00000b20: 7206 0000 0072 2d00 0000 7204 0000 00da  r....r-...r.....
-00000b30: 046c 6973 7472 0a00 0000 7233 0000 0072  .listr....r3...r
-00000b40: 1100 0000 7211 0000 0072 1100 0000 7212  ....r....r....r.
-00000b50: 0000 0072 0c00 0000 4b00 0000 7312 0000  ...r....K...s...
-00000b60: 000a 0004 010c 0c08 0108 011a 010c 010c  ................
-00000b70: 010c 0272 0c00 0000 4e29 11da 0770 6174  ...r....N)...pat
-00000b80: 686c 6962 7202 0000 00da 0674 7970 696e  hlibr......typin
-00000b90: 6772 0300 0000 7204 0000 00da 0870 7964  gr....r......pyd
-00000ba0: 616e 7469 6372 0500 0000 7206 0000 0072  anticr....r....r
-00000bb0: 0700 0000 da0b 5f76 616c 6964 6174 6f72  ......_validator
-00000bc0: 7372 0900 0000 da04 7461 736b 720a 0000  sr......taskr...
-00000bd0: 00da 075f 5f61 6c6c 5f5f 720d 0000 0072  ...__all__r....r
-00000be0: 0b00 0000 720c 0000 0072 1100 0000 7211  ....r....r....r.
-00000bf0: 0000 0072 1100 0000 7212 0000 00da 083c  ...r....r......<
-00000c00: 6d6f 6475 6c65 3e01 0000 0073 1800 0000  module>....s....
-00000c10: 0c00 0c01 0c01 0c02 0c01 0c01 0c02 0c01  ................
-00000c20: 0402 1006 1004 1435                      .......5
+00000290: 3c00 6403 5a0a 6507 650b 6504 6504 6602  <.d.Z.e.e.e.e.f.
+000002a0: 1900 1900 6505 6407 3c00 650c 6404 6408  ....e.d.<.e.d.d.
+000002b0: 6409 8d02 650d 6404 8301 8301 5a0e 650c  d...e.d.....Z.e.
+000002c0: 6405 6408 6409 8d02 650d 6405 8301 8301  d.d.d...e.d.....
+000002d0: 5a0f 650c 6406 6408 6409 8d02 650d 6406  Z.e.d.d.d...e.d.
+000002e0: 8301 8301 5a10 650c 6402 8301 640a 640b  ....Z.e.d...d.d.
+000002f0: 8400 8301 5a11 6403 5300 290c 720b 0000  ....Z.d.S.).r...
+00000300: 0061 6503 0000 0a20 2020 2054 6173 6b43  .ae....    TaskC
+00000310: 6f6c 6c65 6374 5069 7020 636c 6173 730a  ollectPip class.
+00000320: 0a20 2020 2054 6869 7320 636c 6173 7320  .    This class 
+00000330: 6f6e 6c79 2065 6e63 6f64 6573 2074 6865  only encodes the
+00000340: 2061 7474 7269 6275 7465 7320 7265 7175   attributes requ
+00000350: 6972 6564 2074 6f20 7472 6967 6765 7220  ired to trigger 
+00000360: 610a 2020 2020 7461 736b 2d63 6f6c 6c65  a.    task-colle
+00000370: 6374 696f 6e20 6f70 6572 6174 696f 6e2e  ction operation.
+00000380: 204f 7468 6572 2061 7474 7269 6275 7465   Other attribute
+00000390: 7320 2874 6861 7420 6172 6520 6173 7369  s (that are assi
+000003a0: 676e 6564 202a 6475 7269 6e67 2a0a 2020  gned *during*.  
+000003b0: 2020 7461 736b 2063 6f6c 6c65 6374 696f    task collectio
+000003c0: 6e29 2061 7265 2064 6566 696e 6564 2061  n) are defined a
+000003d0: 7320 7061 7274 206f 6620 6672 6163 7461  s part of fracta
+000003e0: 6c2d 7365 7276 6572 2e0a 0a20 2020 2054  l-server...    T
+000003f0: 776f 2063 6173 6573 2061 7265 2073 7570  wo cases are sup
+00000400: 706f 7274 6564 3a0a 0a20 2020 2020 2020  ported:..       
+00000410: 2031 2e20 6070 6163 6b61 6765 6020 6973   1. `package` is
+00000420: 2074 6865 2070 6174 6820 6f66 2061 206c   the path of a l
+00000430: 6f63 616c 2077 6865 656c 2066 696c 653b  ocal wheel file;
+00000440: 0a20 2020 2020 2020 2032 2e20 6070 6163  .        2. `pac
+00000450: 6b61 6765 6020 6973 2074 6865 206e 616d  kage` is the nam
+00000460: 6520 6f66 2061 2070 6163 6b61 6765 2074  e of a package t
+00000470: 6861 7420 6361 6e20 6265 2069 6e73 7461  hat can be insta
+00000480: 6c6c 6564 2076 6961 2060 7069 7060 2e0a  lled via `pip`..
+00000490: 0a0a 2020 2020 4174 7472 6962 7574 6573  ..    Attributes
+000004a0: 3a0a 2020 2020 2020 2020 7061 636b 6167  :.        packag
+000004b0: 653a 0a20 2020 2020 2020 2020 2020 2054  e:.            T
+000004c0: 6865 206e 616d 6520 6f66 2061 2060 7069  he name of a `pi
+000004d0: 7060 2d69 6e73 7461 6c6c 6162 6c65 2070  p`-installable p
+000004e0: 6163 6b61 6765 2c20 6f72 2074 6865 2070  ackage, or the p
+000004f0: 6174 6820 746f 2061 206c 6f63 616c 0a20  ath to a local. 
+00000500: 2020 2020 2020 2020 2020 2077 6865 656c             wheel
+00000510: 2066 696c 652e 0a20 2020 2020 2020 2070   file..        p
+00000520: 6163 6b61 6765 5f76 6572 7369 6f6e 3a20  ackage_version: 
+00000530: 5665 7273 696f 6e20 6f66 2074 6865 2070  Version of the p
+00000540: 6163 6b61 6765 0a20 2020 2020 2020 2070  ackage.        p
+00000550: 6163 6b61 6765 5f65 7874 7261 733a 2050  ackage_extras: P
+00000560: 6163 6b61 6765 2065 7874 7261 7320 746f  ackage extras to
+00000570: 2069 6e63 6c75 6465 2069 6e20 7468 6520   include in the 
+00000580: 6070 6970 2069 6e73 7461 6c6c 6020 636f  `pip install` co
+00000590: 6d6d 616e 640a 2020 2020 2020 2020 7079  mmand.        py
+000005a0: 7468 6f6e 5f76 6572 7369 6f6e 3a20 5079  thon_version: Py
+000005b0: 7468 6f6e 2076 6572 7369 6f6e 2074 6f20  thon version to 
+000005c0: 696e 7374 616c 6c20 616e 6420 7275 6e20  install and run 
+000005d0: 7468 6520 7061 636b 6167 6520 7461 736b  the package task
+000005e0: 730a 2020 2020 2020 2020 7069 6e6e 6564  s.        pinned
+000005f0: 5f70 6163 6b61 6765 5f76 6572 7369 6f6e  _package_version
+00000600: 733a 0a20 2020 2020 2020 2020 2020 2064  s:.            d
+00000610: 6963 7469 6f6e 6172 7920 2770 6163 6b61  ictionary 'packa
+00000620: 6765 273a 2776 6572 7369 6f6e 2720 7573  ge':'version' us
+00000630: 6564 2074 6f20 7069 6e20 7665 7273 696f  ed to pin versio
+00000640: 6e73 2066 6f72 2073 7065 6369 6669 630a  ns for specific.
+00000650: 2020 2020 2020 2020 2020 2020 7061 636b              pack
+00000660: 6167 6573 2e0a 0a20 2020 20da 0770 6163  ages...    ..pac
+00000670: 6b61 6765 4eda 0f70 6163 6b61 6765 5f76  kageN..package_v
+00000680: 6572 7369 6f6e da0e 7061 636b 6167 655f  ersion..package_
+00000690: 6578 7472 6173 da0e 7079 7468 6f6e 5f76  extras..python_v
+000006a0: 6572 7369 6f6e da17 7069 6e6e 6564 5f70  ersion..pinned_p
+000006b0: 6163 6b61 6765 5f76 6572 7369 6f6e 7354  ackage_versionsT
+000006c0: 2901 da0b 616c 6c6f 775f 7265 7573 6563  )...allow_reusec
+000006d0: 0200 0000 0000 0000 0000 0000 0200 0000  ................
+000006e0: 0400 0000 4300 0000 7342 0000 0064 017c  ....C...sB...d.|
+000006f0: 0176 0072 1f7c 01a0 0064 02a1 0173 1174  .v.r.|...d...s.t
+00000700: 0164 037c 019b 0064 049d 0383 0182 0174  .d.|...d.......t
+00000710: 027c 0183 01a0 03a1 0073 1f74 0164 057c  .|.......s.t.d.|
+00000720: 019b 0064 049d 0383 0182 017c 0153 0029  ...d.......|.S.)
+00000730: 064e fa01 2f7a 042e 7768 6c7a 2f4c 6f63  .N../z..whlz/Loc
+00000740: 616c 2d70 6163 6b61 6765 2070 6174 6820  al-package path 
+00000750: 6d75 7374 2062 6520 6120 7768 6565 6c20  must be a wheel 
+00000760: 6669 6c65 2028 6769 7665 6e20 7a02 292e  file (given z.).
+00000770: 7a2c 4c6f 6361 6c2d 7061 636b 6167 6520  z,Local-package 
+00000780: 7061 7468 206d 7573 7420 6265 2061 6273  path must be abs
+00000790: 6f6c 7574 653a 2028 6769 7665 6e20 2904  olute: (given ).
+000007a0: da08 656e 6473 7769 7468 da0a 5661 6c75  ..endswith..Valu
+000007b0: 6545 7272 6f72 7202 0000 00da 0b69 735f  eErrorr......is_
+000007c0: 6162 736f 6c75 7465 2902 da03 636c 73da  absolute)...cls.
+000007d0: 0576 616c 7565 7211 0000 0072 1100 0000  .valuer....r....
+000007e0: 7212 0000 00da 1170 6163 6b61 6765 5f76  r......package_v
+000007f0: 616c 6964 6174 6f72 4100 0000 7318 0000  alidatorA...s...
+00000800: 0008 020a 0102 0102 0102 0106 ff04 ff0c  ................
+00000810: 0402 010a 0104 ff04 037a 2054 6173 6b43  .........z TaskC
+00000820: 6f6c 6c65 6374 5069 702e 7061 636b 6167  ollectPip.packag
+00000830: 655f 7661 6c69 6461 746f 7229 1272 0e00  e_validator).r..
+00000840: 0000 720f 0000 0072 1000 0000 da07 5f5f  ..r....r......__
+00000850: 646f 635f 5fda 0373 7472 da0f 5f5f 616e  doc__..str..__an
+00000860: 6e6f 7461 7469 6f6e 735f 5f72 1400 0000  notations__r....
+00000870: 7204 0000 0072 1500 0000 7216 0000 0072  r....r....r....r
+00000880: 1700 0000 da04 6469 6374 7207 0000 0072  ......dictr....r
+00000890: 0900 0000 da10 5f70 6163 6b61 6765 5f76  ......_package_v
+000008a0: 6572 7369 6f6e da0f 5f70 6163 6b61 6765  ersion.._package
+000008b0: 5f65 7874 7261 73da 0f5f 7079 7468 6f6e  _extras.._python
+000008c0: 5f76 6572 7369 6f6e 721f 0000 0072 1100  _versionr....r..
+000008d0: 0000 7211 0000 0072 1100 0000 7212 0000  ..r....r....r...
+000008e0: 0072 0b00 0000 1600 0000 7324 0000 000a  .r........s$....
+000008f0: 0004 0108 1a10 0110 0110 0118 010a 0206  ................
+00000900: 0104 ff0a 0306 0104 ff0a 0306 0104 ff06  ................
+00000910: 040e 0172 0b00 0000 6300 0000 0000 0000  ...r....c.......
+00000920: 0000 0000 0000 0000 0003 0000 0040 0000  .............@..
+00000930: 0073 6800 0000 6500 5a01 6400 5a02 5500  .sh...e.Z.d.Z.U.
+00000940: 6401 5a03 6504 6402 1900 6505 6403 3c00  d.Z.e.d...e.d.<.
+00000950: 6506 6505 6404 3c00 6507 6505 6405 3c00  e.e.d.<.e.e.d.<.
+00000960: 6508 6700 6406 8d01 5a09 650a 650b 650c  e.g.d...Z.e.e.e.
+00000970: 1900 1900 6505 6407 3c00 650a 6506 1900  ....e.d.<.e.e...
+00000980: 6505 6408 3c00 650a 6506 1900 6505 6409  e.d.<.e.e...e.d.
+00000990: 3c00 640a 640b 8400 5a0d 640c 5300 290d  <.d.d...Z.d.S.).
+000009a0: 720c 0000 007a ac0a 2020 2020 5461 736b  r....z..    Task
+000009b0: 436f 6c6c 6563 7453 7461 7475 7320 636c  CollectStatus cl
+000009c0: 6173 730a 0a20 2020 2041 7474 7269 6275  ass..    Attribu
+000009d0: 7465 733a 0a20 2020 2020 2020 2073 7461  tes:.        sta
+000009e0: 7475 733a 2054 4244 0a20 2020 2020 2020  tus: TBD.       
+000009f0: 2070 6163 6b61 6765 3a20 5442 440a 2020   package: TBD.  
+00000a00: 2020 2020 2020 7665 6e76 5f70 6174 683a        venv_path:
+00000a10: 2054 4244 0a20 2020 2020 2020 2074 6173   TBD.        tas
+00000a20: 6b5f 6c69 7374 3a20 5442 440a 2020 2020  k_list: TBD.    
+00000a30: 2020 2020 6c6f 673a 2054 4244 0a20 2020      log: TBD.   
+00000a40: 2020 2020 2069 6e66 6f3a 2054 4244 0a20       info: TBD. 
+00000a50: 2020 2029 05da 0770 656e 6469 6e67 da0a     )...pending..
+00000a60: 696e 7374 616c 6c69 6e67 da0a 636f 6c6c  installing..coll
+00000a70: 6563 7469 6e67 da04 6661 696c da02 4f4b  ecting..fail..OK
+00000a80: da06 7374 6174 7573 7213 0000 00da 0976  ..statusr......v
+00000a90: 656e 765f 7061 7468 2901 da07 6465 6661  env_path)...defa
+00000aa0: 756c 74da 0974 6173 6b5f 6c69 7374 da03  ult..task_list..
+00000ab0: 6c6f 67da 0469 6e66 6f63 0100 0000 0000  log..infoc......
+00000ac0: 0000 0000 0000 0200 0000 0300 0000 4300  ..............C.
+00000ad0: 0000 731a 0000 007c 00a0 00a1 007d 0174  ..s....|.....}.t
+00000ae0: 017c 006a 0283 017c 0164 013c 007c 0153  .|.j...|.d.<.|.S
+00000af0: 0029 027a 510a 2020 2020 2020 2020 5265  .).zQ.        Re
+00000b00: 7475 726e 2060 7365 6c66 2e64 6963 7428  turn `self.dict(
+00000b10: 2960 2061 6674 6572 2063 6173 7469 6e67  )` after casting
+00000b20: 2060 7365 6c66 2e76 656e 765f 7061 7468   `self.venv_path
+00000b30: 6020 746f 2061 2073 7472 696e 670a 2020  ` to a string.  
+00000b40: 2020 2020 2020 722d 0000 0029 0372 2300        r-...).r#.
+00000b50: 0000 7221 0000 0072 2d00 0000 2902 da04  ..r!...r-...)...
+00000b60: 7365 6c66 da01 6472 1100 0000 7211 0000  self..dr....r...
+00000b70: 0072 1200 0000 da0e 7361 6e69 7469 7365  .r......sanitise
+00000b80: 645f 6469 6374 6400 0000 7306 0000 0008  d_dictd...s.....
+00000b90: 040e 0104 017a 2054 6173 6b43 6f6c 6c65  .....z TaskColle
+00000ba0: 6374 5374 6174 7573 2e73 616e 6974 6973  ctStatus.sanitis
+00000bb0: 6564 5f64 6963 744e 290e 720e 0000 0072  ed_dictN).r....r
+00000bc0: 0f00 0000 7210 0000 0072 2000 0000 7203  ....r....r ...r.
+00000bd0: 0000 0072 2200 0000 7221 0000 0072 0200  ...r"...r!...r..
+00000be0: 0000 7206 0000 0072 2f00 0000 7204 0000  ..r....r/...r...
+00000bf0: 00da 046c 6973 7472 0a00 0000 7234 0000  ...listr....r4..
+00000c00: 0072 1100 0000 7211 0000 0072 1100 0000  .r....r....r....
+00000c10: 7212 0000 0072 0c00 0000 5000 0000 7312  r....r....P...s.
+00000c20: 0000 000a 0004 010c 0c08 0108 011a 010c  ................
+00000c30: 010c 010c 0272 0c00 0000 4e29 11da 0770  .....r....N)...p
+00000c40: 6174 686c 6962 7202 0000 00da 0674 7970  athlibr......typ
+00000c50: 696e 6772 0300 0000 7204 0000 00da 0870  ingr....r......p
+00000c60: 7964 616e 7469 6372 0500 0000 7206 0000  ydanticr....r...
+00000c70: 0072 0700 0000 da0b 5f76 616c 6964 6174  .r......_validat
+00000c80: 6f72 7372 0900 0000 da04 7461 736b 720a  orsr......taskr.
+00000c90: 0000 00da 075f 5f61 6c6c 5f5f 720d 0000  .....__all__r...
+00000ca0: 0072 0b00 0000 720c 0000 0072 1100 0000  .r....r....r....
+00000cb0: 7211 0000 0072 1100 0000 7212 0000 00da  r....r....r.....
+00000cc0: 083c 6d6f 6475 6c65 3e01 0000 0073 1800  .<module>....s..
+00000cd0: 0000 0c00 0c01 0c01 0c02 0c01 0c01 0c02  ................
+00000ce0: 0c01 0402 1006 1004 143a                 .........:
```

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/user.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/user.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/workflow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc` & `fractal_server-1.3.0a4/fractal_server/common/schemas/__pycache__/workflow.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/_validators.py` & `fractal_server-1.3.0a4/fractal_server/common/schemas/_validators.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/applyworkflow.py` & `fractal_server-1.3.0a4/fractal_server/common/schemas/applyworkflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/manifest.py` & `fractal_server-1.3.0a4/fractal_server/common/schemas/manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/project.py` & `fractal_server-1.3.0a4/fractal_server/common/schemas/project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/state.py` & `fractal_server-1.3.0a4/fractal_server/common/schemas/state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/task.py` & `fractal_server-1.3.0a4/fractal_server/common/schemas/task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/task_collection.py` & `fractal_server-1.3.0a4/fractal_server/common/schemas/task_collection.py`

 * *Files 17% similar despite different names*

```diff
@@ -36,20 +36,25 @@
     Attributes:
         package:
             The name of a `pip`-installable package, or the path to a local
             wheel file.
         package_version: Version of the package
         package_extras: Package extras to include in the `pip install` command
         python_version: Python version to install and run the package tasks
+        pinned_package_versions:
+            dictionary 'package':'version' used to pin versions for specific
+            packages.
+
     """
 
     package: str
     package_version: Optional[str] = None
     package_extras: Optional[str] = None
     python_version: Optional[str] = None
+    pinned_package_versions: Optional[dict[str, str]] = None
 
     _package_version = validator("package_version", allow_reuse=True)(
         valstr("package_version")
     )
     _package_extras = validator("package_extras", allow_reuse=True)(
         valstr("package_extras")
     )
```

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/user.py` & `fractal_server-1.3.0a4/fractal_server/common/schemas/user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/schemas/workflow.py` & `fractal_server-1.3.0a4/fractal_server/common/schemas/workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_applyworkflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_dataset.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_manifest.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_project.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_state.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_task.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_task_collection.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_user.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.2.2.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc` & `fractal_server-1.3.0a4/fractal_server/common/tests/__pycache__/test_workflow.cpython-310-pytest-7.3.1.pyc`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/test_dataset.py` & `fractal_server-1.3.0a4/fractal_server/common/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/test_manifest.py` & `fractal_server-1.3.0a4/fractal_server/common/tests/test_manifest.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/test_project.py` & `fractal_server-1.3.0a4/fractal_server/common/tests/test_project.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/test_state.py` & `fractal_server-1.3.0a4/fractal_server/common/tests/test_state.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/test_task.py` & `fractal_server-1.3.0a4/fractal_server/common/tests/test_task.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/test_task_collection.py` & `fractal_server-1.3.0a4/fractal_server/common/tests/test_task_collection.py`

 * *Files 24% similar despite different names*

```diff
@@ -18,7 +18,11 @@
         c = TaskCollectPip(package="some/package")
     with pytest.raises(ValidationError):
         c = TaskCollectPip(package="/some/package.tar.gz")
     with pytest.raises(ValidationError):
         c = TaskCollectPip(package="some-package", package_extras="")
     with pytest.raises(ValidationError):
         c = TaskCollectPip(package="some-package", package_extras=None)
+
+    c = TaskCollectPip(package="some-package", pinned_package_versions={})
+    with pytest.raises(ValidationError):
+        c = TaskCollectPip(package="some-package", pinned_package_versions=1)
```

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/test_user.py` & `fractal_server-1.3.0a4/fractal_server/common/tests/test_user.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/common/tests/test_workflow.py` & `fractal_server-1.3.0a4/fractal_server/common/tests/test_workflow.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/config.py` & `fractal_server-1.3.0a4/fractal_server/config.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/logger.py` & `fractal_server-1.3.0a4/fractal_server/logger.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/main.py` & `fractal_server-1.3.0a4/fractal_server/main.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/migrations/env.py` & `fractal_server-1.3.0a4/fractal_server/migrations/env.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/migrations/script.py.mako` & `fractal_server-1.3.0a4/fractal_server/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py` & `fractal_server-1.3.0a4/fractal_server/migrations/versions/4c308bcaea2b_add_task_args_schema_and_task_args_.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py` & `fractal_server-1.3.0a4/fractal_server/migrations/versions/50a13d6138fd_initial_schema.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py` & `fractal_server-1.3.0a4/fractal_server/migrations/versions/f384e1c0cf5d_drop_task_default_args_columns.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/syringe.py` & `fractal_server-1.3.0a4/fractal_server/syringe.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/fractal_server/tasks/collection.py` & `fractal_server-1.3.0a4/fractal_server/tasks/collection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Copyright 2022 (C) Friedrich Miescher Institute for Biomedical Research and
 # University of Zurich
 #
 # Original authors:
 # Jacopo Nespolo <jacopo.nespolo@exact-lab.it>
+# Tommaso Comparin <tommaso.comparin@exact-lab.it>
+# Yuri Chiucconi <yuri.chiucconi@exact-lab.it>
 #
 # This file is part of Fractal and was originally developed by eXact lab S.r.l.
 # <exact-lab.it> under contract with Liberali Lab from the Friedrich Miescher
 # Institute for Biomedical Research and Pelkmans Lab from the University of
 # Zurich.
 """
 This module takes care of installing tasks so that fractal can execute them
@@ -455,14 +457,17 @@
     """
     Install package in venv
 
     Returns:
         package_root : Path
             the location of the package manifest
     """
+
+    logger = get_logger(logger_name)
+
     pip = venv_path / "venv/bin/pip"
 
     extras = f"[{task_pkg.package_extras}]" if task_pkg.package_extras else ""
 
     if task_pkg.is_local_package:
         pip_install_str = f"{task_pkg.package_path.as_posix()}{extras}"
     else:
@@ -478,14 +483,58 @@
         cwd=venv_path,
         command=f"{pip} install --upgrade pip",
         logger_name=logger_name,
     )
     await execute_command(
         cwd=venv_path, command=cmd_install, logger_name=logger_name
     )
+    if task_pkg.pinned_package_versions:
+        for (
+            pinned_pkg_name,
+            pinned_pkg_version,
+        ) in task_pkg.pinned_package_versions.items():
+
+            logger.debug(
+                "Specific version required: "
+                f"{pinned_pkg_name}=={pinned_pkg_version}"
+            )
+            logger.debug(
+                "Preliminary check: verify that "
+                f"{pinned_pkg_version} is already installed"
+            )
+            stdout_inspect = await execute_command(
+                cwd=venv_path,
+                command=f"{pip} show {pinned_pkg_name}",
+                logger_name=logger_name,
+            )
+            current_version = next(
+                line.split()[-1]
+                for line in stdout_inspect.split("\n")
+                if line.startswith("Version:")
+            )
+            if current_version != pinned_pkg_version:
+                logger.debug(
+                    f"Currently installed version of {pinned_pkg_name}"
+                    f"({current_version}) differs from pinned version "
+                    f"({pinned_pkg_version}); "
+                    f"install version {pinned_pkg_version}."
+                )
+                await execute_command(
+                    cwd=venv_path,
+                    command=(
+                        f"{pip} install "
+                        f"{pinned_pkg_name}=={pinned_pkg_version}"
+                    ),
+                    logger_name=logger_name,
+                )
+            else:
+                logger.debug(
+                    f"Currently installed version of {pinned_pkg_name}"
+                    f"({current_version}) already matches the pinned version."
+                )
 
     # Extract package installation path from `pip show`
     stdout_inspect = await execute_command(
         cwd=venv_path, command=cmd_inspect, logger_name=logger_name
     )
 
     location = Path(
```

### Comparing `fractal_server-1.3.0a3/fractal_server/utils.py` & `fractal_server-1.3.0a4/fractal_server/utils.py`

 * *Files identical despite different names*

### Comparing `fractal_server-1.3.0a3/pyproject.toml` & `fractal_server-1.3.0a4/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fractal-server"
-version = "1.3.0a3"
+version = "1.3.0a4"
 description = "Server component of the Fractal analytics platform"
 authors = [
     "Jacopo Nespolo <jacopo.nespolo@exact-lab.it>",
     "Marco Franzon <marco.franzon@exact-lab.it>",
     "Tommaso Comparin <tommaso.comparin@exact-lab.it>",
 ]
 readme = "README.md"
@@ -72,15 +72,15 @@
 asyncio_mode = "auto"
 filterwarnings = [
     "error::RuntimeWarning",
     "error::pytest.PytestUnraisableExceptionWarning",
 ]
 
 [tool.bumpver]
-current_version = "1.3.0a3"
+current_version = "1.3.0a4"
 version_pattern = "MAJOR.MINOR.PATCH[PYTAGNUM]"
 commit_message = "bump version {old_version} -> {new_version}"
 commit = true
 tag = true
 push = true
 
 [tool.bumpver.file_patterns]
```

### Comparing `fractal_server-1.3.0a3/PKG-INFO` & `fractal_server-1.3.0a4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fractal-server
-Version: 1.3.0a3
+Version: 1.3.0a4
 Summary: Server component of the Fractal analytics platform
 Home-page: https://github.com/fractal-analytics-platform/fractal-server
 License: BSD-3-Clause
 Author: Jacopo Nespolo
 Author-email: jacopo.nespolo@exact-lab.it
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: BSD License
@@ -64,11 +64,9 @@
 [@sampsyo](https://github.com/sampsyo) and collaborators, and it is released
 under the terms of the MIT license.
 
 Fractal was conceived in the Liberali Lab at the Friedrich Miescher Institute
 for Biomedical Research and in the Pelkmans Lab at the University of Zurich
 (both in Switzerland). The project lead is with
 [@gusqgm](https://github.com/gusqgm) & [@jluethi](https://github.com/jluethi).
-The core development is done under contract by
-[@mfranzon](https://github.com/mfranzon), [@tcompa](https://github.com/tcompa)
-& [@japs](https://github.com/japs) of [eXact lab S.r.l.](exact-lab.it).
+The core development is done under contract by [eXact lab S.r.l.](exact-lab.it).
```

