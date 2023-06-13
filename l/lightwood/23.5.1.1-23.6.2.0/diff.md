# Comparing `tmp/lightwood-23.5.1.1.tar.gz` & `tmp/lightwood-23.6.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lightwood-23.5.1.1.tar", last modified: Wed Jun  7 04:40:16 2023, max compression
+gzip compressed data, was "lightwood-23.6.2.0.tar", last modified: Tue Jun 13 03:08:25 2023, max compression
```

## Comparing `lightwood-23.5.1.1.tar` & `lightwood-23.6.2.0.tar`

### file list

```diff
@@ -1,160 +1,160 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.790276 lightwood-23.5.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-06-07 04:40:16.790276 lightwood-23.5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.778276 lightwood-23.5.1.1/lightwood/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/__about__.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.778276 lightwood-23.5.1.1/lightwood/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/analyze.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/explain.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.778276 lightwood-23.5.1.1/lightwood/analysis/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/helpers/acc_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/helpers/conf_stats.py
--rw-r--r--   0 runner    (1001) docker     (123)     5052 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/helpers/feature_importance.py
--rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/helpers/pyod.py
--rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/helpers/shap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.778276 lightwood-23.5.1.1/lightwood/analysis/nc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/icp.py
--rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/nc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/norm.py
--rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nc/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/analysis/nn_conf/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nn_conf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/analysis/nn_conf/temp_scale.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/api/
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/api/high_level.py
--rw-r--r--   0 runner    (1001) docker     (123)    50128 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/api/json_ai.py
--rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/api/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/api/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/data/
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8132 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/data/encoded_ds.py
--rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/data/timeseries_analyzer.py
--rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/data/timeseries_transform.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/
--rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/array/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/array/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/array/array.py
--rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/array/ts_cat_array.py
--rw-r--r--   0 runner    (1001) docker     (123)     5533 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/array/ts_num_array.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/audio/
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/audio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/audio/mfcc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/base.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/categorical/
--rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/categorical/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/categorical/autoencoder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7187 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/categorical/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/categorical/gym.py
--rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/categorical/multihot.py
--rw-r--r--   0 runner    (1001) docker     (123)     7752 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/categorical/onehot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/datetime/
--rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/datetime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/datetime/datetime.py
--rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/datetime/datetime_sin_normalizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/identity/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/identity/identity.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/image/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/image/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/image/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/image/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/image/helpers/img_to_vec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/image/img_2_vec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.782276 lightwood-23.5.1.1/lightwood/encoder/numeric/
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/numeric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6398 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/numeric/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     4769 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/numeric/ts_numeric.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.786276 lightwood-23.5.1.1/lightwood/encoder/text/
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.786276 lightwood-23.5.1.1/lightwood/encoder/text/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/helpers/pretrained_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/helpers/rnn_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    13460 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/pretrained.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     3930 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/short.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/tfidf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/text/vocab.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.786276 lightwood-23.5.1.1/lightwood/encoder/time_series/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/time_series/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.786276 lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/rnn_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/transformer_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    23498 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/time_series/rnn.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/encoder/time_series/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.786276 lightwood-23.5.1.1/lightwood/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/best_of.py
--rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/mean_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/mode_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/stacked_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/ts_stacked_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/ensemble/weighted_mean_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.786276 lightwood-23.5.1.1/lightwood/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/general.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/io.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/log.py
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/parallelism.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/templating.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/text.py
--rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/torch.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/helpers/ts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.790276 lightwood-23.5.1.1/lightwood/mixer/
--rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/arima.py
--rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/ets.py
--rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.790276 lightwood-23.5.1.1/lightwood/mixer/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/ar_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/default_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/qclassic_net.py
--rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/ranger.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/residual_net.py
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/transform_corss_entropy_loss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/helpers/ts.py
--rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/lightgbm.py
--rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/lightgbm_array.py
--rw-r--r--   0 runner    (1001) docker     (123)    14962 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/neural.py
--rw-r--r--   0 runner    (1001) docker     (123)     7820 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/neural_ts.py
--rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/nhits.py
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/prophet.py
--rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/qclassic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9482 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/random_forest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4396 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/regression.py
--rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/sktime.py
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/tabtransformer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/lightwood/mixer/xgboost.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 04:40:16.778276 lightwood-23.5.1.1/lightwood.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-06-07 04:40:16.000000 lightwood-23.5.1.1/lightwood.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-06-07 04:40:16.000000 lightwood-23.5.1.1/lightwood.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 04:40:16.000000 lightwood-23.5.1.1/lightwood.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-06-07 04:40:16.000000 lightwood-23.5.1.1/lightwood.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-07 04:40:16.000000 lightwood-23.5.1.1/lightwood.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 04:40:16.790276 lightwood-23.5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-07 04:40:06.000000 lightwood-23.5.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.239579 lightwood-23.6.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35104 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-06-13 03:08:25.239579 lightwood-23.6.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11115 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.227579 lightwood-23.6.2.0/lightwood/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/__about__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)      883 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/analyze.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/explain.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/analysis/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7250 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/helpers/acc_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4305 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/helpers/conf_stats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5163 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/helpers/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3949 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/helpers/pyod.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4156 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/helpers/shap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/analysis/nc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29232 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16835 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/icp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5728 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22328 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/nc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5722 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/norm.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10049 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nc/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/analysis/nn_conf/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nn_conf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/analysis/nn_conf/temp_scale.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7889 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/api/high_level.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50810 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/api/json_ai.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7843 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/api/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24999 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/api/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10389 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/data/encoded_ds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9993 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/data/timeseries_analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16355 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/data/timeseries_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/encoder/
+-rw-r--r--   0 runner    (1001) docker     (123)     1760 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/encoder/array/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/array/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5366 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/array/array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4768 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/array/ts_cat_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4534 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/array/ts_num_array.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/encoder/audio/
+-rw-r--r--   0 runner    (1001) docker     (123)      226 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/audio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3575 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/audio/mfcc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3960 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood/encoder/categorical/
+-rw-r--r--   0 runner    (1001) docker     (123)      281 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/categorical/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7761 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/categorical/autoencoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8535 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/categorical/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4960 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/categorical/gym.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1439 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/categorical/multihot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7754 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/categorical/onehot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/datetime/
+-rw-r--r--   0 runner    (1001) docker     (123)      213 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/datetime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3618 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/datetime/datetime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4189 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/datetime/datetime_sin_normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2531 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/identity/identity.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/image/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/image/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/image/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/image/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2170 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/image/helpers/img_to_vec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4409 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/image/img_2_vec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/numeric/
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/numeric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/numeric/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4656 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/numeric/ts_numeric.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/text/
+-rw-r--r--   0 runner    (1001) docker     (123)      398 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/text/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/helpers/pretrained_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29481 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/helpers/rnn_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/pretrained.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3976 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/short.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/tfidf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1432 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/text/vocab.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/time_series/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/time_series/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/rnn_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5184 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/transformer_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23498 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/time_series/rnn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/encoder/time_series/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.235579 lightwood-23.6.2.0/lightwood/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      564 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1625 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3691 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/best_of.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1285 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/mean_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4042 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/mode_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3246 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/stacked_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2946 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/ts_stacked_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/ensemble/weighted_mean_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.239579 lightwood-23.6.2.0/lightwood/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1762 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1047 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/general.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2189 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/parallelism.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/templating.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/torch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11967 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/helpers/ts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.239579 lightwood-23.6.2.0/lightwood/mixer/
+-rw-r--r--   0 runner    (1001) docker     (123)     1414 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5159 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/arima.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3939 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3147 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/ets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11686 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.239579 lightwood-23.6.2.0/lightwood/mixer/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2320 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/ar_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/default_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/qclassic_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5526 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/ranger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/residual_net.py
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7062 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/helpers/ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15536 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/lightgbm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4523 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/lightgbm_array.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15938 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/neural.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7620 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/neural_ts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9238 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/nhits.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/prophet.py
+-rw-r--r--   0 runner    (1001) docker     (123)      930 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/qclassic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9092 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/regression.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18540 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/sktime.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/tabtransformer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12090 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/lightwood/mixer/xgboost.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 03:08:25.231579 lightwood-23.6.2.0/lightwood.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    13490 2023-06-13 03:08:25.000000 lightwood-23.6.2.0/lightwood.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4387 2023-06-13 03:08:25.000000 lightwood-23.6.2.0/lightwood.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 03:08:25.000000 lightwood-23.6.2.0/lightwood.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-06-13 03:08:25.000000 lightwood-23.6.2.0/lightwood.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-06-13 03:08:25.000000 lightwood-23.6.2.0/lightwood.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 03:08:25.239579 lightwood-23.6.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2141 2023-06-13 03:08:15.000000 lightwood-23.6.2.0/setup.py
```

### Comparing `lightwood-23.5.1.1/LICENSE` & `lightwood-23.6.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/PKG-INFO` & `lightwood-23.6.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 23.5.1.1
+Version: 23.6.2.0
 Summary: Lightwood is a toolkit for automatic machine learning model building
 Home-page: https://github.com/mindsdb/lightwood
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/lightwood
 Description: # Lightwood
```

### Comparing `lightwood-23.5.1.1/README.md` & `lightwood-23.6.2.0/README.md`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/__init__.py` & `lightwood-23.6.2.0/lightwood/analysis/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/analyze.py` & `lightwood-23.6.2.0/lightwood/analysis/analyze.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 from typing import Dict, List, Tuple, Optional
 
 from dataprep_ml import StatisticalAnalysis
 
 from lightwood.helpers.log import log
-from lightwood.helpers.ts import filter_ds
 from type_infer.dtype import dtype
 from lightwood.ensemble import BaseEnsemble
 from lightwood.analysis.base import BaseAnalysisBlock
 from lightwood.data.encoded_ds import EncodedDs
 from lightwood.encoder.text.pretrained import PretrainedLangEncoder
 from lightwood.api.types import ModelAnalysis, TimeseriesSettings, PredictionArguments
 
@@ -56,16 +55,14 @@
 
     # raw predictions for validation dataset
     args = {} if not is_classification else {"predict_proba": True}
     filtered_df = encoded_val_data.data_frame
     normal_predictions = None
 
     if len(analysis_blocks) > 0:
-        filtered_df = filter_ds(encoded_val_data, tss)
-        encoded_val_data = EncodedDs(encoded_val_data.encoders, filtered_df, encoded_val_data.target)
         normal_predictions = predictor(encoded_val_data, args=PredictionArguments.from_dict(args))
         normal_predictions = normal_predictions.set_index(encoded_val_data.data_frame.index)
 
     # ------------------------- #
     # Run analysis blocks, both core and user-defined
     # ------------------------- #
     kwargs = {
```

