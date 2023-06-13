# Comparing `tmp/yz-core2-1.0.53.tar.gz` & `tmp/yz-core2-1.0.54.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yz-core2-1.0.53.tar", last modified: Tue May 30 09:52:35 2023, max compression
+gzip compressed data, was "yz-core2-1.0.54.tar", last modified: Tue Jun 13 08:36:58 2023, max compression
```

## Comparing `yz-core2-1.0.53.tar` & `yz-core2-1.0.54.tar`

### file list

```diff
@@ -1,125 +1,127 @@
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.715093 yz-core2-1.0.53/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2023-04-21 02:16:16.000000 yz-core2-1.0.53/LICENSE
--rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-05-30 09:52:35.714837 yz-core2-1.0.53/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-21 02:16:16.000000 yz-core2-1.0.53/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-05-30 09:52:35.715153 yz-core2-1.0.53/setup.cfg
--rw-r--r--   0 zhouwei    (501) staff       (20)     1782 2023-05-30 09:47:56.000000 yz-core2-1.0.53/setup.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.652122 yz-core2-1.0.53/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       94 2023-04-21 02:16:16.000000 yz-core2-1.0.53/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      965 2023-04-21 02:16:16.000000 yz-core2-1.0.53/tests/test_setting_reload.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2023-04-21 02:16:16.000000 yz-core2-1.0.53/tests/test_uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.653092 yz-core2-1.0.53/yz_core2.egg-info/
--rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-05-30 09:52:35.000000 yz-core2-1.0.53/yz_core2.egg-info/PKG-INFO
--rw-r--r--   0 zhouwei    (501) staff       (20)     3386 2023-05-30 09:52:35.000000 yz-core2-1.0.53/yz_core2.egg-info/SOURCES.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-05-30 09:52:35.000000 yz-core2-1.0.53/yz_core2.egg-info/dependency_links.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-05-30 09:52:35.000000 yz-core2-1.0.53/yz_core2.egg-info/entry_points.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)      239 2023-05-30 09:52:35.000000 yz-core2-1.0.53/yz_core2.egg-info/requires.txt
--rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-05-30 09:52:35.000000 yz-core2-1.0.53/yz_core2.egg-info/top_level.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.654530 yz-core2-1.0.53/yzcore/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      440 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/__main__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.655496 yz-core2-1.0.53/yzcore/core/
--rw-r--r--   0 zhouwei    (501) staff       (20)       95 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/core/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      301 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/core/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      466 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/core/data_hash.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/core/datastructures.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/core/encoders.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.656196 yz-core2-1.0.53/yzcore/core/management/
--rw-r--r--   0 zhouwei    (501) staff       (20)      614 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/core/management/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      122 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/core/management/base.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.656622 yz-core2-1.0.53/yzcore/core/management/commands/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/core/management/commands/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      594 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/core/management/commands/startapp.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      783 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/core/management/commands/startproject.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/core/management/templates.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     6459 2023-05-05 06:04:45.000000 yz-core2-1.0.53/yzcore/core/storage.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.657412 yz-core2-1.0.53/yzcore/db/
--rw-r--r--   0 zhouwei    (501) staff       (20)       92 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/db/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1413 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/db/db_session.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/db/pymongo_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/db/sqlalchemy_crud_base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/decorators.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2525 2023-05-16 05:58:39.000000 yz-core2-1.0.53/yzcore/default_settings.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2433 2023-04-25 02:04:21.000000 yz-core2-1.0.53/yzcore/exceptions.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.657670 yz-core2-1.0.53/yzcore/extensions/
--rw-r--r--   0 zhouwei    (501) staff       (20)       93 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/extensions/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.658769 yz-core2-1.0.53/yzcore/extensions/storage/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1678 2023-04-25 07:27:56.000000 yz-core2-1.0.53/yzcore/extensions/storage/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.659058 yz-core2-1.0.53/yzcore/extensions/storage/azure/
--rw-r--r--   0 zhouwei    (501) staff       (20)     7411 2023-05-11 08:40:13.000000 yz-core2-1.0.53/yzcore/extensions/storage/azure/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10752 2023-05-11 08:37:54.000000 yz-core2-1.0.53/yzcore/extensions/storage/base.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      634 2023-04-21 07:30:35.000000 yz-core2-1.0.53/yzcore/extensions/storage/const.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.659257 yz-core2-1.0.53/yzcore/extensions/storage/minio/
--rw-r--r--   0 zhouwei    (501) staff       (20)     9571 2023-05-30 09:47:10.000000 yz-core2-1.0.53/yzcore/extensions/storage/minio/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.666708 yz-core2-1.0.53/yzcore/extensions/storage/obs/
--rw-r--r--   0 zhouwei    (501) staff       (20)     8886 2023-05-06 03:12:37.000000 yz-core2-1.0.53/yzcore/extensions/storage/obs/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2023-04-21 02:05:49.000000 yz-core2-1.0.53/yzcore/extensions/storage/obs/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     3101 2023-05-06 02:48:14.000000 yz-core2-1.0.53/yzcore/extensions/storage/obs/obs_inherit.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      654 2023-04-25 06:07:27.000000 yz-core2-1.0.53/yzcore/extensions/storage/obs/utils.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.667289 yz-core2-1.0.53/yzcore/extensions/storage/oss/
--rw-r--r--   0 zhouwei    (501) staff       (20)    12259 2023-05-06 03:12:38.000000 yz-core2-1.0.53/yzcore/extensions/storage/oss/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      762 2023-04-21 02:05:49.000000 yz-core2-1.0.53/yzcore/extensions/storage/oss/const.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1272 2023-05-30 09:09:30.000000 yz-core2-1.0.53/yzcore/extensions/storage/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      265 2023-04-21 02:05:49.000000 yz-core2-1.0.53/yzcore/extensions/storage/utils.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/extensions/uid.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.668213 yz-core2-1.0.53/yzcore/logger/
--rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/logger/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/logger/config.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/logger/filters.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/logger/handlers.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.668592 yz-core2-1.0.53/yzcore/request/
--rw-r--r--   0 zhouwei    (501) staff       (20)      133 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/request/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/request/aio_http.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.669229 yz-core2-1.0.53/yzcore/response/
--rw-r--r--   0 zhouwei    (501) staff       (20)      188 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/response/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/response/response.py
--rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/response/response_code.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.669474 yz-core2-1.0.53/yzcore/templates/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.670786 yz-core2-1.0.53/yzcore/templates/app_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/app_template/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      945 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/app_template/controllers.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      421 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/app_template/models.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      907 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/app_template/schemas.py
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/app_template/tests.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/app_template/views.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.705221 yz-core2-1.0.53/yzcore/templates/project_template/
--rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/.gitignore
--rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/README.md
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.705551 yz-core2-1.0.53/yzcore/templates/project_template/docs/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/docs/install_explain.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      922 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/docs/supervisor.ini
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.705744 yz-core2-1.0.53/yzcore/templates/project_template/migrations/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/migrations/README.md
--rw-r--r--   0 zhouwei    (501) staff       (20)      453 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/requirements.txt
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.706283 yz-core2-1.0.53/yzcore/templates/project_template/src/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.706441 yz-core2-1.0.53/yzcore/templates/project_template/src/apps/
--rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/apps/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.707333 yz-core2-1.0.53/yzcore/templates/project_template/src/conf/
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/conf/config_dev.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/conf/config_dev.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/conf/config_production.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/conf/config_production.yaml
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/conf/config_testing.ini
--rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/conf/config_testing.yaml
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.707866 yz-core2-1.0.53/yzcore/templates/project_template/src/const/
--rw-r--r--   0 zhouwei    (501) staff       (20)      157 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/const/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      409 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/const/_job.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      418 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/const/_task.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      843 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/main.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      807 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/settings.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.709054 yz-core2-1.0.53/yzcore/templates/project_template/src/tests/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/tests/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      840 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/tests/test_xxx.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.709342 yz-core2-1.0.53/yzcore/templates/project_template/src/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/templates/project_template/src/utils/__init__.py
-drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-05-30 09:52:35.714291 yz-core2-1.0.53/yzcore/utils/
--rw-r--r--   0 zhouwei    (501) staff       (20)      386 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/utils/__init__.py
--rw-r--r--   0 zhouwei    (501) staff       (20)      231 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/utils/check_path.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/utils/check_sys.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/utils/crypto.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1830 2023-05-10 06:22:06.000000 yz-core2-1.0.53/yzcore/utils/decorator.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/utils/encoding.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2023-04-21 02:16:16.000000 yz-core2-1.0.53/yzcore/utils/nacos.py
--rw-r--r--   0 zhouwei    (501) staff       (20)     2129 2023-05-09 10:16:49.000000 yz-core2-1.0.53/yzcore/utils/time_utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.843845 yz-core2-1.0.54/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1085 2023-04-21 02:16:16.000000 yz-core2-1.0.54/LICENSE
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-06-13 08:36:58.843695 yz-core2-1.0.54/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2509 2023-04-21 02:16:16.000000 yz-core2-1.0.54/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)       38 2023-06-13 08:36:58.843886 yz-core2-1.0.54/setup.cfg
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1782 2023-06-13 08:35:25.000000 yz-core2-1.0.54/setup.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.827098 yz-core2-1.0.54/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       94 2023-04-21 02:16:16.000000 yz-core2-1.0.54/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      965 2023-04-21 02:16:16.000000 yz-core2-1.0.54/tests/test_setting_reload.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1822 2023-04-21 02:16:16.000000 yz-core2-1.0.54/tests/test_uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.827989 yz-core2-1.0.54/yz_core2.egg-info/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3112 2023-06-13 08:36:58.000000 yz-core2-1.0.54/yz_core2.egg-info/PKG-INFO
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3431 2023-06-13 08:36:58.000000 yz-core2-1.0.54/yz_core2.egg-info/SOURCES.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)        1 2023-06-13 08:36:58.000000 yz-core2-1.0.54/yz_core2.egg-info/dependency_links.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       48 2023-06-13 08:36:58.000000 yz-core2-1.0.54/yz_core2.egg-info/entry_points.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)      239 2023-06-13 08:36:58.000000 yz-core2-1.0.54/yz_core2.egg-info/requires.txt
+-rw-r--r--   0 zhouwei    (501) staff       (20)       13 2023-06-13 08:36:58.000000 yz-core2-1.0.54/yz_core2.egg-info/top_level.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.829097 yz-core2-1.0.54/yzcore/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      440 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/__main__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.830261 yz-core2-1.0.54/yzcore/core/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       95 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/core/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      301 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/core/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      466 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/core/data_hash.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     4722 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/core/datastructures.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5244 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/core/encoders.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.830793 yz-core2-1.0.54/yzcore/core/management/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      614 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/core/management/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      122 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/core/management/base.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.831237 yz-core2-1.0.54/yzcore/core/management/commands/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/core/management/commands/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      594 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/core/management/commands/startapp.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      783 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/core/management/commands/startproject.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     5219 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/core/management/templates.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6459 2023-05-05 06:04:45.000000 yz-core2-1.0.54/yzcore/core/storage.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.831967 yz-core2-1.0.54/yzcore/db/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       92 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/db/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1413 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/db/db_session.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7679 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/db/pymongo_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7165 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/db/sqlalchemy_crud_base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1651 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/decorators.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2525 2023-05-16 05:58:39.000000 yz-core2-1.0.54/yzcore/default_settings.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2433 2023-04-25 02:04:21.000000 yz-core2-1.0.54/yzcore/exceptions.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.832371 yz-core2-1.0.54/yzcore/extensions/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       93 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/extensions/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.833375 yz-core2-1.0.54/yzcore/extensions/storage/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1678 2023-04-25 07:27:56.000000 yz-core2-1.0.54/yzcore/extensions/storage/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.833683 yz-core2-1.0.54/yzcore/extensions/storage/amazon/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:31:05.000000 yz-core2-1.0.54/yzcore/extensions/storage/amazon/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.833770 yz-core2-1.0.54/yzcore/extensions/storage/azure/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     7411 2023-05-11 08:40:13.000000 yz-core2-1.0.54/yzcore/extensions/storage/azure/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10752 2023-05-11 08:37:54.000000 yz-core2-1.0.54/yzcore/extensions/storage/base.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      634 2023-04-21 07:30:35.000000 yz-core2-1.0.54/yzcore/extensions/storage/const.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.834060 yz-core2-1.0.54/yzcore/extensions/storage/minio/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     9614 2023-06-13 08:31:45.000000 yz-core2-1.0.54/yzcore/extensions/storage/minio/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.835246 yz-core2-1.0.54/yzcore/extensions/storage/obs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8886 2023-05-06 03:12:37.000000 yz-core2-1.0.54/yzcore/extensions/storage/obs/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1109 2023-04-21 02:05:49.000000 yz-core2-1.0.54/yzcore/extensions/storage/obs/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     3101 2023-05-06 02:48:14.000000 yz-core2-1.0.54/yzcore/extensions/storage/obs/obs_inherit.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      654 2023-04-25 06:07:27.000000 yz-core2-1.0.54/yzcore/extensions/storage/obs/utils.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.835956 yz-core2-1.0.54/yzcore/extensions/storage/oss/
+-rw-r--r--   0 zhouwei    (501) staff       (20)    11583 2023-06-12 07:03:40.000000 yz-core2-1.0.54/yzcore/extensions/storage/oss/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      762 2023-04-21 02:05:49.000000 yz-core2-1.0.54/yzcore/extensions/storage/oss/const.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1315 2023-06-12 03:08:35.000000 yz-core2-1.0.54/yzcore/extensions/storage/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      265 2023-04-21 02:05:49.000000 yz-core2-1.0.54/yzcore/extensions/storage/utils.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2724 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/extensions/uid.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.836591 yz-core2-1.0.54/yzcore/logger/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     6943 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/logger/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10770 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/logger/config.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1177 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/logger/filters.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    10780 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/logger/handlers.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.836863 yz-core2-1.0.54/yzcore/request/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      133 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/request/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     8293 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/request/aio_http.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.837284 yz-core2-1.0.54/yzcore/response/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      188 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/response/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2934 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/response/response.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)    36606 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/response/response_code.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.837478 yz-core2-1.0.54/yzcore/templates/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.838272 yz-core2-1.0.54/yzcore/templates/app_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/app_template/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      945 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/app_template/controllers.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      421 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/app_template/models.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      907 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/app_template/schemas.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/app_template/tests.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1632 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/app_template/views.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.838775 yz-core2-1.0.54/yzcore/templates/project_template/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1816 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/.gitignore
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2508 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/README.md
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.839152 yz-core2-1.0.54/yzcore/templates/project_template/docs/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/docs/install_explain.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      922 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/docs/supervisor.ini
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.839393 yz-core2-1.0.54/yzcore/templates/project_template/migrations/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/migrations/README.md
+-rw-r--r--   0 zhouwei    (501) staff       (20)      453 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/requirements.txt
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.839953 yz-core2-1.0.54/yzcore/templates/project_template/src/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.840144 yz-core2-1.0.54/yzcore/templates/project_template/src/apps/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       90 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/apps/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.840891 yz-core2-1.0.54/yzcore/templates/project_template/src/conf/
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/conf/config_dev.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/conf/config_dev.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/conf/config_production.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/conf/config_production.yaml
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/conf/config_testing.ini
+-rw-r--r--   0 zhouwei    (501) staff       (20)        0 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/conf/config_testing.yaml
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.841323 yz-core2-1.0.54/yzcore/templates/project_template/src/const/
+-rw-r--r--   0 zhouwei    (501) staff       (20)      157 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/const/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      409 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/const/_job.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      418 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/const/_task.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      843 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/main.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      807 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/settings.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.841635 yz-core2-1.0.54/yzcore/templates/project_template/src/tests/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/tests/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      840 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/tests/test_xxx.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.841780 yz-core2-1.0.54/yzcore/templates/project_template/src/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)       89 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/templates/project_template/src/utils/__init__.py
+drwxr-xr-x   0 zhouwei    (501) staff       (20)        0 2023-06-13 08:36:58.843359 yz-core2-1.0.54/yzcore/utils/
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1215 2023-06-06 06:58:34.000000 yz-core2-1.0.54/yzcore/utils/__init__.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)      231 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/utils/check_path.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1293 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/utils/check_sys.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2229 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/utils/crypto.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1830 2023-05-10 06:22:06.000000 yz-core2-1.0.54/yzcore/utils/decorator.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     9061 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/utils/encoding.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     1755 2023-04-21 02:16:16.000000 yz-core2-1.0.54/yzcore/utils/nacos.py
+-rw-r--r--   0 zhouwei    (501) staff       (20)     2129 2023-05-09 10:16:49.000000 yz-core2-1.0.54/yzcore/utils/time_utils.py
```

### Comparing `yz-core2-1.0.53/LICENSE` & `yz-core2-1.0.54/LICENSE`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/PKG-INFO` & `yz-core2-1.0.54/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.53
+Version: 1.0.54
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yz-core2-1.0.53/README.md` & `yz-core2-1.0.54/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/setup.py` & `yz-core2-1.0.54/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="yz-core2",  # Replace with your own username
-    version="1.0.53",
+    version="1.0.54",
     author="zhouwe1",
     author_email="zhouwei@live.it",
     description="An ID generator for distributed microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/zhouwe1/yz-core.git",
     packages=setuptools.find_packages(),
```

