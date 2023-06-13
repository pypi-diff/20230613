# Comparing `tmp/resotocore-3.5.1.tar.gz` & `tmp/resotocore-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotocore-3.5.1.tar", last modified: Fri Jun  2 14:51:40 2023, max compression
+gzip compressed data, was "resotocore-3.5.2.tar", last modified: Tue Jun 13 13:07:15 2023, max compression
```

## Comparing `resotocore-3.5.1.tar` & `resotocore-3.5.2.tar`

### file list

```diff
@@ -1,804 +1,804 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.436593 resotocore-3.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-02 14:47:48.000000 resotocore-3.5.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-02 14:47:48.000000 resotocore-3.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-06-02 14:51:40.436593 resotocore-3.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-02 14:47:48.000000 resotocore-3.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-02 14:47:48.000000 resotocore-3.5.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.340592 resotocore-3.5.1/resotocore/
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12530 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.340592 resotocore-3.5.1/resotocore/action_handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/action_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/action_handlers/merge_outer_edge_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.340592 resotocore-3.5.1/resotocore/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/analytics/posthog.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/analytics/recurrent_events.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/async_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.344592 resotocore-3.5.1/resotocore/cli/
--rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    27773 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)   226544 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/cli/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)    24074 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/cli/tip_of_the_day.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.344592 resotocore-3.5.1/resotocore/config/
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/config/config_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/config/config_override_service.py
--rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/config/core_config_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/console_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    36431 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/core_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.344592 resotocore-3.5.1/resotocore/db/
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    32045 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/arango_query.py
--rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/arangodb_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/arangodb_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/async_arangodb.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/configdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/db_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/deferred_edge_db.py
--rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (123)    64016 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/graphdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/jobdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/model.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/modeldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/packagedb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/runningtaskdb.py
--rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/subscriberdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/system_data_db.py
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/db/templatedb.py
--rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/error.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.344592 resotocore-3.5.1/resotocore/graph_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/graph_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14670 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/graph_manager/graph_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/ids.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.348592 resotocore-3.5.1/resotocore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/infra_apps/local_runtime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/infra_apps/manifest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13400 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/infra_apps/package_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/infra_apps/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.348592 resotocore-3.5.1/resotocore/jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.316592 resotocore-3.5.1/resotocore/jupyterlite/api/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.348592 resotocore-3.5.1/resotocore/jupyterlite/api/contents/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-02 14:51:36.000000 resotocore-3.5.1/resotocore/jupyterlite/api/contents/all.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.348592 resotocore-3.5.1/resotocore/jupyterlite/api/translations/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-02 14:51:36.000000 resotocore-3.5.1/resotocore/jupyterlite/api/translations/all.json
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-02 14:51:36.000000 resotocore-3.5.1/resotocore/jupyterlite/api/translations/en.json
--rw-r--r--   0 runner    (1001) docker     (123)     3223 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/bootstrap.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.400593 resotocore-3.5.1/resotocore/jupyterlite/build/
--rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1037.51967a2.js
--rw-r--r--   0 runner    (1001) docker     (123)    21710 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1079.cdbaf67.js
--rw-r--r--   0 runner    (1001) docker     (123)     9647 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1084.4cd1c89.js
--rw-r--r--   0 runner    (1001) docker     (123)     1950 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1113.23c9417.js
--rw-r--r--   0 runner    (1001) docker     (123)     9736 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1125.129d070.js
--rw-r--r--   0 runner    (1001) docker     (123)     9342 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1163.ac28297.js
--rw-r--r--   0 runner    (1001) docker     (123)    74541 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1221.c51249a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1245.be46619.js
--rw-r--r--   0 runner    (1001) docker     (123)     9525 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1261.199fc1d.js
--rw-r--r--   0 runner    (1001) docker     (123)    10027 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1272.f334098.js
--rw-r--r--   0 runner    (1001) docker     (123)    14792 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1278.0524a4a.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1290.3981211.js
--rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1295.46e72b8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3404 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1310.23bbe67.js
--rw-r--r--   0 runner    (1001) docker     (123)    10986 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1320.21effe3.js
--rw-r--r--   0 runner    (1001) docker     (123)     6216 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1325.f76267c.js
--rw-r--r--   0 runner    (1001) docker     (123)     7061 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1408.7461890.js
--rw-r--r--   0 runner    (1001) docker     (123)     2273 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1440.a9e7ea1.js
--rw-r--r--   0 runner    (1001) docker     (123)    23820 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1483.616d9ab.js
--rw-r--r--   0 runner    (1001) docker     (123)    47542 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1489.e50b6d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2605 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1507.5705605.js
--rw-r--r--   0 runner    (1001) docker     (123)      624 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/152.525d460.js
--rw-r--r--   0 runner    (1001) docker     (123)    36869 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1520.4e2eb21.js
--rw-r--r--   0 runner    (1001) docker     (123)     1533 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1555.e188f3f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8584 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1559.7c89925.js
--rw-r--r--   0 runner    (1001) docker     (123)     9056 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/160.5f28731.js
--rw-r--r--   0 runner    (1001) docker     (123)   478144 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1603.370a2a6.js
--rw-r--r--   0 runner    (1001) docker     (123)    22415 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1644.0e49167.js
--rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1667.f0afb2b.js
--rw-r--r--   0 runner    (1001) docker     (123)    17330 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1687.27f1ad6.js
--rw-r--r--   0 runner    (1001) docker     (123)   272197 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1725.f151c33.js
--rw-r--r--   0 runner    (1001) docker     (123)    25316 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1767.c8c2f26.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1806.1aaf66b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1838.1202b16.js
--rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1909.28a2def.js
--rw-r--r--   0 runner    (1001) docker     (123)     9485 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/1989.88d258f.js
--rw-r--r--   0 runner    (1001) docker     (123)    89976 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2030.1562cc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     6343 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2047.baed97b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2099.f4b6fcd.js
--rw-r--r--   0 runner    (1001) docker     (123)     6160 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2118.5b65f70.js
--rw-r--r--   0 runner    (1001) docker     (123)     3149 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/213.5769e57.js
--rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2161.dcb27b8.js
--rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2169.635c88e.js
--rw-r--r--   0 runner    (1001) docker     (123)    17630 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/217.90d10e2.js
--rw-r--r--   0 runner    (1001) docker     (123)    35022 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2212.72be094.js
--rw-r--r--   0 runner    (1001) docker     (123)   123689 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2287.997c38e.js
--rw-r--r--   0 runner    (1001) docker     (123)      545 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2303.9ff8710.js
--rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2319.6b4cbb7.js
--rw-r--r--   0 runner    (1001) docker     (123)     2648 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2329.4c5ca6d.js
--rw-r--r--   0 runner    (1001) docker     (123)     8667 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2351.fbd96d8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2358.d5cf7c8.js
--rw-r--r--   0 runner    (1001) docker     (123)     7913 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2359.6451c3e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9289 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/237.f765e77.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2384.71782be.js
--rw-r--r--   0 runner    (1001) docker     (123)     4763 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/240.cddc46b.js
--rw-r--r--   0 runner    (1001) docker     (123)    15476 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2431.648d237.js
--rw-r--r--   0 runner    (1001) docker     (123)    12395 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2546.1f48267.js
--rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2557.75e9da2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4176 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/261.5f53c0e.js
--rw-r--r--   0 runner    (1001) docker     (123)     8923 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2629.c0e1cd6.js
--rw-r--r--   0 runner    (1001) docker     (123)     2328 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2788.46acc8a.js
--rw-r--r--   0 runner    (1001) docker     (123)     8591 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2834.942acc6.js
--rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2887.47ba752.js
--rw-r--r--   0 runner    (1001) docker     (123)     8870 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2956.8880209.js
--rw-r--r--   0 runner    (1001) docker     (123)     4300 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/2973.2a51dc4.js
--rw-r--r--   0 runner    (1001) docker     (123)     8060 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3004.255e79c.js
--rw-r--r--   0 runner    (1001) docker     (123)    17042 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/302.8bcc38f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8560 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3037.70ee38d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3042.7cfad84.js
--rw-r--r--   0 runner    (1001) docker     (123)    10136 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3051.34fac68.js
--rw-r--r--   0 runner    (1001) docker     (123)     9664 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3122.2289fca.js
--rw-r--r--   0 runner    (1001) docker     (123)     2550 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3151.10ef4de.js
--rw-r--r--   0 runner    (1001) docker     (123)    15850 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/316.c850a76.js
--rw-r--r--   0 runner    (1001) docker     (123)    20975 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3196.4e35a17.js
--rw-r--r--   0 runner    (1001) docker     (123)    16159 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3265.a80440a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3277.9c04e75.js
--rw-r--r--   0 runner    (1001) docker     (123)     8847 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/330.126fa98.js
--rw-r--r--   0 runner    (1001) docker     (123)    14007 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3392.29fe6b9.js
--rw-r--r--   0 runner    (1001) docker     (123)    80815 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3413.480a49d.js
--rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3444.47d5ea1.js
--rw-r--r--   0 runner    (1001) docker     (123)     1863 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3469.7d14d0b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9554 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3546.fee1bd7.js
--rw-r--r--   0 runner    (1001) docker     (123)     5145 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/362.6716970.js
--rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3708.410d087.js
--rw-r--r--   0 runner    (1001) docker     (123)      170 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3752.8735345.js
--rw-r--r--   0 runner    (1001) docker     (123)    16215 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3850.903abc2.js
--rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3433 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3880.bd39dce.js
--rw-r--r--   0 runner    (1001) docker     (123)    10216 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3970.236586f.js
--rw-r--r--   0 runner    (1001) docker     (123)   897822 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3976.58893b9.js
--rw-r--r--   0 runner    (1001) docker     (123)     2025 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16446 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/3979.385527e.js
--rw-r--r--   0 runner    (1001) docker     (123)    11331 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/400.d72234b.js
--rw-r--r--   0 runner    (1001) docker     (123)    11916 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4018.1a35967.js
--rw-r--r--   0 runner    (1001) docker     (123)     9851 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/406.9b7af92.js
--rw-r--r--   0 runner    (1001) docker     (123)    11111 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4117.a8107fd.js
--rw-r--r--   0 runner    (1001) docker     (123)    10886 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4182.e2430f9.js
--rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4191.02bbea8.js
--rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4197.53ab10b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9224 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4206.a5f8bb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     8525 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4207.0d0580b.js
--rw-r--r--   0 runner    (1001) docker     (123)    10616 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4262.bb73457.js
--rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4298.5ee510c.js
--rw-r--r--   0 runner    (1001) docker     (123)    83844 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/44.0cfa785.js
--rw-r--r--   0 runner    (1001) docker     (123)     1021 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4410.e4a25d3.js
--rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4466.64d23d1.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4507.8b41ef4.js
--rw-r--r--   0 runner    (1001) docker     (123)     7852 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/451.d9683ad.js
--rw-r--r--   0 runner    (1001) docker     (123)     2977 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4535.34b060a.js
--rw-r--r--   0 runner    (1001) docker     (123)    20495 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4565.43bdb91.js
--rw-r--r--   0 runner    (1001) docker     (123)    22220 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4569.f374f9d.js
--rw-r--r--   0 runner    (1001) docker     (123)    91604 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4615.eb5d40a.js
--rw-r--r--   0 runner    (1001) docker     (123)   119541 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4658.090d4a9.js
--rw-r--r--   0 runner    (1001) docker     (123)       95 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4658.090d4a9.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      356 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4665.aa19a41.js
--rw-r--r--   0 runner    (1001) docker     (123)      142 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4668.f65690b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4695 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4690.3dd4096.js
--rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4715.e7690b9.js
--rw-r--r--   0 runner    (1001) docker     (123)    10282 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4749.46ebbb2.js
--rw-r--r--   0 runner    (1001) docker     (123)     9653 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4750.56c06ab.js
--rw-r--r--   0 runner    (1001) docker     (123)    17648 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4856.2d7415f.js
--rw-r--r--   0 runner    (1001) docker     (123)    41909 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4875.375150e.js
--rw-r--r--   0 runner    (1001) docker     (123)     6350 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/489.b981dea.js
--rw-r--r--   0 runner    (1001) docker     (123)     2209 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/490.c2624d4.js
--rw-r--r--   0 runner    (1001) docker     (123)     2796 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4905.667bf33.js
--rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4931.430433b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/4942.b96c164.js
--rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5016.dd2fe83.js
--rw-r--r--   0 runner    (1001) docker     (123)     5766 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5072.733a1b5.js
--rw-r--r--   0 runner    (1001) docker     (123)     2604 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/509.6448878.js
--rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5096.8ed0d8e.js
--rw-r--r--   0 runner    (1001) docker     (123)     4581 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5126.eecad7a.js
--rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5129.1ba4763.js
--rw-r--r--   0 runner    (1001) docker     (123)     6272 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5153.763d8fa.js
--rw-r--r--   0 runner    (1001) docker     (123)      618 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5155.06b4ea9.js
--rw-r--r--   0 runner    (1001) docker     (123)    32726 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5193.e9f6866.js
--rw-r--r--   0 runner    (1001) docker     (123)     9808 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5213.3e1a360.js
--rw-r--r--   0 runner    (1001) docker     (123)     8503 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5227.8c8acd8.js
--rw-r--r--   0 runner    (1001) docker     (123)    11129 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5238.1751cc3.js
--rw-r--r--   0 runner    (1001) docker     (123)     5579 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/528.2262cb0.js
--rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5292.79d4aba.js
--rw-r--r--   0 runner    (1001) docker     (123)     7706 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5437.31236f7.js
--rw-r--r--   0 runner    (1001) docker     (123)    10580 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5489.848a8cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     5146 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5508.317fca3.js
--rw-r--r--   0 runner    (1001) docker     (123)     9068 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/554.ac98303.js
--rw-r--r--   0 runner    (1001) docker     (123)     2549 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/555.2cd31dd.js
--rw-r--r--   0 runner    (1001) docker     (123)    16702 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5573.ebcdb93.js
--rw-r--r--   0 runner    (1001) docker     (123)   171864 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5666.c5e5324.js
--rw-r--r--   0 runner    (1001) docker     (123)     8628 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5710.70d0b1d.js
--rw-r--r--   0 runner    (1001) docker     (123)   172015 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5747.94ad626.js
--rw-r--r--   0 runner    (1001) docker     (123)    14074 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/582.21b8e7d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5823.5045bdb.js
--rw-r--r--   0 runner    (1001) docker     (123)     2543 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5851.30b7b2a.js
--rw-r--r--   0 runner    (1001) docker     (123)   257877 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5878.32d92fa.js
--rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5880.68f975b.js
--rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5955.88508f7.js
--rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/5971.88c5642.js
--rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6080.aa0ff24.js
--rw-r--r--   0 runner    (1001) docker     (123)    28010 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/61.2808a0d.js
--rw-r--r--   0 runner    (1001) docker     (123)    18045 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6136.b8ba2b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     1343 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6141.9831d58.js
--rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6475.6037fbb.js
--rw-r--r--   0 runner    (1001) docker     (123)     7434 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6493.d796aa5.js
--rw-r--r--   0 runner    (1001) docker     (123)     4963 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6556.b3d9293.js
--rw-r--r--   0 runner    (1001) docker     (123)     5803 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6571.2c8884e.js
--rw-r--r--   0 runner    (1001) docker     (123)    10586 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6576.3ea568e.js
--rw-r--r--   0 runner    (1001) docker     (123)    83397 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6591.94ed352.js
--rw-r--r--   0 runner    (1001) docker     (123)     7388 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6612.1632879.js
--rw-r--r--   0 runner    (1001) docker     (123)   246379 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6623.ae3b3cc.js
--rw-r--r--   0 runner    (1001) docker     (123)      160 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6623.ae3b3cc.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    16150 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6664.2160109.js
--rw-r--r--   0 runner    (1001) docker     (123)     9611 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6747.47be7f5.js
--rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6748.be68f5f.js
--rw-r--r--   0 runner    (1001) docker     (123)     8961 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6870.7940288.js
--rw-r--r--   0 runner    (1001) docker     (123)    11058 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6879.c8367a5.js
--rw-r--r--   0 runner    (1001) docker     (123)    16507 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6898.9bbc12a.js
--rw-r--r--   0 runner    (1001) docker     (123)    10256 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6952.f68b818.js
--rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6985.321ad92.js
--rw-r--r--   0 runner    (1001) docker     (123)    10925 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6993.32cf9a6.js
--rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/6997.b06fe71.js
--rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7041.d4f561e.js
--rw-r--r--   0 runner    (1001) docker     (123)    10338 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7058.805c88e.js
--rw-r--r--   0 runner    (1001) docker     (123)       51 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7058.805c88e.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7174.6c45206.js
--rw-r--r--   0 runner    (1001) docker     (123)    35260 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7334.8859b1b.js
--rw-r--r--   0 runner    (1001) docker     (123)     8497 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7359.6ee65ec.js
--rw-r--r--   0 runner    (1001) docker     (123)     3555 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7364.195178b.js
--rw-r--r--   0 runner    (1001) docker     (123)     9117 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7380.58a4413.js
--rw-r--r--   0 runner    (1001) docker     (123)     7126 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7427.f9c2017.js
--rw-r--r--   0 runner    (1001) docker     (123)      294 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7427.f9c2017.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)    14994 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7463.18fd278.js
--rw-r--r--   0 runner    (1001) docker     (123)    10358 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7509.1e0189e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7526.1a303e5.js
--rw-r--r--   0 runner    (1001) docker     (123)    31492 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7537.1323a15.js
--rw-r--r--   0 runner    (1001) docker     (123)    10078 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7692.33d5169.js
--rw-r--r--   0 runner    (1001) docker     (123)      595 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7746.5908d29.js
--rw-r--r--   0 runner    (1001) docker     (123)    10754 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7808.1d582a2.js
--rw-r--r--   0 runner    (1001) docker     (123)     4962 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/783.c156751.js
--rw-r--r--   0 runner    (1001) docker     (123)     9192 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7858.2386e4d.js
--rw-r--r--   0 runner    (1001) docker     (123)    31628 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/7941.01ea680.js
--rw-r--r--   0 runner    (1001) docker     (123)     5753 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8005.c5ad7b2.js
--rw-r--r--   0 runner    (1001) docker     (123)     7966 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8028.39e2fa1.js
--rw-r--r--   0 runner    (1001) docker     (123)     9977 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8061.cc62561.js
--rw-r--r--   0 runner    (1001) docker     (123)   317511 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8101.cf46d02.js
--rw-r--r--   0 runner    (1001) docker     (123)       50 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8101.cf46d02.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7965 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/812.9b0e86e.js
--rw-r--r--   0 runner    (1001) docker     (123)      855 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/816.c8050f2.js
--rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8165.b2c3285.js
--rw-r--r--   0 runner    (1001) docker     (123)     3150 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8232.a578bf9.js
--rw-r--r--   0 runner    (1001) docker     (123)     1142 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/824.8678196.js
--rw-r--r--   0 runner    (1001) docker     (123)    15838 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8270.89fe7e1.js
--rw-r--r--   0 runner    (1001) docker     (123)     2327 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/833.9cc6653.js
--rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8370.8f855e5.js
--rw-r--r--   0 runner    (1001) docker     (123)    10481 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8373.96b0b3a.js
--rw-r--r--   0 runner    (1001) docker     (123)     2921 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8389.ffe031f.js
--rw-r--r--   0 runner    (1001) docker     (123)     6825 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8412.1528057.js
--rw-r--r--   0 runner    (1001) docker     (123)     9361 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8427.4923f43.js
--rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8542.027afdc.js
--rw-r--r--   0 runner    (1001) docker     (123)     8843 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8594.0112f03.js
--rw-r--r--   0 runner    (1001) docker     (123)    30005 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8656.d5b8e92.js
--rw-r--r--   0 runner    (1001) docker     (123)    12065 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8685.d78bdab.js
--rw-r--r--   0 runner    (1001) docker     (123)   114157 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8698.9817d75.js
--rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8732.9320f73.js
--rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8741.b138cb8.js
--rw-r--r--   0 runner    (1001) docker     (123)     2572 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8785.cf4fe95.js
--rw-r--r--   0 runner    (1001) docker     (123)    27799 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8828.77c71d0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2950 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8883.80c7b63.js
--rw-r--r--   0 runner    (1001) docker     (123)     9758 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8976.3816942.js
--rw-r--r--   0 runner    (1001) docker     (123)      432 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8981.99a4275.js
--rw-r--r--   0 runner    (1001) docker     (123)     1931 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/8990.2a453cf.js
--rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9035.1e45c1b.js
--rw-r--r--   0 runner    (1001) docker     (123)     4177 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9053.45b77fc.js
--rw-r--r--   0 runner    (1001) docker     (123)     9689 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9077.fefb6ca.js
--rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9128.b8fa6f0.js
--rw-r--r--   0 runner    (1001) docker     (123)     9225 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9156.0cefbd3.js
--rw-r--r--   0 runner    (1001) docker     (123)     2790 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9170.0023587.js
--rw-r--r--   0 runner    (1001) docker     (123)    10649 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9196.315f9f9.js
--rw-r--r--   0 runner    (1001) docker     (123)    28388 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9198.9971d70.js
--rw-r--r--   0 runner    (1001) docker     (123)   131443 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/920.d15c177.js
--rw-r--r--   0 runner    (1001) docker     (123)     4000 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9253.0b31caa.js
--rw-r--r--   0 runner    (1001) docker     (123)     8378 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9266.bacd0dd.js
--rw-r--r--   0 runner    (1001) docker     (123)      591 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9307.c3a00ed.js
--rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9321.869e413.js
--rw-r--r--   0 runner    (1001) docker     (123)  1188430 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9344.ba0abcf.js
--rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9382.9014799.js
--rw-r--r--   0 runner    (1001) docker     (123)    29226 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9440.1b10b8f.js
--rw-r--r--   0 runner    (1001) docker     (123)      163 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9440.1b10b8f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9464.79e6ac5.js
--rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9502.9a24831.js
--rw-r--r--   0 runner    (1001) docker     (123)    32420 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9507.1e6cc5d.js
--rw-r--r--   0 runner    (1001) docker     (123)     9206 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9602.62bf0f1.js
--rw-r--r--   0 runner    (1001) docker     (123)     9381 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9621.e2e8b5d.js
--rw-r--r--   0 runner    (1001) docker     (123)      625 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9622.ccab065.js
--rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9626.a178bd0.js
--rw-r--r--   0 runner    (1001) docker     (123)    10559 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9647.ed91993.js
--rw-r--r--   0 runner    (1001) docker     (123)   432928 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9657.bc5c60e.js
--rw-r--r--   0 runner    (1001) docker     (123)     9073 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/97.ad126b0.js
--rw-r--r--   0 runner    (1001) docker     (123)     2515 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9712.796a0a1.js
--rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9733.a3b2a7f.js
--rw-r--r--   0 runner    (1001) docker     (123)    36791 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9737.7dc8f98.js
--rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9777.0b8a504.js
--rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9793.6d63a85.js
--rw-r--r--   0 runner    (1001) docker     (123)    17595 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9806.652c162.js
--rw-r--r--   0 runner    (1001) docker     (123)   179318 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9865.2e3db6f.js
--rw-r--r--   0 runner    (1001) docker     (123)      246 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9865.2e3db6f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4299 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/989.bcca86a.js
--rw-r--r--   0 runner    (1001) docker     (123)    14270 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9943.f3f35c7.js
--rw-r--r--   0 runner    (1001) docker     (123)    18136 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9958.25c8c06.js
--rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/9960.64cd61e.js
--rw-r--r--   0 runner    (1001) docker     (123)     1131 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/add-above.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1210 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/add-below.svg
--rw-r--r--   0 runner    (1001) docker     (123)      227 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/add.svg
--rw-r--r--   0 runner    (1001) docker     (123)      942 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/bug-dot.svg
--rw-r--r--   0 runner    (1001) docker     (123)      585 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/bug.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2481 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/build.svg
--rw-r--r--   0 runner    (1001) docker     (123)      301 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/caret-down-empty-thin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/caret-down-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/caret-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/caret-left.svg
--rw-r--r--   0 runner    (1001) docker     (123)      262 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/caret-right.svg
--rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/caret-up-empty-thin.svg
--rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/caret-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1143 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/case-sensitive.svg
--rw-r--r--   0 runner    (1001) docker     (123)      260 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/check.svg
--rw-r--r--   0 runner    (1001) docker     (123)      316 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/circle-empty.svg
--rw-r--r--   0 runner    (1001) docker     (123)      209 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/circle.svg
--rw-r--r--   0 runner    (1001) docker     (123)      452 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/clear.svg
--rw-r--r--   0 runner    (1001) docker     (123)      562 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/close.svg
--rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/code.svg
--rw-r--r--   0 runner    (1001) docker     (123)      423 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/console.svg
--rw-r--r--   0 runner    (1001) docker     (123)      391 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/copy.svg
--rw-r--r--   0 runner    (1001) docker     (123)      623 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/copyright.svg
--rw-r--r--   0 runner    (1001) docker     (123)      602 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/cut.svg
--rw-r--r--   0 runner    (1001) docker     (123)      312 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/delete.svg
--rw-r--r--   0 runner    (1001) docker     (123)      233 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/download.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1384 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/duplicate.svg
--rw-r--r--   0 runner    (1001) docker     (123)      341 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/edit.svg
--rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/ellipses.svg
--rw-r--r--   0 runner    (1001) docker     (123)      484 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/extension.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (123)      243 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/fast-forward.svg
--rw-r--r--   0 runner    (1001) docker     (123)      229 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/file-upload.svg
--rw-r--r--   0 runner    (1001) docker     (123)      461 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/file.svg
--rw-r--r--   0 runner    (1001) docker     (123)      238 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/filter-list.svg
--rw-r--r--   0 runner    (1001) docker     (123)      451 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/folder-favorite.svg
--rw-r--r--   0 runner    (1001) docker     (123)      285 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/home.svg
--rw-r--r--   0 runner    (1001) docker     (123)      891 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/html5.svg
--rw-r--r--   0 runner    (1001) docker     (123)      454 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/image.svg
--rw-r--r--   0 runner    (1001) docker     (123)      322 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/inspector.svg
--rw-r--r--   0 runner    (1001) docker     (123)      923 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/json.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1017 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/julia.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1151 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/jupyter-favicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2765 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/jupyter.svg
--rw-r--r--   0 runner    (1001) docker     (123)     4156 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/jupyterlab-wordmark.svg
--rw-r--r--   0 runner    (1001) docker     (123)      368 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/kernel.svg
--rw-r--r--   0 runner    (1001) docker     (123)      434 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/keyboard.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.400593 resotocore-3.5.1/resotocore/jupyterlite/build/lab/
--rw-r--r--   0 runner    (1001) docker     (123)    54484 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/lab/bundle.js
--rw-r--r--   0 runner    (1001) docker     (123)      411 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/launch.svg
--rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/launcher.svg
--rw-r--r--   0 runner    (1001) docker     (123)      200 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/line-form.svg
--rw-r--r--   0 runner    (1001) docker     (123)      403 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/link.svg
--rw-r--r--   0 runner    (1001) docker     (123)      371 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/list.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1674 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/listings-info.svg
--rw-r--r--   0 runner    (1001) docker     (123)      428 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/markdown.svg
--rw-r--r--   0 runner    (1001) docker     (123)      600 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/move-down.svg
--rw-r--r--   0 runner    (1001) docker     (123)      610 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/move-up.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/new-folder.svg
--rw-r--r--   0 runner    (1001) docker     (123)      899 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/not-trusted.svg
--rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/notebook.svg
--rw-r--r--   0 runner    (1001) docker     (123)      355 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/numbering.svg
--rw-r--r--   0 runner    (1001) docker     (123)      330 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/offline-bolt.svg
--rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/palette.svg
--rw-r--r--   0 runner    (1001) docker     (123)      404 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/paste.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1303 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/pdf.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1893 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/python.svg
--rw-r--r--   0 runner    (1001) docker     (123)      473 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/r-kernel.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2734 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/react.svg
--rw-r--r--   0 runner    (1001) docker     (123)      388 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/redo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      399 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/refresh.svg
--rw-r--r--   0 runner    (1001) docker     (123)      620 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/regex.svg
--rw-r--r--   0 runner    (1001) docker     (123)      217 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/run.svg
--rw-r--r--   0 runner    (1001) docker     (123)      364 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/running.svg
--rw-r--r--   0 runner    (1001) docker     (123)      346 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/save.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.400593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.324592 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.400593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2971 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
--rw-r--r--   0 runner    (1001) docker     (123)     3219 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
--rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
--rw-r--r--   0 runner    (1001) docker     (123)      763 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.400593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      746 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
--rw-r--r--   0 runner    (1001) docker     (123)      563 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
--rw-r--r--   0 runner    (1001) docker     (123)     3717 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
--rw-r--r--   0 runner    (1001) docker     (123)      457 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2347 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     6730 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      343 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (123)      348 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      365 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
--rw-r--r--   0 runner    (1001) docker     (123)     6167 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
--rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      465 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (123)     3587 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1479 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     5970 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
--rw-r--r--   0 runner    (1001) docker     (123)      513 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (123)      385 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
--rw-r--r--   0 runner    (1001) docker     (123)      477 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
--rw-r--r--   0 runner    (1001) docker     (123)     2310 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     8578 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      422 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
--rw-r--r--   0 runner    (1001) docker     (123)      456 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
--rw-r--r--   0 runner    (1001) docker     (123)      466 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1109 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      332 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      655 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1025 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     9894 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     2325 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.404593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      672 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
--rw-r--r--   0 runner    (1001) docker     (123)     2932 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
--rw-r--r--   0 runner    (1001) docker     (123)    24989 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.408593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      389 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
--rw-r--r--   0 runner    (1001) docker     (123)      440 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.408593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1152 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.408593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.408593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.408593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      551 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (123)      402 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (123)      572 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.408593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
--rw-r--r--   0 runner    (1001) docker     (123)     1284 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.324592 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@retrolab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.408593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      463 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/menus.json
--rw-r--r--   0 runner    (1001) docker     (123)      443 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/top.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.408593 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (123)      491 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/scroll-output.json
--rw-r--r--   0 runner    (1001) docker     (123)    79291 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/schemas/all.json
--rw-r--r--   0 runner    (1001) docker     (123)      439 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/search.svg
--rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/service-worker-b2fb40a.js
--rw-r--r--   0 runner    (1001) docker     (123)      860 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/settings.svg
--rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/spreadsheet.svg
--rw-r--r--   0 runner    (1001) docker     (123)      259 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/stop.svg
--rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/tab.svg
--rw-r--r--   0 runner    (1001) docker     (123)      297 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/table-rows.svg
--rw-r--r--   0 runner    (1001) docker     (123)      825 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/tag.svg
--rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/terminal.svg
--rw-r--r--   0 runner    (1001) docker     (123)      270 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/text-editor.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.328592 resotocore-3.5.1/resotocore/jupyterlite/build/themes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.328592 resotocore-3.5.1/resotocore/jupyterlite/build/themes/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.408593 resotocore-3.5.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
--rw-r--r--   0 runner    (1001) docker     (123)    16232 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.408593 resotocore-3.5.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
--rw-r--r--   0 runner    (1001) docker     (123)    15136 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
--rw-r--r--   0 runner    (1001) docker     (123)   310614 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (123)      538 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/toc.svg
--rw-r--r--   0 runner    (1001) docker     (123)      300 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/tree-view.svg
--rw-r--r--   0 runner    (1001) docker     (123)      828 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/trusted.svg
--rw-r--r--   0 runner    (1001) docker     (123)      334 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/undo.svg
--rw-r--r--   0 runner    (1001) docker     (123)      382 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/vega.svg
--rw-r--r--   0 runner    (1001) docker     (123)      426 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/build/yaml.svg
--rw-r--r--   0 runner    (1001) docker     (123)     7192 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/config-utils.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.328592 resotocore-3.5.1/resotocore/jupyterlite/doc/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.408593 resotocore-3.5.1/resotocore/jupyterlite/doc/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      295 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/doc/workspaces/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.332592 resotocore-3.5.1/resotocore/jupyterlite/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.328592 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.408593 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2562 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.408593 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     8738 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    27007 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      621 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     4825 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     8374 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    15897 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.408593 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/
--rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/install.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     2633 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.412593 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     8195 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js
--rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     6063 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js
--rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     2532 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js
--rw-rw-rw-   0 runner    (1001) docker     (123)   165727 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.412593 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/
--rw-rw-rw-   0 runner    (1001) docker     (123)     4270 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     6512 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     6720 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     8221 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
--rw-rw-rw-   0 runner    (1001) docker     (123)     7915 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.412593 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/
--rw-rw-rw-   0 runner    (1001) docker     (123)     1081 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     2657 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    14685 2023-06-02 14:51:33.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.412593 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2732 2023-06-02 14:51:25.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.416593 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)     2643 2023-06-02 14:51:25.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     8368 2023-06-02 14:51:25.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
--rw-rw-rw-   0 runner    (1001) docker     (123)  3578814 2023-06-02 14:51:25.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     1110 2023-06-02 14:51:25.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)    70520 2023-06-02 14:51:25.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      336 2023-06-02 14:51:25.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (123)     2360 2023-06-02 14:51:25.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
--rw-rw-rw-   0 runner    (1001) docker     (123)    14737 2023-06-02 14:51:25.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     7706 2023-06-02 14:51:25.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-02 14:51:25.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     5802 2023-06-02 14:51:25.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.416593 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/
--rw-rw-rw-   0 runner    (1001) docker     (123)      199 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/install.json
--rw-rw-rw-   0 runner    (1001) docker     (123)     3508 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.416593 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/
--rw-rw-rw-   0 runner    (1001) docker     (123)      224 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     7753 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     3889 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
--rw-rw-rw-   0 runner    (1001) docker     (123)      162 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (123)     2452 2023-06-02 14:51:30.000000 resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.416593 resotocore-3.5.1/resotocore/jupyterlite/files/
--rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/jupyterlite/files/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4609 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (123)    20954 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/icon-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)     2513 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-02 14:51:36.000000 resotocore-3.5.1/resotocore/jupyterlite/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (123)    11794 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/jupyterlite.schema.v0.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.416593 resotocore-3.5.1/resotocore/jupyterlite/kernelspecs/
--rw-r--r--   0 runner    (1001) docker     (123)      777 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/kernelspecs/javascript.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.420593 resotocore-3.5.1/resotocore/jupyterlite/lab/
--rw-r--r--   0 runner    (1001) docker     (123)   324251 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/lab/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (123)      993 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/lab/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/lab/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      144 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/lab/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (123)    10101 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/lab/package.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.420593 resotocore-3.5.1/resotocore/jupyterlite/lab/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      290 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/lab/tree/index.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.420593 resotocore-3.5.1/resotocore/jupyterlite/lab/workspaces/
--rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/lab/workspaces/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      690 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/manifest.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)     1307 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/package.json
--rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/service-worker-b2fb40a.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.420593 resotocore-3.5.1/resotocore/jupyterlite/tree/
--rw-r--r--   0 runner    (1001) docker     (123)      304 1985-10-26 08:15:00.000000 resotocore-3.5.1/resotocore/jupyterlite/tree/index.html
--rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.420593 resotocore-3.5.1/resotocore/model/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/model/adjust_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/model/db_updater.py
--rw-r--r--   0 runner    (1001) docker     (123)    24326 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/model/graph_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/model/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)    54880 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/model/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/model/model_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/model/resolve_in_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/model/transform_kind_convert.py
--rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/model/typed_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.420593 resotocore-3.5.1/resotocore/query/
--rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    48513 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/query/model.py
--rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/query/query_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     8691 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/query/template_expander.py
--rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/query/template_expander_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.420593 resotocore-3.5.1/resotocore/report/
--rw-r--r--   0 runner    (1001) docker     (123)    15062 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/report/benchmark_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/report/inspector_service.py
--rw-r--r--   0 runner    (1001) docker     (123)     6863 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/report/report_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.424593 resotocore-3.5.1/resotocore/static/
--rw-r--r--   0 runner    (1001) docker     (123)   127540 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/api-doc.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/ck-unicode-truecolor.ans
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.424593 resotocore-3.5.1/resotocore/static/report/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.332592 resotocore-3.5.1/resotocore/static/report/benchmark/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.424593 resotocore-3.5.1/resotocore/static/report/benchmark/aws/
--rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/report/benchmark/aws/aws_cis_1_5.json
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/report/benchmark_template.json
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/report/check_template.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.336592 resotocore-3.5.1/resotocore/static/report/checks/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.424593 resotocore-3.5.1/resotocore/static/report/checks/aws/
--rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/report/checks/aws/aws_apigateway.json
--rw-r--r--   0 runner    (1001) docker     (123)    33970 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/report/checks/aws/aws_cloudtrail.json
--rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/report/checks/aws/aws_config.json
--rw-r--r--   0 runner    (1001) docker     (123)    46657 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/report/checks/aws/aws_ec2.json
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/report/checks/aws/aws_efs.json
--rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/report/checks/aws/aws_iam.json
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/report/checks/aws/aws_kms.json
--rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/report/checks/aws/aws_lambda.json
--rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/report/checks/aws/aws_rds.json
--rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/report/checks/aws/aws_s3.json
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/resoto.css
--rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/static/resoto_logo_and_text.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.424593 resotocore-3.5.1/resotocore/task/
--rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/task/job_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/task/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/task/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/task/start_workflow_on_first_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/task/subscribers.py
--rw-r--r--   0 runner    (1001) docker     (123)    30956 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/task/task_description.py
--rw-r--r--   0 runner    (1001) docker     (123)    28462 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/task/task_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.424593 resotocore-3.5.1/resotocore/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/templates/create_first_user.html
--rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.424593 resotocore-3.5.1/resotocore/user/
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/user/user_management.py
--rw-r--r--   0 runner    (1001) docker     (123)    14044 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.428593 resotocore-3.5.1/resotocore/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64797 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/web/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/web/certificate_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/web/content_renderer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/web/directives.py
--rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/web/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/web/tsdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-06-02 14:47:48.000000 resotocore-3.5.1/resotocore/worker_task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.340592 resotocore-3.5.1/resotocore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-06-02 14:51:40.000000 resotocore-3.5.1/resotocore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34481 2023-06-02 14:51:40.000000 resotocore-3.5.1/resotocore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:51:40.000000 resotocore-3.5.1/resotocore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-02 14:51:40.000000 resotocore-3.5.1/resotocore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:51:39.000000 resotocore-3.5.1/resotocore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-02 14:51:40.000000 resotocore-3.5.1/resotocore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-02 14:51:40.000000 resotocore-3.5.1/resotocore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-02 14:51:40.436593 resotocore-3.5.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.428593 resotocore-3.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.428593 resotocore-3.5.1/tests/resotocore/
--rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.428593 resotocore-3.5.1/tests/resotocore/analytics/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/analytics/posthog_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/analytics/recurrent_events_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.428593 resotocore-3.5.1/tests/resotocore/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11912 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/cli/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    56452 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/cli/command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/cli/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.428593 resotocore-3.5.1/tests/resotocore/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/config/config_handler_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/config/config_override_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/config/core_config_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    27555 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/console_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/core_config_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.432593 resotocore-3.5.1/tests/resotocore/db/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/db/arango_query_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/db/arangodb_functions_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/db/async_arangodb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/db/configdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/db/db_access_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (123)    28962 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/db/graphdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/db/jobdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/db/modeldb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/db/runningtaskdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/db/subscriberdb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/db/system_data_db_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/db/templatedb_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/dependencies_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.432593 resotocore-3.5.1/tests/resotocore/graph_manager/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/graph_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6466 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/graph_manager/graph_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2450 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/hypothesis_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.432593 resotocore-3.5.1/tests/resotocore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/infra_apps/local_runtime_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/infra_apps/package_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/message_bus_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.432593 resotocore-3.5.1/tests/resotocore/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/model/adjust_node_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/model/db_updater_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    15404 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/model/graph_access_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/model/json_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/model/model_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    23564 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/model/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/model/resolve_in_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/model/typed_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.432593 resotocore-3.5.1/tests/resotocore/query/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/query/model_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/query/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5778 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/query/template_expander_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.432593 resotocore-3.5.1/tests/resotocore/report/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/report/benchnmark_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/report/inspector_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.432593 resotocore-3.5.1/tests/resotocore/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/task/job_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/task/start_workflow_on_first_subscriber_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/task/subscribers_test.py
--rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/task/task_description_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/task/task_handler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.432593 resotocore-3.5.1/tests/resotocore/user/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/user/user_management_service_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/validator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 14:51:40.436593 resotocore-3.5.1/tests/resotocore/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/web/api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    20088 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/web/api_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/web/certificate_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5305 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/web/content_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-02 14:47:48.000000 resotocore-3.5.1/tests/resotocore/worker_task_queue_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.967096 resotocore-3.5.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 13:03:16.000000 resotocore-3.5.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-13 13:03:16.000000 resotocore-3.5.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-06-13 13:07:15.967096 resotocore-3.5.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-06-13 13:03:16.000000 resotocore-3.5.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-13 13:03:16.000000 resotocore-3.5.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.871096 resotocore-3.5.2/resotocore/
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12555 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.875096 resotocore-3.5.2/resotocore/action_handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/action_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/action_handlers/merge_outer_edge_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.875096 resotocore-3.5.2/resotocore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5287 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/analytics/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/analytics/recurrent_events.py
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/async_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.875096 resotocore-3.5.2/resotocore/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     7019 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30427 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)   229427 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/cli/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25451 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/cli/tip_of_the_day.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.875096 resotocore-3.5.2/resotocore/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     6073 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13279 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/config/config_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6978 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/config/config_override_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12781 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/config/core_config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4206 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/console_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37296 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/core_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.879096 resotocore-3.5.2/resotocore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32054 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/arango_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1646 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/arangodb_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/arangodb_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21148 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/async_arangodb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/configdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14062 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/db_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/deferred_edge_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5399 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64016 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/graphdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/jobdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2192 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/modeldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/packagedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10609 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/runningtaskdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/subscriberdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/system_data_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/db/templatedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11697 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2333 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/error.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.879096 resotocore-3.5.2/resotocore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15560 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/graph_manager/graph_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/ids.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.879096 resotocore-3.5.2/resotocore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4669 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/infra_apps/local_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2360 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/infra_apps/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13703 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/infra_apps/package_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1246 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/infra_apps/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.879096 resotocore-3.5.2/resotocore/jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.863096 resotocore-3.5.2/resotocore/jupyterlite/api/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.879096 resotocore-3.5.2/resotocore/jupyterlite/api/contents/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-06-13 13:07:11.000000 resotocore-3.5.2/resotocore/jupyterlite/api/contents/all.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.879096 resotocore-3.5.2/resotocore/jupyterlite/api/translations/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-13 13:07:11.000000 resotocore-3.5.2/resotocore/jupyterlite/api/translations/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 13:07:11.000000 resotocore-3.5.2/resotocore/jupyterlite/api/translations/en.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3223 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/bootstrap.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.931096 resotocore-3.5.2/resotocore/jupyterlite/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1037.51967a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    21710 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1079.cdbaf67.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9647 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1084.4cd1c89.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1950 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1113.23c9417.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9736 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1125.129d070.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9342 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1163.ac28297.js
+-rw-r--r--   0 runner    (1001) docker     (123)    74541 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1221.c51249a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1245.be46619.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9525 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1261.199fc1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10027 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1272.f334098.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14792 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1278.0524a4a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1290.3981211.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1295.46e72b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1310.23bbe67.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10986 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1320.21effe3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6216 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1325.f76267c.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7061 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1408.7461890.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1440.a9e7ea1.js
+-rw-r--r--   0 runner    (1001) docker     (123)    23820 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1483.616d9ab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    47542 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1489.e50b6d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2605 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1507.5705605.js
+-rw-r--r--   0 runner    (1001) docker     (123)      624 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/152.525d460.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36869 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1520.4e2eb21.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1555.e188f3f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8584 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1559.7c89925.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9056 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/160.5f28731.js
+-rw-r--r--   0 runner    (1001) docker     (123)   478144 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1603.370a2a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22415 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1644.0e49167.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1667.f0afb2b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17330 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1687.27f1ad6.js
+-rw-r--r--   0 runner    (1001) docker     (123)   272197 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1725.f151c33.js
+-rw-r--r--   0 runner    (1001) docker     (123)    25316 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1767.c8c2f26.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1806.1aaf66b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1838.1202b16.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1909.28a2def.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9485 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/1989.88d258f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    89976 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2030.1562cc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6343 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2047.baed97b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2099.f4b6fcd.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6160 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2118.5b65f70.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3149 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/213.5769e57.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2161.dcb27b8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2169.635c88e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17630 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/217.90d10e2.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35022 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2212.72be094.js
+-rw-r--r--   0 runner    (1001) docker     (123)   123689 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2287.997c38e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      545 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     9469 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2303.9ff8710.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2319.6b4cbb7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2648 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2329.4c5ca6d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8667 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2351.fbd96d8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2358.d5cf7c8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7913 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2359.6451c3e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9289 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/237.f765e77.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2384.71782be.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/240.cddc46b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15476 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2431.648d237.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12395 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2546.1f48267.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2557.75e9da2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4176 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/261.5f53c0e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8923 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2629.c0e1cd6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2788.46acc8a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2834.942acc6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2887.47ba752.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8870 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2956.8880209.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4300 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/2973.2a51dc4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8060 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3004.255e79c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17042 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/302.8bcc38f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8560 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3037.70ee38d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3042.7cfad84.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10136 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3051.34fac68.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9664 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3122.2289fca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3151.10ef4de.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15850 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/316.c850a76.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20975 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3196.4e35a17.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16159 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3265.a80440a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3277.9c04e75.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8847 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/330.126fa98.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14007 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3392.29fe6b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    80815 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3413.480a49d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3444.47d5ea1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3469.7d14d0b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9554 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3546.fee1bd7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5145 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/362.6716970.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3708.410d087.js
+-rw-r--r--   0 runner    (1001) docker     (123)      170 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3752.8735345.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16215 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3850.903abc2.js
+-rw-r--r--   0 runner    (1001) docker     (123)      808 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3880.bd39dce.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10216 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3970.236586f.js
+-rw-r--r--   0 runner    (1001) docker     (123)   897822 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3976.58893b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16446 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/3979.385527e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11331 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/400.d72234b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11916 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4018.1a35967.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/406.9b7af92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11111 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4117.a8107fd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10886 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4182.e2430f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4191.02bbea8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3331 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4197.53ab10b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9224 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4206.a5f8bb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8525 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4207.0d0580b.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4262.bb73457.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4298.5ee510c.js
+-rw-r--r--   0 runner    (1001) docker     (123)    83844 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/44.0cfa785.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4410.e4a25d3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3371 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4466.64d23d1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4507.8b41ef4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7852 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/451.d9683ad.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2977 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4535.34b060a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    20495 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4565.43bdb91.js
+-rw-r--r--   0 runner    (1001) docker     (123)    22220 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4569.f374f9d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    91604 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4615.eb5d40a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   119541 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4658.090d4a9.js
+-rw-r--r--   0 runner    (1001) docker     (123)       95 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4658.090d4a9.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      356 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4665.aa19a41.js
+-rw-r--r--   0 runner    (1001) docker     (123)      142 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4668.f65690b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4695 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4690.3dd4096.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4715.e7690b9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10282 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4749.46ebbb2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9653 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4750.56c06ab.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17648 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4856.2d7415f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    41909 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4875.375150e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6350 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/489.b981dea.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2209 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/490.c2624d4.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2796 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4905.667bf33.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4931.430433b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4639 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/4942.b96c164.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5016.dd2fe83.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5766 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5072.733a1b5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/509.6448878.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5096.8ed0d8e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4581 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5126.eecad7a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3825 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5129.1ba4763.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5153.763d8fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)      618 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5155.06b4ea9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32726 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5193.e9f6866.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9808 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5213.3e1a360.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8503 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5227.8c8acd8.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11129 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5238.1751cc3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5579 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/528.2262cb0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5292.79d4aba.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7706 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5437.31236f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10580 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5489.848a8cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5146 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5508.317fca3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9068 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/554.ac98303.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/555.2cd31dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16702 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5573.ebcdb93.js
+-rw-r--r--   0 runner    (1001) docker     (123)   171864 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5666.c5e5324.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8628 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5710.70d0b1d.js
+-rw-r--r--   0 runner    (1001) docker     (123)   172015 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5747.94ad626.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14074 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/582.21b8e7d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9294 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5823.5045bdb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2543 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5851.30b7b2a.js
+-rw-r--r--   0 runner    (1001) docker     (123)   257877 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5878.32d92fa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5880.68f975b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3663 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5955.88508f7.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4727 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/5971.88c5642.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6080.aa0ff24.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28010 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/61.2808a0d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18045 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6136.b8ba2b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6141.9831d58.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6475.6037fbb.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7434 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6493.d796aa5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4963 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6556.b3d9293.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5803 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6571.2c8884e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10586 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6576.3ea568e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    83397 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6591.94ed352.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7388 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6612.1632879.js
+-rw-r--r--   0 runner    (1001) docker     (123)   246379 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6623.ae3b3cc.js
+-rw-r--r--   0 runner    (1001) docker     (123)      160 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6623.ae3b3cc.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    16150 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6664.2160109.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9611 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6747.47be7f5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3577 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6748.be68f5f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8961 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6870.7940288.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11058 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6879.c8367a5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    16507 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6898.9bbc12a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10256 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6952.f68b818.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2054 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6985.321ad92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10925 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6993.32cf9a6.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7233 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/6997.b06fe71.js
+-rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7041.d4f561e.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10338 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7058.805c88e.js
+-rw-r--r--   0 runner    (1001) docker     (123)       51 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7058.805c88e.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2983 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7174.6c45206.js
+-rw-r--r--   0 runner    (1001) docker     (123)    35260 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7334.8859b1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8497 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7359.6ee65ec.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3555 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7364.195178b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9117 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7380.58a4413.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7126 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7427.f9c2017.js
+-rw-r--r--   0 runner    (1001) docker     (123)      294 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7427.f9c2017.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    14994 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7463.18fd278.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10358 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7509.1e0189e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1074 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7526.1a303e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31492 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7537.1323a15.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10078 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7692.33d5169.js
+-rw-r--r--   0 runner    (1001) docker     (123)      595 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7746.5908d29.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10754 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7808.1d582a2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/783.c156751.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9192 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7858.2386e4d.js
+-rw-r--r--   0 runner    (1001) docker     (123)    31628 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/7941.01ea680.js
+-rw-r--r--   0 runner    (1001) docker     (123)     5753 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8005.c5ad7b2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7966 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8028.39e2fa1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9977 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8061.cc62561.js
+-rw-r--r--   0 runner    (1001) docker     (123)   317511 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8101.cf46d02.js
+-rw-r--r--   0 runner    (1001) docker     (123)       50 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8101.cf46d02.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7965 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/812.9b0e86e.js
+-rw-r--r--   0 runner    (1001) docker     (123)      855 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/816.c8050f2.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8165.b2c3285.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3150 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8232.a578bf9.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/824.8678196.js
+-rw-r--r--   0 runner    (1001) docker     (123)    15838 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8270.89fe7e1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2327 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/833.9cc6653.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3035 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8370.8f855e5.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10481 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8373.96b0b3a.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2921 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8389.ffe031f.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6825 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8412.1528057.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9361 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8427.4923f43.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8958 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8542.027afdc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8843 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8594.0112f03.js
+-rw-r--r--   0 runner    (1001) docker     (123)    30005 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8656.d5b8e92.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12065 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8685.d78bdab.js
+-rw-r--r--   0 runner    (1001) docker     (123)   114157 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8698.9817d75.js
+-rw-r--r--   0 runner    (1001) docker     (123)     7346 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8732.9320f73.js
+-rw-r--r--   0 runner    (1001) docker     (123)      123 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8741.b138cb8.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2572 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8785.cf4fe95.js
+-rw-r--r--   0 runner    (1001) docker     (123)    27799 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8828.77c71d0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2950 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8883.80c7b63.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9758 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8976.3816942.js
+-rw-r--r--   0 runner    (1001) docker     (123)      432 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8981.99a4275.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/8990.2a453cf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9035.1e45c1b.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9053.45b77fc.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9689 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9077.fefb6ca.js
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9128.b8fa6f0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9225 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9156.0cefbd3.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2790 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9170.0023587.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10649 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9196.315f9f9.js
+-rw-r--r--   0 runner    (1001) docker     (123)    28388 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9198.9971d70.js
+-rw-r--r--   0 runner    (1001) docker     (123)   131443 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/920.d15c177.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4000 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9253.0b31caa.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8378 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9266.bacd0dd.js
+-rw-r--r--   0 runner    (1001) docker     (123)      591 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9307.c3a00ed.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4159 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9321.869e413.js
+-rw-r--r--   0 runner    (1001) docker     (123)  1188430 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9344.ba0abcf.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9382.9014799.js
+-rw-r--r--   0 runner    (1001) docker     (123)    29226 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9440.1b10b8f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      163 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9440.1b10b8f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3414 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9464.79e6ac5.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9502.9a24831.js
+-rw-r--r--   0 runner    (1001) docker     (123)    32420 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9507.1e6cc5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9206 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9602.62bf0f1.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9381 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9621.e2e8b5d.js
+-rw-r--r--   0 runner    (1001) docker     (123)      625 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9622.ccab065.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9626.a178bd0.js
+-rw-r--r--   0 runner    (1001) docker     (123)    10559 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9647.ed91993.js
+-rw-r--r--   0 runner    (1001) docker     (123)   432928 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9657.bc5c60e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     9073 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/97.ad126b0.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9712.796a0a1.js
+-rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9733.a3b2a7f.js
+-rw-r--r--   0 runner    (1001) docker     (123)    36791 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9737.7dc8f98.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9777.0b8a504.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9793.6d63a85.js
+-rw-r--r--   0 runner    (1001) docker     (123)    17595 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9806.652c162.js
+-rw-r--r--   0 runner    (1001) docker     (123)   179318 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9865.2e3db6f.js
+-rw-r--r--   0 runner    (1001) docker     (123)      246 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9865.2e3db6f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4299 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/989.bcca86a.js
+-rw-r--r--   0 runner    (1001) docker     (123)    14270 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9943.f3f35c7.js
+-rw-r--r--   0 runner    (1001) docker     (123)    18136 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9958.25c8c06.js
+-rw-r--r--   0 runner    (1001) docker     (123)     6697 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/9960.64cd61e.js
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/add-above.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1210 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/add-below.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      227 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/add.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      942 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/bug-dot.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      585 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/bug.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2481 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/build.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      301 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/caret-down-empty-thin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/caret-down-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/caret-left.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      262 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/caret-right.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/caret-up-empty-thin.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      257 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/caret-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1143 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/case-sensitive.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      260 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/check.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      316 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/circle-empty.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      209 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/circle.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      452 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/clear.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      562 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/close.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/code.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      423 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/console.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      391 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/copy.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      623 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/copyright.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      602 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/cut.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      312 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/delete.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      233 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/download.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1384 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/duplicate.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      341 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/edit.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      282 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/ellipses.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      484 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/extension.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (123)       38 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)      243 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/fast-forward.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      229 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/file-upload.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      461 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/file.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      238 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/filter-list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      451 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/folder-favorite.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      285 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      303 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/home.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      891 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/html5.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      454 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/image.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      322 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/inspector.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      923 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/json.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/julia.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/jupyter-favicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2765 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/jupyter.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/jupyterlab-wordmark.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      368 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/kernel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      434 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/keyboard.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.931096 resotocore-3.5.2/resotocore/jupyterlite/build/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)    54484 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/lab/bundle.js
+-rw-r--r--   0 runner    (1001) docker     (123)      411 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/launch.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      317 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/launcher.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      200 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/line-form.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      403 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/link.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      371 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/list.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1674 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/listings-info.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      428 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/markdown.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      600 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/move-down.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      610 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/move-up.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/new-folder.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      899 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/not-trusted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      326 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/notebook.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      355 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/numbering.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      330 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/offline-bolt.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      856 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/palette.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      404 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/paste.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1303 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/pdf.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/python.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      473 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/r-kernel.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/react.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      388 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/redo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      399 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/refresh.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      620 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/regex.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      217 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/run.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      364 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/running.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      346 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/save.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.867096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
+-rw-r--r--   0 runner    (1001) docker     (123)      506 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
+-rw-r--r--   0 runner    (1001) docker     (123)      763 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      746 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
+-rw-r--r--   0 runner    (1001) docker     (123)      563 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3717 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
+-rw-r--r--   0 runner    (1001) docker     (123)      457 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2347 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     6730 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      348 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/completer-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      365 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6167 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1964 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      465 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1479 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
+-rw-r--r--   0 runner    (1001) docker     (123)      513 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (123)      385 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
+-rw-r--r--   0 runner    (1001) docker     (123)      477 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     8578 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      422 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
+-rw-r--r--   0 runner    (1001) docker     (123)      456 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
+-rw-r--r--   0 runner    (1001) docker     (123)      466 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.935096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      332 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      655 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     9894 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      672 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2932 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24989 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      389 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)      440 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1152 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (123)      402 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (123)      572 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)     1284 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.867096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@retrolab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/menus.json
+-rw-r--r--   0 runner    (1001) docker     (123)      443 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@retrolab/application-extension/top.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)      491 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@retrolab/notebook-extension/scroll-output.json
+-rw-r--r--   0 runner    (1001) docker     (123)    79291 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/schemas/all.json
+-rw-r--r--   0 runner    (1001) docker     (123)      439 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/search.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/service-worker-b2fb40a.js
+-rw-r--r--   0 runner    (1001) docker     (123)      860 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/settings.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      336 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/spreadsheet.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      259 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/tab.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      297 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/table-rows.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      825 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/tag.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/terminal.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      270 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/text-editor.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.867096 resotocore-3.5.2/resotocore/jupyterlite/build/themes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.867096 resotocore-3.5.2/resotocore/jupyterlite/build/themes/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    16232 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
+-rw-r--r--   0 runner    (1001) docker     (123)    15136 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (123)        0 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
+-rw-r--r--   0 runner    (1001) docker     (123)   310614 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (123)      538 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/toc.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      300 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/tree-view.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      828 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/trusted.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      334 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/undo.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      382 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/vega.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      426 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/build/yaml.svg
+-rw-r--r--   0 runner    (1001) docker     (123)     7192 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/config-utils.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.867096 resotocore-3.5.2/resotocore/jupyterlite/doc/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/doc/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      295 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/doc/workspaces/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.867096 resotocore-3.5.2/resotocore/jupyterlite/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.867096 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.939096 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2562 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.943096 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8738 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6180 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    27007 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      621 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4825 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8374 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    15897 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.943096 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2633 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.943096 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8195 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6063 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)       88 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2532 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)   165727 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      213 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js.LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.943096 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     4270 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6512 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     6720 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8221 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2337 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7915 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.943096 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1081 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2657 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14685 2023-06-13 13:07:08.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.943096 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2732 2023-06-13 13:07:00.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.947096 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2643 2023-06-13 13:07:00.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     8368 2023-06-13 13:07:00.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)  3578814 2023-06-13 13:07:00.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     1110 2023-06-13 13:07:00.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)    70520 2023-06-13 13:07:00.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      336 2023-06-13 13:07:00.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2360 2023-06-13 13:07:00.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)    14737 2023-06-13 13:07:00.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7706 2023-06-13 13:07:00.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      118 2023-06-13 13:07:00.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     5802 2023-06-13 13:07:00.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.947096 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      199 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3508 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.951096 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/
+-rw-rw-rw-   0 runner    (1001) docker     (123)      224 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     7753 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     3889 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)      162 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (123)     2452 2023-06-13 13:07:05.000000 resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.951096 resotocore-3.5.2/resotocore/jupyterlite/files/
+-rw-r--r--   0 runner    (1001) docker     (123)     7611 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/jupyterlite/files/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4609 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (123)    20954 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/icon-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6937 2023-06-13 13:07:11.000000 resotocore-3.5.2/resotocore/jupyterlite/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11794 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/jupyterlite.schema.v0.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.951096 resotocore-3.5.2/resotocore/jupyterlite/kernelspecs/
+-rw-r--r--   0 runner    (1001) docker     (123)      777 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/kernelspecs/javascript.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.951096 resotocore-3.5.2/resotocore/jupyterlite/lab/
+-rw-r--r--   0 runner    (1001) docker     (123)   324251 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/lab/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (123)      993 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/lab/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1489 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/lab/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      144 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/lab/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10101 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/lab/package.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.951096 resotocore-3.5.2/resotocore/jupyterlite/lab/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      290 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/lab/tree/index.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.951096 resotocore-3.5.2/resotocore/jupyterlite/lab/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/lab/workspaces/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      690 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/manifest.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)     1307 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/package.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1453 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/service-worker-b2fb40a.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.951096 resotocore-3.5.2/resotocore/jupyterlite/tree/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 1985-10-26 08:15:00.000000 resotocore-3.5.2/resotocore/jupyterlite/tree/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)    11196 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.951096 resotocore-3.5.2/resotocore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2162 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/model/adjust_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10201 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/model/db_updater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24326 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/model/graph_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5792 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/model/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55069 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10498 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/model/model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4491 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/model/resolve_in_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/model/transform_kind_convert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1750 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/model/typed_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.951096 resotocore-3.5.2/resotocore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    48513 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/query/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14513 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/query/query_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9013 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/query/template_expander.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1935 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/query/template_expander_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.955096 resotocore-3.5.2/resotocore/report/
+-rw-r--r--   0 runner    (1001) docker     (123)    15297 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/report/benchmark_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18014 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/report/inspector_service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6867 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/report/report_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.955096 resotocore-3.5.2/resotocore/static/
+-rw-r--r--   0 runner    (1001) docker     (123)   129588 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/api-doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/ck-unicode-truecolor.ans
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.955096 resotocore-3.5.2/resotocore/static/report/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.867096 resotocore-3.5.2/resotocore/static/report/benchmark/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.955096 resotocore-3.5.2/resotocore/static/report/benchmark/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)    43058 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/report/benchmark/aws/aws_cis_1_5.json
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/report/benchmark_template.json
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/report/check_template.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.871096 resotocore-3.5.2/resotocore/static/report/checks/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.955096 resotocore-3.5.2/resotocore/static/report/checks/aws/
+-rw-r--r--   0 runner    (1001) docker     (123)     4342 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/report/checks/aws/aws_apigateway.json
+-rw-r--r--   0 runner    (1001) docker     (123)    33970 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/report/checks/aws/aws_cloudtrail.json
+-rw-r--r--   0 runner    (1001) docker     (123)      952 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/report/checks/aws/aws_config.json
+-rw-r--r--   0 runner    (1001) docker     (123)    46657 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/report/checks/aws/aws_ec2.json
+-rw-r--r--   0 runner    (1001) docker     (123)      878 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/report/checks/aws/aws_efs.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24445 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/report/checks/aws/aws_iam.json
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/report/checks/aws/aws_kms.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4915 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/report/checks/aws/aws_lambda.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2416 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/report/checks/aws/aws_rds.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6348 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/report/checks/aws/aws_s3.json
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/resoto.css
+-rw-r--r--   0 runner    (1001) docker     (123)    16175 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/static/resoto_logo_and_text.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.955096 resotocore-3.5.2/resotocore/task/
+-rw-r--r--   0 runner    (1001) docker     (123)     1517 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/task/job_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1582 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/task/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/task/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/task/start_workflow_on_first_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6255 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/task/subscribers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30956 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/task/task_description.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28462 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/task/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.955096 resotocore-3.5.2/resotocore/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      793 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/templates/create_first_user.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1335 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1059 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.955096 resotocore-3.5.2/resotocore/user/
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5791 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/user/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14044 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.959096 resotocore-3.5.2/resotocore/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65833 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/web/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8859 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/web/certificate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8747 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/web/content_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6748 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/web/directives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/web/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5271 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/web/tsdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10412 2023-06-13 13:03:16.000000 resotocore-3.5.2/resotocore/worker_task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.875096 resotocore-3.5.2/resotocore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    17707 2023-06-13 13:07:15.000000 resotocore-3.5.2/resotocore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34481 2023-06-13 13:07:15.000000 resotocore-3.5.2/resotocore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:07:15.000000 resotocore-3.5.2/resotocore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 13:07:15.000000 resotocore-3.5.2/resotocore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:07:15.000000 resotocore-3.5.2/resotocore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-06-13 13:07:15.000000 resotocore-3.5.2/resotocore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-06-13 13:07:15.000000 resotocore-3.5.2/resotocore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      422 2023-06-13 13:07:15.967096 resotocore-3.5.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.959096 resotocore-3.5.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.959096 resotocore-3.5.2/tests/resotocore/
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.959096 resotocore-3.5.2/tests/resotocore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/analytics/posthog_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1502 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/analytics/recurrent_events_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.959096 resotocore-3.5.2/tests/resotocore/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12177 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/cli/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    57404 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/cli/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3655 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/cli/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.959096 resotocore-3.5.2/tests/resotocore/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12759 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/config/config_handler_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6241 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/config/config_override_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4413 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/config/core_config_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27555 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1096 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/console_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8387 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/core_config_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.963096 resotocore-3.5.2/tests/resotocore/db/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/db/arango_query_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1379 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/db/arangodb_functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1173 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/db/async_arangodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4120 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/db/configdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2625 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/db/db_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1645 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28962 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/db/graphdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/db/jobdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/db/modeldb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5510 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/db/runningtaskdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2908 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/db/subscriberdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/db/system_data_db_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/db/templatedb_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/dependencies_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.963096 resotocore-3.5.2/tests/resotocore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7276 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/graph_manager/graph_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2580 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/hypothesis_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.963096 resotocore-3.5.2/tests/resotocore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4677 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/infra_apps/local_runtime_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/infra_apps/package_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/message_bus_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.963096 resotocore-3.5.2/tests/resotocore/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/model/adjust_node_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2518 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/model/db_updater_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15404 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/model/graph_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/model/json_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/model/model_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23570 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/model/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/model/resolve_in_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/model/typed_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.963096 resotocore-3.5.2/tests/resotocore/query/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14448 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/query/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14492 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/query/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6815 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/query/template_expander_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.963096 resotocore-3.5.2/tests/resotocore/report/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/report/benchnmark_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6310 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/report/inspector_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.967096 resotocore-3.5.2/tests/resotocore/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1380 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/task/job_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/task/start_workflow_on_first_subscriber_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/task/subscribers_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10513 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/task/task_description_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9465 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/task/task_handler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.967096 resotocore-3.5.2/tests/resotocore/user/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/user/user_management_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4509 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/validator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:07:15.967096 resotocore-3.5.2/tests/resotocore/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16004 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/web/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21471 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/web/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/web/certificate_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5357 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/web/content_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-06-13 13:03:16.000000 resotocore-3.5.2/tests/resotocore/worker_task_queue_test.py
```

### Comparing `resotocore-3.5.1/LICENSE` & `resotocore-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/PKG-INFO` & `resotocore-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotocore
-Version: 3.5.1
+Version: 3.5.2
 Summary: Keeps all the things.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `resotocore-3.5.1/README.md` & `resotocore-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/pyproject.toml` & `resotocore-3.5.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "resotocore"
-version = "3.5.1"
+version = "3.5.2"
 authors = [{name="Some Engineering Inc."}]
 description = "Keeps all the things."
 license = {file="LICENSE"}
 urls = {"Homepage" = "https://resoto.com"}
 requires-python = ">=3.9"
 classifiers = [ "Programming Language :: Python :: 3" ]
 readme = {file="README.md", content-type="text/markdown"}
```

