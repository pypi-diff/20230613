# Comparing `tmp/aifunc-0.1.0.tar.gz` & `tmp/aifunc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.1.0.tar", max compression
+gzip compressed data, was "aifunc-0.1.1.tar", max compression
```

## Comparing `aifunc-0.1.0.tar` & `aifunc-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,3 @@
--rw-r--r--   0        0        0      683 2023-06-11 22:36:58.363066 aifunc-0.1.0/aifunc/__init__.py
--rw-r--r--   0        0        0      311 2023-06-11 22:41:12.007411 aifunc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      577 2023-06-11 22:41:34.952314 aifunc-0.1.0/setup.py
--rw-r--r--   0        0        0      277 2023-06-11 22:41:34.952581 aifunc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     2250 2023-06-13 06:43:14.680151 aifunc-0.1.1/aifunc/__init__.py
+-rw-r--r--   0        0        0      311 2023-06-13 06:43:23.605045 aifunc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      328 1970-01-01 00:00:00.000000 aifunc-0.1.1/PKG-INFO
```

