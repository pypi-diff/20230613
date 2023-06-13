# Comparing `tmp/ab-test-toolkit-0.0.5.tar.gz` & `tmp/ab-test-toolkit-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ab-test-toolkit-0.0.5.tar", last modified: Sat Jun 10 16:04:19 2023, max compression
+gzip compressed data, was "ab-test-toolkit-0.0.6.tar", last modified: Tue Jun 13 15:38:58 2023, max compression
```

## Comparing `ab-test-toolkit-0.0.5.tar` & `ab-test-toolkit-0.0.6.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-10 16:04:19.206115 ab-test-toolkit-0.0.5/
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     1064 2023-06-03 07:13:56.000000 ab-test-toolkit-0.0.5/LICENSE
--rw-rw-r--   0 kolja     (1000) kolja     (1000)      111 2023-04-27 10:12:58.000000 ab-test-toolkit-0.0.5/MANIFEST.in
--rw-rw-r--   0 kolja     (1000) kolja     (1000)    20044 2023-06-10 16:04:19.206115 ab-test-toolkit-0.0.5/PKG-INFO
--rw-rw-r--   0 kolja     (1000) kolja     (1000)    17217 2023-06-10 15:56:55.000000 ab-test-toolkit-0.0.5/README.md
-drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-10 16:04:19.206115 ab-test-toolkit-0.0.5/ab_test_toolkit/
--rw-rw-r--   0 kolja     (1000) kolja     (1000)       22 2023-06-10 15:55:33.000000 ab-test-toolkit-0.0.5/ab_test_toolkit/__init__.py
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     4245 2023-06-10 15:55:33.000000 ab-test-toolkit-0.0.5/ab_test_toolkit/_modidx.py
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     4453 2023-06-10 15:55:33.000000 ab-test-toolkit-0.0.5/ab_test_toolkit/generator.py
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     7366 2023-06-10 15:55:33.000000 ab-test-toolkit-0.0.5/ab_test_toolkit/plotting.py
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     8370 2023-06-10 15:55:33.000000 ab-test-toolkit-0.0.5/ab_test_toolkit/power.py
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     2033 2023-06-10 15:55:33.000000 ab-test-toolkit-0.0.5/ab_test_toolkit/wrappers.py
-drwxrwxr-x   0 kolja     (1000) kolja     (1000)        0 2023-06-10 16:04:19.206115 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/
--rw-rw-r--   0 kolja     (1000) kolja     (1000)    20044 2023-06-10 16:04:19.000000 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/PKG-INFO
--rw-rw-r--   0 kolja     (1000) kolja     (1000)      490 2023-06-10 16:04:19.000000 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/SOURCES.txt
--rw-rw-r--   0 kolja     (1000) kolja     (1000)        1 2023-06-10 16:04:19.000000 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/dependency_links.txt
--rw-rw-r--   0 kolja     (1000) kolja     (1000)       73 2023-06-10 16:04:19.000000 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/entry_points.txt
--rw-rw-r--   0 kolja     (1000) kolja     (1000)        1 2023-06-03 07:19:15.000000 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/not-zip-safe
--rw-rw-r--   0 kolja     (1000) kolja     (1000)       98 2023-06-10 16:04:19.000000 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/requires.txt
--rw-rw-r--   0 kolja     (1000) kolja     (1000)       16 2023-06-10 16:04:19.000000 ab-test-toolkit-0.0.5/ab_test_toolkit.egg-info/top_level.txt
--rw-rw-r--   0 kolja     (1000) kolja     (1000)      951 2023-06-10 16:04:07.000000 ab-test-toolkit-0.0.5/settings.ini
--rw-rw-r--   0 kolja     (1000) kolja     (1000)       38 2023-06-10 16:04:19.206115 ab-test-toolkit-0.0.5/setup.cfg
--rw-rw-r--   0 kolja     (1000) kolja     (1000)     2711 2023-06-03 07:16:06.000000 ab-test-toolkit-0.0.5/setup.py
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-13 15:38:58.707148 ab-test-toolkit-0.0.6/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     1064 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.6/LICENSE
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      111 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.6/MANIFEST.in
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7816 2023-06-13 15:38:58.707040 ab-test-toolkit-0.0.6/PKG-INFO
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     5301 2023-06-13 11:53:01.000000 ab-test-toolkit-0.0.6/README.md
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-13 15:38:58.705615 ab-test-toolkit-0.0.6/ab_test_toolkit/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       22 2023-06-13 15:33:07.000000 ab-test-toolkit-0.0.6/ab_test_toolkit/__init__.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     6337 2023-06-13 15:33:07.000000 ab-test-toolkit-0.0.6/ab_test_toolkit/_modidx.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     1076 2023-06-13 15:33:07.000000 ab-test-toolkit-0.0.6/ab_test_toolkit/analyze.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     4453 2023-06-13 15:33:07.000000 ab-test-toolkit-0.0.6/ab_test_toolkit/generator.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7403 2023-06-13 15:33:07.000000 ab-test-toolkit-0.0.6/ab_test_toolkit/plotting.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     8370 2023-06-13 15:33:07.000000 ab-test-toolkit-0.0.6/ab_test_toolkit/power.py
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)    11404 2023-06-13 15:33:07.000000 ab-test-toolkit-0.0.6/ab_test_toolkit/wrappers.py
+drwxr-xr-x   0 koljakleineberg   (501) staff       (20)        0 2023-06-13 15:38:58.706842 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     7816 2023-06-13 15:38:58.000000 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/PKG-INFO
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      517 2023-06-13 15:38:58.000000 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-13 15:38:58.000000 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       73 2023-06-13 15:38:58.000000 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/entry_points.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)        1 2023-06-05 07:35:26.000000 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/not-zip-safe
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       98 2023-06-13 15:38:58.000000 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/requires.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       16 2023-06-13 15:38:58.000000 ab-test-toolkit-0.0.6/ab_test_toolkit.egg-info/top_level.txt
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)      951 2023-06-13 15:38:54.000000 ab-test-toolkit-0.0.6/settings.ini
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)       38 2023-06-13 15:38:58.707195 ab-test-toolkit-0.0.6/setup.cfg
+-rw-r--r--   0 koljakleineberg   (501) staff       (20)     2711 2023-06-05 06:50:28.000000 ab-test-toolkit-0.0.6/setup.py
```

### Comparing `ab-test-toolkit-0.0.5/LICENSE` & `ab-test-toolkit-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.5/ab_test_toolkit/generator.py` & `ab-test-toolkit-0.0.6/ab_test_toolkit/generator.py`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.5/ab_test_toolkit/plotting.py` & `ab-test-toolkit-0.0.6/ab_test_toolkit/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -152,19 +152,20 @@
         yaxis_title="PDF",
         legend=dict(yanchor="top", y=1, xanchor="left", x=0.0),
     )
 
     return fig
 
 # %% ../nbs/03_plotting.ipynb 11
-def plot_binary_power(cr0=0.01, cr1=0.012, alpha=0.05, one_sided=True,vline_power=0.8):
+def plot_binary_power(cr0=0.01, cr1=0.012, alpha=0.05, one_sided=True,vline_power=0.8,powers=None):
     """
     Generate a chart that shows the 
     """
-    powers = np.arange(0.1, 0.91, 0.025)
+    if powers==None:
+        powers = np.arange(0.1, 0.91, 0.025)
     sizes = []
     for power in powers:
         size = sample_size_binary(
             cr0=cr0, cr1=cr1, alpha=alpha, power=power, one_sided=one_sided
         )
         sizes.append(size)
         fig = make_subplots()
```

### Comparing `ab-test-toolkit-0.0.5/ab_test_toolkit/power.py` & `ab-test-toolkit-0.0.6/ab_test_toolkit/power.py`

 * *Files identical despite different names*

### Comparing `ab-test-toolkit-0.0.5/settings.ini` & `ab-test-toolkit-0.0.6/settings.ini`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = ab-test-toolkit
 lib_name = %(repo)s
-version = 0.0.5
+version = 0.0.6
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = ab_test_toolkit
```

### Comparing `ab-test-toolkit-0.0.5/setup.py` & `ab-test-toolkit-0.0.6/setup.py`

 * *Files identical despite different names*

