# Comparing `tmp/renard-pipeline-0.1.0.tar.gz` & `tmp/renard_pipeline-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renard-pipeline-0.1.0.tar", max compression
+gzip compressed data, was "renard_pipeline-0.1.1.tar", max compression
```

## Comparing `renard-pipeline-0.1.0.tar` & `renard_pipeline-0.1.1.tar`

### file list

```diff
@@ -1,32 +1,31 @@
--rw-r--r--   0        0        0    35149 2021-10-25 08:27:36.755236 renard-pipeline-0.1.0/LICENSE
--rw-r--r--   0        0        0      700 2023-05-31 07:53:15.539674 renard-pipeline-0.1.0/README.md
--rw-r--r--   0        0        0     1123 2023-06-07 13:32:37.283051 renard-pipeline-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      102 2022-01-19 13:39:41.879749 renard-pipeline-0.1.0/renard/gender.py
--rw-r--r--   0        0        0     5024 2023-05-31 07:53:15.607676 renard-pipeline-0.1.0/renard/graph_utils.py
--rw-r--r--   0        0        0      977 2023-05-31 07:53:15.615676 renard-pipeline-0.1.0/renard/nltk_utils.py
--rw-r--r--   0        0        0       35 2022-03-03 16:21:22.838555 renard-pipeline-0.1.0/renard/pipeline/__init__.py
--rw-r--r--   0        0        0    13433 2023-06-07 11:43:03.784802 renard-pipeline-0.1.0/renard/pipeline/characters_extraction.py
--rw-r--r--   0        0        0    20200 2023-05-31 09:38:26.059941 renard-pipeline-0.1.0/renard/pipeline/core.py
--rw-r--r--   0        0        0       44 2022-09-05 14:31:10.104789 renard-pipeline-0.1.0/renard/pipeline/corefs/__init__.py
--rw-r--r--   0        0        0    41569 2023-04-24 15:18:54.568236 renard-pipeline-0.1.0/renard/pipeline/corefs/bert_corefs.py
--rw-r--r--   0        0        0    10113 2023-03-01 15:12:59.804044 renard-pipeline-0.1.0/renard/pipeline/corefs/corefs.py
--rw-r--r--   0        0        0    15477 2023-05-31 09:18:44.562058 renard-pipeline-0.1.0/renard/pipeline/graph_extraction.py
--rw-r--r--   0        0        0     8470 2023-05-31 07:53:15.615676 renard-pipeline-0.1.0/renard/pipeline/ner.py
--rw-r--r--   0        0        0     1151 2023-05-31 09:18:47.390107 renard-pipeline-0.1.0/renard/pipeline/preconfigured.py
--rw-r--r--   0        0        0      848 2022-02-02 08:44:12.496752 renard-pipeline-0.1.0/renard/pipeline/preprocessing.py
--rw-r--r--   0        0        0     1684 2023-01-23 10:04:47.830213 renard-pipeline-0.1.0/renard/pipeline/progress.py
--rw-r--r--   0        0        0     1489 2023-01-23 10:04:47.862214 renard-pipeline-0.1.0/renard/pipeline/sentiment_analysis.py
--rw-r--r--   0        0        0     8048 2023-01-05 16:45:44.628245 renard-pipeline-0.1.0/renard/pipeline/stanford_corenlp.py
--rw-r--r--   0        0        0     5707 2023-05-31 07:53:15.627676 renard-pipeline-0.1.0/renard/pipeline/tokenization.py
--rw-r--r--   0        0        0     1931 2023-05-31 08:57:09.607082 renard-pipeline-0.1.0/renard/plot_utils.py
--rw-r--r--   0        0        0       55 2022-01-19 09:47:58.225041 renard-pipeline-0.1.0/renard/resources/hypocorisms/__init__.py
--rw-r--r--   0        0        0    11357 2022-01-19 09:47:58.225041 renard-pipeline-0.1.0/renard/resources/hypocorisms/datas/License.txt
--rw-r--r--   0        0        0    21470 2022-01-19 09:47:58.225041 renard-pipeline-0.1.0/renard/resources/hypocorisms/datas/hypocorisms.csv
--rw-r--r--   0        0        0     2720 2023-06-07 09:42:15.373329 renard-pipeline-0.1.0/renard/resources/hypocorisms/hypocorisms.py
--rw-r--r--   0        0        0       49 2022-01-19 13:45:56.740454 renard-pipeline-0.1.0/renard/resources/pronouns/__init__.py
--rw-r--r--   0        0        0      817 2023-06-07 11:33:32.869182 renard-pipeline-0.1.0/renard/resources/pronouns/pronouns.py
--rw-r--r--   0        0        0       45 2023-06-07 11:30:57.743062 renard-pipeline-0.1.0/renard/resources/titles/__init__.py
--rw-r--r--   0        0        0      987 2023-06-07 11:40:28.186772 renard-pipeline-0.1.0/renard/resources/titles/titles.py
--rw-r--r--   0        0        0     3459 2023-05-31 13:00:52.411873 renard-pipeline-0.1.0/renard/utils.py
--rw-r--r--   0        0        0     2046 1970-01-01 00:00:00.000000 renard-pipeline-0.1.0/setup.py
--rw-r--r--   0        0        0     1987 1970-01-01 00:00:00.000000 renard-pipeline-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2021-10-24 09:32:44.395062 renard_pipeline-0.1.1/LICENSE
+-rw-r--r--   0        0        0      700 2023-06-12 16:40:24.076238 renard_pipeline-0.1.1/README.md
+-rw-r--r--   0        0        0     1123 2023-06-12 20:06:32.126658 renard_pipeline-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      102 2022-01-20 08:10:14.365722 renard_pipeline-0.1.1/renard/gender.py
+-rw-r--r--   0        0        0     5024 2023-06-12 16:40:24.077238 renard_pipeline-0.1.1/renard/graph_utils.py
+-rw-r--r--   0        0        0      977 2023-06-12 16:40:24.077238 renard_pipeline-0.1.1/renard/nltk_utils.py
+-rw-r--r--   0        0        0       35 2022-03-08 09:05:03.844457 renard_pipeline-0.1.1/renard/pipeline/__init__.py
+-rw-r--r--   0        0        0    13433 2023-06-12 16:40:24.077238 renard_pipeline-0.1.1/renard/pipeline/characters_extraction.py
+-rw-r--r--   0        0        0    20200 2023-06-12 16:40:24.077238 renard_pipeline-0.1.1/renard/pipeline/core.py
+-rw-r--r--   0        0        0       44 2022-09-04 16:51:08.022976 renard_pipeline-0.1.1/renard/pipeline/corefs/__init__.py
+-rw-r--r--   0        0        0    41569 2023-04-26 07:22:50.834703 renard_pipeline-0.1.1/renard/pipeline/corefs/bert_corefs.py
+-rw-r--r--   0        0        0    10113 2023-03-19 20:56:15.562947 renard_pipeline-0.1.1/renard/pipeline/corefs/corefs.py
+-rw-r--r--   0        0        0    15477 2023-06-12 16:40:24.077238 renard_pipeline-0.1.1/renard/pipeline/graph_extraction.py
+-rw-r--r--   0        0        0     8849 2023-06-12 19:27:25.439530 renard_pipeline-0.1.1/renard/pipeline/ner.py
+-rw-r--r--   0        0        0     1151 2023-06-12 16:40:24.078238 renard_pipeline-0.1.1/renard/pipeline/preconfigured.py
+-rw-r--r--   0        0        0      952 2023-06-12 19:24:34.886891 renard_pipeline-0.1.1/renard/pipeline/preprocessing.py
+-rw-r--r--   0        0        0     1684 2023-01-07 16:22:16.537260 renard_pipeline-0.1.1/renard/pipeline/progress.py
+-rw-r--r--   0        0        0     1489 2023-01-07 16:22:16.537260 renard_pipeline-0.1.1/renard/pipeline/sentiment_analysis.py
+-rw-r--r--   0        0        0     8048 2022-11-21 22:36:54.771428 renard_pipeline-0.1.1/renard/pipeline/stanford_corenlp.py
+-rw-r--r--   0        0        0     5777 2023-06-12 19:27:31.591553 renard_pipeline-0.1.1/renard/pipeline/tokenization.py
+-rw-r--r--   0        0        0     1931 2023-06-12 16:40:24.078238 renard_pipeline-0.1.1/renard/plot_utils.py
+-rw-r--r--   0        0        0       55 2022-01-10 23:56:26.787317 renard_pipeline-0.1.1/renard/resources/hypocorisms/__init__.py
+-rw-r--r--   0        0        0    11357 2022-01-10 15:42:43.716925 renard_pipeline-0.1.1/renard/resources/hypocorisms/datas/License.txt
+-rw-r--r--   0        0        0    21470 2022-01-10 15:37:01.757761 renard_pipeline-0.1.1/renard/resources/hypocorisms/datas/hypocorisms.csv
+-rw-r--r--   0        0        0     2720 2023-06-12 16:40:24.078238 renard_pipeline-0.1.1/renard/resources/hypocorisms/hypocorisms.py
+-rw-r--r--   0        0        0       49 2022-01-20 08:10:14.365722 renard_pipeline-0.1.1/renard/resources/pronouns/__init__.py
+-rw-r--r--   0        0        0      817 2023-06-12 16:40:24.078238 renard_pipeline-0.1.1/renard/resources/pronouns/pronouns.py
+-rw-r--r--   0        0        0       45 2023-06-12 16:40:24.078238 renard_pipeline-0.1.1/renard/resources/titles/__init__.py
+-rw-r--r--   0        0        0      987 2023-06-12 16:40:24.078238 renard_pipeline-0.1.1/renard/resources/titles/titles.py
+-rw-r--r--   0        0        0     3577 2023-06-12 16:40:24.079238 renard_pipeline-0.1.1/renard/utils.py
+-rw-r--r--   0        0        0     1991 1970-01-01 00:00:00.000000 renard_pipeline-0.1.1/PKG-INFO
```

### Comparing `renard-pipeline-0.1.0/LICENSE` & `renard_pipeline-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/README.md` & `renard_pipeline-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/pyproject.toml` & `renard_pipeline-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "renard-pipeline"
-version = "0.1.0"
+version = "0.1.1"
 description = "Relationships Extraction from NARrative Documents"
 authors = ["Arthur Amalvy <arthur.amalvy@univ-avignon.fr>"]
 license = "GPL-3.0-only"
 readme = "README.md"
 packages = [
     { include = "renard" }
 ]
