# Comparing `tmp/django-axes-6.0.1.tar.gz` & `tmp/django-axes-6.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-axes-6.0.1.tar", last modified: Wed May 17 17:48:01 2023, max compression
+gzip compressed data, was "django-axes-6.0.2.tar", last modified: Tue Jun 13 16:29:23 2023, max compression
```

## Comparing `django-axes-6.0.1.tar` & `django-axes-6.0.2.tar`

### file list

```diff
@@ -1,132 +1,136 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.770362 django-axes-6.0.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.762362 django-axes-6.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-17 17:47:48.000000 django-axes-6.0.1/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.762362 django-axes-6.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-05-17 17:47:48.000000 django-axes-6.0.1/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-05-17 17:47:48.000000 django-axes-6.0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-05-17 17:47:48.000000 django-axes-6.0.1/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-05-17 17:47:48.000000 django-axes-6.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-17 17:47:48.000000 django-axes-6.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-17 17:47:48.000000 django-axes-6.0.1/.prospector.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    32218 2023-05-17 17:47:48.000000 django-axes-6.0.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-17 17:47:48.000000 django-axes-6.0.1/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-17 17:47:48.000000 django-axes-6.0.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-17 17:47:48.000000 django-axes-6.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    36432 2023-05-17 17:48:01.770362 django-axes-6.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-05-17 17:47:48.000000 django-axes-6.0.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.762362 django-axes-6.0.1/axes/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     5175 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      380 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.762362 django-axes-6.0.1/axes/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/handlers/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/handlers/database.py
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/handlers/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/handlers/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/handlers/test.py
--rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.758362 django-axes-6.0.1/axes/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.758362 django-axes-6.0.1/axes/locale/ar/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.762362 django-axes-6.0.1/axes/locale/ar/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/ar/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.758362 django-axes-6.0.1/axes/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.762362 django-axes-6.0.1/axes/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.758362 django-axes-6.0.1/axes/locale/pl/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.766362 django-axes-6.0.1/axes/locale/pl/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/pl/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.758362 django-axes-6.0.1/axes/locale/ru/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.766362 django-axes-6.0.1/axes/locale/ru/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/ru/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.758362 django-axes-6.0.1/axes/locale/tr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.766362 django-axes-6.0.1/axes/locale/tr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/tr/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/locale/tr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.766362 django-axes-6.0.1/axes/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.766362 django-axes-6.0.1/axes/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/commands/axes_list_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/commands/axes_reset.py
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/commands/axes_reset_failure_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      552 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/commands/axes_reset_ip.py
--rw-r--r--   0 runner    (1001) docker     (123)      643 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/commands/axes_reset_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/management/commands/axes_reset_username.py
--rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/middleware.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.766362 django-axes-6.0.1/axes/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0002_auto_20151217_2044.py
--rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0003_auto_20160322_0929.py
--rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0004_auto_20181024_1538.py
--rw-r--r--   0 runner    (1001) docker     (123)      218 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0005_remove_accessattempt_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0006_remove_accesslog_trusted.py
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0007_alter_accessattempt_unique_together.py
--rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/0008_accessfailurelog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/signals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-05-17 17:47:48.000000 django-axes-6.0.1/axes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-05-17 17:47:48.000000 django-axes-6.0.1/codecov.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.766362 django-axes-6.0.1/django_axes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    36432 2023-05-17 17:48:01.000000 django-axes-6.0.1/django_axes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2728 2023-05-17 17:48:01.000000 django-axes-6.0.1/django_axes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:48:01.000000 django-axes-6.0.1/django_axes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-17 17:48:01.000000 django-axes-6.0.1/django_axes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-17 17:48:01.000000 django-axes-6.0.1/django_axes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-17 17:48:01.000000 django-axes-6.0.1/django_axes.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.770362 django-axes-6.0.1/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/10_changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/1_requirements.rst
--rw-r--r--   0 runner    (1001) docker     (123)    11121 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/2_installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/3_usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)    64873 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/4_configuration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/5_customization.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/6_integration.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/7_architecture.rst
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/8_reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/9_contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/conf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.770362 django-axes-6.0.1/docs/images/
--rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/images/flow.png
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-17 17:47:48.000000 django-axes-6.0.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-17 17:47:48.000000 django-axes-6.0.1/manage.py
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-17 17:47:48.000000 django-axes-6.0.1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-17 17:47:48.000000 django-axes-6.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-17 17:47:48.000000 django-axes-6.0.1/requirements-qa.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-17 17:47:48.000000 django-axes-6.0.1/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-17 17:47:48.000000 django-axes-6.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-17 17:48:01.770362 django-axes-6.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-05-17 17:47:48.000000 django-axes-6.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-17 17:48:01.770362 django-axes-6.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_admin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_attempts.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_backends.py
--rw-r--r--   0 runner    (1001) docker     (123)     3629 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_checks.py
--rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_failures.py
--rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_handlers.py
--rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)    37892 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_login.py
--rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_management.py
--rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_middleware.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/test_signals.py
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-17 17:47:48.000000 django-axes-6.0.1/tests/urls_empty.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.740020 django-axes-6.0.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.728020 django-axes-6.0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.728020 django-axes-6.0.2/.github/ISSUE_TEMPLATES/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-13 16:29:10.000000 django-axes-6.0.2/.github/ISSUE_TEMPLATES/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (123)      663 2023-06-13 16:29:10.000000 django-axes-6.0.2/.github/ISSUE_TEMPLATES/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (123)      730 2023-06-13 16:29:10.000000 django-axes-6.0.2/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 16:29:10.000000 django-axes-6.0.2/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.728020 django-axes-6.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-06-13 16:29:10.000000 django-axes-6.0.2/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-06-13 16:29:10.000000 django-axes-6.0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2086 2023-06-13 16:29:10.000000 django-axes-6.0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-06-13 16:29:10.000000 django-axes-6.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 16:29:10.000000 django-axes-6.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-13 16:29:10.000000 django-axes-6.0.2/.prospector.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    32447 2023-06-13 16:29:10.000000 django-axes-6.0.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-06-13 16:29:10.000000 django-axes-6.0.2/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-06-13 16:29:10.000000 django-axes-6.0.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-06-13 16:29:10.000000 django-axes-6.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    36661 2023-06-13 16:29:23.740020 django-axes-6.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2495 2023-06-13 16:29:10.000000 django-axes-6.0.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.732020 django-axes-6.0.2/axes/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3216 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3855 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6444 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7082 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.732020 django-axes-6.0.2/axes/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8912 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/handlers/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13006 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/handlers/database.py
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/handlers/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5150 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/handlers/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/handlers/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21297 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.724020 django-axes-6.0.2/axes/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.724020 django-axes-6.0.2/axes/locale/ar/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.732020 django-axes-6.0.2/axes/locale/ar/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2018 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2566 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/locale/ar/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.724020 django-axes-6.0.2/axes/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.732020 django-axes-6.0.2/axes/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.724020 django-axes-6.0.2/axes/locale/pl/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.732020 django-axes-6.0.2/axes/locale/pl/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/locale/pl/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.724020 django-axes-6.0.2/axes/locale/ru/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.732020 django-axes-6.0.2/axes/locale/ru/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/locale/ru/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.724020 django-axes-6.0.2/axes/locale/tr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.732020 django-axes-6.0.2/axes/locale/tr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1412 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/locale/tr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.732020 django-axes-6.0.2/axes/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/management/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.732020 django-axes-6.0.2/axes/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/management/commands/axes_list_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/management/commands/axes_reset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/management/commands/axes_reset_failure_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/management/commands/axes_reset_ip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      643 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/management/commands/axes_reset_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/management/commands/axes_reset_username.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1670 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/middleware.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.736020 django-axes-6.0.2/axes/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     2830 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1722 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/migrations/0002_auto_20151217_2044.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/migrations/0003_auto_20160322_0929.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2196 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/migrations/0004_auto_20181024_1538.py
+-rw-r--r--   0 runner    (1001) docker     (123)      218 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/migrations/0005_remove_accessattempt_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/migrations/0006_remove_accesslog_trusted.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/migrations/0007_alter_accessattempt_unique_together.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2194 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/migrations/0008_accessfailurelog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1940 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1782 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2197 2023-06-13 16:29:10.000000 django-axes-6.0.2/axes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-13 16:29:10.000000 django-axes-6.0.2/codecov.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.736020 django-axes-6.0.2/django_axes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    36661 2023-06-13 16:29:23.000000 django-axes-6.0.2/django_axes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2842 2023-06-13 16:29:23.000000 django-axes-6.0.2/django_axes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:29:23.000000 django-axes-6.0.2/django_axes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:29:23.000000 django-axes-6.0.2/django_axes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-06-13 16:29:23.000000 django-axes-6.0.2/django_axes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 16:29:23.000000 django-axes-6.0.2/django_axes.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.736020 django-axes-6.0.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-13 16:29:10.000000 django-axes-6.0.2/docs/10_changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-13 16:29:10.000000 django-axes-6.0.2/docs/1_requirements.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11123 2023-06-13 16:29:10.000000 django-axes-6.0.2/docs/2_installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-13 16:29:10.000000 django-axes-6.0.2/docs/3_usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    64873 2023-06-13 16:29:10.000000 django-axes-6.0.2/docs/4_configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7789 2023-06-13 16:29:10.000000 django-axes-6.0.2/docs/5_customization.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-13 16:29:10.000000 django-axes-6.0.2/docs/6_integration.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-06-13 16:29:10.000000 django-axes-6.0.2/docs/7_architecture.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-13 16:29:10.000000 django-axes-6.0.2/docs/8_reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-06-13 16:29:10.000000 django-axes-6.0.2/docs/9_contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7426 2023-06-13 16:29:10.000000 django-axes-6.0.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-06-13 16:29:10.000000 django-axes-6.0.2/docs/conf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.736020 django-axes-6.0.2/docs/images/
+-rw-r--r--   0 runner    (1001) docker     (123)   133029 2023-06-13 16:29:10.000000 django-axes-6.0.2/docs/images/flow.png
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-06-13 16:29:10.000000 django-axes-6.0.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-06-13 16:29:10.000000 django-axes-6.0.2/manage.py
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-06-13 16:29:10.000000 django-axes-6.0.2/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-06-13 16:29:10.000000 django-axes-6.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       78 2023-06-13 16:29:10.000000 django-axes-6.0.2/requirements-qa.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-06-13 16:29:10.000000 django-axes-6.0.2/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-06-13 16:29:10.000000 django-axes-6.0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:29:23.740020 django-axes-6.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2408 2023-06-13 16:29:10.000000 django-axes-6.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:23.740020 django-axes-6.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/test_admin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5990 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/test_attempts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/test_backends.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4255 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/test_checks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1939 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/test_failures.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22313 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/test_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39363 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4625 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37892 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/test_login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3760 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/test_management.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1848 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/test_middleware.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/test_signals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 16:29:10.000000 django-axes-6.0.2/tests/urls_empty.py
```

### Comparing `django-axes-6.0.1/.github/workflows/codeql.yml` & `django-axes-6.0.2/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/.github/workflows/release.yml` & `django-axes-6.0.2/.github/workflows/release.yml`

 * *Files 1% similar despite different names*

```diff
@@ -36,8 +36,8 @@
 
       - name: Upload packages to Jazzband
         if: github.event_name == 'push' && startsWith(github.ref, 'refs/tags')
         uses: pypa/gh-action-pypi-publish@release/v1
         with:
           user: jazzband
           password: ${{ secrets.JAZZBAND_RELEASE_KEY }}
