# Comparing `tmp/unittest_parametrize-1.0.0.tar.gz` & `tmp/unittest_parametrize-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unittest_parametrize-1.0.0.tar", last modified: Tue Mar 28 16:35:05 2023, max compression
+gzip compressed data, was "unittest_parametrize-1.1.0.tar", last modified: Tue Jun 13 19:08:15 2023, max compression
```

## Comparing `unittest_parametrize-1.0.0.tar` & `unittest_parametrize-1.1.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-03-28 16:35:05.595205 unittest_parametrize-1.0.0/
--rw-r--r--   0 adamjohnson   (501) staff       (20)       87 2023-03-28 16:35:03.000000 unittest_parametrize-1.0.0/CHANGELOG.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-03-28 10:40:12.000000 unittest_parametrize-1.0.0/LICENSE
--rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-03-28 10:36:40.000000 unittest_parametrize-1.0.0/MANIFEST.in
--rw-r--r--   0 adamjohnson   (501) staff       (20)    12422 2023-03-28 16:35:05.595281 unittest_parametrize-1.0.0/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)    11296 2023-03-28 16:34:33.000000 unittest_parametrize-1.0.0/README.rst
--rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-03-28 10:36:40.000000 unittest_parametrize-1.0.0/pyproject.toml
--rw-r--r--   0 adamjohnson   (501) staff       (20)     1495 2023-03-28 16:35:05.595650 unittest_parametrize-1.0.0/setup.cfg
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-03-28 16:35:05.592466 unittest_parametrize-1.0.0/src/
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-03-28 16:35:05.594159 unittest_parametrize-1.0.0/src/unittest_parametrize/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     5110 2023-03-28 16:34:33.000000 unittest_parametrize-1.0.0/src/unittest_parametrize/__init__.py
--rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-03-28 10:44:29.000000 unittest_parametrize-1.0.0/src/unittest_parametrize/py.typed
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-03-28 16:35:05.594967 unittest_parametrize-1.0.0/src/unittest_parametrize.egg-info/
--rw-r--r--   0 adamjohnson   (501) staff       (20)    12422 2023-03-28 16:35:05.000000 unittest_parametrize-1.0.0/src/unittest_parametrize.egg-info/PKG-INFO
--rw-r--r--   0 adamjohnson   (501) staff       (20)      461 2023-03-28 16:35:05.000000 unittest_parametrize-1.0.0/src/unittest_parametrize.egg-info/SOURCES.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-03-28 16:35:05.000000 unittest_parametrize-1.0.0/src/unittest_parametrize.egg-info/dependency_links.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-03-28 16:35:05.000000 unittest_parametrize-1.0.0/src/unittest_parametrize.egg-info/not-zip-safe
--rw-r--r--   0 adamjohnson   (501) staff       (20)       46 2023-03-28 16:35:05.000000 unittest_parametrize-1.0.0/src/unittest_parametrize.egg-info/requires.txt
--rw-r--r--   0 adamjohnson   (501) staff       (20)       21 2023-03-28 16:35:05.000000 unittest_parametrize-1.0.0/src/unittest_parametrize.egg-info/top_level.txt
-drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-03-28 16:35:05.595091 unittest_parametrize-1.0.0/tests/
--rw-r--r--   0 adamjohnson   (501) staff       (20)     7189 2023-03-28 16:34:33.000000 unittest_parametrize-1.0.0/tests/test_unittest_parametrize.py
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-13 19:08:15.054589 unittest_parametrize-1.1.0/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      150 2023-06-13 19:08:12.000000 unittest_parametrize-1.1.0/CHANGELOG.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1069 2023-03-28 10:40:12.000000 unittest_parametrize-1.1.0/LICENSE
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      103 2023-03-28 10:36:40.000000 unittest_parametrize-1.1.0/MANIFEST.in
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    14325 2023-06-13 19:08:15.054675 unittest_parametrize-1.1.0/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    13148 2023-06-13 14:15:26.000000 unittest_parametrize-1.1.0/README.rst
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      448 2023-03-28 10:36:40.000000 unittest_parametrize-1.1.0/pyproject.toml
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     1536 2023-06-13 19:08:15.055019 unittest_parametrize-1.1.0/setup.cfg
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-13 19:08:15.051968 unittest_parametrize-1.1.0/src/
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-13 19:08:15.053414 unittest_parametrize-1.1.0/src/unittest_parametrize/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     5110 2023-03-28 16:34:33.000000 unittest_parametrize-1.1.0/src/unittest_parametrize/__init__.py
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        0 2023-03-28 10:44:29.000000 unittest_parametrize-1.1.0/src/unittest_parametrize/py.typed
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-13 19:08:15.054153 unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)    14325 2023-06-13 19:08:15.000000 unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/PKG-INFO
+-rw-r--r--   0 adamjohnson   (501) staff       (20)      461 2023-06-13 19:08:15.000000 unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/SOURCES.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-13 19:08:15.000000 unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/dependency_links.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)        1 2023-06-13 19:08:14.000000 unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/not-zip-safe
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       46 2023-06-13 19:08:15.000000 unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/requires.txt
+-rw-r--r--   0 adamjohnson   (501) staff       (20)       21 2023-06-13 19:08:15.000000 unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/top_level.txt
+drwxr-xr-x   0 adamjohnson   (501) staff       (20)        0 2023-06-13 19:08:15.054282 unittest_parametrize-1.1.0/tests/
+-rw-r--r--   0 adamjohnson   (501) staff       (20)     7189 2023-03-28 16:34:33.000000 unittest_parametrize-1.1.0/tests/test_unittest_parametrize.py
```

### Comparing `unittest_parametrize-1.0.0/LICENSE` & `unittest_parametrize-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unittest_parametrize-1.0.0/PKG-INFO` & `unittest_parametrize-1.1.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittest_parametrize
-Version: 1.0.0
+Version: 1.1.0
 Summary: Parametrize tests within unittest TestCases.
 Home-page: https://github.com/adamchainz/unittest-parametrize
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/unittest-parametrize/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ====================
 unittest-parametrize
