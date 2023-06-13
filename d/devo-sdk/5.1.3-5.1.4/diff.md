# Comparing `tmp/devo-sdk-5.1.3.tar.gz` & `tmp/devo-sdk-5.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "devo-sdk-5.1.3.tar", last modified: Thu Mar 23 14:34:09 2023, max compression
+gzip compressed data, was "devo-sdk-5.1.4.tar", last modified: Tue Jun 13 13:57:08 2023, max compression
```

## Comparing `devo-sdk-5.1.3.tar` & `devo-sdk-5.1.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:34:09.880695 devo-sdk-5.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1076 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-03-23 14:34:09.880695 devo-sdk-5.1.3/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     7895 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:34:09.876695 devo-sdk-5.1.3/devo/
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:34:09.876695 devo-sdk-5.1.3/devo/api/
--rw-r--r--   0 runner    (1001) docker     (123)      216 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    36635 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/api/processors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:34:09.876695 devo-sdk-5.1.3/devo/api/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/api/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/api/scripts/client_cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:34:09.876695 devo-sdk-5.1.3/devo/common/
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/common/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:34:09.876695 devo-sdk-5.1.3/devo/common/dates/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/common/dates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/common/dates/dateoperations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/common/dates/dateparser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/common/dates/dateutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:34:09.876695 devo-sdk-5.1.3/devo/common/generic/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/common/generic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/common/generic/configuration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:34:09.876695 devo-sdk-5.1.3/devo/common/loadenv/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/common/loadenv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/common/loadenv/load_env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:34:09.876695 devo-sdk-5.1.3/devo/common/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/common/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/common/logging/log.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:34:09.880695 devo-sdk-5.1.3/devo/sender/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/sender/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    38587 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/sender/data.py
--rw-r--r--   0 runner    (1001) docker     (123)    15439 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/sender/lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/sender/pfx_to_pem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:34:09.880695 devo-sdk-5.1.3/devo/sender/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/sender/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12503 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/sender/scripts/sender_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/devo/sender/transformsyslog.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:34:09.880695 devo-sdk-5.1.3/devo_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9459 2023-03-23 14:34:09.000000 devo-sdk-5.1.3/devo_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-03-23 14:34:09.000000 devo-sdk-5.1.3/devo_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:34:09.000000 devo-sdk-5.1.3/devo_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-03-23 14:34:09.000000 devo-sdk-5.1.3/devo_sdk.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-23 14:34:09.000000 devo-sdk-5.1.3/devo_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-23 14:34:09.000000 devo-sdk-5.1.3/devo_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-03-23 14:34:09.880695 devo-sdk-5.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2816 2023-03-23 14:34:00.000000 devo-sdk-5.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:08.180135 devo-sdk-5.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-06-13 13:57:08.180135 devo-sdk-5.1.4/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7856 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:08.176135 devo-sdk-5.1.4/devo/
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:08.176135 devo-sdk-5.1.4/devo/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      216 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36635 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2732 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/api/processors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:08.176135 devo-sdk-5.1.4/devo/api/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/api/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6687 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/api/scripts/client_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:08.176135 devo-sdk-5.1.4/devo/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/common/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:08.176135 devo-sdk-5.1.4/devo/common/dates/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/common/dates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1816 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/common/dates/dateoperations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2552 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/common/dates/dateparser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1260 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/common/dates/dateutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:08.176135 devo-sdk-5.1.4/devo/common/generic/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/common/generic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7406 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/common/generic/configuration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:08.176135 devo-sdk-5.1.4/devo/common/loadenv/
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/common/loadenv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/common/loadenv/load_env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:08.176135 devo-sdk-5.1.4/devo/common/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/common/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/common/logging/log.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:08.176135 devo-sdk-5.1.4/devo/sender/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/sender/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38587 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/sender/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15439 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/sender/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1309 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/sender/pfx_to_pem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:08.176135 devo-sdk-5.1.4/devo/sender/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/sender/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12524 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/sender/scripts/sender_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2874 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/devo/sender/transformsyslog.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 13:57:08.180135 devo-sdk-5.1.4/devo_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9420 2023-06-13 13:57:08.000000 devo-sdk-5.1.4/devo_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-13 13:57:08.000000 devo-sdk-5.1.4/devo_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 13:57:08.000000 devo-sdk-5.1.4/devo_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-06-13 13:57:08.000000 devo-sdk-5.1.4/devo_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-06-13 13:57:08.000000 devo-sdk-5.1.4/devo_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-06-13 13:57:08.000000 devo-sdk-5.1.4/devo_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-06-13 13:57:08.180135 devo-sdk-5.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2814 2023-06-13 13:56:56.000000 devo-sdk-5.1.4/setup.py
```

### Comparing `devo-sdk-5.1.3/LICENSE` & `devo-sdk-5.1.4/LICENSE`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
 IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
 FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
 AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
 LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
 OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+SOFTWARE.
```

