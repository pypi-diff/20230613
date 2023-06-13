# Comparing `tmp/probabilistic_word_embeddings-1.6.1.tar.gz` & `tmp/probabilistic_word_embeddings-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "probabilistic_word_embeddings-1.6.1.tar", max compression
+gzip compressed data, was "probabilistic_word_embeddings-1.6.2.tar", max compression
```

## Comparing `probabilistic_word_embeddings-1.6.1.tar` & `probabilistic_word_embeddings-1.6.2.tar`

### file list

```diff
@@ -1,23 +1,22 @@
--rw-r--r--   0        0        0     3406 2023-01-18 15:20:33.692173 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/__init__.py
--rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/Card-660.tsv
--rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/MC-30.tsv
--rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
--rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
--rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
--rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/RG-65.tsv
--rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
--rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/SimLex999.tsv
--rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
--rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
--rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
--rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
--rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/YP-130.tsv
--rw-r--r--   0        0        0     7906 2023-05-17 12:15:14.341861 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/embeddings.py
--rw-r--r--   0        0        0    11777 2023-05-17 11:39:54.078679 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/estimation.py
--rwxr-xr-x   0        0        0    10644 2023-05-15 09:22:12.221715 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/evaluation.py
--rw-r--r--   0        0        0     3551 2023-04-25 13:31:30.615164 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/models.py
--rw-r--r--   0        0        0     5699 2023-04-28 08:50:42.813909 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/preprocessing.py
--rw-r--r--   0        0        0     4239 2023-05-16 14:18:02.589041 probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/utils.py
--rw-r--r--   0        0        0      488 2023-05-17 12:15:58.559102 probabilistic_word_embeddings-1.6.1/pyproject.toml
--rw-r--r--   0        0        0      828 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.6.1/setup.py
--rw-r--r--   0        0        0      781 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0     3406 2023-01-18 15:20:33.692173 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/__init__.py
+-rw-r--r--   0        0        0    17101 2022-02-11 12:52:21.792289 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/Card-660.tsv
+-rw-r--r--   0        0        0      544 2022-02-11 12:52:21.794652 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/MC-30.tsv
+-rw-r--r--   0        0        0    53593 2022-02-11 12:52:21.797827 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv
+-rw-r--r--   0        0        0     7219 2022-02-11 12:52:21.805255 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/MTurk-287.tsv
+-rw-r--r--   0        0        0    19626 2022-11-07 15:05:53.936879 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/MTurk-771.tsv
+-rw-r--r--   0        0        0     1209 2022-02-11 12:52:21.810618 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/RG-65.tsv
+-rw-r--r--   0        0        0    49851 2022-02-11 12:52:21.813786 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv
+-rw-r--r--   0        0        0    18024 2022-02-11 12:52:21.820517 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/SimLex999.tsv
+-rw-r--r--   0        0        0    62470 2022-02-11 12:52:21.823693 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv
+-rw-r--r--   0        0        0     7405 2022-02-11 12:52:21.830909 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv
+-rw-r--r--   0        0        0     5134 2022-02-11 12:52:21.833629 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv
+-rw-r--r--   0        0        0     4002 2022-02-11 12:52:21.835687 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv
+-rw-r--r--   0        0        0     2614 2022-02-11 12:52:21.837905 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/YP-130.tsv
+-rw-r--r--   0        0        0     7906 2023-05-17 12:15:14.341861 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/embeddings.py
+-rw-r--r--   0        0        0    11777 2023-05-17 11:39:54.078679 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/estimation.py
+-rwxr-xr-x   0        0        0    10644 2023-05-15 09:22:12.221715 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/evaluation.py
+-rw-r--r--   0        0        0     3551 2023-04-25 13:31:30.615164 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/models.py
+-rw-r--r--   0        0        0     5699 2023-04-28 08:50:42.813909 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/preprocessing.py
+-rw-r--r--   0        0        0     4239 2023-05-16 14:18:02.589041 probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/utils.py
+-rw-r--r--   0        0        0      484 2023-06-13 11:50:16.393042 probabilistic_word_embeddings-1.6.2/pyproject.toml
+-rw-r--r--   0        0        0      766 1970-01-01 00:00:00.000000 probabilistic_word_embeddings-1.6.2/PKG-INFO
```

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/__init__.py` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/__init__.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/Card-660.tsv` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/Card-660.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/MC-30.tsv` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/MC-30.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/MEN-TR-3k.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/MTurk-287.tsv` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/MTurk-287.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/MTurk-771.tsv` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/MTurk-771.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/RG-65.tsv` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/RG-65.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/RW-STANFORD.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/SimLex999.tsv` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/SimLex999.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/SimVerb-3500.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/WS-353-ALL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/WS-353-REL.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/WS-353-SIM.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/data/eval/YP-130.tsv` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/data/eval/YP-130.tsv`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/embeddings.py` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/embeddings.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/estimation.py` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/estimation.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/evaluation.py` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/evaluation.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/models.py` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/models.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/preprocessing.py` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/preprocessing.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/probabilistic_word_embeddings/utils.py` & `probabilistic_word_embeddings-1.6.2/probabilistic_word_embeddings/utils.py`

 * *Files identical despite different names*

### Comparing `probabilistic_word_embeddings-1.6.1/PKG-INFO` & `probabilistic_word_embeddings-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: probabilistic-word-embeddings
-Version: 1.6.1
+Version: 1.6.2
 Summary: Probabilistic Word Embeddings for Python
 License: MIT
 Author: Your Name
 Author-email: you@example.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -15,8 +15,8 @@
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: colorlog
 Requires-Dist: networkx
 Requires-Dist: pandas
 Requires-Dist: progressbar2
 Requires-Dist: scikit-learn
 Requires-Dist: tensorflow (>=2.2,<3.0)
-Requires-Dist: tensorflow-probability (>=0.11,<0.12)
+Requires-Dist: tensorflow-probability
```

