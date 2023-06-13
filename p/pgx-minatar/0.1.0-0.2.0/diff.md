# Comparing `tmp/pgx-minatar-0.1.0.tar.gz` & `tmp/pgx-minatar-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pgx-minatar-0.1.0.tar", last modified: Tue Jun 13 08:28:12 2023, max compression
+gzip compressed data, was "pgx-minatar-0.2.0.tar", last modified: Tue Jun 13 08:45:32 2023, max compression
```

## Comparing `pgx-minatar-0.1.0.tar` & `pgx-minatar-0.2.0.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:28:12.257532 pgx-minatar-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-13 08:28:12.257532 pgx-minatar-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:28:12.253532 pgx-minatar-0.1.0/pgx_minatar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/pgx_minatar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/pgx_minatar/asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/pgx_minatar/breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/pgx_minatar/freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)    25316 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/pgx_minatar/seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/pgx_minatar/space_invaders.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/pgx_minatar/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:28:12.257532 pgx-minatar-0.1.0/pgx_minatar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      448 2023-06-13 08:28:12.000000 pgx-minatar-0.1.0/pgx_minatar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-13 08:28:12.000000 pgx-minatar-0.1.0/pgx_minatar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 08:28:12.000000 pgx-minatar-0.1.0/pgx_minatar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-13 08:28:12.000000 pgx-minatar-0.1.0/pgx_minatar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 08:28:12.000000 pgx-minatar-0.1.0/pgx_minatar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 08:28:12.257532 pgx-minatar-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      885 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:28:12.257532 pgx-minatar-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/tests/test_asterix.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/tests/test_breakout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/tests/test_freeway.py
--rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/tests/test_seaquest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-13 08:28:01.000000 pgx-minatar-0.1.0/tests/test_space_invaders.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:45:32.390928 pgx-minatar-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 08:45:32.390928 pgx-minatar-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:45:32.390928 pgx-minatar-0.2.0/pgx_minatar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/pgx_minatar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12926 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/pgx_minatar/asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9090 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/pgx_minatar/breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8762 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/pgx_minatar/freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25316 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/pgx_minatar/seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10042 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/pgx_minatar/space_invaders.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/pgx_minatar/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:45:32.390928 pgx-minatar-0.2.0/pgx_minatar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 08:45:32.000000 pgx-minatar-0.2.0/pgx_minatar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-06-13 08:45:32.000000 pgx-minatar-0.2.0/pgx_minatar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 08:45:32.000000 pgx-minatar-0.2.0/pgx_minatar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-06-13 08:45:32.000000 pgx-minatar-0.2.0/pgx_minatar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 08:45:32.000000 pgx-minatar-0.2.0/pgx_minatar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 08:45:32.394928 pgx-minatar-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 08:45:32.390928 pgx-minatar-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/tests/test_asterix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/tests/test_breakout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2843 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/tests/test_freeway.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5374 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/tests/test_seaquest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-06-13 08:45:23.000000 pgx-minatar-0.2.0/tests/test_space_invaders.py
```

### Comparing `pgx-minatar-0.1.0/LICENSE` & `pgx-minatar-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.1.0/pgx_minatar/asterix.py` & `pgx-minatar-0.2.0/pgx_minatar/asterix.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,26 +60,26 @@
     def to_svg(
         self,
         *,
         color_theme: Optional[Literal["light", "dark"]] = None,
         scale: Optional[float] = None,
     ) -> str:
         del color_theme, scale
-        from pgx.minatar.utils import visualize_minatar
+        from pgx_minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
     def save_svg(
         self,
         filename,
         *,
         color_theme: Optional[Literal["light", "dark"]] = None,
         scale: Optional[float] = None,
     ) -> None:
-        from pgx.minatar.utils import visualize_minatar
+        from pgx_minatar.utils import visualize_minatar
 
         visualize_minatar(self, filename)
 
 
 class MinAtarAsterix(v1.Env):
     def __init__(
         self,
```

### Comparing `pgx-minatar-0.1.0/pgx_minatar/breakout.py` & `pgx-minatar-0.2.0/pgx_minatar/breakout.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,26 +55,26 @@
     def to_svg(
         self,
         *,
         color_theme: Optional[Literal["light", "dark"]] = None,
         scale: Optional[float] = None,
     ) -> str:
         del color_theme, scale
-        from pgx.minatar.utils import visualize_minatar
+        from pgx_minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
     def save_svg(
         self,
         filename,
         *,
         color_theme: Optional[Literal["light", "dark"]] = None,
         scale: Optional[float] = None,
     ) -> None:
-        from pgx.minatar.utils import visualize_minatar
+        from pgx_minatar.utils import visualize_minatar
 
         visualize_minatar(self, filename)
 
 
 class MinAtarBreakout(v1.Env):
     def __init__(
         self,
```

### Comparing `pgx-minatar-0.1.0/pgx_minatar/freeway.py` & `pgx-minatar-0.2.0/pgx_minatar/freeway.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,26 +49,26 @@
     def to_svg(
         self,
         *,
         color_theme: Optional[Literal["light", "dark"]] = None,
         scale: Optional[float] = None,
     ) -> str:
         del color_theme, scale
-        from pgx.minatar.utils import visualize_minatar
+        from pgx_minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
     def save_svg(
         self,
         filename,
         *,
         color_theme: Optional[Literal["light", "dark"]] = None,
         scale: Optional[float] = None,
     ) -> None:
-        from pgx.minatar.utils import visualize_minatar
+        from pgx_minatar.utils import visualize_minatar
 
         visualize_minatar(self, filename)
 
 
 class MinAtarFreeway(v1.Env):
     def __init__(
         self,
```

### Comparing `pgx-minatar-0.1.0/pgx_minatar/seaquest.py` & `pgx-minatar-0.2.0/pgx_minatar/seaquest.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,26 +72,26 @@
     def to_svg(
         self,
         *,
         color_theme: Optional[Literal["light", "dark"]] = None,
         scale: Optional[float] = None,
     ) -> str:
         del color_theme, scale
-        from pgx.minatar.utils import visualize_minatar
+        from pgx_minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
     def save_svg(
         self,
         filename,
         *,
         color_theme: Optional[Literal["light", "dark"]] = None,
         scale: Optional[float] = None,
     ) -> None:
-        from pgx.minatar.utils import visualize_minatar
+        from pgx_minatar.utils import visualize_minatar
 
         visualize_minatar(self, filename)
 
 
 class MinAtarSeaquest(v1.Env):
     def __init__(
         self,
```

### Comparing `pgx-minatar-0.1.0/pgx_minatar/space_invaders.py` & `pgx-minatar-0.2.0/pgx_minatar/space_invaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -59,26 +59,26 @@
     def to_svg(
         self,
         *,
         color_theme: Optional[Literal["light", "dark"]] = None,
         scale: Optional[float] = None,
     ) -> str:
         del color_theme, scale
-        from pgx.minatar.utils import visualize_minatar
+        from pgx_minatar.utils import visualize_minatar
 
         return visualize_minatar(self)
 
     def save_svg(
         self,
         filename,
         *,
         color_theme: Optional[Literal["light", "dark"]] = None,
         scale: Optional[float] = None,
     ) -> None:
-        from pgx.minatar.utils import visualize_minatar
+        from pgx_minatar.utils import visualize_minatar
 
         visualize_minatar(self, filename)
 
 
 class MinAtarSpaceInvaders(v1.Env):
     def __init__(
         self,
```

### Comparing `pgx-minatar-0.1.0/pgx_minatar/utils.py` & `pgx-minatar-0.2.0/pgx_minatar/utils.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.1.0/setup.py` & `pgx-minatar-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import find_packages, setup
 from pathlib import Path
 
 long_description = (Path(__file__).parent / "README.md").read_text()
 
 setup(
     name="pgx-minatar",
-    version="0.1.0",
-    description="MinAtar extension of Pgx",
+    version="0.2.0",
+    description="MinAtar extension for Pgx",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/sotetsuk/pgx-minatar",
     author="Sotetsu KOYAMADA",
     author_email="sotetsu.koyamada@gmail.com",
     keywords="",
     packages=find_packages(),
```

### Comparing `pgx-minatar-0.1.0/tests/test_asterix.py` & `pgx-minatar-0.2.0/tests/test_asterix.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.1.0/tests/test_breakout.py` & `pgx-minatar-0.2.0/tests/test_breakout.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.1.0/tests/test_freeway.py` & `pgx-minatar-0.2.0/tests/test_freeway.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.1.0/tests/test_seaquest.py` & `pgx-minatar-0.2.0/tests/test_seaquest.py`

 * *Files identical despite different names*

### Comparing `pgx-minatar-0.1.0/tests/test_space_invaders.py` & `pgx-minatar-0.2.0/tests/test_space_invaders.py`

 * *Files identical despite different names*

