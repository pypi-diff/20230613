# Comparing `tmp/drms-0.6.3.tar.gz` & `tmp/drms-0.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "drms-0.6.3.tar", last modified: Thu Oct 13 21:09:03 2022, max compression
+gzip compressed data, was "drms-0.6.4.tar", last modified: Tue Jun 13 14:41:37 2023, max compression
```

## Comparing `drms-0.6.3.tar` & `drms-0.6.4.tar`

### file list

```diff
@@ -1,81 +1,88 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-13 21:09:03.394754 drms-0.6.3/
--rw-r--r--   0 vsts      (1001) docker     (121)      286 2022-10-13 21:08:43.000000 drms-0.6.3/.readthedocs.yml
--rw-r--r--   0 vsts      (1001) docker     (121)     1530 2022-10-13 21:08:43.000000 drms-0.6.3/CHANGELOG.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1505 2022-10-13 21:08:43.000000 drms-0.6.3/CITATION.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1308 2022-10-13 21:08:43.000000 drms-0.6.3/LICENSE.rst
--rw-r--r--   0 vsts      (1001) docker     (121)      580 2022-10-13 21:08:43.000000 drms-0.6.3/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     3711 2022-10-13 21:09:03.394754 drms-0.6.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     2628 2022-10-13 21:08:43.000000 drms-0.6.3/README.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     2376 2022-10-13 21:08:43.000000 drms-0.6.3/conftest.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-13 21:09:03.390754 drms-0.6.3/docs/
--rw-r--r--   0 vsts      (1001) docker     (121)     8065 2022-10-13 21:08:43.000000 drms-0.6.3/docs/Makefile
--rw-r--r--   0 vsts      (1001) docker     (121)       49 2022-10-13 21:08:43.000000 drms-0.6.3/docs/citation.rst
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-13 21:09:03.390754 drms-0.6.3/docs/code_ref/
--rw-r--r--   0 vsts      (1001) docker     (121)      226 2022-10-13 21:08:43.000000 drms-0.6.3/docs/code_ref/index.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     3975 2022-10-13 21:08:43.000000 drms-0.6.3/docs/conf.py
--rw-r--r--   0 vsts      (1001) docker     (121)      417 2022-10-13 21:08:43.000000 drms-0.6.3/docs/index.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     2169 2022-10-13 21:08:43.000000 drms-0.6.3/docs/intro.rst
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-13 21:08:43.000000 drms-0.6.3/docs/rtd_requirements.txt
--rw-r--r--   0 vsts      (1001) docker     (121)    18143 2022-10-13 21:08:43.000000 drms-0.6.3/docs/tutorial.rst
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-13 21:09:03.390754 drms-0.6.3/docs/whatsnew/
--rw-r--r--   0 vsts      (1001) docker     (121)      168 2022-10-13 21:08:43.000000 drms-0.6.3/docs/whatsnew/changelog.rst
--rw-r--r--   0 vsts      (1001) docker     (121)       92 2022-10-13 21:08:43.000000 drms-0.6.3/docs/whatsnew/index.rst
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-13 21:09:03.394754 drms-0.6.3/drms/
--rw-r--r--   0 vsts      (1001) docker     (121)     1505 2022-10-13 21:08:43.000000 drms-0.6.3/drms/CITATION.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1850 2022-10-13 21:08:43.000000 drms-0.6.3/drms/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)      176 2022-10-13 21:09:03.000000 drms-0.6.3/drms/_version.py
--rw-r--r--   0 vsts      (1001) docker     (121)    44131 2022-10-13 21:08:43.000000 drms-0.6.3/drms/client.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5023 2022-10-13 21:08:43.000000 drms-0.6.3/drms/config.py
--rw-r--r--   0 vsts      (1001) docker     (121)      457 2022-10-13 21:08:43.000000 drms-0.6.3/drms/exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (121)    14026 2022-10-13 21:08:43.000000 drms-0.6.3/drms/json.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1017 2022-10-13 21:08:43.000000 drms-0.6.3/drms/main.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-13 21:09:03.394754 drms-0.6.3/drms/tests/
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1295 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/test_client.py
--rw-r--r--   0 vsts      (1001) docker     (121)     5035 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/test_config.py
--rw-r--r--   0 vsts      (1001) docker     (121)      362 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/test_exceptions.py
--rw-r--r--   0 vsts      (1001) docker     (121)      801 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/test_init.py
--rw-r--r--   0 vsts      (1001) docker     (121)      808 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/test_jsoc_basic.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1545 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/test_jsoc_email.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4839 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/test_jsoc_export.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1311 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/test_jsoc_info.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3211 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/test_jsoc_query.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2215 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/test_kis_basic.py
--rw-r--r--   0 vsts      (1001) docker     (121)      775 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/test_main.py
--rw-r--r--   0 vsts      (1001) docker     (121)     4163 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/test_series_info.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3746 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/test_to_datetime.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1882 2022-10-13 21:08:43.000000 drms-0.6.3/drms/tests/test_utils.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2201 2022-10-13 21:08:43.000000 drms-0.6.3/drms/utils.py
--rw-r--r--   0 vsts      (1001) docker     (121)      997 2022-10-13 21:08:43.000000 drms-0.6.3/drms/version.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-13 21:09:03.394754 drms-0.6.3/drms.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     3711 2022-10-13 21:09:03.000000 drms-0.6.3/drms.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1576 2022-10-13 21:09:03.000000 drms-0.6.3/drms.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-13 21:09:03.000000 drms-0.6.3/drms.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       40 2022-10-13 21:09:03.000000 drms-0.6.3/drms.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2022-10-13 21:09:03.000000 drms-0.6.3/drms.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)      272 2022-10-13 21:09:03.000000 drms-0.6.3/drms.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        5 2022-10-13 21:09:03.000000 drms-0.6.3/drms.egg-info/top_level.txt
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-13 21:09:03.394754 drms-0.6.3/examples/
--rw-r--r--   0 vsts      (1001) docker     (121)      100 2022-10-13 21:08:43.000000 drms-0.6.3/examples/README.txt
--rw-r--r--   0 vsts      (1001) docker     (121)     2598 2022-10-13 21:08:43.000000 drms-0.6.3/examples/cutout_export_request.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1702 2022-10-13 21:08:43.000000 drms-0.6.3/examples/export_as_is.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1883 2022-10-13 21:08:43.000000 drms-0.6.3/examples/export_fits.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1280 2022-10-13 21:08:43.000000 drms-0.6.3/examples/export_from_id.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1954 2022-10-13 21:08:43.000000 drms-0.6.3/examples/export_jpg.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2066 2022-10-13 21:08:43.000000 drms-0.6.3/examples/export_movie.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1320 2022-10-13 21:08:43.000000 drms-0.6.3/examples/export_print_urls.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1985 2022-10-13 21:08:43.000000 drms-0.6.3/examples/export_tar.py
--rw-r--r--   0 vsts      (1001) docker     (121)      766 2022-10-13 21:08:43.000000 drms-0.6.3/examples/list_hmi_series.py
--rw-r--r--   0 vsts      (1001) docker     (121)      900 2022-10-13 21:08:43.000000 drms-0.6.3/examples/list_keywords.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2510 2022-10-13 21:08:43.000000 drms-0.6.3/examples/plot_aia_lightcurve.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1594 2022-10-13 21:08:43.000000 drms-0.6.3/examples/plot_hmi_lightcurve.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3080 2022-10-13 21:08:43.000000 drms-0.6.3/examples/plot_hmi_modes.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2581 2022-10-13 21:08:43.000000 drms-0.6.3/examples/plot_polarfield.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2462 2022-10-13 21:08:43.000000 drms-0.6.3/examples/plot_synoptic_mr.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2022-10-13 21:09:03.394754 drms-0.6.3/licenses/
--rw-r--r--   0 vsts      (1001) docker     (121)      240 2022-10-13 21:08:43.000000 drms-0.6.3/licenses/README.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     1069 2022-10-13 21:08:43.000000 drms-0.6.3/licenses/TOWNCRIER.rst
--rw-r--r--   0 vsts      (1001) docker     (121)     2476 2022-10-13 21:08:43.000000 drms-0.6.3/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)     3297 2022-10-13 21:09:03.398754 drms-0.6.3/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)     1050 2022-10-13 21:08:43.000000 drms-0.6.3/setup.py
--rw-r--r--   0 vsts      (1001) docker     (121)     2015 2022-10-13 21:08:43.000000 drms-0.6.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:41:37.692298 drms-0.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-06-13 14:41:19.000000 drms-0.6.4/.codecov.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-06-13 14:41:19.000000 drms-0.6.4/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-13 14:41:19.000000 drms-0.6.4/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:41:37.684298 drms-0.6.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:41:37.688298 drms-0.6.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2232 2023-06-13 14:41:19.000000 drms-0.6.4/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3278 2023-06-13 14:41:19.000000 drms-0.6.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-06-13 14:41:19.000000 drms-0.6.4/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-13 14:41:19.000000 drms-0.6.4/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-06-13 14:41:19.000000 drms-0.6.4/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-13 14:41:19.000000 drms-0.6.4/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1308 2023-06-13 14:41:19.000000 drms-0.6.4/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-06-13 14:41:19.000000 drms-0.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-13 14:41:37.696298 drms-0.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2628 2023-06-13 14:41:19.000000 drms-0.6.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:41:37.688298 drms-0.6.4/changelog/
+-rw-r--r--   0 runner    (1001) docker     (123)     1996 2023-06-13 14:41:19.000000 drms-0.6.4/changelog/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:41:37.688298 drms-0.6.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     8065 2023-06-13 14:41:19.000000 drms-0.6.4/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 14:41:19.000000 drms-0.6.4/docs/citation.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:41:37.688298 drms-0.6.4/docs/code_ref/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-13 14:41:19.000000 drms-0.6.4/docs/code_ref/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3975 2023-06-13 14:41:19.000000 drms-0.6.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      417 2023-06-13 14:41:19.000000 drms-0.6.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2169 2023-06-13 14:41:19.000000 drms-0.6.4/docs/intro.rst
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:41:19.000000 drms-0.6.4/docs/rtd_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    18168 2023-06-13 14:41:19.000000 drms-0.6.4/docs/tutorial.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:41:37.688298 drms-0.6.4/docs/whatsnew/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-13 14:41:19.000000 drms-0.6.4/docs/whatsnew/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-13 14:41:19.000000 drms-0.6.4/docs/whatsnew/index.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:41:37.688298 drms-0.6.4/drms/
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-06-13 14:41:19.000000 drms-0.6.4/drms/CITATION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-06-13 14:41:19.000000 drms-0.6.4/drms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 14:41:37.000000 drms-0.6.4/drms/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44149 2023-06-13 14:41:19.000000 drms-0.6.4/drms/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5023 2023-06-13 14:41:19.000000 drms-0.6.4/drms/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 14:41:19.000000 drms-0.6.4/drms/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14026 2023-06-13 14:41:19.000000 drms-0.6.4/drms/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1017 2023-06-13 14:41:19.000000 drms-0.6.4/drms/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:41:37.692298 drms-0.6.4/drms/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      801 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/test_jsoc_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/test_jsoc_email.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4719 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/test_jsoc_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1311 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/test_jsoc_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/test_jsoc_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2215 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/test_kis_basic.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/test_series_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3746 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/test_to_datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-06-13 14:41:19.000000 drms-0.6.4/drms/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2536 2023-06-13 14:41:19.000000 drms-0.6.4/drms/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-06-13 14:41:19.000000 drms-0.6.4/drms/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:41:37.692298 drms-0.6.4/drms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-13 14:41:37.000000 drms-0.6.4/drms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-06-13 14:41:37.000000 drms-0.6.4/drms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:41:37.000000 drms-0.6.4/drms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-06-13 14:41:37.000000 drms-0.6.4/drms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 14:41:37.000000 drms-0.6.4/drms.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-06-13 14:41:37.000000 drms-0.6.4/drms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 14:41:37.000000 drms-0.6.4/drms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 14:41:37.692298 drms-0.6.4/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-13 14:41:19.000000 drms-0.6.4/examples/README.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2598 2023-06-13 14:41:19.000000 drms-0.6.4/examples/cutout_export_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-06-13 14:41:19.000000 drms-0.6.4/examples/export_as_is.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-06-13 14:41:19.000000 drms-0.6.4/examples/export_fits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1954 2023-06-13 14:41:19.000000 drms-0.6.4/examples/export_jpg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-06-13 14:41:19.000000 drms-0.6.4/examples/export_movie.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-13 14:41:19.000000 drms-0.6.4/examples/export_print_urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-06-13 14:41:19.000000 drms-0.6.4/examples/export_tar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-13 14:41:19.000000 drms-0.6.4/examples/list_hmi_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-06-13 14:41:19.000000 drms-0.6.4/examples/list_keywords.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2510 2023-06-13 14:41:19.000000 drms-0.6.4/examples/plot_aia_lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-13 14:41:19.000000 drms-0.6.4/examples/plot_hmi_lightcurve.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-06-13 14:41:19.000000 drms-0.6.4/examples/plot_hmi_modes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-06-13 14:41:19.000000 drms-0.6.4/examples/plot_polarfield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2462 2023-06-13 14:41:19.000000 drms-0.6.4/examples/plot_synoptic_mr.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1280 2023-06-13 14:41:19.000000 drms-0.6.4/examples/skip_export_from_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-06-13 14:41:19.000000 drms-0.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     3367 2023-06-13 14:41:37.696298 drms-0.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1050 2023-06-13 14:41:19.000000 drms-0.6.4/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-06-13 14:41:19.000000 drms-0.6.4/tox.ini
```

### Comparing `drms-0.6.3/CHANGELOG.rst` & `drms-0.6.4/CHANGELOG.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+0.6.4 (2023-06-09)
+==================
+
+Bug Fixes
+---------
+
+- Modified :meth:`drms.client.Client._convert_numeric_keywords` to use a row-centric approach for handling hexadecimal strings. (`#102 <https://github.com/sunpy/drms/pull/102>`__)
+- Modified :meth:`drms.utils.to_datetime` to work with Pandas 2.0. (`#103 <https://github.com/sunpy/drms/pull/102>`__)
+- Fixed pandas 2.0.0 warning.  (`#97 <https://github.com/sunpy/drms/pull/97>`__)
+
+
 0.6.3 (2022-10-13)
 ==================
 
 Bug Fixes
 ---------
 
 - Updated indexing in a function to prevent FutureWarnings from pandas. (`#73 <https://github.com/sunpy/drms/pull/73>`__)