@@ -50,15 +51,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install unittest-parametrize
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of recommendations to write faster, more accurate tests.
 
 ----
@@ -104,18 +105,18 @@
 ``@parametrize`` modifies the class at definition time with Python’s |__init_subclass__ hook|__.
 It removes the original test method and creates wrapped copies with individual names.
 Thus the parametrization should work regardless of the test runner you use (be it unittest, Django’s test runner, pytest, etc.).
 
 .. |__init_subclass__ hook| replace:: ``__init_subclass__`` hook
 __ https://docs.python.org/3/reference/datamodel.html#object.__init_subclass__
 
-Provide argument names as a string
-----------------------------------
+Provide argument names as separate strings
+------------------------------------------
 
-If you need, you can provide argument names as a sequence of strings instead:
+You can provide argument names as a sequence of strings instead:
 
 .. code-block:: python
 
     from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
 
 
@@ -126,14 +127,46 @@
                 (1, 1),
                 (2, 4),
             ],
         )
         def test_square(self, x: int, expected: int) -> None:
             self.assertEqual(x**2, expected)
 
+
+Use ``ParametrizedTestCase`` in your base test case class
+---------------------------------------------------------
+
+``ParametrizedTestCase`` does nothing if there aren’t any ``@parametrize``-decorated tests within a class.
+Therefore you can include it in your project’s base test case class so that ``@parametrize`` works immediately in all test cases.
+
+For example, within a Django project, you can create a set of project-specific base test case classes extending `those provided by Django <https://docs.djangoproject.com/en/stable/topics/testing/tools/#provided-test-case-classes>`__.
+You can do this in a module like ``example.test``, and use the base classes throughout your test suite.
+To add ``ParametrizedTestCase`` to all your copies, use it in a custom ``SimpleTestCase`` and then mixin to others using multiple inheritance like so:
+
+.. code-block:: python
+
+    from django import test
+    from unittest_parametrize import ParametrizedTestCase
+
+
+    class SimpleTestCase(ParametrizedTestCase, test.SimpleTestCase):
+        pass
+
+
+    class TestCase(SimpleTestCase, test.TestCase):
+        pass
+
+
+    class TransactionTestCase(SimpleTestCase, test.TransactionTestCase):
+        pass
+
+
+    class LiveServerTestCase(SimpleTestCase, test.LiveServerTestCase):
+        pass
+
 Custom test name suffixes
 -------------------------
 
 By default, test names are extended with an index, starting at zero.
 You can see these names when running the tests:
 
 .. code-block:: console
