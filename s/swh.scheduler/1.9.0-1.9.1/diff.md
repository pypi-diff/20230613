# Comparing `tmp/swh.scheduler-1.9.0.tar.gz` & `tmp/swh.scheduler-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/swh.scheduler-1.9.0.tar", last modified: Wed May 31 08:19:27 2023, max compression
+gzip compressed data, was "dist/swh.scheduler-1.9.1.tar", last modified: Tue Jun 13 11:13:44 2023, max compression
```

## Comparing `swh.scheduler-1.9.0.tar` & `swh.scheduler-1.9.1.tar`

### file list

```diff
@@ -1,160 +1,161 @@
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/
--rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/.git-blame-ignore-revs
--rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)      882 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/.pre-commit-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/AUTHORS
--rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/CODE_OF_CONDUCT.md
--rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/CONTRIBUTORS
--rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/LICENSE
--rw-r--r--   0 jenkins    (115) docker     (999)     2630 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/LICENSE.Celery
--rw-r--r--   0 jenkins    (115) docker     (999)      154 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/MANIFEST.in
--rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/Makefile
--rw-r--r--   0 jenkins    (115) docker     (999)     1294 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)      292 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)      664 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/data/
--rw-r--r--   0 jenkins    (115) docker     (999)      646 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/data/README.md
--rw-r--r--   0 jenkins    (115) docker     (999)     1769 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/data/elastic-template.json
--rw-r--r--   0 jenkins    (115) docker     (999)       58 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/data/update-index-settings.json
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/docs/
--rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/docs/_static/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/_static/.placeholder
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/docs/_templates/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/_templates/.placeholder
--rw-r--r--   0 jenkins    (115) docker     (999)      887 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/cli.rst
--rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/conf.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7923 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/index.rst
--rw-r--r--   0 jenkins    (115) docker     (999)     3060 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/docs/simulator.rst
--rw-r--r--   0 jenkins    (115) docker     (999)      750 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/mypy.ini
--rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/pyproject.toml
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/pytest.ini
--rw-r--r--   0 jenkins    (115) docker     (999)       12 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/requirements-journal.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       21 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/requirements-simulator.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/requirements-swh.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      297 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/requirements-test.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      509 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/requirements.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/setup.cfg
--rwxr-xr-x   0 jenkins    (115) docker     (999)     2556 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/setup.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/sql/.gitignore
--rw-r--r--   0 jenkins    (115) docker     (999)     1384 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/sql/Makefile
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/
--rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/
--rw-r--r--   0 jenkins    (115) docker     (999)     2105 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/api/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/api/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      649 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/api/client.py
--rw-r--r--   0 jenkins    (115) docker     (999)      928 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/api/serializers.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4203 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/api/server.py
--rw-r--r--   0 jenkins    (115) docker     (999)    38368 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/backend.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/celery_backend/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/celery_backend/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13335 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/celery_backend/config.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3320 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/celery_backend/pika_listener.py
--rw-r--r--   0 jenkins    (115) docker     (999)    13193 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/celery_backend/recurrent_visits.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6758 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/celery_backend/runner.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/cli/
--rw-r--r--   0 jenkins    (115) docker     (999)     2912 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5302 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/add_forge_now.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7154 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/admin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4791 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/celery_monitor.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2111 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/journal.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7250 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/origin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2552 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/simulator.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12950 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/task.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7052 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/task_type.py
--rw-r--r--   0 jenkins    (115) docker     (999)      584 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/test_cli_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10293 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli/utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/cli_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)      473 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/exc.py
--rw-r--r--   0 jenkins    (115) docker     (999)    18240 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/interface.py
--rw-r--r--   0 jenkins    (115) docker     (999)    12011 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/journal_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8849 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/model.py
--rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/py.typed
--rw-r--r--   0 jenkins    (115) docker     (999)     3552 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/pytest_plugin.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/simulator/
--rw-r--r--   0 jenkins    (115) docker     (999)     5691 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/simulator/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     6293 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/simulator/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2331 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/simulator/origin_scheduler.py
--rw-r--r--   0 jenkins    (115) docker     (999)     7801 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/simulator/origins.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2706 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/simulator/task_scheduler.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/sql/
--rw-r--r--   0 jenkins    (115) docker     (999)       44 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/10-superuser-init.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    10833 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/30-schema.sql
--rw-r--r--   0 jenkins    (115) docker     (999)    14494 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/40-func.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5076 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/50-data.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/60-indexes.sql
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/__init__.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/
--rw-r--r--   0 jenkins    (115) docker     (999)     2111 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/02.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      661 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/03.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1561 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/04.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     5119 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/05.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      625 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/06.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1727 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/07.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1924 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/08.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     7034 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/09.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1581 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/10.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2070 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/11.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1769 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/12.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      967 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/13.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1729 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/14.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1126 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/15.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2467 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/16.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      152 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/17.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      328 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/18.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      958 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/19.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      210 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/20.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2467 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/23.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      471 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/24.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2944 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/25.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1478 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/26.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1113 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/27.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2112 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/28.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     1241 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/29.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      224 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/30-bis.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2991 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/30.sql
--rw-r--r--   0 jenkins    (115) docker     (999)      680 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/31.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     2182 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/32.sql
--rw-r--r--   0 jenkins    (115) docker     (999)     3628 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/33.sql
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2944 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/task.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/tests/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3682 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2630 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/conftest.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh/scheduler/tests/data/
--rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/data/__init__.py
--rw-r--r--   0 jenkins    (115) docker     (999)      555 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/data/logging-config.yaml
--rw-r--r--   0 jenkins    (115) docker     (999)     1357 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2568 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_api_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)    10759 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_celery_tasks.py
--rw-r--r--   0 jenkins    (115) docker     (999)    24126 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_cli.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5586 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_add_forge_now.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4174 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_celery_monitor.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3937 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_journal.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5687 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_origin.py
--rw-r--r--   0 jenkins    (115) docker     (999)     4019 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_task_type.py
--rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1952 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_common.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3859 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_config.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2836 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_init.py
--rw-r--r--   0 jenkins    (115) docker     (999)    30328 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_journal_client.py
--rw-r--r--   0 jenkins    (115) docker     (999)     2731 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_model.py
--rw-r--r--   0 jenkins    (115) docker     (999)     8573 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_recurrent_visits.py
--rw-r--r--   0 jenkins    (115) docker     (999)    61026 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_scheduler.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3532 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_server.py
--rw-r--r--   0 jenkins    (115) docker     (999)     1967 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_simulator.py
--rw-r--r--   0 jenkins    (115) docker     (999)     5366 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/tests/test_utils.py
--rw-r--r--   0 jenkins    (115) docker     (999)     3536 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/swh/scheduler/utils.py
-drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh.scheduler.egg-info/
--rw-r--r--   0 jenkins    (115) docker     (999)     1294 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh.scheduler.egg-info/PKG-INFO
--rw-r--r--   0 jenkins    (115) docker     (999)     4195 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh.scheduler.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh.scheduler.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins    (115) docker     (999)       98 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh.scheduler.egg-info/entry_points.txt
--rw-r--r--   0 jenkins    (115) docker     (999)      486 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh.scheduler.egg-info/requires.txt
--rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-05-31 08:19:27.000000 swh.scheduler-1.9.0/swh.scheduler.egg-info/top_level.txt
--rw-r--r--   0 jenkins    (115) docker     (999)     1681 2023-05-31 08:19:25.000000 swh.scheduler-1.9.0/tox.ini
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/
+-rw-r--r--   0 jenkins    (115) docker     (999)      140 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/.git-blame-ignore-revs
+-rw-r--r--   0 jenkins    (115) docker     (999)      129 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)      882 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/.pre-commit-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)      112 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/AUTHORS
+-rw-r--r--   0 jenkins    (115) docker     (999)     3397 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0 jenkins    (115) docker     (999)       14 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/CONTRIBUTORS
+-rw-r--r--   0 jenkins    (115) docker     (999)    35147 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/LICENSE
+-rw-r--r--   0 jenkins    (115) docker     (999)     2630 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/LICENSE.Celery
+-rw-r--r--   0 jenkins    (115) docker     (999)      154 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/MANIFEST.in
+-rw-r--r--   0 jenkins    (115) docker     (999)      163 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/Makefile
+-rw-r--r--   0 jenkins    (115) docker     (999)     1294 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)      292 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)      664 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)      646 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/data/README.md
+-rw-r--r--   0 jenkins    (115) docker     (999)     1769 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/data/elastic-template.json
+-rw-r--r--   0 jenkins    (115) docker     (999)       58 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/data/update-index-settings.json
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/docs/
+-rw-r--r--   0 jenkins    (115) docker     (999)       24 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)       39 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/docs/_static/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/_static/.placeholder
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/docs/_templates/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/_templates/.placeholder
+-rw-r--r--   0 jenkins    (115) docker     (999)      887 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/cli.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)       43 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/conf.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7923 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/index.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)     3060 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/docs/simulator.rst
+-rw-r--r--   0 jenkins    (115) docker     (999)      750 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/mypy.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)      237 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/pyproject.toml
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/pytest.ini
+-rw-r--r--   0 jenkins    (115) docker     (999)       12 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/requirements-journal.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       21 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/requirements-simulator.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       48 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/requirements-swh.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      297 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/requirements-test.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      509 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/requirements.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      120 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/setup.cfg
+-rwxr-xr-x   0 jenkins    (115) docker     (999)     2556 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/setup.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)       36 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/sql/.gitignore
+-rw-r--r--   0 jenkins    (115) docker     (999)     1384 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/sql/Makefile
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/
+-rw-r--r--   0 jenkins    (115) docker     (999)       76 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2105 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/api/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/api/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      649 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/api/client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      928 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/api/serializers.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4203 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/api/server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    38368 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/backend.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/celery_backend/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/celery_backend/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13335 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/celery_backend/config.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3320 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/celery_backend/pika_listener.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    13193 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/celery_backend/recurrent_visits.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6758 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/celery_backend/runner.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/cli/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2904 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5278 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/add_forge_now.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7130 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/admin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4791 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/celery_monitor.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2095 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/journal.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7280 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/origin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2552 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/simulator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12528 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/task.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7044 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/task_type.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      584 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/test_cli_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10293 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli/utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       62 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/cli_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      473 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/exc.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    18240 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/interface.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    12011 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/journal_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8849 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/model.py
+-rw-r--r--   0 jenkins    (115) docker     (999)       27 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/py.typed
+-rw-r--r--   0 jenkins    (115) docker     (999)     3552 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/pytest_plugin.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/simulator/
+-rw-r--r--   0 jenkins    (115) docker     (999)     5691 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/simulator/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     6293 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/simulator/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2331 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/simulator/origin_scheduler.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     7801 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/simulator/origins.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2706 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/simulator/task_scheduler.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/sql/
+-rw-r--r--   0 jenkins    (115) docker     (999)       44 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/10-superuser-init.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    10833 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/30-schema.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)    14607 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/40-func.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5076 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/50-data.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/60-indexes.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/__init__.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/
+-rw-r--r--   0 jenkins    (115) docker     (999)     2111 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/02.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      661 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/03.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1561 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/04.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     5119 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/05.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      625 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/06.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1727 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/07.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1924 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/08.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     7034 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/09.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1581 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/10.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2070 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/11.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1769 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/12.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      967 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/13.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1729 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/14.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1126 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/15.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2467 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/16.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      152 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/17.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      328 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/18.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      958 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/19.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      210 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/20.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2467 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/23.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      471 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/24.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2944 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/25.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1478 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/26.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1113 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/27.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2112 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/28.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1241 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/29.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      224 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/30-bis.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2991 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/30.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)      680 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/31.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     2182 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/32.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     3628 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/33.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)     1738 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/34.sql
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2944 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/task.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/tests/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3682 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2630 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/conftest.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh/scheduler/tests/data/
+-rw-r--r--   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/data/__init__.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      555 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/data/logging-config.yaml
+-rw-r--r--   0 jenkins    (115) docker     (999)     1357 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2568 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_api_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    10759 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_celery_tasks.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    24098 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_cli.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5595 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_add_forge_now.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4174 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_celery_monitor.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3765 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_journal.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5989 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_origin.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     4018 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_task_type.py
+-rw-r--r--   0 jenkins    (115) docker     (999)      704 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1952 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_common.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3859 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_config.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2836 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_init.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    30328 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_journal_client.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     2731 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_model.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     8555 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_recurrent_visits.py
+-rw-r--r--   0 jenkins    (115) docker     (999)    63287 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_scheduler.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3532 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_server.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     1967 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_simulator.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     5826 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/tests/test_utils.py
+-rw-r--r--   0 jenkins    (115) docker     (999)     3892 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/swh/scheduler/utils.py
+drwxr-xr-x   0 jenkins    (115) docker     (999)        0 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh.scheduler.egg-info/
+-rw-r--r--   0 jenkins    (115) docker     (999)     1294 2023-06-13 11:13:43.000000 swh.scheduler-1.9.1/swh.scheduler.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins    (115) docker     (999)     4229 2023-06-13 11:13:44.000000 swh.scheduler-1.9.1/swh.scheduler.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        1 2023-06-13 11:13:43.000000 swh.scheduler-1.9.1/swh.scheduler.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)       98 2023-06-13 11:13:43.000000 swh.scheduler-1.9.1/swh.scheduler.egg-info/entry_points.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)      486 2023-06-13 11:13:43.000000 swh.scheduler-1.9.1/swh.scheduler.egg-info/requires.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)        4 2023-06-13 11:13:43.000000 swh.scheduler-1.9.1/swh.scheduler.egg-info/top_level.txt
+-rw-r--r--   0 jenkins    (115) docker     (999)     1681 2023-06-13 11:13:42.000000 swh.scheduler-1.9.1/tox.ini
```

### Comparing `swh.scheduler-1.9.0/.pre-commit-config.yaml` & `swh.scheduler-1.9.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/CODE_OF_CONDUCT.md` & `swh.scheduler-1.9.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/LICENSE` & `swh.scheduler-1.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/LICENSE.Celery` & `swh.scheduler-1.9.1/LICENSE.Celery`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/PKG-INFO` & `swh.scheduler-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.scheduler
-Version: 1.9.0
+Version: 1.9.1
 Summary: Software Heritage Scheduler
 Home-page: https://forge.softwareheritage.org/diffusion/DSCH/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-scheduler
```