```

### Comparing `drms-0.6.3/CITATION.rst` & `drms-0.6.4/CITATION.rst`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/LICENSE.rst` & `drms-0.6.4/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/PKG-INFO` & `drms-0.6.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drms
-Version: 0.6.3
+Version: 0.6.4
 Summary: Access HMI, AIA and MDI data with Python from the Standford JSOC DRMS
 Home-page: https://sunpy.org
 Author: The SunPy Community
 Author-email: sunpy@googlegroups.com
 License: BSD 2-Clause
 Keywords: solar physics,solar,science,data
 Platform: any
@@ -14,14 +14,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides: drms
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 Provides-Extra: docs
```

### Comparing `drms-0.6.3/README.rst` & `drms-0.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/conftest.py` & `drms-0.6.4/drms/tests/conftest.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 from urllib.error import URLError, HTTPError
 from urllib.request import urlopen
 
 import pytest
 
-import drms
-
 # Test URLs, used to check if a online site is reachable
 jsoc_testurl = "http://jsoc.stanford.edu/"
 kis_testurl = "http://drms.leibniz-kis.de/"
 
 
 def pytest_addoption(parser):
-    parser.addoption("--email", help="Export email address")
+    parser.addoption("--email", action="store", help="Export email address")
 
 
 class lazily_cached:
     """
     Lazily evaluted function call with cached result.
     """
 
