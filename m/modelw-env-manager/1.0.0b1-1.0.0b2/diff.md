# Comparing `tmp/modelw_env_manager-1.0.0b1.tar.gz` & `tmp/modelw_env_manager-1.0.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelw_env_manager-1.0.0b1.tar", max compression
+gzip compressed data, was "modelw_env_manager-1.0.0b2.tar", max compression
```

## Comparing `modelw_env_manager-1.0.0b1.tar` & `modelw_env_manager-1.0.0b2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0      484 2022-08-29 15:31:59.079500 modelw_env_manager-1.0.0b1/LICENSE
--rw-r--r--   0        0        0      440 2022-12-09 12:34:29.939889 modelw_env_manager-1.0.0b1/README.md
--rw-r--r--   0        0        0     1089 2022-12-09 12:34:29.995890 modelw_env_manager-1.0.0b1/pyproject.toml
--rw-r--r--   0        0        0      100 2022-09-10 15:02:35.429220 modelw_env_manager-1.0.0b1/src/model_w/env_manager/__init__.py
--rw-r--r--   0        0        0     3419 2022-12-09 12:34:29.939889 modelw_env_manager-1.0.0b1/src/model_w/env_manager/_dotenv.py
--rw-r--r--   0        0        0      221 2022-08-29 15:31:59.079500 modelw_env_manager-1.0.0b1/src/model_w/env_manager/_exceptions.py
--rw-r--r--   0        0        0     8439 2022-12-09 12:34:29.939889 modelw_env_manager-1.0.0b1/src/model_w/env_manager/_manager.py
--rw-r--r--   0        0        0     2304 2022-09-09 10:52:17.616896 modelw_env_manager-1.0.0b1/src/model_w/env_manager/_preset.py
--rw-r--r--   0        0        0      646 2022-09-09 10:52:17.616896 modelw_env_manager-1.0.0b1/src/model_w/env_manager/_utils.py
--rw-r--r--   0        0        0        0 2022-09-09 11:00:36.773031 modelw_env_manager-1.0.0b1/src/model_w/env_manager/py.typed
--rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 modelw_env_manager-1.0.0b1/setup.py
--rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 modelw_env_manager-1.0.0b1/PKG-INFO
+-rw-r--r--   0        0        0      484 2022-12-13 11:51:00.259999 modelw_env_manager-1.0.0b2/LICENSE
+-rw-r--r--   0        0        0      440 2022-12-13 11:51:00.259999 modelw_env_manager-1.0.0b2/README.md
+-rw-r--r--   0        0        0     1089 2022-12-13 11:53:32.560010 modelw_env_manager-1.0.0b2/pyproject.toml
+-rw-r--r--   0        0        0      100 2022-12-13 11:51:00.263999 modelw_env_manager-1.0.0b2/src/model_w/env_manager/__init__.py
+-rw-r--r--   0        0        0     3427 2022-12-13 11:51:55.364001 modelw_env_manager-1.0.0b2/src/model_w/env_manager/_dotenv.py
+-rw-r--r--   0        0        0      221 2022-12-13 11:51:00.263999 modelw_env_manager-1.0.0b2/src/model_w/env_manager/_exceptions.py
+-rw-r--r--   0        0        0     8439 2022-12-13 11:51:00.263999 modelw_env_manager-1.0.0b2/src/model_w/env_manager/_manager.py
+-rw-r--r--   0        0        0     2304 2022-12-13 11:51:00.263999 modelw_env_manager-1.0.0b2/src/model_w/env_manager/_preset.py
+-rw-r--r--   0        0        0      646 2022-12-13 11:51:00.263999 modelw_env_manager-1.0.0b2/src/model_w/env_manager/_utils.py
+-rw-r--r--   0        0        0        0 2022-12-13 11:51:00.263999 modelw_env_manager-1.0.0b2/src/model_w/env_manager/py.typed
+-rw-r--r--   0        0        0     1252 1970-01-01 00:00:00.000000 modelw_env_manager-1.0.0b2/setup.py
+-rw-r--r--   0        0        0     1609 1970-01-01 00:00:00.000000 modelw_env_manager-1.0.0b2/PKG-INFO
```

### Comparing `modelw_env_manager-1.0.0b1/pyproject.toml` & `modelw_env_manager-1.0.0b2/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "modelw-env-manager"
-version = "1.0.0b1"
+version = "1.0.0b2"
 packages = [
     {  include = "model_w/env_manager", from = "src" }
 ]
 
 description = "A tool to simplify reading environment variables and .env files"
 authors = ["Rémy Sanchez <remy.sanchez@hyperthese.net>"]
 license = "WTFPL"
```

### Comparing `modelw_env_manager-1.0.0b1/src/model_w/env_manager/_dotenv.py` & `modelw_env_manager-1.0.0b2/src/model_w/env_manager/_dotenv.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     file_name
         Name of the `.env` file you're looking for. Defaults to `.env` but can
         be anything.
     """
 
     prefixes = [Path(sys.prefix).absolute()]
 
-    if py_path := os.getenv("PYTHONPATH"):
+    if py_path := os.getenv("DOTENV_IGNORE_PATH"):
         prefixes.extend(Path(p).absolute() for p in py_path.split(os.pathsep))
 
     candidates = set()
 
     for frame in inspect.stack(0):
         file = Path(frame.filename).absolute()
```

### Comparing `modelw_env_manager-1.0.0b1/src/model_w/env_manager/_manager.py` & `modelw_env_manager-1.0.0b2/src/model_w/env_manager/_manager.py`

 * *Files identical despite different names*

### Comparing `modelw_env_manager-1.0.0b1/src/model_w/env_manager/_preset.py` & `modelw_env_manager-1.0.0b2/src/model_w/env_manager/_preset.py`

 * *Files identical despite different names*

### Comparing `modelw_env_manager-1.0.0b1/src/model_w/env_manager/_utils.py` & `modelw_env_manager-1.0.0b2/src/model_w/env_manager/_utils.py`

 * *Files identical despite different names*

### Comparing `modelw_env_manager-1.0.0b1/setup.py` & `modelw_env_manager-1.0.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 {'': ['*']}
 
 install_requires = \
 ['PyYAML>=6.0', 'python-dotenv>=0.11.0,<1.0']
 
 setup_kwargs = {
     'name': 'modelw-env-manager',
-    'version': '1.0.0b1',
+    'version': '1.0.0b2',
     'description': 'A tool to simplify reading environment variables and .env files',
     'long_description': "# Model W &mdash; Env Manager\n\nThe goal of the env manager is to help managing the loading of environment\nvariables and Django settings (although this is not Django-dependent).\n\nTypical use is:\n\n```python\nfrom model_w.env_manager import EnvManager\n\n\nwith EnvManager() as env:\n    SOME_VALUE = env.get('SOME_VALUE', is_yaml=True, default=False)\n```\n\n## Documentation\n\n[✨ **Documentation is there** ✨](http://modelw-env-manager.rtfd.io/)\n",
     'author': 'Rémy Sanchez',
     'author_email': 'remy.sanchez@hyperthese.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/ModelW/py-env-manager',
```

### Comparing `modelw_env_manager-1.0.0b1/PKG-INFO` & `modelw_env_manager-1.0.0b2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelw-env-manager
-Version: 1.0.0b1
+Version: 1.0.0b2
 Summary: A tool to simplify reading environment variables and .env files
 Home-page: https://github.com/ModelW/py-env-manager
 License: WTFPL
 Keywords: django,env,configuration
 Author: Rémy Sanchez
 Author-email: remy.sanchez@hyperthese.net
 Requires-Python: >=3.8,<4.0
```

