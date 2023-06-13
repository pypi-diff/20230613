# Comparing `tmp/opentelemetry_instrument_openai-0.3.0.tar.gz` & `tmp/opentelemetry_instrument_openai-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentelemetry_instrument_openai-0.3.0.tar", max compression
+gzip compressed data, was "opentelemetry_instrument_openai-0.4.0.tar", max compression
```

## Comparing `opentelemetry_instrument_openai-0.3.0.tar` & `opentelemetry_instrument_openai-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    11349 2023-06-09 23:19:37.566099 opentelemetry_instrument_openai-0.3.0/LICENSE.md
--rw-r--r--   0        0        0     1248 2023-06-13 13:22:34.577607 opentelemetry_instrument_openai-0.3.0/README.md
--rw-r--r--   0        0        0      832 2023-06-13 13:19:29.457154 opentelemetry_instrument_openai-0.3.0/pyproject.toml
--rw-r--r--   0        0        0    16588 2023-06-13 04:33:56.454201 opentelemetry_instrument_openai-0.3.0/src/opentelemetry/instrumentation/openai/__init__.py
--rw-r--r--   0        0        0      611 2023-06-13 04:35:41.149396 opentelemetry_instrument_openai-0.3.0/src/opentelemetry/instrumentation/openai/package.py
--rw-r--r--   0        0        0      594 2023-06-13 13:19:14.874115 opentelemetry_instrument_openai-0.3.0/src/opentelemetry/instrumentation/openai/version.py
--rw-r--r--   0        0        0     2145 1970-01-01 00:00:00.000000 opentelemetry_instrument_openai-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0    11349 2023-06-09 23:19:37.566099 opentelemetry_instrument_openai-0.4.0/LICENSE.md
+-rw-r--r--   0        0        0     1175 2023-06-13 16:52:14.687909 opentelemetry_instrument_openai-0.4.0/README.md
+-rw-r--r--   0        0        0      875 2023-06-13 16:52:29.117415 opentelemetry_instrument_openai-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0    16588 2023-06-13 04:33:56.454201 opentelemetry_instrument_openai-0.4.0/src/opentelemetry/instrumentation/openai/__init__.py
+-rw-r--r--   0        0        0      611 2023-06-13 04:35:41.149396 opentelemetry_instrument_openai-0.4.0/src/opentelemetry/instrumentation/openai/package.py
+-rw-r--r--   0        0        0      596 2023-06-13 16:52:35.655382 opentelemetry_instrument_openai-0.4.0/src/opentelemetry/instrumentation/openai/version.py
+-rw-r--r--   0        0        0     2125 1970-01-01 00:00:00.000000 opentelemetry_instrument_openai-0.4.0/PKG-INFO
```

### Comparing `opentelemetry_instrument_openai-0.3.0/LICENSE.md` & `opentelemetry_instrument_openai-0.4.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrument_openai-0.3.0/pyproject.toml` & `opentelemetry_instrument_openai-0.4.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opentelemetry-instrument-openai"
-version = "0.3.0"
+version = "0.4.0"
 description = "OpenTelemetry openai instrumentation"
 license = "Apache-2.0"
 authors = ["cartermp <pcarter@fastmail.com>"]
 maintainers = ["cartermp <pcarter@fastmail.com>"]
 readme = "README.md"
 packages = [{include = "opentelemetry", from = "src" }]
 
@@ -16,13 +16,16 @@
 opentelemetry-semantic-conventions = "~=0.39b0"
 wrapt = "^1.15.0"
 
 [tool.poetry.group.test.dependencies]
 pytest = "*"
 opentelemetry-test-utils = "~=0.39b0"
 
-# [tool.poetry.plugins."opentelemetry_instrumentor"]
-# openai = "opentelemetry.instrumentation.openai:OpenAIInstrumentor"
+[tool.poetry.extras]
+instruments = ["openai"]
+
+[tool.poetry.plugins."opentelemetry_instrumentor"]
+openai = "opentelemetry.instrumentation.openai:OpenAIInstrumentor"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `opentelemetry_instrument_openai-0.3.0/src/opentelemetry/instrumentation/openai/__init__.py` & `opentelemetry_instrument_openai-0.4.0/src/opentelemetry/instrumentation/openai/__init__.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrument_openai-0.3.0/src/opentelemetry/instrumentation/openai/package.py` & `opentelemetry_instrument_openai-0.4.0/src/opentelemetry/instrumentation/openai/package.py`

 * *Files identical despite different names*

### Comparing `opentelemetry_instrument_openai-0.3.0/src/opentelemetry/instrumentation/openai/version.py` & `opentelemetry_instrument_openai-0.4.0/src/opentelemetry/instrumentation/openai/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.3"
+__version__ = "0.4.0"
```

### Comparing `opentelemetry_instrument_openai-0.3.0/PKG-INFO` & `opentelemetry_instrument_openai-0.4.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,52 @@
 Metadata-Version: 2.1
 Name: opentelemetry-instrument-openai
-Version: 0.3.0
+Version: 0.4.0
 Summary: OpenTelemetry openai instrumentation
 License: Apache-2.0
 Author: cartermp
 Author-email: pcarter@fastmail.com
 Maintainer: cartermp
 Maintainer-email: pcarter@fastmail.com
 Requires-Python: >=3.7.1,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: openai (>=0.27.8,<0.28.0)
+Provides-Extra: instruments
+Requires-Dist: openai (>=0.27.8,<0.28.0) ; extra == "instruments"
 Requires-Dist: opentelemetry-api (>=1.18.0,<1.19.0)
 Requires-Dist: opentelemetry-instrumentation (>=0.39b0,<1.0)
 Requires-Dist: opentelemetry-semantic-conventions (>=0.39b0,<1.0)
 Requires-Dist: wrapt (>=1.15.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # opentelemetry-instrument-openai
 
 It's OpenTelemetry instrumentation (python) for OpenAI's library.
 
-Pproject site: https://github.com/cartermp/opentelemetry-instrument-openai-py
+Project site: https://github.com/cartermp/opentelemetry-instrument-openai-py
 
 ## How to use it
 
 Simple! First, install this package.
 
 ### Usage
 
-It's one line of code too:
+With autoinstrumentation agent:
+
+```
+poetry add opentelemetry-instrument-openai
+poetry run opentelemetry-bootstrap -a install
+poetry run opentelemetry-instrument python your_app.py
+```
+
+If you prefer to do it in code, you can do that too:
 
 ```python
 import openai
 from dotenv import load_dotenv
 from opentelemetry.instrument.openai import OpenAIInstrumentor
 
 OpenAIInstrumentor().instrument()
@@ -47,24 +56,15 @@
 
 openai.ChatCompletion.create(
     model="gpt-3.5-turbo",
     messages=[{"role":"user", "content":"Tell me a joke about opentelemetry"}],
 )
 ```
 
-You can then run your app normally with your own opentelemetry initialization, or use the the autoinstrumentation agent (remove `poetry run` if you're not using poetry).
-
-```
-poetry run opentelemetry-bootstrap -a install
-poetry run opentelemetry-instrument \
-  --traces_exporter console \
-  --metrics_exporter none \
-  --logs_exporter none \
-  python chat.py
-```
+You can then run your app normally with your own opentelemetry initialization.
 
 ## How to develop
 
 Get [poetry](https://python-poetry.org/).
 
 Now install and run tests:
```

