# Comparing `tmp/span_marker-1.1.0.tar.gz` & `tmp/span_marker-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "span_marker-1.1.0.tar", last modified: Sat Jun 10 13:24:05 2023, max compression
+gzip compressed data, was "span_marker-1.1.1.tar", last modified: Tue Jun 13 13:15:24 2023, max compression
```

## Comparing `span_marker-1.1.0.tar` & `span_marker-1.1.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-06-10 13:24:05.389672 span_marker-1.1.0/
--rw-rw-rw-   0        0        0    11558 2023-05-04 23:33:40.000000 span_marker-1.1.0/LICENSE
--rw-rw-rw-   0        0        0     7875 2023-06-10 13:24:05.389672 span_marker-1.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     7298 2023-06-01 10:38:31.000000 span_marker-1.1.0/README.md
--rw-rw-rw-   0        0        0     2455 2023-06-10 13:15:43.000000 span_marker-1.1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-10 13:24:05.389672 span_marker-1.1.0/setup.cfg
--rw-rw-rw-   0        0        0       41 2023-03-28 09:28:01.000000 span_marker-1.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-10 13:24:05.377657 span_marker-1.1.0/span_marker/
--rw-rw-rw-   0        0        0      446 2023-06-10 13:15:59.000000 span_marker-1.1.0/span_marker/__init__.py
--rw-rw-rw-   0        0        0     7018 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/configuration.py
--rw-rw-rw-   0        0        0     6630 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/data_collator.py
--rw-rw-rw-   0        0        0     5066 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/evaluation.py
--rw-rw-rw-   0        0        0     5230 2023-05-31 13:34:45.000000 span_marker-1.1.0/span_marker/label_normalizer.py
--rw-rw-rw-   0        0        0     2471 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/model_card.py
--rw-rw-rw-   0        0        0    30144 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/modeling.py
--rw-rw-rw-   0        0        0     2221 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/output.py
--rw-rw-rw-   0        0        0    11885 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/tokenizer.py
--rw-rw-rw-   0        0        0    19774 2023-06-10 13:15:43.000000 span_marker-1.1.0/span_marker/trainer.py
-drwxrwxrwx   0        0        0        0 2023-06-10 13:24:05.382163 span_marker-1.1.0/span_marker.egg-info/
--rw-rw-rw-   0        0        0     7875 2023-06-10 13:24:05.000000 span_marker-1.1.0/span_marker.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      573 2023-06-10 13:24:05.000000 span_marker-1.1.0/span_marker.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-10 13:24:05.000000 span_marker-1.1.0/span_marker.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      255 2023-06-10 13:24:05.000000 span_marker-1.1.0/span_marker.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-06-10 13:24:05.000000 span_marker-1.1.0/span_marker.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-10 13:24:05.388668 span_marker-1.1.0/tests/
--rw-rw-rw-   0        0        0     1645 2023-06-10 13:15:43.000000 span_marker-1.1.0/tests/test_configuration.py
--rw-rw-rw-   0        0        0     1410 2023-06-01 07:33:08.000000 span_marker-1.1.0/tests/test_model_card.py
--rw-rw-rw-   0        0        0     7875 2023-06-10 13:15:43.000000 span_marker-1.1.0/tests/test_modeling.py
--rw-rw-rw-   0        0        0     8733 2023-06-10 13:15:43.000000 span_marker-1.1.0/tests/test_trainer.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:15:24.035314 span_marker-1.1.1/
+-rw-rw-rw-   0        0        0    11558 2023-05-04 23:33:40.000000 span_marker-1.1.1/LICENSE
+-rw-rw-rw-   0        0        0     7875 2023-06-13 13:15:24.034295 span_marker-1.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7298 2023-06-01 10:38:31.000000 span_marker-1.1.1/README.md
+-rw-rw-rw-   0        0        0     2455 2023-06-10 13:15:43.000000 span_marker-1.1.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 13:15:24.035314 span_marker-1.1.1/setup.cfg
+-rw-rw-rw-   0        0        0       41 2023-03-28 09:28:01.000000 span_marker-1.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:15:24.025295 span_marker-1.1.1/span_marker/
+-rw-rw-rw-   0        0        0      446 2023-06-13 13:12:22.000000 span_marker-1.1.1/span_marker/__init__.py
+-rw-rw-rw-   0        0        0     7018 2023-06-10 13:15:43.000000 span_marker-1.1.1/span_marker/configuration.py
+-rw-rw-rw-   0        0        0     6630 2023-06-13 12:59:46.000000 span_marker-1.1.1/span_marker/data_collator.py
+-rw-rw-rw-   0        0        0     5066 2023-06-10 13:15:43.000000 span_marker-1.1.1/span_marker/evaluation.py
+-rw-rw-rw-   0        0        0     5230 2023-05-31 13:34:45.000000 span_marker-1.1.1/span_marker/label_normalizer.py
+-rw-rw-rw-   0        0        0     2472 2023-06-10 15:07:22.000000 span_marker-1.1.1/span_marker/model_card.py
+-rw-rw-rw-   0        0        0    30304 2023-06-13 13:02:18.000000 span_marker-1.1.1/span_marker/modeling.py
+-rw-rw-rw-   0        0        0     2221 2023-06-10 13:15:43.000000 span_marker-1.1.1/span_marker/output.py
+-rw-rw-rw-   0        0        0    11885 2023-06-13 12:59:46.000000 span_marker-1.1.1/span_marker/tokenizer.py
+-rw-rw-rw-   0        0        0    19774 2023-06-13 12:59:46.000000 span_marker-1.1.1/span_marker/trainer.py
+drwxrwxrwx   0        0        0        0 2023-06-13 13:15:24.030294 span_marker-1.1.1/span_marker.egg-info/
+-rw-rw-rw-   0        0        0     7875 2023-06-13 13:15:23.000000 span_marker-1.1.1/span_marker.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      573 2023-06-13 13:15:24.000000 span_marker-1.1.1/span_marker.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 13:15:23.000000 span_marker-1.1.1/span_marker.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      255 2023-06-13 13:15:23.000000 span_marker-1.1.1/span_marker.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-06-13 13:15:23.000000 span_marker-1.1.1/span_marker.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 13:15:24.034295 span_marker-1.1.1/tests/
+-rw-rw-rw-   0        0        0     1645 2023-06-10 13:15:43.000000 span_marker-1.1.1/tests/test_configuration.py
+-rw-rw-rw-   0        0        0     1410 2023-06-01 07:33:08.000000 span_marker-1.1.1/tests/test_model_card.py
+-rw-rw-rw-   0        0        0     8329 2023-06-13 13:09:20.000000 span_marker-1.1.1/tests/test_modeling.py
+-rw-rw-rw-   0        0        0     8733 2023-06-10 13:15:43.000000 span_marker-1.1.1/tests/test_trainer.py
```

### Comparing `span_marker-1.1.0/LICENSE` & `span_marker-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.0/PKG-INFO` & `span_marker-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: span_marker
-Version: 1.1.0
+Version: 1.1.1
 Summary: Few-Shot Named Entity Recognition using Span Markers
 Author: Tom Aarsen
 Maintainer: Tom Aarsen
 Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER
 Project-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER
 Keywords: data-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-learning,transformers
 Requires-Python: >=3.7
