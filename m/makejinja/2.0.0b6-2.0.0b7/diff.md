# Comparing `tmp/makejinja-2.0.0b6.tar.gz` & `tmp/makejinja-2.0.0b7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "makejinja-2.0.0b6.tar", max compression
+gzip compressed data, was "makejinja-2.0.0b7.tar", max compression
```

## Comparing `makejinja-2.0.0b6.tar` & `makejinja-2.0.0b7.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1067 2023-06-01 20:26:53.944036 makejinja-2.0.0b6/LICENSE
--rw-r--r--   0        0        0    16708 2023-06-01 20:26:53.944036 makejinja-2.0.0b6/README.md
--rw-r--r--   0        0        0      101 2023-06-01 20:26:53.944036 makejinja-2.0.0b6/makejinja/__init__.py
--rw-r--r--   0        0        0       48 2023-06-01 20:26:53.944036 makejinja-2.0.0b6/makejinja/__main__.py
--rw-r--r--   0        0        0     6785 2023-06-01 20:26:53.944036 makejinja-2.0.0b6/makejinja/app.py
--rw-r--r--   0        0        0     1211 2023-06-01 20:26:53.944036 makejinja-2.0.0b6/makejinja/cli.py
--rw-r--r--   0        0        0    12243 2023-06-01 20:26:53.944036 makejinja-2.0.0b6/makejinja/config.py
--rw-r--r--   0        0        0     1060 2023-06-01 20:26:53.944036 makejinja-2.0.0b6/makejinja/loader.py
--rw-r--r--   0        0        0        0 2023-06-01 20:26:53.944036 makejinja-2.0.0b6/makejinja/py.typed
--rw-r--r--   0        0        0      813 2023-06-01 20:28:38.236003 makejinja-2.0.0b6/pyproject.toml
--rw-r--r--   0        0        0    17570 1970-01-01 00:00:00.000000 makejinja-2.0.0b6/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/LICENSE
+-rw-r--r--   0        0        0    16708 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/README.md
+-rw-r--r--   0        0        0      101 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/makejinja/__init__.py
+-rw-r--r--   0        0        0       48 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/makejinja/__main__.py
+-rw-r--r--   0        0        0     6785 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/makejinja/app.py
+-rw-r--r--   0        0        0     1211 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/makejinja/cli.py
+-rw-r--r--   0        0        0    12243 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/makejinja/config.py
+-rw-r--r--   0        0        0     1060 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/makejinja/loader.py
+-rw-r--r--   0        0        0        0 2023-06-13 08:11:33.805403 makejinja-2.0.0b7/makejinja/py.typed
+-rw-r--r--   0        0        0      813 2023-06-13 08:12:52.049161 makejinja-2.0.0b7/pyproject.toml
+-rw-r--r--   0        0        0    17570 1970-01-01 00:00:00.000000 makejinja-2.0.0b7/PKG-INFO
```

### Comparing `makejinja-2.0.0b6/LICENSE` & `makejinja-2.0.0b7/LICENSE`

 * *Files identical despite different names*

### Comparing `makejinja-2.0.0b6/README.md` & `makejinja-2.0.0b7/README.md`

 * *Files identical despite different names*

### Comparing `makejinja-2.0.0b6/makejinja/app.py` & `makejinja-2.0.0b7/makejinja/app.py`

 * *Files identical despite different names*

### Comparing `makejinja-2.0.0b6/makejinja/cli.py` & `makejinja-2.0.0b7/makejinja/cli.py`

 * *Files identical despite different names*

### Comparing `makejinja-2.0.0b6/makejinja/config.py` & `makejinja-2.0.0b7/makejinja/config.py`

 * *Files identical despite different names*

### Comparing `makejinja-2.0.0b6/makejinja/loader.py` & `makejinja-2.0.0b7/makejinja/loader.py`

 * *Files identical despite different names*

### Comparing `makejinja-2.0.0b6/pyproject.toml` & `makejinja-2.0.0b7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "makejinja"
-version = "2.0.0b6"
+version = "2.0.0b7"
 description = "Automatically generate files based on Jinja templates. Use it to easily generate complex Home Assistant dashboards!"
 authors = ["Mirko Lenz <mirko@mirkolenz.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/mirkolenz/makejinja"
 
 [tool.poetry.scripts]
@@ -15,15 +15,15 @@
 jinja2 = "^3.1.2"
 pyyaml = "^6.0"
 rich-click = "^1.6.1"
 typed-settings = "^23.0.1"
 tomli = { version = "^2.0.1", python = "<3.11" }
 
 [tool.poetry.group.dev.dependencies]
-pytest = "^7.3.1"
+pytest = "^7.3.2"
 pytest-cov = "^4.1.0"
 
 [tool.pytest.ini_options]
 addopts = "--cov makejinja --cov-report term-missing -vv"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `makejinja-2.0.0b6/PKG-INFO` & `makejinja-2.0.0b7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: makejinja
-Version: 2.0.0b6
+Version: 2.0.0b7
 Summary: Automatically generate files based on Jinja templates. Use it to easily generate complex Home Assistant dashboards!
 Home-page: https://github.com/mirkolenz/makejinja
 License: MIT
 Author: Mirko Lenz
 Author-email: mirko@mirkolenz.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

