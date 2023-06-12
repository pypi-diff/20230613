# Comparing `tmp/MALDIpy-0.1.2.tar.gz` & `tmp/MALDIpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MALDIpy-0.1.2.tar", last modified: Mon Jun 12 22:12:05 2023, max compression
+gzip compressed data, was "MALDIpy-0.1.3.tar", last modified: Mon Jun 12 22:20:46 2023, max compression
```

## Comparing `MALDIpy-0.1.2.tar` & `MALDIpy-0.1.3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:12:04.997632 MALDIpy-0.1.2/
--rw-r--r--   0 hli       (1002) labmem    (1001)     1062 2023-04-04 21:12:06.000000 MALDIpy-0.1.2/LICENSE
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:12:04.965632 MALDIpy-0.1.2/MALDIpy/
--rw-r--r--   0 hli       (1002) labmem    (1001)      187 2023-06-12 22:10:24.000000 MALDIpy-0.1.2/MALDIpy/__init__.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     7689 2023-06-12 22:10:09.000000 MALDIpy-0.1.2/MALDIpy/featureplot.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     6599 2023-04-06 16:02:36.000000 MALDIpy-0.1.2/MALDIpy/msi_data.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     3084 2023-04-06 18:34:41.000000 MALDIpy-0.1.2/MALDIpy/multi_sample.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     6619 2023-06-10 01:50:57.000000 MALDIpy-0.1.2/MALDIpy/projection.py
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:12:04.993632 MALDIpy-0.1.2/MALDIpy/shell/
--rw-r--r--   0 hli       (1002) labmem    (1001)       61 2023-04-04 21:15:37.000000 MALDIpy-0.1.2/MALDIpy/shell/__init__.py
--rw-r--r--   0 hli       (1002) labmem    (1001)      196 2023-04-04 21:15:37.000000 MALDIpy-0.1.2/MALDIpy/shell/usage.py
--rw-r--r--   0 hli       (1002) labmem    (1001)     1690 2023-04-06 13:55:22.000000 MALDIpy-0.1.2/MALDIpy/single_cell.py
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:12:04.997632 MALDIpy-0.1.2/MALDIpy/src/
--rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.1.2/MALDIpy/src/temp.txt
-drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:12:04.985632 MALDIpy-0.1.2/MALDIpy.egg-info/
--rw-r--r--   0 hli       (1002) labmem    (1001)      575 2023-06-12 22:12:04.000000 MALDIpy-0.1.2/MALDIpy.egg-info/PKG-INFO
--rw-r--r--   0 hli       (1002) labmem    (1001)      441 2023-06-12 22:12:04.000000 MALDIpy-0.1.2/MALDIpy.egg-info/SOURCES.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-06-12 22:12:04.000000 MALDIpy-0.1.2/MALDIpy.egg-info/dependency_links.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)       47 2023-06-12 22:12:04.000000 MALDIpy-0.1.2/MALDIpy.egg-info/entry_points.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        8 2023-06-12 22:12:04.000000 MALDIpy-0.1.2/MALDIpy.egg-info/top_level.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-04-04 21:25:43.000000 MALDIpy-0.1.2/MALDIpy.egg-info/zip-safe
--rw-r--r--   0 hli       (1002) labmem    (1001)      176 2023-04-04 21:15:37.000000 MALDIpy-0.1.2/MANIFEST.in
--rw-r--r--   0 hli       (1002) labmem    (1001)      575 2023-06-12 22:12:04.997632 MALDIpy-0.1.2/PKG-INFO
--rw-r--r--   0 hli       (1002) labmem    (1001)      139 2023-06-12 22:11:17.000000 MALDIpy-0.1.2/README.md
--rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.1.2/requirements.txt
--rw-r--r--   0 hli       (1002) labmem    (1001)       38 2023-06-12 22:12:04.997632 MALDIpy-0.1.2/setup.cfg
--rw-r--r--   0 hli       (1002) labmem    (1001)     1922 2023-06-10 02:02:43.000000 MALDIpy-0.1.2/setup.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:20:46.208704 MALDIpy-0.1.3/
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1062 2023-04-04 21:12:06.000000 MALDIpy-0.1.3/LICENSE
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:20:46.208704 MALDIpy-0.1.3/MALDIpy/
+-rw-r--r--   0 hli       (1002) labmem    (1001)      187 2023-06-12 22:20:25.000000 MALDIpy-0.1.3/MALDIpy/__init__.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     7607 2023-06-12 22:20:09.000000 MALDIpy-0.1.3/MALDIpy/featureplot.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     6599 2023-04-06 16:02:36.000000 MALDIpy-0.1.3/MALDIpy/msi_data.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     3084 2023-04-06 18:34:41.000000 MALDIpy-0.1.3/MALDIpy/multi_sample.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     6619 2023-06-10 01:50:57.000000 MALDIpy-0.1.3/MALDIpy/projection.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:20:46.208704 MALDIpy-0.1.3/MALDIpy/shell/
+-rw-r--r--   0 hli       (1002) labmem    (1001)       61 2023-04-04 21:15:37.000000 MALDIpy-0.1.3/MALDIpy/shell/__init__.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)      196 2023-04-04 21:15:37.000000 MALDIpy-0.1.3/MALDIpy/shell/usage.py
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1690 2023-04-06 13:55:22.000000 MALDIpy-0.1.3/MALDIpy/single_cell.py
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:20:46.208704 MALDIpy-0.1.3/MALDIpy/src/
+-rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.1.3/MALDIpy/src/temp.txt
+drwxr-xr-x   0 hli       (1002) labmem    (1001)        0 2023-06-12 22:20:46.208704 MALDIpy-0.1.3/MALDIpy.egg-info/
+-rw-r--r--   0 hli       (1002) labmem    (1001)      575 2023-06-12 22:20:46.000000 MALDIpy-0.1.3/MALDIpy.egg-info/PKG-INFO
+-rw-r--r--   0 hli       (1002) labmem    (1001)      441 2023-06-12 22:20:46.000000 MALDIpy-0.1.3/MALDIpy.egg-info/SOURCES.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-06-12 22:20:46.000000 MALDIpy-0.1.3/MALDIpy.egg-info/dependency_links.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)       47 2023-06-12 22:20:46.000000 MALDIpy-0.1.3/MALDIpy.egg-info/entry_points.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        8 2023-06-12 22:20:46.000000 MALDIpy-0.1.3/MALDIpy.egg-info/top_level.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)        1 2023-04-04 21:25:43.000000 MALDIpy-0.1.3/MALDIpy.egg-info/zip-safe
+-rw-r--r--   0 hli       (1002) labmem    (1001)      176 2023-04-04 21:15:37.000000 MALDIpy-0.1.3/MANIFEST.in
+-rw-r--r--   0 hli       (1002) labmem    (1001)      575 2023-06-12 22:20:46.208704 MALDIpy-0.1.3/PKG-INFO
+-rw-r--r--   0 hli       (1002) labmem    (1001)      139 2023-06-12 22:20:32.000000 MALDIpy-0.1.3/README.md
+-rw-r--r--   0 hli       (1002) labmem    (1001)        0 2023-04-04 21:12:06.000000 MALDIpy-0.1.3/requirements.txt
+-rw-r--r--   0 hli       (1002) labmem    (1001)       38 2023-06-12 22:20:46.208704 MALDIpy-0.1.3/setup.cfg
+-rw-r--r--   0 hli       (1002) labmem    (1001)     1922 2023-06-10 02:02:43.000000 MALDIpy-0.1.3/setup.py
```

### Comparing `MALDIpy-0.1.2/LICENSE` & `MALDIpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.2/MALDIpy/featureplot.py` & `MALDIpy-0.1.3/MALDIpy/featureplot.py`

 * *Files 2% similar despite different names*

```diff
@@ -173,15 +173,15 @@
     plt.axis('off')
     plt.tight_layout()
     return fig
 
 def plot2features_subset(msi_obj, feats, cmap, scale_auto=False,
                 max_num_1=41000, min_num_1=21000, 
                 max_num_2=50000, min_num_2=25000,
-                         figsize = [5,2.9],subset=[95,185,35,175]):
+                         subset=[95,185,35,175]):
     
     df1 = msi_obj.to_img_mtx(mz=feats[0],smooth=False).iloc[subset[0]:subset[1], subset[2]:subset[3]]
     df2 = msi_obj.to_img_mtx(mz=feats[1],smooth=False).iloc[subset[0]:subset[1], subset[2]:subset[3]]
 
     if scale_auto == True:
         min_num_1 = np.quantile(df1, 0.01)
         max_num_1 = np.quantile(df1, 0.99)