@@ -202,38 +235,69 @@
         def test_square(self, x: int, expected: int) -> None:
             self.assertEqual(x**2, expected)
 
 Use with other test decorators
 ------------------------------
 
 ``@parametrize`` tries to ensure it is the top-most (outermost) decorator.
-This limitation exists to ensure that the decorator applies to each test.
-So decorators like ``@mock.patch.object`` need be beneath ``@parametrize``:
+This limitation exists to ensure that other decorators apply to each parametrized test.
+So decorators like ``@mock.patch`` need be beneath ``@parametrize``:
 
 .. code-block:: python
 
     from unittest import mock
     from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
 
 
-    class MockingTests(ParametrizedTestCase):
+    class CarpentryTests(ParametrizedTestCase):
         @parametrize(
             "nails",
-            [(1,), (2,)],
+            [(11,), (17,)],
         )
-        @mock.patch.object(board, "length", new=9001)
-        def test_boarding(self, nails):
+        @mock.patch("example.hammer", autospec=True)
+        def test_nail_a_board(self, mock_hammer, nails):
             ...
 
+Also note that due to how ``mock.patch`` always adds positional arguments at the start, the parametrized arguments must come last.
+``@parametrize`` always adds parameters as keyword arguments, so you can also use `keyword-only syntax <https://peps.python.org/pep-3102/>`__ for parametrized arguments:
+
+.. code-block:: python
+
+    # ...
+    def test_nail_a_board(self, mock_hammer, *, nails):
+        ...
+
 Multiple ``@parametrize`` decorators
 ------------------------------------
 
 ``@parametrize`` is not stackable.
-To create a cross-product of tests, use |itertools.product()|__:
+To create a cross-product of tests, you can use nested list comprehensions:
+
+.. code-block:: python
+
+    from unittest_parametrize import parametrize
+    from unittest_parametrize import ParametrizedTestCase
+
+
+    class RocketTests(ParametrizedTestCase):
+        @parametrize(
+            "use_ions,hyperdrive_level",
+            [
+                (use_ions, hyperdrive_level)
+                for use_ions in [True, False]
+                for hyperdrive_level in [0, 1, 2]
+            ],
+        )
+        def test_takeoff(self, use_ions, hyperdrive_level) -> None:
+            ...
+
+The above creates 2 * 3 = 6 versions of ``test_takeoff``.
+
+For larger combinations, |itertools.product()|__ may be more readable:
 
 .. |itertools.product()| replace:: ``itertools.product()``
 __ https://docs.python.org/3/library/itertools.html#itertools.product
 
 .. code-block:: python
 
     from itertools import product
@@ -253,44 +317,42 @@
             ),
         )
         def test_takeoff(self, use_ions, hyperdrive_level, nose_colour) -> None:
             ...
 
 The above creates 2 * 3 * 2 = 12 versions of ``test_takeoff``.
 
-Use ``ParametrizedTestCase`` in your base test case class
----------------------------------------------------------
-
-``ParametrizedTestCase`` does nothing if there aren’t any ``@parametrize``-decorated tests within a class.
-Therefore you can include it in your project’s base test case class so that ``@parametrize`` works immediately in all test cases.
+Parametrizing multiple tests in a test case
+-------------------------------------------
 