### Comparing `yz-core2-1.0.53/tests/test_setting_reload.py` & `yz-core2-1.0.54/tests/test_setting_reload.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/tests/test_uid.py` & `yz-core2-1.0.54/tests/test_uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yz_core2.egg-info/PKG-INFO` & `yz-core2-1.0.54/yz_core2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yz-core2
-Version: 1.0.53
+Version: 1.0.54
 Summary: An ID generator for distributed microservices
 Home-page: https://github.com/zhouwe1/yz-core.git
 Author: zhouwe1
 Author-email: zhouwei@live.it
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yz-core2-1.0.53/yz_core2.egg-info/SOURCES.txt` & `yz-core2-1.0.54/yz_core2.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 yzcore/extensions/__init__.py
 yzcore/extensions/uid.py
 yzcore/extensions/storage/__init__.py
 yzcore/extensions/storage/base.py
 yzcore/extensions/storage/const.py
 yzcore/extensions/storage/schemas.py
 yzcore/extensions/storage/utils.py
+yzcore/extensions/storage/amazon/__init__.py
 yzcore/extensions/storage/azure/__init__.py
 yzcore/extensions/storage/minio/__init__.py
 yzcore/extensions/storage/obs/__init__.py
 yzcore/extensions/storage/obs/const.py
 yzcore/extensions/storage/obs/obs_inherit.py
 yzcore/extensions/storage/obs/utils.py
 yzcore/extensions/storage/oss/__init__.py