@@ -51,44 +49,47 @@
             pytest.skip("JSOC is not reachable")
 
     # Skip KIS online site tests if the site is not reachable.
     if item.get_closest_marker("kis") is not None:
         if not kis_reachable():
             pytest.skip("KIS is not reachable")
 
-    # Skip export tests if no email address was specified.
-    if item.get_closest_marker("export") is not None:
-        email = item.config.getoption("email")
-        if email is None:
-            pytest.skip("No email address specified; use the --email option to enable export tests")
-
 
 @pytest.fixture
 def email(request):
     """
     Email address from --email command line option.
     """
-    return request.config.getoption("--email")
+    email = request.config.getoption("--email", None, skip=True)
+    if email is None:
+        pytest.skip("No email address specified; use the --email option to enable export tests")
+    return email
 
 
 @pytest.fixture
 def jsoc_client():
     """
     Client fixture for JSOC online tests, does not use email.
     """
+    import drms
+
     return drms.Client("jsoc")
 
 
 @pytest.fixture
 def jsoc_client_export(email):
     """
     Client fixture for JSOC online tests, uses email if specified.
     """
+    import drms
+
     return drms.Client("jsoc", email=email)
 
 
 @pytest.fixture
 def kis_client():
     """
     Client fixture for KIS online tests.
     """
