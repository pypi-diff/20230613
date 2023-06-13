# Comparing `tmp/pear_ebi-0.1.64.tar.gz` & `tmp/pear_ebi-0.1.65.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pear_ebi-0.1.64.tar", last modified: Fri Jun  9 12:57:19 2023, max compression
+gzip compressed data, was "pear_ebi-0.1.65.tar", last modified: Tue Jun 13 14:02:20 2023, max compression
```

## Comparing `pear_ebi-0.1.64.tar` & `pear_ebi-0.1.65.tar`

### file list

```diff
@@ -1,117 +1,117 @@
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-09 12:57:19.161308 pear_ebi-0.1.64/
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1120 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/LICENSE.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)       93 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/MANIFEST.in
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5693 2023-06-09 12:57:19.161308 pear_ebi-0.1.64/PKG-INFO
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5245 2023-05-09 17:21:50.000000 pear_ebi-0.1.64/README.md
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-09 12:57:19.128808 pear_ebi-0.1.64/pear_ebi/
--rw-r--r--   0 andrear   (1000) andrear   (1000)      349 2023-06-09 12:56:16.000000 pear_ebi-0.1.64/pear_ebi/__init__.py
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)    18447 2023-04-05 18:11:56.000000 pear_ebi-0.1.64/pear_ebi/__main__.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-09 12:57:19.128808 pear_ebi-0.1.64/pear_ebi/calculate_distances/
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-09 12:57:19.150475 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/
--rw-r--r--   0 andrear   (1000) andrear   (1000)       36 2023-02-14 10:37:26.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/AUTHORS
--rw-r--r--   0 andrear   (1000) andrear   (1000)    18337 2023-02-20 10:02:47.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/COPYING
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:26.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/ChangeLog
--rw-r--r--   0 andrear   (1000) andrear   (1000)     9732 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/INSTALL
--rw-r--r--   0 andrear   (1000) andrear   (1000)    20283 2023-02-20 10:02:47.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/Makefile
--rw-r--r--   0 andrear   (1000) andrear   (1000)      490 2023-02-14 10:37:26.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/Makefile.am
--rw-r--r--   0 andrear   (1000) andrear   (1000)    20957 2023-02-20 10:02:47.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/Makefile.in
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:26.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/NEWS
--rw-r--r--   0 andrear   (1000) andrear   (1000)      157 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/README
--rw-r--r--   0 andrear   (1000) andrear   (1000)    50999 2023-02-14 10:37:26.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/Random.cpp
--rw-r--r--   0 andrear   (1000) andrear   (1000)  3230664 2023-02-14 10:37:26.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/Random.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)    33526 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/aclocal.m4
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2366 2023-02-14 10:37:26.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/config.h
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2148 2023-02-14 10:37:26.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/config.h.in
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2271 2023-02-14 10:37:26.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/config.hh
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2073 2023-02-14 10:37:26.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/config.hh.in
--rw-r--r--   0 andrear   (1000) andrear   (1000)    16107 2023-02-20 10:02:47.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/config.log
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)    31318 2023-02-20 16:30:29.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/config.status
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)   188210 2023-02-20 16:30:29.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/configure
--rw-r--r--   0 andrear   (1000) andrear   (1000)      485 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/configure.ac
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)   186547 2023-02-20 16:30:29.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/configure.lineno
--rw-r--r--   0 andrear   (1000) andrear   (1000)    16466 2023-02-14 10:37:26.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/depcomp
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2243 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hash.cc
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1915 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hash.hh
--rw-r--r--   0 andrear   (1000) andrear   (1000)   595768 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hash.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2968 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hashfunc.cc
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2166 2023-02-20 10:02:48.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hashfunc.hh
--rw-r--r--   0 andrear   (1000) andrear   (1000)   331744 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hashfunc.o
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)  4547960 2023-02-20 16:30:29.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hashrf
--rw-r--r--   0 andrear   (1000) andrear   (1000)    28716 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hashrf.cc
--rw-r--r--   0 andrear   (1000) andrear   (1000)  6651416 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hashrf.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)     9556 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/install-sh
--rw-r--r--   0 andrear   (1000) andrear   (1000)      795 2023-02-20 10:02:47.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/label-map.cc
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1026 2023-02-20 10:02:47.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/label-map.hh
--rw-r--r--   0 andrear   (1000) andrear   (1000)   540936 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/label-map.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)    11374 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/missing
--rw-r--r--   0 andrear   (1000) andrear   (1000)    12315 2023-02-20 10:02:47.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/newick.c
--rw-r--r--   0 andrear   (1000) andrear   (1000)      723 2023-02-20 10:02:47.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/newick.h
--rw-r--r--   0 andrear   (1000) andrear   (1000)    38568 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/newick.o
--rw-r--r--   0 andrear   (1000) andrear   (1000)       24 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/stamp-h1
--rw-r--r--   0 andrear   (1000) andrear   (1000)      660 2023-02-22 10:35:23.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/RF_pypy.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     4932 2023-06-09 12:54:40.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/hashrf.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)    24634 2023-04-03 16:09:45.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/maple_RF.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-09 12:57:19.161308 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._CMakeFiles
--rw-r--r--   0 andrear   (1000) andrear   (1000)      269 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._CMakeLists.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._COPYING
--rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._COPYING.LESSER
--rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._CPackConfig.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._CPackSourceConfig.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._CTestTestfile.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._Makefile
--rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._README
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._bin
--rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._cmake_install.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._icon.ico
--rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._icon.jpg
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._tqDist
--rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/._trees
--rw-r--r--   0 andrear   (1000) andrear   (1000)    15581 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/CMakeCache.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2436 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/CMakeLists.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)    35820 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/COPYING
--rw-r--r--   0 andrear   (1000) andrear   (1000)     7815 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/COPYING.LESSER
--rw-r--r--   0 andrear   (1000) andrear   (1000)     4094 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/CPackConfig.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)     4880 2023-02-14 10:37:27.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/CPackSourceConfig.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)      275 2023-02-20 10:02:48.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/CTestTestfile.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)    12995 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/Makefile
--rw-r--r--   0 andrear   (1000) andrear   (1000)     3071 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/README
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1828 2023-02-14 10:37:28.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/cmake_install.cmake
--rw-r--r--   0 andrear   (1000) andrear   (1000)    32038 2023-02-14 10:37:28.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/icon.ico
--rw-r--r--   0 andrear   (1000) andrear   (1000)     7953 2023-02-14 10:37:28.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/icon.jpg
--rw-r--r--   0 andrear   (1000) andrear   (1000)      205 2023-02-20 10:02:50.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/install_manifest.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5429 2023-04-03 16:09:45.000000 pear_ebi-0.1.64/pear_ebi/calculate_distances/tqdist.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-09 12:57:19.161308 pear_ebi-0.1.64/pear_ebi/embeddings/
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1790 2023-04-05 18:11:55.000000 pear_ebi-0.1.64/pear_ebi/embeddings/Isomap_e.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1838 2023-04-05 18:11:55.000000 pear_ebi-0.1.64/pear_ebi/embeddings/LLE_e.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1936 2023-04-05 18:11:55.000000 pear_ebi-0.1.64/pear_ebi/embeddings/PCA_e.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.64/pear_ebi/embeddings/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1473 2023-03-22 16:31:08.000000 pear_ebi-0.1.64/pear_ebi/embeddings/emb_quality.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-09 12:57:19.161308 pear_ebi-0.1.64/pear_ebi/embeddings/graph/
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.64/pear_ebi/embeddings/graph/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)    39664 2023-05-09 14:17:50.000000 pear_ebi-0.1.64/pear_ebi/embeddings/graph/graph.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     2208 2023-04-05 18:11:55.000000 pear_ebi-0.1.64/pear_ebi/embeddings/tSNE_e.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-09 12:57:19.161308 pear_ebi-0.1.64/pear_ebi/interactive_mode/
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.64/pear_ebi/interactive_mode/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5859 2023-02-22 10:35:24.000000 pear_ebi-0.1.64/pear_ebi/interactive_mode/interactive.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-09 12:57:19.161308 pear_ebi-0.1.64/pear_ebi/subsample/
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.64/pear_ebi/subsample/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     3855 2023-02-20 16:46:41.000000 pear_ebi-0.1.64/pear_ebi/subsample/subsample.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5050 2023-02-20 16:46:42.000000 pear_ebi-0.1.64/pear_ebi/subsample/subsample_multiprocess.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     3681 2023-04-19 10:09:29.000000 pear_ebi-0.1.64/pear_ebi/tree_emb_parser.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)    33262 2023-06-09 12:54:41.000000 pear_ebi-0.1.64/pear_ebi/tree_set.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-09 12:57:19.128808 pear_ebi-0.1.64/pear_ebi.egg-info/
--rw-r--r--   0 andrear   (1000) andrear   (1000)     5693 2023-06-09 12:57:19.000000 pear_ebi-0.1.64/pear_ebi.egg-info/PKG-INFO
--rw-r--r--   0 andrear   (1000) andrear   (1000)     4314 2023-06-09 12:57:19.000000 pear_ebi-0.1.64/pear_ebi.egg-info/SOURCES.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)        1 2023-06-09 12:57:19.000000 pear_ebi-0.1.64/pear_ebi.egg-info/dependency_links.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)       52 2023-06-09 12:57:19.000000 pear_ebi-0.1.64/pear_ebi.egg-info/entry_points.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-20 16:30:29.000000 pear_ebi-0.1.64/pear_ebi.egg-info/not-zip-safe
--rw-r--r--   0 andrear   (1000) andrear   (1000)       94 2023-06-09 12:57:19.000000 pear_ebi-0.1.64/pear_ebi.egg-info/requires.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)       14 2023-06-09 12:57:19.000000 pear_ebi-0.1.64/pear_ebi.egg-info/top_level.txt
--rw-r--r--   0 andrear   (1000) andrear   (1000)      228 2023-02-20 16:30:29.000000 pear_ebi-0.1.64/pyproject.toml
--rw-r--r--   0 andrear   (1000) andrear   (1000)      107 2023-06-09 12:57:19.161308 pear_ebi-0.1.64/setup.cfg
--rw-r--r--   0 andrear   (1000) andrear   (1000)     1382 2023-06-09 12:57:15.000000 pear_ebi-0.1.64/setup.py
-drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-09 12:57:19.161308 pear_ebi-0.1.64/test/
--rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-05-10 08:43:26.000000 pear_ebi-0.1.64/test/__init__.py
--rw-r--r--   0 andrear   (1000) andrear   (1000)     3105 2023-06-09 12:54:40.000000 pear_ebi-0.1.64/test/test.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-13 14:02:20.502599 pear_ebi-0.1.65/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1120 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/LICENSE.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       93 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/MANIFEST.in
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5693 2023-06-13 14:02:20.502599 pear_ebi-0.1.65/PKG-INFO
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5245 2023-05-09 17:21:50.000000 pear_ebi-0.1.65/README.md
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-13 14:02:20.432599 pear_ebi-0.1.65/pear_ebi/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      349 2023-06-13 14:02:16.000000 pear_ebi-0.1.65/pear_ebi/__init__.py
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)    18447 2023-04-05 18:11:56.000000 pear_ebi-0.1.65/pear_ebi/__main__.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-13 14:02:20.432599 pear_ebi-0.1.65/pear_ebi/calculate_distances/
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-13 14:02:20.492599 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       36 2023-02-14 10:37:26.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/AUTHORS
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    18337 2023-02-20 10:02:47.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/COPYING
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:26.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/ChangeLog
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     9732 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/INSTALL
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    20283 2023-02-20 10:02:47.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/Makefile
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      490 2023-02-14 10:37:26.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/Makefile.am
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    20957 2023-02-20 10:02:47.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/Makefile.in
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:26.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/NEWS
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      157 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/README
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    50999 2023-02-14 10:37:26.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/Random.cpp
+-rw-r--r--   0 andrear   (1000) andrear   (1000)  3230664 2023-02-14 10:37:26.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/Random.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    33526 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/aclocal.m4
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2366 2023-02-14 10:37:26.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/config.h
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2148 2023-02-14 10:37:26.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/config.h.in
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2271 2023-02-14 10:37:26.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/config.hh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2073 2023-02-14 10:37:26.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/config.hh.in
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    16107 2023-02-20 10:02:47.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/config.log
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)    31318 2023-02-20 16:30:29.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/config.status
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)   188210 2023-02-20 16:30:29.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/configure
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      485 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/configure.ac
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)   186547 2023-02-20 16:30:29.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/configure.lineno
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    16466 2023-02-14 10:37:26.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/depcomp
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2243 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hash.cc
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1915 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hash.hh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)   595768 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hash.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2968 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hashfunc.cc
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2166 2023-02-20 10:02:48.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hashfunc.hh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)   331744 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hashfunc.o
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)  4547960 2023-02-20 16:30:29.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hashrf
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    28716 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hashrf.cc
+-rw-r--r--   0 andrear   (1000) andrear   (1000)  6651416 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hashrf.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     9556 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/install-sh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      795 2023-02-20 10:02:47.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/label-map.cc
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1026 2023-02-20 10:02:47.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/label-map.hh
+-rw-r--r--   0 andrear   (1000) andrear   (1000)   540936 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/label-map.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    11374 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/missing
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    12315 2023-02-20 10:02:47.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/newick.c
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      723 2023-02-20 10:02:47.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/newick.h
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    38568 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/newick.o
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       24 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/stamp-h1
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      660 2023-02-22 10:35:23.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/RF_pypy.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     4932 2023-06-09 12:54:40.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/hashrf.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    24634 2023-04-03 16:09:45.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/maple_RF.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-13 14:02:20.492599 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._CMakeFiles
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      269 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._CMakeLists.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._COPYING
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._COPYING.LESSER
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._CPackConfig.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._CPackSourceConfig.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._CTestTestfile.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._Makefile
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      268 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._README
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._bin
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      213 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._cmake_install.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._icon.ico
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      212 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._icon.jpg
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._tqDist
+-rwxr-xr-x   0 andrear   (1000) andrear   (1000)      212 2023-02-20 16:30:29.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/._trees
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    15581 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/CMakeCache.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2436 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/CMakeLists.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    35820 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/COPYING
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     7815 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/COPYING.LESSER
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     4094 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/CPackConfig.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     4880 2023-02-14 10:37:27.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/CPackSourceConfig.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      275 2023-02-20 10:02:48.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/CTestTestfile.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    12995 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/Makefile
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     3071 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/README
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1828 2023-02-14 10:37:28.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/cmake_install.cmake
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    32038 2023-02-14 10:37:28.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/icon.ico
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     7953 2023-02-14 10:37:28.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/icon.jpg
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      205 2023-02-20 10:02:50.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/install_manifest.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5429 2023-04-03 16:09:45.000000 pear_ebi-0.1.65/pear_ebi/calculate_distances/tqdist.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-13 14:02:20.492599 pear_ebi-0.1.65/pear_ebi/embeddings/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1790 2023-04-05 18:11:55.000000 pear_ebi-0.1.65/pear_ebi/embeddings/Isomap_e.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1838 2023-04-05 18:11:55.000000 pear_ebi-0.1.65/pear_ebi/embeddings/LLE_e.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1936 2023-04-05 18:11:55.000000 pear_ebi-0.1.65/pear_ebi/embeddings/PCA_e.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.65/pear_ebi/embeddings/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1473 2023-03-22 16:31:08.000000 pear_ebi-0.1.65/pear_ebi/embeddings/emb_quality.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-13 14:02:20.502599 pear_ebi-0.1.65/pear_ebi/embeddings/graph/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.65/pear_ebi/embeddings/graph/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    39664 2023-05-09 14:17:50.000000 pear_ebi-0.1.65/pear_ebi/embeddings/graph/graph.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     2208 2023-04-05 18:11:55.000000 pear_ebi-0.1.65/pear_ebi/embeddings/tSNE_e.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-13 14:02:20.502599 pear_ebi-0.1.65/pear_ebi/interactive_mode/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.65/pear_ebi/interactive_mode/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5871 2023-06-13 13:58:57.000000 pear_ebi-0.1.65/pear_ebi/interactive_mode/interactive.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-13 14:02:20.502599 pear_ebi-0.1.65/pear_ebi/subsample/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-14 10:37:30.000000 pear_ebi-0.1.65/pear_ebi/subsample/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     3855 2023-02-20 16:46:41.000000 pear_ebi-0.1.65/pear_ebi/subsample/subsample.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5050 2023-02-20 16:46:42.000000 pear_ebi-0.1.65/pear_ebi/subsample/subsample_multiprocess.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     3681 2023-04-19 10:09:29.000000 pear_ebi-0.1.65/pear_ebi/tree_emb_parser.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)    33262 2023-06-09 12:54:41.000000 pear_ebi-0.1.65/pear_ebi/tree_set.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-13 14:02:20.432599 pear_ebi-0.1.65/pear_ebi.egg-info/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     5693 2023-06-13 14:02:20.000000 pear_ebi-0.1.65/pear_ebi.egg-info/PKG-INFO
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     4314 2023-06-13 14:02:20.000000 pear_ebi-0.1.65/pear_ebi.egg-info/SOURCES.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        1 2023-06-13 14:02:20.000000 pear_ebi-0.1.65/pear_ebi.egg-info/dependency_links.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       52 2023-06-13 14:02:20.000000 pear_ebi-0.1.65/pear_ebi.egg-info/entry_points.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-02-20 16:30:29.000000 pear_ebi-0.1.65/pear_ebi.egg-info/not-zip-safe
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       94 2023-06-13 14:02:20.000000 pear_ebi-0.1.65/pear_ebi.egg-info/requires.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)       14 2023-06-13 14:02:20.000000 pear_ebi-0.1.65/pear_ebi.egg-info/top_level.txt
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      228 2023-02-20 16:30:29.000000 pear_ebi-0.1.65/pyproject.toml
+-rw-r--r--   0 andrear   (1000) andrear   (1000)      107 2023-06-13 14:02:20.502599 pear_ebi-0.1.65/setup.cfg
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     1382 2023-06-13 14:02:12.000000 pear_ebi-0.1.65/setup.py
+drwxr-xr-x   0 andrear   (1000) andrear   (1000)        0 2023-06-13 14:02:20.502599 pear_ebi-0.1.65/test/
+-rw-r--r--   0 andrear   (1000) andrear   (1000)        0 2023-05-10 08:43:26.000000 pear_ebi-0.1.65/test/__init__.py
+-rw-r--r--   0 andrear   (1000) andrear   (1000)     3105 2023-06-09 12:54:40.000000 pear_ebi-0.1.65/test/test.py
```

### Comparing `pear_ebi-0.1.64/LICENSE.txt` & `pear_ebi-0.1.65/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/PKG-INFO` & `pear_ebi-0.1.65/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pear_ebi
-Version: 0.1.64
+Version: 0.1.65
 Summary: Embeds phylogenetic tree distances and produce representations
 Home-page: https://github.com/AndreaRubbi/TreeEmbedding
 Author: Andrea Rubbi
 Author-email: andrea.rubbi.98@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pear_ebi Version: 0.1.64 Summary: Embeds
