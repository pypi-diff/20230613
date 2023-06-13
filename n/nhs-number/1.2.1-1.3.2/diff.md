# Comparing `tmp/nhs_number-1.2.1.tar.gz` & `tmp/nhs_number-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nhs_number-1.2.1.tar", last modified: Mon Mar  1 11:32:25 2021, max compression
+gzip compressed data, was "nhs_number-1.3.2.tar", max compression
```

## Comparing `nhs_number-1.2.1.tar` & `nhs_number-1.3.2.tar`

### file list

```diff
@@ -1,13 +1,10 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-01 11:32:25.000000 nhs_number-1.2.1/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2599 2021-03-01 11:32:25.000000 nhs_number-1.2.1/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     1207 2021-03-01 11:32:03.000000 nhs_number-1.2.1/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-01 11:32:25.000000 nhs_number-1.2.1/nhs_number.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2599 2021-03-01 11:32:25.000000 nhs_number-1.2.1/nhs_number.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2021-03-01 11:32:25.000000 nhs_number-1.2.1/nhs_number.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       11 2021-03-01 11:32:25.000000 nhs_number-1.2.1/nhs_number.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      195 2021-03-01 11:32:25.000000 nhs_number-1.2.1/nhs_number.egg-info/SOURCES.txt
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2021-03-01 11:32:25.000000 nhs_number-1.2.1/nhs_number/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2214 2021-03-01 11:32:03.000000 nhs_number-1.2.1/nhs_number/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      132 2021-03-01 11:32:25.000000 nhs_number-1.2.1/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)     1097 2021-03-01 11:32:03.000000 nhs_number-1.2.1/LICENSE
--rw-rw-r--   0 travis    (2000) travis    (2000)     1364 2021-03-01 11:32:03.000000 nhs_number-1.2.1/setup.py
+-rw-r--r--   0        0        0     1097 2023-06-13 11:51:38.579574 nhs_number-1.3.2/LICENSE
+-rw-r--r--   0        0        0     1232 2023-06-13 11:51:38.579574 nhs_number-1.3.2/README.md
+-rw-r--r--   0        0        0      779 2023-06-13 11:51:38.579574 nhs_number-1.3.2/nhs_number/__init__.py
+-rw-r--r--   0        0        0     5081 2023-06-13 11:51:38.579574 nhs_number-1.3.2/nhs_number/constants.py
+-rw-r--r--   0        0        0     2701 2023-06-13 11:51:38.579574 nhs_number-1.3.2/nhs_number/details.py
+-rw-r--r--   0        0        0     2438 2023-06-13 11:51:38.579574 nhs_number-1.3.2/nhs_number/generate.py
+-rw-r--r--   0        0        0     1814 2023-06-13 11:51:38.579574 nhs_number-1.3.2/nhs_number/standardise.py
+-rw-r--r--   0        0        0     2733 2023-06-13 11:51:38.583574 nhs_number-1.3.2/nhs_number/validate.py
+-rw-r--r--   0        0        0     1595 2023-06-13 11:51:38.583574 nhs_number-1.3.2/pyproject.toml
+-rw-r--r--   0        0        0     2547 1970-01-01 00:00:00.000000 nhs_number-1.3.2/PKG-INFO
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `nhs_number-1.2.1/PKG-INFO` & `nhs_number-1.3.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,58 +1,70 @@
 Metadata-Version: 2.1
-Name: nhs_number
-Version: 1.2.1
-Summary: Python library for checking the validity of NHS Numbers
-Home-page: https://github.com/andylaw/NhsNumberChecks
+Name: nhs-number
+Version: 1.3.2
+Summary: Python package to provide utilities for NHS Numbers, including validity checks, normalisation, and generation.
+Home-page: https://uk-fci.github.io/nhs-number/
+License: MIT
 Author: Andy Law
 Author-email: andy.law@roslin.ed.ac.uk
-License: MIT
-Download-URL: https://github.com/andylaw/NhsNumberChecks/tarball/1.2.1
-Description: # NhsNumberChecks
-        Package to provide utilities to check NHS Numbers for validity
-        <table>
-            <tr>
-                <td>License</td>
-                <td><img src="https://img.shields.io/pypi/l/nhs-number" alt="Licence type badge"></td>
-                <td>Version</td>
-                <td><img src="https://img.shields.io/pypi/v/nhs-number" alt="Version badge"></td>
-            </tr>
-            <tr>
-                <td>Travis CI</td>
-                <td><img src='https://www.travis-ci.com/andylaw/NhsNumberChecks.svg?branch=main'></td>
-                <td>Coverage</td>
-                <td><img src='https://codecov.io/gh/andylaw/NhsNumberChecks/branch/main/graph/badge.svg'></td>
-            </tr>
-            <tr>
-                <td>Wheel</td>
-                <td><img src='https://img.shields.io/pypi/wheel/nhs-number'></td>
-                <td>Implementation</td>
-                <td><img src='https://img.shields.io/pypi/implementation/nhs-number'></td>
-            </tr>
-            <tr>
-                <td>Status</td>
-                <td><img src='https://img.shields.io/pypi/status/nhs-number'></td>
-                <td>Downloads</td>
-                <td><img src='https://img.shields.io/pypi/dm/nhs-number'></td>
-            </tr>
-            <tr>
-                <td>Supported versions</td>
-                <td><img src='https://img.shields.io/pypi/pyversions/nhs-number.svg'></td>
-            </tr>
-        </table>
-        
-Platform: UNKNOWN
+Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Topic :: Scientific/Engineering :: Mathematics
-Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Healthcare Industry
 Classifier: Intended Audience :: Science/Research
-Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
+Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Scientific/Engineering :: Mathematics
+Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
+Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Project-URL: Documentation, https://uk-fci.github.io/nhs-number/
+Project-URL: Issue Tracker, https://github.com/uk-fci/nhs-number/issues
+Project-URL: Repository, https://github.com/uk-fci/nhs-number
 Description-Content-Type: text/markdown
+
+# nhs-number
+
+Python package to provide utilities for NHS Numbers, including validity checks, normalisation, and generation.
+
+## Package Information
+
+<table>
+    <tr>
+        <td>License</td>
+        <td><img src="https://img.shields.io/pypi/l/nhs-number" alt="Licence type badge"></td>
+        <td>Version</td>
+        <td><img src="https://img.shields.io/pypi/v/nhs-number" alt="Version badge"></td>
+    </tr>
+    <tr>
+        <td>Supported versions</td>
+        <td><img src='https://img.shields.io/pypi/pyversions/nhs-number.svg'></td>
+        <td>Coverage</td>
+        <td><img src='https://codecov.io/gh/andylaw/NhsNumberChecks/branch/main/graph/badge.svg'></td>
+    </tr>
+    <tr>
+        <td>Wheel</td>
+        <td><img src='https://img.shields.io/pypi/wheel/nhs-number'></td>
+        <td>Implementation</td>
+        <td><img src='https://img.shields.io/pypi/implementation/nhs-number'></td>
+    </tr>
+    <tr>
+        <td>Status</td>
+        <td><img src='https://img.shields.io/pypi/status/nhs-number'></td>
+        <td>Downloads</td>
+        <td><img src='https://img.shields.io/pypi/dm/nhs-number'></td>
+    </tr>
+</table>
+
+## Documentation
+
+[Documentation](docs/index.md)
+
+## Changelog
+
+[Changelog](docs/changelog.md)
+
+
```

