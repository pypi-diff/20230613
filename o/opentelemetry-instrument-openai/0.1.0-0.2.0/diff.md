# Comparing `tmp/opentelemetry_instrument_openai-0.1.0.tar.gz` & `tmp/opentelemetry_instrument_openai-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrument_openai-0.1.0.tar", max compression
+gzip compressed data, was "opentelemetry_instrument_openai-0.2.0.tar", max compression
```

## Comparing `opentelemetry_instrument_openai-0.1.0.tar` & `opentelemetry_instrument_openai-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11349 2023-06-09 23:19:37.566099 opentelemetry_instrument_openai-0.1.0/LICENSE.md
--rw-r--r--   0        0        0     1153 2023-06-12 00:36:35.825755 opentelemetry_instrument_openai-0.1.0/README.md
--rw-r--r--   0        0        0      828 2023-06-12 00:13:40.579055 opentelemetry_instrument_openai-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     6641 2023-06-11 21:53:08.052821 opentelemetry_instrument_openai-0.1.0/src/opentelemetry/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0      612 2023-06-10 16:54:28.391850 opentelemetry_instrument_openai-0.1.0/src/opentelemetry/instrumentation/openai/package.py
--rw-r--r--   0        0        0      594 2023-06-10 16:54:32.148411 opentelemetry_instrument_openai-0.1.0/src/opentelemetry/instrumentation/openai/version.py
--rw-r--r--   0        0        0     2050 1970-01-01 00:00:00.000000 opentelemetry_instrument_openai-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-09 23:19:37.566099 opentelemetry_instrument_openai-0.2.0/LICENSE.md
+-rw-r--r--   0        0        0     1232 2023-06-13 00:12:47.356785 opentelemetry_instrument_openai-0.2.0/README.md
+-rw-r--r--   0        0        0      828 2023-06-13 05:02:54.254062 opentelemetry_instrument_openai-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    16588 2023-06-13 04:33:56.454201 opentelemetry_instrument_openai-0.2.0/src/opentelemetry/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0      611 2023-06-13 04:35:41.149396 opentelemetry_instrument_openai-0.2.0/src/opentelemetry/instrumentation/openai/package.py
+-rw-r--r--   0        0        0      594 2023-06-13 00:45:20.124028 opentelemetry_instrument_openai-0.2.0/src/opentelemetry/instrumentation/openai/version.py
+-rw-r--r--   0        0        0     2129 1970-01-01 00:00:00.000000 opentelemetry_instrument_openai-0.2.0/PKG-INFO
```

### Comparing `opentelemetry_instrument_openai-0.1.0/LICENSE.md` & `opentelemetry_instrument_openai-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrument_openai-0.1.0/README.md` & `opentelemetry_instrument_openai-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 # opentelemetry-instrument-openai
 
 It's OpenTelemetry instrumentation (python) for OpenAI's library.
 
+Pproject site: https://github.com/cartermp/opentelemetry-instrument-openai-py
+
 ## How to use it
 
 Simple! First, install this package.
 
 ### Autoinstrumentation
 
 ```
```

### Comparing `opentelemetry_instrument_openai-0.1.0/pyproject.toml` & `opentelemetry_instrument_openai-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opentelemetry-instrument-openai"
-version = "0.1.0"
+version = "0.2.0"
 description = "OpenTelemetry openai instrumentation"
 license = "Apache-2.0"
 authors = ["cartermp <pcarter@fastmail.com>"]
 maintainers = ["cartermp <pcarter@fastmail.com>"]
 readme = "README.md"
 packages = [{include = "opentelemetry", from = "src" }]
```

### Comparing `opentelemetry_instrument_openai-0.1.0/src/opentelemetry/instrumentation/openai/package.py` & `opentelemetry_instrument_openai-0.2.0/src/opentelemetry/instrumentation/openai/package.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,9 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-
 _instruments = ("openai ~= 0.27.8",)
```

### Comparing `opentelemetry_instrument_openai-0.1.0/src/opentelemetry/instrumentation/openai/version.py` & `opentelemetry_instrument_openai-0.2.0/src/opentelemetry/instrumentation/openai/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.1"
+__version__ = "0.2"
```

### Comparing `opentelemetry_instrument_openai-0.1.0/PKG-INFO` & `opentelemetry_instrument_openai-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrument-openai
-Version: 0.1.0
+Version: 0.2.0
 Summary: OpenTelemetry openai instrumentation
 License: Apache-2.0
 Author: cartermp
 Author-email: pcarter@fastmail.com
 Maintainer: cartermp
 Maintainer-email: pcarter@fastmail.com
 Requires-Python: >=3.7.1,<4.0
@@ -21,14 +21,16 @@
 Requires-Dist: wrapt (>=1.15.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # opentelemetry-instrument-openai
 
 It's OpenTelemetry instrumentation (python) for OpenAI's library.
 
+Pproject site: https://github.com/cartermp/opentelemetry-instrument-openai-py
+
 ## How to use it
 
 Simple! First, install this package.
 
 ### Autoinstrumentation
 
 ```
```