### Comparing `resotocore-3.5.1/resotocore/__main__.py` & `resotocore-3.5.2/resotocore/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -181,15 +181,15 @@
         config, message_bus, worker_task_queue, config_handler, event_sender, inspector
     )
     merge_outer_edges_handler = MergeOuterEdgesHandler(message_bus, subscriptions, task_handler, db, model)
     cli_deps.extend(task_handler=task_handler, inspector=inspector)
     infra_apps_runtime = LocalResotocoreAppRuntime(cli)
     cli_deps.extend(infra_apps_runtime=infra_apps_runtime)
     infra_apps_package_manager = PackageManager(
-        db.package_entity_db, config_handler, cli.register_alias_template, cli.unregister_alias_template
+        db.package_entity_db, config_handler, cli.register_infra_app_alias, cli.unregister_infra_app_alias
     )
     cli_deps.extend(infra_apps_package_manager=infra_apps_package_manager)
     graph_manager = GraphManager(db, config.snapshots, core_config_handler, task_handler)
     cli_deps.extend(graph_manager=graph_manager)
     api = Api(
         db,
         model,
@@ -202,14 +202,15 @@
         config_handler,
         inspector,
         cli,
         template_expander,
         config,
         user_management,
         config_override_service.get_override,
+        graph_manager,
     )
     event_emitter = emit_recurrent_events(
         event_sender, model, subscriptions, worker_task_queue, message_bus, timedelta(hours=1), timedelta(hours=1)
     )
 
     async def on_start() -> None:
         # queue must be created inside an async function!
