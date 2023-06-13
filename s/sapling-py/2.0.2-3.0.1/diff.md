# Comparing `tmp/sapling-py-2.0.2.tar.gz` & `tmp/sapling-py-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapling-py-2.0.2.tar", last modified: Wed May 31 04:31:40 2023, max compression
+gzip compressed data, was "sapling-py-3.0.1.tar", last modified: Tue Jun 13 20:35:18 2023, max compression
```

## Comparing `sapling-py-2.0.2.tar` & `sapling-py-3.0.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 james      (502) staff       (20)        0 2023-05-31 04:31:40.649584 sapling-py-2.0.2/
--rw-r--r--   0 james      (502) staff       (20)    11357 2022-11-10 06:53:31.000000 sapling-py-2.0.2/LICENSE
--rw-r--r--   0 james      (502) staff       (20)     3321 2023-05-31 04:31:40.649453 sapling-py-2.0.2/PKG-INFO
--rw-r--r--   0 james      (502) staff       (20)     2964 2022-11-10 06:53:31.000000 sapling-py-2.0.2/README.md
-drwxr-xr-x   0 james      (502) staff       (20)        0 2023-05-31 04:31:40.648646 sapling-py-2.0.2/sapling/
--rw-r--r--   0 james      (502) staff       (20)      130 2023-03-30 07:18:05.000000 sapling-py-2.0.2/sapling/__init__.py
--rw-r--r--   0 james      (502) staff       (20)    12946 2023-05-31 04:27:08.000000 sapling-py-2.0.2/sapling/client.py
--rw-r--r--   0 james      (502) staff       (20)       22 2023-05-31 04:27:23.000000 sapling-py-2.0.2/sapling/version.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2023-05-31 04:31:40.649187 sapling-py-2.0.2/sapling_py.egg-info/
--rw-r--r--   0 james      (502) staff       (20)     3321 2023-05-31 04:31:40.000000 sapling-py-2.0.2/sapling_py.egg-info/PKG-INFO
--rw-r--r--   0 james      (502) staff       (20)      269 2023-05-31 04:31:40.000000 sapling-py-2.0.2/sapling_py.egg-info/SOURCES.txt
--rw-r--r--   0 james      (502) staff       (20)        1 2023-05-31 04:31:40.000000 sapling-py-2.0.2/sapling_py.egg-info/dependency_links.txt
--rw-r--r--   0 james      (502) staff       (20)        9 2023-05-31 04:31:40.000000 sapling-py-2.0.2/sapling_py.egg-info/requires.txt
--rw-r--r--   0 james      (502) staff       (20)       13 2023-05-31 04:31:40.000000 sapling-py-2.0.2/sapling_py.egg-info/top_level.txt
--rw-r--r--   0 james      (502) staff       (20)       38 2023-05-31 04:31:40.649622 sapling-py-2.0.2/setup.cfg
--rw-r--r--   0 james      (502) staff       (20)      948 2023-03-30 07:17:57.000000 sapling-py-2.0.2/setup.py
-drwxr-xr-x   0 james      (502) staff       (20)        0 2023-05-31 04:31:40.649315 sapling-py-2.0.2/test/
--rw-r--r--   0 james      (502) staff       (20)        0 2022-11-10 06:53:31.000000 sapling-py-2.0.2/test/__init__.py
+drwxr-xr-x   0 rishabhmarya   (501) staff       (20)        0 2023-06-13 20:35:18.542436 sapling-py-3.0.1/
+-rw-r--r--   0 rishabhmarya   (501) staff       (20)    11357 2023-06-12 19:35:12.000000 sapling-py-3.0.1/LICENSE
+-rw-r--r--   0 rishabhmarya   (501) staff       (20)     3341 2023-06-13 20:35:18.542329 sapling-py-3.0.1/PKG-INFO
+-rw-r--r--   0 rishabhmarya   (501) staff       (20)     2964 2023-06-12 19:35:12.000000 sapling-py-3.0.1/README.md
+drwxr-xr-x   0 rishabhmarya   (501) staff       (20)        0 2023-06-13 20:35:18.541604 sapling-py-3.0.1/sapling/
+-rw-r--r--   0 rishabhmarya   (501) staff       (20)      130 2023-06-12 19:35:12.000000 sapling-py-3.0.1/sapling/__init__.py
+-rw-r--r--   0 rishabhmarya   (501) staff       (20)    17959 2023-06-12 20:07:52.000000 sapling-py-3.0.1/sapling/client.py
+-rw-r--r--   0 rishabhmarya   (501) staff       (20)       22 2023-06-13 20:28:46.000000 sapling-py-3.0.1/sapling/version.py
+drwxr-xr-x   0 rishabhmarya   (501) staff       (20)        0 2023-06-13 20:35:18.542086 sapling-py-3.0.1/sapling_py.egg-info/
+-rw-r--r--   0 rishabhmarya   (501) staff       (20)     3341 2023-06-13 20:35:18.000000 sapling-py-3.0.1/sapling_py.egg-info/PKG-INFO
+-rw-r--r--   0 rishabhmarya   (501) staff       (20)      269 2023-06-13 20:35:18.000000 sapling-py-3.0.1/sapling_py.egg-info/SOURCES.txt
+-rw-r--r--   0 rishabhmarya   (501) staff       (20)        1 2023-06-13 20:35:18.000000 sapling-py-3.0.1/sapling_py.egg-info/dependency_links.txt
+-rw-r--r--   0 rishabhmarya   (501) staff       (20)        9 2023-06-13 20:35:18.000000 sapling-py-3.0.1/sapling_py.egg-info/requires.txt
+-rw-r--r--   0 rishabhmarya   (501) staff       (20)       13 2023-06-13 20:35:18.000000 sapling-py-3.0.1/sapling_py.egg-info/top_level.txt
+-rw-r--r--   0 rishabhmarya   (501) staff       (20)       38 2023-06-13 20:35:18.542470 sapling-py-3.0.1/setup.cfg
+-rw-r--r--   0 rishabhmarya   (501) staff       (20)      948 2023-06-12 19:35:12.000000 sapling-py-3.0.1/setup.py
+drwxr-xr-x   0 rishabhmarya   (501) staff       (20)        0 2023-06-13 20:35:18.542191 sapling-py-3.0.1/test/
+-rw-r--r--   0 rishabhmarya   (501) staff       (20)        0 2023-06-12 19:35:12.000000 sapling-py-3.0.1/test/__init__.py
```

### Comparing `sapling-py-2.0.2/LICENSE` & `sapling-py-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sapling-py-2.0.2/PKG-INFO` & `sapling-py-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: sapling-py
-Version: 2.0.2
+Version: 3.0.1
 Summary: Sapling Python Client
 Home-page: https://sapling.ai
 Author: Sapling Intelligence
 Author-email: info@sapling.ai
 License: Apache License 2.0
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sapling Python Client
 