```

### Comparing `renard-pipeline-0.1.0/renard/graph_utils.py` & `renard_pipeline-0.1.1/renard/graph_utils.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/nltk_utils.py` & `renard_pipeline-0.1.1/renard/nltk_utils.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/pipeline/characters_extraction.py` & `renard_pipeline-0.1.1/renard/pipeline/characters_extraction.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/pipeline/core.py` & `renard_pipeline-0.1.1/renard/pipeline/core.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/pipeline/corefs/bert_corefs.py` & `renard_pipeline-0.1.1/renard/pipeline/corefs/bert_corefs.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/pipeline/corefs/corefs.py` & `renard_pipeline-0.1.1/renard/pipeline/corefs/corefs.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/pipeline/graph_extraction.py` & `renard_pipeline-0.1.1/renard/pipeline/graph_extraction.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/pipeline/ner.py` & `renard_pipeline-0.1.1/renard/pipeline/ner.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 from __future__ import annotations
 from typing import List, Dict, Any, Set, Tuple, Optional, Union, Literal
 from dataclasses import dataclass
+from collections import Counter
+import torch
 from torch._C import Value
 from transformers.tokenization_utils_base import BatchEncoding
 from seqeval.metrics import precision_score, recall_score, f1_score
 from renard.nltk_utils import NLTK_ISO_STRING_TO_LANG, nltk_fix_bio_tags
 from renard.pipeline.core import PipelineStep, Mention
 from renard.pipeline.progress import ProgressReporter
 
