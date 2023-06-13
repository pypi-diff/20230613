# Comparing `tmp/dream_river-0.0.5.tar.gz` & `tmp/dream_river-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dream_river-0.0.5.tar", last modified: Fri Jun  9 08:42:13 2023, max compression
+gzip compressed data, was "dream_river-0.0.6.tar", last modified: Tue Jun 13 08:23:25 2023, max compression
```

## Comparing `dream_river-0.0.5.tar` & `dream_river-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2023-06-09 08:42:13.541824 dream_river-0.0.5/
--rw-rw-rw-   0        0        0     1069 2023-06-09 04:31:46.000000 dream_river-0.0.5/LICENSE
--rw-rw-rw-   0        0        0     1090 2023-06-09 04:31:50.000000 dream_river-0.0.5/LICENSE.txt
--rw-rw-rw-   0        0        0     1413 2023-06-09 08:42:13.541824 dream_river-0.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      866 2023-06-09 08:10:52.000000 dream_river-0.0.5/README.rst
-drwxrwxrwx   0        0        0        0 2023-06-09 08:42:13.517822 dream_river-0.0.5/dream_river/
--rw-rw-rw-   0        0        0     7586 2023-06-09 08:30:13.000000 dream_river-0.0.5/dream_river/ML.py
--rw-rw-rw-   0        0        0      226 2023-06-09 04:57:22.000000 dream_river-0.0.5/dream_river/__init__.py
--rw-rw-rw-   0        0        0     7139 2023-06-09 02:19:03.000000 dream_river-0.0.5/dream_river/convertools.py
--rw-rw-rw-   0        0        0     4967 2023-06-09 04:20:55.000000 dream_river-0.0.5/dream_river/geobox.py
--rw-rw-rw-   0        0        0     7648 2023-06-09 08:30:08.000000 dream_river-0.0.5/dream_river/indices.py
--rw-rw-rw-   0        0        0    15124 2023-06-09 04:21:55.000000 dream_river-0.0.5/dream_river/plotimg.py
-drwxrwxrwx   0        0        0        0 2023-06-09 08:42:13.539823 dream_river-0.0.5/dream_river.egg-info/
--rw-rw-rw-   0        0        0     1413 2023-06-09 08:42:13.000000 dream_river-0.0.5/dream_river.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      360 2023-06-09 08:42:13.000000 dream_river-0.0.5/dream_river.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-09 08:42:13.000000 dream_river-0.0.5/dream_river.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      133 2023-06-09 08:42:13.000000 dream_river-0.0.5/dream_river.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-09 08:42:13.000000 dream_river-0.0.5/dream_river.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       86 2023-06-09 08:42:13.544824 dream_river-0.0.5/setup.cfg
--rw-rw-rw-   0        0        0     1773 2023-06-09 08:41:36.000000 dream_river-0.0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:23:25.328014 dream_river-0.0.6/
+-rw-rw-rw-   0        0        0     1069 2023-06-09 04:31:46.000000 dream_river-0.0.6/LICENSE
+-rw-rw-rw-   0        0        0     1090 2023-06-09 04:31:50.000000 dream_river-0.0.6/LICENSE.txt
+-rw-rw-rw-   0        0        0     1413 2023-06-13 08:23:25.328014 dream_river-0.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      866 2023-06-09 08:10:52.000000 dream_river-0.0.6/README.rst
+drwxrwxrwx   0        0        0        0 2023-06-13 08:23:25.294487 dream_river-0.0.6/dream_river/
+-rw-rw-rw-   0        0        0     8516 2023-06-13 08:14:56.000000 dream_river-0.0.6/dream_river/ML.py
+-rw-rw-rw-   0        0        0      226 2023-06-09 04:57:22.000000 dream_river-0.0.6/dream_river/__init__.py
+-rw-rw-rw-   0        0        0     7139 2023-06-13 08:17:08.000000 dream_river-0.0.6/dream_river/convertools.py
+-rw-rw-rw-   0        0        0     4967 2023-06-09 04:20:55.000000 dream_river-0.0.6/dream_river/geobox.py
+-rw-rw-rw-   0        0        0     7648 2023-06-09 08:30:08.000000 dream_river-0.0.6/dream_river/indices.py
+-rw-rw-rw-   0        0        0    15124 2023-06-09 04:21:55.000000 dream_river-0.0.6/dream_river/plotimg.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:23:25.326379 dream_river-0.0.6/dream_river.egg-info/
+-rw-rw-rw-   0        0        0     1413 2023-06-13 08:23:25.000000 dream_river-0.0.6/dream_river.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      360 2023-06-13 08:23:25.000000 dream_river-0.0.6/dream_river.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 08:23:25.000000 dream_river-0.0.6/dream_river.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      133 2023-06-13 08:23:25.000000 dream_river-0.0.6/dream_river.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 08:23:25.000000 dream_river-0.0.6/dream_river.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       86 2023-06-13 08:23:25.330011 dream_river-0.0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1773 2023-06-13 08:15:59.000000 dream_river-0.0.6/setup.py
```

### Comparing `dream_river-0.0.5/LICENSE` & `dream_river-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.5/LICENSE.txt` & `dream_river-0.0.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.5/PKG-INFO` & `dream_river-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dream_river
-Version: 0.0.5
+Version: 0.0.6
 Summary: This is a library contained rice detection tools and other geospatial tools for jupyter environment on sphere.gistda.or.th in part of Data Cube
 Home-page: https://github.com/Pathakorn40/rice-detection
 Author: Pathakorn Usaha
 Author-email: dreamusaha@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/dream_river/
 Keywords: geography,geospatiol,gis,rice detection
