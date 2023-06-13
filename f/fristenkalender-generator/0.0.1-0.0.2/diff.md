# Comparing `tmp/fristenkalender_generator-0.0.1.tar.gz` & `tmp/fristenkalender_generator-0.0.2.tar.gz`

## Comparing `fristenkalender_generator-0.0.1.tar` & `fristenkalender_generator-0.0.2.tar`

### file list

```diff
@@ -1,32 +1,30 @@
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/README.md
--rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/requirements.in
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/requirements.txt
--rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/setup.cfg
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/setup.py
--rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/tox.ini
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/dependabot.yml
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/workflows/black.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/workflows/coverage.yml
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/workflows/no_byte_order_mark.yml
--rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/workflows/packaging_test.yml
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/workflows/python-publish.yml
--rw-r--r--   0        0        0      687 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/workflows/pythonlint.yml
--rw-r--r--   0        0        0      575 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.github/workflows/unittests.yml
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-coverage.in
--rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-coverage.txt
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-formatting.in
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-formatting.txt
--rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-linting.in
--rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-linting.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-tests.in
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-tests.txt
--rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-type_check.in
--rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/dev_requirements/requirements-type_check.txt
--rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/src/_fristenkalender_generator_version.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/src/fristenkalender_generator/__init__.py
--rw-r--r--   0        0        0     9324 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/src/fristenkalender_generator/bdew_calendar_generator.py
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/src/fristenkalender_generator/py.typed
--rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/.gitignore
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      842 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/README.md
+-rw-r--r--   0        0        0       24 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/requirements.in
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     2174 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/tox.ini
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/.github/dependabot.yml
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/.github/workflows/black.yml
+-rw-r--r--   0        0        0      597 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/.github/workflows/coverage.yml
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/.github/workflows/no_byte_order_mark.yml
+-rw-r--r--   0        0        0      591 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/.github/workflows/packaging_test.yml
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0      702 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/.github/workflows/pythonlint.yml
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/.github/workflows/unittests.yml
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/dev_requirements/requirements-coverage.in
+-rw-r--r--   0        0        0      198 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/dev_requirements/requirements-coverage.txt
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/dev_requirements/requirements-formatting.in
+-rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/dev_requirements/requirements-formatting.txt
+-rw-r--r--   0        0        0       55 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/dev_requirements/requirements-linting.in
+-rw-r--r--   0        0        0      464 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/dev_requirements/requirements-linting.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/dev_requirements/requirements-tests.in
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/dev_requirements/requirements-tests.txt
+-rw-r--r--   0        0        0       70 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/dev_requirements/requirements-type_check.in
+-rw-r--r--   0        0        0      459 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/dev_requirements/requirements-type_check.txt
+-rw-r--r--   0        0        0       18 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/src/_fristenkalender_generator_version.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/src/fristenkalender_generator/__init__.py
+-rw-r--r--   0        0        0     9406 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/src/fristenkalender_generator/bdew_calendar_generator.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/src/fristenkalender_generator/py.typed
+-rw-r--r--   0        0        0     1915 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/.gitignore
+-rw-r--r--   0        0        0     2727 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1889 2020-02-02 00:00:00.000000 fristenkalender_generator-0.0.2/PKG-INFO
```

### Comparing `fristenkalender_generator-0.0.1/.pre-commit-config.yaml` & `fristenkalender_generator-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.1/README.md` & `fristenkalender_generator-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.1/requirements.txt` & `fristenkalender_generator-0.0.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.1/tox.ini` & `fristenkalender_generator-0.0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.1/.github/dependabot.yml` & `fristenkalender_generator-0.0.2/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.1/.github/workflows/black.yml` & `fristenkalender_generator-0.0.2/.github/workflows/black.yml`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.1/.github/workflows/coverage.yml` & `fristenkalender_generator-0.0.2/.github/workflows/coverage.yml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 on: [push]
 jobs:
   coverage:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.11"]
+        python-version: ["3.9", "3.10", "3.11"]
         os: [ubuntu-latest]
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `fristenkalender_generator-0.0.1/.github/workflows/packaging_test.yml` & `fristenkalender_generator-0.0.2/.github/workflows/packaging_test.yml`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.1/.github/workflows/python-publish.yml` & `fristenkalender_generator-0.0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.1/.github/workflows/pythonlint.yml` & `fristenkalender_generator-0.0.2/.github/workflows/pythonlint.yml`

 * *Files 3% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 on: [push]
 jobs:
   pylint:
     name: Python Code Quality and Lint
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.11"]
+        python-version: ["3.9", "3.10", "3.11"]
         os: [ubuntu-latest]
         linter-env: ["linting", "type_check"]
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
```

### Comparing `fristenkalender_generator-0.0.1/.github/workflows/unittests.yml` & `fristenkalender_generator-0.0.2/.github/workflows/unittests.yml`

 * *Files 20% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 on: [push]
 jobs:
   pytest:
     runs-on: ${{ matrix.os }}
     strategy:
       matrix:
-        python-version: ["3.11"]
+        python-version: ["3.9", "3.10", "3.11"]
         os: [ubuntu-latest]
     steps:
       - uses: actions/checkout@v3
       - name: Set up Python ${{ matrix.python-version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python-version }}
