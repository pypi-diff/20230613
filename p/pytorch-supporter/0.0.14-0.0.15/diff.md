# Comparing `tmp/pytorch-supporter-0.0.14.tar.gz` & `tmp/pytorch-supporter-0.0.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-supporter-0.0.14.tar", last modified: Sun Mar 12 11:09:09 2023, max compression
+gzip compressed data, was "pytorch-supporter-0.0.15.tar", last modified: Tue Jun 13 11:28:06 2023, max compression
```

## Comparing `pytorch-supporter-0.0.14.tar` & `pytorch-supporter-0.0.15.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 11:09:09.826262 pytorch-supporter-0.0.14/
--rw-r--r--   0 root         (0) root         (0)     2349 2023-03-12 11:09:09.825262 pytorch-supporter-0.0.14/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2067 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 11:09:09.823262 pytorch-supporter-0.0.14/pytorch_supporter/
--rw-r--r--   0 root         (0) root         (0)       41 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 11:09:09.825262 pytorch-supporter-0.0.14/pytorch_supporter/layers/
--rw-r--r--   0 root         (0) root         (0)      984 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/layers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      198 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/layers/dict_to_parameters.py
--rw-r--r--   0 root         (0) root         (0)      425 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/layers/dot_product.py
--rw-r--r--   0 root         (0) root         (0)      644 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/layers/gru_last_hidden_state.py
--rw-r--r--   0 root         (0) root         (0)      801 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/layers/hidden_state_reset_gru.py
--rw-r--r--   0 root         (0) root         (0)      872 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/layers/hidden_state_reset_lstm.py
--rw-r--r--   0 root         (0) root         (0)      801 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/layers/hidden_state_reset_rnn.py
--rw-r--r--   0 root         (0) root         (0)      589 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/layers/lazily_initialized_linear.py
--rw-r--r--   0 root         (0) root         (0)      655 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/layers/lstm_last_hidden_state.py
--rw-r--r--   0 root         (0) root         (0)      225 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/layers/permute.py
--rw-r--r--   0 root         (0) root         (0)      336 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/layers/reshape.py
--rw-r--r--   0 root         (0) root         (0)      644 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/layers/rnn_last_hidden_state.py
--rw-r--r--   0 root         (0) root         (0)      197 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/layers/select_from_array.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 11:09:09.825262 pytorch-supporter-0.0.14/pytorch_supporter/utils/
--rw-r--r--   0 root         (0) root         (0)      145 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)      802 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/utils/text.py
--rw-r--r--   0 root         (0) root         (0)      835 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter/utils/time_series.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-12 11:09:09.824262 pytorch-supporter-0.0.14/pytorch_supporter.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2349 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1000 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       14 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/pytorch_supporter.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-12 11:09:09.826262 pytorch-supporter-0.0.14/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      604 2023-03-12 11:09:09.000000 pytorch-supporter-0.0.14/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:28:06.108760 pytorch-supporter-0.0.15/
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-06-13 11:28:06.108760 pytorch-supporter-0.0.15/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2154 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:28:06.103760 pytorch-supporter-0.0.15/pytorch_supporter/
+-rw-r--r--   0 root         (0) root         (0)       41 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:28:06.107760 pytorch-supporter-0.0.15/pytorch_supporter/layers/
+-rw-r--r--   0 root         (0) root         (0)      984 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/layers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      198 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/layers/dict_to_parameters.py
+-rw-r--r--   0 root         (0) root         (0)      425 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/layers/dot_product.py
+-rw-r--r--   0 root         (0) root         (0)      644 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/layers/gru_last_hidden_state.py
+-rw-r--r--   0 root         (0) root         (0)      801 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/layers/hidden_state_reset_gru.py
+-rw-r--r--   0 root         (0) root         (0)      872 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/layers/hidden_state_reset_lstm.py
+-rw-r--r--   0 root         (0) root         (0)      801 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/layers/hidden_state_reset_rnn.py
+-rw-r--r--   0 root         (0) root         (0)      707 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/layers/lazily_initialized_linear.py
+-rw-r--r--   0 root         (0) root         (0)      655 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/layers/lstm_last_hidden_state.py
+-rw-r--r--   0 root         (0) root         (0)      225 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/layers/permute.py
+-rw-r--r--   0 root         (0) root         (0)      336 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/layers/reshape.py
+-rw-r--r--   0 root         (0) root         (0)      644 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/layers/rnn_last_hidden_state.py
+-rw-r--r--   0 root         (0) root         (0)      197 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/layers/select_from_array.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:28:06.107760 pytorch-supporter-0.0.15/pytorch_supporter/utils/
+-rw-r--r--   0 root         (0) root         (0)      145 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      802 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/utils/text.py
+-rw-r--r--   0 root         (0) root         (0)      835 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter/utils/time_series.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 11:28:06.104760 pytorch-supporter-0.0.15/pytorch_supporter.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2416 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1000 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       14 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/pytorch_supporter.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-13 11:28:06.108760 pytorch-supporter-0.0.15/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      604 2023-06-13 11:28:05.000000 pytorch-supporter-0.0.15/setup.py
```

### Comparing `pytorch-supporter-0.0.14/PKG-INFO` & `pytorch-supporter-0.0.15/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: pytorch-supporter
-Version: 0.0.14
+Version: 0.0.15
 Summary: Pytorch supporter
 Home-page: https://github.com/automatethem/pytorch-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # pytorch-supporter
 
+https://pypi.org/project/pytorch-supporter
+<pre>
+pip install pytorch-supporter
+</pre>
+
 Supported layers
 
 <pre>
 import pytorch_supporter
 
 pytorch_supporter.layers.DictToParameters
 pytorch_supporter.layers.DotProduct