@@ -199,12 +199,11 @@
     img_combined = np.clip(img1 + img2, 0, 1)
 
     # Convert to 8-bit RGB for visualization
     img_combined_uint8 = (img_combined * 255).astype(np.uint8)
     img_pil = Image.fromarray(img_combined_uint8)
 
     fig, ax  = plt.subplots(1, 1, dpi = 400)
-    fig.set_figheight(figsize[1]); fig.set_figwidth(figsize[0])
     plt.imshow(img_pil)
     plt.axis('off')
     plt.tight_layout()
     return fig
```

### Comparing `MALDIpy-0.1.2/MALDIpy/msi_data.py` & `MALDIpy-0.1.3/MALDIpy/msi_data.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.2/MALDIpy/multi_sample.py` & `MALDIpy-0.1.3/MALDIpy/multi_sample.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.2/MALDIpy/projection.py` & `MALDIpy-0.1.3/MALDIpy/projection.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.2/MALDIpy/single_cell.py` & `MALDIpy-0.1.3/MALDIpy/single_cell.py`

 * *Files identical despite different names*

### Comparing `MALDIpy-0.1.2/MALDIpy.egg-info/PKG-INFO` & `MALDIpy-0.1.3/MALDIpy.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: MALDIpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: MALDI-MS data analysis at the single-cell level
 Home-page: https://github.com/TheHumphreysLab
 Author: Haikuo Li; Dian Li; Qiao Xuanyuan; Benjamin Humphreys
 Author-email: haikuolibio@gmail.com
 License: UNKNOWN
-Description: Updates in MALDIpy v0.1.2; compared to v0.1.1:
+Description: Updates in MALDIpy v0.1.3; compared to v0.1.1:
         
         New functions: MALDIpy.featureplot.plot2features; MALDIpy.featureplot.plot2features_subset
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `MALDIpy-0.1.2/PKG-INFO` & `MALDIpy-0.1.3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: MALDIpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: MALDI-MS data analysis at the single-cell level
 Home-page: https://github.com/TheHumphreysLab
 Author: Haikuo Li; Dian Li; Qiao Xuanyuan; Benjamin Humphreys
 Author-email: haikuolibio@gmail.com
 License: UNKNOWN
-Description: Updates in MALDIpy v0.1.2; compared to v0.1.1:
+Description: Updates in MALDIpy v0.1.3; compared to v0.1.1:
         
         New functions: MALDIpy.featureplot.plot2features; MALDIpy.featureplot.plot2features_subset
         
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `MALDIpy-0.1.2/setup.py` & `MALDIpy-0.1.3/setup.py`

 * *Files identical despite different names*