```

### Comparing `fristenkalender_generator-0.0.1/src/fristenkalender_generator/bdew_calendar_generator.py` & `fristenkalender_generator-0.0.2/src/fristenkalender_generator/bdew_calendar_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 """
 This module can produce a list of calendar entries with bdew Fristen
 """
 
 import dataclasses
+import re
 from calendar import monthrange
 from datetime import date, datetime, timedelta
+from enum import Enum
 from pathlib import Path
-from enum import StrEnum
-import re
 
 from bdew_datetimes.periods import get_nth_working_day_of_month, get_previous_working_day
 from icalendar import Calendar, Event  # type: ignore[import]
 
 
-class FristenType(StrEnum):
+class FristenType(Enum):
     """
     This class represents a type of a Frist
     """
 
     MABIS = "MABIS"
     GPKE = "GPKE"
     GELI = "GELI"
@@ -39,19 +39,19 @@
     """
     This class represents a Frist with a type
     """
 
     type: FristenType
 
 
-_fristen_type_to_label_mapping: dict[FristenType, list[str]] = {
-    FristenType.MABIS: ["5WT", "12WT", "17WT", "18WT", "20WT", "30WT", "42WT", "LWT"],
-    FristenType.GELI: ["16WT"],
-    FristenType.KOV: ["5WT", "10WT", "12WT", "14WT", "17WT", "18WT", "20WT", "21WT", "26WT"],
-    FristenType.GPKE: ["3LWT"],
+_fristen_type_to_label_mapping: dict[str, list[str]] = {
+    FristenType.MABIS.value: ["5WT", "12WT", "17WT", "18WT", "20WT", "30WT", "42WT", "LWT"],
+    FristenType.GELI.value: ["16WT"],
+    FristenType.KOV.value: ["5WT", "10WT", "12WT", "14WT", "17WT", "18WT", "20WT", "21WT", "26WT"],
+    FristenType.GPKE.value: ["3LWT"],
 }
 """
 maps a fristen type to the different fristen associated with the type
 """
 
 
 class FristenkalenderGenerator:
@@ -62,15 +62,17 @@
 
     def generate_fristen_for_type(self, year: int, fristen_type: FristenType) -> list[FristWithAttributesAndType]:
         """
         Generate the list of fristen for a given year with a given type
         """
         fristen: list[FristWithAttributesAndType] = []
 
-        for label in _fristen_type_to_label_mapping[fristen_type]:
+        stringified_fristen_type: str = fristen_type.value
+
+        for label in _fristen_type_to_label_mapping[stringified_fristen_type]:
             if label == "LWT":
                 nth_day = 0
             elif label == "3LWT":
                 nth_day = 3
             elif "LWT" in label:
                 raise NotImplementedError("Only LWT and 3LWT are implemented at the moment")
             else:
```

### Comparing `fristenkalender_generator-0.0.1/.gitignore` & `fristenkalender_generator-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fristenkalender_generator-0.0.1/pyproject.toml` & `fristenkalender_generator-0.0.2/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -9,32 +9,34 @@
 requires = ["hatchling>=1.8.0", "hatch-vcs", "hatch-fancy-pypi-readme"]
 build-backend = "hatchling.build"
 
 [project]
 name = "fristenkalender_generator"
 description = "A Python package that generates the raw data for the 'Hochfrequenz Fristenkalender'"
 license = { text = "MIT" }
-requires-python = ">=3.11"
+requires-python = ">=3.9"
 authors = [
     { name = "Konstantin Klein", email = "konstantin.klein@hochfrequenz.de" },
 ]
 keywords = ["fristenkalender", "bdew", "hochfrequenz"]
 classifiers = [
     "Development Status :: 4 - Beta",
     "Environment :: Console",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3 :: Only",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 dependencies = [
     "bdew_datetimes",
-    "icalendar"
+    "icalendar",
     # add everything you add in requirements.in here
 ]
 dynamic = ["readme", "version"]
 
 [project.urls]
 Changelog = "https://github.com/Hochfrequenz/fristenkalender_generator/releases"
 Homepage = "https://github.com/Hochfrequenz/fristenkalender_generator"
@@ -84,13 +86,8 @@
 
 [tool.hatchling]
 package-data = [
     "src/py.typed", # marks package as type-hinter compatible
 ]
 
 [tool.coverage.run]
-omit = [
-    ".tox/*",
-    "unittests/*",
-]
-
-
+omit = [".tox/*", "unittests/*"]
```

### Comparing `fristenkalender_generator-0.0.1/PKG-INFO` & `fristenkalender_generator-0.0.2/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 Metadata-Version: 2.1
 Name: fristenkalender_generator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A Python package that generates the raw data for the 'Hochfrequenz Fristenkalender'
 Project-URL: Changelog, https://github.com/Hochfrequenz/fristenkalender_generator/releases
 Project-URL: Homepage, https://github.com/Hochfrequenz/fristenkalender_generator
 Author-email: Konstantin Klein <konstantin.klein@hochfrequenz.de>
 License: MIT
 Keywords: bdew,fristenkalender,hochfrequenz
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Python: >=3.11
+Requires-Python: >=3.9
 Requires-Dist: bdew-datetimes
 Requires-Dist: icalendar
 Description-Content-Type: text/markdown
 
 # fristenkalender_generator
 
 ![Unittests status badge](https://github.com/Hochfrequenz/fristenkalender_generator/workflows/Unittests/badge.svg)
```