-For example, within a Django project, you can create a set of project-specific base test case classes extending `those provided by Django <https://docs.djangoproject.com/en/stable/topics/testing/tools/#provided-test-case-classes>`__.
-You can do this in a module like ``example.test``, and use the base classes throughout your test suite.
-To add ``ParametrizedTestCase`` to all your copies, use it in a custom ``SimpleTestCase`` and then mixin to others using multiple inheritance like so:
+``@parametrize`` only works as a function decorator, not a class decorator.
+To parametrize all tests within a test case, create a separate decorator and apply it to each method:
 
 .. code-block:: python
 
-    from django import test
+    from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
 
 
-    class SimpleTestCase(ParametrizedTestCase, test.SimpleTestCase):
-        pass
-
-
-    class TestCase(SimpleTestCase, test.TestCase):
-        pass
+    parametrize_race = parametrize(
+        "race",
+        [("Human",), ("Halfling",), ("Dwarf",), ("Elf",)],
+    )
 
 
-    class TransactionTestCase(SimpleTestCase, test.TransactionTestCase):
-        pass
+    class StatsTests(ParametrizedTestCase):
+        @parametrize_race
+        def test_strength(self, race: str) -> None:
+            ...
 
+        @parametrize_race
+        def test_dexterity(self, race: str) -> None:
+            ...
 
-    class LiveServerTestCase(SimpleTestCase, test.LiveServerTestCase):
-        pass
+        ...
 
 History
 =======
 
 When I started writing unit tests, I learned to use `DDT (Data-Driven Tests) <https://ddt.readthedocs.io/en/latest/>`__ for parametrizing tests.
 It works, but the docs are a bit thin, and the API a little obscure (what does ``@ddt`` stand for again?).
```

### Comparing `unittest_parametrize-1.0.0/README.rst` & `unittest_parametrize-1.1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install unittest-parametrize
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of recommendations to write faster, more accurate tests.
 
 ----
@@ -76,18 +76,18 @@
 ``@parametrize`` modifies the class at definition time with Python’s |__init_subclass__ hook|__.
 It removes the original test method and creates wrapped copies with individual names.
 Thus the parametrization should work regardless of the test runner you use (be it unittest, Django’s test runner, pytest, etc.).
 
 .. |__init_subclass__ hook| replace:: ``__init_subclass__`` hook
 __ https://docs.python.org/3/reference/datamodel.html#object.__init_subclass__
 
-Provide argument names as a string
-----------------------------------
+Provide argument names as separate strings
+------------------------------------------
 
-If you need, you can provide argument names as a sequence of strings instead:
+You can provide argument names as a sequence of strings instead:
 
 .. code-block:: python
 
     from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
 
 
@@ -98,14 +98,46 @@
                 (1, 1),
                 (2, 4),
             ],
         )
         def test_square(self, x: int, expected: int) -> None:
             self.assertEqual(x**2, expected)
 
+
+Use ``ParametrizedTestCase`` in your base test case class
+---------------------------------------------------------
+
+``ParametrizedTestCase`` does nothing if there aren’t any ``@parametrize``-decorated tests within a class.
+Therefore you can include it in your project’s base test case class so that ``@parametrize`` works immediately in all test cases.
+
+For example, within a Django project, you can create a set of project-specific base test case classes extending `those provided by Django <https://docs.djangoproject.com/en/stable/topics/testing/tools/#provided-test-case-classes>`__.
+You can do this in a module like ``example.test``, and use the base classes throughout your test suite.
+To add ``ParametrizedTestCase`` to all your copies, use it in a custom ``SimpleTestCase`` and then mixin to others using multiple inheritance like so:
+
+.. code-block:: python
+
+    from django import test
+    from unittest_parametrize import ParametrizedTestCase
+
+
+    class SimpleTestCase(ParametrizedTestCase, test.SimpleTestCase):
+        pass
+
+
+    class TestCase(SimpleTestCase, test.TestCase):
+        pass
+
+
+    class TransactionTestCase(SimpleTestCase, test.TransactionTestCase):
+        pass
+
+
+    class LiveServerTestCase(SimpleTestCase, test.LiveServerTestCase):
+        pass
+
 Custom test name suffixes
 -------------------------
 
 By default, test names are extended with an index, starting at zero.
 You can see these names when running the tests:
 
 .. code-block:: console
