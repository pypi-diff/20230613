# Comparing `tmp/ctbipython-1.0.2.tar.gz` & `tmp/ctbipython-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctbipython-1.0.2.tar", last modified: Tue Jun 13 15:53:01 2023, max compression
+gzip compressed data, was "ctbipython-1.0.3.tar", last modified: Tue Jun 13 16:45:52 2023, max compression
```

## Comparing `ctbipython-1.0.2.tar` & `ctbipython-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 15:53:01.569013 ctbipython-1.0.2/
--rw-rw-rw-   0        0        0      197 2023-06-13 15:53:01.568015 ctbipython-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1355 2023-05-24 14:03:51.000000 ctbipython-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 15:53:01.554053 ctbipython-1.0.2/ctbipython/
--rw-rw-rw-   0        0        0        0 2023-05-24 12:22:47.000000 ctbipython-1.0.2/ctbipython/__init__.py
--rw-rw-rw-   0        0        0    78792 2023-06-13 15:51:59.000000 ctbipython-1.0.2/ctbipython/ctbi.py
--rw-rw-rw-   0        0        0     3950 2023-06-13 13:13:47.000000 ctbipython-1.0.2/ctbipython/example.py
-drwxrwxrwx   0        0        0        0 2023-06-13 15:53:01.567019 ctbipython-1.0.2/ctbipython.egg-info/
--rw-rw-rw-   0        0        0      197 2023-06-13 15:53:01.000000 ctbipython-1.0.2/ctbipython.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      251 2023-06-13 15:53:01.000000 ctbipython-1.0.2/ctbipython.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 15:53:01.000000 ctbipython-1.0.2/ctbipython.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       38 2023-06-13 15:53:01.000000 ctbipython-1.0.2/ctbipython.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-06-13 15:53:01.000000 ctbipython-1.0.2/ctbipython.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 15:53:01.569013 ctbipython-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      348 2023-06-13 15:52:43.000000 ctbipython-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:45:52.060259 ctbipython-1.0.3/
+-rw-rw-rw-   0        0        0      197 2023-06-13 16:45:52.060259 ctbipython-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1355 2023-05-24 14:03:51.000000 ctbipython-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 16:45:52.043307 ctbipython-1.0.3/ctbipython/
+-rw-rw-rw-   0        0        0        0 2023-05-24 12:22:47.000000 ctbipython-1.0.3/ctbipython/__init__.py
+-rw-rw-rw-   0        0        0    78961 2023-06-13 16:45:41.000000 ctbipython-1.0.3/ctbipython/ctbi.py
+-rw-rw-rw-   0        0        0     3950 2023-06-13 13:13:47.000000 ctbipython-1.0.3/ctbipython/example.py
+drwxrwxrwx   0        0        0        0 2023-06-13 16:45:52.058269 ctbipython-1.0.3/ctbipython.egg-info/
+-rw-rw-rw-   0        0        0      197 2023-06-13 16:45:51.000000 ctbipython-1.0.3/ctbipython.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      251 2023-06-13 16:45:51.000000 ctbipython-1.0.3/ctbipython.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 16:45:51.000000 ctbipython-1.0.3/ctbipython.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       38 2023-06-13 16:45:51.000000 ctbipython-1.0.3/ctbipython.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 16:45:51.000000 ctbipython-1.0.3/ctbipython.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 16:45:52.061259 ctbipython-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      348 2023-06-13 16:45:45.000000 ctbipython-1.0.3/setup.py
```

### Comparing `ctbipython-1.0.2/README.md` & `ctbipython-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `ctbipython-1.0.2/ctbipython/ctbi.py` & `ctbipython-1.0.3/ctbipython/ctbi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1155,28 +1155,30 @@
         if bin_side >= x_t[0]:
             seq_temp_beg = hidd_seq(start=bin_side,end=x_t[0],by=by_minus)[::-1]  
             seq_temp_beg = hidd_seq(start=bin_side,length_out=len(seq_temp_beg)+1,by=by_minus)[::-1]  
 
         if bin_side <= x_t[len(x_t)-1]:
             seq_temp_fin = hidd_seq(start=bin_side,end=x_t[len(x_t)-1],by=by_plus)        
             seq_temp_fin = hidd_seq(start=bin_side,length_out=len(seq_temp_fin)+1,by=by_plus) 
+            if seq_temp_fin[len(seq_temp_fin)-1] <= x_t[len(x_t)-1]:
+                seq_temp_fin = hidd_seq(start=bin_side,length_out=len(seq_temp_fin)+1,by=by_plus) 
                
         if seq_temp_beg is not None and seq_temp_fin is not None:
             seq_bin_side = np.concatenate([seq_temp_beg, seq_temp_fin[1:]]) 
         else:
             if seq_temp_beg is not None:
                 seq_bin_side = seq_temp_beg
             else:
                 if seq_temp_fin is not None:
                     seq_bin_side = seq_temp_fin
         
     # Cut seq_bin_side
     index_side = list(range(0, len(seq_bin_side)))
     ind_min = np.where(seq_bin_side[index_side] <= x_t[0])[0].tolist()
-    ind_max = np.where(seq_bin_side[index_side] >= x_t[len(x_t)-1])[0].tolist()
+    ind_max = np.where(seq_bin_side[index_side] > x_t[len(x_t)-1])[0].tolist()
     seq_bin_side = seq_bin_side[max(ind_min):min(ind_max)+1]
     
     # Find seq_bin_center
     
     seq_bin_center_beg = None
     seq_bin_center_fin = None
```

### Comparing `ctbipython-1.0.2/ctbipython/example.py` & `ctbipython-1.0.3/ctbipython/example.py`

 * *Files identical despite different names*