```

### Comparing `resotocore-3.5.1/resotocore/action_handlers/merge_outer_edge_handler.py` & `resotocore-3.5.2/resotocore/action_handlers/merge_outer_edge_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/analytics/__init__.py` & `resotocore-3.5.2/resotocore/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/analytics/posthog.py` & `resotocore-3.5.2/resotocore/analytics/posthog.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/analytics/recurrent_events.py` & `resotocore-3.5.2/resotocore/analytics/recurrent_events.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/async_extensions.py` & `resotocore-3.5.2/resotocore/async_extensions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/cli/__init__.py` & `resotocore-3.5.2/resotocore/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/cli/cli.py` & `resotocore-3.5.2/resotocore/cli/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -50,14 +50,15 @@
     CLI,
     EmptyContext,
     CLISource,
     NoTerminalOutput,
     OutputTransformer,
     PreserveOutputFormat,
     AliasTemplate,
+    InfraAppAlias,
     ArgsInfo,
     ArgInfo,
     AliasTemplateParameter,
 )
 from resotocore.cli.dependencies import CLIDependencies
 from resotocore.console_renderer import ConsoleRenderer
 from resotocore.error import CLIParseError
@@ -116,23 +117,25 @@
 
     def __init__(
         self,
         dependencies: CLIDependencies,
         parts: List[CLICommand],
         alias_names: Dict[str, str],
         alias_templates: Dict[str, AliasTemplate],
+        infra_app_aliases: Dict[str, InfraAppAlias],
     ):
         super().__init__(dependencies, "misc", True)
         self.all_parts = {p.name: p for p in parts + [self]}
         self.parts = {p.name: p for p in parts + [self] if not isinstance(p, InternalPart)}
         self.alias_names = {a: n for a, n in alias_names.items() if n in self.parts and a not in self.parts}
         self.reverse_alias_names: Dict[str, List[str]] = {
             k: [e[0] for e in v] for k, v in group_by(lambda a: a[1], self.alias_names.items()).items()
         }
         self.alias_templates = alias_templates
+        self.infra_app_aliases = infra_app_aliases
 
     @property
     def name(self) -> str:
         return "help"
 
     def info(self) -> str:
         return "Shows available commands, as well as help for any specific command."
@@ -146,15 +149,19 @@
             return ctx.render_console(f"## Valid placeholder string: \n\n{replacements}")
 
         def overview() -> str:
             all_parts = sorted(self.parts.values(), key=lambda p: p.name)
             parts = [p for p in all_parts if isinstance(p, CLICommand)]
             templates = list(sorted(self.alias_templates.values(), key=attrgetter("name")))
             alias_templates = "\n".join(f"- `{a.name}` - {a.info}" for a in templates)
-            result = f"## Custom Commands \n{alias_templates}\n"
+
+            sorted_infra_app_aliases = list(sorted(self.infra_app_aliases.values(), key=attrgetter("name")))
+            infra_app_aliases = "\n".join(f"- `{a.name}` - {a.description}" for a in sorted_infra_app_aliases)
+
+            result = f"## Custom Commands \n{alias_templates}\n ## Infrastucture Apps \n{infra_app_aliases}\n"
             for category in ["search", "format", "action", "setup", "misc"]:
                 result += f"\n\n## {category.capitalize()} Commands\n"
                 for part in parts:
                     if part.category == category:
                         result += f"- `{part.name}` - {part.info()}\n"
 
             result += dedent(
@@ -190,14 +197,16 @@
                 result += self.all_parts[arg].rendered_help(ctx)
             elif arg in self.alias_names:
                 alias = self.alias_names[arg]
                 explain = f"{arg} is an alias for {alias}\n\n"
                 result = explain + self.all_parts[alias].rendered_help(ctx)
             elif arg in self.alias_templates:
                 result = self.alias_templates[arg].rendered_help(ctx)
+            elif arg in self.infra_app_aliases:
+                result = self.infra_app_aliases[arg].rendered_help(ctx)
             else:
                 result = f"No command found with this name: {arg}"
 
             return stream.just(result)
 
         return CLISource.single(help_command)
 
@@ -217,24 +226,32 @@
 
     def __init__(
         self, dependencies: CLIDependencies, parts: List[CLICommand], env: Dict[str, Any], alias_names: Dict[str, str]
     ):
         dependencies.extend(cli=self)
         alias_templates_list = [AliasTemplate.from_config(cmd) for cmd in dependencies.config.custom_commands.commands]
         alias_templates = {a.name: a for a in alias_templates_list}
-        help_cmd = HelpCommand(dependencies, parts, alias_names, alias_templates)
+        infra_app_aliases: Dict[str, InfraAppAlias] = {}
+        help_cmd = HelpCommand(
+            dependencies,
+            parts,
+            alias_names,
+            alias_templates,
+            infra_app_aliases,
+        )
         cmds = {p.name: p for p in parts + [help_cmd]}
         alias_cmds = {alias: cmds[name] for alias, name in alias_names.items() if name in cmds and alias not in cmds}
         self.cli_env = env
         self.alias_names = alias_names
         self.__direct_commands = cmds
         self.__alias_commands = alias_cmds
         self.__commands: Dict[str, CLICommand] = {**cmds, **alias_cmds}
         self.__dependencies = dependencies
         self.__alias_templates = alias_templates
+        self.__infra_app_aliases = infra_app_aliases
         self.reaper: Optional[Task[None]] = None
 
     @property
     def direct_commands(self) -> Dict[str, CLICommand]:
         return self.__direct_commands
 
     @property
@@ -253,20 +270,42 @@
     def dependencies(self) -> CLIDependencies:
         return self.__dependencies
 
     @property
     def alias_templates(self) -> Dict[str, AliasTemplate]:
         return self.__alias_templates
 
+    @property
+    def infra_app_aliases(self) -> Dict[str, InfraAppAlias]:
+        return self.__infra_app_aliases
+
+    def _no_name_conflict(self, name: str) -> bool:
+        return (
+            name not in self.direct_commands
+            and name not in self.alias_commands
+            and name not in self.alias_templates
+            and name not in self.infra_app_aliases
+        )
+
+    def register_infra_app_alias(self, alias: InfraAppAlias) -> None:
+        """
+        Called when an infra app is registered.
+        """
+        if self._no_name_conflict(alias.name):
+            self.__infra_app_aliases[alias.name] = alias
+
+    def unregister_infra_app_alias(self, name: str) -> None:
+        del self.__infra_app_aliases[name]
+
     def register_alias_template(self, template: AliasTemplate) -> None:
         """
         Called when something introduces a custom command.
         The registered templated will always override any existing template.
         """
-        if template.name not in self.direct_commands and template.name not in self.alias_commands:
+        if self._no_name_conflict(template.name):
             self.alias_templates[template.name] = template
 
     def unregister_alias_template(self, name: str) -> None:
         """
         Called when something removes a custom command.
         """
         if name in self.alias_templates:
@@ -456,19 +495,26 @@
     ) -> List[ParsedCommandLine]:
         async def combine_query_parts(
             commands: List[ExecutableCommand], ctx: CLIContext
         ) -> Tuple[CLIContext, List[ExecutableCommand]]:
             parts = list(takewhile(lambda x: isinstance(x.command, SearchCLIPart), commands))
             if parts:
                 query, options, query_parts = await self.create_query(parts, ctx)
