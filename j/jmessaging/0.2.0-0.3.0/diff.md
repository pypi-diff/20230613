# Comparing `tmp/jmessaging-0.2.0.tar.gz` & `tmp/jmessaging-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/jmessaging-0.2.0.tar", last modified: Thu Oct  7 01:49:17 2021, max compression
+gzip compressed data, was "jmessaging-0.3.0.tar", last modified: Tue Jun 13 00:39:52 2023, max compression
```

## Comparing `jmessaging-0.2.0.tar` & `jmessaging-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,25 @@
-drwxrwxr-x   0 jose-chung  (1000) jose-chung  (1000)        0 2021-10-07 01:49:17.772246 jmessaging-0.2.0/
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)       15 2020-12-03 07:21:26.000000 jmessaging-0.2.0/MANIFEST.in
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     3882 2021-10-07 01:49:17.772246 jmessaging-0.2.0/PKG-INFO
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     2746 2020-12-03 07:21:26.000000 jmessaging-0.2.0/README.md
-drwxrwxr-x   0 jose-chung  (1000) jose-chung  (1000)        0 2021-10-07 01:49:17.768246 jmessaging-0.2.0/docs/
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     6345 2020-12-02 06:30:15.000000 jmessaging-0.2.0/docs/output-background.png
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     1985 2020-12-03 04:27:28.000000 jmessaging-0.2.0/docs/output-colorized.png
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     7068 2020-12-02 06:34:37.000000 jmessaging-0.2.0/docs/output-example.png
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     7005 2020-12-02 06:34:37.000000 jmessaging-0.2.0/docs/output-modified.png
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)    23797 2020-12-03 07:21:26.000000 jmessaging-0.2.0/docs/output-same-line.gif
-drwxrwxr-x   0 jose-chung  (1000) jose-chung  (1000)        0 2021-10-07 01:49:17.768246 jmessaging-0.2.0/jmessaging/
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)      153 2020-12-03 04:56:51.000000 jmessaging-0.2.0/jmessaging/__init__.py
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     2043 2021-10-07 01:39:25.000000 jmessaging-0.2.0/jmessaging/jcolor.py
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     3291 2021-10-07 01:39:25.000000 jmessaging-0.2.0/jmessaging/jmessaging.py
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)      300 2020-12-02 04:48:46.000000 jmessaging-0.2.0/jmessaging/jprint.py
-drwxrwxr-x   0 jose-chung  (1000) jose-chung  (1000)        0 2021-10-07 01:49:17.768246 jmessaging-0.2.0/jmessaging.egg-info/
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     3882 2021-10-07 01:49:17.000000 jmessaging-0.2.0/jmessaging.egg-info/PKG-INFO
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)      384 2021-10-07 01:49:17.000000 jmessaging-0.2.0/jmessaging.egg-info/SOURCES.txt
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)        1 2021-10-07 01:49:17.000000 jmessaging-0.2.0/jmessaging.egg-info/dependency_links.txt
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)       11 2021-10-07 01:49:17.000000 jmessaging-0.2.0/jmessaging.egg-info/top_level.txt
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)       38 2021-10-07 01:49:17.772246 jmessaging-0.2.0/setup.cfg
--rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)      492 2021-10-07 01:39:25.000000 jmessaging-0.2.0/setup.py
+drwxrwxr-x   0 jose-chung  (1000) jose-chung  (1000)        0 2023-06-13 00:39:52.172187 jmessaging-0.3.0/
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     1079 2020-12-02 05:14:37.000000 jmessaging-0.3.0/LICENSE
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)       15 2020-12-03 07:21:26.000000 jmessaging-0.3.0/MANIFEST.in
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     3021 2023-06-13 00:39:52.172187 jmessaging-0.3.0/PKG-INFO
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     2746 2020-12-03 07:21:26.000000 jmessaging-0.3.0/README.md
+drwxrwxr-x   0 jose-chung  (1000) jose-chung  (1000)        0 2023-06-13 00:39:52.168187 jmessaging-0.3.0/docs/
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     6345 2020-12-02 06:30:15.000000 jmessaging-0.3.0/docs/output-background.png
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     1985 2020-12-03 04:27:28.000000 jmessaging-0.3.0/docs/output-colorized.png
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     7068 2020-12-02 06:34:37.000000 jmessaging-0.3.0/docs/output-example.png
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     7005 2020-12-02 06:34:37.000000 jmessaging-0.3.0/docs/output-modified.png
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)    23797 2020-12-03 07:21:26.000000 jmessaging-0.3.0/docs/output-same-line.gif
+drwxrwxr-x   0 jose-chung  (1000) jose-chung  (1000)        0 2023-06-13 00:39:52.168187 jmessaging-0.3.0/jmessaging/
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)      323 2023-06-13 00:33:29.000000 jmessaging-0.3.0/jmessaging/__init__.py
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)      212 2023-06-13 00:33:29.000000 jmessaging-0.3.0/jmessaging/exceptions.py
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     3286 2023-06-13 00:33:29.000000 jmessaging-0.3.0/jmessaging/jcolor.py
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     5711 2023-06-13 00:33:29.000000 jmessaging-0.3.0/jmessaging/jmessage.py
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)      292 2023-06-13 00:33:29.000000 jmessaging-0.3.0/jmessaging/jprint.py
+drwxrwxr-x   0 jose-chung  (1000) jose-chung  (1000)        0 2023-06-13 00:39:52.172187 jmessaging-0.3.0/jmessaging.egg-info/
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)     3021 2023-06-13 00:39:52.000000 jmessaging-0.3.0/jmessaging.egg-info/PKG-INFO
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)      448 2023-06-13 00:39:52.000000 jmessaging-0.3.0/jmessaging.egg-info/SOURCES.txt
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)        1 2023-06-13 00:39:52.000000 jmessaging-0.3.0/jmessaging.egg-info/dependency_links.txt
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)       47 2023-06-13 00:39:52.000000 jmessaging-0.3.0/jmessaging.egg-info/requires.txt
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)       11 2023-06-13 00:39:52.000000 jmessaging-0.3.0/jmessaging.egg-info/top_level.txt
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)       38 2023-06-13 00:39:52.172187 jmessaging-0.3.0/setup.cfg
+-rw-rw-r--   0 jose-chung  (1000) jose-chung  (1000)      647 2023-06-13 00:33:29.000000 jmessaging-0.3.0/setup.py
```

### Comparing `jmessaging-0.2.0/README.md` & `jmessaging-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `jmessaging-0.2.0/docs/output-background.png` & `jmessaging-0.3.0/docs/output-background.png`

 * *Files identical despite different names*

### Comparing `jmessaging-0.2.0/docs/output-colorized.png` & `jmessaging-0.3.0/docs/output-colorized.png`

 * *Files identical despite different names*

### Comparing `jmessaging-0.2.0/docs/output-example.png` & `jmessaging-0.3.0/docs/output-example.png`

 * *Files identical despite different names*

### Comparing `jmessaging-0.2.0/docs/output-modified.png` & `jmessaging-0.3.0/docs/output-modified.png`

 * *Files identical despite different names*

### Comparing `jmessaging-0.2.0/docs/output-same-line.gif` & `jmessaging-0.3.0/docs/output-same-line.gif`

 * *Files identical despite different names*

