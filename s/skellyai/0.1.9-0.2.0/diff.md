# Comparing `tmp/skellyai-0.1.9.tar.gz` & `tmp/skellyai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/skellyai-0.1.9.tar", last modified: Fri Jun  9 20:42:38 2023, max compression
+gzip compressed data, was "dist/skellyai-0.2.0.tar", last modified: Tue Jun 13 03:51:57 2023, max compression
```

## Comparing `skellyai-0.1.9.tar` & `skellyai-0.2.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 20:42:38.374623 skellyai-0.1.9/
--rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-09 20:42:38.373969 skellyai-0.1.9/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-06-09 20:42:38.374778 skellyai-0.1.9/setup.cfg
--rw-r--r--   0 bennicholl   (501) staff       (20)      713 2023-06-09 20:40:39.000000 skellyai-0.1.9/setup.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 20:42:38.366395 skellyai-0.1.9/skellyai/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.1.9/skellyai/__init__.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 20:42:38.370859 skellyai-0.1.9/skellyai/get_multi_labels/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.1.9/skellyai/get_multi_labels/__init__.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     1686 2023-05-19 20:23:21.000000 skellyai-0.1.9/skellyai/get_multi_labels/get_multi_labels.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 20:42:38.372959 skellyai-0.1.9/skellyai/perform_inference/
--rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.1.9/skellyai/perform_inference/__init__.py
--rw-r--r--   0 bennicholl   (501) staff       (20)      838 2023-06-09 19:43:52.000000 skellyai-0.1.9/skellyai/perform_inference/get_probs.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     1922 2023-06-09 20:23:00.000000 skellyai-0.1.9/skellyai/perform_inference/get_probs_mult_keywords.py
--rw-r--r--   0 bennicholl   (501) staff       (20)     3183 2023-05-18 18:08:51.000000 skellyai-0.1.9/skellyai/train_transformer.py
-drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-09 20:42:38.370025 skellyai-0.1.9/skellyai.egg-info/
--rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-09 20:42:38.000000 skellyai-0.1.9/skellyai.egg-info/PKG-INFO
--rw-r--r--   0 bennicholl   (501) staff       (20)      435 2023-06-09 20:42:38.000000 skellyai-0.1.9/skellyai.egg-info/SOURCES.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-06-09 20:42:38.000000 skellyai-0.1.9/skellyai.egg-info/dependency_links.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-06-09 20:42:38.000000 skellyai-0.1.9/skellyai.egg-info/requires.txt
--rw-r--r--   0 bennicholl   (501) staff       (20)       62 2023-06-09 20:42:38.000000 skellyai-0.1.9/skellyai.egg-info/top_level.txt
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 03:51:57.744454 skellyai-0.2.0/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-13 03:51:57.743463 skellyai-0.2.0/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)       38 2023-06-13 03:51:57.744685 skellyai-0.2.0/setup.cfg
+-rw-r--r--   0 bennicholl   (501) staff       (20)      713 2023-06-13 03:51:42.000000 skellyai-0.2.0/setup.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 03:51:57.736591 skellyai-0.2.0/skellyai/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.0/skellyai/__init__.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 03:51:57.739777 skellyai-0.2.0/skellyai/get_multi_labels/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.0/skellyai/get_multi_labels/__init__.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     1686 2023-05-19 20:23:21.000000 skellyai-0.2.0/skellyai/get_multi_labels/get_multi_labels.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 03:51:57.742625 skellyai-0.2.0/skellyai/perform_inference/
+-rw-r--r--   0 bennicholl   (501) staff       (20)        0 2023-05-16 16:47:41.000000 skellyai-0.2.0/skellyai/perform_inference/__init__.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)      838 2023-06-09 19:43:52.000000 skellyai-0.2.0/skellyai/perform_inference/get_probs.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     2501 2023-06-13 03:50:42.000000 skellyai-0.2.0/skellyai/perform_inference/get_probs_mult_keywords.py
+-rw-r--r--   0 bennicholl   (501) staff       (20)     3183 2023-05-18 18:08:51.000000 skellyai-0.2.0/skellyai/train_transformer.py
+drwxr-xr-x   0 bennicholl   (501) staff       (20)        0 2023-06-13 03:51:57.738881 skellyai-0.2.0/skellyai.egg-info/
+-rw-r--r--   0 bennicholl   (501) staff       (20)      407 2023-06-13 03:51:57.000000 skellyai-0.2.0/skellyai.egg-info/PKG-INFO
+-rw-r--r--   0 bennicholl   (501) staff       (20)      435 2023-06-13 03:51:57.000000 skellyai-0.2.0/skellyai.egg-info/SOURCES.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)        1 2023-06-13 03:51:57.000000 skellyai-0.2.0/skellyai.egg-info/dependency_links.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)       33 2023-06-13 03:51:57.000000 skellyai-0.2.0/skellyai.egg-info/requires.txt
+-rw-r--r--   0 bennicholl   (501) staff       (20)       62 2023-06-13 03:51:57.000000 skellyai-0.2.0/skellyai.egg-info/top_level.txt
```

### Comparing `skellyai-0.1.9/skellyai/get_multi_labels/get_multi_labels.py` & `skellyai-0.2.0/skellyai/get_multi_labels/get_multi_labels.py`

 * *Files identical despite different names*

### Comparing `skellyai-0.1.9/skellyai/perform_inference/get_probs.py` & `skellyai-0.2.0/skellyai/perform_inference/get_probs.py`

 * *Files identical despite different names*

### Comparing `skellyai-0.1.9/skellyai/perform_inference/get_probs_mult_keywords.py` & `skellyai-0.2.0/skellyai/perform_inference/get_probs_mult_keywords.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1 +1 @@
-import pandas as pdimport timefrom sagemaker.pytorch.model import PyTorchPredictorfrom sagemaker.deserializers import JSONDeserializerfrom sagemaker.serializers import JSONSerializerfrom sagemaker.predictor_async import AsyncPredictorfrom sagemaker.predictor import Predictordef get_probs(endpoint_key, sentences, questions, df = None):        if type(questions) != list:        raise TypeError("questions parameter must be of type list, with string values inside of that list!")        list_of_probs_for_all_cats = []    for question in questions:            data = {"sentences" : sentences,                     "questions": [question]}                predictor = Predictor(endpoint_name=endpoint_key, serializer=JSONSerializer(), deserializer=JSONDeserializer())        async_predictor = AsyncPredictor(predictor)                        result = async_predictor.predict_async(data, "s3://ask-t5-stage/async_inference/ip")                list_of_probs_for_specific_cat = []                while True:            try:                results = result.get_result()                for result in results:                    list_of_probs_for_specific_cat.append(result[1])                                list_of_probs_for_all_cats.append(list_of_probs_for_specific_cat)                break            except:                time.sleep(5)        if df == None:        return list_of_probs_for_all_cats        elif isinstance(df, pd.DataFrame):        probs_df = pd.DataFrame(list_of_probs_for_all_cats)        probs_df = probs_df.T        probs_df.columns = questions        df.reset_index(drop=True, inplace=True)        probs_df.reset_index(drop=True, inplace=True)        original_df_with_probs = pd.concat([df, probs_df], axis=1)                return original_df_with_probs        else:        raise TypeError("df parameter must be of type pandas dataframe!")        
+import pandas as pdimport timefrom sagemaker.pytorch.model import PyTorchPredictorfrom sagemaker.deserializers import JSONDeserializerfrom sagemaker.serializers import JSONSerializerfrom sagemaker.predictor_async import AsyncPredictorfrom sagemaker.predictor import Predictordef get_probs(endpoint_key, sentences, questions, df = None, threshold = 0.6):        if type(questions) != list:        raise TypeError("questions parameter must be of type list, with string values inside of that list!")        list_of_probs_for_all_cats = []    for question in questions:            data = {"sentences" : sentences,                     "questions": [question]}                predictor = Predictor(endpoint_name=endpoint_key, serializer=JSONSerializer(), deserializer=JSONDeserializer())        async_predictor = AsyncPredictor(predictor)                        result = async_predictor.predict_async(data, "s3://ask-t5-stage/async_inference/ip")                list_of_probs_for_specific_cat = []                while True:            try:                results = result.get_result()                for result in results:                    list_of_probs_for_specific_cat.append(result[1])                                list_of_probs_for_all_cats.append(list_of_probs_for_specific_cat)                break            except:                time.sleep(5)        transpose_list_of_probs_for_all_cats = [list(i) for i in zip(*list_of_probs_for_all_cats)]    probs_df = pd.DataFrame( transpose_list_of_probs_for_all_cats)    probs_df.columns = questions        """nelow code up until the if isinstance line is responsible for creating a thrid column that has the     respective categories assigned to the respective sentences """    label_results = []    for row in transpose_list_of_probs_for_all_cats:        row_result = []        for i, element in enumerate(row):            if element > 0.5:                row_result.append(questions[i])        label_results.append(row_result)    probs_df['labels'] = label_results                if isinstance(df, pd.DataFrame):            df.reset_index(drop=True, inplace=True)        probs_df.reset_index(drop=True, inplace=True)        original_df_with_probs = pd.concat([df, probs_df], axis=1)                return original_df_with_probs        elif df == None:                return probs_df            else:        raise TypeError("df parameter must be of type pandas dataframe!")
```

### Comparing `skellyai-0.1.9/skellyai/train_transformer.py` & `skellyai-0.2.0/skellyai/train_transformer.py`

 * *Files identical despite different names*

