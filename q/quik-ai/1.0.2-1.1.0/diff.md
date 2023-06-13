# Comparing `tmp/quik-ai-1.0.2.tar.gz` & `tmp/quik-ai-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quik-ai-1.0.2.tar", last modified: Sun Jun 11 11:02:00 2023, max compression
+gzip compressed data, was "quik-ai-1.1.0.tar", last modified: Mon Jun 12 22:25:55 2023, max compression
```

## Comparing `quik-ai-1.0.2.tar` & `quik-ai-1.1.0.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-06-11 11:02:00.979385 quik-ai-1.0.2/
--rw-rw-rw-   0        0        0    11554 2023-06-07 20:40:55.000000 quik-ai-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     2262 2023-06-11 11:02:00.980392 quik-ai-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1724 2023-06-10 03:32:27.000000 quik-ai-1.0.2/README.md
--rw-rw-rw-   0        0        0       97 2023-05-29 14:14:26.000000 quik-ai-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0      768 2023-06-11 11:02:00.983373 quik-ai-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      289 2023-06-09 23:06:08.000000 quik-ai-1.0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-11 11:02:00.814022 quik-ai-1.0.2/src/
-drwxrwxrwx   0        0        0        0 2023-06-11 11:02:00.949697 quik-ai-1.0.2/src/quik_ai/
--rw-rw-rw-   0        0        0      429 2023-06-09 00:21:28.000000 quik-ai-1.0.2/src/quik_ai/__init__.py
--rw-rw-rw-   0        0        0     2437 2023-06-11 01:06:26.000000 quik-ai-1.0.2/src/quik_ai/backend.py
--rw-rw-rw-   0        0        0    10544 2023-06-11 11:01:12.000000 quik-ai-1.0.2/src/quik_ai/engine.py
--rw-rw-rw-   0        0        0     4917 2023-06-07 22:39:50.000000 quik-ai-1.0.2/src/quik_ai/heads.py
--rw-rw-rw-   0        0        0    18541 2023-06-08 20:45:11.000000 quik-ai-1.0.2/src/quik_ai/layers.py
--rw-rw-rw-   0        0        0      940 2023-06-07 22:39:39.000000 quik-ai-1.0.2/src/quik_ai/losses.py
--rw-rw-rw-   0        0        0     1291 2023-06-10 01:46:43.000000 quik-ai-1.0.2/src/quik_ai/metrics.py
--rw-rw-rw-   0        0        0    29903 2023-06-10 15:57:06.000000 quik-ai-1.0.2/src/quik_ai/models.py
--rw-rw-rw-   0        0        0     1633 2023-06-06 23:57:01.000000 quik-ai-1.0.2/src/quik_ai/optimizers.py
--rw-rw-rw-   0        0        0     8204 2023-06-11 01:25:52.000000 quik-ai-1.0.2/src/quik_ai/predictors.py
--rw-rw-rw-   0        0        0     9621 2023-06-08 21:13:03.000000 quik-ai-1.0.2/src/quik_ai/tuners.py
--rw-rw-rw-   0        0        0     3344 2023-06-10 16:18:42.000000 quik-ai-1.0.2/src/quik_ai/tuning.py
-drwxrwxrwx   0        0        0        0 2023-06-11 11:02:00.978382 quik-ai-1.0.2/src/quik_ai.egg-info/
--rw-rw-rw-   0        0        0     2262 2023-06-11 11:02:00.000000 quik-ai-1.0.2/src/quik_ai.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      500 2023-06-11 11:02:00.000000 quik-ai-1.0.2/src/quik_ai.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-11 11:02:00.000000 quik-ai-1.0.2/src/quik_ai.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      109 2023-06-11 11:02:00.000000 quik-ai-1.0.2/src/quik_ai.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-06-11 11:02:00.000000 quik-ai-1.0.2/src/quik_ai.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-12 22:25:55.003455 quik-ai-1.1.0/
+-rw-rw-rw-   0        0        0    11554 2023-06-07 20:40:55.000000 quik-ai-1.1.0/LICENSE
+-rw-rw-rw-   0        0        0     2235 2023-06-12 22:25:55.004459 quik-ai-1.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1697 2023-06-11 13:33:07.000000 quik-ai-1.1.0/README.md
+-rw-rw-rw-   0        0        0       97 2023-05-29 14:14:26.000000 quik-ai-1.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0      768 2023-06-12 22:25:55.007446 quik-ai-1.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      289 2023-06-09 23:06:08.000000 quik-ai-1.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:25:54.856707 quik-ai-1.1.0/src/
+drwxrwxrwx   0        0        0        0 2023-06-12 22:25:54.972538 quik-ai-1.1.0/src/quik_ai/
+-rw-rw-rw-   0        0        0      429 2023-06-09 00:21:28.000000 quik-ai-1.1.0/src/quik_ai/__init__.py
+-rw-rw-rw-   0        0        0     2440 2023-06-11 23:04:01.000000 quik-ai-1.1.0/src/quik_ai/backend.py
+-rw-rw-rw-   0        0        0    11500 2023-06-12 22:23:55.000000 quik-ai-1.1.0/src/quik_ai/engine.py
+-rw-rw-rw-   0        0        0     4917 2023-06-07 22:39:50.000000 quik-ai-1.1.0/src/quik_ai/heads.py
+-rw-rw-rw-   0        0        0    18541 2023-06-08 20:45:11.000000 quik-ai-1.1.0/src/quik_ai/layers.py
+-rw-rw-rw-   0        0        0      940 2023-06-07 22:39:39.000000 quik-ai-1.1.0/src/quik_ai/losses.py
+-rw-rw-rw-   0        0        0     1291 2023-06-10 01:46:43.000000 quik-ai-1.1.0/src/quik_ai/metrics.py
+-rw-rw-rw-   0        0        0    29800 2023-06-12 22:25:24.000000 quik-ai-1.1.0/src/quik_ai/models.py
+-rw-rw-rw-   0        0        0     1633 2023-06-06 23:57:01.000000 quik-ai-1.1.0/src/quik_ai/optimizers.py
+-rw-rw-rw-   0        0        0     8255 2023-06-12 21:22:26.000000 quik-ai-1.1.0/src/quik_ai/predictors.py
+-rw-rw-rw-   0        0        0     9621 2023-06-08 21:13:03.000000 quik-ai-1.1.0/src/quik_ai/tuners.py
+-rw-rw-rw-   0        0        0     3344 2023-06-10 16:18:42.000000 quik-ai-1.1.0/src/quik_ai/tuning.py
+drwxrwxrwx   0        0        0        0 2023-06-12 22:25:55.001459 quik-ai-1.1.0/src/quik_ai.egg-info/
+-rw-rw-rw-   0        0        0     2235 2023-06-12 22:25:54.000000 quik-ai-1.1.0/src/quik_ai.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      500 2023-06-12 22:25:54.000000 quik-ai-1.1.0/src/quik_ai.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-12 22:25:54.000000 quik-ai-1.1.0/src/quik_ai.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      109 2023-06-12 22:25:54.000000 quik-ai-1.1.0/src/quik_ai.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-12 22:25:54.000000 quik-ai-1.1.0/src/quik_ai.egg-info/top_level.txt
```

### Comparing `quik-ai-1.0.2/LICENSE` & `quik-ai-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.2/PKG-INFO` & `quik-ai-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quik-ai
-Version: 1.0.2
+Version: 1.1.0
 Summary: Quick Unifying Infrastructure Kit for Machine Learning and AI
 Home-page: https://github.com/touzov1012/quik-ai
-Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.0.2.tar.gz
+Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.1.0.tar.gz
 Author: Aleksandr Touzov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -32,17 +32,17 @@
 head = qa.heads.GaussianMixture()
 ```
 
 3. Specify the predictors used for model fitting.
 ```python
 # All the predictors for the model.
 predictors = [
-    qa.predictors.NumericalPredictor('numerical'),
-    qa.predictors.CategoricalPredictor('categorical'),
-    qa.predictors.PeriodicPredictor('periodic', 24.0),
+    qa.predictors.Numerical('numerical'),
+    qa.predictors.Categorical('categorical'),
+    qa.predictors.Periodic('periodic', 24.0),
 ]
 ```
 
 4. Select the model architecture.
 ```python
 # Select the architecture and feed the response column, and other
 # necessary data for training, testing the model.
```

### Comparing `quik-ai-1.0.2/README.md` & `quik-ai-1.1.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 head = qa.heads.GaussianMixture()
 ```
 
 3. Specify the predictors used for model fitting.
 ```python
 # All the predictors for the model.
 predictors = [
-    qa.predictors.NumericalPredictor('numerical'),
-    qa.predictors.CategoricalPredictor('categorical'),
-    qa.predictors.PeriodicPredictor('periodic', 24.0),
+    qa.predictors.Numerical('numerical'),
+    qa.predictors.Categorical('categorical'),
+    qa.predictors.Periodic('periodic', 24.0),
 ]
 ```
 
 4. Select the model architecture.
 ```python
 # Select the architecture and feed the response column, and other
 # necessary data for training, testing the model.