-          repository_url: https://jazzband.co/projects/django-axes/upload
+          repository-url: https://jazzband.co/projects/django-axes/upload
```

### Comparing `django-axes-6.0.1/.github/workflows/test.yml` & `django-axes-6.0.2/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/CHANGES.rst` & `django-axes-6.0.2/CHANGES.rst`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,23 @@
 
 Changes
 =======
 
 
+6.0.2 (2023-06-13)
+------------------
+
+- Add Django system checks for validating callable import path settings.
+  [iafisher]
+- Improve documentation.
+  [hirotasoshu]
+- Improve repository issue and PR templates.
+  [hirotasoshu]
+
+
 6.0.1 (2023-05-17)
 ------------------
 
 - Fine-tune CI pipelines and RTD build requirements.
   [aleksihakli]
```

### Comparing `django-axes-6.0.1/CODE_OF_CONDUCT.md` & `django-axes-6.0.2/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/CONTRIBUTING.rst` & `django-axes-6.0.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/LICENSE` & `django-axes-6.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/PKG-INFO` & `django-axes-6.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.1
+Version: 6.0.2
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -123,14 +123,25 @@
 See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
 
 Changes
 =======
 
 
+6.0.2 (2023-06-13)
+------------------
+
+- Add Django system checks for validating callable import path settings.
+  [iafisher]
+- Improve documentation.
+  [hirotasoshu]
+- Improve repository issue and PR templates.
+  [hirotasoshu]
+
+
 6.0.1 (2023-05-17)
 ------------------
 
 - Fine-tune CI pipelines and RTD build requirements.
   [aleksihakli]
