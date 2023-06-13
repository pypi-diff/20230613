# Comparing `tmp/jupyter-repo2docker-2022.2.0.tar.gz` & `tmp/jupyter-repo2docker-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-repo2docker-2022.2.0.tar", last modified: Sun Feb  6 14:20:11 2022, max compression
+gzip compressed data, was "jupyter-repo2docker-2023.6.0.tar", last modified: Tue Jun 13 07:24:10 2023, max compression
```

## Comparing `jupyter-repo2docker-2022.2.0.tar` & `jupyter-repo2docker-2023.6.0.tar`

### file list

```diff
@@ -1,81 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-06 14:20:11.580750 jupyter-repo2docker-2022.2.0/
--rw-r--r--   0 runner    (1001) docker     (116)     2335 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (116)     1528 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      196 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     5473 2022-02-06 14:20:11.580750 jupyter-repo2docker-2022.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     4452 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      181 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/ROADMAP.md
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-06 14:20:11.572750 jupyter-repo2docker-2022.2.0/jupyter_repo2docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     5473 2022-02-06 14:20:11.000000 jupyter-repo2docker-2022.2.0/jupyter_repo2docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2608 2022-02-06 14:20:11.000000 jupyter-repo2docker-2022.2.0/jupyter_repo2docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-02-06 14:20:11.000000 jupyter-repo2docker-2022.2.0/jupyter_repo2docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)      171 2022-02-06 14:20:11.000000 jupyter-repo2docker-2022.2.0/jupyter_repo2docker.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)      126 2022-02-06 14:20:11.000000 jupyter-repo2docker-2022.2.0/jupyter_repo2docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       12 2022-02-06 14:20:11.000000 jupyter-repo2docker-2022.2.0/jupyter_repo2docker.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-06 14:20:11.580750 jupyter-repo2docker-2022.2.0/repo2docker/
--rw-r--r--   0 runner    (1001) docker     (116)      123 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    12456 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)      501 2022-02-06 14:20:11.580750 jupyter-repo2docker-2022.2.0/repo2docker/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (116)    26897 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/app.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-06 14:20:11.576750 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/
--rw-r--r--   0 runner    (1001) docker     (116)      373 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3371 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/_r_base.py
--rw-r--r--   0 runner    (1001) docker     (116)    22645 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/base.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-06 14:20:11.576750 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/
--rw-r--r--   0 runner    (1001) docker     (116)    15234 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      870 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/activate-conda.sh
--rw-r--r--   0 runner    (1001) docker     (116)    16000 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.lock
--rw-r--r--   0 runner    (1001) docker     (116)     6182 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-2.7.lock
--rw-r--r--   0 runner    (1001) docker     (116)       95 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-2.7.yml
--rw-r--r--   0 runner    (1001) docker     (116)     5659 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.5.lock
--rw-r--r--   0 runner    (1001) docker     (116)      107 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.5.yml
--rw-r--r--   0 runner    (1001) docker     (116)    15980 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.6.lock
--rw-r--r--   0 runner    (1001) docker     (116)      536 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.6.yml
--rw-r--r--   0 runner    (1001) docker     (116)    16000 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.7.lock
--rw-r--r--   0 runner    (1001) docker     (116)      536 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.7.yml
--rw-r--r--   0 runner    (1001) docker     (116)    17399 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.8.lock
--rw-r--r--   0 runner    (1001) docker     (116)      536 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.8.yml
--rw-r--r--   0 runner    (1001) docker     (116)    17739 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.9.lock
--rw-r--r--   0 runner    (1001) docker     (116)      536 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.9.yml
--rw-r--r--   0 runner    (1001) docker     (116)      457 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.yml
--rwxr-xr-x   0 runner    (1001) docker     (116)     3848 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/freeze.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2605 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/install-base-env.bash
--rw-r--r--   0 runner    (1001) docker     (116)      383 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/requirements.py-3.5.pip
--rw-r--r--   0 runner    (1001) docker     (116)     1986 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/docker.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-06 14:20:11.576750 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/julia/
--rw-r--r--   0 runner    (1001) docker     (116)      102 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/julia/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      979 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/julia/install-repo-dependencies.jl
--rw-r--r--   0 runner    (1001) docker     (116)     6017 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/julia/julia_project.py
--rw-r--r--   0 runner    (1001) docker     (116)     7148 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/julia/julia_require.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-06 14:20:11.580750 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/legacy/
--rw-r--r--   0 runner    (1001) docker     (116)     1522 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/legacy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-06 14:20:11.580750 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/nix/
--rw-r--r--   0 runner    (1001) docker     (116)     3081 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/nix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      537 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/nix/install-nix.bash
--rw-r--r--   0 runner    (1001) docker     (116)     1281 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/nix/nix-shell-wrapper
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-06 14:20:11.580750 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/pipfile/
--rw-r--r--   0 runner    (1001) docker     (116)     7343 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/pipfile/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-06 14:20:11.580750 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/python/
--rw-r--r--   0 runner    (1001) docker     (116)     5871 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/python/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      374 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/python3-login
--rw-r--r--   0 runner    (1001) docker     (116)    16044 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/r.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     2733 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/repo2docker-entrypoint
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-02-06 14:20:11.580750 jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/
--rwxr-xr-x   0 runner    (1001) docker     (116)      229 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2801 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/base.py
--rw-r--r--   0 runner    (1001) docker     (116)    32536 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/dataverse.json
--rw-r--r--   0 runner    (1001) docker     (116)     5011 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/dataverse.py
--rw-r--r--   0 runner    (1001) docker     (116)     3649 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/doi.py
--rw-r--r--   0 runner    (1001) docker     (116)     3574 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/figshare.py
--rw-r--r--   0 runner    (1001) docker     (116)     3469 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/git.py
--rwxr-xr-x   0 runner    (1001) docker     (116)     4083 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/hydroshare.py
--rw-r--r--   0 runner    (1001) docker     (116)     2672 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/mercurial.py
--rw-r--r--   0 runner    (1001) docker     (116)     3877 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/swhid.py
--rw-r--r--   0 runner    (1001) docker     (116)     2713 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/zenodo.py
--rw-r--r--   0 runner    (1001) docker     (116)     4112 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/docker.py
--rw-r--r--   0 runner    (1001) docker     (116)     8669 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/engine.py
--rw-r--r--   0 runner    (1001) docker     (116)     5873 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/semver.py
--rw-r--r--   0 runner    (1001) docker     (116)    16298 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/repo2docker/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)      270 2022-02-06 14:20:11.580750 jupyter-repo2docker-2022.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     3101 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (116)    68751 2022-02-06 14:19:55.000000 jupyter-repo2docker-2022.2.0/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:24:10.261460 jupyter-repo2docker-2023.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2336 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-13 07:24:10.261460 jupyter-repo2docker-2023.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/RELEASE.md
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/ROADMAP.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:24:10.237460 jupyter-repo2docker-2023.6.0/jupyter_repo2docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5428 2023-06-13 07:24:10.000000 jupyter-repo2docker-2023.6.0/jupyter_repo2docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3197 2023-06-13 07:24:10.000000 jupyter-repo2docker-2023.6.0/jupyter_repo2docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:24:10.000000 jupyter-repo2docker-2023.6.0/jupyter_repo2docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-06-13 07:24:10.000000 jupyter-repo2docker-2023.6.0/jupyter_repo2docker.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 07:24:10.000000 jupyter-repo2docker-2023.6.0/jupyter_repo2docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 07:24:10.000000 jupyter-repo2docker-2023.6.0/jupyter_repo2docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:24:10.261460 jupyter-repo2docker-2023.6.0/repo2docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14043 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-06-13 07:24:10.261460 jupyter-repo2docker-2023.6.0/repo2docker/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    29606 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:24:10.245460 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3684 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/_r_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23409 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:24:10.253460 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/
+-rw-r--r--   0 runner    (1001) docker     (123)    17745 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      870 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/activate-conda.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     6178 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-2.7-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-2.7.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19001 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.10-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    19132 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.10-linux-aarch64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.10.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19113 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.11-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    19249 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.11-linux-aarch64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    18532 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.11.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.11.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     5659 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.5-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.5.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    16092 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.6-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.6.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18010 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.7-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    16588 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.7-linux-aarch64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.7.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18872 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.8-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    19003 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.8-linux-aarch64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.8.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    18981 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.9-linux-64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)    19112 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.9-linux-aarch64.lock
+-rw-r--r--   0 runner    (1001) docker     (123)      702 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.9.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.yml
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3971 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/freeze.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2613 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/install-base-env.bash
+-rw-r--r--   0 runner    (1001) docker     (123)     2010 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/docker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:24:10.253460 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/julia/
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/julia/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      979 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/julia/install-repo-dependencies.jl
+-rw-r--r--   0 runner    (1001) docker     (123)     7369 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/julia/julia_project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8073 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/julia/julia_require.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:24:10.253460 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/legacy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:24:10.257460 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/nix/
+-rw-r--r--   0 runner    (1001) docker     (123)     3306 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/nix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/nix/install-nix.bash
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/nix/nix-shell-wrapper
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:24:10.257460 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/pipfile/
+-rw-r--r--   0 runner    (1001) docker     (123)     7935 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/pipfile/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:24:10.257460 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/python/
+-rw-r--r--   0 runner    (1001) docker     (123)     6048 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/python/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      374 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/python3-login
+-rw-r--r--   0 runner    (1001) docker     (123)    16126 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/r.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3356 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/repo2docker-entrypoint
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:24:10.261460 jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      229 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33659 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/dataverse.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/dataverse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/doi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/figshare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/git.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4008 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/hydroshare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2618 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/mercurial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3804 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/swhid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3051 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/zenodo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4268 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/docker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9962 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5873 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/semver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17148 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/repo2docker/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-06-13 07:24:10.261460 jupyter-repo2docker-2023.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3103 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68533 2023-06-13 07:24:00.000000 jupyter-repo2docker-2023.6.0/versioneer.py
```

### Comparing `jupyter-repo2docker-2022.2.0/CONTRIBUTING.md` & `jupyter-repo2docker-2023.6.0/CONTRIBUTING.md`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,24 @@
 
 (And thank you particularly for coming to read the guidelines! :heart_eyes:)
 
 The repo2docker developer documentation is all rendered on our documentation website: [https://repo2docker.readthedocs.io](https://repo2docker.readthedocs.io).
 If you're here, you're probably looking for the [Contributing to repo2docker development](https://repo2docker.readthedocs.io/en/latest/contributing/contributing.html) page.
 
 Please make sure you've read the following sections before opening an issue/pull request:
-* [Process for making a contribution](https://repo2docker.readthedocs.io/en/latest/contributing/contributing.html#process-for-making-a-contribution).
-  * These steps talk you through choosing the right issue template (bug report or feature request) and making a change.
-* [Guidelines to getting a Pull Request merged](https://repo2docker.readthedocs.io/en/latest/contributing/contributing.html#guidelines-to-getting-a-pull-request-merged).
-  * These are tips and tricks to help make your contribution as smooth as possible for you and for the repo2docker maintenance team.
+
+- [Process for making a contribution](https://repo2docker.readthedocs.io/en/latest/contributing/contributing.html#process-for-making-a-contribution).
+  - These steps talk you through choosing the right issue template (bug report or feature request) and making a change.
+- [Guidelines to getting a Pull Request merged](https://repo2docker.readthedocs.io/en/latest/contributing/contributing.html#guidelines-to-getting-a-pull-request-merged).
+  - These are tips and tricks to help make your contribution as smooth as possible for you and for the repo2docker maintenance team.
 
 There are a few other pages to highlight:
 
-* [Our roadmap](https://repo2docker.readthedocs.io/en/latest/contributing/roadmap.html)
-  * We use the roadmap to develop a shared understanding of the project's vision and direction amongst the community of users, contributors, and maintainers.
+- [Our roadmap](https://repo2docker.readthedocs.io/en/latest/contributing/roadmap.html)
+  - We use the roadmap to develop a shared understanding of the project's vision and direction amongst the community of users, contributors, and maintainers.
     This is a great place to get a feel for what the maintainers are thinking about for the short, medium, and long term future of the project.
-* [Design of repo2docker](https://repo2docker.readthedocs.io/en/latest/design.html)
-  * This page explains some of the design principles behind repo2docker.
+- [Design of repo2docker](https://repo2docker.readthedocs.io/en/latest/design.html)
+  - This page explains some of the design principles behind repo2docker.
     Its a good place to understand _why_ the team have made the decisions that they have along the way!
-  * We absolutely encourage discussion around refactoring, updating or extending repo2docker, but please make sure that you've understood this page before opening an issue to discuss the change you'd like to propose.
-* [Common developer tasks and how-tos](https://repo2docker.readthedocs.io/en/latest/contributing/tasks.html)
-  * Some notes on running tests, buildpack dependencies, creating a release, and keeping the pip files up to date.
+  - We absolutely encourage discussion around refactoring, updating or extending repo2docker, but please make sure that you've understood this page before opening an issue to discuss the change you'd like to propose.
+- [Common developer tasks and how-tos](https://repo2docker.readthedocs.io/en/latest/contributing/tasks.html)
+  - Some notes on running tests, buildpack dependencies, creating a release, and keeping the pip files up to date.
```

### Comparing `jupyter-repo2docker-2022.2.0/LICENSE` & `jupyter-repo2docker-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-repo2docker-2022.2.0/PKG-INFO` & `jupyter-repo2docker-2023.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: jupyter-repo2docker
-Version: 2022.2.0
+Version: 2023.6.0
 Summary: Repo2docker: Turn code repositories into Jupyter enabled Docker Images
 Home-page: https://repo2docker.readthedocs.io/en/latest/
 Author: Project Jupyter Contributors
 Author-email: jupyter@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://repo2docker.readthedocs.io
 Project-URL: Funding, https://jupyter.org/about
 Project-URL: Source, https://github.com/jupyterhub/repo2docker/
 Project-URL: Tracker, https://github.com/jupyterhub/repo2docker/issues
 Keywords: reproducible science environments docker
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <a href="https://github.com/jupyterhub/repo2docker"><img src="https://raw.githubusercontent.com/jupyterhub/repo2docker/8731ecf0967cc5fde028c456f2b92be651ebbc18/docs/source/_static/images/repo2docker.png" height="48px" /> repo2docker</a>
 
-[![Build Status](https://github.com/jupyterhub/repo2docker/workflows/Continuous%20Integration/badge.svg)](https://github.com/jupyterhub/repo2docker/actions)
+[![Build Status](https://github.com/jupyterhub/repo2docker/workflows/Test/badge.svg)](https://github.com/jupyterhub/repo2docker/actions)
 [![Documentation Status](https://readthedocs.org/projects/repo2docker/badge/?version=latest)](http://repo2docker.readthedocs.io/en/latest/?badge=latest)
 [![Contribute](https://img.shields.io/badge/I_want_to_contribute!-grey?logo=jupyter)](https://repo2docker.readthedocs.io/en/latest/contributing/contributing.html)
 [![Docker Repository on Quay](https://img.shields.io/badge/quay.io-container-green "Docker Repository on Quay")](https://quay.io/repository/jupyterhub/repo2docker?tab=tags)
 
 `repo2docker` fetches a git repository and builds a container image based on
 the configuration files found in the repository.
 
@@ -52,14 +51,15 @@
 
 For more information, please visit
 [our informational page](https://sustainable-open-science-and-software.github.io/) or download our [participant information sheet](https://sustainable-open-science-and-software.github.io/assets/PIS_sustainable_software.pdf).
 
 ---
 
 ## Using repo2docker
+
 ### Prerequisites
 
 1. Docker to build & run the repositories. The [community edition](https://store.docker.com/search?type=edition&offering=community)
    is recommended.
 2. Python 3.6+.
 
 Supported on Linux and macOS. [See documentation note about Windows support.](http://repo2docker.readthedocs.io/en/latest/install.html#note-about-windows-support)
@@ -104,27 +104,23 @@
     to login with a token:
         http://0.0.0.0:36511/?token=f94f8fabb92e22f5bfab116c382b4707fc2cade56ad1ace0
 ```
 
 If you copy paste that URL into your browser you will see a Jupyter Notebook
 with the contents of the repository you had just built!
 
-For more information on how to use ``repo2docker``, see the
+For more information on how to use `repo2docker`, see the
 [usage guide](http://repo2docker.readthedocs.io/en/latest/usage.html).
 
-
 ## Repository specifications
 
 Repo2Docker looks for configuration files in the source repository to
 determine how the Docker image should be built. For a list of the configuration
-files that ``repo2docker`` can use, see the
+files that `repo2docker` can use, see the
 [complete list of configuration files](https://repo2docker.readthedocs.io/en/latest/config_files.html).
 
 The philosophy of repo2docker is inspired by
 [Heroku Build Packs](https://devcenter.heroku.com/articles/buildpacks).
 
-
 ## Docker Image
 
 Repo2Docker can be run inside a Docker container if access to the Docker Daemon is provided, for example see [BinderHub](https://github.com/jupyterhub/binderhub). Docker images are [published to quay.io](https://quay.io/repository/jupyterhub/repo2docker?tab=tags). The old [Docker Hub image](https://hub.docker.com/r/jupyter/repo2docker) is no longer supported.
-
-
```

#### html2text {}

```diff
@@ -1,70 +1,69 @@
-Metadata-Version: 2.1 Name: jupyter-repo2docker Version: 2022.2.0 Summary:
+Metadata-Version: 2.1 Name: jupyter-repo2docker Version: 2023.6.0 Summary:
 Repo2docker: Turn code repositories into Jupyter enabled Docker Images Home-
 page: https://repo2docker.readthedocs.io/en/latest/ Author: Project Jupyter
 Contributors Author-email: jupyter@googlegroups.com License: BSD Project-URL:
 Documentation, https://repo2docker.readthedocs.io Project-URL: Funding, https:/
 /jupyter.org/about Project-URL: Source, https://github.com/jupyterhub/
 repo2docker/ Project-URL: Tracker, https://github.com/jupyterhub/repo2docker/
-issues Keywords: reproducible science environments docker Platform: UNKNOWN
-Classifier: Environment :: Console Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators Classifier: Intended
-Audience :: Science/Research Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE # [https://raw.githubusercontent.com/jupyterhub/
-repo2docker/8731ecf0967cc5fde028c456f2b92be651ebbc18/docs/source/_static/
-images/repo2docker.png]_repo2docker [![Build Status](https://github.com/
-jupyterhub/repo2docker/workflows/Continuous%20Integration/badge.svg)](https://
-github.com/jupyterhub/repo2docker/actions) [![Documentation Status](https://
-readthedocs.org/projects/repo2docker/badge/?version=latest)](http://
-repo2docker.readthedocs.io/en/latest/?badge=latest) [![Contribute](https://
-img.shields.io/badge/I_want_to_contribute!-grey?logo=jupyter)](https://
-repo2docker.readthedocs.io/en/latest/contributing/contributing.html) [![Docker
-Repository on Quay](https://img.shields.io/badge/quay.io-container-green
-"Docker Repository on Quay")](https://quay.io/repository/jupyterhub/
-repo2docker?tab=tags) `repo2docker` fetches a git repository and builds a
-container image based on the configuration files found in the repository. See
-the [repo2docker documentation](http://repo2docker.readthedocs.io) for more
-information on using repo2docker. For support questions please search or post
-to https://discourse.jupyter.org/c/binder. See the [contributing guide]
-(CONTRIBUTING.md) for information on contributing to repo2docker. --- Please
-note that this repository is participating in a study into sustainability of
-open source projects. Data will be gathered about this repository for
-approximately the next 12 months, starting from 2021-06-11. Data collected will
-include number of contributors, number of PRs, time taken to close/merge these
-PRs, and issues closed. For more information, please visit [our informational
-page](https://sustainable-open-science-and-software.github.io/) or download our
-[participant information sheet](https://sustainable-open-science-and-
-software.github.io/assets/PIS_sustainable_software.pdf). --- ## Using
-repo2docker ### Prerequisites 1. Docker to build & run the repositories. The
-[community edition](https://store.docker.com/
-search?type=edition&offering=community) is recommended. 2. Python 3.6+.
-Supported on Linux and macOS. [See documentation note about Windows support.]
-(http://repo2docker.readthedocs.io/en/latest/install.html#note-about-windows-
-support) ### Installation This a quick guide to installing `repo2docker`, see
-our documentation for [a full guide](https://repo2docker.readthedocs.io/en/
-latest/install.html). To install from PyPI: ```bash pip install jupyter-
-repo2docker ``` To install from source: ```bash git clone https://github.com/
-jupyterhub/repo2docker.git cd repo2docker pip install -e . ``` ### Usage The
-core feature of repo2docker is to fetch a git repository (from GitHub or
-locally), build a container image based on the specifications found in the
-repository & optionally launch the container that you can use to explore the
-repository. **Note that Docker needs to be running on your machine for this to
-work.** Example: ```bash jupyter-repo2docker https://github.com/norvig/pytudes
-``` After building (it might take a while!), it should output in your terminal
-something like: ```bash Copy/paste this URL into your browser when you connect
-for the first time, to login with a token: http://0.0.0.0:36511/
-?token=f94f8fabb92e22f5bfab116c382b4707fc2cade56ad1ace0 ``` If you copy paste
-that URL into your browser you will see a Jupyter Notebook with the contents of
-the repository you had just built! For more information on how to use
-``repo2docker``, see the [usage guide](http://repo2docker.readthedocs.io/en/
+issues Keywords: reproducible science environments docker Classifier:
+Environment :: Console Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: System Administrators Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE # [https://raw.githubusercontent.com/jupyterhub/repo2docker/
+8731ecf0967cc5fde028c456f2b92be651ebbc18/docs/source/_static/images/
+repo2docker.png]_repo2docker [![Build Status](https://github.com/jupyterhub/
+repo2docker/workflows/Test/badge.svg)](https://github.com/jupyterhub/
+repo2docker/actions) [![Documentation Status](https://readthedocs.org/projects/
+repo2docker/badge/?version=latest)](http://repo2docker.readthedocs.io/en/
+latest/?badge=latest) [![Contribute](https://img.shields.io/badge/
+I_want_to_contribute!-grey?logo=jupyter)](https://repo2docker.readthedocs.io/
+en/latest/contributing/contributing.html) [![Docker Repository on Quay](https:/
+/img.shields.io/badge/quay.io-container-green "Docker Repository on Quay")]
+(https://quay.io/repository/jupyterhub/repo2docker?tab=tags) `repo2docker`
+fetches a git repository and builds a container image based on the
+configuration files found in the repository. See the [repo2docker
+documentation](http://repo2docker.readthedocs.io) for more information on using
+repo2docker. For support questions please search or post to https://
+discourse.jupyter.org/c/binder. See the [contributing guide](CONTRIBUTING.md)
+for information on contributing to repo2docker. --- Please note that this
+repository is participating in a study into sustainability of open source
+projects. Data will be gathered about this repository for approximately the
+next 12 months, starting from 2021-06-11. Data collected will include number of
+contributors, number of PRs, time taken to close/merge these PRs, and issues
+closed. For more information, please visit [our informational page](https://
+sustainable-open-science-and-software.github.io/) or download our [participant
+information sheet](https://sustainable-open-science-and-software.github.io/
+assets/PIS_sustainable_software.pdf). --- ## Using repo2docker ###
+Prerequisites 1. Docker to build & run the repositories. The [community
+edition](https://store.docker.com/search?type=edition&offering=community) is
+recommended. 2. Python 3.6+. Supported on Linux and macOS. [See documentation
+note about Windows support.](http://repo2docker.readthedocs.io/en/latest/
+install.html#note-about-windows-support) ### Installation This a quick guide to
+installing `repo2docker`, see our documentation for [a full guide](https://
+repo2docker.readthedocs.io/en/latest/install.html). To install from PyPI:
+```bash pip install jupyter-repo2docker ``` To install from source: ```bash git
+clone https://github.com/jupyterhub/repo2docker.git cd repo2docker pip install
+-e . ``` ### Usage The core feature of repo2docker is to fetch a git repository
+(from GitHub or locally), build a container image based on the specifications
+found in the repository & optionally launch the container that you can use to
+explore the repository. **Note that Docker needs to be running on your machine
+for this to work.** Example: ```bash jupyter-repo2docker https://github.com/
+norvig/pytudes ``` After building (it might take a while!), it should output in
+your terminal something like: ```bash Copy/paste this URL into your browser
+when you connect for the first time, to login with a token: http://0.0.0.0:
+36511/?token=f94f8fabb92e22f5bfab116c382b4707fc2cade56ad1ace0 ``` If you copy
+paste that URL into your browser you will see a Jupyter Notebook with the
+contents of the repository you had just built! For more information on how to
+use `repo2docker`, see the [usage guide](http://repo2docker.readthedocs.io/en/
 latest/usage.html). ## Repository specifications Repo2Docker looks for
 configuration files in the source repository to determine how the Docker image
-should be built. For a list of the configuration files that ``repo2docker`` can
+should be built. For a list of the configuration files that `repo2docker` can
 use, see the [complete list of configuration files](https://
 repo2docker.readthedocs.io/en/latest/config_files.html). The philosophy of
 repo2docker is inspired by [Heroku Build Packs](https://devcenter.heroku.com/
 articles/buildpacks). ## Docker Image Repo2Docker can be run inside a Docker
 container if access to the Docker Daemon is provided, for example see
 [BinderHub](https://github.com/jupyterhub/binderhub). Docker images are
 [published to quay.io](https://quay.io/repository/jupyterhub/
```

### Comparing `jupyter-repo2docker-2022.2.0/README.md` & `jupyter-repo2docker-2023.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # <a href="https://github.com/jupyterhub/repo2docker"><img src="https://raw.githubusercontent.com/jupyterhub/repo2docker/8731ecf0967cc5fde028c456f2b92be651ebbc18/docs/source/_static/images/repo2docker.png" height="48px" /> repo2docker</a>
 
-[![Build Status](https://github.com/jupyterhub/repo2docker/workflows/Continuous%20Integration/badge.svg)](https://github.com/jupyterhub/repo2docker/actions)
+[![Build Status](https://github.com/jupyterhub/repo2docker/workflows/Test/badge.svg)](https://github.com/jupyterhub/repo2docker/actions)
 [![Documentation Status](https://readthedocs.org/projects/repo2docker/badge/?version=latest)](http://repo2docker.readthedocs.io/en/latest/?badge=latest)
 [![Contribute](https://img.shields.io/badge/I_want_to_contribute!-grey?logo=jupyter)](https://repo2docker.readthedocs.io/en/latest/contributing/contributing.html)
 [![Docker Repository on Quay](https://img.shields.io/badge/quay.io-container-green "Docker Repository on Quay")](https://quay.io/repository/jupyterhub/repo2docker?tab=tags)
 
 `repo2docker` fetches a git repository and builds a container image based on
 the configuration files found in the repository.
 
@@ -27,14 +27,15 @@
 
 For more information, please visit
 [our informational page](https://sustainable-open-science-and-software.github.io/) or download our [participant information sheet](https://sustainable-open-science-and-software.github.io/assets/PIS_sustainable_software.pdf).
 
 ---
 
 ## Using repo2docker
+
 ### Prerequisites
 
 1. Docker to build & run the repositories. The [community edition](https://store.docker.com/search?type=edition&offering=community)
    is recommended.
 2. Python 3.6+.
 
 Supported on Linux and macOS. [See documentation note about Windows support.](http://repo2docker.readthedocs.io/en/latest/install.html#note-about-windows-support)
@@ -79,25 +80,23 @@
     to login with a token:
         http://0.0.0.0:36511/?token=f94f8fabb92e22f5bfab116c382b4707fc2cade56ad1ace0
 ```
 
 If you copy paste that URL into your browser you will see a Jupyter Notebook
 with the contents of the repository you had just built!
 
-For more information on how to use ``repo2docker``, see the
+For more information on how to use `repo2docker`, see the
 [usage guide](http://repo2docker.readthedocs.io/en/latest/usage.html).
 
-
 ## Repository specifications
 
 Repo2Docker looks for configuration files in the source repository to
 determine how the Docker image should be built. For a list of the configuration
-files that ``repo2docker`` can use, see the
+files that `repo2docker` can use, see the
 [complete list of configuration files](https://repo2docker.readthedocs.io/en/latest/config_files.html).
 
 The philosophy of repo2docker is inspired by
 [Heroku Build Packs](https://devcenter.heroku.com/articles/buildpacks).
 
-
 ## Docker Image
 
 Repo2Docker can be run inside a Docker container if access to the Docker Daemon is provided, for example see [BinderHub](https://github.com/jupyterhub/binderhub). Docker images are [published to quay.io](https://quay.io/repository/jupyterhub/repo2docker?tab=tags). The old [Docker Hub image](https://hub.docker.com/r/jupyter/repo2docker) is no longer supported.
```

#### html2text {}

```diff
@@ -1,57 +1,56 @@
 # [https://raw.githubusercontent.com/jupyterhub/repo2docker/
 8731ecf0967cc5fde028c456f2b92be651ebbc18/docs/source/_static/images/
 repo2docker.png]_repo2docker [![Build Status](https://github.com/jupyterhub/
-repo2docker/workflows/Continuous%20Integration/badge.svg)](https://github.com/
-jupyterhub/repo2docker/actions) [![Documentation Status](https://
-readthedocs.org/projects/repo2docker/badge/?version=latest)](http://
-repo2docker.readthedocs.io/en/latest/?badge=latest) [![Contribute](https://
-img.shields.io/badge/I_want_to_contribute!-grey?logo=jupyter)](https://
-repo2docker.readthedocs.io/en/latest/contributing/contributing.html) [![Docker
-Repository on Quay](https://img.shields.io/badge/quay.io-container-green
-"Docker Repository on Quay")](https://quay.io/repository/jupyterhub/
-repo2docker?tab=tags) `repo2docker` fetches a git repository and builds a
-container image based on the configuration files found in the repository. See
-the [repo2docker documentation](http://repo2docker.readthedocs.io) for more
-information on using repo2docker. For support questions please search or post
-to https://discourse.jupyter.org/c/binder. See the [contributing guide]
-(CONTRIBUTING.md) for information on contributing to repo2docker. --- Please
-note that this repository is participating in a study into sustainability of
-open source projects. Data will be gathered about this repository for
-approximately the next 12 months, starting from 2021-06-11. Data collected will
-include number of contributors, number of PRs, time taken to close/merge these
-PRs, and issues closed. For more information, please visit [our informational
-page](https://sustainable-open-science-and-software.github.io/) or download our
-[participant information sheet](https://sustainable-open-science-and-
-software.github.io/assets/PIS_sustainable_software.pdf). --- ## Using
-repo2docker ### Prerequisites 1. Docker to build & run the repositories. The
-[community edition](https://store.docker.com/
-search?type=edition&offering=community) is recommended. 2. Python 3.6+.
-Supported on Linux and macOS. [See documentation note about Windows support.]
-(http://repo2docker.readthedocs.io/en/latest/install.html#note-about-windows-
-support) ### Installation This a quick guide to installing `repo2docker`, see
-our documentation for [a full guide](https://repo2docker.readthedocs.io/en/
-latest/install.html). To install from PyPI: ```bash pip install jupyter-
-repo2docker ``` To install from source: ```bash git clone https://github.com/
-jupyterhub/repo2docker.git cd repo2docker pip install -e . ``` ### Usage The
-core feature of repo2docker is to fetch a git repository (from GitHub or
-locally), build a container image based on the specifications found in the
-repository & optionally launch the container that you can use to explore the
-repository. **Note that Docker needs to be running on your machine for this to
-work.** Example: ```bash jupyter-repo2docker https://github.com/norvig/pytudes
-``` After building (it might take a while!), it should output in your terminal
-something like: ```bash Copy/paste this URL into your browser when you connect
-for the first time, to login with a token: http://0.0.0.0:36511/
-?token=f94f8fabb92e22f5bfab116c382b4707fc2cade56ad1ace0 ``` If you copy paste
-that URL into your browser you will see a Jupyter Notebook with the contents of
-the repository you had just built! For more information on how to use
-``repo2docker``, see the [usage guide](http://repo2docker.readthedocs.io/en/
+repo2docker/workflows/Test/badge.svg)](https://github.com/jupyterhub/
+repo2docker/actions) [![Documentation Status](https://readthedocs.org/projects/
+repo2docker/badge/?version=latest)](http://repo2docker.readthedocs.io/en/
+latest/?badge=latest) [![Contribute](https://img.shields.io/badge/
+I_want_to_contribute!-grey?logo=jupyter)](https://repo2docker.readthedocs.io/
+en/latest/contributing/contributing.html) [![Docker Repository on Quay](https:/
+/img.shields.io/badge/quay.io-container-green "Docker Repository on Quay")]
+(https://quay.io/repository/jupyterhub/repo2docker?tab=tags) `repo2docker`
+fetches a git repository and builds a container image based on the
+configuration files found in the repository. See the [repo2docker
+documentation](http://repo2docker.readthedocs.io) for more information on using
+repo2docker. For support questions please search or post to https://
+discourse.jupyter.org/c/binder. See the [contributing guide](CONTRIBUTING.md)
+for information on contributing to repo2docker. --- Please note that this
+repository is participating in a study into sustainability of open source
+projects. Data will be gathered about this repository for approximately the
+next 12 months, starting from 2021-06-11. Data collected will include number of
+contributors, number of PRs, time taken to close/merge these PRs, and issues
+closed. For more information, please visit [our informational page](https://
+sustainable-open-science-and-software.github.io/) or download our [participant
+information sheet](https://sustainable-open-science-and-software.github.io/
+assets/PIS_sustainable_software.pdf). --- ## Using repo2docker ###
+Prerequisites 1. Docker to build & run the repositories. The [community
+edition](https://store.docker.com/search?type=edition&offering=community) is
+recommended. 2. Python 3.6+. Supported on Linux and macOS. [See documentation
+note about Windows support.](http://repo2docker.readthedocs.io/en/latest/
+install.html#note-about-windows-support) ### Installation This a quick guide to
+installing `repo2docker`, see our documentation for [a full guide](https://
+repo2docker.readthedocs.io/en/latest/install.html). To install from PyPI:
+```bash pip install jupyter-repo2docker ``` To install from source: ```bash git
+clone https://github.com/jupyterhub/repo2docker.git cd repo2docker pip install
+-e . ``` ### Usage The core feature of repo2docker is to fetch a git repository
+(from GitHub or locally), build a container image based on the specifications
+found in the repository & optionally launch the container that you can use to
+explore the repository. **Note that Docker needs to be running on your machine
+for this to work.** Example: ```bash jupyter-repo2docker https://github.com/
+norvig/pytudes ``` After building (it might take a while!), it should output in
+your terminal something like: ```bash Copy/paste this URL into your browser
+when you connect for the first time, to login with a token: http://0.0.0.0:
+36511/?token=f94f8fabb92e22f5bfab116c382b4707fc2cade56ad1ace0 ``` If you copy
+paste that URL into your browser you will see a Jupyter Notebook with the
+contents of the repository you had just built! For more information on how to
+use `repo2docker`, see the [usage guide](http://repo2docker.readthedocs.io/en/
 latest/usage.html). ## Repository specifications Repo2Docker looks for
 configuration files in the source repository to determine how the Docker image
-should be built. For a list of the configuration files that ``repo2docker`` can
+should be built. For a list of the configuration files that `repo2docker` can
 use, see the [complete list of configuration files](https://
 repo2docker.readthedocs.io/en/latest/config_files.html). The philosophy of
 repo2docker is inspired by [Heroku Build Packs](https://devcenter.heroku.com/
 articles/buildpacks). ## Docker Image Repo2Docker can be run inside a Docker
 container if access to the Docker Daemon is provided, for example see
 [BinderHub](https://github.com/jupyterhub/binderhub). Docker images are
 [published to quay.io](https://quay.io/repository/jupyterhub/
```

### Comparing `jupyter-repo2docker-2022.2.0/jupyter_repo2docker.egg-info/PKG-INFO` & `jupyter-repo2docker-2023.6.0/jupyter_repo2docker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,35 +1,34 @@
 Metadata-Version: 2.1
 Name: jupyter-repo2docker
-Version: 2022.2.0
+Version: 2023.6.0
 Summary: Repo2docker: Turn code repositories into Jupyter enabled Docker Images
 Home-page: https://repo2docker.readthedocs.io/en/latest/
 Author: Project Jupyter Contributors
 Author-email: jupyter@googlegroups.com
 License: BSD
 Project-URL: Documentation, https://repo2docker.readthedocs.io
 Project-URL: Funding, https://jupyter.org/about
 Project-URL: Source, https://github.com/jupyterhub/repo2docker/
 Project-URL: Tracker, https://github.com/jupyterhub/repo2docker/issues
 Keywords: reproducible science environments docker
-Platform: UNKNOWN
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # <a href="https://github.com/jupyterhub/repo2docker"><img src="https://raw.githubusercontent.com/jupyterhub/repo2docker/8731ecf0967cc5fde028c456f2b92be651ebbc18/docs/source/_static/images/repo2docker.png" height="48px" /> repo2docker</a>
 
-[![Build Status](https://github.com/jupyterhub/repo2docker/workflows/Continuous%20Integration/badge.svg)](https://github.com/jupyterhub/repo2docker/actions)
+[![Build Status](https://github.com/jupyterhub/repo2docker/workflows/Test/badge.svg)](https://github.com/jupyterhub/repo2docker/actions)
 [![Documentation Status](https://readthedocs.org/projects/repo2docker/badge/?version=latest)](http://repo2docker.readthedocs.io/en/latest/?badge=latest)
 [![Contribute](https://img.shields.io/badge/I_want_to_contribute!-grey?logo=jupyter)](https://repo2docker.readthedocs.io/en/latest/contributing/contributing.html)
 [![Docker Repository on Quay](https://img.shields.io/badge/quay.io-container-green "Docker Repository on Quay")](https://quay.io/repository/jupyterhub/repo2docker?tab=tags)
 
 `repo2docker` fetches a git repository and builds a container image based on
 the configuration files found in the repository.
 
@@ -52,14 +51,15 @@
 
 For more information, please visit
 [our informational page](https://sustainable-open-science-and-software.github.io/) or download our [participant information sheet](https://sustainable-open-science-and-software.github.io/assets/PIS_sustainable_software.pdf).
 
 ---
 
 ## Using repo2docker
+
 ### Prerequisites
 
 1. Docker to build & run the repositories. The [community edition](https://store.docker.com/search?type=edition&offering=community)
    is recommended.
 2. Python 3.6+.
 
 Supported on Linux and macOS. [See documentation note about Windows support.](http://repo2docker.readthedocs.io/en/latest/install.html#note-about-windows-support)
@@ -104,27 +104,23 @@
     to login with a token:
         http://0.0.0.0:36511/?token=f94f8fabb92e22f5bfab116c382b4707fc2cade56ad1ace0
 ```
 
 If you copy paste that URL into your browser you will see a Jupyter Notebook
 with the contents of the repository you had just built!
 
-For more information on how to use ``repo2docker``, see the
+For more information on how to use `repo2docker`, see the
 [usage guide](http://repo2docker.readthedocs.io/en/latest/usage.html).
 
-
 ## Repository specifications
 
 Repo2Docker looks for configuration files in the source repository to
 determine how the Docker image should be built. For a list of the configuration
-files that ``repo2docker`` can use, see the
+files that `repo2docker` can use, see the
 [complete list of configuration files](https://repo2docker.readthedocs.io/en/latest/config_files.html).
 
 The philosophy of repo2docker is inspired by
 [Heroku Build Packs](https://devcenter.heroku.com/articles/buildpacks).
 
-
 ## Docker Image
 
 Repo2Docker can be run inside a Docker container if access to the Docker Daemon is provided, for example see [BinderHub](https://github.com/jupyterhub/binderhub). Docker images are [published to quay.io](https://quay.io/repository/jupyterhub/repo2docker?tab=tags). The old [Docker Hub image](https://hub.docker.com/r/jupyter/repo2docker) is no longer supported.
-
-
```

#### html2text {}

```diff
@@ -1,70 +1,69 @@
-Metadata-Version: 2.1 Name: jupyter-repo2docker Version: 2022.2.0 Summary:
+Metadata-Version: 2.1 Name: jupyter-repo2docker Version: 2023.6.0 Summary:
 Repo2docker: Turn code repositories into Jupyter enabled Docker Images Home-
 page: https://repo2docker.readthedocs.io/en/latest/ Author: Project Jupyter
 Contributors Author-email: jupyter@googlegroups.com License: BSD Project-URL:
 Documentation, https://repo2docker.readthedocs.io Project-URL: Funding, https:/
 /jupyter.org/about Project-URL: Source, https://github.com/jupyterhub/
 repo2docker/ Project-URL: Tracker, https://github.com/jupyterhub/repo2docker/
-issues Keywords: reproducible science environments docker Platform: UNKNOWN
-Classifier: Environment :: Console Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: System Administrators Classifier: Intended
-Audience :: Science/Research Classifier: License :: OSI Approved :: BSD License
-Classifier: Programming Language :: Python Classifier: Programming Language ::
-Python :: 3 Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE # [https://raw.githubusercontent.com/jupyterhub/
-repo2docker/8731ecf0967cc5fde028c456f2b92be651ebbc18/docs/source/_static/
-images/repo2docker.png]_repo2docker [![Build Status](https://github.com/
-jupyterhub/repo2docker/workflows/Continuous%20Integration/badge.svg)](https://
-github.com/jupyterhub/repo2docker/actions) [![Documentation Status](https://
-readthedocs.org/projects/repo2docker/badge/?version=latest)](http://
-repo2docker.readthedocs.io/en/latest/?badge=latest) [![Contribute](https://
-img.shields.io/badge/I_want_to_contribute!-grey?logo=jupyter)](https://
-repo2docker.readthedocs.io/en/latest/contributing/contributing.html) [![Docker
-Repository on Quay](https://img.shields.io/badge/quay.io-container-green
-"Docker Repository on Quay")](https://quay.io/repository/jupyterhub/
-repo2docker?tab=tags) `repo2docker` fetches a git repository and builds a
-container image based on the configuration files found in the repository. See
-the [repo2docker documentation](http://repo2docker.readthedocs.io) for more
-information on using repo2docker. For support questions please search or post
-to https://discourse.jupyter.org/c/binder. See the [contributing guide]
-(CONTRIBUTING.md) for information on contributing to repo2docker. --- Please
-note that this repository is participating in a study into sustainability of
-open source projects. Data will be gathered about this repository for
-approximately the next 12 months, starting from 2021-06-11. Data collected will
-include number of contributors, number of PRs, time taken to close/merge these
-PRs, and issues closed. For more information, please visit [our informational
-page](https://sustainable-open-science-and-software.github.io/) or download our
-[participant information sheet](https://sustainable-open-science-and-
-software.github.io/assets/PIS_sustainable_software.pdf). --- ## Using
-repo2docker ### Prerequisites 1. Docker to build & run the repositories. The
-[community edition](https://store.docker.com/
-search?type=edition&offering=community) is recommended. 2. Python 3.6+.
-Supported on Linux and macOS. [See documentation note about Windows support.]
-(http://repo2docker.readthedocs.io/en/latest/install.html#note-about-windows-
-support) ### Installation This a quick guide to installing `repo2docker`, see
-our documentation for [a full guide](https://repo2docker.readthedocs.io/en/
-latest/install.html). To install from PyPI: ```bash pip install jupyter-
-repo2docker ``` To install from source: ```bash git clone https://github.com/
-jupyterhub/repo2docker.git cd repo2docker pip install -e . ``` ### Usage The
-core feature of repo2docker is to fetch a git repository (from GitHub or
-locally), build a container image based on the specifications found in the
-repository & optionally launch the container that you can use to explore the
-repository. **Note that Docker needs to be running on your machine for this to
-work.** Example: ```bash jupyter-repo2docker https://github.com/norvig/pytudes
-``` After building (it might take a while!), it should output in your terminal
-something like: ```bash Copy/paste this URL into your browser when you connect
-for the first time, to login with a token: http://0.0.0.0:36511/
-?token=f94f8fabb92e22f5bfab116c382b4707fc2cade56ad1ace0 ``` If you copy paste
-that URL into your browser you will see a Jupyter Notebook with the contents of
-the repository you had just built! For more information on how to use
-``repo2docker``, see the [usage guide](http://repo2docker.readthedocs.io/en/
+issues Keywords: reproducible science environments docker Classifier:
+Environment :: Console Classifier: Intended Audience :: Developers Classifier:
+Intended Audience :: System Administrators Classifier: Intended Audience ::
+Science/Research Classifier: License :: OSI Approved :: BSD License Classifier:
+Programming Language :: Python Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.6 Description-Content-Type: text/markdown License-File:
+LICENSE # [https://raw.githubusercontent.com/jupyterhub/repo2docker/
+8731ecf0967cc5fde028c456f2b92be651ebbc18/docs/source/_static/images/
+repo2docker.png]_repo2docker [![Build Status](https://github.com/jupyterhub/
+repo2docker/workflows/Test/badge.svg)](https://github.com/jupyterhub/
+repo2docker/actions) [![Documentation Status](https://readthedocs.org/projects/
+repo2docker/badge/?version=latest)](http://repo2docker.readthedocs.io/en/
+latest/?badge=latest) [![Contribute](https://img.shields.io/badge/
+I_want_to_contribute!-grey?logo=jupyter)](https://repo2docker.readthedocs.io/
+en/latest/contributing/contributing.html) [![Docker Repository on Quay](https:/
+/img.shields.io/badge/quay.io-container-green "Docker Repository on Quay")]
+(https://quay.io/repository/jupyterhub/repo2docker?tab=tags) `repo2docker`
+fetches a git repository and builds a container image based on the
+configuration files found in the repository. See the [repo2docker
+documentation](http://repo2docker.readthedocs.io) for more information on using
+repo2docker. For support questions please search or post to https://
+discourse.jupyter.org/c/binder. See the [contributing guide](CONTRIBUTING.md)
+for information on contributing to repo2docker. --- Please note that this
+repository is participating in a study into sustainability of open source
+projects. Data will be gathered about this repository for approximately the
+next 12 months, starting from 2021-06-11. Data collected will include number of
+contributors, number of PRs, time taken to close/merge these PRs, and issues
+closed. For more information, please visit [our informational page](https://
+sustainable-open-science-and-software.github.io/) or download our [participant
+information sheet](https://sustainable-open-science-and-software.github.io/
+assets/PIS_sustainable_software.pdf). --- ## Using repo2docker ###
+Prerequisites 1. Docker to build & run the repositories. The [community
+edition](https://store.docker.com/search?type=edition&offering=community) is
+recommended. 2. Python 3.6+. Supported on Linux and macOS. [See documentation
+note about Windows support.](http://repo2docker.readthedocs.io/en/latest/
+install.html#note-about-windows-support) ### Installation This a quick guide to
+installing `repo2docker`, see our documentation for [a full guide](https://
+repo2docker.readthedocs.io/en/latest/install.html). To install from PyPI:
+```bash pip install jupyter-repo2docker ``` To install from source: ```bash git
+clone https://github.com/jupyterhub/repo2docker.git cd repo2docker pip install
+-e . ``` ### Usage The core feature of repo2docker is to fetch a git repository
+(from GitHub or locally), build a container image based on the specifications
+found in the repository & optionally launch the container that you can use to
+explore the repository. **Note that Docker needs to be running on your machine
+for this to work.** Example: ```bash jupyter-repo2docker https://github.com/
+norvig/pytudes ``` After building (it might take a while!), it should output in
+your terminal something like: ```bash Copy/paste this URL into your browser
+when you connect for the first time, to login with a token: http://0.0.0.0:
+36511/?token=f94f8fabb92e22f5bfab116c382b4707fc2cade56ad1ace0 ``` If you copy
+paste that URL into your browser you will see a Jupyter Notebook with the
+contents of the repository you had just built! For more information on how to
+use `repo2docker`, see the [usage guide](http://repo2docker.readthedocs.io/en/
 latest/usage.html). ## Repository specifications Repo2Docker looks for
 configuration files in the source repository to determine how the Docker image
-should be built. For a list of the configuration files that ``repo2docker`` can
+should be built. For a list of the configuration files that `repo2docker` can
 use, see the [complete list of configuration files](https://
 repo2docker.readthedocs.io/en/latest/config_files.html). The philosophy of
 repo2docker is inspired by [Heroku Build Packs](https://devcenter.heroku.com/
 articles/buildpacks). ## Docker Image Repo2Docker can be run inside a Docker
 container if access to the Docker Daemon is provided, for example see
 [BinderHub](https://github.com/jupyterhub/binderhub). Docker images are
 [published to quay.io](https://quay.io/repository/jupyterhub/
```

### Comparing `jupyter-repo2docker-2022.2.0/jupyter_repo2docker.egg-info/SOURCES.txt` & `jupyter-repo2docker-2023.6.0/jupyter_repo2docker.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 CONTRIBUTING.md
 LICENSE
 MANIFEST.in
 README.md
+RELEASE.md
 ROADMAP.md
 setup.cfg
 setup.py
 versioneer.py
 jupyter_repo2docker.egg-info/PKG-INFO
 jupyter_repo2docker.egg-info/SOURCES.txt
 jupyter_repo2docker.egg-info/dependency_links.txt
@@ -25,31 +26,39 @@
 repo2docker/buildpacks/base.py
 repo2docker/buildpacks/docker.py
 repo2docker/buildpacks/python3-login
 repo2docker/buildpacks/r.py
 repo2docker/buildpacks/repo2docker-entrypoint
 repo2docker/buildpacks/conda/__init__.py
 repo2docker/buildpacks/conda/activate-conda.sh
-repo2docker/buildpacks/conda/environment.lock
-repo2docker/buildpacks/conda/environment.py-2.7.lock
+repo2docker/buildpacks/conda/environment.py-2.7-linux-64.lock
 repo2docker/buildpacks/conda/environment.py-2.7.yml
-repo2docker/buildpacks/conda/environment.py-3.5.lock
+repo2docker/buildpacks/conda/environment.py-3.10-linux-64.lock
+repo2docker/buildpacks/conda/environment.py-3.10-linux-aarch64.lock
+repo2docker/buildpacks/conda/environment.py-3.10.yml
+repo2docker/buildpacks/conda/environment.py-3.11-linux-64.lock
+repo2docker/buildpacks/conda/environment.py-3.11-linux-aarch64.lock
+repo2docker/buildpacks/conda/environment.py-3.11.lock
+repo2docker/buildpacks/conda/environment.py-3.11.yml
+repo2docker/buildpacks/conda/environment.py-3.5-linux-64.lock
 repo2docker/buildpacks/conda/environment.py-3.5.yml
-repo2docker/buildpacks/conda/environment.py-3.6.lock
+repo2docker/buildpacks/conda/environment.py-3.6-linux-64.lock
 repo2docker/buildpacks/conda/environment.py-3.6.yml
-repo2docker/buildpacks/conda/environment.py-3.7.lock
+repo2docker/buildpacks/conda/environment.py-3.7-linux-64.lock
+repo2docker/buildpacks/conda/environment.py-3.7-linux-aarch64.lock
 repo2docker/buildpacks/conda/environment.py-3.7.yml
-repo2docker/buildpacks/conda/environment.py-3.8.lock
+repo2docker/buildpacks/conda/environment.py-3.8-linux-64.lock
+repo2docker/buildpacks/conda/environment.py-3.8-linux-aarch64.lock
 repo2docker/buildpacks/conda/environment.py-3.8.yml
-repo2docker/buildpacks/conda/environment.py-3.9.lock
+repo2docker/buildpacks/conda/environment.py-3.9-linux-64.lock
+repo2docker/buildpacks/conda/environment.py-3.9-linux-aarch64.lock
 repo2docker/buildpacks/conda/environment.py-3.9.yml
 repo2docker/buildpacks/conda/environment.yml
 repo2docker/buildpacks/conda/freeze.py
 repo2docker/buildpacks/conda/install-base-env.bash
-repo2docker/buildpacks/conda/requirements.py-3.5.pip
 repo2docker/buildpacks/julia/__init__.py
 repo2docker/buildpacks/julia/install-repo-dependencies.jl
 repo2docker/buildpacks/julia/julia_project.py
 repo2docker/buildpacks/julia/julia_require.py
 repo2docker/buildpacks/legacy/__init__.py
 repo2docker/buildpacks/nix/__init__.py
 repo2docker/buildpacks/nix/install-nix.bash
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/__main__.py` & `jupyter-repo2docker-2023.6.0/repo2docker/__main__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,20 @@
 import argparse
-import sys
-import os
 import logging
+import os
+import sys
+
+from . import __version__
 from .app import Repo2Docker
 from .engine import BuildError, ImageLoadError
-from . import __version__
-from .utils import validate_and_generate_port_mapping, is_valid_docker_image_name
+from .utils import (
+    R2dState,
+    is_valid_docker_image_name,
+    validate_and_generate_port_mapping,
+)
 
 
 def validate_image_name(image_name):
     """
     Validate image_name read by argparse
 
     Note: Container names must start with an alphanumeric character and
@@ -44,15 +49,15 @@
     def __call__(self, parser, namespace, values, option_string=None):
         # There are 3 cases:
         #  key=value    pass as is
         #  key=         pass as is
         #  key          pass using current value, or don't pass
         if "=" not in values:
             try:
-                value_to_append = "{}={}".format(values, os.environ[values])
+                value_to_append = f"{values}={os.environ[values]}"
             except KeyError:
                 # no local def, so don't pass
                 return
         else:
             value_to_append = values
 
         # destination variable is initially defined as an empty list, so
@@ -84,53 +89,60 @@
         "--config",
         default="repo2docker_config.py",
         help="Path to config file for repo2docker",
     )
 
     argparser.add_argument(
         "--json-logs",
-        default=False,
+        default=None,
         action="store_true",
         help="Emit JSON logs instead of human readable logs",
     )
 
     argparser.add_argument(
         "repo",
         help=(
             "Path to repository that should be built. Could be "
             "local path or a git URL."
         ),
     )
 
     argparser.add_argument(
         "--image-name",
-        help=("Name of image to be built. If unspecified will be " "autogenerated"),
+        help="Name of image to be built. If unspecified will be autogenerated",
         type=validate_image_name,
     )
 
     argparser.add_argument(
         "--ref",
+        default=None,
         help=(
             "Reference to build instead of default reference. For example"
             " branch name or commit for a Git repository."
         ),
     )
 
     argparser.add_argument("--debug", help="Turn on debug logging", action="store_true")
 
     argparser.add_argument(
         "--no-build",
         dest="build",
         action="store_false",
-        help=(
-            "Do not actually build the image. Useful in conjunction " "with --debug."
-        ),
+        help="Do not actually build the image. Useful in conjunction with --debug.",
     )
 
     argparser.add_argument(
+        "--build",
+        dest="build",
+        action="store_true",
+        help="Build the image (default)",
+    )
+    argparser.set_defaults(build=None)
+
+    argparser.add_argument(
         "--build-memory-limit",
         help="Total Memory that can be used by the docker build process",
     )
 
     argparser.add_argument(
         "cmd",
         nargs=argparse.REMAINDER,
@@ -141,45 +153,68 @@
         "--no-run",
         dest="run",
         action="store_false",
         help="Do not run container after it has been built",
     )
 
     argparser.add_argument(
+        "--run",
+        dest="run",
+        action="store_true",
+        help="Run container after it has been built (default).",
+    )
+    argparser.set_defaults(run=None)
+
+    argparser.add_argument(
         "--publish",
         "-p",
         dest="ports",
         action="append",
         help=(
             "Specify port mappings for the image. Needs a command to "
             "run in the container."
         ),
     )
 
     argparser.add_argument(
         "--publish-all",
         "-P",
         dest="all_ports",
+        default=None,
         action="store_true",
         help="Publish all exposed ports to random host ports.",
     )
 
     argparser.add_argument(
         "--no-clean",
         dest="clean",
         action="store_false",
         help="Don't clean up remote checkouts after we are done",
     )
+    argparser.add_argument(
+        "--clean",
+        dest="clean",
+        action="store_true",
+        help="Clean up remote checkouts after we are done (default).",
+    )
+    argparser.set_defaults(clean=None)
 
     argparser.add_argument(
         "--push",
         dest="push",
         action="store_true",
         help="Push docker image to repository",
     )
+    argparser.add_argument(
+        "--no-push",
+        dest="push",
+        action="store_false",
+        help="Don't push docker image to repository (default).",
+    )
+    argparser.set_defaults(push=None)
 
     argparser.add_argument(
         "--volume",
         "-v",
         dest="volumes",
         action="append",
         help="Volumes to mount inside the container, in form src:dest",
@@ -236,19 +271,25 @@
 
     argparser.add_argument("--subdir", type=str, help=Repo2Docker.subdir.help)
 
     argparser.add_argument(
         "--cache-from", action="append", default=[], help=Repo2Docker.cache_from.help
     )
 
-    argparser.add_argument("--engine", help="Name of the container engine")
+    argparser.add_argument(
+        "--engine",
+        type=str,
+        default="docker",
+        help=Repo2Docker.engine.help,
+    )
 
     return argparser
 
 
+# Note: only used by sphinx-autoprogram
 argparser = get_argparser()
 
 
 def make_r2d(argv=None):
     if argv is None:
         argv = sys.argv[1:]
 
@@ -265,104 +306,121 @@
         print("\nAll configurable options:\n")
         Repo2Docker().print_help(classes=True)
         sys.exit(0)
 
     args, traitlet_args = argparser.parse_known_args(argv)
 
     r2d = Repo2Docker()
-    r2d.parse_command_line(traitlet_args)
 
     if args.debug:
         r2d.log_level = logging.DEBUG
 
+    # load CLI after config file, for correct priority
     r2d.load_config_file(args.config)
+    r2d.parse_command_line(traitlet_args)
+
+    if args.debug:
+        # re-apply debug in case log_level was also set via config
+        r2d.log_level = logging.DEBUG
+
     if args.appendix:
         r2d.appendix = args.appendix
 
     for l in args.labels:
         key, _, val = l.partition("=")
         r2d.labels[key] = val
 
     for a in args.build_args:
         key, _, val = a.partition("=")
         r2d.extra_build_args[key] = val
 
+    # repo is a required arg, and should never come from config:
+    if "repo" in r2d.config.Repo2Docker:
+        r2d.log.warning(
+            f"Ignoring Repo2Docker.repo={r2d.repo!r} configuration, using {args.repo!r} from CLI."
+        )
     r2d.repo = args.repo
-    r2d.ref = args.ref
+    if args.ref is not None:
+        r2d.ref = args.ref
 
     # user wants to mount a local directory into the container for
     # editing
     if args.editable:
         # the user has to point at a directory, not just a path for us
         # to be able to mount it. We might have content providers that can
         # provide content from a local `something.zip` file, which we
         # couldn't mount in editable mode
         if os.path.isdir(args.repo):
             r2d.volumes[os.path.abspath(args.repo)] = "."
         else:
             r2d.log.error(
-                'Cannot mount "{}" in editable mode '
-                "as it is not a directory".format(args.repo),
-                extra=dict(phase="failed"),
+                f'Cannot mount "{args.repo}" in editable mode '
+                "as it is not a directory",
+                extra=dict(phase=R2dState.FAILED),
             )
             sys.exit(1)
 
     if args.image_name:
         r2d.output_image_spec = args.image_name
-    else:
-        # we will pick a name after fetching the repository
-        r2d.output_image_spec = ""
 
-    r2d.json_logs = args.json_logs
+    if args.json_logs is not None:
+        r2d.json_logs = args.json_logs
 
-    r2d.dry_run = not args.build
+    if args.build is not None:
+        r2d.dry_run = not args.build
 
     if r2d.dry_run:
         # Can't push nor run if we aren't building
         args.run = False
         args.push = False
 
-    r2d.run = args.run
-    r2d.push = args.push
+    if args.run is not None:
+        r2d.run = args.run
+    if args.push is not None:
+        r2d.push = args.push
 
     # check against r2d.run and not args.run as r2d.run is false on
     # --no-build. Also r2d.volumes and not args.volumes since --editable
     # modified r2d.volumes
     if r2d.volumes and not r2d.run:
         # Can't mount if we aren't running
         print("To Mount volumes with -v, you also need to run the " "container")
         sys.exit(1)
 
     for v in args.volumes:
         src, dest = v.split(":")
         r2d.volumes[src] = dest
 
-    r2d.run_cmd = args.cmd
+    if args.cmd:
+        r2d.run_cmd = args.cmd
 
     if args.all_ports and not r2d.run:
-        print(
-            "To publish user defined port mappings, the container must " "also be run"
-        )
+        print("To publish user-defined port mappings, the container must also be run")
         sys.exit(1)
 
     if args.ports and not r2d.run:
-        print(
-            "To publish user defined port mappings, the container must " "also be run"
-        )
+        print("To publish user-defined port mappings, the container must also be run")
         sys.exit(1)
 
-    if args.ports and not r2d.run_cmd:
+    if args.ports and len(args.ports) > 1 and not r2d.run_cmd:
         print(
-            "To publish user defined port mapping, user must specify "
-            "the command to run in the container"
+            "To publish user-defined port mapping, "
+            "you must specify the command to run in the container"
         )
         sys.exit(1)
 
-    r2d.ports = validate_and_generate_port_mapping(args.ports)
-    r2d.all_ports = args.all_ports
+    if args.ports:
+        # override or update, if also defined in config file?
+        if r2d.ports:
+            r2d.log.warning(
+                f"Ignoring port configuration from config (ports={r2d.ports}), overridden by CLI"
+            )
+        r2d.ports = validate_and_generate_port_mapping(args.ports)
+    if args.all_ports is not None:
+        r2d.all_ports = args.all_ports
 
     if args.user_id:
         r2d.user_id = args.user_id
     if args.user_name:
         r2d.user_name = args.user_name
     if r2d.user_id == 0 and not r2d.dry_run:
         print("Root as the primary user in the image is not permitted.")
@@ -392,21 +450,19 @@
 
     if args.cache_from:
         r2d.cache_from = args.cache_from
 
     if args.engine:
         r2d.engine = args.engine
 
-    r2d.environment = args.environment
+    if args.environment:
+        # extend any environment config from a config file
+        r2d.environment.extend(args.environment)
 
-    # if the source exists locally we don't want to delete it at the end
-    # FIXME: Find a better way to figure out if repo is 'local'. Push this into ContentProvider?
-    if os.path.exists(args.repo):
-        r2d.cleanup_checkout = False
-    else:
+    elif args.clean is not None:
         r2d.cleanup_checkout = args.clean
 
     if args.target_repo_dir:
         r2d.target_repo_dir = args.target_repo_dir
 
     return r2d
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/app.py` & `jupyter-repo2docker-2023.6.0/repo2docker/app.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,46 +3,45 @@
 Images produced by repo2docker can be used with Jupyter notebooks standalone
 or with BinderHub.
 
 Usage:
 
     python -m repo2docker https://github.com/you/your-repo
 """
+import getpass
 import json
-import sys
 import logging
 import os
-import entrypoints
-import getpass
 import shutil
+import sys
 import tempfile
 import time
+import warnings
 from urllib.parse import urlparse
 
+import entrypoints
 import escapism
 from pythonjsonlogger import jsonlogger
-
-from traitlets import Any, Dict, Int, List, Unicode, Bool, default
+from traitlets import Any, Bool, Dict, Int, List, Unicode, default, observe
 from traitlets.config import Application
 
-from . import __version__
+from . import __version__, contentproviders
 from .buildpacks import (
     CondaBuildPack,
     DockerBuildPack,
     JuliaProjectTomlBuildPack,
     JuliaRequireBuildPack,
     LegacyBinderDockerBuildPack,
     NixBuildPack,
     PipfileBuildPack,
     PythonBuildPack,
     RBuildPack,
 )
-from . import contentproviders
 from .engine import BuildError, ContainerEngineException, ImageLoadError
-from .utils import ByteSpecification, chdir
+from .utils import ByteSpecification, R2dState, chdir, get_platform
 
 
 class Repo2Docker(Application):
     """An application for converting git repositories to docker images"""
 
     name = "jupyter-repo2docker"
     version = __version__
@@ -248,14 +247,35 @@
 
         Each Label is a key-value pair, with the key being the name of the label
         and the value its value.
         """,
         config=True,
     )
 
+    platform = Unicode(
+        config=True,
+        help="""
+        Platform to build for, linux/amd64 (recommended) or linux/arm64 (experimental).
+        """,
+    )
+
+    @default("platform")
+    def _platform_default(self):
+        """
+        Default platform
+        """
+        p = get_platform()
+        if p == "linux/arm64":
+            warnings.warn(
+                "Building for linux/arm64 is experimental. "
+                "To use the recommended platform set --Repo2Docker.platform=linux/amd64. "
+                "To silence this warning set --Repo2Docker.platform=linux/arm64."
+            )
+        return p
+
     extra_build_args = Dict(
         {},
         help="""
         Extra build args to pass to the image build process.
         This is pretty much only useful for custom Dockerfile based builds.
         """,
         config=True,
@@ -302,23 +322,29 @@
         Heritage API.
         """,
         config=True,
         allow_none=True,
     )
 
     cleanup_checkout = Bool(
-        False,
+        True,
         help="""
         Delete source repository after building is done.
 
         Useful when repo2docker is doing the git cloning
         """,
         config=True,
     )
 
+    @default("cleanup_checkout")
+    def _defaut_cleanup_checkout(self):
+        # if the source exists locally we don't want to delete it at the end
+        # FIXME: Find a better way to figure out if repo is 'local'. Push this into ContentProvider?
+        return not os.path.exists(self.repo)
+
     output_image_spec = Unicode(
         "",
         help="""
         Docker Image name:tag to tag the built image with.
 
         Required parameter.
         """,
@@ -330,15 +356,15 @@
         help="""
         Set to true to push docker image after building
         """,
         config=True,
     )
 
     run = Bool(
-        False,
+        True,
         help="""
         Run docker image after building
         """,
         config=True,
     )
 
     # FIXME: Refactor class to be able to do --no-build without needing
@@ -347,14 +373,20 @@
         False,
         help="""
         Do not actually build the docker image, just simulate it.
         """,
         config=True,
     )
 
+    @observe("dry_run")
+    def _dry_run_changed(self, change):
+        if change.new:
+            # dry_run forces run and push to be False
+            self.push = self.run = False
+
     # FIXME: Refactor classes to separate build & run steps
     run_cmd = List(
         [],
         help="""
         Command to run when running the container
 
         When left empty, a jupyter notebook is run.
@@ -411,27 +443,40 @@
         help="""
         Name of the container engine.
 
         Defaults to 'docker'.
         """,
     )
 
+    base_image = Unicode(
+        "docker.io/library/buildpack-deps:bionic",
+        config=True,
+        help="""
+        Base image to use when building docker images.
+
+        Only images that match the following criteria are supported:
+        - Ubuntu based distributions, minimum 18.04
+        - Contains set of base packages installed with the buildpack-deps
+          image family: https://hub.docker.com/_/buildpack-deps
+
+        Other images *may* work, but are not officially supported.
+        """,
+    )
+
     def get_engine(self):
         """Return an instance of the container engine.
 
         Currently no arguments are passed to the engine constructor.
         """
         engines = entrypoints.get_group_named("repo2docker.engines")
         try:
             entry = engines[self.engine]
         except KeyError:
             raise ContainerEngineException(
-                "Container engine '{}' not found. Available engines: {}".format(
-                    self.engine, ",".join(engines.keys())
-                )
+                f"Container engine '{self.engine}' not found. Available engines: {','.join(engines.keys())}"
             )
         engine_class = entry.load()
         return engine_class(parent=self)
 
     def fetch(self, url, ref, checkout_path):
         """Fetch the contents of `url` and place it in `checkout_path`.
 
@@ -443,33 +488,28 @@
         """
         picked_content_provider = None
         for ContentProvider in self.content_providers:
             cp = ContentProvider()
             spec = cp.detect(url, ref=ref)
             if spec is not None:
                 picked_content_provider = cp
-                self.log.info(
-                    "Picked {cp} content "
-                    "provider.\n".format(cp=cp.__class__.__name__)
-                )
+                self.log.info(f"Picked {cp.__class__.__name__} content provider.\n")
                 break
 
         if picked_content_provider is None:
-            self.log.error(
-                "No matching content provider found for " "{url}.".format(url=url)
-            )
+            self.log.error(f"No matching content provider found for {url}.")
 
         swh_token = self.config.get("swh_token", self.swh_token)
         if swh_token and isinstance(picked_content_provider, contentproviders.Swhid):
             picked_content_provider.set_auth_token(swh_token)
 
         for log_line in picked_content_provider.fetch(
             spec, checkout_path, yield_output=self.json_logs
         ):
-            self.log.info(log_line, extra=dict(phase="fetching"))
+            self.log.info(log_line, extra=dict(phase=R2dState.FETCHING))
 
         if not self.output_image_spec:
             image_spec = "r2d" + self.repo
             # if we are building from a subdirectory include that in the
             # image name so we can tell builds from different sub-directories
             # apart.
             if self.subdir:
@@ -484,34 +524,33 @@
 
     def json_excepthook(self, etype, evalue, traceback):
         """Called on an uncaught exception when using json logging
 
         Avoids non-JSON output on errors when using --json-logs
         """
         self.log.error(
-            "Error during build: %s",
-            evalue,
+            f"Error during build: {evalue}",
             exc_info=(etype, evalue, traceback),
-            extra=dict(phase="failed"),
+            extra=dict(phase=R2dState.FAILED),
         )
 
     def initialize(self, *args, **kwargs):
         """Init repo2docker configuration before start"""
         # FIXME: Remove this function, move it to setters / traitlet reactors
+        self.log = logging.getLogger("repo2docker")
+        self.log.setLevel(self.log_level)
+        logHandler = logging.StreamHandler()
+        self.log.handlers = []
+        self.log.addHandler(logHandler)
         if self.json_logs:
             # register JSON excepthook to avoid non-JSON output on errors
             sys.excepthook = self.json_excepthook
             # Need to reset existing handlers, or we repeat messages
-            logHandler = logging.StreamHandler()
             formatter = jsonlogger.JsonFormatter()
             logHandler.setFormatter(formatter)
-            self.log = logging.getLogger("repo2docker")
-            self.log.handlers = []
-            self.log.addHandler(logHandler)
-            self.log.setLevel(self.log_level)
         else:
             # due to json logger stuff above,
             # our log messages include carriage returns, newlines, etc.
             # remove the additional newline from the stream handler
             self.log.handlers[0].terminator = ""
             # We don't want a [Repo2Docker] on all messages
             self.log.handlers[0].formatter = logging.Formatter(fmt="%(message)s")
@@ -528,50 +567,52 @@
         # Build a progress setup for each layer, and only emit per-layer
         # info every 1.5s
         progress_layers = {}
         layers = {}
         last_emit_time = time.time()
         for chunk in client.push(self.output_image_spec):
             if client.string_output:
-                self.log.info(chunk, extra=dict(phase="pushing"))
+                self.log.info(chunk, extra=dict(phase=R2dState.PUSHING))
                 continue
             # else this is Docker output
 
             # each chunk can be one or more lines of json events
             # split lines here in case multiple are delivered at once
             for line in chunk.splitlines():
                 line = line.decode("utf-8", errors="replace")
                 try:
                     progress = json.loads(line)
                 except Exception as e:
                     self.log.warning("Not a JSON progress line: %r", line)
                     continue
                 if "error" in progress:
-                    self.log.error(progress["error"], extra=dict(phase="failed"))
+                    self.log.error(progress["error"], extra=dict(phase=R2dState.FAILED))
                     raise ImageLoadError(progress["error"])
                 if "id" not in progress:
                     continue
                 # deprecated truncated-progress data
                 if "progressDetail" in progress and progress["progressDetail"]:
                     progress_layers[progress["id"]] = progress["progressDetail"]
                 else:
                     progress_layers[progress["id"]] = progress["status"]
                 # include full progress data for each layer in 'layers' data
                 layers[progress["id"]] = progress
                 if time.time() - last_emit_time > 1.5:
                     self.log.info(
                         "Pushing image\n",
                         extra=dict(
-                            progress=progress_layers, layers=layers, phase="pushing"
+                            progress=progress_layers,
+                            layers=layers,
+                            phase=R2dState.PUSHING,
                         ),
                     )
                     last_emit_time = time.time()
         self.log.info(
-            "Successfully pushed {}".format(self.output_image_spec),
-            extra=dict(phase="pushing"),
+            f"Successfully pushed {self.output_image_spec}",
+            extra=dict(phase=R2dState.PUSHING),
         )
 
     def run_image(self):
         """Run docker container from built image
 
         and wait for it to finish.
         """
@@ -589,54 +630,61 @@
         if docker_host:
             host_name = urlparse(docker_host).hostname
         else:
             host_name = "127.0.0.1"
         self.hostname = host_name
 
         if not self.run_cmd:
-            port = str(self._get_free_port())
-            self.port = port
+            if len(self.ports) == 1:
+                # single port mapping specified
+                # retrieve container and host port from dict
+                # {'8888/tcp': ('hostname', 'port')}
+                # or
+                # {'8888/tcp': 'port'}
+                container_port_proto, host_port = next(iter(self.ports.items()))
+                if isinstance(host_port, tuple):
+                    # (hostname, port) tuple or string port
+                    host_name, host_port = host_port
+                    self.hostname = host_name
+                host_port = int(host_port)
+                container_port = int(container_port_proto.split("/", 1)[0])
+            else:
+                # no port specified, pick a random one
+                container_port = host_port = str(self._get_free_port())
+                self.ports = {f"{container_port}/tcp": host_port}
+            self.port = host_port
             # To use the option --NotebookApp.custom_display_url
             # make sure the base-notebook image is updated:
             # docker pull jupyter/base-notebook
             run_cmd = [
                 "jupyter",
                 "notebook",
-                "--ip",
-                "0.0.0.0",
-                "--port",
-                port,
-                "--NotebookApp.custom_display_url=http://{}:{}".format(host_name, port),
+                "--ip=0.0.0.0",
+                f"--port={container_port}",
+                f"--NotebookApp.custom_display_url=http://{host_name}:{host_port}",
                 "--NotebookApp.default_url=/lab",
             ]
-            ports = {"%s/tcp" % port: port}
         else:
             # run_cmd given by user, if port is also given then pass it on
             run_cmd = self.run_cmd
-            if self.ports:
-                ports = self.ports
-            else:
-                ports = {}
-        # store ports on self so they can be retrieved in tests
-        self.ports = ports
 
         container_volumes = {}
         if self.volumes:
             image = client.inspect_image(self.output_image_spec)
             image_workdir = image.config["WorkingDir"]
 
             for k, v in self.volumes.items():
                 container_volumes[os.path.abspath(k)] = {
                     "bind": v if v.startswith("/") else os.path.join(image_workdir, v),
                     "mode": "rw",
                 }
 
         run_kwargs = dict(
             publish_all_ports=self.all_ports,
-            ports=ports,
+            ports=self.ports,
             command=run_cmd,
             volumes=container_volumes,
             environment=self.environment,
         )
 
         run_kwargs.update(self.extra_run_kwargs)
 
@@ -655,32 +703,35 @@
         """
 
         last_timestamp = None
         try:
             for line in container.logs(stream=True, timestamps=True):
                 line = line.decode("utf-8")
                 last_timestamp, line = line.split(" ", maxsplit=1)
-                self.log.info(line, extra=dict(phase="running"))
+                self.log.info(line, extra=dict(phase=R2dState.RUNNING))
 
         finally:
             container.reload()
             if container.status == "running":
-                self.log.info("Stopping container...\n", extra=dict(phase="running"))
+                self.log.info(
+                    "Stopping container...\n", extra=dict(phase=R2dState.RUNNING)
+                )
                 container.kill()
             exit_code = container.exitcode
 
             container.wait()
 
             self.log.info(
-                "Container finished running.\n".upper(), extra=dict(phase="running")
+                "Container finished running.\n".upper(),
+                extra=dict(phase=R2dState.RUNNING),
             )
             # are there more logs? Let's send them back too
             late_logs = container.logs(since=last_timestamp).decode("utf-8")
             for line in late_logs.split("\n"):
-                self.log.debug(line + "\n", extra=dict(phase="running"))
+                self.log.debug(line + "\n", extra=dict(phase=R2dState.RUNNING))
 
             container.remove()
             if exit_code:
                 sys.exit(exit_code)
 
     def _get_free_port(self):
         """
@@ -712,121 +763,131 @@
         Build docker image
         """
         # Check if r2d can connect to docker daemon
         if not self.dry_run:
             try:
                 docker_client = self.get_engine()
             except ContainerEngineException as e:
-                self.log.error("\nContainer engine initialization error: %s\n", e)
+                self.log.error(f"\nContainer engine initialization error: {e}\n")
                 self.exit(1)
 
         # If the source to be executed is a directory, continue using the
         # directory. In the case of a local directory, it is used as both the
         # source and target. Reusing a local directory seems better than
         # making a copy of it as it might contain large files that would be
         # expensive to copy.
         if os.path.isdir(self.repo):
+            # never cleanup when we are working in a local repo
+            self.cleanup_checkout = False
             checkout_path = self.repo
         else:
             if self.git_workdir is None:
                 checkout_path = tempfile.mkdtemp(prefix="repo2docker")
             else:
                 checkout_path = self.git_workdir
 
         try:
             self.fetch(self.repo, self.ref, checkout_path)
 
             if self.find_image():
                 self.log.info(
-                    "Reusing existing image ({}), not "
-                    "building.".format(self.output_image_spec)
+                    f"Reusing existing image ({self.output_image_spec}), not building."
                 )
                 # no need to build, so skip to the end by `return`ing here
                 # this will still execute the finally clause and let's us
                 # avoid having to indent the build code by an extra level
                 return
 
             if self.subdir:
                 checkout_path = os.path.join(checkout_path, self.subdir)
                 if not os.path.isdir(checkout_path):
                     self.log.error(
-                        "Subdirectory %s does not exist",
-                        self.subdir,
-                        extra=dict(phase="failure"),
+                        f"Subdirectory {self.subdir} does not exist",
+                        extra=dict(phase=R2dState.FAILED),
                     )
-                    raise FileNotFoundError("Could not find {}".format(checkout_path))
+                    raise FileNotFoundError(f"Could not find {checkout_path}")
 
             with chdir(checkout_path):
                 for BP in self.buildpacks:
-                    bp = BP()
+                    bp = BP(base_image=self.base_image)
                     if bp.detect():
                         picked_buildpack = bp
                         break
                 else:
-                    picked_buildpack = self.default_buildpack()
+                    picked_buildpack = self.default_buildpack(
+                        base_image=self.base_image
+                    )
 
+                picked_buildpack.platform = self.platform
                 picked_buildpack.appendix = self.appendix
                 # Add metadata labels
                 picked_buildpack.labels["repo2docker.version"] = self.version
                 repo_label = "local" if os.path.isdir(self.repo) else self.repo
                 picked_buildpack.labels["repo2docker.repo"] = repo_label
                 picked_buildpack.labels["repo2docker.ref"] = self.ref
 
                 picked_buildpack.labels.update(self.labels)
 
+                build_args = {
+                    "NB_USER": self.user_name,
+                    "NB_UID": str(self.user_id),
+                }
+                if self.target_repo_dir:
+                    build_args["REPO_DIR"] = self.target_repo_dir
+                build_args.update(self.extra_build_args)
+
                 if self.dry_run:
-                    print(picked_buildpack.render())
+                    print(picked_buildpack.render(build_args))
                 else:
                     self.log.debug(
-                        picked_buildpack.render(), extra=dict(phase="building")
+                        picked_buildpack.render(build_args),
+                        extra=dict(phase=R2dState.BUILDING),
                     )
                     if self.user_id == 0:
                         raise ValueError(
                             "Root as the primary user in the image is not permitted."
                         )
 
-                    build_args = {
-                        "NB_USER": self.user_name,
-                        "NB_UID": str(self.user_id),
-                    }
-                    if self.target_repo_dir:
-                        build_args["REPO_DIR"] = self.target_repo_dir
-                    build_args.update(self.extra_build_args)
-
                     self.log.info(
-                        "Using %s builder\n",
-                        bp.__class__.__name__,
-                        extra=dict(phase="building"),
+                        f"Using {bp.__class__.__name__} builder\n",
+                        extra=dict(phase=R2dState.BUILDING),
                     )
 
                     for l in picked_buildpack.build(
                         docker_client,
                         self.output_image_spec,
                         self.build_memory_limit,
                         build_args,
                         self.cache_from,
                         self.extra_build_kwargs,
+                        platform=self.platform,
                     ):
                         if docker_client.string_output:
-                            self.log.info(l, extra=dict(phase="building"))
+                            self.log.info(l, extra=dict(phase=R2dState.BUILDING))
                         # else this is Docker output
                         elif "stream" in l:
-                            self.log.info(l["stream"], extra=dict(phase="building"))
+                            self.log.info(
+                                l["stream"], extra=dict(phase=R2dState.BUILDING)
+                            )
                         elif "error" in l:
-                            self.log.info(l["error"], extra=dict(phase="failure"))
+                            self.log.info(l["error"], extra=dict(phase=R2dState.FAILED))
                             raise BuildError(l["error"])
                         elif "status" in l:
                             self.log.info(
-                                "Fetching base image...\r", extra=dict(phase="building")
+                                "Fetching base image...\r",
+                                extra=dict(phase=R2dState.BUILDING),
                             )
                         else:
-                            self.log.info(json.dumps(l), extra=dict(phase="building"))
+                            self.log.info(
+                                json.dumps(l), extra=dict(phase=R2dState.BUILDING)
+                            )
 
         finally:
             # Cleanup checkout if necessary
+            # never cleanup when checking out a local repo
             if self.cleanup_checkout:
                 shutil.rmtree(checkout_path, ignore_errors=True)
 
     def start(self):
         self.build()
 
         if self.push:
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/base.py` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,48 +1,50 @@
-import textwrap
-import jinja2
-import tarfile
+import hashlib
 import io
+import logging
 import os
 import re
-import logging
 import string
 import sys
-import hashlib
+import tarfile
+import textwrap
+from functools import lru_cache
+
 import escapism
+import jinja2
 
 # Only use syntax features supported by Docker 17.09
 TEMPLATE = r"""
-FROM buildpack-deps:bionic
+FROM {{base_image}}
 
 # Avoid prompts from apt
 ENV DEBIAN_FRONTEND=noninteractive
 
 # Set up locales properly
 RUN apt-get -qq update && \
     apt-get -qq install --yes --no-install-recommends locales > /dev/null && \
     apt-get -qq purge && \
     apt-get -qq clean && \
     rm -rf /var/lib/apt/lists/*
 
 RUN echo "en_US.UTF-8 UTF-8" > /etc/locale.gen && \
     locale-gen
 
-ENV LC_ALL en_US.UTF-8
-ENV LANG en_US.UTF-8
-ENV LANGUAGE en_US.UTF-8
+ENV LC_ALL=en_US.UTF-8 \
+    LANG=en_US.UTF-8 \
+    LANGUAGE=en_US.UTF-8
 
 # Use bash as default shell, rather than sh
-ENV SHELL /bin/bash
+ENV SHELL=/bin/bash
 
 # Set up user
 ARG NB_USER
 ARG NB_UID
-ENV USER ${NB_USER}
-ENV HOME /home/${NB_USER}
+ENV USER=${NB_USER} \
+    HOME=/home/${NB_USER}
 
 RUN groupadd \
         --gid ${NB_UID} \
         ${NB_USER} && \
     useradd \
         --comment "Default user" \
         --create-home \
@@ -77,21 +79,21 @@
 {% endif -%}
 
 EXPOSE 8888
 
 {% if build_env -%}
 # Environment variables required for build
 {% for item in build_env -%}
-ENV {{item[0]}} {{item[1]}}
+ENV {{item[0]}}={{item[1]}}
 {% endfor -%}
 {% endif -%}
 
 {% if path -%}
 # Special case PATH
-ENV PATH {{ ':'.join(path) }}:${PATH}
+ENV PATH={{ ':'.join(path) }}:${PATH}
 {% endif -%}
 
 {% if build_script_files -%}
 # If scripts required during build are present, copy them
 {% for src, dst in build_script_files|dictsort %}
 COPY --chown={{ user }}:{{ user }} {{ src }} {{ dst }}
 {% endfor -%}
@@ -101,32 +103,37 @@
 {{ sd }}
 {% endfor %}
 # ensure root user after build scripts
 USER root
 
 # Allow target path repo is cloned to be configurable
 ARG REPO_DIR=${HOME}
-ENV REPO_DIR ${REPO_DIR}
+ENV REPO_DIR=${REPO_DIR}
+# Create a folder and grant the user permissions if it doesn't exist
+RUN if [ ! -d "${REPO_DIR}" ]; then \
+        /usr/bin/install -o ${NB_USER} -g ${NB_USER} -d "${REPO_DIR}"; \
+    fi
+
 WORKDIR ${REPO_DIR}
 RUN chown ${NB_USER}:${NB_USER} ${REPO_DIR}
 
 # We want to allow two things:
 #   1. If there's a .local/bin directory in the repo, things there
 #      should automatically be in path
 #   2. postBuild and users should be able to install things into ~/.local/bin
 #      and have them be automatically in path
 #
 # The XDG standard suggests ~/.local/bin as the path for local user-specific
 # installs. See https://specifications.freedesktop.org/basedir-spec/basedir-spec-latest.html
-ENV PATH ${HOME}/.local/bin:${REPO_DIR}/.local/bin:${PATH}
+ENV PATH=${HOME}/.local/bin:${REPO_DIR}/.local/bin:${PATH}
 
 {% if env -%}
 # The rest of the environment
 {% for item in env -%}
-ENV {{item[0]}} {{item[1]}}
+ENV {{item[0]}}={{item[1]}}
 {% endfor -%}
 {% endif -%}
 
 # Run pre-assemble scripts! These are instructions that depend on the content
 # of the repository but don't access any files in the repository. By executing
 # them before copying the repository itself we can cache these steps. For
 # example installing APT packages.
@@ -140,15 +147,15 @@
 {% for sd in preassemble_script_directives -%}
 {{ sd }}
 {% endfor %}
 # ensure root user after preassemble scripts
 USER root
 
 # Copy stuff.
-COPY --chown={{ user }}:{{ user }} src/ ${REPO_DIR}
+COPY --chown={{ user }}:{{ user }} src/ ${REPO_DIR}/
 
 # Run assemble scripts! These will actually turn the specification
 # in the repository into an image.
 {% for sd in assemble_script_directives -%}
 {{ sd }}
 {% endfor %}
 
@@ -169,15 +176,15 @@
 RUN ./{{ s }}
 {% endfor %}
 {% endif -%}
 
 # Add start script
 {% if start_script is not none -%}
 RUN chmod +x "{{ start_script }}"
-ENV R2D_ENTRYPOINT "{{ start_script }}"
+ENV R2D_ENTRYPOINT="{{ start_script }}"
 {% endif -%}
 
 # Add entrypoint
 ENV PYTHONUNBUFFERED=1
 COPY /python3-login /usr/local/bin/python3-login
 COPY /repo2docker-entrypoint /usr/local/bin/repo2docker-entrypoint
 ENTRYPOINT ["/usr/local/bin/repo2docker-entrypoint"]
@@ -200,59 +207,68 @@
 class BuildPack:
     """
     A composable BuildPack.
 
     Specifically used for creating Dockerfiles for use with repo2docker only.
 
     Things that are kept constant:
-     - base image
      - some environment variables (such as locale)
      - user creation & ownership of home directory
      - working directory
 
     Everything that is configurable is additive & deduplicative,
     and there are *some* general guarantees of ordering.
 
     """
 
-    def __init__(self):
+    def __init__(self, base_image):
+        """
+        base_image specifies the base image to use when building docker images
+        """
         self.log = logging.getLogger("repo2docker")
         self.appendix = ""
+        self.base_image = base_image
         self.labels = {}
         if sys.platform.startswith("win"):
             self.log.warning(
                 "Windows environment detected. Note that Windows "
                 "support is experimental in repo2docker."
             )
+        self.platform = ""
 
+    @lru_cache()
     def get_packages(self):
         """
         List of packages that are installed in this BuildPack.
 
         Versions are not specified, and ordering is not guaranteed. These
         are usually installed as apt packages.
         """
         return set()
 
+    @lru_cache()
     def get_base_packages(self):
         """
         Base set of apt packages that are installed for all images.
 
         These contain useful images that are commonly used by a lot of images,
         where it would be useful to share a base docker image layer that
         contains them.
 
         These would be installed with a --no-install-recommends option.
         """
         return {
             # Utils!
             "less",
             "unzip",
+            # Gives us envsubst
+            "gettext-base",
         }
 
+    @lru_cache()
     def get_build_env(self):
         """
         Ordered list of environment variables to be set for this image.
 
         Ordered so that environment variables can use other environment
         variables in their values.
 
@@ -260,43 +276,47 @@
         name and the second item being the value.
 
         These environment variables will be set prior to build.
         Use .get_env() to set environment variables after build.
         """
         return []
 
+    @lru_cache()
     def get_env(self):
         """
         Ordered list of environment variables to be set for this image.
 
         Ordered so that environment variables can use other environment
         variables in their values.
 
         Expects tuples, with the first item being the environment variable
         name and the second item being the value.
 
         These variables will not be available to build.
         """
         return []
 
+    @lru_cache()
     def get_path(self):
         """
         Ordered list of file system paths to look for executables in.
 
         Just sets the PATH environment variable. Separated out since
         it is very commonly set by various buildpacks.
         """
         return []
 
+    @lru_cache()
     def get_labels(self):
         """
         Docker labels to set on the built image.
         """
         return self.labels
 
+    @lru_cache()
     def get_build_script_files(self):
         """
         Dict of files to be copied to the container image for use in building.
 
         This is copied before the `build_scripts` & `assemble_scripts` are
         run, so can be executed from either of them.
 
@@ -313,14 +333,15 @@
         """
         for root, dirs, files in os.walk("."):
             if "manifest.xml" in files:
                 self.log.error(
                     f"Found a stencila manifest.xml at {root}. Stencila is no longer supported."
                 )
 
+    @lru_cache()
     def get_build_scripts(self):
         """
         Ordered list of shell script snippets to build the base image.
 
         A list of tuples, where the first item is a username & the
         second is a single logical line of a bash script that should
         be RUN as that user.
@@ -334,27 +355,29 @@
 
         You can use environment variable substitutions in both the
         username and the execution script.
         """
 
         return []
 
+    @lru_cache()
     def get_preassemble_script_files(self):
         """
         Dict of files to be copied to the container image for use in preassembly.
 
         This is copied before the `build_scripts`, `preassemble_scripts` and
         `assemble_scripts` are run, so can be executed from either of them.
 
         It's a dictionary where the key is the source file path in the
         repository and the value is the destination file path inside the
         repository in the container.
         """
         return {}
 
+    @lru_cache()
     def get_preassemble_scripts(self):
         """
         Ordered list of shell snippets to build an image for this repository.
 
         A list of tuples, where the first item is a username & the
         second is a single logical line of a bash script that should
         be RUN as that user.
@@ -363,14 +386,15 @@
         the container image. These should be the scripts that depend on the
         repository but do not need access to the contents.
 
         For example the list of APT packages to install.
         """
         return []
 
+    @lru_cache()
     def get_assemble_scripts(self):
         """
         Ordered list of shell script snippets to build the repo into the image.
 
         A list of tuples, where the first item is a username & the
         second is a single logical line of a bash script that should
         be RUN as that user.
@@ -389,26 +413,28 @@
         dynamic detection.
 
         You can use environment variable substitutions in both the
         username and the execution script.
         """
         return []
 
+    @lru_cache()
     def get_post_build_scripts(self):
         """
         An ordered list of executable scripts to execute after build.
 
         Is run as a non-root user, and must be executable. Used for performing
         build time steps that can not be performed with standard tools.
 
         The scripts should be as deterministic as possible - running it twice
         should not produce different results!
         """
         return []
 
+    @lru_cache()
     def get_start_script(self):
         """
         The path to a script to be executed at container start up.
 
         This script is added as the `ENTRYPOINT` to the container.
 
         It is run as a non-root user, and must be executable. Used for
@@ -453,35 +479,35 @@
 
         t = jinja2.Template(TEMPLATE)
 
         build_script_directives = []
         last_user = "root"
         for user, script in self.get_build_scripts():
             if last_user != user:
-                build_script_directives.append("USER {}".format(user))
+                build_script_directives.append(f"USER {user}")
                 last_user = user
             build_script_directives.append(
                 "RUN {}".format(textwrap.dedent(script.strip("\n")))
             )
 
         assemble_script_directives = []
         last_user = "root"
         for user, script in self.get_assemble_scripts():
             if last_user != user:
-                assemble_script_directives.append("USER {}".format(user))
+                assemble_script_directives.append(f"USER {user}")
                 last_user = user
             assemble_script_directives.append(
                 "RUN {}".format(textwrap.dedent(script.strip("\n")))
             )
 
         preassemble_script_directives = []
         last_user = "root"
         for user, script in self.get_preassemble_scripts():
             if last_user != user:
-                preassemble_script_directives.append("USER {}".format(user))
+                preassemble_script_directives.append(f"USER {user}")
                 last_user = user
             preassemble_script_directives.append(
                 "RUN {}".format(textwrap.dedent(script.strip("\n")))
             )
 
         # Based on a physical location of a build script on the host,
         # create a mapping between:
@@ -510,14 +536,15 @@
             build_script_files=build_script_files,
             base_packages=sorted(self.get_base_packages()),
             post_build_scripts=self.get_post_build_scripts(),
             start_script=self.get_start_script(),
             appendix=self.appendix,
             # For docker 17.09 `COPY --chown`, 19.03 would allow using $NBUSER
             user=build_args.get("NB_UID", DEFAULT_NB_UID),
+            base_image=self.base_image,
         )
 
     @staticmethod
     def generate_build_context_filename(src_path, hash_length=6):
         """
         Generate a filename for a file injected into the Docker build context.
 
@@ -549,14 +576,15 @@
         self,
         client,
         image_spec,
         memory_limit,
         build_args,
         cache_from,
         extra_build_kwargs,
+        platform=None,
     ):
         tarf = io.BytesIO()
         tar = tarfile.open(fileobj=tarf, mode="w")
         dockerfile_tarinfo = tarfile.TarInfo("Dockerfile")
         dockerfile = self.render(build_args).encode("utf-8")
         dockerfile_tarinfo.size = len(dockerfile)
 
@@ -585,16 +613,16 @@
         tar.close()
         tarf.seek(0)
 
         # If you work on this bit of code check the corresponding code in
         # buildpacks/docker.py where it is duplicated
         if not isinstance(memory_limit, int):
             raise ValueError(
-                "The memory limit has to be specified as an"
-                "integer but is '{}'".format(type(memory_limit))
+                "The memory limit has to be specified as an "
+                f"integer but is '{type(memory_limit)}'"
             )
         limits = {}
         if memory_limit:
             # We want to always disable swap. Docker expects `memswap` to
             # be total allowable memory, *including* swap - while `memory`
             # points to non-swap memory. We set both values to the same so
             # we use no swap.
@@ -603,52 +631,54 @@
         build_kwargs = dict(
             fileobj=tarf,
             tag=image_spec,
             custom_context=True,
             buildargs=build_args,
             container_limits=limits,
             cache_from=cache_from,
+            platform=platform,
         )
 
         build_kwargs.update(extra_build_kwargs)
 
-        for line in client.build(**build_kwargs):
-            yield line
+        yield from client.build(**build_kwargs)
 
 
 class BaseImage(BuildPack):
+    @lru_cache()
     def get_build_env(self):
         """Return env directives required for build"""
         return [
             ("APP_BASE", "/srv"),
         ]
 
+    @lru_cache()
     def get_env(self):
         """Return env directives to be set after build"""
         return []
 
     def detect(self):
         return True
 
+    @lru_cache()
     def get_preassemble_scripts(self):
         scripts = []
         try:
             with open(self.binder_path("apt.txt")) as f:
                 extra_apt_packages = []
                 for l in f:
                     package = l.partition("#")[0].strip()
                     if not package:
                         continue
                     # Validate that this is, indeed, just a list of packages
                     # We're doing shell injection around here, gotta be careful.
                     # FIXME: Add support for specifying version numbers
                     if not re.match(r"^[a-z0-9.+-]+", package):
                         raise ValueError(
-                            "Found invalid package name {} in "
-                            "apt.txt".format(package)
+                            f"Found invalid package name {package} in apt.txt"
                         )
                     extra_apt_packages.append(package)
 
             scripts.append(
                 (
                     "root",
                     # This apt-get install is *not* quiet, since users explicitly asked for this
@@ -665,24 +695,27 @@
             )
 
         except FileNotFoundError:
             pass
 
         return scripts
 
+    @lru_cache()
     def get_assemble_scripts(self):
         """Return directives to run after the entire repository has been added to the image"""
         return []
 
+    @lru_cache()
     def get_post_build_scripts(self):
         post_build = self.binder_path("postBuild")
         if os.path.exists(post_build):
             return [post_build]
         return []
 
+    @lru_cache()
     def get_start_script(self):
         start = self.binder_path("start")
         if os.path.exists(start):
             # Return an absolute path to start
             # This is important when built container images start with
             # a working directory that is different from ${REPO_DIR}
             # This isn't a problem with anything else, since start is
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/__init__.py` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 """BuildPack for conda environments"""
 import os
 import re
+import warnings
 from collections.abc import Mapping
+from functools import lru_cache
 
 from ruamel.yaml import YAML
 
-from ..base import BaseImage
-from .._r_base import rstudio_base_scripts
+from ...semver import parse_version as V
 from ...utils import is_local_pip_requirement
+from .._r_base import rstudio_base_scripts
+from ..base import BaseImage
 
 # pattern for parsing conda dependency line
 PYTHON_REGEX = re.compile(r"python\s*=+\s*([\d\.]*)")
 R_REGEX = re.compile(r"r-base\s*=+\s*([\d\.]*)")
 # current directory
 HERE = os.path.dirname(os.path.abspath(__file__))
 
@@ -31,14 +34,23 @@
 
     # The notebook server environment file.
     # As an absolute path within the container.
     _nb_environment_file = ""
     # extra pip requirements.txt for the notebook env
     _nb_requirements_file = ""
 
+    def _conda_platform(self):
+        """Return the conda platform name for the current platform"""
+        if self.platform == "linux/amd64":
+            return "linux-64"
+        if self.platform == "linux/arm64":
+            return "linux-aarch64"
+        raise ValueError(f"Unknown platform {self.platform}")
+
+    @lru_cache()
     def get_build_env(self):
         """Return environment variables to be set.
 
         We set `CONDA_DIR` to the conda install directory and
         the `NB_PYTHON_PREFIX` to the location of the jupyter binary.
 
         """
@@ -55,14 +67,15 @@
             ("NPM_DIR", "${APP_BASE}/npm"),
             ("NPM_CONFIG_GLOBALCONFIG", "${NPM_DIR}/npmrc"),
             ("NB_ENVIRONMENT_FILE", self._nb_environment_file),
             ("MAMBA_ROOT_PREFIX", "${CONDA_DIR}"),
             # this exe should be used for installs after bootstrap with micromamba
             # switch this to /usr/local/bin/micromamba to use it for all installs
             ("MAMBA_EXE", "${CONDA_DIR}/bin/mamba"),
+            ("CONDA_PLATFORM", self._conda_platform()),
         ]
         if self._nb_requirements_file:
             env.append(("NB_REQUIREMENTS_FILE", self._nb_requirements_file))
 
         if self._kernel_environment_file:
             # if kernel environment file is separate
             env.extend(
@@ -73,33 +86,36 @@
             )
             if self._kernel_requirements_file:
                 env.append(("KERNEL_REQUIREMENTS_FILE", self._kernel_requirements_file))
         else:
             env.append(("KERNEL_PYTHON_PREFIX", "${NB_PYTHON_PREFIX}"))
         return env
 
+    @lru_cache()
     def get_env(self):
         """Make kernel env the default for `conda install`"""
         env = super().get_env() + [("CONDA_DEFAULT_ENV", "${KERNEL_PYTHON_PREFIX}")]
         return env
 
+    @lru_cache()
     def get_path(self):
         """Return paths (including conda environment path) to be added to
         the PATH environment variable.
 
         """
         path = super().get_path()
         path.insert(0, "${CONDA_DIR}/bin")
-        if self.py2:
+        if self.separate_kernel_env:
             path.insert(0, "${KERNEL_PYTHON_PREFIX}/bin")
         path.insert(0, "${NB_PYTHON_PREFIX}/bin")
         # This is at the end of $PATH, for backwards compat reasons
         path.append("${NPM_DIR}/bin")
         return path
 
+    @lru_cache()
     def get_build_scripts(self):
         """
         Return series of build-steps common to all Python 3 repositories.
 
         All scripts here should be independent of contents of the repository.
 
         This sets up through `install-base-env.bash` (found in this directory):
@@ -107,15 +123,14 @@
         - a directory for the conda environment and its ownership by the
           notebook user
         - a Python 3 interpreter for the conda environment
         - a Python 3 jupyter kernel
         - a frozen base set of requirements, including:
             - support for Jupyter widgets
             - support for JupyterLab
-            - support for nteract
 
         """
         return super().get_build_scripts() + [
             (
                 "root",
                 r"""
                 TIMEFORMAT='time: %3R' \
@@ -128,16 +143,17 @@
                 r"""
                 mkdir -p ${NPM_DIR} && \
                 chown -R ${NB_USER}:${NB_USER} ${NPM_DIR}
                 """,
             ),
         ]
 
-    major_pythons = {"2": "2.7", "3": "3.7"}
+    major_pythons = {"2": "2.7", "3": "3.10"}
 
+    @lru_cache()
     def get_build_script_files(self):
         """
         Dict of files to be copied to the container image for use in building.
 
         This is copied before the `build_scripts` & `assemble_scripts` are
         run, so can be executed from either of them.
 
@@ -150,44 +166,62 @@
 
         """
         files = {
             "conda/install-base-env.bash": "/tmp/install-base-env.bash",
             "conda/activate-conda.sh": "/etc/profile.d/activate-conda.sh",
         }
         py_version = self.python_version
-        self.log.info("Building conda environment for python=%s" % py_version)
+        if not py_version or len(py_version.split(".")) != 2:
+            raise ValueError(
+                f"{self.__class__.__name__}.python_version must always be specified as 'x.y', e.g. '3.10', got {py_version}."
+            )
+        self.log.info(f"Building conda environment for python={py_version}\n")
         # Select the frozen base environment based on Python version.
         # avoids expensive and possibly conflicting upgrades when changing
         # major Python versions during upgrade.
-        # If no version is specified or no matching X.Y version is found,
-        # the default base environment is used.
-        frozen_name = "environment.lock"
-        pip_frozen_name = "requirements.txt"
-        if py_version:
-            if self.py2:
-                # python 2 goes in a different env
+        conda_platform = self._conda_platform()
+
+        if self.separate_kernel_env:
+            # setup kernel environment (separate from server)
+            # server runs with default env
+            server_py_version = self.major_pythons["3"]
+            self.log.warning(
+                f"User-requested packages for legacy Python version {py_version} will be installed in a separate kernel environment in $KERNEL_PYTHON_PREFIX.\n"
+                f"Jupyter Server will run with {server_py_version} in $NB_PYTHON_PREFIX.\n"
+            )
+            lockfile_name = f"environment.py-{py_version}-{conda_platform}.lock"
+            if not os.path.exists(os.path.join(HERE, lockfile_name)):
+                raise ValueError(
+                    f"Python version {py_version} on {conda_platform} is not supported!"
+                )
+            files[
+                f"conda/{lockfile_name}"
+            ] = self._kernel_environment_file = "/tmp/env/kernel-environment.lock"
+
+            requirements_file_name = f"requirements.py-{py_version}.pip"
+            if os.path.exists(os.path.join(HERE, requirements_file_name)):
                 files[
-                    "conda/environment.py-2.7.lock"
-                ] = self._kernel_environment_file = "/tmp/env/kernel-environment.lock"
-                # additional pip requirements for kernel env
-                if os.path.exists(os.path.join(HERE, "requirements.py-2.7.txt")):
-                    files[
-                        "conda/requirements.py-2.7.txt"
-                    ] = (
-                        self._kernel_requirements_file
-                    ) = "/tmp/env/kernel-requirements.txt"
-            else:
-                py_frozen_name = f"environment.py-{py_version}.lock"
-                if os.path.exists(os.path.join(HERE, py_frozen_name)):
-                    frozen_name = py_frozen_name
-                    pip_frozen_name = f"requirements.py-{py_version}.pip"
-                if not frozen_name:
-                    self.log.warning(f"No frozen env for {py_version}")
+                    f"conda/{requirements_file_name}"
+                ] = self._kernel_requirements_file = "/tmp/env/kernel-requirements.txt"
+        else:
+            # server and kernel are the same
+            server_py_version = py_version
+
+        # setup the server Python environment
+        conda_frozen_name = f"environment.py-{server_py_version}-{conda_platform}.lock"
+        pip_frozen_name = f"requirements.py-{server_py_version}.pip"
+
+        if not os.path.exists(os.path.join(HERE, conda_frozen_name)):
+            # no env, not supported
+            raise ValueError(
+                f"Python version {server_py_version} on {conda_platform} is not supported!"
+            )
+
         files[
-            "conda/" + frozen_name
+            "conda/" + conda_frozen_name
         ] = self._nb_environment_file = "/tmp/env/environment.lock"
 
         # add requirements.txt, if present
         if os.path.exists(os.path.join(HERE, pip_frozen_name)):
             files[
                 "conda/" + pip_frozen_name
             ] = self._nb_requirements_file = "/tmp/env/requirements.txt"
@@ -239,16 +273,17 @@
                     return False
         return True
 
     @property
     def python_version(self):
         """Detect the Python version for a given `environment.yml`
 
-        Will return 'x.y' if version is found (e.g '3.6'),
-        or a Falsy empty string '' if not found.
+        Will always return an `x.y` version.
+        If no version is found, the default Python version is used,
+        via self.major_pythons['3'].
 
         Version information below the minor level is dropped.
         """
         if not hasattr(self, "_python_version"):
             py_version = None
             env = self.environment_yaml
             for dep in env.get("dependencies", []):
@@ -258,21 +293,25 @@
                 if not match:
                     continue
                 py_version = match.group(1)
                 break
 
             # extract major.minor
             if py_version:
-                if len(py_version) == 1:
-                    self._python_version = self.major_pythons.get(py_version[0])
+                py_version_info = py_version.split(".")
+                if len(py_version_info) == 1:
+                    self._python_version = self.major_pythons[py_version_info[0]]
                 else:
                     # return major.minor
-                    self._python_version = ".".join(py_version.split(".")[:2])
+                    self._python_version = ".".join(py_version_info[:2])
             else:
-                self._python_version = ""
+                self._python_version = self.major_pythons["3"]
+                self.log.warning(
+                    f"Python version unspecified, using current default Python version {self._python_version}. This will change in the future."
+                )
 
         return self._python_version
 
     @property
     def r_version(self):
         """Detect the R version for a given `environment.yml`
 
@@ -311,100 +350,123 @@
                     break
 
         return self._uses_r
 
     @property
     def py2(self):
         """Am I building a Python 2 kernel environment?"""
+        warnings.warn(
+            "CondaBuildPack.py2 is deprecated in 2023.2. Use CondaBuildPack.separate_kernel_env.",
+            DeprecationWarning,
+            stacklevel=2,
+        )
         return self.python_version and self.python_version.split(".")[0] == "2"
 
+    # Python versions _older_ than this get a separate kernel env
+    kernel_env_cutoff_version = "3.7"
+
+    @property
+    def separate_kernel_env(self):
+        """Whether the kernel should be installed into a separate env from the server
+
+        Applies to older versions of Python that aren't kept up-to-date
+        """
+        return self.python_version and V(self.python_version) < V(
+            self.kernel_env_cutoff_version
+        )
+
+    @lru_cache()
     def get_preassemble_script_files(self):
         """preassembly only requires environment.yml
 
         enables caching assembly result even when
         repo contents change
         """
         assemble_files = super().get_preassemble_script_files()
         if self._should_preassemble_env:
             environment_yml = self.binder_path("environment.yml")
             if os.path.exists(environment_yml):
                 assemble_files[environment_yml] = environment_yml
         return assemble_files
 
+    @lru_cache()
     def get_env_scripts(self):
         """Return series of build-steps specific to this source repository."""
         scripts = []
         environment_yml = self.binder_path("environment.yml")
-        env_prefix = "${KERNEL_PYTHON_PREFIX}" if self.py2 else "${NB_PYTHON_PREFIX}"
+        env_prefix = (
+            "${KERNEL_PYTHON_PREFIX}"
+            if self.separate_kernel_env
+            else "${NB_PYTHON_PREFIX}"
+        )
         if os.path.exists(environment_yml):
             # TODO: when using micromamba, we call $MAMBA_EXE install -p ...
             # whereas mamba/conda need `env update -p ...` when it's an env.yaml file
             scripts.append(
                 (
                     "${NB_USER}",
-                    r"""
+                    rf"""
                 TIMEFORMAT='time: %3R' \
-                bash -c 'time ${{MAMBA_EXE}} env update -p {0} --file "{1}" && \
+                bash -c 'time ${{MAMBA_EXE}} env update -p {env_prefix} --file "{environment_yml}" && \
                 time ${{MAMBA_EXE}} clean --all -f -y && \
-                ${{MAMBA_EXE}} list -p {0} \
+                ${{MAMBA_EXE}} list -p {env_prefix} \
                 '
-                """.format(
-                        env_prefix, environment_yml
-                    ),
+                """,
                 )
             )
 
         if self.uses_r:
             if self.r_version:
                 r_pin = "=" + self.r_version
             else:
                 r_pin = ""
             scripts.append(
                 (
                     "${NB_USER}",
-                    r"""
-                ${{MAMBA_EXE}} install -p {0} r-base{1} r-irkernel=1.2 r-devtools -y && \
+                    rf"""
+                ${{MAMBA_EXE}} install -p {env_prefix} r-base{r_pin} r-irkernel r-devtools -y && \
                 ${{MAMBA_EXE}} clean --all -f -y && \
-                ${{MAMBA_EXE}} list -p {0}
-                """.format(
-                        env_prefix, r_pin
-                    ),
+                ${{MAMBA_EXE}} list -p {env_prefix}
+                """,
                 )
             )
+            if self.platform != "linux/amd64":
+                raise RuntimeError(
+                    f"RStudio is only available for linux/amd64 ({self.platform})"
+                )
             scripts += rstudio_base_scripts(self.r_version)
             scripts += [
                 (
                     "root",
-                    r"""
+                    rf"""
                     echo auth-none=1 >> /etc/rstudio/rserver.conf && \
                     echo auth-minimum-user-id=0 >> /etc/rstudio/rserver.conf && \
-                    echo "rsession-which-r={0}/bin/R" >> /etc/rstudio/rserver.conf && \
+                    echo "rsession-which-r={env_prefix}/bin/R" >> /etc/rstudio/rserver.conf && \
+                    echo "rsession-ld-library-path={env_prefix}/lib" >> /etc/rstudio/rserver.conf && \
                     echo www-frame-origin=same >> /etc/rstudio/rserver.conf
-                    """.format(
-                        env_prefix
-                    ),
+                    """,
                 ),
                 (
                     "${NB_USER}",
-                    # Install a pinned version of IRKernel and set it up for use!
-                    r"""
-                 R --quiet -e "IRkernel::installspec(prefix='{0}')"
-                 """.format(
-                        env_prefix
-                    ),
+                    # Register the jupyter kernel
+                    rf"""
+                 R --quiet -e "IRkernel::installspec(prefix='{env_prefix}')"
+                 """,
                 ),
             ]
         return scripts
 
+    @lru_cache()
     def get_preassemble_scripts(self):
         scripts = super().get_preassemble_scripts()
         if self._should_preassemble_env:
             scripts.extend(self.get_env_scripts())
         return scripts
 
+    @lru_cache()
     def get_assemble_scripts(self):
         scripts = super().get_assemble_scripts()
         if not self._should_preassemble_env:
             scripts.extend(self.get_env_scripts())
         return scripts
 
     def detect(self):
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/activate-conda.sh` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/activate-conda.sh`

 * *Files identical despite different names*

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.lock` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.11-linux-64.lock`

 * *Files 12% similar despite different names*

```diff
@@ -1,140 +1,168 @@
-# AUTO GENERATED FROM environment.py-3.7.yml, DO NOT MANUALLY MODIFY
-# Frozen on 2022-01-26 18:35:40 UTC
+# AUTO GENERATED FROM environment.py-3.11.yml, DO NOT MANUALLY MODIFY
+# Frozen on 2023-06-08 09:35:47 UTC
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 8daa45fe7e84c647f0c5ab04c1199514abe3834c110cffac7bd4a18cc5375472
+# input_hash: 3896c7e12b9461937f193ac022a4426948268f5b348da74e57eeacea703149a4
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
-https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2021.10.8-ha878542_0.tar.bz2#575611b8a84f45960e87722eeb51fa26
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.36.1-hea4e1c9_2.tar.bz2#bd4f2e711b39af170e7ff15163fe87ee
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-11.2.0-he4da1e4_12.tar.bz2#7ff3b832ba5e6918c0d026976359d065
-https://conda.anaconda.org/conda-forge/linux-64/pandoc-2.17.0.1-h7f98852_0.tar.bz2#bd9fa82641da6dfe5696fd196e3c7cf1
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-11.2.0-h1d223b6_12.tar.bz2#763c5ec8116d984b4a33342236d7da36
-https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-1_gnu.tar.bz2#561e277319a41d4f24f5c05a9ef63c04
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-11.2.0-h1d223b6_12.tar.bz2#d34efbb8d7d6312c816b4bb647b818b1
-https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.18.1-h7f98852_0.tar.bz2#f26ef8098fab1f719c91eb760d63381a
-https://conda.anaconda.org/conda-forge/linux-64/icu-69.1-h9c3ff4c_0.tar.bz2#e0773c9556d588b062a4e1424a6a02fa
-https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
+https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
+https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.11-3_cp311.conda#c2e2630ddb68cf52eec74dc7dfab20b5
+https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
+https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
+https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
+https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
+https://conda.anaconda.org/conda-forge/linux-64/libexpat-2.5.0-hcb278e6_1.conda#6305a3dd2752c76335295da4e581f2fd
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
-https://conda.anaconda.org/conda-forge/linux-64/libuv-1.43.0-h7f98852_0.tar.bz2#b34d856aa7e06ebd79bded72ef4afc16
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.11-h36c2ea0_1013.tar.bz2#dcddf696ff5dfcab567100d691678e18
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h9c3ff4c_0.tar.bz2#fb31bcb7af058244479ca635d20f0f4a
-https://conda.anaconda.org/conda-forge/linux-64/openssl-1.1.1l-h7f98852_0.tar.bz2#de7b38a1542dbe6f41653a8ae71adc53
-https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.5-h516909a_1.tar.bz2#33f601066901f3e1a85af3522a8113f9
-https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
-https://conda.anaconda.org/conda-forge/linux-64/readline-8.1-h46c0cb4_0.tar.bz2#5788de3c8d7a7d64ac56c784c4ef48e6
+https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
+https://conda.anaconda.org/conda-forge/linux-64/libuv-1.44.2-h166bdaf_0.tar.bz2#e5cb4fe581a18ca2185a016eb848fc00
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
+https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
+https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
+https://conda.anaconda.org/conda-forge/linux-64/pandoc-2.19.2-h32600fe_2.conda#326f46f36d15c44cff5f81d505cb717f
+https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
+https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.11-h36c2ea0_1013.tar.bz2#cf7190238072a41e9579e4476a6a60b8
-https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.43.0-h812cca2_1.tar.bz2#d0a7846b7b3b8fb0d8b36904a53b8155
-https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.10.0-ha56f1ee_2.tar.bz2#6ab4eaa11ff01801cffca0a27489dc04
-https://conda.anaconda.org/conda-forge/linux-64/nodejs-14.18.3-h8ca31f7_2.tar.bz2#192a478a1ae899992e4afce84520badb
-https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.37.0-h9cd32fc_0.tar.bz2#eb66fc098824d25518a79e83d12a81d6
-https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.11-h27826a3_1.tar.bz2#84e76fb280e735fec1efd2d21fd9cb27
-https://conda.anaconda.org/conda-forge/linux-64/krb5-1.19.2-hcc1bbae_3.tar.bz2#e29650992ae593bc05fc93722483e5c3
-https://conda.anaconda.org/conda-forge/linux-64/python-3.7.12-hb7a2778_100_cpython.tar.bz2#2d94b3e6a9fdaf83f6955d008c8011a7
+https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-h166bdaf_4.tar.bz2#4b11e365c0275b808be78b30f904e295
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.15.0-h4abf6b9_1.conda#2aabafd88f6876a57c45c00598715ac4
+https://conda.anaconda.org/conda-forge/linux-64/python-3.11.3-h2755cc3_0_cpython.conda#37005ea5f68df6a8a381b70cf4d4a160
+https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
 https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
-https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
+https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
-https://conda.anaconda.org/conda-forge/noarch/backports-1.0-py_2.tar.bz2#0da16b293affa6ac31812376f8eb79dd
-https://conda.anaconda.org/conda-forge/noarch/blinker-1.4-py_1.tar.bz2#fa509a09190583f869ae442bf4d17f5f
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.0.10-pyhd8ed1ab_0.tar.bz2#ea77236c8031cfa821720b21b4cb0ceb
+https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
+https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda#2fb79ec81bad9492b6d59a06b3b647a4
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
+https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
+https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py311hcafe171_0.conda#f4c810ad9d791c8df5ad900ed74b085b
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.3-pyhd8ed1ab_1003.tar.bz2#bbf9a201f6ce99a506f4955374d9a9f4
-https://conda.anaconda.org/conda-forge/noarch/flit-core-3.6.0-pyhd8ed1ab_0.tar.bz2#f8c17f22a3ce533876c468157ff8ff8f
-https://conda.anaconda.org/conda-forge/noarch/idna-3.3-pyhd8ed1ab_0.tar.bz2#40b50b8b030f5f2f22085c062ed013dd
+https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
+https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
+https://conda.anaconda.org/conda-forge/linux-64/greenlet-2.0.2-py311hb755f60_1.conda#82f9885f18cc7ba9bca6687ac97f1d65
+https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-1.0.2-pyhd8ed1ab_0.tar.bz2#eaff56fe28d1236076aa3bb13c35b434
-https://conda.anaconda.org/conda-forge/linux-64/libcurl-7.81.0-h2574ce0_0.tar.bz2#1f8655741d0269ca6756f131522da1e8
-https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.4-pyhd8ed1ab_0.tar.bz2#0d86e4e6ac78912f3f47e0453b124aca
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py311h459d7ec_0.conda#9904dc4adb5d547cb21e136f98cb24b0
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
+https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pamela-1.0.0-py_0.tar.bz2#36f6f18d2f3ae0c93d77a9dbedad08c3
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.13.0-pyhd8ed1ab_0.tar.bz2#f5567b5e7a5abc9133f198b8356674d1
+https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py311h2582759_0.conda#a90f8e278c1cd7064b2713e6b7db87e6
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
+https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
-https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.3.0-pyhd8ed1ab_1.tar.bz2#b7bc0de380f114658af5fe57cebdcd9e
-https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.7-pyhd8ed1ab_0.tar.bz2#727e2216d9c47455d8ddc060eb2caad9
-https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.1-pyh9f0ad1d_0.tar.bz2#aed452f2f9f8bc8b2b0c412975051b5b
-https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.7-2_cp37m.tar.bz2#afff88bf9a7048da740c70aeb8cdbb82
-https://conda.anaconda.org/conda-forge/noarch/pytz-2021.3-pyhd8ed1ab_0.tar.bz2#7e4f811bff46a5a6a7e0094921389395
-https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.0-pyhd8ed1ab_0.tar.bz2#edab14119efe85c3bf131ad747e9005c
+https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.7.0-pyhd8ed1ab_0.conda#99e28be5a278e2319834d7dc99e7bfdd
+https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py311h2582759_0.conda#e53876b66dcc4ba8a0afa63cd8502ac3
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
+https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
+https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
+https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
+https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py311hd4cff14_5.tar.bz2#da8769492e423103c59f469f4f17f8d9
+https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py311h75c88c4_0.conda#db94a7a9e865fbfde8c023b6e8958bb2
+https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
+https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py311h2582759_1.conda#5e997292429a22ad50c11af0a2cb0f08
+https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
-https://conda.anaconda.org/conda-forge/noarch/testpath-0.5.0-pyhd8ed1ab_0.tar.bz2#53b57d6a468bebc7cef1253b177a5e9e
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.1.1-pyhd8ed1ab_0.tar.bz2#a1bc9765ef9499760e88f568b3a6622c
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.0.1-pyha770c72_0.tar.bz2#1fc03816925d3cb7fdab9ab234e7fea7
+https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
+https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
+https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
+https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py311h459d7ec_0.conda#12b1c374ee90a1aa11ea921858394dc8
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.2.3-pyhd8ed1ab_0.tar.bz2#a9e89668df0da0f33c8c4ddf7c118f6d
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.37.1-pyhd8ed1ab_0.tar.bz2#1ca02aaf78d9c70d9a81a3bed5752022
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.7.0-pyhd8ed1ab_0.tar.bz2#947f7f41958eabc0f6e886557512bb76
-https://conda.anaconda.org/conda-forge/noarch/babel-2.9.1-pyh44b312d_0.tar.bz2#74136ed39bfea0832d338df1e58d013e
-https://conda.anaconda.org/conda-forge/linux-64/certifi-2021.10.8-py37h89c1867_1.tar.bz2#48e8442b6097c7d4a0e3494c74ff9eeb
-https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.0-py37h036bc23_0.tar.bz2#05ab26c7685bcb7dd8bc8752c121f823
-https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.5.1-py37hcd2ae1e_0.tar.bz2#739a721301e47f42998af7bd51f0c42c
-https://conda.anaconda.org/conda-forge/linux-64/greenlet-1.1.2-py37hcd2ae1e_1.tar.bz2#f39576dbfb9a1067293d24f0e3b6bdda
-https://conda.anaconda.org/conda-forge/linux-64/importlib-metadata-4.10.1-py37h89c1867_0.tar.bz2#4684501699ad9eccbc29fa694d5343fc
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.4.0-pyhd8ed1ab_0.tar.bz2#9fb134dbabe7851a9d71411064b2c30d
-https://conda.anaconda.org/conda-forge/linux-64/jedi-0.18.1-py37h89c1867_0.tar.bz2#432446f7c13e1babe6bc05ba74d30f64
-https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-4.9.1-py37h89c1867_1.tar.bz2#95df6ebc6f4e8edd5d87aa99c59da605
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.0.1-py37h5e8e339_1.tar.bz2#6c7c14c95d4c435b66261639b64c7c51
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.3-pyhd8ed1ab_0.tar.bz2#be3bfd435802d2c768c6b2439f325f3d
-https://conda.anaconda.org/conda-forge/linux-64/mistune-0.8.4-py37h5e8e339_1005.tar.bz2#2dd7bedc3ea33c30cb9dcf93d64c10eb
-https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2#71f1ab2de48613876becddd496371c85
-https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh9f0ad1d_2.tar.bz2#5909e7b978141dd80d28dbf9de627827
-https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.0-py37h5e8e339_0.tar.bz2#009832a45a0d9240aa3f3329055da1ef
-https://conda.anaconda.org/conda-forge/linux-64/pycurl-7.44.1-py37h88a64d2_1.tar.bz2#4e4c43ae76df275f09cffc5e63ae936d
-https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.18.1-py37h5e8e339_0.tar.bz2#f7e31f8bb6c8b311c3842c090a440e3d
-https://conda.anaconda.org/conda-forge/linux-64/pysocks-1.7.1-py37h89c1867_4.tar.bz2#44df88d27e2891f90e3f06dcfcca0927
-https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/linux-64/pyzmq-22.3.0-py37h336d617_1.tar.bz2#6512cf886a870090430e2f37f41b652e
-https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.6-py37h5e8e339_0.tar.bz2#70ee31b43817f9fb7a46f76db99af94b
-https://conda.anaconda.org/conda-forge/linux-64/setuptools-60.5.0-py37h89c1867_0.tar.bz2#8d99eb0fa9aaae9dddb6a91451ac7907
-https://conda.anaconda.org/conda-forge/linux-64/sniffio-1.2.0-py37h89c1867_2.tar.bz2#464124f171b89cb9b459f47f81cc0e84
-https://conda.anaconda.org/conda-forge/linux-64/tornado-6.1-py37h5e8e339_2.tar.bz2#ec86ae00c96dea5f2d810957a8fabc26
-https://conda.anaconda.org/conda-forge/linux-64/anyio-3.5.0-py37h89c1867_0.tar.bz2#aa263b5829ec141d12bf6a5dec36bf5b
-https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py37h5e8e339_1.tar.bz2#042ff84df84e01a6399caa379deaf044
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/linux-64/y-py-0.5.9-py311hfe55011_0.conda#216fb67bd1016b05fe33672bd71937a8
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
+https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
+https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
-https://conda.anaconda.org/conda-forge/noarch/bleach-4.1.0-pyhd8ed1ab_0.tar.bz2#4a2104c7b22c222bd0fe03aaef12862c
-https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py37h5e8e339_1003.tar.bz2#4ad2e74470a3c08b0f6d59699f0d9a32
-https://conda.anaconda.org/conda-forge/linux-64/cryptography-36.0.1-py37hf1a17b8_0.tar.bz2#7ad2c98aaab85d80017b3a6f79a2aa5d
-https://conda.anaconda.org/conda-forge/noarch/jinja2-3.0.3-pyhd8ed1ab_0.tar.bz2#036d872c653780cb26e797e2e2f61b4c
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.4.0-pyhd8ed1ab_0.tar.bz2#17ec41acce882e5db4efdcc4c01ca7e0
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-7.1.2-pyhd8ed1ab_0.tar.bz2#9a332b6f8f05629435ce59032df8cfa9
-https://conda.anaconda.org/conda-forge/noarch/mako-1.1.6-pyhd8ed1ab_0.tar.bz2#cb952a55037148f6a5ddd9770ee1384f
-https://conda.anaconda.org/conda-forge/noarch/pip-21.3.1-pyhd8ed1ab_0.tar.bz2#e4fe2a9af78ff11f1aced7e62128c6a8
-https://conda.anaconda.org/conda-forge/noarch/pygments-2.11.2-pyhd8ed1ab_0.tar.bz2#caef60540e2239e27bf62569a5015e3b
-https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.19-py37h5e8e339_0.tar.bz2#a909957daac2e6296ce9219940481e1d
-https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-1.4.31-py37h5e8e339_0.tar.bz2#8c316b01e34dea00fe526456be12fae4
-https://conda.anaconda.org/conda-forge/linux-64/terminado-0.12.1-py37h89c1867_1.tar.bz2#658fe17f1a35117ebfb063f3b023c884
-https://conda.anaconda.org/conda-forge/noarch/alembic-1.7.5-pyhd8ed1ab_0.tar.bz2#1102908123392ffc63c01caea136b1d4
+https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
+https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
+https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py311h409f033_3.conda#9025d0786dbbe4bc91fd8e85502decce
+https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
+https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
+https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
+https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
+https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.31-py311h459d7ec_0.conda#f0fc1409f49257fe5ec2d86d0595d9bc
+https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_0.conda#ae465d0fbf9f1979cb2d8d4043d885e2
+https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
+https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py311hd4cff14_3.tar.bz2#5159e874f65ac382773d2b534a1d7b80
+https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.1-py311h63ff55d_0.conda#69ad01f66b8efff535d341ba5b283c2c
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
+https://conda.anaconda.org/conda-forge/noarch/mako-1.2.4-pyhd8ed1ab_0.tar.bz2#0d072f0edc017b6318dbab701e053f94
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
+https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.15-py311h459d7ec_0.conda#d2199e4c33e24003103845ab9b07469e
+https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
+https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
+https://conda.anaconda.org/conda-forge/noarch/alembic-1.11.1-pyhd8ed1ab_0.conda#6a55e123397b42b79c48b31d1b7a91b8
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
+https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.0-py311h38be061_0.conda#1dd43a18a75d59206019e2a2a28555e5
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/jupyter_telemetry-0.1.0-pyhd8ed1ab_1.tar.bz2#bb9ebdb6d5aa2622484aff1faceee181
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.1.2-pyh9f0ad1d_0.tar.bz2#2cbd910890bb328e8959246a1e16fac7
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.1.3-pyhd8ed1ab_0.tar.bz2#bafa5df6d4f8db69a4d197b4657127e7
-https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.1.1-pyhd8ed1ab_0.tar.bz2#34bb0b023e083aa8a4af74311031a352
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-21.0.0-pyhd8ed1ab_0.tar.bz2#8c49efecb7dca466e18b06015e8c88ce
-https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.5-pyh9f0ad1d_2.tar.bz2#5266fcd697043c59621fda522b3d78ee
+https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
+https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.2-pyhd8ed1ab_0.tar.bz2#8f882b197fd9c4941a787926baea4868
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
+https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/certipy-0.1.3-py_0.tar.bz2#23486713ef5712923e7c57cae609b22e
-https://conda.anaconda.org/conda-forge/noarch/nbclient-0.5.10-pyhd8ed1ab_1.tar.bz2#000cfe33d6fa746c5a9d1b29a79342a3
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.24-pyha770c72_0.tar.bz2#edaf527a6d394e2b965aff228c2e552f
-https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.8-pyhd8ed1ab_1.tar.bz2#53f1387c68c21cecb386e2cde51b3f7c
-https://conda.anaconda.org/conda-forge/linux-64/ipython-7.31.1-py37h89c1867_0.tar.bz2#764033508e28c9b0f7b02327416aab9a
-https://conda.anaconda.org/conda-forge/linux-64/nbconvert-6.0.7-py37h89c1867_3.tar.bz2#aa3710e0a8a44d7c7313b37775018446
-https://conda.anaconda.org/conda-forge/noarch/requests-2.27.1-pyhd8ed1ab_0.tar.bz2#7c1c427246b057b8fa97200ecdb2ed62
-https://conda.anaconda.org/conda-forge/linux-64/ipykernel-6.7.0-py37h6531663_0.tar.bz2#1042e547a7d1ec447155d3e727061c2e
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-1.13.4-pyhd8ed1ab_0.tar.bz2#70c6e1f755731d858767cb3c08c56a95
-https://conda.anaconda.org/conda-forge/linux-64/jupyterhub-base-1.4.2-py37h89c1867_0.tar.bz2#a61ccf7a9c83522c9b869816bb041a4c
-https://conda.anaconda.org/conda-forge/noarch/jupyter-resource-usage-0.6.1-pyhd8ed1ab_0.tar.bz2#a35cb988cd5b9b9b2d1c6179a8a86974
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.10.3-pyhd8ed1ab_0.tar.bz2#65d62a616bed5237b85b9e2a88378ec0
-https://conda.anaconda.org/conda-forge/noarch/notebook-6.3.0-pyha770c72_1.tar.bz2#6a53111a5a62d32abfa21aac8fc55a1b
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
+https://conda.anaconda.org/conda-forge/noarch/jupyterhub-base-3.1.1-pyh2a2186d_0.conda#78fc5dfd4577a7ba172fa65eb64b6afb
+https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh210e3f2_0.conda#4b57b688e22d094d1479a35543c18e93
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-1.23.6-pyhd8ed1ab_0.conda#5016f7c6845a6efd270fcee63af9a2a0
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.4.0-pyhd8ed1ab_0.conda#127c702e1b1eff595be82bc6a78cfce0
+https://conda.anaconda.org/conda-forge/noarch/jupyter-resource-usage-0.7.1-pyhd8ed1ab_0.conda#62ed54dc748d19d0cf056a3f90cc8f12
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.4.0-pyhd8ed1ab_0.conda#a86727968b41c20dd3d73b91632e77dc
+https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
+https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
+https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
 https://conda.anaconda.org/conda-forge/noarch/jupyter-offlinenotebook-0.2.2-pyh1d7be83_0.tar.bz2#fe55056ce4bc4bd4953ba440270735fb
-https://conda.anaconda.org/conda-forge/linux-64/jupyterhub-singleuser-1.4.2-py37h89c1867_0.tar.bz2#fb8151960fce2c583c7d1eaf6d4a178a
-https://conda.anaconda.org/conda-forge/noarch/nbclassic-0.3.5-pyhd8ed1ab_0.tar.bz2#e9e2281b7dc08d876fc789af0f571ade
-https://conda.anaconda.org/conda-forge/noarch/nteract_on_jupyter-2.1.3-py_0.tar.bz2#1430ccd983ae6b161e2fbf4377965f7a
-https://conda.anaconda.org/conda-forge/linux-64/widgetsnbextension-3.5.2-py37h89c1867_1.tar.bz2#deaf685ad832b287439250b4ff35f64d
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-7.6.5-pyhd8ed1ab_0.tar.bz2#6f2ee1ec157104df141e2e5afeba98d4
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.2.8-pyhd8ed1ab_0.tar.bz2#e2cc0671571f14af58f832c912dee025
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.4-pyhd8ed1ab_0.conda#e66d4a6e36fcc92fe266932bf85fd35a
+https://conda.anaconda.org/conda-forge/noarch/jupyterhub-singleuser-3.1.1-pyh2a2186d_0.conda#6d0a3394efe9ff7c0ad1ed03a6ca3720
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-2.7.lock` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-2.7-linux-64.lock`

 * *Files 7% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 # AUTO GENERATED FROM environment.py-2.7.yml, DO NOT MANUALLY MODIFY
-# Frozen on 2022-01-26 18:33:44 UTC
+# Frozen on 2022-08-01 23:18:07 UTC
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 6e66c9e333cfc5d702bcabcb832e0f70ee70bd3ef21869e83a2db3596ce0d826
+# input_hash: 7beee4267691da3e6d80db0820d9671e9bc51feff7a943357b4a21783a8f7826
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
-https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2021.10.8-ha878542_0.tar.bz2#575611b8a84f45960e87722eeb51fa26
+https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2022.6.15-ha878542_0.tar.bz2#c320890f77fd1d617fa876e0982002c2
 https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.36.1-hea4e1c9_2.tar.bz2#bd4f2e711b39af170e7ff15163fe87ee
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-11.2.0-he4da1e4_12.tar.bz2#7ff3b832ba5e6918c0d026976359d065
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-11.2.0-h1d223b6_12.tar.bz2#763c5ec8116d984b4a33342236d7da36
-https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-1_gnu.tar.bz2#561e277319a41d4f24f5c05a9ef63c04
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-11.2.0-h1d223b6_12.tar.bz2#d34efbb8d7d6312c816b4bb647b818b1
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-12.1.0-ha89aaad_16.tar.bz2#6f5ba041a41eb102a1027d9e68731be7
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-12.1.0-h8d9b700_16.tar.bz2#f013cf7749536ce43d82afbffdf499ab
+https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-12.1.0-h8d9b700_16.tar.bz2#4f05bc9844f7c101e6e147dab3c88d5c
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.2.1-he1b5a44_1007.tar.bz2#11389072d7d6036fd811c3d9460475cd
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.17-h516909a_0.tar.bz2#a98437ebf6fbbc6e498c64636f3958cf
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.11-h36c2ea0_1013.tar.bz2#dcddf696ff5dfcab567100d691678e18
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h9c3ff4c_0.tar.bz2#fb31bcb7af058244479ca635d20f0f4a
-https://conda.anaconda.org/conda-forge/linux-64/openssl-1.1.1l-h7f98852_0.tar.bz2#de7b38a1542dbe6f41653a8ae71adc53
-https://conda.anaconda.org/conda-forge/linux-64/readline-8.1-h46c0cb4_0.tar.bz2#5788de3c8d7a7d64ac56c784c4ef48e6
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.12-h166bdaf_2.tar.bz2#8302381297332ea50532cf2c67961080
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
+https://conda.anaconda.org/conda-forge/linux-64/openssl-1.1.1q-h166bdaf_0.tar.bz2#07acc367c7fc8b716770cd5b36d31717
+https://conda.anaconda.org/conda-forge/linux-64/readline-8.1.2-h0f457ee_0.tar.bz2#db2ebbe2943aae81ed051a6a9af8e0fa
+https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.2-he1b5a44_2.tar.bz2#bc50a478e0d59f9a62ad164e7d768f63
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.11-h36c2ea0_1013.tar.bz2#cf7190238072a41e9579e4476a6a60b8
-https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.37.0-h9cd32fc_0.tar.bz2#eb66fc098824d25518a79e83d12a81d6
-https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.11-h27826a3_1.tar.bz2#84e76fb280e735fec1efd2d21fd9cb27
+https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.12-h166bdaf_2.tar.bz2#4533821485cde83ab12ff3d8bda83768
+https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.39.2-h4ff8645_0.tar.bz2#2cf5cb4cd116a78e639977eb61ad9987
 https://conda.anaconda.org/conda-forge/linux-64/python-2.7.15-h5a48372_1011_cpython.tar.bz2#d1824ac0987155f58a03b7ffda01db38
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-py_2.tar.bz2#0da16b293affa6ac31812376f8eb79dd
 https://conda.anaconda.org/conda-forge/noarch/backports_abc-0.5-py_1.tar.bz2#6ac8cc52b55791b066dc43469bbaf8f2
 https://conda.anaconda.org/conda-forge/noarch/decorator-4.4.2-py_0.tar.bz2#d2eabb9cabd212e1ec6a9463bd846243
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-2.7-1_cp27mu.tar.bz2#02d6ad6bce3a798e6ee85494cd9b3d8d
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.5.lock` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.5-linux-64.lock`

 * *Files identical despite different names*

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.6.lock` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.6-linux-64.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,85 +1,86 @@
 # AUTO GENERATED FROM environment.py-3.6.yml, DO NOT MANUALLY MODIFY
-# Frozen on 2022-01-26 18:34:43 UTC
+# Frozen on 2022-04-08 20:38:59 UTC
 # Generated by conda-lock.
 # platform: linux-64
 # input_hash: a380aced865172581392c0b25b78cfde69a59becdb41fef3ade37eae6b024aed
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
 https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2021.10.8-ha878542_0.tar.bz2#575611b8a84f45960e87722eeb51fa26
 https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.36.1-hea4e1c9_2.tar.bz2#bd4f2e711b39af170e7ff15163fe87ee
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-11.2.0-he4da1e4_12.tar.bz2#7ff3b832ba5e6918c0d026976359d065
-https://conda.anaconda.org/conda-forge/linux-64/pandoc-2.17.0.1-h7f98852_0.tar.bz2#bd9fa82641da6dfe5696fd196e3c7cf1
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-11.2.0-h1d223b6_12.tar.bz2#763c5ec8116d984b4a33342236d7da36
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-11.2.0-he4da1e4_15.tar.bz2#4ffda9c4352880439042fbb8a9863e8c
+https://conda.anaconda.org/conda-forge/linux-64/pandoc-2.17.1.1-ha770c72_0.tar.bz2#316431b0b4e25f384cfd3428a1a5dd8c
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-11.2.0-h1d223b6_15.tar.bz2#5b7bff215ad9f30325dbe86dd983cb49
 https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-1_gnu.tar.bz2#561e277319a41d4f24f5c05a9ef63c04
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-11.2.0-h1d223b6_12.tar.bz2#d34efbb8d7d6312c816b4bb647b818b1
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-11.2.0-h1d223b6_15.tar.bz2#8041e476e66fcde71f0aa3d614e0efcf
 https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.18.1-h7f98852_0.tar.bz2#f26ef8098fab1f719c91eb760d63381a
-https://conda.anaconda.org/conda-forge/linux-64/icu-69.1-h9c3ff4c_0.tar.bz2#e0773c9556d588b062a4e1424a6a02fa
+https://conda.anaconda.org/conda-forge/linux-64/icu-70.1-h27087fc_0.tar.bz2#87473a15119779e021c314249d4b4aed
+https://conda.anaconda.org/conda-forge/linux-64/keyutils-1.6.1-h166bdaf_0.tar.bz2#30186d27e2c9fa62b45fb1476b7200e3
 https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
 https://conda.anaconda.org/conda-forge/linux-64/libuv-1.43.0-h7f98852_0.tar.bz2#b34d856aa7e06ebd79bded72ef4afc16
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.11-h36c2ea0_1013.tar.bz2#dcddf696ff5dfcab567100d691678e18
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h9c3ff4c_0.tar.bz2#fb31bcb7af058244479ca635d20f0f4a
-https://conda.anaconda.org/conda-forge/linux-64/openssl-1.1.1l-h7f98852_0.tar.bz2#de7b38a1542dbe6f41653a8ae71adc53
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.11-h166bdaf_1014.tar.bz2#757138ba3ddc6777b82e91d9ff62e7b9
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h27087fc_1.tar.bz2#4acfc691e64342b9dae57cf2adc63238
+https://conda.anaconda.org/conda-forge/linux-64/openssl-1.1.1n-h166bdaf_0.tar.bz2#cf0ddbd911fa547e6bc4291ca5e17379
 https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.5-h516909a_1.tar.bz2#33f601066901f3e1a85af3522a8113f9
 https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
 https://conda.anaconda.org/conda-forge/linux-64/readline-8.1-h46c0cb4_0.tar.bz2#5788de3c8d7a7d64ac56c784c4ef48e6
+https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.11-h36c2ea0_1013.tar.bz2#cf7190238072a41e9579e4476a6a60b8
-https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.43.0-h812cca2_1.tar.bz2#d0a7846b7b3b8fb0d8b36904a53b8155
+https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.11-h166bdaf_1014.tar.bz2#def3b82d1a03aa695bb38ac1dd072ff2
+https://conda.anaconda.org/conda-forge/linux-64/krb5-1.19.3-h3790be6_0.tar.bz2#7d862b05445123144bec92cb1acc8ef8
+https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.47.0-h727a467_0.tar.bz2#a22567abfea169ff8048506b1ca9b230
 https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.10.0-ha56f1ee_2.tar.bz2#6ab4eaa11ff01801cffca0a27489dc04
-https://conda.anaconda.org/conda-forge/linux-64/nodejs-14.18.3-h8ca31f7_2.tar.bz2#192a478a1ae899992e4afce84520badb
-https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.37.0-h9cd32fc_0.tar.bz2#eb66fc098824d25518a79e83d12a81d6
-https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.11-h27826a3_1.tar.bz2#84e76fb280e735fec1efd2d21fd9cb27
-https://conda.anaconda.org/conda-forge/linux-64/krb5-1.19.2-hcc1bbae_3.tar.bz2#e29650992ae593bc05fc93722483e5c3
+https://conda.anaconda.org/conda-forge/linux-64/nodejs-14.18.3-h96d913c_3.tar.bz2#45c64ff49b9d353104b9a127869cd108
+https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.37.1-h4ff8645_0.tar.bz2#8057ac02d6d10a162d7eb4b0ca7ed291
+https://conda.anaconda.org/conda-forge/linux-64/libcurl-7.82.0-h7bff187_0.tar.bz2#fa26f833ca8796ad44f9561c5402013d
 https://conda.anaconda.org/conda-forge/linux-64/python-3.6.15-hb7a2778_0_cpython.tar.bz2#2263dbd2d8116aa8dd974602faabb1a2
 https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
 https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
 https://conda.anaconda.org/conda-forge/noarch/backports-1.0-py_2.tar.bz2#0da16b293affa6ac31812376f8eb79dd
 https://conda.anaconda.org/conda-forge/noarch/blinker-1.4-py_1.tar.bz2#fa509a09190583f869ae442bf4d17f5f
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.0.10-pyhd8ed1ab_0.tar.bz2#ea77236c8031cfa821720b21b4cb0ceb
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.0.12-pyhd8ed1ab_0.tar.bz2#1f5b32dabae0f1893ae3283dac7f799e
 https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyh787bdff_2.tar.bz2#ed959a4ba14e6ddfa898630a5474a601
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.3-pyhd8ed1ab_1003.tar.bz2#bbf9a201f6ce99a506f4955374d9a9f4
+https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
 https://conda.anaconda.org/conda-forge/noarch/idna-3.3-pyhd8ed1ab_0.tar.bz2#40b50b8b030f5f2f22085c062ed013dd
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-1.0.2-pyhd8ed1ab_0.tar.bz2#eaff56fe28d1236076aa3bb13c35b434
-https://conda.anaconda.org/conda-forge/linux-64/libcurl-7.81.0-h2574ce0_0.tar.bz2#1f8655741d0269ca6756f131522da1e8
-https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.4-pyhd8ed1ab_0.tar.bz2#0d86e4e6ac78912f3f47e0453b124aca
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-1.1.0-pyhd8ed1ab_0.tar.bz2#e963a4a39cf442dbe5503f66edda083d
+https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.5-pyhd8ed1ab_0.tar.bz2#dc36c992aec485c0efff619ed2e63957
 https://conda.anaconda.org/conda-forge/noarch/pamela-1.0.0-py_0.tar.bz2#36f6f18d2f3ae0c93d77a9dbedad08c3
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.7.1-pyh9f0ad1d_0.tar.bz2#f66647d1ec805566d72ac26f62b19c01
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.13.0-pyhd8ed1ab_0.tar.bz2#f5567b5e7a5abc9133f198b8356674d1
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.14.0-pyhd8ed1ab_0.tar.bz2#6996536cbb531e722a452feebff019a3
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
 https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.3.0-pyhd8ed1ab_1.tar.bz2#b7bc0de380f114658af5fe57cebdcd9e
 https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.7-pyhd8ed1ab_0.tar.bz2#727e2216d9c47455d8ddc060eb2caad9
 https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.1-pyh9f0ad1d_0.tar.bz2#aed452f2f9f8bc8b2b0c412975051b5b
 https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.6-2_cp36m.tar.bz2#6f5b92d833a339da29ad8578c2a648ad
-https://conda.anaconda.org/conda-forge/noarch/pytz-2021.3-pyhd8ed1ab_0.tar.bz2#7e4f811bff46a5a6a7e0094921389395
+https://conda.anaconda.org/conda-forge/noarch/pytz-2022.1-pyhd8ed1ab_0.tar.bz2#b87d66d6d3991d988fb31510c95a9267
 https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.0-pyhd8ed1ab_0.tar.bz2#edab14119efe85c3bf131ad747e9005c
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
-https://conda.anaconda.org/conda-forge/noarch/testpath-0.5.0-pyhd8ed1ab_0.tar.bz2#53b57d6a468bebc7cef1253b177a5e9e
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.0.1-pyha770c72_0.tar.bz2#1fc03816925d3cb7fdab9ab234e7fea7
+https://conda.anaconda.org/conda-forge/noarch/testpath-0.6.0-pyhd8ed1ab_0.tar.bz2#196b1f0165dbc9ea6f03c3b3419323fd
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.1.1-pyha770c72_0.tar.bz2#74761ba7bc682e9009520163a1031ace
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.2.3-pyhd8ed1ab_0.tar.bz2#a9e89668df0da0f33c8c4ddf7c118f6d
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.3.1-pyhd8ed1ab_0.tar.bz2#0fa7710a18a1fa033b8337f6515c9de1
 https://conda.anaconda.org/conda-forge/noarch/wheel-0.37.1-pyhd8ed1ab_0.tar.bz2#1ca02aaf78d9c70d9a81a3bed5752022
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.7.0-pyhd8ed1ab_0.tar.bz2#947f7f41958eabc0f6e886557512bb76
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.6.0-pyhd8ed1ab_0.tar.bz2#855e2c4622f5eb50a4f6f7167b9ba17a
 https://conda.anaconda.org/conda-forge/noarch/babel-2.9.1-pyh44b312d_0.tar.bz2#74136ed39bfea0832d338df1e58d013e
 https://conda.anaconda.org/conda-forge/linux-64/certifi-2021.5.30-py36h5fab9bb_0.tar.bz2#500e3fb737f9d2023755f78f1f22ca69
 https://conda.anaconda.org/conda-forge/linux-64/cffi-1.14.6-py36hd8eec40_1.tar.bz2#2e025dd15559c9882880f005e6c02018
 https://conda.anaconda.org/conda-forge/linux-64/greenlet-1.1.1-py36hc4f0c31_0.tar.bz2#e0509bd49a3747b0442ecabae4a0df1b
 https://conda.anaconda.org/conda-forge/linux-64/importlib-metadata-4.8.1-py36h5fab9bb_0.tar.bz2#ec50a4f999b407d69b3a433c1405f0ba
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.4.0-pyhd8ed1ab_0.tar.bz2#9fb134dbabe7851a9d71411064b2c30d
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.6.0-pyhd8ed1ab_0.tar.bz2#ffee77eddb96c584ed417d2f72670a02
 https://conda.anaconda.org/conda-forge/linux-64/jedi-0.17.2-py36h5fab9bb_1.tar.bz2#e761c2377eafa1268eda3dd192cb06cb
 https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.0.1-py36h8f6f2f9_0.tar.bz2#e450eb239eb68d0467b1c6d0fef28ae9
 https://conda.anaconda.org/conda-forge/linux-64/mistune-0.8.4-py36h8f6f2f9_1004.tar.bz2#a53a196c30fc83ee9f0a84711b8fa681
 https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2#71f1ab2de48613876becddd496371c85
 https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh9f0ad1d_2.tar.bz2#5909e7b978141dd80d28dbf9de627827
 https://conda.anaconda.org/conda-forge/linux-64/psutil-5.8.0-py36h8f6f2f9_1.tar.bz2#ccecd9206d61f029549a81a980174ed8
 https://conda.anaconda.org/conda-forge/linux-64/pycurl-7.44.1-py36h66a4f8d_0.tar.bz2#ab0c8b5ebc4924b67d1ee2b1444abf0b
@@ -87,44 +88,44 @@
 https://conda.anaconda.org/conda-forge/linux-64/pysocks-1.7.1-py36h5fab9bb_3.tar.bz2#4dfb9be0b2975bc7933f32c6db7af205
 https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
 https://conda.anaconda.org/conda-forge/linux-64/pyzmq-22.3.0-py36h7068817_0.tar.bz2#6bd5499ce1e61fde19e5ce8206569303
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.2-py36h8f6f2f9_2.tar.bz2#20b17ae368cb09dd5609203ad3eaf122
 https://conda.anaconda.org/conda-forge/linux-64/setuptools-58.0.4-py36h5fab9bb_2.tar.bz2#d584b24af029d1fc78b6a0d2cc294d40
 https://conda.anaconda.org/conda-forge/linux-64/tornado-6.1-py36h8f6f2f9_1.tar.bz2#3d19680e14cb7cf6f383ba1fd3a72f2c
 https://conda.anaconda.org/conda-forge/noarch/traitlets-4.3.3-pyhd8ed1ab_2.tar.bz2#dacad0ee02418407a5991b0b62dfdc18
-https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.0.1-hd8ed1ab_0.tar.bz2#c0d4ec4bcbceb927bff1103a997410d3
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.1.1-hd8ed1ab_0.tar.bz2#9d1b5bbaa13bca480c80893a87a52c4f
 https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-21.1.0-py36h8f6f2f9_0.tar.bz2#c7ff3bb6bfd8cb82aefb8d960c439743
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
-https://conda.anaconda.org/conda-forge/noarch/bleach-4.1.0-pyhd8ed1ab_0.tar.bz2#4a2104c7b22c222bd0fe03aaef12862c
+https://conda.anaconda.org/conda-forge/noarch/bleach-5.0.0-pyhd8ed1ab_0.tar.bz2#2a2ae7c56b8f72caba261363407b484a
 https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py36h8f6f2f9_1001.tar.bz2#0f244e9624403e17430e9d959530b01c
 https://conda.anaconda.org/conda-forge/linux-64/cryptography-35.0.0-py36hb60f036_0.tar.bz2#d7533bed1783b4abef7e598cee93347d
 https://conda.anaconda.org/conda-forge/linux-64/immutables-0.16-py36h8f6f2f9_0.tar.bz2#e9abd4b9cee6d7dd062ca2b5f4e4c9f3
 https://conda.anaconda.org/conda-forge/noarch/jinja2-3.0.3-pyhd8ed1ab_0.tar.bz2#036d872c653780cb26e797e2e2f61b4c
 https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.1.2-pyhd8ed1ab_0.tar.bz2#94188756716d63117f09d546a30d43e7
 https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-4.8.1-py36h5fab9bb_0.tar.bz2#a6fa892e9d37e4e299b426c8fdb6f1d6
-https://conda.anaconda.org/conda-forge/noarch/mako-1.1.6-pyhd8ed1ab_0.tar.bz2#cb952a55037148f6a5ddd9770ee1384f
+https://conda.anaconda.org/conda-forge/noarch/mako-1.2.0-pyhd8ed1ab_1.tar.bz2#df0535cc0efcc9d418940fc689b1487c
 https://conda.anaconda.org/conda-forge/noarch/pip-21.3.1-pyhd8ed1ab_0.tar.bz2#e4fe2a9af78ff11f1aced7e62128c6a8
 https://conda.anaconda.org/conda-forge/noarch/pygments-2.11.2-pyhd8ed1ab_0.tar.bz2#caef60540e2239e27bf62569a5015e3b
 https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.16-py36h8f6f2f9_0.tar.bz2#602e4a91b1df8519343e4a317a75fd5a
 https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-1.4.25-py36h8f6f2f9_0.tar.bz2#fbe3f8667087f9c6dc0011df8c39f76b
 https://conda.anaconda.org/conda-forge/linux-64/terminado-0.12.1-py36h5fab9bb_0.tar.bz2#292f1173e1c1b446dc5969444f619108
-https://conda.anaconda.org/conda-forge/noarch/alembic-1.7.5-pyhd8ed1ab_0.tar.bz2#1102908123392ffc63c01caea136b1d4
+https://conda.anaconda.org/conda-forge/noarch/alembic-1.7.7-pyhd8ed1ab_0.tar.bz2#9637550104fade18bc6f91aef1f4f02c
 https://conda.anaconda.org/conda-forge/noarch/contextvars-2.4-py_0.tar.bz2#295fe9300971a6bd1dc4b18ad6509be2
 https://conda.anaconda.org/conda-forge/noarch/jupyter_client-7.1.2-pyhd8ed1ab_0.tar.bz2#9a332b6f8f05629435ce59032df8cfa9
 https://conda.anaconda.org/conda-forge/noarch/jupyter_telemetry-0.1.0-pyhd8ed1ab_1.tar.bz2#bb9ebdb6d5aa2622484aff1faceee181
 https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.1.2-pyh9f0ad1d_0.tar.bz2#2cbd910890bb328e8959246a1e16fac7
 https://conda.anaconda.org/conda-forge/noarch/nbformat-5.1.3-pyhd8ed1ab_0.tar.bz2#bafa5df6d4f8db69a4d197b4657127e7
-https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.1.1-pyhd8ed1ab_0.tar.bz2#34bb0b023e083aa8a4af74311031a352
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-21.0.0-pyhd8ed1ab_0.tar.bz2#8c49efecb7dca466e18b06015e8c88ce
+https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.0-pyhd8ed1ab_0.tar.bz2#ecc95c82c788737d6d33f5d564566d89
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-22.0.0-pyhd8ed1ab_0.tar.bz2#1d7e241dfaf5475e893d4b824bb71b44
 https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.5-pyh9f0ad1d_2.tar.bz2#5266fcd697043c59621fda522b3d78ee
 https://conda.anaconda.org/conda-forge/noarch/certipy-0.1.3-py_0.tar.bz2#23486713ef5712923e7c57cae609b22e
 https://conda.anaconda.org/conda-forge/noarch/nbclient-0.5.9-pyhd8ed1ab_0.tar.bz2#21554dd9bbabff27ae87f715fee4d56c
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.24-pyha770c72_0.tar.bz2#edaf527a6d394e2b965aff228c2e552f
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.29-pyha770c72_0.tar.bz2#9e720b57b22ef3032b4fb081697819dd
 https://conda.anaconda.org/conda-forge/linux-64/sniffio-1.2.0-py36h5fab9bb_1.tar.bz2#43c550017bd3ffea3cbc9669617b71eb
-https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.8-pyhd8ed1ab_1.tar.bz2#53f1387c68c21cecb386e2cde51b3f7c
+https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.9-pyhd8ed1ab_0.tar.bz2#0ea179ee251aa7100807c35bc0252693
 https://conda.anaconda.org/conda-forge/linux-64/anyio-3.3.2-py36h5fab9bb_0.tar.bz2#68e1135e2c76b473fc08831ba4b940c0
 https://conda.anaconda.org/conda-forge/linux-64/ipython-7.16.1-py36he448a4c_2.tar.bz2#ac605247c1149f7b275a4bcf9fa0de41
 https://conda.anaconda.org/conda-forge/linux-64/nbconvert-6.0.7-py36h5fab9bb_3.tar.bz2#30f571d5b9a389f49b1d54a0e38871bc
 https://conda.anaconda.org/conda-forge/noarch/requests-2.27.1-pyhd8ed1ab_0.tar.bz2#7c1c427246b057b8fa97200ecdb2ed62
 https://conda.anaconda.org/conda-forge/linux-64/ipykernel-5.5.5-py36hcb3619a_0.tar.bz2#595507013916992bbd551005bfa96bbf
 https://conda.anaconda.org/conda-forge/noarch/jupyter_server-1.13.2-pyhd8ed1ab_0.tar.bz2#b6771ff740526a8a04853fda74dc03f3
 https://conda.anaconda.org/conda-forge/linux-64/jupyterhub-base-1.4.2-py36h5fab9bb_0.tar.bz2#01e91ea234e632cf4ee3284a338a679d
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.7.lock` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.7-linux-64.lock`

 * *Files 15% similar despite different names*

```diff
@@ -1,140 +1,158 @@
 # AUTO GENERATED FROM environment.py-3.7.yml, DO NOT MANUALLY MODIFY
-# Frozen on 2022-01-26 18:35:40 UTC
+# Frozen on 2023-06-08 09:33:53 UTC
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 8daa45fe7e84c647f0c5ab04c1199514abe3834c110cffac7bd4a18cc5375472
+# input_hash: 2339ad954e3f369212967cce974e168db8116914593597b2d8fe8742b677dd60
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
-https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2021.10.8-ha878542_0.tar.bz2#575611b8a84f45960e87722eeb51fa26
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.36.1-hea4e1c9_2.tar.bz2#bd4f2e711b39af170e7ff15163fe87ee
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-11.2.0-he4da1e4_12.tar.bz2#7ff3b832ba5e6918c0d026976359d065
-https://conda.anaconda.org/conda-forge/linux-64/pandoc-2.17.0.1-h7f98852_0.tar.bz2#bd9fa82641da6dfe5696fd196e3c7cf1
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-11.2.0-h1d223b6_12.tar.bz2#763c5ec8116d984b4a33342236d7da36
-https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-1_gnu.tar.bz2#561e277319a41d4f24f5c05a9ef63c04
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-11.2.0-h1d223b6_12.tar.bz2#d34efbb8d7d6312c816b4bb647b818b1
-https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.18.1-h7f98852_0.tar.bz2#f26ef8098fab1f719c91eb760d63381a
-https://conda.anaconda.org/conda-forge/linux-64/icu-69.1-h9c3ff4c_0.tar.bz2#e0773c9556d588b062a4e1424a6a02fa
-https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
+https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
+https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.7-3_cp37m.conda#46277e9cf1ecd46926a31cea47079009
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
+https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
+https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
-https://conda.anaconda.org/conda-forge/linux-64/libuv-1.43.0-h7f98852_0.tar.bz2#b34d856aa7e06ebd79bded72ef4afc16
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.11-h36c2ea0_1013.tar.bz2#dcddf696ff5dfcab567100d691678e18
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h9c3ff4c_0.tar.bz2#fb31bcb7af058244479ca635d20f0f4a
-https://conda.anaconda.org/conda-forge/linux-64/openssl-1.1.1l-h7f98852_0.tar.bz2#de7b38a1542dbe6f41653a8ae71adc53
-https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.5-h516909a_1.tar.bz2#33f601066901f3e1a85af3522a8113f9
-https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
-https://conda.anaconda.org/conda-forge/linux-64/readline-8.1-h46c0cb4_0.tar.bz2#5788de3c8d7a7d64ac56c784c4ef48e6
+https://conda.anaconda.org/conda-forge/linux-64/libuv-1.44.2-h166bdaf_0.tar.bz2#e5cb4fe581a18ca2185a016eb848fc00
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
+https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
+https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
+https://conda.anaconda.org/conda-forge/linux-64/pandoc-2.19.2-h32600fe_2.conda#326f46f36d15c44cff5f81d505cb717f
+https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
+https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.11-h36c2ea0_1013.tar.bz2#cf7190238072a41e9579e4476a6a60b8
-https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.43.0-h812cca2_1.tar.bz2#d0a7846b7b3b8fb0d8b36904a53b8155
-https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.10.0-ha56f1ee_2.tar.bz2#6ab4eaa11ff01801cffca0a27489dc04
-https://conda.anaconda.org/conda-forge/linux-64/nodejs-14.18.3-h8ca31f7_2.tar.bz2#192a478a1ae899992e4afce84520badb
-https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.37.0-h9cd32fc_0.tar.bz2#eb66fc098824d25518a79e83d12a81d6
-https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.11-h27826a3_1.tar.bz2#84e76fb280e735fec1efd2d21fd9cb27
-https://conda.anaconda.org/conda-forge/linux-64/krb5-1.19.2-hcc1bbae_3.tar.bz2#e29650992ae593bc05fc93722483e5c3
-https://conda.anaconda.org/conda-forge/linux-64/python-3.7.12-hb7a2778_100_cpython.tar.bz2#2d94b3e6a9fdaf83f6955d008c8011a7
+https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-h166bdaf_4.tar.bz2#4b11e365c0275b808be78b30f904e295
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.15.0-h4abf6b9_1.conda#2aabafd88f6876a57c45c00598715ac4
+https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.42.0-h2c6b66d_0.conda#1192f6ec654a5bc4ee1d64bdc4a3e5cc
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
+https://conda.anaconda.org/conda-forge/linux-64/python-3.7.12-hf930737_100_cpython.tar.bz2#416558a6f46b7a1fa8db7d0e98aff56a
+https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
 https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
-https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
+https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
-https://conda.anaconda.org/conda-forge/noarch/backports-1.0-py_2.tar.bz2#0da16b293affa6ac31812376f8eb79dd
-https://conda.anaconda.org/conda-forge/noarch/blinker-1.4-py_1.tar.bz2#fa509a09190583f869ae442bf4d17f5f
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.0.10-pyhd8ed1ab_0.tar.bz2#ea77236c8031cfa821720b21b4cb0ceb
+https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
+https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda#2fb79ec81bad9492b6d59a06b3b647a4
+https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
+https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.3-py37hd23a5d3_0.tar.bz2#004724940367fa84ec1d0732c8b27c18
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.3-pyhd8ed1ab_1003.tar.bz2#bbf9a201f6ce99a506f4955374d9a9f4
-https://conda.anaconda.org/conda-forge/noarch/flit-core-3.6.0-pyhd8ed1ab_0.tar.bz2#f8c17f22a3ce533876c468157ff8ff8f
-https://conda.anaconda.org/conda-forge/noarch/idna-3.3-pyhd8ed1ab_0.tar.bz2#40b50b8b030f5f2f22085c062ed013dd
+https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
+https://conda.anaconda.org/conda-forge/linux-64/greenlet-1.1.3-py37hd23a5d3_0.tar.bz2#426c53c95df106039da865c0095e2a65
+https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-1.0.2-pyhd8ed1ab_0.tar.bz2#eaff56fe28d1236076aa3bb13c35b434
-https://conda.anaconda.org/conda-forge/linux-64/libcurl-7.81.0-h2574ce0_0.tar.bz2#1f8655741d0269ca6756f131522da1e8
-https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.4-pyhd8ed1ab_0.tar.bz2#0d86e4e6ac78912f3f47e0453b124aca
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.1-py37h540881e_1.tar.bz2#a9123517674ab0589d955a5adbf58573
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
+https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pamela-1.0.0-py_0.tar.bz2#36f6f18d2f3ae0c93d77a9dbedad08c3
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.13.0-pyhd8ed1ab_0.tar.bz2#f5567b5e7a5abc9133f198b8356674d1
+https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.3-py37h540881e_0.tar.bz2#0c813ad118e926df328bf74899a48047
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
-https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.3.0-pyhd8ed1ab_1.tar.bz2#b7bc0de380f114658af5fe57cebdcd9e
-https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.7-pyhd8ed1ab_0.tar.bz2#727e2216d9c47455d8ddc060eb2caad9
-https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.1-pyh9f0ad1d_0.tar.bz2#aed452f2f9f8bc8b2b0c412975051b5b
-https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.7-2_cp37m.tar.bz2#afff88bf9a7048da740c70aeb8cdbb82
-https://conda.anaconda.org/conda-forge/noarch/pytz-2021.3-pyhd8ed1ab_0.tar.bz2#7e4f811bff46a5a6a7e0094921389395
-https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.0-pyhd8ed1ab_0.tar.bz2#edab14119efe85c3bf131ad747e9005c
+https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.7.0-pyhd8ed1ab_0.conda#99e28be5a278e2319834d7dc99e7bfdd
+https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.18.1-py37h540881e_1.tar.bz2#8e25160800dafbc2a24c0aaa99a981ef
+https://conda.anaconda.org/conda-forge/linux-64/pysocks-1.7.1-py37h89c1867_5.tar.bz2#8c4b0563f96363ee99f1ab864616ac63
+https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
+https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
+https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
+https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py37h540881e_4.tar.bz2#f231119f9790da6da6bd93b250b7e42e
+https://conda.anaconda.org/conda-forge/linux-64/pyzmq-24.0.1-py37h0c0c2a8_0.tar.bz2#732c98a38c84984262940c868793ebb4
+https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
+https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.6-py37h540881e_1.tar.bz2#f3c703ac09e7810d6c9baec89e901fb5
+https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
-https://conda.anaconda.org/conda-forge/noarch/testpath-0.5.0-pyhd8ed1ab_0.tar.bz2#53b57d6a468bebc7cef1253b177a5e9e
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.1.1-pyhd8ed1ab_0.tar.bz2#a1bc9765ef9499760e88f568b3a6622c
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.0.1-pyha770c72_0.tar.bz2#1fc03816925d3cb7fdab9ab234e7fea7
+https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
+https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
+https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
+https://conda.anaconda.org/conda-forge/linux-64/tornado-6.2-py37h540881e_0.tar.bz2#2f0863ba6b29d1d2872b064dd697a492
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.2.3-pyhd8ed1ab_0.tar.bz2#a9e89668df0da0f33c8c4ddf7c118f6d
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.37.1-pyhd8ed1ab_0.tar.bz2#1ca02aaf78d9c70d9a81a3bed5752022
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.7.0-pyhd8ed1ab_0.tar.bz2#947f7f41958eabc0f6e886557512bb76
-https://conda.anaconda.org/conda-forge/noarch/babel-2.9.1-pyh44b312d_0.tar.bz2#74136ed39bfea0832d338df1e58d013e
-https://conda.anaconda.org/conda-forge/linux-64/certifi-2021.10.8-py37h89c1867_1.tar.bz2#48e8442b6097c7d4a0e3494c74ff9eeb
-https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.0-py37h036bc23_0.tar.bz2#05ab26c7685bcb7dd8bc8752c121f823
-https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.5.1-py37hcd2ae1e_0.tar.bz2#739a721301e47f42998af7bd51f0c42c
-https://conda.anaconda.org/conda-forge/linux-64/greenlet-1.1.2-py37hcd2ae1e_1.tar.bz2#f39576dbfb9a1067293d24f0e3b6bdda
-https://conda.anaconda.org/conda-forge/linux-64/importlib-metadata-4.10.1-py37h89c1867_0.tar.bz2#4684501699ad9eccbc29fa694d5343fc
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.4.0-pyhd8ed1ab_0.tar.bz2#9fb134dbabe7851a9d71411064b2c30d
-https://conda.anaconda.org/conda-forge/linux-64/jedi-0.18.1-py37h89c1867_0.tar.bz2#432446f7c13e1babe6bc05ba74d30f64
-https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-4.9.1-py37h89c1867_1.tar.bz2#95df6ebc6f4e8edd5d87aa99c59da605
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.0.1-py37h5e8e339_1.tar.bz2#6c7c14c95d4c435b66261639b64c7c51
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.3-pyhd8ed1ab_0.tar.bz2#be3bfd435802d2c768c6b2439f325f3d
-https://conda.anaconda.org/conda-forge/linux-64/mistune-0.8.4-py37h5e8e339_1005.tar.bz2#2dd7bedc3ea33c30cb9dcf93d64c10eb
-https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2#71f1ab2de48613876becddd496371c85
-https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh9f0ad1d_2.tar.bz2#5909e7b978141dd80d28dbf9de627827
-https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.0-py37h5e8e339_0.tar.bz2#009832a45a0d9240aa3f3329055da1ef
-https://conda.anaconda.org/conda-forge/linux-64/pycurl-7.44.1-py37h88a64d2_1.tar.bz2#4e4c43ae76df275f09cffc5e63ae936d
-https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.18.1-py37h5e8e339_0.tar.bz2#f7e31f8bb6c8b311c3842c090a440e3d
-https://conda.anaconda.org/conda-forge/linux-64/pysocks-1.7.1-py37h89c1867_4.tar.bz2#44df88d27e2891f90e3f06dcfcca0927
-https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/linux-64/pyzmq-22.3.0-py37h336d617_1.tar.bz2#6512cf886a870090430e2f37f41b652e
-https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.6-py37h5e8e339_0.tar.bz2#70ee31b43817f9fb7a46f76db99af94b
-https://conda.anaconda.org/conda-forge/linux-64/setuptools-60.5.0-py37h89c1867_0.tar.bz2#8d99eb0fa9aaae9dddb6a91451ac7907
-https://conda.anaconda.org/conda-forge/linux-64/sniffio-1.2.0-py37h89c1867_2.tar.bz2#464124f171b89cb9b459f47f81cc0e84
-https://conda.anaconda.org/conda-forge/linux-64/tornado-6.1-py37h5e8e339_2.tar.bz2#ec86ae00c96dea5f2d810957a8fabc26
-https://conda.anaconda.org/conda-forge/linux-64/anyio-3.5.0-py37h89c1867_0.tar.bz2#aa263b5829ec141d12bf6a5dec36bf5b
-https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py37h5e8e339_1.tar.bz2#042ff84df84e01a6399caa379deaf044
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/linux-64/y-py-0.5.4-py37hbd0741f_0.tar.bz2#ecadea26afe1035c2be1f159fdd22b4c
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
+https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
-https://conda.anaconda.org/conda-forge/noarch/bleach-4.1.0-pyhd8ed1ab_0.tar.bz2#4a2104c7b22c222bd0fe03aaef12862c
-https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py37h5e8e339_1003.tar.bz2#4ad2e74470a3c08b0f6d59699f0d9a32
-https://conda.anaconda.org/conda-forge/linux-64/cryptography-36.0.1-py37hf1a17b8_0.tar.bz2#7ad2c98aaab85d80017b3a6f79a2aa5d
-https://conda.anaconda.org/conda-forge/noarch/jinja2-3.0.3-pyhd8ed1ab_0.tar.bz2#036d872c653780cb26e797e2e2f61b4c
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.4.0-pyhd8ed1ab_0.tar.bz2#17ec41acce882e5db4efdcc4c01ca7e0
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-7.1.2-pyhd8ed1ab_0.tar.bz2#9a332b6f8f05629435ce59032df8cfa9
-https://conda.anaconda.org/conda-forge/noarch/mako-1.1.6-pyhd8ed1ab_0.tar.bz2#cb952a55037148f6a5ddd9770ee1384f
-https://conda.anaconda.org/conda-forge/noarch/pip-21.3.1-pyhd8ed1ab_0.tar.bz2#e4fe2a9af78ff11f1aced7e62128c6a8
-https://conda.anaconda.org/conda-forge/noarch/pygments-2.11.2-pyhd8ed1ab_0.tar.bz2#caef60540e2239e27bf62569a5015e3b
-https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.19-py37h5e8e339_0.tar.bz2#a909957daac2e6296ce9219940481e1d
-https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-1.4.31-py37h5e8e339_0.tar.bz2#8c316b01e34dea00fe526456be12fae4
-https://conda.anaconda.org/conda-forge/linux-64/terminado-0.12.1-py37h89c1867_1.tar.bz2#658fe17f1a35117ebfb063f3b023c884
-https://conda.anaconda.org/conda-forge/noarch/alembic-1.7.5-pyhd8ed1ab_0.tar.bz2#1102908123392ffc63c01caea136b1d4
+https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
+https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
+https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py37h43b0acd_1.tar.bz2#5111b64bdfdd72d85086ec49c952fe0d
+https://conda.anaconda.org/conda-forge/linux-64/importlib-metadata-4.11.4-py37h89c1867_0.tar.bz2#71107630527e4bd82932952351231efe
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
+https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
+https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
+https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-4.11.1-py37h89c1867_0.tar.bz2#6d184401b7a49bbebbfedc96bc7add1c
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
+https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
+https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.21-py37h540881e_1.tar.bz2#6232de79d3fe4aaa00f5f34d3da55c2a
+https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_0.conda#ae465d0fbf9f1979cb2d8d4043d885e2
+https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
+https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py37h540881e_2.tar.bz2#ff22fac37e988bed992b1f437e05906a
+https://conda.anaconda.org/conda-forge/linux-64/cryptography-38.0.2-py37h5994e8b_1.tar.bz2#5a8bb0074be9d20d456957f92b72beed
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-4.11.4-hd8ed1ab_0.tar.bz2#9a1925fdb91c81437b8012e48ede6851
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-7.4.9-pyhd8ed1ab_0.conda#5cbf9a31a19d4ef9103adb7d71fd45fd
+https://conda.anaconda.org/conda-forge/noarch/mako-1.2.4-pyhd8ed1ab_0.tar.bz2#0d072f0edc017b6318dbab701e053f94
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
+https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-1.4.42-py37h540881e_0.tar.bz2#921bb310665fba1ed0f64f3287fda6d4
+https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
+https://conda.anaconda.org/conda-forge/noarch/alembic-1.11.1-pyhd8ed1ab_0.conda#6a55e123397b42b79c48b31d1b7a91b8
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/jupyter_telemetry-0.1.0-pyhd8ed1ab_1.tar.bz2#bb9ebdb6d5aa2622484aff1faceee181
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.1.2-pyh9f0ad1d_0.tar.bz2#2cbd910890bb328e8959246a1e16fac7
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.1.3-pyhd8ed1ab_0.tar.bz2#bafa5df6d4f8db69a4d197b4657127e7
-https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.1.1-pyhd8ed1ab_0.tar.bz2#34bb0b023e083aa8a4af74311031a352
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-21.0.0-pyhd8ed1ab_0.tar.bz2#8c49efecb7dca466e18b06015e8c88ce
-https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.5-pyh9f0ad1d_2.tar.bz2#5266fcd697043c59621fda522b3d78ee
+https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.8.0-pyhd8ed1ab_0.conda#1ca43103a08456b19222d93fd9d119ac
+https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.2-pyhd8ed1ab_0.tar.bz2#8f882b197fd9c4941a787926baea4868
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
+https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/certipy-0.1.3-py_0.tar.bz2#23486713ef5712923e7c57cae609b22e
-https://conda.anaconda.org/conda-forge/noarch/nbclient-0.5.10-pyhd8ed1ab_1.tar.bz2#000cfe33d6fa746c5a9d1b29a79342a3
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.24-pyha770c72_0.tar.bz2#edaf527a6d394e2b965aff228c2e552f
-https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.8-pyhd8ed1ab_1.tar.bz2#53f1387c68c21cecb386e2cde51b3f7c
-https://conda.anaconda.org/conda-forge/linux-64/ipython-7.31.1-py37h89c1867_0.tar.bz2#764033508e28c9b0f7b02327416aab9a
-https://conda.anaconda.org/conda-forge/linux-64/nbconvert-6.0.7-py37h89c1867_3.tar.bz2#aa3710e0a8a44d7c7313b37775018446
-https://conda.anaconda.org/conda-forge/noarch/requests-2.27.1-pyhd8ed1ab_0.tar.bz2#7c1c427246b057b8fa97200ecdb2ed62
-https://conda.anaconda.org/conda-forge/linux-64/ipykernel-6.7.0-py37h6531663_0.tar.bz2#1042e547a7d1ec447155d3e727061c2e
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-1.13.4-pyhd8ed1ab_0.tar.bz2#70c6e1f755731d858767cb3c08c56a95
-https://conda.anaconda.org/conda-forge/linux-64/jupyterhub-base-1.4.2-py37h89c1867_0.tar.bz2#a61ccf7a9c83522c9b869816bb041a4c
-https://conda.anaconda.org/conda-forge/noarch/jupyter-resource-usage-0.6.1-pyhd8ed1ab_0.tar.bz2#a35cb988cd5b9b9b2d1c6179a8a86974
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.10.3-pyhd8ed1ab_0.tar.bz2#65d62a616bed5237b85b9e2a88378ec0
-https://conda.anaconda.org/conda-forge/noarch/notebook-6.3.0-pyha770c72_1.tar.bz2#6a53111a5a62d32abfa21aac8fc55a1b
+https://conda.anaconda.org/conda-forge/linux-64/ipython-7.33.0-py37h89c1867_0.tar.bz2#e4841787deb237aad17b2d44a2d32c23
+https://conda.anaconda.org/conda-forge/noarch/nbclient-0.7.0-pyhd8ed1ab_0.tar.bz2#87eed34d791330d8acdab6a8ab63113f
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.16.2-pyh210e3f2_0.tar.bz2#6b0f40821b784cac8a33d0c5eb7602c0
+https://conda.anaconda.org/conda-forge/noarch/jupyterhub-base-3.1.1-pyh2a2186d_0.conda#78fc5dfd4577a7ba172fa65eb64b6afb
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-1.23.4-pyhd8ed1ab_0.conda#35b7e9267926e864cc70ce137e6588ca
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.4.0-pyhd8ed1ab_0.conda#127c702e1b1eff595be82bc6a78cfce0
+https://conda.anaconda.org/conda-forge/noarch/jupyter-resource-usage-0.7.1-pyhd8ed1ab_0.conda#62ed54dc748d19d0cf056a3f90cc8f12
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.4.0-pyhd8ed1ab_0.conda#a86727968b41c20dd3d73b91632e77dc
+https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
+https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
+https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
 https://conda.anaconda.org/conda-forge/noarch/jupyter-offlinenotebook-0.2.2-pyh1d7be83_0.tar.bz2#fe55056ce4bc4bd4953ba440270735fb
-https://conda.anaconda.org/conda-forge/linux-64/jupyterhub-singleuser-1.4.2-py37h89c1867_0.tar.bz2#fb8151960fce2c583c7d1eaf6d4a178a
-https://conda.anaconda.org/conda-forge/noarch/nbclassic-0.3.5-pyhd8ed1ab_0.tar.bz2#e9e2281b7dc08d876fc789af0f571ade
-https://conda.anaconda.org/conda-forge/noarch/nteract_on_jupyter-2.1.3-py_0.tar.bz2#1430ccd983ae6b161e2fbf4377965f7a
-https://conda.anaconda.org/conda-forge/linux-64/widgetsnbextension-3.5.2-py37h89c1867_1.tar.bz2#deaf685ad832b287439250b4ff35f64d
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-7.6.5-pyhd8ed1ab_0.tar.bz2#6f2ee1ec157104df141e2e5afeba98d4
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.2.8-pyhd8ed1ab_0.tar.bz2#e2cc0671571f14af58f832c912dee025
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.4-pyhd8ed1ab_0.conda#e66d4a6e36fcc92fe266932bf85fd35a
+https://conda.anaconda.org/conda-forge/noarch/jupyterhub-singleuser-3.1.1-pyh2a2186d_0.conda#6d0a3394efe9ff7c0ad1ed03a6ca3720
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.8.lock` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.9-linux-64.lock`

 * *Files 15% similar despite different names*

```diff
@@ -1,152 +1,167 @@
-# AUTO GENERATED FROM environment.py-3.8.yml, DO NOT MANUALLY MODIFY
-# Frozen on 2022-01-26 18:36:36 UTC
+# AUTO GENERATED FROM environment.py-3.9.yml, DO NOT MANUALLY MODIFY
+# Frozen on 2023-06-08 09:34:51 UTC
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 76e94579a1728608e8c93f5df71d7f564ac6a98a6b3e770fdb3cc24ed7d034c0
+# input_hash: a8b01e6cf54b5f11b1fb28a14c88acae0339819976b3ee55dd4504f09b37ab3c
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
-https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2021.10.8-ha878542_0.tar.bz2#575611b8a84f45960e87722eeb51fa26
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.36.1-hea4e1c9_2.tar.bz2#bd4f2e711b39af170e7ff15163fe87ee
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-11.2.0-he4da1e4_12.tar.bz2#7ff3b832ba5e6918c0d026976359d065
-https://conda.anaconda.org/conda-forge/linux-64/pandoc-2.17.0.1-h7f98852_0.tar.bz2#bd9fa82641da6dfe5696fd196e3c7cf1
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-11.2.0-h1d223b6_12.tar.bz2#763c5ec8116d984b4a33342236d7da36
-https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-1_gnu.tar.bz2#561e277319a41d4f24f5c05a9ef63c04
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-11.2.0-h1d223b6_12.tar.bz2#d34efbb8d7d6312c816b4bb647b818b1
-https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.18.1-h7f98852_0.tar.bz2#f26ef8098fab1f719c91eb760d63381a
-https://conda.anaconda.org/conda-forge/linux-64/icu-69.1-h9c3ff4c_0.tar.bz2#e0773c9556d588b062a4e1424a6a02fa
-https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
+https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
+https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.9-3_cp39.conda#0dd193187d54e585cac7eab942a8847e
+https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
+https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
+https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
+https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
-https://conda.anaconda.org/conda-forge/linux-64/libuv-1.43.0-h7f98852_0.tar.bz2#b34d856aa7e06ebd79bded72ef4afc16
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.11-h36c2ea0_1013.tar.bz2#dcddf696ff5dfcab567100d691678e18
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h9c3ff4c_0.tar.bz2#fb31bcb7af058244479ca635d20f0f4a
-https://conda.anaconda.org/conda-forge/linux-64/openssl-1.1.1l-h7f98852_0.tar.bz2#de7b38a1542dbe6f41653a8ae71adc53
-https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.5-h516909a_1.tar.bz2#33f601066901f3e1a85af3522a8113f9
-https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
-https://conda.anaconda.org/conda-forge/linux-64/readline-8.1-h46c0cb4_0.tar.bz2#5788de3c8d7a7d64ac56c784c4ef48e6
+https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
+https://conda.anaconda.org/conda-forge/linux-64/libuv-1.44.2-h166bdaf_0.tar.bz2#e5cb4fe581a18ca2185a016eb848fc00
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
+https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
+https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
+https://conda.anaconda.org/conda-forge/linux-64/pandoc-2.19.2-h32600fe_2.conda#326f46f36d15c44cff5f81d505cb717f
+https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
+https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.11-h36c2ea0_1013.tar.bz2#cf7190238072a41e9579e4476a6a60b8
-https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.43.0-h812cca2_1.tar.bz2#d0a7846b7b3b8fb0d8b36904a53b8155
-https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.10.0-ha56f1ee_2.tar.bz2#6ab4eaa11ff01801cffca0a27489dc04
-https://conda.anaconda.org/conda-forge/linux-64/nodejs-14.18.3-h8ca31f7_2.tar.bz2#192a478a1ae899992e4afce84520badb
-https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.37.0-h9cd32fc_0.tar.bz2#eb66fc098824d25518a79e83d12a81d6
-https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.11-h27826a3_1.tar.bz2#84e76fb280e735fec1efd2d21fd9cb27
-https://conda.anaconda.org/conda-forge/linux-64/krb5-1.19.2-hcc1bbae_3.tar.bz2#e29650992ae593bc05fc93722483e5c3
-https://conda.anaconda.org/conda-forge/linux-64/python-3.8.12-hb7a2778_2_cpython.tar.bz2#148ea076514259c7f562fbfba956a693
+https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-h166bdaf_4.tar.bz2#4b11e365c0275b808be78b30f904e295
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.15.0-h4abf6b9_1.conda#2aabafd88f6876a57c45c00598715ac4
+https://conda.anaconda.org/conda-forge/linux-64/python-3.9.16-h2782a2a_0_cpython.conda#95c9b7c96a7fd7342e0c9d0a917b8f78
+https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
 https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
-https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
+https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
-https://conda.anaconda.org/conda-forge/noarch/backports-1.0-py_2.tar.bz2#0da16b293affa6ac31812376f8eb79dd
-https://conda.anaconda.org/conda-forge/noarch/blinker-1.4-py_1.tar.bz2#fa509a09190583f869ae442bf4d17f5f
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.0.10-pyhd8ed1ab_0.tar.bz2#ea77236c8031cfa821720b21b4cb0ceb
-https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
+https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
+https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda#2fb79ec81bad9492b6d59a06b3b647a4
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
+https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
+https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py39h227be39_0.conda#4d8b831c8707058f27d355882c6dd198
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.3-pyhd8ed1ab_1003.tar.bz2#bbf9a201f6ce99a506f4955374d9a9f4
-https://conda.anaconda.org/conda-forge/noarch/executing-0.8.2-pyhd8ed1ab_0.tar.bz2#dcd884e2cf5bcdccdf78f7db35999d62
-https://conda.anaconda.org/conda-forge/noarch/flit-core-3.6.0-pyhd8ed1ab_0.tar.bz2#f8c17f22a3ce533876c468157ff8ff8f
-https://conda.anaconda.org/conda-forge/noarch/idna-3.3-pyhd8ed1ab_0.tar.bz2#40b50b8b030f5f2f22085c062ed013dd
+https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
+https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
+https://conda.anaconda.org/conda-forge/linux-64/greenlet-2.0.2-py39h3d6467e_1.conda#bcc2596fee9dccce15c6ae3d475ea013
+https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-1.0.2-pyhd8ed1ab_0.tar.bz2#eaff56fe28d1236076aa3bb13c35b434
-https://conda.anaconda.org/conda-forge/linux-64/libcurl-7.81.0-h2574ce0_0.tar.bz2#1f8655741d0269ca6756f131522da1e8
-https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.4-pyhd8ed1ab_0.tar.bz2#0d86e4e6ac78912f3f47e0453b124aca
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py39hd1e30aa_0.conda#9c858d105816f454c6b64f3e19184b60
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
+https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pamela-1.0.0-py_0.tar.bz2#36f6f18d2f3ae0c93d77a9dbedad08c3
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
-https://conda.anaconda.org/conda-forge/noarch/pathspec-0.9.0-pyhd8ed1ab_0.tar.bz2#f93dc0ccbc0a8472624165f6e256c7d1
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.3.0-pyhd8ed1ab_0.tar.bz2#7bc119135be2a43e1701432399d8c28a
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.13.0-pyhd8ed1ab_0.tar.bz2#f5567b5e7a5abc9133f198b8356674d1
+https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py39h72bdee0_0.conda#1d54d3a75c3192ab7655d9c3d16809f1
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
-https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.3.0-pyhd8ed1ab_1.tar.bz2#b7bc0de380f114658af5fe57cebdcd9e
-https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.7-pyhd8ed1ab_0.tar.bz2#727e2216d9c47455d8ddc060eb2caad9
-https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.1-pyh9f0ad1d_0.tar.bz2#aed452f2f9f8bc8b2b0c412975051b5b
-https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.8-2_cp38.tar.bz2#bfbb29d517281e78ac53e48d21e6e860
-https://conda.anaconda.org/conda-forge/noarch/pytz-2021.3-pyhd8ed1ab_0.tar.bz2#7e4f811bff46a5a6a7e0094921389395
-https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.0-pyhd8ed1ab_0.tar.bz2#edab14119efe85c3bf131ad747e9005c
+https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.7.0-pyhd8ed1ab_0.conda#99e28be5a278e2319834d7dc99e7bfdd
+https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py39h72bdee0_0.conda#659013ef00dcd1751bfd26d894f73857
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
+https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
+https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
+https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
+https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py39hb9d737c_5.tar.bz2#ef9db3c38ae7275f6b14491cfe61a248
+https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py39hb257651_0.conda#9009fbea0e0992dcbdd2312e70c44c09
+https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
+https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py39h72bdee0_1.conda#d9da3b1d13895666f4cc2559d37b8de4
+https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
-https://conda.anaconda.org/conda-forge/noarch/testpath-0.5.0-pyhd8ed1ab_0.tar.bz2#53b57d6a468bebc7cef1253b177a5e9e
-https://conda.anaconda.org/conda-forge/noarch/tomli-1.2.2-pyhd8ed1ab_0.tar.bz2#1c8a2f9ea18c267414e244cee668cd00
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.1.1-pyhd8ed1ab_0.tar.bz2#a1bc9765ef9499760e88f568b3a6622c
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.0.1-pyha770c72_0.tar.bz2#1fc03816925d3cb7fdab9ab234e7fea7
+https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
+https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
+https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
+https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py39hd1e30aa_0.conda#da334eecb1ea2248e28294c49e6f6d89
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.2.3-pyhd8ed1ab_0.tar.bz2#a9e89668df0da0f33c8c4ddf7c118f6d
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.37.1-pyhd8ed1ab_0.tar.bz2#1ca02aaf78d9c70d9a81a3bed5752022
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.7.0-pyhd8ed1ab_0.tar.bz2#947f7f41958eabc0f6e886557512bb76
-https://conda.anaconda.org/conda-forge/noarch/asttokens-2.0.5-pyhd8ed1ab_0.tar.bz2#74badce16f060701fee55c39332f5253
-https://conda.anaconda.org/conda-forge/noarch/babel-2.9.1-pyh44b312d_0.tar.bz2#74136ed39bfea0832d338df1e58d013e
-https://conda.anaconda.org/conda-forge/linux-64/certifi-2021.10.8-py38h578d9bd_1.tar.bz2#52a6cee65a5d10ed1c3f0af24fb48dd3
-https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.0-py38h3931269_0.tar.bz2#9c491a90ae11d08ca97326a0ed876f3a
-https://conda.anaconda.org/conda-forge/linux-64/click-8.0.3-py38h578d9bd_1.tar.bz2#edee3c8cc58ceba6153ac96524146985
-https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.5.1-py38h709712a_0.tar.bz2#e4562edba9cf178746097668eaac5530
-https://conda.anaconda.org/conda-forge/linux-64/greenlet-1.1.2-py38h709712a_1.tar.bz2#dcf19dfc362c994575eb36e73c554902
-https://conda.anaconda.org/conda-forge/linux-64/importlib-metadata-4.10.1-py38h578d9bd_0.tar.bz2#26da12e39b1b93e82fb865e967d0cbe0
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.4.0-pyhd8ed1ab_0.tar.bz2#9fb134dbabe7851a9d71411064b2c30d
-https://conda.anaconda.org/conda-forge/linux-64/jedi-0.18.1-py38h578d9bd_0.tar.bz2#84ca00ec7d71269b633546dc83e0b088
-https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-4.9.1-py38h578d9bd_1.tar.bz2#61eac1660d6bb75978662a457efe948b
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.0.1-py38h497a2fe_1.tar.bz2#1ef7b5f4826ca48a15e2cd98a5c3436d
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.3-pyhd8ed1ab_0.tar.bz2#be3bfd435802d2c768c6b2439f325f3d
-https://conda.anaconda.org/conda-forge/linux-64/mistune-0.8.4-py38h497a2fe_1005.tar.bz2#e842470b42e2640e90a3a2e32729bc92
-https://conda.anaconda.org/conda-forge/linux-64/mypy_extensions-0.4.3-py38h578d9bd_4.tar.bz2#8800523c45d8782e76791d1963f2255a
-https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2#71f1ab2de48613876becddd496371c85
-https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh9f0ad1d_2.tar.bz2#5909e7b978141dd80d28dbf9de627827
-https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.0-py38h497a2fe_0.tar.bz2#f94deecb1bc24f2525de2fdf57a27e92
-https://conda.anaconda.org/conda-forge/linux-64/pycurl-7.44.1-py38h996a351_1.tar.bz2#782a335c4df1f9b00bea7b45ab18503b
-https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.18.1-py38h497a2fe_0.tar.bz2#2e21e97d12a98b0cd1b76cd475579921
-https://conda.anaconda.org/conda-forge/linux-64/pysocks-1.7.1-py38h578d9bd_4.tar.bz2#9c4bbee6f682f2fc7d7803df3996e77e
-https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/linux-64/pyzmq-22.3.0-py38h2035c66_1.tar.bz2#3938fa672dbd1762f9134b2026aebadc
-https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.6-py38h497a2fe_0.tar.bz2#bfcfe5dc66dcc3793fdb439fd0e13788
-https://conda.anaconda.org/conda-forge/linux-64/setuptools-60.5.0-py38h578d9bd_0.tar.bz2#9807c89f3ce846015dbad3c1d04348a5
-https://conda.anaconda.org/conda-forge/linux-64/sniffio-1.2.0-py38h578d9bd_2.tar.bz2#f3551ed88243d9b21494571e3c10e049
-https://conda.anaconda.org/conda-forge/linux-64/tornado-6.1-py38h497a2fe_2.tar.bz2#63b3b55c98b4239134e0be080f448944
-https://conda.anaconda.org/conda-forge/linux-64/typed-ast-1.5.2-py38h497a2fe_0.tar.bz2#082946878c5af9960bb639d993e3cda6
-https://conda.anaconda.org/conda-forge/linux-64/anyio-3.5.0-py38h578d9bd_0.tar.bz2#586fdb2fe49a3aa161060608c2707b0d
-https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py38h497a2fe_1.tar.bz2#0f28a4d17fcad4332e6eb17d7ce2a2f3
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/linux-64/y-py-0.5.9-py39h50f1755_0.conda#f9225a09f5cb046cfdecd2a54448d4c0
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
+https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
+https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
-https://conda.anaconda.org/conda-forge/noarch/black-21.12b0-pyhd8ed1ab_0.tar.bz2#a027de51692086f51b9e17735480bebf
-https://conda.anaconda.org/conda-forge/noarch/bleach-4.1.0-pyhd8ed1ab_0.tar.bz2#4a2104c7b22c222bd0fe03aaef12862c
-https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py38h497a2fe_1003.tar.bz2#9189b42c42b9c87b2b2068cbe31901a8
-https://conda.anaconda.org/conda-forge/linux-64/cryptography-36.0.1-py38h3e25421_0.tar.bz2#acc14d0d71dbf74f6a15f2456951b6cf
-https://conda.anaconda.org/conda-forge/noarch/jinja2-3.0.3-pyhd8ed1ab_0.tar.bz2#036d872c653780cb26e797e2e2f61b4c
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.4.0-pyhd8ed1ab_0.tar.bz2#17ec41acce882e5db4efdcc4c01ca7e0
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-7.1.2-pyhd8ed1ab_0.tar.bz2#9a332b6f8f05629435ce59032df8cfa9
-https://conda.anaconda.org/conda-forge/noarch/mako-1.1.6-pyhd8ed1ab_0.tar.bz2#cb952a55037148f6a5ddd9770ee1384f
-https://conda.anaconda.org/conda-forge/noarch/pip-21.3.1-pyhd8ed1ab_0.tar.bz2#e4fe2a9af78ff11f1aced7e62128c6a8
-https://conda.anaconda.org/conda-forge/noarch/pygments-2.11.2-pyhd8ed1ab_0.tar.bz2#caef60540e2239e27bf62569a5015e3b
-https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.19-py38h497a2fe_0.tar.bz2#694f44b2bd19da8011352ff359f30b76
-https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-1.4.31-py38h497a2fe_0.tar.bz2#2c8a6dd6ec5d18fb55f43a65b83e0d8e
-https://conda.anaconda.org/conda-forge/noarch/stack_data-0.1.4-pyhd8ed1ab_0.tar.bz2#e68dcab1b415c3c44be2a51d7d41e921
-https://conda.anaconda.org/conda-forge/linux-64/terminado-0.12.1-py38h578d9bd_1.tar.bz2#7895939107a904267a9e5f9678c9b27f
-https://conda.anaconda.org/conda-forge/noarch/alembic-1.7.5-pyhd8ed1ab_0.tar.bz2#1102908123392ffc63c01caea136b1d4
+https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
+https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
+https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py39he91dace_3.conda#20080319ef73fbad74dcd6d62f2a3ffe
+https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
+https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
+https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
+https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
+https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.31-py39hd1e30aa_0.conda#bb9509b491be59807c5c935516b223f2
+https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_0.conda#ae465d0fbf9f1979cb2d8d4043d885e2
+https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
+https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py39hb9d737c_3.tar.bz2#4df2495b3be6785029856ab326b949ea
+https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.1-py39hd4f0224_0.conda#977858e1c3a33c7f3770c50691ce751b
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
+https://conda.anaconda.org/conda-forge/noarch/mako-1.2.4-pyhd8ed1ab_0.tar.bz2#0d072f0edc017b6318dbab701e053f94
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
+https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.15-py39hd1e30aa_0.conda#62cb91b2ed1b8c72553b98a1f338ab3e
+https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
+https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
+https://conda.anaconda.org/conda-forge/noarch/alembic-1.11.1-pyhd8ed1ab_0.conda#6a55e123397b42b79c48b31d1b7a91b8
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
+https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.0-py39hf3d152e_0.conda#09aafa6fee56aab97695c6a70194f5e5
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/jupyter_telemetry-0.1.0-pyhd8ed1ab_1.tar.bz2#bb9ebdb6d5aa2622484aff1faceee181
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.1.2-pyh9f0ad1d_0.tar.bz2#2cbd910890bb328e8959246a1e16fac7
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.1.3-pyhd8ed1ab_0.tar.bz2#bafa5df6d4f8db69a4d197b4657127e7
-https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.1.1-pyhd8ed1ab_0.tar.bz2#34bb0b023e083aa8a4af74311031a352
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-21.0.0-pyhd8ed1ab_0.tar.bz2#8c49efecb7dca466e18b06015e8c88ce
-https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.5-pyh9f0ad1d_2.tar.bz2#5266fcd697043c59621fda522b3d78ee
+https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
+https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.2-pyhd8ed1ab_0.tar.bz2#8f882b197fd9c4941a787926baea4868
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
+https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/certipy-0.1.3-py_0.tar.bz2#23486713ef5712923e7c57cae609b22e
-https://conda.anaconda.org/conda-forge/noarch/nbclient-0.5.10-pyhd8ed1ab_1.tar.bz2#000cfe33d6fa746c5a9d1b29a79342a3
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.24-pyha770c72_0.tar.bz2#edaf527a6d394e2b965aff228c2e552f
-https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.8-pyhd8ed1ab_1.tar.bz2#53f1387c68c21cecb386e2cde51b3f7c
-https://conda.anaconda.org/conda-forge/linux-64/ipython-8.0.1-py38h578d9bd_0.tar.bz2#d0eb7c0e84fc4a9222321840b7ff74a3
-https://conda.anaconda.org/conda-forge/linux-64/nbconvert-6.0.7-py38h578d9bd_3.tar.bz2#7d0922152b769b5489407f90e84562a6
-https://conda.anaconda.org/conda-forge/noarch/requests-2.27.1-pyhd8ed1ab_0.tar.bz2#7c1c427246b057b8fa97200ecdb2ed62
-https://conda.anaconda.org/conda-forge/linux-64/ipykernel-6.7.0-py38he5a9106_0.tar.bz2#4ef8df702308288d7abe1358395988c6
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-1.13.4-pyhd8ed1ab_0.tar.bz2#70c6e1f755731d858767cb3c08c56a95
-https://conda.anaconda.org/conda-forge/linux-64/jupyterhub-base-1.4.2-py38h578d9bd_0.tar.bz2#3525d4ef3ef2ca54bd7173b5d91a57af
-https://conda.anaconda.org/conda-forge/noarch/jupyter-resource-usage-0.6.1-pyhd8ed1ab_0.tar.bz2#a35cb988cd5b9b9b2d1c6179a8a86974
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.10.3-pyhd8ed1ab_0.tar.bz2#65d62a616bed5237b85b9e2a88378ec0
-https://conda.anaconda.org/conda-forge/noarch/notebook-6.3.0-pyha770c72_1.tar.bz2#6a53111a5a62d32abfa21aac8fc55a1b
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
+https://conda.anaconda.org/conda-forge/noarch/jupyterhub-base-3.1.1-pyh2a2186d_0.conda#78fc5dfd4577a7ba172fa65eb64b6afb
+https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh210e3f2_0.conda#4b57b688e22d094d1479a35543c18e93
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-1.23.6-pyhd8ed1ab_0.conda#5016f7c6845a6efd270fcee63af9a2a0
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.4.0-pyhd8ed1ab_0.conda#127c702e1b1eff595be82bc6a78cfce0
+https://conda.anaconda.org/conda-forge/noarch/jupyter-resource-usage-0.7.1-pyhd8ed1ab_0.conda#62ed54dc748d19d0cf056a3f90cc8f12
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.4.0-pyhd8ed1ab_0.conda#a86727968b41c20dd3d73b91632e77dc
+https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
+https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
+https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
 https://conda.anaconda.org/conda-forge/noarch/jupyter-offlinenotebook-0.2.2-pyh1d7be83_0.tar.bz2#fe55056ce4bc4bd4953ba440270735fb
-https://conda.anaconda.org/conda-forge/linux-64/jupyterhub-singleuser-1.4.2-py38h578d9bd_0.tar.bz2#1ec75ee653e8a5eeaf8ff2f73f8a774e
-https://conda.anaconda.org/conda-forge/noarch/nbclassic-0.3.5-pyhd8ed1ab_0.tar.bz2#e9e2281b7dc08d876fc789af0f571ade
-https://conda.anaconda.org/conda-forge/noarch/nteract_on_jupyter-2.1.3-py_0.tar.bz2#1430ccd983ae6b161e2fbf4377965f7a
-https://conda.anaconda.org/conda-forge/linux-64/widgetsnbextension-3.5.2-py38h578d9bd_1.tar.bz2#65b76030f93500b2d2866404c9dc1ac9
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-7.6.5-pyhd8ed1ab_0.tar.bz2#6f2ee1ec157104df141e2e5afeba98d4
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.2.8-pyhd8ed1ab_0.tar.bz2#e2cc0671571f14af58f832c912dee025
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.4-pyhd8ed1ab_0.conda#e66d4a6e36fcc92fe266932bf85fd35a
+https://conda.anaconda.org/conda-forge/noarch/jupyterhub-singleuser-3.1.1-pyh2a2186d_0.conda#6d0a3394efe9ff7c0ad1ed03a6ca3720
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/environment.py-3.9.lock` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/environment.py-3.10-linux-64.lock`

 * *Files 14% similar despite different names*

```diff
@@ -1,155 +1,167 @@
-# AUTO GENERATED FROM environment.py-3.9.yml, DO NOT MANUALLY MODIFY
-# Frozen on 2022-01-26 18:37:30 UTC
+# AUTO GENERATED FROM environment.py-3.10.yml, DO NOT MANUALLY MODIFY
+# Frozen on 2023-06-08 09:35:19 UTC
 # Generated by conda-lock.
 # platform: linux-64
-# input_hash: 26314177814dc09ebdfe9ad8cd35b257ebec964ae6e21918e0bfb7bf38675075
+# input_hash: 5e20d8617672faf1f048550dc6ffdcf6288c12f1faf23a9051314056a752d9f3
 @EXPLICIT
 https://conda.anaconda.org/conda-forge/linux-64/_libgcc_mutex-0.1-conda_forge.tar.bz2#d7c89558ba9fa0495403155b64376d81
-https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2021.10.8-ha878542_0.tar.bz2#575611b8a84f45960e87722eeb51fa26
-https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.36.1-hea4e1c9_2.tar.bz2#bd4f2e711b39af170e7ff15163fe87ee
-https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-11.2.0-he4da1e4_12.tar.bz2#7ff3b832ba5e6918c0d026976359d065
-https://conda.anaconda.org/conda-forge/linux-64/pandoc-2.17.0.1-h7f98852_0.tar.bz2#bd9fa82641da6dfe5696fd196e3c7cf1
-https://conda.anaconda.org/conda-forge/noarch/tzdata-2021e-he74cb21_0.tar.bz2#a751ec502589ebdc2eceb183ff602569
-https://conda.anaconda.org/conda-forge/linux-64/libgomp-11.2.0-h1d223b6_12.tar.bz2#763c5ec8116d984b4a33342236d7da36
-https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-1_gnu.tar.bz2#561e277319a41d4f24f5c05a9ef63c04
-https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-11.2.0-h1d223b6_12.tar.bz2#d34efbb8d7d6312c816b4bb647b818b1
+https://conda.anaconda.org/conda-forge/linux-64/ca-certificates-2023.5.7-hbcca054_0.conda#f5c65075fc34438d5b456c7f3f5ab695
+https://conda.anaconda.org/conda-forge/linux-64/ld_impl_linux-64-2.40-h41732ed_0.conda#7aca3059a1729aa76c597603f10b0dd3
+https://conda.anaconda.org/conda-forge/linux-64/libstdcxx-ng-13.1.0-hfd8a6a1_0.conda#067bcc23164642f4c226da631f2a2e1d
+https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.10-3_cp310.conda#4eb33d14d794b0f4be116443ffed3853
+https://conda.anaconda.org/conda-forge/noarch/tzdata-2023c-h71feb2d_0.conda#939e3e74d8be4dac89ce83b20de2492a
+https://conda.anaconda.org/conda-forge/linux-64/libgomp-13.1.0-he5830b7_0.conda#56ca14d57ac29a75d23a39eb3ee0ddeb
+https://conda.anaconda.org/conda-forge/linux-64/_openmp_mutex-4.5-2_gnu.tar.bz2#73aaf86a425cc6e73fcf236a5a46396d
+https://conda.anaconda.org/conda-forge/linux-64/libgcc-ng-13.1.0-he5830b7_0.conda#cd93f779ff018dd85c7544c015c9db3c
 https://conda.anaconda.org/conda-forge/linux-64/bzip2-1.0.8-h7f98852_4.tar.bz2#a1fd65c7ccbf10880423d82bca54eb54
-https://conda.anaconda.org/conda-forge/linux-64/c-ares-1.18.1-h7f98852_0.tar.bz2#f26ef8098fab1f719c91eb760d63381a
-https://conda.anaconda.org/conda-forge/linux-64/icu-69.1-h9c3ff4c_0.tar.bz2#e0773c9556d588b062a4e1424a6a02fa
-https://conda.anaconda.org/conda-forge/linux-64/libev-4.33-h516909a_1.tar.bz2#6f8720dff19e17ce5d48cfe7f3d2f0a3
+https://conda.anaconda.org/conda-forge/linux-64/icu-72.1-hcb278e6_0.conda#7c8d20d847bb45f56bd941578fcfa146
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlicommon-1.0.9-h166bdaf_8.tar.bz2#9194c9bf9428035a05352d031462eae4
 https://conda.anaconda.org/conda-forge/linux-64/libffi-3.4.2-h7f98852_5.tar.bz2#d645c6d2ac96843a2bfaccd2d62b3ac3
 https://conda.anaconda.org/conda-forge/linux-64/libnsl-2.0.0-h7f98852_0.tar.bz2#39b1328babf85c7c3a61636d9cd50206
 https://conda.anaconda.org/conda-forge/linux-64/libsodium-1.0.18-h36c2ea0_1.tar.bz2#c3788462a6fbddafdb413a9f9053e58d
-https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.32.1-h7f98852_1000.tar.bz2#772d69f030955d9646d3d0eaf21d859d
-https://conda.anaconda.org/conda-forge/linux-64/libuv-1.43.0-h7f98852_0.tar.bz2#b34d856aa7e06ebd79bded72ef4afc16
-https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.11-h36c2ea0_1013.tar.bz2#dcddf696ff5dfcab567100d691678e18
-https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.3-h9c3ff4c_0.tar.bz2#fb31bcb7af058244479ca635d20f0f4a
-https://conda.anaconda.org/conda-forge/linux-64/openssl-1.1.1l-h7f98852_0.tar.bz2#de7b38a1542dbe6f41653a8ae71adc53
-https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.5-h516909a_1.tar.bz2#33f601066901f3e1a85af3522a8113f9
-https://conda.anaconda.org/conda-forge/linux-64/libedit-3.1.20191231-he28a2e2_2.tar.bz2#4d331e44109e3f0e19b4cb8f9b82f3e1
-https://conda.anaconda.org/conda-forge/linux-64/readline-8.1-h46c0cb4_0.tar.bz2#5788de3c8d7a7d64ac56c784c4ef48e6
+https://conda.anaconda.org/conda-forge/linux-64/libuuid-2.38.1-h0b41bf4_0.conda#40b61aab5c7ba9ff276c41cfffe6b80b
+https://conda.anaconda.org/conda-forge/linux-64/libuv-1.44.2-h166bdaf_0.tar.bz2#e5cb4fe581a18ca2185a016eb848fc00
+https://conda.anaconda.org/conda-forge/linux-64/libzlib-1.2.13-h166bdaf_4.tar.bz2#f3f9de449d32ca9b9c66a22863c96f41
+https://conda.anaconda.org/conda-forge/linux-64/ncurses-6.4-hcb278e6_0.conda#681105bccc2a3f7f1a837d47d39c9179
+https://conda.anaconda.org/conda-forge/linux-64/openssl-3.1.1-hd590300_1.conda#2e1d7b458ac8f1e3ca4e18b77add6277
+https://conda.anaconda.org/conda-forge/linux-64/xz-5.2.6-h166bdaf_0.tar.bz2#2161070d867d1b1204ea749c8eec4ef0
+https://conda.anaconda.org/conda-forge/linux-64/yaml-0.2.5-h7f98852_2.tar.bz2#4cb3ad778ec2d5a7acbdf254eb1c42ae
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlidec-1.0.9-h166bdaf_8.tar.bz2#4ae4d7795d33e02bd20f6b23d91caf82
+https://conda.anaconda.org/conda-forge/linux-64/libbrotlienc-1.0.9-h166bdaf_8.tar.bz2#04bac51ba35ea023dc48af73c1c88c25
+https://conda.anaconda.org/conda-forge/linux-64/libsqlite-3.42.0-h2797004_0.conda#fdaae20a1cf7cd62130a0973190a31b7
+https://conda.anaconda.org/conda-forge/linux-64/pandoc-2.19.2-h32600fe_2.conda#326f46f36d15c44cff5f81d505cb717f
+https://conda.anaconda.org/conda-forge/linux-64/readline-8.2-h8228510_1.conda#47d31b792659ce70f470b5c82fdfb7a4
+https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.12-h27826a3_0.tar.bz2#5b8c42eb62e9fc961af70bdd6a26e168
 https://conda.anaconda.org/conda-forge/linux-64/zeromq-4.3.4-h9c3ff4c_1.tar.bz2#21743a8d2ea0c8cfbbf8fe489b0347df
-https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.11-h36c2ea0_1013.tar.bz2#cf7190238072a41e9579e4476a6a60b8
-https://conda.anaconda.org/conda-forge/linux-64/libnghttp2-1.43.0-h812cca2_1.tar.bz2#d0a7846b7b3b8fb0d8b36904a53b8155
-https://conda.anaconda.org/conda-forge/linux-64/libssh2-1.10.0-ha56f1ee_2.tar.bz2#6ab4eaa11ff01801cffca0a27489dc04
-https://conda.anaconda.org/conda-forge/linux-64/nodejs-14.18.3-h8ca31f7_2.tar.bz2#192a478a1ae899992e4afce84520badb
-https://conda.anaconda.org/conda-forge/linux-64/sqlite-3.37.0-h9cd32fc_0.tar.bz2#eb66fc098824d25518a79e83d12a81d6
-https://conda.anaconda.org/conda-forge/linux-64/tk-8.6.11-h27826a3_1.tar.bz2#84e76fb280e735fec1efd2d21fd9cb27
-https://conda.anaconda.org/conda-forge/linux-64/krb5-1.19.2-hcc1bbae_3.tar.bz2#e29650992ae593bc05fc93722483e5c3
-https://conda.anaconda.org/conda-forge/linux-64/python-3.9.9-h62f1059_0_cpython.tar.bz2#cecbf6a8fcdae14bf4a1036e5a35319e
+https://conda.anaconda.org/conda-forge/linux-64/zlib-1.2.13-h166bdaf_4.tar.bz2#4b11e365c0275b808be78b30f904e295
+https://conda.anaconda.org/conda-forge/linux-64/brotli-bin-1.0.9-h166bdaf_8.tar.bz2#e5613f2bc717e9945840ff474419b8e4
+https://conda.anaconda.org/conda-forge/linux-64/nodejs-18.15.0-h4abf6b9_1.conda#2aabafd88f6876a57c45c00598715ac4
+https://conda.anaconda.org/conda-forge/linux-64/python-3.10.11-he550d4f_0_cpython.conda#7439c9d24378a82b73a7a53868dacdf1
+https://conda.anaconda.org/conda-forge/noarch/aiofiles-22.1.0-pyhd8ed1ab_0.tar.bz2#a88c206fdb78e34adb1c4081f5f838dd
 https://conda.anaconda.org/conda-forge/noarch/async_generator-1.10-py_0.tar.bz2#d56c596e61b1c4952acf0a9920856c12
-https://conda.anaconda.org/conda-forge/noarch/attrs-21.4.0-pyhd8ed1ab_0.tar.bz2#f70280205d7044c8b8358c8de3190e5d
+https://conda.anaconda.org/conda-forge/noarch/attrs-23.1.0-pyh71513ae_1.conda#3edfead7cedd1ab4400a6c588f3e75f8
 https://conda.anaconda.org/conda-forge/noarch/backcall-0.2.0-pyh9f0ad1d_0.tar.bz2#6006a6d08a3fa99268a2681c7fb55213
-https://conda.anaconda.org/conda-forge/noarch/backports-1.0-py_2.tar.bz2#0da16b293affa6ac31812376f8eb79dd
-https://conda.anaconda.org/conda-forge/noarch/blinker-1.4-py_1.tar.bz2#fa509a09190583f869ae442bf4d17f5f
-https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-2.0.10-pyhd8ed1ab_0.tar.bz2#ea77236c8031cfa821720b21b4cb0ceb
-https://conda.anaconda.org/conda-forge/noarch/dataclasses-0.8-pyhc8e2a94_3.tar.bz2#a362b2124b06aad102e2ee4581acee7d
+https://conda.anaconda.org/conda-forge/noarch/backports-1.0-pyhd8ed1ab_3.conda#54ca2e08b3220c148a1d8329c2678e02
+https://conda.anaconda.org/conda-forge/noarch/blinker-1.6.2-pyhd8ed1ab_0.conda#2fb79ec81bad9492b6d59a06b3b647a4
+https://conda.anaconda.org/conda-forge/linux-64/brotli-1.0.9-h166bdaf_8.tar.bz2#2ff08978892a3e8b954397c461f18418
+https://conda.anaconda.org/conda-forge/noarch/certifi-2023.5.7-pyhd8ed1ab_0.conda#5d1b71c942b8421285934dad1d891ebc
+https://conda.anaconda.org/conda-forge/noarch/charset-normalizer-3.1.0-pyhd8ed1ab_0.conda#7fcff9f6f123696e940bda77bd4d6551
+https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.6.7-py310heca2aa9_0.conda#8ffb020d2b722c962f0b4f06a304f533
 https://conda.anaconda.org/conda-forge/noarch/decorator-5.1.1-pyhd8ed1ab_0.tar.bz2#43afe5ab04e35e17ba28649471dd7364
 https://conda.anaconda.org/conda-forge/noarch/defusedxml-0.7.1-pyhd8ed1ab_0.tar.bz2#961b3a227b437d82ad7054484cfa71b2
-https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.3-pyhd8ed1ab_1003.tar.bz2#bbf9a201f6ce99a506f4955374d9a9f4
-https://conda.anaconda.org/conda-forge/noarch/executing-0.8.2-pyhd8ed1ab_0.tar.bz2#dcd884e2cf5bcdccdf78f7db35999d62
-https://conda.anaconda.org/conda-forge/noarch/flit-core-3.6.0-pyhd8ed1ab_0.tar.bz2#f8c17f22a3ce533876c468157ff8ff8f
-https://conda.anaconda.org/conda-forge/noarch/idna-3.3-pyhd8ed1ab_0.tar.bz2#40b50b8b030f5f2f22085c062ed013dd
+https://conda.anaconda.org/conda-forge/noarch/entrypoints-0.4-pyhd8ed1ab_0.tar.bz2#3cf04868fee0a029769bd41f4b2fbf2d
+https://conda.anaconda.org/conda-forge/noarch/exceptiongroup-1.1.1-pyhd8ed1ab_0.conda#7312299d7a0ea4993159229b7d2dceb2
+https://conda.anaconda.org/conda-forge/noarch/executing-1.2.0-pyhd8ed1ab_0.tar.bz2#4c1bc140e2be5c8ba6e3acab99e25c50
+https://conda.anaconda.org/conda-forge/noarch/flit-core-3.9.0-pyhd8ed1ab_0.conda#e8cfceef004266b259604c3faa2a0191
+https://conda.anaconda.org/conda-forge/linux-64/greenlet-2.0.2-py310hc6cd4ac_1.conda#934c4eb3214284125eff6dd665e9568a
+https://conda.anaconda.org/conda-forge/noarch/idna-3.4-pyhd8ed1ab_0.tar.bz2#34272b248891bddccc64479f9a7fffed
 https://conda.anaconda.org/conda-forge/noarch/ipython_genutils-0.2.0-py_1.tar.bz2#5071c982548b3a20caf70462f04f5287
 https://conda.anaconda.org/conda-forge/noarch/json5-0.9.5-pyh9f0ad1d_0.tar.bz2#10759827a94e6b14996e81fb002c0bda
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-1.0.2-pyhd8ed1ab_0.tar.bz2#eaff56fe28d1236076aa3bb13c35b434
-https://conda.anaconda.org/conda-forge/linux-64/libcurl-7.81.0-h2574ce0_0.tar.bz2#1f8655741d0269ca6756f131522da1e8
-https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.4-pyhd8ed1ab_0.tar.bz2#0d86e4e6ac78912f3f47e0453b124aca
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_widgets-3.0.7-pyhd8ed1ab_1.conda#0c0a54e16b764bafcae35913cc9d60ff
+https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.1.3-py310h2372a71_0.conda#5597d9f9778af6883ae64f0e7d39416c
+https://conda.anaconda.org/conda-forge/noarch/mistune-2.0.5-pyhd8ed1ab_0.conda#61a07195cfc935f1c1901d8ecf4af441
+https://conda.anaconda.org/conda-forge/noarch/nest-asyncio-1.5.6-pyhd8ed1ab_0.tar.bz2#7b868f21adde0d9b8b38f9c16836589b
+https://conda.anaconda.org/conda-forge/noarch/packaging-23.1-pyhd8ed1ab_0.conda#91cda59e66e1e4afe9476f8ef98f5c30
 https://conda.anaconda.org/conda-forge/noarch/pamela-1.0.0-py_0.tar.bz2#36f6f18d2f3ae0c93d77a9dbedad08c3
 https://conda.anaconda.org/conda-forge/noarch/pandocfilters-1.5.0-pyhd8ed1ab_0.tar.bz2#457c2c8c08e54905d6954e79cb5b5db9
 https://conda.anaconda.org/conda-forge/noarch/parso-0.8.3-pyhd8ed1ab_0.tar.bz2#17a565a0c3899244e938cdf417e7b094
-https://conda.anaconda.org/conda-forge/noarch/pathspec-0.9.0-pyhd8ed1ab_0.tar.bz2#f93dc0ccbc0a8472624165f6e256c7d1
 https://conda.anaconda.org/conda-forge/noarch/pickleshare-0.7.5-py_1003.tar.bz2#415f0ebb6198cc2801c73438a9fb5761
-https://conda.anaconda.org/conda-forge/noarch/platformdirs-2.3.0-pyhd8ed1ab_0.tar.bz2#7bc119135be2a43e1701432399d8c28a
-https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.13.0-pyhd8ed1ab_0.tar.bz2#f5567b5e7a5abc9133f198b8356674d1
+https://conda.anaconda.org/conda-forge/noarch/pkgutil-resolve-name-1.3.10-pyhd8ed1ab_0.tar.bz2#89e3c7cdde7d3aaa2aee933b604dd07f
+https://conda.anaconda.org/conda-forge/noarch/prometheus_client-0.17.0-pyhd8ed1ab_0.conda#95c5be3c7cbd872509d16c216617fdab
+https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.5-py310h1fa729e_0.conda#b0f0a014fc04012c05f39df15fe270ce
 https://conda.anaconda.org/conda-forge/noarch/ptyprocess-0.7.0-pyhd3deb0d_0.tar.bz2#359eeb6536da0e687af562ed265ec263
 https://conda.anaconda.org/conda-forge/noarch/pure_eval-0.2.2-pyhd8ed1ab_0.tar.bz2#6784285c7e55cb7212efabc79e4c2883
 https://conda.anaconda.org/conda-forge/noarch/pycparser-2.21-pyhd8ed1ab_0.tar.bz2#076becd9e05608f8dc72757d5f3a91ff
-https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.3.0-pyhd8ed1ab_1.tar.bz2#b7bc0de380f114658af5fe57cebdcd9e
-https://conda.anaconda.org/conda-forge/noarch/pyparsing-3.0.7-pyhd8ed1ab_0.tar.bz2#727e2216d9c47455d8ddc060eb2caad9
-https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.1-pyh9f0ad1d_0.tar.bz2#aed452f2f9f8bc8b2b0c412975051b5b
-https://conda.anaconda.org/conda-forge/linux-64/python_abi-3.9-2_cp39.tar.bz2#39adde4247484de2bb4000122fdcf665
-https://conda.anaconda.org/conda-forge/noarch/pytz-2021.3-pyhd8ed1ab_0.tar.bz2#7e4f811bff46a5a6a7e0094921389395
-https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.0-pyhd8ed1ab_0.tar.bz2#edab14119efe85c3bf131ad747e9005c
+https://conda.anaconda.org/conda-forge/noarch/pygments-2.15.1-pyhd8ed1ab_0.conda#d316679235612869eba305aa7d41d9bf
+https://conda.anaconda.org/conda-forge/noarch/pyjwt-2.7.0-pyhd8ed1ab_0.conda#99e28be5a278e2319834d7dc99e7bfdd
+https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.19.3-py310h1fa729e_0.conda#f732bec05ecc2e302a868d971ae484e0
+https://conda.anaconda.org/conda-forge/noarch/pysocks-1.7.1-pyha2e5f31_6.tar.bz2#2a7de29fb590ca14b5243c4c812c8025
+https://conda.anaconda.org/conda-forge/noarch/python-fastjsonschema-2.17.1-pyhd8ed1ab_0.conda#dd4f393d857e9283eef2442234bd05e3
+https://conda.anaconda.org/conda-forge/noarch/python-json-logger-2.0.7-pyhd8ed1ab_0.conda#a61bf9ec79426938ff785eb69dbb1960
+https://conda.anaconda.org/conda-forge/noarch/pytz-2023.3-pyhd8ed1ab_0.conda#d3076b483092a435832603243567bc31
+https://conda.anaconda.org/conda-forge/linux-64/pyyaml-6.0-py310h5764c6d_5.tar.bz2#9e68d2ff6d98737c855b65f48dd3c597
+https://conda.anaconda.org/conda-forge/linux-64/pyzmq-25.1.0-py310h5bbb5d0_0.conda#58017b4bb8fec6088a8b9ae44744ce4b
+https://conda.anaconda.org/conda-forge/noarch/rfc3986-validator-0.1.1-pyh9f0ad1d_0.tar.bz2#912a71cc01012ee38e6b90ddd561e36f
+https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.7-py310h1fa729e_1.conda#2f9b517412af46255cef5e53a22c264e
+https://conda.anaconda.org/conda-forge/noarch/send2trash-1.8.2-pyh41d4057_0.conda#ada5a17adcd10be4fc7e37e4166ba0e2
+https://conda.anaconda.org/conda-forge/noarch/setuptools-67.7.2-pyhd8ed1ab_0.conda#3b68bc43ec6baa48f7354a446267eefe
 https://conda.anaconda.org/conda-forge/noarch/six-1.16.0-pyh6c4a22f_0.tar.bz2#e5f25f8dbc060e9a8d912e432202afc2
-https://conda.anaconda.org/conda-forge/noarch/testpath-0.5.0-pyhd8ed1ab_0.tar.bz2#53b57d6a468bebc7cef1253b177a5e9e
-https://conda.anaconda.org/conda-forge/noarch/tomli-1.2.2-pyhd8ed1ab_0.tar.bz2#1c8a2f9ea18c267414e244cee668cd00
-https://conda.anaconda.org/conda-forge/noarch/traitlets-5.1.1-pyhd8ed1ab_0.tar.bz2#a1bc9765ef9499760e88f568b3a6622c
-https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.0.1-pyha770c72_0.tar.bz2#1fc03816925d3cb7fdab9ab234e7fea7
+https://conda.anaconda.org/conda-forge/noarch/sniffio-1.3.0-pyhd8ed1ab_0.tar.bz2#dd6cbc539e74cb1f430efbd4575b9303
+https://conda.anaconda.org/conda-forge/noarch/soupsieve-2.3.2.post1-pyhd8ed1ab_0.tar.bz2#146f4541d643d48fc8a75cacf69f03ae
+https://conda.anaconda.org/conda-forge/noarch/tomli-2.0.1-pyhd8ed1ab_0.tar.bz2#5844808ffab9ebdb694585b50ba02a96
+https://conda.anaconda.org/conda-forge/linux-64/tornado-6.3.2-py310h2372a71_0.conda#1c510e74c87dc9b8fe1f7f9e8dbcef96
+https://conda.anaconda.org/conda-forge/noarch/traitlets-5.9.0-pyhd8ed1ab_0.conda#d0b4f5c87cd35ac3fb3d47b223263a64
+https://conda.anaconda.org/conda-forge/noarch/typing_extensions-4.6.3-pyha770c72_0.conda#4a3014a4d107d15475d106b751c4e352
 https://conda.anaconda.org/conda-forge/noarch/webencodings-0.5.1-py_1.tar.bz2#3563be4c5611a44210d9ba0c16113136
-https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.2.3-pyhd8ed1ab_0.tar.bz2#a9e89668df0da0f33c8c4ddf7c118f6d
-https://conda.anaconda.org/conda-forge/noarch/wheel-0.37.1-pyhd8ed1ab_0.tar.bz2#1ca02aaf78d9c70d9a81a3bed5752022
-https://conda.anaconda.org/conda-forge/noarch/zipp-3.7.0-pyhd8ed1ab_0.tar.bz2#947f7f41958eabc0f6e886557512bb76
-https://conda.anaconda.org/conda-forge/noarch/asttokens-2.0.5-pyhd8ed1ab_0.tar.bz2#74badce16f060701fee55c39332f5253
-https://conda.anaconda.org/conda-forge/noarch/babel-2.9.1-pyh44b312d_0.tar.bz2#74136ed39bfea0832d338df1e58d013e
-https://conda.anaconda.org/conda-forge/linux-64/certifi-2021.10.8-py39hf3d152e_1.tar.bz2#67982d98030fde9139a64219dbe4db5e
-https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.0-py39h4bc2ebd_0.tar.bz2#f6191bf565dee581e77549d63737751c
-https://conda.anaconda.org/conda-forge/linux-64/click-8.0.3-py39hf3d152e_1.tar.bz2#30b637487f64a02e32591c667047cf08
-https://conda.anaconda.org/conda-forge/linux-64/debugpy-1.5.1-py39he80948d_0.tar.bz2#111c5b430676182de0f0f038233ba3a4
-https://conda.anaconda.org/conda-forge/linux-64/greenlet-1.1.2-py39he80948d_1.tar.bz2#4b440bda7b4cca6303c6dd9c04cb9fc9
-https://conda.anaconda.org/conda-forge/linux-64/importlib-metadata-4.10.1-py39hf3d152e_0.tar.bz2#b39133cc0b0fc1cd13a239e85be5caee
-https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.4.0-pyhd8ed1ab_0.tar.bz2#9fb134dbabe7851a9d71411064b2c30d
-https://conda.anaconda.org/conda-forge/linux-64/jedi-0.18.1-py39hf3d152e_0.tar.bz2#4a03392442a5ba884c186f25281ef8a1
-https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-4.9.1-py39hf3d152e_1.tar.bz2#e9b6677fca1aa658d98deba00fb89267
-https://conda.anaconda.org/conda-forge/linux-64/markupsafe-2.0.1-py39h3811e60_1.tar.bz2#bba8fc0d724caa73a96220e48aac3b61
-https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.3-pyhd8ed1ab_0.tar.bz2#be3bfd435802d2c768c6b2439f325f3d
-https://conda.anaconda.org/conda-forge/linux-64/mistune-0.8.4-py39h3811e60_1005.tar.bz2#95eb8cbf40bccdcb34888c9e56371570
-https://conda.anaconda.org/conda-forge/linux-64/mypy_extensions-0.4.3-py39hf3d152e_4.tar.bz2#1778f314bd13102e3a1627280cb8ac79
-https://conda.anaconda.org/conda-forge/noarch/packaging-21.3-pyhd8ed1ab_0.tar.bz2#71f1ab2de48613876becddd496371c85
-https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh9f0ad1d_2.tar.bz2#5909e7b978141dd80d28dbf9de627827
-https://conda.anaconda.org/conda-forge/linux-64/psutil-5.9.0-py39h3811e60_0.tar.bz2#3eebabdf4f0bf1d94a97b67263196868
-https://conda.anaconda.org/conda-forge/linux-64/pycurl-7.44.1-py39h72e3413_1.tar.bz2#f3fa6db2ea8983102beb98d87eb85c0b
-https://conda.anaconda.org/conda-forge/linux-64/pyrsistent-0.18.1-py39h3811e60_0.tar.bz2#ed156d752c577f4e9b62159d5aac8557
-https://conda.anaconda.org/conda-forge/linux-64/pysocks-1.7.1-py39hf3d152e_4.tar.bz2#eed9d381f391cad4e96f697e8c74e929
-https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
-https://conda.anaconda.org/conda-forge/linux-64/pyzmq-22.3.0-py39h37b5a0c_1.tar.bz2#90dbe11c01a89fc6fddb90cbe2672e68
-https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml.clib-0.2.6-py39h3811e60_0.tar.bz2#0f9bbd7b79db72e3bc9779432de26427
-https://conda.anaconda.org/conda-forge/linux-64/setuptools-60.5.0-py39hf3d152e_0.tar.bz2#25c23d6577edd40d60ce4e022f407118
-https://conda.anaconda.org/conda-forge/linux-64/sniffio-1.2.0-py39hf3d152e_2.tar.bz2#591e48c37143ef758d6ba0da1cf10a6f
-https://conda.anaconda.org/conda-forge/linux-64/tornado-6.1-py39h3811e60_2.tar.bz2#5a7bb7af2f3bcf31ee6cd817de1d5011
-https://conda.anaconda.org/conda-forge/linux-64/typed-ast-1.5.2-py39h3811e60_0.tar.bz2#f26209afd5f3cb9adbf46002061f6214
-https://conda.anaconda.org/conda-forge/linux-64/anyio-3.5.0-py39hf3d152e_0.tar.bz2#b0d75a9d3fd02ec079504aabb7cd7ec3
-https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py39h3811e60_1.tar.bz2#6770ac3b1842046fcb21c2178d67fa32
+https://conda.anaconda.org/conda-forge/noarch/websocket-client-1.5.2-pyhd8ed1ab_0.conda#bfe7e7cd1476092f51efbcde15dfb110
+https://conda.anaconda.org/conda-forge/noarch/wheel-0.40.0-pyhd8ed1ab_0.conda#49bb0d9e60ce1db25e151780331bb5f3
+https://conda.anaconda.org/conda-forge/noarch/widgetsnbextension-4.0.7-pyhd8ed1ab_0.conda#bcc54b91a8ce88f60f538b87b409909e
+https://conda.anaconda.org/conda-forge/linux-64/y-py-0.5.9-py310h4426083_0.conda#0b3145258baa17d4405c3800a308da99
+https://conda.anaconda.org/conda-forge/noarch/zipp-3.15.0-pyhd8ed1ab_0.conda#13018819ca8f5b7cc675a8faf1f5fedf
+https://conda.anaconda.org/conda-forge/noarch/anyio-3.7.0-pyhd8ed1ab_1.conda#2b35a85d654a47aac8f34c1bb6de7142
+https://conda.anaconda.org/conda-forge/noarch/asttokens-2.2.1-pyhd8ed1ab_0.conda#bf7f54dd0f25c3f06ecb82a07341841a
+https://conda.anaconda.org/conda-forge/noarch/babel-2.12.1-pyhd8ed1ab_1.conda#ac432e732804a81ddcf29c92ead57cde
 https://conda.anaconda.org/conda-forge/noarch/backports.functools_lru_cache-1.6.4-pyhd8ed1ab_0.tar.bz2#c5b3edc62d6309088f4970b3eaaa65a6
-https://conda.anaconda.org/conda-forge/noarch/black-21.12b0-pyhd8ed1ab_0.tar.bz2#a027de51692086f51b9e17735480bebf
-https://conda.anaconda.org/conda-forge/noarch/bleach-4.1.0-pyhd8ed1ab_0.tar.bz2#4a2104c7b22c222bd0fe03aaef12862c
-https://conda.anaconda.org/conda-forge/linux-64/brotlipy-0.7.0-py39h3811e60_1003.tar.bz2#9b1975f772d5d8a398c34e539a7ea1a1
-https://conda.anaconda.org/conda-forge/linux-64/cryptography-36.0.1-py39h95dcef6_0.tar.bz2#986821383dd9622121c1a0b8a745b1e2
-https://conda.anaconda.org/conda-forge/noarch/jinja2-3.0.3-pyhd8ed1ab_0.tar.bz2#036d872c653780cb26e797e2e2f61b4c
-https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.4.0-pyhd8ed1ab_0.tar.bz2#17ec41acce882e5db4efdcc4c01ca7e0
-https://conda.anaconda.org/conda-forge/noarch/jupyter_client-7.1.2-pyhd8ed1ab_0.tar.bz2#9a332b6f8f05629435ce59032df8cfa9
-https://conda.anaconda.org/conda-forge/noarch/mako-1.1.6-pyhd8ed1ab_0.tar.bz2#cb952a55037148f6a5ddd9770ee1384f
-https://conda.anaconda.org/conda-forge/noarch/pip-21.3.1-pyhd8ed1ab_0.tar.bz2#e4fe2a9af78ff11f1aced7e62128c6a8
-https://conda.anaconda.org/conda-forge/noarch/pygments-2.11.2-pyhd8ed1ab_0.tar.bz2#caef60540e2239e27bf62569a5015e3b
-https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.19-py39h3811e60_0.tar.bz2#5e50592662d6b781b7c42fdb4c434e83
-https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-1.4.31-py39h3811e60_0.tar.bz2#16995a401ab29510c6e7665c9aff030f
-https://conda.anaconda.org/conda-forge/noarch/stack_data-0.1.4-pyhd8ed1ab_0.tar.bz2#e68dcab1b415c3c44be2a51d7d41e921
-https://conda.anaconda.org/conda-forge/linux-64/terminado-0.12.1-py39hf3d152e_1.tar.bz2#3e73d7571460790b8487d03b630b970b
-https://conda.anaconda.org/conda-forge/noarch/alembic-1.7.5-pyhd8ed1ab_0.tar.bz2#1102908123392ffc63c01caea136b1d4
+https://conda.anaconda.org/conda-forge/noarch/beautifulsoup4-4.12.2-pyha770c72_0.conda#a362ff7d976217f8fa78c0f1c4f59717
+https://conda.anaconda.org/conda-forge/noarch/bleach-6.0.0-pyhd8ed1ab_0.conda#d48b143d01385872a88ef8417e96c30e
+https://conda.anaconda.org/conda-forge/linux-64/cffi-1.15.1-py310h255011f_3.conda#800596144bb613cd7ac58b80900ce835
+https://conda.anaconda.org/conda-forge/noarch/comm-0.1.3-pyhd8ed1ab_0.conda#168ae0f82cdf7505048e81054c7354e4
+https://conda.anaconda.org/conda-forge/noarch/importlib-metadata-6.6.0-pyha770c72_0.conda#f91a5d5175fb7ff2a91952ec7da59cb9
+https://conda.anaconda.org/conda-forge/noarch/importlib_resources-5.12.0-pyhd8ed1ab_0.conda#e5fd2260a231ee63b6969f4801082f2b
+https://conda.anaconda.org/conda-forge/noarch/jedi-0.18.2-pyhd8ed1ab_0.conda#b5e695ef9c3f0d27d6cd96bf5adc9e07
+https://conda.anaconda.org/conda-forge/noarch/jinja2-3.1.2-pyhd8ed1ab_1.tar.bz2#c8490ed5c70966d232fdd389d0dbed37
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.2.2-pyhd8ed1ab_0.tar.bz2#243f63592c8e449f40cd42eb5cf32f40
+https://conda.anaconda.org/conda-forge/noarch/matplotlib-inline-0.1.6-pyhd8ed1ab_0.tar.bz2#b21613793fcc81d944c76c9f2864a7de
+https://conda.anaconda.org/conda-forge/noarch/pexpect-4.8.0-pyh1a96a4e_2.tar.bz2#330448ce4403cc74990ac07c555942a1
+https://conda.anaconda.org/conda-forge/noarch/pip-23.1.2-pyhd8ed1ab_0.conda#7288da0d36821349cf1126e8670292df
+https://conda.anaconda.org/conda-forge/noarch/python-dateutil-2.8.2-pyhd8ed1ab_0.tar.bz2#dd999d1cc9f79e67dbb855c8924c7984
+https://conda.anaconda.org/conda-forge/noarch/rfc3339-validator-0.1.4-pyhd8ed1ab_0.tar.bz2#fed45fc5ea0813240707998abe49f520
+https://conda.anaconda.org/conda-forge/linux-64/ruamel.yaml-0.17.31-py310h2372a71_0.conda#41e89112e1ec653fb3e62240d06a0e61
+https://conda.anaconda.org/conda-forge/noarch/terminado-0.17.1-pyh41d4057_0.conda#3788984d535770cad699efaeb6cb3037
+https://conda.anaconda.org/conda-forge/noarch/tinycss2-1.2.1-pyhd8ed1ab_0.tar.bz2#7234c9eefff659501cd2fe0d2ede4d48
+https://conda.anaconda.org/conda-forge/noarch/typing-extensions-4.6.3-hd8ed1ab_0.conda#3876f650ed7d0f95d70fa4b647621909
+https://conda.anaconda.org/conda-forge/noarch/urllib3-2.0.3-pyhd8ed1ab_0.conda#ae465d0fbf9f1979cb2d8d4043d885e2
+https://conda.anaconda.org/conda-forge/noarch/aiosqlite-0.19.0-pyhd8ed1ab_0.conda#c60a47f9f29057417165a8af579396a8
+https://conda.anaconda.org/conda-forge/linux-64/argon2-cffi-bindings-21.2.0-py310h5764c6d_3.tar.bz2#12f70cd23e4ea88f913dba50b0f0aba0
+https://conda.anaconda.org/conda-forge/linux-64/cryptography-41.0.1-py310h75e40e8_0.conda#bd5501a8ae0df5ef36b9ed03035ebe3a
+https://conda.anaconda.org/conda-forge/noarch/importlib_metadata-6.6.0-hd8ed1ab_0.conda#3cbc9615f10a3d471532b83e4250b971
+https://conda.anaconda.org/conda-forge/noarch/jsonschema-4.17.3-pyhd8ed1ab_0.conda#723268a468177cd44568eb8f794e0d80
+https://conda.anaconda.org/conda-forge/noarch/mako-1.2.4-pyhd8ed1ab_0.tar.bz2#0d072f0edc017b6318dbab701e053f94
+https://conda.anaconda.org/conda-forge/noarch/platformdirs-3.5.1-pyhd8ed1ab_0.conda#e2be672aece1f060adf7154f76531a35
+https://conda.anaconda.org/conda-forge/noarch/requests-2.31.0-pyhd8ed1ab_0.conda#a30144e4156cdbb236f99ebb49828f8b
+https://conda.anaconda.org/conda-forge/linux-64/sqlalchemy-2.0.15-py310h2372a71_0.conda#90322c707f2ad4eebb8438408b1ffa4e
+https://conda.anaconda.org/conda-forge/noarch/stack_data-0.6.2-pyhd8ed1ab_0.conda#e7df0fdd404616638df5ece6e69ba7af
+https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.6-pyhd8ed1ab_0.conda#078979d33523cb477bd1916ce41aacc9
+https://conda.anaconda.org/conda-forge/noarch/alembic-1.11.1-pyhd8ed1ab_0.conda#6a55e123397b42b79c48b31d1b7a91b8
 https://conda.anaconda.org/conda-forge/noarch/argon2-cffi-21.3.0-pyhd8ed1ab_0.tar.bz2#a0b402db58f73aaab8ee0ca1025a362e
+https://conda.anaconda.org/conda-forge/linux-64/jupyter_core-5.3.0-py310hff52083_0.conda#49428e10aae69baa6b34cb7e275f1ae9
+https://conda.anaconda.org/conda-forge/noarch/jupyter_events-0.6.3-pyhd8ed1ab_0.conda#d98c5196ab6ffeb0c2feca2912801353
 https://conda.anaconda.org/conda-forge/noarch/jupyter_telemetry-0.1.0-pyhd8ed1ab_1.tar.bz2#bb9ebdb6d5aa2622484aff1faceee181
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_pygments-0.1.2-pyh9f0ad1d_0.tar.bz2#2cbd910890bb328e8959246a1e16fac7
-https://conda.anaconda.org/conda-forge/noarch/nbformat-5.1.3-pyhd8ed1ab_0.tar.bz2#bafa5df6d4f8db69a4d197b4657127e7
-https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.1.1-pyhd8ed1ab_0.tar.bz2#34bb0b023e083aa8a4af74311031a352
-https://conda.anaconda.org/conda-forge/noarch/pyopenssl-21.0.0-pyhd8ed1ab_0.tar.bz2#8c49efecb7dca466e18b06015e8c88ce
-https://conda.anaconda.org/conda-forge/noarch/wcwidth-0.2.5-pyh9f0ad1d_2.tar.bz2#5266fcd697043c59621fda522b3d78ee
+https://conda.anaconda.org/conda-forge/noarch/jupyter_ydoc-0.2.4-pyhd8ed1ab_0.conda#be5d4633c1cc40343ed417153a184006
+https://conda.anaconda.org/conda-forge/noarch/oauthlib-3.2.2-pyhd8ed1ab_0.tar.bz2#8f882b197fd9c4941a787926baea4868
+https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.38-pyha770c72_0.conda#59ba1bf8ea558751a0d391249a248765
+https://conda.anaconda.org/conda-forge/noarch/pyopenssl-23.2.0-pyhd8ed1ab_1.conda#34f7d568bf59d18e3fef8c405cbece21
+https://conda.anaconda.org/conda-forge/noarch/ypy-websocket-0.8.2-pyhd8ed1ab_0.conda#5ee5ad3af20138020065985de57f0711
 https://conda.anaconda.org/conda-forge/noarch/certipy-0.1.3-py_0.tar.bz2#23486713ef5712923e7c57cae609b22e
-https://conda.anaconda.org/conda-forge/noarch/nbclient-0.5.10-pyhd8ed1ab_1.tar.bz2#000cfe33d6fa746c5a9d1b29a79342a3
-https://conda.anaconda.org/conda-forge/noarch/prompt-toolkit-3.0.24-pyha770c72_0.tar.bz2#edaf527a6d394e2b965aff228c2e552f
-https://conda.anaconda.org/conda-forge/noarch/urllib3-1.26.8-pyhd8ed1ab_1.tar.bz2#53f1387c68c21cecb386e2cde51b3f7c
-https://conda.anaconda.org/conda-forge/linux-64/ipython-8.0.1-py39hf3d152e_0.tar.bz2#d84d046c9dbdfe7b1b1b722e6369daab
-https://conda.anaconda.org/conda-forge/linux-64/nbconvert-6.0.7-py39hf3d152e_3.tar.bz2#5f914e1113c7a926798c7659efbcd6a3
-https://conda.anaconda.org/conda-forge/noarch/requests-2.27.1-pyhd8ed1ab_0.tar.bz2#7c1c427246b057b8fa97200ecdb2ed62
-https://conda.anaconda.org/conda-forge/linux-64/ipykernel-6.7.0-py39hef51801_0.tar.bz2#673ae0bc269066e8ddabc7c912739e79
-https://conda.anaconda.org/conda-forge/noarch/jupyter_server-1.13.4-pyhd8ed1ab_0.tar.bz2#70c6e1f755731d858767cb3c08c56a95
-https://conda.anaconda.org/conda-forge/linux-64/jupyterhub-base-1.4.2-py39hf3d152e_0.tar.bz2#07d2be5eb6460d504a0291cb2aa8328a
-https://conda.anaconda.org/conda-forge/noarch/jupyter-resource-usage-0.6.1-pyhd8ed1ab_0.tar.bz2#a35cb988cd5b9b9b2d1c6179a8a86974
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.10.3-pyhd8ed1ab_0.tar.bz2#65d62a616bed5237b85b9e2a88378ec0
-https://conda.anaconda.org/conda-forge/noarch/notebook-6.3.0-pyha770c72_1.tar.bz2#6a53111a5a62d32abfa21aac8fc55a1b
+https://conda.anaconda.org/conda-forge/noarch/jupyter_client-8.2.0-pyhd8ed1ab_0.conda#58ca2d50c3b27b86fd7df62eaadbf9a9
+https://conda.anaconda.org/conda-forge/noarch/nbformat-5.9.0-pyhd8ed1ab_0.conda#f525a01528c3eba1d381a232a6971c6a
+https://conda.anaconda.org/conda-forge/noarch/prompt_toolkit-3.0.38-hd8ed1ab_0.conda#45b74f64d8808eda7e6f6e6b1d641fd2
+https://conda.anaconda.org/conda-forge/noarch/ipython-8.14.0-pyh41d4057_0.conda#0a0b0d8177c4a209017b356439292db8
+https://conda.anaconda.org/conda-forge/noarch/jupyterhub-base-3.1.1-pyh2a2186d_0.conda#78fc5dfd4577a7ba172fa65eb64b6afb
+https://conda.anaconda.org/conda-forge/noarch/nbclient-0.8.0-pyhd8ed1ab_0.conda#e78da91cf428faaf05701ce8cc8f2f9b
+https://conda.anaconda.org/conda-forge/noarch/ipykernel-6.23.1-pyh210e3f2_0.conda#4b57b688e22d094d1479a35543c18e93
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-core-7.4.0-pyhd8ed1ab_0.conda#4456e6030a8309bdad57569b0170b6a3
+https://conda.anaconda.org/conda-forge/noarch/ipywidgets-8.0.6-pyhd8ed1ab_0.conda#68627a08556e4a273e4c7bfc84251457
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server-1.23.6-pyhd8ed1ab_0.conda#5016f7c6845a6efd270fcee63af9a2a0
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-pandoc-7.4.0-pyhd8ed1ab_0.conda#127c702e1b1eff595be82bc6a78cfce0
+https://conda.anaconda.org/conda-forge/noarch/jupyter-resource-usage-0.7.1-pyhd8ed1ab_0.conda#62ed54dc748d19d0cf056a3f90cc8f12
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_fileid-0.9.0-pyhd8ed1ab_0.conda#a12525b037a703d7f4512da737d700e6
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab_server-2.22.1-pyhd8ed1ab_0.conda#fc7172a6742a7c3c4331ddd7ed463ffc
+https://conda.anaconda.org/conda-forge/noarch/nbconvert-7.4.0-pyhd8ed1ab_0.conda#a86727968b41c20dd3d73b91632e77dc
+https://conda.anaconda.org/conda-forge/noarch/notebook-shim-0.2.3-pyhd8ed1ab_0.conda#67e0fe74c156267d9159e9133df7fd37
+https://conda.anaconda.org/conda-forge/noarch/jupyter_server_ydoc-0.8.0-pyhd8ed1ab_0.conda#780280d42fbcb2eaf654a6ba7a3e5bb5
+https://conda.anaconda.org/conda-forge/noarch/nbclassic-1.0.0-pyhb4ecaf3_1.conda#a0be31e9bd84d6eae87cdbf74c56b90b
+https://conda.anaconda.org/conda-forge/noarch/notebook-6.5.4-pyha770c72_0.conda#ec4ce3ce0a55ce21b6f5b86049b97af9
 https://conda.anaconda.org/conda-forge/noarch/jupyter-offlinenotebook-0.2.2-pyh1d7be83_0.tar.bz2#fe55056ce4bc4bd4953ba440270735fb
-https://conda.anaconda.org/conda-forge/linux-64/jupyterhub-singleuser-1.4.2-py39hf3d152e_0.tar.bz2#176c4f6b76330d7c6f8534640c6cc193
-https://conda.anaconda.org/conda-forge/noarch/nbclassic-0.3.5-pyhd8ed1ab_0.tar.bz2#e9e2281b7dc08d876fc789af0f571ade
-https://conda.anaconda.org/conda-forge/noarch/nteract_on_jupyter-2.1.3-py_0.tar.bz2#1430ccd983ae6b161e2fbf4377965f7a
-https://conda.anaconda.org/conda-forge/linux-64/widgetsnbextension-3.5.2-py39hf3d152e_1.tar.bz2#26c83eb2efd87c9bbef958b9f7117559
-https://conda.anaconda.org/conda-forge/noarch/ipywidgets-7.6.5-pyhd8ed1ab_0.tar.bz2#6f2ee1ec157104df141e2e5afeba98d4
-https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.2.8-pyhd8ed1ab_0.tar.bz2#e2cc0671571f14af58f832c912dee025
+https://conda.anaconda.org/conda-forge/noarch/jupyterlab-3.6.4-pyhd8ed1ab_0.conda#e66d4a6e36fcc92fe266932bf85fd35a
+https://conda.anaconda.org/conda-forge/noarch/jupyterhub-singleuser-3.1.1-pyh2a2186d_0.conda#6d0a3394efe9ff7c0ad1ed03a6ca3720
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/freeze.py` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/freeze.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,30 +5,25 @@
 Using conda-lock
 
 Usage:
 
 python freeze.py [3.8]
 """
 
-from argparse import ArgumentParser
-from datetime import datetime
 import os
 import pathlib
-import shutil
+from argparse import ArgumentParser
+from datetime import datetime
 from subprocess import check_call
-import sys
 
 from ruamel.yaml import YAML
 
-
 HERE = pathlib.Path(os.path.dirname(os.path.abspath(__file__)))
 
 ENV_FILE = HERE / "environment.yml"
-FROZEN_FILE = os.path.splitext(ENV_FILE)[0] + ".lock"
-
 ENV_FILE_T = HERE / "environment.py-{py}.yml"
 
 yaml = YAML(typ="rt")
 
 
 def freeze(env_file, frozen_file, platform="linux-64"):
     """Freeze a conda environment
@@ -58,14 +53,15 @@
 
     check_call(
         [
             "conda-lock",
             # FIXME: adopt micromamba after ordering is fixed
             # https://github.com/conda-incubator/conda-lock/issues/79
             "--mamba",
+            "--kind=explicit",
             f"--platform={platform}",
             f"--filename-template={frozen_template}",
             f"--file={env_file}",
         ]
     )
 
     with frozen_dest.open("w") as f:
@@ -113,18 +109,24 @@
             "https://repo2docker.readthedocs.io/en/latest/contributing/tasks.html#update-and-freeze-buildpack-dependencies"
         )
     )
     parser.add_argument(
         "py",
         nargs="*",
         help="Python version(s) to update and freeze",
-        default=("2.7", "3.6", "3.7", "3.8", "3.9"),
+        default=("3.7", "3.8", "3.9", "3.10", "3.11"),
+    )
+    parser.add_argument(
+        "platform",
+        nargs="*",
+        help="Platform(s) to update and freeze",
+        default=("linux-64", "linux-aarch64"),
     )
     args = parser.parse_args()
-    default_py = "3.7"
     for py in args.py:
-        env_file = pathlib.Path(str(ENV_FILE_T).format(py=py))
-        set_python(env_file, py)
-        frozen_file = pathlib.Path(os.path.splitext(env_file)[0] + ".lock")
-        freeze(env_file, frozen_file)
-        if py == default_py:
-            shutil.copy(frozen_file, FROZEN_FILE)
+        for platform in args.platform:
+            env_file = pathlib.Path(str(ENV_FILE_T).format(py=py))
+            set_python(env_file, py)
+            frozen_file = pathlib.Path(
+                os.path.splitext(env_file)[0] + f"-{platform}.lock"
+            )
+            freeze(env_file, frozen_file, platform)
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/conda/install-base-env.bash` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/conda/install-base-env.bash`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 #!/bin/bash
 # This downloads and installs a pinned version of micromamba
 # and sets up the base environment
 set -ex
 
 cd $(dirname $0)
 
-export MAMBA_VERSION=0.19.1
-export CONDA_VERSION=4.11.0
+export MAMBA_VERSION=1.4.0
+export CONDA_VERSION=23.1.0
 
-URL="https://anaconda.org/conda-forge/micromamba/${MAMBA_VERSION}/download/linux-64/micromamba-${MAMBA_VERSION}-0.tar.bz2"
+URL="https://anaconda.org/conda-forge/micromamba/${MAMBA_VERSION}/download/${CONDA_PLATFORM}/micromamba-${MAMBA_VERSION}-0.tar.bz2"
 
 # make sure we don't do anything funky with user's $HOME
 # since this is run as root
 unset HOME
 mkdir -p ${CONDA_DIR}
 
 export MICROMAMBA_EXE="/usr/local/bin/micromamba"
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/docker.py` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/docker.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Generates a variety of Dockerfiles based on an input matrix
 """
 import os
+
 import docker
+
 from .base import BuildPack
 
 
 class DockerBuildPack(BuildPack):
     """Docker BuildPack"""
 
     dockerfile = "Dockerfile"
@@ -24,22 +26,23 @@
         self,
         client,
         image_spec,
         memory_limit,
         build_args,
         cache_from,
         extra_build_kwargs,
+        platform=None,
     ):
         """Build a Docker image based on the Dockerfile in the source repo."""
         # If you work on this bit of code check the corresponding code in
         # buildpacks/base.py where it is duplicated
         if not isinstance(memory_limit, int):
             raise ValueError(
-                "The memory limit has to be specified as an"
-                "integer but is '{}'".format(type(memory_limit))
+                "The memory limit has to be specified as an "
+                f"integer but is '{type(memory_limit)}'"
             )
         limits = {}
         if memory_limit:
             # We want to always disable swap. Docker expects `memswap` to
             # be total allowable memory, *including* swap - while `memory`
             # points to non-swap memory. We set both values to the same so
             # we use no swap.
@@ -49,13 +52,13 @@
             path=os.getcwd(),
             dockerfile=self.binder_path(self.dockerfile),
             tag=image_spec,
             buildargs=build_args,
             container_limits=limits,
             cache_from=cache_from,
             labels=self.get_labels(),
+            platform=platform,
         )
 
         build_kwargs.update(extra_build_kwargs)
 
-        for line in client.build(**build_kwargs):
-            yield line
+        yield from client.build(**build_kwargs)
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/julia/install-repo-dependencies.jl` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/julia/install-repo-dependencies.jl`

 * *Files identical despite different names*

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/julia/julia_project.py` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/julia/julia_project.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 """Generates a Dockerfile based on an input matrix for Julia"""
 import functools
 import os
+from functools import lru_cache
 
 import requests
 import semver
 import toml
 
-from ..python import PythonBuildPack
 from ...semver import find_semver_match
+from ..python import PythonBuildPack
 
 
 class JuliaProjectTomlBuildPack(PythonBuildPack):
     """
     Julia build pack which uses conda.
     """
 
     # ALL EXISTING JULIA VERSIONS
     # Note that these must remain ordered, in order for the find_semver_match()
     # function to behave correctly.
     @property
-    @functools.lru_cache(maxsize=1)
+    @lru_cache(maxsize=1)
     def all_julias(self):
         try:
             json = requests.get(
                 "https://julialang-s3.julialang.org/bin/versions.json"
             ).json()
         except Exception as e:
-            raise RuntimeError("Failed to fetch available Julia versions: {e}")
+            raise RuntimeError(f"Failed to fetch available Julia versions: {e}")
         vers = [semver.VersionInfo.parse(v) for v in json.keys()]
         # filter out pre-release versions not supported by find_semver_match()
         filtered_vers = [v for v in vers if v.prerelease is None]
         # properly sort list of VersionInfo
         sorted_vers = sorted(
             filtered_vers, key=functools.cmp_to_key(semver.VersionInfo.compare)
         )
@@ -46,60 +47,90 @@
 
         try:
             # For Project.toml files, install the latest julia version that
             # satisfies the given semver.
             compat = project_toml["compat"]["julia"]
         except:
             # Default version which needs to be manually updated with new major.minor releases
+            #
+            # NOTE: Updates to the default version should go hand in hand with
+            #       updates to tests/julia/project/verify where is intent to
+            #       test the version.
+            #
+            # FIXME: When compat = "1.6" is set below and passed to
+            #        find_semver_match, we get 1.8.2 as of 2022-10-09. We should
+            #        clarify the desired behavior and have a unit test of
+            #        find_semver_match to validate it.
+            #
             compat = "1.6"
 
         match = find_semver_match(compat, self.all_julias)
         if match is None:
             raise RuntimeError("Failed to find a matching Julia version: {compat}")
         return match
 
+    @lru_cache()
     def get_build_env(self):
         """Get additional environment settings for Julia and Jupyter
 
         Returns:
             an ordered list of environment setting tuples
 
             The tuples contain a string of the environment variable name and
             a string of the environment setting:
             - `JULIA_PATH`: base path where all Julia Binaries and libraries
                 will be installed
             - `JULIA_DEPOT_PATH`: path where Julia libraries are installed.
             - `JULIA_VERSION`: default version of julia to be installed
+            - `JULIA_ARCH`: machine architecture used in Julia download URLs
+            - `JULIA_ARCH_SHORT`: machine architecture used in Julia download URLs
             - `JUPYTER`: environment variable required by IJulia to point to
                 the `jupyter` executable
 
             For example, a tuple may be `('JULIA_VERSION', '0.6.0')`.
 
         """
+        if self.platform == "linux/arm64":
+            julia_arch = julia_arch_short = "aarch64"
+        else:
+            julia_arch = "x86_64"
+            julia_arch_short = "x64"
         return super().get_build_env() + [
             ("JULIA_PATH", "${APP_BASE}/julia"),
             ("JULIA_DEPOT_PATH", "${JULIA_PATH}/pkg"),
             ("JULIA_VERSION", self.julia_version),
+            ("JULIA_ARCH", julia_arch),
+            ("JULIA_ARCH_SHORT", julia_arch_short),
             ("JUPYTER", "${NB_PYTHON_PREFIX}/bin/jupyter"),
             ("JUPYTER_DATA_DIR", "${NB_PYTHON_PREFIX}/share/jupyter"),
         ]
 
+    @property
+    def project_dir(self):
+        if self.binder_dir:
+            return "${REPO_DIR}/" + self.binder_dir
+        else:
+            return "${REPO_DIR}"
+
+    @lru_cache()
     def get_env(self):
-        return super().get_env() + [("JULIA_PROJECT", "${REPO_DIR}")]
+        return super().get_env() + [("JULIA_PROJECT", self.project_dir)]
 
+    @lru_cache()
     def get_path(self):
         """Adds path to Julia binaries to user's PATH.
 
         Returns:
             an ordered list of path strings. The path to the Julia
             executable is added to the list.
 
         """
         return super().get_path() + ["${JULIA_PATH}/bin"]
 
+    @lru_cache()
     def get_build_scripts(self):
         """
         Return series of build-steps common to "ALL" Julia repositories
 
         All scripts found here should be independent of contents of a
         particular repository.
 
@@ -108,49 +139,54 @@
 
         """
         return super().get_build_scripts() + [
             (
                 "root",
                 r"""
                 mkdir -p ${JULIA_PATH} && \
-                curl -sSL "https://julialang-s3.julialang.org/bin/linux/x64/${JULIA_VERSION%[.-]*}/julia-${JULIA_VERSION}-linux-x86_64.tar.gz" | tar -xz -C ${JULIA_PATH} --strip-components 1
+                curl -sSL "https://julialang-s3.julialang.org/bin/linux/${JULIA_ARCH_SHORT}/${JULIA_VERSION%[.-]*}/julia-${JULIA_VERSION}-linux-${JULIA_ARCH}.tar.gz" | tar -xz -C ${JULIA_PATH} --strip-components 1
                 """,
             ),
             (
                 "root",
                 r"""
                 mkdir -p ${JULIA_DEPOT_PATH} && \
                 chown ${NB_USER}:${NB_USER} ${JULIA_DEPOT_PATH}
                 """,
             ),
         ]
 
+    @lru_cache()
     def get_assemble_scripts(self):
         """
         Return series of build-steps specific to "this" Julia repository
 
         We make sure that the IJulia package gets installed into the default
         environment, and not the project specific one, by running the
         IJulia install command with JULIA_PROJECT="".
 
         Instantiate and then precompile all packages in the repos julia
         environment.
 
         The parent, CondaBuildPack, will add the build steps for
         any needed Python packages found in environment.yml.
         """
-        return super().get_assemble_scripts() + [
+        scripts = super().get_assemble_scripts()
+        scripts.append(
             (
                 "${NB_USER}",
                 r"""
-                JULIA_PROJECT="" julia -e "using Pkg; Pkg.add(\"IJulia\"); using IJulia; installkernel(\"Julia\", \"--project=${REPO_DIR}\");" && \
-                julia --project=${REPO_DIR} -e 'using Pkg; Pkg.instantiate(); Pkg.resolve(); pkg"precompile"'
-                """,
+            JULIA_PROJECT="" julia -e "using Pkg; Pkg.add(\"IJulia\"); using IJulia; installkernel(\"Julia\", \"--project={project}\");" && \
+            julia --project={project} -e 'using Pkg; Pkg.instantiate(); Pkg.resolve(); pkg"precompile"'
+            """.format(
+                    project=self.project_dir
+                ),
             )
-        ]
+        )
+        return scripts
 
     def detect(self):
         """
         Check if current repo should be built with the Julia Build pack
 
         super().detect() is not called in this function - it would return
         false unless an `environment.yml` is present and we do not want to
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/julia/julia_require.py` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/julia/julia_require.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Generates a Dockerfile based on an input matrix with REQUIRE for legacy Julia"""
 
 import os
+from functools import lru_cache
 
-from ..python import PythonBuildPack
 from ...semver import parse_version as V
+from ..python import PythonBuildPack
 
 
 class JuliaRequireBuildPack(PythonBuildPack):
     """
     Julia build pack which uses conda and REQUIRE.
     """
 
@@ -50,14 +51,15 @@
             julia_version = self.minor_julias[".".join(julia_version_info)]
         else:
             # use supplied julia version
             julia_version = ".".join(julia_version_info)
         self._julia_version = julia_version
         return self._julia_version
 
+    @lru_cache()
     def get_build_env(self):
         """Get additional environment settings for Julia and Jupyter
 
         Returns:
             an ordered list of environment setting tuples
 
             The tuples contain a string of the environment variable name and
@@ -65,40 +67,59 @@
             - `JULIA_PATH`: base path where all Julia Binaries and libraries
                 will be installed
             - `JULIA_HOME`: path where all Julia Binaries will be installed
             - `JULIA_PKGDIR`: path where all Julia libraries will be installed
             - `JULIA_DEPOT_PATH`: path where Julia libraries are installed.
                                   Similar to JULIA_PKGDIR, used in 1.x.
             - `JULIA_VERSION`: default version of julia to be installed
+            - `JULIA_ARCH`: machine architecture used in Julia download URLs
+            - `JULIA_ARCH_SHORT`: machine architecture used in Julia download URLs
             - `JUPYTER`: environment variable required by IJulia to point to
                 the `jupyter` executable
 
             For example, a tuple may be `('JULIA_VERSION', '0.6.0')`.
 
         """
+        if self.platform == "linux/arm64":
+            julia_arch = julia_arch_short = "aarch64"
+        else:
+            julia_arch = "x86_64"
+            julia_arch_short = "x64"
+
+        if V(self.julia_version) < V("0.7"):
+            # IJulia with Julia 0.6 isn't compatible with more recent jupyter-core
+            # point it to the one in the kernel env
+            # I _think_ this is only relevant during installation
+            jupyter = "${KERNEL_PYTHON_PREFIX}/bin/jupyter"
+        else:
+            jupyter = "${NB_PYTHON_PREFIX}/bin/jupyter"
         return super().get_build_env() + [
             ("JULIA_PATH", "${APP_BASE}/julia"),
             ("JULIA_HOME", "${JULIA_PATH}/bin"),  # julia <= 0.6
             ("JULIA_BINDIR", "${JULIA_HOME}"),  # julia >= 0.7
             ("JULIA_PKGDIR", "${JULIA_PATH}/pkg"),
             ("JULIA_DEPOT_PATH", "${JULIA_PKGDIR}"),  # julia >= 0.7
             ("JULIA_VERSION", self.julia_version),
-            ("JUPYTER", "${NB_PYTHON_PREFIX}/bin/jupyter"),
+            ("JULIA_ARCH", julia_arch),
+            ("JULIA_ARCH_SHORT", julia_arch_short),
+            ("JUPYTER", jupyter),
         ]
 
+    @lru_cache()
     def get_path(self):
         """Adds path to Julia binaries to user's PATH.
 
         Returns:
             an ordered list of path strings. The path to the Julia
             executable is added to the list.
 
         """
         return super().get_path() + ["${JULIA_HOME}"]
 
+    @lru_cache()
     def get_build_scripts(self):
         """
         Return series of build-steps common to "ALL" Julia repositories
 
         All scripts found here should be independent of contents of a
         particular repository.
 
@@ -107,15 +128,15 @@
 
         """
         return super().get_build_scripts() + [
             (
                 "root",
                 r"""
                 mkdir -p ${JULIA_PATH} && \
-                curl -sSL "https://julialang-s3.julialang.org/bin/linux/x64/${JULIA_VERSION%[.-]*}/julia-${JULIA_VERSION}-linux-x86_64.tar.gz" | tar -xz -C ${JULIA_PATH} --strip-components 1
+                curl -sSL "https://julialang-s3.julialang.org/bin/linux/${JULIA_ARCH_SHORT}/${JULIA_VERSION%[.-]*}/julia-${JULIA_VERSION}-linux-${JULIA_ARCH}.tar.gz" | tar -xz -C ${JULIA_PATH} --strip-components 1
                 """,
             ),
             (
                 "root",
                 r"""
                 mkdir -p ${JULIA_PKGDIR} && \
                 chown ${NB_USER}:${NB_USER} ${JULIA_PKGDIR}
@@ -128,14 +149,15 @@
                 r"""
                 julia -e 'if (VERSION > v"0.7-") using Pkg; else Pkg.init(); end; Pkg.add("IJulia"); using IJulia;' && \
                 mv ${HOME}/.local/share/jupyter/kernels/julia-${JULIA_VERSION%[.-]*}  ${NB_PYTHON_PREFIX}/share/jupyter/kernels/julia-${JULIA_VERSION%[.-]*}
                 """,
             ),
         ]
 
+    @lru_cache()
     def get_assemble_scripts(self):
         """
         Return series of build-steps specific to "this" Julia repository
 
         Precompile all Julia libraries found in the repository's REQUIRE
         file. The parent, CondaBuildPack, will add the build steps for
         any needed Python packages found in environment.yml.
@@ -155,14 +177,15 @@
             """
                 % {"require": require}
                 # TODO: For some reason, `rm`ing the file fails with permission denied.
                 # && rm /tmp/install-repo-dependencies.jl
             )
         ]
 
+    @lru_cache()
     def get_build_script_files(self):
         files = {
             "julia/install-repo-dependencies.jl": "/tmp/install-repo-dependencies.jl"
         }
         files.update(super().get_build_script_files())
         return files
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/legacy/__init__.py` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/legacy/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,19 +12,22 @@
 
 class LegacyBinderDockerBuildPack:
     """Legacy build pack for compatibility to first version of Binder.
 
     This buildpack has been deprecated.
     """
 
+    def __init__(self, *args, **kwargs):
+        pass
+
     def detect(self):
         """Check if current repo should be built with the Legacy BuildPack."""
         log = logging.getLogger("repo2docker")
         try:
-            with open("Dockerfile", "r") as f:
+            with open("Dockerfile") as f:
                 for line in f:
                     if line.startswith("FROM"):
                         if "andrewosh/binder-base" in line.split("#")[0].lower():
                             log.error(
                                 "The legacy buildpack was removed in January 2020."
                             )
                             log.error(
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/nix/__init__.py` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/nix/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,81 +1,91 @@
 """BuildPack for nixpkgs environments"""
 import os
+from functools import lru_cache
 
-from ..base import BuildPack, BaseImage
+from ..base import BaseImage
 
 
 class NixBuildPack(BaseImage):
     """A nix Package Manager BuildPack"""
 
+    @lru_cache()
     def get_path(self):
         """Return paths to be added to PATH environemnt variable"""
         return super().get_path() + ["/home/${NB_USER}/.nix-profile/bin"]
 
+    @lru_cache()
     def get_env(self):
         """Ordered list of environment variables to be set for this image"""
+
         return super().get_env() + [
             ("NIX_PATH", "nixpkgs=/home/${NB_USER}/.nix-defexpr/channels/nixpkgs"),
             ("NIX_SSL_CERT_FILE", "/etc/ssl/certs/ca-certificates.crt"),
             ("GIT_SSL_CAINFO", "/etc/ssl/certs/ca-certificates.crt"),
         ]
 
+    @lru_cache()
     def get_build_scripts(self):
         """
         Return series of build-steps common to all nix repositories.
         Notice how only root privileges are needed for creating nix
         directory and a nix.conf file.
 
          - create nix directory for user nix installation
          - disable sandboxing because its unsupported inside a Docker container
          - install nix package manager for user
 
         """
+        if self.platform == "linux/arm64":
+            nix_arch = "aarch64"
+        else:
+            nix_arch = "x86_64"
         return super().get_build_scripts() + [
             (
                 "root",
                 """
             mkdir -m 0755 /nix && \
             chown -R ${NB_USER}:${NB_USER} /nix /usr/local/bin/nix-shell-wrapper /home/${NB_USER} && \
             mkdir -p /etc/nix && \
             touch /etc/nix/nix.conf && \
             echo "sandbox = false" >> /etc/nix/nix.conf
             """,
             ),
             (
                 "${NB_USER}",
-                """
-            bash /home/${NB_USER}/.local/bin/install-nix.bash && \
-            rm /home/${NB_USER}/.local/bin/install-nix.bash
+                f"""
+            NIX_ARCH={nix_arch} bash /home/${{NB_USER}}/.local/bin/install-nix.bash && \
+            rm /home/${{NB_USER}}/.local/bin/install-nix.bash
             """,
             ),
         ]
 
+    @lru_cache()
     def get_build_script_files(self):
         """Dict of files to be copied to the container image for use in building"""
         return {
             "nix/install-nix.bash": "/home/${NB_USER}/.local/bin/install-nix.bash",
             "nix/nix-shell-wrapper": "/usr/local/bin/nix-shell-wrapper",
         }
 
+    @lru_cache()
     def get_assemble_scripts(self):
         """Return series of build-steps specific to this source repository."""
         return super().get_assemble_scripts() + [
             (
                 "${NB_USER}",
-                """
+                f"""
             nix-channel --add https://nixos.org/channels/nixpkgs-unstable nixpkgs && \
             nix-channel --update && \
-            nix-shell {}
-            """.format(
-                    self.binder_path("default.nix")
-                ),
+            nix-shell {self.binder_path("default.nix")}
+            """,
             )
         ]
 
+    @lru_cache()
     def get_start_script(self):
         """The path to a script to be executed as ENTRYPOINT"""
         # the shell wrapper script duplicates the behaviour of other buildpacks
         # when it comes to the `start` script as well as handling a binder/
         # sub-directory when it exists
         return "/usr/local/bin/nix-shell-wrapper"
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/nix/install-nix.bash` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/nix/install-nix.bash`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,18 @@
 #!/bin/bash
 # This downloads and installs a pinned version of nix
 set -ex
 
-NIX_VERSION="2.3.9"
-NIX_SHA256="49763fd7fa06bcb712ced2f3f11afd275e3a4d7bc5ff0d6fd1d50a4c3ce7bbf4"
+NIX_VERSION="2.13.2"
+if [ "$NIX_ARCH" = "aarch64" ]; then
+  NIX_SHA256="4ae275a46a2441d3459ae389a90ce6e8f7eff12c2a084b2d003ba6f8d0899603"
+else
+  NIX_SHA256="beaec0f28899c22f33adbe30e4ecfceef87b797278c5210ee693e22e9719dfb4"
+fi
 
 # Do all our operations in /tmp, since we can't rely on current directory being writeable yet.
 cd /tmp
-wget --quiet https://nixos.org/releases/nix/nix-$NIX_VERSION/nix-$NIX_VERSION-x86_64-linux.tar.xz
-echo "$NIX_SHA256  nix-$NIX_VERSION-x86_64-linux.tar.xz" | sha256sum -c
-tar xJf nix-*-x86_64-linux.tar.xz
-sh nix-*-x86_64-linux/install
-rm -r nix-*-x86_64-linux*
+wget --quiet https://nixos.org/releases/nix/nix-$NIX_VERSION/nix-$NIX_VERSION-$NIX_ARCH-linux.tar.xz
+echo "$NIX_SHA256  nix-$NIX_VERSION-$NIX_ARCH-linux.tar.xz" | sha256sum -c
+tar xJf nix-*-$NIX_ARCH-linux.tar.xz
+sh nix-*-$NIX_ARCH-linux/install
+rm -r nix-*-$NIX_ARCH-linux*
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/nix/nix-shell-wrapper` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/nix/nix-shell-wrapper`

 * *Files identical despite different names*

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/pipfile/__init__.py` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/pipfile/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,17 +4,19 @@
 conda will provide the base Python environment,
 same as the Python or Conda build packs.
 """
 
 import json
 import os
 import re
+from functools import lru_cache
 
 import toml
 
+from ...semver import parse_version as V
 from ..conda import CondaBuildPack
 
 VERSION_PAT = re.compile(r"\d+(\.\d+)*")
 
 
 class PipfileBuildPack(CondaBuildPack):
     """Setup Python with pipfile for use with a repository."""
@@ -59,68 +61,81 @@
                 if py_version:
                     break
             if py_version:
                 break
 
         # extract major.minor
         if py_version:
-            if len(py_version.split(".")) == 1:
-                self._python_version = self.major_pythons.get(py_version[0])
+            py_version_info = py_version.split(".")
+            if len(py_version_info) == 1:
+                self._python_version = self.major_pythons[py_version_info[0]]
             else:
                 # return major.minor
-                self._python_version = ".".join(py_version.split(".")[:2])
+                self._python_version = ".".join(py_version_info[:2])
             return self._python_version
         else:
             # use the default Python
             self._python_version = self.major_pythons["3"]
+            self.log.warning(
+                f"Python version unspecified, using current default Python version {self._python_version}. This will change in the future."
+            )
             return self._python_version
 
+    @lru_cache()
     def get_preassemble_script_files(self):
         """Return files needed for preassembly"""
         files = super().get_preassemble_script_files()
         for name in ("requirements3.txt", "Pipfile", "Pipfile.lock"):
             path = self.binder_path(name)
             if os.path.exists(path):
                 files[path] = path
         return files
 
+    @lru_cache()
     def get_preassemble_scripts(self):
         """scripts to run prior to staging the repo contents"""
         scripts = super().get_preassemble_scripts()
         # install pipenv to install dependencies within Pipfile.lock or Pipfile
+        if V(self.python_version) < V("3.6"):
+            # last pipenv version to support 2.7, 3.5
+            pipenv_version = "2021.5.29"
+        else:
+            pipenv_version = "2022.1.8"
         scripts.append(
-            ("${NB_USER}", "${KERNEL_PYTHON_PREFIX}/bin/pip install pipenv==2018.11.26")
+            (
+                "${NB_USER}",
+                f"${{KERNEL_PYTHON_PREFIX}}/bin/pip install --no-cache-dir pipenv=={pipenv_version}",
+            )
         )
         return scripts
 
+    @lru_cache()
     def get_assemble_scripts(self):
         """Return series of build-steps specific to this repository."""
         # If we have either Pipfile.lock, Pipfile, or runtime.txt declare the
         # use of Python 2, Python 2.7 will be made available in the *kernel*
         # environment. The notebook servers environment on the other hand
         # requires Python 3 but may require something additional installed in it
         # still such as `nbgitpuller`. For this purpose, a "requirements3.txt"
         # file will be used to install dependencies for the notebook servers
         # environment, if Python 2 had been specified for the kernel
         # environment.
         assemble_scripts = super().get_assemble_scripts()
 
-        if self.py2:
-            # using Python 2 as a kernel, but Python 3 for the notebook server
+        if self.separate_kernel_env:
+            # using legacy Python (e.g. 2.7) as a kernel
 
             # requirements3.txt allows for packages to be installed to the
             # notebook servers Python environment
             nb_requirements_file = self.binder_path("requirements3.txt")
             if os.path.exists(nb_requirements_file):
                 assemble_scripts.append(
                     (
                         "${NB_USER}",
-                        '${{NB_PYTHON_PREFIX}}/bin/pip install --no-cache-dir -r "{}"'.format(
-                            nb_requirements_file
-                        ),
+                        f'${{NB_PYTHON_PREFIX}}/bin/pip install --no-cache-dir -r "{nb_requirements_file}"',
                     )
                 )
 
         pipfile = self.binder_path("Pipfile")
         pipfile_lock = self.binder_path("Pipfile.lock")
 
         # A Pipfile(.lock) can contain relative references, so we need to be
@@ -150,15 +165,16 @@
         #   let the RUN command continue on the next line. So it is only added
         #   to avoid forcing us to write it all on a single line.
         assemble_scripts.append(
             (
                 "${NB_USER}",
                 """(cd {working_directory} && \\
                     PATH="${{KERNEL_PYTHON_PREFIX}}/bin:$PATH" \\
-                        pipenv install {install_option} --system --dev \\
+                        pipenv install {install_option} --system --dev && \\
+                        pipenv --clear \\
                 )""".format(
                     working_directory=working_directory,
                     install_option="--ignore-pipfile"
                     if os.path.exists(pipfile_lock)
                     else "--skip-lock",
                 ),
             )
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/python/__init__.py` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/python/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Generates Dockerfiles based on an input matrix based on Python."""
 import os
+from functools import lru_cache
 
-from ..conda import CondaBuildPack
 from ...utils import is_local_pip_requirement, open_guess_encoding
+from ..conda import CondaBuildPack
 
 
 class PythonBuildPack(CondaBuildPack):
     """Setup Python for use with a repository."""
 
     @property
     def python_version(self):
@@ -19,14 +20,17 @@
         except FileNotFoundError:
             runtime = ""
 
         if not runtime.startswith("python-"):
             # not a Python runtime (e.g. R, which subclasses this)
             # use the default Python
             self._python_version = self.major_pythons["3"]
+            self.log.warning(
+                f"Python version unspecified, using current default Python version {self._python_version}. This will change in the future."
+            )
             return self._python_version
 
         py_version_info = runtime.split("-", 1)[1].split(".")
         py_version = ""
         if len(py_version_info) == 1:
             py_version = self.major_pythons[py_version_info[0]]
         else:
@@ -41,37 +45,35 @@
         added to preassemble unless local references are found,
         in which case this happens in assemble.
         """
         # KERNEL_PYTHON_PREFIX is the env with the kernel,
         # whether it's distinct from the notebook or the same.
         pip = "${KERNEL_PYTHON_PREFIX}/bin/pip"
         scripts = []
-        if self.py2:
-            # using python 2 kernel,
+        if self.separate_kernel_env:
+            # using legacy Python kernel
             # requirements3.txt allows installation in the notebook server env
             nb_requirements_file = self.binder_path("requirements3.txt")
             if os.path.exists(nb_requirements_file):
                 scripts.append(
                     (
                         "${NB_USER}",
                         # want the $NB_PYHTON_PREFIX environment variable, not for
                         # Python's string formatting to try and replace this
-                        '${{NB_PYTHON_PREFIX}}/bin/pip install --no-cache-dir -r "{}"'.format(
-                            nb_requirements_file
-                        ),
+                        f'${{NB_PYTHON_PREFIX}}/bin/pip install --no-cache-dir -r "{nb_requirements_file}"',
                     )
                 )
 
         # install requirements.txt in the kernel env
         requirements_file = self.binder_path("requirements.txt")
         if os.path.exists(requirements_file):
             scripts.append(
                 (
                     "${NB_USER}",
-                    '{} install --no-cache-dir -r "{}"'.format(pip, requirements_file),
+                    f'{pip} install --no-cache-dir -r "{requirements_file}"',
                 )
             )
         return scripts
 
     @property
     def _should_preassemble_pip(self):
         """Peek in requirements.txt to determine if we can assemble from only env files
@@ -91,29 +93,32 @@
                     if is_local_pip_requirement(line):
                         return False
 
         # didn't find any local references,
         # allow assembly from subset
         return True
 
+    @lru_cache()
     def get_preassemble_script_files(self):
         assemble_files = super().get_preassemble_script_files()
         for name in ("requirements.txt", "requirements3.txt"):
             requirements_txt = self.binder_path(name)
             if os.path.exists(requirements_txt):
                 assemble_files[requirements_txt] = requirements_txt
         return assemble_files
 
+    @lru_cache()
     def get_preassemble_scripts(self):
         """Return scripts to run before adding the full repository"""
         scripts = super().get_preassemble_scripts()
         if self._should_preassemble_pip:
             scripts.extend(self._get_pip_scripts())
         return scripts
 
+    @lru_cache()
     def get_assemble_scripts(self):
         """Return series of build steps that require the full repository"""
         # If we have a runtime.txt & that's set to python-2.7,
         # requirements.txt will be installed in the *kernel* env
         # and requirements3.txt (if it exists)
         # will be installed in the python 3 notebook server env.
         assemble_scripts = super().get_assemble_scripts()
@@ -122,17 +127,15 @@
         # whether it's distinct from the notebook or the same.
         pip = "${KERNEL_PYTHON_PREFIX}/bin/pip"
         if not self._should_preassemble_pip:
             assemble_scripts.extend(self._get_pip_scripts())
 
         # setup.py exists *and* binder dir is not used
         if not self.binder_dir and os.path.exists(setup_py):
-            assemble_scripts.append(
-                ("${NB_USER}", "{} install --no-cache-dir .".format(pip))
-            )
+            assemble_scripts.append(("${NB_USER}", f"{pip} install --no-cache-dir ."))
         return assemble_scripts
 
     def detect(self):
         """Check if current repo should be built with the Python buildpack."""
         requirements_txt = self.binder_path("requirements.txt")
         runtime_txt = self.binder_path("runtime.txt")
         setup_py = "setup.py"
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/r.py` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/r.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,36 @@
-import re
-import os
 import datetime
-import requests
+import os
+import re
+from functools import lru_cache
 
+import requests
 
 from ..semver import parse_version as V
-from .python import PythonBuildPack
 from ._r_base import rstudio_base_scripts
+from .python import PythonBuildPack
+
+# Aproximately the first snapshot on RSPM (Posit package manager)
+# that seems to have a working IRKernel.
+RSPM_CUTOFF_DATE = datetime.date(2018, 12, 7)
 
 
 class RBuildPack(PythonBuildPack):
     """
     Setup R for use with a repository
 
     This sets up R + RStudio + IRKernel for a repository that contains:
 
     1. A `runtime.txt` file with the text:
 
        r-<year>-<month>-<date>
 
        Where 'year', 'month' and 'date' refer to a specific
        date whose CRAN snapshot we will use to fetch packages.
-       Uses https://packagemanager.rstudio.com, or MRAN if no snapshot
-       is found on packagemanager.rstudio.com
+       Uses https://packagemanager.posit.co.
 
     2. A `DESCRIPTION` file signaling an R package
 
     If there is no `runtime.txt`, then the CRAN snapshot is set to latest
     date that is guaranteed to exist across timezones.
 
     Additional R packages are installed if specified either
@@ -34,19 +38,15 @@
     - in a file `install.R`, that will be executed at build time,
       and can be used for installing packages from both CRAN and GitHub
 
     - as dependencies in a `DESCRIPTION` file
 
     - are needed by a specific tool
 
-    The `r-base-core` package from Ubuntu or "Ubuntu packages for R"
-    apt repositories is used to install R itself,
-    rather than any of the methods from https://cran.r-project.org/.
-
-    The `r-base-dev` package is installed as advised in RStudio instructions.
+    R is installed from https://docs.rstudio.com/resources/install-r/
     """
 
     @property
     def runtime(self):
         """
         Return contents of runtime.txt if it exists, '' otherwise
         """
@@ -63,42 +63,47 @@
     @property
     def r_version(self):
         """Detect the R version for a given `runtime.txt`
 
         Will return the version specified by the user or the current default
         version.
         """
+        # Available versions at https://cran.r-project.org/src/base/
         version_map = {
-            "3.4": "3.4",
-            "3.5": "3.5.3-1bionic",
-            "3.5.0": "3.5.0-1bionic",
-            "3.5.1": "3.5.1-2bionic",
-            "3.5.2": "3.5.2-1bionic",
-            "3.5.3": "3.5.3-1bionic",
-            "3.6": "3.6.3-1bionic",
-            "3.6.0": "3.6.0-2bionic",
-            "3.6.1": "3.6.1-3bionic",
-            "4.0": "4.0.5-1.1804.0",
-            "4.0.2": "4.0.2-1.1804.0",
-            "4.1": "4.1.2-1.1804.0",
+            "4.2": "4.2.1",
+            "4.1": "4.1.3",
+            "4.0": "4.0.5",
+            "3.6": "3.6.3",
+            "3.5": "3.5.3",
+            "3.4": "3.4.4",
+            "3.3": "3.3.3",
         }
+
         # the default if nothing is specified
-        r_version = "4.1"
+        # Use full version is needed here, so it a valid semver
+        #
+        # NOTE: When updating this version, also update
+        #       - tests/unit/test_r.py -> test_version_specification
+        #       - tests/r/r-rspm-apt/verify
+        #
+        r_version = version_map["4.2"]
 
         if not hasattr(self, "_r_version"):
             parts = self.runtime.split("-")
+            # If runtime.txt is not set, or if it isn't of the form r-<version>-<yyyy>-<mm>-<dd>,
+            # we don't use any of it in determining r version and just use the default
             if len(parts) == 5:
                 r_version = parts[1]
-                if r_version not in version_map:
-                    raise ValueError(
-                        "Version '{}' of R is not supported.".format(r_version)
-                    )
+                # For versions of form x.y, we want to explicitly provide x.y.z - latest patchlevel
+                # available. Users can however explicitly specify the full version to get something specific
+                if r_version in version_map:
+                    r_version = version_map[r_version]
 
             # translate to the full version string
-            self._r_version = version_map.get(r_version)
+            self._r_version = r_version
 
         return self._r_version
 
     @property
     def checkpoint_date(self):
         """
         Return the date of CRAN checkpoint to use for this repo
@@ -134,122 +139,121 @@
         if not self.binder_dir and os.path.exists(description_R):
             if not self.checkpoint_date:
                 # no R snapshot date set through runtime.txt
                 # Set it to two days ago from today
                 self._checkpoint_date = datetime.date.today() - datetime.timedelta(
                     days=2
                 )
-                self._runtime = "r-{}".format(str(self._checkpoint_date))
+                self._runtime = f"r-{str(self._checkpoint_date)}"
             return True
 
+    @lru_cache()
+    def get_env(self):
+        """
+        Set custom env vars needed for RStudio to load
+        """
+        return super().get_env() + [
+            # rstudio (rsession) can't seem to find R unless we explicitly tell it where
+            # it is - just $PATH isn't enough. I discovered these are the env vars it
+            # looks for by digging through RStudio source and finding
+            # https://github.com/rstudio/rstudio/blob/v2022.02.3+492/src/cpp/r/session/RDiscovery.cpp
+            ("R_HOME", f"/opt/R/{self.r_version}/lib/R"),
+            ("R_DOC_DIR", "${R_HOME}/doc"),
+            ("LD_LIBRARY_PATH", "${R_HOME}/lib:${LD_LIBRARY_PATH}"),
+        ]
+
+    @lru_cache()
     def get_path(self):
         """
         Return paths to be added to the PATH environment variable.
 
         The RStudio package installs its binaries in a non-standard path,
         so we explicitly add that path to PATH.
         """
         return super().get_path() + ["/usr/lib/rstudio-server/bin/"]
 
+    @lru_cache()
     def get_build_env(self):
         """
         Return environment variables to be set.
 
         We want libraries to be installed in a path that users can write to
         without needing root. This is set via the `R_LIBS_USER` environment
         variable, so we set that here.
         """
         return super().get_build_env() + [
             # This is the path where user libraries are installed
             ("R_LIBS_USER", "${APP_BASE}/rlibs")
         ]
 
+    @lru_cache()
     def get_packages(self):
         """
         Return list of packages to be installed.
 
         We install a base version of R, and packages required for RStudio to
         be installed.
         """
         packages = [
             # For rstudio
             "psmisc",
             "libapparmor1",
             "sudo",
             "lsb-release",
+            "libssl-dev",
         ]
-        # For R 3.4 we use the default Ubuntu package, for other versions we
-        # install from a different apt repository
-        if V(self.r_version) < V("3.5"):
-            packages.append("r-base")
-            packages.append("r-base-dev")
-            packages.append("libclang-dev")
 
         return super().get_packages().union(packages)
 
+    @lru_cache()
     def get_rspm_snapshot_url(self, snapshot_date, max_days_prior=7):
         for i in range(max_days_prior):
             snapshots = requests.post(
-                "https://packagemanager.rstudio.com/__api__/url",
+                "https://packagemanager.posit.co/__api__/url",
                 # Ask for midnight UTC snapshot
                 json={
                     "repo": "all",
                     "snapshot": (snapshot_date - datetime.timedelta(days=i)).strftime(
                         "%Y-%m-%dT00:00:00Z"
                     ),
                 },
             ).json()
             # Construct a snapshot URL that will give us binary packages for Ubuntu Bionic (18.04)
             if "upsi" in snapshots:
                 return (
-                    "https://packagemanager.rstudio.com/all/__linux__/bionic/"
+                    # Env variables here are expanded by envsubst in the Dockerfile, after sourcing
+                    # /etc/os-release. This allows us to use distro specific variables here to get
+                    # appropriate binary packages without having to hard code version names here.
+                    "https://packagemanager.posit.co/all/__linux__/${VERSION_CODENAME}/"
                     + snapshots["upsi"]
                 )
         raise ValueError(
-            "No snapshot found for {} or {} days prior in packagemanager.rstudio.com".format(
+            "No snapshot found for {} or {} days prior in packagemanager.posit.co".format(
                 snapshot_date.strftime("%Y-%m-%d"), max_days_prior
             )
         )
 
-    def get_mran_snapshot_url(self, snapshot_date, max_days_prior=7):
-        for i in range(max_days_prior):
-            try_date = snapshot_date - datetime.timedelta(days=i)
-            # Fall back to MRAN if packagemanager.rstudio.com doesn't have it
-            url = "https://mran.microsoft.com/snapshot/{}".format(try_date.isoformat())
-            r = requests.head(url)
-            if r.ok:
-                return url
-        raise ValueError(
-            "No snapshot found for {} or {} days prior in mran.microsoft.com".format(
-                snapshot_date.strftime("%Y-%m-%d"), max_days_prior
-            )
-        )
-
-    def get_cran_mirror_url(self, snapshot_date):
-        # Date after which we will use rspm + binary packages instead of MRAN + source packages
-        rspm_cutoff_date = datetime.date(2022, 1, 1)
-
-        if snapshot_date >= rspm_cutoff_date or self.r_version >= V("4.1"):
-            return self.get_rspm_snapshot_url(snapshot_date)
-        else:
-            return self.get_mran_snapshot_url(snapshot_date)
-
+    @lru_cache()
     def get_devtools_snapshot_url(self):
         """
         Return url of snapshot to use for getting devtools install
 
         devtools is part of our 'core' base install, so we should have some
         control over what version we install here.
         """
-        # Picked from https://packagemanager.rstudio.com/client/#/repos/1/overview
+        # Picked from https://packagemanager.posit.co/client/#/repos/1/overview
         # Hardcoded rather than dynamically determined from a date to avoid extra API calls
-        # Plus, we can always use packagemanager.rstudio.com here as we always install the
+        # Plus, we can always use packagemanager.posit.co here as we always install the
         # necessary apt packages.
-        return "https://packagemanager.rstudio.com/all/__linux__/bionic/2022-01-04+Y3JhbiwyOjQ1MjYyMTU7NzlBRkJEMzg"
+        # Env variables here are expanded by envsubst in the Dockerfile, after sourcing
+        # /etc/os-release. This allows us to use distro specific variables here to get
+        # appropriate binary packages without having to hard code version names here.
+        return "https://packagemanager.posit.co/all/__linux__/${VERSION_CODENAME}/2022-06-03+Y3JhbiwyOjQ1MjYyMTU7RkM5ODcwN0M"
 
+    @lru_cache()
     def get_build_scripts(self):
         """
         Return series of build-steps common to all R repositories
 
         All scripts here should be independent of contents of the repository.
 
         This sets up:
@@ -261,57 +265,46 @@
           (determined by CRAN)
         - IRKernel
         - nbrsessionproxy (to access RStudio via Jupyter Notebook)
 
         We set the snapshot date used to install R libraries from based on the
         contents of runtime.txt.
         """
+        if self.checkpoint_date < RSPM_CUTOFF_DATE:
+            raise RuntimeError(
+                f'Microsoft killed MRAN, the source of R package snapshots before {RSPM_CUTOFF_DATE.strftime("%Y-%m-%d")}. '
+                f'This repo has a snapshot date of {self.checkpoint_date.strftime("%Y-%m-%d")} specified in runtime.txt. '
+                "Please use a newer snapshot date"
+            )
 
-        cran_mirror_url = self.get_cran_mirror_url(self.checkpoint_date)
-
-        # Determine which R apt repository should be enabled
-        if V(self.r_version) >= V("3.5"):
-            if V(self.r_version) >= V("4"):
-                vs = "40"
-            else:
-                vs = "35"
+        cran_mirror_url = self.get_rspm_snapshot_url(self.checkpoint_date)
 
+        if self.platform != "linux/amd64":
+            raise RuntimeError(
+                f"RStudio is only available for linux/amd64 ({self.platform})"
+            )
         scripts = [
             (
                 "root",
                 rf"""
-                echo "deb https://cloud.r-project.org/bin/linux/ubuntu bionic-cran{vs}/" > /etc/apt/sources.list.d/r-ubuntu.list
-                """,
-            ),
-            # Dont use apt-key directly, as gpg does not always respect *_proxy vars. This increase the chances
-            # of being able to reach it from behind a firewall
-            (
-                "root",
-                r"""
-                wget --quiet -O - 'https://keyserver.ubuntu.com/pks/lookup?op=get&search=0xe298a3a825c0d65dfd57cbb651716619e084dab9' | apt-key add -
-                """,
-            ),
-            (
-                "root",
-                # we should have --no-install-recommends on all our apt-get install commands,
-                # but here it's important because it will pull in CRAN packages
-                # via r-recommends, which is only guaranteed to be compatible with the latest r-base-core
-                r"""
                 apt-get update > /dev/null && \
                 apt-get install --yes --no-install-recommends \
-                        r-base-core={R_version} \
-                        r-base-dev={R_version} \
                         libclang-dev \
                         libzmq3-dev > /dev/null && \
+                wget --quiet -O /tmp/r-{self.r_version}.deb \
+                    https://cdn.rstudio.com/r/ubuntu-$(. /etc/os-release && echo $VERSION_ID | sed 's/\.//')/pkgs/r-{self.r_version}_1_amd64.deb && \
+                apt install --yes --no-install-recommends /tmp/r-{self.r_version}.deb > /dev/null && \
+                rm /tmp/r-{self.r_version}.deb && \
                 apt-get -qq purge && \
                 apt-get -qq clean && \
-                rm -rf /var/lib/apt/lists/*
-                """.format(
-                    R_version=self.r_version
-                ),
+                rm -rf /var/lib/apt/lists/* && \
+                ln -s /opt/R/{self.r_version}/bin/R /usr/local/bin/R && \
+                ln -s /opt/R/{self.r_version}/bin/Rscript /usr/local/bin/Rscript && \
+                R --version
+                """,
             ),
         ]
 
         scripts += rstudio_base_scripts(self.r_version)
 
         scripts += [
             (
@@ -322,58 +315,57 @@
                 """,
             ),
             (
                 "root",
                 # Set paths so that RStudio shares libraries with base R
                 # install. This first comments out any R_LIBS_USER that
                 # might be set in /etc/R/Renviron and then sets it.
-                r"""
-                sed -i -e '/^R_LIBS_USER=/s/^/#/' /etc/R/Renviron && \
-                echo "R_LIBS_USER=${R_LIBS_USER}" >> /etc/R/Renviron
+                rf"""
+                sed -i -e '/^R_LIBS_USER=/s/^/#/' /opt/R/{self.r_version}/lib/R/etc/Renviron && \
+                echo "R_LIBS_USER=${{R_LIBS_USER}}" >> /opt/R/{self.r_version}/lib/R/etc/Renviron
                 """,
             ),
             (
                 "root",
                 # RStudio's CRAN mirror needs this to figure out which binary package to serve.
                 # If not set properly, it will just serve up source packages
                 # Quite hilarious, IMO.
                 # See https://docs.rstudio.com/rspm/1.0.12/admin/binaries.html
                 # Set mirror for RStudio too, by modifying rsession.conf
-                r"""
+                rf"""
                 R RHOME && \
-                mkdir -p /usr/lib/R/etc /etc/rstudio && \
-                echo 'options(repos = c(CRAN = "{cran_mirror_url}"))' > /usr/lib/R/etc/Rprofile.site && \
-                echo 'options(HTTPUserAgent = sprintf("R/%s R (%s)", getRversion(), paste(getRversion(), R.version$platform, R.version$arch, R.version$os)))' >> /usr/lib/R/etc/Rprofile.site && \
-                echo 'r-cran-repos={cran_mirror_url}' > /etc/rstudio/rsession.conf
-                """.format(
-                    cran_mirror_url=cran_mirror_url
-                ),
+                mkdir -p /etc/rstudio && \
+                EXPANDED_CRAN_MIRROR_URL="$(. /etc/os-release && echo {cran_mirror_url} | envsubst)" && \
+                echo "options(repos = c(CRAN = \"${{EXPANDED_CRAN_MIRROR_URL}}\"))" > /opt/R/{self.r_version}/lib/R/etc/Rprofile.site && \
+                echo "r-cran-repos=${{EXPANDED_CRAN_MIRROR_URL}}" > /etc/rstudio/rsession.conf
+                """,
             ),
             (
                 "${NB_USER}",
                 # Install a pinned version of devtools, IRKernel and shiny
-                r"""
-                R --quiet -e "install.packages(c('devtools', 'IRkernel', 'shiny'), repos='{devtools_cran_mirror_url}')" && \
-                R --quiet -e "IRkernel::installspec(prefix='$NB_PYTHON_PREFIX')"
-                """.format(
-                    devtools_cran_mirror_url=self.get_devtools_snapshot_url()
-                ),
+                rf"""
+                export EXPANDED_CRAN_MIRROR_URL="$(. /etc/os-release && echo {cran_mirror_url} | envsubst)" && \
+                R --quiet -e "install.packages(c('devtools', 'IRkernel', 'shiny'), repos=Sys.getenv(\"EXPANDED_CRAN_MIRROR_URL\"))" && \
+                R --quiet -e "IRkernel::installspec(prefix=Sys.getenv(\"NB_PYTHON_PREFIX\"))"
+                """,
             ),
         ]
 
         return super().get_build_scripts() + scripts
 
+    @lru_cache()
     def get_preassemble_script_files(self):
         files = super().get_preassemble_script_files()
         installR_path = self.binder_path("install.R")
         if os.path.exists(installR_path):
             files[installR_path] = installR_path
 
         return files
 
+    @lru_cache()
     def get_preassemble_scripts(self):
         """Install contents of install.R
 
         Attempt to execute `install.R` before copying the contents of the
         repository. We speculate that most of the time we do not need access.
         In case this fails we re-run it after copying the repository contents.
 
@@ -385,35 +377,33 @@
         installR_path = self.binder_path("install.R")
         if os.path.exists(installR_path):
             scripts += [
                 (
                     "${NB_USER}",
                     # Delete /tmp/downloaded_packages only if install.R fails, as the second
                     # invocation of install.R might be able to reuse them
-                    "Rscript %s && touch /tmp/.preassembled || true && rm -rf /tmp/downloaded_packages"
-                    % installR_path,
+                    f"Rscript {installR_path} && touch /tmp/.preassembled || true && rm -rf /tmp/downloaded_packages",
                 )
             ]
 
         return super().get_preassemble_scripts() + scripts
 
+    @lru_cache()
     def get_assemble_scripts(self):
         """Install the dependencies of or the repository itself"""
         assemble_scripts = super().get_assemble_scripts()
 
         installR_path = self.binder_path("install.R")
         if os.path.exists(installR_path):
             assemble_scripts += [
                 (
                     "${NB_USER}",
                     # only run install.R if the pre-assembly failed
                     # Delete any downloaded packages in /tmp, as they aren't reused by R
-                    """if [ ! -f /tmp/.preassembled ]; then Rscript {}; rm -rf /tmp/downloaded_packages; fi""".format(
-                        installR_path
-                    ),
+                    f"""if [ ! -f /tmp/.preassembled ]; then Rscript {installR_path}; rm -rf /tmp/downloaded_packages; fi""",
                 )
             ]
 
         description_R = "DESCRIPTION"
         if not self.binder_dir and os.path.exists(description_R):
             assemble_scripts += [
                 ("${NB_USER}", 'R --quiet -e "devtools::install_local(getwd())"')
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/buildpacks/repo2docker-entrypoint` & `jupyter-repo2docker-2023.6.0/repo2docker/buildpacks/repo2docker-entrypoint`

 * *Files 14% similar despite different names*

```diff
@@ -8,30 +8,47 @@
 
 import fcntl
 import os
 import select
 import signal
 import subprocess
 import sys
+import tempfile
 
 # output chunk size to read
 CHUNK_SIZE = 1024
 
 # signals to be forwarded to the child
 # everything catchable, excluding SIGCHLD
 SIGNALS = set(signal.Signals) - {signal.SIGKILL, signal.SIGSTOP, signal.SIGCHLD}
 
 
 def main():
 
-    # open log file to send output
-    log_file = open(
-        os.path.join(os.environ.get("REPO_DIR", "."), ".jupyter-server-log.txt"),
-        "ab",
-    )
+    # open log file to send output to;
+    # preferred location of log file is:
+    #  1. REPO_DIR env variable
+    #  2. current working directory: "."
+    #  3. default temp directory for the OS (e.g. /tmp for linux)
+    log_dirs = [".", tempfile.gettempdir()]
+    log_file = None
+    if "REPO_DIR" in os.environ:
+        log_dirs.insert(0, os.environ["REPO_DIR"])
+    for d in log_dirs:
+        log_path = os.path.join(d, ".jupyter-server-log.txt")
+        try:
+            log_file = open(log_path, "ab")
+        except Exception:
+            continue
+        else:
+            # success
+            break
+    # raise Exception if log_file could not be set
+    if log_file is None:
+        raise Exception("Could not open '.jupyter-server-log.txt' log file " )
 
     # build the command
     # like `exec "$@"`
     command = sys.argv[1:]
     # load entrypoint override from env
     r2d_entrypoint = os.environ.get("R2D_ENTRYPOINT")
     if r2d_entrypoint:
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/base.py` & `jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/base.py`

 * *Files 12% similar despite different names*

```diff
@@ -64,10 +64,10 @@
 class Local(ContentProvider):
     def detect(self, source, ref=None, extra_args=None):
         if os.path.isdir(source):
             return {"path": source}
 
     def fetch(self, spec, output_dir, yield_output=False):
         # nothing to be done if your content is already in the output directory
-        msg = "Local content provider assumes {} == {}".format(spec["path"], output_dir)
+        msg = f'Local content provider assumes {spec["path"]} == {output_dir}'
         assert output_dir == spec["path"], msg
-        yield "Using local repo {}.\n".format(spec["path"])
+        yield f'Using local repo {spec["path"]}.\n'
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/dataverse.json` & `jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/dataverse.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.98%*

 * *Differences: {"'installations'": "{insert: [(48, OrderedDict([('description', 'The Jet Propulsion Laboratory is "*

 * *                    "a federally funded research and development center and NASA field center.'), "*

 * *                    "('full_name', 'NASA/Caltech Jet Propulsion Laboratory'), ('id', 1794), "*

 * *                    "('is_active', True), ('lat', 34.201694), ('lng', -118.171667), ('logo', "*

 * *                    "'https://www.jpl.nasa.gov/assets/images/logo_nasa_trio_black@2x.png'), "*

 * *                    "('name' […]*

```diff
@@ -619,10 +619,36 @@
             "lat": -12.068924,
             "lng": -77.079338,
             "logo": "https://dvn-h-prod.hz.lib.harvard.edu/media/logos/pucp-46x46.png",
             "name": "Pontificia Universidad Cat\u00f3lica del Per\u00fa",
             "slug": "pontificia-universidad-catolica-del-peru",
             "url": "http://datos.pucp.edu.pe",
             "version": "4.13"
+        },
+        {
+            "description": "The Jet Propulsion Laboratory is a federally funded research and development center and NASA field center.",
+            "full_name": "NASA/Caltech Jet Propulsion Laboratory",
+            "id": 1794,
+            "is_active": true,
+            "lat": 34.201694,
+            "lng": -118.171667,
+            "logo": "https://www.jpl.nasa.gov/assets/images/logo_nasa_trio_black@2x.png",
+            "name": "Jet Propulsion Laboratory",
+            "slug": "jpl",
+            "url": "https://dataverse.jpl.nasa.gov",
+            "version": "5.9"
+        },
+        {
+            "description": "The Research Data Repository for the Max Planck Society.",
+            "full_name": "Edmond - Research Data Repository for the Max Planck Society",
+            "id": 1795,
+            "is_active": true,
+            "lat": 48.1366,
+            "lng": 11.5771,
+            "logo": "https://edmond.mpdl.mpg.de/logos/navbar/logo_for_bright.png",
+            "name": "Edmond",
+            "slug": "",
+            "url": "https://edmond.mpdl.mpg.de",
+            "version": "5.10"
         }
     ]
 }
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/dataverse.py` & `jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/dataverse.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,29 @@
-import os
 import json
+import os
 import shutil
+from urllib.parse import parse_qs, urlparse, urlunparse
 
-from urllib.parse import urlparse, urlunparse, parse_qs
-
-from .doi import DoiProvider
 from ..utils import copytree, deep_get
+from .doi import DoiProvider
 
 
 class Dataverse(DoiProvider):
     """
     Provide contents of a Dataverse dataset.
 
     This class loads a a list of existing Dataverse installations from the internal
     file dataverse.json. This file is manually updated with the following command:
 
         python setup.py generate_dataverse_file
     """
 
     def __init__(self):
         data_file = os.path.join(os.path.dirname(__file__), "dataverse.json")
-        with open(data_file, "r") as fp:
+        with open(data_file) as fp:
             self.hosts = json.load(fp)["installations"]
         super().__init__()
 
     def detect(self, doi, ref=None, extra_args=None):
         """Trigger this provider for things that resolve to a Dataverse dataset.
 
         Handles:
@@ -72,17 +71,15 @@
             search_url = urlunparse(
                 parsed_url._replace(path="/api/search", query=search_query)
             )
             self.log.debug("Querying Dataverse: " + search_url)
             data = self.urlopen(search_url).json()["data"]
             if data["count_in_response"] != 1:
                 self.log.debug(
-                    "Dataverse search query failed!\n - doi: {}\n - url: {}\n - resp: {}\n".format(
-                        doi, url, json.dump(data)
-                    )
+                    f"Dataverse search query failed!\n - doi: {doi}\n - url: {url}\n - resp: {json.dump(data)}\n"
                 )
                 return
 
             self.record_id = deep_get(data, "items.0.dataset_persistent_id")
         elif (
             parsed_url.path.startswith("/dataset.xhtml")
             and "persistentId" in query_args
@@ -93,33 +90,37 @@
             return {"record": self.record_id, "host": host}
 
     def fetch(self, spec, output_dir, yield_output=False):
         """Fetch and unpack a Dataverse dataset."""
         record_id = spec["record"]
         host = spec["host"]
 
-        yield "Fetching Dataverse record {}.\n".format(record_id)
-        url = "{}/api/datasets/:persistentId?persistentId={}".format(
-            host["url"], record_id
-        )
+        yield f"Fetching Dataverse record {record_id}.\n"
+        url = f'{host["url"]}/api/datasets/:persistentId?persistentId={record_id}'
 
         resp = self.urlopen(url, headers={"accept": "application/json"})
         record = resp.json()["data"]
 
         for fobj in deep_get(record, "latestVersion.files"):
-            file_url = "{}/api/access/datafile/{}".format(
-                host["url"], deep_get(fobj, "dataFile.id")
+            file_url = (
+                # without format=original you get the preservation format (plain text, tab separated)
+                f'{host["url"]}/api/access/datafile/{deep_get(fobj, "dataFile.id")}?format=original'
             )
-            filename = os.path.join(fobj.get("directoryLabel", ""), fobj["label"])
+            filename = fobj["label"]
+            original_filename = fobj["dataFile"].get("originalFileName", None)
+            if original_filename:
+                # replace preservation format filename (foo.tab) with original filename (foo.dta)
+                filename = original_filename
+
+            filename_with_path = os.path.join(fobj.get("directoryLabel", ""), filename)
 
-            file_ref = {"download": file_url, "filename": filename}
+            file_ref = {"download": file_url, "filename": filename_with_path}
             fetch_map = {key: key for key in file_ref.keys()}
 
-            for line in self.fetch_file(file_ref, fetch_map, output_dir):
-                yield line
+            yield from self.fetch_file(file_ref, fetch_map, output_dir)
 
         new_subdirs = os.listdir(output_dir)
         # if there is only one new subdirectory move its contents
         # to the top level directory
         if len(new_subdirs) == 1 and os.path.isdir(new_subdirs[0]):
             d = new_subdirs[0]
             copytree(os.path.join(output_dir, d), output_dir)
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/doi.py` & `jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/doi.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,96 +1,93 @@
-import os
 import json
-import shutil
 import logging
-
-from os import makedirs
-from os import path
-from requests import Session, HTTPError
-
+import os
+import shutil
+from os import makedirs, path
 from zipfile import ZipFile, is_zipfile
 
-from .base import ContentProvider
-from ..utils import copytree, deep_get
-from ..utils import normalize_doi, is_doi
+from requests import HTTPError, Session
+
 from .. import __version__
+from ..utils import copytree, deep_get, is_doi, normalize_doi
+from .base import ContentProvider
 
 
 class DoiProvider(ContentProvider):
     """Provide contents of a repository identified by a DOI and some helper functions."""
 
     def __init__(self):
         super().__init__()
         self.session = Session()
         self.session.headers.update(
             {
-                "user-agent": "repo2docker {}".format(__version__),
+                "user-agent": f"repo2docker {__version__}",
             }
         )
 
     def _request(self, url, **kwargs):
         return self.session.get(url, **kwargs)
 
     urlopen = _request
 
     def _urlopen(self, req, headers=None):
         """A urlopen() helper"""
         # someone passed a string, not a request
         if not isinstance(req, request.Request):
             req = request.Request(req)
 
-        req.add_header("User-Agent", "repo2docker {}".format(__version__))
+        req.add_header("User-Agent", f"repo2docker {__version__}")
         if headers is not None:
             for key, value in headers.items():
                 req.add_header(key, value)
 
         return request.urlopen(req)
 
     def doi2url(self, doi):
         # Transform a DOI to a URL
         # If not a doi, assume we have a URL and return
         if is_doi(doi):
             doi = normalize_doi(doi)
 
             try:
-                resp = self._request("https://doi.org/{}".format(doi))
+                resp = self._request(f"https://doi.org/{doi}")
                 resp.raise_for_status()
             # If the DOI doesn't resolve, just return URL
             except HTTPError:
                 return doi
             return resp.url
         else:
             # Just return what is actulally just a URL
             return doi
 
     def fetch_file(self, file_ref, host, output_dir, unzip=False):
         # the assumption is that `unzip=True` means that this is the only
         # file related to a record
         file_url = deep_get(file_ref, host["download"])
         fname = deep_get(file_ref, host["filename"])
-        logging.debug("Downloading file {} as {}\n".format(file_url, fname))
+        logging.debug(f"Downloading file {file_url} as {fname}\n")
 
-        yield "Requesting {}\n".format(file_url)
+        yield f"Requesting {file_url}\n"
         resp = self._request(file_url, stream=True)
         resp.raise_for_status()
 
         if path.dirname(fname):
             sub_dir = path.join(output_dir, path.dirname(fname))
             if not path.exists(sub_dir):
-                yield "Creating {}\n".format(sub_dir)
+                yield f"Creating {sub_dir}\n"
                 makedirs(sub_dir, exist_ok=True)
 
         dst_fname = path.join(output_dir, fname)
         with open(dst_fname, "wb") as dst:
-            yield "Fetching {}\n".format(fname)
+            yield f"Fetching {fname}\n"
             for chunk in resp.iter_content(chunk_size=None):
                 dst.write(chunk)
 
         if unzip and is_zipfile(dst_fname):
-            yield "Extracting {}\n".format(fname)
+            yield f"Extracting {fname}\n"
             zfile = ZipFile(dst_fname)
             zfile.extractall(path=output_dir)
             zfile.close()
 
             # delete downloaded file ...
             os.remove(dst_fname)
             # ... and any directories we might have created,
@@ -102,8 +99,8 @@
             # if there is only one new subdirectory move its contents
             # to the top level directory
             if len(new_subdirs) == 1:
                 d = new_subdirs[0]
                 copytree(path.join(output_dir, d), output_dir)
                 shutil.rmtree(path.join(output_dir, d))
 
-            yield "Fetched files: {}\n".format(os.listdir(output_dir))
+            yield f"Fetched files: {os.listdir(output_dir)}\n"
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/figshare.py` & `jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/figshare.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,18 @@
+import json
 import os
 import re
-import json
 import shutil
-
-from os import makedirs
-from os import path
-from urllib.request import Request
+from os import makedirs, path
 from urllib.error import HTTPError
+from urllib.request import Request
 from zipfile import is_zipfile
 
-from .doi import DoiProvider
 from ..utils import copytree, deep_get
+from .doi import DoiProvider
 
 
 class Figshare(DoiProvider):
     """Provide contents of a Figshare article.
 
     See https://docs.figshare.com/#public_article for API docs.
 
@@ -71,30 +69,27 @@
 
     def fetch(self, spec, output_dir, yield_output=False):
         """Fetch and unpack a Figshare article"""
         article_id = spec["article"]
         article_version = spec["version"]
         host = spec["host"]
 
-        yield "Fetching Figshare article {} in version {}.\n".format(
-            article_id, article_version
-        )
+        yield f"Fetching Figshare article {article_id} in version {article_version}.\n"
         resp = self.urlopen(
-            "{}{}/versions/{}".format(host["api"], article_id, article_version),
+            f'{host["api"]}{article_id}/versions/{article_version}',
             headers={"accept": "application/json"},
         )
 
         article = resp.json()
 
         files = deep_get(article, host["filepath"])
         # only fetch files where is_link_only: False
         files = [file for file in files if not file["is_link_only"]]
         only_one_file = len(files) == 1
         for file_ref in files:
             unzip = file_ref["name"].endswith(".zip") and only_one_file
-            for line in self.fetch_file(file_ref, host, output_dir, unzip):
-                yield line
+            yield from self.fetch_file(file_ref, host, output_dir, unzip)
 
     @property
     def content_id(self):
         """The Figshare article ID"""
-        return "{}.v{}".format(self.article_id, self.article_version)
+        return f"{self.article_id}.v{self.article_version}"
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/git.py` & `jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/git.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,81 +1,77 @@
 import subprocess
-import sys
 
+from ..utils import R2dState, check_ref, execute_cmd
 from .base import ContentProvider, ContentProviderException
-from ..utils import execute_cmd, check_ref
 
 
 class Git(ContentProvider):
     """Provide contents of a remote git repository."""
 
     def detect(self, source, ref=None, extra_args=None):
         # Git is our content provider of last resort. This is to maintain the
         # old behaviour when git and local directories were the only supported
         # content providers. This means that this content provider will always
         # match. The downside is that the call to `fetch()` later on might fail
         return {"repo": source, "ref": ref}
 
     def fetch(self, spec, output_dir, yield_output=False):
         repo = spec["repo"]
-        ref = spec.get("ref", None)
+        ref = spec.get("ref") or "HEAD"
 
         # make a, possibly shallow, clone of the remote repository
         try:
             cmd = ["git", "clone"]
-            if ref is None:
+            if ref == "HEAD":
                 # check out of HEAD is performed after the clone is complete
                 cmd.extend(["--depth", "1"])
             else:
                 # don't check out HEAD, the given ref will be checked out later
                 # this prevents HEAD's submodules to be cloned if ref doesn't have them
                 cmd.extend(["--no-checkout"])
             cmd.extend([repo, output_dir])
-            for line in execute_cmd(cmd, capture=yield_output):
-                yield line
+            yield from execute_cmd(cmd, capture=yield_output)
 
         except subprocess.CalledProcessError as e:
-            msg = "Failed to clone repository from {repo}".format(repo=repo)
-            if ref is not None:
-                msg += " (ref {ref})".format(ref=ref)
+            msg = f"Failed to clone repository from {repo}"
+            if ref != "HEAD":
+                msg += f" (ref {ref})"
             msg += "."
             raise ContentProviderException(msg) from e
 
         # check out the specific ref given by the user
-        if ref is not None:
+        if ref != "HEAD":
             hash = check_ref(ref, output_dir)
             if hash is None:
                 self.log.error(
-                    "Failed to check out ref %s", ref, extra=dict(phase="failed")
+                    f"Failed to check out ref {ref}", extra=dict(phase=R2dState.FAILED)
                 )
-                if ref == "master":
+                if ref == "master" or ref == "main":
                     msg = (
-                        "Failed to check out the 'master' branch. "
-                        "Maybe the default branch is not named 'master' "
+                        f"Failed to check out the '{ref}' branch. "
+                        f"Maybe the default branch is not named '{ref}' "
                         "for this repository.\n\nTry not explicitly "
                         "specifying `--ref`."
                     )
                 else:
-                    msg = "Failed to check out ref {}".format(ref)
+                    msg = f"Failed to check out ref {ref}"
                 raise ValueError(msg)
             # We don't need to explicitly checkout things as the reset will
             # take care of that. If the hash is resolved above, we should be
             # able to reset to it
-            for line in execute_cmd(
+            yield from execute_cmd(
                 ["git", "reset", "--hard", hash], cwd=output_dir, capture=yield_output
-            ):
-                yield line
+            )
 
         # ensure that git submodules are initialised and updated
-        for line in execute_cmd(
+        yield from execute_cmd(
             ["git", "submodule", "update", "--init", "--recursive"],
             cwd=output_dir,
             capture=yield_output,
-        ):
-            yield line
+        )
 
         cmd = ["git", "rev-parse", "HEAD"]
         sha1 = subprocess.Popen(cmd, stdout=subprocess.PIPE, cwd=output_dir)
         self._sha1 = sha1.stdout.read().decode().strip()
 
     @property
     def content_id(self):
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/hydroshare.py` & `jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/hydroshare.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,18 +1,17 @@
-import zipfile
+import json
 import os
 import shutil
 import time
-import json
-from datetime import datetime, timezone, timedelta
-
+import zipfile
+from datetime import datetime, timedelta, timezone
 from urllib.request import urlretrieve
 
-from .doi import DoiProvider
 from .base import ContentProviderException
+from .doi import DoiProvider
 
 
 class Hydroshare(DoiProvider):
     """Provide contents of a Hydroshare resource."""
 
     def _fetch_version(self, host):
         """Fetch resource modified date and convert to epoch"""
@@ -55,38 +54,36 @@
         return urlretrieve(bag_url)
 
     def fetch(self, spec, output_dir, yield_output=False, timeout=120):
         """Fetch and unpack a Hydroshare resource"""
         resource_id = spec["resource"]
         host = spec["host"]
 
-        bag_url = "{}{}".format(host["django_irods"], resource_id)
+        bag_url = f'{host["django_irods"]}{resource_id}'
 
-        yield "Downloading {}.\n".format(bag_url)
+        yield f"Downloading {bag_url}.\n"
 
         # bag downloads are prepared on demand and may need some time
         conn = self.urlopen(bag_url)
         total_wait_time = 0
         while (
             conn.status_code == 200
             and conn.headers["content-type"] != "application/zip"
         ):
             wait_time = 10
             total_wait_time += wait_time
             if total_wait_time > timeout:
                 msg = "Bag taking too long to prepare, exiting now, try again later."
                 yield msg
                 raise ContentProviderException(msg)
-            yield "Bag is being prepared, requesting again in {} seconds.\n".format(
-                wait_time
-            )
+            yield f"Bag is being prepared, requesting again in {wait_time} seconds.\n"
             time.sleep(wait_time)
             conn = self.urlopen(bag_url)
         if conn.status_code != 200:
-            msg = "Failed to download bag. status code {}.\n".format(conn.status_code)
+            msg = f"Failed to download bag. status code {conn.status_code}.\n"
             yield msg
             raise ContentProviderException(msg)
         # Bag creation seems to need a small time buffer after it says it's ready.
         time.sleep(1)
         filehandle, _ = self._urlretrieve(bag_url)
         zip_file_object = zipfile.ZipFile(filehandle, "r")
         yield "Downloaded, unpacking contents.\n"
@@ -98,8 +95,8 @@
             shutil.move(os.path.join(contents_dir, f), output_dir)
         yield "Finished, cleaning up.\n"
         shutil.rmtree("temp")
 
     @property
     def content_id(self):
         """The HydroShare resource ID"""
-        return "{}.v{}".format(self.resource_id, self.version)
+        return f"{self.resource_id}.v{self.version}"
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/mercurial.py` & `jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/mercurial.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import subprocess
 
+from ..utils import R2dState, execute_cmd
 from .base import ContentProvider, ContentProviderException
-from ..utils import execute_cmd
 
 args_enabling_topic = ["--config", "extensions.topic="]
 
 
 class Mercurial(ContentProvider):
     """Provide contents of a remote Mercurial repository."""
 
@@ -37,38 +37,36 @@
                 "--config",
                 "phases.publish=False",
             ] + args_enabling_topic
             if ref is not None:
                 # don't update so the clone will include an empty working
                 # directory, the given ref will be updated out later
                 cmd.extend(["--noupdate"])
-            for line in execute_cmd(cmd, capture=yield_output):
-                yield line
+            yield from execute_cmd(cmd, capture=yield_output)
 
         except subprocess.CalledProcessError as error:
             msg = f"Failed to clone repository from {repo}"
             if ref is not None:
                 msg += f" (ref {ref})"
             msg += "."
             raise ContentProviderException(msg) from error
 
         # check out the specific ref given by the user
         if ref is not None:
             try:
-                for line in execute_cmd(
+                yield from execute_cmd(
                     ["hg", "update", "--clean", ref] + args_enabling_topic,
                     cwd=output_dir,
                     capture=yield_output,
-                ):
-                    yield line
+                )
             except subprocess.CalledProcessError:
                 self.log.error(
-                    "Failed to update to ref %s", ref, extra=dict(phase="failed")
+                    f"Failed to update to ref {ref}", extra=dict(phase=R2dState.FAILED)
                 )
-                raise ValueError("Failed to update to ref {}".format(ref))
+                raise ValueError(f"Failed to update to ref {ref}")
 
         cmd = ["hg", "identify", "-i"] + args_enabling_topic
         sha1 = subprocess.Popen(cmd, stdout=subprocess.PIPE, cwd=output_dir)
         self._node_id = sha1.stdout.read().decode().strip()
 
     @property
     def content_id(self):
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/swhid.py` & `jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/swhid.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,20 @@
 import io
 import os
+import re
 import shutil
 import tarfile
 import time
-import re
-
 from os import path
 
 import requests
 
-from .base import ContentProvider
-from ..utils import copytree
 from .. import __version__
+from ..utils import copytree
+from .base import ContentProvider
 
 
 def parse_swhid(swhid):
     swhid_regexp = r"^swh:(?P<version>\d+):(?P<type>ori|cnt|rev|dir|snp|rel):(?P<hash>[0-9a-f]{40})$"
     # only parse/check the <identifier_core> of the swhid
     # see https://docs.softwareheritage.org/devel/swh-model/persistent-identifiers.html
     m = re.match(swhid_regexp, swhid.split(";")[0])
@@ -30,20 +29,20 @@
 
     def __init__(self):
         self.swhid = None
         self.base_url = "https://archive.softwareheritage.org/api/1"
         self.session = requests.Session()
         self.session.headers.update(
             {
-                "user-agent": "repo2docker {}".format(__version__),
+                "user-agent": f"repo2docker {__version__}",
             }
         )
 
     def set_auth_token(self, token):
-        header = {"Authorization": "Bearer {}".format(token)}
+        header = {"Authorization": f"Bearer {token}"}
         self.session.headers.update(header)
 
     def _request(self, url, method="GET"):
         if not url.endswith("/"):
             url = url + "/"
 
         for retries in range(3):
@@ -68,16 +67,16 @@
             swhid_dict
             and swhid_dict["type"] in ("dir", "rev")
             and swhid_dict["version"] == "1"
         ):
             return {"swhid": swhid, "swhid_obj": swhid_dict}
 
     def fetch_directory(self, dir_hash, output_dir):
-        url = "{}/vault/directory/{}/".format(self.base_url, dir_hash)
-        yield "Fetching directory {} from {}\n".format(dir_hash, url)
+        url = f"{self.base_url}/vault/directory/{dir_hash}/"
+        yield f"Fetching directory {dir_hash} from {url}\n"
         resp = self._request(url, "POST")
         receipt = resp.json()
         status = receipt["status"]
         assert status != "failed", receipt
         while status not in ("failed", "done"):
             time.sleep(self.retry_delay)
             resp = self._request(url)
@@ -88,26 +87,26 @@
         resp = self._request(resp.json()["fetch_url"])
         archive = tarfile.open(fileobj=io.BytesIO(resp.content))
         archive.extractall(path=output_dir)
         # the output_dir should have only one subdir named after the dir_hash
         # move its content one level up
         copytree(path.join(output_dir, dir_hash), output_dir)
         shutil.rmtree(path.join(output_dir, dir_hash))
-        yield "Fetched files: {}\n".format(os.listdir(output_dir))
+        yield f"Fetched files: {os.listdir(output_dir)}\n"
 
     def fetch(self, spec, output_dir, yield_output=False):
         swhid = spec["swhid"]
         swhid_obj = spec["swhid_obj"]
 
         if swhid_obj["type"] == "rev":
             # need to get the directory for this revision
             sha1git = swhid_obj["hash"]
-            url = "{}/revision/{}/".format(self.base_url, sha1git)
-            yield "Fetching revision {} from {}\n".format(sha1git, url)
+            url = f"{self.base_url}/revision/{sha1git}/"
+            yield f"Fetching revision {sha1git} from {url}\n"
             resp = self._request(url)
             assert resp.ok, (resp.content, self.session.headers)
             directory = resp.json()["directory"]
-            self.swhid = "swh:1:dir:{}".format(directory)
+            self.swhid = f"swh:1:dir:{directory}"
             yield from self.fetch_directory(directory, output_dir)
         elif swhid_obj["type"] == "dir":
             self.swhid = swhid
             yield from self.fetch_directory(swhid_obj["hash"], output_dir)
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/contentproviders/zenodo.py` & `jupyter-repo2docker-2023.6.0/repo2docker/contentproviders/zenodo.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,30 +1,39 @@
-import os
 import json
+import os
 import shutil
-
-from os import makedirs
-from os import path
-from urllib.request import Request
+from os import makedirs, path
 from urllib.error import HTTPError
+from urllib.request import Request
 
-from .doi import DoiProvider
 from ..utils import copytree, deep_get
+from .doi import DoiProvider
 
 
 class Zenodo(DoiProvider):
     """Provide contents of a Zenodo deposit."""
 
     def __init__(self):
         super().__init__()
         # We need the hostname (url where records are), api url (for metadata),
         # filepath (path to files in metadata), filename (path to filename in
         # metadata), download (path to file download URL), and type (path to item type in metadata)
         self.hosts = [
             {
+                "hostname": [
+                    "https://sandbox.zenodo.org/record/",
+                    "http://sandbox.zenodo.org/record/",
+                ],
+                "api": "https://sandbox.zenodo.org/api/records/",
+                "filepath": "files",
+                "filename": "filename",
+                "download": "links.download",
+                "type": "metadata.upload_type",
+            },
+            {
                 "hostname": ["https://zenodo.org/record/", "http://zenodo.org/record/"],
                 "api": "https://zenodo.org/api/records/",
                 "filepath": "files",
                 "filename": "filename",
                 "download": "links.download",
                 "type": "metadata.upload_type",
             },
@@ -51,27 +60,24 @@
                 return {"record": self.record_id, "host": host}
 
     def fetch(self, spec, output_dir, yield_output=False):
         """Fetch and unpack a Zenodo record"""
         record_id = spec["record"]
         host = spec["host"]
 
-        yield "Fetching Zenodo record {}.\n".format(record_id)
+        yield f"Fetching Zenodo record {record_id}.\n"
         resp = self.urlopen(
-            "{}{}".format(host["api"], record_id),
+            f'{host["api"]}{record_id}',
             headers={"accept": "application/json"},
         )
 
         record = resp.json()
 
         files = deep_get(record, host["filepath"])
         only_one_file = len(files) == 1
         for file_ref in files:
-            for line in self.fetch_file(
-                file_ref, host, output_dir, unzip=only_one_file
-            ):
-                yield line
+            yield from self.fetch_file(file_ref, host, output_dir, unzip=only_one_file)
 
     @property
     def content_id(self):
         """The Zenodo record ID as the content of a record is immutable"""
         return self.record_id
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/docker.py` & `jupyter-repo2docker-2023.6.0/repo2docker/docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 Docker container engine for repo2docker
 """
 
-import docker
-from traitlets import Dict
 from iso8601 import parse_date
+from traitlets import Dict
+
+import docker
 
 from .engine import Container, ContainerEngine, ContainerEngineException, Image
 
 
 class DockerContainer(Container):
     def __init__(self, container):
         self._c = container
@@ -86,14 +87,15 @@
         container_limits=None,
         tag="",
         custom_context=False,
         dockerfile="",
         fileobj=None,
         path="",
         labels=None,
+        platform=None,
         **kwargs,
     ):
         return self._apiclient.build(
             buildargs=buildargs,
             cache_from=cache_from,
             container_limits=container_limits,
             forcerm=True,
@@ -101,26 +103,29 @@
             tag=tag,
             custom_context=custom_context,
             decode=True,
             dockerfile=dockerfile,
             fileobj=fileobj,
             path=path,
             labels=labels,
+            platform=platform,
             **kwargs,
         )
 
     def images(self):
         images = self._apiclient.images()
         return [Image(tags=image["RepoTags"]) for image in images]
 
     def inspect_image(self, image):
         image = self._apiclient.inspect_image(image)
         return Image(tags=image["RepoTags"], config=image["ContainerConfig"])
 
     def push(self, image_spec):
+        if self.registry_credentials:
+            self._apiclient.login(**self.registry_credentials)
         return self._apiclient.push(image_spec, stream=True)
 
     def run(
         self,
         image_spec,
         *,
         command=None,
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/engine.py` & `jupyter-repo2docker-2023.6.0/repo2docker/engine.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 """
 Interface for a repo2docker container engine
 """
 
+import json
+import os
 from abc import ABC, abstractmethod
-from traitlets.config import LoggingConfigurable
 
+from traitlets import Dict, default
+from traitlets.config import LoggingConfigurable
 
 # Based on https://docker-py.readthedocs.io/en/4.2.0/containers.html
 
 
 class Container(ABC):
     """
     Abstract container returned by repo2docker engines
@@ -127,25 +130,56 @@
         If this is `None` the information has not been loaded.
         If not `None` this must include the following fields:
         - WorkingDir: The default working directory
         """
         return self._config
 
     def __repr__(self):
-        return "Image(tags={},config={})".format(self.tags, self.config)
+        return f"Image(tags={self.tags},config={self.config})"
 
 
 class ContainerEngine(LoggingConfigurable):
     """
     Abstract container engine.
 
     Inherits from LoggingConfigurable, which means it has a log property.
     Initialised with a reference to the parent so can also be configured using traitlets.
     """
 
+    registry_credentials = Dict(
+        help="""
+        Credentials dictionary, if set will be used to authenticate with
+        the registry. Typically this will include the keys:
+
+            - `username`: The registry username
+            - `password`: The registry password or token
+            - `registry`: The registry URL
+
+        This can also be set by passing a JSON object in the
+        CONTAINER_ENGINE_REGISTRY_CREDENTIALS environment variable.
+        """,
+        config=True,
+    )
+
+    @default("registry_credentials")
+    def _registry_credentials_default(self):
+        """
+        Set the registry credentials from CONTAINER_ENGINE_REGISTRY_CREDENTIALS
+        """
+        obj = os.getenv("CONTAINER_ENGINE_REGISTRY_CREDENTIALS")
+        if obj:
+            try:
+                return json.loads(obj)
+            except json.JSONDecodeError:
+                self.log.error(
+                    "CONTAINER_ENGINE_REGISTRY_CREDENTIALS is not valid JSON"
+                )
+                raise
+        return {}
+
     string_output = True
     """
     Whether progress events should be strings or an object.
 
     Originally Docker was the only container engine supported by repo2docker.
     Some operations including build() and push() would return generators of events in a Docker specific format.
     This format of events is not easily constructable with other engines so the default is to return strings and raise an exception if an error occurs.
@@ -173,14 +207,15 @@
         container_limits={},
         tag="",
         custom_context=False,
         dockerfile="",
         fileobj=None,
         path="",
         labels=None,
+        platform=None,
         **kwargs,
     ):
         """
         Build a container
 
         Parameters
         ----------
@@ -203,14 +238,16 @@
             Path to Dockerfile within the build context
         fileobj : tarfile
             A tar file-like object containing the build context
         path : str
             path to the Dockerfile
         labels : dict
             Dictionary of labels to set on the image
+        platform: str
+            Platform to build for
 
         Returns
         -------
         A generator of strings. If an error occurs an exception must be thrown.
 
         If `string_output=True` this should instead be whatever Docker returns:
         https://github.com/jupyter/repo2docker/blob/0.11.0/repo2docker/app.py#L725-L735
@@ -244,14 +281,17 @@
         """
         raise NotImplementedError("inspect_image not implemented")
 
     def push(self, image_spec):
         """
         Push image to a registry
 
+        If the registry_credentials traitlets is set it should be used to
+        authenticate with the registry before pushing.
+
         Parameters
         ----------
         image_spec : str
             The repository spec to push to
 
         Returns
         -------
```

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/semver.py` & `jupyter-repo2docker-2023.6.0/repo2docker/semver.py`

 * *Files identical despite different names*

### Comparing `jupyter-repo2docker-2022.2.0/repo2docker/utils.py` & `jupyter-repo2docker-2023.6.0/repo2docker/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,34 @@
-from contextlib import contextmanager
-from functools import partial
 import os
+import platform
 import re
 import subprocess
+import warnings
+from contextlib import contextmanager
+from enum import Enum
+from functools import partial
+from shutil import copy2, copystat
+
 import chardet
+from traitlets import Integer, TraitError
 
-from shutil import copystat, copy2
 
-from traitlets import Integer, TraitError
+class R2dState(Enum):
+    """
+    The current state of repo2docker
+    """
+
+    FETCHING = "fetching"
+    BUILDING = "building"
+    PUSHING = "pushing"
+    RUNNING = "running"
+    FAILED = "failed"
+
+    def __str__(self):
+        return self.value
 
 
 def execute_cmd(cmd, capture=False, **kwargs):
     """
     Call given command, yielding output line by line if capture=True.
 
     Must be yielded from.
@@ -116,47 +133,48 @@
         (docker-py supports this but repo2docker does not)
     """
 
     def check_port(port):
         try:
             p = int(port)
         except ValueError as e:
+            raise ValueError(f'Port specification "{mapping}" has an invalid port.')
+        if not 0 < p <= 65535:
             raise ValueError(
-                'Port specification "{}" has ' "an invalid port.".format(mapping)
-            )
-        if p > 65535:
-            raise ValueError(
-                'Port specification "{}" specifies '
-                "a port above 65535.".format(mapping)
+                f'Port specification "{mapping}" specifies a port outside 1-65535.'
             )
         return port
 
     def check_port_string(p):
         parts = p.split("/")
         if len(parts) == 2:  # 134/tcp
             port, protocol = parts
             if protocol not in ("tcp", "udp"):
                 raise ValueError(
-                    'Port specification "{}" has '
-                    "an invalid protocol.".format(mapping)
+                    f'Port specification "{mapping}" has an invalid protocol.'
                 )
         elif len(parts) == 1:
             port = parts[0]
             protocol = "tcp"
 
         check_port(port)
 
         return "/".join((port, protocol))
 
     ports = {}
     if port_mappings is None:
         return ports
 
     for mapping in port_mappings:
-        parts = mapping.split(":")
+        if ":" in mapping:
+            parts = mapping.split(":")
+        else:
+            # single port '8888' specified,
+            # treat as '8888:8888'
+            parts = [mapping, mapping]
 
         *host, container_port = parts
         # just a port
         if len(host) == 1:
             host = check_port(host[0])
         else:
             host = tuple((host[0], check_port(host[1])))
@@ -285,22 +303,22 @@
         if isinstance(value, (int, float)):
             return int(value)
 
         try:
             num = float(value[:-1])
         except ValueError:
             raise TraitError(
-                "{val} is not a valid memory specification. "
-                "Must be an int or a string with suffix K, M, G, T".format(val=value)
+                f"{value} is not a valid memory specification. "
+                "Must be an int or a string with suffix K, M, G, T"
             )
         suffix = value[-1]
         if suffix not in self.UNIT_SUFFIXES:
             raise TraitError(
-                "{val} is not a valid memory specification. "
-                "Must be an int or a string with suffix K, M, G, T".format(val=value)
+                f"{value} is not a valid memory specification. "
+                "Must be an int or a string with suffix K, M, G, T"
             )
         else:
             return int(float(num) * self.UNIT_SUFFIXES[suffix])
 
 
 def check_ref(ref, cwd=None):
     """Prepare a ref and ensure it works with git reset --hard."""
@@ -504,7 +522,26 @@
         path = line
 
     if path.startswith("."):
         # references a local file
         return True
 
     return False
+
+
+def get_platform():
+    """Return the target platform of the container image
+
+    Returns either `linux/amd64` or `linux/arm64`
+    """
+    m = platform.machine()
+    if m == "x86_64":
+        return "linux/amd64"
+    elif m == "aarch64":
+        # Linux reports aarch64
+        return "linux/arm64"
+    elif m == "arm64":
+        # OSX reports arm64
+        return "linux/arm64"
+    else:
+        warnings.warn(f"Unexpected platform '{m}', defaulting to linux/amd64")
+        return "linux/amd64"
```

### Comparing `jupyter-repo2docker-2022.2.0/setup.py` & `jupyter-repo2docker-2023.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,12 @@
-from distutils.cmd import Command
-from setuptools import setup, find_packages
 import sys
+from distutils.cmd import Command
+
+from setuptools import find_packages, setup
+
 import versioneer
 
 if sys.version_info[0] < 3:
     readme = None
 else:
     with open("README.md", encoding="utf8") as f:
         readme = f.read()
@@ -19,16 +21,16 @@
             "https://services.dataverse.harvard.edu/miniverse/map/installations-json"
         )
 
     def finalize_options(self):
         pass
 
     def run(self):
-        from urllib.request import urlopen
         import json
+        from urllib.request import urlopen
 
         resp = urlopen(self.url, timeout=5)
         resp_body = resp.read()
         data = json.loads(resp_body.decode("utf-8"))
         if "installations" not in data:
             raise ValueError("Malformed installation map.")
```

### Comparing `jupyter-repo2docker-2022.2.0/versioneer.py` & `jupyter-repo2docker-2023.6.0/versioneer.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,15 +271,14 @@
 domain. The `_version.py` that it creates is also in the public domain.
 Specifically, both are released under the Creative Commons "Public Domain
 Dedication" license (CC0-1.0), as described in
 https://creativecommons.org/publicdomain/zero/1.0/ .
 
 """
 
-from __future__ import print_function
 
 try:
     import configparser
 except ImportError:
     import ConfigParser as configparser
 import errno
 import json
@@ -340,15 +339,15 @@
     """Read the project setup.cfg file to determine Versioneer config."""
     # This might raise EnvironmentError (if setup.cfg is missing), or
     # configparser.NoSectionError (if it lacks a [versioneer] section), or
     # configparser.NoOptionError (if it lacks "VCS="). See the docstring at
     # the top of versioneer.py for instructions on writing your setup.cfg .
     setup_cfg = os.path.join(root, "setup.cfg")
     parser = configparser.SafeConfigParser()
-    with open(setup_cfg, "r") as f:
+    with open(setup_cfg) as f:
         parser.readfp(f)
     VCS = parser.get("versioneer", "VCS")  # mandatory
 
     def get(parser, name):
         if parser.has_option("versioneer", name):
             return parser.get("versioneer", name)
         return None
@@ -400,40 +399,40 @@
                 [c] + args,
                 cwd=cwd,
                 env=env,
                 stdout=subprocess.PIPE,
                 stderr=(subprocess.PIPE if hide_stderr else None),
             )
             break
-        except EnvironmentError:
+        except OSError:
             e = sys.exc_info()[1]
             if e.errno == errno.ENOENT:
                 continue
             if verbose:
                 print("unable to run %s" % dispcmd)
                 print(e)
             return None, None
     else:
         if verbose:
-            print("unable to find command, tried %s" % (commands,))
+            print(f"unable to find command, tried {commands}")
         return None, None
     stdout = p.communicate()[0].strip()
     if sys.version_info[0] >= 3:
         stdout = stdout.decode()
     if p.returncode != 0:
         if verbose:
             print("unable to run %s (error)" % dispcmd)
             print("stdout was %s" % stdout)
         return None, p.returncode
     return stdout, p.returncode
 
 
 LONG_VERSION_PY[
     "git"
-] = '''
+] = r'''
 # This file helps to compute a version number in source trees obtained from
 # git-archive tarball (such as those provided by githubs download-from-tag
 # feature). Distribution tarballs (built by setup.py sdist) and build
 # directories (produced by setup.py build) will contain a much shorter file
 # that just contains the computed version number.
 
 # This file is released into the public domain. Generated by
@@ -957,30 +956,30 @@
     """Extract version information from the given file."""
     # the code embedded in _version.py can just fetch the value of these
     # keywords. When used from setup.py, we don't want to import _version.py,
     # so we do it with a regexp instead. This function is not used from
     # _version.py.
     keywords = {}
     try:
-        f = open(versionfile_abs, "r")
+        f = open(versionfile_abs)
         for line in f.readlines():
             if line.strip().startswith("git_refnames ="):
                 mo = re.search(r'=\s*"(.*)"', line)
                 if mo:
                     keywords["refnames"] = mo.group(1)
             if line.strip().startswith("git_full ="):
                 mo = re.search(r'=\s*"(.*)"', line)
                 if mo:
                     keywords["full"] = mo.group(1)
             if line.strip().startswith("git_date ="):
                 mo = re.search(r'=\s*"(.*)"', line)
                 if mo:
                     keywords["date"] = mo.group(1)
         f.close()
-    except EnvironmentError:
+    except OSError:
         pass
     return keywords
 
 
 @register_vcs_handler("git", "keywords")
 def git_versions_from_keywords(keywords, tag_prefix, verbose):
     """Get version information from git keywords."""
@@ -996,28 +995,28 @@
         # older one.
         date = date.strip().replace(" ", "T", 1).replace(" ", "", 1)
     refnames = keywords["refnames"].strip()
     if refnames.startswith("$Format"):
         if verbose:
             print("keywords are unexpanded, not using")
         raise NotThisMethod("unexpanded keywords, not a git-archive tarball")
-    refs = set([r.strip() for r in refnames.strip("()").split(",")])
+    refs = {r.strip() for r in refnames.strip("()").split(",")}
     # starting in git-1.8.3, tags are listed as "tag: foo-1.0" instead of
     # just "foo-1.0". If we see a "tag: " prefix, prefer those.
     TAG = "tag: "
-    tags = set([r[len(TAG) :] for r in refs if r.startswith(TAG)])
+    tags = {r[len(TAG) :] for r in refs if r.startswith(TAG)}
     if not tags:
         # Either we're using git < 1.8.3, or there really are no tags. We use
         # a heuristic: assume all version tags have a digit. The old git %d
         # expansion behaves like git log --decorate=short and strips out the
         # refs/heads/ and refs/tags/ prefixes that would let us distinguish
         # between branches and tags. By ignoring refnames without digits, we
         # filter out many common branch names like "release" and
         # "stabilization", as well as "HEAD" and "master".
-        tags = set([r for r in refs if re.search(r"\d", r)])
+        tags = {r for r in refs if re.search(r"\d", r)}
         if verbose:
             print("discarding '%s', no digits" % ",".join(refs - tags))
     if verbose:
         print("likely tags: %s" % ",".join(sorted(tags)))
     for ref in sorted(tags):
         # sorting will prefer e.g. "2.0" over "2.0rc1"
         if ref.startswith(tag_prefix):
@@ -1103,27 +1102,26 @@
     # now we have TAG-NUM-gHEX or HEX
 
     if "-" in git_describe:
         # TAG-NUM-gHEX
         mo = re.search(r"^(.+)-(\d+)-g([0-9a-f]+)$", git_describe)
         if not mo:
             # unparseable. Maybe git-describe is misbehaving?
-            pieces["error"] = "unable to parse git-describe output: '%s'" % describe_out
+            pieces["error"] = f"unable to parse git-describe output: '{describe_out}'"
             return pieces
 
         # tag
         full_tag = mo.group(1)
         if not full_tag.startswith(tag_prefix):
             if verbose:
                 fmt = "tag '%s' doesn't start with prefix '%s'"
                 print(fmt % (full_tag, tag_prefix))
-            pieces["error"] = "tag '%s' doesn't start with prefix '%s'" % (
-                full_tag,
-                tag_prefix,
-            )
+            pieces[
+                "error"
+            ] = f"tag '{full_tag}' doesn't start with prefix '{tag_prefix}'"
             return pieces
         pieces["closest-tag"] = full_tag[len(tag_prefix) :]
 
         # distance: number of commits since tag
         pieces["distance"] = int(mo.group(2))
 
         # commit: short hex revision ID
@@ -1162,21 +1160,21 @@
             me = os.path.splitext(me)[0] + ".py"
         versioneer_file = os.path.relpath(me)
     except NameError:
         versioneer_file = "versioneer.py"
     files.append(versioneer_file)
     present = False
     try:
-        f = open(".gitattributes", "r")
+        f = open(".gitattributes")
         for line in f.readlines():
             if line.strip().startswith(versionfile_source):
                 if "export-subst" in line.strip().split()[1:]:
                     present = True
         f.close()
-    except EnvironmentError:
+    except OSError:
         pass
     if not present:
         f = open(".gitattributes", "a+")
         f.write("%s export-subst\n" % versionfile_source)
         f.close()
         files.append(".gitattributes")
     run_command(GITS, ["add", "--"] + files)
@@ -1232,15 +1230,15 @@
 
 
 def versions_from_file(filename):
     """Try to determine the version from _version.py if present."""
     try:
         with open(filename) as f:
             contents = f.read()
-    except EnvironmentError:
+    except OSError:
         raise NotThisMethod("unable to read _version.py")
     mo = re.search(
         r"version_json = '''\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
     )
     if not mo:
         mo = re.search(
             r"version_json = '''\r\n(.*)'''  # END VERSION_JSON", contents, re.M | re.S
@@ -1253,15 +1251,15 @@
 def write_to_version_file(filename, versions):
     """Write the given version number to the given _version.py file."""
     os.unlink(filename)
     contents = json.dumps(versions, sort_keys=True, indent=1, separators=(",", ": "))
     with open(filename, "w") as f:
         f.write(SHORT_VERSION_PY % contents)
 
-    print("set %s to '%s'" % (filename, versions["version"]))
+    print(f"set {filename} to '{versions['version']}'")
 
 
 def plus_or_dot(pieces):
     """Return a + if we don't already have one, else return a ."""
     if "+" in pieces.get("closest-tag", ""):
         return "."
     return "+"
@@ -1478,15 +1476,15 @@
             return ver
         except NotThisMethod:
             pass
 
     try:
         ver = versions_from_file(versionfile_abs)
         if verbose:
-            print("got version from file %s %s" % (versionfile_abs, ver))
+            print(f"got version from file {versionfile_abs} {ver}")
         return ver
     except NotThisMethod:
         pass
 
     from_vcs_f = handlers.get("pieces_from_vcs")
     if from_vcs_f:
         try:
@@ -1751,19 +1749,15 @@
 
 
 def do_setup():
     """Main VCS-independent setup function for installing Versioneer."""
     root = get_root()
     try:
         cfg = get_config_from_root(root)
-    except (
-        EnvironmentError,
-        configparser.NoSectionError,
-        configparser.NoOptionError,
-    ) as e:
+    except (OSError, configparser.NoSectionError, configparser.NoOptionError) as e:
         if isinstance(e, (EnvironmentError, configparser.NoSectionError)):
             print("Adding sample versioneer config to setup.cfg", file=sys.stderr)
             with open(os.path.join(root, "setup.cfg"), "a") as f:
                 f.write(SAMPLE_CONFIG)
         print(CONFIG_ERROR, file=sys.stderr)
         return 1
 
@@ -1780,17 +1774,17 @@
                 "VERSIONFILE_SOURCE": cfg.versionfile_source,
             }
         )
 
     ipy = os.path.join(os.path.dirname(cfg.versionfile_source), "__init__.py")
     if os.path.exists(ipy):
         try:
-            with open(ipy, "r") as f:
+            with open(ipy) as f:
                 old = f.read()
-        except EnvironmentError:
+        except OSError:
             old = ""
         if INIT_PY_SNIPPET not in old:
             print(" appending to %s" % ipy)
             with open(ipy, "a") as f:
                 f.write(INIT_PY_SNIPPET)
         else:
             print(" %s unmodified" % ipy)
@@ -1801,20 +1795,20 @@
     # Make sure both the top-level "versioneer.py" and versionfile_source
     # (PKG/_version.py, used by runtime code) are in MANIFEST.in, so
     # they'll be copied into source distributions. Pip won't be able to
     # install the package without this.
     manifest_in = os.path.join(root, "MANIFEST.in")
     simple_includes = set()
     try:
-        with open(manifest_in, "r") as f:
+        with open(manifest_in) as f:
             for line in f:
                 if line.startswith("include "):
                     for include in line.split()[1:]:
                         simple_includes.add(include)
-    except EnvironmentError:
+    except OSError:
         pass
     # That doesn't cover everything MANIFEST.in can do
     # (http://docs.python.org/2/distutils/sourcedist.html#commands), so
     # it might give some false negatives. Appending redundant 'include'
     # lines is safe, though.
     if "versioneer.py" not in simple_includes:
         print(" appending 'versioneer.py' to MANIFEST.in")
@@ -1840,15 +1834,15 @@
 
 
 def scan_setup_py():
     """Validate the contents of setup.py against Versioneer's expectations."""
     found = set()
     setters = False
     errors = 0
-    with open("setup.py", "r") as f:
+    with open("setup.py") as f:
         for line in f.readlines():
             if "import versioneer" in line:
                 found.add("import")
             if "versioneer.get_cmdclass()" in line:
                 found.add("cmdclass")
             if "versioneer.get_version()" in line:
                 found.add("get_version")
```