@@ -144,23 +146,30 @@
 class BertNamedEntityRecognizer(PipelineStep):
     """An entity recognizer based on BERT"""
 
     def __init__(
         self,
         huggingface_model_id: Optional[str] = None,
         batch_size: int = 4,
+        device: Literal["cpu", "cuda", "auto"] = "auto",
     ):
         """
         :param huggingface_model_id: a custom huggingface model id.
             This allows to bypass the ``lang`` pipeline parameter
             which normally choose a huggingface model automatically.
         :param batch_size:
         """
         self.huggingface_model_id = huggingface_model_id
         self.batch_size = batch_size
+
+        if device == "auto":
+            self.device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
+        else:
+            self.device = torch.device(device)
+
         super().__init__()
 
     def _pipeline_init_(self, lang: str, progress_reporter: ProgressReporter):
         from transformers import AutoModelForTokenClassification  # type: ignore
 
         super()._pipeline_init_(lang, progress_reporter)
 
@@ -172,15 +181,15 @@
         else:
             if lang == "eng":
                 self.model = AutoModelForTokenClassification.from_pretrained(
                     "compnet-renard/bert-base-cased-literary-NER"
                 )
             elif lang == "fra":
                 self.model = AutoModelForTokenClassification.from_pretrained(
-                    "Jean-Baptiste/camembert-ner"
+                    "Davlan/bert-base-multilingual-cased-ner-hrl"
                 )
             else:
                 raise ValueError(
                     f"BertNamedEntityRecognizer does not support language {lang}"
                 )
 
     def __call__(
@@ -193,30 +202,31 @@
         """
         :param text:
         :param bert_batch_encoding:
         :param wp_tokens:
         """
         import torch
 
-        device = torch.device("cuda" if torch.cuda.is_available() else "cpu")
-        self.model = self.model.to(device)
+        self.model = self.model.to(self.device)
 
         batches_nb = len(bert_batch_encoding["input_ids"]) // self.batch_size + 1
 
         with torch.no_grad():
             wp_labels = []
 
             for batch_i in self._progress_(range(batches_nb)):
                 batch_start = batch_i * self.batch_size
                 batch_end = batch_start + self.batch_size
                 out = self.model(
-                    bert_batch_encoding["input_ids"][batch_start:batch_end].to(device),
+                    bert_batch_encoding["input_ids"][batch_start:batch_end].to(
+                        self.device
+                    ),
                     attention_mask=bert_batch_encoding["attention_mask"][
                         batch_start:batch_end
-                    ].to(device),
+                    ].to(self.device),
                 )
                 # (batch_size, sentence_size)
                 batch_classes_tens = torch.max(out.logits, dim=2).indices
                 wp_labels += [
                     self.model.config.id2label[tens.item()]
                     for classes_tens in batch_classes_tens
                     for tens in classes_tens
@@ -237,20 +247,27 @@
         """Output a list of labels aligned with regular tokens instead
         of word piece tokens.
 
         :param wp_tokens: word piece tokens
         :param wp_labels: word piece labels
         """
         assert len(wp_tokens) == len(wp_labels)
+
+        # TODO: there is a general way to do that
+        TOKENS_TO_IGNORE = ("[CLS]", "[SEP]", "[PAD]")
+
         labels = []
+
         for wp_token, wp_label in zip(wp_tokens, wp_labels):
-            if wp_token in {"[CLS]", "[SEP]", "[PAD]"}:
+            if wp_token in TOKENS_TO_IGNORE:
                 continue
+
             if not wp_token.startswith("##"):
                 labels.append(wp_label)
+
         return labels
 
     def supported_langs(self) -> Union[Set[str], Literal["any"]]:
         return {"eng", "fra"}
 
     def needs(self) -> Set[str]:
         return {"bert_batch_encoding", "wp_tokens"}
```

### Comparing `renard-pipeline-0.1.0/renard/pipeline/preconfigured.py` & `renard_pipeline-0.1.1/renard/pipeline/preconfigured.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/pipeline/preprocessing.py` & `renard_pipeline-0.1.1/renard/pipeline/preprocessing.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Tuple, Set, Dict, Any
+from typing import List, Tuple, Set, Dict, Any, Literal, Union
 import re
 from renard.pipeline.core import PipelineStep
 
 
 class CustomSubstitutionPreprocessor(PipelineStep):
     """A preprocessor allowing regex-based substition"""
 
@@ -23,7 +23,10 @@
         return {"text": text}
 
     def needs(self) -> Set[str]:
         return set()
 
     def production(self) -> Set[str]:
         return set()
+
+    def supported_langs(self) -> Union[Set[str], Literal["any"]]:
+        return "any"
```

### Comparing `renard-pipeline-0.1.0/renard/pipeline/progress.py` & `renard_pipeline-0.1.1/renard/pipeline/progress.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/pipeline/sentiment_analysis.py` & `renard_pipeline-0.1.1/renard/pipeline/sentiment_analysis.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/pipeline/stanford_corenlp.py` & `renard_pipeline-0.1.1/renard/pipeline/stanford_corenlp.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/pipeline/tokenization.py` & `renard_pipeline-0.1.1/renard/pipeline/tokenization.py`

 * *Files 6% similar despite different names*

```diff
@@ -80,17 +80,17 @@
         if not self.huggingface_model_id is None:
             self.tokenizer = AutoTokenizer.from_pretrained(self.huggingface_model_id)
             self.lang = "unknown"
         else:
             if lang == "eng":
                 self.tokenizer = AutoTokenizer.from_pretrained("bert-base-cased")
             elif lang == "fra":
-                self.tokenizer = AutoTokenizer.from_pretrained("camembert-base")
-            else:
-                raise ValueError(f"BertTokenizer does not support language {lang}")
+                self.tokenizer = AutoTokenizer.from_pretrained(
+                    "Davlan/bert-base-multilingual-cased-ner-hrl"
+                )
 
     def __call__(
         self, text: str, chapters: Optional[List[str]] = None, **kwargs
     ) -> Dict[str, Any]:
         """
         :param text:
         """
@@ -150,18 +150,25 @@
             "chapter_tokens",
         }
 
     @staticmethod
     def wp_tokens_to_tokens(wp_tokens: List[str]) -> List[str]:
         """Convert word piece tokens to 'regular' tokens
 
-        :wp_tokens: word piece tokens
+        :param wp_tokens: word piece tokens
         """
