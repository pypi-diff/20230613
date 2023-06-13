# Comparing `tmp/modelbusinesscards-0.0.1.tar.gz` & `tmp/modelbusinesscards-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelbusinesscards-0.0.1.tar", last modified: Tue Jun 13 16:54:45 2023, max compression
+gzip compressed data, was "modelbusinesscards-0.0.2.tar", last modified: Tue Jun 13 17:20:54 2023, max compression
```

## Comparing `modelbusinesscards-0.0.1.tar` & `modelbusinesscards-0.0.2.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 16:54:45.063351 modelbusinesscards-0.0.1/
--rw-r--r--   0 upsolver   (501) staff       (20)      212 2023-06-13 16:54:45.063098 modelbusinesscards-0.0.1/PKG-INFO
--rw-r--r--   0 upsolver   (501) staff       (20)     4540 2023-06-13 16:37:28.000000 modelbusinesscards-0.0.1/README.md
--rw-r--r--   0 upsolver   (501) staff       (20)       38 2023-06-13 16:54:45.063428 modelbusinesscards-0.0.1/setup.cfg
--rw-r--r--   0 upsolver   (501) staff       (20)      606 2023-06-10 01:47:01.000000 modelbusinesscards-0.0.1/setup.py
-drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 16:54:45.051205 modelbusinesscards-0.0.1/src/
-drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 16:54:45.059681 modelbusinesscards-0.0.1/src/modelbusinesscards/
--rw-r--r--   0 upsolver   (501) staff       (20)       48 2023-06-09 22:06:30.000000 modelbusinesscards-0.0.1/src/modelbusinesscards/__init__.py
--rw-r--r--   0 upsolver   (501) staff       (20)      198 2023-06-10 01:15:47.000000 modelbusinesscards-0.0.1/src/modelbusinesscards/__main__.py
--rw-r--r--   0 upsolver   (501) staff       (20)      549 2023-06-09 22:06:51.000000 modelbusinesscards-0.0.1/src/modelbusinesscards/entities.py
--rw-r--r--   0 upsolver   (501) staff       (20)     1200 2023-06-10 01:13:37.000000 modelbusinesscards-0.0.1/src/modelbusinesscards/main.py
--rw-r--r--   0 upsolver   (501) staff       (20)     3721 2023-06-10 01:38:59.000000 modelbusinesscards-0.0.1/src/modelbusinesscards/parser.py
--rw-r--r--   0 upsolver   (501) staff       (20)     2000 2023-06-10 02:27:24.000000 modelbusinesscards-0.0.1/src/modelbusinesscards/writer.py
-drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 16:54:45.062736 modelbusinesscards-0.0.1/src/modelbusinesscards.egg-info/
--rw-r--r--   0 upsolver   (501) staff       (20)      212 2023-06-13 16:54:44.000000 modelbusinesscards-0.0.1/src/modelbusinesscards.egg-info/PKG-INFO
--rw-r--r--   0 upsolver   (501) staff       (20)      449 2023-06-13 16:54:45.000000 modelbusinesscards-0.0.1/src/modelbusinesscards.egg-info/SOURCES.txt
--rw-r--r--   0 upsolver   (501) staff       (20)        1 2023-06-13 16:54:44.000000 modelbusinesscards-0.0.1/src/modelbusinesscards.egg-info/dependency_links.txt
--rw-r--r--   0 upsolver   (501) staff       (20)        1 2023-06-10 00:57:20.000000 modelbusinesscards-0.0.1/src/modelbusinesscards.egg-info/not-zip-safe
--rw-r--r--   0 upsolver   (501) staff       (20)       19 2023-06-13 16:54:44.000000 modelbusinesscards-0.0.1/src/modelbusinesscards.egg-info/top_level.txt
+drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 17:20:54.176463 modelbusinesscards-0.0.2/
+-rw-r--r--   0 upsolver   (501) staff       (20)     1067 2023-06-13 17:07:56.000000 modelbusinesscards-0.0.2/LICENSE
+-rw-r--r--   0 upsolver   (501) staff       (20)      247 2023-06-13 17:20:54.176113 modelbusinesscards-0.0.2/PKG-INFO
+-rw-r--r--   0 upsolver   (501) staff       (20)     4697 2023-06-13 17:19:04.000000 modelbusinesscards-0.0.2/README.md
+-rw-r--r--   0 upsolver   (501) staff       (20)       38 2023-06-13 17:20:54.176591 modelbusinesscards-0.0.2/setup.cfg
+-rw-r--r--   0 upsolver   (501) staff       (20)      625 2023-06-13 17:20:10.000000 modelbusinesscards-0.0.2/setup.py
+drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 17:20:54.170421 modelbusinesscards-0.0.2/src/
+drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 17:20:54.173897 modelbusinesscards-0.0.2/src/modelbusinesscards/
+-rw-r--r--   0 upsolver   (501) staff       (20)       48 2023-06-09 22:06:30.000000 modelbusinesscards-0.0.2/src/modelbusinesscards/__init__.py
+-rw-r--r--   0 upsolver   (501) staff       (20)      198 2023-06-10 01:15:47.000000 modelbusinesscards-0.0.2/src/modelbusinesscards/__main__.py
+-rw-r--r--   0 upsolver   (501) staff       (20)      549 2023-06-09 22:06:51.000000 modelbusinesscards-0.0.2/src/modelbusinesscards/entities.py
+-rw-r--r--   0 upsolver   (501) staff       (20)     1200 2023-06-10 01:13:37.000000 modelbusinesscards-0.0.2/src/modelbusinesscards/main.py
+-rw-r--r--   0 upsolver   (501) staff       (20)     3721 2023-06-10 01:38:59.000000 modelbusinesscards-0.0.2/src/modelbusinesscards/parser.py
+-rw-r--r--   0 upsolver   (501) staff       (20)     2000 2023-06-10 02:27:24.000000 modelbusinesscards-0.0.2/src/modelbusinesscards/writer.py
+drwxr-xr-x   0 upsolver   (501) staff       (20)        0 2023-06-13 17:20:54.175737 modelbusinesscards-0.0.2/src/modelbusinesscards.egg-info/
+-rw-r--r--   0 upsolver   (501) staff       (20)      247 2023-06-13 17:20:54.000000 modelbusinesscards-0.0.2/src/modelbusinesscards.egg-info/PKG-INFO
+-rw-r--r--   0 upsolver   (501) staff       (20)      457 2023-06-13 17:20:54.000000 modelbusinesscards-0.0.2/src/modelbusinesscards.egg-info/SOURCES.txt
+-rw-r--r--   0 upsolver   (501) staff       (20)        1 2023-06-13 17:20:54.000000 modelbusinesscards-0.0.2/src/modelbusinesscards.egg-info/dependency_links.txt
+-rw-r--r--   0 upsolver   (501) staff       (20)        1 2023-06-10 00:57:20.000000 modelbusinesscards-0.0.2/src/modelbusinesscards.egg-info/not-zip-safe
+-rw-r--r--   0 upsolver   (501) staff       (20)       19 2023-06-13 17:20:54.000000 modelbusinesscards-0.0.2/src/modelbusinesscards.egg-info/top_level.txt
```

### Comparing `modelbusinesscards-0.0.1/README.md` & `modelbusinesscards-0.0.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # 📇 Model Business (Logic) Cards 📇
 