```

### Comparing `django-axes-6.0.1/README.rst` & `django-axes-6.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/admin.py` & `django-axes-6.0.2/axes/admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/apps.py` & `django-axes-6.0.2/axes/apps.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/attempts.py` & `django-axes-6.0.2/axes/attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/backends.py` & `django-axes-6.0.2/axes/backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/checks.py` & `django-axes-6.0.2/axes/checks.py`

 * *Files 19% similar despite different names*

```diff
@@ -17,28 +17,31 @@
         " Reconfigure settings.AXES_CACHE and settings.CACHES per django-axes configuration documentation."
     )
     MIDDLEWARE_INVALID = (
         "You do not have 'axes.middleware.AxesMiddleware' in your settings.MIDDLEWARE."
     )
     BACKEND_INVALID = "You do not have 'axes.backends.AxesStandaloneBackend' or a subclass in your settings.AUTHENTICATION_BACKENDS."
     SETTING_DEPRECATED = "You have a deprecated setting {deprecated_setting} configured in your project settings"
+    CALLABLE_INVALID = "{callable_setting} is not a valid callable."
 
 
 class Hints:
     CACHE_INVALID = None
     MIDDLEWARE_INVALID = None
     BACKEND_INVALID = "AxesModelBackend was renamed to AxesStandaloneBackend in django-axes version 5.0."
     SETTING_DEPRECATED = None
