# Comparing `tmp/peek-core-device-3.4.1.tar.gz` & `tmp/peek-core-device-3.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "peek-core-device-3.4.1.tar", last modified: Wed May 17 03:30:46 2023, max compression
+gzip compressed data, was "peek-core-device-3.4.2.tar", last modified: Tue Jun 13 11:58:53 2023, max compression
```

## Comparing `peek-core-device-3.4.1.tar` & `peek-core-device-3.4.2.tar`

### file list

```diff
@@ -1,231 +1,231 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.831324 peek-core-device-3.4.1/
--rw-r--r--   0 root         (0) root         (0)      407 2023-05-17 03:30:46.830324 peek-core-device-3.4.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      138 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.821324 peek-core-device-3.4.1/peek_core_device/
--rw-r--r--   0 root         (0) root         (0)      466 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/PlatformDependencyTest.py
--rw-r--r--   0 root         (0) root         (0)      692 2023-05-17 03:30:46.000000 peek-core-device-3.4.1/peek_core_device/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.822324 peek-core-device-3.4.1/peek_core_device/_private/
--rw-r--r--   0 root         (0) root         (0)      224 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/PluginNames.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.822324 peek-core-device-3.4.1/peek_core_device/_private/admin-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.822324 peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-cache-status/
--rw-r--r--   0 root         (0) root         (0)     1644 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.html
--rw-r--r--   0 root         (0) root         (0)       33 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.scss
--rw-r--r--   0 root         (0) root         (0)     2443 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.822324 peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-info-table/
--rw-r--r--   0 root         (0) root         (0)     5597 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-info-table/device-info.component.html
--rw-r--r--   0 root         (0) root         (0)     5442 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-info-table/device-info.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.822324 peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-update-table/
--rw-r--r--   0 root         (0) root         (0)     1741 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-update-table/device-update.component.html
--rw-r--r--   0 root         (0) root         (0)     2504 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-update-table/device-update.component.ts
--rw-r--r--   0 root         (0) root         (0)     2986 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/device.component.html
--rw-r--r--   0 root         (0) root         (0)      209 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/device.component.ts
--rw-r--r--   0 root         (0) root         (0)     3125 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/device.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.822324 peek-core-device-3.4.1/peek_core_device/_private/admin-app/edit-setting-table/
--rw-r--r--   0 root         (0) root         (0)     2595 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/edit-setting-table/edit.component.html
--rw-r--r--   0 root         (0) root         (0)     1502 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/edit-setting-table/edit.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.822324 peek-core-device-3.4.1/peek_core_device/_private/admin-app/loading/
--rw-r--r--   0 root         (0) root         (0)      302 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/loading/loading.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.822324 peek-core-device-3.4.1/peek_core_device/_private/admin-app/tuples/
--rw-r--r--   0 root         (0) root         (0)      528 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/tuples/DeviceCacheStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)     3278 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/tuples/DeviceInfoTable.ts
--rw-r--r--   0 root         (0) root         (0)      469 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/tuples/UpdateOfflineCacheSettingAction.ts
--rw-r--r--   0 root         (0) root         (0)       53 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/tuples/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.823324 peek-core-device-3.4.1/peek_core_device/_private/admin-app/upload-device-update/
--rw-r--r--   0 root         (0) root         (0)     3134 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.html
--rw-r--r--   0 root         (0) root         (0)     4085 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.823324 peek-core-device-3.4.1/peek_core_device/_private/alembic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/alembic/__init__.py
--rw-r--r--   0 root         (0) root         (0)      318 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/alembic/env.py
--rw-r--r--   0 root         (0) root         (0)      524 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/alembic/script.py.mako
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.823324 peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/
--rw-r--r--   0 root         (0) root         (0)     1916 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/02f9305f9e7f_added_gps_tracking.py
--rw-r--r--   0 root         (0) root         (0)     1681 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/2561b7732a6c_gps_devicetoken_on_cascade.py
--rw-r--r--   0 root         (0) root         (0)      895 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/4b0d6309e556_add_offline_cache_enable.py
--rw-r--r--   0 root         (0) root         (0)      800 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/5dd43ff7ea8e_added_filesize_to_update_tuple.py
--rw-r--r--   0 root         (0) root         (0)     1313 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/6bf6ecef3108_timezone_aware.py
--rw-r--r--   0 root         (0) root         (0)     1129 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/7f628c121c4c_replaced_isonline_with_devicestatus.py
--rw-r--r--   0 root         (0) root         (0)      810 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/97d44e5aeb18_add_lastbandwidthmetric.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4139 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/d94277dd8aca_initial_table_creation.py
--rw-r--r--   0 root         (0) root         (0)       94 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/alembic.ini
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.823324 peek-core-device-3.4.1/peek_core_device/_private/both-app/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.823324 peek-core-device-3.4.1/peek_core_device/_private/both-app/connect/
--rw-r--r--   0 root         (0) root         (0)     3212 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-app/connect/connect.component.ts
--rw-r--r--   0 root         (0) root         (0)     2405 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-app/connect/connect.component.web.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.823324 peek-core-device-3.4.1/peek_core_device/_private/both-app/connecting/
--rw-r--r--   0 root         (0) root         (0)     1448 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-app/connecting/connecting.component.ts
--rw-r--r--   0 root         (0) root         (0)     1098 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-app/connecting/connecting.component.web.html
--rw-r--r--   0 root         (0) root         (0)      285 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-app/device.component.ts
--rw-r--r--   0 root         (0) root         (0)      471 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-app/device.component.web.html
--rw-r--r--   0 root         (0) root         (0)     2988 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-app/device.module.ts
--rw-r--r--   0 root         (0) root         (0)     1006 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-app/device.routes.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.824324 peek-core-device-3.4.1/peek_core_device/_private/both-app/enroll/
--rw-r--r--   0 root         (0) root         (0)     3897 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-app/enroll/enroll.component.ts
--rw-r--r--   0 root         (0) root         (0)     1295 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-app/enroll/enroll.component.web.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.824324 peek-core-device-3.4.1/peek_core_device/_private/both-app/enrolling/
--rw-r--r--   0 root         (0) root         (0)     1536 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-app/enrolling/enrolling.component.ts
--rw-r--r--   0 root         (0) root         (0)      582 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-app/enrolling/enrolling.component.web.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.824324 peek-core-device-3.4.1/peek_core_device/_private/both-app/loading/
--rw-r--r--   0 root         (0) root         (0)      537 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-app/loading/loading.component.ts
--rw-r--r--   0 root         (0) root         (0)      489 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-app/loading/loading.component.web.html
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.824324 peek-core-device-3.4.1/peek_core_device/_private/both-cfg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.824324 peek-core-device-3.4.1/peek_core_device/_private/both-cfg/connect/
--rw-r--r--   0 root         (0) root         (0)     2539 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-cfg/connect/connect.component.ts
--rw-r--r--   0 root         (0) root         (0)      305 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-cfg/connect/connect.component.web.html
--rw-r--r--   0 root         (0) root         (0)     1602 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-cfg/core-device-cfg.component.ts
--rw-r--r--   0 root         (0) root         (0)     1864 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-cfg/core-device-cfg.component.web.html
--rw-r--r--   0 root         (0) root         (0)     2798 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/both-cfg/core-device-cfg.module.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.824324 peek-core-device-3.4.1/peek_core_device/_private/client/
--rw-r--r--   0 root         (0) root         (0)     3629 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/client/ClientEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      527 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/client/DeviceTupleDataObservableProxy.py
--rw-r--r--   0 root         (0) root         (0)      496 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/client/DeviceTupleProcessorActionProxy.py
--rw-r--r--   0 root         (0) root         (0)     2175 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/client/UpdateDownloadHandler.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/client/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.824324 peek-core-device-3.4.1/peek_core_device/_private/client/controllers/
--rw-r--r--   0 root         (0) root         (0)     1808 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/client/controllers/BandwidthTestController.py
--rw-r--r--   0 root         (0) root         (0)     3949 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/client/controllers/DeviceOnlineController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/client/controllers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.825324 peek-core-device-3.4.1/peek_core_device/_private/server/
--rw-r--r--   0 root         (0) root         (0)     4271 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/DeviceApi.py
--rw-r--r--   0 root         (0) root         (0)     5495 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/LogicEntryHook.py
--rw-r--r--   0 root         (0) root         (0)      532 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/TupleActionProcessor.py
--rw-r--r--   0 root         (0) root         (0)     3789 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/TupleDataObservable.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.825324 peek-core-device-3.4.1/peek_core_device/_private/server/admin_backend/
--rw-r--r--   0 root         (0) root         (0)     2170 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/admin_backend/SettingPropertyHandler.py
--rw-r--r--   0 root         (0) root         (0)      318 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/admin_backend/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.825324 peek-core-device-3.4.1/peek_core_device/_private/server/controller/
--rw-r--r--   0 root         (0) root         (0)     2786 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/controller/BandwidthResultController.py
--rw-r--r--   0 root         (0) root         (0)     4319 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/controller/DeviceStatusController.py
--rw-r--r--   0 root         (0) root         (0)     4352 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/controller/EnrollmentController.py
--rw-r--r--   0 root         (0) root         (0)     5391 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/controller/GpsController.py
--rw-r--r--   0 root         (0) root         (0)     3978 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/controller/MainController.py
--rw-r--r--   0 root         (0) root         (0)     3238 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/controller/NotifierController.py
--rw-r--r--   0 root         (0) root         (0)     3701 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/controller/OfflineCacheController.py
--rw-r--r--   0 root         (0) root         (0)     5731 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/controller/UpdateController.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/controller/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.826324 peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/
--rw-r--r--   0 root         (0) root         (0)     2324 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/ClientSettingsTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1240 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/DeviceGpsLocationTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     3152 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/DeviceInfoTableTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     3001 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/DeviceInfoTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     2556 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/DeviceUpdateTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1348 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/OfflineCacheCombinedStatusTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)     1692 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/OfflineCacheSettingTupleProvider.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.826324 peek-core-device-3.4.1/peek_core_device/_private/server/update_resources/
--rw-r--r--   0 root         (0) root         (0)     2350 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/update_resources/DeviceUpdateUploadResource.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/server/update_resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.826324 peek-core-device-3.4.1/peek_core_device/_private/storage/
--rw-r--r--   0 root         (0) root         (0)      711 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/storage/DeclarativeBase.py
--rw-r--r--   0 root         (0) root         (0)     3713 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/storage/DeviceInfoTable.py
--rw-r--r--   0 root         (0) root         (0)     1431 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/storage/DeviceUpdateTuple.py
--rw-r--r--   0 root         (0) root         (0)     1005 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/storage/GpsLocationHistoryTable.py
--rw-r--r--   0 root         (0) root         (0)     1242 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/storage/GpsLocationTable.py
--rw-r--r--   0 root         (0) root         (0)     8668 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/storage/Setting.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/storage/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.827324 peek-core-device-3.4.1/peek_core_device/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      777 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/AlterDeviceUpdateAction.py
--rw-r--r--   0 root         (0) root         (0)      509 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/BandwidthTestResultTuple.py
--rw-r--r--   0 root         (0) root         (0)      342 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/BandwidthTestTuple.py
--rw-r--r--   0 root         (0) root         (0)      686 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/ClientSettingsTuple.py
--rw-r--r--   0 root         (0) root         (0)      602 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/CreateDeviceUpdateAction.py
--rw-r--r--   0 root         (0) root         (0)      414 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/DeviceBackgroundStateTupleAction.py
--rw-r--r--   0 root         (0) root         (0)      545 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/DeviceCacheStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      446 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/EnrolDeviceAction.py
--rw-r--r--   0 root         (0) root         (0)      847 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/OfflineCacheCombinedStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      691 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/OfflineCacheLoaderStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      447 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/OfflineCacheSettingTuple.py
--rw-r--r--   0 root         (0) root         (0)      890 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/OfflineCacheStatusAction.py
--rw-r--r--   0 root         (0) root         (0)     1459 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/OfflineCacheStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      506 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/UpdateAppliedAction.py
--rw-r--r--   0 root         (0) root         (0)      590 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/UpdateDeviceGpsLocationTupleAction.py
--rw-r--r--   0 root         (0) root         (0)      620 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/UpdateDeviceOnlineAction.py
--rw-r--r--   0 root         (0) root         (0)      587 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/UpdateEnrollmentAction.py
--rw-r--r--   0 root         (0) root         (0)      588 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/UpdateOfflineCacheSettingAction.py
--rw-r--r--   0 root         (0) root         (0)      637 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/WebClientVortexDetailsTuple.py
--rw-r--r--   0 root         (0) root         (0)      347 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/_private/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.827324 peek-core-device-3.4.1/peek_core_device/admin-doc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.827324 peek-core-device-3.4.1/peek_core_device/admin-doc/admin_tasks/
--rw-r--r--   0 root         (0) root         (0)    64585 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/admin-doc/admin_tasks/admin_task_devices.png
--rw-r--r--   0 root         (0) root         (0)     1475 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/admin-doc/admin_tasks/admin_tasks.rst
--rw-r--r--   0 root         (0) root         (0)    62597 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/admin-doc/admin_tasks/device_search.png
--rw-r--r--   0 root         (0) root         (0)    25072 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/admin-doc/admin_tasks/offline_cache_info.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.827324 peek-core-device-3.4.1/peek_core_device/admin-doc/general_settings/
--rw-r--r--   0 root         (0) root         (0)    41296 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/admin-doc/general_settings/general_settings.png
--rw-r--r--   0 root         (0) root         (0)      875 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/admin-doc/general_settings/general_settings.rst
--rw-r--r--   0 root         (0) root         (0)      433 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/admin-doc/index.rst
--rw-r--r--   0 root         (0) root         (0)      515 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/admin-doc/overview.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.827324 peek-core-device-3.4.1/peek_core_device/both-doc/
--rw-r--r--   0 root         (0) root         (0)      848 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/both-doc/index.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.828324 peek-core-device-3.4.1/peek_core_device/plugin-module/
--rw-r--r--   0 root         (0) root         (0)      552 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/DeviceGpsLocationTuple.ts
--rw-r--r--   0 root         (0) root         (0)     2952 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/DeviceInfoTuple.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.829324 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/
--rw-r--r--   0 root         (0) root         (0)      333 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/PluginNames.ts
--rw-r--r--   0 root         (0) root         (0)     1051 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-background.service.ts
--rw-r--r--   0 root         (0) root         (0)     7381 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-bandwidth-test.service.ts
--rw-r--r--   0 root         (0) root         (0)      767 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-loading.module.ts
--rw-r--r--   0 root         (0) root         (0)     1180 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-nav.service.ts
--rw-r--r--   0 root         (0) root         (0)     1024 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-online.service.ts
--rw-r--r--   0 root         (0) root         (0)     7060 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-server.service.ts
--rw-r--r--   0 root         (0) root         (0)     2937 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-tuple.service.ts
--rw-r--r--   0 root         (0) root         (0)     5938 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-update.service.ts
--rw-r--r--   0 root         (0) root         (0)      592 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-update.service.web.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.829324 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/gps/
--rw-r--r--   0 root         (0) root         (0)      711 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/gps/GpsLocationUpdateTupleAction.ts
--rw-r--r--   0 root         (0) root         (0)     6740 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/gps/private-gps-location.service.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.829324 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/hardware-info/
--rw-r--r--   0 root         (0) root         (0)     2318 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/hardware-info/hardware-info.ts
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/hardware-info/is-field.dweb.ts
--rw-r--r--   0 root         (0) root         (0)       29 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/hardware-info/is-field.mweb.ts
--rw-r--r--   0 root         (0) root         (0)     1255 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/index.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.830324 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/
--rw-r--r--   0 root         (0) root         (0)      497 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/BandwidthTestResultTuple.ts
--rw-r--r--   0 root         (0) root         (0)      383 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/BandwidthTestTuple.ts
--rw-r--r--   0 root         (0) root         (0)      635 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/ClientSettingsTuple.ts
--rw-r--r--   0 root         (0) root         (0)      451 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/DeviceBackgroundStateTupleAction.ts
--rw-r--r--   0 root         (0) root         (0)      662 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/DeviceUpdateLocalValuesTuple.ts
--rw-r--r--   0 root         (0) root         (0)      551 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/DeviceUpdateTuple.ts
--rw-r--r--   0 root         (0) root         (0)      438 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/EnrolDeviceAction.ts
--rw-r--r--   0 root         (0) root         (0)      670 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/OfflineCacheCombinedStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      391 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/OfflineCacheSettingTuple.ts
--rw-r--r--   0 root         (0) root         (0)      477 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/OfflineCacheStatusAction.ts
--rw-r--r--   0 root         (0) root         (0)     3198 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/OfflineCacheStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)      470 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/UpdateAppliedAction.ts
--rw-r--r--   0 root         (0) root         (0)      641 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/UpdateDeviceOnlineAction.ts
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.830324 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/admin/
--rw-r--r--   0 root         (0) root         (0)      523 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/admin/AlterDeviceUpdateAction.ts
--rw-r--r--   0 root         (0) root         (0)      467 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/admin/CreateDeviceUpdateAction.ts
--rw-r--r--   0 root         (0) root         (0)      572 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts
--rw-r--r--   0 root         (0) root         (0)      455 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/admin/UpdateEnrollmentAction.ts
--rw-r--r--   0 root         (0) root         (0)      152 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/server-info-tuple-defaults.ts
--rw-r--r--   0 root         (0) root         (0)      731 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/server-info-tuple.ts
--rw-r--r--   0 root         (0) root         (0)     2337 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/device-enrolled.guard.ts
--rw-r--r--   0 root         (0) root         (0)     3849 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/device-enrolment.service.ts
--rw-r--r--   0 root         (0) root         (0)    23425 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/device-offline-cache.service.ts
--rw-r--r--   0 root         (0) root         (0)     1553 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/device-status.service.ts
--rw-r--r--   0 root         (0) root         (0)      356 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/gps-location.service.ts
--rw-r--r--   0 root         (0) root         (0)      546 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/index.ts
--rw-r--r--   0 root         (0) root         (0)      301 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.830324 peek-core-device-3.4.1/peek_core_device/plugin-module/tuples/
--rw-r--r--   0 root         (0) root         (0)     1344 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/plugin-module/tuples/OfflineCacheLoaderStatusTuple.ts
--rw-r--r--   0 root         (0) root         (0)     6342 2023-05-17 03:30:46.000000 peek-core-device-3.4.1/peek_core_device/plugin_package.json
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.830324 peek-core-device-3.4.1/peek_core_device/server/
--rw-r--r--   0 root         (0) root         (0)     2404 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/server/DeviceApiABC.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/server/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.830324 peek-core-device-3.4.1/peek_core_device/tuples/
--rw-r--r--   0 root         (0) root         (0)     1312 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/tuples/DeviceDetailTuple.py
--rw-r--r--   0 root         (0) root         (0)      494 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/tuples/DeviceGpsLocationTuple.py
--rw-r--r--   0 root         (0) root         (0)     1479 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/tuples/DeviceInfoTuple.py
--rw-r--r--   0 root         (0) root         (0)      814 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/tuples/DeviceStatusTuple.py
--rw-r--r--   0 root         (0) root         (0)      344 2023-05-17 03:29:54.000000 peek-core-device-3.4.1/peek_core_device/tuples/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-17 03:30:46.821324 peek-core-device-3.4.1/peek_core_device.egg-info/
--rw-r--r--   0 root         (0) root         (0)      407 2023-05-17 03:30:46.000000 peek-core-device-3.4.1/peek_core_device.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    11609 2023-05-17 03:30:46.000000 peek-core-device-3.4.1/peek_core_device.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-17 03:30:46.000000 peek-core-device-3.4.1/peek_core_device.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       32 2023-05-17 03:30:46.000000 peek-core-device-3.4.1/peek_core_device.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-05-17 03:30:46.000000 peek-core-device-3.4.1/peek_core_device.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-17 03:30:46.831324 peek-core-device-3.4.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2547 2023-05-17 03:30:46.000000 peek-core-device-3.4.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.486934 peek-core-device-3.4.2/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-06-13 11:58:53.486934 peek-core-device-3.4.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      138 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.476934 peek-core-device-3.4.2/peek_core_device/
+-rw-r--r--   0 root         (0) root         (0)      466 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/PlatformDependencyTest.py
+-rw-r--r--   0 root         (0) root         (0)      692 2023-06-13 11:58:53.000000 peek-core-device-3.4.2/peek_core_device/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.476934 peek-core-device-3.4.2/peek_core_device/_private/
+-rw-r--r--   0 root         (0) root         (0)      224 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/PluginNames.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.476934 peek-core-device-3.4.2/peek_core_device/_private/admin-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.476934 peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-cache-status/
+-rw-r--r--   0 root         (0) root         (0)     1644 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.html
+-rw-r--r--   0 root         (0) root         (0)       33 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.scss
+-rw-r--r--   0 root         (0) root         (0)     2443 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.477934 peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-info-table/
+-rw-r--r--   0 root         (0) root         (0)     5597 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-info-table/device-info.component.html
+-rw-r--r--   0 root         (0) root         (0)     5442 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-info-table/device-info.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.477934 peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-update-table/
+-rw-r--r--   0 root         (0) root         (0)     1741 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-update-table/device-update.component.html
+-rw-r--r--   0 root         (0) root         (0)     2504 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-update-table/device-update.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2986 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/device.component.html
+-rw-r--r--   0 root         (0) root         (0)      209 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/device.component.ts
+-rw-r--r--   0 root         (0) root         (0)     3125 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/device.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.477934 peek-core-device-3.4.2/peek_core_device/_private/admin-app/edit-setting-table/
+-rw-r--r--   0 root         (0) root         (0)     2595 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/edit-setting-table/edit.component.html
+-rw-r--r--   0 root         (0) root         (0)     1502 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/edit-setting-table/edit.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.477934 peek-core-device-3.4.2/peek_core_device/_private/admin-app/loading/
+-rw-r--r--   0 root         (0) root         (0)      302 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/loading/loading.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.477934 peek-core-device-3.4.2/peek_core_device/_private/admin-app/tuples/
+-rw-r--r--   0 root         (0) root         (0)      528 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/tuples/DeviceCacheStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     3278 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/tuples/DeviceInfoTable.ts
+-rw-r--r--   0 root         (0) root         (0)      469 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/tuples/UpdateOfflineCacheSettingAction.ts
+-rw-r--r--   0 root         (0) root         (0)       53 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/tuples/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.477934 peek-core-device-3.4.2/peek_core_device/_private/admin-app/upload-device-update/
+-rw-r--r--   0 root         (0) root         (0)     3134 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.html
+-rw-r--r--   0 root         (0) root         (0)     4085 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.477934 peek-core-device-3.4.2/peek_core_device/_private/alembic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/alembic/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      318 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/alembic/env.py
+-rw-r--r--   0 root         (0) root         (0)      524 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/alembic/script.py.mako
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.478934 peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/
+-rw-r--r--   0 root         (0) root         (0)     1916 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/02f9305f9e7f_added_gps_tracking.py
+-rw-r--r--   0 root         (0) root         (0)     1681 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/2561b7732a6c_gps_devicetoken_on_cascade.py
+-rw-r--r--   0 root         (0) root         (0)      895 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/4b0d6309e556_add_offline_cache_enable.py
+-rw-r--r--   0 root         (0) root         (0)      800 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/5dd43ff7ea8e_added_filesize_to_update_tuple.py
+-rw-r--r--   0 root         (0) root         (0)     1313 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/6bf6ecef3108_timezone_aware.py
+-rw-r--r--   0 root         (0) root         (0)     1129 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/7f628c121c4c_replaced_isonline_with_devicestatus.py
+-rw-r--r--   0 root         (0) root         (0)      810 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/97d44e5aeb18_add_lastbandwidthmetric.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4139 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/d94277dd8aca_initial_table_creation.py
+-rw-r--r--   0 root         (0) root         (0)       94 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/alembic.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.478934 peek-core-device-3.4.2/peek_core_device/_private/both-app/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.478934 peek-core-device-3.4.2/peek_core_device/_private/both-app/connect/
+-rw-r--r--   0 root         (0) root         (0)     3212 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-app/connect/connect.component.ts
+-rw-r--r--   0 root         (0) root         (0)     2405 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-app/connect/connect.component.web.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.478934 peek-core-device-3.4.2/peek_core_device/_private/both-app/connecting/
+-rw-r--r--   0 root         (0) root         (0)     1448 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-app/connecting/connecting.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1098 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-app/connecting/connecting.component.web.html
+-rw-r--r--   0 root         (0) root         (0)      285 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-app/device.component.ts
+-rw-r--r--   0 root         (0) root         (0)      471 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-app/device.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     2988 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-app/device.module.ts
+-rw-r--r--   0 root         (0) root         (0)     1006 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-app/device.routes.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.478934 peek-core-device-3.4.2/peek_core_device/_private/both-app/enroll/
+-rw-r--r--   0 root         (0) root         (0)     3897 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-app/enroll/enroll.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1295 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-app/enroll/enroll.component.web.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.479934 peek-core-device-3.4.2/peek_core_device/_private/both-app/enrolling/
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-app/enrolling/enrolling.component.ts
+-rw-r--r--   0 root         (0) root         (0)      582 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-app/enrolling/enrolling.component.web.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.479934 peek-core-device-3.4.2/peek_core_device/_private/both-app/loading/
+-rw-r--r--   0 root         (0) root         (0)      537 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-app/loading/loading.component.ts
+-rw-r--r--   0 root         (0) root         (0)      489 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-app/loading/loading.component.web.html
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.479934 peek-core-device-3.4.2/peek_core_device/_private/both-cfg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.479934 peek-core-device-3.4.2/peek_core_device/_private/both-cfg/connect/
+-rw-r--r--   0 root         (0) root         (0)     2539 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-cfg/connect/connect.component.ts
+-rw-r--r--   0 root         (0) root         (0)      305 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-cfg/connect/connect.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     1602 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-cfg/core-device-cfg.component.ts
+-rw-r--r--   0 root         (0) root         (0)     1864 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-cfg/core-device-cfg.component.web.html
+-rw-r--r--   0 root         (0) root         (0)     2798 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/both-cfg/core-device-cfg.module.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.479934 peek-core-device-3.4.2/peek_core_device/_private/client/
+-rw-r--r--   0 root         (0) root         (0)     3629 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/client/ClientEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      527 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/client/DeviceTupleDataObservableProxy.py
+-rw-r--r--   0 root         (0) root         (0)      496 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/client/DeviceTupleProcessorActionProxy.py
+-rw-r--r--   0 root         (0) root         (0)     2175 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/client/UpdateDownloadHandler.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/client/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.479934 peek-core-device-3.4.2/peek_core_device/_private/client/controllers/
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/client/controllers/BandwidthTestController.py
+-rw-r--r--   0 root         (0) root         (0)     3949 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/client/controllers/DeviceOnlineController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/client/controllers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.480934 peek-core-device-3.4.2/peek_core_device/_private/server/
+-rw-r--r--   0 root         (0) root         (0)     4271 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/DeviceApi.py
+-rw-r--r--   0 root         (0) root         (0)     5495 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/LogicEntryHook.py
+-rw-r--r--   0 root         (0) root         (0)      532 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/TupleActionProcessor.py
+-rw-r--r--   0 root         (0) root         (0)     3688 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/TupleDataObservable.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.480934 peek-core-device-3.4.2/peek_core_device/_private/server/admin_backend/
+-rw-r--r--   0 root         (0) root         (0)     2170 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/admin_backend/SettingPropertyHandler.py
+-rw-r--r--   0 root         (0) root         (0)      318 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/admin_backend/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.480934 peek-core-device-3.4.2/peek_core_device/_private/server/controller/
+-rw-r--r--   0 root         (0) root         (0)     2786 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/controller/BandwidthResultController.py
+-rw-r--r--   0 root         (0) root         (0)     4319 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/controller/DeviceStatusController.py
+-rw-r--r--   0 root         (0) root         (0)     4352 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/controller/EnrollmentController.py
+-rw-r--r--   0 root         (0) root         (0)     5391 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/controller/GpsController.py
+-rw-r--r--   0 root         (0) root         (0)     3978 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/controller/MainController.py
+-rw-r--r--   0 root         (0) root         (0)     3238 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/controller/NotifierController.py
+-rw-r--r--   0 root         (0) root         (0)     3701 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/controller/OfflineCacheController.py
+-rw-r--r--   0 root         (0) root         (0)     5731 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/controller/UpdateController.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/controller/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.481934 peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/ClientSettingsTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1240 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/DeviceGpsLocationTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/DeviceInfoTableTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     3001 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/DeviceInfoTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/DeviceUpdateTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1348 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/OfflineCacheCombinedStatusTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)     1692 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/OfflineCacheSettingTupleProvider.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.481934 peek-core-device-3.4.2/peek_core_device/_private/server/update_resources/
+-rw-r--r--   0 root         (0) root         (0)     2350 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/update_resources/DeviceUpdateUploadResource.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/server/update_resources/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.481934 peek-core-device-3.4.2/peek_core_device/_private/storage/
+-rw-r--r--   0 root         (0) root         (0)      711 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/storage/DeclarativeBase.py
+-rw-r--r--   0 root         (0) root         (0)     3713 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/storage/DeviceInfoTable.py
+-rw-r--r--   0 root         (0) root         (0)     1431 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/storage/DeviceUpdateTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1005 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/storage/GpsLocationHistoryTable.py
+-rw-r--r--   0 root         (0) root         (0)     1242 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/storage/GpsLocationTable.py
+-rw-r--r--   0 root         (0) root         (0)     9117 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/storage/Setting.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/storage/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.482934 peek-core-device-3.4.2/peek_core_device/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      777 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/AlterDeviceUpdateAction.py
+-rw-r--r--   0 root         (0) root         (0)      509 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/BandwidthTestResultTuple.py
+-rw-r--r--   0 root         (0) root         (0)      342 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/BandwidthTestTuple.py
+-rw-r--r--   0 root         (0) root         (0)      812 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/ClientSettingsTuple.py
+-rw-r--r--   0 root         (0) root         (0)      602 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/CreateDeviceUpdateAction.py
+-rw-r--r--   0 root         (0) root         (0)      414 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/DeviceBackgroundStateTupleAction.py
+-rw-r--r--   0 root         (0) root         (0)      545 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/DeviceCacheStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      446 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/EnrolDeviceAction.py
+-rw-r--r--   0 root         (0) root         (0)      847 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/OfflineCacheCombinedStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      691 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/OfflineCacheLoaderStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      447 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/OfflineCacheSettingTuple.py
+-rw-r--r--   0 root         (0) root         (0)      890 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/OfflineCacheStatusAction.py
+-rw-r--r--   0 root         (0) root         (0)     1459 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/OfflineCacheStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      506 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/UpdateAppliedAction.py
+-rw-r--r--   0 root         (0) root         (0)      590 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/UpdateDeviceGpsLocationTupleAction.py
+-rw-r--r--   0 root         (0) root         (0)      620 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/UpdateDeviceOnlineAction.py
+-rw-r--r--   0 root         (0) root         (0)      587 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/UpdateEnrollmentAction.py
+-rw-r--r--   0 root         (0) root         (0)      588 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/UpdateOfflineCacheSettingAction.py
+-rw-r--r--   0 root         (0) root         (0)      637 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/WebClientVortexDetailsTuple.py
+-rw-r--r--   0 root         (0) root         (0)      347 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/_private/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.482934 peek-core-device-3.4.2/peek_core_device/admin-doc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.483934 peek-core-device-3.4.2/peek_core_device/admin-doc/admin_tasks/
+-rw-r--r--   0 root         (0) root         (0)    64585 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/admin-doc/admin_tasks/admin_task_devices.png
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/admin-doc/admin_tasks/admin_tasks.rst
+-rw-r--r--   0 root         (0) root         (0)    62597 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/admin-doc/admin_tasks/device_search.png
+-rw-r--r--   0 root         (0) root         (0)    25072 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/admin-doc/admin_tasks/offline_cache_info.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.483934 peek-core-device-3.4.2/peek_core_device/admin-doc/general_settings/
+-rw-r--r--   0 root         (0) root         (0)    41296 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/admin-doc/general_settings/general_settings.png
+-rw-r--r--   0 root         (0) root         (0)      875 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/admin-doc/general_settings/general_settings.rst
+-rw-r--r--   0 root         (0) root         (0)      433 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/admin-doc/index.rst
+-rw-r--r--   0 root         (0) root         (0)      515 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/admin-doc/overview.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.483934 peek-core-device-3.4.2/peek_core_device/both-doc/
+-rw-r--r--   0 root         (0) root         (0)      848 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/both-doc/index.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.483934 peek-core-device-3.4.2/peek_core_device/plugin-module/
+-rw-r--r--   0 root         (0) root         (0)      552 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/DeviceGpsLocationTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/DeviceInfoTuple.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.484934 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/
+-rw-r--r--   0 root         (0) root         (0)      333 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/PluginNames.ts
+-rw-r--r--   0 root         (0) root         (0)     1051 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-background.service.ts
+-rw-r--r--   0 root         (0) root         (0)     8054 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-bandwidth-test.service.ts
+-rw-r--r--   0 root         (0) root         (0)      767 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-loading.module.ts
+-rw-r--r--   0 root         (0) root         (0)     1180 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-nav.service.ts
+-rw-r--r--   0 root         (0) root         (0)     1024 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-online.service.ts
+-rw-r--r--   0 root         (0) root         (0)     7060 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-server.service.ts
+-rw-r--r--   0 root         (0) root         (0)     2937 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-tuple.service.ts
+-rw-r--r--   0 root         (0) root         (0)     5938 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-update.service.ts
+-rw-r--r--   0 root         (0) root         (0)      592 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-update.service.web.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.484934 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/gps/
+-rw-r--r--   0 root         (0) root         (0)      711 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/gps/GpsLocationUpdateTupleAction.ts
+-rw-r--r--   0 root         (0) root         (0)     6740 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/gps/private-gps-location.service.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.484934 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/hardware-info/
+-rw-r--r--   0 root         (0) root         (0)     2318 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/hardware-info/hardware-info.ts
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/hardware-info/is-field.dweb.ts
+-rw-r--r--   0 root         (0) root         (0)       29 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/hardware-info/is-field.mweb.ts
+-rw-r--r--   0 root         (0) root         (0)     1255 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/index.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.485934 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/
+-rw-r--r--   0 root         (0) root         (0)      497 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/BandwidthTestResultTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      383 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/BandwidthTestTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      789 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/ClientSettingsTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      451 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/DeviceBackgroundStateTupleAction.ts
+-rw-r--r--   0 root         (0) root         (0)      662 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/DeviceUpdateLocalValuesTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      551 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/DeviceUpdateTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      438 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/EnrolDeviceAction.ts
+-rw-r--r--   0 root         (0) root         (0)      670 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/OfflineCacheCombinedStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      391 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/OfflineCacheSettingTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      477 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/OfflineCacheStatusAction.ts
+-rw-r--r--   0 root         (0) root         (0)     3198 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/OfflineCacheStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      470 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/UpdateAppliedAction.ts
+-rw-r--r--   0 root         (0) root         (0)      641 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/UpdateDeviceOnlineAction.ts
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.485934 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/admin/
+-rw-r--r--   0 root         (0) root         (0)      523 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/admin/AlterDeviceUpdateAction.ts
+-rw-r--r--   0 root         (0) root         (0)      467 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/admin/CreateDeviceUpdateAction.ts
+-rw-r--r--   0 root         (0) root         (0)      572 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts
+-rw-r--r--   0 root         (0) root         (0)      455 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/admin/UpdateEnrollmentAction.ts
+-rw-r--r--   0 root         (0) root         (0)      152 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/server-info-tuple-defaults.ts
+-rw-r--r--   0 root         (0) root         (0)      731 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/server-info-tuple.ts
+-rw-r--r--   0 root         (0) root         (0)     2337 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/device-enrolled.guard.ts
+-rw-r--r--   0 root         (0) root         (0)     3849 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/device-enrolment.service.ts
+-rw-r--r--   0 root         (0) root         (0)    24494 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/device-offline-cache.service.ts
+-rw-r--r--   0 root         (0) root         (0)     1553 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/device-status.service.ts
+-rw-r--r--   0 root         (0) root         (0)      356 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/gps-location.service.ts
+-rw-r--r--   0 root         (0) root         (0)      546 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/index.ts
+-rw-r--r--   0 root         (0) root         (0)      301 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.485934 peek-core-device-3.4.2/peek_core_device/plugin-module/tuples/
+-rw-r--r--   0 root         (0) root         (0)     1344 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/plugin-module/tuples/OfflineCacheLoaderStatusTuple.ts
+-rw-r--r--   0 root         (0) root         (0)     6342 2023-06-13 11:58:53.000000 peek-core-device-3.4.2/peek_core_device/plugin_package.json
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.485934 peek-core-device-3.4.2/peek_core_device/server/
+-rw-r--r--   0 root         (0) root         (0)     2404 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/server/DeviceApiABC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/server/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.486934 peek-core-device-3.4.2/peek_core_device/tuples/
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/tuples/DeviceDetailTuple.py
+-rw-r--r--   0 root         (0) root         (0)      494 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/tuples/DeviceGpsLocationTuple.py
+-rw-r--r--   0 root         (0) root         (0)     1479 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/tuples/DeviceInfoTuple.py
+-rw-r--r--   0 root         (0) root         (0)      814 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/tuples/DeviceStatusTuple.py
+-rw-r--r--   0 root         (0) root         (0)      344 2023-06-13 11:58:03.000000 peek-core-device-3.4.2/peek_core_device/tuples/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:58:53.476934 peek-core-device-3.4.2/peek_core_device.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      407 2023-06-13 11:58:53.000000 peek-core-device-3.4.2/peek_core_device.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    11609 2023-06-13 11:58:53.000000 peek-core-device-3.4.2/peek_core_device.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 11:58:53.000000 peek-core-device-3.4.2/peek_core_device.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       32 2023-06-13 11:58:53.000000 peek-core-device-3.4.2/peek_core_device.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-06-13 11:58:53.000000 peek-core-device-3.4.2/peek_core_device.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 11:58:53.487934 peek-core-device-3.4.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2547 2023-06-13 11:58:53.000000 peek-core-device-3.4.2/setup.py
```

### Comparing `peek-core-device-3.4.1/peek_core_device/__init__.py` & `peek-core-device-3.4.2/peek_core_device/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import Type
 
 from peek_plugin_base.client.PluginClientEntryHookABC import \
     PluginClientEntryHookABC
 from peek_plugin_base.server.PluginLogicEntryHookABC import \
     PluginLogicEntryHookABC
 