+![](http://img.shields.io/pypi/v/modelbusinesscards.svg?style=flat-square)
+![](http://img.shields.io/pypi/l/modelbusinesscards.svg?style=flat-square)
+
+---
+
+
 > Inspired by "[Model Cards for Model Reporting](https://arxiv.org/abs/1810.03993)" and the continued work of some of its authors [Timnit Gebru](https://twitter.com/timnitGebru) and [Margaret Mitchell](https://twitter.com/mmitchell_ai). Also inspired by my personal experiences building [Gideon](https://github.com/youmustfight/gideon), a AI-first tool for public defenders, and the hallucinations that could impact legal workers.
 
 Model Business Cards is a proof of concept, and Python package for generating documentation about the use of generative AI models focused on LLMs. As the AI community has pushed for better transparency about the biases and behaviors of models through the publishing of "Model Cards", we now have to push one step further into implementation decisions. 
 
 This is inspired by my desire to see builders in the goverment, legal, and social services share best practices and be easily auditable.
```

### Comparing `modelbusinesscards-0.0.1/src/modelbusinesscards/entities.py` & `modelbusinesscards-0.0.2/src/modelbusinesscards/entities.py`

 * *Files identical despite different names*

### Comparing `modelbusinesscards-0.0.1/src/modelbusinesscards/main.py` & `modelbusinesscards-0.0.2/src/modelbusinesscards/main.py`

 * *Files identical despite different names*

### Comparing `modelbusinesscards-0.0.1/src/modelbusinesscards/parser.py` & `modelbusinesscards-0.0.2/src/modelbusinesscards/parser.py`

 * *Files identical despite different names*

### Comparing `modelbusinesscards-0.0.1/src/modelbusinesscards/writer.py` & `modelbusinesscards-0.0.2/src/modelbusinesscards/writer.py`

 * *Files identical despite different names*