+    CALLABLE_INVALID = None
 
 
 class Codes:
     CACHE_INVALID = "axes.W001"
     MIDDLEWARE_INVALID = "axes.W002"
     BACKEND_INVALID = "axes.W003"
     SETTING_DEPRECATED = "axes.W004"
+    CALLABLE_INVALID = "axes.W005"
 
 
 @register(Tags.security, Tags.caches, Tags.compatibility)
 def axes_cache_check(app_configs, **kwargs):  # pylint: disable=unused-argument
     axes_handler = getattr(settings, "AXES_HANDLER", "")
 
     axes_cache_key = getattr(settings, "AXES_CACHE", "default")
@@ -149,7 +152,53 @@
                     id=Codes.SETTING_DEPRECATED,
                 )
             )
         except AttributeError:
             pass
 
     return warnings
+
+
+@register
+def axes_conf_check(app_configs, **kwargs):  # pylint: disable=unused-argument
+    warnings = []
+
+    callable_settings = [
+        "AXES_CLIENT_IP_CALLABLE",
+        "AXES_CLIENT_STR_CALLABLE",
+        "AXES_LOCKOUT_CALLABLE",
+        "AXES_USERNAME_CALLABLE",
+        "AXES_WHITELIST_CALLABLE",
+        "AXES_COOLOFF_TIME",
+        "AXES_LOCKOUT_PARAMETERS",
+    ]
+
+    for callable_setting in callable_settings:
+        value = getattr(settings, callable_setting)
+        if not is_valid_callable(value):
+            warnings.append(
+                Warning(
+                    msg=Messages.CALLABLE_INVALID.format(
+                        callable_setting=callable_setting
+                    ),
+                    hint=Hints.CALLABLE_INVALID,
+                    id=Codes.CALLABLE_INVALID,
+                )
+            )
+
+    return warnings
+
+
+def is_valid_callable(value) -> bool:
+    if value is None:
+        return True
+
+    if callable(value):
+        return True
+
+    if isinstance(value, str):
+        try:
+            import_string(value)
+        except ImportError:
+            return False
+
+    return True
```

### Comparing `django-axes-6.0.1/axes/conf.py` & `django-axes-6.0.2/axes/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/decorators.py` & `django-axes-6.0.2/axes/decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/handlers/base.py` & `django-axes-6.0.2/axes/handlers/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/handlers/cache.py` & `django-axes-6.0.2/axes/handlers/cache.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/handlers/database.py` & `django-axes-6.0.2/axes/handlers/database.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/handlers/dummy.py` & `django-axes-6.0.2/axes/handlers/dummy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/handlers/proxy.py` & `django-axes-6.0.2/axes/handlers/proxy.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/handlers/test.py` & `django-axes-6.0.2/axes/handlers/test.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/helpers.py` & `django-axes-6.0.2/axes/helpers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/locale/ar/LC_MESSAGES/django.mo` & `django-axes-6.0.2/axes/locale/ar/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/locale/ar/LC_MESSAGES/django.po` & `django-axes-6.0.2/axes/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/locale/de/LC_MESSAGES/django.mo` & `django-axes-6.0.2/axes/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/locale/de/LC_MESSAGES/django.po` & `django-axes-6.0.2/axes/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/locale/pl/LC_MESSAGES/django.mo` & `django-axes-6.0.2/axes/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/locale/pl/LC_MESSAGES/django.po` & `django-axes-6.0.2/axes/locale/pl/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/locale/ru/LC_MESSAGES/django.mo` & `django-axes-6.0.2/axes/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/locale/ru/LC_MESSAGES/django.po` & `django-axes-6.0.2/axes/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/locale/tr/LC_MESSAGES/django.mo` & `django-axes-6.0.2/axes/locale/tr/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/locale/tr/LC_MESSAGES/django.po` & `django-axes-6.0.2/axes/locale/tr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/management/commands/axes_reset_failure_logs.py` & `django-axes-6.0.2/axes/management/commands/axes_reset_failure_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/management/commands/axes_reset_ip.py` & `django-axes-6.0.2/axes/management/commands/axes_reset_ip.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/management/commands/axes_reset_logs.py` & `django-axes-6.0.2/axes/management/commands/axes_reset_logs.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/management/commands/axes_reset_username.py` & `django-axes-6.0.2/axes/management/commands/axes_reset_username.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/middleware.py` & `django-axes-6.0.2/axes/middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/migrations/0001_initial.py` & `django-axes-6.0.2/axes/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/migrations/0002_auto_20151217_2044.py` & `django-axes-6.0.2/axes/migrations/0002_auto_20151217_2044.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/migrations/0003_auto_20160322_0929.py` & `django-axes-6.0.2/axes/migrations/0003_auto_20160322_0929.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/migrations/0004_auto_20181024_1538.py` & `django-axes-6.0.2/axes/migrations/0004_auto_20181024_1538.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/migrations/0007_alter_accessattempt_unique_together.py` & `django-axes-6.0.2/axes/migrations/0007_alter_accessattempt_unique_together.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/migrations/0008_accessfailurelog.py` & `django-axes-6.0.2/axes/migrations/0008_accessfailurelog.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/models.py` & `django-axes-6.0.2/axes/models.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/signals.py` & `django-axes-6.0.2/axes/signals.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/axes/utils.py` & `django-axes-6.0.2/axes/utils.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/django_axes.egg-info/PKG-INFO` & `django-axes-6.0.2/django_axes.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-axes
-Version: 6.0.1
+Version: 6.0.2
 Summary: Keep track of failed login attempts in Django-powered sites.
 Home-page: https://github.com/jazzband/django-axes
 Author: Josh VanderLinden, Philip Neustrom, Michael Blume, Alex Clark, Camilo Nova, Aleksi Hakli
 Author-email: security@jazzband.co
 Maintainer: Jazzband
 Maintainer-email: security@jazzband.co
 License: MIT
