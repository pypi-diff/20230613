# Comparing `tmp/scratchpad-py-0.0.5.tar.gz` & `tmp/scratchpad-py-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scratchpad-py-0.0.5.tar", last modified: Fri Jun  9 09:04:22 2023, max compression
+gzip compressed data, was "scratchpad-py-0.0.6.tar", last modified: Tue Jun 13 12:05:58 2023, max compression
```

## Comparing `scratchpad-py-0.0.5.tar` & `scratchpad-py-0.0.6.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-09 09:04:22.247809 scratchpad-py-0.0.5/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1074 2023-02-17 01:58:03.000000 scratchpad-py-0.0.5/LICENSE
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3333 2023-06-09 09:04:22.246159 scratchpad-py-0.0.5/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)     2884 2023-02-17 01:58:03.000000 scratchpad-py-0.0.5/README.md
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-09 09:04:22.199780 scratchpad-py-0.0.5/scratchpad/
--rw-r--r--   0 vscode    (1000) vscode    (1000)      845 2023-02-17 01:58:03.000000 scratchpad-py-0.0.5/scratchpad/__init__.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1433 2023-06-09 09:01:35.000000 scratchpad-py-0.0.5/scratchpad/composite_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      650 2023-02-22 06:42:20.000000 scratchpad-py-0.0.5/scratchpad/console_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      635 2023-02-22 06:42:57.000000 scratchpad-py-0.0.5/scratchpad/file_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1465 2023-06-09 09:01:35.000000 scratchpad-py-0.0.5/scratchpad/fluent_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1209 2023-02-22 06:32:15.000000 scratchpad-py-0.0.5/scratchpad/jandi_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      835 2023-02-22 07:03:25.000000 scratchpad-py-0.0.5/scratchpad/line_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      887 2023-02-22 07:03:59.000000 scratchpad-py-0.0.5/scratchpad/logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1491 2023-02-22 03:08:03.000000 scratchpad-py-0.0.5/scratchpad/logger_impl.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      634 2023-02-22 07:03:50.000000 scratchpad-py-0.0.5/scratchpad/logger_interface.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      260 2023-02-22 07:04:40.000000 scratchpad-py-0.0.5/scratchpad/memory_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      130 2023-02-22 07:04:47.000000 scratchpad-py-0.0.5/scratchpad/null_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)       23 2023-02-17 01:58:03.000000 scratchpad-py-0.0.5/scratchpad/retry.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)     1703 2023-02-22 07:05:09.000000 scratchpad-py-0.0.5/scratchpad/scribe_logger.py
--rw-r--r--   0 vscode    (1000) vscode    (1000)      941 2023-02-22 07:05:38.000000 scratchpad-py-0.0.5/scratchpad/telegram_logger.py
-drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-09 09:04:22.241278 scratchpad-py-0.0.5/scratchpad_py.egg-info/
--rw-r--r--   0 vscode    (1000) vscode    (1000)     3333 2023-06-09 09:04:22.000000 scratchpad-py-0.0.5/scratchpad_py.egg-info/PKG-INFO
--rw-r--r--   0 vscode    (1000) vscode    (1000)      610 2023-06-09 09:04:22.000000 scratchpad-py-0.0.5/scratchpad_py.egg-info/SOURCES.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-09 09:04:22.000000 scratchpad-py-0.0.5/scratchpad_py.egg-info/dependency_links.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       80 2023-06-09 09:04:22.000000 scratchpad-py-0.0.5/scratchpad_py.egg-info/requires.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       11 2023-06-09 09:04:22.000000 scratchpad-py-0.0.5/scratchpad_py.egg-info/top_level.txt
--rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-09 09:04:22.248803 scratchpad-py-0.0.5/setup.cfg
--rw-r--r--   0 vscode    (1000) vscode    (1000)      961 2023-06-09 09:01:42.000000 scratchpad-py-0.0.5/setup.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-13 12:05:58.041845 scratchpad-py-0.0.6/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1074 2023-02-17 01:58:03.000000 scratchpad-py-0.0.6/LICENSE
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3497 2023-06-13 12:05:58.040825 scratchpad-py-0.0.6/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3048 2023-06-13 12:05:06.000000 scratchpad-py-0.0.6/README.md
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-13 12:05:58.006745 scratchpad-py-0.0.6/scratchpad/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      902 2023-06-13 11:01:46.000000 scratchpad-py-0.0.6/scratchpad/__init__.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1433 2023-06-09 09:01:35.000000 scratchpad-py-0.0.6/scratchpad/composite_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      650 2023-02-22 06:42:20.000000 scratchpad-py-0.0.6/scratchpad/console_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      635 2023-02-22 06:42:57.000000 scratchpad-py-0.0.6/scratchpad/file_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1453 2023-06-13 11:53:01.000000 scratchpad-py-0.0.6/scratchpad/fluent_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1209 2023-02-22 06:32:15.000000 scratchpad-py-0.0.6/scratchpad/jandi_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      835 2023-06-13 11:54:13.000000 scratchpad-py-0.0.6/scratchpad/line_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      887 2023-02-22 07:03:59.000000 scratchpad-py-0.0.6/scratchpad/logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1491 2023-02-22 03:08:03.000000 scratchpad-py-0.0.6/scratchpad/logger_impl.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      634 2023-02-22 07:03:50.000000 scratchpad-py-0.0.6/scratchpad/logger_interface.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      260 2023-02-22 07:04:40.000000 scratchpad-py-0.0.6/scratchpad/memory_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      130 2023-02-22 07:04:47.000000 scratchpad-py-0.0.6/scratchpad/null_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       23 2023-02-17 01:58:03.000000 scratchpad-py-0.0.6/scratchpad/retry.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     1703 2023-02-22 07:05:09.000000 scratchpad-py-0.0.6/scratchpad/scribe_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      786 2023-06-13 12:02:04.000000 scratchpad-py-0.0.6/scratchpad/slack_logger.py
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      941 2023-02-22 07:05:38.000000 scratchpad-py-0.0.6/scratchpad/telegram_logger.py
+drwxr-xr-x   0 vscode    (1000) vscode    (1000)        0 2023-06-13 12:05:58.036417 scratchpad-py-0.0.6/scratchpad_py.egg-info/
+-rw-r--r--   0 vscode    (1000) vscode    (1000)     3497 2023-06-13 12:05:57.000000 scratchpad-py-0.0.6/scratchpad_py.egg-info/PKG-INFO
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      637 2023-06-13 12:05:57.000000 scratchpad-py-0.0.6/scratchpad_py.egg-info/SOURCES.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)        1 2023-06-13 12:05:57.000000 scratchpad-py-0.0.6/scratchpad_py.egg-info/dependency_links.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       80 2023-06-13 12:05:57.000000 scratchpad-py-0.0.6/scratchpad_py.egg-info/requires.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       11 2023-06-13 12:05:57.000000 scratchpad-py-0.0.6/scratchpad_py.egg-info/top_level.txt
+-rw-r--r--   0 vscode    (1000) vscode    (1000)       38 2023-06-13 12:05:58.042929 scratchpad-py-0.0.6/setup.cfg
+-rw-r--r--   0 vscode    (1000) vscode    (1000)      961 2023-06-13 12:03:16.000000 scratchpad-py-0.0.6/setup.py
```

### Comparing `scratchpad-py-0.0.5/LICENSE` & `scratchpad-py-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.5/PKG-INFO` & `scratchpad-py-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchpad-py
-Version: 0.0.5
+Version: 0.0.6
 Summary: python logger libary
 Home-page: https://github.com/chirichidi/scratch-pad-py
 Author: chirichidi
 Author-email: tolessnoise@gmail.com
 Keywords: logger
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 
 
 mind blowing python toolset. why not pr?
 
 
 # Spec
 
