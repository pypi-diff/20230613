# Comparing `tmp/google-cloud-gke-backup-0.4.3.tar.gz` & `tmp/google-cloud-gke-backup-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-gke-backup-0.4.3.tar", last modified: Mon Mar 27 14:58:14 2023, max compression
+gzip compressed data, was "google-cloud-gke-backup-0.4.4.tar", last modified: Tue Jun 13 15:00:12 2023, max compression
```

## Comparing `google-cloud-gke-backup-0.4.3.tar` & `google-cloud-gke-backup-0.4.4.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:14.738238 google-cloud-gke-backup-0.4.3/
--rw-rw-r--   0 root         (0)     1003    11358 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     4778 2023-03-27 14:58:14.738238 google-cloud-gke-backup-0.4.3/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3866 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:14.726241 google-cloud-gke-backup-0.4.3/google/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:14.726241 google-cloud-gke-backup-0.4.3/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:14.730240 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup/
--rw-rw-r--   0 root         (0)     1003     3498 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:14.730240 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/
--rw-rw-r--   0 root         (0)     1003     3181 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     9647 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       84 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:14.730240 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:14.730240 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/
--rw-rw-r--   0 root         (0)     1003      761 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py
--rw-rw-r--   0 root         (0)     1003   134960 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py
--rw-rw-r--   0 root         (0)     1003   148486 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/client.py
--rw-rw-r--   0 root         (0)     1003    31038 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:14.734239 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/transports/
--rw-rw-r--   0 root         (0)     1003     1372 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    20623 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py
--rw-rw-r--   0 root         (0)     1003    38111 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    39090 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   132052 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:14.734239 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/
--rw-rw-r--   0 root         (0)     1003     2884 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    14189 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/backup.py
--rw-rw-r--   0 root         (0)     1003    11568 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/backup_plan.py
--rw-rw-r--   0 root         (0)     1003     2520 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/common.py
--rw-rw-r--   0 root         (0)     1003    36417 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/gkebackup.py
--rw-rw-r--   0 root         (0)     1003    22049 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/restore.py
--rw-rw-r--   0 root         (0)     1003     4643 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/restore_plan.py
--rw-rw-r--   0 root         (0)     1003    12237 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/volume.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:14.734239 google-cloud-gke-backup-0.4.3/google_cloud_gke_backup.egg-info/
--rw-r--r--   0 root         (0)     1003     4778 2023-03-27 14:58:14.000000 google-cloud-gke-backup-0.4.3/google_cloud_gke_backup.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1851 2023-03-27 14:58:14.000000 google-cloud-gke-backup-0.4.3/google_cloud_gke_backup.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:14.000000 google-cloud-gke-backup-0.4.3/google_cloud_gke_backup.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-03-27 14:58:14.000000 google-cloud-gke-backup-0.4.3/google_cloud_gke_backup.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-03-27 14:58:14.000000 google-cloud-gke-backup-0.4.3/google_cloud_gke_backup.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      315 2023-03-27 14:58:14.000000 google-cloud-gke-backup-0.4.3/google_cloud_gke_backup.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-03-27 14:58:14.000000 google-cloud-gke-backup-0.4.3/google_cloud_gke_backup.egg-info/top_level.txt
--rw-rw-r--   0 root         (0)     1003       67 2023-03-27 14:58:14.738238 google-cloud-gke-backup-0.4.3/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2933 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:14.734239 google-cloud-gke-backup-0.4.3/tests/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:14.734239 google-cloud-gke-backup-0.4.3/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:14.734239 google-cloud-gke-backup-0.4.3/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-03-27 14:58:14.734239 google-cloud-gke-backup-0.4.3/tests/unit/gapic/gke_backup_v1/
--rw-rw-r--   0 root         (0)     1003      600 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/tests/unit/gapic/gke_backup_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   597772 2023-03-27 14:56:22.000000 google-cloud-gke-backup-0.4.3/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     4778 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3866 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.242712 google-cloud-gke-backup-0.4.4/google/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.242712 google-cloud-gke-backup-0.4.4/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.246713 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup/
+-rw-rw-r--   0 root         (0)     1003     3498 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.246713 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/
+-rw-rw-r--   0 root         (0)     1003     3181 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9647 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       84 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.246713 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.246713 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/
+-rw-rw-r--   0 root         (0)     1003      761 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py
+-rw-rw-r--   0 root         (0)     1003   159833 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py
+-rw-rw-r--   0 root         (0)     1003   173179 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/client.py
+-rw-rw-r--   0 root         (0)     1003    31038 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.250713 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/
+-rw-rw-r--   0 root         (0)     1003     1372 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    22951 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    46982 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    47961 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   166853 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.250713 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/
+-rw-rw-r--   0 root         (0)     1003     2884 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    14215 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/backup.py
+-rw-rw-r--   0 root         (0)     1003    11959 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/backup_plan.py
+-rw-rw-r--   0 root         (0)     1003     2520 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/common.py
+-rw-rw-r--   0 root         (0)     1003    36417 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/gkebackup.py
+-rw-rw-r--   0 root         (0)     1003    22577 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/restore.py
+-rw-rw-r--   0 root         (0)     1003     4643 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/restore_plan.py
+-rw-rw-r--   0 root         (0)     1003    12236 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/volume.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/
+-rw-r--r--   0 root         (0)     1003     4778 2023-06-13 15:00:12.000000 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1851 2023-06-13 15:00:12.000000 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-13 15:00:12.000000 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-06-13 15:00:12.000000 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-06-13 15:00:12.000000 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      352 2023-06-13 15:00:12.000000 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-06-13 15:00:12.000000 google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/top_level.txt
+-rw-rw-r--   0 root         (0)     1003       67 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2980 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-06-13 15:00:12.254714 google-cloud-gke-backup-0.4.4/tests/unit/gapic/gke_backup_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/tests/unit/gapic/gke_backup_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   666141 2023-06-13 14:58:11.000000 google-cloud-gke-backup-0.4.4/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py
```

### Comparing `google-cloud-gke-backup-0.4.3/LICENSE` & `google-cloud-gke-backup-0.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/MANIFEST.in` & `google-cloud-gke-backup-0.4.4/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/PKG-INFO` & `google-cloud-gke-backup-0.4.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-backup
-Version: 0.4.3
+Version: 0.4.4
 Summary: Google Cloud Gke Backup API client library
 Home-page: https://github.com/googleapis/python-gke-backup
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-gke-backup-0.4.3/README.rst` & `google-cloud-gke-backup-0.4.4/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup/__init__.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup/gapic_version.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.4.3"  # {x-release-please-version}
+__version__ = "0.4.4"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/__init__.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/gapic_metadata.json` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/gapic_version.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/gapic_version.py`

 * *Files 18% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.4.3"  # {x-release-please-version}