```

### Comparing `quik-ai-1.0.2/setup.cfg` & `quik-ai-1.1.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2071 7569 6b2d 6169 0d0a 7665 7273   = quik-ai..vers
-00000020: 696f 6e20 3d20 312e 302e 320d 0a61 7574  ion = 1.0.2..aut
+00000020: 696f 6e20 3d20 312e 312e 300d 0a61 7574  ion = 1.1.0..aut
 00000030: 686f 7220 3d20 416c 656b 7361 6e64 7220  hor = Aleksandr 
 00000040: 546f 757a 6f76 0d0a 6465 7363 7269 7074  Touzov..descript
 00000050: 696f 6e20 3d20 5175 6963 6b20 556e 6966  ion = Quick Unif
 00000060: 7969 6e67 2049 6e66 7261 7374 7275 6374  ying Infrastruct
 00000070: 7572 6520 4b69 7420 666f 7220 4d61 6368  ure Kit for Mach
 00000080: 696e 6520 4c65 6172 6e69 6e67 2061 6e64  ine Learning and
 00000090: 2041 490d 0a6c 6f6e 675f 6465 7363 7269   AI..long_descri
@@ -15,16 +15,16 @@
 000000e0: 726b 646f 776e 0d0a 7572 6c20 3d20 6874  rkdown..url = ht
 000000f0: 7470 733a 2f2f 6769 7468 7562 2e63 6f6d  tps://github.com
 00000100: 2f74 6f75 7a6f 7631 3031 322f 7175 696b  /touzov1012/quik
 00000110: 2d61 690d 0a64 6f77 6e6c 6f61 645f 7572  -ai..download_ur
 00000120: 6c20 3d20 6874 7470 733a 2f2f 6769 7468  l = https://gith
 00000130: 7562 2e63 6f6d 2f74 6f75 7a6f 7631 3031  ub.com/touzov101
 00000140: 322f 7175 696b 2d61 692f 6172 6368 6976  2/quik-ai/archiv
-00000150: 652f 7265 6673 2f74 6167 732f 7631 2e30  e/refs/tags/v1.0
-00000160: 2e32 2e74 6172 2e67 7a0d 0a63 6c61 7373  .2.tar.gz..class
+00000150: 652f 7265 6673 2f74 6167 732f 7631 2e31  e/refs/tags/v1.1
+00000160: 2e30 2e74 6172 2e67 7a0d 0a63 6c61 7373  .0.tar.gz..class
 00000170: 6966 6965 7273 203d 200d 0a09 5072 6f67  ifiers = ...Prog
 00000180: 7261 6d6d 696e 6720 4c61 6e67 7561 6765  ramming Language
 00000190: 203a 3a20 5079 7468 6f6e 203a 3a20 330d   :: Python :: 3.
 000001a0: 0a09 4c69 6365 6e73 6520 3a3a 204f 5349  ..License :: OSI
 000001b0: 2041 7070 726f 7665 6420 3a3a 2041 7061   Approved :: Apa
 000001c0: 6368 6520 536f 6674 7761 7265 204c 6963  che Software Lic
 000001d0: 656e 7365 0d0a 094f 7065 7261 7469 6e67  ense...Operating
```

### Comparing `quik-ai-1.0.2/src/quik_ai/backend.py` & `quik-ai-1.1.0/src/quik_ai/backend.py`

 * *Files 3% similar despite different names*

```diff
@@ -65,15 +65,17 @@
     return new_df
 
 def get_k_from_end(data, k, fill=0):
     rows = len(data)
     if rows >= k:
         return data[-k:]
     else:
-        pad_rows = np.full((k-rows, data.shape[1]), fill) if len(data.shape) > 1 else np.full((k-rows,), fill)
+        fill_shape = list(data.shape)
+        fill_shape[0] = k-rows
+        pad_rows = np.full(fill_shape, fill)
         return np.concatenate((pad_rows, data), axis=0)
 
 def train_val_test_split(df, p=[0.8,0.1,0.1]):
     
     n0 = int(df.shape[0] * p[0])
     n1 = int(df.shape[0] * (p[0] + p[1]))
     n2 = int(df.shape[0] * (p[0] + p[1] + p[2]))
