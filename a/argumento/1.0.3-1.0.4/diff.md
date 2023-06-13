# Comparing `tmp/argumento-1.0.3.tar.gz` & `tmp/argumento-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\PyProjects\OK\config-args\dist\.tmp-6ci6_4xi\argumento-1.0.3.tar", last modified: Wed Jun  7 09:07:46 2023, max compression
+gzip compressed data, was "D:\PyProjects\OK\config-args\dist\.tmp-i0s5itj7\argumento-1.0.4.tar", last modified: Tue Jun 13 18:25:38 2023, max compression
```

## Comparing `argumento-1.0.3.tar` & `argumento-1.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-06-07 09:07:46.000000 argumento-1.0.3/
--rw-rw-rw-   0        0        0    35823 2023-05-04 00:20:50.000000 argumento-1.0.3/LICENSE
--rw-rw-rw-   0        0        0     1438 2023-06-07 09:07:46.000000 argumento-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      961 2023-06-07 09:04:28.000000 argumento-1.0.3/README.md
--rw-rw-rw-   0        0        0      813 2023-06-07 09:07:20.000000 argumento-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-06-07 09:07:46.000000 argumento-1.0.3/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-06-07 09:07:46.000000 argumento-1.0.3/src/
-drwxrwxrwx   0        0        0        0 2023-06-07 09:07:46.000000 argumento-1.0.3/src/argumento/
--rw-rw-rw-   0        0        0       84 2023-06-06 18:28:39.000000 argumento-1.0.3/src/argumento/__init__.py
--rw-rw-rw-   0        0        0       23 2023-06-07 09:04:28.000000 argumento-1.0.3/src/argumento/_version.py
--rw-rw-rw-   0        0        0     4809 2023-06-06 18:33:43.000000 argumento-1.0.3/src/argumento/parsers.py
-drwxrwxrwx   0        0        0        0 2023-06-07 09:07:46.000000 argumento-1.0.3/src/argumento.egg-info/
--rw-rw-rw-   0        0        0     1438 2023-06-07 09:07:46.000000 argumento-1.0.3/src/argumento.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      293 2023-06-07 09:07:46.000000 argumento-1.0.3/src/argumento.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-07 09:07:46.000000 argumento-1.0.3/src/argumento.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       23 2023-06-07 09:07:46.000000 argumento-1.0.3/src/argumento.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-06-07 09:07:46.000000 argumento-1.0.3/src/argumento.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 18:25:38.000000 argumento-1.0.4/
+-rw-rw-rw-   0        0        0    35823 2023-05-04 00:20:50.000000 argumento-1.0.4/LICENSE
+-rw-rw-rw-   0        0        0     1438 2023-06-13 18:25:38.000000 argumento-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      961 2023-06-07 09:04:28.000000 argumento-1.0.4/README.md
+-rw-rw-rw-   0        0        0      813 2023-06-07 09:07:20.000000 argumento-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-06-13 18:25:38.000000 argumento-1.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-06-13 18:25:38.000000 argumento-1.0.4/src/
+drwxrwxrwx   0        0        0        0 2023-06-13 18:25:38.000000 argumento-1.0.4/src/argumento/
+-rw-rw-rw-   0        0        0       84 2023-06-06 18:28:39.000000 argumento-1.0.4/src/argumento/__init__.py
+-rw-rw-rw-   0        0        0       23 2023-06-13 18:23:59.000000 argumento-1.0.4/src/argumento/_version.py
+-rw-rw-rw-   0        0        0     4860 2023-06-13 18:23:40.000000 argumento-1.0.4/src/argumento/parsers.py
+drwxrwxrwx   0        0        0        0 2023-06-13 18:25:38.000000 argumento-1.0.4/src/argumento.egg-info/
+-rw-rw-rw-   0        0        0     1438 2023-06-13 18:25:38.000000 argumento-1.0.4/src/argumento.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      293 2023-06-13 18:25:38.000000 argumento-1.0.4/src/argumento.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 18:25:38.000000 argumento-1.0.4/src/argumento.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       23 2023-06-13 18:25:38.000000 argumento-1.0.4/src/argumento.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-06-13 18:25:38.000000 argumento-1.0.4/src/argumento.egg-info/top_level.txt
```

### Comparing `argumento-1.0.3/LICENSE` & `argumento-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `argumento-1.0.3/PKG-INFO` & `argumento-1.0.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argumento
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package for combining config and command-line args
 Author-email: OK111 <oleg.khadartsev@gmail.com>
 Project-URL: Homepage, https://github.com/OlegKhadartsev/config-args
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `argumento-1.0.3/README.md` & `argumento-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `argumento-1.0.3/pyproject.toml` & `argumento-1.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `argumento-1.0.3/src/argumento/parsers.py` & `argumento-1.0.4/src/argumento/parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,33 +62,33 @@
 
 
 class ParserToml(ParserBase):
     def __init__(self, config_file: str):
         super().__init__(config_file)
 
     def _read_config(self) -> dict:
-        with open(self._config_file, "r") as f:
+        with open(self._config_file, 'r', encoding='utf8') as f:
             return toml.load(f)
 
 
 class ParserYaml(ParserBase):
     def __init__(self, config_file: str):
         super().__init__(config_file)
 
     def _read_config(self) -> dict:
-        with open(self._config_file, "r") as f:
+        with open(self._config_file, 'r', encoding='utf8') as f:
             return yaml.safe_load(f)
 
 
 class ParserJson(ParserBase):
     def __init__(self, config_file: str):
         super().__init__(config_file)
 
     def _read_config(self) -> dict:
-        with open(self._config_file, "r") as f:
+        with open(self._config_file, 'r', encoding='utf8') as f:
             return json.loads(f.read(), encoding='utf8')
 
 
 class ParserFactory:
     def __init__(self):
         self._parsers = {}
```

### Comparing `argumento-1.0.3/src/argumento.egg-info/PKG-INFO` & `argumento-1.0.4/src/argumento.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: argumento
-Version: 1.0.3
+Version: 1.0.4
 Summary: Package for combining config and command-line args
 Author-email: OK111 <oleg.khadartsev@gmail.com>
 Project-URL: Homepage, https://github.com/OlegKhadartsev/config-args
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

