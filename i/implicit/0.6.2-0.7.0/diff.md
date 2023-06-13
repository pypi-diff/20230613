# Comparing `tmp/implicit-0.6.2.tar.gz` & `tmp/implicit-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "implicit-0.6.2.tar", last modified: Wed Jun  7 18:24:02 2023, max compression
+gzip compressed data, was "implicit-0.7.0.tar", last modified: Tue Jun 13 05:14:54 2023, max compression
```

## Comparing `implicit-0.6.2.tar` & `implicit-0.7.0.tar`

### file list

```diff
@@ -1,81 +1,81 @@
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2023-06-07 18:24:02.221217 implicit-0.6.2/
--rw-rw-r--   0 ben       (1000) ben       (1000)      247 2023-01-08 04:50:20.000000 implicit-0.6.2/CMakeLists.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)     1083 2023-01-08 04:50:20.000000 implicit-0.6.2/LICENSE
--rw-rw-r--   0 ben       (1000) ben       (1000)      248 2023-06-07 18:22:58.000000 implicit-0.6.2/MANIFEST.in
--rw-rw-r--   0 ben       (1000) ben       (1000)     6020 2023-06-07 18:24:02.221217 implicit-0.6.2/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)     5170 2023-05-29 21:38:00.000000 implicit-0.6.2/README.md
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2023-06-07 18:24:02.217217 implicit-0.6.2/implicit/
--rw-rw-r--   0 ben       (1000) ben       (1000)      670 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/CMakeLists.txt
--rw-r--r--   0 ben       (1000) ben       (1000)      177 2023-06-07 17:34:01.000000 implicit-0.6.2/implicit/__init__.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     5777 2023-05-29 21:38:00.000000 implicit-0.6.2/implicit/_nearest_neighbours.pyx
--rw-rw-r--   0 ben       (1000) ben       (1000)     2682 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/als.py
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2023-06-07 18:24:02.217217 implicit-0.6.2/implicit/ann/
--rw-rw-r--   0 ben       (1000) ben       (1000)        0 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/ann/__init__.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     9132 2023-05-29 21:38:00.000000 implicit-0.6.2/implicit/ann/annoy.py
--rw-rw-r--   0 ben       (1000) ben       (1000)    10476 2023-05-29 21:38:00.000000 implicit-0.6.2/implicit/ann/faiss.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     9475 2023-05-29 21:38:00.000000 implicit-0.6.2/implicit/ann/nmslib.py
--rw-r--r--   0 ben       (1000) ben       (1000)     2249 2023-06-07 17:34:01.000000 implicit-0.6.2/implicit/approximate_als.py
--rw-r--r--   0 ben       (1000) ben       (1000)     2604 2023-06-07 17:34:01.000000 implicit-0.6.2/implicit/bpr.py
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2023-06-07 18:24:02.217217 implicit-0.6.2/implicit/cpu/
--rw-rw-r--   0 ben       (1000) ben       (1000)      903 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/cpu/CMakeLists.txt
--rw-r--r--   0 ben       (1000) ben       (1000)        0 2023-06-07 17:34:01.000000 implicit-0.6.2/implicit/cpu/__init__.py
--rw-rw-r--   0 ben       (1000) ben       (1000)    11462 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/cpu/_als.pyx
--rw-rw-r--   0 ben       (1000) ben       (1000)    20235 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/cpu/als.py
--rw-rw-r--   0 ben       (1000) ben       (1000)      542 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/cpu/bpr.h
--rw-rw-r--   0 ben       (1000) ben       (1000)    12499 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/cpu/bpr.pyx
--rw-rw-r--   0 ben       (1000) ben       (1000)    11745 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/cpu/lmf.pyx
--rw-r--r--   0 ben       (1000) ben       (1000)     9523 2023-06-07 17:34:01.000000 implicit-0.6.2/implicit/cpu/matrix_factorization_base.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1208 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/cpu/select.h
--rw-rw-r--   0 ben       (1000) ben       (1000)     2665 2023-05-29 21:38:00.000000 implicit-0.6.2/implicit/cpu/topk.pyx
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2023-06-07 18:24:02.217217 implicit-0.6.2/implicit/datasets/
--rw-rw-r--   0 ben       (1000) ben       (1000)        0 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/datasets/__init__.py
--rw-rw-r--   0 ben       (1000) ben       (1000)      769 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/datasets/_download.py
--rw-r--r--   0 ben       (1000) ben       (1000)     3883 2023-05-29 21:35:55.000000 implicit-0.6.2/implicit/datasets/github.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     3237 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/datasets/lastfm.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     4592 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/datasets/million_song_dataset.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     3819 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/datasets/movielens.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     2876 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/datasets/reddit.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     2820 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/datasets/sketchfab.py
--rw-rw-r--   0 ben       (1000) ben       (1000)    16532 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/evaluation.pyx
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2023-06-07 18:24:02.221217 implicit-0.6.2/implicit/gpu/
--rw-rw-r--   0 ben       (1000) ben       (1000)     2816 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/gpu/CMakeLists.txt
--rw-r--r--   0 ben       (1000) ben       (1000)      364 2023-06-07 17:34:01.000000 implicit-0.6.2/implicit/gpu/__init__.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     8577 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/gpu/_cuda.pyx
--rw-rw-r--   0 ben       (1000) ben       (1000)     8603 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/gpu/als.cu
--rw-rw-r--   0 ben       (1000) ben       (1000)      741 2023-05-29 22:59:24.000000 implicit-0.6.2/implicit/gpu/als.h
--rw-rw-r--   0 ben       (1000) ben       (1000)      606 2023-05-29 21:38:00.000000 implicit-0.6.2/implicit/gpu/als.pxd
--rw-rw-r--   0 ben       (1000) ben       (1000)    12042 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/gpu/als.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     4882 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/gpu/bpr.cu
--rw-rw-r--   0 ben       (1000) ben       (1000)      548 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/gpu/bpr.h
--rw-rw-r--   0 ben       (1000) ben       (1000)      616 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/gpu/bpr.pxd
--rw-r--r--   0 ben       (1000) ben       (1000)     7001 2023-06-07 17:34:01.000000 implicit-0.6.2/implicit/gpu/bpr.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1662 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/gpu/dot.cuh
--rw-rw-r--   0 ben       (1000) ben       (1000)    14929 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/gpu/knn.cu
--rw-rw-r--   0 ben       (1000) ben       (1000)      915 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/gpu/knn.h
--rw-rw-r--   0 ben       (1000) ben       (1000)      456 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/gpu/knn.pxd
--rw-rw-r--   0 ben       (1000) ben       (1000)     7648 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/gpu/matrix.cu
--rw-rw-r--   0 ben       (1000) ben       (1000)     2136 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/gpu/matrix.h
--rw-rw-r--   0 ben       (1000) ben       (1000)     1570 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/gpu/matrix.pxd
--rw-r--r--   0 ben       (1000) ben       (1000)     8998 2023-06-07 17:34:01.000000 implicit-0.6.2/implicit/gpu/matrix_factorization_base.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     1209 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/gpu/random.cu
--rw-rw-r--   0 ben       (1000) ben       (1000)      583 2023-05-29 21:38:00.000000 implicit-0.6.2/implicit/gpu/random.h
--rw-rw-r--   0 ben       (1000) ben       (1000)      337 2023-05-29 21:38:00.000000 implicit-0.6.2/implicit/gpu/random.pxd
--rw-rw-r--   0 ben       (1000) ben       (1000)     2488 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/gpu/utils.h
--rw-rw-r--   0 ben       (1000) ben       (1000)      109 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/gpu/utils.pxd
--rw-r--r--   0 ben       (1000) ben       (1000)     2272 2023-06-07 17:34:01.000000 implicit-0.6.2/implicit/lmf.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     2202 2023-01-08 04:50:20.000000 implicit-0.6.2/implicit/nearest_neighbours.h
--rw-rw-r--   0 ben       (1000) ben       (1000)     8688 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/nearest_neighbours.py
--rw-r--r--   0 ben       (1000) ben       (1000)     8218 2023-06-07 17:34:01.000000 implicit-0.6.2/implicit/recommender_base.py
--rw-rw-r--   0 ben       (1000) ben       (1000)     5427 2023-06-07 18:18:21.000000 implicit-0.6.2/implicit/utils.py
-drwxrwxr-x   0 ben       (1000) ben       (1000)        0 2023-06-07 18:24:02.217217 implicit-0.6.2/implicit.egg-info/
--rw-rw-r--   0 ben       (1000) ben       (1000)     6020 2023-06-07 18:24:02.000000 implicit-0.6.2/implicit.egg-info/PKG-INFO
--rw-rw-r--   0 ben       (1000) ben       (1000)     1693 2023-06-07 18:24:02.000000 implicit-0.6.2/implicit.egg-info/SOURCES.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)        1 2023-06-07 18:24:02.000000 implicit-0.6.2/implicit.egg-info/dependency_links.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       29 2023-06-07 18:24:02.000000 implicit-0.6.2/implicit.egg-info/requires.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)        9 2023-06-07 18:24:02.000000 implicit-0.6.2/implicit.egg-info/top_level.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)     1000 2023-06-07 18:18:20.000000 implicit-0.6.2/pyproject.toml
--rw-rw-r--   0 ben       (1000) ben       (1000)       93 2023-01-08 04:50:20.000000 implicit-0.6.2/requirements-dev.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)       42 2023-01-08 04:50:20.000000 implicit-0.6.2/requirements.txt
--rw-rw-r--   0 ben       (1000) ben       (1000)      701 2023-06-07 18:24:02.221217 implicit-0.6.2/setup.cfg
--rw-rw-r--   0 ben       (1000) ben       (1000)     2204 2023-06-07 18:18:21.000000 implicit-0.6.2/setup.py
--rw-rw-r--   0 ben       (1000) ben       (1000)      329 2023-01-08 04:50:20.000000 implicit-0.6.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:14:54.737289 implicit-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-06-13 05:01:40.000000 implicit-0.7.0/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-06-13 05:01:40.000000 implicit-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-13 05:01:40.000000 implicit-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-13 05:14:54.737289 implicit-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5170 2023-06-13 05:01:40.000000 implicit-0.7.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:14:54.733289 implicit-0.7.0/implicit/
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/_nearest_neighbours.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/als.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:14:54.733289 implicit-0.7.0/implicit/ann/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/ann/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9132 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/ann/annoy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10476 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/ann/faiss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9475 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/ann/nmslib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2249 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/approximate_als.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2604 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/bpr.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:14:54.733289 implicit-0.7.0/implicit/cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)      903 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/cpu/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/cpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11859 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/cpu/_als.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    20339 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/cpu/als.py
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/cpu/bpr.h
+-rw-r--r--   0 runner    (1001) docker     (123)    12441 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/cpu/bpr.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)    11687 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/cpu/lmf.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     9523 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/cpu/matrix_factorization_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1208 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/cpu/select.h
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/cpu/topk.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:14:54.733289 implicit-0.7.0/implicit/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      769 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/datasets/_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/datasets/lastfm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4592 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/datasets/million_song_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/datasets/movielens.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/datasets/reddit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2820 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/datasets/sketchfab.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16475 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/evaluation.pyx
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:14:54.737289 implicit-0.7.0/implicit/gpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     2500 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/CMakeLists.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9996 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/_cuda.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     9912 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/als.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/als.h
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/als.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)    12909 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/als.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4837 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/bpr.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/bpr.h
+-rw-r--r--   0 runner    (1001) docker     (123)      616 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/bpr.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     7001 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/bpr.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/convert.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)     1662 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/dot.cuh
+-rw-r--r--   0 runner    (1001) docker     (123)    11940 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/knn.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/knn.h
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/knn.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     9169 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/matrix.cu
+-rw-r--r--   0 runner    (1001) docker     (123)     3117 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/matrix.h
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/matrix.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     8998 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/matrix_factorization_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/random.cu
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/random.h
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/random.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/utils.h
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/gpu/utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2272 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/lmf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/nearest_neighbours.h
+-rw-r--r--   0 runner    (1001) docker     (123)     8725 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/nearest_neighbours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8218 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/recommender_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5425 2023-06-13 05:01:40.000000 implicit-0.7.0/implicit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 05:14:54.733289 implicit-0.7.0/implicit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6020 2023-06-13 05:14:54.000000 implicit-0.7.0/implicit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-06-13 05:14:54.000000 implicit-0.7.0/implicit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 05:14:54.000000 implicit-0.7.0/implicit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-06-13 05:14:54.000000 implicit-0.7.0/implicit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 05:14:54.000000 implicit-0.7.0/implicit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-06-13 05:01:40.000000 implicit-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-06-13 05:01:40.000000 implicit-0.7.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-06-13 05:01:40.000000 implicit-0.7.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-13 05:14:54.737289 implicit-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-06-13 05:01:40.000000 implicit-0.7.0/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-13 05:01:40.000000 implicit-0.7.0/tox.ini
```

### Comparing `implicit-0.6.2/LICENSE` & `implicit-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/PKG-INFO` & `implicit-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: implicit
-Version: 0.6.2
+Version: 0.7.0
 Summary: Collaborative Filtering for Implicit Feedback Datasets
 Home-page: http://github.com/benfred/implicit/
 Author: Ben Frederickson
 Author-email: ben@benfrederickson.com
 License: MIT
 Keywords: Matrix Factorization,Implicit Alternating Least Squares,Collaborative Filtering,Recommender Systems
 Classifier: Development Status :: 4 - Beta
