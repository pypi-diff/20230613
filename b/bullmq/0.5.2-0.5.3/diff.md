# Comparing `tmp/bullmq-0.5.2.tar.gz` & `tmp/bullmq-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bullmq-0.5.2.tar", last modified: Sun Jun 11 15:42:31 2023, max compression
+gzip compressed data, was "bullmq-0.5.3.tar", last modified: Tue Jun 13 16:46:50 2023, max compression
```

## Comparing `bullmq-0.5.2.tar` & `bullmq-0.5.3.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:42:31.614063 bullmq-0.5.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-11 15:42:31.614063 bullmq-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-11 15:40:53.000000 bullmq-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:42:31.610063 bullmq-0.5.2/bullmq/
--rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-11 15:42:29.000000 bullmq-0.5.2/bullmq/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/backoffs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:42:31.614063 bullmq-0.5.2/bullmq/commands/
--rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/addJob-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/changeDelay-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/changePriority-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/cleanJobsInSet-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/drain-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/extendLock-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/getCounts-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/getRanges-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/getState-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/getStateV2-7.lua
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/isFinished-3.lua
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/isJobInList-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/moveJobFromActiveToWait-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/moveStalledJobsToWait-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/moveToActive-9.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/moveToDelayed-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/moveToFinished-12.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/moveToWaitingChildren-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/obliterate-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/pause-4.lua
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/promote-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/releaseLock-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/removeJob-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/removeRepeatable-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/reprocessJob-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/retryJob-8.lua
--rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/retryJobs-6.lua
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/saveStacktrace-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/updateData-1.lua
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-11 15:42:04.000000 bullmq-0.5.2/bullmq/commands/updateProgress-2.lua
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/error_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/event_emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/job.py
--rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/queue.py
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/redis_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/timer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:42:31.614063 bullmq-0.5.2/bullmq/types/
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/types/backoff_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/types/job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/types/keep_jobs.py
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/types/queue_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/types/retry_job_options.py
--rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/types/worker_options.py
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7490 2023-06-11 15:40:53.000000 bullmq-0.5.2/bullmq/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-11 15:42:31.610063 bullmq-0.5.2/bullmq.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-11 15:42:31.000000 bullmq-0.5.2/bullmq.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-11 15:42:31.000000 bullmq-0.5.2/bullmq.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-11 15:42:31.000000 bullmq-0.5.2/bullmq.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-11 15:42:31.000000 bullmq-0.5.2/bullmq.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-11 15:42:31.000000 bullmq-0.5.2/bullmq.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-11 15:42:31.614063 bullmq-0.5.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-11 15:40:53.000000 bullmq-0.5.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:46:50.098966 bullmq-0.5.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-13 16:46:50.098966 bullmq-0.5.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-06-13 16:44:57.000000 bullmq-0.5.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:46:50.094966 bullmq-0.5.3/bullmq/
+-rw-r--r--   0 runner    (1001) docker     (123)      269 2023-06-13 16:46:47.000000 bullmq-0.5.3/bullmq/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/backoffs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:46:50.098966 bullmq-0.5.3/bullmq/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)     8265 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/addJob-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/changeDelay-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1751 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/changePriority-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     9172 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/cleanJobsInSet-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/drain-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/extendLock-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/getCounts-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/getRanges-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1313 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/getState-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/getStateV2-7.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/isFinished-3.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/isJobInList-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1875 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/moveJobFromActiveToWait-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    11660 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/moveStalledJobsToWait-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     6914 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/moveToActive-9.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/moveToDelayed-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)    21068 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/moveToFinished-12.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/moveToWaitingChildren-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/obliterate-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/pause-4.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/promote-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      292 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/releaseLock-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     7777 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/removeJob-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/removeRepeatable-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/reprocessJob-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/retryJob-8.lua
+-rw-r--r--   0 runner    (1001) docker     (123)     1843 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/retryJobs-6.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/saveStacktrace-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/updateData-1.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-06-13 16:46:16.000000 bullmq-0.5.3/bullmq/commands/updateProgress-2.lua
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/error_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/event_emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7666 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/job.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4847 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/redis_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16635 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/timer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:46:50.098966 bullmq-0.5.3/bullmq/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/types/backoff_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/types/job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/types/keep_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/types/queue_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/types/retry_job_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1190 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/types/worker_options.py
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7829 2023-06-13 16:44:57.000000 bullmq-0.5.3/bullmq/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:46:50.094966 bullmq-0.5.3/bullmq.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1671 2023-06-13 16:46:50.000000 bullmq-0.5.3/bullmq.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1627 2023-06-13 16:46:50.000000 bullmq-0.5.3/bullmq.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:46:50.000000 bullmq-0.5.3/bullmq.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-13 16:46:50.000000 bullmq-0.5.3/bullmq.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 16:46:50.000000 bullmq-0.5.3/bullmq.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-13 16:46:50.098966 bullmq-0.5.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-06-13 16:44:57.000000 bullmq-0.5.3/setup.py
```

### Comparing `bullmq-0.5.2/PKG-INFO` & `bullmq-0.5.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.5.2
+Version: 0.5.3
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.5.2/README.md` & `bullmq-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/backoffs.py` & `bullmq-0.5.3/bullmq/backoffs.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/addJob-8.lua` & `bullmq-0.5.3/bullmq/commands/addJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/changeDelay-3.lua` & `bullmq-0.5.3/bullmq/commands/changeDelay-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/changePriority-4.lua` & `bullmq-0.5.3/bullmq/commands/changePriority-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/cleanJobsInSet-2.lua` & `bullmq-0.5.3/bullmq/commands/cleanJobsInSet-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/drain-4.lua` & `bullmq-0.5.3/bullmq/commands/drain-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/getCounts-1.lua` & `bullmq-0.5.3/bullmq/commands/getCounts-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/getRanges-1.lua` & `bullmq-0.5.3/bullmq/commands/getRanges-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/getState-7.lua` & `bullmq-0.5.3/bullmq/commands/getState-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/getStateV2-7.lua` & `bullmq-0.5.3/bullmq/commands/getStateV2-7.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/isFinished-3.lua` & `bullmq-0.5.3/bullmq/commands/isFinished-3.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/moveJobFromActiveToWait-9.lua` & `bullmq-0.5.3/bullmq/commands/moveJobFromActiveToWait-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/moveStalledJobsToWait-8.lua` & `bullmq-0.5.3/bullmq/commands/moveStalledJobsToWait-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/moveToActive-9.lua` & `bullmq-0.5.3/bullmq/commands/moveToActive-9.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/moveToDelayed-8.lua` & `bullmq-0.5.3/bullmq/commands/moveToDelayed-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/moveToFinished-12.lua` & `bullmq-0.5.3/bullmq/commands/moveToFinished-12.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/moveToWaitingChildren-4.lua` & `bullmq-0.5.3/bullmq/commands/moveToWaitingChildren-4.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/obliterate-2.lua` & `bullmq-0.5.3/bullmq/commands/obliterate-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/promote-6.lua` & `bullmq-0.5.3/bullmq/commands/promote-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/removeJob-1.lua` & `bullmq-0.5.3/bullmq/commands/removeJob-1.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/removeRepeatable-2.lua` & `bullmq-0.5.3/bullmq/commands/removeRepeatable-2.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/reprocessJob-6.lua` & `bullmq-0.5.3/bullmq/commands/reprocessJob-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/retryJob-8.lua` & `bullmq-0.5.3/bullmq/commands/retryJob-8.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/commands/retryJobs-6.lua` & `bullmq-0.5.3/bullmq/commands/retryJobs-6.lua`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/event_emitter.py` & `bullmq-0.5.3/bullmq/event_emitter.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/job.py` & `bullmq-0.5.3/bullmq/job.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/queue.py` & `bullmq-0.5.3/bullmq/queue.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/redis_connection.py` & `bullmq-0.5.3/bullmq/redis_connection.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/scripts.py` & `bullmq-0.5.3/bullmq/scripts.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/timer.py` & `bullmq-0.5.3/bullmq/timer.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/types/job_options.py` & `bullmq-0.5.3/bullmq/types/job_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/types/worker_options.py` & `bullmq-0.5.3/bullmq/types/worker_options.py`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/bullmq/worker.py` & `bullmq-0.5.3/bullmq/worker.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 from uuid import uuid4
 from bullmq.scripts import Scripts
 from bullmq.redis_connection import RedisConnection
 from bullmq.event_emitter import EventEmitter
 from bullmq.job import Job
 from bullmq.timer import Timer
 from bullmq.types import WorkerOptions