-Loggers: composite, console, file, fluent, jandi, line, memory, null, scribe, telegram
+Loggers: composite, console, file, fluent, jandi, line, memory, null, scribe, telegram, slack
 
 
 
 # Logger interface
 ```
 from .logger_interface import LoggerInterface
 
@@ -96,15 +96,15 @@
     "type": "composite",
     "message": "hello world"
 }
 
 compositLogger = CompositeLogger(
     config={
         "defaults": {
-            "datetime": datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+            "datetime": lambda: datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
             "program": "scratch-pad-python",
         },
         "loggerFilterPairs": [
             {
                 "logger": consoleLogger,
                 "filter": None
             },
@@ -159,14 +159,26 @@
         "type": "fluent",
         "message": "hello world"
     }
 
 logger.info(message)
 ```
 
+SlackLogger
+```
+url = "url"
+logger = SlackLogger(url=url)
+message = {
+    "type": "slack",
+    "message": "hello world"
+}
+
+logger.info(message)
+```
+
 #
 stuff) 
 
 
 scribe-docker for ScribeLogger : https://hub.docker.com/r/polonaiz/facebook-scribe
```

### Comparing `scratchpad-py-0.0.5/README.md` & `scratchpad-py-0.0.6/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 mind blowing python toolset. why not pr?
 
 
 # Spec
 
