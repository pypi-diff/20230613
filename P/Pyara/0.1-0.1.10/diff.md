# Comparing `tmp/Pyara-0.1.tar.gz` & `tmp/Pyara-0.1.10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\Pyara-0.1.tar", last modified: Sun May 28 18:35:40 2023, max compression
+gzip compressed data, was "dist\Pyara-0.1.10.tar", last modified: Tue Jun 13 12:39:18 2023, max compression
```

## Comparing `Pyara-0.1.tar` & `Pyara-0.1.10.tar`

### file list

```diff
@@ -1,11 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-28 18:35:40.000000 Pyara-0.1/
--rw-rw-rw-   0        0        0      295 2023-05-28 18:35:40.000000 Pyara-0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-28 18:35:40.000000 Pyara-0.1/Pyara.egg-info/
--rw-rw-rw-   0        0        0      295 2023-05-28 18:35:40.000000 Pyara-0.1/Pyara.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      172 2023-05-28 18:35:40.000000 Pyara-0.1/Pyara.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-28 18:35:40.000000 Pyara-0.1/Pyara.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-05-21 09:07:37.000000 Pyara-0.1/Pyara.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        1 2023-05-28 18:35:40.000000 Pyara-0.1/Pyara.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       48 2023-04-10 18:25:02.000000 Pyara-0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-28 18:35:40.000000 Pyara-0.1/setup.cfg
--rw-rw-rw-   0        0        0      450 2023-05-28 18:32:05.000000 Pyara-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:39:18.000000 Pyara-0.1.10/
+-rw-rw-rw-   0        0        0     1098 2023-06-05 08:31:19.000000 Pyara-0.1.10/LICENSE
+-rw-rw-rw-   0        0        0      539 2023-06-13 12:39:18.000000 Pyara-0.1.10/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-06-13 12:39:18.000000 Pyara-0.1.10/Pyara.egg-info/
+-rw-rw-rw-   0        0        0      539 2023-06-13 12:39:18.000000 Pyara-0.1.10/Pyara.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2023-06-13 12:39:18.000000 Pyara-0.1.10/Pyara.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 12:39:18.000000 Pyara-0.1.10/Pyara.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-05-21 09:07:37.000000 Pyara-0.1.10/Pyara.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       33 2023-06-13 12:39:18.000000 Pyara-0.1.10/Pyara.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2023-06-13 12:39:18.000000 Pyara-0.1.10/Pyara.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       48 2023-04-10 18:25:02.000000 Pyara-0.1.10/README.md
+-rw-rw-rw-   0        0        0      108 2023-06-05 08:20:17.000000 Pyara-0.1.10/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 12:39:18.000000 Pyara-0.1.10/setup.cfg
+-rw-rw-rw-   0        0        0      988 2023-06-13 12:39:16.000000 Pyara-0.1.10/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:39:18.000000 Pyara-0.1.10/src/
+-rw-rw-rw-   0        0        0      118 2023-06-13 12:08:03.000000 Pyara-0.1.10/src/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 12:39:18.000000 Pyara-0.1.10/src/pyara/
+drwxrwxrwx   0        0        0        0 2023-06-13 12:39:18.000000 Pyara-0.1.10/src/pyara/Model/
+-rw-rw-rw-   0        0        0        0 2023-06-11 12:49:19.000000 Pyara-0.1.10/src/pyara/Model/__init__.py
+-rw-rw-rw-   0        0        0     3983 2023-06-05 08:24:59.000000 Pyara-0.1.10/src/pyara/Model/model.py
+-rw-rw-rw-   0        0        0        0 2023-06-11 12:49:10.000000 Pyara-0.1.10/src/pyara/__init__.py
+-rw-rw-rw-   0        0        0     6412 2023-06-11 12:30:09.000000 Pyara-0.1.10/src/pyara/audio_prepare.py
+-rw-rw-rw-   0        0        0     1029 2023-05-21 08:36:42.000000 Pyara-0.1.10/src/pyara/config.py
+-rw-rw-rw-   0        0        0      798 2023-06-11 12:52:20.000000 Pyara-0.1.10/src/pyara/main.py
```