```

### Comparing `yz-core2-1.0.53/yzcore/core/datastructures.py` & `yz-core2-1.0.54/yzcore/core/datastructures.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/core/encoders.py` & `yz-core2-1.0.54/yzcore/core/encoders.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/core/management/__init__.py` & `yz-core2-1.0.54/yzcore/core/management/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/core/management/commands/startapp.py` & `yz-core2-1.0.54/yzcore/core/management/commands/startapp.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/core/management/commands/startproject.py` & `yz-core2-1.0.54/yzcore/core/management/commands/startproject.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/core/management/templates.py` & `yz-core2-1.0.54/yzcore/core/management/templates.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/core/storage.py` & `yz-core2-1.0.54/yzcore/core/storage.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/db/db_session.py` & `yz-core2-1.0.54/yzcore/db/db_session.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/db/pymongo_crud_base.py` & `yz-core2-1.0.54/yzcore/db/pymongo_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/db/sqlalchemy_crud_base.py` & `yz-core2-1.0.54/yzcore/db/sqlalchemy_crud_base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/decorators.py` & `yz-core2-1.0.54/yzcore/decorators.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/default_settings.py` & `yz-core2-1.0.54/yzcore/default_settings.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/exceptions.py` & `yz-core2-1.0.54/yzcore/exceptions.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/extensions/storage/__init__.py` & `yz-core2-1.0.54/yzcore/extensions/storage/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/extensions/storage/azure/__init__.py` & `yz-core2-1.0.54/yzcore/extensions/storage/azure/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/extensions/storage/base.py` & `yz-core2-1.0.54/yzcore/extensions/storage/base.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/extensions/storage/const.py` & `yz-core2-1.0.54/yzcore/extensions/storage/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/extensions/storage/minio/__init__.py` & `yz-core2-1.0.54/yzcore/extensions/storage/minio/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,19 +123,20 @@
 
     def get_sign_url(self, key, expire=0):
         expire_time = timedelta(seconds=expire or self.private_expire_time)
         url = self.minioClient.presigned_get_object(self.bucket_name, key, expires=expire_time)
         return '//' + url.split('//', 1)[-1]
 
     def post_sign_url(self, key):