+    import drms
+
     return drms.Client("kis")
```

### Comparing `drms-0.6.3/docs/Makefile` & `drms-0.6.4/docs/Makefile`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/docs/conf.py` & `drms-0.6.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/docs/intro.rst` & `drms-0.6.4/docs/intro.rst`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/docs/tutorial.rst` & `drms-0.6.4/docs/tutorial.rst`

 * *Files 0% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
 .. warning::
     Please replace the email below with your own registered email.
 
 .. code-block:: python
 
     >>> import os
-    >>> email_address = os.environ["JSOC_EMAIL"]
+    >>> email_address = os.environ["JSOC_EMAIL"]  # doctest: +REMOTE_DATA
 
 First, we start again with importing the ``drms`` library and creating a `~drms.client.Client` instance:
 
 .. code-block:: python
 
     >>> import drms
     >>> client = drms.Client(email=email_address, verbose=True)  # doctest: +REMOTE_DATA
```

### Comparing `drms-0.6.3/drms/CITATION.rst` & `drms-0.6.4/drms/CITATION.rst`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/__init__.py` & `drms-0.6.4/drms/__init__.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/client.py` & `drms-0.6.4/drms/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -647,15 +647,15 @@
             # we need a special treatment for integer strings that start
             # with '0x', like QUALITY. The following to_numeric call is
             # still necessary as the results are still Python objects.
             if k in int_keys and kdf[k].dtype is np.dtype(object):
                 idx = kdf[k].str.startswith("0x")
                 if idx.any():
                     k_idx = kdf.columns.get_loc(k)
