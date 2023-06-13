# Comparing `tmp/kgclitest-0.2.0.tar.gz` & `tmp/kgclitest-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kgclitest-0.2.0.tar", max compression
+gzip compressed data, was "kgclitest-0.3.0.tar", max compression
```

## Comparing `kgclitest-0.2.0.tar` & `kgclitest-0.3.0.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       17 2023-06-13 16:07:17.983285 kgclitest-0.2.0/README.md
--rw-r--r--   0        0        0      398 2023-06-13 16:08:37.193241 kgclitest-0.2.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-06-13 15:46:34.033982 kgclitest-0.2.0/src/kgclitest/__init__.py
--rw-r--r--   0        0        0      357 2023-06-13 15:58:19.853589 kgclitest-0.2.0/src/kgclitest/greetings.py
--rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 kgclitest-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0       17 2023-06-13 16:07:17.983285 kgclitest-0.3.0/README.md
+-rw-r--r--   0        0        0      398 2023-06-13 16:25:20.442670 kgclitest-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-06-13 15:46:34.033982 kgclitest-0.3.0/src/kgclitest/__init__.py
+-rw-r--r--   0        0        0      357 2023-06-13 16:25:01.752681 kgclitest-0.3.0/src/kgclitest/greetings.py
+-rw-r--r--   0        0        0      397 1970-01-01 00:00:00.000000 kgclitest-0.3.0/PKG-INFO
```

