# Comparing `tmp/elifearticle-0.8.0.tar.gz` & `tmp/elifearticle-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elifearticle-0.8.0.tar", last modified: Fri Sep  2 18:59:20 2022, max compression
+gzip compressed data, was "elifearticle-0.9.0.tar", last modified: Fri Sep  9 01:39:32 2022, max compression
```

## Comparing `elifearticle-0.8.0.tar` & `elifearticle-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2022-09-02 18:59:20.655815 elifearticle-0.8.0/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     1071 2022-09-02 18:58:52.000000 elifearticle-0.8.0/LICENSE
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       24 2022-09-02 18:58:52.000000 elifearticle-0.8.0/MANIFEST.in
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      705 2022-09-02 18:59:20.655815 elifearticle-0.8.0/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      205 2022-09-02 18:58:52.000000 elifearticle-0.8.0/README.md
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2022-09-02 18:59:20.655815 elifearticle-0.8.0/elifearticle/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       22 2022-09-02 18:58:52.000000 elifearticle-0.8.0/elifearticle/__init__.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    12249 2022-09-02 18:58:52.000000 elifearticle-0.8.0/elifearticle/article.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)    27153 2022-09-02 18:58:52.000000 elifearticle-0.8.0/elifearticle/parse.py
--rw-r--r--   0 jenkins   (1002) jenkins    (998)     4988 2022-09-02 18:58:52.000000 elifearticle-0.8.0/elifearticle/utils.py
-drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2022-09-02 18:59:20.655815 elifearticle-0.8.0/elifearticle.egg-info/
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      705 2022-09-02 18:59:20.000000 elifearticle-0.8.0/elifearticle.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      327 2022-09-02 18:59:20.000000 elifearticle-0.8.0/elifearticle.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2022-09-02 18:59:20.000000 elifearticle-0.8.0/elifearticle.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       21 2022-09-02 18:59:20.000000 elifearticle-0.8.0/elifearticle.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       13 2022-09-02 18:59:20.000000 elifearticle-0.8.0/elifearticle.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       77 2022-09-02 18:58:52.000000 elifearticle-0.8.0/requirements.txt
--rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2022-09-02 18:59:20.655815 elifearticle-0.8.0/setup.cfg
--rw-r--r--   0 jenkins   (1002) jenkins    (998)      768 2022-09-02 18:58:52.000000 elifearticle-0.8.0/setup.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2022-09-09 01:39:32.592198 elifearticle-0.9.0/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     1071 2022-09-09 01:39:04.000000 elifearticle-0.9.0/LICENSE
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       24 2022-09-09 01:39:04.000000 elifearticle-0.9.0/MANIFEST.in
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      705 2022-09-09 01:39:32.592198 elifearticle-0.9.0/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      205 2022-09-09 01:39:04.000000 elifearticle-0.9.0/README.md
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2022-09-09 01:39:32.592198 elifearticle-0.9.0/elifearticle/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       22 2022-09-09 01:39:04.000000 elifearticle-0.9.0/elifearticle/__init__.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    12360 2022-09-09 01:39:04.000000 elifearticle-0.9.0/elifearticle/article.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)    27153 2022-09-09 01:39:04.000000 elifearticle-0.9.0/elifearticle/parse.py
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)     4988 2022-09-09 01:39:04.000000 elifearticle-0.9.0/elifearticle/utils.py
+drwxr-xr-x   0 jenkins   (1002) jenkins    (998)        0 2022-09-09 01:39:32.592198 elifearticle-0.9.0/elifearticle.egg-info/
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      705 2022-09-09 01:39:32.000000 elifearticle-0.9.0/elifearticle.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      327 2022-09-09 01:39:32.000000 elifearticle-0.9.0/elifearticle.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)        1 2022-09-09 01:39:32.000000 elifearticle-0.9.0/elifearticle.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       21 2022-09-09 01:39:32.000000 elifearticle-0.9.0/elifearticle.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       13 2022-09-09 01:39:32.000000 elifearticle-0.9.0/elifearticle.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       77 2022-09-09 01:39:04.000000 elifearticle-0.9.0/requirements.txt
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)       38 2022-09-09 01:39:32.592198 elifearticle-0.9.0/setup.cfg
+-rw-r--r--   0 jenkins   (1002) jenkins    (998)      768 2022-09-09 01:39:04.000000 elifearticle-0.9.0/setup.py
```

### Comparing `elifearticle-0.8.0/LICENSE` & `elifearticle-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `elifearticle-0.8.0/PKG-INFO` & `elifearticle-0.9.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elifearticle
-Version: 0.8.0
+Version: 0.9.0
 Summary: eLife article objects.
 Home-page: https://github.com/elifesciences/elife-article
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `elifearticle-0.8.0/elifearticle/article.py` & `elifearticle-0.9.0/elifearticle/article.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,14 +74,16 @@
         self.version = None
         self.publisher_name = None
         self.issue = None
         self.review_articles = []
         self.clinical_trials = []
         self.preprint = None
         self.related_objects = []
+        # group_title for use in posted_content Crossref deposits of preprints
+        self.group_title = None
 
     def add_contributor(self, contributor):
         self.contributors.append(contributor)
 
     def add_research_organism(self, research_organism):
         self.research_organisms.append(research_organism)
```

### Comparing `elifearticle-0.8.0/elifearticle/parse.py` & `elifearticle-0.9.0/elifearticle/parse.py`

 * *Files identical despite different names*

### Comparing `elifearticle-0.8.0/elifearticle/utils.py` & `elifearticle-0.9.0/elifearticle/utils.py`

 * *Files identical despite different names*

### Comparing `elifearticle-0.8.0/elifearticle.egg-info/PKG-INFO` & `elifearticle-0.9.0/elifearticle.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: elifearticle
-Version: 0.8.0
+Version: 0.9.0
 Summary: eLife article objects.
 Home-page: https://github.com/elifesciences/elife-article
 Maintainer: eLife Sciences Publications Ltd.
 Maintainer-email: tech-team@elifesciences.org
 License: MIT
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `elifearticle-0.8.0/setup.py` & `elifearticle-0.9.0/setup.py`

 * *Files identical despite different names*