-                    kdf[kdf.columns[k_idx]] = kdf[kdf.columns[k_idx]].apply(int, base=16)
+                    kdf.loc[idx, kdf.columns[k_idx]] = kdf.loc[idx, kdf.columns[k_idx]].apply(int, base=16)
             if k in num_keys:
                 kdf[k] = _pd_to_numeric_coerce(kdf[k])
 
     @staticmethod
     def _raise_query_error(d, status=None):
         """
         Raises a DrmsQueryError, using the json error message from d.
```

### Comparing `drms-0.6.3/drms/config.py` & `drms-0.6.4/drms/config.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/json.py` & `drms-0.6.4/drms/json.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/main.py` & `drms-0.6.4/drms/main.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/tests/test_client.py` & `drms-0.6.4/drms/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/tests/test_config.py` & `drms-0.6.4/drms/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/tests/test_init.py` & `drms-0.6.4/drms/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/tests/test_jsoc_basic.py` & `drms-0.6.4/drms/tests/test_jsoc_basic.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/tests/test_jsoc_email.py` & `drms-0.6.4/drms/tests/test_jsoc_email.py`

 * *Files 7% similar despite different names*

```diff
@@ -34,32 +34,29 @@
 @pytest.mark.parametrize("email", invalid_emails)
 def test_email_invalid_init(email):
     with pytest.raises(ValueError):
         drms.Client("jsoc", email=email)
 
 
 @pytest.mark.jsoc
-@pytest.mark.export
 @pytest.mark.remote_data
 def test_email_cmdopt_check(email):
     c = drms.Client("jsoc")
     assert c.check_email(email)
 
 
 @pytest.mark.jsoc
-@pytest.mark.export
 @pytest.mark.remote_data
 def test_email_cmdopt_set(email):
     c = drms.Client("jsoc")
     c.email = email
     assert c.email == email
 
 
 @pytest.mark.jsoc
-@pytest.mark.export
 @pytest.mark.remote_data
 def test_email_cmdopt_init(email):
     c = drms.Client("jsoc", email=email)
     assert c.email == email
 
 
 def test_query_invalid():
```

### Comparing `drms-0.6.3/drms/tests/test_jsoc_export.py` & `drms-0.6.4/drms/tests/test_jsoc_export.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import pytest
 
 import drms
 
 
 @pytest.mark.jsoc
-@pytest.mark.export
 @pytest.mark.remote_data
 @pytest.mark.parametrize("method", ["url_quick", "url"])
 def test_export_asis_basic(jsoc_client_export, method):
     r = jsoc_client_export.export(
         "hmi.v_avg120[2150]{mean,power}",
         protocol="as-is",
         method=method,
@@ -30,15 +29,14 @@
         assert filename.endswith("mean.fits") or filename.endswith("power.fits")
 
     for url in r.urls.url:
         assert url.endswith("mean.fits") or url.endswith("power.fits")
 
 
 @pytest.mark.jsoc
-@pytest.mark.export
 @pytest.mark.remote_data
 def test_export_fits_basic(jsoc_client_export):
     r = jsoc_client_export.export(
         "hmi.sharp_720s[4864][2014.11.30_00:00_TAI]{continuum, magnetogram}",
         protocol="fits",
         method="url",
         requestor=False,
@@ -59,15 +57,14 @@
         assert filename.endswith("continuum.fits") or filename.endswith("magnetogram.fits")
 
     for url in r.urls.url:
         assert url.endswith("continuum.fits") or url.endswith("magnetogram.fits")
 
 
 @pytest.mark.jsoc
-@pytest.mark.export
 @pytest.mark.remote_data
 def test_export_im_patch(jsoc_client_export):
     # TODO: check that this has actually done the export/processing properly?
     # NOTE: processing exports seem to fail silently on the server side if
     # the correct names/arguments are not passed. Not clear how to check
     # that this has not happened.
     process = {
@@ -105,15 +102,14 @@
         assert filename.endswith("image.fits")
 
     for url in req.urls.url:
         assert url.endswith("image.fits")
 
 
 @pytest.mark.jsoc
-@pytest.mark.export
 @pytest.mark.remote_data
 def test_export_rebin(jsoc_client_export):
     # TODO: check that this has actually done the export/processing properly?
     # NOTE: processing exports seem to fail silently on the server side if
     # the correct names/arguments are not passed. Not clear how to check
     # that this has not happened.
     req = jsoc_client_export.export(
@@ -137,22 +133,20 @@
         assert filename.endswith("magnetogram.fits")
 
     for url in req.urls.url:
         assert url.endswith("magnetogram.fits")
 
 
 @pytest.mark.jsoc
-@pytest.mark.export
 @pytest.mark.remote_data
 def test_export_invalid_process(jsoc_client_export):
     with pytest.raises(ValueError, match="foobar is not one of the allowed processing options"):
         jsoc_client_export.export(
             "aia.lev1_euv_12s[2015-10-17T04:33:30.000/1m@12s][171]{image}", process={"foobar": {}}
         )
 
 
 @pytest.mark.jsoc
-@pytest.mark.export
 @pytest.mark.remote_data
 def test_export_email(jsoc_client):
     with pytest.raises(ValueError):
         jsoc_client.export("hmi.v_45s[2016.04.01_TAI/1d@6h]{Dopplergram}")
```

### Comparing `drms-0.6.3/drms/tests/test_jsoc_info.py` & `drms-0.6.4/drms/tests/test_jsoc_info.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/tests/test_jsoc_query.py` & `drms-0.6.4/drms/tests/test_jsoc_query.py`

 * *Files 3% similar despite different names*

```diff
@@ -91,11 +91,14 @@
 @pytest.mark.remote_data
 def test_query_invalid_series(jsoc_client):
     with pytest.raises(DrmsQueryError):
         keys = jsoc_client.query("foo", key="T_REC")
 
 
 @pytest.mark.remote_data
-def test_query_hexadecimal_strings():
+@pytest.mark.parametrize(
+    "query", ["hmi.v_45s[2014.01.01_00:00:35_TAI-2014.01.01_01:00:35_TAI]", "hmi.M_720s[2011.04.14_00:30:00_TAI/6h@2h]"]
+)
+def test_query_hexadecimal_strings(query):
     # Exercise the part of client.py that deals with hexadecimal strings
     c = drms.Client()
-    c.query("hmi.v_45s[2014.01.01_00:00:35_TAI-2014.01.01_01:00:35_TAI]", key="**ALL**")
+    c.query(query, key="**ALL**")
```

### Comparing `drms-0.6.3/drms/tests/test_kis_basic.py` & `drms-0.6.4/drms/tests/test_kis_basic.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/tests/test_main.py` & `drms-0.6.4/drms/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/tests/test_series_info.py` & `drms-0.6.4/drms/tests/test_series_info.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/tests/test_to_datetime.py` & `drms-0.6.4/drms/tests/test_to_datetime.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/tests/test_utils.py` & `drms-0.6.4/drms/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms/utils.py` & `drms-0.6.4/drms/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 import re
 
 import numpy as np
 import pandas as pd
+from packaging.version import Version
 
 __all__ = ["to_datetime"]
 
+PD_VERSION = Version(pd.__version__)
+
 
 def _pd_to_datetime_coerce(arg):
+    if PD_VERSION >= Version("2.0.0"):
+        return pd.to_datetime(arg, errors="coerce", format="mixed", dayfirst=False)
     return pd.to_datetime(arg, errors="coerce")
 
 
 def _pd_to_numeric_coerce(arg):
     return pd.to_numeric(arg, errors="coerce")
 
 
@@ -60,15 +65,19 @@
         Set to True to omit the endswith('_TAI') check.
 
     Returns
     -------
     result : pandas.Series or pandas.Timestamp
         Pandas series or a single Timestamp object.
     """
