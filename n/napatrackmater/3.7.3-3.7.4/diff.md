# Comparing `tmp/napatrackmater-3.7.3.tar.gz` & `tmp/napatrackmater-3.7.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-07gw48r1/napatrackmater-3.7.3.tar", last modified: Mon Jun 12 14:14:09 2023, max compression
+gzip compressed data, was "/mnt/c/Users/rando/Downloads/Python_Workspace/NapaTrackMater/dist/.tmp-1x1ogdc2/napatrackmater-3.7.4.tar", last modified: Tue Jun 13 21:46:22 2023, max compression
```

## Comparing `napatrackmater-3.7.3.tar` & `napatrackmater-3.7.4.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 14:14:09.765534 napatrackmater-3.7.3/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.7.3/LICENSE
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-12 14:14:09.761533 napatrackmater-3.7.3/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.7.3/README.md
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 14:14:09.589459 napatrackmater-3.7.3/napatrackmater/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.7.3/napatrackmater/CloudAutoEncoder.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.7.3/napatrackmater/DeepEmbeddedClustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.7.3/napatrackmater/Trackmate.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.7.3/napatrackmater/Trackvector.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.7.3/napatrackmater/__init__.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13407 2023-06-12 14:11:53.000000 napatrackmater-3.7.3/napatrackmater/clustering.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.7.3/napatrackmater/fast_radius_regression.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.7.3/napatrackmater/fate_mapping.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.7.3/napatrackmater/pretrained.py
--rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-12 14:13:48.000000 napatrackmater-3.7.3/napatrackmater/version.py
-drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-12 14:14:09.736240 napatrackmater-3.7.3/napatrackmater.egg-info/
--rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-12 14:14:08.000000 napatrackmater-3.7.3/napatrackmater.egg-info/PKG-INFO
--rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-12 14:14:09.000000 napatrackmater-3.7.3/napatrackmater.egg-info/SOURCES.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-12 14:14:08.000000 napatrackmater-3.7.3/napatrackmater.egg-info/dependency_links.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-12 14:14:08.000000 napatrackmater-3.7.3/napatrackmater.egg-info/entry_points.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-12 14:14:08.000000 napatrackmater-3.7.3/napatrackmater.egg-info/requires.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-12 14:14:08.000000 napatrackmater-3.7.3/napatrackmater.egg-info/top_level.txt
--rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-12 14:14:09.766531 napatrackmater-3.7.3/setup.cfg
--rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.7.3/setup.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-13 21:46:22.518399 napatrackmater-3.7.4/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1541 2023-02-25 13:00:46.000000 napatrackmater-3.7.4/LICENSE
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-13 21:46:22.513579 napatrackmater-3.7.4/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2276 2023-02-25 13:36:08.000000 napatrackmater-3.7.4/README.md
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-13 21:46:22.318125 napatrackmater-3.7.4/napatrackmater/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1261 2023-06-02 10:49:22.000000 napatrackmater-3.7.4/napatrackmater/CloudAutoEncoder.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      887 2023-06-02 10:42:27.000000 napatrackmater-3.7.4/napatrackmater/DeepEmbeddedClustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)   110394 2023-06-11 19:02:37.000000 napatrackmater-3.7.4/napatrackmater/Trackmate.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    16848 2023-04-23 10:20:11.000000 napatrackmater-3.7.4/napatrackmater/Trackvector.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1723 2023-06-11 17:28:48.000000 napatrackmater-3.7.4/napatrackmater/__init__.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13565 2023-06-13 21:44:31.000000 napatrackmater-3.7.4/napatrackmater/clustering.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     3675 2023-04-23 07:54:27.000000 napatrackmater-3.7.4/napatrackmater/fast_radius_regression.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)    13011 2023-04-23 09:37:34.000000 napatrackmater-3.7.4/napatrackmater/fate_mapping.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     6008 2023-06-02 10:44:48.000000 napatrackmater-3.7.4/napatrackmater/pretrained.py
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       25 2023-06-13 21:46:06.000000 napatrackmater-3.7.4/napatrackmater/version.py
+drwxrwxrwx   0 debian    (1000) debian    (1000)        0 2023-06-13 21:46:22.486838 napatrackmater-3.7.4/napatrackmater.egg-info/
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     2816 2023-06-13 21:46:21.000000 napatrackmater-3.7.4/napatrackmater.egg-info/PKG-INFO
+-rwxrwxrwx   0 debian    (1000) debian    (1000)      573 2023-06-13 21:46:21.000000 napatrackmater-3.7.4/napatrackmater.egg-info/SOURCES.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)        1 2023-06-13 21:46:21.000000 napatrackmater-3.7.4/napatrackmater.egg-info/dependency_links.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       55 2023-06-13 21:46:21.000000 napatrackmater-3.7.4/napatrackmater.egg-info/entry_points.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       57 2023-06-13 21:46:21.000000 napatrackmater-3.7.4/napatrackmater.egg-info/requires.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       15 2023-06-13 21:46:21.000000 napatrackmater-3.7.4/napatrackmater.egg-info/top_level.txt
+-rwxrwxrwx   0 debian    (1000) debian    (1000)       38 2023-06-13 21:46:22.519400 napatrackmater-3.7.4/setup.cfg
+-rwxrwxrwx   0 debian    (1000) debian    (1000)     1325 2023-06-11 13:21:48.000000 napatrackmater-3.7.4/setup.py
```

### Comparing `napatrackmater-3.7.3/LICENSE` & `napatrackmater-3.7.4/LICENSE`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.3/PKG-INFO` & `napatrackmater-3.7.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.7.3
+Version: 3.7.4
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.7.3/README.md` & `napatrackmater-3.7.4/README.md`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.3/napatrackmater/CloudAutoEncoder.py` & `napatrackmater-3.7.4/napatrackmater/CloudAutoEncoder.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.3/napatrackmater/DeepEmbeddedClustering.py` & `napatrackmater-3.7.4/napatrackmater/DeepEmbeddedClustering.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.3/napatrackmater/Trackmate.py` & `napatrackmater-3.7.4/napatrackmater/Trackmate.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.3/napatrackmater/Trackvector.py` & `napatrackmater-3.7.4/napatrackmater/Trackvector.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.3/napatrackmater/__init__.py` & `napatrackmater-3.7.4/napatrackmater/__init__.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.3/napatrackmater/clustering.py` & `napatrackmater-3.7.4/napatrackmater/clustering.py`

 * *Files 1% similar despite different names*

```diff
@@ -157,18 +157,21 @@
        properties = regionprops(label_image)
        futures = []
        with concurrent.futures.ThreadPoolExecutor(max_workers = nthreads) as executor:
              for prop in properties:
                           futures.append(executor.submit(get_current_label_binary, prop))
              for r in concurrent.futures.as_completed(futures):
                         binary_image, label, centroid = r.result()             
