# Comparing `tmp/pystac-client-0.7.0.tar.gz` & `tmp/pystac-client-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pystac-client-0.7.0.tar", last modified: Mon Jun 12 21:16:01 2023, max compression
+gzip compressed data, was "pystac-client-0.7.1.tar", last modified: Tue Jun 13 12:48:18 2023, max compression
```

## Comparing `pystac-client-0.7.0.tar` & `pystac-client-0.7.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:16:01.587874 pystac-client-0.7.0/
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-12 21:15:37.000000 pystac-client-0.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-12 21:15:37.000000 pystac-client-0.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-12 21:16:01.587874 pystac-client-0.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-06-12 21:15:37.000000 pystac-client-0.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:16:01.587874 pystac-client-0.7.0/pystac_client/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/collection_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/conformance.py
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    32409 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/item_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12401 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/stac_api_io.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-12 21:15:37.000000 pystac-client-0.7.0/pystac_client/warnings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:16:01.587874 pystac-client-0.7.0/pystac_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3175 2023-06-12 21:16:01.000000 pystac-client-0.7.0/pystac_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-12 21:16:01.000000 pystac-client-0.7.0/pystac_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 21:16:01.000000 pystac-client-0.7.0/pystac_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-12 21:16:01.000000 pystac-client-0.7.0/pystac_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-12 21:16:01.000000 pystac-client-0.7.0/pystac_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-12 21:16:01.000000 pystac-client-0.7.0/pystac_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 21:16:01.587874 pystac-client-0.7.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 21:16:01.587874 pystac-client-0.7.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-12 21:15:37.000000 pystac-client-0.7.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    25263 2023-06-12 21:15:37.000000 pystac-client-0.7.0/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-12 21:15:37.000000 pystac-client-0.7.0/tests/test_collection_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29284 2023-06-12 21:15:37.000000 pystac-client-0.7.0/tests/test_item_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-06-12 21:15:37.000000 pystac-client-0.7.0/tests/test_stac_api_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:48:18.773177 pystac-client-0.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-13 12:48:04.000000 pystac-client-0.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-13 12:48:04.000000 pystac-client-0.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-13 12:48:18.773177 pystac-client-0.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-06-13 12:48:04.000000 pystac-client-0.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:48:18.773177 pystac-client-0.7.1/pystac_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      431 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11237 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7170 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/conformance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32409 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/item_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2217 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12350 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/stac_api_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-13 12:48:04.000000 pystac-client-0.7.1/pystac_client/warnings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:48:18.773177 pystac-client-0.7.1/pystac_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-13 12:48:18.000000 pystac-client-0.7.1/pystac_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-06-13 12:48:18.000000 pystac-client-0.7.1/pystac_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 12:48:18.000000 pystac-client-0.7.1/pystac_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 12:48:18.000000 pystac-client-0.7.1/pystac_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-06-13 12:48:18.000000 pystac-client-0.7.1/pystac_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 12:48:18.000000 pystac-client-0.7.1/pystac_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 12:48:18.773177 pystac-client-0.7.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 12:48:18.773177 pystac-client-0.7.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-06-13 12:48:04.000000 pystac-client-0.7.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25263 2023-06-13 12:48:04.000000 pystac-client-0.7.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2810 2023-06-13 12:48:04.000000 pystac-client-0.7.1/tests/test_collection_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29284 2023-06-13 12:48:04.000000 pystac-client-0.7.1/tests/test_item_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9118 2023-06-13 12:48:04.000000 pystac-client-0.7.1/tests/test_stac_api_io.py
```

### Comparing `pystac-client-0.7.0/LICENSE` & `pystac-client-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/PKG-INFO` & `pystac-client-0.7.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac-client
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python library for working with SpatioTemporal Asset Catalog (STAC) APIs.
 Author-email: Jon Duckworth <duckontheweb@gmail.com>, Matthew Hanson <matt.a.hanson@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/pystac-client
 Project-URL: documentation, https://pystac-client.readthedocs.io
 Project-URL: repository, https://github.com/stac-utils/pystac-client.git