```

### Comparing `implicit-0.6.2/README.md` & `implicit-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/CMakeLists.txt` & `implicit-0.7.0/implicit/CMakeLists.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+if(NOT CYTHON_FLAGS)
+    set(CYTHON_FLAGS
+        "--directive always_allow_keywords=True,binding=True,embedsignature=True,language_level=3"
+    )
+endif()
+
 add_cython_target(_nearest_neighbours CXX)
 add_library(_nearest_neighbours MODULE ${_nearest_neighbours})
 python_extension_module(_nearest_neighbours)
 install(TARGETS _nearest_neighbours LIBRARY DESTINATION implicit)
 
 add_cython_target(evaluation CXX)
 add_library(evaluation MODULE ${evaluation})
```

### Comparing `implicit-0.6.2/implicit/_nearest_neighbours.pyx` & `implicit-0.7.0/implicit/_nearest_neighbours.pyx`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/als.py` & `implicit-0.7.0/implicit/als.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
     factors : int, optional
         The number of latent factors to compute
     regularization : float, optional
         The regularization factor to use
     alpha : float, optional
         The weight to give to positive examples.
     dtype : data-type, optional
-        Specifies whether to generate 64 bit or 32 bit floating point factors
+        Specifies whether to generate 64 bit or 32 bit or 16 bit floating point factors
     use_native : bool, optional
         Use native extensions to speed up model fitting
     use_cg : bool, optional
         Use a faster Conjugate Gradient solver to calculate factors
     use_gpu : bool, optional
         Fit on the GPU if available, default is to run on GPU only if available
     iterations : int, optional
@@ -57,14 +57,15 @@
         Default is None.
     """
     if use_gpu:
         return implicit.gpu.als.AlternatingLeastSquares(
             factors,
             regularization,
             alpha,
+            dtype=dtype,
             iterations=iterations,
             calculate_training_loss=calculate_training_loss,
             random_state=random_state,
         )
     return implicit.cpu.als.AlternatingLeastSquares(
         factors,
         regularization,
```