#### html2text {}

```diff
@@ -1,35 +1,33 @@
-Metadata-Version: 2.1 Name: nhs_number Version: 1.2.1 Summary: Python library
-for checking the validity of NHS Numbers Home-page: https://github.com/andylaw/
-NhsNumberChecks Author: Andy Law Author-email: andy.law@roslin.ed.ac.uk
-License: MIT Download-URL: https://github.com/andylaw/NhsNumberChecks/tarball/
-1.2.1 Description: # NhsNumberChecks Package to provide utilities to check NHS
-Numbers for validity
-License   [Licence type badge]             Version        [Version badge]
-                                                          [https://
-          [https://www.travis-ci.com/                     codecov.io/gh/
-Travis CI andylaw/                         Coverage       andylaw/
-          NhsNumberChecks.svg?branch=main]                NhsNumberChecks/
-                                                          branch/main/graph/
-                                                          badge.svg]
-                                                          [https://
-          [https://img.shields.io/pypi/                   img.shields.io/
-Wheel     wheel/nhs-number]                Implementation pypi/
-                                                          implementation/
-                                                          nhs-number]
-                                                          [https://
-Status    [https://img.shields.io/pypi/    Downloads      img.shields.io/
-          status/nhs-number]                              pypi/dm/nhs-
-                                                          number]
-Supported [https://img.shields.io/pypi/
-versions  pyversions/nhs-number.svg]
-Platform: UNKNOWN Classifier: Development Status :: 5 - Production/Stable
-Classifier: License :: OSI Approved :: MIT License Classifier: Topic ::
-Scientific/Engineering :: Mathematics Classifier: Topic :: Software Development
-:: Libraries :: Python Modules Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Healthcare Industry Classifier: Intended
-Audience :: Science/Research Classifier: Topic :: Scientific/Engineering ::
-Medical Science Apps. Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7 Classifier: Programming
-Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6 Classifier: Programming
-Language :: Python :: 3.7 Description-Content-Type: text/markdown
+Metadata-Version: 2.1 Name: nhs-number Version: 1.3.2 Summary: Python package
+to provide utilities for NHS Numbers, including validity checks, normalisation,
+and generation. Home-page: https://uk-fci.github.io/nhs-number/ License: MIT
+Author: Andy Law Author-email: andy.law@roslin.ed.ac.uk Requires-Python:
+>=3.7,<4.0 Classifier: Development Status :: 5 - Production/Stable Classifier:
+Intended Audience :: Developers Classifier: Intended Audience :: Healthcare
+Industry Classifier: Intended Audience :: Science/Research Classifier: License
+:: OSI Approved :: MIT License Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
+Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
+Language :: Python :: 3.11 Classifier: Topic :: Scientific/Engineering ::
+Mathematics Classifier: Topic :: Scientific/Engineering :: Medical Science
+Apps. Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Project-URL: Documentation, https://uk-fci.github.io/nhs-number/ Project-URL:
+Issue Tracker, https://github.com/uk-fci/nhs-number/issues Project-URL:
+Repository, https://github.com/uk-fci/nhs-number Description-Content-Type:
+text/markdown # nhs-number Python package to provide utilities for NHS Numbers,
+including validity checks, normalisation, and generation. ## Package
+Information
+License            [Licence type badge] Version        [Version badge]
+                   [https://                           [https://codecov.io/gh/
+Supported versions img.shields.io/pypi/ Coverage       andylaw/NhsNumberChecks/
+                   pyversions/nhs-                     branch/main/graph/
+                   number.svg]                         badge.svg]
+                   [https://                           [https://img.shields.io/
+Wheel              img.shields.io/pypi/ Implementation pypi/implementation/nhs-
+                   wheel/nhs-number]                   number]
+                   [https://                           [https://img.shields.io/
+Status             img.shields.io/pypi/ Downloads      pypi/dm/nhs-number]
+                   status/nhs-number]
+## Documentation [Documentation](docs/index.md) ## Changelog [Changelog](docs/
+changelog.md)
```

