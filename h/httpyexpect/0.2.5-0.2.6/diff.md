# Comparing `tmp/httpyexpect-0.2.5.tar.gz` & `tmp/httpyexpect-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "httpyexpect-0.2.5.tar", last modified: Wed May 24 07:46:44 2023, max compression
+gzip compressed data, was "httpyexpect-0.2.6.tar", last modified: Tue Jun 13 11:06:33 2023, max compression
```

## Comparing `httpyexpect-0.2.5.tar` & `httpyexpect-0.2.6.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.359299 httpyexpect-0.2.5/httpyexpect/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/base_exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/httpyexpect/client/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/client/custom_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/client/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/client/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/client/translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/httpyexpect/server/
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/server/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/httpyexpect/server/handlers/
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/server/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/server/handlers/fastapi_.py
--rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/httpyexpect/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.359299 httpyexpect-0.2.5/httpyexpect.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-05-24 07:46:44.000000 httpyexpect-0.2.5/httpyexpect.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-05-24 07:46:44.000000 httpyexpect-0.2.5/httpyexpect.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:46:44.000000 httpyexpect-0.2.5/httpyexpect.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-24 07:46:44.000000 httpyexpect-0.2.5/httpyexpect.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-24 07:46:44.000000 httpyexpect-0.2.5/httpyexpect.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-24 07:46:44.000000 httpyexpect-0.2.5/httpyexpect.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-24 07:46:44.367299 httpyexpect-0.2.5/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.355299 httpyexpect-0.2.5/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      750 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/fixtures/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (123)      729 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/integration/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/tests/integration/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/integration/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/integration/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/integration/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/integration/test_fastapi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (123)      722 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-24 07:46:44.363299 httpyexpect-0.2.5/tests/unit/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/fixtures/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/fixtures/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/test_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/test_server_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/test_translator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-05-24 07:46:31.000000 httpyexpect-0.2.5/tests/unit/test_validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11452 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3107 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.911759 httpyexpect-0.2.6/httpyexpect/
+-rw-r--r--   0 runner    (1001) docker     (123)      791 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/base_exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.911759 httpyexpect-0.2.6/httpyexpect/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/client/custom_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3457 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/client/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9293 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/client/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/client/translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/httpyexpect/server/
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6011 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/server/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/httpyexpect/server/handlers/
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/server/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/server/handlers/fastapi_.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/httpyexpect/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.911759 httpyexpect-0.2.6/httpyexpect.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3781 2023-06-13 11:06:33.000000 httpyexpect-0.2.6/httpyexpect.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-06-13 11:06:33.000000 httpyexpect-0.2.6/httpyexpect.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:06:33.000000 httpyexpect-0.2.6/httpyexpect.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:06:33.000000 httpyexpect-0.2.6/httpyexpect.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-06-13 11:06:33.000000 httpyexpect-0.2.6/httpyexpect.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-06-13 11:06:33.000000 httpyexpect-0.2.6/httpyexpect.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      865 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.911759 httpyexpect-0.2.6/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      750 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/fixtures/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (123)      729 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/integration/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/tests/integration/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/integration/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/integration/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/integration/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/integration/test_fastapi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:06:33.915758 httpyexpect-0.2.6/tests/unit/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/fixtures/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/fixtures/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8382 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/test_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1986 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5468 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/test_server_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6005 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/test_translator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2338 2023-06-13 11:06:24.000000 httpyexpect-0.2.6/tests/unit/test_validation.py
```

### Comparing `httpyexpect-0.2.5/LICENSE` & `httpyexpect-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/PKG-INFO` & `httpyexpect-0.2.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpyexpect
-Version: 0.2.5
+Version: 0.2.6
 Summary: An opinionated way to translate server side HTTP errors to the client side.
 Home-page: https://github.com/ghga-de/httpyexpect
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `httpyexpect-0.2.5/README.md` & `httpyexpect-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/httpyexpect/__init__.py` & `httpyexpect-0.2.6/httpyexpect/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,8 +11,8 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """An opinionated way to translate server side HTTP errors to the client side."""
 
-__version__ = "0.2.5"
+__version__ = "0.2.6"
```