@@ -174,38 +206,69 @@
         def test_square(self, x: int, expected: int) -> None:
             self.assertEqual(x**2, expected)
 
 Use with other test decorators
 ------------------------------
 
 ``@parametrize`` tries to ensure it is the top-most (outermost) decorator.
-This limitation exists to ensure that the decorator applies to each test.
-So decorators like ``@mock.patch.object`` need be beneath ``@parametrize``:
+This limitation exists to ensure that other decorators apply to each parametrized test.
+So decorators like ``@mock.patch`` need be beneath ``@parametrize``:
 
 .. code-block:: python
 
     from unittest import mock
     from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
 
 
-    class MockingTests(ParametrizedTestCase):
+    class CarpentryTests(ParametrizedTestCase):
         @parametrize(
             "nails",
-            [(1,), (2,)],
+            [(11,), (17,)],
         )
-        @mock.patch.object(board, "length", new=9001)
-        def test_boarding(self, nails):
+        @mock.patch("example.hammer", autospec=True)
+        def test_nail_a_board(self, mock_hammer, nails):
             ...
 
+Also note that due to how ``mock.patch`` always adds positional arguments at the start, the parametrized arguments must come last.
+``@parametrize`` always adds parameters as keyword arguments, so you can also use `keyword-only syntax <https://peps.python.org/pep-3102/>`__ for parametrized arguments:
+
+.. code-block:: python
+
+    # ...
+    def test_nail_a_board(self, mock_hammer, *, nails):
+        ...
+
 Multiple ``@parametrize`` decorators
 ------------------------------------
 
 ``@parametrize`` is not stackable.
-To create a cross-product of tests, use |itertools.product()|__:
+To create a cross-product of tests, you can use nested list comprehensions:
+
+.. code-block:: python
+
+    from unittest_parametrize import parametrize
+    from unittest_parametrize import ParametrizedTestCase
+
+
+    class RocketTests(ParametrizedTestCase):
+        @parametrize(
+            "use_ions,hyperdrive_level",
+            [
+                (use_ions, hyperdrive_level)
+                for use_ions in [True, False]
+                for hyperdrive_level in [0, 1, 2]
+            ],
+        )
+        def test_takeoff(self, use_ions, hyperdrive_level) -> None:
+            ...
+
+The above creates 2 * 3 = 6 versions of ``test_takeoff``.
+
+For larger combinations, |itertools.product()|__ may be more readable:
 
 .. |itertools.product()| replace:: ``itertools.product()``
 __ https://docs.python.org/3/library/itertools.html#itertools.product
 
 .. code-block:: python
 
     from itertools import product
@@ -225,44 +288,42 @@
             ),
         )
         def test_takeoff(self, use_ions, hyperdrive_level, nose_colour) -> None:
             ...
 
 The above creates 2 * 3 * 2 = 12 versions of ``test_takeoff``.
 
-Use ``ParametrizedTestCase`` in your base test case class
----------------------------------------------------------
-
-``ParametrizedTestCase`` does nothing if there aren’t any ``@parametrize``-decorated tests within a class.
-Therefore you can include it in your project’s base test case class so that ``@parametrize`` works immediately in all test cases.
+Parametrizing multiple tests in a test case
+-------------------------------------------
 