### Comparing `swh.scheduler-1.9.0/conftest.py` & `swh.scheduler-1.9.1/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/data/README.md` & `swh.scheduler-1.9.1/data/README.md`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/data/elastic-template.json` & `swh.scheduler-1.9.1/data/elastic-template.json`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/docs/cli.rst` & `swh.scheduler-1.9.1/docs/cli.rst`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/docs/index.rst` & `swh.scheduler-1.9.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/docs/simulator.rst` & `swh.scheduler-1.9.1/docs/simulator.rst`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/mypy.ini` & `swh.scheduler-1.9.1/mypy.ini`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/setup.py` & `swh.scheduler-1.9.1/setup.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/sql/Makefile` & `swh.scheduler-1.9.1/sql/Makefile`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/__init__.py` & `swh.scheduler-1.9.1/swh/scheduler/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/api/client.py` & `swh.scheduler-1.9.1/swh/scheduler/api/client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/api/serializers.py` & `swh.scheduler-1.9.1/swh/scheduler/api/serializers.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/api/server.py` & `swh.scheduler-1.9.1/swh/scheduler/api/server.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/backend.py` & `swh.scheduler-1.9.1/swh/scheduler/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,15 +49,15 @@
 
     return query.format(keys=query_keys, placeholders=placeholders)
 
 
 class SchedulerBackend:
     """Backend for the Software Heritage scheduling database."""
 