-    s = pd.Series(tstr, dtype=object).astype(str)
-    if force or s.str.endswith("_TAI").any():
-        s = s.str.replace("_TAI", "")
-        s = s.str.replace("_", " ")
-        s = s.str.replace(".", "-", regex=True, n=2)
-    res = _pd_to_datetime_coerce(s)
+    date = pd.Series(tstr, dtype=object).astype(str)
+    if force or date.str.endswith("_TAI").any():
+        date = date.str.replace("_TAI", "")
+        date = date.str.replace("_", " ")
+        if PD_VERSION >= Version("2.0.0"):
+            regex = False
+        else:
+            regex = True
+        date = date.str.replace(".", "-", regex=regex, n=2)
+    res = _pd_to_datetime_coerce(date)
     res = res.dt.tz_localize(None)
     return res.iloc[0] if (len(res) == 1) and np.isscalar(tstr) else res
```

### Comparing `drms-0.6.3/drms/version.py` & `drms-0.6.4/drms/version.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/drms.egg-info/PKG-INFO` & `drms-0.6.4/drms.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: drms
-Version: 0.6.3
+Version: 0.6.4
 Summary: Access HMI, AIA and MDI data with Python from the Standford JSOC DRMS
 Home-page: https://sunpy.org
 Author: The SunPy Community
 Author-email: sunpy@googlegroups.com
 License: BSD 2-Clause
 Keywords: solar physics,solar,science,data
 Platform: any
