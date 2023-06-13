# Comparing `tmp/h-vialib-1.2.0.tar.gz` & `tmp/h-vialib-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h-vialib-1.2.0.tar", last modified: Wed May 31 11:27:28 2023, max compression
+gzip compressed data, was "h-vialib-1.2.1.tar", last modified: Tue Jun 13 11:53:11 2023, max compression
```

## Comparing `h-vialib-1.2.0.tar` & `h-vialib-1.2.1.tar`

### file list

```diff
@@ -1,68 +1,68 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.757838 h-vialib-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.749838 h-vialib-1.2.0/.cookiecutter/
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.cookiecutter/cookiecutter.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.749838 h-vialib-1.2.0/.cookiecutter/includes/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.749838 h-vialib-1.2.0/.cookiecutter/includes/README/
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.cookiecutter/includes/README/head.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.749838 h-vialib-1.2.0/.cookiecutter/includes/setuptools/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.cookiecutter/includes/setuptools/install_requires
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.749838 h-vialib-1.2.0/.cookiecutter/includes/tox/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.cookiecutter/includes/tox/deps
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.749838 h-vialib-1.2.0/.github/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-31 11:27:20.000000 h-vialib-1.2.0/.python-version
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-31 11:27:20.000000 h-vialib-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2237 2023-05-31 11:27:20.000000 h-vialib-1.2.0/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-31 11:27:28.757838 h-vialib-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-05-31 11:27:20.000000 h-vialib-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-05-31 11:27:20.000000 h-vialib-1.2.0/bin/make_python
--rwxr-xr-x   0 runner    (1001) docker     (123)     1367 2023-05-31 11:27:20.000000 h-vialib-1.2.0/bin/make_template
--rw-r--r--   0 runner    (1001) docker     (123)     4295 2023-05-31 11:27:20.000000 h-vialib-1.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-31 11:27:28.757838 h-vialib-1.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.749838 h-vialib-1.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/src/h_vialib/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/_flat_dict.py
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/_params.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/src/h_vialib/secure/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/secure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      720 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/secure/encryption.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/secure/expiry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/secure/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-05-31 11:27:20.000000 h-vialib-1.2.0/src/h_vialib/secure/url.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/src/h_vialib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-05-31 11:27:28.000000 h-vialib-1.2.0/src/h_vialib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-31 11:27:28.000000 h-vialib-1.2.0/src/h_vialib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-31 11:27:28.000000 h-vialib-1.2.0/src/h_vialib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-31 11:27:28.000000 h-vialib-1.2.0/src/h_vialib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-31 11:27:28.000000 h-vialib-1.2.0/src/h_vialib.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/tests/functional/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/functional/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/functional/sanity_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.753838 h-vialib-1.2.0/tests/unit/h_vialib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/_flat_dict_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/_params_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5525 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/client_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/configuration_test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:28.757838 h-vialib-1.2.0/tests/unit/h_vialib/secure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/secure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/secure/encryption_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/secure/expiry_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/secure/token_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tests/unit/h_vialib/secure/url_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-31 11:27:20.000000 h-vialib-1.2.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.653978 h-vialib-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.645978 h-vialib-1.2.1/.cookiecutter/
+-rw-r--r--   0 runner    (1001) docker     (123)      820 2023-06-13 11:53:01.000000 h-vialib-1.2.1/.cookiecutter/cookiecutter.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.645978 h-vialib-1.2.1/.cookiecutter/includes/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.649978 h-vialib-1.2.1/.cookiecutter/includes/README/
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-06-13 11:53:01.000000 h-vialib-1.2.1/.cookiecutter/includes/README/head.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.649978 h-vialib-1.2.1/.cookiecutter/includes/setuptools/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 11:53:01.000000 h-vialib-1.2.1/.cookiecutter/includes/setuptools/install_requires
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.649978 h-vialib-1.2.1/.cookiecutter/includes/tox/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-06-13 11:53:01.000000 h-vialib-1.2.1/.cookiecutter/includes/tox/deps
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.649978 h-vialib-1.2.1/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-06-13 11:53:01.000000 h-vialib-1.2.1/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.649978 h-vialib-1.2.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2258 2023-06-13 11:53:01.000000 h-vialib-1.2.1/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-13 11:53:01.000000 h-vialib-1.2.1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-06-13 11:53:01.000000 h-vialib-1.2.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 11:53:01.000000 h-vialib-1.2.1/.python-version
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-06-13 11:53:01.000000 h-vialib-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2329 2023-06-13 11:53:01.000000 h-vialib-1.2.1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-13 11:53:11.653978 h-vialib-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4307 2023-06-13 11:53:01.000000 h-vialib-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.649978 h-vialib-1.2.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      527 2023-06-13 11:53:01.000000 h-vialib-1.2.1/bin/make_python
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1367 2023-06-13 11:53:01.000000 h-vialib-1.2.1/bin/make_template
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-06-13 11:53:01.000000 h-vialib-1.2.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-06-13 11:53:11.653978 h-vialib-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.645978 h-vialib-1.2.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.649978 h-vialib-1.2.1/src/h_vialib/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-13 11:53:01.000000 h-vialib-1.2.1/src/h_vialib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-06-13 11:53:01.000000 h-vialib-1.2.1/src/h_vialib/_flat_dict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-13 11:53:01.000000 h-vialib-1.2.1/src/h_vialib/_params.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5048 2023-06-13 11:53:01.000000 h-vialib-1.2.1/src/h_vialib/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3708 2023-06-13 11:53:01.000000 h-vialib-1.2.1/src/h_vialib/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-06-13 11:53:01.000000 h-vialib-1.2.1/src/h_vialib/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.653978 h-vialib-1.2.1/src/h_vialib/secure/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-06-13 11:53:01.000000 h-vialib-1.2.1/src/h_vialib/secure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      720 2023-06-13 11:53:01.000000 h-vialib-1.2.1/src/h_vialib/secure/encryption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-06-13 11:53:01.000000 h-vialib-1.2.1/src/h_vialib/secure/expiry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-13 11:53:01.000000 h-vialib-1.2.1/src/h_vialib/secure/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5015 2023-06-13 11:53:01.000000 h-vialib-1.2.1/src/h_vialib/secure/url.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.649978 h-vialib-1.2.1/src/h_vialib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4827 2023-06-13 11:53:11.000000 h-vialib-1.2.1/src/h_vialib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-06-13 11:53:11.000000 h-vialib-1.2.1/src/h_vialib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:53:11.000000 h-vialib-1.2.1/src/h_vialib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-06-13 11:53:11.000000 h-vialib-1.2.1/src/h_vialib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 11:53:11.000000 h-vialib-1.2.1/src/h_vialib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.653978 h-vialib-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.653978 h-vialib-1.2.1/tests/functional/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/functional/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/functional/sanity_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2954 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.653978 h-vialib-1.2.1/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.653978 h-vialib-1.2.1/tests/unit/h_vialib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/unit/h_vialib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/unit/h_vialib/_flat_dict_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3180 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/unit/h_vialib/_params_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5611 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/unit/h_vialib/client_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/unit/h_vialib/configuration_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:11.653978 h-vialib-1.2.1/tests/unit/h_vialib/secure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/unit/h_vialib/secure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1541 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/unit/h_vialib/secure/encryption_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3787 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/unit/h_vialib/secure/expiry_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/unit/h_vialib/secure/token_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3303 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tests/unit/h_vialib/secure/url_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1798 2023-06-13 11:53:01.000000 h-vialib-1.2.1/tox.ini
```

### Comparing `h-vialib-1.2.0/.cookiecutter/cookiecutter.json` & `h-vialib-1.2.1/.cookiecutter/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/.github/workflows/ci.yml` & `h-vialib-1.2.1/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/LICENSE` & `h-vialib-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/Makefile` & `h-vialib-1.2.1/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -63,15 +63,15 @@
 $(call help,make template,"update from the latest cookiecutter template")
 template: python
 	@pyenv exec tox -e template -- $$(if [ -n "$${template+x}" ]; then echo "--template $$template"; fi) $$(if [ -n "$${checkout+x}" ]; then echo "--checkout $$checkout"; fi) $$(if [ -n "$${directory+x}" ]; then echo "--directory $$directory"; fi)
 
 .PHONY: clean
 $(call help,make clean,"delete temporary files etc")
 clean:
-	@rm -rf build dist .tox
+	@rm -rf build dist .tox .coverage coverage .eslintcache node_modules supervisord.log supervisord.pid yarn-error.log
 	@find . -path '*/__pycache__*' -delete
 	@find . -path '*.egg-info*' -delete
 
 .PHONY: python
 python:
 	@bin/make_python
```

### Comparing `h-vialib-1.2.0/PKG-INFO` & `h-vialib-1.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h-vialib
-Version: 1.2.0
+Version: 1.2.1
 Summary: Library functions for use with Via.
 Home-page: https://github.com/hypothesis/h-vialib
 Project-URL: Bug Tracker, https://github.com/hypothesis/h-vialib/issues
 Project-URL: Changelog, https://github.com/hypothesis/h-vialib/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: h-vialib Version: 1.2.0 Summary: Library functions
+Metadata-Version: 2.1 Name: h-vialib Version: 1.2.1 Summary: Library functions
 for use with Via. Home-page: https://github.com/hypothesis/h-vialib Project-
 URL: Bug Tracker, https://github.com/hypothesis/h-vialib/issues Project-URL:
 Changelog, https://github.com/hypothesis/h-vialib/releases Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: BSD
 License Classifier: Intended Audience :: Developers Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE [https://
 img.shields.io/github/actions/workflow/status/hypothesis/h-vialib/
```

### Comparing `h-vialib-1.2.0/README.md` & `h-vialib-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/bin/make_python` & `h-vialib-1.2.1/bin/make_python`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/bin/make_template` & `h-vialib-1.2.1/bin/make_template`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/pyproject.toml` & `h-vialib-1.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -83,14 +83,16 @@
 
 # Fail if there are *any* messages from PyLint.
 # The letters refer to PyLint's message categories, see
 # https://pylint.pycqa.org/en/latest/messages/messages_introduction.html
 fail-on = ["C", "E", "F", "I", "R", "W"]
 
 [tool.pylint.messages_control]
+ignore-paths=[
+]
 enable = [
     "bad-inline-option",
     "deprecated-pragma",
     "useless-suppression",
     "use-symbolic-message-instead",
 ]
 disable = [
```

### Comparing `h-vialib-1.2.0/setup.cfg` & `h-vialib-1.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/src/h_vialib/_flat_dict.py` & `h-vialib-1.2.1/src/h_vialib/_flat_dict.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/src/h_vialib/_params.py` & `h-vialib-1.2.1/src/h_vialib/_params.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/src/h_vialib/client.py` & `h-vialib-1.2.1/src/h_vialib/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 
 from h_vialib.secure import Encryption, ViaSecureURL
 
 
 class ContentType(str, Enum):
     PDF = "pdf"
     HTML = "html"
-    VIDEO = "video"
+    YOUTUBE = "youtube"
 
 
 class ViaDoc:
     """A doc we want to proxy with content type."""
 
     _GOOGLE_DRIVE_REGEX = re.compile(
         r"^https://drive.google.com/uc\?id=(.*)&export=download$", re.IGNORECASE
@@ -102,15 +102,15 @@
     def _url_for(self, doc, query):
         if self._service_url is None:
             raise ValueError("Cannot rewrite URLs without a service URL")
 
         # Optimisation to skip routing for documents we know the type of
         content_type_paths = {
             ContentType.PDF: "/pdf",
-            ContentType.VIDEO: "/video",
+            ContentType.YOUTUBE: "/video/youtube",
         }
         path = content_type_paths.get(doc.content_type, "/route")
 
         query["url"] = doc.url
 
         return self._service_url._replace(path=path, query=urlencode(query)).geturl()
```

### Comparing `h-vialib-1.2.0/src/h_vialib/configuration.py` & `h-vialib-1.2.1/src/h_vialib/configuration.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/src/h_vialib/secure/encryption.py` & `h-vialib-1.2.1/src/h_vialib/secure/encryption.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/src/h_vialib/secure/expiry.py` & `h-vialib-1.2.1/src/h_vialib/secure/expiry.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/src/h_vialib/secure/token.py` & `h-vialib-1.2.1/src/h_vialib/secure/token.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/src/h_vialib/secure/url.py` & `h-vialib-1.2.1/src/h_vialib/secure/url.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/src/h_vialib.egg-info/PKG-INFO` & `h-vialib-1.2.1/src/h_vialib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h-vialib
-Version: 1.2.0
+Version: 1.2.1
 Summary: Library functions for use with Via.
 Home-page: https://github.com/hypothesis/h-vialib
 Project-URL: Bug Tracker, https://github.com/hypothesis/h-vialib/issues
 Project-URL: Changelog, https://github.com/hypothesis/h-vialib/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Intended Audience :: Developers
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: h-vialib Version: 1.2.0 Summary: Library functions
+Metadata-Version: 2.1 Name: h-vialib Version: 1.2.1 Summary: Library functions
 for use with Via. Home-page: https://github.com/hypothesis/h-vialib Project-
 URL: Bug Tracker, https://github.com/hypothesis/h-vialib/issues Project-URL:
 Changelog, https://github.com/hypothesis/h-vialib/releases Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: BSD
 License Classifier: Intended Audience :: Developers Requires-Python: >=3.8
 Description-Content-Type: text/markdown License-File: LICENSE [https://
 img.shields.io/github/actions/workflow/status/hypothesis/h-vialib/
```

### Comparing `h-vialib-1.2.0/src/h_vialib.egg-info/SOURCES.txt` & `h-vialib-1.2.1/src/h_vialib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/tests/pyproject.toml` & `h-vialib-1.2.1/tests/pyproject.toml`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/tests/unit/h_vialib/_params_test.py` & `h-vialib-1.2.1/tests/unit/h_vialib/_params_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/tests/unit/h_vialib/client_test.py` & `h-vialib-1.2.1/tests/unit/h_vialib/client_test.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,20 @@
     DEFAULT_VALUES = {
         "via.client.ignoreOtherConfiguration": "1",
         "via.client.openSidebar": "1",
         "via.external_link_mode": "new-tab",
     }
 
     @pytest.mark.parametrize(
-        "content_type,path", ((None, "/route"), ("pdf", "/pdf"), ("video", "/video"))
+        "content_type,path",
+        (
+            (None, "/route"),
+            (ContentType.PDF, "/pdf"),
+            (ContentType.YOUTUBE, "/video/youtube"),
+        ),
     )
     def test_url_for(self, client, content_type, path):
         url = "http://example.com&a=1&a=2"
 
         final_url = client.url_for(url, content_type)
 
         expected_query = dict(self.DEFAULT_VALUES)
```

### Comparing `h-vialib-1.2.0/tests/unit/h_vialib/configuration_test.py` & `h-vialib-1.2.1/tests/unit/h_vialib/configuration_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/tests/unit/h_vialib/secure/encryption_test.py` & `h-vialib-1.2.1/tests/unit/h_vialib/secure/encryption_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/tests/unit/h_vialib/secure/expiry_test.py` & `h-vialib-1.2.1/tests/unit/h_vialib/secure/expiry_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/tests/unit/h_vialib/secure/token_test.py` & `h-vialib-1.2.1/tests/unit/h_vialib/secure/token_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/tests/unit/h_vialib/secure/url_test.py` & `h-vialib-1.2.1/tests/unit/h_vialib/secure/url_test.py`

 * *Files identical despite different names*

### Comparing `h-vialib-1.2.0/tox.ini` & `h-vialib-1.2.1/tox.ini`

 * *Files 13% similar despite different names*

```diff
@@ -10,19 +10,24 @@
 
 [testenv]
 skip_install =
     format,checkformatting,coverage,template: true
 setenv =
     PYTHONUNBUFFERED = 1
     OBJC_DISABLE_INITIALIZE_FORK_SAFETY = YES
+    dev: DEV = {env:DEV:true}
+    dev: SENTRY_ENVIRONMENT = {env:SENTRY_ENVIRONMENT:dev}
+    dev: NEW_RELIC_APP_NAME = {env:NEW_RELIC_APP_NAME:h-vialib}
+    dev: NEW_RELIC_ENVIRONMENT = {env:NEW_RELIC_ENVIRONMENT:dev}
 passenv =
     HOME
     PYTEST_ADDOPTS
     dev: DEBUG
     dev: SENTRY_DSN
+    dev: NEW_RELIC_LICENSE_KEY
 deps =
     dev: ipython
     format,checkformatting: black
     format,checkformatting: isort
     lint: toml
     lint: pylint
     lint: pydocstyle
```

