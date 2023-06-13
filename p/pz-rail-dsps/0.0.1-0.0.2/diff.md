# Comparing `tmp/pz_rail_dsps-0.0.1.tar.gz` & `tmp/pz_rail_dsps-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pz_rail_dsps-0.0.1.tar", last modified: Tue Jun 13 16:58:27 2023, max compression
+gzip compressed data, was "pz_rail_dsps-0.0.2.tar", last modified: Tue Jun 13 18:44:32 2023, max compression
```

## Comparing `pz_rail_dsps-0.0.1.tar` & `pz_rail_dsps-0.0.2.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.094871 pz_rail_dsps-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/.copier-answers.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.090871 pz_rail_dsps-0.0.1/.github/
--rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/.github/pull_request_template.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.090871 pz_rail_dsps-0.0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/.github/workflows/add-issue-to-project-tracker.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/.github/workflows/linting.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/.github/workflows/smoke-test.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/.github/workflows/testing-and-coverage.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-13 16:58:27.094871 pz_rail_dsps-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:58:27.094871 pz_rail_dsps-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.086871 pz_rail_dsps-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.090871 pz_rail_dsps-0.0.1/src/pz_rail_dsps.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-13 16:58:27.000000 pz_rail_dsps-0.0.1/src/pz_rail_dsps.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2207 2023-06-13 16:58:27.000000 pz_rail_dsps-0.0.1/src/pz_rail_dsps.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:58:27.000000 pz_rail_dsps-0.0.1/src/pz_rail_dsps.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-13 16:58:27.000000 pz_rail_dsps-0.0.1/src/pz_rail_dsps.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 16:58:27.000000 pz_rail_dsps-0.0.1/src/pz_rail_dsps.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.086871 pz_rail_dsps-0.0.1/src/rail/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.086871 pz_rail_dsps-0.0.1/src/rail/creation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.090871 pz_rail_dsps-0.0.1/src/rail/creation/engines/
--rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/creation/engines/dsps_photometry_creator.py
--rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/creation/engines/dsps_sed_modeler.py
--rw-r--r--   0 runner    (1001) docker     (123)    10960 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/creation/engines/flowEngine.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/creation/engines/galaxy_population_components.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.090871 pz_rail_dsps-0.0.1/src/rail/dsps/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/dsps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 16:58:26.000000 pz_rail_dsps-0.0.1/src/rail/dsps/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.086871 pz_rail_dsps-0.0.1/src/rail/examples_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.086871 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.086871 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.086871 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.094871 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_g_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_r_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_g_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_i_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)    15568 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_r_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_u_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_y_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)    12896 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_z_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/mzls_z_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_b_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_g_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_i_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_r_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_v_transmission.h5
--rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_z_transmission.h5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.086871 pz_rail_dsps-0.0.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:58:27.094871 pz_rail_dsps-0.0.1/tests/dsps/
--rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-06-13 16:58:11.000000 pz_rail_dsps-0.0.1/tests/dsps/test_dsps_interface.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.030225 pz_rail_dsps-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.copier-answers.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)     3329 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.github/workflows/add-issue-to-project-tracker.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.github/workflows/linting.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.github/workflows/smoke-test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.github/workflows/testing-and-coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-13 18:44:32.030225 pz_rail_dsps-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1786 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 18:44:32.030225 pz_rail_dsps-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1818 2023-06-13 18:44:32.000000 pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2167 2023-06-13 18:44:32.000000 pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 18:44:32.000000 pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-13 18:44:32.000000 pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 18:44:32.000000 pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/rail/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/rail/creation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/rail/creation/engines/
+-rw-r--r--   0 runner    (1001) docker     (123)    10058 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/creation/engines/dsps_photometry_creator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18379 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/creation/engines/dsps_sed_modeler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/creation/engines/galaxy_population_components.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.030225 pz_rail_dsps-0.0.2/src/rail/dsps/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/dsps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-13 18:44:31.000000 pz_rail_dsps-0.0.2/src/rail/dsps/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/rail/examples_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.030225 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_g_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_r_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    16496 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_g_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    14608 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_i_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    15568 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_r_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     9136 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_u_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    17296 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_y_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)    12896 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_z_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     4072 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/mzls_z_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_b_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3568 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_g_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3792 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_i_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3560 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_r_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3536 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_v_transmission.h5
+-rw-r--r--   0 runner    (1001) docker     (123)     3528 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_z_transmission.h5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.026225 pz_rail_dsps-0.0.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 18:44:32.030225 pz_rail_dsps-0.0.2/tests/dsps/
+-rw-r--r--   0 runner    (1001) docker     (123)     8871 2023-06-13 18:44:19.000000 pz_rail_dsps-0.0.2/tests/dsps/test_dsps_interface.py
```

### Comparing `pz_rail_dsps-0.0.1/.github/pull_request_template.md` & `pz_rail_dsps-0.0.2/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/.github/workflows/linting.yml` & `pz_rail_dsps-0.0.2/.github/workflows/linting.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/.github/workflows/publish-to-pypi.yml` & `pz_rail_dsps-0.0.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/.github/workflows/smoke-test.yml` & `pz_rail_dsps-0.0.2/.github/workflows/smoke-test.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/.github/workflows/testing-and-coverage.yml` & `pz_rail_dsps-0.0.2/.github/workflows/testing-and-coverage.yml`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/.gitignore` & `pz_rail_dsps-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/.pre-commit-config.yaml` & `pz_rail_dsps-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/LICENSE` & `pz_rail_dsps-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/PKG-INFO` & `pz_rail_dsps-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz_rail_dsps
-Version: 0.0.1
+Version: 0.0.2
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_dsps-0.0.1/pyproject.toml` & `pz_rail_dsps-0.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/pz_rail_dsps.egg-info/PKG-INFO` & `pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pz-rail-dsps
-Version: 0.0.1
+Version: 0.0.2
 Author-email: "LSST Dark Energy Science Collaboration (DESC)" <later@later.com>
 License: MIT License
         
         Copyright (c) 2023 LSST Dark Energy Science Collaboration (DESC)
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
         of this software and associated documentation files (the "Software"), to deal
```

