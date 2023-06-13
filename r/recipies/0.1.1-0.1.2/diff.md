# Comparing `tmp/recipies-0.1.1.tar.gz` & `tmp/recipies-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "recipies-0.1.1.tar", last modified: Tue Jun 13 10:58:58 2023, max compression
+gzip compressed data, was "recipies-0.1.2.tar", last modified: Tue Jun 13 14:40:26 2023, max compression
```

## Comparing `recipies-0.1.1.tar` & `recipies-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,25 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 10:58:58.383807 recipies-0.1.1/
--rw-rw-rw-   0        0        0     1135 2023-06-13 10:44:53.000000 recipies-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     3588 2023-06-13 10:58:58.383807 recipies-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     3009 2023-06-13 10:57:08.000000 recipies-0.1.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 10:58:58.377804 recipies-0.1.1/recipies.egg-info/
--rw-rw-rw-   0        0        0     3588 2023-06-13 10:58:58.000000 recipies-0.1.1/recipies.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      364 2023-06-13 10:58:58.000000 recipies-0.1.1/recipies.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 10:58:58.000000 recipies-0.1.1/recipies.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-06-13 10:58:58.000000 recipies-0.1.1/recipies.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2023-06-13 10:50:53.000000 recipies-0.1.1/recipies.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0      119 2023-06-13 10:58:58.000000 recipies-0.1.1/recipies.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 10:58:58.000000 recipies-0.1.1/recipies.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 10:58:58.384809 recipies-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0     2821 2023-06-13 10:58:25.000000 recipies-0.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 10:58:58.382808 recipies-0.1.1/tests/
--rw-rw-rw-   0        0        0     3712 2022-11-25 13:30:22.000000 recipies-0.1.1/tests/test_ingredients.py
--rw-rw-rw-   0        0        0      682 2022-11-25 13:30:22.000000 recipies-0.1.1/tests/test_recipe.py
--rw-rw-rw-   0        0        0        0 2022-11-25 14:11:21.000000 recipies-0.1.1/tests/test_recipys.py
--rw-rw-rw-   0        0        0     3407 2022-11-25 13:30:22.000000 recipies-0.1.1/tests/test_selectors.py
--rw-rw-rw-   0        0        0    13306 2023-06-01 11:16:00.000000 recipies-0.1.1/tests/test_steps.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:40:26.917679 recipies-0.1.2/
+-rw-rw-rw-   0        0        0     1135 2023-06-13 10:44:53.000000 recipies-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     3591 2023-06-13 14:40:26.916671 recipies-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     3009 2023-06-13 10:57:08.000000 recipies-0.1.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 14:40:26.907930 recipies-0.1.2/recipies.egg-info/
+-rw-rw-rw-   0        0        0     3591 2023-06-13 14:40:26.000000 recipies-0.1.2/recipies.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      426 2023-06-13 14:40:26.000000 recipies-0.1.2/recipies.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 14:40:26.000000 recipies-0.1.2/recipies.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-06-13 10:50:53.000000 recipies-0.1.2/recipies.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      119 2023-06-13 14:40:26.000000 recipies-0.1.2/recipies.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-06-13 14:40:26.000000 recipies-0.1.2/recipies.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 14:40:26.912055 recipies-0.1.2/recipys/
+-rw-rw-rw-   0        0        0        0 2022-11-25 13:30:22.000000 recipies-0.1.2/recipys/__init__.py
+-rw-rw-rw-   0        0        0     4775 2022-11-25 13:30:22.000000 recipies-0.1.2/recipys/ingredients.py
+-rw-rw-rw-   0        0        0     6057 2022-11-25 13:30:22.000000 recipies-0.1.2/recipys/recipe.py
+-rw-rw-rw-   0        0        0     8322 2022-11-25 13:30:22.000000 recipies-0.1.2/recipys/selector.py
+-rw-rw-rw-   0        0        0    15196 2023-06-12 12:33:59.000000 recipies-0.1.2/recipys/step.py
+-rw-rw-rw-   0        0        0       42 2023-06-13 14:40:26.917679 recipies-0.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     2724 2023-06-13 14:40:20.000000 recipies-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 14:40:26.916671 recipies-0.1.2/tests/
+-rw-rw-rw-   0        0        0     3712 2022-11-25 13:30:22.000000 recipies-0.1.2/tests/test_ingredients.py
+-rw-rw-rw-   0        0        0      682 2022-11-25 13:30:22.000000 recipies-0.1.2/tests/test_recipe.py
+-rw-rw-rw-   0        0        0        0 2022-11-25 14:11:21.000000 recipies-0.1.2/tests/test_recipys.py
+-rw-rw-rw-   0        0        0     3407 2022-11-25 13:30:22.000000 recipies-0.1.2/tests/test_selectors.py
+-rw-rw-rw-   0        0        0    13306 2023-06-01 11:16:00.000000 recipies-0.1.2/tests/test_steps.py
```

### Comparing `recipies-0.1.1/LICENSE` & `recipies-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `recipies-0.1.1/PKG-INFO` & `recipies-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: recipies
-Version: 0.1.1
-Summary: A modular preprocessing package for Pandas Dataframe
+Version: 0.1.2
+Summary: A modular preprocessing package for a Pandas Dataframe.
 Home-page: https://github.com/rvandewater/recipys
 Author: Robin van de Water
 Author-email: robin.vandewater@hpi.de
 License: MIT license
 Keywords: recipies
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `recipies-0.1.1/README.md` & `recipies-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `recipies-0.1.1/recipies.egg-info/PKG-INFO` & `recipies-0.1.2/recipies.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: recipies
-Version: 0.1.1
-Summary: A modular preprocessing package for Pandas Dataframe
+Version: 0.1.2
+Summary: A modular preprocessing package for a Pandas Dataframe.
 Home-page: https://github.com/rvandewater/recipys
 Author: Robin van de Water
 Author-email: robin.vandewater@hpi.de
 License: MIT license
 Keywords: recipies
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `recipies-0.1.1/setup.py` & `recipies-0.1.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,24 +55,23 @@
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Programming Language :: Python :: 3.10",
     ],
-    description="A modular preprocessing package for Pandas Dataframe",
-    entry_points={"console_scripts": ["recipys = recipys.recipe:Recipe"]},
+    description="A modular preprocessing package for a Pandas Dataframe.",
     install_requires=parse_environment_yml(),
     license="MIT license",
     long_description=readme,
     long_description_content_type='text/markdown',
     include_package_data=True,
     keywords="recipies",
     name="recipies",
-    packages=find_packages(include=["recipies"]),
+    packages=["recipys"],
     setup_requires=setup_requirements,
     test_suite="tests",
     tests_require=[],
     url="https://github.com/rvandewater/recipys",
-    version="0.1.1",
+    version="0.1.2",
     zip_safe=False,
 )
```

### Comparing `recipies-0.1.1/tests/test_ingredients.py` & `recipies-0.1.2/tests/test_ingredients.py`

 * *Files identical despite different names*

### Comparing `recipies-0.1.1/tests/test_recipe.py` & `recipies-0.1.2/tests/test_recipe.py`

 * *Files identical despite different names*

### Comparing `recipies-0.1.1/tests/test_selectors.py` & `recipies-0.1.2/tests/test_selectors.py`

 * *Files identical despite different names*

### Comparing `recipies-0.1.1/tests/test_steps.py` & `recipies-0.1.2/tests/test_steps.py`

 * *Files identical despite different names*

