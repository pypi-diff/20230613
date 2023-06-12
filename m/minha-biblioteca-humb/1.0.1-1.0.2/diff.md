# Comparing `tmp/minha-biblioteca-humb-1.0.1.tar.gz` & `tmp/minha-biblioteca-humb-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minha-biblioteca-humb-1.0.1.tar", last modified: Mon Jun 12 23:46:46 2023, max compression
+gzip compressed data, was "minha-biblioteca-humb-1.0.2.tar", last modified: Mon Jun 12 23:50:59 2023, max compression
```

## Comparing `minha-biblioteca-humb-1.0.1.tar` & `minha-biblioteca-humb-1.0.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 23:46:46.234079 minha-biblioteca-humb-1.0.1/
--rw-rw-rw-   0        0        0      167 2023-06-12 23:46:46.232084 minha-biblioteca-humb-1.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 23:46:46.208720 minha-biblioteca-humb-1.0.1/minha_biblioteca/
--rw-rw-rw-   0        0        0        0 2023-06-12 23:46:12.000000 minha-biblioteca-humb-1.0.1/minha_biblioteca/__init__.py
--rw-rw-rw-   0        0        0       47 2023-06-12 21:37:06.000000 minha-biblioteca-humb-1.0.1/minha_biblioteca/modulo1.py
-drwxrwxrwx   0        0        0        0 2023-06-12 23:46:46.230064 minha-biblioteca-humb-1.0.1/minha_biblioteca_humb.egg-info/
--rw-rw-rw-   0        0        0      167 2023-06-12 23:46:45.000000 minha-biblioteca-humb-1.0.1/minha_biblioteca_humb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-12 23:46:46.000000 minha-biblioteca-humb-1.0.1/minha_biblioteca_humb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 23:46:45.000000 minha-biblioteca-humb-1.0.1/minha_biblioteca_humb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-12 23:46:45.000000 minha-biblioteca-humb-1.0.1/minha_biblioteca_humb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 23:46:46.234079 minha-biblioteca-humb-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      218 2023-06-12 23:46:20.000000 minha-biblioteca-humb-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:50:59.287076 minha-biblioteca-humb-1.0.2/
+-rw-rw-rw-   0        0        0      167 2023-06-12 23:50:59.286074 minha-biblioteca-humb-1.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 23:50:59.267378 minha-biblioteca-humb-1.0.2/minha_biblioteca/
+-rw-rw-rw-   0        0        0        0 2023-06-12 23:46:12.000000 minha-biblioteca-humb-1.0.2/minha_biblioteca/__init__.py
+-rw-rw-rw-   0        0        0       55 2023-06-12 23:50:41.000000 minha-biblioteca-humb-1.0.2/minha_biblioteca/modulo1.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:50:59.284082 minha-biblioteca-humb-1.0.2/minha_biblioteca_humb.egg-info/
+-rw-rw-rw-   0        0        0      167 2023-06-12 23:50:58.000000 minha-biblioteca-humb-1.0.2/minha_biblioteca_humb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-12 23:50:59.000000 minha-biblioteca-humb-1.0.2/minha_biblioteca_humb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 23:50:58.000000 minha-biblioteca-humb-1.0.2/minha_biblioteca_humb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-12 23:50:59.000000 minha-biblioteca-humb-1.0.2/minha_biblioteca_humb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 23:50:59.287076 minha-biblioteca-humb-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      218 2023-06-12 23:50:49.000000 minha-biblioteca-humb-1.0.2/setup.py
```

