# Comparing `tmp/pyramid_route_7-0.3.1.tar.gz` & `tmp/pyramid_route_7-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyramid_route_7-0.3.1.tar", last modified: Thu Mar 25 20:48:26 2021, max compression
+gzip compressed data, was "pyramid_route_7-0.4.0.tar", last modified: Tue Jun 13 18:54:36 2023, max compression
```

## Comparing `pyramid_route_7-0.3.1.tar` & `pyramid_route_7-0.4.0.tar`

### file list

```diff
@@ -1,28 +1,29 @@
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:48:26.000000 pyramid_route_7-0.3.1/
--rw-r--r--   0 jvanasco   (501) admin       (80)      332 2021-03-25 20:45:45.000000 pyramid_route_7-0.3.1/CHANGES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)     1082 2020-10-19 19:53:49.000000 pyramid_route_7-0.3.1/EXAMPLE.md
--rw-r--r--   0 jvanasco   (501) admin       (80)     1148 2015-06-05 23:51:31.000000 pyramid_route_7-0.3.1/LICENSE.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      203 2021-03-25 20:44:11.000000 pyramid_route_7-0.3.1/MANIFEST.in
--rw-r--r--   0 jvanasco   (501) admin       (80)     7018 2021-03-25 20:48:26.000000 pyramid_route_7-0.3.1/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       48 2020-10-15 03:26:28.000000 pyramid_route_7-0.3.1/pyproject.toml
--rw-r--r--   0 jvanasco   (501) admin       (80)     5073 2020-10-19 20:29:20.000000 pyramid_route_7-0.3.1/README.rst
--rw-r--r--   0 jvanasco   (501) admin       (80)       69 2021-03-25 20:48:26.000000 pyramid_route_7-0.3.1/setup.cfg
--rw-r--r--   0 jvanasco   (501) admin       (80)     1514 2021-03-25 20:47:23.000000 pyramid_route_7-0.3.1/setup.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:48:26.000000 pyramid_route_7-0.3.1/src/
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:48:26.000000 pyramid_route_7-0.3.1/src/pyramid_route_7/
--rw-r--r--   0 jvanasco   (501) admin       (80)     4965 2021-03-25 20:45:18.000000 pyramid_route_7-0.3.1/src/pyramid_route_7/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:48:26.000000 pyramid_route_7-0.3.1/src/pyramid_route_7.egg-info/
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 20:48:25.000000 pyramid_route_7-0.3.1/src/pyramid_route_7.egg-info/dependency_links.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 20:48:07.000000 pyramid_route_7-0.3.1/src/pyramid_route_7.egg-info/not-zip-safe
--rw-r--r--   0 jvanasco   (501) admin       (80)     7018 2021-03-25 20:48:25.000000 pyramid_route_7-0.3.1/src/pyramid_route_7.egg-info/PKG-INFO
--rw-r--r--   0 jvanasco   (501) admin       (80)       34 2021-03-25 20:48:25.000000 pyramid_route_7-0.3.1/src/pyramid_route_7.egg-info/requires.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)      497 2021-03-25 20:48:25.000000 pyramid_route_7-0.3.1/src/pyramid_route_7.egg-info/SOURCES.txt
--rw-r--r--   0 jvanasco   (501) admin       (80)       16 2021-03-25 20:48:25.000000 pyramid_route_7-0.3.1/src/pyramid_route_7.egg-info/top_level.txt
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:48:26.000000 pyramid_route_7-0.3.1/tests/
--rw-r--r--   0 jvanasco   (501) admin       (80)        0 2020-10-19 19:35:32.000000 pyramid_route_7-0.3.1/tests/__init__.py
-drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2021-03-25 20:48:26.000000 pyramid_route_7-0.3.1/tests/r7testapp/
--rw-r--r--   0 jvanasco   (501) admin       (80)     1122 2020-10-19 20:13:07.000000 pyramid_route_7-0.3.1/tests/r7testapp/__init__.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      481 2020-10-19 19:39:44.000000 pyramid_route_7-0.3.1/tests/r7testapp/views.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     3019 2020-10-19 20:30:53.000000 pyramid_route_7-0.3.1/tests/test_app.py
--rw-r--r--   0 jvanasco   (501) admin       (80)     3375 2020-10-19 20:32:13.000000 pyramid_route_7-0.3.1/tests/test_config.py
--rw-r--r--   0 jvanasco   (501) admin       (80)      137 2020-10-15 19:02:48.000000 pyramid_route_7-0.3.1/tox.ini
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 18:54:36.543269 pyramid_route_7-0.4.0/
+-rw-r--r--   0 jvanasco   (501) admin       (80)      390 2023-06-13 18:46:04.000000 pyramid_route_7-0.4.0/CHANGES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1082 2020-10-19 19:53:49.000000 pyramid_route_7-0.4.0/EXAMPLE.md
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1148 2015-06-05 23:51:31.000000 pyramid_route_7-0.4.0/LICENSE.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)      203 2021-03-25 20:44:11.000000 pyramid_route_7-0.4.0/MANIFEST.in
+-rw-r--r--   0 jvanasco   (501) admin       (80)     5883 2023-06-13 18:54:36.543602 pyramid_route_7-0.4.0/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)     5073 2020-10-19 20:29:20.000000 pyramid_route_7-0.4.0/README.rst
+-rw-r--r--   0 jvanasco   (501) admin       (80)       40 2023-06-13 18:46:04.000000 pyramid_route_7-0.4.0/pyproject.toml
+-rw-r--r--   0 jvanasco   (501) admin       (80)      211 2023-06-13 18:54:36.545166 pyramid_route_7-0.4.0/setup.cfg
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1827 2023-06-13 18:46:04.000000 pyramid_route_7-0.4.0/setup.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 18:54:36.504529 pyramid_route_7-0.4.0/src/
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 18:54:36.523409 pyramid_route_7-0.4.0/src/pyramid_route_7/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     6204 2023-06-13 18:46:04.000000 pyramid_route_7-0.4.0/src/pyramid_route_7/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2023-06-13 18:54:31.000000 pyramid_route_7-0.4.0/src/pyramid_route_7/py.typed
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 18:54:36.533218 pyramid_route_7-0.4.0/src/pyramid_route_7.egg-info/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     5883 2023-06-13 18:54:36.000000 pyramid_route_7-0.4.0/src/pyramid_route_7.egg-info/PKG-INFO
+-rw-r--r--   0 jvanasco   (501) admin       (80)      526 2023-06-13 18:54:36.000000 pyramid_route_7-0.4.0/src/pyramid_route_7.egg-info/SOURCES.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2023-06-13 18:54:36.000000 pyramid_route_7-0.4.0/src/pyramid_route_7.egg-info/dependency_links.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)        1 2021-03-25 20:48:07.000000 pyramid_route_7-0.4.0/src/pyramid_route_7.egg-info/not-zip-safe
+-rw-r--r--   0 jvanasco   (501) admin       (80)       39 2023-06-13 18:54:36.000000 pyramid_route_7-0.4.0/src/pyramid_route_7.egg-info/requires.txt
+-rw-r--r--   0 jvanasco   (501) admin       (80)       16 2023-06-13 18:54:36.000000 pyramid_route_7-0.4.0/src/pyramid_route_7.egg-info/top_level.txt
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 18:54:36.536688 pyramid_route_7-0.4.0/tests/
+-rw-r--r--   0 jvanasco   (501) admin       (80)        0 2020-10-19 19:35:32.000000 pyramid_route_7-0.4.0/tests/__init__.py
+drwxr-xr-x   0 jvanasco   (501) admin       (80)        0 2023-06-13 18:54:36.540323 pyramid_route_7-0.4.0/tests/r7testapp/
+-rw-r--r--   0 jvanasco   (501) admin       (80)     1128 2023-06-13 18:46:04.000000 pyramid_route_7-0.4.0/tests/r7testapp/__init__.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      481 2020-10-19 19:39:44.000000 pyramid_route_7-0.4.0/tests/r7testapp/views.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3028 2023-06-13 18:46:04.000000 pyramid_route_7-0.4.0/tests/test_app.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)     3346 2023-06-13 18:46:04.000000 pyramid_route_7-0.4.0/tests/test_config.py
+-rw-r--r--   0 jvanasco   (501) admin       (80)      149 2023-06-13 18:46:04.000000 pyramid_route_7-0.4.0/tox.ini
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyramid_route_7-0.3.1/EXAMPLE.md` & `pyramid_route_7-0.4.0/EXAMPLE.md`

 * *Files identical despite different names*

### Comparing `pyramid_route_7-0.3.1/LICENSE.txt` & `pyramid_route_7-0.4.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyramid_route_7-0.3.1/README.rst` & `pyramid_route_7-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `pyramid_route_7-0.3.1/setup.py` & `pyramid_route_7-0.4.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 with open(os.path.join(HERE, "src", "pyramid_route_7", "__init__.py")) as v_file:
     VERSION = re.compile(r'.*__VERSION__ = "(.*?)"', re.S).match(v_file.read()).group(1)
 
 requires = [
     "pyramid",
 ]
 tests_require = [
+    "mypy",
     "pytest",
     "webtest",
 ]
 testing_extras = tests_require + []
 
 setup(
     name="pyramid_route_7",
@@ -34,22 +35,28 @@
     description=description,
     long_description=long_description,
     keywords="web pyramid routing routes",
     license="MIT",
     classifiers=[
         "Intended Audience :: Developers",
         "Framework :: Pyramid",
-        "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: MIT License",
     ],
     packages=find_packages(
         where="src",
     ),
     package_dir={"": "src"},
+    package_data={"pyramid_route_7": ["py.typed"]},
     include_package_data=True,
     zip_safe=False,
     install_requires=requires,
     tests_require=tests_require,
     extras_require={
         "testing": testing_extras,
     },
```