+Metadata-Version: 2.1 Name: pear_ebi Version: 0.1.65 Summary: Embeds
 phylogenetic tree distances and produce representations Home-page: https://
 github.com/AndreaRubbi/TreeEmbedding Author: Andrea Rubbi Author-email:
 andrea.rubbi.98@gmail.com License: MIT License Classifier: Development Status
 :: 3 - Alpha Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Description-Content-Type: text/markdown License-File: LICENSE.txt
 ****** Phylogeny Embedding &
```

### Comparing `pear_ebi-0.1.64/README.md` & `pear_ebi-0.1.65/README.md`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/__main__.py` & `pear_ebi-0.1.65/pear_ebi/__main__.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/COPYING` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/COPYING`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/INSTALL` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/INSTALL`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/Makefile` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/Makefile`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/Makefile.in` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/Makefile.in`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/Random.cpp` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/Random.cpp`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/Random.o` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/Random.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/aclocal.m4` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/aclocal.m4`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/config.h` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/config.h`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/config.h.in` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/config.h.in`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/config.hh` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/config.hh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/config.hh.in` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/config.hh.in`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/config.log` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/config.log`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/config.status` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/config.status`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/configure` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/configure`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/configure.lineno` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/configure.lineno`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/depcomp` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/depcomp`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hash.cc` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hash.cc`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hash.hh` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hash.hh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hash.o` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hash.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hashfunc.cc` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hashfunc.cc`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hashfunc.hh` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hashfunc.hh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hashfunc.o` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hashfunc.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hashrf` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hashrf`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hashrf.cc` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hashrf.cc`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/hashrf.o` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/hashrf.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/install-sh` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/install-sh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/label-map.cc` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/label-map.cc`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/label-map.hh` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/label-map.hh`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/label-map.o` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/label-map.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/missing` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/missing`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/newick.c` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/newick.c`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/newick.h` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/newick.h`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/HashRF/newick.o` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/HashRF/newick.o`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/RF_pypy.py` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/RF_pypy.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/hashrf.py` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/hashrf.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/maple_RF.py` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/maple_RF.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/CMakeCache.txt` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/CMakeCache.txt`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/CMakeLists.txt` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/COPYING` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/COPYING`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/COPYING.LESSER` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/COPYING.LESSER`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/CPackConfig.cmake` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/CPackConfig.cmake`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/CPackSourceConfig.cmake` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/CPackSourceConfig.cmake`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/Makefile` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/Makefile`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/README` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/README`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/cmake_install.cmake` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/cmake_install.cmake`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/icon.ico` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/icon.ico`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/tqDist/icon.jpg` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/tqDist/icon.jpg`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/calculate_distances/tqdist.py` & `pear_ebi-0.1.65/pear_ebi/calculate_distances/tqdist.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/embeddings/Isomap_e.py` & `pear_ebi-0.1.65/pear_ebi/embeddings/Isomap_e.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/embeddings/LLE_e.py` & `pear_ebi-0.1.65/pear_ebi/embeddings/LLE_e.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/embeddings/PCA_e.py` & `pear_ebi-0.1.65/pear_ebi/embeddings/PCA_e.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/embeddings/emb_quality.py` & `pear_ebi-0.1.65/pear_ebi/embeddings/emb_quality.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/embeddings/graph/graph.py` & `pear_ebi-0.1.65/pear_ebi/embeddings/graph/graph.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/embeddings/tSNE_e.py` & `pear_ebi-0.1.65/pear_ebi/embeddings/tSNE_e.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/interactive_mode/interactive.py` & `pear_ebi-0.1.65/pear_ebi/interactive_mode/interactive.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 def exit_program():
     print("[orange1]- Leaving PEAR -")
     exit()
 
 
 def calculate_distances(SET):