### Comparing `nhs_number-1.2.1/README.md` & `nhs_number-1.3.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,23 @@
-# NhsNumberChecks
-Package to provide utilities to check NHS Numbers for validity
+# nhs-number
+
+Python package to provide utilities for NHS Numbers, including validity checks, normalisation, and generation.
+
+## Package Information
+
 <table>
     <tr>
         <td>License</td>
         <td><img src="https://img.shields.io/pypi/l/nhs-number" alt="Licence type badge"></td>
         <td>Version</td>
         <td><img src="https://img.shields.io/pypi/v/nhs-number" alt="Version badge"></td>
     </tr>
     <tr>
-        <td>Travis CI</td>
-        <td><img src='https://www.travis-ci.com/andylaw/NhsNumberChecks.svg?branch=main'></td>
+        <td>Supported versions</td>
+        <td><img src='https://img.shields.io/pypi/pyversions/nhs-number.svg'></td>
         <td>Coverage</td>
         <td><img src='https://codecov.io/gh/andylaw/NhsNumberChecks/branch/main/graph/badge.svg'></td>
     </tr>
     <tr>
         <td>Wheel</td>
         <td><img src='https://img.shields.io/pypi/wheel/nhs-number'></td>
         <td>Implementation</td>
@@ -21,12 +25,17 @@
     </tr>
     <tr>
         <td>Status</td>
         <td><img src='https://img.shields.io/pypi/status/nhs-number'></td>
         <td>Downloads</td>
         <td><img src='https://img.shields.io/pypi/dm/nhs-number'></td>
     </tr>
-    <tr>
-        <td>Supported versions</td>
-        <td><img src='https://img.shields.io/pypi/pyversions/nhs-number.svg'></td>
-    </tr>
 </table>