-For example, within a Django project, you can create a set of project-specific base test case classes extending `those provided by Django <https://docs.djangoproject.com/en/stable/topics/testing/tools/#provided-test-case-classes>`__.
-You can do this in a module like ``example.test``, and use the base classes throughout your test suite.
-To add ``ParametrizedTestCase`` to all your copies, use it in a custom ``SimpleTestCase`` and then mixin to others using multiple inheritance like so:
+``@parametrize`` only works as a function decorator, not a class decorator.
+To parametrize all tests within a test case, create a separate decorator and apply it to each method:
 
 .. code-block:: python
 
-    from django import test
+    from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
 
 
-    class SimpleTestCase(ParametrizedTestCase, test.SimpleTestCase):
-        pass
-
-
-    class TestCase(SimpleTestCase, test.TestCase):
-        pass
+    parametrize_race = parametrize(
+        "race",
+        [("Human",), ("Halfling",), ("Dwarf",), ("Elf",)],
+    )
 
 
-    class TransactionTestCase(SimpleTestCase, test.TransactionTestCase):
-        pass
+    class StatsTests(ParametrizedTestCase):
+        @parametrize_race
+        def test_strength(self, race: str) -> None:
+            ...
 
+        @parametrize_race
+        def test_dexterity(self, race: str) -> None:
+            ...
 
-    class LiveServerTestCase(SimpleTestCase, test.LiveServerTestCase):
-        pass
+        ...
 
 History
 =======
 
 When I started writing unit tests, I learned to use `DDT (Data-Driven Tests) <https://ddt.readthedocs.io/en/latest/>`__ for parametrizing tests.
 It works, but the docs are a bit thin, and the API a little obscure (what does ``@ddt`` stand for again?).
```

### Comparing `unittest_parametrize-1.0.0/setup.cfg` & `unittest_parametrize-1.1.0/setup.cfg`

 * *Files 8% similar despite different names*

```diff
@@ -1,30 +1,31 @@
 [metadata]
 name = unittest_parametrize
-version = 1.0.0
+version = 1.1.0
 description = Parametrize tests within unittest TestCases.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 url = https://github.com/adamchainz/unittest-parametrize
 author = Adam Johnson
 author_email = me@adamj.eu
 license = MIT
-license_file = LICENSE
+license_files = LICENSE
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: Developers
 	License :: OSI Approved :: MIT License
 	Natural Language :: English
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3.7
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
 	Programming Language :: Python :: 3.10
 	Programming Language :: Python :: 3.11
+	Programming Language :: Python :: 3.12
 	Typing :: Typed
 keywords = unittest
 project_urls = 
 	Changelog = https://github.com/adamchainz/unittest-parametrize/blob/main/CHANGELOG.rst
 	Mastodon = https://fosstodon.org/@adamchainz
 	Twitter = https://twitter.com/adamchainz
```

### Comparing `unittest_parametrize-1.0.0/src/unittest_parametrize/__init__.py` & `unittest_parametrize-1.1.0/src/unittest_parametrize/__init__.py`

 * *Files identical despite different names*

### Comparing `unittest_parametrize-1.0.0/src/unittest_parametrize.egg-info/PKG-INFO` & `unittest_parametrize-1.1.0/src/unittest_parametrize.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittest-parametrize
-Version: 1.0.0
+Version: 1.1.0
 Summary: Parametrize tests within unittest TestCases.
 Home-page: https://github.com/adamchainz/unittest-parametrize
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/unittest-parametrize/blob/main/CHANGELOG.rst
 Project-URL: Mastodon, https://fosstodon.org/@adamchainz
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 ====================
 unittest-parametrize
@@ -50,15 +51,15 @@
 
 Install with:
 
 .. code-block:: bash
 
     python -m pip install unittest-parametrize
 
-Python 3.7 to 3.11 supported.
+Python 3.7 to 3.12 supported.
 
 ----
 
 **Testing a Django project?**
 Check out my book `Speed Up Your Django Tests <https://adamchainz.gumroad.com/l/suydt>`__ which covers loads of recommendations to write faster, more accurate tests.
 
 ----