+from bullmq.utils import isRedisVersionLowerThan
 
 import asyncio
 import traceback
 import time
+import math
 
 class Worker(EventEmitter):
     def __init__(self, name: str, processor: Callable[[Job, str], asyncio.Future], opts: WorkerOptions = {}):
         super().__init__()
         self.name = name
         self.processor = processor
         final_opts = {
@@ -100,14 +102,19 @@
         if result:
             job, job_id, limit_until, delay_until = result
 
         # If there are no jobs in the waiting list we keep waiting with BRPOPLPUSH
         if job is None:
             timeout = min(delay_until - int(time.time() * 1000)
                           if delay_until else 5000, 5000) / 1000
+            
+            redis_version = await self.blockingRedisConnection.getRedisVersion()
+            # Only Redis v6.0.0 and above supports doubles as block time
+            timeout = int(math.ceil(timeout)) if isRedisVersionLowerThan(redis_version, '6.0.0') else timeout
+
             job_id = await self.bclient.brpoplpush(self.scripts.keys["wait"], self.scripts.keys["active"], timeout)
             if job_id:
                 job, job_id, limit_until, delay_until = await self.scripts.moveToActive(token, self.opts, job_id)
 
         if job and job_id:
             return Job.fromJSON(self, job, job_id)
```

### Comparing `bullmq-0.5.2/bullmq.egg-info/PKG-INFO` & `bullmq-0.5.3/bullmq.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bullmq
-Version: 0.5.2
+Version: 0.5.3
 Summary: BullMQ for Python
 Home-page: https://bullmq.io
 Author: Taskforce.sh Inc.
 Author-email: manast@taskforce.sh
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `bullmq-0.5.2/bullmq.egg-info/SOURCES.txt` & `bullmq-0.5.3/bullmq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bullmq-0.5.2/setup.py` & `bullmq-0.5.3/setup.py`

 * *Files identical despite different names*

