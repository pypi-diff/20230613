# Comparing `tmp/unittest_gpt-0.1.0.tar.gz` & `tmp/unittest_gpt-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unittest_gpt-0.1.0.tar", max compression
+gzip compressed data, was "unittest_gpt-0.1.1.tar", max compression
```

## Comparing `unittest_gpt-0.1.0.tar` & `unittest_gpt-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1063 2023-06-13 03:30:07.274660 unittest_gpt-0.1.0/LICENSE
--rw-r--r--   0        0        0     5259 2023-06-13 03:30:38.442316 unittest_gpt-0.1.0/README.md
--rw-r--r--   0        0        0      370 2023-06-13 03:30:38.442600 unittest_gpt-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      767 2023-06-13 03:30:38.442889 unittest_gpt-0.1.0/src/Search/binary_search.py
--rw-r--r--   0        0        0     1483 2023-06-13 03:30:38.443043 unittest_gpt-0.1.0/src/file_utils.py
--rw-r--r--   0        0        0     8642 2023-06-13 03:30:38.443216 unittest_gpt-0.1.0/src/unit_test_agent.py
--rw-r--r--   0        0        0     5665 1970-01-01 00:00:00.000000 unittest_gpt-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-13 19:08:18.775053 unittest_gpt-0.1.1/LICENSE
+-rw-r--r--   0        0        0     5259 2023-06-13 03:30:38.442316 unittest_gpt-0.1.1/README.md
+-rw-r--r--   0        0        0      459 2023-06-13 19:10:09.299855 unittest_gpt-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      767 2023-06-13 03:30:38.442889 unittest_gpt-0.1.1/src/Search/binary_search.py
+-rw-r--r--   0        0        0     1483 2023-06-13 03:30:38.443043 unittest_gpt-0.1.1/src/file_utils.py
+-rw-r--r--   0        0        0     8642 2023-06-13 03:30:38.443216 unittest_gpt-0.1.1/src/unit_test_agent.py
+-rw-r--r--   0        0        0     5843 1970-01-01 00:00:00.000000 unittest_gpt-0.1.1/PKG-INFO
```

### Comparing `unittest_gpt-0.1.0/LICENSE` & `unittest_gpt-0.1.1/LICENSE`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 MIT License
 
-Copyright (c) 2023 skuzie
+Copyright (c) 2023 Akshay Lingamaneni
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `unittest_gpt-0.1.0/README.md` & `unittest_gpt-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `unittest_gpt-0.1.0/src/Search/binary_search.py` & `unittest_gpt-0.1.1/src/Search/binary_search.py`

 * *Files identical despite different names*

### Comparing `unittest_gpt-0.1.0/src/file_utils.py` & `unittest_gpt-0.1.1/src/file_utils.py`

 * *Files identical despite different names*

### Comparing `unittest_gpt-0.1.0/src/unit_test_agent.py` & `unittest_gpt-0.1.1/src/unit_test_agent.py`

 * *Files identical despite different names*

### Comparing `unittest_gpt-0.1.0/PKG-INFO` & `unittest_gpt-0.1.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,22 @@
 Metadata-Version: 2.1
 Name: unittest-gpt
-Version: 0.1.0
+Version: 0.1.1
 Summary: Auto generate unit test using PyTest and Gpt
 License: MIT
 Author: Akshay Lingamaneni
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: pytest (>=6.0,<7.0)
+Requires-Dist: autopep8 (>=2.0.2,<3.0.0)
+Requires-Dist: langchain (>=0.0.199,<0.0.200)
+Requires-Dist: openai (>=0.27.8,<0.28.0)
+Requires-Dist: pytest (>=7.3.2,<8.0.0)
+Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 
 <div align="center">
 <h1 align="center">
 <img src="https://raw.githubusercontent.com/PKief/vscode-material-icon-theme/ec559a9f6bfd399b82bb44393651661b08aaf7ba/icons/folder-markdown-open.svg" width="100" />
 <br>
```

