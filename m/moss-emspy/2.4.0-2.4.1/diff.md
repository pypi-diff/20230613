# Comparing `tmp/moss_emspy-2.4.0.tar.gz` & `tmp/moss_emspy-2.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moss_emspy-2.4.0.tar", max compression
+gzip compressed data, was "moss_emspy-2.4.1.tar", max compression
```

## Comparing `moss_emspy-2.4.0.tar` & `moss_emspy-2.4.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1115 2022-09-26 08:21:52.814978 moss_emspy-2.4.0/LICENSE
--rw-r--r--   0        0        0     1230 2022-09-26 08:21:52.814978 moss_emspy-2.4.0/moss/__init__.py
--rw-r--r--   0        0        0     1185 2023-04-16 10:30:37.279604 moss_emspy-2.4.0/moss/ems/__init__.py
--rw-r--r--   0        0        0     7137 2023-04-16 09:51:00.208561 moss_emspy-2.4.0/moss/ems/emscatalog.py
--rw-r--r--   0        0        0    25703 2023-04-03 13:08:26.488973 moss_emspy-2.4.0/moss/ems/emslayer.py
--rw-r--r--   0        0        0    16243 2023-04-03 13:08:15.673554 moss_emspy-2.4.0/moss/ems/emsobjectclass.py
--rw-r--r--   0        0        0    16725 2022-10-05 12:06:00.147216 moss_emspy-2.4.0/moss/ems/emsproject.py
--rw-r--r--   0        0        0     8662 2022-09-26 08:21:52.818977 moss_emspy-2.4.0/moss/ems/emsqueryresult.py
--rw-r--r--   0        0        0    18452 2023-04-03 13:08:26.489982 moss_emspy-2.4.0/moss/ems/emsservice.py
--rw-r--r--   0        0        0        0 2022-02-12 20:31:35.158789 moss_emspy-2.4.0/moss/ems/extra/__init__.py
--rw-r--r--   0        0        0     4664 2022-09-26 08:21:52.818977 moss_emspy-2.4.0/moss/ems/extra/geometry_converter.py
--rw-r--r--   0        0        0     4654 2022-09-26 08:21:52.819977 moss_emspy-2.4.0/moss/ems/extra/query_objectclass_layers.py
--rw-r--r--   0        0        0        0 2021-11-05 12:24:09.717673 moss_emspy-2.4.0/moss/ems/scripts/__init__.py
--rw-r--r--   0        0        0     9739 2022-10-22 20:31:19.779053 moss_emspy-2.4.0/moss/ems/scripts/ems_cli_compare.py
--rw-r--r--   0        0        0    11611 2023-04-03 13:08:26.490972 moss_emspy-2.4.0/moss/ems/scripts/ems_cli_dump.py
--rw-r--r--   0        0        0     8052 2022-09-29 13:01:45.822424 moss_emspy-2.4.0/moss/ems/scripts/ems_cli_export.py
--rw-r--r--   0        0        0    31992 2022-09-29 13:16:34.765919 moss_emspy-2.4.0/moss/ems/scripts/ems_cli_import.py
--rw-r--r--   0        0        0     6753 2023-04-03 13:08:26.491972 moss_emspy-2.4.0/moss/ems/scripts/ems_cli_load.py
--rw-r--r--   0        0        0    14800 2023-04-03 13:08:26.493972 moss_emspy-2.4.0/moss/ems/scripts/moss_emscli.py
--rw-r--r--   0        0        0        0 2021-11-05 12:24:09.720686 moss_emspy-2.4.0/moss/ems/scripts/utilities/__init__.py
--rw-r--r--   0        0        0     2713 2021-11-05 12:24:09.721674 moss_emspy-2.4.0/moss/ems/scripts/utilities/promptutil.py
--rw-r--r--   0        0        0     1256 2022-09-26 08:21:52.818977 moss_emspy-2.4.0/moss/ems/utilities/__init__.py
--rw-r--r--   0        0        0     6637 2022-09-26 08:21:52.818977 moss_emspy-2.4.0/moss/ems/utilities/pagination_query.py
--rw-r--r--   0        0        0     2437 2022-09-26 08:21:52.818977 moss_emspy-2.4.0/moss/ems/utilities/session_baseurl.py
--rw-r--r--   0        0        0     2106 2021-11-05 12:24:09.723724 moss_emspy-2.4.0/moss/ems/utilities/sortutil.py
--rw-r--r--   0        0        0     1903 2023-04-16 10:30:37.356567 moss_emspy-2.4.0/pyproject.toml
--rw-r--r--   0        0        0      433 2021-11-05 12:24:09.707673 moss_emspy-2.4.0/README.md
--rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 moss_emspy-2.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1115 2022-09-26 08:21:52.814978 moss_emspy-2.4.1/LICENSE
+-rw-r--r--   0        0        0     1230 2022-09-26 08:21:52.814978 moss_emspy-2.4.1/moss/__init__.py
+-rw-r--r--   0        0        0     1185 2023-06-13 07:10:45.414277 moss_emspy-2.4.1/moss/ems/__init__.py
+-rw-r--r--   0        0        0     7137 2023-04-17 19:02:57.899662 moss_emspy-2.4.1/moss/ems/emscatalog.py
+-rw-r--r--   0        0        0    25703 2023-04-03 13:08:26.488973 moss_emspy-2.4.1/moss/ems/emslayer.py
+-rw-r--r--   0        0        0    16243 2023-04-03 13:08:15.673554 moss_emspy-2.4.1/moss/ems/emsobjectclass.py
+-rw-r--r--   0        0        0    16725 2022-10-05 12:06:00.147216 moss_emspy-2.4.1/moss/ems/emsproject.py
+-rw-r--r--   0        0        0     8662 2022-09-26 08:21:52.818977 moss_emspy-2.4.1/moss/ems/emsqueryresult.py
+-rw-r--r--   0        0        0    18452 2023-04-03 13:08:26.489982 moss_emspy-2.4.1/moss/ems/emsservice.py
+-rw-r--r--   0        0        0        0 2022-02-12 20:31:35.158789 moss_emspy-2.4.1/moss/ems/extra/__init__.py
+-rw-r--r--   0        0        0     4664 2022-09-26 08:21:52.818977 moss_emspy-2.4.1/moss/ems/extra/geometry_converter.py
+-rw-r--r--   0        0        0     4654 2022-09-26 08:21:52.819977 moss_emspy-2.4.1/moss/ems/extra/query_objectclass_layers.py
+-rw-r--r--   0        0        0        0 2021-11-05 12:24:09.717673 moss_emspy-2.4.1/moss/ems/scripts/__init__.py
+-rw-r--r--   0        0        0     9739 2022-10-22 20:31:19.779053 moss_emspy-2.4.1/moss/ems/scripts/ems_cli_compare.py
+-rw-r--r--   0        0        0    11611 2023-04-03 13:08:26.490972 moss_emspy-2.4.1/moss/ems/scripts/ems_cli_dump.py
+-rw-r--r--   0        0        0     8052 2022-09-29 13:01:45.822424 moss_emspy-2.4.1/moss/ems/scripts/ems_cli_export.py
+-rw-r--r--   0        0        0    31992 2022-09-29 13:16:34.765919 moss_emspy-2.4.1/moss/ems/scripts/ems_cli_import.py
+-rw-r--r--   0        0        0     6753 2023-04-03 13:08:26.491972 moss_emspy-2.4.1/moss/ems/scripts/ems_cli_load.py
+-rw-r--r--   0        0        0    14800 2023-04-03 13:08:26.493972 moss_emspy-2.4.1/moss/ems/scripts/moss_emscli.py
+-rw-r--r--   0        0        0        0 2021-11-05 12:24:09.720686 moss_emspy-2.4.1/moss/ems/scripts/utilities/__init__.py
+-rw-r--r--   0        0        0     2713 2021-11-05 12:24:09.721674 moss_emspy-2.4.1/moss/ems/scripts/utilities/promptutil.py
+-rw-r--r--   0        0        0     1256 2022-09-26 08:21:52.818977 moss_emspy-2.4.1/moss/ems/utilities/__init__.py
+-rw-r--r--   0        0        0     6637 2022-09-26 08:21:52.818977 moss_emspy-2.4.1/moss/ems/utilities/pagination_query.py
+-rw-r--r--   0        0        0     2437 2022-09-26 08:21:52.818977 moss_emspy-2.4.1/moss/ems/utilities/session_baseurl.py
+-rw-r--r--   0        0        0     2106 2021-11-05 12:24:09.723724 moss_emspy-2.4.1/moss/ems/utilities/sortutil.py
+-rw-r--r--   0        0        0     1903 2023-06-13 07:10:45.460265 moss_emspy-2.4.1/pyproject.toml
+-rw-r--r--   0        0        0      433 2021-11-05 12:24:09.707673 moss_emspy-2.4.1/README.md
+-rw-r--r--   0        0        0     1559 1970-01-01 00:00:00.000000 moss_emspy-2.4.1/PKG-INFO
```

### Comparing `moss_emspy-2.4.0/LICENSE` & `moss_emspy-2.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/__init__.py` & `moss_emspy-2.4.1/moss/__init__.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/__init__.py` & `moss_emspy-2.4.1/moss/ems/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,8 +15,8 @@
 # THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS
 # OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 # FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL
 # THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 # LIABILITY, WHETHER IN AN ACTION OF CONTRACT,TORT OR OTHERWISE, ARISING FROM, OUT
 # OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
 #
