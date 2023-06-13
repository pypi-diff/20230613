# Comparing `tmp/nhs_number-1.3.2.tar.gz` & `tmp/nhs_number-1.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nhs_number-1.3.2.tar", max compression
+gzip compressed data, was "nhs_number-1.3.3.tar", max compression
```

## Comparing `nhs_number-1.3.2.tar` & `nhs_number-1.3.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1097 2023-06-13 11:51:38.579574 nhs_number-1.3.2/LICENSE
--rw-r--r--   0        0        0     1232 2023-06-13 11:51:38.579574 nhs_number-1.3.2/README.md
--rw-r--r--   0        0        0      779 2023-06-13 11:51:38.579574 nhs_number-1.3.2/nhs_number/__init__.py
--rw-r--r--   0        0        0     5081 2023-06-13 11:51:38.579574 nhs_number-1.3.2/nhs_number/constants.py
--rw-r--r--   0        0        0     2701 2023-06-13 11:51:38.579574 nhs_number-1.3.2/nhs_number/details.py
--rw-r--r--   0        0        0     2438 2023-06-13 11:51:38.579574 nhs_number-1.3.2/nhs_number/generate.py
--rw-r--r--   0        0        0     1814 2023-06-13 11:51:38.579574 nhs_number-1.3.2/nhs_number/standardise.py
--rw-r--r--   0        0        0     2733 2023-06-13 11:51:38.583574 nhs_number-1.3.2/nhs_number/validate.py
--rw-r--r--   0        0        0     1595 2023-06-13 11:51:38.583574 nhs_number-1.3.2/pyproject.toml
--rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 nhs_number-1.3.2/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-06-13 13:54:57.104990 nhs_number-1.3.3/LICENSE
+-rw-r--r--   0        0        0     1301 2023-06-13 13:54:57.104990 nhs_number-1.3.3/README.md
+-rw-r--r--   0        0        0      779 2023-06-13 13:54:57.108990 nhs_number-1.3.3/nhs_number/__init__.py
+-rw-r--r--   0        0        0     5081 2023-06-13 13:54:57.108990 nhs_number-1.3.3/nhs_number/constants.py
+-rw-r--r--   0        0        0     2701 2023-06-13 13:54:57.108990 nhs_number-1.3.3/nhs_number/details.py
+-rw-r--r--   0        0        0     2438 2023-06-13 13:54:57.108990 nhs_number-1.3.3/nhs_number/generate.py
+-rw-r--r--   0        0        0     1814 2023-06-13 13:54:57.108990 nhs_number-1.3.3/nhs_number/standardise.py
+-rw-r--r--   0        0        0     2733 2023-06-13 13:54:57.108990 nhs_number-1.3.3/nhs_number/validate.py
+-rw-r--r--   0        0        0     1585 2023-06-13 13:54:57.108990 nhs_number-1.3.3/pyproject.toml
+-rw-r--r--   0        0        0     2606 1970-01-01 00:00:00.000000 nhs_number-1.3.3/PKG-INFO
```

### Comparing `nhs_number-1.3.2/LICENSE` & `nhs_number-1.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.2/README.md` & `nhs_number-1.3.3/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -29,13 +29,13 @@
         <td>Downloads</td>
         <td><img src='https://img.shields.io/pypi/dm/nhs-number'></td>
     </tr>
 </table>
 
 ## Documentation
 
-[Documentation](docs/index.md)
+A new and improved documentation site is available at <https://nhs-number.uk-fci.tech>
 
-## Changelog
 
-[Changelog](docs/changelog.md)
+## Changelog
 
+<https://nhs-number.uk-fci.tech/changelog/>
```

#### html2text {}

```diff
@@ -7,9 +7,10 @@
                    number.svg]                         badge.svg]
                    [https://                           [https://img.shields.io/
 Wheel              img.shields.io/pypi/ Implementation pypi/implementation/nhs-
                    wheel/nhs-number]                   number]
                    [https://                           [https://img.shields.io/
 Status             img.shields.io/pypi/ Downloads      pypi/dm/nhs-number]
                    status/nhs-number]
-## Documentation [Documentation](docs/index.md) ## Changelog [Changelog](docs/
-changelog.md)
+## Documentation A new and improved documentation site is available at
+nhs-number.uk-fci.tech> ## Changelog
+nhs-number.uk-fci.tech/changelog/>
```

### Comparing `nhs_number-1.3.2/nhs_number/__init__.py` & `nhs_number-1.3.3/nhs_number/__init__.py`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.2/nhs_number/constants.py` & `nhs_number-1.3.3/nhs_number/constants.py`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.2/nhs_number/details.py` & `nhs_number-1.3.3/nhs_number/details.py`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.2/nhs_number/generate.py` & `nhs_number-1.3.3/nhs_number/generate.py`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.2/nhs_number/standardise.py` & `nhs_number-1.3.3/nhs_number/standardise.py`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.2/nhs_number/validate.py` & `nhs_number-1.3.3/nhs_number/validate.py`

 * *Files identical despite different names*