+__version__ = "0.4.4"  # {x-release-please-version}
```

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/__init__.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/async_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -40,14 +40,18 @@
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
+from google.iam.v1 import iam_policy_pb2  # type: ignore
+from google.iam.v1 import policy_pb2  # type: ignore
+from google.longrunning import operations_pb2
 from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 
 from google.cloud.gke_backup_v1.services.backup_for_gke import pagers
 from google.cloud.gke_backup_v1.types import backup
 from google.cloud.gke_backup_v1.types import backup as gcg_backup
@@ -3293,14 +3297,639 @@
             client_info=DEFAULT_CLIENT_INFO,
         )
 
         # Certain fields should be provided within the metadata header;
         # add these here.
         metadata = tuple(metadata) + (
             gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def list_operations(
+        self,
+        request: Optional[operations_pb2.ListOperationsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operations_pb2.ListOperationsResponse:
+        r"""Lists operations that match the specified filter in the request.
+
+        Args:
+            request (:class:`~.operations_pb2.ListOperationsRequest`):
+                The request object. Request message for
+                `ListOperations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.operations_pb2.ListOperationsResponse:
+                Response message for ``ListOperations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.ListOperationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.list_operations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def get_operation(
+        self,
+        request: Optional[operations_pb2.GetOperationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operations_pb2.Operation:
+        r"""Gets the latest state of a long-running operation.
+
+        Args:
+            request (:class:`~.operations_pb2.GetOperationRequest`):
+                The request object. Request message for
+                `GetOperation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.operations_pb2.Operation:
+                An ``Operation`` object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.GetOperationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.get_operation,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def delete_operation(
+        self,
+        request: Optional[operations_pb2.DeleteOperationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> None:
+        r"""Deletes a long-running operation.
+
+        This method indicates that the client is no longer interested
+        in the operation result. It does not cancel the operation.
+        If the server doesn't support this method, it returns
+        `google.rpc.Code.UNIMPLEMENTED`.
+
+        Args:
+            request (:class:`~.operations_pb2.DeleteOperationRequest`):
+                The request object. Request message for
+                `DeleteOperation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            None
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.DeleteOperationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.delete_operation,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+    async def cancel_operation(
+        self,
+        request: Optional[operations_pb2.CancelOperationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> None:
+        r"""Starts asynchronous cancellation on a long-running operation.
+
+        The server makes a best effort to cancel the operation, but success
+        is not guaranteed.  If the server doesn't support this method, it returns
+        `google.rpc.Code.UNIMPLEMENTED`.
+
+        Args:
+            request (:class:`~.operations_pb2.CancelOperationRequest`):
+                The request object. Request message for
+                `CancelOperation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            None
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.CancelOperationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.cancel_operation,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+    async def set_iam_policy(
+        self,
+        request: Optional[iam_policy_pb2.SetIamPolicyRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> policy_pb2.Policy:
+        r"""Sets the IAM access control policy on the specified function.
+
+        Replaces any existing policy.
+
+        Args:
+            request (:class:`~.iam_policy_pb2.SetIamPolicyRequest`):
+                The request object. Request message for `SetIamPolicy`
+                method.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.policy_pb2.Policy:
+                Defines an Identity and Access Management (IAM) policy.
+                It is used to specify access control policies for Cloud
+                Platform resources.
+                A ``Policy`` is a collection of ``bindings``. A
+                ``binding`` binds one or more ``members`` to a single
+                ``role``. Members can be user accounts, service
+                accounts, Google groups, and domains (such as G Suite).
+                A ``role`` is a named list of permissions (defined by
+                IAM or configured by users). A ``binding`` can
+                optionally specify a ``condition``, which is a logic
+                expression that further constrains the role binding
+                based on attributes about the request and/or target
+                resource.
+
+                **JSON Example**
+
+                ::
+
+                    {
+                      "bindings": [
+                        {
+                          "role": "roles/resourcemanager.organizationAdmin",
+                          "members": [
+                            "user:mike@example.com",
+                            "group:admins@example.com",
+                            "domain:google.com",
+                            "serviceAccount:my-project-id@appspot.gserviceaccount.com"
+                          ]
+                        },
+                        {
+                          "role": "roles/resourcemanager.organizationViewer",
+                          "members": ["user:eve@example.com"],
+                          "condition": {
+                            "title": "expirable access",
+                            "description": "Does not grant access after Sep 2020",
+                            "expression": "request.time <
+                            timestamp('2020-10-01T00:00:00.000Z')",
+                          }
+                        }
+                      ]
+                    }
+
+                **YAML Example**
+
+                ::
+
+                    bindings:
+                    - members:
+                      - user:mike@example.com
+                      - group:admins@example.com
+                      - domain:google.com
+                      - serviceAccount:my-project-id@appspot.gserviceaccount.com
+                      role: roles/resourcemanager.organizationAdmin
+                    - members:
+                      - user:eve@example.com
+                      role: roles/resourcemanager.organizationViewer
+                      condition:
+                        title: expirable access
+                        description: Does not grant access after Sep 2020
+                        expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
+
+                For a description of IAM and its features, see the `IAM
+                developer's
+                guide <https://cloud.google.com/iam/docs>`__.
+        """
+        # Create or coerce a protobuf request object.
+
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = iam_policy_pb2.SetIamPolicyRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.set_iam_policy,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("resource", request.resource),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def get_iam_policy(
+        self,
+        request: Optional[iam_policy_pb2.GetIamPolicyRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> policy_pb2.Policy:
+        r"""Gets the IAM access control policy for a function.
+
+        Returns an empty policy if the function exists and does not have a
+        policy set.
+
+        Args:
+            request (:class:`~.iam_policy_pb2.GetIamPolicyRequest`):
+                The request object. Request message for `GetIamPolicy`
+                method.
+            retry (google.api_core.retry.Retry): Designation of what errors, if
+                any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.policy_pb2.Policy:
+                Defines an Identity and Access Management (IAM) policy.
+                It is used to specify access control policies for Cloud
+                Platform resources.
+                A ``Policy`` is a collection of ``bindings``. A
+                ``binding`` binds one or more ``members`` to a single
+                ``role``. Members can be user accounts, service
+                accounts, Google groups, and domains (such as G Suite).
+                A ``role`` is a named list of permissions (defined by
+                IAM or configured by users). A ``binding`` can
+                optionally specify a ``condition``, which is a logic
+                expression that further constrains the role binding
+                based on attributes about the request and/or target
+                resource.
+
+                **JSON Example**
+
+                ::
+
+                    {
+                      "bindings": [
+                        {
+                          "role": "roles/resourcemanager.organizationAdmin",
+                          "members": [
+                            "user:mike@example.com",
+                            "group:admins@example.com",
+                            "domain:google.com",
+                            "serviceAccount:my-project-id@appspot.gserviceaccount.com"
+                          ]
+                        },
+                        {
+                          "role": "roles/resourcemanager.organizationViewer",
+                          "members": ["user:eve@example.com"],
+                          "condition": {
+                            "title": "expirable access",
+                            "description": "Does not grant access after Sep 2020",
+                            "expression": "request.time <
+                            timestamp('2020-10-01T00:00:00.000Z')",
+                          }
+                        }
+                      ]
+                    }
+
+                **YAML Example**
+
+                ::
+
+                    bindings:
+                    - members:
+                      - user:mike@example.com
+                      - group:admins@example.com
+                      - domain:google.com
+                      - serviceAccount:my-project-id@appspot.gserviceaccount.com
+                      role: roles/resourcemanager.organizationAdmin
+                    - members:
+                      - user:eve@example.com
+                      role: roles/resourcemanager.organizationViewer
+                      condition:
+                        title: expirable access
+                        description: Does not grant access after Sep 2020
+                        expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
+
+                For a description of IAM and its features, see the `IAM
+                developer's
+                guide <https://cloud.google.com/iam/docs>`__.
+        """
+        # Create or coerce a protobuf request object.
+
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = iam_policy_pb2.GetIamPolicyRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.get_iam_policy,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("resource", request.resource),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def test_iam_permissions(
+        self,
+        request: Optional[iam_policy_pb2.TestIamPermissionsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> iam_policy_pb2.TestIamPermissionsResponse:
+        r"""Tests the specified IAM permissions against the IAM access control
+            policy for a function.
+
+        If the function does not exist, this will return an empty set
+        of permissions, not a NOT_FOUND error.
+
+        Args:
+            request (:class:`~.iam_policy_pb2.TestIamPermissionsRequest`):
+                The request object. Request message for
+                `TestIamPermissions` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.iam_policy_pb2.TestIamPermissionsResponse:
+                Response message for ``TestIamPermissions`` method.
+        """
+        # Create or coerce a protobuf request object.
+
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = iam_policy_pb2.TestIamPermissionsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.test_iam_permissions,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("resource", request.resource),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def get_location(
+        self,
+        request: Optional[locations_pb2.GetLocationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.Location:
+        r"""Gets information about a location.
+
+        Args:
+            request (:class:`~.location_pb2.GetLocationRequest`):
+                The request object. Request message for
+                `GetLocation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.Location:
+                Location object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.GetLocationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.get_location,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = await rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    async def list_locations(
+        self,
+        request: Optional[locations_pb2.ListLocationsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.ListLocationsResponse:
+        r"""Lists information about the supported locations for this service.
+
+        Args:
+            request (:class:`~.location_pb2.ListLocationsRequest`):
+                The request object. Request message for
+                `ListLocations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.ListLocationsResponse:
+                Response message for ``ListLocations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.ListLocationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._client._transport.list_locations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
         )
 
         # Send the request.
         response = await rpc(
             request,
             retry=retry,
             timeout=timeout,
```

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/client.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/client.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,14 +44,18 @@
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
     OptionalRetry = Union[retries.Retry, object]  # type: ignore
 
 from google.api_core import operation  # type: ignore
 from google.api_core import operation_async  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
+from google.iam.v1 import iam_policy_pb2  # type: ignore
+from google.iam.v1 import policy_pb2  # type: ignore
+from google.longrunning import operations_pb2
 from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import timestamp_pb2  # type: ignore
 
 from google.cloud.gke_backup_v1.services.backup_for_gke import pagers
 from google.cloud.gke_backup_v1.types import backup
 from google.cloud.gke_backup_v1.types import backup as gcg_backup
@@ -3596,14 +3600,639 @@
         .. warning::
             ONLY use as a context manager if the transport is NOT shared
             with other clients! Exiting the with block will CLOSE the transport
             and may cause errors in other clients!
         """
         self.transport.close()
 
+    def list_operations(
+        self,
+        request: Optional[operations_pb2.ListOperationsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operations_pb2.ListOperationsResponse:
+        r"""Lists operations that match the specified filter in the request.
+
+        Args:
+            request (:class:`~.operations_pb2.ListOperationsRequest`):
+                The request object. Request message for
+                `ListOperations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.operations_pb2.ListOperationsResponse:
+                Response message for ``ListOperations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.ListOperationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.list_operations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def get_operation(
+        self,
+        request: Optional[operations_pb2.GetOperationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> operations_pb2.Operation:
+        r"""Gets the latest state of a long-running operation.
+
+        Args:
+            request (:class:`~.operations_pb2.GetOperationRequest`):
+                The request object. Request message for
+                `GetOperation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.operations_pb2.Operation:
+                An ``Operation`` object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.GetOperationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.get_operation,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def delete_operation(
+        self,
+        request: Optional[operations_pb2.DeleteOperationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> None:
+        r"""Deletes a long-running operation.
+
+        This method indicates that the client is no longer interested
+        in the operation result. It does not cancel the operation.
+        If the server doesn't support this method, it returns
+        `google.rpc.Code.UNIMPLEMENTED`.
+
+        Args:
+            request (:class:`~.operations_pb2.DeleteOperationRequest`):
+                The request object. Request message for
+                `DeleteOperation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            None
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.DeleteOperationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.delete_operation,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+    def cancel_operation(
+        self,
+        request: Optional[operations_pb2.CancelOperationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> None:
+        r"""Starts asynchronous cancellation on a long-running operation.
+
+        The server makes a best effort to cancel the operation, but success
+        is not guaranteed.  If the server doesn't support this method, it returns
+        `google.rpc.Code.UNIMPLEMENTED`.
+
+        Args:
+            request (:class:`~.operations_pb2.CancelOperationRequest`):
+                The request object. Request message for
+                `CancelOperation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                    if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            None
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = operations_pb2.CancelOperationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.cancel_operation,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+    def set_iam_policy(
+        self,
+        request: Optional[iam_policy_pb2.SetIamPolicyRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> policy_pb2.Policy:
+        r"""Sets the IAM access control policy on the specified function.
+
+        Replaces any existing policy.
+
+        Args:
+            request (:class:`~.iam_policy_pb2.SetIamPolicyRequest`):
+                The request object. Request message for `SetIamPolicy`
+                method.
+            retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.policy_pb2.Policy:
+                Defines an Identity and Access Management (IAM) policy.
+                It is used to specify access control policies for Cloud
+                Platform resources.
+                A ``Policy`` is a collection of ``bindings``. A
+                ``binding`` binds one or more ``members`` to a single
+                ``role``. Members can be user accounts, service
+                accounts, Google groups, and domains (such as G Suite).
+                A ``role`` is a named list of permissions (defined by
+                IAM or configured by users). A ``binding`` can
+                optionally specify a ``condition``, which is a logic
+                expression that further constrains the role binding
+                based on attributes about the request and/or target
+                resource.
+
+                **JSON Example**
+
+                ::
+
+                    {
+                      "bindings": [
+                        {
+                          "role": "roles/resourcemanager.organizationAdmin",
+                          "members": [
+                            "user:mike@example.com",
+                            "group:admins@example.com",
+                            "domain:google.com",
+                            "serviceAccount:my-project-id@appspot.gserviceaccount.com"
+                          ]
+                        },
+                        {
+                          "role": "roles/resourcemanager.organizationViewer",
+                          "members": ["user:eve@example.com"],
+                          "condition": {
+                            "title": "expirable access",
+                            "description": "Does not grant access after Sep 2020",
+                            "expression": "request.time <
+                            timestamp('2020-10-01T00:00:00.000Z')",
+                          }
+                        }
+                      ]
+                    }
+
+                **YAML Example**
+
+                ::
+
+                    bindings:
+                    - members:
+                      - user:mike@example.com
+                      - group:admins@example.com
+                      - domain:google.com
+                      - serviceAccount:my-project-id@appspot.gserviceaccount.com
+                      role: roles/resourcemanager.organizationAdmin
+                    - members:
+                      - user:eve@example.com
+                      role: roles/resourcemanager.organizationViewer
+                      condition:
+                        title: expirable access
+                        description: Does not grant access after Sep 2020
+                        expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
+
+                For a description of IAM and its features, see the `IAM
+                developer's
+                guide <https://cloud.google.com/iam/docs>`__.
+        """
+        # Create or coerce a protobuf request object.
+
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = iam_policy_pb2.SetIamPolicyRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.set_iam_policy,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("resource", request.resource),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def get_iam_policy(
+        self,
+        request: Optional[iam_policy_pb2.GetIamPolicyRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> policy_pb2.Policy:
+        r"""Gets the IAM access control policy for a function.
+
+        Returns an empty policy if the function exists and does not have a
+        policy set.
+
+        Args:
+            request (:class:`~.iam_policy_pb2.GetIamPolicyRequest`):
+                The request object. Request message for `GetIamPolicy`
+                method.
+            retry (google.api_core.retry.Retry): Designation of what errors, if
+                any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.policy_pb2.Policy:
+                Defines an Identity and Access Management (IAM) policy.
+                It is used to specify access control policies for Cloud
+                Platform resources.
+                A ``Policy`` is a collection of ``bindings``. A
+                ``binding`` binds one or more ``members`` to a single
+                ``role``. Members can be user accounts, service
+                accounts, Google groups, and domains (such as G Suite).
+                A ``role`` is a named list of permissions (defined by
+                IAM or configured by users). A ``binding`` can
+                optionally specify a ``condition``, which is a logic
+                expression that further constrains the role binding
+                based on attributes about the request and/or target
+                resource.
+
+                **JSON Example**
+
+                ::
+
+                    {
+                      "bindings": [
+                        {
+                          "role": "roles/resourcemanager.organizationAdmin",
+                          "members": [
+                            "user:mike@example.com",
+                            "group:admins@example.com",
+                            "domain:google.com",
+                            "serviceAccount:my-project-id@appspot.gserviceaccount.com"
+                          ]
+                        },
+                        {
+                          "role": "roles/resourcemanager.organizationViewer",
+                          "members": ["user:eve@example.com"],
+                          "condition": {
+                            "title": "expirable access",
+                            "description": "Does not grant access after Sep 2020",
+                            "expression": "request.time <
+                            timestamp('2020-10-01T00:00:00.000Z')",
+                          }
+                        }
+                      ]
+                    }
+
+                **YAML Example**
+
+                ::
+
+                    bindings:
+                    - members:
+                      - user:mike@example.com
+                      - group:admins@example.com
+                      - domain:google.com
+                      - serviceAccount:my-project-id@appspot.gserviceaccount.com
+                      role: roles/resourcemanager.organizationAdmin
+                    - members:
+                      - user:eve@example.com
+                      role: roles/resourcemanager.organizationViewer
+                      condition:
+                        title: expirable access
+                        description: Does not grant access after Sep 2020
+                        expression: request.time < timestamp('2020-10-01T00:00:00.000Z')
+
+                For a description of IAM and its features, see the `IAM
+                developer's
+                guide <https://cloud.google.com/iam/docs>`__.
+        """
+        # Create or coerce a protobuf request object.
+
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = iam_policy_pb2.GetIamPolicyRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.get_iam_policy,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("resource", request.resource),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def test_iam_permissions(
+        self,
+        request: Optional[iam_policy_pb2.TestIamPermissionsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> iam_policy_pb2.TestIamPermissionsResponse:
+        r"""Tests the specified IAM permissions against the IAM access control
+            policy for a function.
+
+        If the function does not exist, this will return an empty set
+        of permissions, not a NOT_FOUND error.
+
+        Args:
+            request (:class:`~.iam_policy_pb2.TestIamPermissionsRequest`):
+                The request object. Request message for
+                `TestIamPermissions` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.iam_policy_pb2.TestIamPermissionsResponse:
+                Response message for ``TestIamPermissions`` method.
+        """
+        # Create or coerce a protobuf request object.
+
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = iam_policy_pb2.TestIamPermissionsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.test_iam_permissions,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("resource", request.resource),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def get_location(
+        self,
+        request: Optional[locations_pb2.GetLocationRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.Location:
+        r"""Gets information about a location.
+
+        Args:
+            request (:class:`~.location_pb2.GetLocationRequest`):
+                The request object. Request message for
+                `GetLocation` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.Location:
+                Location object.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.GetLocationRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.get_location,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
+    def list_locations(
+        self,
+        request: Optional[locations_pb2.ListLocationsRequest] = None,
+        *,
+        retry: OptionalRetry = gapic_v1.method.DEFAULT,
+        timeout: Union[float, object] = gapic_v1.method.DEFAULT,
+        metadata: Sequence[Tuple[str, str]] = (),
+    ) -> locations_pb2.ListLocationsResponse:
+        r"""Lists information about the supported locations for this service.
+
+        Args:
+            request (:class:`~.location_pb2.ListLocationsRequest`):
+                The request object. Request message for
+                `ListLocations` method.
+            retry (google.api_core.retry.Retry): Designation of what errors,
+                 if any, should be retried.
+            timeout (float): The timeout for this request.
+            metadata (Sequence[Tuple[str, str]]): Strings which should be
+                sent along with the request as metadata.
+        Returns:
+            ~.location_pb2.ListLocationsResponse:
+                Response message for ``ListLocations`` method.
+        """
+        # Create or coerce a protobuf request object.
+        # The request isn't a proto-plus wrapped type,
+        # so it must be constructed via keyword expansion.
+        if isinstance(request, dict):
+            request = locations_pb2.ListLocationsRequest(**request)
+
+        # Wrap the RPC method; this adds retry and timeout information,
+        # and friendly error handling.
+        rpc = gapic_v1.method.wrap_method(
+            self._transport.list_locations,
+            default_timeout=None,
+            client_info=DEFAULT_CLIENT_INFO,
+        )
+
+        # Certain fields should be provided within the metadata header;
+        # add these here.
+        metadata = tuple(metadata) + (
+            gapic_v1.routing_header.to_grpc_metadata((("name", request.name),)),
+        )
+
+        # Send the request.
+        response = rpc(
+            request,
+            retry=retry,
+            timeout=timeout,
+            metadata=metadata,
+        )
+
+        # Done; return the response.
+        return response
+
 
 DEFAULT_CLIENT_INFO = gapic_v1.client_info.ClientInfo(
     gapic_version=package_version.__version__
 )
 
 
 __all__ = ("BackupForGKEClient",)
```

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/base.py`

 * *Files 8% similar despite different names*

```diff
@@ -18,14 +18,17 @@
 
 import google.api_core
 from google.api_core import exceptions as core_exceptions
 from google.api_core import gapic_v1, operations_v1
 from google.api_core import retry as retries
 import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
+from google.iam.v1 import iam_policy_pb2  # type: ignore
+from google.iam.v1 import policy_pb2  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 from google.oauth2 import service_account  # type: ignore
 
 from google.cloud.gke_backup_v1 import gapic_version as package_version
 from google.cloud.gke_backup_v1.types import (
     backup,
     backup_plan,
@@ -600,12 +603,96 @@
     ) -> Callable[
         [gkebackup.GetVolumeRestoreRequest],
         Union[volume.VolumeRestore, Awaitable[volume.VolumeRestore]],
     ]:
         raise NotImplementedError()
 
     @property
+    def list_operations(
+        self,
+    ) -> Callable[
+        [operations_pb2.ListOperationsRequest],
+        Union[
+            operations_pb2.ListOperationsResponse,
+            Awaitable[operations_pb2.ListOperationsResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def get_operation(
+        self,
+    ) -> Callable[
+        [operations_pb2.GetOperationRequest],
+        Union[operations_pb2.Operation, Awaitable[operations_pb2.Operation]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def cancel_operation(
+        self,
+    ) -> Callable[[operations_pb2.CancelOperationRequest], None,]:
+        raise NotImplementedError()
+
+    @property
+    def delete_operation(
+        self,
+    ) -> Callable[[operations_pb2.DeleteOperationRequest], None,]:
+        raise NotImplementedError()
+
+    @property
+    def set_iam_policy(
+        self,
+    ) -> Callable[
+        [iam_policy_pb2.SetIamPolicyRequest],
+        Union[policy_pb2.Policy, Awaitable[policy_pb2.Policy]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def get_iam_policy(
+        self,
+    ) -> Callable[
+        [iam_policy_pb2.GetIamPolicyRequest],
+        Union[policy_pb2.Policy, Awaitable[policy_pb2.Policy]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def test_iam_permissions(
+        self,
+    ) -> Callable[
+        [iam_policy_pb2.TestIamPermissionsRequest],
+        Union[
+            iam_policy_pb2.TestIamPermissionsResponse,
+            Awaitable[iam_policy_pb2.TestIamPermissionsResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def get_location(
+        self,
+    ) -> Callable[
+        [locations_pb2.GetLocationRequest],
+        Union[locations_pb2.Location, Awaitable[locations_pb2.Location]],
+    ]:
+        raise NotImplementedError()
+
+    @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest],
+        Union[
+            locations_pb2.ListLocationsResponse,
+            Awaitable[locations_pb2.ListLocationsResponse],
+        ],
+    ]:
+        raise NotImplementedError()
+
+    @property
     def kind(self) -> str:
         raise NotImplementedError()
 
 
 __all__ = ("BackupForGKETransport",)
```

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,61 +9,109 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
-from google.api_core import gapic_v1, grpc_helpers, operations_v1
-import google.auth  # type: ignore
+from google.api_core import gapic_v1, grpc_helpers_async, operations_v1
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
+from google.iam.v1 import iam_policy_pb2  # type: ignore
+from google.iam.v1 import policy_pb2  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 import grpc  # type: ignore
+from grpc.experimental import aio  # type: ignore
 
 from google.cloud.gke_backup_v1.types import (
     backup,
     backup_plan,
     gkebackup,
     restore,
     restore_plan,
     volume,
 )
 
 from .base import DEFAULT_CLIENT_INFO, BackupForGKETransport
+from .grpc import BackupForGKEGrpcTransport
 
 
-class BackupForGKEGrpcTransport(BackupForGKETransport):
-    """gRPC backend transport for BackupForGKE.
+class BackupForGKEGrpcAsyncIOTransport(BackupForGKETransport):
+    """gRPC AsyncIO backend transport for BackupForGKE.
 
     BackupForGKE allows Kubernetes administrators to configure,
     execute, and manage backup and restore operations for their GKE
     clusters.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
     """
 
-    _stubs: Dict[str, Callable]
+    _grpc_channel: aio.Channel
+    _stubs: Dict[str, Callable] = {}
+
+    @classmethod
+    def create_channel(
+        cls,
+        host: str = "gkebackup.googleapis.com",
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        quota_project_id: Optional[str] = None,
+        **kwargs,
+    ) -> aio.Channel:
+        """Create and return a gRPC AsyncIO channel object.
+        Args:
+            host (Optional[str]): The host for the channel to use.
+            credentials (Optional[~.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify this application to the service. If
+                none are specified, the client will attempt to ascertain
+                the credentials from the environment.
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is ignored if ``channel`` is provided.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            kwargs (Optional[dict]): Keyword arguments, which are passed to the
+                channel creation.
+        Returns:
+            aio.Channel: A gRPC AsyncIO channel object.
+        """
+
+        return grpc_helpers_async.create_channel(
+            host,
+            credentials=credentials,
+            credentials_file=credentials_file,
+            quota_project_id=quota_project_id,
+            default_scopes=cls.AUTH_SCOPES,
+            scopes=scopes,
+            default_host=cls.DEFAULT_HOST,
+            **kwargs,
+        )
 
     def __init__(
         self,
         *,
         host: str = "gkebackup.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[grpc.Channel] = None,
+        channel: Optional[aio.Channel] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -79,17 +127,18 @@
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
                 This argument is ignored if ``channel`` is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
                 This argument is ignored if ``channel`` is provided.
-            scopes (Optional(Sequence[str])): A list of scopes. This argument is
-                ignored if ``channel`` is provided.
-            channel (Optional[grpc.Channel]): A ``Channel`` instance through
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            channel (Optional[aio.Channel]): A ``Channel`` instance through
                 which to make calls.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
@@ -108,36 +157,35 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
 
         Raises:
-          google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
+            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
               creation failed for any reason.
           google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
               and ``credentials_file`` are passed.
         """
         self._grpc_channel = None
         self._ssl_channel_credentials = ssl_channel_credentials
         self._stubs: Dict[str, Callable] = {}
-        self._operations_client: Optional[operations_v1.OperationsClient] = None
+        self._operations_client: Optional[operations_v1.OperationsAsyncClient] = None
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
         if channel:
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
-
         else:
             if api_mtls_endpoint:
                 host = api_mtls_endpoint
 
                 # Create SSL credentials with client_cert_source or application
                 # default SSL credentials.
                 if client_cert_source:
@@ -183,91 +231,53 @@
                     ("grpc.max_receive_message_length", -1),
                 ],
             )
 
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
-    @classmethod
-    def create_channel(
-        cls,
-        host: str = "gkebackup.googleapis.com",
-        credentials: Optional[ga_credentials.Credentials] = None,
-        credentials_file: Optional[str] = None,
-        scopes: Optional[Sequence[str]] = None,
-        quota_project_id: Optional[str] = None,
-        **kwargs,
-    ) -> grpc.Channel:
-        """Create and return a gRPC channel object.
-        Args:
-            host (Optional[str]): The host for the channel to use.
-            credentials (Optional[~.Credentials]): The
-                authorization credentials to attach to requests. These
-                credentials identify this application to the service. If
-                none are specified, the client will attempt to ascertain
-                the credentials from the environment.
-            credentials_file (Optional[str]): A file with credentials that can
-                be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is mutually exclusive with credentials.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            quota_project_id (Optional[str]): An optional project to use for billing
-                and quota.
-            kwargs (Optional[dict]): Keyword arguments, which are passed to the
-                channel creation.
-        Returns:
-            grpc.Channel: A gRPC channel object.
+    @property
+    def grpc_channel(self) -> aio.Channel:
+        """Create the channel designed to connect to this service.
 
-        Raises:
-            google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
-              and ``credentials_file`` are passed.
+        This property caches on the instance; repeated calls return
+        the same channel.
         """
-
-        return grpc_helpers.create_channel(
-            host,
-            credentials=credentials,
-            credentials_file=credentials_file,
-            quota_project_id=quota_project_id,
-            default_scopes=cls.AUTH_SCOPES,
-            scopes=scopes,
-            default_host=cls.DEFAULT_HOST,
-            **kwargs,
-        )
-
-    @property
-    def grpc_channel(self) -> grpc.Channel:
-        """Return the channel designed to connect to this service."""
+        # Return the channel from cache.
         return self._grpc_channel
 
     @property
-    def operations_client(self) -> operations_v1.OperationsClient:
+    def operations_client(self) -> operations_v1.OperationsAsyncClient:
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
         # Quick check: Only create a new client if we do not already have one.
         if self._operations_client is None:
-            self._operations_client = operations_v1.OperationsClient(self.grpc_channel)
+            self._operations_client = operations_v1.OperationsAsyncClient(
+                self.grpc_channel
+            )
 
         # Return the client from cache.
         return self._operations_client
 
     @property
     def create_backup_plan(
         self,
-    ) -> Callable[[gkebackup.CreateBackupPlanRequest], operations_pb2.Operation]:
+    ) -> Callable[
+        [gkebackup.CreateBackupPlanRequest], Awaitable[operations_pb2.Operation]
+    ]:
         r"""Return a callable for the create backup plan method over gRPC.
 
         Creates a new BackupPlan in a given location.
 
         Returns:
             Callable[[~.CreateBackupPlanRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -279,23 +289,23 @@
             )
         return self._stubs["create_backup_plan"]
 
     @property
     def list_backup_plans(
         self,
     ) -> Callable[
-        [gkebackup.ListBackupPlansRequest], gkebackup.ListBackupPlansResponse
+        [gkebackup.ListBackupPlansRequest], Awaitable[gkebackup.ListBackupPlansResponse]
     ]:
         r"""Return a callable for the list backup plans method over gRPC.
 
         Lists BackupPlans in a given location.
 
         Returns:
             Callable[[~.ListBackupPlansRequest],
-                    ~.ListBackupPlansResponse]:
+                    Awaitable[~.ListBackupPlansResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -306,22 +316,22 @@
                 response_deserializer=gkebackup.ListBackupPlansResponse.deserialize,
             )
         return self._stubs["list_backup_plans"]
 
     @property
     def get_backup_plan(
         self,
-    ) -> Callable[[gkebackup.GetBackupPlanRequest], backup_plan.BackupPlan]:
+    ) -> Callable[[gkebackup.GetBackupPlanRequest], Awaitable[backup_plan.BackupPlan]]:
         r"""Return a callable for the get backup plan method over gRPC.
 
         Retrieve the details of a single BackupPlan.
 
         Returns:
             Callable[[~.GetBackupPlanRequest],
-                    ~.BackupPlan]:
+                    Awaitable[~.BackupPlan]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -332,22 +342,24 @@
                 response_deserializer=backup_plan.BackupPlan.deserialize,
             )
         return self._stubs["get_backup_plan"]
 
     @property
     def update_backup_plan(
         self,
-    ) -> Callable[[gkebackup.UpdateBackupPlanRequest], operations_pb2.Operation]:
+    ) -> Callable[
+        [gkebackup.UpdateBackupPlanRequest], Awaitable[operations_pb2.Operation]
+    ]:
         r"""Return a callable for the update backup plan method over gRPC.
 
         Update a BackupPlan.
 
         Returns:
             Callable[[~.UpdateBackupPlanRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -358,22 +370,24 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_backup_plan"]
 
     @property
     def delete_backup_plan(
         self,
-    ) -> Callable[[gkebackup.DeleteBackupPlanRequest], operations_pb2.Operation]:
+    ) -> Callable[
+        [gkebackup.DeleteBackupPlanRequest], Awaitable[operations_pb2.Operation]
+    ]:
         r"""Return a callable for the delete backup plan method over gRPC.
 
         Deletes an existing BackupPlan.
 
         Returns:
             Callable[[~.DeleteBackupPlanRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -384,22 +398,22 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_backup_plan"]
 
     @property
     def create_backup(
         self,
-    ) -> Callable[[gkebackup.CreateBackupRequest], operations_pb2.Operation]:
+    ) -> Callable[[gkebackup.CreateBackupRequest], Awaitable[operations_pb2.Operation]]:
         r"""Return a callable for the create backup method over gRPC.
 
         Creates a Backup for the given BackupPlan.
 
         Returns:
             Callable[[~.CreateBackupRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -410,22 +424,24 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_backup"]
 
     @property
     def list_backups(
         self,
-    ) -> Callable[[gkebackup.ListBackupsRequest], gkebackup.ListBackupsResponse]:
+    ) -> Callable[
+        [gkebackup.ListBackupsRequest], Awaitable[gkebackup.ListBackupsResponse]
+    ]:
         r"""Return a callable for the list backups method over gRPC.
 
         Lists the Backups for a given BackupPlan.
 
         Returns:
             Callable[[~.ListBackupsRequest],
-                    ~.ListBackupsResponse]:
+                    Awaitable[~.ListBackupsResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -434,22 +450,24 @@
                 "/google.cloud.gkebackup.v1.BackupForGKE/ListBackups",
                 request_serializer=gkebackup.ListBackupsRequest.serialize,
                 response_deserializer=gkebackup.ListBackupsResponse.deserialize,
             )
         return self._stubs["list_backups"]
 
     @property
-    def get_backup(self) -> Callable[[gkebackup.GetBackupRequest], backup.Backup]:
+    def get_backup(
+        self,
+    ) -> Callable[[gkebackup.GetBackupRequest], Awaitable[backup.Backup]]:
         r"""Return a callable for the get backup method over gRPC.
 
         Retrieve the details of a single Backup.
 
         Returns:
             Callable[[~.GetBackupRequest],
-                    ~.Backup]:
+                    Awaitable[~.Backup]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -460,22 +478,22 @@
                 response_deserializer=backup.Backup.deserialize,
             )
         return self._stubs["get_backup"]
 
     @property
     def update_backup(
         self,
-    ) -> Callable[[gkebackup.UpdateBackupRequest], operations_pb2.Operation]:
+    ) -> Callable[[gkebackup.UpdateBackupRequest], Awaitable[operations_pb2.Operation]]:
         r"""Return a callable for the update backup method over gRPC.
 
         Update a Backup.
 
         Returns:
             Callable[[~.UpdateBackupRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -486,22 +504,22 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_backup"]
 
     @property
     def delete_backup(
         self,
-    ) -> Callable[[gkebackup.DeleteBackupRequest], operations_pb2.Operation]:
+    ) -> Callable[[gkebackup.DeleteBackupRequest], Awaitable[operations_pb2.Operation]]:
         r"""Return a callable for the delete backup method over gRPC.
 
         Deletes an existing Backup.
 
         Returns:
             Callable[[~.DeleteBackupRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -513,23 +531,24 @@
             )
         return self._stubs["delete_backup"]
 
     @property
     def list_volume_backups(
         self,
     ) -> Callable[
-        [gkebackup.ListVolumeBackupsRequest], gkebackup.ListVolumeBackupsResponse
+        [gkebackup.ListVolumeBackupsRequest],
+        Awaitable[gkebackup.ListVolumeBackupsResponse],
     ]:
         r"""Return a callable for the list volume backups method over gRPC.
 
         Lists the VolumeBackups for a given Backup.
 
         Returns:
             Callable[[~.ListVolumeBackupsRequest],
-                    ~.ListVolumeBackupsResponse]:
+                    Awaitable[~.ListVolumeBackupsResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -540,22 +559,22 @@
                 response_deserializer=gkebackup.ListVolumeBackupsResponse.deserialize,
             )
         return self._stubs["list_volume_backups"]
 
     @property
     def get_volume_backup(
         self,
-    ) -> Callable[[gkebackup.GetVolumeBackupRequest], volume.VolumeBackup]:
+    ) -> Callable[[gkebackup.GetVolumeBackupRequest], Awaitable[volume.VolumeBackup]]:
         r"""Return a callable for the get volume backup method over gRPC.
 
         Retrieve the details of a single VolumeBackup.
 
         Returns:
             Callable[[~.GetVolumeBackupRequest],
-                    ~.VolumeBackup]:
+                    Awaitable[~.VolumeBackup]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -566,22 +585,24 @@
                 response_deserializer=volume.VolumeBackup.deserialize,
             )
         return self._stubs["get_volume_backup"]
 
     @property
     def create_restore_plan(
         self,
-    ) -> Callable[[gkebackup.CreateRestorePlanRequest], operations_pb2.Operation]:
+    ) -> Callable[
+        [gkebackup.CreateRestorePlanRequest], Awaitable[operations_pb2.Operation]
+    ]:
         r"""Return a callable for the create restore plan method over gRPC.
 
         Creates a new RestorePlan in a given location.
 
         Returns:
             Callable[[~.CreateRestorePlanRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -593,23 +614,24 @@
             )
         return self._stubs["create_restore_plan"]
 
     @property
     def list_restore_plans(
         self,
     ) -> Callable[
-        [gkebackup.ListRestorePlansRequest], gkebackup.ListRestorePlansResponse
+        [gkebackup.ListRestorePlansRequest],
+        Awaitable[gkebackup.ListRestorePlansResponse],
     ]:
         r"""Return a callable for the list restore plans method over gRPC.
 
         Lists RestorePlans in a given location.
 
         Returns:
             Callable[[~.ListRestorePlansRequest],
-                    ~.ListRestorePlansResponse]:
+                    Awaitable[~.ListRestorePlansResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -620,22 +642,24 @@
                 response_deserializer=gkebackup.ListRestorePlansResponse.deserialize,
             )
         return self._stubs["list_restore_plans"]
 
     @property
     def get_restore_plan(
         self,
-    ) -> Callable[[gkebackup.GetRestorePlanRequest], restore_plan.RestorePlan]:
+    ) -> Callable[
+        [gkebackup.GetRestorePlanRequest], Awaitable[restore_plan.RestorePlan]
+    ]:
         r"""Return a callable for the get restore plan method over gRPC.
 
         Retrieve the details of a single RestorePlan.
 
         Returns:
             Callable[[~.GetRestorePlanRequest],
-                    ~.RestorePlan]:
+                    Awaitable[~.RestorePlan]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -646,22 +670,24 @@
                 response_deserializer=restore_plan.RestorePlan.deserialize,
             )
         return self._stubs["get_restore_plan"]
 
     @property
     def update_restore_plan(
         self,
-    ) -> Callable[[gkebackup.UpdateRestorePlanRequest], operations_pb2.Operation]:
+    ) -> Callable[
+        [gkebackup.UpdateRestorePlanRequest], Awaitable[operations_pb2.Operation]
+    ]:
         r"""Return a callable for the update restore plan method over gRPC.
 
         Update a RestorePlan.
 
         Returns:
             Callable[[~.UpdateRestorePlanRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -672,22 +698,24 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_restore_plan"]
 
     @property
     def delete_restore_plan(
         self,
-    ) -> Callable[[gkebackup.DeleteRestorePlanRequest], operations_pb2.Operation]:
+    ) -> Callable[
+        [gkebackup.DeleteRestorePlanRequest], Awaitable[operations_pb2.Operation]
+    ]:
         r"""Return a callable for the delete restore plan method over gRPC.
 
         Deletes an existing RestorePlan.
 
         Returns:
             Callable[[~.DeleteRestorePlanRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -698,22 +726,24 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_restore_plan"]
 
     @property
     def create_restore(
         self,
-    ) -> Callable[[gkebackup.CreateRestoreRequest], operations_pb2.Operation]:
+    ) -> Callable[
+        [gkebackup.CreateRestoreRequest], Awaitable[operations_pb2.Operation]
+    ]:
         r"""Return a callable for the create restore method over gRPC.
 
         Creates a new Restore for the given RestorePlan.
 
         Returns:
             Callable[[~.CreateRestoreRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -724,22 +754,24 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_restore"]
 
     @property
     def list_restores(
         self,
-    ) -> Callable[[gkebackup.ListRestoresRequest], gkebackup.ListRestoresResponse]:
+    ) -> Callable[
+        [gkebackup.ListRestoresRequest], Awaitable[gkebackup.ListRestoresResponse]
+    ]:
         r"""Return a callable for the list restores method over gRPC.
 
         Lists the Restores for a given RestorePlan.
 
         Returns:
             Callable[[~.ListRestoresRequest],
-                    ~.ListRestoresResponse]:
+                    Awaitable[~.ListRestoresResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -748,22 +780,24 @@
                 "/google.cloud.gkebackup.v1.BackupForGKE/ListRestores",
                 request_serializer=gkebackup.ListRestoresRequest.serialize,
                 response_deserializer=gkebackup.ListRestoresResponse.deserialize,
             )
         return self._stubs["list_restores"]
 
     @property
-    def get_restore(self) -> Callable[[gkebackup.GetRestoreRequest], restore.Restore]:
+    def get_restore(
+        self,
+    ) -> Callable[[gkebackup.GetRestoreRequest], Awaitable[restore.Restore]]:
         r"""Return a callable for the get restore method over gRPC.
 
         Retrieves the details of a single Restore.
 
         Returns:
             Callable[[~.GetRestoreRequest],
-                    ~.Restore]:
+                    Awaitable[~.Restore]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -774,22 +808,24 @@
                 response_deserializer=restore.Restore.deserialize,
             )
         return self._stubs["get_restore"]
 
     @property
     def update_restore(
         self,
-    ) -> Callable[[gkebackup.UpdateRestoreRequest], operations_pb2.Operation]:
+    ) -> Callable[
+        [gkebackup.UpdateRestoreRequest], Awaitable[operations_pb2.Operation]
+    ]:
         r"""Return a callable for the update restore method over gRPC.
 
         Update a Restore.
 
         Returns:
             Callable[[~.UpdateRestoreRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -800,22 +836,24 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_restore"]
 
     @property
     def delete_restore(
         self,
-    ) -> Callable[[gkebackup.DeleteRestoreRequest], operations_pb2.Operation]:
+    ) -> Callable[
+        [gkebackup.DeleteRestoreRequest], Awaitable[operations_pb2.Operation]
+    ]:
         r"""Return a callable for the delete restore method over gRPC.
 
         Deletes an existing Restore.
 
         Returns:
             Callable[[~.DeleteRestoreRequest],
-                    ~.Operation]:
+                    Awaitable[~.Operation]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -827,23 +865,24 @@
             )
         return self._stubs["delete_restore"]
 
     @property
     def list_volume_restores(
         self,
     ) -> Callable[
-        [gkebackup.ListVolumeRestoresRequest], gkebackup.ListVolumeRestoresResponse
+        [gkebackup.ListVolumeRestoresRequest],
+        Awaitable[gkebackup.ListVolumeRestoresResponse],
     ]:
         r"""Return a callable for the list volume restores method over gRPC.
 
         Lists the VolumeRestores for a given Restore.
 
         Returns:
             Callable[[~.ListVolumeRestoresRequest],
-                    ~.ListVolumeRestoresResponse]:
+                    Awaitable[~.ListVolumeRestoresResponse]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -854,22 +893,22 @@
                 response_deserializer=gkebackup.ListVolumeRestoresResponse.deserialize,
             )
         return self._stubs["list_volume_restores"]
 
     @property
     def get_volume_restore(
         self,
-    ) -> Callable[[gkebackup.GetVolumeRestoreRequest], volume.VolumeRestore]:
+    ) -> Callable[[gkebackup.GetVolumeRestoreRequest], Awaitable[volume.VolumeRestore]]:
         r"""Return a callable for the get volume restore method over gRPC.
 
         Retrieve the details of a single VolumeRestore.
 
         Returns:
             Callable[[~.GetVolumeRestoreRequest],
-                    ~.VolumeRestore]:
+                    Awaitable[~.VolumeRestore]]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -878,15 +917,197 @@
                 "/google.cloud.gkebackup.v1.BackupForGKE/GetVolumeRestore",
                 request_serializer=gkebackup.GetVolumeRestoreRequest.serialize,
                 response_deserializer=volume.VolumeRestore.deserialize,
             )
         return self._stubs["get_volume_restore"]
 
     def close(self):
-        self.grpc_channel.close()
+        return self.grpc_channel.close()
+
+    @property
+    def delete_operation(
+        self,
+    ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
+        r"""Return a callable for the delete_operation method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "delete_operation" not in self._stubs:
+            self._stubs["delete_operation"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/DeleteOperation",
+                request_serializer=operations_pb2.DeleteOperationRequest.SerializeToString,
+                response_deserializer=None,
+            )
+        return self._stubs["delete_operation"]
+
+    @property
+    def cancel_operation(
+        self,
+    ) -> Callable[[operations_pb2.CancelOperationRequest], None]:
+        r"""Return a callable for the cancel_operation method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "cancel_operation" not in self._stubs:
+            self._stubs["cancel_operation"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/CancelOperation",
+                request_serializer=operations_pb2.CancelOperationRequest.SerializeToString,
+                response_deserializer=None,
+            )
+        return self._stubs["cancel_operation"]
+
+    @property
+    def get_operation(
+        self,
+    ) -> Callable[[operations_pb2.GetOperationRequest], operations_pb2.Operation]:
+        r"""Return a callable for the get_operation method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_operation" not in self._stubs:
+            self._stubs["get_operation"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/GetOperation",
+                request_serializer=operations_pb2.GetOperationRequest.SerializeToString,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["get_operation"]
+
+    @property
+    def list_operations(
+        self,
+    ) -> Callable[
+        [operations_pb2.ListOperationsRequest], operations_pb2.ListOperationsResponse
+    ]:
+        r"""Return a callable for the list_operations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_operations" not in self._stubs:
+            self._stubs["list_operations"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/ListOperations",
+                request_serializer=operations_pb2.ListOperationsRequest.SerializeToString,
+                response_deserializer=operations_pb2.ListOperationsResponse.FromString,
+            )
+        return self._stubs["list_operations"]
+
+    @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest], locations_pb2.ListLocationsResponse
+    ]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_locations" not in self._stubs:
+            self._stubs["list_locations"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/ListLocations",
+                request_serializer=locations_pb2.ListLocationsRequest.SerializeToString,
+                response_deserializer=locations_pb2.ListLocationsResponse.FromString,
+            )
+        return self._stubs["list_locations"]
+
+    @property
+    def get_location(
+        self,
+    ) -> Callable[[locations_pb2.GetLocationRequest], locations_pb2.Location]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_location" not in self._stubs:
+            self._stubs["get_location"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/GetLocation",
+                request_serializer=locations_pb2.GetLocationRequest.SerializeToString,
+                response_deserializer=locations_pb2.Location.FromString,
+            )
+        return self._stubs["get_location"]
+
+    @property
+    def set_iam_policy(
+        self,
+    ) -> Callable[[iam_policy_pb2.SetIamPolicyRequest], policy_pb2.Policy]:
+        r"""Return a callable for the set iam policy method over gRPC.
+        Sets the IAM access control policy on the specified
+        function. Replaces any existing policy.
+        Returns:
+            Callable[[~.SetIamPolicyRequest],
+                    ~.Policy]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "set_iam_policy" not in self._stubs:
+            self._stubs["set_iam_policy"] = self.grpc_channel.unary_unary(
+                "/google.iam.v1.IAMPolicy/SetIamPolicy",
+                request_serializer=iam_policy_pb2.SetIamPolicyRequest.SerializeToString,
+                response_deserializer=policy_pb2.Policy.FromString,
+            )
+        return self._stubs["set_iam_policy"]
+
+    @property
+    def get_iam_policy(
+        self,
+    ) -> Callable[[iam_policy_pb2.GetIamPolicyRequest], policy_pb2.Policy]:
+        r"""Return a callable for the get iam policy method over gRPC.
+        Gets the IAM access control policy for a function.
+        Returns an empty policy if the function exists and does
+        not have a policy set.
+        Returns:
+            Callable[[~.GetIamPolicyRequest],
+                    ~.Policy]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_iam_policy" not in self._stubs:
+            self._stubs["get_iam_policy"] = self.grpc_channel.unary_unary(
+                "/google.iam.v1.IAMPolicy/GetIamPolicy",
+                request_serializer=iam_policy_pb2.GetIamPolicyRequest.SerializeToString,
+                response_deserializer=policy_pb2.Policy.FromString,
+            )
+        return self._stubs["get_iam_policy"]
 
     @property
-    def kind(self) -> str:
-        return "grpc"
+    def test_iam_permissions(
+        self,
+    ) -> Callable[
+        [iam_policy_pb2.TestIamPermissionsRequest],
+        iam_policy_pb2.TestIamPermissionsResponse,
+    ]:
+        r"""Return a callable for the test iam permissions method over gRPC.
+        Tests the specified permissions against the IAM access control
+        policy for a function. If the function does not exist, this will
+        return an empty set of permissions, not a NOT_FOUND error.
+        Returns:
+            Callable[[~.TestIamPermissionsRequest],
+                    ~.TestIamPermissionsResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "test_iam_permissions" not in self._stubs:
+            self._stubs["test_iam_permissions"] = self.grpc_channel.unary_unary(
+                "/google.iam.v1.IAMPolicy/TestIamPermissions",
+                request_serializer=iam_policy_pb2.TestIamPermissionsRequest.SerializeToString,
+                response_deserializer=iam_policy_pb2.TestIamPermissionsResponse.FromString,
+            )
+        return self._stubs["test_iam_permissions"]
 
 
-__all__ = ("BackupForGKEGrpcTransport",)
+__all__ = ("BackupForGKEGrpcAsyncIOTransport",)
```

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc_asyncio.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/grpc.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,106 +9,64 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-from typing import Awaitable, Callable, Dict, Optional, Sequence, Tuple, Union
+from typing import Callable, Dict, Optional, Sequence, Tuple, Union
 import warnings
 
-from google.api_core import gapic_v1, grpc_helpers_async, operations_v1
+from google.api_core import gapic_v1, grpc_helpers, operations_v1
+import google.auth  # type: ignore
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
+from google.iam.v1 import iam_policy_pb2  # type: ignore
+from google.iam.v1 import policy_pb2  # type: ignore
 from google.longrunning import operations_pb2  # type: ignore
 import grpc  # type: ignore
-from grpc.experimental import aio  # type: ignore
 
 from google.cloud.gke_backup_v1.types import (
     backup,
     backup_plan,
     gkebackup,
     restore,
     restore_plan,
     volume,
 )
 
 from .base import DEFAULT_CLIENT_INFO, BackupForGKETransport
-from .grpc import BackupForGKEGrpcTransport
 
 
-class BackupForGKEGrpcAsyncIOTransport(BackupForGKETransport):
-    """gRPC AsyncIO backend transport for BackupForGKE.
+class BackupForGKEGrpcTransport(BackupForGKETransport):
+    """gRPC backend transport for BackupForGKE.
 
     BackupForGKE allows Kubernetes administrators to configure,
     execute, and manage backup and restore operations for their GKE
     clusters.
 
     This class defines the same methods as the primary client, so the
     primary client can load the underlying transport implementation
     and call it.
 
     It sends protocol buffers over the wire using gRPC (which is built on
     top of HTTP/2); the ``grpcio`` package must be installed.
     """
 
-    _grpc_channel: aio.Channel
-    _stubs: Dict[str, Callable] = {}
-
-    @classmethod
-    def create_channel(
-        cls,
-        host: str = "gkebackup.googleapis.com",
-        credentials: Optional[ga_credentials.Credentials] = None,
-        credentials_file: Optional[str] = None,
-        scopes: Optional[Sequence[str]] = None,
-        quota_project_id: Optional[str] = None,
-        **kwargs,
-    ) -> aio.Channel:
-        """Create and return a gRPC AsyncIO channel object.
-        Args:
-            host (Optional[str]): The host for the channel to use.
-            credentials (Optional[~.Credentials]): The
-                authorization credentials to attach to requests. These
-                credentials identify this application to the service. If
-                none are specified, the client will attempt to ascertain
-                the credentials from the environment.
-            credentials_file (Optional[str]): A file with credentials that can
-                be loaded with :func:`google.auth.load_credentials_from_file`.
-                This argument is ignored if ``channel`` is provided.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            quota_project_id (Optional[str]): An optional project to use for billing
-                and quota.
-            kwargs (Optional[dict]): Keyword arguments, which are passed to the
-                channel creation.
-        Returns:
-            aio.Channel: A gRPC AsyncIO channel object.
-        """
-
-        return grpc_helpers_async.create_channel(
-            host,
-            credentials=credentials,
-            credentials_file=credentials_file,
-            quota_project_id=quota_project_id,
-            default_scopes=cls.AUTH_SCOPES,
-            scopes=scopes,
-            default_host=cls.DEFAULT_HOST,
-            **kwargs,
-        )
+    _stubs: Dict[str, Callable]
 
     def __init__(
         self,
         *,
         host: str = "gkebackup.googleapis.com",
         credentials: Optional[ga_credentials.Credentials] = None,
         credentials_file: Optional[str] = None,
         scopes: Optional[Sequence[str]] = None,
-        channel: Optional[aio.Channel] = None,
+        channel: Optional[grpc.Channel] = None,
         api_mtls_endpoint: Optional[str] = None,
         client_cert_source: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         ssl_channel_credentials: Optional[grpc.ChannelCredentials] = None,
         client_cert_source_for_mtls: Optional[Callable[[], Tuple[bytes, bytes]]] = None,
         quota_project_id: Optional[str] = None,
         client_info: gapic_v1.client_info.ClientInfo = DEFAULT_CLIENT_INFO,
         always_use_jwt_access: Optional[bool] = False,
@@ -124,18 +82,17 @@
                 credentials identify the application to the service; if none
                 are specified, the client will attempt to ascertain the
                 credentials from the environment.
                 This argument is ignored if ``channel`` is provided.
             credentials_file (Optional[str]): A file with credentials that can
                 be loaded with :func:`google.auth.load_credentials_from_file`.
                 This argument is ignored if ``channel`` is provided.
-            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
-                service. These are only used when credentials are not specified and
-                are passed to :func:`google.auth.default`.
-            channel (Optional[aio.Channel]): A ``Channel`` instance through
+            scopes (Optional(Sequence[str])): A list of scopes. This argument is
+                ignored if ``channel`` is provided.
+            channel (Optional[grpc.Channel]): A ``Channel`` instance through
                 which to make calls.
             api_mtls_endpoint (Optional[str]): Deprecated. The mutual TLS endpoint.
                 If provided, it overrides the ``host`` argument and tries to create
                 a mutual TLS channel with client SSL credentials from
                 ``client_cert_source`` or application default SSL credentials.
             client_cert_source (Optional[Callable[[], Tuple[bytes, bytes]]]):
                 Deprecated. A callback to provide client SSL certificate bytes and
@@ -154,35 +111,36 @@
                 API requests. If ``None``, then default info will be used.
                 Generally, you only need to set this if you're developing
                 your own client library.
             always_use_jwt_access (Optional[bool]): Whether self signed JWT should
                 be used for service account credentials.
 
         Raises:
-            google.auth.exceptions.MutualTlsChannelError: If mutual TLS transport
+          google.auth.exceptions.MutualTLSChannelError: If mutual TLS transport
               creation failed for any reason.
           google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
               and ``credentials_file`` are passed.
         """
         self._grpc_channel = None
         self._ssl_channel_credentials = ssl_channel_credentials
         self._stubs: Dict[str, Callable] = {}
-        self._operations_client: Optional[operations_v1.OperationsAsyncClient] = None
+        self._operations_client: Optional[operations_v1.OperationsClient] = None
 
         if api_mtls_endpoint:
             warnings.warn("api_mtls_endpoint is deprecated", DeprecationWarning)
         if client_cert_source:
             warnings.warn("client_cert_source is deprecated", DeprecationWarning)
 
         if channel:
             # Ignore credentials if a channel was passed.
             credentials = False
             # If a channel was explicitly provided, set it.
             self._grpc_channel = channel
             self._ssl_channel_credentials = None
+
         else:
             if api_mtls_endpoint:
                 host = api_mtls_endpoint
 
                 # Create SSL credentials with client_cert_source or application
                 # default SSL credentials.
                 if client_cert_source:
@@ -228,53 +186,91 @@
                     ("grpc.max_receive_message_length", -1),
                 ],
             )
 
         # Wrap messages. This must be done after self._grpc_channel exists
         self._prep_wrapped_messages(client_info)
 
-    @property
-    def grpc_channel(self) -> aio.Channel:
-        """Create the channel designed to connect to this service.
+    @classmethod
+    def create_channel(
+        cls,
+        host: str = "gkebackup.googleapis.com",
+        credentials: Optional[ga_credentials.Credentials] = None,
+        credentials_file: Optional[str] = None,
+        scopes: Optional[Sequence[str]] = None,
+        quota_project_id: Optional[str] = None,
+        **kwargs,
+    ) -> grpc.Channel:
+        """Create and return a gRPC channel object.
+        Args:
+            host (Optional[str]): The host for the channel to use.
+            credentials (Optional[~.Credentials]): The
+                authorization credentials to attach to requests. These
+                credentials identify this application to the service. If
+                none are specified, the client will attempt to ascertain
+                the credentials from the environment.
+            credentials_file (Optional[str]): A file with credentials that can
+                be loaded with :func:`google.auth.load_credentials_from_file`.
+                This argument is mutually exclusive with credentials.
+            scopes (Optional[Sequence[str]]): A optional list of scopes needed for this
+                service. These are only used when credentials are not specified and
+                are passed to :func:`google.auth.default`.
+            quota_project_id (Optional[str]): An optional project to use for billing
+                and quota.
+            kwargs (Optional[dict]): Keyword arguments, which are passed to the
+                channel creation.
+        Returns:
+            grpc.Channel: A gRPC channel object.
 
-        This property caches on the instance; repeated calls return
-        the same channel.
+        Raises:
+            google.api_core.exceptions.DuplicateCredentialArgs: If both ``credentials``
+              and ``credentials_file`` are passed.
         """
-        # Return the channel from cache.
+
+        return grpc_helpers.create_channel(
+            host,
+            credentials=credentials,
+            credentials_file=credentials_file,
+            quota_project_id=quota_project_id,
+            default_scopes=cls.AUTH_SCOPES,
+            scopes=scopes,
+            default_host=cls.DEFAULT_HOST,
+            **kwargs,
+        )
+
+    @property
+    def grpc_channel(self) -> grpc.Channel:
+        """Return the channel designed to connect to this service."""
         return self._grpc_channel
 
     @property
-    def operations_client(self) -> operations_v1.OperationsAsyncClient:
+    def operations_client(self) -> operations_v1.OperationsClient:
         """Create the client designed to process long-running operations.
 
         This property caches on the instance; repeated calls return the same
         client.
         """
         # Quick check: Only create a new client if we do not already have one.
         if self._operations_client is None:
-            self._operations_client = operations_v1.OperationsAsyncClient(
-                self.grpc_channel
-            )
+            self._operations_client = operations_v1.OperationsClient(self.grpc_channel)
 
         # Return the client from cache.
         return self._operations_client
 
     @property
     def create_backup_plan(
         self,
-    ) -> Callable[
-        [gkebackup.CreateBackupPlanRequest], Awaitable[operations_pb2.Operation]
-    ]:
+    ) -> Callable[[gkebackup.CreateBackupPlanRequest], operations_pb2.Operation]:
         r"""Return a callable for the create backup plan method over gRPC.
 
         Creates a new BackupPlan in a given location.
 
         Returns:
             Callable[[~.CreateBackupPlanRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -286,23 +282,23 @@
             )
         return self._stubs["create_backup_plan"]
 
     @property
     def list_backup_plans(
         self,
     ) -> Callable[
-        [gkebackup.ListBackupPlansRequest], Awaitable[gkebackup.ListBackupPlansResponse]
+        [gkebackup.ListBackupPlansRequest], gkebackup.ListBackupPlansResponse
     ]:
         r"""Return a callable for the list backup plans method over gRPC.
 
         Lists BackupPlans in a given location.
 
         Returns:
             Callable[[~.ListBackupPlansRequest],
-                    Awaitable[~.ListBackupPlansResponse]]:
+                    ~.ListBackupPlansResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -313,22 +309,22 @@
                 response_deserializer=gkebackup.ListBackupPlansResponse.deserialize,
             )
         return self._stubs["list_backup_plans"]
 
     @property
     def get_backup_plan(
         self,
-    ) -> Callable[[gkebackup.GetBackupPlanRequest], Awaitable[backup_plan.BackupPlan]]:
+    ) -> Callable[[gkebackup.GetBackupPlanRequest], backup_plan.BackupPlan]:
         r"""Return a callable for the get backup plan method over gRPC.
 
         Retrieve the details of a single BackupPlan.
 
         Returns:
             Callable[[~.GetBackupPlanRequest],
-                    Awaitable[~.BackupPlan]]:
+                    ~.BackupPlan]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -339,24 +335,22 @@
                 response_deserializer=backup_plan.BackupPlan.deserialize,
             )
         return self._stubs["get_backup_plan"]
 
     @property
     def update_backup_plan(
         self,
-    ) -> Callable[
-        [gkebackup.UpdateBackupPlanRequest], Awaitable[operations_pb2.Operation]
-    ]:
+    ) -> Callable[[gkebackup.UpdateBackupPlanRequest], operations_pb2.Operation]:
         r"""Return a callable for the update backup plan method over gRPC.
 
         Update a BackupPlan.
 
         Returns:
             Callable[[~.UpdateBackupPlanRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -367,24 +361,22 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_backup_plan"]
 
     @property
     def delete_backup_plan(
         self,
-    ) -> Callable[
-        [gkebackup.DeleteBackupPlanRequest], Awaitable[operations_pb2.Operation]
-    ]:
+    ) -> Callable[[gkebackup.DeleteBackupPlanRequest], operations_pb2.Operation]:
         r"""Return a callable for the delete backup plan method over gRPC.
 
         Deletes an existing BackupPlan.
 
         Returns:
             Callable[[~.DeleteBackupPlanRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -395,22 +387,22 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_backup_plan"]
 
     @property
     def create_backup(
         self,
-    ) -> Callable[[gkebackup.CreateBackupRequest], Awaitable[operations_pb2.Operation]]:
+    ) -> Callable[[gkebackup.CreateBackupRequest], operations_pb2.Operation]:
         r"""Return a callable for the create backup method over gRPC.
 
         Creates a Backup for the given BackupPlan.
 
         Returns:
             Callable[[~.CreateBackupRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -421,24 +413,22 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_backup"]
 
     @property
     def list_backups(
         self,
-    ) -> Callable[
-        [gkebackup.ListBackupsRequest], Awaitable[gkebackup.ListBackupsResponse]
-    ]:
+    ) -> Callable[[gkebackup.ListBackupsRequest], gkebackup.ListBackupsResponse]:
         r"""Return a callable for the list backups method over gRPC.
 
         Lists the Backups for a given BackupPlan.
 
         Returns:
             Callable[[~.ListBackupsRequest],
-                    Awaitable[~.ListBackupsResponse]]:
+                    ~.ListBackupsResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -447,24 +437,22 @@
                 "/google.cloud.gkebackup.v1.BackupForGKE/ListBackups",
                 request_serializer=gkebackup.ListBackupsRequest.serialize,
                 response_deserializer=gkebackup.ListBackupsResponse.deserialize,
             )
         return self._stubs["list_backups"]
 
     @property
-    def get_backup(
-        self,
-    ) -> Callable[[gkebackup.GetBackupRequest], Awaitable[backup.Backup]]:
+    def get_backup(self) -> Callable[[gkebackup.GetBackupRequest], backup.Backup]:
         r"""Return a callable for the get backup method over gRPC.
 
         Retrieve the details of a single Backup.
 
         Returns:
             Callable[[~.GetBackupRequest],
-                    Awaitable[~.Backup]]:
+                    ~.Backup]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -475,22 +463,22 @@
                 response_deserializer=backup.Backup.deserialize,
             )
         return self._stubs["get_backup"]
 
     @property
     def update_backup(
         self,
-    ) -> Callable[[gkebackup.UpdateBackupRequest], Awaitable[operations_pb2.Operation]]:
+    ) -> Callable[[gkebackup.UpdateBackupRequest], operations_pb2.Operation]:
         r"""Return a callable for the update backup method over gRPC.
 
         Update a Backup.
 
         Returns:
             Callable[[~.UpdateBackupRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -501,22 +489,22 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_backup"]
 
     @property
     def delete_backup(
         self,
-    ) -> Callable[[gkebackup.DeleteBackupRequest], Awaitable[operations_pb2.Operation]]:
+    ) -> Callable[[gkebackup.DeleteBackupRequest], operations_pb2.Operation]:
         r"""Return a callable for the delete backup method over gRPC.
 
         Deletes an existing Backup.
 
         Returns:
             Callable[[~.DeleteBackupRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -528,24 +516,23 @@
             )
         return self._stubs["delete_backup"]
 
     @property
     def list_volume_backups(
         self,
     ) -> Callable[
-        [gkebackup.ListVolumeBackupsRequest],
-        Awaitable[gkebackup.ListVolumeBackupsResponse],
+        [gkebackup.ListVolumeBackupsRequest], gkebackup.ListVolumeBackupsResponse
     ]:
         r"""Return a callable for the list volume backups method over gRPC.
 
         Lists the VolumeBackups for a given Backup.
 
         Returns:
             Callable[[~.ListVolumeBackupsRequest],
-                    Awaitable[~.ListVolumeBackupsResponse]]:
+                    ~.ListVolumeBackupsResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -556,22 +543,22 @@
                 response_deserializer=gkebackup.ListVolumeBackupsResponse.deserialize,
             )
         return self._stubs["list_volume_backups"]
 
     @property
     def get_volume_backup(
         self,
-    ) -> Callable[[gkebackup.GetVolumeBackupRequest], Awaitable[volume.VolumeBackup]]:
+    ) -> Callable[[gkebackup.GetVolumeBackupRequest], volume.VolumeBackup]:
         r"""Return a callable for the get volume backup method over gRPC.
 
         Retrieve the details of a single VolumeBackup.
 
         Returns:
             Callable[[~.GetVolumeBackupRequest],
-                    Awaitable[~.VolumeBackup]]:
+                    ~.VolumeBackup]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -582,24 +569,22 @@
                 response_deserializer=volume.VolumeBackup.deserialize,
             )
         return self._stubs["get_volume_backup"]
 
     @property
     def create_restore_plan(
         self,
-    ) -> Callable[
-        [gkebackup.CreateRestorePlanRequest], Awaitable[operations_pb2.Operation]
-    ]:
+    ) -> Callable[[gkebackup.CreateRestorePlanRequest], operations_pb2.Operation]:
         r"""Return a callable for the create restore plan method over gRPC.
 
         Creates a new RestorePlan in a given location.
 
         Returns:
             Callable[[~.CreateRestorePlanRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -611,24 +596,23 @@
             )
         return self._stubs["create_restore_plan"]
 
     @property
     def list_restore_plans(
         self,
     ) -> Callable[
-        [gkebackup.ListRestorePlansRequest],
-        Awaitable[gkebackup.ListRestorePlansResponse],
+        [gkebackup.ListRestorePlansRequest], gkebackup.ListRestorePlansResponse
     ]:
         r"""Return a callable for the list restore plans method over gRPC.
 
         Lists RestorePlans in a given location.
 
         Returns:
             Callable[[~.ListRestorePlansRequest],
-                    Awaitable[~.ListRestorePlansResponse]]:
+                    ~.ListRestorePlansResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -639,24 +623,22 @@
                 response_deserializer=gkebackup.ListRestorePlansResponse.deserialize,
             )
         return self._stubs["list_restore_plans"]
 
     @property
     def get_restore_plan(
         self,
-    ) -> Callable[
-        [gkebackup.GetRestorePlanRequest], Awaitable[restore_plan.RestorePlan]
-    ]:
+    ) -> Callable[[gkebackup.GetRestorePlanRequest], restore_plan.RestorePlan]:
         r"""Return a callable for the get restore plan method over gRPC.
 
         Retrieve the details of a single RestorePlan.
 
         Returns:
             Callable[[~.GetRestorePlanRequest],
-                    Awaitable[~.RestorePlan]]:
+                    ~.RestorePlan]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -667,24 +649,22 @@
                 response_deserializer=restore_plan.RestorePlan.deserialize,
             )
         return self._stubs["get_restore_plan"]
 
     @property
     def update_restore_plan(
         self,
-    ) -> Callable[
-        [gkebackup.UpdateRestorePlanRequest], Awaitable[operations_pb2.Operation]
-    ]:
+    ) -> Callable[[gkebackup.UpdateRestorePlanRequest], operations_pb2.Operation]:
         r"""Return a callable for the update restore plan method over gRPC.
 
         Update a RestorePlan.
 
         Returns:
             Callable[[~.UpdateRestorePlanRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -695,24 +675,22 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_restore_plan"]
 
     @property
     def delete_restore_plan(
         self,
-    ) -> Callable[
-        [gkebackup.DeleteRestorePlanRequest], Awaitable[operations_pb2.Operation]
-    ]:
+    ) -> Callable[[gkebackup.DeleteRestorePlanRequest], operations_pb2.Operation]:
         r"""Return a callable for the delete restore plan method over gRPC.
 
         Deletes an existing RestorePlan.
 
         Returns:
             Callable[[~.DeleteRestorePlanRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -723,24 +701,22 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["delete_restore_plan"]
 
     @property
     def create_restore(
         self,
-    ) -> Callable[
-        [gkebackup.CreateRestoreRequest], Awaitable[operations_pb2.Operation]
-    ]:
+    ) -> Callable[[gkebackup.CreateRestoreRequest], operations_pb2.Operation]:
         r"""Return a callable for the create restore method over gRPC.
 
         Creates a new Restore for the given RestorePlan.
 
         Returns:
             Callable[[~.CreateRestoreRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -751,24 +727,22 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["create_restore"]
 
     @property
     def list_restores(
         self,
-    ) -> Callable[
-        [gkebackup.ListRestoresRequest], Awaitable[gkebackup.ListRestoresResponse]
-    ]:
+    ) -> Callable[[gkebackup.ListRestoresRequest], gkebackup.ListRestoresResponse]:
         r"""Return a callable for the list restores method over gRPC.
 
         Lists the Restores for a given RestorePlan.
 
         Returns:
             Callable[[~.ListRestoresRequest],
-                    Awaitable[~.ListRestoresResponse]]:
+                    ~.ListRestoresResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -777,24 +751,22 @@
                 "/google.cloud.gkebackup.v1.BackupForGKE/ListRestores",
                 request_serializer=gkebackup.ListRestoresRequest.serialize,
                 response_deserializer=gkebackup.ListRestoresResponse.deserialize,
             )
         return self._stubs["list_restores"]
 
     @property
-    def get_restore(
-        self,
-    ) -> Callable[[gkebackup.GetRestoreRequest], Awaitable[restore.Restore]]:
+    def get_restore(self) -> Callable[[gkebackup.GetRestoreRequest], restore.Restore]:
         r"""Return a callable for the get restore method over gRPC.
 
         Retrieves the details of a single Restore.
 
         Returns:
             Callable[[~.GetRestoreRequest],
-                    Awaitable[~.Restore]]:
+                    ~.Restore]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -805,24 +777,22 @@
                 response_deserializer=restore.Restore.deserialize,
             )
         return self._stubs["get_restore"]
 
     @property
     def update_restore(
         self,
-    ) -> Callable[
-        [gkebackup.UpdateRestoreRequest], Awaitable[operations_pb2.Operation]
-    ]:
+    ) -> Callable[[gkebackup.UpdateRestoreRequest], operations_pb2.Operation]:
         r"""Return a callable for the update restore method over gRPC.
 
         Update a Restore.
 
         Returns:
             Callable[[~.UpdateRestoreRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -833,24 +803,22 @@
                 response_deserializer=operations_pb2.Operation.FromString,
             )
         return self._stubs["update_restore"]
 
     @property
     def delete_restore(
         self,
-    ) -> Callable[
-        [gkebackup.DeleteRestoreRequest], Awaitable[operations_pb2.Operation]
-    ]:
+    ) -> Callable[[gkebackup.DeleteRestoreRequest], operations_pb2.Operation]:
         r"""Return a callable for the delete restore method over gRPC.
 
         Deletes an existing Restore.
 
         Returns:
             Callable[[~.DeleteRestoreRequest],
-                    Awaitable[~.Operation]]:
+                    ~.Operation]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -862,24 +830,23 @@
             )
         return self._stubs["delete_restore"]
 
     @property
     def list_volume_restores(
         self,
     ) -> Callable[
-        [gkebackup.ListVolumeRestoresRequest],
-        Awaitable[gkebackup.ListVolumeRestoresResponse],
+        [gkebackup.ListVolumeRestoresRequest], gkebackup.ListVolumeRestoresResponse
     ]:
         r"""Return a callable for the list volume restores method over gRPC.
 
         Lists the VolumeRestores for a given Restore.
 
         Returns:
             Callable[[~.ListVolumeRestoresRequest],
-                    Awaitable[~.ListVolumeRestoresResponse]]:
+                    ~.ListVolumeRestoresResponse]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -890,22 +857,22 @@
                 response_deserializer=gkebackup.ListVolumeRestoresResponse.deserialize,
             )
         return self._stubs["list_volume_restores"]
 
     @property
     def get_volume_restore(
         self,
-    ) -> Callable[[gkebackup.GetVolumeRestoreRequest], Awaitable[volume.VolumeRestore]]:
+    ) -> Callable[[gkebackup.GetVolumeRestoreRequest], volume.VolumeRestore]:
         r"""Return a callable for the get volume restore method over gRPC.
 
         Retrieve the details of a single VolumeRestore.
 
         Returns:
             Callable[[~.GetVolumeRestoreRequest],
-                    Awaitable[~.VolumeRestore]]:
+                    ~.VolumeRestore]:
                 A function that, when called, will call the underlying RPC
                 on the server.
         """
         # Generate a "stub function" on-the-fly which will actually make
         # the request.
         # gRPC handles serialization and deserialization, so we just need
         # to pass in the functions for each.
@@ -914,11 +881,201 @@
                 "/google.cloud.gkebackup.v1.BackupForGKE/GetVolumeRestore",
                 request_serializer=gkebackup.GetVolumeRestoreRequest.serialize,
                 response_deserializer=volume.VolumeRestore.deserialize,
             )
         return self._stubs["get_volume_restore"]
 
     def close(self):
-        return self.grpc_channel.close()
+        self.grpc_channel.close()
+
+    @property
+    def delete_operation(
+        self,
+    ) -> Callable[[operations_pb2.DeleteOperationRequest], None]:
+        r"""Return a callable for the delete_operation method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "delete_operation" not in self._stubs:
+            self._stubs["delete_operation"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/DeleteOperation",
+                request_serializer=operations_pb2.DeleteOperationRequest.SerializeToString,
+                response_deserializer=None,
+            )
+        return self._stubs["delete_operation"]
+
+    @property
+    def cancel_operation(
+        self,
+    ) -> Callable[[operations_pb2.CancelOperationRequest], None]:
+        r"""Return a callable for the cancel_operation method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "cancel_operation" not in self._stubs:
+            self._stubs["cancel_operation"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/CancelOperation",
+                request_serializer=operations_pb2.CancelOperationRequest.SerializeToString,
+                response_deserializer=None,
+            )
+        return self._stubs["cancel_operation"]
+
+    @property
+    def get_operation(
+        self,
+    ) -> Callable[[operations_pb2.GetOperationRequest], operations_pb2.Operation]:
+        r"""Return a callable for the get_operation method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_operation" not in self._stubs:
+            self._stubs["get_operation"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/GetOperation",
+                request_serializer=operations_pb2.GetOperationRequest.SerializeToString,
+                response_deserializer=operations_pb2.Operation.FromString,
+            )
+        return self._stubs["get_operation"]
+
+    @property
+    def list_operations(
+        self,
+    ) -> Callable[
+        [operations_pb2.ListOperationsRequest], operations_pb2.ListOperationsResponse
+    ]:
+        r"""Return a callable for the list_operations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_operations" not in self._stubs:
+            self._stubs["list_operations"] = self.grpc_channel.unary_unary(
+                "/google.longrunning.Operations/ListOperations",
+                request_serializer=operations_pb2.ListOperationsRequest.SerializeToString,
+                response_deserializer=operations_pb2.ListOperationsResponse.FromString,
+            )
+        return self._stubs["list_operations"]
+
+    @property
+    def list_locations(
+        self,
+    ) -> Callable[
+        [locations_pb2.ListLocationsRequest], locations_pb2.ListLocationsResponse
+    ]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "list_locations" not in self._stubs:
+            self._stubs["list_locations"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/ListLocations",
+                request_serializer=locations_pb2.ListLocationsRequest.SerializeToString,
+                response_deserializer=locations_pb2.ListLocationsResponse.FromString,
+            )
+        return self._stubs["list_locations"]
+
+    @property
+    def get_location(
+        self,
+    ) -> Callable[[locations_pb2.GetLocationRequest], locations_pb2.Location]:
+        r"""Return a callable for the list locations method over gRPC."""
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_location" not in self._stubs:
+            self._stubs["get_location"] = self.grpc_channel.unary_unary(
+                "/google.cloud.location.Locations/GetLocation",
+                request_serializer=locations_pb2.GetLocationRequest.SerializeToString,
+                response_deserializer=locations_pb2.Location.FromString,
+            )
+        return self._stubs["get_location"]
+
+    @property
+    def set_iam_policy(
+        self,
+    ) -> Callable[[iam_policy_pb2.SetIamPolicyRequest], policy_pb2.Policy]:
+        r"""Return a callable for the set iam policy method over gRPC.
+        Sets the IAM access control policy on the specified
+        function. Replaces any existing policy.
+        Returns:
+            Callable[[~.SetIamPolicyRequest],
+                    ~.Policy]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "set_iam_policy" not in self._stubs:
+            self._stubs["set_iam_policy"] = self.grpc_channel.unary_unary(
+                "/google.iam.v1.IAMPolicy/SetIamPolicy",
+                request_serializer=iam_policy_pb2.SetIamPolicyRequest.SerializeToString,
+                response_deserializer=policy_pb2.Policy.FromString,
+            )
+        return self._stubs["set_iam_policy"]
+
+    @property
+    def get_iam_policy(
+        self,
+    ) -> Callable[[iam_policy_pb2.GetIamPolicyRequest], policy_pb2.Policy]:
+        r"""Return a callable for the get iam policy method over gRPC.
+        Gets the IAM access control policy for a function.
+        Returns an empty policy if the function exists and does
+        not have a policy set.
+        Returns:
+            Callable[[~.GetIamPolicyRequest],
+                    ~.Policy]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "get_iam_policy" not in self._stubs:
+            self._stubs["get_iam_policy"] = self.grpc_channel.unary_unary(
+                "/google.iam.v1.IAMPolicy/GetIamPolicy",
+                request_serializer=iam_policy_pb2.GetIamPolicyRequest.SerializeToString,
+                response_deserializer=policy_pb2.Policy.FromString,
+            )
+        return self._stubs["get_iam_policy"]
+
+    @property
+    def test_iam_permissions(
+        self,
+    ) -> Callable[
+        [iam_policy_pb2.TestIamPermissionsRequest],
+        iam_policy_pb2.TestIamPermissionsResponse,
+    ]:
+        r"""Return a callable for the test iam permissions method over gRPC.
+        Tests the specified permissions against the IAM access control
+        policy for a function. If the function does not exist, this will
+        return an empty set of permissions, not a NOT_FOUND error.
+        Returns:
+            Callable[[~.TestIamPermissionsRequest],
+                    ~.TestIamPermissionsResponse]:
+                A function that, when called, will call the underlying RPC
+                on the server.
+        """
+        # Generate a "stub function" on-the-fly which will actually make
+        # the request.
+        # gRPC handles serialization and deserialization, so we just need
+        # to pass in the functions for each.
+        if "test_iam_permissions" not in self._stubs:
+            self._stubs["test_iam_permissions"] = self.grpc_channel.unary_unary(
+                "/google.iam.v1.IAMPolicy/TestIamPermissions",
+                request_serializer=iam_policy_pb2.TestIamPermissionsRequest.SerializeToString,
+                response_deserializer=iam_policy_pb2.TestIamPermissionsResponse.FromString,
+            )
+        return self._stubs["test_iam_permissions"]
+
+    @property
+    def kind(self) -> str:
+        return "grpc"
 
 
-__all__ = ("BackupForGKEGrpcAsyncIOTransport",)
+__all__ = ("BackupForGKEGrpcTransport",)
```

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/services/backup_for_gke/transports/rest.py`

 * *Files 9% similar despite different names*

```diff
@@ -28,14 +28,18 @@
     rest_streaming,
 )
 from google.api_core import exceptions as core_exceptions
 from google.api_core import retry as retries
 from google.auth import credentials as ga_credentials  # type: ignore
 from google.auth.transport.grpc import SslCredentials  # type: ignore
 from google.auth.transport.requests import AuthorizedSession  # type: ignore
+from google.cloud.location import locations_pb2  # type: ignore
+from google.iam.v1 import iam_policy_pb2  # type: ignore
+from google.iam.v1 import policy_pb2  # type: ignore
+from google.longrunning import operations_pb2
 from google.protobuf import json_format
 import grpc  # type: ignore
 from requests import __version__ as requests_version
 
 try:
     OptionalRetry = Union[retries.Retry, gapic_v1.method._MethodDefault]
 except AttributeError:  # pragma: NO COVER
@@ -814,14 +818,213 @@
 
         Override in a subclass to manipulate the response
         after it is returned by the BackupForGKE server but before
         it is returned to user code.
         """
         return response
 
+    def pre_get_location(
+        self,
+        request: locations_pb2.GetLocationRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[locations_pb2.GetLocationRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for get_location
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the BackupForGKE server.
+        """
+        return request, metadata
+
+    def post_get_location(
+        self, response: locations_pb2.Location
+    ) -> locations_pb2.Location:
+        """Post-rpc interceptor for get_location
+
+        Override in a subclass to manipulate the response
+        after it is returned by the BackupForGKE server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_list_locations(
+        self,
+        request: locations_pb2.ListLocationsRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[locations_pb2.ListLocationsRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for list_locations
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the BackupForGKE server.
+        """
+        return request, metadata
+
+    def post_list_locations(
+        self, response: locations_pb2.ListLocationsResponse
+    ) -> locations_pb2.ListLocationsResponse:
+        """Post-rpc interceptor for list_locations
+
+        Override in a subclass to manipulate the response
+        after it is returned by the BackupForGKE server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_get_iam_policy(
+        self,
+        request: iam_policy_pb2.GetIamPolicyRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[iam_policy_pb2.GetIamPolicyRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for get_iam_policy
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the BackupForGKE server.
+        """
+        return request, metadata
+
+    def post_get_iam_policy(self, response: policy_pb2.Policy) -> policy_pb2.Policy:
+        """Post-rpc interceptor for get_iam_policy
+
+        Override in a subclass to manipulate the response
+        after it is returned by the BackupForGKE server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_set_iam_policy(
+        self,
+        request: iam_policy_pb2.SetIamPolicyRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[iam_policy_pb2.SetIamPolicyRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for set_iam_policy
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the BackupForGKE server.
+        """
+        return request, metadata
+
+    def post_set_iam_policy(self, response: policy_pb2.Policy) -> policy_pb2.Policy:
+        """Post-rpc interceptor for set_iam_policy
+
+        Override in a subclass to manipulate the response
+        after it is returned by the BackupForGKE server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_test_iam_permissions(
+        self,
+        request: iam_policy_pb2.TestIamPermissionsRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[iam_policy_pb2.TestIamPermissionsRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for test_iam_permissions
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the BackupForGKE server.
+        """
+        return request, metadata
+
+    def post_test_iam_permissions(
+        self, response: iam_policy_pb2.TestIamPermissionsResponse
+    ) -> iam_policy_pb2.TestIamPermissionsResponse:
+        """Post-rpc interceptor for test_iam_permissions
+
+        Override in a subclass to manipulate the response
+        after it is returned by the BackupForGKE server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_cancel_operation(
+        self,
+        request: operations_pb2.CancelOperationRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[operations_pb2.CancelOperationRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for cancel_operation
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the BackupForGKE server.
+        """
+        return request, metadata
+
+    def post_cancel_operation(self, response: None) -> None:
+        """Post-rpc interceptor for cancel_operation
+
+        Override in a subclass to manipulate the response
+        after it is returned by the BackupForGKE server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_delete_operation(
+        self,
+        request: operations_pb2.DeleteOperationRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[operations_pb2.DeleteOperationRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for delete_operation
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the BackupForGKE server.
+        """
+        return request, metadata
+
+    def post_delete_operation(self, response: None) -> None:
+        """Post-rpc interceptor for delete_operation
+
+        Override in a subclass to manipulate the response
+        after it is returned by the BackupForGKE server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_get_operation(
+        self,
+        request: operations_pb2.GetOperationRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[operations_pb2.GetOperationRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for get_operation
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the BackupForGKE server.
+        """
+        return request, metadata
+
+    def post_get_operation(
+        self, response: operations_pb2.Operation
+    ) -> operations_pb2.Operation:
+        """Post-rpc interceptor for get_operation
+
+        Override in a subclass to manipulate the response
+        after it is returned by the BackupForGKE server but before
+        it is returned to user code.
+        """
+        return response
+
+    def pre_list_operations(
+        self,
+        request: operations_pb2.ListOperationsRequest,
+        metadata: Sequence[Tuple[str, str]],
+    ) -> Tuple[operations_pb2.ListOperationsRequest, Sequence[Tuple[str, str]]]:
+        """Pre-rpc interceptor for list_operations
+
+        Override in a subclass to manipulate the request or metadata
+        before they are sent to the BackupForGKE server.
+        """
+        return request, metadata
+
+    def post_list_operations(
+        self, response: operations_pb2.ListOperationsResponse
+    ) -> operations_pb2.ListOperationsResponse:
+        """Post-rpc interceptor for list_operations
+
+        Override in a subclass to manipulate the response
+        after it is returned by the BackupForGKE server but before
+        it is returned to user code.
+        """
+        return response
+
 
 @dataclasses.dataclass
 class BackupForGKERestStub:
     _session: AuthorizedSession
     _host: str
     _interceptor: BackupForGKERestInterceptor
 
@@ -3382,14 +3585,690 @@
         self,
     ) -> Callable[[gkebackup.UpdateRestorePlanRequest], operations_pb2.Operation]:
         # The return type is fine, but mypy isn't sophisticated enough to determine what's going on here.
         # In C++ this would require a dynamic_cast
         return self._UpdateRestorePlan(self._session, self._host, self._interceptor)  # type: ignore
 
     @property
+    def get_location(self):
+        return self._GetLocation(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _GetLocation(BackupForGKERestStub):
+        def __call__(
+            self,
+            request: locations_pb2.GetLocationRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> locations_pb2.Location:
+
+            r"""Call the get location method over HTTP.
+
+            Args:
+                request (locations_pb2.GetLocationRequest):
+                    The request object for GetLocation method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                locations_pb2.Location: Response from GetLocation method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{name=projects/*/locations/*}",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_get_location(request, metadata)
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = locations_pb2.Location()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_get_location(resp)
+            return resp
+
+    @property
+    def list_locations(self):
+        return self._ListLocations(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _ListLocations(BackupForGKERestStub):
+        def __call__(
+            self,
+            request: locations_pb2.ListLocationsRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> locations_pb2.ListLocationsResponse:
+
+            r"""Call the list locations method over HTTP.
+
+            Args:
+                request (locations_pb2.ListLocationsRequest):
+                    The request object for ListLocations method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                locations_pb2.ListLocationsResponse: Response from ListLocations method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{name=projects/*}/locations",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_list_locations(request, metadata)
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = locations_pb2.ListLocationsResponse()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_list_locations(resp)
+            return resp
+
+    @property
+    def get_iam_policy(self):
+        return self._GetIamPolicy(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _GetIamPolicy(BackupForGKERestStub):
+        def __call__(
+            self,
+            request: iam_policy_pb2.GetIamPolicyRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> policy_pb2.Policy:
+
+            r"""Call the get iam policy method over HTTP.
+
+            Args:
+                request (iam_policy_pb2.GetIamPolicyRequest):
+                    The request object for GetIamPolicy method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                policy_pb2.Policy: Response from GetIamPolicy method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{resource=projects/*/locations/*/backupPlans/*}:getIamPolicy",
+                },
+                {
+                    "method": "get",
+                    "uri": "/v1/{resource=projects/*/locations/*/backupPlans/*/backups/*}:getIamPolicy",
+                },
+                {
+                    "method": "get",
+                    "uri": "/v1/{resource=projects/*/locations/*/backupPlans/*/backups/*/volumeBackups/*}:getIamPolicy",
+                },
+                {
+                    "method": "get",
+                    "uri": "/v1/{resource=projects/*/locations/*/restorePlans/*}:getIamPolicy",
+                },
+                {
+                    "method": "get",
+                    "uri": "/v1/{resource=projects/*/locations/*/restorePlans/*/restores/*}:getIamPolicy",
+                },
+                {
+                    "method": "get",
+                    "uri": "/v1/{resource=projects/*/locations/*/restorePlans/*/restores/*/volumeRestores/*}:getIamPolicy",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_get_iam_policy(request, metadata)
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = policy_pb2.Policy()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_get_iam_policy(resp)
+            return resp
+
+    @property
+    def set_iam_policy(self):
+        return self._SetIamPolicy(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _SetIamPolicy(BackupForGKERestStub):
+        def __call__(
+            self,
+            request: iam_policy_pb2.SetIamPolicyRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> policy_pb2.Policy:
+
+            r"""Call the set iam policy method over HTTP.
+
+            Args:
+                request (iam_policy_pb2.SetIamPolicyRequest):
+                    The request object for SetIamPolicy method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                policy_pb2.Policy: Response from SetIamPolicy method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1/{resource=projects/*/locations/*/backupPlans/*}:setIamPolicy",
+                    "body": "*",
+                },
+                {
+                    "method": "post",
+                    "uri": "/v1/{resource=projects/*/locations/*/backupPlans/*/backups/*}:setIamPolicy",
+                    "body": "*",
+                },
+                {
+                    "method": "post",
+                    "uri": "/v1/{resource=projects/*/locations/*/backupPlans/*/backups/*/volumeBackups/*}:setIamPolicy",
+                    "body": "*",
+                },
+                {
+                    "method": "post",
+                    "uri": "/v1/{resource=projects/*/locations/*/restorePlans/*}:setIamPolicy",
+                    "body": "*",
+                },
+                {
+                    "method": "post",
+                    "uri": "/v1/{resource=projects/*/locations/*/restorePlans/*/restores/*}:setIamPolicy",
+                    "body": "*",
+                },
+                {
+                    "method": "post",
+                    "uri": "/v1/{resource=projects/*/locations/*/restorePlans/*/restores/*/volumeRestores/*}:setIamPolicy",
+                    "body": "*",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_set_iam_policy(request, metadata)
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            body = json.loads(json.dumps(transcoded_request["body"]))
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = policy_pb2.Policy()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_set_iam_policy(resp)
+            return resp
+
+    @property
+    def test_iam_permissions(self):
+        return self._TestIamPermissions(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _TestIamPermissions(BackupForGKERestStub):
+        def __call__(
+            self,
+            request: iam_policy_pb2.TestIamPermissionsRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> iam_policy_pb2.TestIamPermissionsResponse:
+
+            r"""Call the test iam permissions method over HTTP.
+
+            Args:
+                request (iam_policy_pb2.TestIamPermissionsRequest):
+                    The request object for TestIamPermissions method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                iam_policy_pb2.TestIamPermissionsResponse: Response from TestIamPermissions method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1/{resource=projects/*/locations/*/backupPlans/*}:testIamPermissions",
+                    "body": "*",
+                },
+                {
+                    "method": "post",
+                    "uri": "/v1/{resource=projects/*/locations/*/backupPlans/*/backups/*}:testIamPermissions",
+                    "body": "*",
+                },
+                {
+                    "method": "post",
+                    "uri": "/v1/{resource=projects/*/locations/*/backupPlans/*/backups/*/volumeBackups/*}:testIamPermissions",
+                    "body": "*",
+                },
+                {
+                    "method": "post",
+                    "uri": "/v1/{resource=projects/*/locations/*/restorePlans/*}:testIamPermissions",
+                    "body": "*",
+                },
+                {
+                    "method": "post",
+                    "uri": "/v1/{resource=projects/*/locations/*/restorePlans/*/restores/*}:testIamPermissions",
+                    "body": "*",
+                },
+                {
+                    "method": "post",
+                    "uri": "/v1/{resource=projects/*/locations/*/restorePlans/*/restores/*/volumeRestores/*}:testIamPermissions",
+                    "body": "*",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_test_iam_permissions(
+                request, metadata
+            )
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            body = json.loads(json.dumps(transcoded_request["body"]))
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = iam_policy_pb2.TestIamPermissionsResponse()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_test_iam_permissions(resp)
+            return resp
+
+    @property
+    def cancel_operation(self):
+        return self._CancelOperation(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _CancelOperation(BackupForGKERestStub):
+        def __call__(
+            self,
+            request: operations_pb2.CancelOperationRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> None:
+
+            r"""Call the cancel operation method over HTTP.
+
+            Args:
+                request (operations_pb2.CancelOperationRequest):
+                    The request object for CancelOperation method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "post",
+                    "uri": "/v1/{name=projects/*/locations/*/operations/*}:cancel",
+                    "body": "*",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_cancel_operation(
+                request, metadata
+            )
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            body = json.loads(json.dumps(transcoded_request["body"]))
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+                data=body,
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            return self._interceptor.post_cancel_operation(None)
+
+    @property
+    def delete_operation(self):
+        return self._DeleteOperation(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _DeleteOperation(BackupForGKERestStub):
+        def __call__(
+            self,
+            request: operations_pb2.DeleteOperationRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> None:
+
+            r"""Call the delete operation method over HTTP.
+
+            Args:
+                request (operations_pb2.DeleteOperationRequest):
+                    The request object for DeleteOperation method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "delete",
+                    "uri": "/v1/{name=projects/*/locations/*}/operations",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_delete_operation(
+                request, metadata
+            )
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            return self._interceptor.post_delete_operation(None)
+
+    @property
+    def get_operation(self):
+        return self._GetOperation(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _GetOperation(BackupForGKERestStub):
+        def __call__(
+            self,
+            request: operations_pb2.GetOperationRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> operations_pb2.Operation:
+
+            r"""Call the get operation method over HTTP.
+
+            Args:
+                request (operations_pb2.GetOperationRequest):
+                    The request object for GetOperation method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                operations_pb2.Operation: Response from GetOperation method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{name=projects/*/locations/*/operations/*}",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_get_operation(request, metadata)
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = operations_pb2.Operation()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_get_operation(resp)
+            return resp
+
+    @property
+    def list_operations(self):
+        return self._ListOperations(self._session, self._host, self._interceptor)  # type: ignore
+
+    class _ListOperations(BackupForGKERestStub):
+        def __call__(
+            self,
+            request: operations_pb2.ListOperationsRequest,
+            *,
+            retry: OptionalRetry = gapic_v1.method.DEFAULT,
+            timeout: Optional[float] = None,
+            metadata: Sequence[Tuple[str, str]] = (),
+        ) -> operations_pb2.ListOperationsResponse:
+
+            r"""Call the list operations method over HTTP.
+
+            Args:
+                request (operations_pb2.ListOperationsRequest):
+                    The request object for ListOperations method.
+                retry (google.api_core.retry.Retry): Designation of what errors, if any,
+                    should be retried.
+                timeout (float): The timeout for this request.
+                metadata (Sequence[Tuple[str, str]]): Strings which should be
+                    sent along with the request as metadata.
+
+            Returns:
+                operations_pb2.ListOperationsResponse: Response from ListOperations method.
+            """
+
+            http_options: List[Dict[str, str]] = [
+                {
+                    "method": "get",
+                    "uri": "/v1/{name=projects/*/locations/*}/operations",
+                },
+            ]
+
+            request, metadata = self._interceptor.pre_list_operations(request, metadata)
+            request_kwargs = json_format.MessageToDict(request)
+            transcoded_request = path_template.transcode(http_options, **request_kwargs)
+
+            uri = transcoded_request["uri"]
+            method = transcoded_request["method"]
+
+            # Jsonify the query params
+            query_params = json.loads(json.dumps(transcoded_request["query_params"]))
+
+            # Send the request
+            headers = dict(metadata)
+            headers["Content-Type"] = "application/json"
+
+            response = getattr(self._session, method)(
+                "{host}{uri}".format(host=self._host, uri=uri),
+                timeout=timeout,
+                headers=headers,
+                params=rest_helpers.flatten_query_params(query_params),
+            )
+
+            # In case of error, raise the appropriate core_exceptions.GoogleAPICallError exception
+            # subclass.
+            if response.status_code >= 400:
+                raise core_exceptions.from_http_response(response)
+
+            resp = operations_pb2.ListOperationsResponse()
+            resp = json_format.Parse(response.content.decode("utf-8"), resp)
+            resp = self._interceptor.post_list_operations(resp)
+            return resp
+
+    @property
     def kind(self) -> str:
         return "rest"
 
     def close(self):
         self._session.close()
```

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/__init__.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/backup.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/backup.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,16 @@
             [delete_lock_days][google.cloud.gkebackup.v1.Backup.delete_lock_days]).
         retain_days (int):
             The age (in days) after which this Backup will be
             automatically deleted. Must be an integer value >= 0:
 
             -  If 0, no automatic deletion will occur for this Backup.
             -  If not 0, this must be >=
-               [delete_lock_days][google.cloud.gkebackup.v1.Backup.delete_lock_days].
+               [delete_lock_days][google.cloud.gkebackup.v1.Backup.delete_lock_days]
+               and <= 365.
 
             Once a Backup is created, this value may only be increased.
 
             Defaults to the parent BackupPlan's
             [backup_retain_days][google.cloud.gkebackup.v1.BackupPlan.RetentionPolicy.backup_retain_days]
             value.
         retain_expire_time (google.protobuf.timestamp_pb2.Timestamp):
```

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/backup_plan.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/backup_plan.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,24 +109,28 @@
                 BackupPlan does NOT affect existing Backups under it.
                 Backups created AFTER a successful update will inherit the
                 new value.
 
                 Default: 0 (no delete blocking)
             backup_retain_days (int):
                 The default maximum age of a Backup created via this
-                BackupPlan. This field MUST be an integer value >= 0. If
-                specified, a Backup created under this BackupPlan will be
-                automatically deleted after its age reaches (create_time +
-                backup_retain_days). If not specified, Backups created under
-                this BackupPlan will NOT be subject to automatic deletion.
-                Updating this field does NOT affect existing Backups under
-                it. Backups created AFTER a successful update will
-                automatically pick up the new value. NOTE:
-                backup_retain_days must be >=
+                BackupPlan. This field MUST be an integer value >= 0 and <=
+                365. If specified, a Backup created under this BackupPlan
+                will be automatically deleted after its age reaches
+                (create_time + backup_retain_days). If not specified,
+                Backups created under this BackupPlan will NOT be subject to
+                automatic deletion. Updating this field does NOT affect
+                existing Backups under it. Backups created AFTER a
+                successful update will automatically pick up the new value.
+                NOTE: backup_retain_days must be >=
                 [backup_delete_lock_days][google.cloud.gkebackup.v1.BackupPlan.RetentionPolicy.backup_delete_lock_days].
+                If
+                [cron_schedule][google.cloud.gkebackup.v1.BackupPlan.Schedule.cron_schedule]
+                is defined, then this must be <= 360 \* the creation
+                interval.
 
                 Default: 0 (no automatic deletion)
             locked (bool):
                 This flag denotes whether the retention policy of this
                 BackupPlan is locked. If set to True, no further update is
                 allowed on this policy, including the ``locked`` field
                 itself.
@@ -151,15 +155,17 @@
         r"""Schedule defines scheduling parameters for automatically
         creating Backups via this BackupPlan.
 
         Attributes:
             cron_schedule (str):
                 A standard `cron <https://wikipedia.com/wiki/cron>`__ string
                 that defines a repeating schedule for creating Backups via
-                this BackupPlan.
+                this BackupPlan. If this is defined, then
+                [backup_retain_days][google.cloud.gkebackup.v1.BackupPlan.RetentionPolicy.backup_retain_days]
+                must also be defined.
 
                 Default (empty): no automatic backup creation will occur.
             paused (bool):
                 This flag denotes whether automatic Backup
                 creation is paused for this BackupPlan.
 
                 Default: False
```

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/common.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/common.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/gkebackup.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/gkebackup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/restore.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/restore.py`

 * *Files 5% similar despite different names*

```diff
@@ -275,38 +275,36 @@
             are executed in order defined - this order
             matters, as changes made by a rule may impact
             the filtering logic of subsequent rules. An
             empty list means no substitution will occur.
     """
 
     class VolumeDataRestorePolicy(proto.Enum):
-        r"""Defines how volume data should be restored
+        r"""Defines how volume data should be restored.
 
         Values:
             VOLUME_DATA_RESTORE_POLICY_UNSPECIFIED (0):
                 Unspecified (illegal).
             RESTORE_VOLUME_DATA_FROM_BACKUP (1):
-                For each PVC to be restored, will create a
-                new underlying volume (and PV) from the
-                corresponding VolumeBackup contained within the
-                Backup.
+                For each PVC to be restored, create a new
+                underlying volume and PV from the corresponding
+                VolumeBackup contained within the Backup.
             REUSE_VOLUME_HANDLE_FROM_BACKUP (2):
                 For each PVC to be restored, attempt to reuse
                 the original PV contained in the Backup (with
-                its original underlying volume).  Note that
-                option is likely only usable when restoring a
-                workload to its original cluster.
+                its original underlying volume). This option is
+                likely only usable when restoring a workload to
+                its original cluster.
             NO_VOLUME_DATA_RESTORATION (3):
-                For each PVC to be restored, PVCs will be
-                created without any particular action to restore
-                data.  In this case, the normal Kubernetes
-                provisioning logic would kick in, and this would
-                likely result in either dynamically provisioning
-                blank PVs or binding to statically provisioned
-                PVs.
+                For each PVC to be restored, create PVC
+                without any particular action to restore data.
+                In this case, the normal Kubernetes provisioning
+                logic would kick in, and this would likely
+                result in either dynamically provisioning blank
+                PVs or binding to statically provisioned PVs.
         """
         VOLUME_DATA_RESTORE_POLICY_UNSPECIFIED = 0
         RESTORE_VOLUME_DATA_FROM_BACKUP = 1
         REUSE_VOLUME_HANDLE_FROM_BACKUP = 2
         NO_VOLUME_DATA_RESTORATION = 3
 
     class ClusterResourceConflictPolicy(proto.Enum):
@@ -319,19 +317,19 @@
                 Unspecified. Only allowed if no
                 cluster-scoped resources will be restored.
             USE_EXISTING_VERSION (1):
                 Do not attempt to restore the conflicting
                 resource.
             USE_BACKUP_VERSION (2):
                 Delete the existing version before
-                re-creating it from the Backup. Note that this
-                is a dangerous option which could cause
-                unintentional data loss if used inappropriately
-                - for example, deleting a CRD will cause
-                Kubernetes to delete all CRs of that type.
+                re-creating it from the Backup. This is a
+                dangerous option which could cause unintentional
+                data loss if used inappropriately. For example,
+                deleting a CRD will cause Kubernetes to delete
+                all CRs of that type.
         """
         CLUSTER_RESOURCE_CONFLICT_POLICY_UNSPECIFIED = 0
         USE_EXISTING_VERSION = 1
         USE_BACKUP_VERSION = 2
 
     class NamespacedResourceRestoreMode(proto.Enum):
         r"""Defines the behavior for handling the situation where sets of
@@ -389,25 +387,39 @@
         )
         resource_kind: str = proto.Field(
             proto.STRING,
             number=2,
         )
 
     class ClusterResourceRestoreScope(proto.Message):
-        r"""Identifies the cluster-scoped resources to restore from the
-        Backup.
+        r"""Defines the scope of cluster-scoped resources to restore.
+        Some group kinds are not reasonable choices for a restore, and
+        will cause an error if selected here. Any scope selection that
+        would restore "all valid" resources automatically excludes these
+        group kinds. - gkebackup.gke.io/BackupJob
+        - gkebackup.gke.io/RestoreJob
+        - metrics.k8s.io/NodeMetrics
+        - migration.k8s.io/StorageState
+        - migration.k8s.io/StorageVersionMigration
+        - Node
+        - snapshot.storage.k8s.io/VolumeSnapshotContent
+        - storage.k8s.io/CSINode
+
+        Some group kinds are driven by restore configuration elsewhere,
+        and will cause an error if selected here.
+        - Namespace
+        - PersistentVolume
 
         Attributes:
             selected_group_kinds (MutableSequence[google.cloud.gke_backup_v1.types.RestoreConfig.GroupKind]):
-                A list of "types" of cluster-scoped resources
-                to be restored from the Backup.  An empty list
-                means that NO cluster-scoped resources will be
-                restored. Note that Namespaces and
-                PersistentVolume restoration is handled
-                separately and is not governed by this field.
+                A list of cluster-scoped resource group kinds
+                to restore from the backup. If specified, only
+                the selected resources will be restored.
+                Mutually exclusive to any other field in the
+                message.
         """
 
         selected_group_kinds: MutableSequence[
             "RestoreConfig.GroupKind"
         ] = proto.RepeatedField(
             proto.MESSAGE,
             number=1,
@@ -453,15 +465,15 @@
                 (https://en.wikipedia.org/wiki/Regular_expression) that is
                 compared against the fields matched by the target_json_path
                 expression (and must also have passed the previous filters).
                 Substitution will not be performed against fields whose
                 value does not match this expression. If this field is NOT
                 specified, then ALL fields matched by the target_json_path
                 expression will undergo substitution. Note that an empty
-                (e.g., "", rather than unspecified) value for for this field
+                (e.g., "", rather than unspecified) value for this field
                 will only match empty fields.
             new_value (str):
                 This is the new value to set for any fields
                 that pass the filtering and selection criteria.
                 To remove a value from a Kubernetes resource,
                 either leave this field unspecified, or set it
                 to the empty string ("").
```

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/restore_plan.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/restore_plan.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/google/cloud/gke_backup_v1/types/volume.py` & `google-cloud-gke-backup-0.4.4/google/cloud/gke_backup_v1/types/volume.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
     r"""Represents the operation of restoring a volume from a
     VolumeBackup. Next id: 13
 
     Attributes:
         name (str):
             Output only. Full name of the VolumeRestore resource.
             Format:
-            ``projects/*/locations/*/restorePlans/*/restores/*/volumeRestores/*``.
+            ``projects/*/locations/*/restorePlans/*/restores/*/volumeRestores/*``
         uid (str):
             Output only. Server generated global unique identifier of
             `UUID <https://en.wikipedia.org/wiki/Universally_unique_identifier>`__
             format.
         create_time (google.protobuf.timestamp_pb2.Timestamp):
             Output only. The timestamp when this
             VolumeRestore resource was created.
```

### Comparing `google-cloud-gke-backup-0.4.3/google_cloud_gke_backup.egg-info/PKG-INFO` & `google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-gke-backup
-Version: 0.4.3
+Version: 0.4.4
 Summary: Google Cloud Gke Backup API client library
 Home-page: https://github.com/googleapis/python-gke-backup
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-gke-backup-0.4.3/google_cloud_gke_backup.egg-info/SOURCES.txt` & `google-cloud-gke-backup-0.4.4/google_cloud_gke_backup.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/setup.py` & `google-cloud-gke-backup-0.4.4/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,15 @@
     release_status = "Development Status :: 5 - Production/Stable"
 
 dependencies = [
     "google-api-core[grpc] >= 1.34.0, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.*,!=2.4.*,!=2.5.*,!=2.6.*,!=2.7.*,!=2.8.*,!=2.9.*,!=2.10.*",
     "proto-plus >= 1.22.0, <2.0.0dev",
     "proto-plus >= 1.22.2, <2.0.0dev; python_version>='3.11'",
     "protobuf>=3.19.5,<5.0.0dev,!=3.20.0,!=3.20.1,!=4.21.0,!=4.21.1,!=4.21.2,!=4.21.3,!=4.21.4,!=4.21.5",
+    "grpc-google-iam-v1 >= 0.12.4, <1.0.0dev",
 ]
 url = "https://github.com/googleapis/python-gke-backup"
 
 package_root = os.path.abspath(os.path.dirname(__file__))
 
 readme_filename = os.path.join(package_root, "README.rst")
 with io.open(readme_filename, encoding="utf-8") as readme_file:
```

### Comparing `google-cloud-gke-backup-0.4.3/tests/__init__.py` & `google-cloud-gke-backup-0.4.4/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/tests/unit/__init__.py` & `google-cloud-gke-backup-0.4.4/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/tests/unit/gapic/__init__.py` & `google-cloud-gke-backup-0.4.4/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/tests/unit/gapic/gke_backup_v1/__init__.py` & `google-cloud-gke-backup-0.4.4/tests/unit/gapic/gke_backup_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-gke-backup-0.4.3/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py` & `google-cloud-gke-backup-0.4.4/tests/unit/gapic/gke_backup_v1/test_backup_for_gke.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,18 @@
 )
 from google.api_core import client_options
 from google.api_core import exceptions as core_exceptions
 from google.api_core import operation_async  # type: ignore
 import google.auth
 from google.auth import credentials as ga_credentials
 from google.auth.exceptions import MutualTLSChannelError
+from google.cloud.location import locations_pb2
+from google.iam.v1 import iam_policy_pb2  # type: ignore
+from google.iam.v1 import options_pb2  # type: ignore
+from google.iam.v1 import policy_pb2  # type: ignore
 from google.longrunning import operations_pb2
 from google.oauth2 import service_account
 from google.protobuf import empty_pb2  # type: ignore
 from google.protobuf import field_mask_pb2  # type: ignore
 from google.protobuf import json_format
 from google.protobuf import timestamp_pb2  # type: ignore
 import grpc
@@ -15859,14 +15863,23 @@
         "create_restore",
         "list_restores",
         "get_restore",
         "update_restore",
         "delete_restore",
         "list_volume_restores",
         "get_volume_restore",
+        "set_iam_policy",
+        "get_iam_policy",
+        "test_iam_permissions",
+        "get_location",
+        "list_locations",
+        "get_operation",
+        "cancel_operation",
+        "delete_operation",
+        "list_operations",
     )
     for method in methods:
         with pytest.raises(NotImplementedError):
             getattr(transport, method)(request=object())
 
     with pytest.raises(NotImplementedError):
         transport.close()
@@ -16739,14 +16752,1902 @@
         type(getattr(client.transport, "grpc_channel")), "close"
     ) as close:
         async with client:
             close.assert_not_called()
         close.assert_called_once()
 
 
+def test_get_location_rest_bad_request(
+    transport: str = "rest", request_type=locations_pb2.GetLocationRequest
+):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict(
+        {"name": "projects/sample1/locations/sample2"}, request
+    )
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.get_location(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        locations_pb2.GetLocationRequest,
+        dict,
+    ],
+)
+def test_get_location_rest(request_type):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {"name": "projects/sample1/locations/sample2"}
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = locations_pb2.Location()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.get_location(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+def test_list_locations_rest_bad_request(
+    transport: str = "rest", request_type=locations_pb2.ListLocationsRequest
+):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict({"name": "projects/sample1"}, request)
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.list_locations(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        locations_pb2.ListLocationsRequest,
+        dict,
+    ],
+)
+def test_list_locations_rest(request_type):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {"name": "projects/sample1"}
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = locations_pb2.ListLocationsResponse()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.list_locations(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+def test_get_iam_policy_rest_bad_request(
+    transport: str = "rest", request_type=iam_policy_pb2.GetIamPolicyRequest
+):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict(
+        {"resource": "projects/sample1/locations/sample2/backupPlans/sample3"}, request
+    )
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.get_iam_policy(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        iam_policy_pb2.GetIamPolicyRequest,
+        dict,
+    ],
+)
+def test_get_iam_policy_rest(request_type):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {
+        "resource": "projects/sample1/locations/sample2/backupPlans/sample3"
+    }
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = policy_pb2.Policy()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.get_iam_policy(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, policy_pb2.Policy)
+
+
+def test_set_iam_policy_rest_bad_request(
+    transport: str = "rest", request_type=iam_policy_pb2.SetIamPolicyRequest
+):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict(
+        {"resource": "projects/sample1/locations/sample2/backupPlans/sample3"}, request
+    )
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.set_iam_policy(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        iam_policy_pb2.SetIamPolicyRequest,
+        dict,
+    ],
+)
+def test_set_iam_policy_rest(request_type):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {
+        "resource": "projects/sample1/locations/sample2/backupPlans/sample3"
+    }
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = policy_pb2.Policy()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.set_iam_policy(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, policy_pb2.Policy)
+
+
+def test_test_iam_permissions_rest_bad_request(
+    transport: str = "rest", request_type=iam_policy_pb2.TestIamPermissionsRequest
+):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict(
+        {"resource": "projects/sample1/locations/sample2/backupPlans/sample3"}, request
+    )
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.test_iam_permissions(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        iam_policy_pb2.TestIamPermissionsRequest,
+        dict,
+    ],
+)
+def test_test_iam_permissions_rest(request_type):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {
+        "resource": "projects/sample1/locations/sample2/backupPlans/sample3"
+    }
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = iam_policy_pb2.TestIamPermissionsResponse()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.test_iam_permissions(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, iam_policy_pb2.TestIamPermissionsResponse)
+
+
+def test_cancel_operation_rest_bad_request(
+    transport: str = "rest", request_type=operations_pb2.CancelOperationRequest
+):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict(
+        {"name": "projects/sample1/locations/sample2/operations/sample3"}, request
+    )
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.cancel_operation(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        operations_pb2.CancelOperationRequest,
+        dict,
+    ],
+)
+def test_cancel_operation_rest(request_type):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {"name": "projects/sample1/locations/sample2/operations/sample3"}
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = None
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = "{}"
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.cancel_operation(request)
+
+    # Establish that the response is the type that we expect.
+    assert response is None
+
+
+def test_delete_operation_rest_bad_request(
+    transport: str = "rest", request_type=operations_pb2.DeleteOperationRequest
+):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict(
+        {"name": "projects/sample1/locations/sample2"}, request
+    )
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.delete_operation(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        operations_pb2.DeleteOperationRequest,
+        dict,
+    ],
+)
+def test_delete_operation_rest(request_type):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {"name": "projects/sample1/locations/sample2"}
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = None
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = "{}"
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.delete_operation(request)
+
+    # Establish that the response is the type that we expect.
+    assert response is None
+
+
+def test_get_operation_rest_bad_request(
+    transport: str = "rest", request_type=operations_pb2.GetOperationRequest
+):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict(
+        {"name": "projects/sample1/locations/sample2/operations/sample3"}, request
+    )
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.get_operation(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        operations_pb2.GetOperationRequest,
+        dict,
+    ],
+)
+def test_get_operation_rest(request_type):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {"name": "projects/sample1/locations/sample2/operations/sample3"}
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.Operation()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.get_operation(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, operations_pb2.Operation)
+
+
+def test_list_operations_rest_bad_request(
+    transport: str = "rest", request_type=operations_pb2.ListOperationsRequest
+):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    request = request_type()
+    request = json_format.ParseDict(
+        {"name": "projects/sample1/locations/sample2"}, request
+    )
+
+    # Mock the http request call within the method and fake a BadRequest error.
+    with mock.patch.object(Session, "request") as req, pytest.raises(
+        core_exceptions.BadRequest
+    ):
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 400
+        response_value.request = Request()
+        req.return_value = response_value
+        client.list_operations(request)
+
+
+@pytest.mark.parametrize(
+    "request_type",
+    [
+        operations_pb2.ListOperationsRequest,
+        dict,
+    ],
+)
+def test_list_operations_rest(request_type):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="rest",
+    )
+    request_init = {"name": "projects/sample1/locations/sample2"}
+    request = request_type(**request_init)
+    # Mock the http request call within the method and fake a response.
+    with mock.patch.object(type(client.transport._session), "request") as req:
+        # Designate an appropriate value for the returned response.
+        return_value = operations_pb2.ListOperationsResponse()
+
+        # Wrap the value into a proper Response obj
+        response_value = Response()
+        response_value.status_code = 200
+        json_return_value = json_format.MessageToJson(return_value)
+
+        response_value._content = json_return_value.encode("UTF-8")
+        req.return_value = response_value
+
+        response = client.list_operations(request)
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, operations_pb2.ListOperationsResponse)
+
+
+def test_delete_operation(transport: str = "grpc"):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.DeleteOperationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = None
+        response = client.delete_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert response is None
+
+
+@pytest.mark.asyncio
+async def test_delete_operation_async(transport: str = "grpc"):
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.DeleteOperationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.delete_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert response is None
+
+
+def test_delete_operation_field_headers():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.DeleteOperationRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
+        call.return_value = None
+
+        client.delete_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_delete_operation_field_headers_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.DeleteOperationRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        await client.delete_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_delete_operation_from_dict():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = None
+
+        response = client.delete_operation(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_delete_operation_from_dict_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.delete_operation(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+def test_cancel_operation(transport: str = "grpc"):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.CancelOperationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = None
+        response = client.cancel_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert response is None
+
+
+@pytest.mark.asyncio
+async def test_cancel_operation_async(transport: str = "grpc"):
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.CancelOperationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.cancel_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert response is None
+
+
+def test_cancel_operation_field_headers():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.CancelOperationRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
+        call.return_value = None
+
+        client.cancel_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_cancel_operation_field_headers_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.CancelOperationRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        await client.cancel_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_cancel_operation_from_dict():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = None
+
+        response = client.cancel_operation(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_cancel_operation_from_dict_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.cancel_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.cancel_operation(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+def test_get_operation(transport: str = "grpc"):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.GetOperationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation()
+        response = client.get_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, operations_pb2.Operation)
+
+
+@pytest.mark.asyncio
+async def test_get_operation_async(transport: str = "grpc"):
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.GetOperationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation()
+        )
+        response = await client.get_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, operations_pb2.Operation)
+
+
+def test_get_operation_field_headers():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.GetOperationRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        call.return_value = operations_pb2.Operation()
+
+        client.get_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_get_operation_field_headers_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.GetOperationRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation()
+        )
+        await client.get_operation(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_get_operation_from_dict():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.Operation()
+
+        response = client.get_operation(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_get_operation_from_dict_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_operation), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation()
+        )
+        response = await client.get_operation(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+def test_list_operations(transport: str = "grpc"):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.ListOperationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.ListOperationsResponse()
+        response = client.list_operations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, operations_pb2.ListOperationsResponse)
+
+
+@pytest.mark.asyncio
+async def test_list_operations_async(transport: str = "grpc"):
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = operations_pb2.ListOperationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.ListOperationsResponse()
+        )
+        response = await client.list_operations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, operations_pb2.ListOperationsResponse)
+
+
+def test_list_operations_field_headers():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.ListOperationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
+        call.return_value = operations_pb2.ListOperationsResponse()
+
+        client.list_operations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_list_operations_field_headers_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = operations_pb2.ListOperationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.ListOperationsResponse()
+        )
+        await client.list_operations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_list_operations_from_dict():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = operations_pb2.ListOperationsResponse()
+
+        response = client.list_operations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_list_operations_from_dict_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_operations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.ListOperationsResponse()
+        )
+        response = await client.list_operations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+def test_list_locations(transport: str = "grpc"):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.ListLocationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.ListLocationsResponse()
+        response = client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+@pytest.mark.asyncio
+async def test_list_locations_async(transport: str = "grpc"):
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.ListLocationsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        response = await client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.ListLocationsResponse)
+
+
+def test_list_locations_field_headers():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.ListLocationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        call.return_value = locations_pb2.ListLocationsResponse()
+
+        client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_list_locations_field_headers_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.ListLocationsRequest()
+    request.name = "locations"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        await client.list_locations(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations",
+    ) in kw["metadata"]
+
+
+def test_list_locations_from_dict():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.ListLocationsResponse()
+
+        response = client.list_locations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_list_locations_from_dict_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.ListLocationsResponse()
+        )
+        response = await client.list_locations(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+def test_get_location(transport: str = "grpc"):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.GetLocationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.Location()
+        response = client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+@pytest.mark.asyncio
+async def test_get_location_async(transport: str = "grpc_asyncio"):
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = locations_pb2.GetLocationRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        response = await client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, locations_pb2.Location)
+
+
+def test_get_location_field_headers():
+    client = BackupForGKEClient(credentials=ga_credentials.AnonymousCredentials())
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.GetLocationRequest()
+    request.name = "locations/abc"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        call.return_value = locations_pb2.Location()
+
+        client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations/abc",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_get_location_field_headers_async():
+    client = BackupForGKEAsyncClient(credentials=ga_credentials.AnonymousCredentials())
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = locations_pb2.GetLocationRequest()
+    request.name = "locations/abc"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_location), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        await client.get_location(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "name=locations/abc",
+    ) in kw["metadata"]
+
+
+def test_get_location_from_dict():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = locations_pb2.Location()
+
+        response = client.get_location(
+            request={
+                "name": "locations/abc",
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_get_location_from_dict_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_locations), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            locations_pb2.Location()
+        )
+        response = await client.get_location(
+            request={
+                "name": "locations",
+            }
+        )
+        call.assert_called()
+
+
+def test_set_iam_policy(transport: str = "grpc"):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = iam_policy_pb2.SetIamPolicyRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.set_iam_policy), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = policy_pb2.Policy(
+            version=774,
+            etag=b"etag_blob",
+        )
+        response = client.set_iam_policy(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, policy_pb2.Policy)
+
+    assert response.version == 774
+
+    assert response.etag == b"etag_blob"
+
+
+@pytest.mark.asyncio
+async def test_set_iam_policy_async(transport: str = "grpc_asyncio"):
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = iam_policy_pb2.SetIamPolicyRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.set_iam_policy), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            policy_pb2.Policy(
+                version=774,
+                etag=b"etag_blob",
+            )
+        )
+        response = await client.set_iam_policy(request)
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, policy_pb2.Policy)
+
+    assert response.version == 774
+
+    assert response.etag == b"etag_blob"
+
+
+def test_set_iam_policy_field_headers():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = iam_policy_pb2.SetIamPolicyRequest()
+    request.resource = "resource/value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.set_iam_policy), "__call__") as call:
+        call.return_value = policy_pb2.Policy()
+
+        client.set_iam_policy(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "resource=resource/value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_set_iam_policy_field_headers_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = iam_policy_pb2.SetIamPolicyRequest()
+    request.resource = "resource/value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.set_iam_policy), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(policy_pb2.Policy())
+
+        await client.set_iam_policy(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "resource=resource/value",
+    ) in kw["metadata"]
+
+
+def test_set_iam_policy_from_dict():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.set_iam_policy), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = policy_pb2.Policy()
+
+        response = client.set_iam_policy(
+            request={
+                "resource": "resource_value",
+                "policy": policy_pb2.Policy(version=774),
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_set_iam_policy_from_dict_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.set_iam_policy), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(policy_pb2.Policy())
+
+        response = await client.set_iam_policy(
+            request={
+                "resource": "resource_value",
+                "policy": policy_pb2.Policy(version=774),
+            }
+        )
+        call.assert_called()
+
+
+def test_get_iam_policy(transport: str = "grpc"):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = iam_policy_pb2.GetIamPolicyRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_iam_policy), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = policy_pb2.Policy(
+            version=774,
+            etag=b"etag_blob",
+        )
+
+        response = client.get_iam_policy(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, policy_pb2.Policy)
+
+    assert response.version == 774
+
+    assert response.etag == b"etag_blob"
+
+
+@pytest.mark.asyncio
+async def test_get_iam_policy_async(transport: str = "grpc_asyncio"):
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = iam_policy_pb2.GetIamPolicyRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_iam_policy), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            policy_pb2.Policy(
+                version=774,
+                etag=b"etag_blob",
+            )
+        )
+
+        response = await client.get_iam_policy(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, policy_pb2.Policy)
+
+    assert response.version == 774
+
+    assert response.etag == b"etag_blob"
+
+
+def test_get_iam_policy_field_headers():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = iam_policy_pb2.GetIamPolicyRequest()
+    request.resource = "resource/value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_iam_policy), "__call__") as call:
+        call.return_value = policy_pb2.Policy()
+
+        client.get_iam_policy(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "resource=resource/value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_get_iam_policy_field_headers_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = iam_policy_pb2.GetIamPolicyRequest()
+    request.resource = "resource/value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_iam_policy), "__call__") as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(policy_pb2.Policy())
+
+        await client.get_iam_policy(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "resource=resource/value",
+    ) in kw["metadata"]
+
+
+def test_get_iam_policy_from_dict():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_iam_policy), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = policy_pb2.Policy()
+
+        response = client.get_iam_policy(
+            request={
+                "resource": "resource_value",
+                "options": options_pb2.GetPolicyOptions(requested_policy_version=2598),
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_get_iam_policy_from_dict_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_iam_policy), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(policy_pb2.Policy())
+
+        response = await client.get_iam_policy(
+            request={
+                "resource": "resource_value",
+                "options": options_pb2.GetPolicyOptions(requested_policy_version=2598),
+            }
+        )
+        call.assert_called()
+
+
+def test_test_iam_permissions(transport: str = "grpc"):
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = iam_policy_pb2.TestIamPermissionsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.test_iam_permissions), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = iam_policy_pb2.TestIamPermissionsResponse(
+            permissions=["permissions_value"],
+        )
+
+        response = client.test_iam_permissions(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, iam_policy_pb2.TestIamPermissionsResponse)
+
+    assert response.permissions == ["permissions_value"]
+
+
+@pytest.mark.asyncio
+async def test_test_iam_permissions_async(transport: str = "grpc_asyncio"):
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport=transport,
+    )
+
+    # Everything is optional in proto3 as far as the runtime is concerned,
+    # and we are mocking out the actual API, so just send an empty request.
+    request = iam_policy_pb2.TestIamPermissionsRequest()
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.test_iam_permissions), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            iam_policy_pb2.TestIamPermissionsResponse(
+                permissions=["permissions_value"],
+            )
+        )
+
+        response = await client.test_iam_permissions(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+
+        assert args[0] == request
+
+    # Establish that the response is the type that we expect.
+    assert isinstance(response, iam_policy_pb2.TestIamPermissionsResponse)
+
+    assert response.permissions == ["permissions_value"]
+
+
+def test_test_iam_permissions_field_headers():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = iam_policy_pb2.TestIamPermissionsRequest()
+    request.resource = "resource/value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.test_iam_permissions), "__call__"
+    ) as call:
+        call.return_value = iam_policy_pb2.TestIamPermissionsResponse()
+
+        client.test_iam_permissions(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls) == 1
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "resource=resource/value",
+    ) in kw["metadata"]
+
+
+@pytest.mark.asyncio
+async def test_test_iam_permissions_field_headers_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+
+    # Any value that is part of the HTTP/1.1 URI should be sent as
+    # a field header. Set these to a non-empty value.
+    request = iam_policy_pb2.TestIamPermissionsRequest()
+    request.resource = "resource/value"
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.test_iam_permissions), "__call__"
+    ) as call:
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            iam_policy_pb2.TestIamPermissionsResponse()
+        )
+
+        await client.test_iam_permissions(request)
+
+        # Establish that the underlying gRPC stub method was called.
+        assert len(call.mock_calls)
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == request
+
+    # Establish that the field header was sent.
+    _, _, kw = call.mock_calls[0]
+    assert (
+        "x-goog-request-params",
+        "resource=resource/value",
+    ) in kw["metadata"]
+
+
+def test_test_iam_permissions_from_dict():
+    client = BackupForGKEClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.test_iam_permissions), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = iam_policy_pb2.TestIamPermissionsResponse()
+
+        response = client.test_iam_permissions(
+            request={
+                "resource": "resource_value",
+                "permissions": ["permissions_value"],
+            }
+        )
+        call.assert_called()
+
+
+@pytest.mark.asyncio
+async def test_test_iam_permissions_from_dict_async():
+    client = BackupForGKEAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+    )
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.test_iam_permissions), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            iam_policy_pb2.TestIamPermissionsResponse()
+        )
+
+        response = await client.test_iam_permissions(
+            request={
+                "resource": "resource_value",
+                "permissions": ["permissions_value"],
+            }
+        )
+        call.assert_called()
+
+
 def test_transport_close():
     transports = {
         "rest": "_session",
         "grpc": "_grpc_channel",
     }
 
     for transport, close_name in transports.items():
```