-__version__ = '3.4.1'
+__version__ = '3.4.2'
 
 
 def peekLogicEntryHook() -> Type[PluginLogicEntryHookABC]:
     from ._private.server.LogicEntryHook import LogicEntryHook
 
     return LogicEntryHook
```

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.html` & `peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.ts` & `peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-cache-status/device-cache-status.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-info-table/device-info.component.html` & `peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-info-table/device-info.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-info-table/device-info.component.ts` & `peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-info-table/device-info.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-update-table/device-update.component.html` & `peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-update-table/device-update.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/admin-app/device-update-table/device-update.component.ts` & `peek-core-device-3.4.2/peek_core_device/_private/admin-app/device-update-table/device-update.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/admin-app/device.component.html` & `peek-core-device-3.4.2/peek_core_device/_private/admin-app/device.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/admin-app/device.module.ts` & `peek-core-device-3.4.2/peek_core_device/_private/admin-app/device.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/admin-app/edit-setting-table/edit.component.html` & `peek-core-device-3.4.2/peek_core_device/_private/admin-app/edit-setting-table/edit.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/admin-app/edit-setting-table/edit.component.ts` & `peek-core-device-3.4.2/peek_core_device/_private/admin-app/edit-setting-table/edit.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/admin-app/tuples/DeviceCacheStatusTuple.ts` & `peek-core-device-3.4.2/peek_core_device/_private/admin-app/tuples/DeviceCacheStatusTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/admin-app/tuples/DeviceInfoTable.ts` & `peek-core-device-3.4.2/peek_core_device/_private/admin-app/tuples/DeviceInfoTable.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.html` & `peek-core-device-3.4.2/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.ts` & `peek-core-device-3.4.2/peek_core_device/_private/admin-app/upload-device-update/upload-device-update.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/alembic/script.py.mako` & `peek-core-device-3.4.2/peek_core_device/_private/alembic/script.py.mako`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/02f9305f9e7f_added_gps_tracking.py` & `peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/02f9305f9e7f_added_gps_tracking.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/2561b7732a6c_gps_devicetoken_on_cascade.py` & `peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/2561b7732a6c_gps_devicetoken_on_cascade.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/4b0d6309e556_add_offline_cache_enable.py` & `peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/4b0d6309e556_add_offline_cache_enable.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/5dd43ff7ea8e_added_filesize_to_update_tuple.py` & `peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/5dd43ff7ea8e_added_filesize_to_update_tuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/6bf6ecef3108_timezone_aware.py` & `peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/6bf6ecef3108_timezone_aware.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/7f628c121c4c_replaced_isonline_with_devicestatus.py` & `peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/7f628c121c4c_replaced_isonline_with_devicestatus.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/97d44e5aeb18_add_lastbandwidthmetric.py` & `peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/97d44e5aeb18_add_lastbandwidthmetric.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/alembic/versions/d94277dd8aca_initial_table_creation.py` & `peek-core-device-3.4.2/peek_core_device/_private/alembic/versions/d94277dd8aca_initial_table_creation.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-app/connect/connect.component.ts` & `peek-core-device-3.4.2/peek_core_device/_private/both-app/connect/connect.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-app/connect/connect.component.web.html` & `peek-core-device-3.4.2/peek_core_device/_private/both-app/connect/connect.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-app/connecting/connecting.component.ts` & `peek-core-device-3.4.2/peek_core_device/_private/both-app/connecting/connecting.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-app/connecting/connecting.component.web.html` & `peek-core-device-3.4.2/peek_core_device/_private/both-app/connecting/connecting.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-app/device.module.ts` & `peek-core-device-3.4.2/peek_core_device/_private/both-app/device.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-app/device.routes.ts` & `peek-core-device-3.4.2/peek_core_device/_private/both-app/device.routes.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-app/enroll/enroll.component.ts` & `peek-core-device-3.4.2/peek_core_device/_private/both-app/enroll/enroll.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-app/enroll/enroll.component.web.html` & `peek-core-device-3.4.2/peek_core_device/_private/both-app/enroll/enroll.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-app/enrolling/enrolling.component.ts` & `peek-core-device-3.4.2/peek_core_device/_private/both-app/enrolling/enrolling.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-app/enrolling/enrolling.component.web.html` & `peek-core-device-3.4.2/peek_core_device/_private/both-app/enrolling/enrolling.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-app/loading/loading.component.ts` & `peek-core-device-3.4.2/peek_core_device/_private/both-app/loading/loading.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-cfg/connect/connect.component.ts` & `peek-core-device-3.4.2/peek_core_device/_private/both-cfg/connect/connect.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-cfg/core-device-cfg.component.ts` & `peek-core-device-3.4.2/peek_core_device/_private/both-cfg/core-device-cfg.component.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-cfg/core-device-cfg.component.web.html` & `peek-core-device-3.4.2/peek_core_device/_private/both-cfg/core-device-cfg.component.web.html`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/both-cfg/core-device-cfg.module.ts` & `peek-core-device-3.4.2/peek_core_device/_private/both-cfg/core-device-cfg.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/client/ClientEntryHook.py` & `peek-core-device-3.4.2/peek_core_device/_private/client/ClientEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/client/DeviceTupleDataObservableProxy.py` & `peek-core-device-3.4.2/peek_core_device/_private/client/DeviceTupleDataObservableProxy.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/client/UpdateDownloadHandler.py` & `peek-core-device-3.4.2/peek_core_device/_private/client/UpdateDownloadHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/client/controllers/BandwidthTestController.py` & `peek-core-device-3.4.2/peek_core_device/_private/client/controllers/BandwidthTestController.py`

 * *Files 9% similar despite different names*