@@ -123,14 +123,25 @@
 See `CONTRIBUTING <CONTRIBUTING.rst>`__.
 
 
 Changes
 =======
 
 
+6.0.2 (2023-06-13)
+------------------
+
+- Add Django system checks for validating callable import path settings.
+  [iafisher]
+- Improve documentation.
+  [hirotasoshu]
+- Improve repository issue and PR templates.
+  [hirotasoshu]
+
+
 6.0.1 (2023-05-17)
 ------------------
 
 - Fine-tune CI pipelines and RTD build requirements.
   [aleksihakli]
```

### Comparing `django-axes-6.0.1/django_axes.egg-info/SOURCES.txt` & `django-axes-6.0.2/django_axes.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -10,15 +10,18 @@
 manage.py
 mypy.ini
 pyproject.toml
 requirements-qa.txt
 requirements-test.txt
 requirements.txt
 setup.py
+.github/PULL_REQUEST_TEMPLATE.md
 .github/dependabot.yml
+.github/ISSUE_TEMPLATES/bug_report.md
+.github/ISSUE_TEMPLATES/feature_request.md
 .github/workflows/codeql.yml
 .github/workflows/release.yml
 .github/workflows/test.yml
 axes/__init__.py
 axes/admin.py
 axes/apps.py
 axes/attempts.py
