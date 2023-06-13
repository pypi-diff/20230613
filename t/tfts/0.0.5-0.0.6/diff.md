# Comparing `tmp/tfts-0.0.5.tar.gz` & `tmp/tfts-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tfts-0.0.5.tar", max compression
+gzip compressed data, was "tfts-0.0.6.tar", max compression
```

## Comparing `tfts-0.0.5.tar` & `tfts-0.0.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
--rwxr-xr-x   0        0        0     1093 2022-12-02 13:17:06.945455 tfts-0.0.5/LICENSE
--rw-r--r--   0        0        0     9783 2022-12-02 13:17:06.945455 tfts-0.0.5/README.md
--rw-r--r--   0        0        0     2346 2022-12-02 13:17:30.853699 tfts-0.0.5/pyproject.toml
--rw-r--r--   0        0        0      462 2022-12-02 13:17:30.857699 tfts-0.0.5/tfts/__init__.py
--rw-r--r--   0        0        0       20 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/datasets/__init__.py
--rw-r--r--   0        0        0     3051 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/datasets/get_data.py
--rw-r--r--   0        0        0       20 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/features/__init__.py
--rw-r--r--   0        0        0      109 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/features/ar_feature.py
--rw-r--r--   0        0        0       49 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/features/time_feature.py
--rw-r--r--   0        0        0       42 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/features/two_order_feature.py
--rw-r--r--   0        0        0       18 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/layers/__init__.py
--rw-r--r--   0        0        0     5295 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/layers/attention_layer.py
--rw-r--r--   0        0        0     4370 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/layers/autoformer_layer.py
--rw-r--r--   0        0        0     3213 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/layers/cnn_layer.py
--rw-r--r--   0        0        0     1510 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/layers/deepar_layer.py
--rw-r--r--   0        0        0     3953 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/layers/dense_layer.py
--rw-r--r--   0        0        0     7289 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/layers/embed_layer.py
--rw-r--r--   0        0        0      325 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/layers/mask_layer.py
--rw-r--r--   0        0        0     6148 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/layers/nbeats_layer.py
--rw-r--r--   0        0        0     4081 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/layers/unet_layer.py
--rw-r--r--   0        0        0       18 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/models/__init__.py
--rw-r--r--   0        0        0     2064 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/models/auto_config.py
--rw-r--r--   0        0        0     4263 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/models/auto_model.py
--rw-r--r--   0        0        0     7507 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/models/autoformer.py
--rw-r--r--   0        0        0     5709 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/models/bert.py
--rw-r--r--   0        0        0     1560 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/models/deepar.py
--rw-r--r--   0        0        0    12036 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/models/informer.py
--rw-r--r--   0        0        0     2784 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/models/nbeats.py
--rw-r--r--   0        0        0     7413 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/models/rnn.py
--rw-r--r--   0        0        0    13860 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/models/seq2seq.py
--rw-r--r--   0        0        0     5501 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/models/tcn.py
--rw-r--r--   0        0        0    18783 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/models/transformer.py
--rw-r--r--   0        0        0     4887 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/models/unet.py
--rw-r--r--   0        0        0    12689 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/models/wavenet.py
--rw-r--r--   0        0        0    13293 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/trainer.py
--rw-r--r--   0        0        0      429 2022-12-02 13:17:06.949455 tfts-0.0.5/tfts/tuner.py
--rw-r--r--   0        0        0    10802 1970-01-01 00:00:00.000000 tfts-0.0.5/setup.py
--rw-r--r--   0        0        0    11248 1970-01-01 00:00:00.000000 tfts-0.0.5/PKG-INFO
+-rwxr-xr-x   0        0        0     1093 2023-06-13 04:09:54.906426 tfts-0.0.6/LICENSE
+-rw-r--r--   0        0        0    10195 2023-06-13 04:09:54.906426 tfts-0.0.6/README.md
+-rw-r--r--   0        0        0     2346 2023-06-13 04:10:24.048173 tfts-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0      462 2023-06-13 04:10:24.052173 tfts-0.0.6/tfts/__init__.py
+-rw-r--r--   0        0        0       20 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/datasets/__init__.py
+-rw-r--r--   0        0        0     3822 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/datasets/get_data.py
+-rw-r--r--   0        0        0       20 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/features/__init__.py
+-rw-r--r--   0        0        0      109 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/features/ar_feature.py
+-rw-r--r--   0        0        0       49 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/features/time_feature.py
+-rw-r--r--   0        0        0       42 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/features/two_order_feature.py
+-rw-r--r--   0        0        0       18 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/__init__.py
+-rw-r--r--   0        0        0     9975 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/attention_layer.py
+-rw-r--r--   0        0        0     5329 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/autoformer_layer.py
+-rw-r--r--   0        0        0     3245 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/cnn_layer.py
+-rw-r--r--   0        0        0     1716 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/deepar_layer.py
+-rw-r--r--   0        0        0     4003 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/dense_layer.py
+-rw-r--r--   0        0        0     8593 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/embed_layer.py
+-rw-r--r--   0        0        0     1387 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/mask_layer.py
+-rw-r--r--   0        0        0     6420 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/nbeats_layer.py
+-rw-r--r--   0        0        0     4081 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/layers/unet_layer.py
+-rw-r--r--   0        0        0       18 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/__init__.py
+-rw-r--r--   0        0        0     2064 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/auto_config.py
+-rw-r--r--   0        0        0     4263 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/auto_model.py
+-rw-r--r--   0        0        0     7507 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/autoformer.py
+-rw-r--r--   0        0        0     5721 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/bert.py
+-rw-r--r--   0        0        0     1560 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/deepar.py
+-rw-r--r--   0        0        0    10177 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/informer.py
+-rw-r--r--   0        0        0     2784 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/nbeats.py
+-rw-r--r--   0        0        0      123 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/patchtst.py
+-rw-r--r--   0        0        0     7428 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/rnn.py
+-rw-r--r--   0        0        0    13873 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/seq2seq.py
+-rw-r--r--   0        0        0     5513 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/tcn.py
+-rw-r--r--   0        0        0      111 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/tide.py
+-rw-r--r--   0        0        0    18805 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/transformer.py
+-rw-r--r--   0        0        0     4905 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/unet.py
+-rw-r--r--   0        0        0    12701 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/models/wavenet.py
+-rw-r--r--   0        0        0    13386 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/trainer.py
+-rw-r--r--   0        0        0      429 2023-06-13 04:09:54.910426 tfts-0.0.6/tfts/tuner.py
+-rw-r--r--   0        0        0    11461 1970-01-01 00:00:00.000000 tfts-0.0.6/PKG-INFO
```

### Comparing `tfts-0.0.5/LICENSE` & `tfts-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `tfts-0.0.5/README.md` & `tfts-0.0.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -81,16 +81,16 @@
 Encoder only model inputs
 
 ```python
 train_length = 49
 predict_length = 10
 n_feature = 2
 
-x_train = np.random.rand(1, train_length, n_feature)  # feature: (n, train_length, feature)
-y_train = np.random.rand(1, predict_length, 1)  # y: (n, predict_length, 1)
+x_train = np.random.rand(1, train_length, n_feature)  # inputs: (batch, train_length, feature)
+y_train = np.random.rand(1, predict_length, 1)  # target: (batch, predict_length, 1)
 x_valid = np.random.rand(1, train_length, n_feature)
 y_valid = np.random.rand(1, predict_length, 1)
 
 model = AutoModel("rnn", predict_length=predict_length)
 trainer = KerasTrainer(model)
 trainer.train(train_dataset=(x_train, y_train), valid_dataset=(x_valid, y_valid), n_epochs=1)
 
@@ -103,19 +103,19 @@
 
 train_length = 49
 predict_length = 10
 n_encoder_feature = 2
 n_decoder_feature = 3
 
 x_train = (
-    np.random.rand(1, train_length, 1),  # x: (n, train_length, 1)
-    np.random.rand(1, train_length, n_encoder_feature),  # encoder_feature: (n, train_length, encoder_features)
-    np.random.rand(1, predict_length, n_decoder_feature),  # decoder_feature: (n, predict_length, decoder_features)
+    np.random.rand(1, train_length, 1),  # inputs: (batch, train_length, 1)
+    np.random.rand(1, train_length, n_encoder_feature),  # encoder_feature: (batch, train_length, encoder_features)
+    np.random.rand(1, predict_length, n_decoder_feature),  # decoder_feature: (batch, predict_length, decoder_features)
 )
-y_train = np.random.rand(1, predict_length, 1)  # y: (n, predict_length, 1)
+y_train = np.random.rand(1, predict_length, 1)  # target: (batch, predict_length, 1)
 x_valid = (
     np.random.rand(1, train_length, 1),
     np.random.rand(1, train_length, n_encoder_feature),
     np.random.rand(1, predict_length, n_decoder_feature),
 )
 y_valid = np.random.rand(1, predict_length, 1)
 
@@ -124,15 +124,15 @@
 trainer.train((x_train, y_train), (x_valid, y_valid), n_epochs=1)
 ```
 
 ```python
 # option2: tf.data.Dataset
 
 class FakeReader(object):
-    def __init__(self, predict_length=10):
+    def __init__(self, predict_length):
         train_length = 49
         n_encoder_feature = 2
         n_decoder_feature = 3
         self.x = np.random.rand(15, train_length, 1)
         self.encoder_feature = np.random.rand(15, train_length, n_encoder_feature)
         self.decoder_feature = np.random.rand(15, predict_length, n_decoder_feature)
         self.target = np.random.rand(15, predict_length, 1)
@@ -149,44 +149,65 @@
 
     def iter(self):
         for i in range(len(self.x)):
             yield self[i]
 
 
 predict_length = 10
-train_reader = FakeReader(predict_length=10)
+train_reader = FakeReader(predict_length=predict_length)
 train_loader = tf.data.Dataset.from_generator(
     train_reader.iter,
     ({"x": tf.float32, "encoder_feature": tf.float32, "decoder_feature": tf.float32}, tf.float32),
 )
 train_loader = train_loader.batch(batch_size=1)
-valid_reader = FakeReader(predict_length=10)
+valid_reader = FakeReader(predict_length=predict_length)
 valid_loader = tf.data.Dataset.from_generator(
     valid_reader.iter,
     ({"x": tf.float32, "encoder_feature": tf.float32, "decoder_feature": tf.float32}, tf.float32),
 )
 valid_loader = valid_loader.batch(batch_size=1)
 
 model = AutoModel("seq2seq", predict_length=predict_length)
 trainer = KerasTrainer(model)
 trainer.train(train_dataset=train_loader, valid_dataset=valid_loader, n_epochs=1)
 ```
 
+**Prepare custom model params**
+
+```python
+import tensorflow as tf
+import tfts
+from tfts import AutoModel, AutoConfig
+
+config = AutoConfig('rnn').get_config()
+print(config)
+
+custom_model_params = {
+    "rnn_size": 128,
+    "dense_size": 128,
+}
+
+model = AutoModel('rnn', predict_length=7, custom_model_params=custom_model_params)
+```
+
 **Build your own model**
 
-The models tfts support to use in `AutoModel()`
+<details><summary> Full list of model tfts supported using AutoModel </summary>
+
 - rnn
 - tcn
 - bert
 - nbeats
 - seq2seq
 - wavenet
 - transformer
 
-You could build the model based on tfts backbone, especially
+</details>
+
+You could build the custom model based on tfts, especially
 - add custom-defined embeddings for categorical variables
 - add custom-defined head layers for classification or anomaly task
 
 ```python
 import tensorflow as tf
 from tensorflow.keras.layers import Input, Dense
 from tfts import AutoModel
