# Comparing `tmp/superinvoke-1.0.4.tar.gz` & `tmp/superinvoke-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "superinvoke-1.0.4.tar", max compression
+gzip compressed data, was "superinvoke-1.0.5.tar", max compression
```

## Comparing `superinvoke-1.0.4.tar` & `superinvoke-1.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1061 2021-11-05 22:01:21.839383 superinvoke-1.0.4/LICENSE
--rw-r--r--   0        0        0       75 2021-11-05 22:01:43.303591 superinvoke-1.0.4/README.md
--rw-r--r--   0        0        0     2564 2023-06-13 17:19:33.806910 superinvoke-1.0.4/pyproject.toml
--rw-r--r--   0        0        0      331 2023-06-13 17:19:27.754831 superinvoke-1.0.4/superinvoke/__init__.py
--rw-r--r--   0        0        0       30 2022-04-06 17:00:43.796843 superinvoke-1.0.4/superinvoke/collections/__init__.py
--rw-r--r--   0        0        0     1488 2022-08-24 22:29:27.352392 superinvoke-1.0.4/superinvoke/collections/env.py
--rw-r--r--   0        0        0      413 2023-06-12 11:40:33.828956 superinvoke-1.0.4/superinvoke/collections/misc.py
--rw-r--r--   0        0        0     7087 2023-06-11 16:54:26.768939 superinvoke-1.0.4/superinvoke/collections/tool.py
--rw-r--r--   0        0        0      699 2023-02-10 15:52:26.982795 superinvoke-1.0.4/superinvoke/constants.py
--rw-r--r--   0        0        0       40 2022-04-06 21:27:18.109926 superinvoke-1.0.4/superinvoke/extensions/__init__.py
--rw-r--r--   0        0        0       44 2023-05-19 11:24:00.575959 superinvoke-1.0.4/superinvoke/extensions/collection.py
--rw-r--r--   0        0        0     6322 2023-06-13 17:10:28.315796 superinvoke-1.0.4/superinvoke/extensions/context.py
--rw-r--r--   0        0        0      944 2021-11-05 17:48:25.409401 superinvoke-1.0.4/superinvoke/extensions/task.py
--rw-r--r--   0        0        0     1264 2023-06-12 11:29:55.724880 superinvoke-1.0.4/superinvoke/main.py
--rw-r--r--   0        0        0       82 2022-04-06 16:46:10.227621 superinvoke-1.0.4/superinvoke/objects/__init__.py
--rw-r--r--   0        0        0      731 2022-08-24 23:38:36.765460 superinvoke-1.0.4/superinvoke/objects/common.py
--rw-r--r--   0        0        0     1676 2023-05-19 11:21:45.118391 superinvoke-1.0.4/superinvoke/objects/env.py
--rw-r--r--   0        0        0     1819 2023-02-10 15:57:47.706638 superinvoke-1.0.4/superinvoke/objects/tool.py
--rw-r--r--   0        0        0     3251 2023-06-13 17:24:15.926588 superinvoke-1.0.4/superinvoke/utils.py
--rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 superinvoke-1.0.4/setup.py
--rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 superinvoke-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1061 2021-11-05 22:01:21.839383 superinvoke-1.0.5/LICENSE
+-rw-r--r--   0        0        0       75 2021-11-05 22:01:43.303591 superinvoke-1.0.5/README.md
+-rw-r--r--   0        0        0     2564 2023-06-13 19:28:32.258267 superinvoke-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0      331 2023-06-13 19:28:38.538330 superinvoke-1.0.5/superinvoke/__init__.py
+-rw-r--r--   0        0        0       30 2022-04-06 17:00:43.796843 superinvoke-1.0.5/superinvoke/collections/__init__.py
+-rw-r--r--   0        0        0     1488 2022-08-24 22:29:27.352392 superinvoke-1.0.5/superinvoke/collections/env.py
+-rw-r--r--   0        0        0      413 2023-06-12 11:40:33.828956 superinvoke-1.0.5/superinvoke/collections/misc.py
+-rw-r--r--   0        0        0     7087 2023-06-11 16:54:26.768939 superinvoke-1.0.5/superinvoke/collections/tool.py
+-rw-r--r--   0        0        0      699 2023-02-10 15:52:26.982795 superinvoke-1.0.5/superinvoke/constants.py
+-rw-r--r--   0        0        0       40 2022-04-06 21:27:18.109926 superinvoke-1.0.5/superinvoke/extensions/__init__.py
+-rw-r--r--   0        0        0       44 2023-05-19 11:24:00.575959 superinvoke-1.0.5/superinvoke/extensions/collection.py
+-rw-r--r--   0        0        0     6322 2023-06-13 17:10:28.315796 superinvoke-1.0.5/superinvoke/extensions/context.py
+-rw-r--r--   0        0        0      944 2021-11-05 17:48:25.409401 superinvoke-1.0.5/superinvoke/extensions/task.py
+-rw-r--r--   0        0        0     1264 2023-06-12 11:29:55.724880 superinvoke-1.0.5/superinvoke/main.py
+-rw-r--r--   0        0        0       82 2022-04-06 16:46:10.227621 superinvoke-1.0.5/superinvoke/objects/__init__.py
+-rw-r--r--   0        0        0      731 2022-08-24 23:38:36.765460 superinvoke-1.0.5/superinvoke/objects/common.py
+-rw-r--r--   0        0        0     1676 2023-05-19 11:21:45.118391 superinvoke-1.0.5/superinvoke/objects/env.py
+-rw-r--r--   0        0        0     1987 2023-06-13 19:28:07.406020 superinvoke-1.0.5/superinvoke/objects/tool.py
+-rw-r--r--   0        0        0     3251 2023-06-13 17:24:15.926588 superinvoke-1.0.5/superinvoke/utils.py
+-rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 superinvoke-1.0.5/setup.py
+-rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 superinvoke-1.0.5/PKG-INFO
```

### Comparing `superinvoke-1.0.4/LICENSE` & `superinvoke-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.4/pyproject.toml` & `superinvoke-1.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "superinvoke"
-version = "1.0.4"
+version = "1.0.5"
 description = "An Invoke wrapper with extra handy features."
 license = "MIT"
 authors = ["Alex <alex@neoxelox.com>"]
 maintainers = ["Alex <alex@neoxelox.com>"]
 readme = "README.md"
 homepage = "https://github.com/neoxelox/superinvoke"
 repository = "https://github.com/neoxelox/superinvoke"