@@ -32,15 +32,15 @@
 License-File: LICENSE
 
 # STAC Client <!-- omit in toc -->
 
 [![CI](https://github.com/stac-utils/pystac-client/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/stac-utils/pystac-client/actions/workflows/continuous-integration.yml)
 [![Release](https://github.com/stac-utils/pystac-client/actions/workflows/release.yml/badge.svg)](https://github.com/stac-utils/pystac-client/actions/workflows/release.yml)
 [![PyPI version](https://badge.fury.io/py/pystac-client.svg)](https://badge.fury.io/py/pystac-client)
-[![Documentation](https://readthedocs.org/projects/pystac-client/badge/?version=latest)](https://pystac-client.readthedocs.io/en/latest/)
+[![Documentation](https://readthedocs.org/projects/pystac-client/badge/?version=stable)](https://pystac-client.readthedocs.io)
 [![codecov](https://codecov.io/gh/stac-utils/pystac-client/branch/main/graph/badge.svg)](https://codecov.io/gh/stac-utils/pystac-client)
 
 A Python client for working with [STAC](https://stacspec.org/) Catalogs and APIs.
 
 ## Table of Contents
 
 - [Table of Contents](#table-of-contents)
```

### Comparing `pystac-client-0.7.0/README.md` & `pystac-client-0.7.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # STAC Client <!-- omit in toc -->
 
 [![CI](https://github.com/stac-utils/pystac-client/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/stac-utils/pystac-client/actions/workflows/continuous-integration.yml)
 [![Release](https://github.com/stac-utils/pystac-client/actions/workflows/release.yml/badge.svg)](https://github.com/stac-utils/pystac-client/actions/workflows/release.yml)
 [![PyPI version](https://badge.fury.io/py/pystac-client.svg)](https://badge.fury.io/py/pystac-client)
-[![Documentation](https://readthedocs.org/projects/pystac-client/badge/?version=latest)](https://pystac-client.readthedocs.io/en/latest/)
+[![Documentation](https://readthedocs.org/projects/pystac-client/badge/?version=stable)](https://pystac-client.readthedocs.io)
 [![codecov](https://codecov.io/gh/stac-utils/pystac-client/branch/main/graph/badge.svg)](https://codecov.io/gh/stac-utils/pystac-client)
 
 A Python client for working with [STAC](https://stacspec.org/) Catalogs and APIs.
 
 ## Table of Contents
 
 - [Table of Contents](#table-of-contents)
```

### Comparing `pystac-client-0.7.0/pyproject.toml` & `pystac-client-0.7.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/pystac_client/_utils.py` & `pystac-client-0.7.1/pystac_client/_utils.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/pystac_client/cli.py` & `pystac-client-0.7.1/pystac_client/cli.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/pystac_client/client.py` & `pystac-client-0.7.1/pystac_client/client.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/pystac_client/collection_client.py` & `pystac-client-0.7.1/pystac_client/collection_client.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/pystac_client/conformance.py` & `pystac-client-0.7.1/pystac_client/conformance.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/pystac_client/item_search.py` & `pystac-client-0.7.1/pystac_client/item_search.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/pystac_client/mixins.py` & `pystac-client-0.7.1/pystac_client/mixins.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/pystac_client/stac_api_io.py` & `pystac-client-0.7.1/pystac_client/stac_api_io.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,28 +22,27 @@
     identify_stac_object_type,
     merge_common_properties,
     migrate_to_latest,
 )
 from pystac.stac_io import DefaultStacIO
 from requests import Request, Session
 from requests.adapters import HTTPAdapter
-from typing_extensions import TypeAlias
 
 import pystac_client
 
 from .exceptions import APIError
 
 if TYPE_CHECKING:
     from pystac.catalog import Catalog as Catalog_Type
     from pystac.stac_object import STACObject as STACObject_Type
 
 logger = logging.getLogger(__name__)
 
 
-Timeout: TypeAlias = Union[float, Tuple[float, float], Tuple[float, None]]
+Timeout = Union[float, Tuple[float, float], Tuple[float, None]]
 
 
 class StacApiIO(DefaultStacIO):
     def __init__(
         self,
         headers: Optional[Dict[str, str]] = None,
         conformance: Optional[List[str]] = None,
```

### Comparing `pystac-client-0.7.0/pystac_client/warnings.py` & `pystac-client-0.7.1/pystac_client/warnings.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/pystac_client.egg-info/PKG-INFO` & `pystac-client-0.7.1/pystac_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pystac-client
-Version: 0.7.0
+Version: 0.7.1
 Summary: Python library for working with SpatioTemporal Asset Catalog (STAC) APIs.
 Author-email: Jon Duckworth <duckontheweb@gmail.com>, Matthew Hanson <matt.a.hanson@gmail.com>
 Maintainer-email: Pete Gadomski <pete.gadomski@gmail.com>
 License: Apache-2.0
 Project-URL: homepage, https://github.com/stac-utils/pystac-client
 Project-URL: documentation, https://pystac-client.readthedocs.io
 Project-URL: repository, https://github.com/stac-utils/pystac-client.git
@@ -32,15 +32,15 @@
 License-File: LICENSE
 
 # STAC Client <!-- omit in toc -->
 
 [![CI](https://github.com/stac-utils/pystac-client/actions/workflows/continuous-integration.yml/badge.svg)](https://github.com/stac-utils/pystac-client/actions/workflows/continuous-integration.yml)
 [![Release](https://github.com/stac-utils/pystac-client/actions/workflows/release.yml/badge.svg)](https://github.com/stac-utils/pystac-client/actions/workflows/release.yml)
 [![PyPI version](https://badge.fury.io/py/pystac-client.svg)](https://badge.fury.io/py/pystac-client)
-[![Documentation](https://readthedocs.org/projects/pystac-client/badge/?version=latest)](https://pystac-client.readthedocs.io/en/latest/)
+[![Documentation](https://readthedocs.org/projects/pystac-client/badge/?version=stable)](https://pystac-client.readthedocs.io)
 [![codecov](https://codecov.io/gh/stac-utils/pystac-client/branch/main/graph/badge.svg)](https://codecov.io/gh/stac-utils/pystac-client)
 
 A Python client for working with [STAC](https://stacspec.org/) Catalogs and APIs.
 
 ## Table of Contents
 
 - [Table of Contents](#table-of-contents)
```

### Comparing `pystac-client-0.7.0/pystac_client.egg-info/SOURCES.txt` & `pystac-client-0.7.1/pystac_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/pystac_client.egg-info/requires.txt` & `pystac-client-0.7.1/pystac_client.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/tests/test_cli.py` & `pystac-client-0.7.1/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/tests/test_client.py` & `pystac-client-0.7.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/tests/test_collection_client.py` & `pystac-client-0.7.1/tests/test_collection_client.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/tests/test_item_search.py` & `pystac-client-0.7.1/tests/test_item_search.py`

 * *Files identical despite different names*

### Comparing `pystac-client-0.7.0/tests/test_stac_api_io.py` & `pystac-client-0.7.1/tests/test_stac_api_io.py`

 * *Files identical despite different names*