```

### Comparing `quik-ai-1.0.2/src/quik_ai/heads.py` & `quik-ai-1.1.0/src/quik_ai/heads.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.2/src/quik_ai/layers.py` & `quik-ai-1.1.0/src/quik_ai/layers.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.2/src/quik_ai/losses.py` & `quik-ai-1.1.0/src/quik_ai/losses.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.2/src/quik_ai/metrics.py` & `quik-ai-1.1.0/src/quik_ai/metrics.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.2/src/quik_ai/models.py` & `quik-ai-1.1.0/src/quik_ai/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,19 +118,15 @@
     def __build_input_layers(self, time_window, **kwargs):
         input_layers = {}
         
         input_names = self.get_input_names()
         
         for name in input_names:
             dtype = self.driver.get_input_dtype(name)
-            shape = self.driver.get_input_shape(name)
-
-            # append time dimension
-            if time_window > 1:
-                shape = (time_window,) + shape
+            shape = self.driver.get_input_shape(name, time_window)
 
             input_layers[name] = tf.keras.Input(name=name, dtype=dtype, shape=shape)
         
         return input_layers
     
     def __build_input_tensor(self, hp, input_layers, time_window, time_dropout, seed, **kwargs):
```

### Comparing `quik-ai-1.0.2/src/quik_ai/optimizers.py` & `quik-ai-1.1.0/src/quik_ai/optimizers.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.2/src/quik_ai/predictors.py` & `quik-ai-1.1.0/src/quik_ai/predictors.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     def body(self, inputs, driver, normalize, **kwargs):  
         
         outputs = []
         
         if normalize:
             for name in self.names:
                 normal_layer = tf.keras.layers.Normalization()
-                normal_layer.adapt(driver.get_training_data(name))
+                normal_layer.adapt(driver.get_data_tensor(driver.training_data, name))
                 outputs.append(normal_layer(inputs[name]))
         else:
             for name in self.names:
                 outputs.append(inputs[name])
         
         return tf.concat(outputs, axis=-1)
 
@@ -196,15 +196,15 @@
         
         # apply dropout to each input
         for i in range(len(outputs)):
             outputs[i] = dropout_layer(outputs[i])
             
             # encode to numeric
             encode_layer = tf.keras.layers.StringLookup(oov_token=self.dropout_token)
-            encode_layer.adapt(driver.get_training_data(self.names[i]))
+            encode_layer.adapt(np.unique(driver.get_data_tensor(driver.training_data, self.names[i])))
             outputs[i] = encode_layer(outputs[i])
             
             # get the vocab size for this input
             vocab_size = len(encode_layer.get_vocabulary())
         
             # if one hot encoding
             if use_one_hot:
```

### Comparing `quik-ai-1.0.2/src/quik_ai/tuners.py` & `quik-ai-1.1.0/src/quik_ai/tuners.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.2/src/quik_ai/tuning.py` & `quik-ai-1.1.0/src/quik_ai/tuning.py`

 * *Files identical despite different names*

### Comparing `quik-ai-1.0.2/src/quik_ai.egg-info/PKG-INFO` & `quik-ai-1.1.0/src/quik_ai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: quik-ai
-Version: 1.0.2
+Version: 1.1.0
 Summary: Quick Unifying Infrastructure Kit for Machine Learning and AI
 Home-page: https://github.com/touzov1012/quik-ai
-Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.0.2.tar.gz
+Download-URL: https://github.com/touzov1012/quik-ai/archive/refs/tags/v1.1.0.tar.gz
 Author: Aleksandr Touzov
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -32,17 +32,17 @@
 head = qa.heads.GaussianMixture()
 ```
 
 3. Specify the predictors used for model fitting.
 ```python
 # All the predictors for the model.
 predictors = [
-    qa.predictors.NumericalPredictor('numerical'),
-    qa.predictors.CategoricalPredictor('categorical'),
-    qa.predictors.PeriodicPredictor('periodic', 24.0),
+    qa.predictors.Numerical('numerical'),
+    qa.predictors.Categorical('categorical'),
+    qa.predictors.Periodic('periodic', 24.0),
 ]
 ```
 
 4. Select the model architecture.
 ```python
 # Select the architecture and feed the response column, and other
 # necessary data for training, testing the model.
```