### Comparing `pyramid_route_7-0.3.1/src/pyramid_route_7/__init__.py` & `pyramid_route_7-0.4.0/src/pyramid_route_7/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,51 @@
+# stdlib
 import logging
-
-log = logging.getLogger(__name__)
-
-from pyramid.exceptions import ConfigurationError
-
 import re
+from typing import Optional
+from typing import TYPE_CHECKING
 
-__VERSION__ = "0.3.1"
+# pypi
+from pyramid.exceptions import ConfigurationError  # type: ignore[import]
 
+# typing
+if TYPE_CHECKING:
+    from pyramid.config import Configurator  # type: ignore[import]
 
 # ==============================================================================
 
+__VERSION__ = "0.4.0"
+
+# ------------------------------------------------------------------------------
+
+log = logging.getLogger(__name__)
 
 REGEX_route_pattern = re.compile(r"\{(([\w]+)\|([\w]+))\}", re.I)
 REGEX_route_kvpattern = re.compile(r"\{(\@([\w]+))\}", re.I)
 
-
-# ==============================================================================
+# ------------------------------------------------------------------------------
 
 
-def add_route_7_kvpattern(config, pattern_key, pattern_regex):
+def add_route_7_kvpattern(
+    config: "Configurator",
+    pattern_key: str,
+    pattern_regex: str,
+):
     r"""
     registers a kvpattern with the configurator.
     a kvpattern is a shortcut pattern for both keys and values.
 
+    :param config: pyramid config
+    :type config: `pyramid.config.Configurator` instance
+    :param pattern_key: the name of the pattern
+    :type pattern_key: str
+    :param pattern_regex: the pattern in regex notation
+    :type pattern_regex: str
+    :returns: None
+
     it is invoked as such:
 
         config.add_route_7_kvpattern("year", r"\d\d\d\d")
         config.add_route_7_kvpattern("month", r"\d\d")
         config.add_route_7_kvpattern("day", r"\d\d")
         config.add_route("ymd", "/{@year}/{@month}/{@day}")
 
@@ -48,19 +66,32 @@
         config.add_route("user_profile-subfolder2", "/path/to/user/{@user_id}/subfolder-two")
     """
     if pattern_key in config.registry.route_7["kvpattern"]:
         raise ConfigurationError("`pattern_key` exists")
     config.registry.route_7["kvpattern"][pattern_key] = pattern_regex
 
 