### Comparing `implicit-0.6.2/implicit/ann/annoy.py` & `implicit-0.7.0/implicit/ann/annoy.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/ann/faiss.py` & `implicit-0.7.0/implicit/ann/faiss.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/ann/nmslib.py` & `implicit-0.7.0/implicit/ann/nmslib.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/approximate_als.py` & `implicit-0.7.0/implicit/approximate_als.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/bpr.py` & `implicit-0.7.0/implicit/bpr.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/cpu/CMakeLists.txt` & `implicit-0.7.0/implicit/cpu/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/cpu/_als.pyx` & `implicit-0.7.0/implicit/cpu/_als.pyx`

 * *Files 4% similar despite different names*

```diff
@@ -51,15 +51,24 @@
                       int * ldb, int * info) nogil:
     if floating is double:
         cython_lapack.dgesv(n, nrhs, a, lda, piv, b, ldb, info)
     else:
         cython_lapack.sgesv(n, nrhs, a, lda, piv, b, ldb, info)
 
 
+def _check_als_dtype(X):
+    _ALLOWED_DTYPES = (np.float32, np.float64)
+    if X.dtype not in _ALLOWED_DTYPES:
+        raise ValueError(f"Invalid dtype {X.dtype} for cpu ALS model. "
+                         f"Allowed dtypes are: {_ALLOWED_DTYPES}")
+
+
 def least_squares(Cui, X, Y, regularization, num_threads=0):
+    _check_als_dtype(X)
+    _check_als_dtype(Y)
     YtY = np.dot(np.transpose(Y), Y)
     _least_squares(YtY, Cui.indptr, Cui.indices, Cui.data.astype('float32'),
                    X, Y, regularization, num_threads)
 
 
 @cython.boundscheck(False)
 def _least_squares(YtY, integral[:] indptr, integral[:] indices, float[:] data,
@@ -128,14 +137,16 @@
 
         finally:
             free(A)
             free(b)
 
 
 def least_squares_cg(Cui, X, Y, regularization, num_threads=0, cg_steps=3):
+    _check_als_dtype(X)
+    _check_als_dtype(Y)
     return _least_squares_cg(Cui.indptr, Cui.indices, Cui.data.astype('float32'),
                              X, Y, regularization, num_threads, cg_steps)
 
 
 @cython.cdivision(True)
 @cython.boundscheck(False)
 def _least_squares_cg(integral[:] indptr, integral[:] indices, float[:] data,
@@ -232,14 +243,15 @@
         finally:
             free(p)
             free(r)
             free(Ap)
 
 
 def calculate_loss(Cui, X, Y, regularization, num_threads=0):
+    """ Calculates the loss for an ALS model """
     return _calculate_loss(Cui, Cui.indptr, Cui.indices, Cui.data.astype('float32'),
                            X, Y, regularization, num_threads)
 
 
 @cython.cdivision(True)
 @cython.boundscheck(False)
 def _calculate_loss(Cui, integral[:] indptr, integral[:] indices, float[:] data,
@@ -280,15 +292,15 @@
 
                     total_confidence += confidence
                     loss += confidence
 
                 loss += dot(&N, r, &one, &X[u, 0], &one)
                 user_norm += dot(&N, &X[u, 0], &one, &X[u, 0], &one)
 
-            for u in prange(users, schedule='dynamic', chunksize=8):
+            for i in prange(items, schedule='dynamic', chunksize=8):
                 item_norm += dot(&N, &Y[i, 0], &one, &Y[i, 0], &one)
 
         finally:
             free(r)
 
     loss += regularization * (item_norm + user_norm)
     return loss / (total_confidence + Cui.shape[0] * Cui.shape[1] - Cui.nnz)
```

### Comparing `implicit-0.6.2/implicit/cpu/als.py` & `implicit-0.7.0/implicit/cpu/als.py`

 * *Files 5% similar despite different names*

```diff
@@ -429,40 +429,41 @@
         """Converts this model to an equivalent version running on the gpu"""
         import implicit.gpu.als
 
         ret = implicit.gpu.als.AlternatingLeastSquares(
             factors=self.factors,
             regularization=self.regularization,
             alpha=self.alpha,
+            dtype=self.dtype,
             iterations=self.iterations,
             calculate_training_loss=self.calculate_training_loss,
             random_state=self.random_state,
         )
         if self.user_factors is not None:
             ret.user_factors = implicit.gpu.Matrix(self.user_factors)
         if self.item_factors is not None:
             ret.item_factors = implicit.gpu.Matrix(self.item_factors)
         return ret
 
     def save(self, fileobj_or_path):
-        args = dict(
-            user_factors=self.user_factors,
-            item_factors=self.item_factors,
-            regularization=self.regularization,
-            factors=self.factors,
-            num_threads=self.num_threads,
-            iterations=self.iterations,
-            use_native=self.use_native,
-            use_cg=self.use_cg,
-            cg_steps=self.cg_steps,
-            calculate_training_loss=self.calculate_training_loss,
-            dtype=self.dtype.name,
-            random_state=self.random_state,
-            alpha=self.alpha,
-        )
+        args = {
+            "user_factors": self.user_factors,
+            "item_factors": self.item_factors,
+            "regularization": self.regularization,
+            "factors": self.factors,
+            "num_threads": self.num_threads,
+            "iterations": self.iterations,
+            "use_native": self.use_native,
+            "use_cg": self.use_cg,
+            "cg_steps": self.cg_steps,
+            "calculate_training_loss": self.calculate_training_loss,
+            "dtype": self.dtype.name,
+            "random_state": self.random_state,
+            "alpha": self.alpha,
+        }
         # filter out 'None' valued args, since we can't go np.load on
         # them without using pickle
         args = {k: v for k, v in args.items() if v is not None}
         np.savez(fileobj_or_path, **args)
 
 
 def least_squares(Cui, X, Y, regularization, num_threads=0):
@@ -551,7 +552,10 @@
             rsnew = r.dot(r)
             if rsnew < 1e-20:
                 break
             p = r + (rsnew / rsold) * p
             rsold = rsnew
 
         X[u] = x
+
+
+calculate_loss = _als.calculate_loss
```

### Comparing `implicit-0.6.2/implicit/cpu/bpr.h` & `implicit-0.7.0/implicit/cpu/bpr.h`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/cpu/bpr.pyx` & `implicit-0.7.0/implicit/cpu/bpr.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# cython: language_level=3
-# cython: embedsignature=True
-
 import cython
 
 from cython cimport floating, integral
 
 import logging
 import multiprocessing
 import time
```

### Comparing `implicit-0.6.2/implicit/cpu/lmf.pyx` & `implicit-0.7.0/implicit/cpu/lmf.pyx`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-# cython: language_level=3
-# cython: embedsignature=True
-
 import cython
 
 from cython cimport floating, integral
 
 import logging
 import multiprocessing
 import time
```

### Comparing `implicit-0.6.2/implicit/cpu/matrix_factorization_base.py` & `implicit-0.7.0/implicit/cpu/matrix_factorization_base.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/cpu/select.h` & `implicit-0.7.0/implicit/cpu/select.h`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/cpu/topk.pyx` & `implicit-0.7.0/implicit/cpu/topk.pyx`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/datasets/_download.py` & `implicit-0.7.0/implicit/datasets/_download.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/datasets/lastfm.py` & `implicit-0.7.0/implicit/datasets/lastfm.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/datasets/million_song_dataset.py` & `implicit-0.7.0/implicit/datasets/million_song_dataset.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/datasets/movielens.py` & `implicit-0.7.0/implicit/datasets/movielens.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/datasets/reddit.py` & `implicit-0.7.0/implicit/datasets/reddit.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/datasets/sketchfab.py` & `implicit-0.7.0/implicit/datasets/sketchfab.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/evaluation.pyx` & `implicit-0.7.0/implicit/evaluation.pyx`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,8 @@
 # distutils: language = c++