-                ctx_wq = evolve(ctx, query=query, query_options=options)
-                # re-evaluate remaining commands - to take the adapted context into account
-                remaining = [self.command(c.name, c.arg, ctx_wq) for c in commands[len(parts) :]]  # noqa: E203
-                return ctx_wq, [*query_parts, *remaining]
-            return ctx, commands
+                ctx_wq = evolve(ctx, query=query, query_options=options, commands=commands)
+                part_offset = len(parts)
+                remaining = [
+                    self.command(c.name, c.arg, ctx_wq, position=pos + part_offset)
+                    for pos, c in enumerate(commands[len(parts) :])
+                ]  # noqa: E203
+                rewritten_parts = [*query_parts, *remaining]
+            else:
+                ctx_wq = evolve(ctx, commands=commands)
+                rewritten_parts = [self.command(c.name, c.arg, ctx_wq, position=pos) for pos, c in enumerate(commands)]
+            # re-evaluate remaining commands - to take the adapted context into account
+            return ctx_wq, rewritten_parts
 
         def rewrite_command_line(cmds: List[ExecutableCommand], ctx: CLIContext) -> List[ExecutableCommand]:
             """
             Rewrite the command line to make it more user-friendly.
             Rules:
             - add the list command if no output format is defined
             - add a format to write commands if no output format is defined
@@ -511,21 +557,20 @@
             if isinstance(last_command, NoTerminalOutput) and ctx.console_renderer:
                 return evolve(ctx, env=cmd_env, console_renderer=ConsoleRenderer.default_renderer())
             else:
                 return evolve(context, env=cmd_env)
 
         async def parse_line(parsed: ParsedCommands) -> ParsedCommandLine:
             ctx = adjust_context(parsed)
-            ctx, commands = await combine_query_parts(
-                [self.command(c.cmd, c.args, ctx, position=i) for i, c in enumerate(parsed.commands)], ctx
-            )
-            rewritten = rewrite_command_line(commands, ctx)
-            not_met = [r for cmd in rewritten for r in cmd.action.required if r.name not in context.uploaded_files]
-            envelope = {k: v for cmd in rewritten for k, v in cmd.action.envelope.items()}
-            return ParsedCommandLine(ctx, parsed, rewritten, not_met, envelope)
+            executable = [self.command(c.cmd, c.args, ctx, position=i) for i, c in enumerate(parsed.commands)]
+            rewritten = rewrite_command_line(executable, ctx)
+            ctx, commands = await combine_query_parts(rewritten, ctx)
+            not_met = [r for cmd in commands for r in cmd.action.required if r.name not in context.uploaded_files]
+            envelope = {k: v for cmd in commands for k, v in cmd.action.envelope.items()}
+            return ParsedCommandLine(ctx, parsed, commands, not_met, envelope)
 
         def expand_aliases(line: ParsedCommands) -> ParsedCommands:
             def expand_alias(alias_cmd: ParsedCommand) -> List[ParsedCommand]:
                 alias: AliasTemplate = self.alias_templates[alias_cmd.cmd]
                 available: Dict[str, AliasTemplateParameter] = {p.name: p for p in alias.parameters}
                 props: Dict[str, JsonElement] = self.replacements(**{**self.cli_env, **context.env})  # type: ignore
                 props["args"] = alias_cmd.args or ""
@@ -543,32 +588,46 @@
                     raise AttributeError(
                         f"Alias {alias_cmd.cmd} not enough parameters provided. Missing: {', '.join(undefined)}"
                     )
                 rendered = alias.render(props)
                 log.debug(f"The rendered alias template is: {rendered}")
                 return single_commands.parse(rendered)  # type: ignore
 
+            def expand_infra_app_alias(alias_cmd: ParsedCommand) -> List[ParsedCommand]:
+                alias: InfraAppAlias = self.infra_app_aliases[alias_cmd.cmd]
+                props: Dict[str, JsonElement] = self.replacements(**{**self.cli_env, **context.env})  # type: ignore
+                props["args"] = alias_cmd.args or ""
+                rendered = alias.render(props)
+                log.debug(f"The rendered infra app alias template is: {rendered}")
+                return single_commands.parse(rendered)  # type: ignore
+
             result: List[ParsedCommand] = []
             for cmd in line.commands:
                 if cmd.cmd in self.alias_templates:
                     result.extend(expand_alias(cmd))
+                elif cmd.cmd in self.infra_app_aliases:
+                    result.extend(expand_infra_app_alias(cmd))
                 else:
                     result.append(cmd)
 
             return ParsedCommands(result, line.env)
 
         async def send_analytics(parsed: List[ParsedCommands], raw: List[ParsedCommands]) -> None:
             command_names = [cmd.cmd for line in parsed for cmd in line.commands]
             used_aliases = [cmd.cmd for line in raw for cmd in line.commands if cmd.cmd in self.alias_templates]
+            used_infra_app_aliases = [
+                cmd.cmd for line in raw for cmd in line.commands if cmd.cmd in self.infra_app_aliases
+            ]
             resoto_session_id = context.env.get("resoto_session_id")
             await self.dependencies.event_sender.core_event(
                 CoreEvent.CLICommand,
                 {
                     "command_names": command_names,
                     "used_aliases": used_aliases,
+                    "used_infra_app_aliases": used_infra_app_aliases,
                     "session_id": resoto_session_id,
                     "source": context.source or "unknown",
                 },
                 command_lines=len(parsed),
                 commands=len(command_names),
             )
```

### Comparing `resotocore-3.5.1/resotocore/cli/command.py` & `resotocore-3.5.2/resotocore/cli/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 import tempfile
 from abc import abstractmethod, ABC
 from argparse import Namespace
 from asyncio import Future, Task
 from asyncio.subprocess import Process
 from collections import defaultdict
 from contextlib import suppress
-from datetime import timedelta
+from datetime import timedelta, datetime
 from functools import partial, lru_cache
 from itertools import dropwhile, chain
 from tempfile import TemporaryDirectory
 from typing import (
     Dict,
     List,
     Tuple,
@@ -63,14 +63,15 @@
     is_node,
     js_value_at,
     js_value_get,
     key_values_parser,
     parse_time_or_delta,
     strip_quotes,
 )
+from resotocore.cli.dependencies import CLIDependencies
 from resotocore.cli.model import (
     CLICommand,
     CLIContext,
     EmptyContext,
     CLIAction,
     CLISource,
     CLIFlow,
@@ -79,20 +80,20 @@
     PreserveOutputFormat,
     MediaType,
     CLIFileRequirement,
     ParsedCommand,
     NoTerminalOutput,
     ArgsInfo,
     ArgInfo,
+    EntityProvider,
 )
-from resotocore.cli.dependencies import CLIDependencies
 from resotocore.cli.tip_of_the_day import SuggestionPolicy, SuggestionStrategy, get_suggestion_strategy
 from resotocore.config import ConfigEntity
 from resotocore.db.async_arangodb import AsyncCursor
-from resotocore.db.graphdb import HistoryChange
+from resotocore.db.graphdb import HistoryChange, GraphDB
 from resotocore.db.model import QueryModel
 from resotocore.db.runningtaskdb import RunningTaskData
 from resotocore.dependencies import system_info
 from resotocore.error import CLIParseError, ClientError, CLIExecutionError
 from resotocore.ids import ConfigId, TaskId, InfraAppName, TaskDescriptorId, GraphName, Email, Password
 from resotocore.infra_apps.manifest import AppManifest
 from resotocore.infra_apps.package_manager import Failure
@@ -166,15 +167,15 @@
 log = logging.getLogger(__name__)
 
 
 # A SearchCLIPart is a command that can be used on the command line.
 # Such a part is not executed, but builds a search, which is executed.
 # Therefore, the parse method is implemented in a dummy fashion here.
 # The real interpretation happens in CLI.create_query.
-class SearchCLIPart(CLICommand, ABC):
+class SearchCLIPart(CLICommand, EntityProvider, ABC):
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         return CLISource.empty()
 
 
 class SearchPart(SearchCLIPart):
     """
 
@@ -184,14 +185,15 @@
 
     This command allows to search the graph using filters, traversals, functions and aggregates.
 
     ## Options
 
     - `--with-edges`: Return edges in addition to nodes.
     - `--explain`: Instead of executing the search, analyze its cost.
+    - `--at <time|delta>`: Perform search on the snapshot of a graph just before the given time.
 
     ## Parameters
 
     - `search-statement` [mandatory]: The search to execute.
 
 
     ### Filters
@@ -351,14 +353,18 @@
     # Do not execute the search, but show an explanation of the search cost.
     > search --explain is(graph_root) -[0:1]->
     available_nr_items: 142670
     estimated_cost: 58569
     estimated_nr_items: 8
     full_collection_scan: false
     rating: simple
+
+    # Search all volumes on a snapshot from the past
+    > search --at 2023-05-07T12:34:56Z is(volume)
+    > search --at 1w is(volume)
     ```
 
     ## Environment Variables
 
     - `graph` [default=resoto]: the name of the graph to operate on.
     - `section` [default=reported]: interpret all property paths with respect to this section.
        With section `reported` set, the search `name=~"test"` would be interpreted as `reported.name=~"test"`.
@@ -377,14 +383,15 @@
     def info(self) -> str:
         return "Search the graph."
 
     def args_info(self) -> ArgsInfo:
         return [
             ArgInfo(expects_value=True, value_hint="search"),
             ArgInfo("--with-edges", help_text="include edges in result"),
+            ArgInfo("--at", help_text="timestamp | timedelta"),
         ]
 
 
 class HistoryPart(SearchCLIPart):
     """
     ```shell
     history [--before <time|delta>] [--after <time|delta>] [--change <change>] [search-statement]
@@ -1305,15 +1312,15 @@
                 tm, tu = (total, null_value) if arg else (null_value + total, 0)
                 yield f"total matched: {tm}"
                 yield f"total unmatched: {tu}"
 
         return CLIFlow(to_count)
 
 
-class ExecuteSearchCommand(CLICommand, InternalPart):
+class ExecuteSearchCommand(CLICommand, InternalPart, EntityProvider):
     """
     ```shell
     execute_search [--with-edges] [--explain] <search-statement>
     ```
 
     This command is usually not invoked directly - use `search` instead.
 
@@ -1345,14 +1352,15 @@
         parser = NoExitArgumentParser()
         parser.add_argument("--with-edges", dest="with-edges", default=None, action="store_true")
         parser.add_argument("--explain", dest="explain", default=None, action="store_true")
         parser.add_argument("--history", dest="history", default=None, action="store_true")
         parser.add_argument("--after", dest="after", default=None)
         parser.add_argument("--before", dest="before", default=None)
         parser.add_argument("--change", dest="change", default=None)
+        parser.add_argument("--at", dest="at", default=None)
         try:
             # try to parse as many arguments as possible
             args, remaining = args_parts_parser.parse_partial(arg)
             # try to parse the parsed arguments
             parsed, rest = parser.parse_known_args(list(args))
             parsed_args = {k: v for k, v in vars(parsed).items() if v is not None}
             # join the unparsed arguments and the remaining arg string
@@ -1370,41 +1378,66 @@
             result.append(f"--{key}")
             if value is not True:
                 result.append(f"'{value}'")  # put the value into single quotes to maintain the spaces
         return " ".join(result) + " " if result else ""
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLISource:
         # db name is coming from the env
-        graph_name = ctx.graph_name
+        current_graph_name = ctx.graph_name
         if not arg:
             raise CLIParseError("search command needs a search-statement to execute, but nothing was given!")
 
+        def parse_at(x: Optional[str]) -> Optional[datetime]:
+            if x is None:
+                return None
+            try:
+                return parse_time_or_delta(strip_quotes(x))
+            except Exception as ex:
+                raise CLIParseError(f"Could not parse {x} as timestamp or timedelta.") from ex
+
         # Read all argument flags / options
         parsed, rest = self.parse_known(arg)
         with_edges: bool = parsed.get("with-edges", False)
         explain: bool = parsed.get("explain", False)
         history: bool = parsed.get("history", False)
+        at: Optional[datetime] = parse_at(parsed.get("at", None))
 
         # all templates are expanded at this point, so we can call the parser directly.
         query = parse_query(rest, **ctx.env)
-        db = self.dependencies.db_access.get_graph_db(graph_name)
 
-        async def load_query_model() -> QueryModel:
+        async def get_db(at: Optional[datetime], graph_name: GraphName) -> Tuple[GraphDB, GraphName]:
+            db_access = cast(CLIDependencies, self.dependencies).db_access
+            if at:
+                # if we search at some specific time: find a snapshot at that time
+                snapshot_name = await cast(CLIDependencies, self.dependencies).graph_manager.snapshot_at(
+                    time=at, graph_name=graph_name
+                )
+                if not snapshot_name:
+                    raise CLIParseError(f"No graph snapshot at {at} found for graph {graph_name}.")
+
+                return db_access.get_graph_db(snapshot_name), snapshot_name
+
+            return db_access.get_graph_db(graph_name), graph_name
+
+        async def load_query_model(db: GraphDB, graph_name: GraphName) -> QueryModel:
             model = await self.dependencies.model_handler.load_model(graph_name)
             query_model = QueryModel(query, model)
             await db.to_query(query_model)  # only here to validate the query itself (can throw)
             return query_model
 
         async def explain_search() -> AsyncIterator[Json]:
-            query_model = await load_query_model()
+            db, graph_name = await get_db(at, current_graph_name)
+            query_model = await load_query_model(db, graph_name)
             explanation = await db.explain(query_model, with_edges)
             yield to_js(explanation)
 
         async def prepare() -> Tuple[Optional[int], AsyncIterator[Json]]:
-            query_model = await load_query_model()
+            db, graph_name = await get_db(at, current_graph_name)
+
+            query_model = await load_query_model(db, graph_name)
             count = ctx.env.get("count", "true").lower() != "false"
             timeout = if_set(ctx.env.get("search_timeout"), duration)
             if history:
                 before = if_set(parsed.get("before"), lambda x: parse_time_or_delta(strip_quotes(x)))  # type: ignore
                 after = if_set(parsed.get("after"), lambda x: parse_time_or_delta(strip_quotes(x)))  # type: ignore
                 change = if_set(parsed.get("change"), lambda x: HistoryChange[strip_quotes(x)])  # type: ignore
                 context = await db.search_history(query_model, change, before, after, timeout=timeout)
@@ -1887,30 +1920,30 @@
             else:
                 result = sorted([k.fqn for k in model.kinds.values() if isinstance(k, ComplexKind) and show(k)])
                 return len(model.kinds), stream.iterate(result)
 
         return CLISource(source)
 
 
-class SetDesiredStateBase(CLICommand, ABC):
+class SetDesiredStateBase(CLICommand, EntityProvider, ABC):
     @abstractmethod
     def patch(self, arg: Optional[str], ctx: CLIContext) -> Json:
         # deriving classes need to define how to patch
         pass
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIFlow:
         buffer_size = 1000
         func = partial(self.set_desired, arg, ctx.graph_name, self.patch(arg, ctx))
         return CLIFlow(lambda in_stream: stream.flatmap(stream.chunks(in_stream, buffer_size), func))
 
     async def set_desired(
         self, arg: Optional[str], graph_name: GraphName, patch: Json, items: List[Json]
     ) -> AsyncIterator[JsonElement]:
         model = await self.dependencies.model_handler.load_model(graph_name)
-        db = self.dependencies.db_access.get_graph_db(graph_name)
+        db = cast(CLIDependencies, self.dependencies).db_access.get_graph_db(graph_name)
         node_ids = []
         for item in items:
             if "id" in item:
                 node_ids.append(item["id"])
             elif isinstance(item, str):
                 node_ids.append(item)
         async for update in db.update_nodes_desired(model, patch, node_ids):
@@ -2023,28 +2056,28 @@
             r_id = js_value_get(elem, NodePath.reported_id, "<no id>")
             r_name = js_value_get(elem, NodePath.reported_name, "<no name>")
             r_kind = js_value_get(elem, NodePath.reported_kind, "<no kind>")
             log.info(f"Node id={r_id}, name={r_name}, kind={r_kind} marked for cleanup. {reason}. ({uid})")
             yield elem
 
 
-class SetMetadataStateBase(CLICommand, ABC):
+class SetMetadataStateBase(CLICommand, EntityProvider, ABC):
     @abstractmethod
     def patch(self, arg: Optional[str], ctx: CLIContext) -> Json:
         # deriving classes need to define how to patch
         pass
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIFlow:
         buffer_size = 1000
         func = partial(self.set_metadata, ctx.graph_name, self.patch(arg, ctx))
         return CLIFlow(lambda in_stream: stream.flatmap(stream.chunks(in_stream, buffer_size), func))
 
     async def set_metadata(self, graph_name: GraphName, patch: Json, items: List[Json]) -> AsyncIterator[JsonElement]:
         model = await self.dependencies.model_handler.load_model(graph_name)
-        db = self.dependencies.db_access.get_graph_db(graph_name)
+        db = cast(CLIDependencies, self.dependencies).db_access.get_graph_db(graph_name)
         node_ids = []
         for item in items:
             if "id" in item:
                 node_ids.append(item["id"])
             elif isinstance(item, str):
                 node_ids.append(item)
         async for update in db.update_nodes_metadata(model, patch, node_ids):
@@ -3014,15 +3047,15 @@
 
     def update_node_in_graphdb(self, model: Model, **env: str) -> Callable[[WorkerTask, Future[Json]], Awaitable[Json]]:
         async def to_result(task: WorkerTask, future_result: Future[Json]) -> Json:
             nid = js_value_at(task.data, ["node", "id"])
             try:
                 result = await future_result
                 if is_node(result):
-                    db = self.dependencies.db_access.get_graph_db(GraphName(env["graph"]))
+                    db = cast(CLIDependencies, self.dependencies).db_access.get_graph_db(GraphName(env["graph"]))
                     try:
                         updated: Json = await db.update_node(model, result["id"], result, True, None)
                         return updated
                     except ClientError as ex:
                         # if the change could not be reflected in database, show success
                         log.warning(
                             f"Update not reflected in db. Wait until next collector run. Reason: {str(ex)}",
@@ -3428,15 +3461,15 @@
             "info": [],
         }
 
     async def create_backup(self, arg: Optional[str]) -> AsyncIterator[str]:
         temp_dir: str = tempfile.mkdtemp()
         maybe_proc: Optional[Process] = None
         try:
-            db_config = self.dependencies.config.db
+            db_config = cast(CLIDependencies, self.dependencies).config.db
             if not shutil.which("arangodump"):
                 raise CLIParseError("db_backup expects the executable `arangodump` to be in path!")
             # fmt: off
             process = await asyncio.create_subprocess_exec(
                 "arangodump",
                 "--progress", "false",  # do not show progress
                 "--include-system-collections", "true",  # graphs are considered a system collection
@@ -3492,15 +3525,15 @@
         maybe_proc: Optional[Process] = None
         try:
             # extract tar file
             with tarfile.open(backup_file, "r") as tar:
                 tar.extractall(temp_dir, members=safe_members_in_tarfile(tar))
 
             # fmt: off
-            db_conf = self.dependencies.config.db
+            db_conf = cast(CLIDependencies, self.dependencies).config.db
             process = await asyncio.create_subprocess_exec(
                 "arangorestore",
                 "--progress", "false",  # do not show progress
                 "--include-system-collections", "true",  # graphs are considered a system collection
                 "--threads", "8",  # default is 2
                 "--log.level", "error",  # only print error messages
                 "--input-directory", temp_dir,  # directory to write to
@@ -3716,15 +3749,17 @@
         async def list_templates() -> Tuple[Optional[int], AsyncIterator[Json]]:
             templates = await self.dependencies.template_expander.list_templates()
             return len(templates), stream.iterate(template_str(t) for t in templates)
 
         async def put_template(name: str, template_query: str) -> AsyncIterator[str]:
             # try to render_console the template with dummy values and see if the search can be parsed
             try:
-                rendered_query = self.dependencies.template_expander.render(template_query, defaultdict(lambda: True))
+                rendered_query = cast(CLIDependencies, self.dependencies).template_expander.render(
+                    template_query, defaultdict(lambda: True)
+                )
                 parse_query(rendered_query, **ctx.env)
             except Exception as ex:
                 raise CLIParseError(f"Given template does not define a valid search: {template_query}") from ex
             await self.dependencies.template_expander.put_template(Template(name, template_query))
             yield f"Template {name} added to the search library.\n{template_query}"
 
         async def delete_template(name: str) -> AsyncIterator[str]:
@@ -4622,15 +4657,15 @@
             ]
         }
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         async def create_certificate(
             common_name: str, dns_names: List[str], ip_addresses: List[str], days_valid: int
         ) -> AsyncIterator[str]:
-            key, cert = self.dependencies.cert_handler.create_key_and_cert(
+            key, cert = cast(CLIDependencies, self.dependencies).cert_handler.create_key_and_cert(
                 common_name, dns_names, ip_addresses, days_valid
             )
             with TemporaryDirectory() as tmpdir:
                 key_file = os.path.join(tmpdir, f"{common_name}.key")
                 cert_file = os.path.join(tmpdir, f"{common_name}.crt")
                 write_cert_to_file(cert, cert_file, rename=False)
                 write_key_to_file(key, key_file, rename=False)
@@ -4652,23 +4687,31 @@
                 2,
                 produces=MediaType.FilePath,
             )
         else:
             return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
 
 
-class ReportCommand(CLICommand):
+class ReportCommand(CLICommand, EntityProvider):
     """
     ```shell
     report benchmarks list
     report benchmark show <benchmark-id>
-    report benchmark run <benchmark-id> [--accounts <account-id>] [--severity <level>] [--only-failing]
+    report benchmark run <benchmark-id>
+                         [--accounts <account-id>]
+                         [--severity <level>]
+                         [--only-failing]
+                         [--only-check-results]
     report checks list
     report checks show <check-id>
-    report checks run <check-id> [--accounts <account-id>] [--severity <level>] [--only-failing]
+    report checks run <check-id>
+                      [--accounts <account-id>]
+                      [--severity <level>]
+                      [--only-failing]
+                      [--only-check-results]
     ```
 
     List and run benchmarks as well as specific benchmark checks.
     Benchmarks are a collection of checks that are run against all or specific accounts.
     Every check has a severity, that can also be used to filter relevant checks.
 
     The result of a benchmark run is a report in Markdown format.
@@ -4678,14 +4721,16 @@
     ## Parameters
     - `--accounts` [optional]: List of account ids (space separated) to run the benchmark against.
         If not specified, the benchmark is run against all accounts.
     - `--severity` [optional]: Severity level to filter checks. One of `info`, `low`, `medium`, `high`, `critical`
 
     ## Options
     - `--only-failing` [optional]: Only include checks that are failing in the report.