@@ -66,9 +70,7 @@
 #window_length = sequence_length + 1
 train_x, train_label = pytorch_supporter.utils.slice_time_series_data_from_np_array(train_np_array, x_column_indexes=[0, 1, 2, 3, 4, 5], label_column_indexes=[3], sequence_length=7)
 #print(train_x.shape) #(973, 7, 6)
 #print(train_labels.shape) #(973, 1)
 #print(validation_x.shape) #(238, 7, 6)
 #print(validation_labels.shape) #(238, 1)
 </pre>
-
-
```

### Comparing `pytorch-supporter-0.0.14/README.md` & `pytorch-supporter-0.0.15/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,14 @@
 # pytorch-supporter
 
+https://pypi.org/project/pytorch-supporter
+<pre>
+pip install pytorch-supporter
+</pre>
+
 Supported layers
 
 <pre>
 import pytorch_supporter
 
 pytorch_supporter.layers.DictToParameters
 pytorch_supporter.layers.DotProduct
```

### Comparing `pytorch-supporter-0.0.14/pytorch_supporter/layers/__init__.py` & `pytorch-supporter-0.0.15/pytorch_supporter/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.14/pytorch_supporter/layers/gru_last_hidden_state.py` & `pytorch-supporter-0.0.15/pytorch_supporter/layers/gru_last_hidden_state.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.14/pytorch_supporter/layers/hidden_state_reset_gru.py` & `pytorch-supporter-0.0.15/pytorch_supporter/layers/hidden_state_reset_gru.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.14/pytorch_supporter/layers/hidden_state_reset_lstm.py` & `pytorch-supporter-0.0.15/pytorch_supporter/layers/hidden_state_reset_lstm.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.14/pytorch_supporter/layers/hidden_state_reset_rnn.py` & `pytorch-supporter-0.0.15/pytorch_supporter/layers/hidden_state_reset_rnn.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.14/pytorch_supporter/layers/lazily_initialized_linear.py` & `pytorch-supporter-0.0.15/pytorch_supporter/layers/lazily_initialized_linear.py`

 * *Files 13% similar despite different names*

```diff
@@ -7,11 +7,15 @@
         self.out_features = out_features
 
     def forward(self, x):
         if not self.layer:
             in_features = x.shape[1]
             self.layer = torch.nn.Linear(in_features=in_features, out_features=self.out_features)
             if x.is_cuda:
-                device = torch.device('cuda' if torch.cuda.is_available() else 'cpu')
+                device = "cpu"
+                if torch.cuda.is_available():
+                    device = "cuda"
+                elif torch.backends.mps.is_available():
+                    device = "mps"
                 self.layer = self.layer.to(device)
         x = self.layer(x)
         return x
```

### Comparing `pytorch-supporter-0.0.14/pytorch_supporter/layers/lstm_last_hidden_state.py` & `pytorch-supporter-0.0.15/pytorch_supporter/layers/lstm_last_hidden_state.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.14/pytorch_supporter/layers/rnn_last_hidden_state.py` & `pytorch-supporter-0.0.15/pytorch_supporter/layers/rnn_last_hidden_state.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.14/pytorch_supporter/utils/text.py` & `pytorch-supporter-0.0.15/pytorch_supporter/utils/text.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.14/pytorch_supporter/utils/time_series.py` & `pytorch-supporter-0.0.15/pytorch_supporter/utils/time_series.py`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.14/pytorch_supporter.egg-info/PKG-INFO` & `pytorch-supporter-0.0.15/pytorch_supporter.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: pytorch-supporter
-Version: 0.0.14
+Version: 0.0.15
 Summary: Pytorch supporter
 Home-page: https://github.com/automatethem/pytorch-supporter
 Author: Sang Ki Kwon
 Author-email: automatethem@gmail.com
 License: MIT
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 
 # pytorch-supporter
 
+https://pypi.org/project/pytorch-supporter
+<pre>
+pip install pytorch-supporter
+</pre>
+
 Supported layers
 
 <pre>
 import pytorch_supporter
 
 pytorch_supporter.layers.DictToParameters
 pytorch_supporter.layers.DotProduct
@@ -66,9 +70,7 @@
 #window_length = sequence_length + 1
 train_x, train_label = pytorch_supporter.utils.slice_time_series_data_from_np_array(train_np_array, x_column_indexes=[0, 1, 2, 3, 4, 5], label_column_indexes=[3], sequence_length=7)
 #print(train_x.shape) #(973, 7, 6)
 #print(train_labels.shape) #(973, 1)
 #print(validation_x.shape) #(238, 7, 6)
 #print(validation_labels.shape) #(238, 1)
 </pre>
-
-
```

### Comparing `pytorch-supporter-0.0.14/pytorch_supporter.egg-info/SOURCES.txt` & `pytorch-supporter-0.0.15/pytorch_supporter.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pytorch-supporter-0.0.14/setup.py` & `pytorch-supporter-0.0.15/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 def requirements():
     with open(os.path.join(os.path.dirname(__file__), 'requirements.txt'), encoding='utf-8') as f:
         return f.read().splitlines()
 
 setuptools.setup(
 	name='pytorch-supporter',
-	version='0.0.14',
+	version='0.0.15',
 	description='Pytorch supporter',
 	long_description=open('README.md').read(),
 	long_description_content_type='text/markdown',
 	author='Sang Ki Kwon',
 	url='https://github.com/automatethem/pytorch-supporter',
 	install_requires=requirements(),
 	author_email='automatethem@gmail.com',
```