-def add_route_7_pattern(config, pattern_name, pattern_regex):
+def add_route_7_pattern(
+    config: "Configurator",
+    pattern_name: str,
+    pattern_regex: str,
+) -> None:
     r"""
     registers a pattern with the configurator.
     a pattern is a shortcut pattern for ONLY the values.
     it must be invoked with a key
+
+    :param config: pyramid config
+    :type config: `pyramid.config.Configurator` instance
+    :param pattern_name: the name of the pattern
+    :type pattern_name: str
+    :param pattern_regex: the pattern in regex notation
+    :type pattern_regex: str
+    :returns: None
+
     it is invoked as such:
 
         config.add_route_7_pattern("d4", r"\d\d\d\d")
         config.add_route_7_pattern("d2", r"\d\d")
         config.add_route("ymd", "/{year|d4}/{month|d2}/{day|d2}")
 
     note that they syntax for expanding a route_pattern is
@@ -70,53 +101,63 @@
         config.add_route("ymd",  r"/{year:\d\d\d\d}/{month:\d\d}/{day:\d\d}")
     """
     if pattern_name in config.registry.route_7["pattern"]:
         raise ConfigurationError("`pattern_name` exists")
     config.registry.route_7["pattern"][pattern_name] = pattern_regex
 
 
-def add_route_7(config, name, pattern=None, **kwargs):
+def add_route_7(
+    config: "Configurator", name: str, pattern: Optional[str] = None, **kwargs
+) -> None:
     """
     Configuration directive that can be used to register a route
     route_7 allows for a microsyntax in the route declarations.
     after the route declarations are expanded, they are passed onto `add_route`
+
+    :param config: pyramid config
+    :type config: `pyramid.config.Configurator` instance
+    :param name: the name of the route
+    :type name: str
+    :param pattern: the pattern in regex notation
+    :type pattern: str
+    :returns: None
     """
     try:
         if pattern:
             _pattern_og = pattern
             _pattern_latest = pattern
 
             # set dedupes
             _route_patterns = set(REGEX_route_pattern.findall(pattern))
             _route_kvpatterns = set(REGEX_route_kvpattern.findall(pattern))
             if _route_patterns or _route_kvpatterns:
                 log.debug("processing %s", pattern)
 