+        client = self._internal_minio_client_first()
         expire_time = datetime.now() + timedelta(seconds=self.policy_expire_time)
         policy = PostPolicy(bucket_name=self.bucket_name, expiration=expire_time)
         policy.add_starts_with_condition('$key', key)
         # policy.add_content_length_range_condition(1, 1024*1024*1024)  # 限制文件大小
-        return self.minioClient.presigned_post_policy(policy)
+        return client.presigned_post_policy(policy)
 
     def put_sign_url(self, key):
         return self.minioClient.presigned_put_object(self.bucket_name, key)
 
     def iter_objects(self, prefix='', marker=None, delimiter=None, max_keys=100):
         client = self._internal_minio_client_first()
         objects = client.list_objects(self.bucket_name, prefix=prefix, recursive=True)
```

### Comparing `yz-core2-1.0.53/yzcore/extensions/storage/obs/__init__.py` & `yz-core2-1.0.54/yzcore/extensions/storage/obs/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/extensions/storage/obs/const.py` & `yz-core2-1.0.54/yzcore/extensions/storage/obs/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/extensions/storage/obs/obs_inherit.py` & `yz-core2-1.0.54/yzcore/extensions/storage/obs/obs_inherit.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/extensions/storage/obs/utils.py` & `yz-core2-1.0.54/yzcore/extensions/storage/obs/utils.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/extensions/storage/oss/__init__.py` & `yz-core2-1.0.54/yzcore/extensions/storage/oss/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import os
 import json
 import base64
 import hmac
 import datetime
 import hashlib
 from urllib import parse