### Comparing `lightwood-23.5.1.1/lightwood/analysis/base.py` & `lightwood-23.6.2.0/lightwood/analysis/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/explain.py` & `lightwood-23.6.2.0/lightwood/analysis/explain.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/helpers/acc_stats.py` & `lightwood-23.6.2.0/lightwood/analysis/helpers/acc_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/helpers/conf_stats.py` & `lightwood-23.6.2.0/lightwood/analysis/helpers/conf_stats.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/helpers/feature_importance.py` & `lightwood-23.6.2.0/lightwood/analysis/helpers/feature_importance.py`

 * *Files 2% similar despite different names*

```diff
@@ -77,14 +77,15 @@
             else:
                 log.info(f"[PFI] Computing importance for all {len(shuffled_cols)} columns: {shuffled_cols}")
 
             for col in shuffled_cols:
                 shuffle_data = deepcopy(ref_data)
                 shuffle_data.clear_cache()
                 shuffle_data.data_frame[col] = shuffle(shuffle_data.data_frame[col].values)
+                shuffle_data.build_cache()  # TODO: bottleneck, add a method to build a single column instead!
 
                 shuffled_preds = ns.predictor(shuffle_data, args=PredictionArguments.from_dict(args))
                 shuffled_col_accuracy[col] = np.mean(list(evaluate_accuracies(
                     shuffle_data.data_frame,
                     shuffled_preds['prediction'],
                     ns.target,
                     ns.accuracy_functions
```

### Comparing `lightwood-23.5.1.1/lightwood/analysis/helpers/pyod.py` & `lightwood-23.6.2.0/lightwood/analysis/helpers/pyod.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/helpers/shap.py` & `lightwood-23.6.2.0/lightwood/analysis/helpers/shap.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/nc/base.py` & `lightwood-23.6.2.0/lightwood/analysis/nc/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/nc/calibrate.py` & `lightwood-23.6.2.0/lightwood/analysis/nc/calibrate.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/nc/icp.py` & `lightwood-23.6.2.0/lightwood/analysis/nc/icp.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/nc/metrics.py` & `lightwood-23.6.2.0/lightwood/analysis/nc/metrics.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/nc/nc.py` & `lightwood-23.6.2.0/lightwood/analysis/nc/nc.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/nc/norm.py` & `lightwood-23.6.2.0/lightwood/analysis/nc/norm.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/nc/util.py` & `lightwood-23.6.2.0/lightwood/analysis/nc/util.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/analysis/nn_conf/temp_scale.py` & `lightwood-23.6.2.0/lightwood/analysis/nn_conf/temp_scale.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/api/__init__.py` & `lightwood-23.6.2.0/lightwood/api/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/api/high_level.py` & `lightwood-23.6.2.0/lightwood/api/high_level.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/api/json_ai.py` & `lightwood-23.6.2.0/lightwood/api/json_ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
     tss = problem_defintion.timeseries_settings
     encoder_lookup = {
         dtype.integer: "NumericEncoder",
         dtype.float: "NumericEncoder",
         dtype.binary: "BinaryEncoder",
         dtype.categorical: "CategoricalAutoEncoder"
         if statistical_analysis is None
-        or len(statistical_analysis.histograms[col_name]) > 100
+        or len(statistical_analysis.histograms[col_name]['x']) > 16
         else "OneHotEncoder",
         dtype.tags: "MultiHotEncoder",
         dtype.date: "DatetimeEncoder",
         dtype.datetime: "DatetimeEncoder",
         dtype.image: "Img2VecEncoder",
         dtype.rich_text: "PretrainedLangEncoder",
         dtype.short_text: "CategoricalAutoEncoder",
@@ -613,15 +613,14 @@
                 "target_encoder", "$encoders[self.target]"
             )
 
         elif mixers[i]["module"] == "RandomForest":
             mixers[i]["args"]["target_encoder"] = mixers[i]["args"].get(
                 "target_encoder", "$encoders[self.target]"
             )