@@ -204,16 +225,16 @@
     model = tf.keras.Model(inputs=inputs, outputs=outputs)
     model.compile(loss="mse", optimizer="rmsprop")
     return model
 ```
 
 ## Examples
 
-- [TFTS-Bert](https://github.com/LongxingTan/KDDCup2022-Baidu) wins the **3rd place** in KDD Cup 2022 Baidu-wind power forecasting
-- [TFTS-Seq2seq](https://github.com/LongxingTan/Data-competitions/tree/master/tianchi-enso-prediction) wins the **4th place** in Alibaba Tianchi-ENSO prediction 2021
+- [TFTS-Bert](https://github.com/LongxingTan/KDDCup2022-Baidu) wins the **3rd place** in KDD Cup 2022-wind power forecasting
+- [TFTS-Seq2seq](https://github.com/LongxingTan/Data-competitions/tree/master/tianchi-enso-prediction) wins the **4th place** in Tianchi-ENSO prediction 2021
 
 <!-- ### Performance
 
 [Time series prediction](./examples/run_prediction.py) performance is evaluated by tfts implementation, not official
 
 | Performance | [web traffic<sup>mape</sup>]() | [grocery sales<sup>wrmse</sup>](https://www.kaggle.com/competitions/favorita-grocery-sales-forecasting/data) | [m5 sales<sup>val</sup>]() | [ventilator<sup>val</sup>]() |
 | :-- | :-: | :-: | :-: | :-: |
@@ -234,15 +255,15 @@
 - [More complex prediction task](./notebooks)
 - [Time series classification](./examples/run_classification.py)
 - [Anomaly detection](./examples/run_anomaly.py)
 - [Uncertainty prediction](examples/run_uncertainty.py)
 - [Parameters tuning by optuna](examples/run_optuna_tune.py)
 - [Serving by tf-serving](./examples) -->
 
-if you prefer other DL frameworks, try [pytorch-forecasting](https://github.com/jdb78/pytorch-forecasting), [gluonts](https://github.com/awslabs/gluonts), [paddlets](https://github.com/PaddlePaddle/PaddleTS)
+For other DL frameworks, try [pytorch-forecasting](https://github.com/jdb78/pytorch-forecasting), [gluonts](https://github.com/awslabs/gluonts), [paddlets](https://github.com/PaddlePaddle/PaddleTS)
 
 ## Citation
 
 If you find tfts project useful in your research, please consider cite:
 
 ```
 @misc{tfts2020,
```

### Comparing `tfts-0.0.5/pyproject.toml` & `tfts-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 [tool.nbqa.mutate]
 isort = 1
 black = 1
 
 [tool.poetry]
 name = "tfts"
 readme = "README.md"  # Markdown files are supported
-version = "0.0.5"  # is being replaced automatically
+version = "0.0.6"  # is being replaced automatically
 
 authors = ["Longxing Tan"]
 classifiers = [
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.7",
```

### Comparing `tfts-0.0.5/tfts/datasets/get_data.py` & `tfts-0.0.6/tfts/datasets/get_data.py`

 * *Files 20% similar despite different names*

```diff
@@ -20,14 +20,26 @@
         return get_air_passengers(train_length, predict_length, test_size=test_size)
 
     else:
         raise ValueError("unsupported data of {} yet, try 'sine', 'airpassengers'".format(name))
 
 
 def get_sine(train_sequence_length: int = 24, predict_sequence_length: int = 8, test_size: float = 0.2, n_examples=100):
+    """
+    Generate synthetic sine wave data.
+
+    Parameters:
+    train_sequence_length (int): Length of the training sequence.
+    predict_sequence_length (int): Length of the prediction sequence.
+    test_size (float): Fraction of the data to use for validation.
+    n_examples (int): Number of examples to generate.
+
+    Returns:
+    (tuple): Two tuples of numpy arrays containing training and validation data.
+    """
     x = []
     y = []
     for _ in range(n_examples):
         rand = random.random() * 2 * np.pi
         sig1 = np.sin(np.linspace(rand, 3.0 * np.pi + rand, train_sequence_length + predict_sequence_length))
         sig2 = np.cos(np.linspace(rand, 3.0 * np.pi + rand, train_sequence_length + predict_sequence_length))
 
@@ -53,15 +65,26 @@
         x_valid = x[slice:]
         y_valid = y[slice:]
         return (x_train, y_train), (x_valid, y_valid)
     return x, y
 
 
 def get_air_passengers(train_sequence_length: int = 24, predict_sequence_length: int = 8, test_size: float = 0.2):
-    """Air passengers data, just use divide 500 to normalize it"""
+    """
+    A function that loads and preprocesses the air passenger data.
+
+    Args:
+        train_sequence_length (int): The length of each input sequence.
+        predict_sequence_length (int): The length of each output sequence.
+        test_size (float): The fraction of the data to use for validation.
+
+    Returns:
+        Tuple of training and validation data, each containing inputs and outputs.
+
+    """
     # air_passenger_url = "../examples/data/international-airline-passengers.csv"
     df = pd.read_csv(air_passenger_url, parse_dates=None, date_parser=None, nrows=144)
     v = df.iloc[:, 1:2].values
     v = (v - np.max(v)) / (np.max(v) - np.min(v))  # MinMaxScaler
 
     x, y = [], []
     for seq in range(1, train_sequence_length + 1):
```

### Comparing `tfts-0.0.5/tfts/layers/autoformer_layer.py` & `tfts-0.0.6/tfts/layers/autoformer_layer.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,39 +11,42 @@
 class SeriesDecomp(tf.keras.layers.Layer):
     def __init__(self, kernel_size: int) -> None:
         super().__init__()
         self.kernel_size = kernel_size
         self.moving_avg = AveragePooling1D(pool_size=kernel_size, strides=1, padding="same")
 
     def call(self, x):
-        """_summary_
+        """
+        Perform time-series decomposition on the input tensor.
 
         Parameters
         ----------
-        x : _type_
-            _description_
+        x : tf.Tensor
+            A 3D tensor with shape (batch_size, sequence_length, input_dim).
 
         Returns
         -------
-        _type_
-            _description_
+        Tuple[tf.Tensor, tf.Tensor]
+            A tuple of two 3D tensors:
+            - The residual tensor, shape (batch_size, sequence_length, input_dim).
+            - The moving average tensor, which is a smoothed version of the input tensor.
         """
         x_ma = self.moving_avg(x)
         return x - x_ma, x_ma
 
     def get_config(self):
         config = {
             "kernel_size": self.kernel_size,
         }
         base_config = super().get_config()
         return dict(list(base_config.items()) + list(config.items()))
 
 
 class AutoCorrelation(tf.keras.layers.Layer):
-    """Auto"""
+    """Self-Attention layer that computes time-delayed autocorrelation between queries and keys"""
 
     def __init__(self, d_model: int, num_heads: int, attention_dropout: float = 0.0) -> None:
         super().__init__()
         self.d_model = d_model
         self.num_heads = num_heads
         self.depth = d_model // num_heads
         self.attention_dropout = attention_dropout
@@ -52,14 +55,30 @@
         self.wq = Dense(self.d_model, name="q")
         self.wk = Dense(self.d_model, name="k")
         self.wv = Dense(self.d_model, name="v")
         self.drop = Dropout(self.attention_dropout)
         self.dense = Dense(self.d_model, name="project")
 
     def time_delay_agg(self, q, k, v):  # TODO: v not used in process
+        """Compute time-delayed autocorrelation between queries and keys.
+
+        Parameters
+        ----------
+        q : Tensor of shape (batch_size, num_heads, timesteps, depth)
+            Queries.
+        k : Tensor of shape (batch_size, num_heads, timesteps, depth)
+            Keys.
+        v : Tensor of shape (batch_size, num_heads, timesteps, depth)
+            Values.
+
+        Returns
+        -------
+        Tensor of shape (batch_size, num_heads, timesteps, depth)
+            Time-delayed autocorrelation between queries and keys.
+        """
         batch_size = tf.shape(q)[0]
         time_steps = tf.shape(q)[2]
         q_fft = tf.signal.rfft(tf.transpose(q, perm=[0, 1, 3, 2]))
         k_fft = tf.signal.rfft(tf.transpose(k, perm=[0, 1, 3, 2]))
         S_qk = q_fft * tf.math.conj(k_fft)
         R_qk = tf.signal.irfft(S_qk)
```

### Comparing `tfts-0.0.5/tfts/layers/cnn_layer.py` & `tfts-0.0.6/tfts/layers/cnn_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,24 +39,24 @@
             padding="valid",
             dilation_rate=self.dilation_rate,
             activation=self.activation,
         )
         super(ConvTemp, self).build(input_shape)
 
     def call(self, inputs):
-        """_summary_
+        """forward pass
 
         Parameters
         ----------
-        inputs : _type_
-            _description_
+        inputs : inputs
+            tensor with batch * sequence * features
 
         Returns
         -------
-        _type_
+        tf.Tensor
             _description_
         """
         if self.causal:
             padding_size = (self.kernel_size - 1) * self.dilation_rate
             # padding: dim 1 is batch, [0,0]; dim 2 is time, [padding_size, 0]; dim 3 is feature [0,0]
             inputs = tf.pad(inputs, [[0, 0], [padding_size, 0], [0, 0]])
```

### Comparing `tfts-0.0.5/tfts/layers/deepar_layer.py` & `tfts-0.0.6/tfts/layers/deepar_layer.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,26 +21,25 @@
             name="gauss_w2", shape=(in_channels, self.units), initializer=tf.keras.initializers.GlorotNormal()
         )
         self.bias1 = self.add_weight(name="gauss_b1", shape=(self.units,), initializer=tf.keras.initializers.Zeros())
         self.bias2 = self.add_weight(name="gauss_b2", shape=(self.units,), initializer=tf.keras.initializers.Zeros())
         super(GaussianLayer, self).build(input_shape)
 
     def call(self, x):
-        """_summary_
+        """Returns mean and standard deviation tensors.
 
-        Parameters
-        ----------
-        x : _type_
-            _description_
+        Args:
+          x (tf.Tensor): Input tensor.
 
-        Returns
-        -------
-        _type_
-            _description_
+        Returns:
+          Tuple[tf.Tensor, tf.Tensor]: Mean and standard deviation tensors.
         """
         mu = tf.matmul(x, self.weight1) + self.bias1
         sig = tf.matmul(x, self.weight2) + self.bias2
         sig_pos = tf.math.log1p(tf.math.exp(sig)) + 1e-7
         return mu, sig_pos
 
     def get_config(self):
-        return
+        """Returns the configuration of the layer."""
+        config = {"units": self.units}
+        base_config = super(GaussianLayer, self).get_config()
+        return {**base_config, **config}
```

### Comparing `tfts-0.0.5/tfts/layers/dense_layer.py` & `tfts-0.0.6/tfts/layers/dense_layer.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,25 +45,21 @@
         if self.use_bias:
             self.bias = self.add_weight(
                 "bias", shape=[self.hidden_size], initializer=self.bias_initializer, dtype=self.dtype, trainable=True
             )
         super(DenseTemp, self).build(input_shape)
 
     def call(self, inputs):
-        """_summary_
+        """Computes the output of the layer.
 
-        Parameters
-        ----------
-        inputs : _type_
-            _description_
+        Args:
+            inputs: Tensor of shape (batch_size, sequence_length, input_dim)
 
-        Returns
-        -------
-        _type_
-            _description_
+        Returns:
+            output: Tensor of shape (batch_size, sequence_length, hidden_size)
         """
         output = tf.einsum("ijk,kl->ijl", inputs, self.kernel)
 
         if self.use_bias:
             output += self.bias
 
         if self.activation is not None:
```

### Comparing `tfts-0.0.5/tfts/layers/embed_layer.py` & `tfts-0.0.6/tfts/layers/embed_layer.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,16 +5,24 @@
 import numpy as np
 import tensorflow as tf
 from tensorflow.keras.layers import GRU, LSTM, Conv1D, Dense, Dropout, Embedding, LayerNormalization, SpatialDropout1D
 
 
 class TokenEmbedding(tf.keras.layers.Layer):
     """
-    x: batch * time * feature
-    outout: batch * time * new_attention_size）
+    A layer that performs token embedding.
+
+    Args:
+        embed_size (int): The size of the embedding.
+
+    Input shape:
+        - 3D tensor with shape `(batch_size, time_steps, input_dim)`
+
+    Output shape:
+        - 3D tensor with shape `(batch_size, time_steps, embed_size)`
     """
 
     def __init__(self, embed_size: int):
         super(TokenEmbedding, self).__init__()
         self.embed_size = embed_size
 
     def build(self, input_shape):
@@ -22,25 +30,22 @@
             name="token_weights",
             shape=[input_shape[-1], self.embed_size],
             initializer=tf.random_normal_initializer(mean=0.0, stddev=self.embed_size**-0.5),
         )
         super(TokenEmbedding, self).build(input_shape)
 
     def call(self, x):