-from yzcore.extensions.storage.base import StorageManagerBase, StorageRequestError, IMAGE_FORMAT_SET
+from yzcore.extensions.storage.base import StorageManagerBase, StorageRequestError
 from yzcore.extensions.storage.oss.const import *
 from yzcore.extensions.storage.schemas import OssConfig
 
 try:
     import oss2
     from oss2 import CaseInsensitiveDict
 except:
@@ -37,21 +37,21 @@
     def __init(self, bucket_name=None):
         """初始化对象"""
 
         if oss2 is None:
             raise ImportError("'oss2' must be installed to use OssManager")
 
         self.auth = oss2.Auth(self.access_key_id, self.access_key_secret)
+        self.bucket_name = bucket_name if bucket_name else self.bucket_name
 
         # 优先内网endpoint
         if self.internal_endpoint:
-            self.endpoint = self.internal_endpoint
-
-        self.bucket_name = bucket_name if bucket_name else self.bucket_name
-        self.bucket = oss2.Bucket(self.auth, self.endpoint, self.bucket_name)
+            self.bucket = oss2.Bucket(self.auth, self.internal_endpoint, self.bucket_name)
+        else:
+            self.bucket = oss2.Bucket(self.auth, self.endpoint, self.bucket_name)
 
         if self.cache_path:
             try:
                 os.makedirs(self.cache_path)
             except OSError:
                 pass
 