-                        label, centroid, cloud = get_label_centroid_cloud(binary_image,  num_points, ndim, label, centroid,  min_size)
-                        clouds.append(cloud)  
-                        labels.append(label)   
-                        centroids.append(centroid)
+                        results = get_label_centroid_cloud(binary_image,  num_points, ndim, label, centroid,  min_size)
+                        
+                        if results is not None:
+                                label, centroid, cloud = results
+                                clouds.append(cloud)  
+                                labels.append(label)   
+                                centroids.append(centroid)
 
        return labels, centroids, clouds
 
 def get_label_centroid_cloud(binary_image,  num_points, ndim, label, centroid, min_size):
                             
                             valid = []  
                              
@@ -201,15 +204,15 @@
                                     if ndim == 2:
                                       cloud = get_panda_cloud_xy(points)
                                     if ndim == 3:
                                       cloud = get_panda_cloud_xyz(points)  
                                     else:
                                       cloud = get_panda_cloud_xyz(points)    
                                      
-                            return  label, centroid, cloud       
+                                    return  label, centroid, cloud       
        
 
 def get_panda_cloud_xy(points):
         
         cloud = PyntCloud(pd.DataFrame(data=points, columns=["x", "y"]))
 
         return cloud
```

### Comparing `napatrackmater-3.7.3/napatrackmater/fast_radius_regression.py` & `napatrackmater-3.7.4/napatrackmater/fast_radius_regression.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.3/napatrackmater/fate_mapping.py` & `napatrackmater-3.7.4/napatrackmater/fate_mapping.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.3/napatrackmater/pretrained.py` & `napatrackmater-3.7.4/napatrackmater/pretrained.py`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.3/napatrackmater.egg-info/PKG-INFO` & `napatrackmater-3.7.4/napatrackmater.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napatrackmater
-Version: 3.7.3
+Version: 3.7.4
 Summary: Import Trackmate XML files for Track Visualization and analysis in Napari.
 Home-page: https://github.com/kapoorlab/NapaTrackMater/
 Author: Varun Kapoor, Mari Tolonen
 Author-email: randomaccessiblekapoor@gmail.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `napatrackmater-3.7.3/napatrackmater.egg-info/SOURCES.txt` & `napatrackmater-3.7.4/napatrackmater.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `napatrackmater-3.7.3/setup.py` & `napatrackmater-3.7.4/setup.py`

 * *Files identical despite different names*