+    - `--only-check-results` [optional]: Only include the check result, not the benchmark structure in the report.
+                                         This is useful, if you want to process the result with other action commands.
 
     ## Examples
 
     ```shell
     # List all available chekcs
     > report checks list
     aws_apigateway_authorizers_enabled
@@ -4733,14 +4778,15 @@
             ArgInfo(
                 "--severity",
                 True,
                 help_text="The severity level to filter checks",
                 possible_values=[s.value for s in ReportSeverity],
             ),
             ArgInfo("--only-failing", False, help_text="Filter only failing checks."),
+            ArgInfo("--only-check-results", False, help_text="Only dump results."),
         ]
         return {
             "benchmark": {
                 "list": [],
                 "run": [ArgInfo(None, help_text="<benchmark-id>"), *run_args],
                 "show": [ArgInfo(None, help_text="<benchmark-id>")],
             },
@@ -4799,37 +4845,38 @@
                 ctx.graph_name,
                 parsed_args.identifier,
                 accounts=parsed_args.accounts,
                 severity=parsed_args.severity,
                 only_failing=parsed_args.only_failing,
             )
             if not result.is_empty():
-                for node in result.to_graph():
+                for node in result.to_graph(parsed_args.only_check_results):
                     yield node
 
         async def run_check(parsed_args: Namespace) -> AsyncIterator[Json]:
             result = await self.dependencies.inspector.perform_checks(
                 ctx.graph_name,
                 check_ids=[parsed_args.identifier],
                 accounts=parsed_args.accounts,
                 severity=parsed_args.severity,
                 only_failing=parsed_args.only_failing,
             )
             if not parsed_args.only_failing or result.has_failed():
-                for node in result.to_graph():
+                for node in result.to_graph(parsed_args.only_check_results):
                     yield node
 
         async def show_help() -> AsyncIterator[str]:
             yield f"Do not understand: {arg}\n\n" + self.rendered_help(ctx)
 
         run_parser = NoExitArgumentParser()
         run_parser.add_argument("identifier")
         run_parser.add_argument("--accounts", nargs="+")
         run_parser.add_argument("--severity", type=ReportSeverity, choices=list(ReportSeverity))
         run_parser.add_argument("--only-failing", action="store_true", default=False)
+        run_parser.add_argument("--only-check-results", action="store_true", default=False)
 
         action = self.action_from_arg(arg)
         args = re.split("\\s+", arg.strip(), maxsplit=2) if arg else []
         if action == "benchmark_list":
             return CLISource.no_count(list_benchmarks)
         elif action == "benchmark_show":
             return CLISource.no_count(partial(show_benchmark, args[2].strip()))
@@ -4843,15 +4890,15 @@
         elif action == "check_run":
             parsed = run_parser.parse_args(args[2].split() if len(args) > 2 else [])
             return CLISource.no_count(partial(run_check, parsed))
         else:
             return CLISource.single(show_help)
 
 
-class InfrastructureAppsCommand(CLICommand):
+class AppsCommand(CLICommand):
     """
     ```shell
     apps search [pattern] [--index-url https://cdn.some.engineering/resoto/apps/index.json]
     app info <app_name> [--index-url https://cdn.some.engineering/resoto/apps/index.json]
     app install <app_name> [--index-url https://cdn.some.engineering/resoto/apps/index.json]
     app edit <app_name>
     app uninstall <app_name>
@@ -4999,16 +5046,21 @@
             config = config or f"resoto.apps.{app_name}"
             ce = await self.dependencies.config_handler.get_config(ConfigId(config))
             if ce:
                 app_config = ce.config
             else:
                 raise ValueError(f"Config {config} not found.")
 
+            async def stream_to_iterator(in_stream: Stream) -> AsyncIterator[JsonElement]:
+                async with in_stream.stream() as streamer:
+                    async for item in streamer:
+                        yield item
+
             stdin: AsyncIterator[JsonElement] = (
-                stream.iterate(in_stream) if isinstance(in_stream, Stream) else in_stream
+                stream_to_iterator(in_stream) if isinstance(in_stream, Stream) else in_stream
             )
 
             if dry_run:
                 return runtime.generate_template(
                     graph=ctx.graph_name,
                     manifest=manifest,
                     config=app_config,
@@ -5308,15 +5360,15 @@
             return CLISource.single(lambda: stream.just(self.rendered_help(ctx)))
 
 
 class GraphCommand(CLICommand):
     """
     ```shell
     graph list [pattern]
-    graph copy [-force] [from_graph_namae] <to_graph_name>
+    graph copy [--force] [from_graph_namae] <to_graph_name>
     graph snapshot [from_graph_name] <snapshot_label>
     graph delete <graph_name>
     graph export [--force] [graph_name] <file_name>
     graph import [--force] [graph_name] <file_name>
     ```
 
     - `graph list [pattern]`: Lists all graphs. Supports filtering by pattern.
@@ -5410,15 +5462,15 @@
                 yield path
             finally:
                 shutil.rmtree(temp_dir)
 
         async def graph_export(graph_name: Optional[GraphName], file_name: str) -> AsyncIterator[JsonElement]:
             if not graph_name:
                 graph_name = ctx.graph_name
-            lines = self.dependencies.graph_manager.export_graph(graph_name)
+            lines = cast(CLIDependencies, self.dependencies).graph_manager.export_graph(graph_name)
             return write_result_to_file(lines, file_name)
 
         async def graph_import(
             graph_name: Optional[GraphName], file_name: str, force: bool
         ) -> AsyncIterator[JsonElement]:
             if not graph_name:
                 graph_name = ctx.graph_name
@@ -5506,15 +5558,15 @@
         DumpCommand(d, "format"),
         EchoCommand(d, "misc", allowed_in_source_position=True),
         EnvCommand(d, "misc", allowed_in_source_position=True),
         ExecuteTaskCommand(d, "action", allowed_in_source_position=True),
         ExecuteSearchCommand(d, "search", allowed_in_source_position=True),
         FlattenCommand(d, "misc"),
         FormatCommand(d, "format"),
-        HeadCommand(d, "misc"),
+        HeadCommand(d, "search"),
         HistoryPart(d, "search", allowed_in_source_position=True),
         HttpCommand(d, "action"),
         JobsCommand(d, "action", allowed_in_source_position=True),
         JqCommand(d, "misc"),
         JsonCommand(d, "misc", allowed_in_source_position=True),
         KindsCommand(d, "search", allowed_in_source_position=True),
         LimitPart(d, "search"),
@@ -5527,23 +5579,23 @@
         SetDesiredCommand(d, "action"),
         SetMetadataCommand(d, "action"),
         SleepCommand(d, "misc", allowed_in_source_position=True),
         SortPart(d, "search"),
         SuccessorsPart(d, "search"),
         SystemCommand(d, "setup", allowed_in_source_position=True),
         TagCommand(d, "action"),
-        TailCommand(d, "misc"),
+        TailCommand(d, "search"),
         UniqCommand(d, "misc"),
         UserCommand(d, "setup", allowed_in_source_position=True),
         WorkflowsCommand(d, "action", allowed_in_source_position=True),
         WelcomeCommand(d, "misc", allowed_in_source_position=True),
         TipOfTheDayCommand(d, "misc", allowed_in_source_position=True),
         WriteCommand(d, "misc"),
-        InfrastructureAppsCommand(d, "apps", allowed_in_source_position=True),
-        GraphCommand(d, "graph", allowed_in_source_position=True),
+        AppsCommand(d, "misc", allowed_in_source_position=True),
+        GraphCommand(d, "setup", allowed_in_source_position=True),
     ]
     # commands that are only available when the system is started in debug mode
     if d.config.runtime.debug:
         commands.extend(
             [
                 FileCommand(d, "misc"),
                 UploadCommand(d, "misc"),
```

### Comparing `resotocore-3.5.1/resotocore/cli/dependencies.py` & `resotocore-3.5.2/resotocore/cli/dependencies.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/cli/model.py` & `resotocore-3.5.2/resotocore/cli/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 import inspect
 import json
 from abc import ABC, abstractmethod
 from asyncio import iscoroutine
 from datetime import timedelta
 from enum import Enum
 from functools import reduce
-from operator import attrgetter
 from textwrap import dedent
 from typing import Optional, List, Any, Dict, Tuple, Callable, Union, Awaitable, Type, cast, Set, AsyncIterator
 
 from aiostream import stream
 from aiostream.core import Stream
 from attrs import define, field
 from parsy import test_char, string
@@ -61,24 +60,29 @@
 
 @define(frozen=True)
 class CLIContext:
     env: Dict[str, str] = field(factory=dict)
     uploaded_files: Dict[str, str] = field(factory=dict)  # id -> path
     query: Optional[Query] = None
     query_options: Dict[str, Any] = field(factory=dict)
+    commands: List[ExecutableCommand] = field(factory=list)
     console_renderer: Optional[ConsoleRenderer] = None
     source: Optional[str] = None  # who is calling
 
     @property
     def graph_name(self) -> GraphName:
         return GraphName(self.env["graph"])
 
     def variable_in_section(self, variable: str) -> str:
-        # if there is no query, always assume the root section
-        section = self.env.get("section") if self.query else PathRoot
+        # if there is no entity provider, always assume the root section
+        section = (
+            self.env.get("section")
+            if self.query or self.commands and isinstance(self.commands[0].command, EntityProvider)
+            else PathRoot
+        )
         return variable_to_absolute(section, variable)
 
     def render_console(self, element: Union[str, JupyterMixin]) -> str:
         if self.console_renderer:
             return self.console_renderer.render(element)
         elif isinstance(element, JupyterMixin):
             return str(element)
@@ -326,33 +330,87 @@
 @define(order=True, hash=True, frozen=True)
 class AliasTemplateParameter:
     name: str
     description: str
     default: Optional[JsonElement] = None
 
     def example_value(self) -> JsonElement:
-        return self.default if self.default else f"test_{self.name}"
+        return self.default if self.default else f"test-{self.name.replace('_', '-')}"
+
+    @property
+    def arg_name(self) -> str:
+        return "--" + self.name.replace("_", "-")
+
+
+@define(order=True, hash=True, frozen=True)
+class InfraAppAliasParameter:
+    name: str
+    help: str
+    default: Optional[JsonElement]
 
     @property
     def arg_name(self) -> str:
         return "--" + self.name.replace("_", "-")
 
 
 # pylint: disable=not-an-iterable
 @define(order=True, hash=True, frozen=True)
+class InfraAppAlias:
+    name: str
+    description: str
+    readme: str
+    parameters: List[InfraAppAliasParameter]
+
+    def template(self) -> str:
+        return f"apps run {self.name}" + r" {{args}}"
+
+    def render(self, props: Json) -> str:
+        return render_template(self.template(), props)
+
+    def help(self) -> str:
+        args = " ".join(f"{arg.arg_name} <value>" for arg in self.parameters)
+
+        indent = "        "
+        desc = ""
+        if self.readme:
+            for line in self.readme.splitlines():
+                desc += f"\n{indent}{line}"
+
+        def param_info_infra_apps(param: InfraAppAliasParameter) -> str:
+            default = f" [default: {param.default}]" if param.default else " [required]"
+            return f"- `{param.arg_name}`{default}: {param.help}"
+
+        arg_info = f"\n{indent}".join(param_info_infra_apps(param) for param in (self.parameters or []))
+        result = dedent(
+            f"""
+        {self.name}: {self.description}
+        ```shell
+        {self.name} {args}
+        ```
+        {desc}
+        ## Parameters
+        {arg_info}"""
+        )
+        return result
+
+    def rendered_help(self, ctx: CLIContext) -> str:
+        return ctx.render_console(self.help())
+
+
+# pylint: disable=not-an-iterable
+@define(order=True, hash=True, frozen=True)
 class AliasTemplate:
     name: str
     info: str
     template: str
     parameters: List[AliasTemplateParameter] = field(factory=list)
     description: Optional[str] = None
     # only use args_description if the template does not use explicit parameters
     args_description: Dict[str, str] = field(factory=dict)
     allowed_in_source_position: bool = False
-    infra_app_parameters: Optional[Dict[str, Any]] = None  # todo: remove this abomination
 
     def render(self, props: Json) -> str:
         return render_template(self.template, props)
 
     def args_info(self) -> ArgsInfo:
         args_desc = [ArgInfo(name, expects_value=True, help_text=desc) for name, desc in self.args_description.items()]
         param = [
@@ -365,46 +423,28 @@
         ]
         return args_desc + param
 
     def help_with_params(self) -> str:
         args = " ".join(f"{arg.arg_name} <value>" for arg in self.parameters)
 
         def param_info(p: AliasTemplateParameter) -> str:
-            default = f" [default: {p.default}]" if p.default else ""
-            return f"- `{p.name}`{default}: {p.description}"
+            default = f" [default: {p.default}]" if p.default else " [required]"
+            return f"- `{p.arg_name}`{default}: {p.description}"
+
+        def sort_required_name(p: AliasTemplateParameter) -> Any:
+            return p.default is not None, p.name
 
         indent = "            "
-        arg_info = f"\n{indent}".join(param_info(arg) for arg in sorted(self.parameters, key=attrgetter("name")))
+        arg_info = f"\n{indent}".join(param_info(arg) for arg in sorted(self.parameters, key=sort_required_name))
         minimal = " ".join(f'{p.arg_name} "{p.example_value()}"' for p in self.parameters if p.default is None)
         desc = ""
         if self.description:
             for line in self.description.splitlines():
                 desc += f"\n{indent}{line}"
 
-        if self.infra_app_parameters:
-
-            def param_info_infra_apps(name: str, arg_info: Dict[str, Any]) -> str:
-                default = f" [default: {arg_info.get('default')}]" if arg_info.get("default") else ""
-                return f"- `{name}`{default}: {arg_info.get('help')}"
-
-            arg_info = f"\n{indent}".join(
-                param_info_infra_apps(name, arg) for name, arg in self.infra_app_parameters.items()
-            )
-            result = dedent(
-                f"""
-            {self.name}: {self.info}
-            ```shell
-            {self.name} {args}
-            ```
-            {desc}
-            ## Parameters
-            {arg_info}"""
-            )
-            return result
-
         return dedent(
             f"""
             {self.name}: {self.info}
             ```shell
             {self.name} {args}
             ```
             {desc}
@@ -436,16 +476,14 @@
         args_info = args_info or ("<args>" if "{args}" in self.template else "")
         return (
             f"{self.name}: {self.info}\n```shell\n{self.name} {args}\n```\n\n"
             f"## Parameters\n{args_info}\n\n{self.description}\n\n"
         )
 
     def help(self) -> str:
-        if self.infra_app_parameters:  # todo: remove this abomination
-            return self.help_with_params()
         return self.help_with_params() if self.parameters else self.help_no_params_args()
 
     def rendered_help(self, ctx: CLIContext) -> str:
         return ctx.render_console(self.help())
 
     @staticmethod
     def from_config(cfg: AliasTemplateConfig) -> AliasTemplate:
@@ -493,14 +531,20 @@
 class InternalPart(ABC):
     """
     Internal parts can be executed but are not shown via help.
     They usually get injected by the CLI Interpreter to ease usability.
     """
 
 
+class EntityProvider(ABC):
+    """
+    Mark this command as a provider of entities with: id, reported, desired, metadata.
+    """
+
+
 class OutputTransformer(ABC):
     """
     Mark all commands that transform the output stream (formatting).
     """
 
 
 class PreserveOutputFormat(ABC):
@@ -597,14 +641,22 @@
         pass
 
     @abstractmethod
     async def execute_cli_command(self, cli_input: str, sink: Sink[T], ctx: CLIContext = EmptyContext) -> List[T]:
         pass
 
     @abstractmethod
+    def register_infra_app_alias(self, alias: InfraAppAlias) -> None:
+        pass
+
+    @abstractmethod
+    def unregister_infra_app_alias(self, name: str) -> None:
+        pass
+
+    @abstractmethod
     def register_alias_template(self, template: AliasTemplate) -> None:
         """
         Called when something introduces a custom command.
         """
 
     @abstractmethod
     def unregister_alias_template(self, name: str) -> None:
@@ -638,14 +690,19 @@
         pass
 
     @property
     @abstractmethod
     def alias_templates(self) -> Dict[str, AliasTemplate]:
         pass
 
+    @property
+    @abstractmethod
+    def infra_app_aliases(self) -> Dict[str, InfraAppAlias]:
+        pass
+
     @staticmethod
     def replacements(**env: str) -> Dict[str, str]:
         now_string = env.get("now")
         ut = from_utc(now_string) if now_string else utc()
         t = ut.date()
         try:
             n = ut.astimezone(get_local_tzinfo())
```

### Comparing `resotocore-3.5.1/resotocore/cli/tip_of_the_day.py` & `resotocore-3.5.2/resotocore/cli/tip_of_the_day.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/config/__init__.py` & `resotocore-3.5.2/resotocore/config/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from __future__ import annotations
 
 from abc import ABC, abstractmethod
-from attrs import define
-from typing import Any, Dict, Optional, AsyncIterator, List, cast, Callable, Awaitable
+from typing import Any, Dict, Optional, AsyncIterator, List, Callable, Awaitable
 
+from attrs import define
 from jsons import set_deserializer, set_serializer
 
+from resotocore.ids import ConfigId
 from resotocore.model.model import Model, Kind
 from resotocore.types import Json
-from resotocore.ids import ConfigId
 from resotocore.util import value_in_path, value_in_path_get
 
 
 @define(order=True, hash=True, frozen=True)
 class ConfigEntity:
     id: ConfigId
     config: Json
@@ -21,15 +21,15 @@
     def analytics(self) -> Dict[str, Any]:
         analytics: Dict[str, Any] = {"config_id": self.id}
         if "resotoworker" not in self.config:
             return analytics
 
         # provider information
         collectors: List[str] = []
-        collectors.extend(cast(List[str], value_in_path(self.config, ["resotoworker", "collector"])))
+        collectors.extend(value_in_path_get(self.config, ["resotoworker", "collector"], []))
         if "example" in collectors:
             collectors.remove("example")
         analytics["how_many_providers"] = len(collectors)
 
         # authentication information
         if "aws" in collectors:
             aws_use_access_secret_key = (
```

### Comparing `resotocore-3.5.1/resotocore/config/config_handler_service.py` & `resotocore-3.5.2/resotocore/config/config_handler_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/config/config_override_service.py` & `resotocore-3.5.2/resotocore/config/config_override_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/config/core_config_handler.py` & `resotocore-3.5.2/resotocore/config/core_config_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/console_renderer.py` & `resotocore-3.5.2/resotocore/console_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/constants.py` & `resotocore-3.5.2/resotocore/constants.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/core_config.py` & `resotocore-3.5.2/resotocore/core_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -383,18 +383,21 @@
             ),
             template=(
                 # aggregate the result by cloud -> account -> region -> resource
                 # resulting structure looks like this:
                 # {"aws": {"account1": {"region1": {"id1": {"id": "xxx", "name": "yyy", "kind": "zzz" }}}}}
                 # note: Pagerduty is able to render JSON objects in their webUI, but not arrays.
                 "head 100 | chunk 100 | jq --no-rewrite '"
+                "{{#group_resources}}"
                 '[group_by(.ancestors.cloud.reported.name) | .[] | {(.[0].ancestors.cloud.reported.name // "no-cloud"): '  # noqa: E501
                 '[group_by(.ancestors.account.reported.name) | .[] | {(.[0].ancestors.account.reported.name // "no-account"): '  # noqa: E501
                 '[group_by(.ancestors.region.reported.name) | .[] | {(.[0].ancestors.region.reported.name // "no-region"): '  # noqa: E501
-                "[.[] | {(.id): {id: .reported.id, name: .reported.name, kind: .reported.kind}}] | add }] | add }] | add }] | add'"  # noqa: E501
+                "{{/group_resources}}"
+                "[.[] | {({{resource_id}}): { {{#resource_properties.as_list.with_index}}{{key}}: {{value}}{{^last}},{{/last}}{{/resource_properties.as_list.with_index}} }}] | add "  # noqa: E501
+                "{{#group_resources}}}] | add }] | add }] | add {{/group_resources}}'"
                 "| jq --no-rewrite '{payload: "
                 '{summary: "{{summary}}", '
                 'timestamp: "@utc@", '
                 'source:"{{source}}", '
                 'severity: "{{severity}}", '
                 'component: "{{component}}", '
                 "custom_details: .}, "
@@ -441,14 +444,29 @@
                     "https://resoto.com",
                 ),
                 AliasTemplateParameterConfig(
                     "webhook_url",
                     "The complete url of the pagerduty events API.",
                     "https://events.pagerduty.com/v2/enqueue",
                 ),
+                AliasTemplateParameterConfig(
+                    "group_resources",
+                    "Group Resource by cloud, account, and region.",
+                    True,
+                ),
+                AliasTemplateParameterConfig(
+                    "resource_id",
+                    "Property to show as resource identifier.",
+                    ".id",
+                ),
+                AliasTemplateParameterConfig(
+                    "resource_properties",
+                    "Dictionary of properties to show.",
+                    dict(id=".reported.id", name=".reported.name", kind=".reported.kind"),
+                ),
             ],
             allowed_in_source_position=False,
         ),
     ]
 
 
 @define()
@@ -659,15 +677,15 @@
         factory=lambda: {"collect_and_cleanup": WorkflowConfig(schedule="0 * * * *")},
         metadata={"description": "Workflow related properties."},
     )
 
 
 def config_model() -> List[Json]:
     config_classes = {EditableConfig, CustomCommandsConfig}