### Comparing `devo-sdk-5.1.3/PKG-INFO` & `devo-sdk-5.1.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devo-sdk
-Version: 5.1.3
+Version: 5.1.4
 Summary: Devo Software Development Kit for Python.
 Home-page: https://github.com/DevoInc/python-sdk
 Author: Devo, Inc.
 Author-email: support@devo.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,142 +22,156 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![License](https://img.shields.io/github/license/DevoInc/python-sdk)
 ![Wheel](https://img.shields.io/pypi/wheel/devo-sdk)
 ![Version](https://img.shields.io/pypi/v/devo-sdk)
-![Python](https://img.shields.io/pypi/pyversions/devo-sdk) 
+![Python](https://img.shields.io/pypi/pyversions/devo-sdk)
 ![Tests](https://github.com/DevoInc/python-sdk/actions/workflows/python-pull-request.yml/badge.svg)
 
 # Devo Python SDK
 
 This is the SDK to access Devo directly from Python. It can be used to:
+
 * Send events and files to Devo.
 * Make queries.
 * Manage deferred tasks.
 
 ## Requirements
 
 The Devo SDK for Python requires Python 3.7+
 
-## Compatibility 
+## Compatibility
+
 - Tested compatibility for python 3.7, 3.8 and 3.9
 
 ## Quick Start
-### Installing the SDK
 
+### Installing the SDK
 
 You can install the Devo SDK by using `easy_install` or `pip`:
 
-    #option 1
-    easy_install devo-sdk
-    
-    #option 2
-    pip install devo-sdk
+```console
+#option 1
+easy_install devo-sdk
 
+#option 2
+pip install devo-sdk
+```
 
 You can use sources files, cloning the project too:
 
-    #option 3
-    python setup.py install
-    
-    #option 4
-    pip install .
-    
-    #option 5 - dev option
-    pip install -e .
+```console
+#option 3
+python setup.py install
+
+#option 4
+pip install .
+
+#option 5 - dev option
+pip install -e .
+```
 
 ### Documentation
 
 There is specific documentation in the _[docs](https://github.com/DevoInc/python-sdk/tree/master/docs)_ folder for each part of SDK:
+
 * [Sender](https://github.com/DevoInc/python-sdk/tree/master/docs/sender/sender.md)
-    * [Data](https://github.com/DevoInc/python-sdk/tree/master/docs/sender/data.md)
-    * [Lookups](https://github.com/DevoInc/python-sdk/tree/master/docs/sender/lookup.md)
+  * [Data](https://github.com/DevoInc/python-sdk/tree/master/docs/sender/data.md)
+  * [Lookups](https://github.com/DevoInc/python-sdk/tree/master/docs/sender/lookup.md)
 * [Common](https://github.com/DevoInc/python-sdk/tree/master/docs/common.md)
 * API:
-    * [Api query](https://github.com/DevoInc/python-sdk/tree/master/docs/api/api.md)
-    * [Api tasks management](https://github.com/DevoInc/python-sdk/tree/master/docs/api/task.md)
-        * [Destination: email](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_email.md)
-        * [Destination: redis](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_redis.md)
-        * [Destination: S3](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_s3.md)
-
+  * [Api query](https://github.com/DevoInc/python-sdk/tree/master/docs/api/api.md)
+  * [Api tasks management](https://github.com/DevoInc/python-sdk/tree/master/docs/api/task.md)
+    * [Destination: email](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_email.md)
+    * [Destination: redis](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_redis.md)
+    * [Destination: S3](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_s3.md)
 
 ## Contributing
+
 See [PyLibs contributing guide](https://github.com/DevoInc/python-sdk/tree/master/CONTRIBUTING.md).<br/>
 Pull and merge requests are welcome ☺
 
 ## Endpoints
-##### Sender
+
+### Sender
+
 To send data with Devo SDK, first choose the required endpoint depending on the region your are accessing from:
 
 | Region | Endpoint             | Port |
 |--------|----------------------|------|
 | USA    | collector-us.devo.io | 443  |
 | Canada | collector-ca.devo.io | 443  |
 | Europe | collector-eu.devo.io | 443  |
 | APAC   | collector-ap.devo.io | 443  |
 
 You have more information in the official documentation of Devo, [Sending data to Devo](https://docs.devo.com/space/latest/94652410/Sending%20data%20to%20Devo).
 
-##### API
+### API
+
 To perform a request with API, first choose the required endpoint depending on the region your are accessing from:
 
 | Region | Endpoint                               |
 |--------|----------------------------------------|
-| USA    | https://apiv2-us.devo.com/search/query |
-| Canada | https://apiv2-ca.devo.com/search/query |
-| Europe | https://apiv2-eu.devo.com/search/query |
-| APAC   | https://api-apac.devo.com/search/query |
+| USA    | <https://apiv2-us.devo.com/search/query> |
+| Canada | <https://apiv2-ca.devo.com/search/query> |
+| Europe | <https://apiv2-eu.devo.com/search/query> |
+| APAC   | <https://api-apac.devo.com/search/query> |
 
 You have more information in the official documentation of Devo, [REST API](https://docs.devo.com/space/latest/95128275/Query%20API).
 
 ## Credentials
+
 To obtain the access credentials necessary to use this SDK, you must have an account in [DEVO](https://www.devo.com/).<br/>
-Check the [security credentials](https://docs.devo.com/space/latest/94763701/Security%20credentials) info for more details. 
+Check the [security credentials](https://docs.devo.com/space/latest/94763701/Security%20credentials) info for more details.
+
+### Certificates
+
+You need use a three files (Cert, key and chain) to secure send data to Devo.
+Administrator users can find them in **Administration** → **Credentials**, in the X.509 tab.
+
+### API authorization
 
-##### Certificates
-You need use a three files (Cert, key and chain) to secure send data to Devo. 
-Administrator users can find them in **Administration** → **Credentials**, in the X.509 tab. 
-
-##### API authorization
-You can use a domain API key and API secret to sign the request. These are are a pair of credentials that every 
-Devo account owns. Administrator users can find them in **Administration** → **Credentials**, in the Access Keys tab. 
+You can use a domain API key and API secret to sign the request. These are are a pair of credentials that every
+Devo account owns. Administrator users can find them in **Administration** → **Credentials**, in the Access Keys tab.
 
 ## Launch tests
+
 ### run_tests script
+
 You can run tests from the main folder of SDK
 To launch this script, you need either the environment variables loaded in the system, or the _environment.env_ file in the root of the SDK with the correct values, since to test all the SDK functionalities it is necessary to connect to Devo for the tests of sending and extracting data. There is an example file called _environment.env.example_
 
 Its normal, by the way, TCP tests fails in clients or not Devo developers systems.
 
 ```console
-~/projects/devo-python-sdk > python setup.py test 
+~/projects/devo-python-sdk > python setup.py test
 ```
 
 ```console
 ~/projects/devo-python-sdk > python run_tests.py
 ```
 
 You can add option "Coverage" for create HTML report about tests.
 
-```console
+```text
 ~/projects/devo-python-sdk > python run_tests.py --coverage
 ```
 
 You can also run the test for just one module. This is a useful feature if you are developing functionality in just one module.
 
 ```console
-~/projects/devo-python-sdk > python run_tests.py -m SEND_CLI
+~/projects/devo-python-sdk > python run_tests.py -m SENDER_CLI
 ```
 
 You can also exclude one or several tests with `-M` parameter:
 
 ```console
-~/projects/devo-python-sdk > python run_tests.py -M SEND_CLI,API_CLI
+~/projects/devo-python-sdk > python run_tests.py -M SENDER_CLI,API_CLI
 ```
 
 Using the --help flag prints the available modules to use:
 
 ```console
 ~/projects/devo-python-sdk > python run_tests.py --help
 usage: run_tests.py [-h] [--coverage [COVERAGE]] [-m [MODULE]]
@@ -193,28 +207,28 @@
 
 ### Run using Unittest command
 
 You can see references in [unittest documentation](https://docs.python.org/3/library/unittest.html)
 
 For commands like:
 
-```bash
-python -m unittest discover -p "*.py" 
+```console
+python -m unittest discover -p "*.py"
 ```
 
-If you launch this command from the root directory of the SDK, you need to have the environment variables in your 
-system for all the tests that require connection to Devo can work, not being able to use the environment.env file 
+If you launch this command from the root directory of the SDK, you need to have the environment variables in your
+system for all the tests that require connection to Devo can work, not being able to use the environment.env file
 as in the script.
 
-
 ### Contact Us
 
 You can contact with us at _support@devo.com_.
 
 ## License
+
 MIT License
 
 (C) 2022 Devo, Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the 'Software'), to deal in
 the Software without restriction, including without limitation the rights to
```

### Comparing `devo-sdk-5.1.3/README.md` & `devo-sdk-5.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,138 +1,152 @@
 ![License](https://img.shields.io/github/license/DevoInc/python-sdk)
 ![Wheel](https://img.shields.io/pypi/wheel/devo-sdk)
 ![Version](https://img.shields.io/pypi/v/devo-sdk)
-![Python](https://img.shields.io/pypi/pyversions/devo-sdk) 
+![Python](https://img.shields.io/pypi/pyversions/devo-sdk)
 ![Tests](https://github.com/DevoInc/python-sdk/actions/workflows/python-pull-request.yml/badge.svg)
 
 # Devo Python SDK
 
 This is the SDK to access Devo directly from Python. It can be used to:
+
 * Send events and files to Devo.
 * Make queries.
 * Manage deferred tasks.
 
 ## Requirements
 
 The Devo SDK for Python requires Python 3.7+
 
-## Compatibility 
+## Compatibility
+
 - Tested compatibility for python 3.7, 3.8 and 3.9
 
 ## Quick Start
-### Installing the SDK
 
+### Installing the SDK
 
 You can install the Devo SDK by using `easy_install` or `pip`:
 
-    #option 1
-    easy_install devo-sdk
-    
-    #option 2
-    pip install devo-sdk
+```console
+#option 1
+easy_install devo-sdk
 
+#option 2
+pip install devo-sdk
+```
 
 You can use sources files, cloning the project too:
 
-    #option 3
-    python setup.py install
-    
-    #option 4
-    pip install .
-    
-    #option 5 - dev option
-    pip install -e .
+```console
+#option 3
+python setup.py install
+
+#option 4
+pip install .
+
+#option 5 - dev option
+pip install -e .
+```
 
 ### Documentation
 
 There is specific documentation in the _[docs](docs)_ folder for each part of SDK:
+
 * [Sender](docs/sender/sender.md)
-    * [Data](docs/sender/data.md)
-    * [Lookups](docs/sender/lookup.md)
+  * [Data](docs/sender/data.md)
+  * [Lookups](docs/sender/lookup.md)
 * [Common](docs/common.md)
 * API:
-    * [Api query](docs/api/api.md)
-    * [Api tasks management](docs/api/task.md)
-        * [Destination: email](docs/api/destination_email.md)
-        * [Destination: redis](docs/api/destination_redis.md)
-        * [Destination: S3](docs/api/destination_s3.md)
-
+  * [Api query](docs/api/api.md)
+  * [Api tasks management](docs/api/task.md)
+    * [Destination: email](docs/api/destination_email.md)
+    * [Destination: redis](docs/api/destination_redis.md)
+    * [Destination: S3](docs/api/destination_s3.md)
 
 ## Contributing
+
 See [PyLibs contributing guide](CONTRIBUTING.md).<br/>
 Pull and merge requests are welcome ☺
 
 ## Endpoints
-##### Sender
+
+### Sender
+
 To send data with Devo SDK, first choose the required endpoint depending on the region your are accessing from:
 
 | Region | Endpoint             | Port |
 |--------|----------------------|------|
 | USA    | collector-us.devo.io | 443  |
 | Canada | collector-ca.devo.io | 443  |
 | Europe | collector-eu.devo.io | 443  |
 | APAC   | collector-ap.devo.io | 443  |
 
 You have more information in the official documentation of Devo, [Sending data to Devo](https://docs.devo.com/space/latest/94652410/Sending%20data%20to%20Devo).
 
-##### API
+### API
+
 To perform a request with API, first choose the required endpoint depending on the region your are accessing from:
 
 | Region | Endpoint                               |
 |--------|----------------------------------------|
-| USA    | https://apiv2-us.devo.com/search/query |
-| Canada | https://apiv2-ca.devo.com/search/query |
-| Europe | https://apiv2-eu.devo.com/search/query |
-| APAC   | https://api-apac.devo.com/search/query |
+| USA    | <https://apiv2-us.devo.com/search/query> |
+| Canada | <https://apiv2-ca.devo.com/search/query> |
+| Europe | <https://apiv2-eu.devo.com/search/query> |
+| APAC   | <https://api-apac.devo.com/search/query> |
 
 You have more information in the official documentation of Devo, [REST API](https://docs.devo.com/space/latest/95128275/Query%20API).
 
 ## Credentials
+
 To obtain the access credentials necessary to use this SDK, you must have an account in [DEVO](https://www.devo.com/).<br/>
-Check the [security credentials](https://docs.devo.com/space/latest/94763701/Security%20credentials) info for more details. 
+Check the [security credentials](https://docs.devo.com/space/latest/94763701/Security%20credentials) info for more details.
+
+### Certificates
+
+You need use a three files (Cert, key and chain) to secure send data to Devo.
+Administrator users can find them in **Administration** → **Credentials**, in the X.509 tab.
+
+### API authorization
 
-##### Certificates
-You need use a three files (Cert, key and chain) to secure send data to Devo. 
-Administrator users can find them in **Administration** → **Credentials**, in the X.509 tab. 
-
-##### API authorization
-You can use a domain API key and API secret to sign the request. These are are a pair of credentials that every 
-Devo account owns. Administrator users can find them in **Administration** → **Credentials**, in the Access Keys tab. 
+You can use a domain API key and API secret to sign the request. These are are a pair of credentials that every
+Devo account owns. Administrator users can find them in **Administration** → **Credentials**, in the Access Keys tab.
 
 ## Launch tests
+
 ### run_tests script
+
 You can run tests from the main folder of SDK
 To launch this script, you need either the environment variables loaded in the system, or the _environment.env_ file in the root of the SDK with the correct values, since to test all the SDK functionalities it is necessary to connect to Devo for the tests of sending and extracting data. There is an example file called _environment.env.example_
 
 Its normal, by the way, TCP tests fails in clients or not Devo developers systems.
 
 ```console
-~/projects/devo-python-sdk > python setup.py test 
+~/projects/devo-python-sdk > python setup.py test
 ```
 
 ```console
 ~/projects/devo-python-sdk > python run_tests.py
 ```
 
 You can add option "Coverage" for create HTML report about tests.
 
-```console
+```text
 ~/projects/devo-python-sdk > python run_tests.py --coverage
 ```
 
 You can also run the test for just one module. This is a useful feature if you are developing functionality in just one module.
 
 ```console
-~/projects/devo-python-sdk > python run_tests.py -m SEND_CLI
+~/projects/devo-python-sdk > python run_tests.py -m SENDER_CLI
 ```
 
 You can also exclude one or several tests with `-M` parameter:
 
 ```console
-~/projects/devo-python-sdk > python run_tests.py -M SEND_CLI,API_CLI
+~/projects/devo-python-sdk > python run_tests.py -M SENDER_CLI,API_CLI
 ```
 
 Using the --help flag prints the available modules to use:
 
 ```console
 ~/projects/devo-python-sdk > python run_tests.py --help
 usage: run_tests.py [-h] [--coverage [COVERAGE]] [-m [MODULE]]
@@ -168,28 +182,28 @@
 
 ### Run using Unittest command
 
 You can see references in [unittest documentation](https://docs.python.org/3/library/unittest.html)
 
 For commands like:
 
-```bash
-python -m unittest discover -p "*.py" 
+```console
+python -m unittest discover -p "*.py"
 ```
 
-If you launch this command from the root directory of the SDK, you need to have the environment variables in your 
-system for all the tests that require connection to Devo can work, not being able to use the environment.env file 
+If you launch this command from the root directory of the SDK, you need to have the environment variables in your
+system for all the tests that require connection to Devo can work, not being able to use the environment.env file
 as in the script.
 
-
 ### Contact Us
 
 You can contact with us at _support@devo.com_.
 
 ## License
+
 MIT License
 
 (C) 2022 Devo, Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the 'Software'), to deal in
 the Software without restriction, including without limitation the rights to
```

### Comparing `devo-sdk-5.1.3/devo/api/client.py` & `devo-sdk-5.1.4/devo/api/client.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/devo/api/processors.py` & `devo-sdk-5.1.4/devo/api/processors.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/devo/api/scripts/client_cli.py` & `devo-sdk-5.1.4/devo/api/scripts/client_cli.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/devo/common/__init__.py` & `devo-sdk-5.1.4/devo/common/__init__.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/devo/common/dates/dateoperations.py` & `devo-sdk-5.1.4/devo/common/dates/dateoperations.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/devo/common/dates/dateparser.py` & `devo-sdk-5.1.4/devo/common/dates/dateparser.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/devo/common/dates/dateutils.py` & `devo-sdk-5.1.4/devo/common/dates/dateutils.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/devo/common/generic/configuration.py` & `devo-sdk-5.1.4/devo/common/generic/configuration.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/devo/common/loadenv/load_env.py` & `devo-sdk-5.1.4/devo/common/loadenv/load_env.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/devo/common/logging/log.py` & `devo-sdk-5.1.4/devo/common/logging/log.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/devo/sender/data.py` & `devo-sdk-5.1.4/devo/sender/data.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/devo/sender/lookup.py` & `devo-sdk-5.1.4/devo/sender/lookup.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/devo/sender/pfx_to_pem.py` & `devo-sdk-5.1.4/devo/sender/pfx_to_pem.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/devo/sender/scripts/sender_cli.py` & `devo-sdk-5.1.4/devo/sender/scripts/sender_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     print(str(import_error), "- Use 'pip install click' or install this "
                              "package with [click] option")
     sys.exit(1)
 
 import os
 from devo.common import Configuration
 from devo.sender.lookup import Lookup
-from devo.sender.data import Sender, DevoSenderException
+from devo.sender.data import Sender, DevoSenderException, open_file
 from devo.__version__ import __version__
 # Groups
 # ------------------------------------------------------------------------------
 
 
 @click.group(invoke_without_command=True)
 @click.option('--version', "-v", is_flag=True, default=False)
@@ -97,26 +97,26 @@
 
         if config.get('file', False):
             if not Path(config['file']).is_file():
                 print_error(str("File '%s' does not found"
                                 % Path(config['file']).absolute()))
                 return
             if config['multiline']:
-                with open(config['file'], mode='r') as file:
+                with open_file(config['file'], mode='r') as file:
                     content = file.read()
                     if not config['raw']:
                         sended += con.send(tag=config['tag'], msg=content,
                                            multiline=config['multiline'],
                                            zip=config.get("zip", False))
                     else:
                         sended += con.send_raw(content,
                                                multiline=config['multiline'],
                                                zip=config.get("zip", False))
             else:
-                with open(config['file'], mode='r') as file:
+                with open_file(config['file'], mode='r') as file:
                     if config['header']:
                         next(file)
                     for line in file:
                         if config['raw']:
                             sended += con.send_raw(line)
                         else:
                             sended += con.send(tag=config['tag'], msg=line,
```

### Comparing `devo-sdk-5.1.3/devo/sender/transformsyslog.py` & `devo-sdk-5.1.4/devo/sender/transformsyslog.py`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/devo_sdk.egg-info/PKG-INFO` & `devo-sdk-5.1.4/devo_sdk.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: devo-sdk
-Version: 5.1.3
+Version: 5.1.4
 Summary: Devo Software Development Kit for Python.
 Home-page: https://github.com/DevoInc/python-sdk
 Author: Devo, Inc.
 Author-email: support@devo.com
 License: MIT
 Classifier: Programming Language :: Python
 Classifier: Development Status :: 5 - Production/Stable
@@ -22,142 +22,156 @@
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 ![License](https://img.shields.io/github/license/DevoInc/python-sdk)
 ![Wheel](https://img.shields.io/pypi/wheel/devo-sdk)
 ![Version](https://img.shields.io/pypi/v/devo-sdk)
-![Python](https://img.shields.io/pypi/pyversions/devo-sdk) 
+![Python](https://img.shields.io/pypi/pyversions/devo-sdk)
 ![Tests](https://github.com/DevoInc/python-sdk/actions/workflows/python-pull-request.yml/badge.svg)
 
 # Devo Python SDK
 
 This is the SDK to access Devo directly from Python. It can be used to:
+
 * Send events and files to Devo.
 * Make queries.
 * Manage deferred tasks.
 
 ## Requirements
 
 The Devo SDK for Python requires Python 3.7+
 
-## Compatibility 
+## Compatibility
+
 - Tested compatibility for python 3.7, 3.8 and 3.9
 
 ## Quick Start
-### Installing the SDK
 
+### Installing the SDK
 
 You can install the Devo SDK by using `easy_install` or `pip`:
 
-    #option 1
-    easy_install devo-sdk
-    
-    #option 2
-    pip install devo-sdk
+```console
+#option 1
+easy_install devo-sdk
 
+#option 2
+pip install devo-sdk
+```
 
 You can use sources files, cloning the project too:
 
-    #option 3
-    python setup.py install
-    
-    #option 4
-    pip install .
-    
-    #option 5 - dev option
-    pip install -e .
+```console
+#option 3
+python setup.py install
+
+#option 4
+pip install .
+
+#option 5 - dev option
+pip install -e .
+```
 
 ### Documentation
 
 There is specific documentation in the _[docs](https://github.com/DevoInc/python-sdk/tree/master/docs)_ folder for each part of SDK:
+
 * [Sender](https://github.com/DevoInc/python-sdk/tree/master/docs/sender/sender.md)
-    * [Data](https://github.com/DevoInc/python-sdk/tree/master/docs/sender/data.md)
-    * [Lookups](https://github.com/DevoInc/python-sdk/tree/master/docs/sender/lookup.md)
+  * [Data](https://github.com/DevoInc/python-sdk/tree/master/docs/sender/data.md)
+  * [Lookups](https://github.com/DevoInc/python-sdk/tree/master/docs/sender/lookup.md)
 * [Common](https://github.com/DevoInc/python-sdk/tree/master/docs/common.md)
 * API:
-    * [Api query](https://github.com/DevoInc/python-sdk/tree/master/docs/api/api.md)
-    * [Api tasks management](https://github.com/DevoInc/python-sdk/tree/master/docs/api/task.md)
-        * [Destination: email](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_email.md)
-        * [Destination: redis](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_redis.md)
-        * [Destination: S3](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_s3.md)
-
+  * [Api query](https://github.com/DevoInc/python-sdk/tree/master/docs/api/api.md)
+  * [Api tasks management](https://github.com/DevoInc/python-sdk/tree/master/docs/api/task.md)
+    * [Destination: email](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_email.md)
+    * [Destination: redis](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_redis.md)
+    * [Destination: S3](https://github.com/DevoInc/python-sdk/tree/master/docs/api/destination_s3.md)
 
 ## Contributing
+
 See [PyLibs contributing guide](https://github.com/DevoInc/python-sdk/tree/master/CONTRIBUTING.md).<br/>
 Pull and merge requests are welcome ☺
 
 ## Endpoints
-##### Sender
+
+### Sender
+
 To send data with Devo SDK, first choose the required endpoint depending on the region your are accessing from:
 
 | Region | Endpoint             | Port |
 |--------|----------------------|------|
 | USA    | collector-us.devo.io | 443  |
 | Canada | collector-ca.devo.io | 443  |
 | Europe | collector-eu.devo.io | 443  |
 | APAC   | collector-ap.devo.io | 443  |
 
 You have more information in the official documentation of Devo, [Sending data to Devo](https://docs.devo.com/space/latest/94652410/Sending%20data%20to%20Devo).
 
-##### API
+### API
+
 To perform a request with API, first choose the required endpoint depending on the region your are accessing from:
 
 | Region | Endpoint                               |
 |--------|----------------------------------------|
-| USA    | https://apiv2-us.devo.com/search/query |
-| Canada | https://apiv2-ca.devo.com/search/query |
-| Europe | https://apiv2-eu.devo.com/search/query |
-| APAC   | https://api-apac.devo.com/search/query |
+| USA    | <https://apiv2-us.devo.com/search/query> |
+| Canada | <https://apiv2-ca.devo.com/search/query> |
+| Europe | <https://apiv2-eu.devo.com/search/query> |
+| APAC   | <https://api-apac.devo.com/search/query> |
 
 You have more information in the official documentation of Devo, [REST API](https://docs.devo.com/space/latest/95128275/Query%20API).
 
 ## Credentials
+
 To obtain the access credentials necessary to use this SDK, you must have an account in [DEVO](https://www.devo.com/).<br/>
-Check the [security credentials](https://docs.devo.com/space/latest/94763701/Security%20credentials) info for more details. 
+Check the [security credentials](https://docs.devo.com/space/latest/94763701/Security%20credentials) info for more details.
+
+### Certificates
+
+You need use a three files (Cert, key and chain) to secure send data to Devo.
+Administrator users can find them in **Administration** → **Credentials**, in the X.509 tab.
+
+### API authorization
 
-##### Certificates
-You need use a three files (Cert, key and chain) to secure send data to Devo. 
-Administrator users can find them in **Administration** → **Credentials**, in the X.509 tab. 
-
-##### API authorization
-You can use a domain API key and API secret to sign the request. These are are a pair of credentials that every 
-Devo account owns. Administrator users can find them in **Administration** → **Credentials**, in the Access Keys tab. 
+You can use a domain API key and API secret to sign the request. These are are a pair of credentials that every
+Devo account owns. Administrator users can find them in **Administration** → **Credentials**, in the Access Keys tab.
 
 ## Launch tests
+
 ### run_tests script
+
 You can run tests from the main folder of SDK
 To launch this script, you need either the environment variables loaded in the system, or the _environment.env_ file in the root of the SDK with the correct values, since to test all the SDK functionalities it is necessary to connect to Devo for the tests of sending and extracting data. There is an example file called _environment.env.example_
 
 Its normal, by the way, TCP tests fails in clients or not Devo developers systems.
 
 ```console
-~/projects/devo-python-sdk > python setup.py test 
+~/projects/devo-python-sdk > python setup.py test
 ```
 
 ```console
 ~/projects/devo-python-sdk > python run_tests.py
 ```
 
 You can add option "Coverage" for create HTML report about tests.
 
-```console
+```text
 ~/projects/devo-python-sdk > python run_tests.py --coverage
 ```
 
 You can also run the test for just one module. This is a useful feature if you are developing functionality in just one module.
 
 ```console
-~/projects/devo-python-sdk > python run_tests.py -m SEND_CLI
+~/projects/devo-python-sdk > python run_tests.py -m SENDER_CLI
 ```
 
 You can also exclude one or several tests with `-M` parameter:
 
 ```console
-~/projects/devo-python-sdk > python run_tests.py -M SEND_CLI,API_CLI
+~/projects/devo-python-sdk > python run_tests.py -M SENDER_CLI,API_CLI
 ```
 
 Using the --help flag prints the available modules to use:
 
 ```console
 ~/projects/devo-python-sdk > python run_tests.py --help
 usage: run_tests.py [-h] [--coverage [COVERAGE]] [-m [MODULE]]
@@ -193,28 +207,28 @@
 
 ### Run using Unittest command
 
 You can see references in [unittest documentation](https://docs.python.org/3/library/unittest.html)
 
 For commands like:
 
-```bash
-python -m unittest discover -p "*.py" 
+```console
+python -m unittest discover -p "*.py"
 ```
 
-If you launch this command from the root directory of the SDK, you need to have the environment variables in your 
-system for all the tests that require connection to Devo can work, not being able to use the environment.env file 
+If you launch this command from the root directory of the SDK, you need to have the environment variables in your
+system for all the tests that require connection to Devo can work, not being able to use the environment.env file
 as in the script.
 
-
 ### Contact Us
 
 You can contact with us at _support@devo.com_.
 
 ## License
+
 MIT License
 
 (C) 2022 Devo, Inc.
 
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the 'Software'), to deal in
 the Software without restriction, including without limitation the rights to
```

### Comparing `devo-sdk-5.1.3/devo_sdk.egg-info/SOURCES.txt` & `devo-sdk-5.1.4/devo_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `devo-sdk-5.1.3/setup.py` & `devo-sdk-5.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,17 +20,17 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
-INSTALL_REQUIRES = ['requests>=2.27', 'click==8.1.3', 'PyYAML==6.0',
-                    'pem==21.2.0', 'pyopenssl==23.0.*', 'urllib3>=1.26.5',
-                    'pytz>=2019.3', 'cryptography>=39.0.1']
+INSTALL_REQUIRES = ['requests>=2.31', 'click==8.1.3', 'PyYAML==6.0',
+                    'pem==21.2.0', 'pyopenssl>=23.0', 'urllib3>=1.26.5',
+                    'pytz>=2019.3', 'cryptography>=41.0.1']
 CLI = ['devo-sender=devo.sender.scripts.sender_cli:cli',
        'devo-api=devo.api.scripts.client_cli:cli']
 
 
 def read(*parts):
     """
     Build an absolute path from *parts* and and return the contents of the
```