-    current_version = 33
+    current_version = 34
 
     def __init__(self, db, min_pool_conns=1, max_pool_conns=10):
         """
         Args:
             db_conn: either a libpq connection string, or a psycopg2 connection
 
         """
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/celery_backend/config.py` & `swh.scheduler-1.9.1/swh/scheduler/celery_backend/config.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/celery_backend/pika_listener.py` & `swh.scheduler-1.9.1/swh/scheduler/celery_backend/pika_listener.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/celery_backend/recurrent_visits.py` & `swh.scheduler-1.9.1/swh/scheduler/celery_backend/recurrent_visits.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/celery_backend/runner.py` & `swh.scheduler-1.9.1/swh/scheduler/celery_backend/runner.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/cli/__init__.py` & `swh.scheduler-1.9.1/swh/scheduler/cli/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
     ctx.ensure_object(dict)
 
     logger = logging.getLogger(__name__)
     scheduler = None
     conf = config.read(config_file, DEFAULT_CONFIG)
     if "scheduler" not in conf:
-        raise ValueError("missing 'scheduler' configuration")
+        ctx.fail("missing 'scheduler' configuration")
 
     if database:
         conf["scheduler"]["cls"] = "postgresql"
         conf["scheduler"]["db"] = database
     elif url:
         conf["scheduler"]["cls"] = "remote"
         conf["scheduler"]["url"] = url
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/cli/add_forge_now.py` & `swh.scheduler-1.9.1/swh/scheduler/cli/add_forge_now.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
     type=click.Choice(["production", "staging"]),
     help='Determine preset to use, "production" by default.',
 )
 @click.pass_context
 def add_forge_now(ctx, preset):
     """Manipulate add-forge-now requests."""
     if not ctx.obj["scheduler"]:
-        raise ValueError("Scheduler class (local/remote) must be instantiated")
+        ctx.fail("Scheduler class (local/remote) must be instantiated")
 
     ctx.obj["preset"] = preset
 
 
 @add_forge_now.command("register-lister")
 @click.argument("lister_name", nargs=1, required=True)
 @click.argument("options", nargs=-1)
@@ -71,15 +71,15 @@
     task_types: Dict[str, Dict] = {}
     for listing_type, task_type_name in task_type_names.items():
         task_type = scheduler.get_task_type(task_type_name)
         if task_type:
             task_types[listing_type] = task_type
 
     if not task_types:
-        raise ValueError(f"Unknown lister type {lister_name}.")
+        ctx.fail(f"Unknown lister type {lister_name}.")
 
     (args, kw) = parse_options(options)
 
     # Recurring policy on production
     if preset == "production":
         policy = "recurring"
     else:  # staging, "full" but limited listing as a oneshot
@@ -154,15 +154,15 @@
         if not task_type:
             unknown_task_types.append(visit_type_name)
             continue
         queue_name = task_type["backend_name"]
         visit_type_to_queue[visit_type_name] = f"{queue_name_prefix}:{queue_name}"
 
     if unknown_task_types:
-        raise ValueError(f"Unknown task types {','.join(unknown_task_types)}.")
+        ctx.fail(f"Unknown task types {','.join(unknown_task_types)}.")
 
     send_to_celery(
         scheduler,
         visit_type_to_queue=visit_type_to_queue,
         enabled=preset == "production",
         lister_name=lister_name,
         lister_instance_name=lister_instance_name,
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/cli/admin.py` & `swh.scheduler-1.9.1/swh/scheduler/cli/admin.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     logger = logging.getLogger(__name__ + ".runner")
     scheduler = ctx.obj["scheduler"]
     logger.debug("Scheduler %s", scheduler)
     task_types = []
     for task_type_name in task_type_names:
         task_type = scheduler.get_task_type(task_type_name)
         if not task_type:
-            raise ValueError(f"Unknown {task_type_name}")
+            ctx.fail(f"Unknown {task_type_name}")
         task_types.append(task_type)
 
     try:
         while True:
             logger.debug("Run ready tasks")
             try:
                 ntasks = len(run_ready_tasks(scheduler, app, task_types, with_priority))
@@ -91,15 +91,15 @@
 def listener(ctx):
     """Starts a swh-scheduler listener service.
 
     This service is responsible for listening at task lifecycle events and
     handle their workflow status in the database."""
     scheduler_backend = ctx.obj["scheduler"]
     if not scheduler_backend:
-        raise ValueError("Scheduler class (local/remote) must be instantiated")
+        ctx.fail("Scheduler class (local/remote) must be instantiated")
 
     broker = (
         ctx.obj["config"]
         .get("celery", {})
         .get("task_broker", "amqp://guest@localhost/%2f")
     )
 
@@ -155,15 +155,15 @@
             visit_types.append(task_type["type"][5:])
     else:
         # Check that the passed visit types exist in the scheduler
         for visit_type in visit_types:
             task_type_name = f"load-{visit_type}"
             task_type = scheduler.get_task_type(task_type_name)
             if not task_type:
-                raise ValueError(f"Unknown task type: {task_type_name}")
+                ctx.fail(f"Unknown task type: {task_type_name}")
 
     exc_queue: Queue[Tuple[str, BaseException]] = Queue()
     threads: VisitSchedulerThreads = {}
 
     try:
         # Spawn initial threads
         for visit_type in visit_types:
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/cli/celery_monitor.py` & `swh.scheduler-1.9.1/swh/scheduler/cli/celery_monitor.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/cli/journal.py` & `swh.scheduler-1.9.1/swh/scheduler/cli/journal.py`

 * *Files 6% similar despite different names*

```diff
@@ -32,21 +32,21 @@
     if not ctx.obj["scheduler"]:
         message = "Scheduler class (local/remote) must be instantiated."
         any_exception = ctx.obj.get("scheduler_exc")
         if any_exception:
             extra_message = f"Scheduler problems: {any_exception}"
             message = "\n".join([message, extra_message])
             logger.exception(any_exception)
-        raise ValueError(message)
+        ctx.fail(message)
 
     scheduler = ctx.obj["scheduler"]
     config = ctx.obj["config"]
 
     if "journal" not in config:
-        raise ValueError("Missing 'journal' configuration key")
+        ctx.fail("Missing 'journal' configuration key")
 
     journal_cfg = config["journal"]
     journal_cfg["stop_after_objects"] = stop_after_objects or journal_cfg.get(
         "stop_after_objects"
     )
 
     client = get_journal_client(
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/cli/origin.py` & `swh.scheduler-1.9.1/swh/scheduler/cli/origin.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,18 +21,19 @@
 
 
 @cli.group("origin")
 @click.pass_context
 def origin(ctx):
     """Manipulate listed origins."""
     if not ctx.obj["scheduler"]:
-        raise ValueError("Scheduler class (local/remote) must be instantiated")
+        ctx.fail("Scheduler class (local/remote) must be instantiated")
 
 
 def format_origins(
+    ctx: click.Context,
     origins: List[ListedOrigin],
     fields: Optional[List[str]] = None,
     with_header: bool = True,
 ) -> Iterable[str]:
     """Format a list of origins as CSV.
 
     Arguments:
@@ -49,17 +50,15 @@
 
     expected_fields = [field.name for field in attr.fields(ListedOrigin)]
     if not fields:
         fields = expected_fields
 
     unknown_fields = set(fields) - set(expected_fields)
     if unknown_fields:
-        raise ValueError(
-            "Unknown ListedOrigin field(s): %s" % ", ".join(unknown_fields)
-        )
+        ctx.fail("Unknown ListedOrigin field(s): %s" % ", ".join(unknown_fields))
 
     output = StringIO()
     writer = csv.writer(output)
 
     def csv_row(data):
         """Return a single CSV-formatted row. We clear the output buffer after we're
         done to keep it reasonably sized."""
@@ -103,15 +102,17 @@
         parsed_fields: Optional[List[str]] = fields.split(",")
     else:
         parsed_fields = None
 
     scheduler = ctx.obj["scheduler"]
 
     origins = scheduler.grab_next_visits(type, count, policy=policy)
-    for line in format_origins(origins, fields=parsed_fields, with_header=with_header):
+    for line in format_origins(
+        ctx, origins, fields=parsed_fields, with_header=with_header
+    ):
         click.echo(line)
 
 
 @origin.command("schedule-next")
 @click.option(
     "--policy", "-p", default="oldest_scheduled_first", help="Scheduling policy"
 )
@@ -197,15 +198,16 @@
 
     from .utils import get_task_type, send_to_celery
 
     scheduler = ctx.obj["scheduler"]
 
     task_type = get_task_type(scheduler, visit_type_name)
     if not task_type:
-        raise ValueError(f"Unknown task type {task_type}.")
+        ctx.fail(f"Unknown task type {task_type}.")
+        assert False  # for mypy
 
     queue_name = queue or task_type["backend_name"]
 
     send_to_celery(
         scheduler,
         visit_type_to_queue={visit_type_name: queue_name},
         policy=policy,
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/cli/simulator.py` & `swh.scheduler-1.9.1/swh/scheduler/cli/simulator.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/cli/task.py` & `swh.scheduler-1.9.1/swh/scheduler/cli/task.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,16 @@
 DATETIME = click.DateTime()
 
 
 @cli.group("task")
 @click.pass_context
 def task(ctx):
     """Manipulate tasks."""
-    pass
+    if not ctx.obj["scheduler"]:
+        ctx.fail("Scheduler class (local/remote) must be instantiated")
 
 
 @task.command("schedule")
 @click.option(
     "--columns",
     "-c",
     multiple=True,
@@ -81,16 +82,14 @@
     from swh.scheduler.utils import utcnow
 
     from .utils import pretty_print_task
 
     tasks = []
     now = utcnow()
     scheduler = ctx.obj["scheduler"]
-    if not scheduler:
-        raise ValueError("Scheduler class (local/remote) must be instantiated")
 
     reader = csv.reader(file, delimiter=delimiter)
     for line in reader:
         task = dict(zip(columns, line))
         args = json.loads(task.pop("args", "[]"))
         kwargs = json.loads(task.pop("kwargs", "{}"))
         task["arguments"] = {
@@ -140,20 +139,18 @@
     Note: if the priority is not given, the task won't have the priority set,
     which is considered as the lowest priority level.
 
     """
     from .utils import parse_options, task_add
 
     scheduler = ctx.obj["scheduler"]
-    if not scheduler:
-        raise ValueError("Scheduler class (local/remote) must be instantiated")
 
     task_type = scheduler.get_task_type(task_type_name)
     if not task_type:
-        raise ValueError(f"Unknown task name {task_type_name}.")
+        ctx.fail(f"Unknown task name {task_type_name}.")
 
     (args, kw) = parse_options(options)
     task_add(
         scheduler,
         task_type_name=task_type_name,
         policy=policy,
         priority=priority,
@@ -278,16 +275,14 @@
 
     You can override the number of tasks to fetch with the --limit flag.
 
     """
     from .utils import pretty_print_task
 
     scheduler = ctx.obj["scheduler"]
-    if not scheduler:
-        raise ValueError("Scheduler class (local/remote) must be instantiated")
 
     output = []
     for task_type in task_types:
         pending = scheduler.peek_ready_tasks(
             task_type,
             timestamp=before,
             num_tasks=num_tasks,
@@ -379,16 +374,14 @@
 ):
     """List tasks."""
     from operator import itemgetter
 
     from .utils import pretty_print_run, pretty_print_task
 
     scheduler = ctx.obj["scheduler"]
-    if not scheduler:
-        raise ValueError("Scheduler class (local/remote) must be instantiated")
 
     if not task_type:
         task_type = [x["type"] for x in scheduler.get_task_types()]
 
     # if task_id is not given, default value for status is
     #  'next_run_not_scheduled'
     # if task_id is given, default status is 'all'
@@ -450,16 +443,14 @@
     Eg.
 
        swh-scheduler task respawn 1 3 12
     """
     from swh.scheduler.utils import utcnow
 
     scheduler = ctx.obj["scheduler"]
-    if not scheduler:
-        raise ValueError("Scheduler class (local/remote) must be instantiated")
     if next_run is None:
         next_run = utcnow()
     output = []
 
     task_ids_int = [int(id_) for id_ in task_ids]
 
     scheduler.set_status_tasks(
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/cli/task_type.py` & `swh.scheduler-1.9.1/swh/scheduler/cli/task_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -40,15 +40,15 @@
 
 @cli.group("task-type")
 @click.pass_context
 def task_type(ctx):
     """Manipulate task types."""
     scheduler = ctx.obj["scheduler"]
     if not scheduler:
-        raise ValueError("Scheduler class (local/remote) must be instantiated")
+        ctx.fail("Scheduler class (local/remote) must be instantiated")
 
 
 @task_type.command("list")
 @click.option("--verbose", "-v", is_flag=True, default=False, help="Verbose mode")
 @click.option(
     "--task_type",
     "-t",
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/cli/test_cli_utils.py` & `swh.scheduler-1.9.1/swh/scheduler/cli/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/cli/utils.py` & `swh.scheduler-1.9.1/swh/scheduler/cli/utils.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/interface.py` & `swh.scheduler-1.9.1/swh/scheduler/interface.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/journal_client.py` & `swh.scheduler-1.9.1/swh/scheduler/journal_client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/model.py` & `swh.scheduler-1.9.1/swh/scheduler/model.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/pytest_plugin.py` & `swh.scheduler-1.9.1/swh/scheduler/pytest_plugin.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/simulator/__init__.py` & `swh.scheduler-1.9.1/swh/scheduler/simulator/__init__.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/simulator/common.py` & `swh.scheduler-1.9.1/swh/scheduler/simulator/common.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/simulator/origin_scheduler.py` & `swh.scheduler-1.9.1/swh/scheduler/simulator/origin_scheduler.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/simulator/origins.py` & `swh.scheduler-1.9.1/swh/scheduler/simulator/origins.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/simulator/task_scheduler.py` & `swh.scheduler-1.9.1/swh/scheduler/simulator/task_scheduler.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/30-schema.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/30-schema.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/40-func.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/40-func.sql`

 * *Files 0% similar despite different names*

```diff
@@ -34,25 +34,27 @@
     where not exists(select 1
                      from task
                      where type = t.type and
                            md5(arguments::text) = md5(t.arguments::text) and
                            arguments = t.arguments and
                            policy = t.policy and
                            priority is not distinct from t.priority and
-                           status = t.status);
+                           status = t.status and
+                           (policy != 'oneshot' or next_run = t.next_run));
 
   return query
     select distinct t.*
     from tmp_task tt inner join task t on (
       tt.type = t.type and
       md5(tt.arguments::text) = md5(t.arguments::text) and
       tt.arguments = t.arguments and
       tt.policy = t.policy and
       tt.priority is not distinct from t.priority and
-      tt.status = t.status
+      tt.status = t.status and
+      tt.next_run = t.next_run
     );
 end;
 $$;
 
 comment on function swh_scheduler_create_tasks_from_temp () is 'Create tasks in bulk from the temporary table';
 
 create or replace function swh_scheduler_peek_no_priority_tasks (task_type text, ts timestamptz default now(),
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/50-data.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/50-data.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/60-indexes.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/60-indexes.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/02.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/02.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/03.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/03.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/04.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/04.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/05.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/05.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/06.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/06.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/07.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/07.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/08.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/08.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/09.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/09.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/10.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/10.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/11.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/11.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/12.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/12.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/13.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/13.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/14.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/14.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/15.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/15.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/16.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/16.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/19.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/19.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/23.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/23.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/25.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/25.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/26.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/26.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/27.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/27.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/28.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/28.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/29.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/29.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/30.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/30.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/31.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/31.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/32.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/32.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/sql/upgrades/33.sql` & `swh.scheduler-1.9.1/swh/scheduler/sql/upgrades/33.sql`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/task.py` & `swh.scheduler-1.9.1/swh/scheduler/task.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/common.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/common.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/conftest.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/data/logging-config.yaml` & `swh.scheduler-1.9.1/swh/scheduler/tests/data/logging-config.yaml`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/tasks.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/tasks.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_api_client.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_celery_tasks.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_celery_tasks.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_cli.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -161,24 +161,26 @@
 """.lstrip()
     assert result.exit_code == 0, result.output
     assert re.fullmatch(expected, result.output, re.MULTILINE), result.output
 
 
 def test_schedule_unknown_task_type(swh_scheduler):
     """When scheduling unknown task type, the cli should raise."""
-    with pytest.raises(ValueError, match="Unknown"):
-        invoke(
-            swh_scheduler,
-            False,
-            [
-                "task",
-                "add",
-                "unknown-task-type-should-raise",
-            ],
-        )
+    result = invoke(
+        swh_scheduler,
+        True,
+        [
+            "task",
+            "add",
+            "unknown-task-type-should-raise",
+        ],
+    )
+
+    assert "Unknown" in result.output
+    assert result.exit_code != 0
 
 
 def test_list_pending_tasks_none(swh_scheduler):
     result = invoke(
         swh_scheduler,
         False,
         [
@@ -897,26 +899,27 @@
 
     task_types = swh_scheduler.get_task_types()
     task_type_names = [t["type"] for t in task_types]
     known_task_type = random.choice(task_type_names)
     unknown_task_type = "unknown-task-type"
     assert unknown_task_type not in task_type_names
 
-    with pytest.raises(ValueError, match="Unknown"):
-        invoke(
-            swh_scheduler,
-            False,
-            [
-                "start-runner",
-                "--task-type",
-                known_task_type,
-                "--task-type",
-                unknown_task_type,
-            ],
-        )
+    result = invoke(
+        swh_scheduler,
+        True,
+        [
+            "start-runner",
+            "--task-type",
+            known_task_type,
+            "--task-type",
+            unknown_task_type,
+        ],
+    )
+    assert "Unknown" in result.output
+    assert result.exit_code != 0
 
 
 @pytest.mark.parametrize("flag_priority", ["--with-priority", "--without-priority"])
 def test_cli_task_runner_with_known_tasks(
     swh_scheduler, storage, caplog, flag_priority
 ):
     """Trigger runner with known tasks runs smoothly."""
@@ -947,14 +950,14 @@
 def test_cli_task_runner_no_task(swh_scheduler, storage):
     """Trigger runner with no parameter should run as before."""
 
     # The runner will just iterate over the existing tasks from the scheduler and do
     # noop. We are just checking the runner does not explode here.
     result = invoke(
         swh_scheduler,
-        False,
+        True,
         [
             "start-runner",
         ],
     )
 
     assert result.exit_code == 0, result.output
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_add_forge_now.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_add_forge_now.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,25 +20,27 @@
     )
 
 
 def test_schedule_first_visits_cli_unknown_visit_type(
     swh_scheduler,
 ):
     "Calling cli without a known visit type should raise"
-    with pytest.raises(ValueError, match="Unknown"):
-        invoke(
-            swh_scheduler,
-            args=(
-                "schedule-first-visits",
-                "-t",
-                "unknown-vt0",
-                "--type-name",
-                "unknown-visit-type1",
-            ),
-        )
+    result = invoke(
+        swh_scheduler,
+        (
+            "schedule-first-visits",
+            "-t",
+            "unknown-vt0",
+            "--type-name",
+            "unknown-visit-type1",
+        ),
+        True,
+    )
+    assert "Unknown" in result.output
+    assert result.exit_code != 0
 
 
 @pytest.mark.parametrize(
     "cmd_args, subcmd_args",
     [
         ([], []),
         ([], ["--lister-name", "github", "--lister-instance-name", "github"]),
@@ -164,15 +166,17 @@
     assert len(expected_msgs) > 0
     for msg in expected_msgs:
         assert msg in output
 
 
 def test_register_lister_unknown_task_type(swh_scheduler):
     """When scheduling unknown task type, the cli should raise."""
-    with pytest.raises(ValueError, match="Unknown"):
-        invoke(
-            swh_scheduler,
-            [
-                "register-lister",
-                "unknown-lister-type-should-raise",
-            ],
-        )
+    result = invoke(
+        swh_scheduler,
+        [
+            "register-lister",
+            "unknown-lister-type-should-raise",
+        ],
+        True,
+    )
+    assert "Unknown" in result.output
+    assert result.exit_code != 0
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_celery_monitor.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_celery_monitor.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_journal.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_journal.py`

 * *Files 20% similar despite different names*

```diff
@@ -41,57 +41,55 @@
 
 @pytest.fixture
 def swh_scheduler_cfg_path(swh_scheduler_cfg, tmp_path):
     """Write scheduler configuration in temporary path and returns such path"""
     return _write_configuration_path(swh_scheduler_cfg, tmp_path)
 
 
-def invoke(args: List[str], config_path: str, catch_exceptions: bool = False) -> Result:
+def invoke(args: List[str], config_path: str) -> Result:
     """Invoke swh scheduler journal subcommands"""
     runner = CliRunner()
-    result = runner.invoke(cli, ["-C" + config_path] + args)
-    if not catch_exceptions and result.exception:
-        print(result.output)
-        raise result.exception
-    return result
+    return runner.invoke(cli, ["-C" + config_path] + args)
 
 
 def test_cli_journal_client_origin_visit_status_misconfiguration_no_scheduler(
     swh_scheduler_cfg, tmp_path
 ):
     config = swh_scheduler_cfg.copy()
     config["scheduler"] = {"cls": "foo"}
     config_path = _write_configuration_path(config, tmp_path)
-    with pytest.raises(ValueError, match="must be instantiated"):
-        invoke(
-            [
-                "journal-client",
-                "--stop-after-objects",
-                "1",
-            ],
-            config_path,
-        )
+    result = invoke(
+        [
+            "journal-client",
+            "--stop-after-objects",
+            "1",
+        ],
+        config_path,
+    )
+    assert "must be instantiated" in result.output
+    assert result.exit_code != 0
 
 
 def test_cli_journal_client_origin_visit_status_misconfiguration_missing_journal_conf(
     swh_scheduler_cfg, tmp_path
 ):
     config = swh_scheduler_cfg.copy()
     config.pop("journal", None)
     config_path = _write_configuration_path(config, tmp_path)
 
-    with pytest.raises(ValueError, match="Missing 'journal'"):
-        invoke(
-            [
-                "journal-client",
-                "--stop-after-objects",
-                "1",
-            ],
-            config_path,
-        )
+    result = invoke(
+        [
+            "journal-client",
+            "--stop-after-objects",
+            "1",
+        ],
+        config_path,
+    )
+    assert "Missing 'journal'" in result.output
+    assert result.exit_code != 0
 
 
 def test_cli_journal_client_origin_visit_status(
     swh_scheduler_cfg,
     swh_scheduler_cfg_path,
 ):
     kafka_server = swh_scheduler_cfg["journal"]["brokers"][0]
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_origin.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_origin.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Copyright (C) 2021  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from typing import Tuple
+from unittest.mock import MagicMock
 
 import pytest
 
 from swh.scheduler.cli.origin import format_origins
 from swh.scheduler.tests.common import TASK_TYPES
 from swh.scheduler.tests.test_cli import invoke as basic_invoke
 
@@ -25,36 +26,44 @@
 
     assert "Commands:" in result.stdout
 
 
 def test_format_origins_basic(listed_origins):
     listed_origins = listed_origins[:100]
 
-    basic_output = list(format_origins(listed_origins))
+    ctx = MagicMock()
+
+    basic_output = list(format_origins(ctx, listed_origins))
+    assert ctx.method_calls == []
     # 1 header line + all origins
     assert len(basic_output) == len(listed_origins) + 1
 
-    no_header_output = list(format_origins(listed_origins, with_header=False))
+    no_header_output = list(format_origins(ctx, listed_origins, with_header=False))
+    assert ctx.method_calls == []
     assert basic_output[1:] == no_header_output
 
 
 def test_format_origins_fields_unknown(listed_origins):
     listed_origins = listed_origins[:10]
 
-    it = format_origins(listed_origins, fields=["unknown_field"])
+    ctx = MagicMock()
+    it = format_origins(ctx, listed_origins, fields=["unknown_field"])
+    assert ctx.method_calls == []
 
-    with pytest.raises(ValueError, match="unknown_field"):
-        next(it)
+    next(it)
+    ctx.fail.assert_called()
 
 
 def test_format_origins_fields(listed_origins):
     listed_origins = listed_origins[:10]
     fields = ["lister_id", "url", "visit_type"]
 
-    output = list(format_origins(listed_origins, fields=fields))
+    ctx = MagicMock()
+    output = list(format_origins(ctx, listed_origins, fields=fields))
+    assert ctx.method_calls == []
     assert output[0] == ",".join(fields)
     for i, origin in enumerate(listed_origins):
         assert output[i + 1] == f"{origin.lister_id},{origin.url},{origin.visit_type}"
 
 
 def test_grab_next(swh_scheduler, listed_origins_by_type):
     NUM_RESULTS = 10
@@ -114,16 +123,21 @@
     assert scheduled_tasks <= all_possible_tasks
 
 
 def test_send_to_celery_unknown_visit_type(
     swh_scheduler,
 ):
     "Calling cli without a known visit type should raise"
-    with pytest.raises(ValueError, match="Unknown"):
-        invoke(swh_scheduler, args=("send-to-celery", "unknown-visit-type"))
+    result = invoke(
+        swh_scheduler,
+        args=("send-to-celery", "unknown-visit-type"),
+        catch_exceptions=True,
+    )
+    assert "Unknown" in result.output
+    assert result.exit_code != 0
 
 
 @pytest.mark.parametrize(
     "extra_cmd_args",
     [[], ["--lister-name", "github", "--lister-instance-name", "github"]],
 )
 def test_send_to_celery(
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_task_type.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_task_type.py`

 * *Files 3% similar despite different names*

```diff
@@ -121,9 +121,10 @@
         assert task_type_desc["type"] == task
         assert task_type_desc["backoff_factor"] == 1
 
 
 @pytest.mark.parametrize("cli_command", ["list", "register", "add"])
 def test_cli_task_type_raise(cli_runner, cli_command):
     """Without a proper configuration, the cli raises"""
-    with pytest.raises(ValueError, match="Scheduler class"):
-        cli_runner.invoke(cli, ["task-type", cli_command], catch_exceptions=False)
+    result = cli_runner.invoke(cli, ["task-type", cli_command])
+    assert "Scheduler class" in result.output
+    assert result.exit_code != 0
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_cli_utils.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_cli_utils.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_common.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_common.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_config.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_init.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_journal_client.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_journal_client.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_model.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_recurrent_visits.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_recurrent_visits.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,26 +59,27 @@
     }
 
 
 def test_cli_schedule_recurrent_unknown_visit_type(swh_scheduler):
     """When passed an unknown visit type, the recurrent visit scheduler should refuse
     to start."""
 
-    with pytest.raises(ValueError, match="Unknown"):
-        invoke(
-            swh_scheduler,
-            False,
-            [
-                "schedule-recurrent",
-                "--visit-type",
-                "unknown",
-                "--visit-type",
-                "test-git",
-            ],
-        )
+    result = invoke(
+        swh_scheduler,
+        True,
+        [
+            "schedule-recurrent",
+            "--visit-type",
+            "unknown",
+            "--visit-type",
+            "test-git",
+        ],
+    )
+    assert "Unknown" in result.output
+    assert result.exit_code != 0
 
 
 def test_cli_schedule_recurrent_noop(swh_scheduler, mocker):
     """When passing no visit types, the recurrent visit scheduler should start."""
 
     spawn_visit_scheduler_thread = mocker.patch(
         f"{MODULE_NAME}.spawn_visit_scheduler_thread"
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_scheduler.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_scheduler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,15 @@
-# Copyright (C) 2017-2022  The Software Heritage developers
+# Copyright (C) 2017-2023  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 from collections import defaultdict
 import copy
-import datetime
-from datetime import timedelta
+from datetime import datetime, timedelta, timezone
 import inspect
 import random
 from typing import Any, Dict, List, Optional, Tuple
 import uuid
 
 import attr
 from psycopg2.extras import execute_values
@@ -21,15 +20,15 @@
 from swh.scheduler.interface import ListedOriginPageToken, SchedulerInterface
 from swh.scheduler.model import (
     LastVisitStatus,
     ListedOrigin,
     OriginVisitStats,
     SchedulerMetrics,
 )
-from swh.scheduler.utils import utcnow
+from swh.scheduler.utils import create_oneshot_task_dict, utcnow
 
 from .common import (
     LISTERS,
     TASK_TYPES,
     TEMPLATES,
     tasks_from_template,
     tasks_with_priority_from_template,
@@ -154,14 +153,77 @@
                 del task["priority"]
                 assert task == orig_task
 
         expected_priorities = NUM_PRIORITY_TASKS.copy()
         expected_priorities[None] += num_git
         assert dict(actual_priorities) == expected_priorities
 
+    def test_create_tasks_with_custom_next_run(self, swh_scheduler):
+        self._create_task_types(swh_scheduler)
+        first_next_run = utcnow()
+        second_next_run = utcnow() + timedelta(hours=6)
+        task_type = TEMPLATES["test-git"]["type"]
+
+        tasks = swh_scheduler.create_tasks(
+            [create_oneshot_task_dict(task_type, next_run=first_next_run)]
+        )
+        assert tasks
+        assert tasks[0]["next_run"] == first_next_run
+
+        tasks += swh_scheduler.create_tasks(
+            [create_oneshot_task_dict(task_type, next_run=second_next_run)]
+        )
+        assert len(tasks) > 1
+        assert tasks[1]["next_run"] == second_next_run
+
+        ready_tasks = swh_scheduler.peek_ready_tasks(task_type, timestamp=utcnow())
+        assert ready_tasks
+        assert ready_tasks[0]["id"] == tasks[0]["id"]
+
+        ready_tasks = swh_scheduler.peek_ready_tasks(
+            task_type, timestamp=utcnow() + timedelta(hours=6)
+        )
+        assert len(ready_tasks) > 1
+        assert ready_tasks[1]["id"] == tasks[1]["id"]
+
+        grabbed_tasks = swh_scheduler.grab_ready_tasks(
+            task_type, timestamp=utcnow() + timedelta(hours=6)
+        )
+        assert len(grabbed_tasks) == len(ready_tasks)
+
+        backend_tasks = [
+            {
+                "task": task["id"],
+                "backend_id": str(uuid.uuid4()),
+                "scheduled": utcnow() + timedelta(hours=i * 6),
+            }
+            for i, task in enumerate(grabbed_tasks)
+        ]
+
+        swh_scheduler.mass_schedule_task_runs(backend_tasks)
+
+        task_runs = swh_scheduler.get_task_runs(task_ids=[task["id"] for task in tasks])
+        assert len(task_runs) == len(tasks)
+        for i, task in enumerate(backend_tasks):
+            status = "eventful"
+            start = utcnow() + timedelta(hours=i * 6)
+            end = start + timedelta(minutes=5)
+            task_run = swh_scheduler.start_task_run(
+                task["backend_id"],
+                timestamp=start,
+            )
+            task_run = swh_scheduler.end_task_run(
+                task["backend_id"],
+                status=status,
+                timestamp=end,
+            )
+            assert task_run["status"] == status
+            assert task_run["started"] == start
+            assert task_run["ended"] == end
+
     def test_peek_ready_tasks_no_priority(self, swh_scheduler):
         self._create_task_types(swh_scheduler)
         t = utcnow()
         task_type = TEMPLATES["test-git"]["type"]
         tasks = tasks_from_template(TEMPLATES["test-git"], t, 100)
         random.shuffle(tasks)
         swh_scheduler.create_tasks(tasks)
@@ -323,15 +385,15 @@
         self._create_task_types(swh_scheduler)
         t = utcnow()
         tasks = tasks_from_template(TEMPLATES["test-git"], t, 100)
         tasks = swh_scheduler.create_tasks(tasks)
         assert make_real_dicts(swh_scheduler.search_tasks()) == make_real_dicts(tasks)
 
     def assert_filtered_task_ok(
-        self, task: Dict[str, Any], after: datetime.datetime, before: datetime.datetime
+        self, task: Dict[str, Any], after: datetime, before: datetime
     ) -> None:
         """Ensure filtered tasks have the right expected properties
         (within the range, recurring disabled, etc..)
 
         """
         started = task["started"]
         date = started if started is not None else task["scheduled"]
@@ -908,15 +970,15 @@
         self, swh_scheduler, listed_origins_by_type
     ):
         visit_type, origins = self._grab_next_visits_setup(
             swh_scheduler, listed_origins_by_type
         )
 
         # Give all origins but one a last_scheduled date
-        base_date = datetime.datetime(2020, 1, 1, 0, 0, 0, tzinfo=datetime.timezone.utc)
+        base_date = datetime(2020, 1, 1, 0, 0, 0, tzinfo=timezone.utc)
         visit_stats = [
             OriginVisitStats(
                 url=origin.url,
                 visit_type=origin.visit_type,
                 last_snapshot=None,
                 last_successful=None,
                 last_visit=None,
@@ -1053,15 +1115,15 @@
         listed_origins_by_type,
     ):
         visit_type, origins = self._grab_next_visits_setup(
             swh_scheduler, listed_origins_by_type
         )
 
         # Update known origins with a `last_update` field that we control
-        base_date = datetime.datetime(2020, 1, 1, 0, 0, 0, tzinfo=datetime.timezone.utc)
+        base_date = datetime(2020, 1, 1, 0, 0, 0, tzinfo=timezone.utc)
         updated_origins = [
             attr.evolve(origin, last_update=base_date - timedelta(seconds=i))
             for i, origin in enumerate(origins)
         ]
         updated_origins = swh_scheduler.record_listed_origins(updated_origins)
 
         # We expect to retrieve origins with the oldest update date, that is
@@ -1081,15 +1143,15 @@
         listed_origins_by_type,
     ):
         visit_type, origins = self._grab_next_visits_setup(
             swh_scheduler, listed_origins_by_type
         )
 
         # Update known origins with a `last_update` field that we control
-        base_date = datetime.datetime(2020, 1, 1, 0, 0, 0, tzinfo=datetime.timezone.utc)
+        base_date = datetime(2020, 1, 1, 0, 0, 0, tzinfo=timezone.utc)
         updated_origins = [
             attr.evolve(origin, last_update=base_date - timedelta(seconds=i))
             for i, origin in enumerate(origins)
         ]
         updated_origins = swh_scheduler.record_listed_origins(updated_origins)
 
         # Update the visit stats with a known visit at a controlled date for
@@ -1284,15 +1346,15 @@
         # deterministic order)
         origin1 = attr.evolve(
             listed_origins[0], first_seen=utcnow(), last_seen=utcnow()
         )
         origin2 = attr.evolve(
             origin1,
             lister_id=lister2.id,
-            last_update=origin1.last_update + datetime.timedelta(seconds=10),
+            last_update=origin1.last_update + timedelta(seconds=10),
         )
 
         origins = [origin1, origin2]
         recorded_origins = swh_scheduler.record_listed_origins(origins)
 
         expected_origins = sorted(recorded_origins, key=lambda o: o.last_update)
 
@@ -1557,15 +1619,15 @@
         ret = swh_scheduler.update_metrics(lister_id=fake_uuid)
 
         assert len(ret) == 0
 
     def test_update_metrics_explicit_timestamp(self, swh_scheduler, listed_origins):
         swh_scheduler.record_listed_origins(listed_origins)
 
-        ts = datetime.datetime(2020, 1, 1, 0, 0, 0, tzinfo=datetime.timezone.utc)
+        ts = datetime(2020, 1, 1, 0, 0, 0, tzinfo=timezone.utc)
 
         ret = swh_scheduler.update_metrics(timestamp=ts)
 
         assert all(metric.last_update == ts for metric in ret)
 
     def test_update_metrics_twice(self, swh_scheduler, listed_origins):
         swh_scheduler.record_listed_origins(listed_origins)
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_server.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_simulator.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_simulator.py`

 * *Files identical despite different names*

### Comparing `swh.scheduler-1.9.0/swh/scheduler/tests/test_utils.py` & `swh.scheduler-1.9.1/swh/scheduler/tests/test_utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,82 +1,99 @@
 # Copyright (C) 2017-2022  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
-from datetime import timezone
-from unittest.mock import patch
+from datetime import datetime, timedelta, timezone
 import uuid
 
+import pytest
+
 from swh.scheduler import model, utils
 
 from .common import LISTERS
 
 
-@patch("swh.scheduler.utils.datetime")
-def test_create_oneshot_task_dict_simple(mock_datetime):
-    mock_datetime.now.return_value = "some-date"
+@pytest.fixture
+def mock_datetime(mocker):
+    now = datetime.now(tz=timezone.utc)
+    mock_datetime = mocker.patch("swh.scheduler.utils.datetime")
+    mock_datetime.now.return_value = now
+    return mock_datetime
+
 
+def test_create_oneshot_task_dict_simple(mock_datetime):
     actual_task = utils.create_oneshot_task_dict("some-task-type")
 
     expected_task = {
         "policy": "oneshot",
         "type": "some-task-type",
-        "next_run": "some-date",
+        "next_run": mock_datetime.now.return_value,
         "arguments": {
             "args": [],
             "kwargs": {},
         },
     }
 
     assert actual_task == expected_task
     mock_datetime.now.assert_called_once_with(tz=timezone.utc)
 
 
-@patch("swh.scheduler.utils.datetime")
-def test_create_oneshot_task_dict_other_call(mock_datetime):
-    mock_datetime.now.return_value = "some-other-date"
+def test_create_oneshot_task_dict_with_next_run():
+    next_run = datetime.now(tz=timezone.utc) + timedelta(hours=1)
+    actual_task = utils.create_oneshot_task_dict("some-task-type", next_run=next_run)
 
+    expected_task = {
+        "policy": "oneshot",
+        "type": "some-task-type",
+        "next_run": next_run,
+        "arguments": {
+            "args": [],
+            "kwargs": {},
+        },
+    }
+
+    assert actual_task == expected_task
+
+
+def test_create_oneshot_task_dict_other_call(mock_datetime):
     actual_task = utils.create_oneshot_task_dict(
         "some-task-type", "arg0", "arg1", priority="high", other_stuff="normal"
     )
 
     expected_task = {
         "policy": "oneshot",
         "type": "some-task-type",
-        "next_run": "some-other-date",
+        "next_run": mock_datetime.now.return_value,
         "arguments": {
             "args": ("arg0", "arg1"),
             "kwargs": {"other_stuff": "normal"},
         },
         "priority": "high",
     }
 
     assert actual_task == expected_task
     mock_datetime.now.assert_called_once_with(tz=timezone.utc)
 
 
-@patch("swh.scheduler.utils.datetime")
 def test_create_task_dict(mock_datetime):
-    mock_datetime.now.return_value = "date"
-
     actual_task = utils.create_task_dict(
         "task-type",
         "recurring",
         "arg0",
         "arg1",
         priority="low",
         other_stuff="normal",
         retries_left=3,
     )
 
     expected_task = {
         "policy": "recurring",
         "type": "task-type",
-        "next_run": "date",
+        "next_run": mock_datetime.now.return_value,
         "arguments": {
             "args": ("arg0", "arg1"),
             "kwargs": {"other_stuff": "normal"},
         },
         "priority": "low",
         "retries_left": 3,
     }
```

### Comparing `swh.scheduler-1.9.0/swh/scheduler/utils.py` & `swh.scheduler-1.9.1/swh/scheduler/utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # Copyright (C) 2017-2022  The Software Heritage developers
 # See the AUTHORS file at the top-level directory of this distribution
 # License: GNU General Public License version 3, or any later version
 # See top-level LICENSE file for more information
 
 
 from datetime import datetime, timezone
-from typing import Any, Dict, List
+from typing import Any, Dict, List, Optional
 
 from .interface import SchedulerInterface
 from .model import ListedOrigin, Lister
 
 
 def utcnow():
     return datetime.now(tz=timezone.utc)
@@ -30,23 +30,27 @@
     from swh.scheduler.celery_backend.config import app
 
     for module in app.conf.CELERY_IMPORTS:
         __import__(module)
     return app.tasks[task_name]
 
 
-def create_task_dict(type, policy, *args, **kwargs):
+def create_task_dict(
+    type: str, policy: str, *args, next_run: Optional[datetime] = None, **kwargs
+) -> Dict[str, Any]:
     """Create a task with type and policy, scheduled for as soon as
        possible.
 
     Args:
-        type (str): Type of oneshot task as per swh-scheduler's db
+        type: Type of oneshot task as per swh-scheduler's db
                     table task_type's column (Ex: load-git,
                     check-deposit)
-        policy (str): oneshot or recurring policy
+        policy: oneshot or recurring policy
+        next_run: optional date and time from which the task can be executed,
+            use current time otherwise
 
     Returns:
         Expected dictionary for the one-shot task scheduling api
         (swh.scheduler.backend.create_tasks)
 
     """
     task_extra = {}
@@ -54,15 +58,15 @@
         if extra_key in kwargs:
             extra_val = kwargs.pop(extra_key)
             task_extra[extra_key] = extra_val
 
     task = {
         "policy": policy,
         "type": type,
-        "next_run": utcnow(),
+        "next_run": next_run or utcnow(),
         "arguments": {
             "args": args if args else [],
             "kwargs": kwargs if kwargs else {},
         },
     }
     task.update(task_extra)
     return task
@@ -100,21 +104,24 @@
 
     missing_lister_ids = lister_ids - set(listers)
     assert not missing_lister_ids, f"Missing listers: {missing_lister_ids}"
 
     return [create_origin_task_dict(o, listers[o.lister_id]) for o in origins]
 
 
-def create_oneshot_task_dict(type, *args, **kwargs):
+def create_oneshot_task_dict(
+    type: str, *args, next_run: Optional[datetime] = None, **kwargs
+):
     """Create a oneshot task scheduled for as soon as possible.
 
     Args:
-        type (str): Type of oneshot task as per swh-scheduler's db
-                    table task_type's column (Ex: load-git,
-                    check-deposit)
+        type: Type of oneshot task as per swh-scheduler's db
+            table task_type's column (Ex: load-git, check-deposit)
+        next_run: optional date and time from which the task can be executed,
+            use current time otherwise
 
     Returns:
         Expected dictionary for the one-shot task scheduling api
-        (swh.scheduler.backend.create_tasks)
+        (:func:`swh.scheduler.backend.create_tasks`)
 
     """
-    return create_task_dict(type, "oneshot", *args, **kwargs)
+    return create_task_dict(type, "oneshot", *args, next_run=next_run, **kwargs)
```

### Comparing `swh.scheduler-1.9.0/swh.scheduler.egg-info/PKG-INFO` & `swh.scheduler-1.9.1/swh.scheduler.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: swh.scheduler
-Version: 1.9.0
+Version: 1.9.1
 Summary: Software Heritage Scheduler
 Home-page: https://forge.softwareheritage.org/diffusion/DSCH/
 Author: Software Heritage developers
 Author-email: swh-devel@inria.fr
 Project-URL: Bug Reports, https://forge.softwareheritage.org/maniphest
 Project-URL: Funding, https://www.softwareheritage.org/donate
 Project-URL: Source, https://forge.softwareheritage.org/source/swh-scheduler
```

### Comparing `swh.scheduler-1.9.0/swh.scheduler.egg-info/SOURCES.txt` & `swh.scheduler-1.9.1/swh.scheduler.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -110,14 +110,15 @@
 swh/scheduler/sql/upgrades/28.sql
 swh/scheduler/sql/upgrades/29.sql
 swh/scheduler/sql/upgrades/30-bis.sql
 swh/scheduler/sql/upgrades/30.sql
 swh/scheduler/sql/upgrades/31.sql
 swh/scheduler/sql/upgrades/32.sql
 swh/scheduler/sql/upgrades/33.sql
+swh/scheduler/sql/upgrades/34.sql
 swh/scheduler/sql/upgrades/__init__.py
 swh/scheduler/tests/__init__.py
 swh/scheduler/tests/common.py
 swh/scheduler/tests/conftest.py
 swh/scheduler/tests/tasks.py
 swh/scheduler/tests/test_api_client.py
 swh/scheduler/tests/test_celery_tasks.py
```

### Comparing `swh.scheduler-1.9.0/tox.ini` & `swh.scheduler-1.9.1/tox.ini`

 * *Files identical despite different names*