-        """_summary_
+        """
+        Performs the token embedding.
 
-        Parameters
-        ----------
-        x : _type_
-            _description_
+        Args:
+            x (tensor): Input tensor.
 
-        Returns
-        -------
-        _type_
-            _description_
+        Returns:
+            Tensor: Embedded tensor.
         """
         y = tf.einsum("bsf,fk->bsk", x, self.token_weights)
         return y
 
     def get_config(self):
         config = {"embed_size": self.embed_size}
         base_config = super(TokenEmbedding, self).get_config()
@@ -53,25 +58,26 @@
         self.embed_size = embed_size
 
     def build(self, input_shape):
         self.rnn = GRU(self.embed_size, return_sequences=True, return_state=True)
         super().build(input_shape)
 
     def call(self, x):
-        """_summary_
+        """
+        Forward pass of the layer.
 
         Parameters
         ----------
-        x : _type_
-            _description_
+        x : tf.Tensor
+            Input tensor of shape `(batch_size, sequence_length, input_dim)`.
 
         Returns
         -------
-        _type_
-            _description_
+        y : tf.Tensor
+            Output tensor of shape `(batch_size, sequence_length, embed_size)`.
         """
         y, _ = self.rnn(x)
         return y
 
     def get_config(self):
         config = {"embed_size": self.embed_size}
         base_config = super(TokenRnnEmbedding, self).get_config()
@@ -83,27 +89,23 @@
         super(PositionalEmbedding, self).__init__()
         self.max_len = max_len
 
     def build(self, input_shape):
         super(PositionalEmbedding, self).build(input_shape)
 
     def call(self, x, masking=True):
-        """_summary_
+        """
+        Applies positional encoding to the input tensor.
 
-        Parameters
-        ----------
-        x : _type_
-            _description_
-        masking : bool, optional
-            _description_, by default True
+        Parameters:
+        x (tf.Tensor): Input tensor of shape (batch_size, sequence_length, embedding_dim).
+        masking (bool, optional): If True, applies masking to the output tensor, by default True.
 
