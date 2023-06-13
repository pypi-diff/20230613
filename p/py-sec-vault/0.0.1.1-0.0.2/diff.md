# Comparing `tmp/py_sec_vault-0.0.1.1.tar.gz` & `tmp/py_sec_vault-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py_sec_vault-0.0.1.1.tar", max compression
+gzip compressed data, was "py_sec_vault-0.0.2.tar", max compression
```

## Comparing `py_sec_vault-0.0.1.1.tar` & `py_sec_vault-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,5 @@
--rw-r--r--   0        0        0     1096 2023-06-09 13:11:12.838127 py_sec_vault-0.0.1.1/LICENSE
--rw-r--r--   0        0        0       65 2023-06-09 13:10:13.618732 py_sec_vault-0.0.1.1/README.md
--rw-r--r--   0        0        0      446 2023-06-13 10:51:59.679966 py_sec_vault-0.0.1.1/pyproject.toml
--rw-r--r--   0        0        0       48 2023-06-12 20:29:45.699053 py_sec_vault-0.0.1.1/src/__init__.py
--rw-r--r--   0        0        0       60 2023-06-13 10:51:46.807554 py_sec_vault-0.0.1.1/src/vault/__init__.py
--rw-r--r--   0        0        0       39 2023-06-13 10:51:26.649903 py_sec_vault-0.0.1.1/src/vault/main.py
--rw-r--r--   0        0        0      512 1970-01-01 00:00:00.000000 py_sec_vault-0.0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1096 2023-06-09 13:11:12.838127 py_sec_vault-0.0.2/LICENSE
+-rw-r--r--   0        0        0       65 2023-06-09 13:10:13.618732 py_sec_vault-0.0.2/README.md
+-rw-r--r--   0        0        0      444 2023-06-12 21:02:47.593958 py_sec_vault-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0       48 2023-06-12 20:29:45.699053 py_sec_vault-0.0.2/src/__init__.py
+-rw-r--r--   0        0        0      510 1970-01-01 00:00:00.000000 py_sec_vault-0.0.2/PKG-INFO
```

### Comparing `py_sec_vault-0.0.1.1/LICENSE` & `py_sec_vault-0.0.2/LICENSE`

 * *Files identical despite different names*