@@ -14,14 +14,15 @@
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
 Provides: drms
 Requires-Python: >=3.8
 Description-Content-Type: text/x-rst
 Provides-Extra: tests
 Provides-Extra: docs
```

### Comparing `drms-0.6.3/drms.egg-info/SOURCES.txt` & `drms-0.6.4/drms.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,24 @@
+.codecov.yaml
+.editorconfig
+.gitattributes
+.gitignore
+.pre-commit-config.yaml
 .readthedocs.yml
 CHANGELOG.rst
 CITATION.rst
 LICENSE.rst
 MANIFEST.in
 README.rst
-conftest.py
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
+.github/workflows/ci.yml
+changelog/README.rst
 docs/Makefile
 docs/citation.rst
 docs/conf.py
 docs/index.rst
 docs/intro.rst
 docs/rtd_requirements.txt
 docs/tutorial.rst
@@ -33,14 +39,15 @@
 drms.egg-info/SOURCES.txt
 drms.egg-info/dependency_links.txt
 drms.egg-info/entry_points.txt
 drms.egg-info/not-zip-safe
 drms.egg-info/requires.txt
 drms.egg-info/top_level.txt
 drms/tests/__init__.py
+drms/tests/conftest.py
 drms/tests/test_client.py
 drms/tests/test_config.py
 drms/tests/test_exceptions.py
 drms/tests/test_init.py
 drms/tests/test_jsoc_basic.py
 drms/tests/test_jsoc_email.py
 drms/tests/test_jsoc_export.py
@@ -51,21 +58,19 @@
 drms/tests/test_series_info.py
 drms/tests/test_to_datetime.py
 drms/tests/test_utils.py
 examples/README.txt
 examples/cutout_export_request.py
 examples/export_as_is.py
 examples/export_fits.py
-examples/export_from_id.py
 examples/export_jpg.py
 examples/export_movie.py
 examples/export_print_urls.py
 examples/export_tar.py
 examples/list_hmi_series.py
 examples/list_keywords.py
 examples/plot_aia_lightcurve.py
 examples/plot_hmi_lightcurve.py
 examples/plot_hmi_modes.py
 examples/plot_polarfield.py
 examples/plot_synoptic_mr.py