```

### Comparing `superinvoke-1.0.4/superinvoke/collections/env.py` & `superinvoke-1.0.5/superinvoke/collections/env.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.4/superinvoke/collections/tool.py` & `superinvoke-1.0.5/superinvoke/collections/tool.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.4/superinvoke/constants.py` & `superinvoke-1.0.5/superinvoke/constants.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.4/superinvoke/extensions/context.py` & `superinvoke-1.0.5/superinvoke/extensions/context.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.4/superinvoke/extensions/task.py` & `superinvoke-1.0.5/superinvoke/extensions/task.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.4/superinvoke/main.py` & `superinvoke-1.0.5/superinvoke/main.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.4/superinvoke/objects/common.py` & `superinvoke-1.0.5/superinvoke/objects/common.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.4/superinvoke/objects/env.py` & `superinvoke-1.0.5/superinvoke/objects/env.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.4/superinvoke/objects/tool.py` & `superinvoke-1.0.5/superinvoke/objects/tool.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,14 +26,18 @@
         self.version = version
         self.tags = tags
         self.links = links
         self._managed = True
 
         if path is None:
             self.path = utils.path(f"{constants.Paths.TOOLS}/{self.name}")
+
+            # Windows executables have to end with .exe
+            if constants.Platforms.CURRENT == constants.Platforms.WINDOWS:
+                self.path += ".exe"
         else:
             self.path = str(path)
             self._managed = False
 
     def __str__(self) -> str:
         return self.path
```

### Comparing `superinvoke-1.0.4/superinvoke/utils.py` & `superinvoke-1.0.5/superinvoke/utils.py`

 * *Files identical despite different names*

### Comparing `superinvoke-1.0.4/setup.py` & `superinvoke-1.0.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['download==0.3.5',
  'neoxelox-invoke==2.0.0',
  'rich==12.5.1',
  'semantic-version==2.10.0']
 
 setup_kwargs = {
     'name': 'superinvoke',
-    'version': '1.0.4',
+    'version': '1.0.5',
     'description': 'An Invoke wrapper with extra handy features.',
     'long_description': '# superinvoke\n\nAn Invoke wrapper with extra handy features.\n\nTODO: EXPLAIN\n',
     'author': 'Alex',
     'author_email': 'alex@neoxelox.com',
     'maintainer': 'Alex',
     'maintainer_email': 'alex@neoxelox.com',
     'url': 'https://github.com/neoxelox/superinvoke',
```

### Comparing `superinvoke-1.0.4/PKG-INFO` & `superinvoke-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: superinvoke
-Version: 1.0.4
+Version: 1.0.5
 Summary: An Invoke wrapper with extra handy features.
 Home-page: https://github.com/neoxelox/superinvoke
 License: MIT
 Keywords: plugin,wrapper,invoke,pyinvoke,superinvoke
 Author: Alex
 Author-email: alex@neoxelox.com
 Maintainer: Alex
```

