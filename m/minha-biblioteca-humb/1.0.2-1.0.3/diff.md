# Comparing `tmp/minha-biblioteca-humb-1.0.2.tar.gz` & `tmp/minha-biblioteca-humb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minha-biblioteca-humb-1.0.2.tar", last modified: Mon Jun 12 23:50:59 2023, max compression
+gzip compressed data, was "minha-biblioteca-humb-1.0.3.tar", last modified: Tue Jun 13 00:11:00 2023, max compression
```

## Comparing `minha-biblioteca-humb-1.0.2.tar` & `minha-biblioteca-humb-1.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 23:50:59.287076 minha-biblioteca-humb-1.0.2/
--rw-rw-rw-   0        0        0      167 2023-06-12 23:50:59.286074 minha-biblioteca-humb-1.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 23:50:59.267378 minha-biblioteca-humb-1.0.2/minha_biblioteca/
--rw-rw-rw-   0        0        0        0 2023-06-12 23:46:12.000000 minha-biblioteca-humb-1.0.2/minha_biblioteca/__init__.py
--rw-rw-rw-   0        0        0       55 2023-06-12 23:50:41.000000 minha-biblioteca-humb-1.0.2/minha_biblioteca/modulo1.py
-drwxrwxrwx   0        0        0        0 2023-06-12 23:50:59.284082 minha-biblioteca-humb-1.0.2/minha_biblioteca_humb.egg-info/
--rw-rw-rw-   0        0        0      167 2023-06-12 23:50:58.000000 minha-biblioteca-humb-1.0.2/minha_biblioteca_humb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-12 23:50:59.000000 minha-biblioteca-humb-1.0.2/minha_biblioteca_humb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 23:50:58.000000 minha-biblioteca-humb-1.0.2/minha_biblioteca_humb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-12 23:50:59.000000 minha-biblioteca-humb-1.0.2/minha_biblioteca_humb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 23:50:59.287076 minha-biblioteca-humb-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      218 2023-06-12 23:50:49.000000 minha-biblioteca-humb-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 00:11:00.479719 minha-biblioteca-humb-1.0.3/
+-rw-rw-rw-   0        0        0      167 2023-06-13 00:11:00.478771 minha-biblioteca-humb-1.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 00:11:00.456112 minha-biblioteca-humb-1.0.3/minha_biblioteca/
+-rw-rw-rw-   0        0        0        0 2023-06-12 23:46:12.000000 minha-biblioteca-humb-1.0.3/minha_biblioteca/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-06-13 00:03:30.000000 minha-biblioteca-humb-1.0.3/minha_biblioteca/modulo1.py
+drwxrwxrwx   0        0        0        0 2023-06-13 00:11:00.477191 minha-biblioteca-humb-1.0.3/minha_biblioteca_humb.egg-info/
+-rw-rw-rw-   0        0        0      167 2023-06-13 00:10:59.000000 minha-biblioteca-humb-1.0.3/minha_biblioteca_humb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-13 00:11:00.000000 minha-biblioteca-humb-1.0.3/minha_biblioteca_humb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 00:10:59.000000 minha-biblioteca-humb-1.0.3/minha_biblioteca_humb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-13 00:11:00.000000 minha-biblioteca-humb-1.0.3/minha_biblioteca_humb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 00:11:00.480716 minha-biblioteca-humb-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      218 2023-06-13 00:10:37.000000 minha-biblioteca-humb-1.0.3/setup.py
```

