# Comparing `tmp/langchain_util-0.1.1.tar.gz` & `tmp/langchain_util-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "langchain_util-0.1.1.tar", max compression
+gzip compressed data, was "langchain_util-0.1.7.tar", max compression
```

## Comparing `langchain_util-0.1.1.tar` & `langchain_util-0.1.7.tar`

### file list

```diff
@@ -1,8 +1,17 @@
--rw-r--r--   0        0        0        0 2023-05-07 23:32:05.575677 langchain_util-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-07 23:33:44.665502 langchain_util-0.1.1/langchain_util/__init__.py
--rw-r--r--   0        0        0      105 2023-05-08 00:49:14.383337 langchain_util-0.1.1/langchain_util/chains/__init__.py
--rw-r--r--   0        0        0      310 2023-05-08 00:49:16.495330 langchain_util-0.1.1/langchain_util/chains/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     2873 2023-05-08 22:17:58.624591 langchain_util-0.1.1/langchain_util/chains/__pycache__/concatenate_chain.cpython-311.pyc
--rw-r--r--   0        0        0     1303 2023-05-08 22:17:54.772616 langchain_util-0.1.1/langchain_util/chains/concatenate_chain.py
--rw-r--r--   0        0        0      470 2023-05-09 00:19:56.311297 langchain_util-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      479 1970-01-01 00:00:00.000000 langchain_util-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2023-05-07 23:32:05.575677 langchain_util-0.1.7/README.md
+-rw-r--r--   0        0        0        0 2023-05-07 23:33:44.665502 langchain_util-0.1.7/langchain_util/__init__.py
+-rw-r--r--   0        0        0      201 2023-05-24 14:34:25.789099 langchain_util-0.1.7/langchain_util/chains/__init__.py
+-rw-r--r--   0        0        0      422 2023-05-24 14:47:00.360172 langchain_util-0.1.7/langchain_util/chains/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     2873 2023-05-08 22:17:58.624591 langchain_util-0.1.7/langchain_util/chains/__pycache__/concatenate_chain.cpython-311.pyc
+-rw-r--r--   0        0        0     1303 2023-05-08 22:17:54.772616 langchain_util-0.1.7/langchain_util/chains/concatenate_chain.py
+-rw-r--r--   0        0        0       67 2023-05-24 14:33:46.772328 langchain_util-0.1.7/langchain_util/chains/sentiment/__init__.py
+-rw-r--r--   0        0        0      423 2023-05-24 14:49:11.149647 langchain_util-0.1.7/langchain_util/chains/sentiment/parser.py
+-rw-r--r--   0        0        0     3605 2023-05-24 14:50:10.984649 langchain_util-0.1.7/langchain_util/chains/sentiment/sentiment_chain.py
+-rw-r--r--   0        0        0     1449 2023-05-24 14:49:03.753776 langchain_util-0.1.7/langchain_util/chains/sentiment/stuff_prompt.py
+-rw-r--r--   0        0        0     8495 2023-05-24 14:55:37.040463 langchain_util-0.1.7/langchain_util/text_splitter.py
+-rw-r--r--   0        0        0       90 2023-05-18 00:19:13.373206 langchain_util-0.1.7/langchain_util/tools/__init__.py
+-rw-r--r--   0        0        0      299 2023-05-18 01:10:04.752968 langchain_util-0.1.7/langchain_util/tools/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0        0        0     1992 2023-05-18 01:10:04.752968 langchain_util-0.1.7/langchain_util/tools/__pycache__/agent_as_tool.cpython-311.pyc
+-rw-r--r--   0        0        0     1178 2023-05-18 00:18:40.074432 langchain_util-0.1.7/langchain_util/tools/agent_as_tool.py
+-rw-r--r--   0        0        0      462 2023-06-13 19:36:14.590553 langchain_util-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      481 1970-01-01 00:00:00.000000 langchain_util-0.1.7/PKG-INFO
```

### Comparing `langchain_util-0.1.1/langchain_util/chains/__pycache__/concatenate_chain.cpython-311.pyc` & `langchain_util-0.1.7/langchain_util/chains/__pycache__/concatenate_chain.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `langchain_util-0.1.1/langchain_util/chains/concatenate_chain.py` & `langchain_util-0.1.7/langchain_util/chains/concatenate_chain.py`

 * *Files identical despite different names*