@@ -104,18 +105,18 @@
 ``@parametrize`` modifies the class at definition time with Python’s |__init_subclass__ hook|__.
 It removes the original test method and creates wrapped copies with individual names.
 Thus the parametrization should work regardless of the test runner you use (be it unittest, Django’s test runner, pytest, etc.).
 
 .. |__init_subclass__ hook| replace:: ``__init_subclass__`` hook
 __ https://docs.python.org/3/reference/datamodel.html#object.__init_subclass__
 
-Provide argument names as a string
-----------------------------------
+Provide argument names as separate strings
+------------------------------------------
 
-If you need, you can provide argument names as a sequence of strings instead:
+You can provide argument names as a sequence of strings instead:
 
 .. code-block:: python
 
     from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
 
 
@@ -126,14 +127,46 @@
                 (1, 1),
                 (2, 4),
             ],
         )
         def test_square(self, x: int, expected: int) -> None:
             self.assertEqual(x**2, expected)
 
+
+Use ``ParametrizedTestCase`` in your base test case class
+---------------------------------------------------------
+
+``ParametrizedTestCase`` does nothing if there aren’t any ``@parametrize``-decorated tests within a class.
+Therefore you can include it in your project’s base test case class so that ``@parametrize`` works immediately in all test cases.
+
+For example, within a Django project, you can create a set of project-specific base test case classes extending `those provided by Django <https://docs.djangoproject.com/en/stable/topics/testing/tools/#provided-test-case-classes>`__.
+You can do this in a module like ``example.test``, and use the base classes throughout your test suite.
+To add ``ParametrizedTestCase`` to all your copies, use it in a custom ``SimpleTestCase`` and then mixin to others using multiple inheritance like so:
+
+.. code-block:: python
+
+    from django import test
+    from unittest_parametrize import ParametrizedTestCase
+
+
+    class SimpleTestCase(ParametrizedTestCase, test.SimpleTestCase):
+        pass
+
+
+    class TestCase(SimpleTestCase, test.TestCase):
+        pass
+
+
+    class TransactionTestCase(SimpleTestCase, test.TransactionTestCase):
+        pass
+
+
+    class LiveServerTestCase(SimpleTestCase, test.LiveServerTestCase):
+        pass
+
 Custom test name suffixes
 -------------------------
 
 By default, test names are extended with an index, starting at zero.
 You can see these names when running the tests:
 
 .. code-block:: console
@@ -202,38 +235,69 @@
         def test_square(self, x: int, expected: int) -> None:
             self.assertEqual(x**2, expected)
 
 Use with other test decorators
 ------------------------------
 
 ``@parametrize`` tries to ensure it is the top-most (outermost) decorator.
-This limitation exists to ensure that the decorator applies to each test.
-So decorators like ``@mock.patch.object`` need be beneath ``@parametrize``:
+This limitation exists to ensure that other decorators apply to each parametrized test.
+So decorators like ``@mock.patch`` need be beneath ``@parametrize``:
 
 .. code-block:: python
 
     from unittest import mock
     from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
 
 
-    class MockingTests(ParametrizedTestCase):
+    class CarpentryTests(ParametrizedTestCase):
         @parametrize(
             "nails",
-            [(1,), (2,)],
+            [(11,), (17,)],
         )
-        @mock.patch.object(board, "length", new=9001)
-        def test_boarding(self, nails):
+        @mock.patch("example.hammer", autospec=True)
+        def test_nail_a_board(self, mock_hammer, nails):
             ...
 
+Also note that due to how ``mock.patch`` always adds positional arguments at the start, the parametrized arguments must come last.
+``@parametrize`` always adds parameters as keyword arguments, so you can also use `keyword-only syntax <https://peps.python.org/pep-3102/>`__ for parametrized arguments:
+
+.. code-block:: python
+
+    # ...
+    def test_nail_a_board(self, mock_hammer, *, nails):
+        ...
+
 Multiple ``@parametrize`` decorators
 ------------------------------------
 
 ``@parametrize`` is not stackable.