+
+        # TODO: there is a general way to do that
+        TOKENS_TO_IGNORE = ("[CLS]", "[SEP]", "[PAD]")
+
         tokens = []
+
         for wp_token in wp_tokens:
-            if wp_token in {"[CLS]", "[SEP]", "[PAD]"}:
+            if wp_token in TOKENS_TO_IGNORE:
                 continue
+
             if not wp_token.startswith("##"):
                 tokens.append(wp_token)
             else:
                 tokens[-1] += wp_token[2:]
+
         return tokens
```

### Comparing `renard-pipeline-0.1.0/renard/plot_utils.py` & `renard_pipeline-0.1.1/renard/plot_utils.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/resources/hypocorisms/datas/License.txt` & `renard_pipeline-0.1.1/renard/resources/hypocorisms/datas/License.txt`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/resources/hypocorisms/datas/hypocorisms.csv` & `renard_pipeline-0.1.1/renard/resources/hypocorisms/datas/hypocorisms.csv`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/resources/hypocorisms/hypocorisms.py` & `renard_pipeline-0.1.1/renard/resources/hypocorisms/hypocorisms.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/resources/pronouns/pronouns.py` & `renard_pipeline-0.1.1/renard/resources/pronouns/pronouns.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/resources/titles/titles.py` & `renard_pipeline-0.1.1/renard/resources/titles/titles.py`

 * *Files identical despite different names*

### Comparing `renard-pipeline-0.1.0/renard/utils.py` & `renard_pipeline-0.1.1/renard/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -78,30 +78,32 @@
     for subseq_i, subseq in enumerate(windowed(seq, len(pattern))):
         if list(subseq) == pattern:
             start_indices.append(subseq_i)
     return start_indices
 
 
 def load_conll2002_bio(
-    path: str, tag_conversion_map: Optional[Dict[str, str]] = None
+    path: str, tag_conversion_map: Optional[Dict[str, str]] = None, **kwargs
 ) -> Tuple[List[List[str]], List[str], List[str]]:
     """Load a file under CoNLL2022 BIO format.  Sentences are expected
     to be separated by end of lines.
 
     :param path: path to the CoNLL-2002 formatted file
     :param tag_conversion_map: conversion map for tags found in the
-        input file. Example : ``{'B': 'B-PER', 'I': 'I-PER'}``
+        input file.  Example : ``{'B': 'B-PER', 'I': 'I-PER'}``
+    :param kwargs: additional kwargs for ``open`` (such as
+        ``encoding`` or ``newline``).
 
     :return: ``(sentences, tokens, tag)``
     """
 
     if tag_conversion_map is None:
         tag_conversion_map = {}
 