@@ -318,22 +318,7 @@
         meta = self.bucket.head_object(key)
         return {
             'etag': meta.etag.lower(),
             'size': meta.content_length,
             'last_modified': meta.headers['Last-Modified'],
             'content_type': meta.headers['Content-Type']
         }
-
-    @property
-    def host(self):
-        return u'//{}.{}'.format(self.bucket_name, self.endpoint.replace('-internal', ''))
-
-    def get_file_url(self, key, with_scheme=False):
-        if not any((self.image_domain, self.asset_domain)):
-            resource_url = u"//{}.{}/{}".format(self.bucket_name, self.endpoint.replace('-internal', ''), key)
-        elif key.split('.')[-1].lower() in IMAGE_FORMAT_SET:
-            resource_url = u"//{domain}/{key}".format(domain=self.image_domain, key=key)
-        else:
-            resource_url = u"//{domain}/{key}".format(domain=self.asset_domain, key=key)
-        if with_scheme:
-            resource_url = self.scheme + ':' + resource_url
-        return resource_url
```

### Comparing `yz-core2-1.0.53/yzcore/extensions/storage/oss/const.py` & `yz-core2-1.0.54/yzcore/extensions/storage/oss/const.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/extensions/storage/schemas.py` & `yz-core2-1.0.54/yzcore/extensions/storage/schemas.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,7 +42,11 @@
 
 class AzureConfig(BaseConfig):
     connection_string: str
     account_key: str
     account_name: str
     access_key_id: Optional[str] = None
     access_key_secret: Optional[str] = None