-    return dataclasses_to_resotocore_model(config_classes, allow_unknown_props=False)
+    return dataclasses_to_resotocore_model(config_classes, use_optional_as_required=True)
 
 
 # Define rules to validate this config
 # Note: since validation rules do not cover all attributes, we allow unknown properties explicitly.
 schema_registry.add(
     schema_name(EditableConfig),
     dict(
```

### Comparing `resotocore-3.5.1/resotocore/db/__init__.py` & `resotocore-3.5.2/resotocore/db/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/db/arango_query.py` & `resotocore-3.5.2/resotocore/db/arango_query.py`

 * *Files 0% similar despite different names*

```diff
@@ -434,15 +434,15 @@
                 direction = "OUTBOUND" if nav.direction == Direction.outbound else "INBOUND"
                 unique = "uniqueEdges: 'path'" if with_edges else "uniqueVertices: 'global'"
                 pre, term_string = term(crsr, cl.term) if cl.term else (None, "true")
                 pre_string = pre + " FILTER" if pre else "FILTER"
                 filter_clause = f"({term_string})"
                 inner = traversal_filter(cl.with_clause, crsr, depth + 1) if cl.with_clause else ""
                 filter_root = f"({l0crsr}._key=={crsr}._key) or " if depth > 0 else ""
-                edge_type_traversals = f", {direction} ".join(db.edge_collection(et) for et in nav.edge_types)
+                edge_type_traversals = f", {direction} ".join(f"`{db.edge_collection(et)}`" for et in nav.edge_types)
                 return (
                     f"FOR {crsr} IN 0..{nav.until} {direction} {in_crs} "
                     f"{edge_type_traversals} OPTIONS {{ bfs: true, {unique} }} "
                     f"{pre_string} {filter_root}{filter_clause} "
                 ) + inner
 
             def collect_filter(cl: WithClause, depth: int) -> str:
@@ -496,15 +496,15 @@
             else:
                 graph_cursor = in_c
                 outer_for = f"FOR {in_c} in {in_crsr} "
 
             query_part += (
                 f"LET {out} =({outer_for}"
                 f"FOR {out_crsr}{link_str} IN {start}..{until} {dir_bound} {graph_cursor} "
-                f"{db.edge_collection(edge_type)} OPTIONS {{ bfs: true, {unique} }} "
+                f"`{db.edge_collection(edge_type)}` OPTIONS {{ bfs: true, {unique} }} "
                 f"RETURN DISTINCT {inout_result}) "
             )
             return out
 
         def navigation(in_crsr: str, nav: Navigation) -> str:
             nonlocal query_part
             all_walks = []
```

### Comparing `resotocore-3.5.1/resotocore/db/arangodb_extensions.py` & `resotocore-3.5.2/resotocore/db/arangodb_extensions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/db/arangodb_functions.py` & `resotocore-3.5.2/resotocore/db/arangodb_functions.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/db/async_arangodb.py` & `resotocore-3.5.2/resotocore/db/async_arangodb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/db/configdb.py` & `resotocore-3.5.2/resotocore/db/configdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/db/db_access.py` & `resotocore-3.5.2/resotocore/db/db_access.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/db/deferred_edge_db.py` & `resotocore-3.5.2/resotocore/db/deferred_edge_db.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/db/entitydb.py` & `resotocore-3.5.2/resotocore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/db/graphdb.py` & `resotocore-3.5.2/resotocore/db/graphdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/db/model.py` & `resotocore-3.5.2/resotocore/db/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/db/packagedb.py` & `resotocore-3.5.2/resotocore/db/packagedb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/db/runningtaskdb.py` & `resotocore-3.5.2/resotocore/db/runningtaskdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/db/system_data_db.py` & `resotocore-3.5.2/resotocore/db/system_data_db.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/dependencies.py` & `resotocore-3.5.2/resotocore/dependencies.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/error.py` & `resotocore-3.5.2/resotocore/error.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/graph_manager/graph_manager.py` & `resotocore-3.5.2/resotocore/graph_manager/graph_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from typing import List, Optional, AsyncIterator, cast, Tuple
 from asyncio import Lock
 
 import logging
 
 from resotocore.db.db_access import DbAccess
 from resotocore.db.graphdb import EventGraphDB
-from resotocore.util import utc_str, UTC_Date_Format_short
+from resotocore.util import utc_str, UTC_Date_Format_short, utc
 from resotocore.ids import GraphName, TaskDescriptorId
 from resotocore.web.service import Service
 from resotocore.util import check_graph_name, Periodic
 from resotocore.types import Json
 from resotocore.model.model import Kind
 from resotocore.model.typed_model import from_js, to_js_str
 from resotocore.model.graph_access import EdgeTypes
@@ -111,14 +111,32 @@
         if self.snapshot_cleanup_worker:
             await self.snapshot_cleanup_worker.stop()
             self.snapshot_cleanup_worker = None
 
     async def list(self, pattern: Optional[str]) -> List[GraphName]:
         return [key for key in await self.db_access.list_graphs() if pattern is None or re.match(pattern, key)]
 
+    async def snapshot_at(self, *, time: datetime, graph_name: GraphName) -> Optional[GraphName]:
+        regex = rf"snapshot-{graph_name}-.*-(.+)"
+        graphs = await self.list(regex)
+        graphs_with_time = []
+        for graph in graphs:
+            match = re.match(regex, graph)
+            if match:
+                graphs_with_time.append((parse(match.group(1)), graph))
+
+        graphs_with_time.sort(reverse=True, key=lambda x: x[0])
+        # take the first graph that is older than the given time
+        for graph_time, graph in graphs_with_time:
+            if graph_time <= time:
+                return graph
+
+        # nothing found
+        return None
+
     async def copy(
         self, source: GraphName, destination: GraphName, replace_existing: bool, validate_name: bool = True
     ) -> GraphName:
         if not self.lock:
             raise RuntimeError("GraphManager has not been started")
 
         async with self.lock:
@@ -149,16 +167,22 @@
         destination_model_db = await self.db_access.get_graph_model_db(destination)
 
         model_kinds = [kind async for kind in source_model_db.all()]
         await destination_model_db.update_many(model_kinds)
 
         return destination
 
-    async def snapshot(self, source: GraphName, label: str) -> GraphName:
-        time = utc_str(date_format=UTC_Date_Format_short)
+    async def snapshot(self, source: GraphName, label: str, timestamp: Optional[datetime] = None) -> GraphName:
+        if not timestamp:
+            timestamp = utc()
+
+        if source.startswith("snapshot-"):
+            raise ValueError("Can not snapshot a snapshot")
+
+        time = utc_str(timestamp, date_format=UTC_Date_Format_short)
         check_graph_name(label)
         snapshot_name = GraphName(f"snapshot-{source}-{label}-{time}")
         return await self.copy(source, snapshot_name, replace_existing=False, validate_name=False)
 
     async def delete(self, graph_name: GraphName) -> None:
         await self.db_access.delete_graph(graph_name)
         await self.db_access.delete_graph_model(graph_name)
```

### Comparing `resotocore-3.5.1/resotocore/infra_apps/local_runtime.py` & `resotocore-3.5.2/resotocore/infra_apps/local_runtime.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/infra_apps/manifest.py` & `resotocore-3.5.2/resotocore/infra_apps/manifest.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/infra_apps/package_manager.py` & `resotocore-3.5.2/resotocore/infra_apps/package_manager.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from resotocore.db.packagedb import PackageEntityDb, InfraAppPackage
 from resotocore.config import ConfigHandler
 from resotocore.config import ConfigEntity
 from resotocore.ids import InfraAppName, ConfigId
 from resotocore.model.model import Kind, ComplexKind
 from resotocore.types import Json
 from resotocore.model.typed_model import from_js
-from resotocore.cli.model import AliasTemplate
+from resotocore.cli.model import InfraAppAlias, InfraAppAliasParameter
 from logging import getLogger
 from resotocore.web.service import Service
 
 logger = getLogger(__name__)
 
 
 def config_id(name: InfraAppName) -> ConfigId:
@@ -63,15 +63,15 @@
 
 
 class PackageManager(Service):
     def __init__(
         self,
         entity_db: PackageEntityDb,
         config_handler: ConfigHandler,
-        add_command_alias: Callable[[AliasTemplate], None],
+        add_command_alias: Callable[[InfraAppAlias], None],
         remove_command_alias: Callable[[str], None],
         repos_cache_directory: Path = Path.home() / ".cache" / "resoto-infra-apps",
     ) -> None:
         """
         Package manager for infra apps.
 
         Args:
@@ -91,25 +91,33 @@
 
     async def start(self) -> None:
         self.update_lock = asyncio.Lock()
         self.repos_cache_directory.mkdir(parents=True, exist_ok=True)
 
         # set up custom commands
         manifests = [await self.get_manifest(name) async for name in self.list()]
-        self._setup_custom_commands([m for m in manifests if m is not None])
+        self._setup_command_aliases([m for m in manifests if m is not None])
 
-    def _setup_custom_commands(self, manifests: List[AppManifest]) -> None:
+    def _setup_command_aliases(self, manifests: List[AppManifest]) -> None:
         for manifest in manifests:
-            alias_template = AliasTemplate(
+
+            def to_param(arg: Tuple[str, Json]) -> InfraAppAliasParameter:
+                name, arg_schema = arg
+                return InfraAppAliasParameter(
+                    name=name,
+                    help=arg_schema.get("help", ""),
+                    default=arg_schema.get("default", None),
+                )
+
+            parameters = [to_param(arg) for arg in (manifest.args_schema or {}).items()]
+            alias_template = InfraAppAlias(
                 name=manifest.name,
-                info=manifest.description,
-                template=f"apps run {manifest.name}" + r" {{args}}",
-                description=manifest.readme,
-                allowed_in_source_position=True,
-                infra_app_parameters=manifest.args_schema,
+                description=manifest.description,
+                readme=manifest.readme,
+                parameters=parameters,
             )
             self.add_command_alias(alias_template)
 
     async def stop(self) -> None:
         if self.cleanup_task:
             self.cleanup_task.cancel()
             await self.cleanup_task
@@ -259,15 +267,15 @@
         config_entity = ConfigEntity(conf_id, manifest.default_config or {}, None)
         try:
             if await self.config_handler.get_config(conf_id) is None:
                 await self.config_handler.put_config(config_entity, validate=manifest.config_schema is not None)
             stored = await self.entity_db.update(InfraAppPackage(manifest, url))
 
             # add the custom command alias
-            self._setup_custom_commands([manifest])
+            self._setup_command_aliases([manifest])
 
             return stored.manifest
         except Exception as e:
             logger.error(f"Failed to install {manifest.name} from {url}", exc_info=e)
             return ManifestInstallFailed(manifest.name, str(e))
 
     async def _fetch_manifest(self, app_name: InfraAppName, url: str) -> Union[Failure, AppManifest]:
```

### Comparing `resotocore-3.5.1/resotocore/infra_apps/runtime.py` & `resotocore-3.5.2/resotocore/infra_apps/runtime.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/api/contents/all.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.03125%*

 * *Differences: {"'additionalProperties'": 'False',*

 * * "'description'": "'Inspector settings.'",*

 * * "'jupyter.lab.menus'": "OrderedDict([('main', [OrderedDict([('id', 'jp-mainmenu-help'), ('items', "*

 * *                        "[OrderedDict([('type', 'separator'), ('rank', 0.1)]), "*

 * *                        "OrderedDict([('command', 'inspector:open'), ('rank', 0.1)]), "*

 * *                        "OrderedDict([('type', 'separator'), ('rank', 0.1)])])])])])",*

 * * "'jupyter.lab.shortcuts'": "[OrderedDict([('command', 'inspector:open'), (' […]*

```diff
@@ -1,25 +1,37 @@
 {
-    "content": [
+    "additionalProperties": false,
+    "description": "Inspector settings.",
+    "jupyter.lab.menus": {
+        "main": [
+            {
+                "id": "jp-mainmenu-help",
+                "items": [
+                    {
+                        "rank": 0.1,
+                        "type": "separator"
+                    },
+                    {
+                        "command": "inspector:open",
+                        "rank": 0.1
+                    },
+                    {
+                        "rank": 0.1,
+                        "type": "separator"
+                    }
+                ]
+            }
+        ]
+    },
+    "jupyter.lab.shortcuts": [
         {
-            "content": null,
-            "created": "2023-06-02T14:51:36.280535Z",
-            "format": null,
-            "last_modified": "2023-06-02T14:47:48.361319Z",
-            "mimetype": null,
-            "name": "example.ipynb",
-            "path": "example.ipynb",
-            "size": 7611,
-            "type": "notebook",
-            "writable": true
+            "command": "inspector:open",
+            "keys": [
+                "Accel I"
+            ],
+            "selector": "body"
         }
     ],
-    "created": "2023-06-02T14:51:36.280535Z",
-    "format": "json",
-    "last_modified": "2023-06-02T14:51:36.280535Z",
-    "mimetype": null,
-    "name": "",
-    "path": "",
-    "size": null,
-    "type": "directory",
-    "writable": true
+    "properties": {},
+    "title": "Inspector",
+    "type": "object"
 }
```

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/bootstrap.js` & `resotocore-3.5.2/resotocore/jupyterlite/bootstrap.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1037.51967a2.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1037.51967a2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1079.cdbaf67.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1079.cdbaf67.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1084.4cd1c89.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1084.4cd1c89.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1113.23c9417.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1113.23c9417.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1125.129d070.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1125.129d070.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1163.ac28297.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1163.ac28297.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1221.c51249a.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1221.c51249a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1245.be46619.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1245.be46619.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1261.199fc1d.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1261.199fc1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1272.f334098.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1272.f334098.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1278.0524a4a.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1278.0524a4a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt` & `resotocore-3.5.2/resotocore/jupyterlite/build/1278.0524a4a.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1290.3981211.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1290.3981211.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1295.46e72b8.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1295.46e72b8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1310.23bbe67.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1310.23bbe67.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1320.21effe3.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1320.21effe3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1325.f76267c.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1325.f76267c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1408.7461890.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1408.7461890.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1440.a9e7ea1.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1440.a9e7ea1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1483.616d9ab.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1483.616d9ab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1489.e50b6d4.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1489.e50b6d4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1507.5705605.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1507.5705605.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/152.525d460.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/152.525d460.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1520.4e2eb21.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1520.4e2eb21.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1555.e188f3f.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1555.e188f3f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1559.7c89925.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1559.7c89925.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/160.5f28731.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/160.5f28731.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1603.370a2a6.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1603.370a2a6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1644.0e49167.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1644.0e49167.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1667.f0afb2b.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1667.f0afb2b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1687.27f1ad6.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1687.27f1ad6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1725.f151c33.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1725.f151c33.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1767.c8c2f26.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1767.c8c2f26.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1806.1aaf66b.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1806.1aaf66b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1838.1202b16.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1838.1202b16.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1909.28a2def.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1909.28a2def.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/1989.88d258f.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/1989.88d258f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2030.1562cc6.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2030.1562cc6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2047.baed97b.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2047.baed97b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2099.f4b6fcd.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2099.f4b6fcd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2118.5b65f70.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2118.5b65f70.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/213.5769e57.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/213.5769e57.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2161.dcb27b8.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2161.dcb27b8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2169.635c88e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2169.635c88e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/217.90d10e2.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/217.90d10e2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2212.72be094.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2212.72be094.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2287.997c38e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2287.997c38e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt` & `resotocore-3.5.2/resotocore/jupyterlite/build/2287.997c38e.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2303.9ff8710.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2303.9ff8710.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2319.6b4cbb7.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2319.6b4cbb7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2329.4c5ca6d.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2329.4c5ca6d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2351.fbd96d8.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2351.fbd96d8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2358.d5cf7c8.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2358.d5cf7c8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2359.6451c3e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2359.6451c3e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/237.f765e77.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/237.f765e77.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2384.71782be.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2384.71782be.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/240.cddc46b.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/240.cddc46b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2431.648d237.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2431.648d237.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2546.1f48267.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2546.1f48267.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2557.75e9da2.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2557.75e9da2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/261.5f53c0e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/261.5f53c0e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2629.c0e1cd6.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2629.c0e1cd6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2788.46acc8a.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2788.46acc8a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2834.942acc6.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2834.942acc6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2887.47ba752.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2887.47ba752.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2956.8880209.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2956.8880209.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/2973.2a51dc4.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/2973.2a51dc4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3004.255e79c.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3004.255e79c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/302.8bcc38f.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/302.8bcc38f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3037.70ee38d.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3037.70ee38d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3042.7cfad84.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3042.7cfad84.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3051.34fac68.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3051.34fac68.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3122.2289fca.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3122.2289fca.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3151.10ef4de.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3151.10ef4de.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/316.c850a76.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/316.c850a76.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3196.4e35a17.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3196.4e35a17.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3265.a80440a.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3265.a80440a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3277.9c04e75.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3277.9c04e75.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/330.126fa98.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/330.126fa98.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3392.29fe6b9.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3392.29fe6b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3413.480a49d.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3413.480a49d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3444.47d5ea1.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3444.47d5ea1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3469.7d14d0b.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3469.7d14d0b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3546.fee1bd7.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3546.fee1bd7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/362.6716970.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/362.6716970.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3708.410d087.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3708.410d087.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3850.903abc2.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3850.903abc2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt` & `resotocore-3.5.2/resotocore/jupyterlite/build/3850.903abc2.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3880.bd39dce.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3880.bd39dce.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3970.236586f.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3970.236586f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3976.58893b9.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3976.58893b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt` & `resotocore-3.5.2/resotocore/jupyterlite/build/3976.58893b9.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/3979.385527e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/3979.385527e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/400.d72234b.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/400.d72234b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4018.1a35967.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4018.1a35967.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/406.9b7af92.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/406.9b7af92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4117.a8107fd.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4117.a8107fd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4182.e2430f9.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4182.e2430f9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4191.02bbea8.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4191.02bbea8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4197.53ab10b.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4197.53ab10b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4206.a5f8bb0.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4206.a5f8bb0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4207.0d0580b.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4207.0d0580b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4262.bb73457.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4262.bb73457.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4298.5ee510c.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4298.5ee510c.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/44.0cfa785.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/44.0cfa785.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt` & `resotocore-3.5.2/resotocore/jupyterlite/build/44.0cfa785.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4410.e4a25d3.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4410.e4a25d3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4466.64d23d1.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4466.64d23d1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/451.d9683ad.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/451.d9683ad.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4535.34b060a.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4535.34b060a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4565.43bdb91.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4565.43bdb91.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4569.f374f9d.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4569.f374f9d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4615.eb5d40a.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4615.eb5d40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4658.090d4a9.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4658.090d4a9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4690.3dd4096.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4690.3dd4096.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4715.e7690b9.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4715.e7690b9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4749.46ebbb2.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4749.46ebbb2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4750.56c06ab.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4750.56c06ab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4856.2d7415f.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4856.2d7415f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4875.375150e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4875.375150e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/489.b981dea.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/489.b981dea.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/490.c2624d4.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/490.c2624d4.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4905.667bf33.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4905.667bf33.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4931.430433b.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4931.430433b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/4942.b96c164.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/4942.b96c164.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5016.dd2fe83.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5016.dd2fe83.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5072.733a1b5.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5072.733a1b5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/509.6448878.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/509.6448878.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5096.8ed0d8e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5096.8ed0d8e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5126.eecad7a.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5126.eecad7a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5129.1ba4763.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5129.1ba4763.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5153.763d8fa.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5153.763d8fa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5155.06b4ea9.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5155.06b4ea9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5193.e9f6866.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5193.e9f6866.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5213.3e1a360.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5213.3e1a360.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5227.8c8acd8.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5227.8c8acd8.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5238.1751cc3.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5238.1751cc3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/528.2262cb0.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/528.2262cb0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5292.79d4aba.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5292.79d4aba.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5437.31236f7.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5437.31236f7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5489.848a8cf.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5489.848a8cf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5508.317fca3.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5508.317fca3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/554.ac98303.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/554.ac98303.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/555.2cd31dd.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/555.2cd31dd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5573.ebcdb93.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5573.ebcdb93.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5666.c5e5324.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5666.c5e5324.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5710.70d0b1d.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5710.70d0b1d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5747.94ad626.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5747.94ad626.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/582.21b8e7d.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/582.21b8e7d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5823.5045bdb.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5823.5045bdb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5851.30b7b2a.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5851.30b7b2a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5878.32d92fa.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5878.32d92fa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5880.68f975b.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5880.68f975b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5955.88508f7.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5955.88508f7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/5971.88c5642.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/5971.88c5642.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6080.aa0ff24.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6080.aa0ff24.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/61.2808a0d.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/61.2808a0d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6136.b8ba2b2.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6136.b8ba2b2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6141.9831d58.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6141.9831d58.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6475.6037fbb.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6475.6037fbb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6493.d796aa5.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6493.d796aa5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6556.b3d9293.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6556.b3d9293.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6571.2c8884e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6571.2c8884e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6576.3ea568e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6576.3ea568e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6591.94ed352.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6591.94ed352.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6612.1632879.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6612.1632879.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6623.ae3b3cc.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6623.ae3b3cc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6664.2160109.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6664.2160109.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6747.47be7f5.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6747.47be7f5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6748.be68f5f.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6748.be68f5f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6870.7940288.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6870.7940288.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6879.c8367a5.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6879.c8367a5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6898.9bbc12a.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6898.9bbc12a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6952.f68b818.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6952.f68b818.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6985.321ad92.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6985.321ad92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6993.32cf9a6.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6993.32cf9a6.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/6997.b06fe71.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/6997.b06fe71.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7041.d4f561e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7041.d4f561e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7058.805c88e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7058.805c88e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7174.6c45206.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7174.6c45206.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7334.8859b1b.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7334.8859b1b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7359.6ee65ec.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7359.6ee65ec.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7364.195178b.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7364.195178b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7380.58a4413.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7380.58a4413.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7427.f9c2017.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7427.f9c2017.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7463.18fd278.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7463.18fd278.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7509.1e0189e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7509.1e0189e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7526.1a303e5.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7526.1a303e5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7537.1323a15.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7537.1323a15.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7692.33d5169.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7692.33d5169.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7746.5908d29.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7746.5908d29.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7808.1d582a2.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7808.1d582a2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/783.c156751.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/783.c156751.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7858.2386e4d.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7858.2386e4d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/7941.01ea680.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/7941.01ea680.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8005.c5ad7b2.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8005.c5ad7b2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8028.39e2fa1.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8028.39e2fa1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8061.cc62561.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8061.cc62561.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8101.cf46d02.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8101.cf46d02.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/812.9b0e86e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/812.9b0e86e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/816.c8050f2.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/816.c8050f2.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8165.b2c3285.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8165.b2c3285.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8232.a578bf9.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8232.a578bf9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/824.8678196.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/824.8678196.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8270.89fe7e1.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8270.89fe7e1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/833.9cc6653.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/833.9cc6653.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8370.8f855e5.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8370.8f855e5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8373.96b0b3a.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8373.96b0b3a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8389.ffe031f.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8389.ffe031f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8412.1528057.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8412.1528057.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8427.4923f43.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8427.4923f43.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8542.027afdc.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8542.027afdc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8594.0112f03.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8594.0112f03.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8656.d5b8e92.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8656.d5b8e92.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8685.d78bdab.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8685.d78bdab.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8698.9817d75.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8698.9817d75.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8732.9320f73.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8732.9320f73.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8785.cf4fe95.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8785.cf4fe95.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8828.77c71d0.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8828.77c71d0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8883.80c7b63.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8883.80c7b63.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8976.3816942.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8976.3816942.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/8990.2a453cf.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/8990.2a453cf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9035.1e45c1b.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9035.1e45c1b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9053.45b77fc.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9053.45b77fc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9077.fefb6ca.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9077.fefb6ca.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9128.b8fa6f0.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9128.b8fa6f0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9156.0cefbd3.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9156.0cefbd3.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9170.0023587.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9170.0023587.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9196.315f9f9.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9196.315f9f9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9198.9971d70.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9198.9971d70.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/920.d15c177.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/920.d15c177.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9253.0b31caa.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9253.0b31caa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9266.bacd0dd.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9266.bacd0dd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9307.c3a00ed.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9307.c3a00ed.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9321.869e413.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9321.869e413.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9344.ba0abcf.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9344.ba0abcf.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9382.9014799.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9382.9014799.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9440.1b10b8f.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9440.1b10b8f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9464.79e6ac5.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9464.79e6ac5.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9502.9a24831.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9502.9a24831.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9507.1e6cc5d.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9507.1e6cc5d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9602.62bf0f1.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9602.62bf0f1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9621.e2e8b5d.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9621.e2e8b5d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9622.ccab065.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9622.ccab065.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9626.a178bd0.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9626.a178bd0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9647.ed91993.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9647.ed91993.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9657.bc5c60e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9657.bc5c60e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/97.ad126b0.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/97.ad126b0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9712.796a0a1.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9712.796a0a1.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9737.7dc8f98.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9737.7dc8f98.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9777.0b8a504.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9777.0b8a504.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9793.6d63a85.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9793.6d63a85.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9806.652c162.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9806.652c162.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9865.2e3db6f.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9865.2e3db6f.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/989.bcca86a.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/989.bcca86a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9943.f3f35c7.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9943.f3f35c7.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9958.25c8c06.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9958.25c8c06.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/9960.64cd61e.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/9960.64cd61e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/add-above.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/add-above.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/add-below.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/add-below.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/bug-dot.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/bug-dot.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/bug.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/bug.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/build.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/build.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/case-sensitive.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/case-sensitive.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/close.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/close.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/copyright.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/copyright.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/cut.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/cut.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/duplicate.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/duplicate.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/fa-brands-400.woff2` & `resotocore-3.5.2/resotocore/jupyterlite/build/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/fa-regular-400.woff2` & `resotocore-3.5.2/resotocore/jupyterlite/build/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/fa-solid-900.woff2` & `resotocore-3.5.2/resotocore/jupyterlite/build/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/html5.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/html5.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/json.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/json.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/julia.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/julia.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/jupyter-favicon.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/jupyter-favicon.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/jupyter.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/jupyter.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/jupyterlab-wordmark.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/jupyterlab-wordmark.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/lab/bundle.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/lab/bundle.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/listings-info.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/listings-info.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/move-down.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/move-down.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/move-up.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/move-up.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/not-trusted.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/not-trusted.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/palette.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/palette.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/pdf.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/pdf.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/python.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/python.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/react.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/react.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/regex.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/regex.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/application-extension/sidebar.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/commands.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/toc-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/schemas/all.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/schemas/all.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/service-worker-b2fb40a.js` & `resotocore-3.5.2/resotocore/jupyterlite/build/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/settings.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/settings.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/tag.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/tag.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/terminal.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/terminal.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css` & `resotocore-3.5.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css` & `resotocore-3.5.2/resotocore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/third-party-licenses.json` & `resotocore-3.5.2/resotocore/jupyterlite/build/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/toc.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/toc.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/build/trusted.svg` & `resotocore-3.5.2/resotocore/jupyterlite/build/trusted.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/config-utils.js` & `resotocore-3.5.2/resotocore/jupyterlite/config-utils.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/102.c877ef340ee478be48c0.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/290.85fbfc269929f73a8f25.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/322.47953449e4616f51d135.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/441.4368412449ba90ea9225.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/568.34b49b2d3ba8db46b0cc.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/866.1ce3c77b50c9eb671961.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.7e46d8af7cfb9637087e.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/518.a3c6a3ae7ee95e5158aa.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/568.371c75f0cd43fa31532d.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/652.07cda501733578161e13.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/951.b9fa6250974e699a3731.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/all.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/ipykernel-6.9.2-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/piplite-0.0.8-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/pyodide_kernel-0.0.8-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-3.6.4-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/pypi/widgetsnbextension-4.0.7-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/remoteEntry.b340cae4b3c1bda6a7fd.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/kernel.v0.schema.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/schema/piplite.v0.schema.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/@jupyterlite/pyodide-kernel-extension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/133.f3efd6f2704522ff3b63.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/423.a173fe7fc002e2014c2a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/478.f7319c49bce7c550ff08.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/657.b28ffbba9c00cc1d1f86.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/855.3df3272be51618b38ffb.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.d87fbfbef62a029ce69b.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/747.8eb3ddccc7ec4987bff9.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.aa1060b2d1221f8e5688.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json` & `resotocore-3.5.2/resotocore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/files/example.ipynb` & `resotocore-3.5.2/resotocore/jupyterlite/files/example.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/icon-120x120.png` & `resotocore-3.5.2/resotocore/jupyterlite/icon-120x120.png`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/icon-512x512.png` & `resotocore-3.5.2/resotocore/jupyterlite/icon-512x512.png`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/index.html` & `resotocore-3.5.2/resotocore/jupyterlite/index.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/jupyter-lite.ipynb` & `resotocore-3.5.2/resotocore/jupyterlite/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/jupyter-lite.json` & `resotocore-3.5.2/resotocore/jupyterlite/jupyter-lite.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/jupyterlite.schema.v0.json` & `resotocore-3.5.2/resotocore/jupyterlite/jupyterlite.schema.v0.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/kernelspecs/javascript.svg` & `resotocore-3.5.2/resotocore/jupyterlite/kernelspecs/javascript.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/lab/favicon.ico` & `resotocore-3.5.2/resotocore/jupyterlite/lab/favicon.ico`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/lab/index.html` & `resotocore-3.5.2/resotocore/jupyterlite/lab/index.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/lab/jupyter-lite.ipynb` & `resotocore-3.5.2/resotocore/jupyterlite/lab/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/lab/package.json` & `resotocore-3.5.2/resotocore/jupyterlite/lab/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/manifest.webmanifest` & `resotocore-3.5.2/resotocore/jupyterlite/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/package.json` & `resotocore-3.5.2/resotocore/jupyterlite/package.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/jupyterlite/service-worker-b2fb40a.js` & `resotocore-3.5.2/resotocore/jupyterlite/service-worker-b2fb40a.js`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/message_bus.py` & `resotocore-3.5.2/resotocore/message_bus.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/metrics.py` & `resotocore-3.5.2/resotocore/metrics.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/model/adjust_node.py` & `resotocore-3.5.2/resotocore/model/adjust_node.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/model/db_updater.py` & `resotocore-3.5.2/resotocore/model/db_updater.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/model/graph_access.py` & `resotocore-3.5.2/resotocore/model/graph_access.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/model/json_schema.py` & `resotocore-3.5.2/resotocore/model/json_schema.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/model/model.py` & `resotocore-3.5.2/resotocore/model/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from __future__ import annotations
 
 import json
 import re
 import sys
+import textwrap
 from abc import ABC, abstractmethod
 from functools import lru_cache
 
 from attrs import define
 from datetime import datetime, timezone, date
 from json import JSONDecodeError
 from typing import Union, Any, Optional, Callable, Type, Sequence, Dict, List, Set, cast, Tuple, Iterable
@@ -959,19 +960,22 @@
                     result[n] = v
             return result if has_coerced else None
         else:
             return None
 
     def create_yaml(self, elem: JsonElement, initial_level: int = 0, overrides: Optional[Json] = None) -> str:
         def safe_string(s: str, indent: int, default_style: Optional[str] = None) -> str:
-            return remove_suffix(
-                # 2 spaces per indent
-                yaml.dump(s, indent=indent * 2, allow_unicode=True, width=sys.maxsize, default_style=default_style),
-                "\n...\n",
-            ).strip()
+            # 2 spaces per indent
+            yml = yaml.dump(s, indent=0, allow_unicode=True, width=sys.maxsize, default_style=default_style)
+            yml = remove_suffix(yml, "\n...\n")
+            if default_style == "|":
+                yml = textwrap.indent(yml, " " * (max(0, indent - 1) * 2)).lstrip()
+            else:
+                yml = yml.strip()
+            return yml
 
         def override_note(overrides: Optional[Json], prop_name: str) -> Optional[str]:
             if overrides:
                 override = overrides.get(prop_name)
                 # leaf node of the override tree
                 if isinstance(override, (str, list, int, float, bool)):
                     note = (
@@ -1016,23 +1020,23 @@
                     str_value = walk_element(value, sub, indent + 1, overrides=override_child)
                     if description:
                         for line in description.splitlines():
                             result += f"{prepend}# {line}\n"
                     maybe_space = "" if str_value.startswith("\n") else " "
                     safe_prop = safe_string(prop, indent)
                     result += f"{prepend}{safe_prop}:{maybe_space}{str_value}\n"
-                return result.rstrip()
+                return remove_suffix(result, "\n")
             elif isinstance(e, list) and e:
                 prepend = "  " * indent + "-"
                 sub = kind.inner if isinstance(kind, ArrayKind) else kind
                 result = "\n"
                 for item in e:
                     item_str = walk_element(item, sub, indent + 1, False).lstrip()
                     result += f"{prepend} {item_str}\n"
-                return result.rstrip()
+                return remove_suffix(result, "\n")
             elif isinstance(e, list):
                 return "[]"
             elif is_env_var_string(e):
                 return str(e)
             elif isinstance(e, str):
                 # if the string contains a newline, try a literal block, else a quoted string
                 return safe_string(e, indent, "|" if "\n" in e else "'")
```

### Comparing `resotocore-3.5.1/resotocore/model/model_handler.py` & `resotocore-3.5.2/resotocore/model/model_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/model/resolve_in_graph.py` & `resotocore-3.5.2/resotocore/model/resolve_in_graph.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/model/transform_kind_convert.py` & `resotocore-3.5.2/resotocore/model/transform_kind_convert.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/model/typed_model.py` & `resotocore-3.5.2/resotocore/model/typed_model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/query/__init__.py` & `resotocore-3.5.2/resotocore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/query/model.py` & `resotocore-3.5.2/resotocore/query/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/query/query_parser.py` & `resotocore-3.5.2/resotocore/query/query_parser.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/query/template_expander.py` & `resotocore-3.5.2/resotocore/query/template_expander.py`

 * *Files 1% similar despite different names*

```diff
@@ -172,24 +172,34 @@
     def from_now(result: str) -> str:
         return utc_str(utc() + duration(result))
 
     @staticmethod
     def ago(result: str) -> str:
         return utc_str(utc() - duration(result))
 
+    @staticmethod
+    def as_list(result: Any) -> List[Any]:
+        if isinstance(result, list):
+            return result
+        elif isinstance(result, dict):
+            return [{"key": k, "value": v} for k, v in result.items()]
+        else:
+            return [result]
+
 
 # noinspection PyTypeChecker
 getter: PropertyGetter = functools.partial(
     default_getter,
     virtuals={
         **default_virtuals,
         "with_index": VirtualFunctions.with_index,
         "parens": VirtualFunctions.parens,
         "from_now": VirtualFunctions.from_now,
         "ago": VirtualFunctions.ago,
+        "as_list": VirtualFunctions.as_list,
     },
 )
 
 
 def render_template(template: str, props: Json, more_props: Iterable[Json] = (), tags: TagsTuple = default_tags) -> str:
     """
     Render given provided template with given property values.
```

### Comparing `resotocore-3.5.1/resotocore/query/template_expander_service.py` & `resotocore-3.5.2/resotocore/query/template_expander_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/report/__init__.py` & `resotocore-3.5.2/resotocore/report/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,25 +280,32 @@
             description=reported["description"],
             documentation=reported.get("documentation"),
             accounts=reported["accounts"],
             only_failed=reported["only_failed"],
             severity=if_set(reported.get("severity"), ReportSeverity),
         )
 
-    def to_graph(self) -> List[Json]:
+    def to_graph(self, only_checks: bool = False) -> List[Json]:
         result = []
 
         def visit_check_collection(collection: CheckCollectionResult) -> None:
-            result.append(collection.to_node())
+            if not only_checks:
+                result.append(collection.to_node())
             for check in collection.checks:
                 result.append(check.to_node())
-                result.append({"from": collection.node_id, "to": check.node_id, "type": "edge", "edge_type": "default"})
+                if not only_checks:
+                    result.append(
+                        {"from": collection.node_id, "to": check.node_id, "type": "edge", "edge_type": "default"}
+                    )
             for child in collection.children:
                 visit_check_collection(child)
-                result.append({"from": collection.node_id, "to": child.node_id, "type": "edge", "edge_type": "default"})
+                if not only_checks:
+                    result.append(
+                        {"from": collection.node_id, "to": child.node_id, "type": "edge", "edge_type": "default"}
+                    )
 
         visit_check_collection(self)
         return result
 
 
 class Inspector(ABC):
     """
```

### Comparing `resotocore-3.5.1/resotocore/report/benchmark_renderer.py` & `resotocore-3.5.2/resotocore/report/benchmark_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/report/inspector_service.py` & `resotocore-3.5.2/resotocore/report/inspector_service.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/report/report_config.py` & `resotocore-3.5.2/resotocore/report/report_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -149,8 +149,8 @@
         # Benchmark and BenchmarkConfig are structurally identical.
         # If Benchmark needs to change, the config is here to have a migration path.
         return from_js(cfg.config[BenchmarkConfigRoot], Benchmark)
 
 
 def config_model() -> List[Json]:
     config_classes = {ReportCheckCollectionConfig, BenchmarkConfig}
-    return dataclasses_to_resotocore_model(config_classes, allow_unknown_props=False)
+    return dataclasses_to_resotocore_model(config_classes, use_optional_as_required=True)
```

### Comparing `resotocore-3.5.1/resotocore/static/api-doc.yaml` & `resotocore-3.5.2/resotocore/static/api-doc.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -876,14 +876,21 @@
           required: false
           schema:
             type: string
             enum:
               - reported
               - desired
               - metadata
+        - name: at
+          in: query
+          description: "The timestamp to use for the search. If not defined the latest version of the graph is used."
+          required: false
+          schema:
+            type: string
+            format: date-time
       requestBody:
         description: "The search to perform"
         content:
           text/plain:
             schema:
               type: string
               example: is(graph_root) and reported.name=="root" -->
@@ -924,14 +931,21 @@
         - name: count
           in: query
           description: "Optional parameter to get a Ck-Element-Count header which returns the number of returned json elements"
           required: false
           schema:
             type: boolean
             default: true
+        - name: at
+          in: query
+          description: "The timestamp to use for the search. If not defined the latest version of the graph is used."
+          required: false
+          schema:
+            type: string
+            format: date-time
       requestBody:
         description: "The search to perform"
         content:
           text/plain:
             schema:
               type: string
               example: is(graph_root) and reported.name=="root" -->
@@ -1134,14 +1148,21 @@
         - name: search_timeout
           in: query
           description: "Optional duration the search is allowed to run."
           required: false
           schema:
             type: string
             example: "30s"
+        - name: at
+          in: query
+          description: "The timestamp to use for the search. If not defined the latest version of the graph is used."
+          required: false
+          schema:
+            type: string
+            format: date-time
       requestBody:
         description: "The search to perform"
         content:
           text/plain:
             schema:
               type: string
               example: is(graph_root) and reported.name=="root" -->
@@ -1329,14 +1350,21 @@
           required: false
           schema:
             type: string
             enum:
               - reported
               - desired
               - metadata
+        - name: at
+          in: query
+          description: "The timestamp to use for the search. If not defined the latest version of the graph is used."
+          required: false
+          schema:
+            type: string
+            format: date-time
       requestBody:
         description: "The aggregation search to perform"
         content:
           text/plain:
             schema:
               type: string
               example: |
@@ -1372,14 +1400,21 @@
           required: false
           schema:
             type: string
             enum:
               - reported
               - desired
               - metadata
+        - name: at
+          in: query
+          description: "The timestamp to use for the search. If not defined the latest version of the graph is used."
+          required: false
+          schema:
+            type: string
+            format: date-time
       requestBody:
         description: "The search to perform"
         content:
           text/plain:
             schema:
               type: string
               example: |
@@ -1502,14 +1537,21 @@
           required: false
           schema:
             type: string
             enum:
               - reported
               - desired
               - metadata
+        - name: at
+          in: query
+          description: "The timestamp to use for the search. If not defined the latest version of the graph is used."
+          required: false
+          schema:
+            type: string
+            format: date-time
       requestBody:
         description: "The search to perform"
         content:
           text/plain:
             schema:
               type: string
               example: is(graph_root) and reported.name=="root" -->
@@ -1574,14 +1616,21 @@
           required: false
           schema:
             type: string
             enum:
               - node_created
               - node_updated
               - node_deleted
+        - name: at
+          in: query
+          description: "The timestamp to use for the search. If not defined the latest version of the graph is used."
+          required: false
+          schema:
+            type: string
+            format: date-time
       requestBody:
         description: "The search to perform"
         content:
           text/plain:
             schema:
               type: string
               example: is(volume) and reported.volume_size>100
@@ -1712,14 +1761,21 @@
           required: false
           schema:
             type: string
             enum:
               - node_created
               - node_updated
               - node_deleted
+        - name: at
+          in: query
+          description: "The timestamp to use for the search. If not defined the latest version of the graph is used."
+          required: false
+          schema:
+            type: string
+            format: date-time
       requestBody:
         description: "The aggregation search to perform"
         content:
           text/plain:
             schema:
               type: string
               example: |
```

### Comparing `resotocore-3.5.1/resotocore/static/ck-unicode-truecolor.ans` & `resotocore-3.5.2/resotocore/static/ck-unicode-truecolor.ans`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/static/report/benchmark/aws/aws_cis_1_5.json` & `resotocore-3.5.2/resotocore/static/report/benchmark/aws/aws_cis_1_5.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/static/report/check_template.json` & `resotocore-3.5.2/resotocore/static/report/check_template.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/static/report/checks/aws/aws_apigateway.json` & `resotocore-3.5.2/resotocore/static/report/checks/aws/aws_apigateway.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/static/report/checks/aws/aws_cloudtrail.json` & `resotocore-3.5.2/resotocore/static/report/checks/aws/aws_cloudtrail.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/static/report/checks/aws/aws_config.json` & `resotocore-3.5.2/resotocore/static/report/checks/aws/aws_config.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/static/report/checks/aws/aws_ec2.json` & `resotocore-3.5.2/resotocore/static/report/checks/aws/aws_ec2.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/static/report/checks/aws/aws_efs.json` & `resotocore-3.5.2/resotocore/static/report/checks/aws/aws_efs.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/static/report/checks/aws/aws_iam.json` & `resotocore-3.5.2/resotocore/static/report/checks/aws/aws_iam.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/static/report/checks/aws/aws_kms.json` & `resotocore-3.5.2/resotocore/static/report/checks/aws/aws_kms.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/static/report/checks/aws/aws_lambda.json` & `resotocore-3.5.2/resotocore/static/report/checks/aws/aws_lambda.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/static/report/checks/aws/aws_rds.json` & `resotocore-3.5.2/resotocore/static/report/checks/aws/aws_rds.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/static/report/checks/aws/aws_s3.json` & `resotocore-3.5.2/resotocore/static/report/checks/aws/aws_s3.json`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/static/resoto_logo_and_text.svg` & `resotocore-3.5.2/resotocore/static/resoto_logo_and_text.svg`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/task/__init__.py` & `resotocore-3.5.2/resotocore/task/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/task/model.py` & `resotocore-3.5.2/resotocore/task/model.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/task/scheduler.py` & `resotocore-3.5.2/resotocore/task/scheduler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/task/start_workflow_on_first_subscriber.py` & `resotocore-3.5.2/resotocore/task/start_workflow_on_first_subscriber.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/task/subscribers.py` & `resotocore-3.5.2/resotocore/task/subscribers.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/task/task_description.py` & `resotocore-3.5.2/resotocore/task/task_description.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/task/task_handler.py` & `resotocore-3.5.2/resotocore/task/task_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/templates/base.html` & `resotocore-3.5.2/resotocore/templates/base.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/templates/create_first_user.html` & `resotocore-3.5.2/resotocore/templates/create_first_user.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/templates/login.html` & `resotocore-3.5.2/resotocore/templates/login.html`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/types.py` & `resotocore-3.5.2/resotocore/types.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/user/__init__.py` & `resotocore-3.5.2/resotocore/user/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,8 +108,8 @@
         List all users.
         :return: the list of users.
         """
 
 
 def config_model() -> List[Json]:
     config_classes: Set[Type[Any]] = {ResotoUsersConfig}
-    return dataclasses_to_resotocore_model(config_classes, allow_unknown_props=False)
+    return dataclasses_to_resotocore_model(config_classes, use_optional_as_required=True)
```

### Comparing `resotocore-3.5.1/resotocore/user/user_management.py` & `resotocore-3.5.2/resotocore/user/user_management.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/util.py` & `resotocore-3.5.2/resotocore/util.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/validator.py` & `resotocore-3.5.2/resotocore/validator.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/web/api.py` & `resotocore-3.5.2/resotocore/web/api.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,33 +50,36 @@
 from aiohttp.web_fileresponse import FileResponse
 from aiohttp.web_response import json_response
 from aiohttp_swagger3 import SwaggerFile, SwaggerUiSettings
 from aiostream import stream
 from attrs import evolve
 from networkx.readwrite import cytoscape_data
 from resotoui import ui_path
+from dateutil import parser as date_parser
 
 from resotocore.analytics import AnalyticsEventSender, AnalyticsEvent
 from resotocore.cli.command import alias_names
 from resotocore.cli.model import (
     ParsedCommandLine,
     CLIContext,
     CLICommand,
     InternalPart,
     WorkerCustomCommand,
     CLI,
     AliasTemplate,
+    InfraAppAlias,
 )
 from resotocore.config import ConfigHandler, ConfigValidation, ConfigEntity
 from resotocore.console_renderer import ConsoleColorSystem, ConsoleRenderer
 from resotocore.core_config import CoreConfig
 from resotocore.db.db_access import DbAccess
 from resotocore.db.graphdb import GraphDB, HistoryChange
 from resotocore.db.model import QueryModel
 from resotocore.error import NotFoundError
+from resotocore.graph_manager.graph_manager import GraphManager
 from resotocore.ids import TaskId, ConfigId, NodeId, SubscriberId, WorkerId, GraphName, Email, Password
 from resotocore.message_bus import MessageBus, Message, ActionDone, Action, ActionError, ActionInfo, ActionProgress
 from resotocore.model.db_updater import merge_graph_process
 from resotocore.model.graph_access import Section
 from resotocore.model.json_schema import json_schema
 from resotocore.model.model import Kind, Model
 from resotocore.model.model_handler import ModelHandler
@@ -156,14 +159,15 @@
         config_handler: ConfigHandler,
         inspector: Inspector,
         cli: CLI,
         query_parser: QueryParser,
         config: CoreConfig,
         user_management: UserManagement,
         get_override: Callable[[ConfigId], Optional[Json]],
+        graph_manager: GraphManager,
     ):
         self.db = db
         self.model_handler = model_handler
         self.subscription_handler = subscription_handler
         self.workflow_handler = workflow_handler
         self.message_bus = message_bus
         self.event_sender = event_sender
