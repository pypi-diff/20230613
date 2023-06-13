# Comparing `tmp/torchbones-1.2.4.tar.gz` & `tmp/torchbones-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchbones-1.2.4.tar", last modified: Mon Jun 12 20:59:20 2023, max compression
+gzip compressed data, was "torchbones-1.2.5.tar", last modified: Tue Jun 13 21:35:48 2023, max compression
```

## Comparing `torchbones-1.2.4.tar` & `torchbones-1.2.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-12 20:59:20.274487 torchbones-1.2.4/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-12 20:59:20.274487 torchbones-1.2.4/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-12 20:59:20.274487 torchbones-1.2.4/setup.cfg
--rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-12 20:59:16.000000 torchbones-1.2.4/setup.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-12 20:59:20.264487 torchbones-1.2.4/torchbones/
--rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.2.4/torchbones/__init__.py
--rw-r--r--   0 oross314  (1000) oross314  (1000)    17205 2023-06-12 20:59:10.000000 torchbones-1.2.4/torchbones/main.py
-drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-12 20:59:20.274487 torchbones-1.2.4/torchbones.egg-info/
--rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-12 20:59:20.000000 torchbones-1.2.4/torchbones.egg-info/PKG-INFO
--rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-12 20:59:20.000000 torchbones-1.2.4/torchbones.egg-info/SOURCES.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-12 20:59:20.000000 torchbones-1.2.4/torchbones.egg-info/dependency_links.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-12 20:59:20.000000 torchbones-1.2.4/torchbones.egg-info/requires.txt
--rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-12 20:59:20.000000 torchbones-1.2.4/torchbones.egg-info/top_level.txt
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-13 21:35:48.244228 torchbones-1.2.5/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-13 21:35:48.244228 torchbones-1.2.5/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       38 2023-06-13 21:35:48.244228 torchbones-1.2.5/setup.cfg
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      465 2023-06-13 21:35:21.000000 torchbones-1.2.5/setup.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-13 21:35:48.244228 torchbones-1.2.5/torchbones/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       28 2023-05-26 19:25:50.000000 torchbones-1.2.5/torchbones/__init__.py
+-rw-r--r--   0 oross314  (1000) oross314  (1000)    20117 2023-06-13 21:35:23.000000 torchbones-1.2.5/torchbones/main.py
+drwxr-xr-x   0 oross314  (1000) oross314  (1000)        0 2023-06-13 21:35:48.244228 torchbones-1.2.5/torchbones.egg-info/
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      202 2023-06-13 21:35:48.000000 torchbones-1.2.5/torchbones.egg-info/PKG-INFO
+-rw-r--r--   0 oross314  (1000) oross314  (1000)      219 2023-06-13 21:35:48.000000 torchbones-1.2.5/torchbones.egg-info/SOURCES.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)        1 2023-06-13 21:35:48.000000 torchbones-1.2.5/torchbones.egg-info/dependency_links.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       43 2023-06-13 21:35:48.000000 torchbones-1.2.5/torchbones.egg-info/requires.txt
+-rw-r--r--   0 oross314  (1000) oross314  (1000)       11 2023-06-13 21:35:48.000000 torchbones-1.2.5/torchbones.egg-info/top_level.txt
```