-licenses/README.rst
-licenses/TOWNCRIER.rst
+examples/skip_export_from_id.py
```

### Comparing `drms-0.6.3/examples/cutout_export_request.py` & `drms-0.6.4/examples/cutout_export_request.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/examples/export_as_is.py` & `drms-0.6.4/examples/export_as_is.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/examples/export_fits.py` & `drms-0.6.4/examples/export_fits.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/examples/export_from_id.py` & `drms-0.6.4/examples/skip_export_from_id.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/examples/export_jpg.py` & `drms-0.6.4/examples/export_jpg.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/examples/export_movie.py` & `drms-0.6.4/examples/export_movie.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/examples/export_print_urls.py` & `drms-0.6.4/examples/export_print_urls.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/examples/export_tar.py` & `drms-0.6.4/examples/export_tar.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/examples/list_hmi_series.py` & `drms-0.6.4/examples/list_hmi_series.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/examples/list_keywords.py` & `drms-0.6.4/examples/list_keywords.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/examples/plot_aia_lightcurve.py` & `drms-0.6.4/examples/plot_aia_lightcurve.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/examples/plot_hmi_lightcurve.py` & `drms-0.6.4/examples/plot_hmi_lightcurve.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/examples/plot_hmi_modes.py` & `drms-0.6.4/examples/plot_hmi_modes.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/examples/plot_polarfield.py` & `drms-0.6.4/examples/plot_polarfield.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/examples/plot_synoptic_mr.py` & `drms-0.6.4/examples/plot_synoptic_mr.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/pyproject.toml` & `drms-0.6.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/setup.cfg` & `drms-0.6.4/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -20,14 +20,15 @@
 	Natural Language :: English
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 	Topic :: Scientific/Engineering :: Astronomy
 	Topic :: Scientific/Engineering :: Physics
 
 [options]
 zip_safe = False
 python_requires = >=3.8
 packages = find:
@@ -46,14 +47,15 @@
 	astropy
 	matplotlib
 	sphinx
 	sphinx-automodapi
 	sphinx-gallery
 	sphinx-changelog
 	sunpy-sphinx-theme
+	towncrier<22.12.0
 
 [options.packages.find]
 exclude = drms._dev
 
 [options.entry_points]
 console_scripts = 
 	drms = drms.main:main
@@ -64,22 +66,21 @@
 doctest_plus = enabled
 doctest_optionflags = NORMALIZE_WHITESPACE FLOAT_CMP ELLIPSIS
 addopts = --doctest-rst -p no:unraisableexception -p no:threadexception
 markers = 
 	remote_data: marks this test function as needing remote data.
 	jsoc: marks the test function as needing a connection to JSOC.
 	kis: marks the test function as needing a connection to KIS.
-	export: marks the test function as needing a JSOC registered email address.
 remote_data_strict = True
-junit_family = xunit2
 filterwarnings = 
 	error
 	always::pytest.PytestConfigWarning
 	ignore:numpy.ufunc size changed:RuntimeWarning
 	ignore:numpy.ndarray size changed:RuntimeWarning
+	ignore:The --rsyncdir command line argument and rsyncdirs config variable are deprecated.:DeprecationWarning
 
 [pycodestyle]
 max_line_length = 110
 
 [flake8]
 max-line-length = 110
 exclude =
```

### Comparing `drms-0.6.3/setup.py` & `drms-0.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `drms-0.6.3/tox.ini` & `drms-0.6.4/tox.ini`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,20 @@
 [tox]
 envlist =
-    py{38,39,310}{,-online,-sunpy}
+    py{38,39,310,311}{,-online,-sunpy,-oldestdeps}
     build_docs
     codestyle
 isolated_build = true
 requires =
     setuptools >=56, !=61.0.0
     pip >= 19.3.1
     tox-pypi-filter >= 0.12
 
 [testenv]
 pypi_filter = https://raw.githubusercontent.com/sunpy/sunpy/main/.test_package_pins.txt
-# Run the tests in a temporary directory to make sure that we don't import
-# drms from the source tree
-changedir = .tmp/{envname}
 description =
     run tests
     online: that require remote data
     sunpy: run the sunpy jsoc tests to ensure we dont break them
 setenv =
     MPLBACKEND = agg
     COLUMNS = 180
@@ -26,15 +23,18 @@
     JSOC_EMAIL = jsoc@sunpy.org
 passenv =
     HTTP_PROXY
     HTTPS_PROXY
     NO_PROXY
     CIRCLECI
 deps =
+    pytest-xdist
     pytest-timeout
+    # Oldest deps we pin against
+    oldestdeps: pandas<2.0
     # These are specific extras we use to run the sunpy tests.
     sunpy: git+https://github.com/sunpy/sunpy
     sunpy: beautifulsoup4
     sunpy: pytest-mock
     sunpy: python-dateutil
     sunpy: scipy
     sunpy: tqdm
```