```

### Comparing `django-axes-6.0.1/docs/1_requirements.rst` & `django-axes-6.0.2/docs/1_requirements.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/docs/2_installation.rst` & `django-axes-6.0.2/docs/2_installation.rst`

 * *Files 0% similar despite different names*

```diff
@@ -116,15 +116,15 @@
 To keep old behaviour with the new flag, configure the following:
 
 #. If you did not use any flags, use ``settings.AXES_LOCKOUT_PARAMETERS = ["ip_address"]``,
 #. If you used ``settings.AXES_ONLY_USER_FAILURES``, use ``settings.AXES_LOCKOUT_PARAMETERS = ["username"]``,
 #. If you used ``settings.AXES_LOCK_OUT_BY_USER_OR_IP``, use ``settings.AXES_LOCKOUT_PARAMETERS = ["username", "ip_address"]``, and
 #. If you used ``settings.AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP``, use ``settings.AXES_LOCKOUT_PARAMETERS = [["username", "ip_address"]]``,
 #. If you used ``settings.AXES_USE_USER_AGENT``, add ``"user_agent"`` to your list(s) of lockout parameters.
-    #. ``settings.AXES_USE_USER_AGENT`` would become ``settings.AXES_LOCKOUT_PARAMETERS = ["ip_address", "user_agent"]``
+    #. ``settings.AXES_USE_USER_AGENT`` would become ``settings.AXES_LOCKOUT_PARAMETERS = [["ip_address", "user_agent"]]``
     #. ``settings.AXES_USE_USER_AGENT`` with ``settings.AXES_ONLY_USER_FAILURES`` would become ``settings.AXES_LOCKOUT_PARAMETERS = [["username", "user_agent"]]``
     #. ``settings.AXES_USE_USER_AGENT`` with ``settings.AXES_LOCK_OUT_BY_USER_OR_IP`` would become ``settings.AXES_LOCKOUT_PARAMETERS = [["ip_address", "user_agent"], "username"]``
     #. ``settings.AXES_USE_USER_AGENT`` with ``settings.AXES_LOCK_OUT_BY_COMBINATION_USER_AND_IP`` would become ``settings.AXES_LOCKOUT_PARAMETERS = [["ip_address", "user_agent", "username"]]``
     #. Other combinations of flags were previously not considered; the flags had precedence over each other as described in the documentation but were less-than-trivial to understand in their previous form. The new form is more explicit and flexible, although it requires more in-depth configuration.
 
 The new lockout parameters define a combined list of attributes to consider when tracking failed authentication attempts.
 They can be any combination of ``username``, ``ip_address`` or ``user_agent`` in a list of strings or list of lists of strings.
