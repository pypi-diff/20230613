# Comparing `tmp/envppp-0.1.0.tar.gz` & `tmp/envppp-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "envppp-0.1.0.tar", last modified: Mon Jun 12 23:49:11 2023, max compression
+gzip compressed data, was "envppp-0.1.1.tar", last modified: Tue Jun 13 00:04:22 2023, max compression
```

## Comparing `envppp-0.1.0.tar` & `envppp-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     1261 2023-06-12 23:06:59.317213 envppp-0.1.0/README.md
--rw-r--r--   0        0        0      380 2023-06-12 23:49:11.572628 envppp-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      283 2023-06-02 22:03:53.328736 envppp-0.1.0/src/main.py
--rw-r--r--   0        0        0     1449 1970-01-01 00:00:00.000000 envppp-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1261 2023-06-12 23:06:59.317213 envppp-0.1.1/README.md
+-rw-r--r--   0        0        0      397 2023-06-13 00:04:22.797659 envppp-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      283 2023-06-02 22:03:53.328736 envppp-0.1.1/src/main.py
+-rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 envppp-0.1.1/PKG-INFO
```

### Comparing `envppp-0.1.0/README.md` & `envppp-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `envppp-0.1.0/PKG-INFO` & `envppp-0.1.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 Metadata-Version: 2.1
 Name: envppp
-Version: 0.1.0
+Version: 0.1.1
 Summary: Uma cli para criar projetos em python, javascript e C++
 Author: Every
+Project-URL: Repository, https://github.com/Every2/envpp
 Requires-Python: >=3.11
 Requires-Dist: typer[all]>=0.9.0
 Description-Content-Type: text/markdown
 
 # envpp
 
 Cli para criar projetos em Python, Javascript e C++ que pode ser criada em qualquer ambiente.
```

