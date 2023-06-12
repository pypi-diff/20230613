# Comparing `tmp/minha-biblioteca-humb-1.0.0.tar.gz` & `tmp/minha-biblioteca-humb-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "minha-biblioteca-humb-1.0.0.tar", last modified: Mon Jun 12 23:43:32 2023, max compression
+gzip compressed data, was "minha-biblioteca-humb-1.0.1.tar", last modified: Mon Jun 12 23:46:46 2023, max compression
```

## Comparing `minha-biblioteca-humb-1.0.0.tar` & `minha-biblioteca-humb-1.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 23:43:32.843752 minha-biblioteca-humb-1.0.0/
--rw-rw-rw-   0        0        0      167 2023-06-12 23:43:32.841768 minha-biblioteca-humb-1.0.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-06-12 23:43:32.772985 minha-biblioteca-humb-1.0.0/minha_biblioteca/
--rw-rw-rw-   0        0        0      204 2023-06-12 21:10:31.000000 minha-biblioteca-humb-1.0.0/minha_biblioteca/__init__.py
--rw-rw-rw-   0        0        0       47 2023-06-12 21:37:06.000000 minha-biblioteca-humb-1.0.0/minha_biblioteca/modulo1.py
-drwxrwxrwx   0        0        0        0 2023-06-12 23:43:32.837128 minha-biblioteca-humb-1.0.0/minha_biblioteca_humb.egg-info/
--rw-rw-rw-   0        0        0      167 2023-06-12 23:43:32.000000 minha-biblioteca-humb-1.0.0/minha_biblioteca_humb.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-06-12 23:43:32.000000 minha-biblioteca-humb-1.0.0/minha_biblioteca_humb.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 23:43:32.000000 minha-biblioteca-humb-1.0.0/minha_biblioteca_humb.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-12 23:43:32.000000 minha-biblioteca-humb-1.0.0/minha_biblioteca_humb.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 23:43:32.844757 minha-biblioteca-humb-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      218 2023-06-12 23:43:23.000000 minha-biblioteca-humb-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:46:46.234079 minha-biblioteca-humb-1.0.1/
+-rw-rw-rw-   0        0        0      167 2023-06-12 23:46:46.232084 minha-biblioteca-humb-1.0.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-12 23:46:46.208720 minha-biblioteca-humb-1.0.1/minha_biblioteca/
+-rw-rw-rw-   0        0        0        0 2023-06-12 23:46:12.000000 minha-biblioteca-humb-1.0.1/minha_biblioteca/__init__.py
+-rw-rw-rw-   0        0        0       47 2023-06-12 21:37:06.000000 minha-biblioteca-humb-1.0.1/minha_biblioteca/modulo1.py
+drwxrwxrwx   0        0        0        0 2023-06-12 23:46:46.230064 minha-biblioteca-humb-1.0.1/minha_biblioteca_humb.egg-info/
+-rw-rw-rw-   0        0        0      167 2023-06-12 23:46:45.000000 minha-biblioteca-humb-1.0.1/minha_biblioteca_humb.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-06-12 23:46:46.000000 minha-biblioteca-humb-1.0.1/minha_biblioteca_humb.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 23:46:45.000000 minha-biblioteca-humb-1.0.1/minha_biblioteca_humb.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2023-06-12 23:46:45.000000 minha-biblioteca-humb-1.0.1/minha_biblioteca_humb.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 23:46:46.234079 minha-biblioteca-humb-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      218 2023-06-12 23:46:20.000000 minha-biblioteca-humb-1.0.1/setup.py
```