-            for (_macro, _key, _p_name) in _route_patterns:
+            for _macro, _key, _p_name in _route_patterns:
                 if _p_name not in config.registry.route_7["pattern"]:
                     raise ConfigurationError("missing pattern `%s`" % _p_name)
                 _p_value = config.registry.route_7["pattern"][_p_name]
                 _pattern_latest = pattern  # stash for logging
                 pattern = pattern.replace(_macro, "%s:%s" % (_key, _p_value))
                 log.debug("  updating %s > %s", _pattern_latest, pattern)  # updating
 
-            for (_macro, _p_name) in _route_kvpatterns:
+            for _macro, _p_name in _route_kvpatterns:
                 if _p_name not in config.registry.route_7["kvpattern"]:
                     raise ConfigurationError("missing kvpattern `%s`" % _p_name)
                 _p_value = config.registry.route_7["kvpattern"][_p_name]
                 _pattern_latest = pattern  # stash for logging
                 pattern = pattern.replace(_macro, "%s:%s" % (_p_name, _p_value))
                 log.debug("  updating %s > %s", _pattern_latest, pattern)  # updating
 
             if _pattern_og != pattern:
                 log.debug("     final %s > %s", _pattern_og, pattern)  # updating
-    except:
+    except:  # noqa: E722
         raise
     config.add_route(name, pattern=pattern, **kwargs)
 
 
