# Comparing `tmp/pnsgraph-0.0.1.tar.gz` & `tmp/pnsgraph-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pnsgraph-0.0.1.tar", last modified: Tue May 30 03:40:04 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `pnsgraph-0.0.1.tar` & `pnsgraph-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxrwxrwx   0        0        0        0 2023-05-30 03:40:04.668000 pnsgraph-0.0.1/
--rw-rw-rw-   0        0        0      101 2023-05-30 03:40:04.652000 pnsgraph-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-30 03:40:04.634000 pnsgraph-0.0.1/pnsgraph.egg-info/
--rw-rw-rw-   0        0        0      101 2023-05-30 03:40:04.000000 pnsgraph-0.0.1/pnsgraph.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      136 2023-05-30 03:40:04.000000 pnsgraph-0.0.1/pnsgraph.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 03:40:04.000000 pnsgraph-0.0.1/pnsgraph.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        1 2023-05-30 03:40:04.000000 pnsgraph-0.0.1/pnsgraph.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-30 03:40:04.664000 pnsgraph-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      222 2023-05-30 00:37:01.000000 pnsgraph-0.0.1/setup.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/setup.py
+-rw-r--r--   0        0        0     2486 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/src/pnsgraph/MSG.py
+-rw-r--r--   0        0        0     8979 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/src/pnsgraph/SSG.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/src/pnsgraph/__init__.py
+-rw-r--r--   0        0        0     6325 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/src/pnsgraph/pgraph.py
+-rw-r--r--   0        0        0     2108 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/src/pnsgraph/testfile.py
+-rw-r--r--   0        0        0     1084 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/LICENSE
+-rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/README.md
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     2052 2020-02-02 00:00:00.000000 pnsgraph-0.0.3/PKG-INFO
```