-        Returns
-        -------
-        _type_
-            _description_
+        Returns:
+        tf.Tensor: Output tensor of the same shape as the input tensor, after applying positional encoding.
         """
         E = x.get_shape().as_list()[-1]  # static
         batch_size, seq_length = tf.shape(x)[0], tf.shape(x)[1]  # dynamic
 
         position_ind = tf.tile(tf.expand_dims(tf.range(seq_length), 0), [batch_size, 1])  # => batch_size * seq_length
         position_enc = np.array(
             [[pos / np.power(10000, (i - i % 2) / E) for i in range(E)] for pos in range(self.max_len)]
@@ -129,27 +131,27 @@
         super(PositionalEncoding, self).__init__()
         self.max_len = max_len
 
     def build(self, input_shape):
         super(PositionalEncoding, self).build(input_shape)
 
     def call(self, x, masking=True):
-        """_summary_
+        """Applies positional encoding to the input tensor.
 
         Parameters
         ----------
-        x : _type_
-            _description_
+        x : tf.Tensor
+            The input tensor of shape (batch_size, seq_length, embed_dim).
         masking : bool, optional
-            _description_, by default True
+            Whether to mask padded values, by default True.
 
         Returns
         -------
-        _type_
-            _description_
+        tf.Tensor
+            The output tensor of shape (batch_size, seq_length, embed_dim) with positional encoding applied.
         """
         E = x.get_shape().as_list()[-1]  # static
         batch_size, seq_length = tf.shape(x)[0], tf.shape(x)[1]  # dynamic
         with tf.name_scope("position_encode"):
             # # => batch_size * seq_length
             position_ind = tf.tile(tf.expand_dims(tf.range(seq_length), 0), [batch_size, 1])
             position_enc = np.array(
@@ -171,26 +173,32 @@
         return dict(list(base_config.items()) + list(config.items()))
 
 
 class FixedEmbedding(tf.keras.layers.Layer):
     def __init__(self) -> None:
         super().__init__()
 
+    def build(self, input_shape):
+        self.embed = tf.keras.layers.Embedding(input_dim=input_shape[1], output_dim=input_shape[2])
+        super().build(input_shape)
+
     def call(self, x, **kwargs):
-        """_summary_
+        """Perform the embedding lookup operation.
 
         Parameters
         ----------
-        x : _type_
-            _description_
+        x : tf.Tensor
+            The input tensor of shape (batch_size, seq_length).
+        kwargs : dict
+            Additional keyword arguments.
 
         Returns
         -------
-        _type_
-            _description_
+        tf.Tensor
+            The tensor of embeddings of shape (batch_size, seq_length, embedding_size).
         """
         return self.embed(x)
 
 
 class TemporalEmbedding(tf.keras.layers.Layer):
     # minute, hour, weekday, day, month
     def __init__(self, embed_size, embed_type="fixed") -> None:
@@ -209,35 +217,39 @@
             _description_
         """
         return
 
 
 class DataEmbedding(tf.keras.layers.Layer):
     def __init__(self, embed_size: int, dropout: float = 0.0):
+        """
+        Data Embedding layer.
+
+        Args:
+            embed_size (int): Embedding size for tokens.
+            dropout (float, optional): Dropout rate to apply. Defaults to 0.0.
+        """
         super(DataEmbedding, self).__init__()
         self.embed_size = embed_size
         self.value_embedding = TokenEmbedding(embed_size)
         self.positional_embedding = PositionalEncoding()
         self.dropout = Dropout(dropout)
 
     def build(self, input_shape):
         super(DataEmbedding, self).build(input_shape)
 
     def call(self, x):
-        """_summary_
+        """
+        Forward pass of the layer.
 
-        Parameters
-        ----------
-        x : _type_
-            _description_
+        Args:
+            x (tf.Tensor): Input tensor of shape (batch_size, seq_length).
 
-        Returns
-        -------
-        _type_
-            _description_
+        Returns:
+            tf.Tensor: Output tensor of shape (batch_size, seq_length, embed_size).
         """
         ve = self.value_embedding(x)
         pe = self.positional_embedding(ve)
         return self.dropout(ve + pe)
 
     def get_config(self):
         config = {"embed_size": self.embed_size}
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `tfts-0.0.5/tfts/layers/nbeats_layer.py` & `tfts-0.0.6/tfts/layers/nbeats_layer.py`

 * *Files 11% similar despite different names*

```diff
@@ -21,25 +21,26 @@
 
     def build(self, input_shape):
         self.layers = [Dense(self.hidden_size, activation="relu") for _ in range(self.n_block_layers)]
         self.theta = Dense(self.train_sequence_length + self.predict_sequence_length, use_bias=False, activation=None)
         super(GenericBlock, self).build(input_shape)
 
     def call(self, inputs):
-        """_summary_
+        """Compute the output of the Generic Block.
 
         Parameters
         ----------
-        inputs : _type_
-            _description_
+        inputs : tf.Tensor
+            A tensor of shape (batch_size, train_sequence_length, input_size)
 
         Returns
         -------
-        _type_
-            _description_
+        Tuple[tf.Tensor, tf.Tensor]
+            A tuple of two tensors, the first of shape (batch_size, train_sequence_length, output_size)
+            and the second of shape (batch_size, predict_sequence_length, output_size)
         """
         x = inputs
         for layer in self.layers:
             x = layer(x)
         x = self.theta(x)
         return x[:, : self.train_sequence_length], x[:, -self.predict_sequence_length :]
```

### Comparing `tfts-0.0.5/tfts/layers/unet_layer.py` & `tfts-0.0.6/tfts/layers/unet_layer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.5/tfts/models/auto_config.py` & `tfts-0.0.6/tfts/models/auto_config.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.5/tfts/models/auto_model.py` & `tfts-0.0.6/tfts/models/auto_model.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.5/tfts/models/autoformer.py` & `tfts-0.0.6/tfts/models/autoformer.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.5/tfts/models/bert.py` & `tfts-0.0.6/tfts/models/bert.py`

 * *Files 0% similar despite different names*

```diff
@@ -147,13 +147,13 @@
         # outputs = tf.math.cumsum(outputs, axis=1)
 
         # grafting
         # base = decoder_features[:, :, -1:]
         # outputs += base
 
         if self.params["skip_connect_circle"]:
-            x_mean = x[:, -self.predict_sequence_length :, :]
+            x_mean = x[:, -self.predict_sequence_length :, 0:1]
             outputs = outputs + x_mean
         if self.params["skip_connect_mean"]:
-            x_mean = tf.tile(tf.reduce_mean(x, axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
+            x_mean = tf.tile(tf.reduce_mean(x[..., 0:1], axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
             outputs = outputs + x_mean
         return outputs
```

### Comparing `tfts-0.0.5/tfts/models/deepar.py` & `tfts-0.0.6/tfts/models/deepar.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.5/tfts/models/informer.py` & `tfts-0.0.6/tfts/models/wavenet.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,99 +1,62 @@
 """
-`Informer: Beyond Efficient Transformer for Long Sequence Time-Series Forecasting
-<https://arxiv.org/abs/2012.07436>`_
+`WaveNet: A Generative Model for Raw Audio
+<https://arxiv.org/abs/1609.03499>`_
 """
 
 from typing import Any, Callable, Dict, Optional, Tuple, Type
 
+import numpy as np
 import tensorflow as tf
-from tensorflow.keras.layers import (
-    Activation,
-    BatchNormalization,
-    Conv1D,
-    Dense,
-    Dropout,
-    LayerNormalization,
-    MaxPool1D,
-)
+from tensorflow.keras.layers import Dense
 
-from tfts.layers.attention_layer import FullAttention, SelfAttention
-from tfts.layers.embed_layer import DataEmbedding, TokenEmbedding
+from tfts.layers.attention_layer import FullAttention
+from tfts.layers.cnn_layer import ConvTemp
+from tfts.layers.dense_layer import DenseTemp
 
 params = {
-    "n_encoder_layers": 1,
-    "n_decoder_layers": 1,
-    "attention_hidden_sizes": 32 * 1,
-    "num_heads": 1,
-    "attention_dropout": 0.0,
-    "ffn_hidden_sizes": 32 * 1,
-    "ffn_filter_sizes": 32 * 1,
-    "ffn_dropout": 0.0,
+    "dilation_rates": [2**i for i in range(3)],
+    "kernel_sizes": [2 for _ in range(3)],
+    "filters": 32,
+    "dense_hidden_size": 32,
+    "scheduler_sampling": 1,  # 0 means teacher forcing, 1 means use last prediction
+    "use_attention": False,
     "skip_connect_circle": False,
     "skip_connect_mean": False,
 }
 
 
-class Informer(object):
-    """Informer model for time series"""
+class WaveNet(object):
+    """WaveNet model for time series"""
 
     def __init__(
         self,
         predict_sequence_length: int = 1,
         custom_model_params: Optional[Dict[str, Any]] = None,
         custom_model_head: Optional[Callable] = None,
     ):
-        """
-
-        :param custom_model_params: _description_
-        :type custom_model_params: _type_
-        :param dynamic_decoding: _description_, defaults to True
-        :type dynamic_decoding: bool, optional
-        """
         if custom_model_params:
             params.update(custom_model_params)
         self.params = params
         self.predict_sequence_length = predict_sequence_length
-        self.encoder_embedding = TokenEmbedding(params["attention_hidden_sizes"])
-        self.decoder_embedding = TokenEmbedding(params["attention_hidden_sizes"])
         self.encoder = Encoder(
-            layers=[
-                EncoderLayer(
-                    attention_hidden_sizes=params["attention_hidden_sizes"],
-                    num_heads=params["num_heads"],
-                    attention_dropout=params["attention_dropout"],
-                    ffn_dropout=params["ffn_dropout"],
-                    ffn_hidden_sizes=params["ffn_hidden_sizes"],
-                )
-                for _ in range(params["n_encoder_layers"])
-            ],
-            # conv_layers = [
-            #     CustomConv(
-            #         filters=params['attention_hidden_sizes']
-            #     ) for _ in range(params['n_encoder_layers'] - 1)
-            # ],
-            norm_layer=LayerNormalization(),
+            kernel_sizes=params["kernel_sizes"],
+            dilation_rates=params["dilation_rates"],
+            filters=params["filters"],
+            dense_hidden_size=params["dense_hidden_size"],
         )
-        self.decoder = Decoder(
-            layers=[
-                DecoderLayer(
-                    attention_hidden_sizes=params["attention_hidden_sizes"],
-                    num_heads=params["num_heads"],
-                    attention_dropout=params["attention_dropout"],
-                    ffn_dropout=params["ffn_dropout"],
-                    ffn_hidden_sizes=params["ffn_hidden_sizes"],
-                )
-                for _ in range(params["n_decoder_layers"])
-            ]
+        self.decoder = Decoder1(
+            filters=params["filters"],
+            dilation_rates=params["dilation_rates"],
+            dense_hidden_size=params["dense_hidden_size"],
+            predict_sequence_length=predict_sequence_length,
         )
-        self.projection = Dense(1)
-        # self.projection = Dense(predict_sequence_length, activation=None)
 
     def __call__(self, inputs, teacher=None):
-        """Informer call fucntion
+        """wavenet call
 
         Parameters
         ----------
         inputs : _type_
             _description_
         teacher : _type_, optional
             _description_, by default None
@@ -110,258 +73,274 @@
             x = inputs["x"]
             encoder_feature = inputs["encoder_feature"]
             decoder_feature = inputs["decoder_feature"]
             encoder_feature = tf.concat([x, encoder_feature], axis=-1)
         else:
             encoder_feature = x = inputs
             decoder_feature = tf.cast(
-                tf.reshape(tf.range(self.predict_sequence_length), (-1, self.predict_sequence_length, 1)), tf.float32
+                tf.tile(
+                    tf.reshape(tf.range(self.predict_sequence_length), (1, self.predict_sequence_length, 1)),
+                    (tf.shape(encoder_feature)[0], 1, 1),
+                ),
+                tf.float32,
             )
 
-        encoder_feature = self.encoder_embedding(encoder_feature)  # batch * seq * embedding_size
-        memory = self.encoder(encoder_feature, mask=None)
-
-        decoder_feature = self.decoder_embedding(decoder_feature)
-        decoder_outputs = self.decoder(decoder_feature, memory=memory)
-        decoder_outputs = self.projection(decoder_outputs)
-        # decoder_outputs = decoder_outputs[:, -self.predict_sequence_length:, :]
+        encoder_state, encoder_outputs = self.encoder(encoder_feature)
+        decoder_outputs = self.decoder(
+            decoder_features=decoder_feature,
+            decoder_init_input=x[:, -1],
+            teacher=teacher,
+            encoder_outputs=encoder_outputs,
+        )
 
         if self.params["skip_connect_circle"]:
             x_mean = x[:, -self.predict_sequence_length :, 0:1]
             decoder_outputs = decoder_outputs + x_mean
         if self.params["skip_connect_mean"]:
-            x_mean = tf.tile(tf.reduce_mean(x[:, :, 0:1], axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
+            x_mean = tf.tile(tf.reduce_mean(x[..., 0:1], axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
             decoder_outputs = decoder_outputs + x_mean
         return decoder_outputs
 
 
-class Encoder(tf.keras.layers.Layer):
-    def __init__(self, layers, conv_layers=None, norm_layer=None) -> None:
-        super(Encoder, self).__init__()
-        self.layers = layers
-        self.conv_layers = conv_layers if conv_layers is not None else None
-        self.norm_layer = norm_layer
+class Encoder(object):
+    def __init__(self, kernel_sizes, filters, dilation_rates, dense_hidden_size):
+        self.filters = filters
+        self.conv_times = []
+        for i, (kernel_size, dilation) in enumerate(zip(kernel_sizes, dilation_rates)):
+            self.conv_times.append(
+                ConvTemp(filters=2 * filters, kernel_size=kernel_size, causal=True, dilation_rate=dilation)
+            )
+        self.dense_time1 = DenseTemp(hidden_size=filters, activation="tanh", name="encoder_dense_time1")
+        self.dense_time2 = DenseTemp(hidden_size=filters + filters, name="encoder_dense_time2")
+        self.dense_time3 = DenseTemp(hidden_size=dense_hidden_size, activation="relu", name="encoder_dense_time3")
+        self.dense_time4 = DenseTemp(hidden_size=1, name="encoder_dense_time_4")
+
+    def __call__(self, x):
+        inputs = self.dense_time1(inputs=x)
+
+        skip_outputs = []
+        conv_inputs = [inputs]
+        for conv_time in self.conv_times:
+            dilated_conv = conv_time(inputs)
+            conv_filter, conv_gate = tf.split(dilated_conv, 2, axis=2)
+            dilated_conv = tf.nn.tanh(conv_filter) * tf.nn.sigmoid(conv_gate)
+            outputs = self.dense_time2(inputs=dilated_conv)
+            skips, residuals = tf.split(outputs, [self.filters, self.filters], axis=2)
+            inputs += residuals
+            conv_inputs.append(inputs)  # batch_size * time_sequence_length * filters
+            skip_outputs.append(skips)
+
+        skip_outputs = tf.nn.relu(tf.concat(skip_outputs, axis=2))
+        h = self.dense_time3(skip_outputs)
+        # [batch_size, time_sequence_length, filters] * time_sequence_length
+        y_hat = self.dense_time4(h)
+        return y_hat, conv_inputs[:-1]
+
+
+class Decoder1(object):
+    def __init__(self, filters, dilation_rates, dense_hidden_size, predict_sequence_length=24):
+        self.predict_sequence_length = predict_sequence_length
+        self.dilation_rates = dilation_rates
+        self.dense1 = Dense(filters, activation="tanh")
+        self.dense2 = Dense(2 * filters, use_bias=True)
+        self.dense3 = Dense(2 * filters, use_bias=False)
+        self.dense4 = Dense(2 * filters)
+        self.dense5 = Dense(dense_hidden_size, activation="relu")
+        self.dense6 = Dense(1)
 
-    def call(self, x, mask=None):
-        """Informer encoder call function
+    def __call__(
+        self,
+        decoder_features,
+        decoder_init_input,
+        encoder_outputs,
+        teacher=None,
+        scheduler_sampling=0,
+        training=None,
+        **kwargs
+    ):
+        """_summary_
 
         Parameters
         ----------
-        x : _type_
+        decoder_features : _type_
+            _description_
+        decoder_init_input : _type_
             _description_
-        mask : _type_, optional
+        encoder_outputs : _type_
+            _description_
+        teacher : _type_, optional
+            _description_, by default None
+        scheduler_sampling : int, optional
+            _description_, by default 0
+        training : _type_, optional
             _description_, by default None
 
         Returns
         -------
         _type_
             _description_
         """
-        if self.conv_layers is not None:
-            for attn_layer, conv_layer in zip(self.layers, self.conv_layers):
-                x = attn_layer(x, mask)
-                x = conv_layer(x)
-            x = self.layers[-1](x, mask)
-
-        else:
-            for attn_layer in self.layers:
-                x = attn_layer(x, mask)
-
-        if self.norm_layer is not None:
-            x = self.norm_layer(x)
-        return x
+        decoder_outputs = []
+        prev_output = decoder_init_input  # the initial input for decoder
 
+        for i in range(self.predict_sequence_length):
+            if training:
+                p = np.random.uniform(low=0, high=1, size=1)[0]
+                if teacher is not None and p > scheduler_sampling:
+                    this_input = teacher[:, i : i + 1]
+                else:
+                    this_input = prev_output
+            else:
+                this_input = prev_output
+
+            if decoder_features is not None:
+                this_input = tf.concat([this_input, decoder_features[:, i]], axis=-1)
+
+            x = self.dense1(this_input)
+            skip_outputs = []
+
+            for i, dilation in enumerate(self.dilation_rates):
+                state = encoder_outputs[i][:, -dilation, :]
+                # use 2 dense layer to calculate a kernel=2 convolution
+                dilated_conv = self.dense2(state) + self.dense3(x)
+                conv_filter, conv_gate = tf.split(dilated_conv, 2, axis=1)
+                dilated_conv = tf.nn.tanh(conv_filter) * tf.nn.sigmoid(conv_gate)
+                out = self.dense4(dilated_conv)
+                skip, residual = tf.split(out, 2, axis=1)
+                x += residual
+                # x = residual
+                encoder_outputs[i] = tf.concat([encoder_outputs[i], tf.expand_dims(x, 1)], axis=1)
+                skip_outputs.append(skip)
+
+            skip_outputs = tf.nn.relu(tf.concat(skip_outputs, axis=1))
+            skip_outputs = self.dense5(skip_outputs)
+            this_output = self.dense6(skip_outputs)
+            decoder_outputs.append(this_output)
 
-class EncoderLayer(tf.keras.layers.Layer):
-    def __init__(self, attention_hidden_sizes, num_heads, attention_dropout, ffn_hidden_sizes, ffn_dropout) -> None:
-        super().__init__()
-        self.attention_hidden_sizes = attention_hidden_sizes
-        self.num_heads = num_heads
-        self.attention_dropout = attention_dropout
-        self.ffn_hidden_sizes = ffn_hidden_sizes
-        self.ffn_dropout = ffn_dropout
-
-    def build(self, input_shape):
-        self.attn_layer = SelfAttention(self.attention_hidden_sizes, self.num_heads, self.attention_dropout)
-        self.drop = Dropout(self.ffn_dropout)
-        self.norm1 = LayerNormalization()
-        self.conv1 = Conv1D(filters=self.ffn_hidden_sizes, kernel_size=1)
-        self.conv2 = Conv1D(filters=self.attention_hidden_sizes, kernel_size=1)
-        self.norm2 = LayerNormalization()
-        super(EncoderLayer, self).build(input_shape)
+        decoder_outputs = tf.concat(decoder_outputs, axis=1)
+        return tf.expand_dims(decoder_outputs, -1)
 
-    def call(self, x, mask=None):
-        """Informer encoder layer call
 
-        Parameters
-        ----------
-        x : _type_
-            _description_
-        mask : _type_, optional
-            _description_, by default None
+class Decoder2(object):
+    """Decoder need avoid future data leaks"""
 
-        Returns
-        -------
-        _type_
-            _description_
-        """
-        input = x
-        x = self.attn_layer(x, mask)
-        x = self.drop(x)
-        x = x + input
-
-        y = x = self.norm1(x)
-        y = self.conv1(y)
-        y = self.drop(y)
-        y = self.conv2(y)
-        y = self.drop(y)
-        y = x + y
-        y = self.norm2(y)
-        return y
-
-    def get_config(self):
-        config = {
-            "attention_hidden_sizes": self.attention_hidden_sizes,
-            "num_heads": self.num_heads,
-            "attention_dropout": self.attention_dropout,
-            "ffn_hidden_sizes": self.ffn_hidden_sizes,
-            "ffn_dropout": self.ffn_dropout,
-        }
-        base_config = super(EncoderLayer, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
-
-
-class CustomConv(tf.keras.layers.Layer):
-    def __init__(self, filters) -> None:
-        super().__init__()
+    def __init__(self, filters, dilation_rates, dense_hidden_size, predict_sequence_length=24):
         self.filters = filters
+        self.dilation_rates = dilation_rates
+        self.predict_sequence_length = predict_sequence_length
+        self.dense_1 = Dense(filters, activation="tanh", name="decoder_dense_1")
+        self.dense_2 = Dense(2 * filters, name="decoder_dense_2")
+        self.dense_3 = Dense(2 * filters, use_bias=False, name="decoder_dense_3")
+        self.dense_4 = Dense(2 * filters, name="decoder_dense_4")
+        self.dense_5 = Dense(dense_hidden_size, activation="relu", name="decoder_dense_5")
+        self.dense_6 = Dense(1, name="decoder_dense_6")
 
-    def build(self, input_shape):
-        self.conv = Conv1D(filters=self.filters, kernel_size=3, padding="same")
-        self.norm = BatchNormalization()
-        self.activation = Activation("elu")
-        self.pool = MaxPool1D(pool_size=3, strides=2, padding="same")
-        super(CustomConv, self).build(input_shape)
-
-    def call(self, x):
-        """Informer custom conv
+    def __call__(self, decoder_features, decoder_init_input, encoder_states, teacher=None):
+        """_summary_
 
         Parameters
         ----------
         x : _type_
             _description_
-
-        Returns
-        -------
-        _type_
+        decoder_feature : _type_
             _description_
-        """
-        x = self.conv(x)
-        x = self.norm(x)
-        x = self.activation(x)
-        x = self.pool(x)
-        return x
-
-
-class Decoder(tf.keras.layers.Layer):
-    def __init__(self, layers, norm_layer=None):
-        super().__init__()
-        self.layers = layers
-        self.norm = norm_layer
-
-    def call(self, x, memory=None, x_mask=None, memory_mask=None):
-        """Informer decoder call function
-
-        Parameters
-        ----------
-        x : _type_
+        encoder_states : _type_
             _description_
-        memory : _type_, optional
-            _description_, by default None
-        x_mask : _type_, optional
-            _description_, by default None
-        memory_mask : _type_, optional
+        predict_seq_length : _type_
+            _description_
+        teacher : _type_, optional
             _description_, by default None
 
         Returns
         -------
         _type_
             _description_
         """
-        for layer in self.layers:
-            x = layer(x, memory, x_mask, memory_mask)
 
-        if self.norm is not None:
-            x = self.norm(x)
-        return x
+        def cond_fn(time, prev_output, decoder_output_ta):
+            return time < self.predict_sequence_length
+
+        def body(time, prev_output, decoder_output_ta):
+            if time == 0 or teacher is None:
+                current_input = prev_output
+            else:
+                current_input = teacher[:, time - 1, :]
+
+            if decoder_features is not None:
+                current_feature = decoder_features[:, time, :]
+                current_input = tf.concat([current_input, current_feature], axis=1)
+
+            inputs = self.dense_1(current_input)
+
+            skip_outputs = []
+            for i, dilation in enumerate(self.dilation_rates):
+                state = encoder_states[i][:, -dilation, :]
+
+                dilated_conv = self.dense_2(state) + self.dense_3(inputs)
+                conv_filter, conv_gate = tf.split(dilated_conv, 2, axis=1)
+                dilated_conv = tf.nn.tanh(conv_filter) * tf.nn.sigmoid(conv_gate)
+                outputs = self.dense_4(dilated_conv)
+                skips, residuals = tf.split(outputs, [self.filters, self.filters], axis=1)
+                inputs += residuals
+                encoder_states[i] = tf.concat([encoder_states[i], tf.expand_dims(inputs, 1)], axis=1)
+                skip_outputs.append(skips)
+
+            skip_outputs = tf.nn.relu(tf.concat(skip_outputs, axis=1))
+            h = self.dense_5(skip_outputs)
+            y_hat = self.dense_6(h)
+            decoder_output_ta = decoder_output_ta.write(time, y_hat)
+            return time + 1, y_hat, decoder_output_ta
+
+        loop_init = [
+            tf.constant(0, dtype=tf.int32),
+            decoder_init_input,
+            tf.TensorArray(dtype=tf.float32, size=self.predict_sequence_length),
+        ]
+        _, _, decoder_outputs_ta = tf.while_loop(cond=cond_fn, body=body, loop_vars=loop_init)
+        decoder_outputs = decoder_outputs_ta.stack()
+        decoder_outputs = tf.transpose(decoder_outputs, [1, 0, 2])
+        return decoder_outputs
+
 
+class Decoder3(tf.keras.layers.Layer):
+    """Multi-steps static decoding"""
 
-class DecoderLayer(tf.keras.layers.Layer):
-    def __init__(self, attention_hidden_sizes, num_heads, attention_dropout, ffn_hidden_sizes, ffn_dropout) -> None:
-        super().__init__()
-        self.attention_hidden_sizes = attention_hidden_sizes
-        self.num_heads = num_heads
-        self.attention_dropout = attention_dropout
-        self.ffn_hidden_sizes = ffn_hidden_sizes
-        self.ffn_dropout = ffn_dropout
-
-    def build(self, input_shape):
-        self.attn1 = SelfAttention(self.attention_hidden_sizes, self.num_heads, self.attention_dropout)
-        self.attn2 = FullAttention(self.attention_hidden_sizes, self.num_heads, self.attention_dropout)
-        self.conv1 = Conv1D(filters=self.ffn_hidden_sizes, kernel_size=1)
-        self.conv2 = Conv1D(filters=self.attention_hidden_sizes, kernel_size=1)
-        self.drop = Dropout(self.ffn_dropout)
-        self.norm1 = LayerNormalization()
-        self.norm2 = LayerNormalization()
-        self.norm3 = LayerNormalization()
-        self.activation = Activation("relu")
-        super(DecoderLayer, self).build(input_shape)
+    def __init__(self, kernel_sizes, dilation_rates, filters, dense_size, **kwargs) -> None:
+        super(Decoder3, self).__init__()
+        self.dense = Dense(units=dense_size, activation=None)
 
-    def call(self, x, memory=None, x_mask=None, memory_mask=None):
-        """Informer decoder layer call function
+    def call(
+        self,
+        decoder_features,
+        decoder_init_input,
+        init_state,
+        teacher=None,
+        scheduler_sampling=0,
+        training=None,
+        **kwargs
+    ):
+        """_summary_
 
         Parameters
         ----------
-        x : _type_
+        decoder_features : _type_
             _description_
-        memory : _type_, optional
-            _description_, by default None
-        x_mask : _type_, optional
+        decoder_init_input : _type_
+            _description_
+        init_state : _type_
+            _description_
+        teacher : _type_, optional
             _description_, by default None
-        memory_mask : _type_, optional
+        scheduler_sampling : int, optional
+            _description_, by default 0
+        training : _type_, optional
             _description_, by default None
 
         Returns
         -------
         _type_
             _description_
         """
-        x0 = x
-        x = self.attn1(x, x_mask)
-        x = self.drop(x)
-        x = x + x0
-        x = self.norm1(x)
-
-        x1 = x
-        x = self.attn2(x, memory, memory, mask=memory_mask)
-        x = self.drop(x)
-        x = x + x1
-        x = self.norm2(x)
-
-        x2 = x
-        x = self.conv1(x)
-        x = self.activation(x)
-        x = self.drop(x)
-        x = self.conv2(x)
-        x = x + x2
-        return self.norm3(x)
-
-    def get_config(self):
-        config = {
-            "attention_hidden_sizes": self.attention_hidden_sizes,
-            "num_heads": self.num_heads,
-            "attention_dropout": self.attention_dropout,
-            "ffn_hidden_sizes": self.ffn_hidden_sizes,
-            "ffn_dropout": self.ffn_dropout,
-        }
-        base_config = super(DecoderLayer, self).get_config()
-        return dict(list(base_config.items()) + list(config.items()))
+
+        x = self.rnn(decoder_features, initial_state=init_state)
+        x = self.dense(x)
+        return x
```

### Comparing `tfts-0.0.5/tfts/models/nbeats.py` & `tfts-0.0.6/tfts/models/nbeats.py`

 * *Files identical despite different names*

### Comparing `tfts-0.0.5/tfts/models/rnn.py` & `tfts-0.0.6/tfts/models/rnn.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
         self.dense1 = Dense(128, activation="relu")
         self.bn = BatchNormalization()
         self.drop1 = Dropout(0.25)
         self.dense2 = Dense(128, activation="relu")
         self.drop2 = Dropout(0.25)
 
     def __call__(self, inputs, teacher=None):
-        """_summary_
+        """RNN model call
 
         Parameters
         ----------
         inputs : _type_
             _description_
         teacher : _type_, optional
             _description_, by default None
@@ -98,15 +98,15 @@
         outputs = self.project1(encoder_output)
         outputs = tf.expand_dims(outputs, -1)
 
         if self.params["skip_connect_circle"]:
             x_mean = x[:, -self.predict_sequence_length :, 0:1]
             outputs = outputs + x_mean
         if self.params["skip_connect_mean"]:
-            x_mean = tf.tile(tf.reduce_mean(x, axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
+            x_mean = tf.tile(tf.reduce_mean(x[..., 0:1], axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
             outputs = outputs + x_mean
         return outputs
 
 
 class Encoder(tf.keras.layers.Layer):
     def __init__(self, rnn_type, rnn_size, rnn_dropout=0, dense_size=32, **kwargs):
         super(Encoder, self).__init__(**kwargs)
```

### Comparing `tfts-0.0.5/tfts/models/seq2seq.py` & `tfts-0.0.6/tfts/models/seq2seq.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,18 +90,18 @@
             init_state=encoder_state,
             teacher=teacher,
             scheduler_sampling=self.params["scheduler_sampling"],
             encoder_output=encoder_outputs,
         )
 
         if self.params["skip_connect_circle"]:
-            x_mean = x[:, : self.predict_sequence_length, :]
+            x_mean = x[:, -self.predict_sequence_length :, 0:1]
             decoder_outputs = decoder_outputs + x_mean
         if self.params["skip_connect_mean"]:
-            x_mean = tf.tile(tf.reduce_mean(x, axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
+            x_mean = tf.tile(tf.reduce_mean(x[..., 0:1], axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
             decoder_outputs = decoder_outputs + x_mean
         return decoder_outputs
 
 
 class Encoder(tf.keras.layers.Layer):
     def __init__(self, rnn_type, rnn_size, rnn_dropout=0, dense_size=32, **kwargs):
         super(Encoder, self).__init__(**kwargs)
```

### Comparing `tfts-0.0.5/tfts/models/tcn.py` & `tfts-0.0.6/tfts/models/tcn.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,18 +94,18 @@
         outputs = self.project1(encoder_output)
         outputs = tf.expand_dims(outputs, -1)
 
         # outputs = tf.tile(outputs, (1, self.predict_sequence_length, 1))   # stupid
         # outputs = self.dense3(encoder_outputs)
 
         if self.params["skip_connect_circle"]:
-            x_mean = x[:, -self.predict_sequence_length :, :]
+            x_mean = x[:, -self.predict_sequence_length :, 0:1]
             outputs = outputs + x_mean
         if self.params["skip_connect_mean"]:
-            x_mean = tf.tile(tf.reduce_mean(x, axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
+            x_mean = tf.tile(tf.reduce_mean(x[..., 0:1], axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
             outputs = outputs + x_mean
         return outputs
 
 
 class Encoder(object):
     def __init__(self, kernel_sizes, dilation_rates, filters, dense_hidden_size):
         self.filters = filters
```

### Comparing `tfts-0.0.5/tfts/models/transformer.py` & `tfts-0.0.6/tfts/models/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,18 +126,18 @@
         memory = self.encoder(encoder_feature, src_mask=None)
 
         # decoder_outputs = self.decoder(decoder_features, init_input=x[:, -1:], encoder_memory=memory, teacher=teacher)
         decoder_outputs = self.decoder(decoder_feature, memory)
         decoder_outputs = self.project(decoder_outputs)
 
         if self.params["skip_connect_circle"]:
-            x_mean = x[:, -self.predict_sequence_length :, :]
+            x_mean = x[:, -self.predict_sequence_length :, 0:1]
             decoder_outputs = decoder_outputs + x_mean
         if self.params["skip_connect_mean"]:
-            x_mean = tf.tile(tf.reduce_mean(x, axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
+            x_mean = tf.tile(tf.reduce_mean(x[..., 0:1], axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
             decoder_outputs = decoder_outputs + x_mean
         return decoder_outputs
 
 
 class Encoder(tf.keras.layers.Layer):
     def __init__(
         self,
@@ -232,15 +232,15 @@
             ffn_dropout,
         )
         self.projection = Dense(units=1, name="final_projection")
 
     def call(
         self, decoder_features, init_input, encoder_memory, teacher=None, scheduler_sampling=0, training=None, **kwargs
     ):
-        """_summary_
+        """Transformer decoder
 
         Parameters
         ----------
         decoder_features : _type_
             _description_
         init_input : _type_
             _description_
```

### Comparing `tfts-0.0.5/tfts/models/unet.py` & `tfts-0.0.6/tfts/models/unet.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,23 +52,23 @@
         _type_
             _description_
         """
         pool1 = self.AvgPool1D1(x)
         pool2 = self.AvgPool1D2(x)
 
         encoder_output = self.encoder([x, pool1, pool2])
-        decoder_output = self.decoder(encoder_output, predict_seq_length=self.predict_sequence_length)
+        decoder_outputs = self.decoder(encoder_output, predict_seq_length=self.predict_sequence_length)
 
         if self.params["skip_connect_circle"]:
-            x_mean = x[:, -self.predict_sequence_length :, :]
-            decoder_output = decoder_output + x_mean
+            x_mean = x[:, -self.predict_sequence_length :, 0:1]
+            decoder_outputs = decoder_outputs + x_mean
         if self.params["skip_connect_mean"]:
-            x_mean = tf.tile(tf.reduce_mean(x, axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
-            decoder_output = decoder_output + x_mean
-        return decoder_output
+            x_mean = tf.tile(tf.reduce_mean(x[..., 0:1], axis=1, keepdims=True), [1, self.predict_sequence_length, 1])
+            decoder_outputs = decoder_outputs + x_mean
+        return decoder_outputs
 
 
 class Encoder(object):
     def __init__(self):
         pass
 
     def __call__(self, input_tensor, units=64, kernel_size=2, depth=2):
```

### Comparing `tfts-0.0.5/tfts/trainer.py` & `tfts-0.0.6/tfts/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 """tfts Trainer"""
 
+from collections.abc import Iterable
 import logging
 from typing import Any, Callable, Dict, Optional, Tuple, Type, Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import tensorflow as tf
@@ -69,15 +70,15 @@
             _description_, by default False
         stop_no_improve_epochs : _type_, optional
             if None, no early stop; otherwise, training will stop after no_improve_epochs, by default None
         transform : _type_, optional
             _description_, by default None
         """
         self.learning_rate = learning_rate
-        self.eval_metric = eval_metric
+        self.eval_metric = eval_metric if isinstance(eval_metric, Iterable) else [eval_metric]
         self.use_ema = use_ema
         self.transform = transform
         self.global_step = tf.Variable(0, trainable=False, dtype=tf.int32)
 
         if use_ema:
             self.ema = tf.train.ExponentialMovingAverage(0.9).apply(self.model.trainable_variables)
```

### Comparing `tfts-0.0.5/setup.py` & `tfts-0.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,30 +1,307 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tfts
+Version: 0.0.6
+Summary: Deep learning time series with TensorFlow
+Home-page: https://time-series-prediction.readthedocs.io
+Author: Longxing Tan
+Requires-Python: >=3.7.1,<3.11
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Topic :: Scientific/Engineering
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Libraries
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: matplotlib
+Requires-Dist: numpy
+Requires-Dist: optuna (>=2.3.0,<3.0.0)
+Requires-Dist: pandas (>=1.2.0,<2.0.0)
+Project-URL: Documentation, https://time-series-prediction.readthedocs.io
+Project-URL: Repository, https://github.com/LongxingTan/Time-series-prediction
+Description-Content-Type: text/markdown
 
-packages = \
-['tfts', 'tfts.datasets', 'tfts.features', 'tfts.layers', 'tfts.models']
+[license-image]: https://img.shields.io/badge/License-MIT-blue.svg
+[license-url]: https://opensource.org/licenses/MIT
+[pypi-image]: https://badge.fury.io/py/tfts.svg
+[pypi-url]: https://pypi.python.org/pypi/tfts
+[pepy-image]: https://pepy.tech/badge/tfts/month
+[pepy-url]: https://pepy.tech/project/tfts
+[build-image]: https://github.com/LongxingTan/Time-series-prediction/actions/workflows/test.yml/badge.svg?branch=master
+[build-url]: https://github.com/LongxingTan/Time-series-prediction/actions/workflows/test.yml?query=branch%3Amaster
+[lint-image]: https://github.com/LongxingTan/Time-series-prediction/actions/workflows/lint.yml/badge.svg?branch=master
+[lint-url]: https://github.com/LongxingTan/Time-series-prediction/actions/workflows/lint.yml?query=branch%3Amaster
+[docs-image]: https://readthedocs.org/projects/time-series-prediction/badge/?version=latest
+[docs-url]: https://time-series-prediction.readthedocs.io/en/latest/?version=latest
+[coverage-image]: https://codecov.io/gh/longxingtan/Time-series-prediction/branch/master/graph/badge.svg
+[coverage-url]: https://codecov.io/github/longxingtan/Time-series-prediction?branch=master
+[contributing-image]: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat
+[contributing-url]: https://github.com/longxingtan/Time-series-prediction/blob/master/CONTRIBUTING.md
+[codeql-image]: https://github.com/longxingtan/Time-series-prediction/actions/workflows/codeql-analysis.yml/badge.svg
+[codeql-url]: https://github.com/longxingtan/Time-series-prediction/actions/workflows/codeql-analysis.yml
 
-package_data = \
-{'': ['*']}
+<h1 align="center">
+<img src="./docs/source/_static/logo.svg" width="490" align=center/>
+</h1><br>
 
-install_requires = \
-['matplotlib', 'numpy', 'optuna>=2.3.0,<3.0.0', 'pandas>=1.2.0,<2.0.0']
-
-setup_kwargs = {
-    'name': 'tfts',
-    'version': '0.0.5',
-    'description': 'Deep learning time series with TensorFlow',
-    'long_description': '[license-image]: https://img.shields.io/badge/License-MIT-blue.svg\n[license-url]: https://opensource.org/licenses/MIT\n[pypi-image]: https://badge.fury.io/py/tfts.svg\n[pypi-url]: https://pypi.python.org/pypi/tfts\n[pepy-image]: https://pepy.tech/badge/tfts/month\n[pepy-url]: https://pepy.tech/project/tfts\n[build-image]: https://github.com/LongxingTan/Time-series-prediction/actions/workflows/test.yml/badge.svg?branch=master\n[build-url]: https://github.com/LongxingTan/Time-series-prediction/actions/workflows/test.yml?query=branch%3Amaster\n[lint-image]: https://github.com/LongxingTan/Time-series-prediction/actions/workflows/lint.yml/badge.svg?branch=master\n[lint-url]: https://github.com/LongxingTan/Time-series-prediction/actions/workflows/lint.yml?query=branch%3Amaster\n[docs-image]: https://readthedocs.org/projects/time-series-prediction/badge/?version=latest\n[docs-url]: https://time-series-prediction.readthedocs.io/en/latest/?version=latest\n[coverage-image]: https://codecov.io/gh/longxingtan/Time-series-prediction/branch/master/graph/badge.svg\n[coverage-url]: https://codecov.io/github/longxingtan/Time-series-prediction?branch=master\n[contributing-image]: https://img.shields.io/badge/contributions-welcome-brightgreen.svg?style=flat\n[contributing-url]: https://github.com/longxingtan/Time-series-prediction/blob/master/CONTRIBUTING.md\n[codeql-image]: https://github.com/longxingtan/Time-series-prediction/actions/workflows/codeql-analysis.yml/badge.svg\n[codeql-url]: https://github.com/longxingtan/Time-series-prediction/actions/workflows/codeql-analysis.yml\n\n<h1 align="center">\n<img src="./docs/source/_static/logo.svg" width="490" align=center/>\n</h1><br>\n\n[![LICENSE][license-image]][license-url]\n[![PyPI Version][pypi-image]][pypi-url]\n[![Download][pepy-image]][pepy-url]\n[![Build Status][build-image]][build-url]\n[![Lint Status][lint-image]][lint-url]\n[![Docs Status][docs-image]][docs-url]\n[![Code Coverage][coverage-image]][coverage-url]\n[![Contributing][contributing-image]][contributing-url]\n[![CodeQL Status][codeql-image]][codeql-url]\n\n**[Documentation](https://time-series-prediction.readthedocs.io)** | **[Tutorials](https://time-series-prediction.readthedocs.io/en/latest/tutorials.html)** | **[Release Notes](https://time-series-prediction.readthedocs.io/en/latest/CHANGELOG.html)** | **[中文](https://github.com/LongxingTan/Time-series-prediction/blob/master/README_CN.md)**\n\n**TFTS** (TensorFlow Time Series) is an easy-to-use python package for time series, supporting the classical and SOTA deep learning methods in TensorFlow or Keras.\n- Flexible and powerful design for time series task\n- Advanced deep learning models for industry, research and competition\n- Documentation lives at [time-series-prediction.readthedocs.io](https://time-series-prediction.readthedocs.io)\n\n## Tutorial\n\n**Installation**\n\n- python >= 3.7\n- tensorflow >= 2.4\n\n``` bash\n$ pip install tfts\n```\n\n**Basic usage**\n\n[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LHdbrXmQGBSQuNTsbbM5-lAk5WENWF-Q?usp=sharing)\n\n``` python\nimport matplotlib.pyplot as plt\nimport tfts\nfrom tfts import AutoModel, AutoConfig, KerasTrainer\n\ntrain_length = 24\npredict_length = 8\n(x_train, y_train), (x_valid, y_valid) = tfts.get_data("sine", train_length, predict_length, test_size=0.2)\n\nmodel = AutoModel("seq2seq", predict_length=predict_length)\ntrainer = KerasTrainer(model)\ntrainer.train((x_train, y_train), (x_valid, y_valid), n_epochs=3)\n\npred = trainer.predict(x_valid)\ntrainer.plot(history=x_valid, true=y_valid, pred=pred)\nplt.show()\n```\n\n**Prepare your own data**\n\nYou could train your own data by preparing 3D data as inputs, for both inputs and targets\n\n- option1 `np.ndarray`\n- option2 `tf.data.Dataset`\n\nEncoder only model inputs\n\n```python\ntrain_length = 49\npredict_length = 10\nn_feature = 2\n\nx_train = np.random.rand(1, train_length, n_feature)  # feature: (n, train_length, feature)\ny_train = np.random.rand(1, predict_length, 1)  # y: (n, predict_length, 1)\nx_valid = np.random.rand(1, train_length, n_feature)\ny_valid = np.random.rand(1, predict_length, 1)\n\nmodel = AutoModel("rnn", predict_length=predict_length)\ntrainer = KerasTrainer(model)\ntrainer.train(train_dataset=(x_train, y_train), valid_dataset=(x_valid, y_valid), n_epochs=1)\n\n```\n\nEncoder-decoder model inputs\n\n```python\n# option1: np.ndarray\n\ntrain_length = 49\npredict_length = 10\nn_encoder_feature = 2\nn_decoder_feature = 3\n\nx_train = (\n    np.random.rand(1, train_length, 1),  # x: (n, train_length, 1)\n    np.random.rand(1, train_length, n_encoder_feature),  # encoder_feature: (n, train_length, encoder_features)\n    np.random.rand(1, predict_length, n_decoder_feature),  # decoder_feature: (n, predict_length, decoder_features)\n)\ny_train = np.random.rand(1, predict_length, 1)  # y: (n, predict_length, 1)\nx_valid = (\n    np.random.rand(1, train_length, 1),\n    np.random.rand(1, train_length, n_encoder_feature),\n    np.random.rand(1, predict_length, n_decoder_feature),\n)\ny_valid = np.random.rand(1, predict_length, 1)\n\nmodel = AutoModel("seq2seq", predict_length=predict_length)\ntrainer = KerasTrainer(model)\ntrainer.train((x_train, y_train), (x_valid, y_valid), n_epochs=1)\n```\n\n```python\n# option2: tf.data.Dataset\n\nclass FakeReader(object):\n    def __init__(self, predict_length=10):\n        train_length = 49\n        n_encoder_feature = 2\n        n_decoder_feature = 3\n        self.x = np.random.rand(15, train_length, 1)\n        self.encoder_feature = np.random.rand(15, train_length, n_encoder_feature)\n        self.decoder_feature = np.random.rand(15, predict_length, n_decoder_feature)\n        self.target = np.random.rand(15, predict_length, 1)\n\n    def __len__(self):\n        return len(self.x)\n\n    def __getitem__(self, idx):\n        return {\n            "x": self.x[idx],\n            "encoder_feature": self.encoder_feature[idx],\n            "decoder_feature": self.decoder_feature[idx],\n        }, self.target[idx]\n\n    def iter(self):\n        for i in range(len(self.x)):\n            yield self[i]\n\n\npredict_length = 10\ntrain_reader = FakeReader(predict_length=10)\ntrain_loader = tf.data.Dataset.from_generator(\n    train_reader.iter,\n    ({"x": tf.float32, "encoder_feature": tf.float32, "decoder_feature": tf.float32}, tf.float32),\n)\ntrain_loader = train_loader.batch(batch_size=1)\nvalid_reader = FakeReader(predict_length=10)\nvalid_loader = tf.data.Dataset.from_generator(\n    valid_reader.iter,\n    ({"x": tf.float32, "encoder_feature": tf.float32, "decoder_feature": tf.float32}, tf.float32),\n)\nvalid_loader = valid_loader.batch(batch_size=1)\n\nmodel = AutoModel("seq2seq", predict_length=predict_length)\ntrainer = KerasTrainer(model)\ntrainer.train(train_dataset=train_loader, valid_dataset=valid_loader, n_epochs=1)\n```\n\n**Build your own model**\n\nThe models tfts support to use in `AutoModel()`\n- rnn\n- tcn\n- bert\n- nbeats\n- seq2seq\n- wavenet\n- transformer\n\nYou could build the model based on tfts backbone, especially\n- add custom-defined embeddings for categorical variables\n- add custom-defined head layers for classification or anomaly task\n\n```python\nimport tensorflow as tf\nfrom tensorflow.keras.layers import Input, Dense\nfrom tfts import AutoModel\n\n\ndef build_model():\n    train_length = 24\n    train_features = 15\n    predict_length = 16\n\n    inputs = Input([train_length, train_features])\n    backbone = AutoModel("seq2seq", predict_length=predict_length)\n    outputs = backbone(inputs)\n    outputs = Dense(1, activation="sigmoid")(outputs)\n    model = tf.keras.Model(inputs=inputs, outputs=outputs)\n    model.compile(loss="mse", optimizer="rmsprop")\n    return model\n```\n\n## Examples\n\n- [TFTS-Bert](https://github.com/LongxingTan/KDDCup2022-Baidu) wins the **3rd place** in KDD Cup 2022 Baidu-wind power forecasting\n- [TFTS-Seq2seq](https://github.com/LongxingTan/Data-competitions/tree/master/tianchi-enso-prediction) wins the **4th place** in Alibaba Tianchi-ENSO prediction 2021\n\n<!-- ### Performance\n\n[Time series prediction](./examples/run_prediction.py) performance is evaluated by tfts implementation, not official\n\n| Performance | [web traffic<sup>mape</sup>]() | [grocery sales<sup>wrmse</sup>](https://www.kaggle.com/competitions/favorita-grocery-sales-forecasting/data) | [m5 sales<sup>val</sup>]() | [ventilator<sup>val</sup>]() |\n| :-- | :-: | :-: | :-: | :-: |\n| [RNN]() | 672 | 47.7% |52.6% | 61.4% |\n| [DeepAR]() | 672 | 47.7% |52.6% | 61.4% |\n| [Seq2seq]() | 672 | 47.7% |52.6% | 61.4% |\n| [TCN]() | 672 | 47.7% |52.6% | 61.4% |\n| [WaveNet]() | 672 | 47.7% |52.6% | 61.4% |\n| [Bert]() | 672 | 47.7% |52.6% | 61.4% |\n| [Transformer]() | 672 | 47.7% |52.6% | 61.4% |\n| [Temporal-fusion-transformer]() | 672 | 47.7% |52.6% | 61.4% |\n| [Informer]() | 672 | 47.7% |52.6% | 61.4% |\n| [AutoFormer]() | 672 | 47.7% |52.6% | 61.4% |\n| [N-beats]() | 672 | 47.7% |52.6% | 61.4% |\n| [U-Net]() | 672 | 47.7% |52.6% | 61.4% |\n\n### More demos\n- [More complex prediction task](./notebooks)\n- [Time series classification](./examples/run_classification.py)\n- [Anomaly detection](./examples/run_anomaly.py)\n- [Uncertainty prediction](examples/run_uncertainty.py)\n- [Parameters tuning by optuna](examples/run_optuna_tune.py)\n- [Serving by tf-serving](./examples) -->\n\nif you prefer other DL frameworks, try [pytorch-forecasting](https://github.com/jdb78/pytorch-forecasting), [gluonts](https://github.com/awslabs/gluonts), [paddlets](https://github.com/PaddlePaddle/PaddleTS)\n\n## Citation\n\nIf you find tfts project useful in your research, please consider cite:\n\n```\n@misc{tfts2020,\n  author = {Longxing Tan},\n  title = {Time series prediction},\n  year = {2020},\n  publisher = {GitHub},\n  journal = {GitHub repository},\n  howpublished = {\\url{https://github.com/longxingtan/time-series-prediction}},\n}\n```\n',
-    'author': 'Longxing Tan',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://time-series-prediction.readthedocs.io',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.1,<3.11',
+[![LICENSE][license-image]][license-url]
+[![PyPI Version][pypi-image]][pypi-url]
+[![Download][pepy-image]][pepy-url]
+[![Build Status][build-image]][build-url]
+[![Lint Status][lint-image]][lint-url]
+[![Docs Status][docs-image]][docs-url]
+[![Code Coverage][coverage-image]][coverage-url]
+[![Contributing][contributing-image]][contributing-url]
+[![CodeQL Status][codeql-image]][codeql-url]
+
+**[Documentation](https://time-series-prediction.readthedocs.io)** | **[Tutorials](https://time-series-prediction.readthedocs.io/en/latest/tutorials.html)** | **[Release Notes](https://time-series-prediction.readthedocs.io/en/latest/CHANGELOG.html)** | **[中文](https://github.com/LongxingTan/Time-series-prediction/blob/master/README_CN.md)**
+
+**TFTS** (TensorFlow Time Series) is an easy-to-use python package for time series, supporting the classical and SOTA deep learning methods in TensorFlow or Keras.
+- Flexible and powerful design for time series task
+- Advanced deep learning models for industry, research and competition
+- Documentation lives at [time-series-prediction.readthedocs.io](https://time-series-prediction.readthedocs.io)
+
+## Tutorial
+
+**Installation**
+
+- python >= 3.7
+- tensorflow >= 2.4
+
+``` bash
+$ pip install tfts
+```
+
+**Basic usage**
+
+[![Open In Colab](https://colab.research.google.com/assets/colab-badge.svg)](https://colab.research.google.com/drive/1LHdbrXmQGBSQuNTsbbM5-lAk5WENWF-Q?usp=sharing)
+
+``` python
+import matplotlib.pyplot as plt
+import tfts
+from tfts import AutoModel, AutoConfig, KerasTrainer
+
+train_length = 24
+predict_length = 8
+(x_train, y_train), (x_valid, y_valid) = tfts.get_data("sine", train_length, predict_length, test_size=0.2)
+
+model = AutoModel("seq2seq", predict_length=predict_length)
+trainer = KerasTrainer(model)
+trainer.train((x_train, y_train), (x_valid, y_valid), n_epochs=3)
+
+pred = trainer.predict(x_valid)
+trainer.plot(history=x_valid, true=y_valid, pred=pred)
+plt.show()
+```
+
+**Prepare your own data**
+
+You could train your own data by preparing 3D data as inputs, for both inputs and targets
+
+- option1 `np.ndarray`
+- option2 `tf.data.Dataset`
+
+Encoder only model inputs
+
+```python
+train_length = 49
+predict_length = 10
+n_feature = 2
+
+x_train = np.random.rand(1, train_length, n_feature)  # inputs: (batch, train_length, feature)
+y_train = np.random.rand(1, predict_length, 1)  # target: (batch, predict_length, 1)
+x_valid = np.random.rand(1, train_length, n_feature)
+y_valid = np.random.rand(1, predict_length, 1)
+
+model = AutoModel("rnn", predict_length=predict_length)
+trainer = KerasTrainer(model)
+trainer.train(train_dataset=(x_train, y_train), valid_dataset=(x_valid, y_valid), n_epochs=1)
+
+```
+
+Encoder-decoder model inputs
+
+```python
+# option1: np.ndarray
+
+train_length = 49
+predict_length = 10
+n_encoder_feature = 2
+n_decoder_feature = 3
+
+x_train = (
+    np.random.rand(1, train_length, 1),  # inputs: (batch, train_length, 1)
+    np.random.rand(1, train_length, n_encoder_feature),  # encoder_feature: (batch, train_length, encoder_features)
+    np.random.rand(1, predict_length, n_decoder_feature),  # decoder_feature: (batch, predict_length, decoder_features)
+)
+y_train = np.random.rand(1, predict_length, 1)  # target: (batch, predict_length, 1)
+x_valid = (
+    np.random.rand(1, train_length, 1),
+    np.random.rand(1, train_length, n_encoder_feature),
+    np.random.rand(1, predict_length, n_decoder_feature),
+)
+y_valid = np.random.rand(1, predict_length, 1)
+
+model = AutoModel("seq2seq", predict_length=predict_length)
+trainer = KerasTrainer(model)
+trainer.train((x_train, y_train), (x_valid, y_valid), n_epochs=1)
+```
+
+```python
+# option2: tf.data.Dataset
+
+class FakeReader(object):
+    def __init__(self, predict_length):
+        train_length = 49
+        n_encoder_feature = 2
+        n_decoder_feature = 3
+        self.x = np.random.rand(15, train_length, 1)
+        self.encoder_feature = np.random.rand(15, train_length, n_encoder_feature)
+        self.decoder_feature = np.random.rand(15, predict_length, n_decoder_feature)
+        self.target = np.random.rand(15, predict_length, 1)
+
+    def __len__(self):
+        return len(self.x)
+
+    def __getitem__(self, idx):
+        return {
+            "x": self.x[idx],
+            "encoder_feature": self.encoder_feature[idx],
+            "decoder_feature": self.decoder_feature[idx],
+        }, self.target[idx]
+
+    def iter(self):
+        for i in range(len(self.x)):
+            yield self[i]
+
+
+predict_length = 10
+train_reader = FakeReader(predict_length=predict_length)
+train_loader = tf.data.Dataset.from_generator(
+    train_reader.iter,
+    ({"x": tf.float32, "encoder_feature": tf.float32, "decoder_feature": tf.float32}, tf.float32),
+)
+train_loader = train_loader.batch(batch_size=1)
+valid_reader = FakeReader(predict_length=predict_length)
+valid_loader = tf.data.Dataset.from_generator(
+    valid_reader.iter,
+    ({"x": tf.float32, "encoder_feature": tf.float32, "decoder_feature": tf.float32}, tf.float32),
+)
+valid_loader = valid_loader.batch(batch_size=1)
+
+model = AutoModel("seq2seq", predict_length=predict_length)
+trainer = KerasTrainer(model)
+trainer.train(train_dataset=train_loader, valid_dataset=valid_loader, n_epochs=1)
+```
+
+**Prepare custom model params**
+
+```python
+import tensorflow as tf
+import tfts
+from tfts import AutoModel, AutoConfig
+
+config = AutoConfig('rnn').get_config()
+print(config)
+
+custom_model_params = {
+    "rnn_size": 128,
+    "dense_size": 128,
 }
 
+model = AutoModel('rnn', predict_length=7, custom_model_params=custom_model_params)
+```
+
+**Build your own model**
+
+<details><summary> Full list of model tfts supported using AutoModel </summary>
+
+- rnn
+- tcn
+- bert
+- nbeats
+- seq2seq
+- wavenet
+- transformer
+
+</details>
+
+You could build the custom model based on tfts, especially
+- add custom-defined embeddings for categorical variables
+- add custom-defined head layers for classification or anomaly task
+
+```python
+import tensorflow as tf
+from tensorflow.keras.layers import Input, Dense
+from tfts import AutoModel
+
+
+def build_model():
+    train_length = 24
+    train_features = 15
+    predict_length = 16
+
+    inputs = Input([train_length, train_features])
+    backbone = AutoModel("seq2seq", predict_length=predict_length)
+    outputs = backbone(inputs)
+    outputs = Dense(1, activation="sigmoid")(outputs)
+    model = tf.keras.Model(inputs=inputs, outputs=outputs)
+    model.compile(loss="mse", optimizer="rmsprop")
+    return model
+```
+
+## Examples
+
+- [TFTS-Bert](https://github.com/LongxingTan/KDDCup2022-Baidu) wins the **3rd place** in KDD Cup 2022-wind power forecasting
+- [TFTS-Seq2seq](https://github.com/LongxingTan/Data-competitions/tree/master/tianchi-enso-prediction) wins the **4th place** in Tianchi-ENSO prediction 2021
+
+<!-- ### Performance
+
+[Time series prediction](./examples/run_prediction.py) performance is evaluated by tfts implementation, not official
+
+| Performance | [web traffic<sup>mape</sup>]() | [grocery sales<sup>wrmse</sup>](https://www.kaggle.com/competitions/favorita-grocery-sales-forecasting/data) | [m5 sales<sup>val</sup>]() | [ventilator<sup>val</sup>]() |
+| :-- | :-: | :-: | :-: | :-: |
+| [RNN]() | 672 | 47.7% |52.6% | 61.4% |
+| [DeepAR]() | 672 | 47.7% |52.6% | 61.4% |
+| [Seq2seq]() | 672 | 47.7% |52.6% | 61.4% |
+| [TCN]() | 672 | 47.7% |52.6% | 61.4% |
+| [WaveNet]() | 672 | 47.7% |52.6% | 61.4% |
+| [Bert]() | 672 | 47.7% |52.6% | 61.4% |
+| [Transformer]() | 672 | 47.7% |52.6% | 61.4% |
+| [Temporal-fusion-transformer]() | 672 | 47.7% |52.6% | 61.4% |
+| [Informer]() | 672 | 47.7% |52.6% | 61.4% |
+| [AutoFormer]() | 672 | 47.7% |52.6% | 61.4% |
+| [N-beats]() | 672 | 47.7% |52.6% | 61.4% |
+| [U-Net]() | 672 | 47.7% |52.6% | 61.4% |
+
+### More demos
+- [More complex prediction task](./notebooks)
+- [Time series classification](./examples/run_classification.py)
+- [Anomaly detection](./examples/run_anomaly.py)
+- [Uncertainty prediction](examples/run_uncertainty.py)
+- [Parameters tuning by optuna](examples/run_optuna_tune.py)
+- [Serving by tf-serving](./examples) -->
+
+For other DL frameworks, try [pytorch-forecasting](https://github.com/jdb78/pytorch-forecasting), [gluonts](https://github.com/awslabs/gluonts), [paddlets](https://github.com/PaddlePaddle/PaddleTS)
+
+## Citation
+
+If you find tfts project useful in your research, please consider cite:
+
+```
+@misc{tfts2020,
+  author = {Longxing Tan},
+  title = {Time series prediction},
+  year = {2020},
+  publisher = {GitHub},
+  journal = {GitHub repository},
+  howpublished = {\url{https://github.com/longxingtan/time-series-prediction}},
+}
+```
 
-setup(**setup_kwargs)
```