```

### Comparing `span_marker-1.1.0/README.md` & `span_marker-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.0/pyproject.toml` & `span_marker-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.0/span_marker/configuration.py` & `span_marker-1.1.1/span_marker/configuration.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.0/span_marker/data_collator.py` & `span_marker-1.1.1/span_marker/data_collator.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.0/span_marker/evaluation.py` & `span_marker-1.1.1/span_marker/evaluation.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.0/span_marker/label_normalizer.py` & `span_marker-1.1.1/span_marker/label_normalizer.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.0/span_marker/model_card.py` & `span_marker-1.1.1/span_marker/model_card.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 - ner
 - named-entity-recognition
 pipeline_tag: token-classification
 ---
 
 # SpanMarker for Named Entity Recognition
 
-This is a [SpanMarker](https://github.com/tomaarsen/SpanMarkerNER) model that can be used\
+This is a [SpanMarker](https://github.com/tomaarsen/SpanMarkerNER) model that can be used \
 for Named Entity Recognition. {% if encoder_name_or_path %}In particular, this SpanMarker model uses \
 {% if is_public_model %}\
 [{{ encoder_name_or_path }}](https://huggingface.co/{{ encoder_name_or_path }})\
 {% else %}\
 "{{ encoder_name_or_path }}"\
 {% endif %} as the underlying encoder. {% endif %}
```

### Comparing `span_marker-1.1.0/span_marker/modeling.py` & `span_marker-1.1.1/span_marker/modeling.py`

 * *Files 1% similar despite different names*

```diff
@@ -379,20 +379,22 @@
 
         # Disable dropout, etc.
         self.eval()
 
         if not inputs:
             return []
 
+        # Track whether the input was a string sentence or a list of tokens
+        single_input = False
         # Check if inputs is a string, i.e. a string sentence, or
         # if it is a list of strings without spaces, i.e. if it's 1 tokenized sentence
         if isinstance(inputs, str) or (
             isinstance(inputs, list) and all(isinstance(element, str) and " " not in element for element in inputs)
         ):
-            # return self._predict_one(inputs, allow_overlapping=allow_overlapping)
+            single_input = True
             dataset = Dataset.from_dict({"tokens": [inputs]})
 
         # Otherwise, we likely have a list of strings, i.e. a list of string sentences,
         # or a list of lists of strings, i.e. a list of tokenized sentences
         # if isinstance(inputs, list) and all(isinstance(element, str) and " " not in element for element in inputs):
         # return [self._predict_one(sentence) for sentence in inputs]
         elif isinstance(inputs, list):
@@ -514,15 +516,16 @@
                 sorted(
                     sentence_entities,
                     key=lambda entity: entity["char_start_index"]
                     if isinstance(sentence, str)
                     else entity["word_start_index"],
                 )
             )
-        if len(all_entities) == 1:
+        # if the input was a string or a list of tokens, return a list of dictionaries
+        if single_input and len(all_entities) == 1:
             return all_entities[0]
         return all_entities
 
     def save_pretrained(
         self,
         save_directory: Union[str, os.PathLike],
         is_main_process: bool = True,
```

### Comparing `span_marker-1.1.0/span_marker/output.py` & `span_marker-1.1.1/span_marker/output.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.0/span_marker/tokenizer.py` & `span_marker-1.1.1/span_marker/tokenizer.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.0/span_marker/trainer.py` & `span_marker-1.1.1/span_marker/trainer.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.0/span_marker.egg-info/PKG-INFO` & `span_marker-1.1.1/span_marker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: span-marker
-Version: 1.1.0
+Version: 1.1.1
 Summary: Few-Shot Named Entity Recognition using Span Markers
 Author: Tom Aarsen
 Maintainer: Tom Aarsen
 Project-URL: Documentation, https://tomaarsen.github.io/SpanMarkerNER
 Project-URL: Repository, https://github.com/tomaarsen/SpanMarkerNER
 Keywords: data-science,natural-language-processing,artificial-intelligence,mlops,nlp,machine-learning,transformers
 Requires-Python: >=3.7
```

### Comparing `span_marker-1.1.0/span_marker.egg-info/SOURCES.txt` & `span_marker-1.1.1/span_marker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.0/tests/test_configuration.py` & `span_marker-1.1.1/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.0/tests/test_model_card.py` & `span_marker-1.1.1/tests/test_model_card.py`

 * *Files identical despite different names*

### Comparing `span_marker-1.1.0/tests/test_modeling.py` & `span_marker-1.1.1/tests/test_modeling.py`

 * *Files 10% similar despite different names*

```diff
@@ -82,22 +82,33 @@
 ) -> None:
     model = finetuned_conll_span_marker_model.try_cuda()
 
     # Single sentence
     pred_entities = model.predict(inputs)
     compare_entities(pred_entities, gold_entities)
 
+    # Single sentence, but nested
+    pred_entity_list = model.predict([inputs])
+    for pred_entities in pred_entity_list:
+        compare_entities(pred_entities, gold_entities)
+
     # Multiple sentences
     pred_entity_list = model.predict([inputs] * 3)
     for pred_entities in pred_entity_list:
         compare_entities(pred_entities, gold_entities)
 
     # As a Dataset
-    pred_entities = model.predict(Dataset.from_dict({"tokens": [inputs]}))
-    compare_entities(pred_entities, gold_entities)
+    pred_entity_list = model.predict(Dataset.from_dict({"tokens": [inputs]}))
+    for pred_entities in pred_entity_list:
+        compare_entities(pred_entities, gold_entities)
+
+    # As a non-singular Dataset
+    pred_entity_list = model.predict(Dataset.from_dict({"tokens": [inputs] * 2}))
+    for pred_entities in pred_entity_list:
+        compare_entities(pred_entities, gold_entities)
 
 
 @pytest.mark.parametrize(
     ("inputs", "gold_entity_list"),
     [
         (
             Dataset.from_dict(
```

### Comparing `span_marker-1.1.0/tests/test_trainer.py` & `span_marker-1.1.1/tests/test_trainer.py`

 * *Files identical despite different names*