-    methods = ["hashrf", "hashrf_weighted", "days_RF", "quartet", "triplet"]
+    methods = ["hashrf_RF", "hashrf_wRF", "days_RF", "tqdist_quartet", "tqdist_triplet"]
     while True:
         try:
             method = int(
                 input(
                     "Method (1:hashrf - 2:weighted hashrf - 3:day's rf - 4:quartet - 5:triplet): "
                 )
             )
```

### Comparing `pear_ebi-0.1.64/pear_ebi/subsample/subsample.py` & `pear_ebi-0.1.65/pear_ebi/subsample/subsample.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/subsample/subsample_multiprocess.py` & `pear_ebi-0.1.65/pear_ebi/subsample/subsample_multiprocess.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/tree_emb_parser.py` & `pear_ebi-0.1.65/pear_ebi/tree_emb_parser.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi/tree_set.py` & `pear_ebi-0.1.65/pear_ebi/tree_set.py`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/pear_ebi.egg-info/PKG-INFO` & `pear_ebi-0.1.65/pear_ebi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pear-ebi
-Version: 0.1.64
+Version: 0.1.65
 Summary: Embeds phylogenetic tree distances and produce representations
 Home-page: https://github.com/AndreaRubbi/TreeEmbedding
 Author: Andrea Rubbi
 Author-email: andrea.rubbi.98@gmail.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3.7
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pear-ebi Version: 0.1.64 Summary: Embeds
+Metadata-Version: 2.1 Name: pear-ebi Version: 0.1.65 Summary: Embeds
 phylogenetic tree distances and produce representations Home-page: https://
 github.com/AndreaRubbi/TreeEmbedding Author: Andrea Rubbi Author-email:
 andrea.rubbi.98@gmail.com License: MIT License Classifier: Development Status
 :: 3 - Alpha Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Description-Content-Type: text/markdown License-File: LICENSE.txt
 ****** Phylogeny Embedding &
```

### Comparing `pear_ebi-0.1.64/pear_ebi.egg-info/SOURCES.txt` & `pear_ebi-0.1.65/pear_ebi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pear_ebi-0.1.64/setup.py` & `pear_ebi-0.1.65/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 
 setup(
     name="pear_ebi",
-    version="0.1.64",
+    version="0.1.65",
     license="MIT License",
     description="Embeds phylogenetic tree distances and produce representations",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Andrea Rubbi",
     author_email="andrea.rubbi.98@gmail.com",
     url="https://github.com/AndreaRubbi/TreeEmbedding",
```

### Comparing `pear_ebi-0.1.64/test/test.py` & `pear_ebi-0.1.65/test/test.py`

 * *Files identical despite different names*