-# cython: language_level=3
-# cython: embedsignature=True
 
 import cython
 import numpy as np
 from scipy.sparse import coo_matrix, csr_matrix
 from tqdm.auto import tqdm
 
 from libc.math cimport fmin
```

### Comparing `implicit-0.6.2/implicit/gpu/_cuda.pyx` & `implicit-0.7.0/implicit/gpu/_cuda.pyx`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 """ Various thin cython wrappers on top of CUDA functions """
 
 import cython
 import numpy as np
 from cython.operator import dereference
 
 from cython cimport view
+from libc.stdint cimport uint16_t
 from libcpp cimport bool
 from libcpp.utility cimport move, pair
 
 from .als cimport LeastSquaresSolver as CppLeastSquaresSolver
 from .bpr cimport bpr_update as cpp_bpr_update
 from .knn cimport KnnQuery as CppKnnQuery
 from .matrix cimport COOMatrix as CppCOOMatrix
 from .matrix cimport CSRMatrix as CppCSRMatrix
 from .matrix cimport Matrix as CppMatrix
 from .matrix cimport Vector as CppVector
-from .matrix cimport calculate_norms as cpp_calculate_norms
 from .random cimport RandomState as CppRandomState
 from .utils cimport get_device_count as cpp_get_device_count
 
 
 cdef class RandomState(object):
     cdef CppRandomState * c_random
 
@@ -45,72 +45,80 @@
 
     def __cinit__(self, size_t max_temp_memory=0):
         self.c_knn = new CppKnnQuery(max_temp_memory)
 
     def __dealloc__(self):
         del self.c_knn
 
+    @cython.boundscheck(False)
     def topk(self, Matrix items, Matrix m, int k, Matrix item_norms=None,
              COOMatrix query_filter=None, IntVector item_filter=None):
         cdef CppMatrix * queries = m.c_matrix
         cdef CppCOOMatrix * c_query_filter = NULL
         cdef CppVector[int] * c_item_filter = NULL
         cdef size_t rows = queries.rows
-        cdef int[:, :] x
-        cdef float[:, :] y
+        cdef int[:, :] indices_view
+        cdef float[:, :] distances_view
 
-        cdef float * c_item_norms = NULL
+        cdef CppMatrix * c_item_norms = NULL
         if item_norms is not None:
-            c_item_norms = item_norms.c_matrix.data
+            c_item_norms = item_norms.c_matrix
 
         if query_filter is not None:
             c_query_filter = query_filter.c_matrix
 
         if item_filter is not None:
             c_item_filter = item_filter.c_vector
 
-
         indices = np.zeros((rows, k), dtype="int32")
         distances = np.zeros((rows, k), dtype="float32")
-        x = indices
-        y = distances
+        indices_view = indices
+        distances_view = distances
 
         with nogil:
             self.c_knn.topk(dereference(items.c_matrix), dereference(queries), k,
-                            &x[0, 0], &y[0, 0], c_item_norms, c_query_filter, c_item_filter)
+                            &indices_view[0, 0], &distances_view[0, 0], c_item_norms, c_query_filter, c_item_filter)
 
         return indices, distances
 
-
 cdef class Matrix(object):
     cdef CppMatrix * c_matrix
 
     def __cinit__(self, X):
         if X is None:
             self.c_matrix = NULL
             return
 
-        cdef float[:, :] c_X
+        cdef float[:, :] temp_float
+        cdef uint16_t[:, :] temp_half
         cdef long data
 
         # see if the input support CAI (cupy/pytorch/cudf etc)
         cai = getattr(X, "__cuda_array_interface__", None)
         if cai:
             shape = cai["shape"]
             data = cai["data"][0]
-            self.c_matrix = new CppMatrix(shape[0], shape[1], <float*>data, False)
+            itemsize = int(cai["typestr"][2])
+            self.c_matrix = new CppMatrix(shape[0], shape[1], <void*>data, False, itemsize)
         else:
             # otherwise assume we're a buffer on host
-            c_X = X
-            self.c_matrix = new CppMatrix(X.shape[0], X.shape[1], &c_X[0, 0], True)
+
+            if X.dtype.char == "f":
+                temp_float = X
+                self.c_matrix = new CppMatrix(X.shape[0], X.shape[1], &temp_float[0, 0], True, 4)
+            elif X.dtype.char == "e":
+                temp_half = X.view(np.uint16)
+                self.c_matrix = new CppMatrix(X.shape[0], X.shape[1], &temp_half[0, 0], True, 2)
+            else:
+                raise ValueError(f"unhandled dtype for GPU Matrix {X.dtype}")
 
     @classmethod
     def zeros(cls, rows, cols):
         ret = Matrix(None)
-        ret.c_matrix = new CppMatrix(rows, cols, NULL, True)
+        ret.c_matrix = new CppMatrix(rows, cols, NULL, True, 4)
         return ret
 
     @property
     def shape(self):
         return self.c_matrix.rows, self.c_matrix.cols
 
     def __getitem__(self, idx):
@@ -150,34 +158,58 @@
         return ret
 
     def assign_rows(self, rowids, Matrix other):
         cdef IntVector rows
         rows = IntVector(np.array(rowids).astype("int32"))
         self.c_matrix.assign_rows(dereference(rows.c_vector), dereference(other.c_matrix))
 
+    def astype(self, dtype):
+        dtype = np.dtype(dtype)
+        _ALLOWED_DTYPES = (np.float16, np.float32)
+        if dtype not in _ALLOWED_DTYPES:
+            raise ValueError(f"Invalid dtype '{dtype}' for GPU model. "
+                             f"Allowed dtypes are: {_ALLOWED_DTYPES}")
+
+        cdef int itemsize = dtype.itemsize
+        ret = Matrix(None)
+        ret.c_matrix = new CppMatrix(self.c_matrix.astype(itemsize))
+        return ret
+
     def resize(self, size_t rows, size_t cols):
         self.c_matrix.resize(rows, cols)
 
     def to_numpy(self):
-        ret = np.zeros((self.c_matrix.rows, self.c_matrix.cols), dtype="float32")
-        cdef float[:, :] temp = ret
-        self.c_matrix.to_host(&temp[0, 0])
-        return ret
+        cdef float[:, :] temp_float
+        cdef uint16_t[:, :] temp_half
+
+        if self.c_matrix.itemsize == 4:
+            ret = np.zeros((self.c_matrix.rows, self.c_matrix.cols), dtype="float32")
+            temp_float = ret
+            self.c_matrix.to_host(&temp_float[0, 0])
+            return ret
+        elif self.c_matrix.itemsize == 2:
+            ret = np.zeros((self.c_matrix.rows, self.c_matrix.cols), dtype="float16")
+            temp_half = ret.view(np.uint16)
+            self.c_matrix.to_host(&temp_half[0, 0])
+            return ret
+        else:
+            raise ValueError(f"Invalid itemsize {self.c_matrix.itemsize}")
 
     def __repr__(self):
         return f"Matrix({str(self.to_numpy())})"
 
     def __str__(self):
         return str(self.to_numpy())
 
     def __dealloc__(self):
         if self.c_matrix is not NULL:
             del self.c_matrix
 
 
+
 cdef class IntVector(object):
     cdef CppVector[int] * c_vector
 
     def __cinit__(self, int[:] data):
         self.c_vector = new CppVector[int](len(data), &data[0])
 
     def __dealloc__(self):
@@ -237,15 +269,15 @@
 
     def __dealloc__(self):
         del self.c_solver
 
 
 def calculate_norms(Matrix items):
     ret = Matrix(None)
-    ret.c_matrix = new CppMatrix(cpp_calculate_norms(dereference(items.c_matrix)))
+    ret.c_matrix = new CppMatrix(items.c_matrix.calculate_norms())
     return ret
 
 
 def get_device_count():
     return cpp_get_device_count()
```

