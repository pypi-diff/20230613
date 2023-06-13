# Comparing `tmp/aifunc-0.3.2.tar.gz` & `tmp/aifunc-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aifunc-0.3.2.tar", max compression
+gzip compressed data, was "aifunc-0.3.3.tar", max compression
```

## Comparing `aifunc-0.3.2.tar` & `aifunc-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0       94 2023-06-13 21:34:20.685507 aifunc-0.3.2/aifunc/__init__.py
--rw-r--r--   0        0        0      278 2023-06-13 21:16:41.149289 aifunc-0.3.2/aifunc/evaluate_answer.py
--rw-r--r--   0        0        0     3104 2023-06-13 21:38:04.332387 aifunc-0.3.2/aifunc/evaluate_answer.yaml
--rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.3.2/aifunc/generate_question.py
--rw-r--r--   0        0        0      403 2023-06-13 21:07:34.602635 aifunc-0.3.2/aifunc/generate_question.yaml
--rw-r--r--   0        0        0     3099 2023-06-13 21:19:44.719890 aifunc-0.3.2/aifunc/utility.py
--rw-r--r--   0        0        0      348 2023-06-13 21:38:17.041688 aifunc-0.3.2/pyproject.toml
--rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0       94 2023-06-13 21:34:20.685507 aifunc-0.3.3/aifunc/__init__.py
+-rw-r--r--   0        0        0      372 2023-06-13 21:47:21.569396 aifunc-0.3.3/aifunc/evaluate_answer.py
+-rw-r--r--   0        0        0     3180 2023-06-13 21:46:26.251737 aifunc-0.3.3/aifunc/evaluate_answer.yaml
+-rw-r--r--   0        0        0      126 2023-06-13 21:16:09.346300 aifunc-0.3.3/aifunc/generate_question.py
+-rw-r--r--   0        0        0      403 2023-06-13 21:07:34.602635 aifunc-0.3.3/aifunc/generate_question.yaml
+-rw-r--r--   0        0        0     3099 2023-06-13 21:19:44.719890 aifunc-0.3.3/aifunc/utility.py
+-rw-r--r--   0        0        0      348 2023-06-13 21:47:44.251717 aifunc-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0      403 1970-01-01 00:00:00.000000 aifunc-0.3.3/PKG-INFO
```

### Comparing `aifunc-0.3.2/aifunc/evaluate_answer.yaml` & `aifunc-0.3.3/aifunc/evaluate_answer.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 function_name: "evaluate_answer"
 instruction: |
-  Given a question, a reference answer and the answer, evaluate the answer based on its presentation and content.
+  Given a question, a reference answer and the myanswer, evaluate the myanswer based on its presentation and content. Provide suggest answer at the end.
   Presentation will be scored out of 20 points, considering factors like clarity, coherence, and language.
-  Content will be scored out of 80 points, based on the amount of information from the reference answer that is captured in the provided answer.
+  Content will be scored out of 80 points, based on the amount of information from the reference answer that is captured in the myanswer.
   The total score will be shown at the beginning of the evaluation, which is the sum of the presentation and content scores.
   Points can be deducted for any drawbacks in the answer. Give specific suggestions for improvement if possible.
   Provide the suggested answer at the end which combines the reference answer and user answer only if the user answer provides additional value to the question.
 
 example_conversations: 
   - prompt: |
       What is a performance contract?
       Reference Answer: Performance contracts enable fine-grained prediction and scrutiny of NF.
-      Performance contract characterizes the NF performance.
+      myanswer: Performance contract characterizes the NF performance.
 
     answer: |
-      Total score: 75
-      Content score: 60
-      Evaluation: The answer captures some of the reference answer information but not entirely. The reference answer implies that performance contracts allow for detailed prediction and monitoring of NF (Network Functions), while the answer simply states that a performance contract characterizes NF performance. The details about "fine-grained prediction" and "scrutiny" aren't present in the answer.
-      Presentation score: 15
-      Evaluation: The presentation is mostly clear and coherent but could use more sophisticated language. Suggestion for improvement: Try to use more technical vocabulary related to the topic and ensure the sentences flow well with each other for better coherence.
-      Suggested Answer: As the user's answer does not provide additional value, the suggested answer is the same as the reference answer: 'Performance contracts enable fine-grained prediction and scrutiny of NF.'
+        Total score: 75
+        Content score: 60
+        Evaluation: The answer captures some of the reference answer information but not entirely. The reference answer implies that performance contracts allow for detailed prediction and monitoring of NF (Network Functions), while the answer simply states that a performance contract characterizes NF performance. The details about "fine-grained prediction" and "scrutiny" aren't present in the answer.
+        Presentation score: 15
+        Evaluation: The presentation is mostly clear and coherent but could use more sophisticated language. Suggestion for improvement: Try to use more technical vocabulary related to the topic and ensure the sentences flow well with each other for better coherence.
+        Suggested Answer: As the user's answer does not provide additional value, the suggested answer is the same as the reference answer: 'Performance contracts enable fine-grained prediction and scrutiny of NF.'
       
   - prompt: |
       Can you explain the Vigor approach and how it verifies that NF code is memory-safe and satisfies semantic properties?
       Reference Answer: Vigor, which verifies that NF code written in C satisfies semantic properties and is memory-safe by assuming clear separation of NF code into a library of commonly used NF data structures, verified by experts, and stateless NF logic using the verified library and verified automatically using symbolic execution.
-      I do not know.
+      myanswer: I do not know.
     answer: |
-      Total score: 0
-      Content score: 0
-      Evaluation: Not attempted.
-      Presentation score: 0
-      Evaluation: Not Attempted
-      Suggested Answer: Since the answer is not attempted, the suggested answer is the same as the reference answer. Vigor, which verifies that NF code written in C satisfies semantic properties and is memory-safe by assuming clear separation of NF code into a library of commonly used NF data structures, verified by experts, and stateless NF logic using the verified library and verified automatically using symbolic execution.
+        Total score: 0
+        Content score: 0
+        Evaluation: Not attempted.
+        Presentation score: 0
+        Evaluation: Not Attempted
+        Suggested Answer: Since the answer is not attempted, the suggested answer is the same as the reference answer. Vigor, which verifies that NF code written in C satisfies semantic properties and is memory-safe by assuming clear separation of NF code into a library of commonly used NF data structures, verified by experts, and stateless NF logic using the verified library and verified automatically using symbolic execution.
```

### Comparing `aifunc-0.3.2/aifunc/utility.py` & `aifunc-0.3.3/aifunc/utility.py`

 * *Files identical despite different names*