-            mixers[i]["args"]["use_optuna"] = True
 
         elif mixers[i]["module"] == "LightGBMArray":
             mixers[i]["args"]["input_cols"] = mixers[i]["args"].get(
                 "input_cols", "$input_cols"
             )
             mixers[i]["args"]["target_encoder"] = mixers[i]["args"].get(
                 "target_encoder", "$encoders[self.target]"
@@ -940,22 +939,25 @@
 
 prepped_encoders = {{}}
 
 # Prepare input encoders
 parallel_encoding = parallel_encoding_check(data['train'], self.encoders)
 
 if parallel_encoding:
+    log.debug('Preparing in parallel...')
     for col_name, encoder in self.encoders.items():
         if col_name != self.target and not encoder.is_trainable_encoder:
             prepped_encoders[col_name] = (encoder, concatenated_train_dev[col_name], 'prepare')
     prepped_encoders = mut_method_call(prepped_encoders)
 
 else:
+    log.debug('Preparing sequentially...')
     for col_name, encoder in self.encoders.items():
         if col_name != self.target and not encoder.is_trainable_encoder:
+            log.debug(f'Preparing encoder for {{col_name}}...')
             encoder.prepare(concatenated_train_dev[col_name])
             prepped_encoders[col_name] = encoder
 
 # Store encoders
 for col_name, encoder in prepped_encoders.items():
     self.encoders[col_name] = encoder
 
@@ -993,15 +995,30 @@
     # ----------------- #
     # Featurize Data Body
     # ----------------- #
 
     feature_body = f"""
 log.info('Featurizing the data')
 
-feature_data = {{ key: EncodedDs(self.encoders, data, self.target) for key, data in split_data.items() if key != "stratified_on"}}
+tss = self.problem_definition.timeseries_settings
+
+feature_data = dict()
+for key, data in split_data.items():
+    if key != 'stratified_on':
+
+        # compute and store two splits - full and filtered (useful for time series post-train analysis)
+        if key not in self.feature_cache:
+            featurized_split = EncodedDs(self.encoders, data, self.target)
+            filtered_subset = EncodedDs(self.encoders, filter_ts(data, tss), self.target)
+
+            for k, s in zip((key, f'{{key}}_filtered'), (featurized_split, filtered_subset)):
+                self.feature_cache[k] = s
+
+        for k in (key, f'{{key}}_filtered'):
+            feature_data[k] = self.feature_cache[k]
 
 return feature_data
 
 """  # noqa
 
     feature_body = align(feature_body, 2)
 
@@ -1014,17 +1031,15 @@
 
 # --------------- #
 # Extract data
 # --------------- #
 # Extract the featurized data into train/dev/test
 encoded_train_data = enc_data['train']
 encoded_dev_data = enc_data['dev']
-encoded_test_data = enc_data['test']
-filtered_df = filter_ds(encoded_test_data, self.problem_definition.timeseries_settings)
-encoded_test_data = EncodedDs(encoded_test_data.encoders, filtered_df, encoded_test_data.target)
+encoded_test_data = enc_data['test_filtered']
 
 log.info('Training the mixers')
 
 # --------------- #
 # Fit Models
 # --------------- #
 # Assign list of mixers
@@ -1170,14 +1185,15 @@
 # Update the mixers with partial fit
 if self.problem_definition.fit_on_all and all([not m.trains_once for m in self.mixers]):
     log.info(f'[Learn phase 8/{n_phases}] - Adjustment on validation requested')
     self.adjust(enc_train_test["test"].data_frame, ConcatedEncodedDs([enc_train_test["train"],
                                                                       enc_train_test["dev"]]).data_frame,
                                                                       adjust_args={'learn_call': True})
 
+self.feature_cache = dict()  # empty feature cache to avoid large predictor objects
 """
     learn_body = align(learn_body, 2)
     # ----------------- #
     # Predict Body
     # ----------------- #
 
     predict_body = f"""
@@ -1204,21 +1220,22 @@
 log.info(f'[Predict phase 2/{{n_phases}}] - Feature generation')
 encoded_ds = self.featurize({{"predict_data": data}})["predict_data"]
 encoded_data = encoded_ds.get_encoded_data(include_target=False)
 
 log.info(f'[Predict phase 3/{{n_phases}}] - Calling ensemble')
 df = self.ensemble(encoded_ds, args=self.pred_args)
 
-if self.pred_args.all_mixers:
-    return df
-else:
+if not self.pred_args.all_mixers:
     log.info(f'[Predict phase 4/{{n_phases}}] - Analyzing output')
-    insights, global_insights = {call(json_ai.explainer)}
+    df, global_insights = {call(json_ai.explainer)}
     self.global_insights = {{**self.global_insights, **global_insights}}
-    return insights
+
+self.feature_cache = dict()  # empty feature cache to avoid large predictor objects
+
+return df
 """
 
     predict_body = align(predict_body, 2)
 
     predictor_code = f"""
 {IMPORTS}
 {IMPORT_EXTERNAL_DIRS}
@@ -1248,14 +1265,17 @@
 
         # Initial stats analysis
         self.statistical_analysis = None
         self.ts_analysis = None
         self.runtime_log = dict()
         self.global_insights = dict()
 
+        # Feature cache
+        self.feature_cache = dict()
+
     @timed
     def analyze_data(self, data: pd.DataFrame) -> None:
         # Perform a statistical analysis on the unprocessed data
 {analyze_data_body}
 
     @timed
     def preprocess(self, data: pd.DataFrame) -> pd.DataFrame:
```

### Comparing `lightwood-23.5.1.1/lightwood/api/predictor.py` & `lightwood-23.6.2.0/lightwood/api/predictor.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/api/types.py` & `lightwood-23.6.2.0/lightwood/api/types.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/data/encoded_ds.py` & `lightwood-23.6.2.0/lightwood/data/encoded_ds.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,92 +1,117 @@
 import inspect
-from typing import List, Tuple
+from typing import List, Tuple, Dict
 import torch
 import numpy as np
 import pandas as pd
 from torch.utils.data import Dataset
 from lightwood.encoder.base import BaseEncoder
 
 
 class EncodedDs(Dataset):
-    def __init__(self, encoders: List[BaseEncoder], data_frame: pd.DataFrame, target: str) -> None:
+    def __init__(self, encoders: Dict[str, BaseEncoder], data_frame: pd.DataFrame, target: str) -> None:
         """
         Create a Lightwood datasource from a data frame and some encoders. This class inherits from `torch.utils.data.Dataset`.
         
         Note: normal behavior is to cache encoded representations to avoid duplicated computations. If you want an option to disable, this please open an issue.
          
         :param encoders: list of Lightwood encoders used to encode the data per each column.
         :param data_frame: original dataframe.
         :param target: name of the target column to predict.
         """  # noqa
         self.data_frame = data_frame
         self.encoders = encoders
         self.target = target
-        self.cache_encoded = True
-        self.cache = [None] * len(self.data_frame)
         self.encoder_spans = {}
-        self.input_length = 0
+        self.input_length = 0  # feature tensor dim
 
         # save encoder span, has to use same iterator as in __getitem__ for correct indeces
         for col in self.data_frame:
             if col != self.target and self.encoders.get(col, False):
                 self.encoder_spans[col] = (self.input_length,
                                            self.input_length + self.encoders[col].output_size)
                 self.input_length += self.encoders[col].output_size
 
+        # if cache enabled, we immediately build it
+        self.use_cache = True
+        self.cache_built = False
+        self.X_cache: torch.Tensor = torch.full((len(self.data_frame),), fill_value=torch.nan)
+        self.Y_cache: torch.Tensor = torch.full((len(self.data_frame),), fill_value=torch.nan)
+        self.build_cache()
+
     def __len__(self):
         """
         The length of an `EncodedDs` datasource equals the amount of rows of the original dataframe.
 
         :return: length of the `EncodedDs`
         """
         return int(self.data_frame.shape[0])
 
     def __getitem__(self, idx: int) -> Tuple[torch.Tensor, torch.Tensor]:
         """
         The getter yields a tuple (X, y), where:
-          - `X `is a concatenation of all encoded representations of the row
-          - `y` is the encoded target
+          - `X `is a concatenation of all encoded representations of the row. Size: (B, n_features)
+          - `y` is the encoded target. Size: (B, n_features)
           
         :param idx: index of the row to access.
         
         :return: tuple (X, y) with encoded data.
         
         """  # noqa
-        if self.cache_encoded:
-            if self.cache[idx] is not None:
-                return self.cache[idx]
+        if self.use_cache and self.X_cache[idx] is not torch.nan:
+            X = self.X_cache[idx, :]
+            Y = self.Y_cache[idx]
+        else:
+            X, Y = self._encode_idxs([idx, ])
+            if self.use_cache:
+                self.X_cache[idx, :] = X
+                self.Y_cache[idx, :] = Y
+
+        return X, Y
+
+    def _encode_idxs(self, idxs: list):
+        if not isinstance(idxs, list):
+            raise Exception(f"Passed indexes is not an iterable. Check the type! Index: {idxs}")
 
-        X = torch.FloatTensor()
-        Y = torch.FloatTensor()
+        X = torch.zeros((len(idxs), self.input_length))
+        Y = torch.zeros((len(idxs),))
         for col in self.data_frame:
             if self.encoders.get(col, None):
                 kwargs = {}
                 if 'dependency_data' in inspect.signature(self.encoders[col].encode).parameters:
-                    kwargs['dependency_data'] = {dep: [self.data_frame.iloc[idx][dep]]
+                    kwargs['dependency_data'] = {dep: [self.data_frame.iloc[idxs][dep]]
                                                  for dep in self.encoders[col].dependencies}
                 if hasattr(self.encoders[col], 'data_window'):
                     cols = [self.target] + [f'{self.target}_timestep_{i}'
                                             for i in range(1, self.encoders[col].data_window)]
-                    data = [self.data_frame[cols].iloc[idx].tolist()]
+                    data = self.data_frame[cols].iloc[idxs].values
                 else:
                     cols = [col]
-                    data = self.data_frame[cols].iloc[idx].tolist()
+                    data = self.data_frame[cols].iloc[idxs].values.flatten()
 
-                encoded_tensor = self.encoders[col].encode(data, **kwargs)[0]
+                encoded_tensor = self.encoders[col].encode(data, **kwargs)
                 if torch.isnan(encoded_tensor).any() or torch.isinf(encoded_tensor).any():
                     raise Exception(f'Encoded tensor: {encoded_tensor} contains nan or inf values, this tensor is \
                                       the encoding of column {col} using {self.encoders[col].__class__}')
                 if col != self.target:
-                    X = torch.cat([X, encoded_tensor])
+                    a, b = self.encoder_spans[col]
+                    X[:, a:b] = torch.squeeze(encoded_tensor, dim=list(range(2, len(encoded_tensor.shape))))
+
+                # target post-processing
                 else:
                     Y = encoded_tensor
 
-        if self.cache_encoded:
-            self.cache[idx] = (X, Y)
+                    if len(encoded_tensor.shape) > 2:
+                        Y = encoded_tensor.squeeze()
+
+                    if len(encoded_tensor.shape) < 2:
+                        Y = encoded_tensor.unsqueeze(1)
+
+                    # else:
+                    #     Y = encoded_tensor.ravel()
 
         return X, Y
 
     def get_column_original_data(self, column_name: str) -> pd.Series:
         """
         Gets the original data for any given column of the `EncodedDs`.
 
@@ -98,52 +123,79 @@
     def get_encoded_column_data(self, column_name: str) -> torch.Tensor:
         """
         Gets the encoded data for any given column of the `EncodedDs`.
 
         :param column_name: name of the column.
         :return: A `torch.Tensor` with the encoded data of the `column_name` column.
         """
+        if self.use_cache and self.cache_built:
+            if column_name == self.target and self.Y_cache is not None:
+                return self.Y_cache
+            elif self.X_cache is not torch.nan:
+                a, b = self.encoder_spans[column_name]
+                return self.X_cache[:, a:b]
+
         kwargs = {}
         if 'dependency_data' in inspect.signature(self.encoders[column_name].encode).parameters:
             deps = [dep for dep in self.encoders[column_name].dependencies if dep in self.data_frame.columns]
-            kwargs['dependency_data'] = {dep: self.data_frame[dep].tolist() for dep in deps}
+            kwargs['dependency_data'] = {dep: self.data_frame[dep] for dep in deps}
         encoded_data = self.encoders[column_name].encode(self.data_frame[column_name], **kwargs)
         if torch.isnan(encoded_data).any() or torch.isinf(encoded_data).any():
             raise Exception(f'Encoded tensor: {encoded_data} contains nan or inf values')
 
         if not isinstance(encoded_data, torch.Tensor):
             raise Exception(
-                f'The encoder: {self.encoders[column_name]} for column: {column_name} does not return a Tensor !')
+                f'The encoder: {self.encoders[column_name]} for column: {column_name} does not return a Tensor!')
+
+        if self.use_cache and not self.cache_built:
+            if column_name == self.target:
+                self.Y_cache = encoded_data
+            else:
+                a, b = self.encoder_spans[column_name]
+                self.X_cache = self.X_cache[:, a:b]
+
         return encoded_data
 
-    def get_encoded_data(self, include_target=True) -> torch.Tensor:
+    def get_encoded_data(self, include_target: bool = True) -> torch.Tensor:
         """
         Gets all encoded data.
 
         :param include_target: whether to include the target column in the output or not.
         :return: A `torch.Tensor` with the encoded dataframe.
         """
         encoded_dfs = []
         for col in self.data_frame.columns:
             if (include_target or col != self.target) and self.encoders.get(col, False):
                 encoded_dfs.append(self.get_encoded_column_data(col))
 
         return torch.cat(encoded_dfs, 1)
 
+    def build_cache(self):
+        """ This method builds a cache for the entire dataframe provided at initialization. """
+        if not self.use_cache:
+            raise RuntimeError("Cannot build a cache for EncodedDS with `use_cache` set to False.")
+
+        idxs = list(range(len(self.data_frame)))
+        X, Y = self._encode_idxs(idxs)
+        self.X_cache = X
+        self.Y_cache = Y
+        self.cache_built = True
+
     def clear_cache(self):
-        """
-        Clears the `EncodedDs` cache.
-        """
-        self.cache = [None] * len(self.data_frame)
+        """ Clears the `EncodedDs` cache. """
+        self.X_cache = torch.full((len(self.data_frame),), fill_value=torch.nan)
+        self.Y_cache = torch.full((len(self.data_frame),), fill_value=torch.nan)
+        self.cache_built = False
 
 
 class ConcatedEncodedDs(EncodedDs):
     """
     `ConcatedEncodedDs` abstracts over multiple encoded datasources (`EncodedDs`) as if they were a single entity.
     """  # noqa
+
     # TODO: We should probably delete this abstraction, it's not really useful and it adds complexity/overhead
     def __init__(self, encoded_ds_arr: List[EncodedDs]) -> None:
         # @TODO: missing super() call here?
         self.encoded_ds_arr = encoded_ds_arr
         self.encoded_ds_lengths = [len(x) for x in self.encoded_ds_arr]
         self.encoders = self.encoded_ds_arr[0].encoders
         self.encoder_spans = self.encoded_ds_arr[0].encoder_spans
```

### Comparing `lightwood-23.5.1.1/lightwood/data/timeseries_analyzer.py` & `lightwood-23.6.2.0/lightwood/data/timeseries_analyzer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/data/timeseries_transform.py` & `lightwood-23.6.2.0/lightwood/data/timeseries_transform.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/__init__.py` & `lightwood-23.6.2.0/lightwood/encoder/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/array/array.py` & `lightwood-23.6.2.0/lightwood/encoder/array/array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/array/ts_cat_array.py` & `lightwood-23.6.2.0/lightwood/encoder/array/ts_cat_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/array/ts_num_array.py` & `lightwood-23.6.2.0/lightwood/encoder/array/ts_num_array.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 from typing import List, Dict, Iterable, Optional
 
 import torch
-import torch.nn.functional as F
 
 from lightwood.encoder import BaseEncoder
 from lightwood.encoder.numeric import TsNumericEncoder
 
 
 class TsArrayNumericEncoder(BaseEncoder):
-    def __init__(self, timesteps: int, is_target: bool = False, positive_domain: bool = False, grouped_by=None):
+    def __init__(self, timesteps: int, is_target: bool = False, positive_domain: bool = False, grouped_by=None, nan=0):
         """
         This encoder handles arrays of numerical time series data by wrapping the numerical encoder with behavior specific to time series tasks.
         
         :param timesteps: length of forecasting horizon, as defined by TimeseriesSettings.window.
         :param is_target: whether this encoder corresponds to the target column.
         :param positive_domain: whether the column domain is expected to be positive numbers.
         :param grouped_by: what columns, if any, are considered to group the original column and yield multiple time series.
         """  # noqa
         super(TsArrayNumericEncoder, self).__init__(is_target=is_target)
         self.normalizers = None
         self.group_combinations = None
         self.dependencies = grouped_by
         self.data_window = timesteps
         self.positive_domain = positive_domain
+        self.nan_value = nan
         self.sub_encoder = TsNumericEncoder(is_target=is_target, positive_domain=positive_domain, grouped_by=grouped_by)
         self.output_size = self.data_window * self.sub_encoder.output_size
 
     def prepare(self, priming_data):
         """
         This method prepares the underlying time series numerical encoder.
         """
@@ -48,42 +48,17 @@
         if not self.is_prepared:
             raise Exception('You need to call "prepare" before calling "encode" or "decode".')
         if self.sub_encoder.normalizers is None and self.normalizers is not None:
             self.sub_encoder.normalizers = self.normalizers
         if not dependency_data:
             dependency_data = {'__default': [None] * len(data)}
 
-        ret = []
-        for series in data:
-            ret.append(self.encode_one(series, dependency_data=dependency_data))
+        ret = self.sub_encoder.encode(data, dependency_data=dependency_data)
 
-        return torch.vstack(ret)
-
-    def encode_one(self, data: Iterable, dependency_data: Optional[Dict[str, str]] = {}) -> torch.Tensor:
-        """
-        Encodes a single windowed slice of any given time series.
-
-        :param data: windowed slice of a numerical time series.
-        :param dependency_data: used to determine the correct normalizer for the input.
-        
-        :return: an encoded time series array, as per the underlying `TsNumericEncoder` object. 
-        The output of this encoder for all time steps is concatenated, so the final shape of the tensor is (1, NxK), where N: self.data_window and K: sub-encoder # of output features. 
-        """  # noqa
-        ret = []
-
-        for data_point in data:
-            ret.append(self.sub_encoder.encode([data_point], dependency_data=dependency_data))
-
-        ret = torch.hstack(ret)
-        padding_size = self.output_size - ret.shape[-1]
-
-        if padding_size > 0:
-            ret = F.pad(ret, (0, padding_size))
-
-        return ret
+        return torch.Tensor(ret).nan_to_num(self.nan_value)
 
     def decode(self, encoded_values, dependency_data=None) -> List[List]:
         """
         Decodes a list of encoded arrays into values in their original domains.
 
         :param encoded_values: encoded slices of numerical time series.
         :param dependency_data: used to determine the correct normalizer for the input.
```

### Comparing `lightwood-23.5.1.1/lightwood/encoder/audio/mfcc.py` & `lightwood-23.6.2.0/lightwood/encoder/audio/mfcc.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/base.py` & `lightwood-23.6.2.0/lightwood/encoder/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/categorical/autoencoder.py` & `lightwood-23.6.2.0/lightwood/encoder/categorical/autoencoder.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/categorical/binary.py` & `lightwood-23.6.2.0/lightwood/encoder/categorical/binary.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 import torch
 import numpy as np
 from scipy.special import softmax
 
 from lightwood.encoder.base import BaseEncoder
 from lightwood.helpers.constants import _UNCOMMON_WORD
+from lightwood.helpers.log import log
 
 
 class BinaryEncoder(BaseEncoder):
     """
    Creates a one-hot-encoding for binary class data. Assume two arbitrary categories :math:`A` and :math:`B`; representation for them will be as such:
 
     .. math::
@@ -30,25 +31,28 @@
 
     Users should note that models will be presented with the inverse of the target weights, `inv_target_weights`, which will perform the 1/target_value_per_class operation. **This means large values will result in small weights for the model**.
     """ # noqa
     def __init__(
         self,
         is_target: bool = False,
         target_weights: Dict[str, float] = None,
+        handle_unknown: str = 'use_encoded_value'
     ):
         super().__init__(is_target)
         """
         :param is_target: Whether encoder featurizes target column
         :param target_weights: Percentage of total population represented by each category (from [0, 1]), as a dictionary.
+        :param handle_unknown: if set to `use_encoded_value`, will assign all classes with index greater than 1 to a special UNKNOWN index. This doesn't affect the encoded representation of shape (B, 2). During decoding, any unknown or otherwise known but "out-of-bounds" word will be decoded back to the lightwood unknown category token. If this argument is set to `error`, the encoder will raise an error while preparing if there are more than two observed classes.
         """  # noqa
 
         self.map = {}  # category name -> index
         self.rev_map = {}  # index -> category name
         self.output_size = 2
         self.encoder_class_type = str
+        self.handle_unknown = handle_unknown
 
         # Weight-balance info if encoder represents target
         self.target_weights = None
         self.index_weights = None
         if self.is_target:
             self.target_weights = dc(target_weights)
 
@@ -63,21 +67,24 @@
 
         unq_cats = np.unique([i for i in priming_data if i is not None]).tolist()
 
         self.map = {cat: indx for indx, cat in enumerate(unq_cats)}
         self.rev_map = {indx: cat for cat, indx in self.map.items()}
 
         # Enforce only binary; map must have exactly 2 classes.
-        if len(self.map) > 2:
-            raise ValueError(f'Issue with dtype; data has > 2 classes. All classes are: {self.map}')
+        if len(self.map) > 2 and self.handle_unknown == 'use_encoded_value':
+            log.warning('Warning: dtype for binary encoder has > 2 classes. Extra classes will be pointed to an invalid token. Try overriding this encoder with a multi-class categorical encoder, otherwise performance may not be optimal.')  # noqa
+            log.warning(f'Observed classes are: {self.map}.')
+        elif self.handle_unknown == 'error':
+            raise ValueError(f'Data has > 2 classes and encoder is in strict mode. Aborting. All classes are: {self.map}.')  # noqa
 
         # For target-only, report on relative weights of classes
         if self.is_target:
 
-            self.index_weights = torch.Tensor([1, 1])  # Equally wt. both classes
+            self.index_weights = torch.ones(self.output_size)  # Equally wt. both classes
 
             # If target weights provided, weight by inverse
             if self.target_weights is not None:
 
                 # Check target weights properly specified
                 if sum([np.isclose(i, 0) for i in self.target_weights.values()]) > 0:
                     raise ValueError('Target weights cannot be 0')
@@ -98,20 +105,22 @@
         :returns Encoded data of form :math:`N_{rows} x 2`
         """  # noqa
         if not self.is_prepared:
             raise Exception(
                 'You need to call "prepare" before calling "encode" or "decode".'
             )
 
-        ret = torch.zeros(size=(len(column_data), 2))
+        ret = torch.zeros(size=(len(column_data), self.output_size))
 
         for idx, word in enumerate(column_data):
             index = self.map.get(word, None)
 
-            if index is not None:
+            if index is None or index >= self.output_size:
+                pass  # any unknown value is ignored
+            else:
                 ret[idx, index] = 1
 
         return torch.Tensor(ret)
 
     def decode(self, encoded_data: torch.Tensor):
         """
         Given encoded data, return in form of original category labels.
@@ -126,15 +135,19 @@
         encoded_data_list = encoded_data.tolist()
         ret = []
 
         for vector in encoded_data_list:
             if not np.any(vector):  # Vector of all 0s -> unknown category
                 ret.append(_UNCOMMON_WORD)
             else:
-                ret.append(self.rev_map[np.argmax(vector)])
+                idx = np.argmax(vector)
+                if idx >= self.output_size:
+                    ret.append(_UNCOMMON_WORD)  # known, but not either of the supported categories
+                else:
+                    ret.append(self.rev_map[idx])
 
         return ret
 
     def decode_probabilities(self, encoded_data: torch.Tensor) -> Tuple[List[str], List[List[float]], Dict[int, str]]:
         """
         Provides decoded answers, as well as a probability assignment to each data point.
```

### Comparing `lightwood-23.5.1.1/lightwood/encoder/categorical/gym.py` & `lightwood-23.6.2.0/lightwood/encoder/categorical/gym.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/categorical/multihot.py` & `lightwood-23.6.2.0/lightwood/encoder/categorical/multihot.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/categorical/onehot.py` & `lightwood-23.6.2.0/lightwood/encoder/categorical/onehot.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,20 +64,20 @@
         """ # noqa
         if self.is_prepared:
             raise Exception('You can only call "prepare" once for a given encoder.')
 
         unq_cats = np.unique([i for i in priming_data if i is not None]).tolist()
 
         if self.use_unknown:
-            log.info("Encoding UNKNOWN categories as index 0")
+            log.debug("Encoding UNKNOWN categories as index 0")
             self.map = {cat: indx + 1 for indx, cat in enumerate(unq_cats)}
             self.map.update({_UNCOMMON_WORD: 0})
             self.rev_map = {indx: cat for cat, indx in self.map.items()}
         else:
-            log.info("Encoding UNKNOWN categories as vector of all 0s")
+            log.debug("Encoding UNKNOWN categories as vector of all 0s")
             self.map = {cat: indx for indx, cat in enumerate(unq_cats)}
             self.rev_map = {indx: cat for cat, indx in self.map.items()}
 
         # Set the length of output
         self.output_size = len(self.map)
 
         # For target-only, report on relative weights of classes
```

### Comparing `lightwood-23.5.1.1/lightwood/encoder/datetime/datetime.py` & `lightwood-23.6.2.0/lightwood/encoder/datetime/datetime.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/datetime/datetime_sin_normalizer.py` & `lightwood-23.6.2.0/lightwood/encoder/datetime/datetime_sin_normalizer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/helpers.py` & `lightwood-23.6.2.0/lightwood/encoder/helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/identity/identity.py` & `lightwood-23.6.2.0/lightwood/encoder/identity/identity.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/image/helpers/img_to_vec.py` & `lightwood-23.6.2.0/lightwood/encoder/image/helpers/img_to_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/image/img_2_vec.py` & `lightwood-23.6.2.0/lightwood/encoder/image/img_2_vec.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/text/helpers/pretrained_helpers.py` & `lightwood-23.6.2.0/lightwood/encoder/text/helpers/pretrained_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/text/helpers/rnn_helpers.py` & `lightwood-23.6.2.0/lightwood/encoder/text/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/text/pretrained.py` & `lightwood-23.6.2.0/lightwood/encoder/text/pretrained.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,29 +1,32 @@
-"""
-"""
+import os
 import time
+from typing import Iterable
+from collections import deque
+
+import numpy as np
 import torch
 from torch.utils.data import DataLoader
-import os
 import pandas as pd
-from lightwood.encoder.text.helpers.pretrained_helpers import TextEmbed
-from lightwood.helpers.device import get_device_from_name
-from lightwood.encoder.base import BaseEncoder
-from lightwood.helpers.log import log
-from lightwood.helpers.torch import LightwoodAutocast
 from type_infer.dtype import dtype
 from transformers import (
     DistilBertModel,
     DistilBertForSequenceClassification,
     DistilBertTokenizerFast,
     AdamW,
     get_linear_schedule_with_warmup,
 )
+from sklearn.model_selection import train_test_split
+
+from lightwood.encoder.text.helpers.pretrained_helpers import TextEmbed
+from lightwood.helpers.device import get_device_from_name
+from lightwood.encoder.base import BaseEncoder
+from lightwood.helpers.log import log
+from lightwood.helpers.torch import LightwoodAutocast
 from lightwood.helpers.general import is_none
-from typing import Iterable
 
 
 class PretrainedLangEncoder(BaseEncoder):
     is_trainable_encoder: bool = True
 
     """
     Creates a contextualized embedding to represent input text via the [CLS] token vector from DistilBERT (transformers). (Sanh et al. 2019 - https://arxiv.org/abs/1910.01108).
@@ -44,15 +47,14 @@
         embed_mode: bool = True,
         device: str = '',
     ):
         """
         :param is_target: Whether this encoder represents the target. NOT functional for text generation yet.
         :param batch_size: size of batch while fine-tuning
         :param max_position_embeddings: max sequence length of input text
-        :param custom_train: If True, trains model on target procided
         :param frozen: If True, freezes transformer layers during training.
         :param epochs: number of epochs to train model with
         :param output_type: Data dtype of the target; if categorical/binary, the option to return logits is possible.
         :param embed_mode: If True, assumes the output of the encode() step is the CLS embedding (this can be trained or not). If False, returns the logits of the tuned task.
         :param device: name of the device that get_device_from_name will attempt to use.
         """ # noqa
         super().__init__(is_target)
@@ -60,20 +62,22 @@
         self.output_type = output_type
         self.name = "distilbert text encoder"
 
         self._max_len = max_position_embeddings
         self._frozen = frozen
         self._batch_size = batch_size
         self._epochs = epochs
+        self._patience = 3  # measured in batches rather than epochs
+        self._val_loss_every = 5  # how many batches to wait before checking val loss. If -1, will check train loss instead of val for early stopping.  # noqa
+        self._tr_loss_every = 2  # same as above, but only applies if `_val_loss_every` is set to -1
 
         # Model setup
         self._model = None
         self.model_type = None
 
-        # TODO: Other LMs; Distilbert is a good balance of speed/performance
         self._classifier_model_class = DistilBertForSequenceClassification
         self._embeddings_model_class = DistilBertModel
         self._pretrained_model_name = "distilbert-base-uncased"
         self._tokenizer = DistilBertTokenizerFast.from_pretrained(self._pretrained_model_name)
 
         self.device = get_device_from_name(device)
 
@@ -86,74 +90,81 @@
         if self.embed_mode:
             log.info("Embedding mode on. [CLS] embedding dim output of encode()")
         else:
             log.info("Embedding mode off. Logits are output of encode()")
 
     def prepare(
         self,
-        train_priming_data: Iterable[str],
-        dev_priming_data: Iterable[str],
+        train_priming_data: pd.Series,
+        dev_priming_data: pd.Series,
         encoded_target_values: torch.Tensor,
     ):
         """
         Fine-tunes a transformer on the priming data.
 
-        CURRENTLY WIP; train + dev are placeholders for a validation-based approach. 
-
+        Transformer is fine-tuned with weight-decay on training split. 
+        
         Train + Dev are concatenated together and a transformer is then fine tuned with weight-decay applied on the transformer parameters. The option to freeze the underlying transformer and only train a linear layer exists if `frozen=True`. This trains faster, with the exception that the performance is often lower than fine-tuning on internal benchmarks.
-
+        
         :param train_priming_data: Text data in the train set
-        :param dev_priming_data: Text data in the dev set (not currently supported; can be empty)
+        :param dev_priming_data: Text data in the dev set
         :param encoded_target_values: Encoded target labels in Nrows x N_output_dimension
         """ # noqa
         if self.is_prepared:
             raise Exception("Encoder is already prepared.")
 
         os.environ['TOKENIZERS_PARALLELISM'] = 'true'
 
-        # TODO -> we shouldn't be concatenating these together
-        if len(dev_priming_data) > 0:
-            priming_data = pd.concat([train_priming_data, dev_priming_data]).values
+        # remove empty strings (`None`s for dtype `object`)
+        filtered_tr = train_priming_data[~train_priming_data.isna()]
+        filtered_dev = dev_priming_data[~dev_priming_data.isna()]
+
+        if filtered_dev.shape[0] > 0:
+            priming_data = pd.concat([filtered_tr, filtered_dev]).tolist()
+            val_size = (len(dev_priming_data)) / len(train_priming_data)
         else:
-            priming_data = train_priming_data.tolist()
+            priming_data = filtered_tr.tolist()
+            val_size = 0.1  # leave out 0.1 for validation
+
+        # Label encode the OHE/binary output for classification
+        labels = encoded_target_values.argmax(dim=1)
 
-        # Replaces empty strings with ''
-        priming_data = [x if x is not None else "" for x in priming_data]
+        # Split into train and validation sets
+        train_texts, val_texts, train_labels, val_labels = train_test_split(priming_data, labels, test_size=val_size)
 
         # If classification, then fine-tune
-        if (self.output_type in (dtype.categorical, dtype.binary)):
-            log.info("Training model.")
+        if self.output_type in (dtype.categorical, dtype.binary):
+            log.info("Training model.\n\tOutput trained is categorical")
 
             # Prepare priming data into tokenized form + attention masks
-            text = self._tokenizer(priming_data, truncation=True, padding=True)
-
-            log.info("\tOutput trained is categorical")
-
-            # Label encode the OHE/binary output for classification
-            labels = encoded_target_values.argmax(dim=1)
+            training_text = self._tokenizer(train_texts, truncation=True, padding=True)
+            validation_text = self._tokenizer(val_texts, truncation=True, padding=True)
 
             # Construct the model
             self._model = self._classifier_model_class.from_pretrained(
                 self._pretrained_model_name,
                 num_labels=len(encoded_target_values[0]),  # max classes to test
             ).to(self.device)
 
             # Construct the dataset for training
-            xinp = TextEmbed(text, labels)
-            dataset = DataLoader(xinp, batch_size=self._batch_size, shuffle=True)
+            xinp = TextEmbed(training_text, train_labels)
+            train_dataset = DataLoader(xinp, batch_size=self._batch_size, shuffle=True)
+
+            # Construct the dataset for validation
+            xvalinp = TextEmbed(validation_text, val_labels)
+            val_dataset = DataLoader(xvalinp, batch_size=self._batch_size, shuffle=True)
 
             # Set max length of input string; affects input to the model
             if self._max_len is None:
                 self._max_len = self._model.config.max_position_embeddings
 
             if self._frozen:
                 log.info("\tFrozen Model + Training Classifier Layers")
                 """
-                Freeze the base transformer model and train
-                a linear layer on top
+                Freeze the base transformer model and train a linear layer on top
                 """
                 # Freeze all the transformer parameters
                 for param in self._model.base_model.parameters():
                     param.requires_grad = False
 
                 optimizer_grouped_parameters = self._model.parameters()
 
@@ -185,54 +196,49 @@
                     },
                 ]
 
             optimizer = AdamW(optimizer_grouped_parameters, lr=1e-5)
             scheduler = get_linear_schedule_with_warmup(
                 optimizer,
                 num_warmup_steps=0,  # default value for GLUE
-                num_training_steps=len(dataset) * self._epochs,
+                num_training_steps=len(train_dataset) * self._epochs,
             )
 
             # Train model; declare optimizer earlier if desired.
             self._tune_model(
-                dataset, optim=optimizer, scheduler=scheduler, n_epochs=self._epochs
+                train_dataset, val_dataset, optim=optimizer, scheduler=scheduler, n_epochs=self._epochs
             )
 
         else:
             log.info("Target is not classification; Embeddings Generator only")
 
             self.model_type = "embeddings_generator"
             self._model = self._embeddings_model_class.from_pretrained(
                 self._pretrained_model_name
             ).to(self.device)
 
             # TODO: Not a great flag
-            # Currently, if the task is not classification, you must have
-            # an embedding generator only.
+            # Currently, if the task is not classification, you must have an embedding generator only
             if self.embed_mode is False:
                 log.info("Embedding mode must be ON for non-classification targets.")
                 self.embed_mode = True
 
         self.is_prepared = True
         encoded = self.encode(priming_data[0:1])
         self.output_size = len(encoded[0])
 
-    def _tune_model(self, dataset, optim, scheduler, n_epochs=1):
+    def _tune_model(self, train_dataset, val_dataset, optim, scheduler, n_epochs=1):
         """
-        Given a model, train for n_epochs.
-        Specifically intended for tuning; it does NOT use loss/
-        stopping criterion.
-
-        model - torch.nn model;
-        dataset - torch.DataLoader; dataset to train
-        device - torch.device; cuda/cpu
-        log - lightwood.logger.log; log.info output
+        Given a model, tune for n_epochs.
+
+        train_dataset - torch.DataLoader; dataset to train
+        val_dataset - torch.DataLoader; dataset used to compute validation loss + early stopping
         optim - transformers.optimization.AdamW; optimizer
         scheduler - scheduling params
-        n_epochs - number of epochs to train
+        n_epochs - max number of epochs to train for, provided there is no early stopping
 
         """ # noqa
         self._model.train()
 
         if optim is None:
             log.info("No opt. provided, setting all params with AdamW.")
             optim = AdamW(self._model.parameters(), lr=5e-5)
@@ -240,40 +246,80 @@
             log.info("Optimizer provided")
 
         if scheduler is None:
             log.info("No scheduler provided.")
         else:
             log.info("Scheduler provided.")
 
+        best_tr_loss = best_val_loss = float("inf")
+        tr_loss_queue = deque(maxlen=self._patience)
+        patience_counter = self._patience
+
         started = time.time()
         for epoch in range(n_epochs):
             total_loss = 0
 
-            for batch in dataset:
+            for bidx, batch in enumerate(train_dataset):
                 optim.zero_grad()
 
                 with LightwoodAutocast():
-                    inpids = batch["input_ids"].to(self.device)
-                    attn = batch["attention_mask"].to(self.device)
-                    labels = batch["labels"].to(self.device)
-                    outputs = self._model(inpids, attention_mask=attn, labels=labels)
-                    loss = outputs[0]
+                    loss = self._call(batch)
 
+                tr_loss_queue.append(loss.item())
                 total_loss += loss.item()
 
                 loss.backward()
                 optim.step()
                 if scheduler is not None:
                     scheduler.step()
                 if time.time() - started > self.stop_after:
                     break
 
+                # val-based early stopping
+                if False and (self._val_loss_every != -1) and (bidx % self._val_loss_every == 0):
+                    self._model.eval()
+                    val_loss = 0
+
+                    for vbatch in val_dataset:
+                        val_loss += self._call(vbatch).item()
+
+                    log.info(f"Epoch {epoch+1} train batch {bidx+1} - Validation loss: {val_loss/len(val_dataset)}")
+                    if val_loss / len(val_dataset) >= best_val_loss:
+                        break
+
+                    best_val_loss = val_loss / len(val_dataset)
+                    self._model.train()
+
+                # train-based early stopping
+                elif False and (bidx + 1) % self._tr_loss_every == 0:
+                    self._model.eval()
+
+                    tr_loss = np.average(tr_loss_queue)
+                    log.info(f"Epoch {epoch} train batch {bidx} - Train loss: {tr_loss}")  # noqa
+                    self._model.train()
+
+                    if tr_loss >= best_tr_loss and patience_counter == 0:
+                        break
+                    elif patience_counter > 0:
+                        patience_counter -= 1
+                    elif tr_loss < best_tr_loss:
+                        best_tr_loss = tr_loss
+                        patience_counter = self._patience
+
             if time.time() - started > self.stop_after:
                 break
-            self._train_callback(epoch, total_loss / len(dataset))
+            self._train_callback(epoch, total_loss / len(train_dataset))
+
+    def _call(self, batch):
+        inpids = batch["input_ids"].to(self.device)
+        attn = batch["attention_mask"].to(self.device)
+        labels = batch["labels"].to(self.device)
+        outputs = self._model(inpids, attention_mask=attn, labels=labels)
+        loss = outputs[0]
+        return loss
 
     def _train_callback(self, epoch, loss):
         log.info(f"{self.name} at epoch {epoch+1} and loss {loss}!")
 
     def encode(self, column_data: Iterable[str]) -> torch.Tensor:
         """
         Converts each text example in a column into encoded state. This can be either a vector embedding of the [CLS] token (represents the full text input) OR the logits prediction of the output.
```

### Comparing `lightwood-23.5.1.1/lightwood/encoder/text/rnn.py` & `lightwood-23.6.2.0/lightwood/encoder/text/rnn.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/text/short.py` & `lightwood-23.6.2.0/lightwood/encoder/text/short.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,14 +4,16 @@
 from lightwood.encoder.categorical import CategoricalAutoEncoder
 from type_infer.helpers import tokenize_text
 from lightwood.helpers.torch import concat_vectors_and_pad, average_vectors
 import pandas as pd
 
 
 class ShortTextEncoder(BaseEncoder):
+    is_trainable_encoder = False
+
     def __init__(self, is_target=False, mode=None, device=''):
         """
         :param is_target:
         :param mode:
             None or "concat" or "mean".
             When None, it will be set automatically based on is_target:
             (is_target) -> 'concat'
@@ -51,15 +53,15 @@
         return average_vectors(vecs)
 
     def prepare(self, priming_data):
         no_null_sentences = (x if x is not None else '' for x in priming_data)
         unique_tokens = set()
         max_words_per_sent = 0
         for sent in no_null_sentences:
-            tokens = tokenize_text(sent)
+            tokens = list(tokenize_text(sent))
             max_words_per_sent = max(max_words_per_sent, len(tokens))
             for tok in tokens:
                 unique_tokens.add(tok)
 
         self.cae.prepare(pd.Series(list(unique_tokens)), pd.Series([]))
 
         if self._mode == 'concat':
@@ -74,15 +76,15 @@
         encoded = self.encode([priming_data[0]])
         self.output_size = len(encoded[0])
 
     def encode(self, column_data: List[str]) -> torch.Tensor:
         no_null_sentences = (x if x is not None else '' for x in column_data)
         output = []
         for sent in no_null_sentences:
-            tokens = tokenize_text(sent)
+            tokens = list(tokenize_text(sent))
             encoded_words = self.cae.encode(tokens)
             encoded_sent = self._combine_fn(encoded_words)
             output.append(torch.Tensor(encoded_sent))
         output = torch.stack(output)
         return output
 
     def decode(self, vectors):
```

### Comparing `lightwood-23.5.1.1/lightwood/encoder/text/tfidf.py` & `lightwood-23.6.2.0/lightwood/encoder/text/tfidf.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/text/vocab.py` & `lightwood-23.6.2.0/lightwood/encoder/text/vocab.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/common.py` & `lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/common.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/rnn_helpers.py` & `lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/rnn_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/time_series/helpers/transformer_helpers.py` & `lightwood-23.6.2.0/lightwood/encoder/time_series/helpers/transformer_helpers.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/time_series/rnn.py` & `lightwood-23.6.2.0/lightwood/encoder/time_series/rnn.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/encoder/time_series/ts.py` & `lightwood-23.6.2.0/lightwood/encoder/time_series/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/ensemble/__init__.py` & `lightwood-23.6.2.0/lightwood/ensemble/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/ensemble/base.py` & `lightwood-23.6.2.0/lightwood/ensemble/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/ensemble/best_of.py` & `lightwood-23.6.2.0/lightwood/ensemble/best_of.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/ensemble/mean_ensemble.py` & `lightwood-23.6.2.0/lightwood/ensemble/mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/ensemble/mode_ensemble.py` & `lightwood-23.6.2.0/lightwood/ensemble/mode_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/ensemble/stacked_ensemble.py` & `lightwood-23.6.2.0/lightwood/ensemble/stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/ensemble/ts_stacked_ensemble.py` & `lightwood-23.6.2.0/lightwood/ensemble/ts_stacked_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/ensemble/weighted_mean_ensemble.py` & `lightwood-23.6.2.0/lightwood/ensemble/weighted_mean_ensemble.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/helpers/__init__.py` & `lightwood-23.6.2.0/lightwood/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/helpers/device.py` & `lightwood-23.6.2.0/lightwood/helpers/device.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/helpers/general.py` & `lightwood-23.6.2.0/lightwood/helpers/general.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/helpers/io.py` & `lightwood-23.6.2.0/lightwood/helpers/io.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/helpers/log.py` & `lightwood-23.6.2.0/lightwood/helpers/log.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/helpers/parallelism.py` & `lightwood-23.6.2.0/lightwood/helpers/parallelism.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/helpers/templating.py` & `lightwood-23.6.2.0/lightwood/helpers/templating.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/helpers/text.py` & `lightwood-23.6.2.0/lightwood/helpers/text.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/helpers/torch.py` & `lightwood-23.6.2.0/lightwood/helpers/torch.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/helpers/ts.py` & `lightwood-23.6.2.0/lightwood/helpers/ts.py`

 * *Files 1% similar despite different names*

```diff
@@ -293,21 +293,20 @@
                     candidate_sps[group] = None
             if not candidate_sps[group]:
                 candidate_sps[group] = [1]
 
     return candidate_sps
 
 
-def filter_ds(ds, tss, n_rows=1):
+def filter_ts(df: pd.DataFrame, tss, n_rows=1):
     """
     This method triggers only for timeseries datasets.
 
     It returns a dataframe that filters out all but the first ``n_rows`` per group.
     """  # noqa
-    df = ds.data_frame
     if tss.is_timeseries:
         gby = tss.group_by
         if gby is None:
             df = df.iloc[[0]]
         else:
             ndf = pd.DataFrame(columns=df.columns)
             for group in get_ts_groups(df, tss):
```

### Comparing `lightwood-23.5.1.1/lightwood/mixer/__init__.py` & `lightwood-23.6.2.0/lightwood/mixer/__init__.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/arima.py` & `lightwood-23.6.2.0/lightwood/mixer/arima.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/base.py` & `lightwood-23.6.2.0/lightwood/mixer/base.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/ets.py` & `lightwood-23.6.2.0/lightwood/mixer/ets.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/gluonts.py` & `lightwood-23.6.2.0/lightwood/mixer/gluonts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/helpers/ar_net.py` & `lightwood-23.6.2.0/lightwood/mixer/helpers/ar_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/helpers/default_net.py` & `lightwood-23.6.2.0/lightwood/mixer/helpers/default_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/helpers/qclassic_net.py` & `lightwood-23.6.2.0/lightwood/mixer/helpers/qclassic_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/helpers/ranger.py` & `lightwood-23.6.2.0/lightwood/mixer/helpers/ranger.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/helpers/residual_net.py` & `lightwood-23.6.2.0/lightwood/mixer/helpers/residual_net.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/helpers/transform_corss_entropy_loss.py` & `lightwood-23.6.2.0/lightwood/mixer/helpers/transform_corss_entropy_loss.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/helpers/ts.py` & `lightwood-23.6.2.0/lightwood/mixer/helpers/ts.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/lightgbm.py` & `lightwood-23.6.2.0/lightwood/mixer/lightgbm.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/lightgbm_array.py` & `lightwood-23.6.2.0/lightwood/mixer/lightgbm_array.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/neural.py` & `lightwood-23.6.2.0/lightwood/mixer/neural.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import time
 from copy import deepcopy
+from collections import deque
 from typing import Dict, List, Optional
 
 import torch
 import numpy as np
 import pandas as pd
 from torch import nn
 import torch_optimizer as ad_optim
@@ -38,34 +39,39 @@
             stop_after: float,
             target: str,
             dtype_dict: Dict[str, str],
             target_encoder: BaseEncoder,
             net: str,
             fit_on_dev: bool,
             search_hyperparameters: bool,
-            n_epochs: Optional[int] = None
+            n_epochs: Optional[int] = None,
+            lr: Optional[float] = None,
     ):
         """
         The Neural mixer trains a fully connected dense network from concatenated encoded outputs of each of the features in the dataset to predicted the encoded output. 
         
         :param stop_after: How long the total fitting process should take
         :param target: Name of the target column
         :param dtype_dict: Data type dictionary
         :param target_encoder: Reference to the encoder used for the target
         :param net: The network type to use (`DeafultNet` or `ArNet`)
         :param fit_on_dev: If we should fit on the dev dataset
         :param search_hyperparameters: If the network should run a more through hyperparameter search (currently disabled)
         :param n_epochs: amount of epochs that the network will be trained for. Supersedes all other early stopping criteria if specified.
+        :param lr: learning rate for the network. By default, it is automatically selected based on an initial search process.
         """ # noqa
         super().__init__(stop_after)
         self.dtype_dict = dtype_dict
         self.target = target
         self.target_encoder = target_encoder
+        self.num_hidden = 1
         self.epochs_to_best = 0
         self.n_epochs = n_epochs
+        self.lr = lr
+        self.loss_hist_len = 7  # length of queue to use for early stopping
         self.fit_on_dev = fit_on_dev
         self.net_name = net
         self.supports_proba = dtype_dict[target] in [dtype.binary, dtype.categorical]
         self.search_hyperparameters = search_hyperparameters
         self.stable = True
 
     def _final_tuning(self, data):
@@ -102,77 +108,89 @@
         elif self.dtype_dict[self.target] in (dtype.integer, dtype.float, dtype.quantity, dtype.num_array):
             criterion = MSELoss()
         else:
             criterion = MSELoss()
 
         return criterion
 
-    def _select_optimizer(self) -> Optimizer:
-        optimizer = ad_optim.Ranger(self.model.parameters(), lr=self.lr, weight_decay=2e-2)
+    def _select_optimizer(self, model, lr) -> Optimizer:
+        optimizer = ad_optim.Ranger(model.parameters(), lr=lr, weight_decay=2e-2)
         return optimizer
 
-    def _find_lr(self, dl):
-        optimizer = self._select_optimizer()
+    def _find_lr(self, train_data):
+        lr = 1e-4  # good starting point as search escalates
+        lrs = deque([5e-4, 1e-3, 2e-3, 3e-3, 5e-3, 1e-2, 5e-2, 1e-1])
+        starting_model = deepcopy(self.model)
         criterion = self._select_criterion()
         scaler = GradScaler()
 
-        running_losses: List[float] = []
-        cum_loss = 0
-        lr_log = []
+        running_losses = deque(maxlen=self.loss_hist_len)
+        lr_log = deque(maxlen=self.loss_hist_len)
         best_model = self.model
         stop = False
-        batches = 0
-        for epoch in range(1, 101):
-            if stop:
-                break
 
-            for i, (X, Y) in enumerate(dl):
-                if stop:
-                    break
+        n_steps = 10
+        cum_loss = 0
+
+        while stop is False:
+            # overfit learning on first n_steps samples (biased, but we only want an intuition on what LR is decent)
+            dl = DataLoader(train_data,
+                            batch_size=min(len(train_data.data_frame), 32, self.batch_size),
+                            shuffle=False)
+            dl_iter = iter(dl)
+            self.model = deepcopy(starting_model)
+            self.model.train()
+            optimizer = self._select_optimizer(self.model, lr=lr)
+
+            for i in range(n_steps):
+                try:
+                    X, Y = next(dl_iter)
+                except StopIteration:
+                    dl_iter = iter(dl)
+                    X, Y = next(dl_iter)
 
-                batches += len(X)
                 X = X.to(self.model.device)
                 Y = Y.to(self.model.device)
+
                 with LightwoodAutocast():
                     optimizer.zero_grad()
                     Yh = self._net_call(X)
                     loss = criterion(Yh, Y)
                     if LightwoodAutocast.active:
                         scaler.scale(loss).backward()
                         scaler.step(optimizer)
                         scaler.update()
                     else:
                         loss.backward()
                         optimizer.step()
                 cum_loss += loss.item()
 
-                # Account for ranger lookahead update
-                if (i + 1) * epoch % 6:
-                    batches = 0
-                    lr = optimizer.param_groups[0]['lr']
-                    log.info(f'Loss of {cum_loss} with learning rate {lr}')
-                    running_losses.append(cum_loss)
-                    lr_log.append(lr)
-                    cum_loss = 0
-                    if len(running_losses) < 2 or np.mean(running_losses[:-1]) > np.mean(running_losses):
-                        optimizer.param_groups[0]['lr'] = lr * 1.4
-                        # Time saving since we don't have to start training fresh
-                        best_model = deepcopy(self.model)
-                    else:
-                        stop = True
+            log.info(f'Loss of {cum_loss} with learning rate {lr}')
+            running_losses.append(cum_loss)
+            lr_log.append(lr)
+            cum_loss = 0
+            lr = lrs.popleft()
+            if len(lrs) == 0:
+                stop = True
+
+            # store model if best so far
+            inv_running_losses = list(running_losses)[::-1]  # invert so when tied we pick the most aggresive LR
+            best_loss_idx = np.nanargmin(inv_running_losses)  # nanargmin ignores nans that may arise
+            if best_loss_idx == 0:
+                best_model = deepcopy(self.model)  # store model for slight time savings
+                best_loss_lr = lr_log[-1]
 
-        best_loss_lr = lr_log[np.argmin(running_losses)]
         lr = best_loss_lr
         log.info(f'Found learning rate of: {lr}')
         return lr, best_model
 
     def _max_fit(self, train_dl, dev_dl, criterion, optimizer, scaler, stop_after, return_model_after):
         epochs_to_best = 0
         best_dev_error = pow(2, 32)
-        running_errors = []
+        running_errors = deque(maxlen=self.loss_hist_len)
         best_model = self.model
 
         for epoch in range(1, return_model_after + 1):
             self.model = self.model.train()
             running_losses: List[float] = []
             for i, (X, Y) in enumerate(train_dl):
                 X = X.to(self.model.device)
@@ -211,18 +229,19 @@
             # manually set epoch limit
             if self.n_epochs is not None:
                 if epoch > self.n_epochs:
                     break
 
             # automated early stopping
             else:
-                if len(running_errors) >= 5:
-                    delta_mean = np.average([running_errors[-i - 1] - running_errors[-i] for i in range(1, 5)],
-                                            weights=[(1 / 2)**i for i in range(1, 5)])
-                    if delta_mean <= 0:
+                if len(running_errors) >= self.loss_hist_len:
+                    delta_mean = np.average([
+                        running_errors[-i - 1] - running_errors[-i] for i in range(len(running_errors) - 1)],
+                        weights=[(1 / 2)**i for i in range(len(running_errors) - 1)])
+                    if delta_mean >= 0:
                         break
                 elif (time.time() - self.started) > stop_after:
                     break
                 elif running_errors[-1] < 0.0001 or train_error < 0.0001:
                     break
 
         if np.isnan(best_dev_error):
@@ -239,16 +258,17 @@
                 Yh = self._net_call(X)
                 running_losses.append(criterion(Yh, Y).item())
             return np.mean(running_losses)
 
     def _init_net(self, ds: EncodedDs):
         self.net_class = DefaultNet if self.net_name == 'DefaultNet' else ArNet
 
-        net_kwargs = {'input_size': len(ds[0][0]),
-                      'output_size': len(ds[0][1]),
+        X, Y = ds[0]
+        net_kwargs = {'input_size': len(X),
+                      'output_size': len(Y),
                       'num_hidden': self.num_hidden,
                       'dropout': 0}
 
         if self.net_class == ArNet:
             net_kwargs['encoder_span'] = ds.encoder_spans
             net_kwargs['target_name'] = self.target
 
@@ -270,25 +290,21 @@
         self.started = time.time()
         self.batch_size = min(200, int(len(train_data) / 10))
         self.batch_size = max(40, self.batch_size)
 
         dev_dl = DataLoader(dev_data, batch_size=self.batch_size, shuffle=False)
         train_dl = DataLoader(train_data, batch_size=self.batch_size, shuffle=False)
 
-        self.lr = 1e-4
-        self.num_hidden = 1
-
-        # Find learning rate
-        # keep the weights
+        # Find learning rate & keep initial weights
         self._init_net(train_data)
         if not self.lr:
-            self.lr, self.model = self._find_lr(train_dl)
+            self.lr, self.model = self._find_lr(train_data)
 
         # Keep on training
-        optimizer = self._select_optimizer()
+        optimizer = self._select_optimizer(self.model, lr=self.lr)
         criterion = self._select_criterion()
         scaler = GradScaler()
 
         # Only 0.8 of the remaining time budget is used to allow some time for the final tuning and partial fit
         self.model, epoch_to_best_model, _ = self._max_fit(
             train_dl, dev_dl, criterion, optimizer, scaler, (self.stop_after - (time.time() - self.started)) * 0.8,
             return_model_after=20000)
@@ -310,15 +326,15 @@
         :param dev_data: Data used for early stopping and hyperparameter determination
         """
 
         # Based this on how long the initial training loop took, at a low learning rate as to not mock anything up tooo badly # noqa
         self.started = time.time()
         train_dl = DataLoader(train_data, batch_size=self.batch_size, shuffle=True)
         dev_dl = DataLoader(dev_data, batch_size=self.batch_size, shuffle=True)
-        optimizer = self._select_optimizer()
+        optimizer = self._select_optimizer(self.model, lr=self.lr)
         criterion = self._select_criterion()
         scaler = GradScaler()
 
         self.model, _, _ = self._max_fit(train_dl, dev_dl, criterion, optimizer, scaler,
                                          self.stop_after * 0.1, max(1, int(self.epochs_to_best / 3)))
 
     def __call__(self, ds: EncodedDs,
```

### Comparing `lightwood-23.5.1.1/lightwood/mixer/neural_ts.py` & `lightwood-23.6.2.0/lightwood/mixer/neural_ts.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,18 +3,16 @@
 from typing import Dict, Optional, List
 
 import numpy as np
 import pandas as pd
 
 import torch
 from torch import nn
-import torch_optimizer as ad_optim
 from torch.cuda.amp import GradScaler
 from torch.utils.data import DataLoader
-from torch.optim.optimizer import Optimizer
 
 from type_infer.dtype import dtype
 from lightwood.api.types import PredictionArguments
 from lightwood.encoder.base import BaseEncoder
 from lightwood.data.encoded_ds import EncodedDs, ConcatedEncodedDs
 from lightwood.mixer.neural import Neural
 from lightwood.mixer.helpers.ar_net import ArNet
@@ -72,18 +70,14 @@
         if self.dtype_dict[self.target] in (dtype.integer, dtype.float, dtype.num_tsarray, dtype.quantity):
             criterion = nn.L1Loss()
         else:
             criterion = super()._select_criterion()
 
         return criterion
 
-    def _select_optimizer(self) -> Optimizer:
-        optimizer = ad_optim.Ranger(self.model.parameters(), lr=self.lr)
-        return optimizer
-
     def _fit(self, train_data: EncodedDs, dev_data: EncodedDs) -> None:
         """
         :param train_data: The network is fit/trained on this
         :param dev_data: Data used for early stopping and hyperparameter determination
         """  # noqa
         self.started = time.time()
         original_train = deepcopy(train_data.data_frame)
@@ -102,18 +96,18 @@
 
         self.lr = 1e-4
         self.num_hidden = 1
 
         # Find learning rate
         # keep the weights
         self._init_net(train_data)
-        self.lr, self.model = self._find_lr(train_dl)
+        self.lr, self.model = self._find_lr(train_data)
 
         # Keep on training
-        optimizer = self._select_optimizer()
+        optimizer = self._select_optimizer(self.model, lr=self.lr)
         criterion = self._select_criterion()
         scaler = GradScaler()
 
         # Only 0.8 of the remaining time budget is used to allow some time for the final tuning and partial fit
         self.model, epoch_to_best_model, _ = self._max_fit(
             train_dl, dev_dl, criterion, optimizer, scaler, (self.stop_after - (time.time() - self.started)) * 0.8,
             return_model_after=20000)
```

### Comparing `lightwood-23.5.1.1/lightwood/mixer/nhits.py` & `lightwood-23.6.2.0/lightwood/mixer/nhits.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/prophet.py` & `lightwood-23.6.2.0/lightwood/mixer/prophet.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/qclassic.py` & `lightwood-23.6.2.0/lightwood/mixer/qclassic.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/random_forest.py` & `lightwood-23.6.2.0/lightwood/mixer/random_forest.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from sklearn.metrics import mean_squared_error
 from sklearn.model_selection import check_cv, cross_val_predict
 from sklearn.ensemble import RandomForestRegressor, RandomForestClassifier
 
 from type_infer.dtype import dtype
 from lightwood.helpers.log import log
 from lightwood.encoder.base import BaseEncoder
-from lightwood.data.encoded_ds import ConcatedEncodedDs, EncodedDs
+from lightwood.data.encoded_ds import EncodedDs, ConcatedEncodedDs
 from lightwood.mixer.base import BaseMixer
 from lightwood.api.types import PredictionArguments
 
 
 class RandomForest(BaseMixer):
     model: Union[RandomForestClassifier, RandomForestRegressor]
     dtype_dict: dict
@@ -29,16 +29,16 @@
 
     def __init__(
             self,
             stop_after: float,
             target: str,
             dtype_dict: Dict[str, str],
             fit_on_dev: bool,
-            use_optuna: bool,
-            target_encoder: BaseEncoder
+            target_encoder: BaseEncoder,
+            use_optuna: bool = False,
     ):
         """
         The `RandomForest` mixer supports both regression and classification tasks. 
         It inherits from sklearn.ensemble.RandomForestRegressor and sklearn.ensemble.RandomForestClassifier.
         (https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestRegressor.html)
         (https://scikit-learn.org/stable/modules/generated/sklearn.ensemble.RandomForestClassifier.html)
 
@@ -53,15 +53,15 @@
         self.dtype_dict = dtype_dict
         self.fit_on_dev = fit_on_dev
         self.use_optuna = use_optuna
         self.target_encoder = target_encoder
 
         self.model = None
         self.positive_domain = False
-        self.num_trials = 20
+        self.num_trials = 5
         self.cv = 3
         self.map = {}
 
         self.cls_dtypes = [dtype.categorical, dtype.binary, dtype.cat_tsarray]
         self.float_dtypes = [dtype.float, dtype.quantity, dtype.num_tsarray]
         self.num_dtypes = [dtype.integer] + self.float_dtypes
         self.supports_proba = dtype_dict[target] in self.cls_dtypes
@@ -96,15 +96,14 @@
         if self.fit_on_dev:
             train_data = ConcatedEncodedDs([train_data, dev_data])
 
         # initialize the model
         init_params = {
             'n_estimators': 50,
             'max_depth': 5,
-            'max_features': 1.,
             'bootstrap': True,
             'n_jobs': -1,
             'random_state': 0
         }
 
         if self.is_classifier:
             X = train_data.get_encoded_data(include_target=False)
@@ -124,23 +123,18 @@
             self.model.fit(X, Y)  # sample_weight
 
         # optimize params
         metric, predict_method = (self._multi_logloss, 'predict_proba') if self.is_classifier \
             else (mean_squared_error, 'predict')
 
         def objective(trial: trial_module.Trial):
-            criterion = trial.suggest_categorical("criterion",
-                                                  ["gini", "entropy"]) if self.is_classifier else 'squared_error'
+            criterion = trial.suggest_categorical("criterion", "gini") if self.is_classifier else 'squared_error'
 
             params = {
                 'n_estimators': trial.suggest_int('n_estimators', 2, 512),
-                'max_depth': trial.suggest_int('max_depth', 2, 15),
-                'min_samples_split': trial.suggest_int("min_samples_split", 2, 20),
-                'min_samples_leaf': trial.suggest_int("min_samples_leaf", 1, 20),
-                'max_features': trial.suggest_float("max_features", 0.1, 1),
                 'criterion': criterion,
             }
 
             self.model.set_params(**params)
 
             y_pred = cross_val_predict(self.model, X, Y, cv=self.cv, method=predict_method)
             cv = check_cv(self.cv, Y, classifier=self.is_classifier)  #
@@ -199,15 +193,15 @@
         Call a trained RandomForest mixer to output predictions for the target column.
 
         :param ds: input data with values for all non-target columns.
         :param args: inference-time arguments (e.g. whether to output predicted labels or probabilities).
 
         :return: dataframe with predictions.
         """
-        data = ds.get_encoded_data(include_target=False)
+        data = ds.get_encoded_data(include_target=False).numpy()
 
         if self.is_classifier:
             predictions = self.model.predict_proba(data)
             decoded_predictions = self.model.classes_.take(np.argmax(predictions, axis=1), axis=0)
         else:
             predictions = self.model.predict(data)
             if predictions.ndim == 1:
```

### Comparing `lightwood-23.5.1.1/lightwood/mixer/regression.py` & `lightwood-23.6.2.0/lightwood/mixer/regression.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,18 +83,15 @@
         Make predictions based on datasource with the same features as the ones used for fitting
 
         :param ds: Predictions are generate from it
         :param arg: Any additional arguments used in predicting
 
         :returns: A dataframe cotaining the decoded predictions and (depending on the args) additional information such as the probabilites for each target class
         """ # noqa
-        X = []
-        for x, _ in ds:
-            X.append(x.tolist())
-
+        X = ds.get_encoded_data(include_target=False)
         Yh = self.model.predict(X)
 
         decoded_predictions = self.target_encoder.decode(torch.Tensor(Yh))
 
         ydf = pd.DataFrame({'prediction': decoded_predictions})
 
         if args.predict_proba and self.label_map:
```

### Comparing `lightwood-23.5.1.1/lightwood/mixer/sktime.py` & `lightwood-23.6.2.0/lightwood/mixer/sktime.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/tabtransformer.py` & `lightwood-23.6.2.0/lightwood/mixer/tabtransformer.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/unit.py` & `lightwood-23.6.2.0/lightwood/mixer/unit.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood/mixer/xgboost.py` & `lightwood-23.6.2.0/lightwood/mixer/xgboost.py`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood.egg-info/PKG-INFO` & `lightwood-23.6.2.0/lightwood.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lightwood
-Version: 23.5.1.1
+Version: 23.6.2.0
 Summary: Lightwood is a toolkit for automatic machine learning model building
 Home-page: https://github.com/mindsdb/lightwood
 Author: MindsDB Inc
 Author-email: community@mindsdb.com
 License: GPL-3.0
 Download-URL: https://pypi.org/project/lightwood
 Description: # Lightwood
```

### Comparing `lightwood-23.5.1.1/lightwood.egg-info/SOURCES.txt` & `lightwood-23.6.2.0/lightwood.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `lightwood-23.5.1.1/lightwood.egg-info/requires.txt` & `lightwood-23.6.2.0/lightwood.egg-info/requires.txt`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-type_infer==0.0.9
-dataprep_ml==0.0.8
-mindsdb-evaluator>=0.0.7
+type_infer>=0.0.10
+dataprep_ml>=0.0.9
+mindsdb-evaluator>=0.0.9
 numpy
 nltk<3.6,>=3
 python-dateutil>=2.8.1
 pandas<1.5.0,>=1.1.5
 schema>=0.6.8
 torch<2.1,>=2.0.0
 requests>=2.0.0
@@ -30,28 +30,28 @@
 xgboost<=1.8.0,>=1.6.0
 tab-transformer-pytorch>=0.2.1
 typing-inspect
 six
 regex
 
 [all_extras]
+pyod==1.0.4
+gluonts<0.12.0,>=0.11.0
 autopep8>=1.5.7
-mxnet<2.0.0,>=1.6.0
-pillow>8.3.1
-torchvision<0.11.0,>=0.10.0
-librosa==0.8.1
+shap>=0.40.0
+neuralforecast==1.5.0
 qiskit==0.31.0
 prophet==1.1
-pystan==2.19.1.1
-neuralforecast==1.5.0
-pyod==1.0.4
 lightgbm<=3.3.3,>=3.3.0
-gluonts<0.12.0,>=0.11.0
-shap>=0.40.0
+torchvision
 suod
+pystan==2.19.1.1
+pillow>8.3.1
+librosa==0.8.1
+mxnet<2.0.0,>=1.6.0
 
 [audio]
 librosa==0.8.1
 
 [dev]
 autopep8>=1.5.7
 
@@ -62,15 +62,15 @@
 pystan==2.19.1.1
 prophet==1.1
 neuralforecast==1.5.0
 mxnet<2.0.0,>=1.6.0
 gluonts<0.12.0,>=0.11.0
 
 [image]
-torchvision<0.11.0,>=0.10.0
+torchvision
 pillow>8.3.1
 
 [quantum]
 qiskit==0.31.0
 
 [xai]
 shap>=0.40.0
```

### Comparing `lightwood-23.5.1.1/requirements.txt` & `lightwood-23.6.2.0/requirements.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-type_infer ==0.0.9
-dataprep_ml ==0.0.8
-mindsdb-evaluator >=0.0.7
+type_infer >=0.0.10
+dataprep_ml >=0.0.9
+mindsdb-evaluator >=0.0.9
 numpy
 nltk >=3,<3.6
 python-dateutil >=2.8.1
 pandas >=1.1.5, <1.5.0
 schema >=0.6.8
 torch >=2.0.0, <2.1
 requests >=2.0.0
```

### Comparing `lightwood-23.5.1.1/setup.py` & `lightwood-23.6.2.0/setup.py`

 * *Files identical despite different names*

