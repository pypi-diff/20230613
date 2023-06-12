# Comparing `tmp/mypackagez123g-1.0.4.tar.gz` & `tmp/mypackagez123g-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypackagez123g-1.0.4.tar", max compression
+gzip compressed data, was "mypackagez123g-1.1.0.tar", max compression
```

## Comparing `mypackagez123g-1.0.4.tar` & `mypackagez123g-1.1.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0        0 2023-06-12 21:56:23.093136 mypackagez123g-1.0.4/README.md
--rw-r--r--   0        0        0        0 2023-06-12 21:56:23.093136 mypackagez123g-1.0.4/mypackagez123g/__init__.py
--rw-r--r--   0        0        0      267 2023-06-12 21:56:41.950437 mypackagez123g-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 mypackagez123g-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-06-12 22:02:35.712435 mypackagez123g-1.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 22:02:35.712435 mypackagez123g-1.1.0/mypackagez123g/__init__.py
+-rw-r--r--   0        0        0      267 2023-06-12 22:02:50.280640 mypackagez123g-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0      436 1970-01-01 00:00:00.000000 mypackagez123g-1.1.0/PKG-INFO
```