### Comparing `httpyexpect-0.2.5/httpyexpect/base_exception.py` & `httpyexpect-0.2.6/httpyexpect/base_exception.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/httpyexpect/client/__init__.py` & `httpyexpect-0.2.6/httpyexpect/client/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/httpyexpect/client/custom_types.py` & `httpyexpect-0.2.6/httpyexpect/client/custom_types.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/httpyexpect/client/exceptions.py` & `httpyexpect-0.2.6/httpyexpect/client/exceptions.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/httpyexpect/client/mapping.py` & `httpyexpect-0.2.6/httpyexpect/client/mapping.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/httpyexpect/client/translator.py` & `httpyexpect-0.2.6/httpyexpect/client/translator.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/httpyexpect/models.py` & `httpyexpect-0.2.6/httpyexpect/models.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/httpyexpect/server/__init__.py` & `httpyexpect-0.2.6/httpyexpect/server/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/httpyexpect/server/exceptions.py` & `httpyexpect-0.2.6/httpyexpect/server/exceptions.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/httpyexpect/server/handlers/__init__.py` & `httpyexpect-0.2.6/httpyexpect/server/handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/httpyexpect/server/handlers/fastapi_.py` & `httpyexpect-0.2.6/httpyexpect/server/handlers/fastapi_.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/httpyexpect/validation.py` & `httpyexpect-0.2.6/httpyexpect/validation.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/httpyexpect.egg-info/PKG-INFO` & `httpyexpect-0.2.6/httpyexpect.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: httpyexpect
-Version: 0.2.5
+Version: 0.2.6
 Summary: An opinionated way to translate server side HTTP errors to the client side.
 Home-page: https://github.com/ghga-de/httpyexpect
 Author: German Human Genome Phenome Archive (GHGA)
 Author-email: contact@ghga.de
 License: Apache 2.0
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `httpyexpect-0.2.5/httpyexpect.egg-info/SOURCES.txt` & `httpyexpect-0.2.6/httpyexpect.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/setup.cfg` & `httpyexpect-0.2.6/setup.cfg`

 * *Files 13% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 python_requires = >= 3.9
 
 [options.package_data]
 * = *.yaml, *.json, *.html
 
 [options.extras_require]
 fastapi = 
-	fastapi>=0.79.0,<0.89.0
+	fastapi>=0.96.0
 dev = 
 	datamodel-code-generator==0.19.0
 all = 
 	%(fastapi)s
 	%(dev)s
 
 [options.packages.find]
```

### Comparing `httpyexpect-0.2.5/setup.py` & `httpyexpect-0.2.6/setup.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/fixtures/__init__.py` & `httpyexpect-0.2.6/tests/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/fixtures/utils.py` & `httpyexpect-0.2.6/tests/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/integration/__init__.py` & `httpyexpect-0.2.6/tests/integration/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/integration/fixtures/__init__.py` & `httpyexpect-0.2.6/tests/integration/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/integration/fixtures/utils.py` & `httpyexpect-0.2.6/tests/integration/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/integration/test_client.py` & `httpyexpect-0.2.6/tests/integration/test_client.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/integration/test_fastapi.py` & `httpyexpect-0.2.6/tests/integration/test_fastapi.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/unit/__init__.py` & `httpyexpect-0.2.6/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/unit/fixtures/__init__.py` & `httpyexpect-0.2.6/tests/unit/fixtures/__init__.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/unit/fixtures/utils.py` & `httpyexpect-0.2.6/tests/unit/fixtures/utils.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/unit/test_mapping.py` & `httpyexpect-0.2.6/tests/unit/test_mapping.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/unit/test_models.py` & `httpyexpect-0.2.6/tests/unit/test_models.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/unit/test_server_exceptions.py` & `httpyexpect-0.2.6/tests/unit/test_server_exceptions.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/unit/test_translator.py` & `httpyexpect-0.2.6/tests/unit/test_translator.py`

 * *Files identical despite different names*

### Comparing `httpyexpect-0.2.5/tests/unit/test_validation.py` & `httpyexpect-0.2.6/tests/unit/test_validation.py`

 * *Files identical despite different names*