+
+## Documentation
+
+[Documentation](docs/index.md)
+
+## Changelog
+
+[Changelog](docs/changelog.md)
+
```

#### html2text {}

```diff
@@ -1,20 +1,15 @@
-# NhsNumberChecks Package to provide utilities to check NHS Numbers for
-validity
-License   [Licence type badge]             Version        [Version badge]
-                                                          [https://
-          [https://www.travis-ci.com/                     codecov.io/gh/
-Travis CI andylaw/                         Coverage       andylaw/
-          NhsNumberChecks.svg?branch=main]                NhsNumberChecks/
-                                                          branch/main/graph/
-                                                          badge.svg]
-                                                          [https://
-          [https://img.shields.io/pypi/                   img.shields.io/
-Wheel     wheel/nhs-number]                Implementation pypi/
-                                                          implementation/
-                                                          nhs-number]
-                                                          [https://
-Status    [https://img.shields.io/pypi/    Downloads      img.shields.io/
-          status/nhs-number]                              pypi/dm/nhs-
-                                                          number]
-Supported [https://img.shields.io/pypi/
-versions  pyversions/nhs-number.svg]
+# nhs-number Python package to provide utilities for NHS Numbers, including
+validity checks, normalisation, and generation. ## Package Information
+License            [Licence type badge] Version        [Version badge]
+                   [https://                           [https://codecov.io/gh/
+Supported versions img.shields.io/pypi/ Coverage       andylaw/NhsNumberChecks/
+                   pyversions/nhs-                     branch/main/graph/
+                   number.svg]                         badge.svg]
+                   [https://                           [https://img.shields.io/
+Wheel              img.shields.io/pypi/ Implementation pypi/implementation/nhs-
+                   wheel/nhs-number]                   number]
+                   [https://                           [https://img.shields.io/
+Status             img.shields.io/pypi/ Downloads      pypi/dm/nhs-number]
+                   status/nhs-number]
+## Documentation [Documentation](docs/index.md) ## Changelog [Changelog](docs/
+changelog.md)
```

### Comparing `nhs_number-1.2.1/nhs_number/__init__.py` & `nhs_number-1.3.2/nhs_number/standardise.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,56 @@
 """
-Python code to check the validity of NHS Numbers
-"""
-# License: MIT (http://www.opensource.org/licenses/mit-license.php)
+Normalises NHS numbers into a standard string format
+
+Originally derived from Andy Law's nhs_number Python package validation code
 
-__version__ = '1.2.1'
-__author__ = "Andy Law <andy.law@roslin.ed.ac.uk>"
+License: MIT (https://www.opensource.org/licenses/mit-license.php)
 
+Contributors
+* Andy Law <andy.law@roslin.ed.ac.uk>
+* Marcus Baw <marcusbaw@gmail.com>
+"""
+# standard imports
+from __future__ import annotations # for Python 3.7 (remove once we stop supporting 3.7)
 import re
+import warnings
 
-GOOD_FORMAT = r'^(\d{10}|\d{3} \d{3} \d{4}|\d{3}-\d{3}-\d{4})$'
+# third-party imports
 
+# local imports
 
-def is_valid(nhs_number):
-    """
-        Checks the supplied NHS number (as a string) is valid and returns True or False
-    """
-    # Use the normalise_number() function to check that this is a valid format to start with
-    # Any non-valid input will result in an empty string return
-    nhs_number = normalise_number(nhs_number)
-    if not nhs_number:
-        return False
-
-    # The first 9 numbers are used to calculate the checksum, which should match the last digit
-    (first_part, check_digit) = (nhs_number[:-1], int(nhs_number[-1]))
-
-    # For the algorithm that calculates the checksum digit, see
-    # https://www.closer.ac.uk/wp-content/uploads/CLOSER-NHS-ID-Resource-Report-Apr2018.pdf
-    parts_list = [int(digit) * (10 - index) for index, digit in enumerate(first_part)]
-    list_sum = sum(parts_list)
-    checksum = 11 - (list_sum % 11)
-    if checksum == 11:
-        checksum = 0
-
-    # NOTE: a checksum of 10 is invalid (and is quoted as a special case), but the check for equality
-    # will catch that circumstance anyway
-    return False if checksum != check_digit else True
+
+GOOD_FORMAT = r"^(\d{10}|\d{3} \d{3} \d{4}|\d{3}-\d{3}-\d{4})$"
 
 
-def normalise_number(nhs_number):
+def standardise_format(nhs_number: str | int) -> str:
     """
     Extract the 10 digits of an NHS number if the supplied string is a valid
-    format.
+    format. If supplied as an int it will attempt to convert it to a string for
+    processing.
     Valid formats are:
       123 456 7890
       123-456-7890
       1234567890
     with any amount of leading and trailing white space
     If Valid, this routine will return '1234567890' for all of the above inputs.
-    An invalid input will result in the empty string which makes it possible to use a call
-    to this function to test for valid format (but not valid checksum)
+    An invalid input will result in the empty string which makes it possible
+    to use a call to this function to test for valid format (but not valid
+    checksum)
     :type nhs_number: basestring
     :param nhs_number:
     :return: 10 digit numerical string or the empty string
     """
-    working_number = nhs_number.strip()
+    if isinstance(nhs_number, int):
+        working_number = str(nhs_number).zfill(10)
+    else:
+        working_number = nhs_number.strip()
     if re.search(GOOD_FORMAT, working_number) is None:
-        working_number = ''
-    working_number = re.sub('[- ]', '', working_number)
+        working_number = ""
+    working_number = re.sub("[- ]", "", working_number)
     return working_number
+
+
+def normalise_number(nhs_number: str) -> str:
+    warnings.warn("The normalise_number() function is deprecated - use "
+                  "standardise_format() instead", DeprecationWarning)
+    return standardise_format(nhs_number)
```

### Comparing `nhs_number-1.2.1/LICENSE` & `nhs_number-1.3.2/LICENSE`

 * *Files identical despite different names*