### Comparing `implicit-0.6.2/implicit/gpu/als.cu` & `implicit-0.7.0/implicit/gpu/als.cu`

 * *Files 7% similar despite different names*

```diff
@@ -1,109 +1,116 @@
 #include <math.h>
+#include <stdexcept>
 #include <stdio.h>
 
 #include <cublas_v2.h>
 #include <cuda_runtime.h>
 
 #include "implicit/gpu/als.h"
+#include "implicit/gpu/convert.cuh"
 #include "implicit/gpu/dot.cuh"
 #include "implicit/gpu/utils.h"
 
 namespace implicit {
 namespace gpu {
 
 using std::invalid_argument;
 
-__global__ void least_squares_cg_kernel(int factors, size_t user_count,
-                                        size_t item_count, float *X,
-                                        const float *Y, const float *YtY,
-                                        const int *indptr, const int *indices,
-                                        const float *data, int cg_steps) {
+namespace {
+// We apparently need different stopping criteria for half precision
+constexpr float SMALL = 1e-20;
+} // namespace
+
+template <typename T>
+__global__ void
+least_squares_cg_kernel(int factors, size_t user_count, size_t item_count, T *X,
+                        const T *Y, const float *YtY, const int *indptr,
+                        const int *indices, const float *data, int cg_steps) {
   extern __shared__ float shared_memory[];
   float *P = &shared_memory[0];
   float *shared = &shared_memory[factors];
 
   float Ap = 0;
   float p = 0;
   float r = 0;
 
   // Stride over users in the grid:
   // https://devblogs.nvidia.com/parallelforall/cuda-pro-tip-write-flexible-kernels-grid-stride-loops/
   for (int u = blockIdx.x; u < user_count; u += gridDim.x) {
-    float *x = &X[u * factors];
-    float x_value = x[threadIdx.x];
+    T *x = &X[u * factors];
+
+    float x_value = convert<T, float>(x[threadIdx.x]);
 
     // handle 0-sized rows
     if (indptr[u] == indptr[u + 1]) {
       x[threadIdx.x] = 0;
       continue;
     }
 
     // calculate residual r = YtCuPu - YtCuY Xu
     r = 0;
     for (int i = 0; i < factors; ++i) {
-      r -= x[i] * YtY[i * factors + threadIdx.x];
+      r -= convert<T, float>(x[i]) * YtY[i * factors + threadIdx.x];
     }
     for (int index = indptr[u]; index < indptr[u + 1]; ++index) {
-      float Yi = Y[indices[index] * factors + threadIdx.x];
+      float Yi = convert<T, float>(Y[indices[index] * factors + threadIdx.x]);
       float confidence = data[index];
 
       if (confidence > 0) {
         r += (confidence - (confidence - 1) * dot(Yi, x_value, shared)) * Yi;
       } else {
         confidence *= -1;
         r += (-(confidence - 1) * dot(Yi, x_value, shared)) * Yi;
       }
     }
     P[threadIdx.x] = p = r;
     __syncthreads();
 
     float rsold = dot(r, r, shared);
-    if (rsold < 1e-20)
+    if (rsold < SMALL)
       continue;
 
     for (int it = 0; it < cg_steps; ++it) {
       // calculate Ap = YtCuYp - without actually calculating YtCuY
       Ap = 0;
       for (int i = 0; i < factors; ++i) {
         Ap += P[i] * YtY[i * factors + threadIdx.x];
       }
       for (int index = indptr[u]; index < indptr[u + 1]; ++index) {
-        float Yi = Y[indices[index] * factors + threadIdx.x];
+        float Yi = convert<T, float>(Y[indices[index] * factors + threadIdx.x]);
         float confidence = data[index];
         if (confidence < 0)
           confidence *= -1;
 
         Ap += (confidence - 1) * dot(Yi, p, shared) * Yi;
       }
 
       // standard CG update
       float alpha = rsold / dot(p, Ap, shared);
       x_value += alpha * p;
       r -= alpha * Ap;
       __syncthreads();
       float rsnew = dot(r, r, shared);
-      if (rsnew < 1e-20)
+      if (rsnew < SMALL)
         break;
 
       P[threadIdx.x] = p = r + (rsnew / rsold) * p;
       rsold = rsnew;
       __syncthreads();
     }
 
     // this shouldn't happen - but if we hit a NaN in the above code then
     // complain and don't let it perpetuate
     if (isnan(rsold)) {
       if (threadIdx.x == 0) {
         printf("Warning NaN Detected in row %i of %lu\n", u, user_count);
       }
-      x[threadIdx.x] = 0;
-    } else {
-      x[threadIdx.x] = x_value;
+      x_value = 0;
     }
+    x[threadIdx.x] = convert<float, T>(x_value);
   }
 }
 
 __global__ void l2_regularize_kernel(size_t factors, float regularization,
                                      float *YtY) {
   YtY[threadIdx.x * factors + threadIdx.x] += regularization;
 }
@@ -118,21 +125,33 @@
     throw invalid_argument("YtY and Y should have the same number of columns");
 
   // calculate YtY: note this expects col-major (and we have row-major
   // basically) so that we're inverting the CUBLAS_OP_T/CU_BLAS_OP_N ordering to
   // overcome this (like calculate YYt instead of YtY)
   size_t factors = Y.cols, item_count = Y.rows;
   float alpha = 1.0, beta = 0.;
-  CHECK_CUBLAS(cublasSgemm(blas_handle, CUBLAS_OP_N, CUBLAS_OP_T, factors,
-                           factors, item_count, &alpha, Y.data, factors, Y.data,
-                           factors, &beta, YtY->data, factors));
+  if (Y.itemsize == 4) {
+    CHECK_CUBLAS(cublasSgemm(blas_handle, CUBLAS_OP_N, CUBLAS_OP_T, factors,
+                             factors, item_count, &alpha, Y, factors, Y,
+                             factors, &beta, *YtY, factors));
+
+  } else if (Y.itemsize == 2) {
+    // our factors are float16, but we accumulate into a float32 YtY
+    CHECK_CUBLAS(cublasSgemmEx(blas_handle, CUBLAS_OP_N, CUBLAS_OP_T, factors,
+                               factors, item_count, &alpha, Y.data, CUDA_R_16F,
+                               factors, Y.data, CUDA_R_16F, factors, &beta,
+                               YtY->data, CUDA_R_32F, factors));
+  } else {
+    throw std::invalid_argument("invalid dtype for calculate_yty");
+  }
+
   CHECK_CUDA(cudaDeviceSynchronize());
 
   // regularize the matrix
-  l2_regularize_kernel<<<1, factors>>>(factors, regularization, YtY->data);
+  l2_regularize_kernel<<<1, factors>>>(factors, regularization, *YtY);
   CHECK_CUDA(cudaDeviceSynchronize());
 }
 
 void LeastSquaresSolver::least_squares(const CSRMatrix &Cui, Matrix *X,
                                        const Matrix &YtY, const Matrix &Y,
                                        int cg_steps) const {
   int item_count = Y.rows, user_count = X->rows, factors = X->cols;
@@ -140,59 +159,73 @@
     throw invalid_argument("X and Y should have the same number of columns");
   if (X->cols != YtY.cols)
     throw invalid_argument("Columns of X don't match number of factors");
   if (Cui.rows > X->rows)
     throw invalid_argument("Dimensionality mismatch between rows of Cui and X");
   if (Cui.cols > Y.rows)
     throw invalid_argument("Dimensionality mismatch between cols of Cui and Y");
+  if (Y.itemsize != X->itemsize)
+    throw invalid_argument("X and Y should have the same dtype");
 
   // TODO: multi-gpu support
   int devId;
   CHECK_CUDA(cudaGetDevice(&devId));
 
   int multiprocessor_count;
   CHECK_CUDA(cudaDeviceGetAttribute(&multiprocessor_count,
                                     cudaDevAttrMultiProcessorCount, devId));
 
   int block_count = 256 * multiprocessor_count;
   int thread_count = factors;
-  int shared_memory_size = sizeof(float) * (2 * factors);
+  int shared_memory_size = sizeof(Y.itemsize) * (2 * factors);
 
-  least_squares_cg_kernel<<<block_count, thread_count, shared_memory_size>>>(
-      factors, user_count, item_count, X->data, Y.data, YtY.data, Cui.indptr,
-      Cui.indices, Cui.data, cg_steps);
+  if (Y.itemsize == 4) {
+    least_squares_cg_kernel<float>
+        <<<block_count, thread_count, shared_memory_size>>>(
+            factors, user_count, item_count, *X, Y, YtY, Cui.indptr,
+            Cui.indices, Cui.data, cg_steps);
+  } else if (Y.itemsize == 2) {
+    least_squares_cg_kernel<half>
+        <<<block_count, thread_count, shared_memory_size>>>(
+            factors, user_count, item_count, *X, Y, YtY, Cui.indptr,
+            Cui.indices, Cui.data, cg_steps);
+  } else {
+    throw invalid_argument(
+        "invalid dtype in LeastSquaresSolver::least_squares");
+  }
 
   CHECK_CUDA(cudaDeviceSynchronize());
 }
 
+template <typename T>
 __global__ void calculate_loss_kernel(int factors, size_t user_count,
-                                      size_t item_count, const float *X,
-                                      const float *Y, const float *YtY,
-                                      const int *indptr, const int *indices,
-                                      const float *data, float regularization,
-                                      float *output) {
+                                      size_t item_count, const T *X, const T *Y,
+                                      const float *YtY, const int *indptr,
+                                      const int *indices, const float *data,
+                                      float regularization, float *output) {
   // https://devblogs.nvidia.com/parallelforall/using-shared-memory-cuda-cc/
   extern __shared__ float shared_memory[];
   float *shared = &shared_memory[0];
 
   float loss = 0, user_norm = 0, item_norm = 0, total_confidence = 0, r = 0;
 
   for (int u = blockIdx.x; u < user_count; u += gridDim.x) {
-    const float *x = &X[u * factors];
-    float x_value = x[threadIdx.x];
+    const T *x = &X[u * factors];
+    float x_value = convert<T, float>(x[threadIdx.x]);
 
     // calculates r = (YtCuY.dot(Xu) - 2 * YtCuPu).dot(Xu), without calculating
     // YtCuY
     r = 0;
     for (int i = 0; i < factors; ++i) {
-      r += x[i] * YtY[i * factors + threadIdx.x];
+      // TODO: is this correct?
+      r += convert<T, float>(x[i]) * YtY[i * factors + threadIdx.x];
     }
 
     for (int index = indptr[u]; index < indptr[u + 1]; ++index) {
-      float Yi = Y[indices[index] * factors + threadIdx.x];
+      float Yi = convert<T, float>(Y[indices[index] * factors + threadIdx.x]);
       float confidence = data[index];
       if (confidence > 0) {
         r +=
             ((confidence - 1) * dot(Yi, x_value, shared) - 2 * confidence) * Yi;
       } else {
         confidence *= -1;
         r += ((confidence - 1) * dot(Yi, x_value, shared)) * Yi;
@@ -202,15 +235,15 @@
     }
     loss += dot(x_value, r, shared);
 
     user_norm += dot(x_value, x_value, shared);
   }
 
   for (int i = blockIdx.x; i < item_count; i += gridDim.x) {
-    float y = Y[i * factors + threadIdx.x];
+    float y = convert<T, float>(Y[i * factors + threadIdx.x]);
     item_norm += dot(y, y, shared);
   }
 
   loss += regularization * (item_norm + user_norm);
   if (threadIdx.x == 0) {
     atomicAdd(output, loss);
     atomicAdd(output + 1, total_confidence);
@@ -219,30 +252,37 @@
 
 float LeastSquaresSolver::calculate_loss(const CSRMatrix &Cui, const Matrix &X,
                                          const Matrix &Y,
                                          float regularization) {
   size_t item_count = Y.rows, factors = Y.cols, user_count = X.rows;
 
   Matrix YtY(factors, factors, NULL);
-  calculate_yty(Y, &YtY, regularization);
+  calculate_yty(Y, &YtY, 0.0);
 
-  float alpha = 1.0, beta = 0.;
-  CHECK_CUBLAS(cublasSgemm(blas_handle, CUBLAS_OP_N, CUBLAS_OP_T, factors,
-                           factors, item_count, &alpha, Y.data, factors, Y.data,
-                           factors, &beta, YtY.data, factors));
-  CHECK_CUDA(cudaDeviceSynchronize());
   float temp[2] = {0, 0};
   Matrix output(2, 1, temp);
-  calculate_loss_kernel<<<1024, factors, sizeof(float) * factors>>>(
-      factors, user_count, item_count, X.data, Y.data, YtY.data, Cui.indptr,
-      Cui.indices, Cui.data, regularization, output.data);
+
+  if (Y.itemsize == 4) {
+    calculate_loss_kernel<float><<<1024, factors, X.itemsize * factors>>>(
+        factors, user_count, item_count, X, Y, YtY, Cui.indptr, Cui.indices,
+        Cui.data, regularization, output);
+  } else if (Y.itemsize == 2) {
+    calculate_loss_kernel<half><<<1024, factors, X.itemsize * factors>>>(
+        factors, user_count, item_count, X, Y, YtY, Cui.indptr, Cui.indices,
+        Cui.data, regularization, output);
+  } else {
+    throw invalid_argument(
+        "invalid dtype in LeastSquaresSolver::calculate_loss");
+  }
   CHECK_CUDA(cudaDeviceSynchronize());
   output.to_host(temp);
 
-  return temp[0] / (temp[1] + Cui.rows * Cui.cols - Cui.nonzeros);
+  size_t rows = Cui.rows, cols = Cui.cols;
+  return temp[0] / (temp[1] + rows * cols - Cui.nonzeros);
 }
 
 LeastSquaresSolver::~LeastSquaresSolver() {
   CHECK_CUBLAS(cublasDestroy(blas_handle));
 }
+
 } // namespace gpu
 } // namespace implicit
```