-To create a cross-product of tests, use |itertools.product()|__:
+To create a cross-product of tests, you can use nested list comprehensions:
+
+.. code-block:: python
+
+    from unittest_parametrize import parametrize
+    from unittest_parametrize import ParametrizedTestCase
+
+
+    class RocketTests(ParametrizedTestCase):
+        @parametrize(
+            "use_ions,hyperdrive_level",
+            [
+                (use_ions, hyperdrive_level)
+                for use_ions in [True, False]
+                for hyperdrive_level in [0, 1, 2]
+            ],
+        )
+        def test_takeoff(self, use_ions, hyperdrive_level) -> None:
+            ...
+
+The above creates 2 * 3 = 6 versions of ``test_takeoff``.
+
+For larger combinations, |itertools.product()|__ may be more readable:
 
 .. |itertools.product()| replace:: ``itertools.product()``
 __ https://docs.python.org/3/library/itertools.html#itertools.product
 
 .. code-block:: python
 
     from itertools import product
@@ -253,44 +317,42 @@
             ),
         )
         def test_takeoff(self, use_ions, hyperdrive_level, nose_colour) -> None:
             ...
 
 The above creates 2 * 3 * 2 = 12 versions of ``test_takeoff``.
 
-Use ``ParametrizedTestCase`` in your base test case class
----------------------------------------------------------
-
-``ParametrizedTestCase`` does nothing if there aren’t any ``@parametrize``-decorated tests within a class.
-Therefore you can include it in your project’s base test case class so that ``@parametrize`` works immediately in all test cases.
+Parametrizing multiple tests in a test case
+-------------------------------------------
 
-For example, within a Django project, you can create a set of project-specific base test case classes extending `those provided by Django <https://docs.djangoproject.com/en/stable/topics/testing/tools/#provided-test-case-classes>`__.
-You can do this in a module like ``example.test``, and use the base classes throughout your test suite.
-To add ``ParametrizedTestCase`` to all your copies, use it in a custom ``SimpleTestCase`` and then mixin to others using multiple inheritance like so:
+``@parametrize`` only works as a function decorator, not a class decorator.
+To parametrize all tests within a test case, create a separate decorator and apply it to each method:
 
 .. code-block:: python
 
-    from django import test
+    from unittest_parametrize import parametrize
     from unittest_parametrize import ParametrizedTestCase
 
 
-    class SimpleTestCase(ParametrizedTestCase, test.SimpleTestCase):
-        pass
-
-
-    class TestCase(SimpleTestCase, test.TestCase):
-        pass
+    parametrize_race = parametrize(
+        "race",
+        [("Human",), ("Halfling",), ("Dwarf",), ("Elf",)],
+    )
 
 
-    class TransactionTestCase(SimpleTestCase, test.TransactionTestCase):
-        pass
+    class StatsTests(ParametrizedTestCase):
+        @parametrize_race
+        def test_strength(self, race: str) -> None:
+            ...
 
+        @parametrize_race
+        def test_dexterity(self, race: str) -> None:
+            ...
 
-    class LiveServerTestCase(SimpleTestCase, test.LiveServerTestCase):
-        pass
+        ...
 
 History
 =======
 
 When I started writing unit tests, I learned to use `DDT (Data-Driven Tests) <https://ddt.readthedocs.io/en/latest/>`__ for parametrizing tests.
 It works, but the docs are a bit thin, and the API a little obscure (what does ``@ddt`` stand for again?).
```

### Comparing `unittest_parametrize-1.0.0/tests/test_unittest_parametrize.py` & `unittest_parametrize-1.1.0/tests/test_unittest_parametrize.py`

 * *Files identical despite different names*

