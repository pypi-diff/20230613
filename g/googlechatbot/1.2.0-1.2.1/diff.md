# Comparing `tmp/googlechatbot-1.2.0.tar.gz` & `tmp/googlechatbot-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "googlechatbot-1.2.0.tar", last modified: Thu Feb 23 08:19:21 2023, max compression
+gzip compressed data, was "googlechatbot-1.2.1.tar", last modified: Tue Jun 13 09:40:31 2023, max compression
```

## Comparing `googlechatbot-1.2.0.tar` & `googlechatbot-1.2.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:19:21.394895 googlechatbot-1.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-02-23 08:19:10.000000 googlechatbot-1.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-23 08:19:21.394895 googlechatbot-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-02-23 08:19:10.000000 googlechatbot-1.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:19:21.390895 googlechatbot-1.2.0/googlechatbot/
--rw-r--r--   0 runner    (1001) docker     (123)       77 2023-02-23 08:19:10.000000 googlechatbot-1.2.0/googlechatbot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-02-23 08:19:10.000000 googlechatbot-1.2.0/googlechatbot/chat_bot.py
--rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-02-23 08:19:10.000000 googlechatbot-1.2.0/googlechatbot/chat_card.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:19:21.394895 googlechatbot-1.2.0/googlechatbot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-02-23 08:19:21.000000 googlechatbot-1.2.0/googlechatbot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-02-23 08:19:21.000000 googlechatbot-1.2.0/googlechatbot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-23 08:19:21.000000 googlechatbot-1.2.0/googlechatbot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-02-23 08:19:21.000000 googlechatbot-1.2.0/googlechatbot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-02-23 08:19:21.000000 googlechatbot-1.2.0/googlechatbot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-23 08:19:21.394895 googlechatbot-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-02-23 08:19:10.000000 googlechatbot-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-23 08:19:21.394895 googlechatbot-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-02-23 08:19:10.000000 googlechatbot-1.2.0/tests/test_googlechatbot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:40:31.312310 googlechatbot-1.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-06-13 09:40:20.000000 googlechatbot-1.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-13 09:40:31.312310 googlechatbot-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-06-13 09:40:20.000000 googlechatbot-1.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:40:31.312310 googlechatbot-1.2.1/googlechatbot/
+-rw-r--r--   0 runner    (1001) docker     (123)       77 2023-06-13 09:40:20.000000 googlechatbot-1.2.1/googlechatbot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-13 09:40:20.000000 googlechatbot-1.2.1/googlechatbot/chat_bot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2223 2023-06-13 09:40:20.000000 googlechatbot-1.2.1/googlechatbot/chat_card.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:40:31.312310 googlechatbot-1.2.1/googlechatbot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-06-13 09:40:31.000000 googlechatbot-1.2.1/googlechatbot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-06-13 09:40:31.000000 googlechatbot-1.2.1/googlechatbot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 09:40:31.000000 googlechatbot-1.2.1/googlechatbot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-13 09:40:31.000000 googlechatbot-1.2.1/googlechatbot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 09:40:31.000000 googlechatbot-1.2.1/googlechatbot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 09:40:31.312310 googlechatbot-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-13 09:40:20.000000 googlechatbot-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 09:40:31.312310 googlechatbot-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-06-13 09:40:20.000000 googlechatbot-1.2.1/tests/test_googlechatbot.py
```

### Comparing `googlechatbot-1.2.0/LICENSE` & `googlechatbot-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `googlechatbot-1.2.0/PKG-INFO` & `googlechatbot-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googlechatbot
-Version: 1.2.0
+Version: 1.2.1
 Summary: A small package to simplify the creation of Google Chat Bots
 Home-page: https://github.com/javicv/googlechatbot
 Author: Javier Collado
 Author-email: javicv@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `googlechatbot-1.2.0/README.md` & `googlechatbot-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `googlechatbot-1.2.0/googlechatbot/chat_bot.py` & `googlechatbot-1.2.1/googlechatbot/chat_bot.py`

 * *Files identical despite different names*

### Comparing `googlechatbot-1.2.0/googlechatbot/chat_card.py` & `googlechatbot-1.2.1/googlechatbot/chat_card.py`

 * *Files identical despite different names*

### Comparing `googlechatbot-1.2.0/googlechatbot.egg-info/PKG-INFO` & `googlechatbot-1.2.1/googlechatbot.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: googlechatbot
-Version: 1.2.0
+Version: 1.2.1
 Summary: A small package to simplify the creation of Google Chat Bots
 Home-page: https://github.com/javicv/googlechatbot
 Author: Javier Collado
 Author-email: javicv@gmail.com
 License: Apache License 2.0
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `googlechatbot-1.2.0/setup.py` & `googlechatbot-1.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='googlechatbot',
-    version='1.2.0',
+    version='1.2.1',
     description='A small package to simplify the creation of Google Chat Bots',
     long_description=readme,
     long_description_content_type="text/markdown",
     author='Javier Collado',
     author_email='javicv@gmail.com',
     url='https://github.com/javicv/googlechatbot',
     license="Apache License 2.0",
```

### Comparing `googlechatbot-1.2.0/tests/test_googlechatbot.py` & `googlechatbot-1.2.1/tests/test_googlechatbot.py`

 * *Files identical despite different names*