-__version__ = "2.4.0"
+__version__ = "2.4.1"
```

### Comparing `moss_emspy-2.4.0/moss/ems/emscatalog.py` & `moss_emspy-2.4.1/moss/ems/emscatalog.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/emslayer.py` & `moss_emspy-2.4.1/moss/ems/emslayer.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/emsobjectclass.py` & `moss_emspy-2.4.1/moss/ems/emsobjectclass.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/emsproject.py` & `moss_emspy-2.4.1/moss/ems/emsproject.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/emsqueryresult.py` & `moss_emspy-2.4.1/moss/ems/emsqueryresult.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/emsservice.py` & `moss_emspy-2.4.1/moss/ems/emsservice.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/extra/geometry_converter.py` & `moss_emspy-2.4.1/moss/ems/extra/geometry_converter.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/extra/query_objectclass_layers.py` & `moss_emspy-2.4.1/moss/ems/extra/query_objectclass_layers.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/scripts/ems_cli_compare.py` & `moss_emspy-2.4.1/moss/ems/scripts/ems_cli_compare.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/scripts/ems_cli_dump.py` & `moss_emspy-2.4.1/moss/ems/scripts/ems_cli_dump.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/scripts/ems_cli_export.py` & `moss_emspy-2.4.1/moss/ems/scripts/ems_cli_export.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/scripts/ems_cli_import.py` & `moss_emspy-2.4.1/moss/ems/scripts/ems_cli_import.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/scripts/ems_cli_load.py` & `moss_emspy-2.4.1/moss/ems/scripts/ems_cli_load.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/scripts/moss_emscli.py` & `moss_emspy-2.4.1/moss/ems/scripts/moss_emscli.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/scripts/utilities/promptutil.py` & `moss_emspy-2.4.1/moss/ems/scripts/utilities/promptutil.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/utilities/__init__.py` & `moss_emspy-2.4.1/moss/ems/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/utilities/pagination_query.py` & `moss_emspy-2.4.1/moss/ems/utilities/pagination_query.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/utilities/session_baseurl.py` & `moss_emspy-2.4.1/moss/ems/utilities/session_baseurl.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/moss/ems/utilities/sortutil.py` & `moss_emspy-2.4.1/moss/ems/utilities/sortutil.py`

 * *Files identical despite different names*

### Comparing `moss_emspy-2.4.0/pyproject.toml` & `moss_emspy-2.4.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "moss_emspy"
-version = "2.4.0"
+version = "2.4.1"
 description = "Package to interact with MOSS WEGA-EMS"
 license = "MIT"
 authors = ["M.O.S.S.Computer Grafik Systeme GmbH <develop@moss.de>"]
 maintainers = ["M.O.S.S.Computer Grafik Systeme GmbH <develop@moss.de>"]
 homepage = "https://www.moss.de/"
 packages = [{ include = "moss" }]
 readme = "README.md"