-Loggers: composite, console, file, fluent, jandi, line, memory, null, scribe, telegram
+Loggers: composite, console, file, fluent, jandi, line, memory, null, scribe, telegram, slack
 
 
 
 # Logger interface
 ```
 from .logger_interface import LoggerInterface
 
@@ -81,15 +81,15 @@
     "type": "composite",
     "message": "hello world"
 }
 
 compositLogger = CompositeLogger(
     config={
         "defaults": {
-            "datetime": datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+            "datetime": lambda: datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
             "program": "scratch-pad-python",
         },
         "loggerFilterPairs": [
             {
                 "logger": consoleLogger,
                 "filter": None
             },
@@ -144,14 +144,26 @@
         "type": "fluent",
         "message": "hello world"
     }
 
 logger.info(message)
 ```
 
+SlackLogger
+```
+url = "url"
+logger = SlackLogger(url=url)
+message = {
+    "type": "slack",
+    "message": "hello world"
+}
+
+logger.info(message)
+```
+
 #
 stuff) 
 
 
 scribe-docker for ScribeLogger : https://hub.docker.com/r/polonaiz/facebook-scribe
```

### Comparing `scratchpad-py-0.0.5/scratchpad/__init__.py` & `scratchpad-py-0.0.6/scratchpad/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from .logger_impl import LoggerImpl
 from .logger_interface import LoggerInterface
 from .logger import Logger
 from .memory_logger import MemoryLogger
 from .null_logger import NullLogger
 from .scribe_logger import ScribeLogger
 from .telegram_logger import TelegramLogger
+from .slack_logger import SlackLogger
 from .retry import Retry
 
 __all__ = [
     'CompositeLogger',
     'ConsoleLogger',
     'FileLogger',
     'FluentLogger',
@@ -26,9 +27,10 @@
     'LoggerImpl',
     'LoggerInterface',
     'Logger',
     'MemoryLogger',
     'NullLogger',
     'ScribeLogger',
     'TelegramLogger',
+    'SlackLogger',
     'Retry',
 ]
```

### Comparing `scratchpad-py-0.0.5/scratchpad/composite_logger.py` & `scratchpad-py-0.0.6/scratchpad/composite_logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.5/scratchpad/console_logger.py` & `scratchpad-py-0.0.6/scratchpad/console_logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.5/scratchpad/file_logger.py` & `scratchpad-py-0.0.6/scratchpad/file_logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.5/scratchpad/fluent_logger.py` & `scratchpad-py-0.0.6/scratchpad/fluent_logger.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,12 +47,12 @@
             raise e
 
 
 if __name__ == "__main__":
     logger = FluentLogger()
 
     message = {
-            "type": "fluent",
-            "message": "hello world"
-        }
+        "type": "fluent",
+        "message": "hello world"
+    }
 
     logger.log(message)