```

### Comparing `django-axes-6.0.1/docs/3_usage.rst` & `django-axes-6.0.2/docs/3_usage.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/docs/4_configuration.rst` & `django-axes-6.0.2/docs/4_configuration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/docs/5_customization.rst` & `django-axes-6.0.2/docs/5_customization.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/docs/6_integration.rst` & `django-axes-6.0.2/docs/6_integration.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/docs/7_architecture.rst` & `django-axes-6.0.2/docs/7_architecture.rst`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/docs/Makefile` & `django-axes-6.0.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/docs/conf.py` & `django-axes-6.0.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/docs/images/flow.png` & `django-axes-6.0.2/docs/images/flow.png`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/pyproject.toml` & `django-axes-6.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/setup.py` & `django-axes-6.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/tests/base.py` & `django-axes-6.0.2/tests/base.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/tests/settings.py` & `django-axes-6.0.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/tests/test_admin.py` & `django-axes-6.0.2/tests/test_admin.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/tests/test_attempts.py` & `django-axes-6.0.2/tests/test_attempts.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/tests/test_backends.py` & `django-axes-6.0.2/tests/test_backends.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/tests/test_checks.py` & `django-axes-6.0.2/tests/test_checks.py`

 * *Files 14% similar despite different names*

```diff
@@ -106,7 +106,26 @@
             id=Codes.SETTING_DEPRECATED,
         )
 
     @override_settings(AXES_DISABLE_SUCCESS_ACCESS_LOG=True)
     def test_deprecated_success_access_log_flag(self):
         warnings = run_checks()
         self.assertEqual(warnings, [self.disable_success_access_log_warning])
+
+
+class ConfCheckTestCase(AxesTestCase):
+    @override_settings(AXES_USERNAME_CALLABLE="module.not_defined")
+    def test_invalid_import_path(self):
+        warnings = run_checks()
+        warning = Warning(
+            msg=Messages.CALLABLE_INVALID.format(
+                callable_setting="AXES_USERNAME_CALLABLE"
+            ),
+            hint=Hints.CALLABLE_INVALID,
+            id=Codes.CALLABLE_INVALID,
+        )
+        self.assertEqual(warnings, [warning])
+
+    @override_settings(AXES_COOLOFF_TIME=lambda: 1)
+    def test_valid_callable(self):
+        warnings = run_checks()
+        self.assertEqual(warnings, [])
```

### Comparing `django-axes-6.0.1/tests/test_decorators.py` & `django-axes-6.0.2/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/tests/test_failures.py` & `django-axes-6.0.2/tests/test_failures.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/tests/test_handlers.py` & `django-axes-6.0.2/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/tests/test_helpers.py` & `django-axes-6.0.2/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/tests/test_logging.py` & `django-axes-6.0.2/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/tests/test_login.py` & `django-axes-6.0.2/tests/test_login.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/tests/test_management.py` & `django-axes-6.0.2/tests/test_management.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/tests/test_middleware.py` & `django-axes-6.0.2/tests/test_middleware.py`

 * *Files identical despite different names*

### Comparing `django-axes-6.0.1/tests/test_models.py` & `django-axes-6.0.2/tests/test_models.py`

 * *Files identical despite different names*