### Comparing `implicit-0.6.2/implicit/gpu/als.h` & `implicit-0.7.0/implicit/gpu/als.h`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/gpu/als.pxd` & `implicit-0.7.0/implicit/gpu/als.pxd`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/gpu/als.py` & `implicit-0.7.0/implicit/gpu/als.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,16 @@
     ----------
     factors : int, optional
         The number of latent factors to compute
     regularization : float, optional
         The regularization factor to use
     alpha : float, optional
         The weight to give to positive examples.
+    dtype : data-type, optional
+        Specifies whether to use 16 bit or 32 bit floating point factors
     iterations : int, optional
         The number of ALS iterations to use when fitting data
     calculate_training_loss : bool, optional
         Whether to log out the training loss at each iteration
     random_state : int, RandomState or None, optional
         The random state for seeding the initial item and user factors.
         Default is None.
@@ -44,27 +46,29 @@
     """
 
     def __init__(
         self,
         factors=64,
         regularization=0.01,
         alpha=1.0,
+        dtype=np.float32,
         iterations=15,
         calculate_training_loss=False,
         random_state=None,
     ):
         if not implicit.gpu.HAS_CUDA:
             raise ValueError("No CUDA extension has been built, can't train on GPU.")
 
         super().__init__()
 
         # parameters on how to factorize
         self.factors = factors
         self.regularization = regularization
         self.alpha = alpha
+        self.dtype = dtype
 
         # options on how to fit the model
         self.iterations = iterations
         self.calculate_training_loss = calculate_training_loss
         self.fit_callback = None
         self.random_state = random_state
         self.cg_steps = 3
@@ -119,18 +123,21 @@
         s = time.time()
 
         # Initialize the variables randomly if they haven't already been set
         if self.user_factors is None:
             self.user_factors = random_state.uniform(
                 users, self.factors, low=-0.5 / self.factors, high=0.5 / self.factors
             )
+            self.user_factors = self.user_factors.astype(self.dtype)
+
         if self.item_factors is None:
             self.item_factors = random_state.uniform(
                 items, self.factors, low=-0.5 / self.factors, high=0.5 / self.factors
             )
+            self.item_factors = self.item_factors.astype(self.dtype)
 
         log.debug("Initialized factors in %s", time.time() - s)
 
         # invalidate cached norms and squared factors
         self._item_norms = self._user_norms = None
         self._item_norms_host = self._user_norms_host = None
         self._YtY = self._XtX = None
@@ -172,28 +179,28 @@
             log.info("Final training loss %.4f", loss)
 
     def recalculate_user(self, userid, user_items):
         if self.alpha != 1.0:
             user_items = self.alpha * user_items
 
         users = 1 if np.isscalar(userid) else len(userid)
-        user_factors = implicit.gpu.Matrix.zeros(users, self.factors)
+        user_factors = implicit.gpu.Matrix.zeros(users, self.factors).astype(self.dtype)
         Cui = implicit.gpu.CSRMatrix(user_items)
 
         self.solver.least_squares(
             Cui, user_factors, self.YtY, self.item_factors, cg_steps=self.factors
         )
         return user_factors[0] if np.isscalar(userid) else user_factors
 
     def recalculate_item(self, itemid, item_users):
         if self.alpha != 1.0:
             item_users = self.alpha * item_users
 
         items = 1 if np.isscalar(itemid) else len(itemid)
-        item_factors = implicit.gpu.Matrix.zeros(items, self.factors)
+        item_factors = implicit.gpu.Matrix.zeros(items, self.factors).astype(self.dtype)
         Ciu = implicit.gpu.CSRMatrix(item_users)
         self.solver.least_squares(
             Ciu, item_factors, self.XtX, self.user_factors, cg_steps=self.factors
         )
         return item_factors[0] if np.isscalar(itemid) else item_factors
 
     def partial_fit_users(self, userids, user_items):
@@ -281,14 +288,15 @@
 
     def to_cpu(self) -> implicit.cpu.als.AlternatingLeastSquares:
         """Converts this model to an equivalent version running on the CPU"""
         ret = implicit.cpu.als.AlternatingLeastSquares(
             factors=self.factors,
             regularization=self.regularization,
             alpha=self.alpha,
+            dtype=self.dtype,
             iterations=self.iterations,
             calculate_training_loss=self.calculate_training_loss,
             random_state=self.random_state,
         )
         ret.user_factors = self.user_factors.to_numpy() if self.user_factors is not None else None
         ret.item_factors = self.item_factors.to_numpy() if self.item_factors is not None else None
         return ret
@@ -302,7 +310,21 @@
 
     def __setstate__(self, state):
         super().__setstate__(state)
         if self._XtX is not None:
             self._XtX = implicit.gpu.Matrix(self._XtX)
         if self._YtY is not None:
             self._YtY = implicit.gpu.Matrix(self._YtY)
+
+
+def calculate_loss(Cui, X, Y, regularization, solver=None):
+    """Calculates the loss for an ALS model"""
+    if not isinstance(Cui, implicit.gpu.CSRMatrix):
+        Cui = implicit.gpu.CSRMatrix(Cui)
+    if not isinstance(X, implicit.gpu.Matrix):
+        X = implicit.gpu.Matrix(X)
+    if not isinstance(Y, implicit.gpu.Matrix):
+        Y = implicit.gpu.Matrix(Y)
+    if solver is None:
+        solver = implicit.gpu.LeastSquaresSolver()
+
+    return solver.calculate_loss(Cui, X, Y, regularization)
```

### Comparing `implicit-0.6.2/implicit/gpu/bpr.cu` & `implicit-0.7.0/implicit/gpu/bpr.cu`

 * *Files 2% similar despite different names*

```diff
@@ -112,19 +112,18 @@
                                     cudaDevAttrMultiProcessorCount, devId));
 
   int factors = X->cols;
   int block_count = 256 * multiprocessor_count;
   int thread_count = factors;
   int shared_memory_size = sizeof(float) * (factors);
 
-  // TODO: get rows passed in here
   bpr_update_kernel<<<block_count, thread_count, shared_memory_size>>>(
       nonzeros, random_likes, random_dislikes, itemids.data, userids.data,
-      indptr.data, factors, X->data, Y->data, learning_rate, reg,
-      verify_negative_samples, stats);
+      indptr.data, factors, *X, *Y, learning_rate, reg, verify_negative_samples,
+      stats);
 
   CHECK_CUDA(cudaDeviceSynchronize());
 
   // we're returning the number of correctly ranked items, get that value from
   // the device
   int output[2];
   CHECK_CUDA(
```

### Comparing `implicit-0.6.2/implicit/gpu/bpr.h` & `implicit-0.7.0/implicit/gpu/bpr.h`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/gpu/bpr.pxd` & `implicit-0.7.0/implicit/gpu/bpr.pxd`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/gpu/bpr.py` & `implicit-0.7.0/implicit/gpu/bpr.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/gpu/dot.cuh` & `implicit-0.7.0/implicit/gpu/dot.cuh`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/gpu/matrix.pxd` & `implicit-0.7.0/implicit/gpu/matrix.pxd`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,27 @@
     cdef cppclass Vector[T]:
         Vector(size_t size, T * data) except +
         void to_host(T * output) except +
         T * data
         size_t size
 
     cdef cppclass Matrix:
-        Matrix(size_t rows, size_t cols, float * data, bool host) except +
+        Matrix(size_t rows, size_t cols, void * data, bool host, size_t itemsize) except +
         Matrix(const Matrix & other, size_t rowid) except +
         Matrix(const Matrix & other, size_t start, size_t end) except +
         Matrix(const Matrix & other, const Vector[int] & rowids) except +
         Matrix(Matrix && other) except +
-        void to_host(float * output) except +
+        void to_host(void * output) except +
         void resize(size_t rows, size_t cols) except +
         void assign_rows(const Vector[int] & rowids, const Matrix & other) except +
+        Matrix calculate_norms() except +
+        Matrix astype(size_t itemsize) except +
         size_t rows, cols
-        float * data
-
-    Matrix calculate_norms(const Matrix & items) except +
+        void * data
+        size_t itemsize
 
     cdef cppclass KnnQuery:
         KnnQuery()
         void query(const Matrix & items, const Matrix & queries, int k,
                    int * indices, float * distances) except +
         void argpartition(const Matrix & items, int k, int * indices, float * distances) except +
         void argsort(Matrix * items, int * indices) except +
```

### Comparing `implicit-0.6.2/implicit/gpu/matrix_factorization_base.py` & `implicit-0.7.0/implicit/gpu/matrix_factorization_base.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/gpu/random.cu` & `implicit-0.7.0/implicit/gpu/random.cu`

 * *Files 16% similar despite different names*

```diff
@@ -14,28 +14,29 @@
 RandomState::RandomState(long seed) {
   CHECK_CURAND(curandCreateGenerator(&rng, CURAND_RNG_PSEUDO_DEFAULT));
   CHECK_CURAND(curandSetPseudoRandomGeneratorSeed(rng, seed));
 }
 
 Matrix RandomState::uniform(size_t rows, size_t cols, float low, float high) {
   Matrix ret(rows, cols, NULL);
-  CHECK_CURAND(curandGenerateUniform(rng, ret.data, rows * cols));
+  CHECK_CURAND(curandGenerateUniform(rng, ret, rows * cols));
 
   if ((low != 0.0) || (high != 1.0)) {
-    auto start = thrust::device_pointer_cast(ret.data);
+    float *data = ret;
+    auto start = thrust::device_pointer_cast(data);
     thrust::transform(start, start + rows * cols, start,
                       thrust::placeholders::_1 =
                           thrust::placeholders::_1 * (high - low) + low);
   }
 
   return ret;
 }
 
 Matrix RandomState::randn(size_t rows, size_t cols, float mean, float stddev) {
   Matrix ret(rows, cols, NULL);
-  CHECK_CURAND(curandGenerateNormal(rng, ret.data, rows * cols, mean, stddev));
+  CHECK_CURAND(curandGenerateNormal(rng, ret, rows * cols, mean, stddev));
   return ret;
 }
 
 RandomState::~RandomState() { curandDestroyGenerator(rng); }
 } // namespace gpu
 } // namespace implicit
```

### Comparing `implicit-0.6.2/implicit/gpu/random.h` & `implicit-0.7.0/implicit/gpu/random.h`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/gpu/utils.h` & `implicit-0.7.0/implicit/gpu/utils.h`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/lmf.py` & `implicit-0.7.0/implicit/lmf.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/nearest_neighbours.h` & `implicit-0.7.0/implicit/nearest_neighbours.h`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/nearest_neighbours.py` & `implicit-0.7.0/implicit/nearest_neighbours.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,18 +154,20 @@
         self.__dict__.update(state)
         if self.similarity is not None:
             self.scorer = NearestNeighboursScorer(self.similarity)
         else:
             self.scorer = None
 
     def save(self, fileobj_or_path):
-        args = dict(K=self.K)
+        args = {"K": self.K}
         m = self.similarity
         if m is not None:
-            args.update(dict(shape=m.shape, data=m.data, indptr=m.indptr, indices=m.indices))
+            args.update(
+                {"shape": m.shape, "data": m.data, "indptr": m.indptr, "indices": m.indices}
+            )
         np.savez(fileobj_or_path, **args)
 
     @classmethod
     def load(cls, fileobj_or_path):
         # numpy.save automatically appends a npz suffic, numpy.load doesn't apparently
         if isinstance(fileobj_or_path, str) and not fileobj_or_path.endswith(".npz"):
             fileobj_or_path = fileobj_or_path + ".npz"
```

### Comparing `implicit-0.6.2/implicit/recommender_base.py` & `implicit-0.7.0/implicit/recommender_base.py`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/implicit/utils.py` & `implicit-0.7.0/implicit/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,17 +86,17 @@
     user_items = kwargs.pop("user_items") if "user_items" in kwargs else None
     item_users = kwargs.pop("item_users") if "item_users" in kwargs else None
 
     # pylint: disable=unsubscriptable-object
     for i, idx in enumerate(ids):
         current_kwargs = kwargs
         if user_items is not None:
-            current_kwargs = dict(user_items=user_items[i], **kwargs)
+            current_kwargs = {"user_items": user_items[i], **kwargs}
         elif item_users is not None:
-            current_kwargs = dict(item_users=item_users[i], **kwargs)
+            current_kwargs = {"item_users": item_users[i], **kwargs}
 
         batch_ids, batch_scores = func(idx, *args, N=N, **current_kwargs)
 
         # pad out to N items if we're returned fewer
         missing_items = N - len(batch_ids)
         if missing_items > 0:
             batch_ids = np.append(batch_ids, np.full(missing_items, -1))
```

### Comparing `implicit-0.6.2/implicit.egg-info/PKG-INFO` & `implicit-0.7.0/implicit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: implicit
-Version: 0.6.2
+Version: 0.7.0
 Summary: Collaborative Filtering for Implicit Feedback Datasets
 Home-page: http://github.com/benfred/implicit/
 Author: Ben Frederickson
 Author-email: ben@benfrederickson.com
 License: MIT
 Keywords: Matrix Factorization,Implicit Alternating Least Squares,Collaborative Filtering,Recommender Systems
 Classifier: Development Status :: 4 - Beta
```

### Comparing `implicit-0.6.2/implicit.egg-info/SOURCES.txt` & `implicit-0.7.0/implicit.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,14 @@
 implicit/cpu/bpr.pyx
 implicit/cpu/lmf.pyx
 implicit/cpu/matrix_factorization_base.py
 implicit/cpu/select.h
 implicit/cpu/topk.pyx
 implicit/datasets/__init__.py
 implicit/datasets/_download.py
-implicit/datasets/github.py
 implicit/datasets/lastfm.py
 implicit/datasets/million_song_dataset.py
 implicit/datasets/movielens.py
 implicit/datasets/reddit.py
 implicit/datasets/sketchfab.py
 implicit/gpu/CMakeLists.txt
 implicit/gpu/__init__.py
@@ -54,14 +53,15 @@
 implicit/gpu/als.h
 implicit/gpu/als.pxd
 implicit/gpu/als.py
 implicit/gpu/bpr.cu
 implicit/gpu/bpr.h
 implicit/gpu/bpr.pxd
 implicit/gpu/bpr.py
+implicit/gpu/convert.cuh
 implicit/gpu/dot.cuh
 implicit/gpu/knn.cu
 implicit/gpu/knn.h
 implicit/gpu/knn.pxd
 implicit/gpu/matrix.cu
 implicit/gpu/matrix.h
 implicit/gpu/matrix.pxd
```

### Comparing `implicit-0.6.2/pyproject.toml` & `implicit-0.7.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `implicit-0.6.2/setup.cfg` & `implicit-0.7.0/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [bumpversion]
-current_version = 0.6.2
+current_version = 0.7.0
 commit = True
 tag = True
 
 [metadata]
-description-file = README.md
+description_file = README.md
 
 [flake8]
 max-line-length = 100
 exclude = build,.eggs,.tox
 ignore = E203,W503
 
 [isort]
```

### Comparing `implicit-0.6.2/setup.py` & `implicit-0.7.0/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,19 +3,14 @@
 
 from packaging.version import Version
 from setuptools import find_packages
 from skbuild import setup
 from skbuild.cmaker import get_cmake_version
 from skbuild.exceptions import SKBuildError
 
-try:
-    import numpy.distutils  # noqa
-except ImportError:
-    pass
-
 # Add CMake as a build requirement if cmake is not installed or is too low a version
 setup_requires = []
 try:
     if Version(get_cmake_version()) < Version("3.17"):
         setup_requires.append("cmake>=3.17")
 except SKBuildError:
     setup_requires.append("cmake>=3.17")
@@ -32,15 +27,15 @@
     # we seem to be picking up a bunch of unrelated files from thrust/spdlog/rmm
     # filter the cmake manifest down to things from this package only
     return [f for f in cmake_manifest if "implicit" in f]
 
 
 setup(
     name="implicit",
-    version="0.6.2",
+    version="0.7.0",
     description="Collaborative Filtering for Implicit Feedback Datasets",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     url="http://github.com/benfred/implicit/",
     author="Ben Frederickson",
     author_email="ben@benfrederickson.com",
     license="MIT",
```

