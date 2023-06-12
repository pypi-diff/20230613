# Comparing `tmp/devcheck-0.1.tar.gz` & `tmp/devcheck-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devcheck-0.1.tar", last modified: Mon Jun 12 21:21:28 2023, max compression
+gzip compressed data, was "devcheck-0.2.tar", last modified: Mon Jun 12 22:11:30 2023, max compression
```

## Comparing `devcheck-0.1.tar` & `devcheck-0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 21:21:28.715899 devcheck-0.1/
--rw-rw-rw-   0        0        0       77 2023-06-12 21:21:28.715674 devcheck-0.1/PKG-INFO
--rw-rw-rw-   0        0        0        0 2023-06-12 20:38:49.000000 devcheck-0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-12 21:21:28.705963 devcheck-0.1/devcheck/
--rw-rw-rw-   0        0        0        0 2023-06-12 20:38:31.000000 devcheck-0.1/devcheck/__init__.py
--rw-rw-rw-   0        0        0     3005 2023-06-12 20:50:02.000000 devcheck-0.1/devcheck/main.py
-drwxrwxrwx   0        0        0        0 2023-06-12 21:21:28.713757 devcheck-0.1/devcheck.egg-info/
--rw-rw-rw-   0        0        0       77 2023-06-12 21:21:28.000000 devcheck-0.1/devcheck.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      219 2023-06-12 21:21:28.000000 devcheck-0.1/devcheck.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 21:21:28.000000 devcheck-0.1/devcheck.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-06-12 21:21:28.000000 devcheck-0.1/devcheck.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        9 2023-06-12 21:21:28.000000 devcheck-0.1/devcheck.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-12 21:21:28.716465 devcheck-0.1/setup.cfg
--rw-rw-rw-   0        0        0      287 2023-06-12 20:40:38.000000 devcheck-0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:11:30.286108 devcheck-0.2/
+-rw-rw-rw-   0        0        0       77 2023-06-12 22:11:30.284557 devcheck-0.2/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:38:49.000000 devcheck-0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-12 22:11:30.277164 devcheck-0.2/devcheck/
+-rw-rw-rw-   0        0        0        0 2023-06-12 20:38:31.000000 devcheck-0.2/devcheck/__init__.py
+-rw-rw-rw-   0        0        0     4285 2023-06-12 22:10:44.000000 devcheck-0.2/devcheck/main.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:11:30.282370 devcheck-0.2/devcheck.egg-info/
+-rw-rw-rw-   0        0        0       77 2023-06-12 22:11:30.000000 devcheck-0.2/devcheck.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      219 2023-06-12 22:11:30.000000 devcheck-0.2/devcheck.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 22:11:30.000000 devcheck-0.2/devcheck.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-06-12 22:11:30.000000 devcheck-0.2/devcheck.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        9 2023-06-12 22:11:30.000000 devcheck-0.2/devcheck.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-12 22:11:30.286739 devcheck-0.2/setup.cfg
+-rw-rw-rw-   0        0        0      287 2023-06-12 21:24:54.000000 devcheck-0.2/setup.py
```

