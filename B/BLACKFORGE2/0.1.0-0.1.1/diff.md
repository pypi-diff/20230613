# Comparing `tmp/BLACKFORGE2-0.1.0.tar.gz` & `tmp/BLACKFORGE2-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BLACKFORGE2-0.1.0.tar", last modified: Tue Jun 13 00:48:27 2023, max compression
+gzip compressed data, was "BLACKFORGE2-0.1.1.tar", last modified: Tue Jun 13 01:22:05 2023, max compression
```

## Comparing `BLACKFORGE2-0.1.0.tar` & `BLACKFORGE2-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 00:48:27.541964 BLACKFORGE2-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-06-13 00:48:27.517567 BLACKFORGE2-0.1.0/BLACKFORGE2/
--rw-rw-rw-   0        0        0    14021 2023-06-13 00:41:32.000000 BLACKFORGE2-0.1.0/BLACKFORGE2/FORGE.py
--rw-rw-rw-   0        0        0       19 2023-06-13 00:42:01.000000 BLACKFORGE2-0.1.0/BLACKFORGE2/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 00:48:27.539968 BLACKFORGE2-0.1.0/BLACKFORGE2.egg-info/
--rw-rw-rw-   0        0        0      311 2023-06-13 00:48:27.000000 BLACKFORGE2-0.1.0/BLACKFORGE2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-06-13 00:48:27.000000 BLACKFORGE2-0.1.0/BLACKFORGE2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 00:48:27.000000 BLACKFORGE2-0.1.0/BLACKFORGE2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-06-13 00:48:27.000000 BLACKFORGE2-0.1.0/BLACKFORGE2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-13 00:48:27.000000 BLACKFORGE2-0.1.0/BLACKFORGE2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      311 2023-06-13 00:48:27.540966 BLACKFORGE2-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       70 2023-06-13 00:44:29.000000 BLACKFORGE2-0.1.0/README.rst
--rw-rw-rw-   0        0        0       42 2023-06-13 00:48:27.541964 BLACKFORGE2-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      491 2023-06-13 00:47:58.000000 BLACKFORGE2-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 01:22:05.807400 BLACKFORGE2-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-06-13 01:22:05.791406 BLACKFORGE2-0.1.1/BLACKFORGE2/
+-rw-rw-rw-   0        0        0    14022 2023-06-13 01:21:34.000000 BLACKFORGE2-0.1.1/BLACKFORGE2/FORGE.py
+-rw-rw-rw-   0        0        0       20 2023-06-13 01:21:24.000000 BLACKFORGE2-0.1.1/BLACKFORGE2/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 01:22:05.805402 BLACKFORGE2-0.1.1/BLACKFORGE2.egg-info/
+-rw-rw-rw-   0        0        0      311 2023-06-13 01:22:05.000000 BLACKFORGE2-0.1.1/BLACKFORGE2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      246 2023-06-13 01:22:05.000000 BLACKFORGE2-0.1.1/BLACKFORGE2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 01:22:05.000000 BLACKFORGE2-0.1.1/BLACKFORGE2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-06-13 01:22:05.000000 BLACKFORGE2-0.1.1/BLACKFORGE2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 01:22:05.000000 BLACKFORGE2-0.1.1/BLACKFORGE2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-06-13 00:44:16.000000 BLACKFORGE2-0.1.1/LICENSE
+-rw-rw-rw-   0        0        0      311 2023-06-13 01:22:05.807400 BLACKFORGE2-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       70 2023-06-13 00:44:29.000000 BLACKFORGE2-0.1.1/README.rst
+-rw-rw-rw-   0        0        0       42 2023-06-13 01:22:05.807400 BLACKFORGE2-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      491 2023-06-13 01:21:42.000000 BLACKFORGE2-0.1.1/setup.py
```

### Comparing `BLACKFORGE2-0.1.0/BLACKFORGE2/FORGE.py` & `BLACKFORGE2-0.1.1/BLACKFORGE2/FORGE.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" BLACKFORGE """
+""" BLACKFORGE2 """
 """ Developed by Setoichi at Savior Systems """
 """ (/0_0)/ """
 import pygame
 import pygame.gfxdraw
 import math, random, sys
 
 from pygame.locals import *
```

### Comparing `BLACKFORGE2-0.1.0/LICENSE` & `BLACKFORGE2-0.1.1/LICENSE`

 * *Files identical despite different names*

