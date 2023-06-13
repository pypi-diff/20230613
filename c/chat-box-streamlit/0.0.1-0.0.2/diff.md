# Comparing `tmp/chat-box-streamlit-0.0.1.tar.gz` & `tmp/chat-box-streamlit-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chat-box-streamlit-0.0.1.tar", last modified: Sat Jun 10 11:36:57 2023, max compression
+gzip compressed data, was "chat-box-streamlit-0.0.2.tar", last modified: Tue Jun 13 07:20:44 2023, max compression
```

## Comparing `chat-box-streamlit-0.0.1.tar` & `chat-box-streamlit-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:36:57.387960 chat-box-streamlit-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-10 11:36:47.000000 chat-box-streamlit-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-10 11:36:47.000000 chat-box-streamlit-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-10 11:36:57.387960 chat-box-streamlit-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-10 11:36:47.000000 chat-box-streamlit-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:36:57.387960 chat-box-streamlit-0.0.1/chat_box/
--rw-r--r--   0 runner    (1001) docker     (123)      804 2023-06-10 11:36:47.000000 chat-box-streamlit-0.0.1/chat_box/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-10 11:36:57.387960 chat-box-streamlit-0.0.1/chat_box_streamlit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-10 11:36:57.000000 chat-box-streamlit-0.0.1/chat_box_streamlit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-10 11:36:57.000000 chat-box-streamlit-0.0.1/chat_box_streamlit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-10 11:36:57.000000 chat-box-streamlit-0.0.1/chat_box_streamlit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-10 11:36:57.000000 chat-box-streamlit-0.0.1/chat_box_streamlit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-10 11:36:57.000000 chat-box-streamlit-0.0.1/chat_box_streamlit.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-10 11:36:57.387960 chat-box-streamlit-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-10 11:36:49.000000 chat-box-streamlit-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:20:44.885592 chat-box-streamlit-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-13 07:20:27.000000 chat-box-streamlit-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-13 07:20:27.000000 chat-box-streamlit-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-13 07:20:44.885592 chat-box-streamlit-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-06-13 07:20:27.000000 chat-box-streamlit-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:20:44.885592 chat-box-streamlit-0.0.2/chat_box/
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-13 07:20:27.000000 chat-box-streamlit-0.0.2/chat_box/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:20:44.885592 chat-box-streamlit-0.0.2/chat_box_streamlit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-06-13 07:20:44.000000 chat-box-streamlit-0.0.2/chat_box_streamlit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-06-13 07:20:44.000000 chat-box-streamlit-0.0.2/chat_box_streamlit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:20:44.000000 chat-box-streamlit-0.0.2/chat_box_streamlit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 07:20:44.000000 chat-box-streamlit-0.0.2/chat_box_streamlit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 07:20:44.000000 chat-box-streamlit-0.0.2/chat_box_streamlit.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:20:44.885592 chat-box-streamlit-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-06-13 07:20:29.000000 chat-box-streamlit-0.0.2/setup.py
```

### Comparing `chat-box-streamlit-0.0.1/LICENSE` & `chat-box-streamlit-0.0.2/LICENSE`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-Copyright (c) 2018-2021 Streamlit Inc.
+MIT License
+
+Copyright (c) 2022 SSK-14
 
 Permission is hereby granted, free of charge, to any person obtaining a copy
 of this software and associated documentation files (the "Software"), to deal
 in the Software without restriction, including without limitation the rights
 to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
 copies of the Software, and to permit persons to whom the Software is
 furnished to do so, subject to the following conditions:
```

### Comparing `chat-box-streamlit-0.0.1/PKG-INFO` & `chat-box-streamlit-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: 
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/plain
 License-File: LICENSE
```

### Comparing `chat-box-streamlit-0.0.1/chat_box_streamlit.egg-info/PKG-INFO` & `chat-box-streamlit-0.0.2/chat_box_streamlit.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chat-box-streamlit
-Version: 0.0.1
+Version: 0.0.2
 Summary: Seamlessly visualize engaging conversations in a sleek ChatBox.
 Home-page: 
 Author: SSK-14
 Author-email: sanjaykumar1481999@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/plain
 License-File: LICENSE
```

### Comparing `chat-box-streamlit-0.0.1/setup.py` & `chat-box-streamlit-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="chat-box-streamlit",
-    version="0.0.1",
+    version="0.0.2",
     author="SSK-14",
     author_email="sanjaykumar1481999@gmail.com",
     description="Seamlessly visualize engaging conversations in a sleek ChatBox.",
     long_description="ChatBox is a powerful Streamlit component designed to effortlessly display and showcase interactive chat conversations between users. With its seamless integration with Streamlit, ChatBox offers a sleek and intuitive interface for visualizing dynamic dialogues, making it an ideal solution for chatbots, virtual assistants, and interactive conversational applications.",
     long_description_content_type="text/plain",
     url="",
     packages=setuptools.find_packages(),
```