```

### Comparing `dream_river-0.0.5/README.rst` & `dream_river-0.0.6/README.rst`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.5/dream_river/ML.py` & `dream_river-0.0.6/dream_river/ML.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,30 +9,31 @@
 import geopandas as gpd
 import matplotlib.pyplot as plt
 from io import StringIO
 from odc.io.cgroups import get_cpu_quota
 from sklearn.ensemble import RandomForestClassifier
 from sklearn import model_selection
 from sklearn.metrics import accuracy_score
+from IPython.display import Image
 from datacube.utils import geometry
 from datacube.utils.cog import write_cog
 from dea_tools.classification import collect_training_data, predict_xr
-
+from dea_tools.bandindices import calculate_indices
 from convertools import vectorize
 import warnings
 warnings.filterwarnings("ignore")
 
 def custom_loadband(query):
 
     # Initialise datacube
     dc = datacube.Datacube(app='extract_VI')
 
     # Load data using query
     dd = dc.load(**query)
-    
+
     # band index
     dd['NDVI']=(dd.nir - dd.red)/(dd.nir + dd.red)
     dd['GNDVI']=(dd.nir - dd.green)/(dd.nir + dd.green)
     dd['EVI']=((2.5 * (dd.nir - dd.red))/(dd.nir + 6 * dd.red -7.5 * dd.blue + 1))
     dd['SAVI']=((1.5 * (dd.nir - dd.red))/(dd.nir + dd.red + 0.5))
     dd['NDWI']=(dd.green - dd.nir)/(dd.green + dd.nir)
 
@@ -48,15 +49,15 @@
     
     # band index
     ds['NDVI']=(ds.nir - ds.red)/(ds.nir + ds.red)
     ds['GNDVI']=(ds.nir - ds.green)/(ds.nir + ds.green)
     ds['EVI']=((2.5 * (ds.nir - ds.red))/(ds.nir + 6 * ds.red -7.5 * ds.blue + 1))
     ds['SAVI']=((1.5 * (ds.nir - ds.red))/(ds.nir + ds.red + 0.5))
     ds['NDWI']=(ds.green - ds.nir)/(ds.green + ds.nir)
-    
+
     return ds
 
 def rice_detect(ds, product, outname_raster, outname_vector, query, field):
     
     ######### Part create Training data ############################################## 
     
     # create polygon 
@@ -70,45 +71,50 @@
     
     # Extract data using shapfile(polygon)
     column_names, model_input = collect_training_data(gdf=input_data,
                                                       dc_query=query,
                                                       ncpus=ncpus,
                                                       feature_func=custom_loadband,
                                                       field=field,
-                                                      zonal_stats='mean')
+                                                      zonal_stats='median')
     
     ########### preprocessing training data ##########################################
-    print(column_names)
-   
+    print('column_name of training data:',column_names)
+  
     # Create a DataFrame from model_input
     df = pd.DataFrame(model_input, columns=column_names)
 
     # Create a GeoDataFrame from the DataFrame
     gdf = gpd.GeoDataFrame(df)
     
+    input_column_names = ['values', 'NDVI','GNDVI', 'EVI', 'SAVI', 'NDWI']
+    df = df[input_column_names]
+
+    print(df)
+    
     # Define the query conditions
-    ndvi_condition = (df['NDVI'].between(0.4, 0.65))
-    gndvi_condition = (df['GNDVI'].between(0.4, 0.8))
-    savi_condition = (df['SAVI'].between(0.4, 0.6))
-    evi_condition = (df['EVI'].between(0.2, 0.8))
-    ndwi_condition = (df['NDWI'].between(-0.5, -0.26))
+    ndvi_condition = (df['NDVI'].between(0.6, 0.9))
+    gndvi_condition = (df['GNDVI'].between(0.28, 0.368))
+    savi_condition = (df['SAVI'].between(0.256, 0.648))
+    evi_condition = (df['EVI'].between(0.4, 0.8))
+    ndwi_condition = (df['NDWI'].between(-0.55,-0.267))
  
-
-
     # Modify the input training data for single class labels
-    model_input[:, 0] = np.where((ndvi_condition & (savi_condition|evi_condition|gndvi_condition)), 1, 0)
+    model_input[:, 0] = np.where((ndvi_condition & ~(ndwi_condition|gndvi_condition|savi_condition )) ,1 ,0) 
+    #& (savi_condition|gndvi_condition|ndwi_condition)
     
+    # convert model_input to dataframe
+    df2 = pd.DataFrame(model_input, columns=column_names)
     
-
-    # to check parameter as input
-    A = gdf.describe()
-    print(A)
-
+    model_input = df2[input_column_names].values
     
-    # Split into training and testing data (trai80/test20)
+    # print(model_input[:, 0])
+    # print(input_column_names)
+    
+    # Split into training and testing data (train80/test20)
     model_train, model_test = model_selection.train_test_split(model_input, 
                                                                stratify=model_input[:, 0], 
                                                                train_size=0.7, 
                                                                random_state=0)
     print('#'*40)
     print("Train shape(70%):", model_train.shape)
     print("Test shape(30%):", model_test.shape)
@@ -117,29 +123,29 @@
     
     # Convert model_train to a NumPy array
     model_train_array = model_train
     model_test_array = model_test
     ############## Model preparation #################################################
 
     # Select the variables we want to use to train our model
-    model_variables = [col for col in column_names if col not in ["values"]]
+    model_variables = [col for col in input_column_names if col not in ["values"]]
     
     print('The variables for Training Model :', model_variables)
     
     # Extract relevant indices from the processed shapefile
-    model_col_indices = [column_names.index(var_name) for var_name in model_variables]
+    model_col_indices = [input_column_names.index(var_name) for var_name in model_variables]
     
     # Initialise model
-    model = RandomForestClassifier(n_estimators=50)
+    model = RandomForestClassifier(n_estimators=500)
     
     print("Initial call RF ML")
     ####################### Train Model/ predict #############################################
     
     # Train model
-    model.fit(model_train_array[:, model_col_indices], model_train_array[:, column_names.index('values')])
+    model.fit(model_train_array[:, model_col_indices], model_train_array[:, input_column_names.index('values')])
     
     # Predict data
     predictions = model.predict( model_test_array[:, model_col_indices])
     
     print('Training Model!!!')
     
     # show the accuracy of prediction
@@ -147,15 +153,16 @@
     print('The accuracy of model is :',acc)
     
     # This shows the feature importance of the input features for predicting the class labels provided
     plt.bar(x=model_variables, height=model.feature_importances_)
     plt.gca().set_ylabel('Importance', labelpad=10)
     plt.gca().set_xlabel('Variable', labelpad=10);
     
-    
+######################## classify #################################################
+
     shape = input_data
     
     # Compute the bounding box of the union of all geometries in shp
     xmin, ymin, xmax, ymax = shape.unary_union.bounds
     
     # Convert bounding box coordinates to decimal degrees
     gdf_crs_decimal_degrees = shape.to_crs("EPSG:4326")
@@ -178,28 +185,42 @@
     
     
     
     # Use custom function to generate input data
     input_data = custom_function(product,query=query2)
     
     
+    input_data2 = input_data[['NDVI','GNDVI', 'EVI', 'SAVI', 'NDWI']]
+    
+    print(input_data2)
+    
+
     # Predict landcover using the trained model
-    predicted = predict_xr(model, input_data, clean=True)
+    predicted = predict_xr(model, input_data2, clean=True)
     
     print('predicted!!!')
+    
+#################################
+#     print('*'*60)
 
+#     # Calculate accuracy
+#     # acc = accuracy_score(predicted.values, input_data2.values)
+#     # print('The accuracy of the classification result is:', acc)
+    
+#     print('*'*60)
     
 #################################### Plot output ############################################## 
- 
+    # print(predicted.Predictions)
+    
     # Set up plot
-    fig, axes = plt.subplots(1, 2, figsize=(14, 6))
+    fig, axes = plt.subplots(1, 2, figsize=(15, 6))
 
     # Plot classified image
     predicted.Predictions.plot(ax=axes[0], 
-                   cmap='Greens', 
+                   cmap='Reds', 
                    add_labels=False, 
                    add_colorbar=False)
 
     # Plot true colour image
     (input_data[['red', 'green', 'blue']]
      .squeeze('time')
      .to_array()
```