-    with open(os.path.expanduser(path)) as f:
+    with open(os.path.expanduser(path), **kwargs) as f:
         raw_data = f.read()
 
     sents = []
     sent_tokens = []
     tags = []
     for line in raw_data.split("\n"):
         line = line.strip("\n")
```

### Comparing `renard-pipeline-0.1.0/PKG-INFO` & `renard_pipeline-0.1.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 Metadata-Version: 2.1
 Name: renard-pipeline
-Version: 0.1.0
+Version: 0.1.1
 Summary: Relationships Extraction from NARrative Documents
 License: GPL-3.0-only
 Author: Arthur Amalvy
 Author-email: arthur.amalvy@univ-avignon.fr
 Requires-Python: >=3.8,<3.11
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: spacy
 Provides-Extra: stanza
-Requires-Dist: coreferee (>=1.4.0,<2.0.0); extra == "spacy"
+Requires-Dist: coreferee (>=1.4.0,<2.0.0) ; extra == "spacy"
 Requires-Dist: matplotlib (>=3.5.3,<4.0.0)
 Requires-Dist: more-itertools (>=8.12.0,<9.0.0)
 Requires-Dist: nameparser (>=1.1.0,<2.0.0)
 Requires-Dist: networkx (>=2.6.3,<3.0.0)
 Requires-Dist: nltk (>=3.6.5,<4.0.0)
 Requires-Dist: pandas (>=1.4.4,<2.0.0)
 Requires-Dist: pytest (>=7.2.1,<8.0.0)
 Requires-Dist: seqeval (==1.2.2)
-Requires-Dist: spacy (>=3.5.0,<4.0.0); extra == "spacy"
-Requires-Dist: spacy-transformers (>=1.2.1,<2.0.0); extra == "spacy"
-Requires-Dist: stanza (>=1.3.0,<2.0.0); extra == "stanza"
+Requires-Dist: spacy (>=3.5.0,<4.0.0) ; extra == "spacy"
+Requires-Dist: spacy-transformers (>=1.2.1,<2.0.0) ; extra == "spacy"
+Requires-Dist: stanza (>=1.3.0,<2.0.0) ; extra == "stanza"
 Requires-Dist: torch (>=1.10.2,<2.0.0)
 Requires-Dist: tqdm (>=4.62.3,<5.0.0)
 Requires-Dist: transformers (>=4.11.3,<5.0.0)
 Description-Content-Type: text/markdown
 
 # Renard
```