### Comparing `nhs_number-1.3.2/pyproject.toml` & `nhs_number-1.3.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "nhs-number"
-version = "1.3.2"
+version = "1.3.3"
 description = "Python package to provide utilities for NHS Numbers, including validity checks, normalisation, and generation."
 authors = [
     "Andy Law <andy.law@roslin.ed.ac.uk>",
     "Marcus Baw <marcusbaw@gmail.com>",
     ]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "nhs_number"}]
-homepage = "https://uk-fci.github.io/nhs-number/"
-documentation = "https://uk-fci.github.io/nhs-number/"
+homepage = "https://nhs-number.uk-fci.tech/"
+documentation = "https://nhs-number.uk-fci.tech/"
 repository = "https://github.com/uk-fci/nhs-number"
 
 exclude = ["tests/local-test-data/*"]
 
 classifiers = [
     'Development Status :: 5 - Production/Stable',
     'License :: OSI Approved :: MIT License',
```

### Comparing `nhs_number-1.3.2/PKG-INFO` & `nhs_number-1.3.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: nhs-number
-Version: 1.3.2
+Version: 1.3.3
 Summary: Python package to provide utilities for NHS Numbers, including validity checks, normalisation, and generation.
-Home-page: https://uk-fci.github.io/nhs-number/
+Home-page: https://nhs-number.uk-fci.tech/
 License: MIT
 Author: Andy Law
 Author-email: andy.law@roslin.ed.ac.uk
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
@@ -17,15 +17,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Project-URL: Documentation, https://uk-fci.github.io/nhs-number/
+Project-URL: Documentation, https://nhs-number.uk-fci.tech/
 Project-URL: Issue Tracker, https://github.com/uk-fci/nhs-number/issues
 Project-URL: Repository, https://github.com/uk-fci/nhs-number
 Description-Content-Type: text/markdown
 
 # nhs-number
 
 Python package to provide utilities for NHS Numbers, including validity checks, normalisation, and generation.
@@ -57,14 +57,14 @@
         <td>Downloads</td>
         <td><img src='https://img.shields.io/pypi/dm/nhs-number'></td>
     </tr>
 </table>
 
 ## Documentation
 
-[Documentation](docs/index.md)
+A new and improved documentation site is available at <https://nhs-number.uk-fci.tech>
 
-## Changelog
 
-[Changelog](docs/changelog.md)
+## Changelog
 
+<https://nhs-number.uk-fci.tech/changelog/>
```

#### html2text {}

```diff
@@ -1,33 +1,33 @@
-Metadata-Version: 2.1 Name: nhs-number Version: 1.3.2 Summary: Python package
+Metadata-Version: 2.1 Name: nhs-number Version: 1.3.3 Summary: Python package
 to provide utilities for NHS Numbers, including validity checks, normalisation,
-and generation. Home-page: https://uk-fci.github.io/nhs-number/ License: MIT
-Author: Andy Law Author-email: andy.law@roslin.ed.ac.uk Requires-Python:
->=3.7,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
-Intended Audience :: Developers Classifier: Intended Audience :: Healthcare
-Industry Classifier: Intended Audience :: Science/Research Classifier: License
-:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+and generation. Home-page: https://nhs-number.uk-fci.tech/ License: MIT Author:
+Andy Law Author-email: andy.law@roslin.ed.ac.uk Requires-Python: >=3.7,<4.0
+Classifier: Development Status :: 5 - Production/Stable Classifier: Intended
+Audience :: Developers Classifier: Intended Audience :: Healthcare Industry
+Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
+Approved :: MIT License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
 Mathematics Classifier: Topic :: Scientific/Engineering :: Medical Science
 Apps. Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Project-URL: Documentation, https://uk-fci.github.io/nhs-number/ Project-URL:
-Issue Tracker, https://github.com/uk-fci/nhs-number/issues Project-URL:
-Repository, https://github.com/uk-fci/nhs-number Description-Content-Type:
-text/markdown # nhs-number Python package to provide utilities for NHS Numbers,
-including validity checks, normalisation, and generation. ## Package
-Information
+Project-URL: Documentation, https://nhs-number.uk-fci.tech/ Project-URL: Issue
+Tracker, https://github.com/uk-fci/nhs-number/issues Project-URL: Repository,
+https://github.com/uk-fci/nhs-number Description-Content-Type: text/markdown #
+nhs-number Python package to provide utilities for NHS Numbers, including
+validity checks, normalisation, and generation. ## Package Information
 License            [Licence type badge] Version        [Version badge]
                    [https://                           [https://codecov.io/gh/
 Supported versions img.shields.io/pypi/ Coverage       andylaw/NhsNumberChecks/
                    pyversions/nhs-                     branch/main/graph/
                    number.svg]                         badge.svg]
                    [https://                           [https://img.shields.io/
 Wheel              img.shields.io/pypi/ Implementation pypi/implementation/nhs-
                    wheel/nhs-number]                   number]
                    [https://                           [https://img.shields.io/
 Status             img.shields.io/pypi/ Downloads      pypi/dm/nhs-number]
                    status/nhs-number]
-## Documentation [Documentation](docs/index.md) ## Changelog [Changelog](docs/
-changelog.md)
+## Documentation A new and improved documentation site is available at
+nhs-number.uk-fci.tech> ## Changelog
+nhs-number.uk-fci.tech/changelog/>
```