@@ -87,7 +88,9 @@
 
 License
 -------
 
 Copyright 2022 Sapling Intelligence, Inc.
 
 Licensed under the Apache License, Version 2.0.
+
+
```

### Comparing `sapling-py-2.0.2/README.md` & `sapling-py-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `sapling-py-2.0.2/sapling/client.py` & `sapling-py-3.0.1/sapling/client.py`

 * *Files 18% similar despite different names*

```diff
@@ -50,14 +50,22 @@
         :param variety: Specifies regional English variety preference. Defaults to the configuration in the user Sapling dashboard.
         :type variety: str
         :param medical: If true, the backend will apply Sapling's medical dictionary.
         :type medical: bool
         :param auto_apply: Whether to return a field with edits applied to the text
         :type auto_apply: bool
         :rtype: list[dict]
+        :return:
+            - sentence: Unedited sentence
+            - sentence_start: Offset of sentence from start of text
+            - start: Offset of edit start relative to sentence
+            - end: Offset of edit end relative to sentence
+            - replacement: Suggested replacement
+            - error_type: Error type
+            - general_error_type: General Error type
 
         Supported languages:
             - `de`:  German (Deutsch)
             - `el`:  Greek (Ελληνικά)
             - `en`:  English (US/UK/CA/AU)
             - `es`:  Spanish (Español)
             - `fr`:  French  (Français) (`fr-fr` and `fr-ca` coming soon)
@@ -362,14 +370,21 @@
         '''
         Score a piece of text on how likely it was generated by AI.
 
         :param text: Text to
         :type text: str
         :param sent_scores: If true, each sentence will also be scored individually.
         :type sent_scores: bool
+
+        :rtype: dict
+        :return:
+            - score: float between 0 and 1, probability that text is AI generated
+            - sentence_scores: If sent_scores is set, will return a list of scores per sentence.
+            - text: text that was processed
+
         '''
         url = f'{self.url_endpoint}aidetect'
         data = {
             'key': self.api_key,
             'text': text,
         }
         if sent_scores is not None:
@@ -378,7 +393,134 @@
             url,
             json=data,
             timeout=self.timeout,
         )
         if 200 <= resp.status_code < 300:
             return resp.json()
         raise Exception(f'HTTP {resp.status_code}: resp.text')
+
+    def chunk_text(
+        self,
+        text,
+        max_length,
+        step_size=None,
+    ):
+        '''
+        Break an input text into blocks of length of most max_length. When splitting the text, the API follows the following preference stack:
+
+        page break > paragraph breaks > line breaks > tabs > punctuation > all other whitespace
+
+        :param text: Text to be chunked
+        :type text: str
+        :param max_length: Maximum length of text segments.
+        :type max_length: integer
+        :param step_size: Size of window to look for split points.
+        :type step_size: integer
+        :rtype: dict
+        :return:
+            - chunks: List of resulting chunks
+        '''
+        url = f'{self.url_endpoint}ingest/chunk_text'
+        data = {
+            'key': self.api_key,
+            'text': text,
+            'max_length': max_length
+        }
+        if step_size is not None:
+            data['step_size'] = step_size
+        resp = requests.post(
+            url,
+            json=data,
+            timeout=self.timeout,
+        )
+        if 200 <= resp.status_code < 300:
+            return resp.json()
+        raise Exception(f'HTTP {resp.status_code}: {resp.text}')
+
+    def chunk_html(
+        self,
+        html,
+        max_length,
+        step_size=None,
+    ):
+        '''
+        Break an input text into blocks of length of most max_length. When splitting the text, the API follows the following preference stack:
+
+        page break > paragraph breaks > line breaks > tabs > punctuation > all other whitespace
+
+        Note: This endpoint not only breaks up the HTML but also discards all HTML tags, resulting in plain text.
+
+        :param html: HTML to be chunked
+        :type html: str
+        :param max_length: Maximum length of text segments.
+        :type max_length: integer
+        :param step_size: Size of window to look for split points.
+        :type step_size: integer
+        :rtype: dict
+        :return:
+            - chunks: List of resulting chunks representing the segmented text contained within the HTML
+        '''
+        url = f'{self.url_endpoint}ingest/chunk_html'
+        data = {
+            'key': self.api_key,
+            'html': html,
+            'max_length': max_length
+        }
+        if step_size is not None:
+            data['step_size'] = step_size
+        resp = requests.post(
+            url,
+            json=data,
+            timeout=self.timeout,
+        )
+        if 200 <= resp.status_code < 300:
+            return resp.json()
+        raise Exception(f'HTTP {resp.status_code}: {resp.text}')
+
+    def postprocess(
+        self,
+        text,
+        session_id,
+        operations,
+    ):
+        '''
+        Performs a variety of operations that are useful for working with the outputs of an NLP (whether human or AI) system. These include:
+            - Fixing or restoring punctuation
+            - Fixing capitalization
+            - Fixing or restoring whitespace
+        Example use cases include repairing transcriptions or captions.
+
+        :param text: Text to postprocess
+        :type text: str
+        :param session_id: Unique name or UUID of document or portion of text that is being chunked
+        :type text: str
+        :param operations: Operations to apply. The currently accepted operations are:
+            - capitalize
+            - punctuate
+            - fixspaces
+        :type operations: list[str]
+        :rtype: list[dict]
+        :return:
+            Same as the edits endpoint:
+            - sentence: Unedited sentence
+            - sentence_start: Offset of sentence from start of text
+            - start: Offset of edit start relative to sentence
+            - end: Offset of edit end relative to sentence
+            - replacement: Suggested replacement
+            - error_type: Error type
+            - general_error_type: General Error type
+        '''
+        url = f'{self.url_endpoint}postprocess'
+        data = {
+            'key': self.api_key,
+            'text': text,
+            'session_id': session_id,
+            'operations': operations,
+        }
+        resp = requests.post(
+            url,
+            json=data,
+            timeout=self.timeout,
+        )
+        if 200 <= resp.status_code < 300:
+            return resp.json()
+        raise Exception(f'HTTP {resp.status_code}: {resp.text}')
```

### Comparing `sapling-py-2.0.2/sapling_py.egg-info/PKG-INFO` & `sapling-py-3.0.1/sapling_py.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: sapling-py
-Version: 2.0.2
+Version: 3.0.1
 Summary: Sapling Python Client
 Home-page: https://sapling.ai
 Author: Sapling Intelligence
 Author-email: info@sapling.ai
 License: Apache License 2.0
+Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Sapling Python Client
 
@@ -87,7 +88,9 @@
 
 License
 -------
 
 Copyright 2022 Sapling Intelligence, Inc.
 
 Licensed under the Apache License, Version 2.0.
+
+
```

### Comparing `sapling-py-2.0.2/setup.py` & `sapling-py-3.0.1/setup.py`

 * *Files identical despite different names*