@@ -16,15 +16,15 @@
     "Intended Audience :: Developers",
     "Environment :: Other Environment",
     "Topic :: Software Development :: Libraries :: Python Modules"
 ]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4"
-requests = "^2.28.0"
+requests = "^2.27.0"
 anytree = "2.8.0"
 tqdm = "4.64.0"
 
 [tool.poetry.dev-dependencies]
 black = "^22.6.0"
 isort = "^5.10.1"
 pytest = "^7.1.2"
@@ -59,14 +59,14 @@
 [tool.taskipy.tasks]
 new_release = "generate_release && push_tag"
 generate_release = "poetry run cz bump --changelog"
 push_tag = "git push --tags"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "2.4.0"
+version = "2.4.1"
 tag_format = "$version"
 version_files = [
     "moss/ems/__init__.py",
     "pyproject.toml:version"
 ]
 changelog_file = "CHANGELOG.md"
```

### Comparing `moss_emspy-2.4.0/PKG-INFO` & `moss_emspy-2.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moss-emspy
-Version: 2.4.0
+Version: 2.4.1
 Summary: Package to interact with MOSS WEGA-EMS
 Home-page: https://www.moss.de/
 License: MIT
 Keywords: wegaems
 Author: M.O.S.S.Computer Grafik Systeme GmbH
 Author-email: develop@moss.de
 Maintainer: M.O.S.S.Computer Grafik Systeme GmbH
@@ -20,15 +20,15 @@
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: anytree (==2.8.0)
-Requires-Dist: requests (>=2.28.0,<3.0.0)
+Requires-Dist: requests (>=2.27.0,<3.0.0)
 Requires-Dist: tqdm (==4.64.0)
 Description-Content-Type: text/markdown
 
 # MOSS emspy
 
 ## Description
```

