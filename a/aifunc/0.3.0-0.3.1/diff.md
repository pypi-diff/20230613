# Comparing `tmp/aifunc-0.3.0.tar.gz` & `tmp/aifunc-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.3.0.tar", max compression
+gzip compressed data, was "aifunc-0.3.1.tar", max compression
```

## Comparing `aifunc-0.3.0.tar` & `aifunc-0.3.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0      116 2023-06-13 21:25:04.012556 aifunc-0.3.0/aifunc/__init__.py
--rw-r--r--   0        0        0      278 2023-06-13 21:16:41.149289 aifunc-0.3.0/aifunc/evaluate_answer.py
--rw-r--r--   0        0        0     3158 2023-06-13 21:23:31.819124 aifunc-0.3.0/aifunc/evaluate_answer.yaml
--rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.3.0/aifunc/generate_question.py
--rw-r--r--   0        0        0      403 2023-06-13 21:07:34.602635 aifunc-0.3.0/aifunc/generate_question.yaml
--rw-r--r--   0        0        0     3099 2023-06-13 21:19:44.719890 aifunc-0.3.0/aifunc/utility.py
--rw-r--r--   0        0        0      348 2023-06-13 21:25:25.734778 aifunc-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      116 2023-06-13 21:25:04.012556 aifunc-0.3.1/aifunc/__init__.py
+-rw-r--r--   0        0        0      278 2023-06-13 21:16:41.149289 aifunc-0.3.1/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0     4242 2023-06-13 21:31:19.370957 aifunc-0.3.1/aifunc/evaluate_answer.yaml
+-rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.3.1/aifunc/generate_question.py
+-rw-r--r--   0        0        0      403 2023-06-13 21:07:34.602635 aifunc-0.3.1/aifunc/generate_question.yaml
+-rw-r--r--   0        0        0     3099 2023-06-13 21:19:44.719890 aifunc-0.3.1/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-13 21:33:00.825337 aifunc-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.3.1/PKG-INFO
```

### Comparing `aifunc-0.3.0/aifunc/evaluate_answer.yaml` & `aifunc-0.3.1/aifunc/evaluate_answer.yaml`

 * *Files 20% similar despite different names*

```diff
@@ -29,7 +29,19 @@
     answer: |
       Total score: 98
       Content score: 80
       Evaluation: The answer captures most of the reference answer information and adds additional valuable details about the nature of performance contracts. It could be improved by including the "fine-grained prediction" aspect mentioned in the reference answer.
       Presentation score: 18
       Evaluation: The presentation is clear, coherent, and uses appropriate language. Suggestion for improvement: Consider rephrasing "binding agreement" to something more specific and related to the topic, like "operational agreement in network functionality."
       Suggested Answer: Performance contracts, allowing for systematic observation and detailed analysis, serve as an operational agreement in network functionality. They enable fine-grained prediction and scrutiny of NF.
+      
+  - prompt: |
+      Can you explain the Vigor approach and how it verifies that NF code is memory-safe and satisfies semantic properties?
+      Reference Answer: Vigor, which verifies that NF code written in C satisfies semantic properties and is memory-safe by assuming clear separation of NF code into a library of commonly used NF data structures, verified by experts, and stateless NF logic using the verified library and verified automatically using symbolic execution.
+      I do not know.
+    answer: |
+      Total score: 0
+      Content score: 0
+      Evaluation: Not attempted.
+      Presentation score: 0
+      Evaluation: Not Attempted
+      Suggested Answer: Since the answer is not attempted, the suggested answer is the same as the reference answer. Vigor, which verifies that NF code written in C satisfies semantic properties and is memory-safe by assuming clear separation of NF code into a library of commonly used NF data structures, verified by experts, and stateless NF logic using the verified library and verified automatically using symbolic execution.
```

### Comparing `aifunc-0.3.0/aifunc/utility.py` & `aifunc-0.3.1/aifunc/utility.py`

 * *Files identical despite different names*