```

### Comparing `scratchpad-py-0.0.5/scratchpad/jandi_logger.py` & `scratchpad-py-0.0.6/scratchpad/jandi_logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.5/scratchpad/line_logger.py` & `scratchpad-py-0.0.6/scratchpad/line_logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.5/scratchpad/logger.py` & `scratchpad-py-0.0.6/scratchpad/logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.5/scratchpad/logger_impl.py` & `scratchpad-py-0.0.6/scratchpad/logger_impl.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.5/scratchpad/logger_interface.py` & `scratchpad-py-0.0.6/scratchpad/logger_interface.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.5/scratchpad/scribe_logger.py` & `scratchpad-py-0.0.6/scratchpad/scribe_logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.5/scratchpad/telegram_logger.py` & `scratchpad-py-0.0.6/scratchpad/telegram_logger.py`

 * *Files identical despite different names*

### Comparing `scratchpad-py-0.0.5/scratchpad_py.egg-info/PKG-INFO` & `scratchpad-py-0.0.6/scratchpad_py.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scratchpad-py
-Version: 0.0.5
+Version: 0.0.6
 Summary: python logger libary
 Home-page: https://github.com/chirichidi/scratch-pad-py
 Author: chirichidi
 Author-email: tolessnoise@gmail.com
 Keywords: logger
 Classifier: Programming Language :: Python :: 3.7
 Classifier: License :: OSI Approved :: MIT License
@@ -20,15 +20,15 @@
 
 
 mind blowing python toolset. why not pr?
 
 
 # Spec
 
-Loggers: composite, console, file, fluent, jandi, line, memory, null, scribe, telegram
+Loggers: composite, console, file, fluent, jandi, line, memory, null, scribe, telegram, slack
 
 
 
 # Logger interface
 ```
 from .logger_interface import LoggerInterface
 
@@ -96,15 +96,15 @@
     "type": "composite",
     "message": "hello world"
 }
 
 compositLogger = CompositeLogger(
     config={
         "defaults": {
-            "datetime": datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
+            "datetime": lambda: datetime.now().strftime("%Y-%m-%d %H:%M:%S"),
             "program": "scratch-pad-python",
         },
         "loggerFilterPairs": [
             {
                 "logger": consoleLogger,
                 "filter": None
             },
@@ -159,14 +159,26 @@
         "type": "fluent",
         "message": "hello world"
     }
 
 logger.info(message)
 ```
 
+SlackLogger
+```
+url = "url"
+logger = SlackLogger(url=url)
+message = {
+    "type": "slack",
+    "message": "hello world"
+}
+
+logger.info(message)
+```
+
 #
 stuff) 
 
 
 scribe-docker for ScribeLogger : https://hub.docker.com/r/polonaiz/facebook-scribe
```

### Comparing `scratchpad-py-0.0.5/scratchpad_py.egg-info/SOURCES.txt` & `scratchpad-py-0.0.6/scratchpad_py.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,13 +11,14 @@
 scratchpad/logger.py
 scratchpad/logger_impl.py
 scratchpad/logger_interface.py
 scratchpad/memory_logger.py
 scratchpad/null_logger.py
 scratchpad/retry.py
 scratchpad/scribe_logger.py
+scratchpad/slack_logger.py
 scratchpad/telegram_logger.py
 scratchpad_py.egg-info/PKG-INFO
 scratchpad_py.egg-info/SOURCES.txt
 scratchpad_py.egg-info/dependency_links.txt
 scratchpad_py.egg-info/requires.txt
 scratchpad_py.egg-info/top_level.txt
```

### Comparing `scratchpad-py-0.0.5/setup.py` & `scratchpad-py-0.0.6/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_descriprion = f.read()
 
 setuptools.setup(
     name             = 'scratchpad-py',
-    version          = '0.0.5',
+    version          = '0.0.6',
     description      = 'python logger libary',
     long_description = long_descriprion,
     long_description_content_type = "text/markdown",
     author           = 'chirichidi',
     author_email     = 'tolessnoise@gmail.com',
     url              = "https://github.com/chirichidi/scratch-pad-py",
     packages         = ["scratchpad"],
```