### Comparing `pz_rail_dsps-0.0.1/src/pz_rail_dsps.egg-info/SOURCES.txt` & `pz_rail_dsps-0.0.2/src/pz_rail_dsps.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,14 @@
 src/pz_rail_dsps.egg-info/PKG-INFO
 src/pz_rail_dsps.egg-info/SOURCES.txt
 src/pz_rail_dsps.egg-info/dependency_links.txt
 src/pz_rail_dsps.egg-info/requires.txt
 src/pz_rail_dsps.egg-info/top_level.txt
 src/rail/creation/engines/dsps_photometry_creator.py
 src/rail/creation/engines/dsps_sed_modeler.py
-src/rail/creation/engines/flowEngine.py
 src/rail/creation/engines/galaxy_population_components.py
 src/rail/dsps/__init__.py
 src/rail/dsps/_version.py
 src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_g_transmission.h5
 src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_r_transmission.h5
 src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_g_transmission.h5
 src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_i_transmission.h5
```

### Comparing `pz_rail_dsps-0.0.1/src/rail/creation/engines/dsps_photometry_creator.py` & `pz_rail_dsps-0.0.2/src/rail/creation/engines/dsps_photometry_creator.py`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/creation/engines/dsps_sed_modeler.py` & `pz_rail_dsps-0.0.2/src/rail/creation/engines/dsps_sed_modeler.py`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/creation/engines/galaxy_population_components.py` & `pz_rail_dsps-0.0.2/src/rail/creation/engines/galaxy_population_components.py`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_g_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_g_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_r_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/bass_r_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_g_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_g_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_i_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_i_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_r_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_r_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_u_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_u_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_y_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_y_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_z_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/lsst_z_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/mzls_z_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/mzls_z_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_b_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_b_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_g_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_g_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_i_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_i_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_r_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_r_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_v_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_v_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_z_transmission.h5` & `pz_rail_dsps-0.0.2/src/rail/examples_data/creation_data/data/dsps_default_data/filters/suprimecam_z_transmission.h5`

 * *Files identical despite different names*

### Comparing `pz_rail_dsps-0.0.1/tests/dsps/test_dsps_interface.py` & `pz_rail_dsps-0.0.2/tests/dsps/test_dsps_interface.py`

 * *Files identical despite different names*