-def includeme(config):
+def includeme(config: "Configurator") -> None:
     """Function that gets called when client code calls config.include"""
     config.add_directive("add_route_7", add_route_7)
     config.add_directive("add_route_7_pattern", add_route_7_pattern)
     config.add_directive("add_route_7_kvpattern", add_route_7_kvpattern)
     config.registry.route_7 = {"pattern": {}, "kvpattern": {}}
```

### Comparing `pyramid_route_7-0.3.1/tests/r7testapp/__init__.py` & `pyramid_route_7-0.4.0/tests/r7testapp/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,23 +4,23 @@
 def main(global_config, **settings):
     """This function returns a Pyramid WSGI application."""
     config = Configurator(settings=settings)
     config.add_static_view("static", "static", cache_max_age=3600)
     config.add_route("home", "/")
 
     config.include("pyramid_route_7")
-    config.add_route_7_pattern("d4", "\d\d\d\d")
-    config.add_route_7_pattern("d2", "\d\d")
-    config.add_route_7_kvpattern("year", "\d\d\d\d")
-    config.add_route_7_kvpattern("month", "\d\d")
-    config.add_route_7_kvpattern("day", "\d\d")
+    config.add_route_7_pattern("d4", r"\d\d\d\d")
+    config.add_route_7_pattern("d2", r"\d\d")
+    config.add_route_7_kvpattern("year", r"\d\d\d\d")
+    config.add_route_7_kvpattern("month", r"\d\d")
+    config.add_route_7_kvpattern("day", r"\d\d")
     config.add_route_7("ymd-kvpattern", "/ymd-kvpattern/{@year}/{@month}/{@day}")
     config.add_route_7("ymd-pattern", "/ymd-pattern/{year|d4}/{month|d2}/{day|d2}")
 
-    config.add_route_7_kvpattern("user_id", "\d\d\d")
+    config.add_route_7_kvpattern("user_id", r"\d\d\d")
     config.add_route_7("user_profile", "/path/to/user/{@user_id}")
     config.add_route_7(
         "user_profile-subfolder1", "/path/to/user/{@user_id}/subfolder-one"
     )
     config.add_route_7(
         "user_profile-subfolder2", "/path/to/user/{@user_id}/subfolder-two"
     )
```

### Comparing `pyramid_route_7-0.3.1/tests/test_app.py` & `pyramid_route_7-0.4.0/tests/test_app.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 """
 IMPORTANT
 
 whitespace in the this file IS SIGNIFICANT AND IMPORTANT.
 the test-cases check for specific whitespace
 """
 
-import pyramid_route_7
-
 # stdblib
 import unittest
 
 # pypi
 from pyramid import testing
 from webtest import TestApp
 
+# local
+# import pyramid_route_7
 
 # ==============================================================================
 
 
 class PyramidTestApp(unittest.TestCase):
     def setUp(self):
         from .r7testapp import main
```

### Comparing `pyramid_route_7-0.3.1/tests/test_config.py` & `pyramid_route_7-0.4.0/tests/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 from __future__ import print_function
 
-import pyramid_route_7
-
 # stdblib
 import unittest
 
 # pypi
 from pyramid import testing
-from pyramid.urldispatch import Route
 from pyramid.interfaces import IRoutesMapper
 
+# local
+# import pyramid_route_7
 
 # ==============================================================================
 
 
 class TestConfig(unittest.TestCase):
     def setUp(self):
         self.config = config = testing.setUp()
```