### Comparing `dream_river-0.0.5/dream_river/convertools.py` & `dream_river-0.0.6/dream_river/convertools.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,16 +29,16 @@
     # Convert our mean index xarray into a numpy array, we need
     # to be explicit about the datatype to satisfy felzenszwalb
     input_array = VI.values.astype(np.float64)
     
     # Calculate the segments (image segmentation)
     segments = felzenszwalb(input_array, 
                              scale=1, 
-                             sigma=0.5, 
-                             min_size=90, 
+                             sigma=0.8, 
+                             min_size=50, 
                              channel_axis=-1)
     
     # Calculate the zonal mean index across the segments
     segments_zonal_mean_qs = scipy.ndimage.mean(input=input_array,
                                                 labels=segments,
                                                 index=segments)
```

### Comparing `dream_river-0.0.5/dream_river/geobox.py` & `dream_river-0.0.6/dream_river/geobox.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.5/dream_river/indices.py` & `dream_river-0.0.6/dream_river/indices.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.5/dream_river/plotimg.py` & `dream_river-0.0.6/dream_river/plotimg.py`

 * *Files identical despite different names*

### Comparing `dream_river-0.0.5/dream_river.egg-info/PKG-INFO` & `dream_river-0.0.6/dream_river.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dream-river
-Version: 0.0.5
+Version: 0.0.6
 Summary: This is a library contained rice detection tools and other geospatial tools for jupyter environment on sphere.gistda.or.th in part of Data Cube
 Home-page: https://github.com/Pathakorn40/rice-detection
 Author: Pathakorn Usaha
 Author-email: dreamusaha@gmail.com
 License: MIT
 Download-URL: https://pypi.org/project/dream_river/
 Keywords: geography,geospatiol,gis,rice detection
```

### Comparing `dream_river-0.0.5/setup.py` & `dream_river-0.0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 DESC ='This is a library that contain rice cultivated area detection tools and other geospatial tools for jupyter environment on https://sphere.gistda.or.th/ in part of Data Cube. Thus, you needs go to sphere.gistda (https://sphere.gistda.or.th/) and register the account to access jupyter lab environment interactively from a browser.'
 
 setup(
     name='dream_river',
     packages=['dream_river'],
-    version='0.0.5',
+    version='0.0.6',
     license='MIT',
     author_email='dreamusaha@gmail.com',
     description= 'This is a library contained rice detection tools and other geospatial tools for jupyter environment on sphere.gistda.or.th in part of Data Cube',
     long_description= DESC,
     author='Pathakorn Usaha',
     url= 'https://github.com/Pathakorn40/rice-detection',
     download_url= 'https://pypi.org/project/dream_river/',
```