@@ -173,14 +177,15 @@
         self.inspector = inspector
         self.cli = cli
         self.query_parser = query_parser
         self.config = config
         self.user_management = user_management
         self.get_override = get_override
         self.auth_handler = AuthHandler(db.system_data_db, config, cert_handler, AlwaysAllowed | DeferredCheck)
+        self.graph_manager = graph_manager
 
         self.app = web.Application(
             client_max_size=config.api.max_request_size or 1024**2,
             # note on order: the middleware is passed in the order provided.
             middlewares=[
                 metrics_handler,
                 self.auth_handler.middleware(),
@@ -952,14 +957,26 @@
         await graph_db.abort_update(batch_id)
         return web.HTTPOk(body="Batch aborted.")
 
     async def graph_query_model_from_request(self, request: Request) -> Tuple[GraphDB, QueryModel]:
         section = section_of(request)
         query_string = await request.text()
         graph_name = GraphName(request.match_info.get("graph_id", "resoto"))
+        raw_at = request.query.get("at")
+        at = date_parser.parse(raw_at) if raw_at else None
+
+        snapshot_name = None
+
+        if at:
+            snapshot_name = await self.graph_manager.snapshot_at(time=at, graph_name=graph_name)
+            if not snapshot_name:
+                raise ValueError(f"No snapshot found for {graph_name} at {at}")
+
+        graph_name = snapshot_name or graph_name
+
         graph_db = self.db.get_graph_db(graph_name)
         q = await self.query_parser.parse_query(query_string, section, **request.query)
         m = await self.model_handler.load_model(graph_name)
         return graph_db, QueryModel(q, m)
 
     async def raw(self, request: Request) -> StreamResponse:
         graph_db, query_model = await self.graph_query_model_from_request(request)
@@ -1059,22 +1076,32 @@
                 "name": cmd.name,
                 "info": cmd.info,
                 "help": cmd.help(),
                 "args": to_js(cmd.args_info(), force_dict=True),
                 "source": cmd.allowed_in_source_position,
             }
 
+        def infra_app_alias_json(cmd: InfraAppAlias) -> Json:
+            return {
+                "name": cmd.name,
+                "info": cmd.description,
+                "help": cmd.readme,
+                "args": to_js(cmd.parameters, force_dict=True),
+                "source": True,
+            }
+
         commands = [cmd_json(cmd) for cmd in self.cli.direct_commands.values() if not isinstance(cmd, InternalPart)]
         replacements = self.cli.replacements()
         return web.json_response(
             {
                 "commands": commands,
                 "replacements": replacements,
                 "alias_names": alias_names(),
                 "alias_templates": [alias_json(alias) for alias in self.cli.alias_templates.values()],
+                "infra_app_aliases": [infra_app_alias_json(alias) for alias in self.cli.infra_app_aliases.values()],
             }
         )
 
     @staticmethod
     def cli_context_from_request(request: Request) -> CLIContext:
         try:
             columns = int(request.headers.get("Resoto-Shell-Columns", "120"))
```

### Comparing `resotocore-3.5.1/resotocore/web/auth.py` & `resotocore-3.5.2/resotocore/web/auth.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/web/certificate_handler.py` & `resotocore-3.5.2/resotocore/web/certificate_handler.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/web/content_renderer.py` & `resotocore-3.5.2/resotocore/web/content_renderer.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/web/directives.py` & `resotocore-3.5.2/resotocore/web/directives.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/web/tsdb.py` & `resotocore-3.5.2/resotocore/web/tsdb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore/worker_task_queue.py` & `resotocore-3.5.2/resotocore/worker_task_queue.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/resotocore.egg-info/PKG-INFO` & `resotocore-3.5.2/resotocore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotocore
-Version: 3.5.1
+Version: 3.5.2
 Summary: Keeps all the things.
 Author: Some Engineering Inc.
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `resotocore-3.5.1/resotocore.egg-info/SOURCES.txt` & `resotocore-3.5.2/resotocore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/__init__.py` & `resotocore-3.5.2/tests/resotocore/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/analytics/posthog_test.py` & `resotocore-3.5.2/tests/resotocore/analytics/posthog_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/analytics/recurrent_events_test.py` & `resotocore-3.5.2/tests/resotocore/analytics/recurrent_events_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/cli/cli_test.py` & `resotocore-3.5.2/tests/resotocore/cli/cli_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     FlattenCommand,
     UniqCommand,
     EchoCommand,
     AggregateToCountCommand,
     PredecessorsPart,
     DumpCommand,
 )
-from resotocore.cli.model import ParsedCommands, ParsedCommand, CLIContext, CLI
+from resotocore.cli.model import ParsedCommands, ParsedCommand, CLIContext, CLI, InfraAppAlias
 from resotocore.error import CLIParseError
 from resotocore.model.graph_access import EdgeTypes
 from resotocore.util import utc
 
 
 def test_strip() -> None:
     assert strip_quotes("'test'") == "test"
@@ -125,14 +125,19 @@
     result = await cli.execute_cli_command("help kind", stream.list)
     assert len(result[0]) == 1
 
     # help for alias template
     result = await cli.execute_cli_command("help discord", stream.list)
     assert len(result[0]) == 1
 
+    # help for infra app alias
+    cli.register_infra_app_alias(InfraAppAlias("testcommand", "this is a test alias", "this is a readme", []))
+    result = await cli.execute_cli_command("help testcommand", stream.list)
+    assert len(result[0]) == 1
+
 
 @pytest.mark.asyncio
 async def test_parse_env_vars(cli: CLI) -> None:
     result = await cli.execute_cli_command('test=foo bla="bar"   d=true env', stream.list)
     # the env is allowed to have more items. Check only for this subset.
     assert {"test": "foo", "bla": "bar", "d": True}.items() <= result[0][0].items()
```

### Comparing `resotocore-3.5.1/tests/resotocore/cli/command_test.py` & `resotocore-3.5.2/tests/resotocore/cli/command_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,53 +11,57 @@
 from _pytest.logging import LogCaptureFixture
 from aiohttp import ClientTimeout
 from aiohttp.web import Request
 from aiostream import stream
 from aiostream.core import Stream
 from attrs import evolve
 from pytest import fixture
+import asyncio
 
 from resotocore import version
 from resotocore.cli import is_node
 from resotocore.cli.cli import CLIService
-from resotocore.cli.command import HttpCommand, JqCommand, AggregateCommand
-from resotocore.cli.model import CLIContext, WorkerCustomCommand, CLI
+from resotocore.cli.command import HttpCommand, JqCommand, AggregateCommand, all_commands
 from resotocore.cli.dependencies import CLIDependencies
+from resotocore.cli.model import CLIContext, WorkerCustomCommand, CLI
 from resotocore.cli.tip_of_the_day import generic_tips
 from resotocore.console_renderer import ConsoleRenderer, ConsoleColorSystem
 from resotocore.db.graphdb import ArangoGraphDB
 from resotocore.db.jobdb import JobDb
 from resotocore.error import CLIParseError
-from resotocore.ids import InfraAppName
+from resotocore.graph_manager.graph_manager import GraphManager
+from resotocore.ids import InfraAppName, GraphName
 from resotocore.infra_apps.package_manager import PackageManager
 from resotocore.infra_apps.runtime import Runtime
 from resotocore.model.model import Model
 from resotocore.model.typed_model import to_js
 from resotocore.query.model import Template, Query
 from resotocore.report import Inspector
 from resotocore.report.report_config import BenchmarkConfig
 from resotocore.task.task_description import TimeTrigger, Workflow, EventTrigger
 from resotocore.task.task_handler import TaskHandlerService
 from resotocore.types import JsonElement, Json
 from resotocore.user import UsersConfigId
 from resotocore.util import AccessJson, utc_str, utc
 from resotocore.worker_task_queue import WorkerTask
-from resotocore.ids import InfraAppName, GraphName
-from resotocore.infra_apps.package_manager import PackageManager
-from resotocore.infra_apps.runtime import Runtime
-from resotocore.graph_manager.graph_manager import GraphManager
 from tests.resotocore.util_test import not_in_path
 
 
 @fixture
 def json_source() -> str:
     nums = ",".join([f'{{ "num": {a}, "inner": {{"num": {a%10}}}}}' for a in range(0, 100)])
     return "json [" + nums + "," + nums + "]"
 
 
+def test_known_category(cli_deps: CLIDependencies) -> None:
+    allowed_categories = {"search", "format", "action", "setup", "misc"}
+    for cmd in all_commands(cli_deps):
+        assert cmd.category in allowed_categories, f"Unknown category {cmd.category} for command {cmd.name}"
+
+
 @pytest.mark.asyncio
 async def test_echo_source(cli: CLI) -> None:
     # no arg passed to json
     result = await cli.execute_cli_command("echo", stream.list)
     assert result[0] == [""]
 
     # simple string passed to json
@@ -1095,27 +1099,34 @@
                     yaml.safe_load(file.read())
 
     # install a package
     assert "installed successfully" in (await execute("apps install cleanup-untagged", str))[0]
     manifest = await package_manager.get_manifest(InfraAppName("cleanup-untagged"))
     assert manifest is not None
     assert manifest.name == "cleanup-untagged"
+    # install discord app
+    assert "installed successfully" in (await execute("apps install discordapp", str))[0]
 
     # info about the app
     info_json = (await execute("apps info cleanup-untagged", Json))[0]
     assert info_json["name"] == "cleanup-untagged"
 
     # run the app
     result = await execute("apps run cleanup-untagged --dry-run", str)
     assert result[0].startswith("search /metadata.protected == false and /metadata.phantom")
 
     # run the app with stdin
     result = await execute("echo foo | apps run cleanup-untagged --dry-run", str)
     assert result[0].startswith("search /metadata.protected == false and /metadata.phantom")
 
+    # run discord app with stdin
+    result = await execute("search is(graph_root) | apps run discordapp --title foo --dry-run", str)
+    assert "http POST https://discordapp.com" in result[0]
+    await execute("apps uninstall discordapp", str)
+
     # update the app
     assert (
         "App cleanup-untagged updated sucessfully to the latest version"
         in (await execute("apps update cleanup-untagged", str))[0]
     )
 
     # update all apps
@@ -1249,17 +1260,28 @@
     snapshots = await graph_manager.list("snapshot.*")
     assert len(snapshots) == 1
     # implicitly use the current graph as a source
     await execute("graph snapshot foobar", str)
     snapshots = await graph_manager.list("snapshot.*")
     assert len(snapshots) == 2
     assert snapshots[0].startswith("snapshot")
+    await asyncio.sleep(1.1)
+
+    # search using a timestamp
+    at_timestamp = await execute(f"search is(graph_root) --at {utc_str()}", str)
+    assert at_timestamp == ["kind=graph_root, name=root"]
+    # search using timedelta
+    assert await execute("search is(graph_root) --at 0s", str) == ["kind=graph_root, name=root"]
+
     for snapshot in snapshots:
         await graph_manager.delete(GraphName(snapshot))
 
+    with pytest.raises(Exception):
+        await execute(f"search is(graph_root) --at {utc_str()}", str)
+
     # delete a graph
     await execute("graph delete graphtest2", str)
     graph_names = await graph_manager.list(None)
     assert set(graph_names) == {"ns", "graphtest", "graphtest3"}
 
     dump = os.path.join(tmp_directory, "dump")
```

### Comparing `resotocore-3.5.1/tests/resotocore/cli/model_test.py` & `resotocore-3.5.2/tests/resotocore/cli/model_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 from textwrap import dedent
 
-from resotocore.cli.model import CLIContext, AliasTemplate, AliasTemplateParameter
+from resotocore.cli.model import (
+    CLIContext,
+    AliasTemplate,
+    AliasTemplateParameter,
+    InfraAppAlias,
+    InfraAppAliasParameter,
+)
 from resotocore.console_renderer import ConsoleRenderer, ConsoleColorSystem
 
 
 def test_format() -> None:
     context = CLIContext()
     fn = context.formatter("foo={foo} and bla={bla}: {bar}")
     assert fn({}) == "foo=null and bla=null: null"
@@ -36,28 +42,28 @@
         """
         foo: does foes
         ```shell
         foo --a <value> --b <value>
         ```
 
         ## Parameters
-        - `a`: some a
-        - `b` [default: bv]: some b
+        - `--a` [required]: some a
+        - `--b` [default: bv]: some b
 
         ## Template
         ```shell
         > {{a}} | {{b}}
         ```
 
         ## Example
         ```shell
         # Executing this command
-        > foo --a "test_a"
+        > foo --a "test-a"
         # Will expand to this command
-        > test_a | bv
+        > test-a | bv
         ```
         """
     )
 
     tpl_no_args = AliasTemplate(
         "bla",
         "does blas",
@@ -80,7 +86,36 @@
             - `p1`: is doing awesome
             - `p2`: enables after burners
 
             This is doing bla
             """
         ).strip()
     )
+
+
+def test_infra_app_alias() -> None:
+    params = [
+        InfraAppAliasParameter(
+            name="param_a",
+            help="some a",
+            default=None,
+        ),
+        InfraAppAliasParameter(
+            name="param_b",
+            help="some b",
+            default="default_b",
+        ),
+    ]
+    alias = InfraAppAlias("foo", "does foes", "readme", params)
+    assert alias.render({"args": "args_go_here"}) == "apps run foo args_go_here"
+    assert alias.rendered_help(CLIContext()) == dedent(
+        """
+        foo: does foes
+        ```shell
+        foo --param-a <value> --param-b <value>
+        ```
+
+        readme
+        ## Parameters
+        - `--param-a` [required]: some a
+        - `--param-b` [default: default_b]: some b"""
+    )
```

### Comparing `resotocore-3.5.1/tests/resotocore/config/config_handler_service_test.py` & `resotocore-3.5.2/tests/resotocore/config/config_handler_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/config/config_override_service_test.py` & `resotocore-3.5.2/tests/resotocore/config/config_override_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/config/core_config_handler_test.py` & `resotocore-3.5.2/tests/resotocore/config/core_config_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/conftest.py` & `resotocore-3.5.2/tests/resotocore/conftest.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/console_renderer_test.py` & `resotocore-3.5.2/tests/resotocore/console_renderer_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/core_config_test.py` & `resotocore-3.5.2/tests/resotocore/core_config_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/db/arango_query_test.py` & `resotocore-3.5.2/tests/resotocore/db/arango_query_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/db/arangodb_functions_test.py` & `resotocore-3.5.2/tests/resotocore/db/arangodb_functions_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/db/async_arangodb_test.py` & `resotocore-3.5.2/tests/resotocore/db/async_arangodb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/db/configdb_test.py` & `resotocore-3.5.2/tests/resotocore/db/configdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/db/db_access_test.py` & `resotocore-3.5.2/tests/resotocore/db/db_access_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/db/entitydb.py` & `resotocore-3.5.2/tests/resotocore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/db/graphdb_test.py` & `resotocore-3.5.2/tests/resotocore/db/graphdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/db/jobdb_test.py` & `resotocore-3.5.2/tests/resotocore/db/jobdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/db/modeldb_test.py` & `resotocore-3.5.2/tests/resotocore/db/modeldb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/db/runningtaskdb_test.py` & `resotocore-3.5.2/tests/resotocore/db/runningtaskdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/db/subscriberdb_test.py` & `resotocore-3.5.2/tests/resotocore/db/subscriberdb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/db/system_data_db_test.py` & `resotocore-3.5.2/tests/resotocore/db/system_data_db_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/db/templatedb_test.py` & `resotocore-3.5.2/tests/resotocore/db/templatedb_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/dependencies_test.py` & `resotocore-3.5.2/tests/resotocore/dependencies_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/graph_manager/graph_manager_test.py` & `resotocore-3.5.2/tests/resotocore/graph_manager/graph_manager_test.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from resotocore.types import Json
 from resotocore.config.core_config_handler import CoreConfigHandler
 from resotocore.core_config import SnapshotsScheduleConfig, SnapshotSchedule, ResotoCoreSnapshotsConfigId
 from resotocore.task import TaskHandler
 import pytest
 from tests.resotocore.db.graphdb_test import create_multi_collector_graph
 import re
+from resotolib.utils import utc
+from datetime import timedelta
 
 
 @pytest.mark.asyncio
 async def test_graph_manager(
     foo_model: Model,
     db_access: DbAccess,
     core_config_handler: CoreConfigHandler,
@@ -51,32 +53,47 @@
     assert GraphName("test_graph") in await graph_manager.list(".*")
 
     # copy
     await graph_manager.copy(GraphName("test_graph"), GraphName("test_graph_copy"), False, False)
     assert set(await graph_manager.list(".*")).issuperset(["test_graph", "test_graph_copy"])
 
     # snapshot
-    await graph_manager.snapshot(GraphName("test_graph"), "label")
+    now = utc()
+    await graph_manager.snapshot(GraphName("test_graph"), "label", timestamp=now)
     graphs = await graph_manager.list(".*")
     for name in ["test_graph", "test_graph_copy", "snapshot-test_graph-label-.*"]:
         for graph in graphs:
             if re.match(name, graph):
                 break
         else:
             raise AssertionError(f"Could not find graph with name {name} in {graphs}")
 
+    # snapshots at specific time
+    now = now + timedelta(seconds=42)
+    await graph_manager.snapshot(GraphName("test_graph"), "label", timestamp=now)
+    somewhere_in_the_past = now
+    now = now + timedelta(seconds=42)
+    await graph_manager.snapshot(GraphName("test_graph"), "label", timestamp=now)
+    now = now + timedelta(seconds=42)
+    await graph_manager.snapshot(GraphName("test_graph"), "label", timestamp=now)
+    found = await graph_manager.snapshot_at(time=somewhere_in_the_past, graph_name=GraphName("test_graph"))
+    assert found is not None
+
     # test snapshot cleanup
     await graph_manager._clean_outdated_snapshots(
         SnapshotsScheduleConfig(snapshots={"label": SnapshotSchedule("0 1 2 3 4", 0)})
     )
     graphs = await graph_manager.list(".*")
     for graph in graphs:
         if re.match("snapshot-test_graph-label-.*", graph):
             raise AssertionError(f"Found outdated snapshot {graph} in {graphs}")
 
+    # no snapshots after the cleanup
+    assert await graph_manager.snapshot_at(time=somewhere_in_the_past, graph_name=GraphName("test_graph")) is None
+
     # delete
     await graph_manager.delete(GraphName("test_graph_copy"))
     assert GraphName("test_graph_copy") not in set(await graph_manager.list(".*"))
 
     # periodic snapshot callback
     for job in await task_handler.list_jobs():
         await task_handler.delete_job(job.id, force=True)
```

### Comparing `resotocore-3.5.1/tests/resotocore/hypothesis_extension.py` & `resotocore-3.5.2/tests/resotocore/hypothesis_extension.py`

 * *Files 16% similar despite different names*

```diff
@@ -38,24 +38,25 @@
     def draw(self, st: SearchStrategy[T]) -> T:
         return cast(T, self._drawer(st))
 
     def optional(self, st: SearchStrategy[T]) -> Optional[T]:
         return self.draw(optional(st))
 
 
+any_ws_digits_string = text(alphabet=string.ascii_letters + string.whitespace + string.digits, min_size=0, max_size=10)
 any_string = text(alphabet=string.ascii_letters, min_size=3, max_size=10)
 kind_gen = sampled_from(["volume", "instance", "load_balancer", "volume_type"])
 
 
 @composite
 def json_element_gen(ud: UD) -> JsonElement:
     return cast(JsonElement, ud(json_object_gen | json_simple_element_gen | json_array_gen))
 
 
-json_simple_element_gen = any_string | booleans() | integers(min_value=0, max_value=100000) | just(None)
+json_simple_element_gen = any_ws_digits_string | booleans() | integers(min_value=0, max_value=100000) | just(None)
 json_object_gen = dictionaries(any_string, json_element_gen(), min_size=1, max_size=5)
 json_array_gen = lists(json_element_gen(), max_size=5)
 
 
 @composite
 def node_gen(ud: UD) -> Json:
     d = Drawer(ud)
```

### Comparing `resotocore-3.5.1/tests/resotocore/infra_apps/local_runtime_test.py` & `resotocore-3.5.2/tests/resotocore/infra_apps/local_runtime_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/infra_apps/package_manager_test.py` & `resotocore-3.5.2/tests/resotocore/infra_apps/package_manager_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from typing import cast, Awaitable, Dict
 from resotocore.db.packagedb import PackageEntityDb, app_package_entity_db
 from resotocore.infra_apps.package_manager import PackageManager
 from resotocore.infra_apps.manifest import AppManifest
 from resotocore.ids import InfraAppName
 from resotocore.db.async_arangodb import AsyncArangoDB
 from resotocore.config import ConfigHandler
-from resotocore.cli.model import AliasTemplate
+from resotocore.cli.model import InfraAppAlias
 from arango.database import StandardDatabase
-from collections import defaultdict
 from types import SimpleNamespace
 import pytest
 from asyncio import Future
 import aiofiles
 import aiohttp
 from pathlib import Path
 
@@ -42,18 +41,18 @@
     ),
 )
 
 
 @pytest.mark.asyncio
 async def test_install_delete(package_entity_db: PackageEntityDb) -> None:
     name = InfraAppName("cleanup-untagged")
-    enabled_aliases: Dict[str, AliasTemplate] = {}
+    enabled_aliases: Dict[str, InfraAppAlias] = {}
 
-    def enable_alias(ta: AliasTemplate) -> None:
-        enabled_aliases[ta.name] = ta
+    def enable_alias(alias: InfraAppAlias) -> None:
+        enabled_aliases[alias.name] = alias
 
     def disable_alias(name: str) -> None:
         enabled_aliases.pop(name)
 
     package_manager = PackageManager(
         package_entity_db,
         config_handler,
@@ -74,16 +73,17 @@
     assert installed_app is not None
     assert installed_app.name == name
 
     # check that the alias is created
     alias_template = enabled_aliases.get(name)
     assert alias_template is not None
     assert alias_template.name == manifest.name
-    assert alias_template.template == f"apps run {manifest.name}" + r" {{args}}"
-    assert alias_template.info == manifest.description
+    assert alias_template.template() == f"apps run {manifest.name}" + r" {{args}}"
+    assert alias_template.description == manifest.description
+    assert alias_template.readme == manifest.readme
 
     # update is possible
     updated_manifest = await package_manager.update(name)
     assert updated_manifest is not None
     assert updated_manifest.name == name
 
     # update all is possible
```

### Comparing `resotocore-3.5.1/tests/resotocore/message_bus_test.py` & `resotocore-3.5.2/tests/resotocore/message_bus_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/model/__init__.py` & `resotocore-3.5.2/tests/resotocore/model/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/model/adjust_node_test.py` & `resotocore-3.5.2/tests/resotocore/model/adjust_node_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/model/db_updater_test.py` & `resotocore-3.5.2/tests/resotocore/model/db_updater_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/model/graph_access_test.py` & `resotocore-3.5.2/tests/resotocore/model/graph_access_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/model/json_schema_test.py` & `resotocore-3.5.2/tests/resotocore/model/json_schema_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/model/model_handler_test.py` & `resotocore-3.5.2/tests/resotocore/model/model_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/model/model_test.py` & `resotocore-3.5.2/tests/resotocore/model/model_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -479,56 +479,61 @@
           # The zip code.
           zip: '134'
           # The name of the city.
           # And another line.
           city: |-
             gotham
             manor house
+
           number: 123
           float: 1.2345
         # The list of addresses.
         addresses:
           - # The zip code.
             zip: '134'
             # The name of the city.
             # And another line.
             city: |-
               gotham
               manor house
+
             number: 123
             float: 1.2345
           - # The zip code.
             zip: '134'
             # The name of the city.
             # And another line.
             city: |-
               gotham
               manor house
+
             number: 123
             float: 1.2345
         # Other addresses.
         other_addresses:
           home:
             # The zip code.
             zip: '134'
             # The name of the city.
             # And another line.
             city: |-
               gotham
               manor house
+
             number: 123
             float: 1.2345
           work:
             # The zip code.
             zip: '134'
             # The name of the city.
             # And another line.
             city: |-
               gotham
               manor house
+
             number: 123
             float: 1.2345
         simple:
           - 1
           - 2
           - 3
           - 4
@@ -539,11 +544,11 @@
           """.rstrip()
     )
 
     assert person == yaml.safe_load(person_kind.create_yaml(person))
 
 
 @given(json_object_gen)