+
+
+class AmazonConfig(BaseConfig):
+    pass
```

### Comparing `yz-core2-1.0.53/yzcore/extensions/uid.py` & `yz-core2-1.0.54/yzcore/extensions/uid.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/logger/__init__.py` & `yz-core2-1.0.54/yzcore/logger/__init__.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/logger/config.py` & `yz-core2-1.0.54/yzcore/logger/config.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/logger/filters.py` & `yz-core2-1.0.54/yzcore/logger/filters.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/logger/handlers.py` & `yz-core2-1.0.54/yzcore/logger/handlers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/request/aio_http.py` & `yz-core2-1.0.54/yzcore/request/aio_http.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/response/response.py` & `yz-core2-1.0.54/yzcore/response/response.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/response/response_code.py` & `yz-core2-1.0.54/yzcore/response/response_code.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/templates/app_template/controllers.py` & `yz-core2-1.0.54/yzcore/templates/app_template/controllers.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/templates/app_template/schemas.py` & `yz-core2-1.0.54/yzcore/templates/app_template/schemas.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/templates/app_template/views.py` & `yz-core2-1.0.54/yzcore/templates/app_template/views.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/templates/project_template/.gitignore` & `yz-core2-1.0.54/yzcore/templates/project_template/.gitignore`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/templates/project_template/README.md` & `yz-core2-1.0.54/yzcore/templates/project_template/README.md`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/templates/project_template/docs/supervisor.ini` & `yz-core2-1.0.54/yzcore/templates/project_template/docs/supervisor.ini`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/templates/project_template/src/main.py` & `yz-core2-1.0.54/yzcore/templates/project_template/src/main.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/templates/project_template/src/settings.py` & `yz-core2-1.0.54/yzcore/templates/project_template/src/settings.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/templates/project_template/src/tests/test_xxx.py` & `yz-core2-1.0.54/yzcore/templates/project_template/src/tests/test_xxx.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/utils/check_sys.py` & `yz-core2-1.0.54/yzcore/utils/check_sys.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/utils/crypto.py` & `yz-core2-1.0.54/yzcore/utils/crypto.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/utils/decorator.py` & `yz-core2-1.0.54/yzcore/utils/decorator.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/utils/encoding.py` & `yz-core2-1.0.54/yzcore/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/utils/nacos.py` & `yz-core2-1.0.54/yzcore/utils/nacos.py`

 * *Files identical despite different names*

### Comparing `yz-core2-1.0.53/yzcore/utils/time_utils.py` & `yz-core2-1.0.54/yzcore/utils/time_utils.py`

 * *Files identical despite different names*

