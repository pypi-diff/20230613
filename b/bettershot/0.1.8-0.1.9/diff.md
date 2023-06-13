# Comparing `tmp/bettershot-0.1.8.tar.gz` & `tmp/bettershot-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bettershot-0.1.8.tar", max compression
+gzip compressed data, was "bettershot-0.1.9.tar", max compression
```

## Comparing `bettershot-0.1.8.tar` & `bettershot-0.1.9.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-08 01:12:47.902493 bettershot-0.1.8/README.md
--rw-r--r--   0        0        0     1801 2023-06-13 04:39:44.931456 bettershot-0.1.8/bettershot/__init__.py
--rw-r--r--   0        0        0      309 2023-06-13 04:39:48.409452 bettershot-0.1.8/pyproject.toml
--rw-r--r--   0        0        0      444 1970-01-01 00:00:00.000000 bettershot-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     2681 2023-06-13 12:48:27.546485 bettershot-0.1.9/README.md
+-rw-r--r--   0        0        0     1457 2023-06-13 12:48:35.978291 bettershot-0.1.9/bettershot/__init__.py
+-rw-r--r--   0        0        0      309 2023-06-13 12:48:39.936611 bettershot-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     3125 1970-01-01 00:00:00.000000 bettershot-0.1.9/PKG-INFO
```