-@settings(max_examples=50, suppress_health_check=HealthCheck.all())
+@settings(max_examples=200, suppress_health_check=HealthCheck.all())
 def test_yaml_generation(js: Json) -> None:
     kind = ComplexKind("test", [], [])
     assert js == yaml.safe_load(kind.create_yaml(js))
```

### Comparing `resotocore-3.5.1/tests/resotocore/model/typed_model_test.py` & `resotocore-3.5.2/tests/resotocore/model/typed_model_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/query/__init__.py` & `resotocore-3.5.2/tests/resotocore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/query/model_test.py` & `resotocore-3.5.2/tests/resotocore/query/model_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/query/query_parser_test.py` & `resotocore-3.5.2/tests/resotocore/query/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/query/template_expander_test.py` & `resotocore-3.5.2/tests/resotocore/query/template_expander_test.py`

 * *Files 18% similar despite different names*

```diff
@@ -112,14 +112,33 @@
 
 def test_render_list() -> None:
     attrs = {"is": ["alb", "elb"]}
     res = render_template("query {{#is.with_index}}{{^first}} or {{/first}}is({{value}}){{/is.with_index}}", attrs)
     assert res == "query is(alb) or is(elb)"
 
 
+def test_render_as_list() -> None:
+    # dictionary as list: every item will be available as [{key: ..., value: ...}]
+    attrs: Json = {"props": {"foo": 1, "bla": 2, "bar": 3}}
+    res = render_template(
+        "query {{#props.as_list.with_index}}{{key}}=={{value}}{{^last}}, {{/last}}{{/props.as_list.with_index}}", attrs
+    )
+    assert res == "query foo==1, bla==2, bar==3"
+    # if the input is already a list, the items will be available as is
+    attrs = {"props": [{"key": "foo", "value": 1}, {"key": "bla", "value": 2}, {"key": "bar", "value": 3}]}
+    res = render_template(
+        "query {{#props.as_list.with_index}}{{key}}=={{value}}{{^last}}, {{/last}}{{/props.as_list.with_index}}", attrs
+    )
+    assert res == "query foo==1, bla==2, bar==3"
+    # if the input is neither dict or list, it will be wrapped in a single element list
+    attrs = {"props": "test"}
+    res = render_template("query {{#props.as_list.with_index}}{{value}}=={{index}}{{/props.as_list.with_index}}", attrs)
+    assert res == "query test==0"
+
+
 def test_from_now() -> None:
     res = render_template("{{delta.from_now}}", {"delta": "4h"})
     in_4_hours = utc() + timedelta(hours=4)
     assert abs((in_4_hours - from_utc(res)).total_seconds()) < 1
 
 
 def test_render_filter() -> None:
```

### Comparing `resotocore-3.5.1/tests/resotocore/report/benchnmark_renderer_test.py` & `resotocore-3.5.2/tests/resotocore/report/benchnmark_renderer_test.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,7 +12,13 @@
     bench_result = await inspector_service.perform_benchmark(GraphName("ns"), "test")
     render_result = [elem async for elem in respond_benchmark_result(stream.iterate(bench_result.to_graph()))]
     assert len(render_result) == 1
     assert (
         render_result[0]
         == "# Report for account sub_root\n\nTitle: test\n\nVersion: 1.5\n\nSummary: all 2 checks failed\n\n## Failed Checks \n\n- ❌ medium: Test\n- ❌ medium: Test\n\n\n## Section 1 (all checks ❌)\n\nTest section.\n\n- ❌ **medium**: Test\n\n  - Risk: Some risk\n\n  - There are 11 `foo` resources failing this check.\n\n  - Remediation: Some remediation text. See [Link](https://example.com) for more details.\n\n## Section 2 (all checks ❌)\n\nTest section.\n\n- ❌ **medium**: Test\n\n  - Risk: Some risk\n\n  - There are 11 `foo` resources failing this check.\n\n  - Remediation: Some remediation text. See [Link](https://example.com) for more details.\n\n"  # noqa: E501
     )
+
+    # only render checks
+    check_result = bench_result.to_graph(True)
+    assert len(check_result) == 2
+    for c in check_result:
+        assert c["kind"] == "report_check_result"
```

### Comparing `resotocore-3.5.1/tests/resotocore/report/inspector_service_test.py` & `resotocore-3.5.2/tests/resotocore/report/inspector_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/task/job_handler_test.py` & `resotocore-3.5.2/tests/resotocore/task/job_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/task/start_workflow_on_first_subscriber_test.py` & `resotocore-3.5.2/tests/resotocore/task/start_workflow_on_first_subscriber_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/task/subscribers_test.py` & `resotocore-3.5.2/tests/resotocore/task/subscribers_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/task/task_description_test.py` & `resotocore-3.5.2/tests/resotocore/task/task_description_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/task/task_handler_test.py` & `resotocore-3.5.2/tests/resotocore/task/task_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/user/user_management_service_test.py` & `resotocore-3.5.2/tests/resotocore/user/user_management_service_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/util_test.py` & `resotocore-3.5.2/tests/resotocore/util_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/validator_test.py` & `resotocore-3.5.2/tests/resotocore/validator_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/web/api_client.py` & `resotocore-3.5.2/tests/resotocore/web/api_client.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/web/api_test.py` & `resotocore-3.5.2/tests/resotocore/web/api_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,26 +6,29 @@
 import tempfile
 
 
 import pytest
 from _pytest.fixtures import fixture
 from aiohttp import ClientSession, MultipartReader
 from networkx import MultiDiGraph
+from datetime import timedelta
 from resotoclient import models as rc
 from resotoclient.async_client import ResotoClient
 
 from resotolib.utils import get_free_port
 from tests.resotocore import create_graph
 from resotocore.__main__ import run
 from resotocore.analytics import AnalyticsEvent
 from resotocore.db.db_access import DbAccess
 from resotocore.model.model import predefined_kinds, Kind
 from resotocore.model.typed_model import to_js
-from resotocore.util import rnd_str, AccessJson, utc
+from resotocore.util import rnd_str, AccessJson, utc, utc_str
 from resotocore.ids import GraphName
+from resotoclient.json_utils import json_loadb
+from resotoclient.models import JsObject
 
 
 def graph_to_json(graph: MultiDiGraph) -> List[rc.JsObject]:
     ga: List[rc.JsValue] = [{**node, "type": "node"} for _, node in graph.nodes(data=True)]
     for from_node, to_node, data in graph.edges(data=True):
         ga.append({"type": "edge", "from": from_node, "to": to_node, "edge_type": data["edge_type"]})
     return ga
@@ -270,14 +273,44 @@
     assert result_list[0].get("id") == "3"  # first node is the parent node
 
     # search graph
     result_graph = [res async for res in core_client.search_graph('id("3") -[0:]->', graph=g)]
     assert len(result_graph) == 21  # 11 nodes + 10 edges
     assert result_list[0].get("id") == "3"  # first node is the parent node
 
+    # search graph at specific timestamp
+    async def search_graph_at(
+        search: str, section: Optional[str] = "reported", graph: str = "resoto", at: Optional[str] = None
+    ) -> AsyncIterator[JsObject]:
+        params = {}
+        if section:
+            params["section"] = section
+        if at:
+            params["at"] = at
+        response = await core_client._post(f"/graph/{graph}/search/graph", params=params, data=search, stream=True)
+        if response.status_code == 200:
+            async for line in response.async_iter_lines():
+                yield json_loadb(line)
+        else:
+            raise AttributeError(await response.text())
+
+    with pytest.raises(AttributeError):
+        # no snapshots 420 weeks ago
+        result = [
+            res
+            async for res in search_graph_at('id("3") -[0:]->', graph=g, at=(utc() - timedelta(weeks=420)).isoformat())
+        ]
+        assert len(result) == 0
+
+    # create a snapshot
+    [result async for result in core_client.cli_execute("graph snapshot graphtest test_label")]
+    # now we should see some snapshots
+    result_graph = [res async for res in search_graph_at('id("3") -[0:]->', graph=g, at=utc_str())]
+    assert len(result_graph) == 21  # 11 nodes + 10 edges
+
     # aggregate
     result_aggregate = core_client.search_aggregate("aggregate(kind as kind: sum(1) as count): all", graph=g)
     assert {r["group"]["kind"]: r["count"] async for r in result_aggregate} == {
         "bla": 100,
         "cloud": 1,
         "foo": 11,
         "graph_root": 1,
```

### Comparing `resotocore-3.5.1/tests/resotocore/web/certificate_handler_test.py` & `resotocore-3.5.2/tests/resotocore/web/certificate_handler_test.py`

 * *Files identical despite different names*

### Comparing `resotocore-3.5.1/tests/resotocore/web/content_renderer_test.py` & `resotocore-3.5.2/tests/resotocore/web/content_renderer_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,16 +63,16 @@
 @settings(max_examples=20, suppress_health_check=HealthCheck.all(), deadline=1000)
 @pytest.mark.asyncio
 async def test_text_simple_elements(elements: List[JsonElement]) -> None:
     async with stream.iterate(elements).stream() as streamer:
         result = ""
         async for elem in respond_text(streamer):
             result += elem + "\n"
-        # every element is rendered as single line
-        assert len(elements) + 1 == len(result.split("\n"))
+        # every element is rendered as one or more line (string with \n is rendered as multiple lines)
+        assert len(elements) + 1 <= len(result.split("\n"))
 
 
 @given(lists(node_gen(), min_size=1, max_size=10))
 @settings(max_examples=20, suppress_health_check=HealthCheck.all(), deadline=1000)
 @pytest.mark.asyncio
 async def test_text_complex_elements(elements: List[JsonElement]) -> None:
     async with stream.iterate(elements).stream() as streamer:
```

### Comparing `resotocore-3.5.1/tests/resotocore/worker_task_queue_test.py` & `resotocore-3.5.2/tests/resotocore/worker_task_queue_test.py`

 * *Files identical despite different names*

