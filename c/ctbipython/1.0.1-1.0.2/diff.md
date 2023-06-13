# Comparing `tmp/ctbipython-1.0.1.tar.gz` & `tmp/ctbipython-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctbipython-1.0.1.tar", last modified: Tue Jun 13 14:21:58 2023, max compression
+gzip compressed data, was "ctbipython-1.0.2.tar", last modified: Tue Jun 13 15:53:01 2023, max compression
```

## Comparing `ctbipython-1.0.1.tar` & `ctbipython-1.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 14:21:58.065994 ctbipython-1.0.1/
--rw-rw-rw-   0        0        0      197 2023-06-13 14:21:58.065994 ctbipython-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     1355 2023-05-24 14:03:51.000000 ctbipython-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 14:21:58.040833 ctbipython-1.0.1/ctbipython/
--rw-rw-rw-   0        0        0        0 2023-05-24 12:22:47.000000 ctbipython-1.0.1/ctbipython/__init__.py
--rw-rw-rw-   0        0        0    78791 2023-05-31 21:59:28.000000 ctbipython-1.0.1/ctbipython/ctbi.py
--rw-rw-rw-   0        0        0     3950 2023-06-13 13:13:47.000000 ctbipython-1.0.1/ctbipython/example.py
-drwxrwxrwx   0        0        0        0 2023-06-13 14:21:58.064994 ctbipython-1.0.1/ctbipython.egg-info/
--rw-rw-rw-   0        0        0      197 2023-06-13 14:21:57.000000 ctbipython-1.0.1/ctbipython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-13 14:21:57.000000 ctbipython-1.0.1/ctbipython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 14:21:57.000000 ctbipython-1.0.1/ctbipython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-13 14:21:57.000000 ctbipython-1.0.1/ctbipython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 14:21:57.000000 ctbipython-1.0.1/ctbipython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 14:21:58.066991 ctbipython-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      348 2023-06-13 13:14:03.000000 ctbipython-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:53:01.569013 ctbipython-1.0.2/
+-rw-rw-rw-   0        0        0      197 2023-06-13 15:53:01.568015 ctbipython-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1355 2023-05-24 14:03:51.000000 ctbipython-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 15:53:01.554053 ctbipython-1.0.2/ctbipython/
+-rw-rw-rw-   0        0        0        0 2023-05-24 12:22:47.000000 ctbipython-1.0.2/ctbipython/__init__.py
+-rw-rw-rw-   0        0        0    78792 2023-06-13 15:51:59.000000 ctbipython-1.0.2/ctbipython/ctbi.py
+-rw-rw-rw-   0        0        0     3950 2023-06-13 13:13:47.000000 ctbipython-1.0.2/ctbipython/example.py
+drwxrwxrwx   0        0        0        0 2023-06-13 15:53:01.567019 ctbipython-1.0.2/ctbipython.egg-info/
+-rw-rw-rw-   0        0        0      197 2023-06-13 15:53:01.000000 ctbipython-1.0.2/ctbipython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-13 15:53:01.000000 ctbipython-1.0.2/ctbipython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 15:53:01.000000 ctbipython-1.0.2/ctbipython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-13 15:53:01.000000 ctbipython-1.0.2/ctbipython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 15:53:01.000000 ctbipython-1.0.2/ctbipython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 15:53:01.569013 ctbipython-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      348 2023-06-13 15:52:43.000000 ctbipython-1.0.2/setup.py
```

### Comparing `ctbipython-1.0.1/README.md` & `ctbipython-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `ctbipython-1.0.1/ctbipython/ctbi.py` & `ctbipython-1.0.2/ctbipython/ctbi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1168,15 +1168,15 @@
             else:
                 if seq_temp_fin is not None:
                     seq_bin_side = seq_temp_fin
         
     # Cut seq_bin_side
     index_side = list(range(0, len(seq_bin_side)))
     ind_min = np.where(seq_bin_side[index_side] <= x_t[0])[0].tolist()
-    ind_max = np.where(seq_bin_side[index_side] > x_t[len(x_t)-1])[0].tolist()
+    ind_max = np.where(seq_bin_side[index_side] >= x_t[len(x_t)-1])[0].tolist()
     seq_bin_side = seq_bin_side[max(ind_min):min(ind_max)+1]
     
     # Find seq_bin_center
     
     seq_bin_center_beg = None
     seq_bin_center_fin = None
```

### Comparing `ctbipython-1.0.1/ctbipython/example.py` & `ctbipython-1.0.2/ctbipython/example.py`

 * *Files identical despite different names*