```diff
@@ -34,17 +34,19 @@
     def shutdown(self):
         if self._endpoint:
             self._endpoint.shutdown()
             self._endpoint = None
 
     @deferToThreadWrapWithLogger(logger)
     def _createTestData(self):
+        BASE64_SIZE = 1.3
+        PACKET_SIZE = int((100.0 * 1024.0) / BASE64_SIZE)
 
         testData = ""
-        while len(testData) < 100 * 1024:
+        while len(testData) < PACKET_SIZE:
             testData += str(random())
 
         logger.debug(f"Generated testData of size {len(testData)}")
 
         tuple_ = BandwidthTestTuple(testData=testData)
 
         self._vortexMsg = PayloadEnvelope(
```

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/client/controllers/DeviceOnlineController.py` & `peek-core-device-3.4.2/peek_core_device/_private/client/controllers/DeviceOnlineController.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/DeviceApi.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/DeviceApi.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/LogicEntryHook.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/LogicEntryHook.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/TupleActionProcessor.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/TupleActionProcessor.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/TupleDataObservable.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/TupleDataObservable.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from vortex.handler.TupleDataObservableHandler import TupleDataObservableHandler
-
 from peek_core_device._private.PluginNames import deviceFilt
 from peek_core_device._private.PluginNames import deviceObservableName
 from peek_core_device._private.server.controller.OfflineCacheController import (
     OfflineCacheController,
 )
 from peek_core_device._private.server.tuple_providers.ClientSettingsTupleProvider import (
     ClientSettingsTupleProvider,
@@ -29,27 +27,25 @@
 from peek_core_device._private.storage.DeviceInfoTable import DeviceInfoTable
 from peek_core_device._private.storage.DeviceUpdateTuple import (
     DeviceUpdateTuple,
 )
 from peek_core_device._private.tuples.ClientSettingsTuple import (
     ClientSettingsTuple,
 )
-from peek_core_device._private.tuples.DeviceCacheStatusTuple import (
-    DeviceCacheStatusTuple,
-)
 from peek_core_device._private.tuples.OfflineCacheCombinedStatusTuple import (
     OfflineCacheCombinedStatusTuple,
 )
 from peek_core_device._private.tuples.OfflineCacheSettingTuple import (
     OfflineCacheSettingTuple,
 )
 from peek_core_device.tuples.DeviceGpsLocationTuple import (
     DeviceGpsLocationTuple,
 )
 from peek_core_device.tuples.DeviceInfoTuple import DeviceInfoTuple
+from vortex.handler.TupleDataObservableHandler import TupleDataObservableHandler
 
 
 def makeTupleDataObservableHandler(
     ormSessionCreator, offlineCacheController: OfflineCacheController, userApi
 ):
     """ " Make Tuple Data Observable Handler
```

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/admin_backend/SettingPropertyHandler.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/admin_backend/SettingPropertyHandler.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/controller/BandwidthResultController.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/controller/BandwidthResultController.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/controller/DeviceStatusController.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/controller/DeviceStatusController.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/controller/EnrollmentController.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/controller/EnrollmentController.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/controller/GpsController.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/controller/GpsController.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/controller/MainController.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/controller/MainController.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/controller/NotifierController.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/controller/NotifierController.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/controller/OfflineCacheController.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/controller/OfflineCacheController.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/controller/UpdateController.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/controller/UpdateController.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/ClientSettingsTupleProvider.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/ClientSettingsTupleProvider.py`

 * *Files 17% similar despite different names*

```diff
@@ -10,14 +10,18 @@
 from peek_core_device._private.storage.Setting import FIELD_ENROLLMENT_ENABLED
 from peek_core_device._private.storage.Setting import OFFICE_ENROLLMENT_ENABLED
 from peek_core_device._private.storage.Setting import (
     OFFLINE_CACHE_REFRESH_SECONDS,
 )
 from peek_core_device._private.storage.Setting import (
     OFFLINE_MASTER_SWITCH_ENABLED,
+    CHECK_BANDWIDTH_SECONDS,
+    ABORT_RETRY_SECONDS,
+    PAUSE_TIMEOUT_SECONDS,
+    SEND_STATS_TO_SERVER_SECONDS,
 )
 from peek_core_device._private.storage.Setting import (
     SLOW_NETWORK_BANDWIDTH_METRIC_THRESHOLD,
 )
 from peek_core_device._private.storage.Setting import globalSetting
 from peek_core_device._private.tuples.ClientSettingsTuple import (
     ClientSettingsTuple,
@@ -30,15 +34,14 @@
     def __init__(self, ormSessionCreator):
         self._ormSessionCreator = ormSessionCreator
 
     @deferToThreadWrapWithLogger(logger)
     def makeVortexMsg(
         self, filt: dict, tupleSelector: TupleSelector
     ) -> Union[Deferred, bytes]:
-
         ormSession = self._ormSessionCreator()
         try:
             clientSetting = ClientSettingsTuple()
 
             clientSetting.fieldEnrollmentEnabled = globalSetting(
                 ormSession, FIELD_ENROLLMENT_ENABLED
             )
@@ -47,20 +50,38 @@
                 ormSession, OFFICE_ENROLLMENT_ENABLED
             )
 
             clientSetting.slowNetworkBandwidthMetricThreshold = globalSetting(
                 ormSession, SLOW_NETWORK_BANDWIDTH_METRIC_THRESHOLD
             )
 
+            clientSetting.offlineMasterSwitchEnabled = globalSetting(
+                ormSession, OFFLINE_MASTER_SWITCH_ENABLED
+            )
+
+            # Timers
+
             clientSetting.offlineCacheSyncSeconds = globalSetting(
                 ormSession, OFFLINE_CACHE_REFRESH_SECONDS
             )
 
-            clientSetting.offlineMasterSwitchEnabled = globalSetting(
-                ormSession, OFFLINE_MASTER_SWITCH_ENABLED
+            clientSetting.checkBandwidthSeconds = globalSetting(
+                ormSession, CHECK_BANDWIDTH_SECONDS
+            )
+
+            clientSetting.abortRetrySeconds = globalSetting(
+                ormSession, ABORT_RETRY_SECONDS
+            )
+
+            clientSetting.pauseTimeoutSeconds = globalSetting(
+                ormSession, PAUSE_TIMEOUT_SECONDS
+            )
+
+            clientSetting.sendStateToServerSeconds = globalSetting(
+                ormSession, SEND_STATS_TO_SERVER_SECONDS
             )
 
             # Create the vortex message
             return (
                 Payload(filt, tuples=[clientSetting])
                 .makePayloadEnvelope()
                 .toVortexMsg()
```

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/DeviceGpsLocationTupleProvider.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/DeviceGpsLocationTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/DeviceInfoTableTupleProvider.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/DeviceInfoTableTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/DeviceInfoTupleProvider.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/DeviceInfoTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/DeviceUpdateTupleProvider.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/DeviceUpdateTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/OfflineCacheCombinedStatusTupleProvider.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/OfflineCacheCombinedStatusTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/tuple_providers/OfflineCacheSettingTupleProvider.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/tuple_providers/OfflineCacheSettingTupleProvider.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/server/update_resources/DeviceUpdateUploadResource.py` & `peek-core-device-3.4.2/peek_core_device/_private/server/update_resources/DeviceUpdateUploadResource.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/storage/DeclarativeBase.py` & `peek-core-device-3.4.2/peek_core_device/_private/storage/DeclarativeBase.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/storage/DeviceInfoTable.py` & `peek-core-device-3.4.2/peek_core_device/_private/storage/DeviceInfoTable.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/storage/DeviceUpdateTuple.py` & `peek-core-device-3.4.2/peek_core_device/_private/storage/DeviceUpdateTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/storage/GpsLocationHistoryTable.py` & `peek-core-device-3.4.2/peek_core_device/_private/storage/GpsLocationHistoryTable.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/storage/GpsLocationTable.py` & `peek-core-device-3.4.2/peek_core_device/_private/storage/GpsLocationTable.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/storage/Setting.py` & `peek-core-device-3.4.2/peek_core_device/_private/storage/Setting.py`

 * *Files 4% similar despite different names*

```diff
@@ -279,21 +279,39 @@
     "Field Enrollment Enabled", True, propertyDict=globalProperties
 )
 
 OFFICE_ENROLLMENT_ENABLED = PropertyKey(
     "Office Enrollment Enabled", False, propertyDict=globalProperties
 )
 
-OFFLINE_CACHE_REFRESH_SECONDS = PropertyKey(
-    "Offline Cache Refresh Seconds", 24 * 60 * 60, propertyDict=globalProperties
-)
-
 OFFLINE_MASTER_SWITCH_ENABLED = PropertyKey(
     "Offline Master Switch Enabled", True, propertyDict=globalProperties
 )
 
 
 SLOW_NETWORK_BANDWIDTH_METRIC_THRESHOLD = PropertyKey(
     "Slow Network Bandwidth Metric Threshold",
     1200,
     propertyDict=globalProperties,
 )
+
+# Timers
+
+OFFLINE_CACHE_REFRESH_SECONDS = PropertyKey(
+    "Offline Cache Refresh Seconds", 24 * 60 * 60, propertyDict=globalProperties
+)
+
+CHECK_BANDWIDTH_SECONDS = PropertyKey(
+    "Check Bandwidth Seconds", 5 * 60, propertyDict=globalProperties
+)
+
+ABORT_RETRY_SECONDS = PropertyKey(
+    "Abort Retry Seconds", 15 * 60, propertyDict=globalProperties
+)
+
+PAUSE_TIMEOUT_SECONDS = PropertyKey(
+    "Pause Timeout Seconds", 60, propertyDict=globalProperties
+)
+
+SEND_STATS_TO_SERVER_SECONDS = PropertyKey(
+    "Send Stats To Server Seconds", 5 * 60, propertyDict=globalProperties
+)
```

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/tuples/AlterDeviceUpdateAction.py` & `peek-core-device-3.4.2/peek_core_device/_private/tuples/AlterDeviceUpdateAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/tuples/CreateDeviceUpdateAction.py` & `peek-core-device-3.4.2/peek_core_device/_private/tuples/CreateDeviceUpdateAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/tuples/DeviceCacheStatusTuple.py` & `peek-core-device-3.4.2/peek_core_device/_private/tuples/DeviceCacheStatusTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/tuples/OfflineCacheCombinedStatusTuple.py` & `peek-core-device-3.4.2/peek_core_device/_private/tuples/OfflineCacheCombinedStatusTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/tuples/OfflineCacheLoaderStatusTuple.py` & `peek-core-device-3.4.2/peek_core_device/_private/tuples/OfflineCacheLoaderStatusTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/tuples/OfflineCacheStatusAction.py` & `peek-core-device-3.4.2/peek_core_device/_private/tuples/OfflineCacheStatusAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/tuples/OfflineCacheStatusTuple.py` & `peek-core-device-3.4.2/peek_core_device/_private/tuples/OfflineCacheStatusTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/tuples/UpdateDeviceGpsLocationTupleAction.py` & `peek-core-device-3.4.2/peek_core_device/_private/tuples/UpdateDeviceGpsLocationTupleAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/tuples/UpdateDeviceOnlineAction.py` & `peek-core-device-3.4.2/peek_core_device/_private/tuples/UpdateDeviceOnlineAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/tuples/UpdateEnrollmentAction.py` & `peek-core-device-3.4.2/peek_core_device/_private/tuples/UpdateEnrollmentAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/tuples/UpdateOfflineCacheSettingAction.py` & `peek-core-device-3.4.2/peek_core_device/_private/tuples/UpdateOfflineCacheSettingAction.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/_private/tuples/WebClientVortexDetailsTuple.py` & `peek-core-device-3.4.2/peek_core_device/_private/tuples/WebClientVortexDetailsTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/admin-doc/admin_tasks/admin_task_devices.png` & `peek-core-device-3.4.2/peek_core_device/admin-doc/admin_tasks/admin_task_devices.png`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/admin-doc/admin_tasks/admin_tasks.rst` & `peek-core-device-3.4.2/peek_core_device/admin-doc/admin_tasks/admin_tasks.rst`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/admin-doc/admin_tasks/device_search.png` & `peek-core-device-3.4.2/peek_core_device/admin-doc/admin_tasks/device_search.png`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/admin-doc/admin_tasks/offline_cache_info.png` & `peek-core-device-3.4.2/peek_core_device/admin-doc/admin_tasks/offline_cache_info.png`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/admin-doc/general_settings/general_settings.png` & `peek-core-device-3.4.2/peek_core_device/admin-doc/general_settings/general_settings.png`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/admin-doc/general_settings/general_settings.rst` & `peek-core-device-3.4.2/peek_core_device/admin-doc/general_settings/general_settings.rst`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/admin-doc/overview.rst` & `peek-core-device-3.4.2/peek_core_device/admin-doc/overview.rst`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/both-doc/index.rst` & `peek-core-device-3.4.2/peek_core_device/both-doc/index.rst`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/DeviceGpsLocationTuple.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/DeviceGpsLocationTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/DeviceInfoTuple.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/DeviceInfoTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-background.service.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-background.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-bandwidth-test.service.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-bandwidth-test.service.ts`

 * *Files 8% similar despite different names*

```diff
@@ -30,21 +30,24 @@
 export class DeviceBandwidthTestService extends NgLifeCycleEvents {
     private bandwidthTestEndpoint: PayloadEndpoint;
     private unsubLastBandwidthTest = new Subject<void>();
 
     readonly RESPONSE_TIMEOUT_SECONDS = 30.0;
     private slowNetworkBandwidthMetricThreshold: number = 1200;
     private readonly CHECK_PERIOD_SECONDS = 15 * 60;
+    private readonly CHECK_BACKOFF_SECONDS = 5;
 
     private _isSlowNetwork: boolean = true;
     private _lastMetric: number = 1300;
 
     private _testRunning: boolean = false;
     private _lastNetworkType: string | null = null;
 
+    private _offlineCachingRunning: boolean = false;
+
     readonly status$ = new BehaviorSubject<BandwidthStatusI>({
         isSlowNetwork: null,
         lastMetric: null,
     });
 
     constructor(
         private vortexService: VortexService,
@@ -73,15 +76,16 @@
 
         interval(this.CHECK_PERIOD_SECONDS * 1000)
             .pipe(takeUntil(this.onDestroyEvent))
             .pipe(
                 filter(
                     () =>
                         this.vortexStatusService.snapshot.isOnline &&
-                        !this._testRunning
+                        !this._testRunning &&
+                        !this._offlineCachingRunning
                 )
             )
             .subscribe(() => this.startTest());
 
         const startTestShortly = () => {
             setTimeout(() => this.startTest(), 30 * 1000);
         };
@@ -107,14 +111,18 @@
         });
 
         // this service is constructed when the app starts,
         // check what our network is like, after all the subscriptions complete
         startTestShortly();
     }
 
+    setOfflineCachingRunning(value: boolean): void {
+        this._offlineCachingRunning = value;
+    }
+
     get isSlowNetwork(): boolean {
         return this._isSlowNetwork;
     }
 
     get lastMetric(): number {
         return this._lastMetric;
     }
@@ -124,21 +132,32 @@
     }
 
     startTest(): void {
         if (this._testRunning) {
             console.log("Subsequent call to start bandwidth test ignored");
             return;
         }
-        console.log("Starting bandwidth test ignored");
+        if (this._offlineCachingRunning) {
+            console.log(
+                "Offline cache test skipped while offline caching is" +
+                    " in progres"
+            );
+            return;
+        }
+        console.log("Starting bandwidth test");
 
         this._testRunning = true;
 
         this._performBandwidthTest()
             .catch((e) => console.log(`ERROR _performBandwidthTest: ${e}`))
-            .then(() => (this._testRunning = false));
+            .then(() => {
+                setTimeout(() => {
+                    this._testRunning = false;
+                }, this.CHECK_BACKOFF_SECONDS * 1000);
+            });
     }
 
     private _performBandwidthTest(): Promise<number | null> {
         if (this.enrolmentService.deviceInfo == null)
             throw new Error("We need a deviceInfo tuple set first");
 
         const startPoll = new Date().getTime();
@@ -184,14 +203,18 @@
 
             // Finally request the response
             this.vortexService.sendFilt(deviceBandwidthTestFilt);
         });
     }
 
     private applyBandwidthMetric(responseTimeMs: number | null) {
+        if (this._offlineCachingRunning) {
+            return;
+        }
+
         this._lastMetric = responseTimeMs;
 
         if (this.slowNetworkBandwidthMetricThreshold == null) {
             this._isSlowNetwork = true;
         } else if (responseTimeMs == null) {
             this._isSlowNetwork = true;
         } else {
```

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-loading.module.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-loading.module.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-nav.service.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-nav.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-online.service.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-online.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-server.service.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-server.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-tuple.service.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-tuple.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-update.service.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-update.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/device-update.service.web.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/device-update.service.web.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/gps/GpsLocationUpdateTupleAction.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/gps/GpsLocationUpdateTupleAction.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/gps/private-gps-location.service.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/gps/private-gps-location.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/hardware-info/hardware-info.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/hardware-info/hardware-info.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/index.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/index.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/ClientSettingsTuple.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/ClientSettingsTuple.ts`

 * *Files 21% similar despite different names*

```diff
@@ -6,14 +6,19 @@
     // The tuple name here should end in "Tuple" as well, but it doesn't, as it's a table
     public static readonly tupleName =
         deviceTuplePrefix + "ClientSettingsTuple";
 
     fieldEnrollmentEnabled: boolean;
     officeEnrollmentEnabled: boolean;
     slowNetworkBandwidthMetricThreshold: number;
-    offlineCacheSyncSeconds: number = 0;
     offlineMasterSwitchEnabled: boolean;
 
+    offlineCacheSyncSeconds: number = 0;
+    checkBandwidthSeconds: number = 0;
+    abortRetrySeconds: number = 0;
+    pauseTimeoutSeconds: number = 0;
+    sendStateToServerSeconds: number = 0;
+
     constructor() {
         super(ClientSettingsTuple.tupleName);
     }
 }
```

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/DeviceUpdateLocalValuesTuple.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/DeviceUpdateLocalValuesTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/DeviceUpdateTuple.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/DeviceUpdateTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/OfflineCacheCombinedStatusTuple.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/OfflineCacheCombinedStatusTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/OfflineCacheStatusTuple.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/OfflineCacheStatusTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/UpdateDeviceOnlineAction.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/UpdateDeviceOnlineAction.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/admin/AlterDeviceUpdateAction.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/admin/AlterDeviceUpdateAction.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/admin/SettingPropertyTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/_private/tuples/server-info-tuple.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/_private/tuples/server-info-tuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/device-enrolled.guard.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/device-enrolled.guard.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/device-enrolment.service.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/device-enrolment.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/device-offline-cache.service.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/device-offline-cache.service.ts`

 * *Files 6% similar despite different names*

```diff
@@ -22,16 +22,17 @@
 } from "./_private/tuples/OfflineCacheStatusTuple";
 import { OfflineCacheStatusAction } from "./_private/tuples/OfflineCacheStatusAction";
 import { OfflineCacheCombinedStatusTuple } from "@peek/peek_core_device/_private/tuples/OfflineCacheCombinedStatusTuple";
 
 class Timer {
     private _startTime: Date;
 
-    constructor(private timeoutSeconds: number) {
-        this.reset();
+    // Default to a year, it will never time out
+    constructor(private timeoutSeconds: number = 365 * 24 * 60 * 68) {
+        this._startTime = new Date();
     }
 
     get expired(): boolean {
         return (
             this._startTime.getTime() + this.timeoutSeconds * 1000 <
             new Date().getTime()
         );
@@ -107,31 +108,29 @@
     private settings: OfflineCacheSettingTuple | null = null;
     private allCientsSettingsTuple: ClientSettingsTuple | null = null;
     private deviceInfo: DeviceInfoTuple = new DeviceInfoTuple();
 
     private unsub = new Subject<void>();
 
     // Check the bandwidth every 5 minutes
-    private readonly checkBandwidthTimer = new Timer(5 * 60);
+    private readonly checkBandwidthTimer = new Timer();
 
     // Check the bandwidth every 15 minutes
     // This assumes the field device is transitioning through bad internet
     // If they turn on their wifi, we're in for a predicament.
-    private readonly abortRetryTimer = new Timer(15 * 60);
+    private readonly abortRetryTimer = new Timer();
 
     // Give loaders 60 seconds to pause
-    private readonly pauseTimeoutTimer = new Timer(60);
+    private readonly pauseTimeoutTimer = new Timer();
 
     // This will be reinitialised when the settings come from the server
-    private readonly scheduledNextCacheStartTimer = new Timer(24 * 60 * 60);
+    private readonly scheduledNextCacheStartTimer = new Timer();
 
     // Run every 2 to 5 minutes, so we don't overload the server
-    private readonly sendStateToServerTimer = new Timer(
-        2 * 60 + Math.floor(Math.random() * 3 * 60)
-    );
+    private readonly sendStateToServerTimer = new Timer();
 
     // Make note of the last network type
     private _lastNetworkType = "";
 
     constructor(
         private vortexService: VortexService,
         private vortexStatusService: VortexStatusService,
@@ -176,19 +175,39 @@
         // noinspection TypeScriptValidateJSTypes
         this.tupleService.offlineObserver
             .subscribeToTupleSelector(ts)
             .pipe(takeUntil(this.onDestroyEvent))
             .subscribe((settings: ClientSettingsTuple[]) => {
                 if (settings.length !== 0) {
                     this.allCientsSettingsTuple = settings[0];
+                    this.setupTimersFromSettings();
                     this.processStateLoaded();
                 }
             });
     }
 
+    private setupTimersFromSettings(): void {
+        this.sendStateToServerTimer.setTimeout(
+            this.allCientsSettingsTuple.sendStateToServerSeconds +
+                Math.floor(Math.random() * 5 * 60) // Add some randomness
+        );
+        this.scheduledNextCacheStartTimer.setTimeout(
+            this.allCientsSettingsTuple.offlineCacheSyncSeconds
+        );
+        this.checkBandwidthTimer.setTimeout(
+            this.allCientsSettingsTuple.checkBandwidthSeconds
+        );
+        this.pauseTimeoutTimer.setTimeout(
+            this.allCientsSettingsTuple.pauseTimeoutSeconds
+        );
+        this.abortRetryTimer.setTimeout(
+            this.allCientsSettingsTuple.abortRetrySeconds
+        );
+    }
+
     private setupThisDeviceOfflineSettingsSubscription() {
         this.unsub.next();
 
         const offlineSettingTs = new TupleSelector(
             OfflineCacheSettingTuple.tupleName,
             { deviceToken: this.deviceInfo.deviceToken }
         );
@@ -276,15 +295,14 @@
     }
 
     private sendStateToServer(force: boolean = false) {
         this._status$.next(this.status);
 
         if (!force && !this.sendStateToServerTimer.expired) return;
         if (!this.vortexStatusService.snapshot.isOnline) return;
-
         this.sendStateToServerTimer.reset();
 
         const combinedTuple = new OfflineCacheCombinedStatusTuple();
         combinedTuple.deviceToken = this.deviceInfo.deviceToken;
         combinedTuple.loaderStatusList = this._loaderCachingStatusList;
         combinedTuple.offlineCacheStatus = this.status;
 
@@ -297,22 +315,34 @@
                 action.lastCachingStartDate = this.status.lastCachingStartDate;
                 return this.tupleService.tupleAction.pushAction(action);
             })
             .then(() => console.log("Offline cache status sent successfully"))
             .catch((e) => console.log(`ERROR: ${e}`));
     }
 
+    private get isRunning(): boolean {
+        return (
+            this.status.state === StateMachineE.StartRunning ||
+            this.status.state === StateMachineE.Running ||
+            this.status.state === StateMachineE.StartPausing ||
+            this.status.state === StateMachineE.Pausing
+        );
+    }
+
     private runStateMachine(): void {
         if (this.stateMachineLock.isLocked) return;
 
         this.stateMachineLock.lock();
         // console.log(`StateMachine Start = ${this.status.stateString}`);
         this.tryRunStateMachine() //
             .catch((e) => console.log(`ERROR asyncStateMachine: ${e}`))
             .then(() => {
+                this.deviceBandwidthTestService.setOfflineCachingRunning(
+                    this.isRunning
+                );
                 // console.log(`StateMachine End = ${this.status.stateString}`);
 
                 setTimeout(() => {
                     try {
                         // Don't unlock it until we're going to run next
                         this.stateMachineLock.unlock();
                         if (this.status.state === StateMachineE.Disabled)
@@ -342,17 +372,14 @@
                 return;
             }
             case StateMachineE.Disabled: {
                 // Do nothing, The state machine shouldn't be running
                 return;
             }
             case StateMachineE.ScheduleNextRun: {
-                this.scheduledNextCacheStartTimer.setTimeout(
-                    this.allCientsSettingsTuple.offlineCacheSyncSeconds
-                );
                 // Ensure the caching does not start before it's due to.
                 if (this.status.lastCachingStartDate != null) {
                     this.scheduledNextCacheStartTimer.reset(
                         this.status.lastCachingStartDate
                     );
                 }
                 this.status.state = StateMachineE.Enabled;
```

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/device-status.service.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/device-status.service.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/index.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/index.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin-module/tuples/OfflineCacheLoaderStatusTuple.ts` & `peek-core-device-3.4.2/peek_core_device/plugin-module/tuples/OfflineCacheLoaderStatusTuple.ts`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/plugin_package.json` & `peek-core-device-3.4.2/peek_core_device/plugin_package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9964285714285716%*

 * *Differences: {"'plugin'": "{'version': '3.4.2'}"}*

```diff
@@ -179,15 +179,15 @@
     },
     "plugin": {
         "buildDate": "#BUILD_DATE#",
         "buildNumber": "#PLUGIN_BUILD#",
         "creator": "Synerty Pty Ltd",
         "packageName": "peek_core_device",
         "title": "Device",
-        "version": "3.4.1",
+        "version": "3.4.2",
         "website": "www.synerty.com"
     },
     "requiresServices": [
         "logic",
         "storage",
         "admin",
         "field",
```

### Comparing `peek-core-device-3.4.1/peek_core_device/server/DeviceApiABC.py` & `peek-core-device-3.4.2/peek_core_device/server/DeviceApiABC.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/tuples/DeviceDetailTuple.py` & `peek-core-device-3.4.2/peek_core_device/tuples/DeviceDetailTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/tuples/DeviceInfoTuple.py` & `peek-core-device-3.4.2/peek_core_device/tuples/DeviceInfoTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device/tuples/DeviceStatusTuple.py` & `peek-core-device-3.4.2/peek_core_device/tuples/DeviceStatusTuple.py`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/peek_core_device.egg-info/SOURCES.txt` & `peek-core-device-3.4.2/peek_core_device.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `peek-core-device-3.4.1/setup.py` & `peek-core-device-3.4.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 #
 # Modify these values to fork a new plugin
 #
 author = "Synerty"
 author_email = "contact@synerty.com"
 py_package_name = "peek_core_device"
 pip_package_name = py_package_name.replace("_", "-")
-package_version = "3.4.1"
+package_version = "3.4.2"
 description = "Peek Core Device - Device management for the peek platform."
 
 download_url = "https://bitbucket.org/synerty/%s/get/%s.zip"
 download_url %= pip_package_name, package_version
 url = "https://bitbucket.org/synerty/%s" % pip_package_name
 
 #
```

