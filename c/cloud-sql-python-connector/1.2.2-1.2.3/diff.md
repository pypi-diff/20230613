# Comparing `tmp/cloud-sql-python-connector-1.2.2.tar.gz` & `tmp/cloud-sql-python-connector-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloud-sql-python-connector-1.2.2.tar", last modified: Thu Apr 13 19:16:41 2023, max compression
+gzip compressed data, was "cloud-sql-python-connector-1.2.3.tar", last modified: Tue May  9 19:15:45 2023, max compression
```

## Comparing `cloud-sql-python-connector-1.2.2.tar` & `cloud-sql-python-connector-1.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 19:16:41.730187 cloud-sql-python-connector-1.2.2/
--rw-rw-r--   0 root         (0)     1003    11358 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/LICENSE
--rw-r--r--   0 root         (0)     1003    21826 2023-04-13 19:16:41.730187 cloud-sql-python-connector-1.2.2/PKG-INFO
--rw-rw-r--   0 root         (0)     1003    20679 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/README.md
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 19:16:41.730187 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/
--rw-r--r--   0 root         (0)     1003    21826 2023-04-13 19:16:41.000000 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003      935 2023-04-13 19:16:41.000000 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-13 19:16:41.000000 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2023-04-13 19:16:41.000000 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2023-04-13 19:16:41.000000 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      156 2023-04-13 19:16:41.000000 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2023-04-13 19:16:41.000000 cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 19:16:41.730187 cloud-sql-python-connector-1.2.2/google/
--rw-rw-r--   0 root         (0)     1003      746 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 19:16:41.730187 cloud-sql-python-connector-1.2.2/google/cloud/
--rw-rw-r--   0 root         (0)     1003      746 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 19:16:41.730187 cloud-sql-python-connector-1.2.2/google/cloud/sql/
--rw-rw-r--   0 root         (0)     1003        0 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2023-04-13 19:16:41.730187 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/
--rw-rw-r--   0 root         (0)     1003      876 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/__init__.py
--rw-rw-r--   0 root         (0)     1003     1838 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/asyncpg.py
--rwxrwxr-x   0 root         (0)     1003    13625 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/connector.py
--rw-rw-r--   0 root         (0)     1003     1454 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/exceptions.py
--rw-rw-r--   0 root         (0)     1003    17656 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/instance.py
--rw-rw-r--   0 root         (0)     1003     2031 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/pg8000.py
--rw-rw-r--   0 root         (0)     1003     1926 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/pymysql.py
--rw-rw-r--   0 root         (0)     1003     2451 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/pytds.py
--rw-rw-r--   0 root         (0)     1003     2954 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/rate_limiter.py
--rw-rw-r--   0 root         (0)     1003     9329 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/refresh_utils.py
--rwxrwxr-x   0 root         (0)     1003     4371 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/utils.py
--rw-rw-r--   0 root         (0)     1003      597 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/version.py
--rw-rw-r--   0 root         (0)     1003       67 2023-04-13 19:16:41.734187 cloud-sql-python-connector-1.2.2/setup.cfg
--rw-rw-r--   0 root         (0)     1003     2871 2023-04-13 19:14:13.000000 cloud-sql-python-connector-1.2.2/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-09 19:15:45.258746 cloud-sql-python-connector-1.2.3/
+-rw-rw-r--   0 root         (0)     1003    11358 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/LICENSE
+-rw-r--r--   0 root         (0)     1003    21826 2023-05-09 19:15:45.258746 cloud-sql-python-connector-1.2.3/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003    20679 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/README.md
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-09 19:15:45.254745 cloud-sql-python-connector-1.2.3/cloud_sql_python_connector.egg-info/
+-rw-r--r--   0 root         (0)     1003    21826 2023-05-09 19:15:45.000000 cloud-sql-python-connector-1.2.3/cloud_sql_python_connector.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003      935 2023-05-09 19:15:45.000000 cloud-sql-python-connector-1.2.3/cloud_sql_python_connector.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-09 19:15:45.000000 cloud-sql-python-connector-1.2.3/cloud_sql_python_connector.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2023-05-09 19:15:45.000000 cloud-sql-python-connector-1.2.3/cloud_sql_python_connector.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2023-05-09 19:15:45.000000 cloud-sql-python-connector-1.2.3/cloud_sql_python_connector.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      156 2023-05-09 19:15:45.000000 cloud-sql-python-connector-1.2.3/cloud_sql_python_connector.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2023-05-09 19:15:45.000000 cloud-sql-python-connector-1.2.3/cloud_sql_python_connector.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-09 19:15:45.254745 cloud-sql-python-connector-1.2.3/google/
+-rw-rw-r--   0 root         (0)     1003      746 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-09 19:15:45.254745 cloud-sql-python-connector-1.2.3/google/cloud/
+-rw-rw-r--   0 root         (0)     1003      746 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/cloud/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-09 19:15:45.254745 cloud-sql-python-connector-1.2.3/google/cloud/sql/
+-rw-rw-r--   0 root         (0)     1003        0 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/cloud/sql/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2023-05-09 19:15:45.258746 cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/
+-rw-rw-r--   0 root         (0)     1003      876 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1838 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/asyncpg.py
+-rwxrwxr-x   0 root         (0)     1003    13625 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/connector.py
+-rw-rw-r--   0 root         (0)     1003     1454 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/exceptions.py
+-rw-rw-r--   0 root         (0)     1003    17656 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/instance.py
+-rw-rw-r--   0 root         (0)     1003     2031 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/pg8000.py
+-rw-rw-r--   0 root         (0)     1003     1926 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/pymysql.py
+-rw-rw-r--   0 root         (0)     1003     2451 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/pytds.py
+-rw-rw-r--   0 root         (0)     1003     2954 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/rate_limiter.py
+-rw-rw-r--   0 root         (0)     1003     9329 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/refresh_utils.py
+-rwxrwxr-x   0 root         (0)     1003     4371 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/utils.py
+-rw-rw-r--   0 root         (0)     1003      597 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/version.py
+-rw-rw-r--   0 root         (0)     1003       67 2023-05-09 19:15:45.258746 cloud-sql-python-connector-1.2.3/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     2871 2023-05-09 19:13:33.000000 cloud-sql-python-connector-1.2.3/setup.py
```

### Comparing `cloud-sql-python-connector-1.2.2/LICENSE` & `cloud-sql-python-connector-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/PKG-INFO` & `cloud-sql-python-connector-1.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-sql-python-connector
-Version: 1.2.2
+Version: 1.2.3
 Summary: The Cloud SQL Python Connector is a library that can be used alongside a database driver to allow users with sufficient permissions to connect to a Cloud SQL database without having to manually allowlist IPs or manage SSL certificates.
 Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cloud-sql-python-connector-1.2.2/README.md` & `cloud-sql-python-connector-1.2.3/README.md`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/PKG-INFO` & `cloud-sql-python-connector-1.2.3/cloud_sql_python_connector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloud-sql-python-connector
-Version: 1.2.2
+Version: 1.2.3
 Summary: The Cloud SQL Python Connector is a library that can be used alongside a database driver to allow users with sufficient permissions to connect to a Cloud SQL database without having to manually allowlist IPs or manage SSL certificates.
 Home-page: https://github.com/GoogleCloudPlatform/cloud-sql-python-connector
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cloud-sql-python-connector-1.2.2/cloud_sql_python_connector.egg-info/SOURCES.txt` & `cloud-sql-python-connector-1.2.3/cloud_sql_python_connector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/google/__init__.py` & `cloud-sql-python-connector-1.2.3/google/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/google/cloud/__init__.py` & `cloud-sql-python-connector-1.2.3/google/cloud/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/__init__.py` & `cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/__init__.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/asyncpg.py` & `cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/asyncpg.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/connector.py` & `cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/connector.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/exceptions.py` & `cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/exceptions.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/instance.py` & `cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/instance.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/pg8000.py` & `cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/pg8000.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/pymysql.py` & `cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/pymysql.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/pytds.py` & `cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/pytds.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/rate_limiter.py` & `cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/rate_limiter.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/refresh_utils.py` & `cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/refresh_utils.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/utils.py` & `cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/utils.py`

 * *Files identical despite different names*

### Comparing `cloud-sql-python-connector-1.2.2/google/cloud/sql/connector/version.py` & `cloud-sql-python-connector-1.2.3/google/cloud/sql/connector/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "1.2.2"
+__version__ = "1.2.3"
```

### Comparing `cloud-sql-python-connector-1.2.2/setup.py` & `cloud-sql-python-connector-1.2.3/setup.py`

 * *Files identical despite different names*

