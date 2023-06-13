# Comparing `tmp/ipyfilite-0.1.7.tar.gz` & `tmp/ipyfilite-0.1.8.tar.gz`

## Comparing `ipyfilite-0.1.7.tar` & `ipyfilite-0.1.8.tar`

### file list

```diff
@@ -1,64 +1,68 @@
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/.coveragerc
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/.eslintignore
--rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/.eslintrc.js
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/.npmignore
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/.prettierignore
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/.prettierrc
--rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/MANIFEST.in
--rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/babel.config.js
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/codecov.yml
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/install.json
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite.json
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/jest.config.js
--rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/package.json
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/pytest.ini
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/readthedocs.yml
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/setup.py
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/tsconfig.eslint.json
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/tsconfig.json
--rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/webpack.config.js
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/css/widget.css
--rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/docs/Makefile
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/docs/environment.yml
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/docs/make.bat
--rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/docs/source/conf.py
--rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/docs/source/develop-install.rst
--rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/docs/source/index.rst
--rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/docs/source/installing.rst
--rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/docs/source/introduction.rst
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/docs/source/_static/helper.js
--rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/docs/source/examples/index.rst
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/docs/source/examples/introduction.nblink
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/examples/example.txt
--rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/examples/introduction.ipynb
--rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/__init__.py
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/_frontend.py
--rw-r--r--   0        0        0     3101 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/_manager.py
--rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/_version.py
--rw-r--r--   0        0        0     8148 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/http.py
--rw-r--r--   0        0        0     6140 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/upload.py
--rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/labextension/package.json
--rw-r--r--   0        0        0    10419 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/labextension/static/480.522a35aad26b3baab1ae.js
--rw-r--r--   0        0        0    10010 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/labextension/static/568.f51073d63c90f5a53748.js
--rw-r--r--   0        0        0     6262 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/labextension/static/remoteEntry.2c0ba414ad48ffdc77a7.js
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/labextension/static/style.js
--rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/labextension/static/third-party-licenses.json
--rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/nbextension/extension.js
--rw-r--r--   0        0        0    10768 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/nbextension/index.js
--rw-r--r--   0        0        0    28884 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/nbextension/index.js.map
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/tests/__init__.py
--rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/tests/conftest.py
--rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/tests/test_nbextension_path.py
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/ipyfilite/tests/test_upload.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/src/extension.ts
--rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/src/index.ts
--rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/src/plugin.ts
--rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/src/version.ts
--rw-r--r--   0        0        0     4665 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/src/widget.ts
--rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/src/__tests__/index.spec.ts
--rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/src/__tests__/utils.ts
--rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/.gitignore
--rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/LICENSE.txt
--rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/README.md
--rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 ipyfilite-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/.coveragerc
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/.eslintignore
+-rw-r--r--   0        0        0      807 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/.eslintrc.js
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/.npmignore
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/.prettierignore
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/.prettierrc
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/MANIFEST.in
+-rw-r--r--   0        0        0      177 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/babel.config.js
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/codecov.yml
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/install.json
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite.json
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/jest.config.js
+-rw-r--r--   0        0        0     3071 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/package.json
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/pytest.ini
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/readthedocs.yml
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/setup.py
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/tsconfig.eslint.json
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/tsconfig.json
+-rw-r--r--   0        0        0     2117 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/webpack.config.js
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/css/widget.css
+-rw-r--r--   0        0        0      611 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/docs/Makefile
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/docs/environment.yml
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/docs/make.bat
+-rw-r--r--   0        0        0     6647 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/docs/source/conf.py
+-rw-r--r--   0        0        0      821 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/docs/source/develop-install.rst
+-rw-r--r--   0        0        0      764 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/docs/source/index.rst
+-rw-r--r--   0        0        0     1011 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/docs/source/installing.rst
+-rw-r--r--   0        0        0      109 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/docs/source/introduction.rst
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/docs/source/_static/helper.js
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/docs/source/examples/index.rst
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/docs/source/examples/introduction.nblink
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/examples/example.txt
+-rw-r--r--   0        0        0     1117 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/examples/introduction.ipynb
+-rw-r--r--   0        0        0     1998 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/__init__.py
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/_frontend.py
+-rw-r--r--   0        0        0     4136 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/_manager.py
+-rw-r--r--   0        0        0      202 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/_version.py
+-rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/upload.py
+-rw-r--r--   0        0        0      518 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/download/__init__.py
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/download/fs.js
+-rw-r--r--   0        0        0     6318 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/http/__init__.py
+-rw-r--r--   0        0        0     1880 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/http/blob.js
+-rw-r--r--   0        0        0     3187 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/labextension/package.json
+-rw-r--r--   0        0        0    10682 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/labextension/static/367.2b53dbfb84806314e897.js
+-rw-r--r--   0        0        0      921 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/labextension/static/480.d744653fa4c869369de5.js
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/labextension/static/568.1f78854f2c5197037e64.js
+-rw-r--r--   0        0        0     6240 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/labextension/static/remoteEntry.7fc7bd0e9744231b6636.js
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/labextension/static/style.js
+-rw-r--r--   0        0        0     2452 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/labextension/static/third-party-licenses.json
+-rw-r--r--   0        0        0      408 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/nbextension/extension.js
+-rw-r--r--   0        0        0    11876 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/nbextension/index.js
+-rw-r--r--   0        0        0    32727 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/nbextension/index.js.map
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/tests/__init__.py
+-rw-r--r--   0        0        0     1429 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/tests/conftest.py
+-rw-r--r--   0        0        0      463 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/tests/test_nbextension_path.py
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/ipyfilite/tests/test_upload.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/src/extension.ts
+-rw-r--r--   0        0        0      145 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/src/index.ts
+-rw-r--r--   0        0        0     1114 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/src/plugin.ts
+-rw-r--r--   0        0        0      573 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/src/version.ts
+-rw-r--r--   0        0        0     6920 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/src/widget.ts
+-rw-r--r--   0        0        0      587 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/src/__tests__/index.spec.ts
+-rw-r--r--   0        0        0     3366 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/src/__tests__/utils.ts
+-rw-r--r--   0        0        0     1999 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/.gitignore
+-rw-r--r--   0        0        0     1498 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/LICENSE.txt
+-rw-r--r--   0        0        0     3243 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/README.md
+-rw-r--r--   0        0        0     3091 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 ipyfilite-0.1.8/PKG-INFO
```

### Comparing `ipyfilite-0.1.7/.eslintrc.js` & `ipyfilite-0.1.8/.eslintrc.js`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/MANIFEST.in` & `ipyfilite-0.1.8/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/package.json` & `ipyfilite-0.1.8/package.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.96875%*

 * *Differences: {"'version'": "'0.1.8'"}*

```diff
@@ -87,9 +87,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.7"
+    "version": "0.1.8"
 }
```

### Comparing `ipyfilite-0.1.7/tsconfig.json` & `ipyfilite-0.1.8/tsconfig.json`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/webpack.config.js` & `ipyfilite-0.1.8/webpack.config.js`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/docs/Makefile` & `ipyfilite-0.1.8/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/docs/make.bat` & `ipyfilite-0.1.8/docs/make.bat`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/docs/source/conf.py` & `ipyfilite-0.1.8/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/docs/source/develop-install.rst` & `ipyfilite-0.1.8/docs/source/develop-install.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/docs/source/index.rst` & `ipyfilite-0.1.8/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/docs/source/installing.rst` & `ipyfilite-0.1.8/docs/source/installing.rst`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/examples/introduction.ipynb` & `ipyfilite-0.1.8/examples/introduction.ipynb`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/ipyfilite/__init__.py` & `ipyfilite-0.1.8/ipyfilite/__init__.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/ipyfilite/_manager.py` & `ipyfilite-0.1.8/ipyfilite/_manager.py`

 * *Files 24% similar despite different names*

```diff
@@ -26,14 +26,29 @@
                 "ipyfilite only works inside a Pyodide kernel in JupyterLite",
                 FutureWarning,
             )
         else:
             self._channel = js.BroadcastChannel.new("ipyfilite")
             self._channel.onmessage = self._on_file_upload
 
+            self._download_fs = pyodide.code.run_js(
+                (Path(__file__).parent / "download" / "fs.js").read_text()
+            )
+            self._download_fs._session = str(self._session)
+            self._download_fs._channel = self._channel
+            self._download_fs._pyodide = pyodide_js
+
+            if Path("/download").exists():
+                pyodide_js.FS.unmount("/download")
+            else:
+                Path("/download").mkdir()
+            pyodide_js.FS.mount(self._download_fs, None, "/download")
+
+            self._download_root = pyodide_js.FS.lookupPath("/download").node
+
     @property
     def session(self) -> uuid.UUID:
         return self._session
 
     @classmethod
     def instance(cls):
         ip = get_ipython()
@@ -59,21 +74,25 @@
     def _on_file_upload(self, event):
         import js
         import pyodide
         import pyodide_js
 
         if (
             not getattr(event, "data", None)
+            or not getattr(event.data, "kind", None)
             or not getattr(event.data, "files", None)
             or not getattr(event.data, "uuid", None)
             or not getattr(event.data, "session", None)
             or not getattr(event.data, "widget", None)
         ):
             return
 
+        if event.data.kind != "upload":
+            return
+
         if event.data.session != str(self.session):
             return
 
         if event.data.widget not in self._upload_widgets:
             return
 
         upload_path = Path("/uploads") / event.data.uuid
@@ -100,7 +119,16 @@
                         file.lastModified / 1000, tz=dt.timezone.utc
                     ),
                     path=upload_path / file.name,
                 )
                 for file in event.data.files
             ],
         )
+
+    def register_download(self, uuid: str, name: str) -> Path:
+        path = self._download_fs.create_download(
+            self._download_root, uuid, name
+        )
+        return Path(path)
+
+    def unregister_download(self, uuid: str):
+        self._download_fs.close_download(self._download_root, uuid)
```

### Comparing `ipyfilite-0.1.7/ipyfilite/http.py` & `ipyfilite-0.1.8/ipyfilite/http/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -149,81 +149,17 @@
         accept_ranges = response.getheader("accept-ranges", None)
         accept_ranges = accept_ranges.lower() if accept_ranges else None
 
     return (content_length, accept_ranges)
 
 
 if _has_pyodide:
-    _RawHTTPBlobPyodide = pyodide.code.run_js("""
-class _RawHTTPBlobPyodide {
-    constructor(url, name, content_length, buffer_size, js) {
-        this._url = url;
-        this._content_length = content_length;
-
-        this._buffer_start = 0;
-        this._buffer = null;
-        this._buffer_size = buffer_size;
-
-        this._js = js;
-    }
-
-    get size() {
-        return this._content_length;
-    }
-
-    slice(start=0, end=this.size, contentType="") {
-        if (end <= start) {
-            return new Blob(undefined, { type: contentType });
-        }
-
-        if (this._buffer !== null) {
-            if (
-                start >= this._buffer_start &&
-                end <= (this._buffer_start + this._buffer.size)
-            ) {
-                return this._buffer.slice(
-                    start - this._buffer_start,
-                    end - this._buffer_start,
-                    contentType,
-                );
-            }
-        }
-
-        const new_start = Math.max(0, start);
-        const new_end = Math.max(Math.min(
-            Math.max(end - 1, start + this._buffer_size - 1),
-            this._content_length - 1,
-        ), start + 1);
-
-        const xhr = new XMLHttpRequest();
-        xhr.responseType = "blob";
-        xhr.open("GET", this._url, false);
-        xhr.setRequestHeader("range", `bytes=${start}-${new_end}`);
-        xhr.send(null);
-
-        if (xhr.status == 200) {
-            throw new this._js.FS.ErrnoError(
-                this._js.ERRNO_CODES.EOPNOTSUPP
-            );
-        }
-
-        const response = xhr.response;
-
-        const real_start = new_start;
-        const real_end = real_start + response.size;
-
-        this._buffer_start = Math.max(
-            real_start, real_end - this._buffer_size,
-        );
-        this._buffer = response.slice(this._buffer_start - real_start);
-
-        return response.slice(0, end-start, contentType);
-    }
-} _RawHTTPBlobPyodide
-    """)
+    _RawHTTPBlobPyodide = pyodide.code.run_js(
+        (Path(__file__).parent / "blob.js").read_text()
+    )
 
 
 class _RawHTTPFileUrllib(io.RawIOBase):
     def __init__(self, url: str, content_length: int):
         super().__init__()
 
         self._url = url
```

### Comparing `ipyfilite-0.1.7/ipyfilite/upload.py` & `ipyfilite-0.1.8/ipyfilite/upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -190,13 +190,14 @@
         from IPython.display import display
 
         display(self)
 
         future = asyncio.Future()
         self.observe(future.set_result, "value")
         await future
+        self.unobserve(future.set_result, "value")
 
         return self.value
 
     def __del__(self):
         IpyfiliteManager.instance().unregister_upload(self)
         super().__del__()
```

### Comparing `ipyfilite-0.1.7/ipyfilite/labextension/package.json` & `ipyfilite-0.1.8/ipyfilite/labextension/package.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9677734375%*

 * *Differences: {"'jupyterlab'": "{'_build': {'load': 'static/remoteEntry.7fc7bd0e9744231b6636.js'}}",*

 * * "'version'": "'0.1.8'"}*

```diff
@@ -46,15 +46,15 @@
         "dist/*.js",
         "css/*.css"
     ],
     "homepage": "https://github.com/juntyr/ipyfilite",
     "jupyterlab": {
         "_build": {
             "extension": "./extension",
-            "load": "static/remoteEntry.2c0ba414ad48ffdc77a7.js"
+            "load": "static/remoteEntry.7fc7bd0e9744231b6636.js"
         },
         "extension": "lib/plugin",
         "outputDir": "ipyfilite/labextension/",
         "sharedPackages": {
             "@jupyter-widgets/base": {
                 "bundled": false,
                 "singleton": true
@@ -91,9 +91,9 @@
         "test": "jest",
         "watch": "npm-run-all -p watch:*",
         "watch:labextension": "jupyter labextension watch .",
         "watch:lib": "tsc -w",
         "watch:nbextension": "webpack --watch --mode=development"
     },
     "types": "./lib/index.d.ts",
-    "version": "0.1.7"
+    "version": "0.1.8"
 }
```

### Comparing `ipyfilite-0.1.7/ipyfilite/labextension/static/480.522a35aad26b3baab1ae.js` & `ipyfilite-0.1.8/ipyfilite/labextension/static/367.2b53dbfb84806314e897.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,343 +1,325 @@
 (self.webpackChunkipyfilite = self.webpackChunkipyfilite || []).push([
-    [480], {
-        480: function(e, t, i) {
-            "use strict";
-            var n = this && this.__createBinding || (Object.create ? function(e, t, i, n) {
-                    void 0 === n && (n = i), Object.defineProperty(e, n, {
-                        enumerable: !0,
-                        get: function() {
-                            return t[i]
-                        }
-                    })
-                } : function(e, t, i, n) {
-                    void 0 === n && (n = i), e[n] = t[i]
-                }),
-                s = this && this.__setModuleDefault || (Object.create ? function(e, t) {
-                    Object.defineProperty(e, "default", {
-                        enumerable: !0,
-                        value: t
-                    })
-                } : function(e, t) {
-                    e.default = t
-                }),
-                l = this && this.__importStar || function(e) {
-                    if (e && e.__esModule) return e;
-                    var t = {};
-                    if (null != e)
-                        for (var i in e) "default" !== i && Object.prototype.hasOwnProperty.call(e, i) && n(t, e, i);
-                    return s(t, e), t
-                };
-            Object.defineProperty(t, "__esModule", {
-                value: !0
-            });
-            const a = i(829),
-                r = l(i(367)),
-                o = i(657),
-                u = {
-                    id: "ipyfilite:plugin",
-                    requires: [a.IJupyterWidgetRegistry],
-                    activate: function(e, t) {
-                        t.registerWidget({
-                            name: o.MODULE_NAME,
-                            version: o.MODULE_VERSION,
-                            exports: r
-                        })
-                    },
-                    autoStart: !0
-                };
-            t.default = u
-        },
-        657: (e, t, i) => {
+    [367], {
+        657: (e, t, n) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.MODULE_NAME = t.MODULE_VERSION = void 0;
-            const n = i(147);
-            t.MODULE_VERSION = n.version, t.MODULE_NAME = n.name
+            const i = n(147);
+            t.MODULE_VERSION = i.version, t.MODULE_NAME = i.name
         },
-        367: (e, t, i) => {
+        367: (e, t, n) => {
             "use strict";
             Object.defineProperty(t, "__esModule", {
                 value: !0
             }), t.FileUploadLiteView = t.FileUploadLiteModel = void 0;
-            const n = i(829),
-                s = i(657);
-            i(204);
-            class l extends n.DOMWidgetModel {
+            const i = n(829),
+                s = n(657);
+            n(204);
+            class a extends i.DOMWidgetModel {
                 defaults() {
                     return Object.assign(Object.assign({}, super.defaults()), {
-                        _model_name: l.model_name,
-                        _model_module: l.model_module,
-                        _model_module_version: l.model_module_version,
-                        _view_name: l.view_name,
-                        _view_module: l.view_module,
-                        _view_module_version: l.view_module_version,
-                        _session: n.uuid(),
+                        _model_name: a.model_name,
+                        _model_module: a.model_module,
+                        _model_module_version: a.model_module_version,
+                        _view_name: a.view_name,
+                        _view_module: a.view_module,
+                        _view_module_version: a.view_module_version,
+                        _session: i.uuid(),
                         accept: "",
                         description: "Upload",
                         disabled: !1,
                         icon: "upload",
                         button_style: "",
                         multiple: !1,
                         value: [],
                         style: null
                     })
                 }
             }
-            t.FileUploadLiteModel = l, l.serializers = Object.assign(Object.assign({}, n.DOMWidgetModel.serializers), {
+            t.FileUploadLiteModel = a, a.serializers = Object.assign(Object.assign({}, i.DOMWidgetModel.serializers), {
                 value: {
                     serialize: e => e
                 }
-            }), l.model_name = "FileUploadLiteModel", l.model_module = s.MODULE_NAME, l.model_module_version = s.MODULE_VERSION, l.view_name = "FileUploadLiteView", l.view_module = s.MODULE_NAME, l.view_module_version = s.MODULE_VERSION;
-            class a extends n.DOMWidgetView {
+            }), a.model_name = "FileUploadLiteModel", a.model_module = s.MODULE_NAME, a.model_module_version = s.MODULE_VERSION, a.view_name = "FileUploadLiteView", a.view_module = s.MODULE_NAME, a.view_module_version = s.MODULE_VERSION;
+            class o extends i.DOMWidgetView {
                 preinitialize() {
                     this.tagName = "button"
                 }
                 render() {
                     super.render(), this.el.classList.add("jupyter-widgets"), this.el.classList.add("widget-upload-lite"), this.el.classList.add("jupyter-button"), this.fileInput = document.createElement("input"), this.fileInput.type = "file", this.fileInput.style.display = "none", this.el.addEventListener("click", (() => {
                         this.fileInput.click()
                     })), this.fileInput.addEventListener("click", (() => {
                         this.fileInput.value = ""
                     })), this.fileInput.addEventListener("change", (() => {
                         var e;
-                        const t = n.uuid(),
-                            i = Array.from(null !== (e = this.fileInput.files) && void 0 !== e ? e : []).map((e => ({
+                        const t = i.uuid(),
+                            n = Array.from(null !== (e = this.fileInput.files) && void 0 !== e ? e : []).map((e => ({
                                 name: e.name,
                                 type: e.type,
                                 size: e.size,
                                 last_modified: e.lastModified,
                                 path: `/uploads/${t}/${e.name}`
                             })));
-                        r.getBroadcastChannel().postMessage({
+                        l.getBroadcastChannel().postMessage({
+                            kind: "upload",
                             files: this.fileInput.files,
                             uuid: t,
                             session: this.model.get("_session"),
                             widget: this.model.model_id
                         }), this.model.set({
-                            value: i
+                            value: n
                         }), this.touch()
                     })), this.listenTo(this.model, "change:button_style", this.update_button_style), this.set_button_style(), this.update()
                 }
                 update() {
                     this.el.disabled = this.model.get("disabled"), this.el.setAttribute("title", this.model.get("tooltip"));
                     const e = this.model.get("value"),
                         t = `${this.model.get("description")} (${e.length})`,
-                        i = this.model.get("icon");
-                    if (t.length || i.length) {
-                        if (this.el.textContent = "", i.length) {
+                        n = this.model.get("icon");
+                    if (t.length || n.length) {
+                        if (this.el.textContent = "", n.length) {
                             const e = document.createElement("i");
-                            e.classList.add("fa"), e.classList.add("fa-" + i), 0 === t.length && e.classList.add("center"), this.el.appendChild(e)
+                            e.classList.add("fa"), e.classList.add("fa-" + n), 0 === t.length && e.classList.add("center"), this.el.appendChild(e)
                         }
                         this.el.appendChild(document.createTextNode(t))
                     }
                     return this.fileInput.accept = this.model.get("accept"), this.fileInput.multiple = this.model.get("multiple"), super.update()
                 }
                 update_button_style() {
-                    this.update_mapped_classes(a.class_map, "button_style", this.el)
+                    this.update_mapped_classes(o.class_map, "button_style", this.el)
                 }
                 set_button_style() {
-                    this.set_mapped_classes(a.class_map, "button_style", this.el)
+                    this.set_mapped_classes(o.class_map, "button_style", this.el)
                 }
             }
-            var r;
-            t.FileUploadLiteView = a, a.class_map = {
+            var l;
+            t.FileUploadLiteView = o, o.class_map = {
                     primary: ["mod-primary"],
                     success: ["mod-success"],
                     info: ["mod-info"],
                     warning: ["mod-warning"],
                     danger: ["mod-danger"]
                 },
                 function(e) {
                     const t = new BroadcastChannel("ipyfilite");
+
+                    function n(e, t) {
+                        const n = document.createElement("a");
+                        n.href = URL.createObjectURL(new Blob(t)), n.download = e, n.click()
+                    }
                     e.getBroadcastChannel = function() {
                         return t
+                    };
+                    const i = new Map;
+                    t.onmessage = function(e) {
+                        if (e.data && e.data.kind)
+                            if ("download-open" === e.data.kind) {
+                                if (i.has(e.data.uuid)) return void console.warn(`Download stream for '${e.data.uuid}' already open.`);
+                                i.set(e.data.uuid, {
+                                    name: e.data.name,
+                                    chunks: [],
+                                    size: 0,
+                                    segment: 0
+                                })
+                            } else if ("download-chunk" === e.data.kind) {
+                            if (!i.has(e.data.uuid)) return void console.warn(`No download stream for '${e.data.uuid}' is open to write to.`);
+                            const t = i.get(e.data.uuid),
+                                s = new Uint8Array(e.data.chunk);
+                            t.chunks.push(s), t.size += s.length, t.size >= 268435456 && (t.segment += 1, n(`${t.name}.${t.segment.toString().padStart(3,"0")}`, t.chunks), t.chunks = [], t.size = 0)
+                        } else if ("download-close" === e.data.kind) {
+                            if (!i.has(e.data.uuid)) return void console.warn(`No download stream for '${e.data.uuid}' is open to close.`);
+                            const t = i.get(e.data.uuid);
+                            if (i.delete(e.data.uuid), t.segment > 0 && 0 === t.chunks.length) return;
+                            t.segment > 0 ? (t.segment += 1, n(`${t.name}.${t.segment.toString().padStart(3,"0")}`, t.chunks)) : n(t.name, t.chunks)
+                        }
                     }
-                }(r || (r = {}))
+                }(l || (l = {}))
         },
-        889: (e, t, i) => {
-            (t = i(645)(!1)).push([e.id, ".custom-widget {\n  background-color: lightseagreen;\n  padding: 0px 2px;\n}\n", ""]), e.exports = t
+        889: (e, t, n) => {
+            (t = n(645)(!1)).push([e.id, ".custom-widget {\n  background-color: lightseagreen;\n  padding: 0px 2px;\n}\n", ""]), e.exports = t
         },
         645: e => {
             "use strict";
             e.exports = function(e) {
                 var t = [];
                 return t.toString = function() {
                     return this.map((function(t) {
-                        var i = function(e, t) {
-                            var i, n, s, l = e[1] || "",
-                                a = e[3];
-                            if (!a) return l;
+                        var n = function(e, t) {
+                            var n, i, s, a = e[1] || "",
+                                o = e[3];
+                            if (!o) return a;
                             if (t && "function" == typeof btoa) {
-                                var r = (i = a, n = btoa(unescape(encodeURIComponent(JSON.stringify(i)))), s = "sourceMappingURL=data:application/json;charset=utf-8;base64,".concat(n), "/*# ".concat(s, " */")),
-                                    o = a.sources.map((function(e) {
-                                        return "/*# sourceURL=".concat(a.sourceRoot || "").concat(e, " */")
+                                var l = (n = o, i = btoa(unescape(encodeURIComponent(JSON.stringify(n)))), s = "sourceMappingURL=data:application/json;charset=utf-8;base64,".concat(i), "/*# ".concat(s, " */")),
+                                    r = o.sources.map((function(e) {
+                                        return "/*# sourceURL=".concat(o.sourceRoot || "").concat(e, " */")
                                     }));
-                                return [l].concat(o).concat([r]).join("\n")
+                                return [a].concat(r).concat([l]).join("\n")
                             }
-                            return [l].join("\n")
+                            return [a].join("\n")
                         }(t, e);
-                        return t[2] ? "@media ".concat(t[2], " {").concat(i, "}") : i
+                        return t[2] ? "@media ".concat(t[2], " {").concat(n, "}") : n
                     })).join("")
-                }, t.i = function(e, i, n) {
+                }, t.i = function(e, n, i) {
                     "string" == typeof e && (e = [
                         [null, e, ""]
                     ]);
                     var s = {};
-                    if (n)
-                        for (var l = 0; l < this.length; l++) {
-                            var a = this[l][0];
-                            null != a && (s[a] = !0)
+                    if (i)
+                        for (var a = 0; a < this.length; a++) {
+                            var o = this[a][0];
+                            null != o && (s[o] = !0)
                         }
-                    for (var r = 0; r < e.length; r++) {
-                        var o = [].concat(e[r]);
-                        n && s[o[0]] || (i && (o[2] ? o[2] = "".concat(i, " and ").concat(o[2]) : o[2] = i), t.push(o))
+                    for (var l = 0; l < e.length; l++) {
+                        var r = [].concat(e[l]);
+                        i && s[r[0]] || (n && (r[2] ? r[2] = "".concat(n, " and ").concat(r[2]) : r[2] = n), t.push(r))
                     }
                 }, t
             }
         },
-        204: (e, t, i) => {
-            var n = i(379),
-                s = i(889);
+        204: (e, t, n) => {
+            var i = n(379),
+                s = n(889);
             "string" == typeof(s = s.__esModule ? s.default : s) && (s = [
                 [e.id, s, ""]
             ]);
-            n(s, {
+            i(s, {
                 insert: "head",
                 singleton: !1
             }), e.exports = s.locals || {}
         },
-        379: (e, t, i) => {
+        379: (e, t, n) => {
             "use strict";
-            var n, s = function() {
+            var i, s = function() {
                     var e = {};
                     return function(t) {
                         if (void 0 === e[t]) {
-                            var i = document.querySelector(t);
-                            if (window.HTMLIFrameElement && i instanceof window.HTMLIFrameElement) try {
-                                i = i.contentDocument.head
+                            var n = document.querySelector(t);
+                            if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
+                                n = n.contentDocument.head
                             } catch (e) {
-                                i = null
+                                n = null
                             }
-                            e[t] = i
+                            e[t] = n
                         }
                         return e[t]
                     }
                 }(),
-                l = [];
+                a = [];
 
-            function a(e) {
-                for (var t = -1, i = 0; i < l.length; i++)
-                    if (l[i].identifier === e) {
-                        t = i;
+            function o(e) {
+                for (var t = -1, n = 0; n < a.length; n++)
+                    if (a[n].identifier === e) {
+                        t = n;
                         break
                     } return t
             }
 
-            function r(e, t) {
-                for (var i = {}, n = [], s = 0; s < e.length; s++) {
-                    var r = e[s],
-                        o = t.base ? r[0] + t.base : r[0],
-                        u = i[o] || 0,
-                        d = "".concat(o, " ").concat(u);
-                    i[o] = u + 1;
-                    var c = a(d),
+            function l(e, t) {
+                for (var n = {}, i = [], s = 0; s < e.length; s++) {
+                    var l = e[s],
+                        r = t.base ? l[0] + t.base : l[0],
+                        d = n[r] || 0,
+                        u = "".concat(r, " ").concat(d);
+                    n[r] = d + 1;
+                    var c = o(u),
                         p = {
-                            css: r[1],
-                            media: r[2],
-                            sourceMap: r[3]
-                        }; - 1 !== c ? (l[c].references++, l[c].updater(p)) : l.push({
-                        identifier: d,
-                        updater: b(p, t),
+                            css: l[1],
+                            media: l[2],
+                            sourceMap: l[3]
+                        }; - 1 !== c ? (a[c].references++, a[c].updater(p)) : a.push({
+                        identifier: u,
+                        updater: h(p, t),
                         references: 1
-                    }), n.push(d)
+                    }), i.push(u)
                 }
-                return n
+                return i
             }
 
-            function o(e) {
+            function r(e) {
                 var t = document.createElement("style"),
-                    n = e.attributes || {};
-                if (void 0 === n.nonce) {
-                    var l = i.nc;
-                    l && (n.nonce = l)
+                    i = e.attributes || {};
+                if (void 0 === i.nonce) {
+                    var a = n.nc;
+                    a && (i.nonce = a)
                 }
-                if (Object.keys(n).forEach((function(e) {
-                        t.setAttribute(e, n[e])
+                if (Object.keys(i).forEach((function(e) {
+                        t.setAttribute(e, i[e])
                     })), "function" == typeof e.insert) e.insert(t);
                 else {
-                    var a = s(e.insert || "head");
-                    if (!a) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
-                    a.appendChild(t)
+                    var o = s(e.insert || "head");
+                    if (!o) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                    o.appendChild(t)
                 }
                 return t
             }
-            var u, d = (u = [], function(e, t) {
-                return u[e] = t, u.filter(Boolean).join("\n")
+            var d, u = (d = [], function(e, t) {
+                return d[e] = t, d.filter(Boolean).join("\n")
             });
 
-            function c(e, t, i, n) {
-                var s = i ? "" : n.media ? "@media ".concat(n.media, " {").concat(n.css, "}") : n.css;
-                if (e.styleSheet) e.styleSheet.cssText = d(t, s);
+            function c(e, t, n, i) {
+                var s = n ? "" : i.media ? "@media ".concat(i.media, " {").concat(i.css, "}") : i.css;
+                if (e.styleSheet) e.styleSheet.cssText = u(t, s);
                 else {
-                    var l = document.createTextNode(s),
-                        a = e.childNodes;
-                    a[t] && e.removeChild(a[t]), a.length ? e.insertBefore(l, a[t]) : e.appendChild(l)
+                    var a = document.createTextNode(s),
+                        o = e.childNodes;
+                    o[t] && e.removeChild(o[t]), o.length ? e.insertBefore(a, o[t]) : e.appendChild(a)
                 }
             }
 
-            function p(e, t, i) {
-                var n = i.css,
-                    s = i.media,
-                    l = i.sourceMap;
-                if (s ? e.setAttribute("media", s) : e.removeAttribute("media"), l && "undefined" != typeof btoa && (n += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(l)))), " */")), e.styleSheet) e.styleSheet.cssText = n;
+            function p(e, t, n) {
+                var i = n.css,
+                    s = n.media,
+                    a = n.sourceMap;
+                if (s ? e.setAttribute("media", s) : e.removeAttribute("media"), a && "undefined" != typeof btoa && (i += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(a)))), " */")), e.styleSheet) e.styleSheet.cssText = i;
                 else {
                     for (; e.firstChild;) e.removeChild(e.firstChild);
-                    e.appendChild(document.createTextNode(n))
+                    e.appendChild(document.createTextNode(i))
                 }
             }
-            var f = null,
-                m = 0;
+            var m = null,
+                f = 0;
 
-            function b(e, t) {
-                var i, n, s;
+            function h(e, t) {
+                var n, i, s;
                 if (t.singleton) {
-                    var l = m++;
-                    i = f || (f = o(t)), n = c.bind(null, i, l, !1), s = c.bind(null, i, l, !0)
-                } else i = o(t), n = p.bind(null, i, t), s = function() {
+                    var a = f++;
+                    n = m || (m = r(t)), i = c.bind(null, n, a, !1), s = c.bind(null, n, a, !0)
+                } else n = r(t), i = p.bind(null, n, t), s = function() {
                     ! function(e) {
                         if (null === e.parentNode) return !1;
                         e.parentNode.removeChild(e)
-                    }(i)
+                    }(n)
                 };
-                return n(e),
+                return i(e),
                     function(t) {
                         if (t) {
                             if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap) return;
-                            n(e = t)
+                            i(e = t)
                         } else s()
                     }
             }
             e.exports = function(e, t) {
-                (t = t || {}).singleton || "boolean" == typeof t.singleton || (t.singleton = (void 0 === n && (n = Boolean(window && document && document.all && !window.atob)), n));
-                var i = r(e = e || [], t);
+                (t = t || {}).singleton || "boolean" == typeof t.singleton || (t.singleton = (void 0 === i && (i = Boolean(window && document && document.all && !window.atob)), i));
+                var n = l(e = e || [], t);
                 return function(e) {
                     if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
-                        for (var n = 0; n < i.length; n++) {
-                            var s = a(i[n]);
-                            l[s].references--
+                        for (var i = 0; i < n.length; i++) {
+                            var s = o(n[i]);
+                            a[s].references--
                         }
-                        for (var o = r(e, t), u = 0; u < i.length; u++) {
-                            var d = a(i[u]);
-                            0 === l[d].references && (l[d].updater(), l.splice(d, 1))
+                        for (var r = l(e, t), d = 0; d < n.length; d++) {
+                            var u = o(n[d]);
+                            0 === a[u].references && (a[u].updater(), a.splice(u, 1))
                         }
-                        i = o
+                        n = r
                     }
                 }
             }
         },
         147: e => {
             "use strict";
-            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.7","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
+            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.8","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
         }
     }
 ]);
```

### Comparing `ipyfilite-0.1.7/ipyfilite/labextension/static/568.f51073d63c90f5a53748.js` & `ipyfilite-0.1.8/ipyfilite/nbextension/index.js`

 * *Files 19% similar despite different names*

#### js-beautify {}

```diff
@@ -1,315 +1,380 @@
-(self.webpackChunkipyfilite = self.webpackChunkipyfilite || []).push([
-    [568], {
-        568: function(e, t, i) {
-            "use strict";
-            var n = this && this.__createBinding || (Object.create ? function(e, t, i, n) {
-                    void 0 === n && (n = i), Object.defineProperty(e, n, {
-                        enumerable: !0,
-                        get: function() {
-                            return t[i]
+define(["@jupyter-widgets/base"], (e => (() => {
+    var t = {
+            889: (e, t, n) => {
+                (t = n(352)(!1)).push([e.id, ".custom-widget {\n  background-color: lightseagreen;\n  padding: 0px 2px;\n}\n", ""]), e.exports = t
+            },
+            352: e => {
+                "use strict";
+                e.exports = function(e) {
+                    var t = [];
+                    return t.toString = function() {
+                        return this.map((function(t) {
+                            var n = function(e, t) {
+                                var n, i, s, a = e[1] || "",
+                                    o = e[3];
+                                if (!o) return a;
+                                if (t && "function" == typeof btoa) {
+                                    var r = (n = o, i = btoa(unescape(encodeURIComponent(JSON.stringify(n)))), s = "sourceMappingURL=data:application/json;charset=utf-8;base64,".concat(i), "/*# ".concat(s, " */")),
+                                        l = o.sources.map((function(e) {
+                                            return "/*# sourceURL=".concat(o.sourceRoot || "").concat(e, " */")
+                                        }));
+                                    return [a].concat(l).concat([r]).join("\n")
+                                }
+                                return [a].join("\n")
+                            }(t, e);
+                            return t[2] ? "@media ".concat(t[2], " {").concat(n, "}") : n
+                        })).join("")
+                    }, t.i = function(e, n, i) {
+                        "string" == typeof e && (e = [
+                            [null, e, ""]
+                        ]);
+                        var s = {};
+                        if (i)
+                            for (var a = 0; a < this.length; a++) {
+                                var o = this[a][0];
+                                null != o && (s[o] = !0)
+                            }
+                        for (var r = 0; r < e.length; r++) {
+                            var l = [].concat(e[r]);
+                            i && s[l[0]] || (n && (l[2] ? l[2] = "".concat(n, " and ").concat(l[2]) : l[2] = n), t.push(l))
                         }
-                    })
-                } : function(e, t, i, n) {
-                    void 0 === n && (n = i), e[n] = t[i]
-                }),
-                s = this && this.__exportStar || function(e, t) {
-                    for (var i in e) "default" === i || Object.prototype.hasOwnProperty.call(t, i) || n(t, e, i)
-                };
-            Object.defineProperty(t, "__esModule", {
-                value: !0
-            }), s(i(657), t), s(i(367), t)
-        },
-        657: (e, t, i) => {
-            "use strict";
-            Object.defineProperty(t, "__esModule", {
-                value: !0
-            }), t.MODULE_NAME = t.MODULE_VERSION = void 0;
-            const n = i(147);
-            t.MODULE_VERSION = n.version, t.MODULE_NAME = n.name
-        },
-        367: (e, t, i) => {
-            "use strict";
-            Object.defineProperty(t, "__esModule", {
-                value: !0
-            }), t.FileUploadLiteView = t.FileUploadLiteModel = void 0;
-            const n = i(829),
-                s = i(657);
-            i(204);
-            class l extends n.DOMWidgetModel {
-                defaults() {
-                    return Object.assign(Object.assign({}, super.defaults()), {
-                        _model_name: l.model_name,
-                        _model_module: l.model_module,
-                        _model_module_version: l.model_module_version,
-                        _view_name: l.view_name,
-                        _view_module: l.view_module,
-                        _view_module_version: l.view_module_version,
-                        _session: n.uuid(),
-                        accept: "",
-                        description: "Upload",
-                        disabled: !1,
-                        icon: "upload",
-                        button_style: "",
-                        multiple: !1,
-                        value: [],
-                        style: null
-                    })
+                    }, t
                 }
-            }
-            t.FileUploadLiteModel = l, l.serializers = Object.assign(Object.assign({}, n.DOMWidgetModel.serializers), {
-                value: {
-                    serialize: e => e
+            },
+            204: (e, t, n) => {
+                var i = n(379),
+                    s = n(889);
+                "string" == typeof(s = s.__esModule ? s.default : s) && (s = [
+                    [e.id, s, ""]
+                ]);
+                i(s, {
+                    insert: "head",
+                    singleton: !1
+                }), e.exports = s.locals || {}
+            },
+            379: (e, t, n) => {
+                "use strict";
+                var i, s = function() {
+                        var e = {};
+                        return function(t) {
+                            if (void 0 === e[t]) {
+                                var n = document.querySelector(t);
+                                if (window.HTMLIFrameElement && n instanceof window.HTMLIFrameElement) try {
+                                    n = n.contentDocument.head
+                                } catch (e) {
+                                    n = null
+                                }
+                                e[t] = n
+                            }
+                            return e[t]
+                        }
+                    }(),
+                    a = [];
+
+                function o(e) {
+                    for (var t = -1, n = 0; n < a.length; n++)
+                        if (a[n].identifier === e) {
+                            t = n;
+                            break
+                        } return t
                 }
-            }), l.model_name = "FileUploadLiteModel", l.model_module = s.MODULE_NAME, l.model_module_version = s.MODULE_VERSION, l.view_name = "FileUploadLiteView", l.view_module = s.MODULE_NAME, l.view_module_version = s.MODULE_VERSION;
-            class a extends n.DOMWidgetView {
-                preinitialize() {
-                    this.tagName = "button"
+
+                function r(e, t) {
+                    for (var n = {}, i = [], s = 0; s < e.length; s++) {
+                        var r = e[s],
+                            l = t.base ? r[0] + t.base : r[0],
+                            d = n[l] || 0,
+                            u = "".concat(l, " ").concat(d);
+                        n[l] = d + 1;
+                        var c = o(u),
+                            p = {
+                                css: r[1],
+                                media: r[2],
+                                sourceMap: r[3]
+                            }; - 1 !== c ? (a[c].references++, a[c].updater(p)) : a.push({
+                            identifier: u,
+                            updater: h(p, t),
+                            references: 1
+                        }), i.push(u)
+                    }
+                    return i
                 }
-                render() {
-                    super.render(), this.el.classList.add("jupyter-widgets"), this.el.classList.add("widget-upload-lite"), this.el.classList.add("jupyter-button"), this.fileInput = document.createElement("input"), this.fileInput.type = "file", this.fileInput.style.display = "none", this.el.addEventListener("click", (() => {
-                        this.fileInput.click()
-                    })), this.fileInput.addEventListener("click", (() => {
-                        this.fileInput.value = ""
-                    })), this.fileInput.addEventListener("change", (() => {
-                        var e;
-                        const t = n.uuid(),
-                            i = Array.from(null !== (e = this.fileInput.files) && void 0 !== e ? e : []).map((e => ({
-                                name: e.name,
-                                type: e.type,
-                                size: e.size,
-                                last_modified: e.lastModified,
-                                path: `/uploads/${t}/${e.name}`
-                            })));
-                        o.getBroadcastChannel().postMessage({
-                            files: this.fileInput.files,
-                            uuid: t,
-                            session: this.model.get("_session"),
-                            widget: this.model.model_id
-                        }), this.model.set({
-                            value: i
-                        }), this.touch()
-                    })), this.listenTo(this.model, "change:button_style", this.update_button_style), this.set_button_style(), this.update()
+
+                function l(e) {
+                    var t = document.createElement("style"),
+                        i = e.attributes || {};
+                    if (void 0 === i.nonce) {
+                        var a = n.nc;
+                        a && (i.nonce = a)
+                    }
+                    if (Object.keys(i).forEach((function(e) {
+                            t.setAttribute(e, i[e])
+                        })), "function" == typeof e.insert) e.insert(t);
+                    else {
+                        var o = s(e.insert || "head");
+                        if (!o) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
+                        o.appendChild(t)
+                    }
+                    return t
                 }
-                update() {
-                    this.el.disabled = this.model.get("disabled"), this.el.setAttribute("title", this.model.get("tooltip"));
-                    const e = this.model.get("value"),
-                        t = `${this.model.get("description")} (${e.length})`,
-                        i = this.model.get("icon");
-                    if (t.length || i.length) {
-                        if (this.el.textContent = "", i.length) {
-                            const e = document.createElement("i");
-                            e.classList.add("fa"), e.classList.add("fa-" + i), 0 === t.length && e.classList.add("center"), this.el.appendChild(e)
-                        }
-                        this.el.appendChild(document.createTextNode(t))
+                var d, u = (d = [], function(e, t) {
+                    return d[e] = t, d.filter(Boolean).join("\n")
+                });
+
+                function c(e, t, n, i) {
+                    var s = n ? "" : i.media ? "@media ".concat(i.media, " {").concat(i.css, "}") : i.css;
+                    if (e.styleSheet) e.styleSheet.cssText = u(t, s);
+                    else {
+                        var a = document.createTextNode(s),
+                            o = e.childNodes;
+                        o[t] && e.removeChild(o[t]), o.length ? e.insertBefore(a, o[t]) : e.appendChild(a)
                     }
-                    return this.fileInput.accept = this.model.get("accept"), this.fileInput.multiple = this.model.get("multiple"), super.update()
                 }
-                update_button_style() {
-                    this.update_mapped_classes(a.class_map, "button_style", this.el)
+
+                function p(e, t, n) {
+                    var i = n.css,
+                        s = n.media,
+                        a = n.sourceMap;
+                    if (s ? e.setAttribute("media", s) : e.removeAttribute("media"), a && "undefined" != typeof btoa && (i += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(a)))), " */")), e.styleSheet) e.styleSheet.cssText = i;
+                    else {
+                        for (; e.firstChild;) e.removeChild(e.firstChild);
+                        e.appendChild(document.createTextNode(i))
+                    }
                 }
-                set_button_style() {
-                    this.set_mapped_classes(a.class_map, "button_style", this.el)
+                var f = null,
+                    m = 0;
+
+                function h(e, t) {
+                    var n, i, s;
+                    if (t.singleton) {
+                        var a = m++;
+                        n = f || (f = l(t)), i = c.bind(null, n, a, !1), s = c.bind(null, n, a, !0)
+                    } else n = l(t), i = p.bind(null, n, t), s = function() {
+                        ! function(e) {
+                            if (null === e.parentNode) return !1;
+                            e.parentNode.removeChild(e)
+                        }(n)
+                    };
+                    return i(e),
+                        function(t) {
+                            if (t) {
+                                if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap) return;
+                                i(e = t)
+                            } else s()
+                        }
                 }
-            }
-            var o;
-            t.FileUploadLiteView = a, a.class_map = {
-                    primary: ["mod-primary"],
-                    success: ["mod-success"],
-                    info: ["mod-info"],
-                    warning: ["mod-warning"],
-                    danger: ["mod-danger"]
-                },
-                function(e) {
-                    const t = new BroadcastChannel("ipyfilite");
-                    e.getBroadcastChannel = function() {
-                        return t
-                    }
-                }(o || (o = {}))
-        },
-        889: (e, t, i) => {
-            (t = i(645)(!1)).push([e.id, ".custom-widget {\n  background-color: lightseagreen;\n  padding: 0px 2px;\n}\n", ""]), e.exports = t
-        },
-        645: e => {
-            "use strict";
-            e.exports = function(e) {
-                var t = [];
-                return t.toString = function() {
-                    return this.map((function(t) {
-                        var i = function(e, t) {
-                            var i, n, s, l = e[1] || "",
-                                a = e[3];
-                            if (!a) return l;
-                            if (t && "function" == typeof btoa) {
-                                var o = (i = a, n = btoa(unescape(encodeURIComponent(JSON.stringify(i)))), s = "sourceMappingURL=data:application/json;charset=utf-8;base64,".concat(n), "/*# ".concat(s, " */")),
-                                    r = a.sources.map((function(e) {
-                                        return "/*# sourceURL=".concat(a.sourceRoot || "").concat(e, " */")
-                                    }));
-                                return [l].concat(r).concat([o]).join("\n")
+                e.exports = function(e, t) {
+                    (t = t || {}).singleton || "boolean" == typeof t.singleton || (t.singleton = (void 0 === i && (i = Boolean(window && document && document.all && !window.atob)), i));
+                    var n = r(e = e || [], t);
+                    return function(e) {
+                        if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
+                            for (var i = 0; i < n.length; i++) {
+                                var s = o(n[i]);
+                                a[s].references--
                             }
-                            return [l].join("\n")
-                        }(t, e);
-                        return t[2] ? "@media ".concat(t[2], " {").concat(i, "}") : i
-                    })).join("")
-                }, t.i = function(e, i, n) {
-                    "string" == typeof e && (e = [
-                        [null, e, ""]
-                    ]);
-                    var s = {};
-                    if (n)
-                        for (var l = 0; l < this.length; l++) {
-                            var a = this[l][0];
-                            null != a && (s[a] = !0)
-                        }
-                    for (var o = 0; o < e.length; o++) {
-                        var r = [].concat(e[o]);
-                        n && s[r[0]] || (i && (r[2] ? r[2] = "".concat(i, " and ").concat(r[2]) : r[2] = i), t.push(r))
-                    }
-                }, t
-            }
-        },
-        204: (e, t, i) => {
-            var n = i(379),
-                s = i(889);
-            "string" == typeof(s = s.__esModule ? s.default : s) && (s = [
-                [e.id, s, ""]
-            ]);
-            n(s, {
-                insert: "head",
-                singleton: !1
-            }), e.exports = s.locals || {}
-        },
-        379: (e, t, i) => {
-            "use strict";
-            var n, s = function() {
-                    var e = {};
-                    return function(t) {
-                        if (void 0 === e[t]) {
-                            var i = document.querySelector(t);
-                            if (window.HTMLIFrameElement && i instanceof window.HTMLIFrameElement) try {
-                                i = i.contentDocument.head
-                            } catch (e) {
-                                i = null
+                            for (var l = r(e, t), d = 0; d < n.length; d++) {
+                                var u = o(n[d]);
+                                0 === a[u].references && (a[u].updater(), a.splice(u, 1))
                             }
-                            e[t] = i
+                            n = l
                         }
-                        return e[t]
                     }
-                }(),
-                l = [];
-
-            function a(e) {
-                for (var t = -1, i = 0; i < l.length; i++)
-                    if (l[i].identifier === e) {
-                        t = i;
-                        break
-                    } return t
-            }
-
-            function o(e, t) {
-                for (var i = {}, n = [], s = 0; s < e.length; s++) {
-                    var o = e[s],
-                        r = t.base ? o[0] + t.base : o[0],
-                        d = i[r] || 0,
-                        u = "".concat(r, " ").concat(d);
-                    i[r] = d + 1;
-                    var c = a(u),
-                        p = {
-                            css: o[1],
-                            media: o[2],
-                            sourceMap: o[3]
-                        }; - 1 !== c ? (l[c].references++, l[c].updater(p)) : l.push({
-                        identifier: u,
-                        updater: b(p, t),
-                        references: 1
-                    }), n.push(u)
-                }
-                return n
-            }
-
-            function r(e) {
-                var t = document.createElement("style"),
-                    n = e.attributes || {};
-                if (void 0 === n.nonce) {
-                    var l = i.nc;
-                    l && (n.nonce = l)
-                }
-                if (Object.keys(n).forEach((function(e) {
-                        t.setAttribute(e, n[e])
-                    })), "function" == typeof e.insert) e.insert(t);
-                else {
-                    var a = s(e.insert || "head");
-                    if (!a) throw new Error("Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.");
-                    a.appendChild(t)
-                }
-                return t
-            }
-            var d, u = (d = [], function(e, t) {
-                return d[e] = t, d.filter(Boolean).join("\n")
-            });
-
-            function c(e, t, i, n) {
-                var s = i ? "" : n.media ? "@media ".concat(n.media, " {").concat(n.css, "}") : n.css;
-                if (e.styleSheet) e.styleSheet.cssText = u(t, s);
-                else {
-                    var l = document.createTextNode(s),
-                        a = e.childNodes;
-                    a[t] && e.removeChild(a[t]), a.length ? e.insertBefore(l, a[t]) : e.appendChild(l)
                 }
-            }
-
-            function p(e, t, i) {
-                var n = i.css,
-                    s = i.media,
-                    l = i.sourceMap;
-                if (s ? e.setAttribute("media", s) : e.removeAttribute("media"), l && "undefined" != typeof btoa && (n += "\n/*# sourceMappingURL=data:application/json;base64,".concat(btoa(unescape(encodeURIComponent(JSON.stringify(l)))), " */")), e.styleSheet) e.styleSheet.cssText = n;
-                else {
-                    for (; e.firstChild;) e.removeChild(e.firstChild);
-                    e.appendChild(document.createTextNode(n))
+            },
+            112: function(e, t, n) {
+                "use strict";
+                var i = this && this.__createBinding || (Object.create ? function(e, t, n, i) {
+                        void 0 === i && (i = n), Object.defineProperty(e, i, {
+                            enumerable: !0,
+                            get: function() {
+                                return t[n]
+                            }
+                        })
+                    } : function(e, t, n, i) {
+                        void 0 === i && (i = n), e[i] = t[n]
+                    }),
+                    s = this && this.__exportStar || function(e, t) {
+                        for (var n in e) "default" === n || Object.prototype.hasOwnProperty.call(t, n) || i(t, e, n)
+                    };
+                Object.defineProperty(t, "__esModule", {
+                    value: !0
+                }), window.__webpack_public_path__ = document.querySelector("body").getAttribute("data-base-url") + "nbextensions/ipyfilite", s(n(607), t)
+            },
+            607: function(e, t, n) {
+                "use strict";
+                var i = this && this.__createBinding || (Object.create ? function(e, t, n, i) {
+                        void 0 === i && (i = n), Object.defineProperty(e, i, {
+                            enumerable: !0,
+                            get: function() {
+                                return t[n]
+                            }
+                        })
+                    } : function(e, t, n, i) {
+                        void 0 === i && (i = n), e[i] = t[n]
+                    }),
+                    s = this && this.__exportStar || function(e, t) {
+                        for (var n in e) "default" === n || Object.prototype.hasOwnProperty.call(t, n) || i(t, e, n)
+                    };
+                Object.defineProperty(t, "__esModule", {
+                    value: !0
+                }), s(n(412), t), s(n(891), t)
+            },
+            412: (e, t, n) => {
+                "use strict";
+                Object.defineProperty(t, "__esModule", {
+                    value: !0
+                }), t.MODULE_NAME = t.MODULE_VERSION = void 0;
+                const i = n(147);
+                t.MODULE_VERSION = i.version, t.MODULE_NAME = i.name
+            },
+            891: (e, t, n) => {
+                "use strict";
+                Object.defineProperty(t, "__esModule", {
+                    value: !0
+                }), t.FileUploadLiteView = t.FileUploadLiteModel = void 0;
+                const i = n(146),
+                    s = n(412);
+                n(204);
+                class a extends i.DOMWidgetModel {
+                    defaults() {
+                        return Object.assign(Object.assign({}, super.defaults()), {
+                            _model_name: a.model_name,
+                            _model_module: a.model_module,
+                            _model_module_version: a.model_module_version,
+                            _view_name: a.view_name,
+                            _view_module: a.view_module,
+                            _view_module_version: a.view_module_version,
+                            _session: i.uuid(),
+                            accept: "",
+                            description: "Upload",
+                            disabled: !1,
+                            icon: "upload",
+                            button_style: "",
+                            multiple: !1,
+                            value: [],
+                            style: null
+                        })
+                    }
                 }
-            }
-            var f = null,
-                m = 0;
-
-            function b(e, t) {
-                var i, n, s;
-                if (t.singleton) {
-                    var l = m++;
-                    i = f || (f = r(t)), n = c.bind(null, i, l, !1), s = c.bind(null, i, l, !0)
-                } else i = r(t), n = p.bind(null, i, t), s = function() {
-                    ! function(e) {
-                        if (null === e.parentNode) return !1;
-                        e.parentNode.removeChild(e)
-                    }(i)
-                };
-                return n(e),
-                    function(t) {
-                        if (t) {
-                            if (t.css === e.css && t.media === e.media && t.sourceMap === e.sourceMap) return;
-                            n(e = t)
-                        } else s()
+                t.FileUploadLiteModel = a, a.serializers = Object.assign(Object.assign({}, i.DOMWidgetModel.serializers), {
+                    value: {
+                        serialize: e => e
                     }
-            }
-            e.exports = function(e, t) {
-                (t = t || {}).singleton || "boolean" == typeof t.singleton || (t.singleton = (void 0 === n && (n = Boolean(window && document && document.all && !window.atob)), n));
-                var i = o(e = e || [], t);
-                return function(e) {
-                    if (e = e || [], "[object Array]" === Object.prototype.toString.call(e)) {
-                        for (var n = 0; n < i.length; n++) {
-                            var s = a(i[n]);
-                            l[s].references--
-                        }
-                        for (var r = o(e, t), d = 0; d < i.length; d++) {
-                            var u = a(i[d]);
-                            0 === l[u].references && (l[u].updater(), l.splice(u, 1))
+                }), a.model_name = "FileUploadLiteModel", a.model_module = s.MODULE_NAME, a.model_module_version = s.MODULE_VERSION, a.view_name = "FileUploadLiteView", a.view_module = s.MODULE_NAME, a.view_module_version = s.MODULE_VERSION;
+                class o extends i.DOMWidgetView {
+                    preinitialize() {
+                        this.tagName = "button"
+                    }
+                    render() {
+                        super.render(), this.el.classList.add("jupyter-widgets"), this.el.classList.add("widget-upload-lite"), this.el.classList.add("jupyter-button"), this.fileInput = document.createElement("input"), this.fileInput.type = "file", this.fileInput.style.display = "none", this.el.addEventListener("click", (() => {
+                            this.fileInput.click()
+                        })), this.fileInput.addEventListener("click", (() => {
+                            this.fileInput.value = ""
+                        })), this.fileInput.addEventListener("change", (() => {
+                            var e;
+                            const t = i.uuid(),
+                                n = Array.from(null !== (e = this.fileInput.files) && void 0 !== e ? e : []).map((e => ({
+                                    name: e.name,
+                                    type: e.type,
+                                    size: e.size,
+                                    last_modified: e.lastModified,
+                                    path: `/uploads/${t}/${e.name}`
+                                })));
+                            r.getBroadcastChannel().postMessage({
+                                kind: "upload",
+                                files: this.fileInput.files,
+                                uuid: t,
+                                session: this.model.get("_session"),
+                                widget: this.model.model_id
+                            }), this.model.set({
+                                value: n
+                            }), this.touch()
+                        })), this.listenTo(this.model, "change:button_style", this.update_button_style), this.set_button_style(), this.update()
+                    }
+                    update() {
+                        this.el.disabled = this.model.get("disabled"), this.el.setAttribute("title", this.model.get("tooltip"));
+                        const e = this.model.get("value"),
+                            t = `${this.model.get("description")} (${e.length})`,
+                            n = this.model.get("icon");
+                        if (t.length || n.length) {
+                            if (this.el.textContent = "", n.length) {
+                                const e = document.createElement("i");
+                                e.classList.add("fa"), e.classList.add("fa-" + n), 0 === t.length && e.classList.add("center"), this.el.appendChild(e)
+                            }
+                            this.el.appendChild(document.createTextNode(t))
                         }
-                        i = r
+                        return this.fileInput.accept = this.model.get("accept"), this.fileInput.multiple = this.model.get("multiple"), super.update()
+                    }
+                    update_button_style() {
+                        this.update_mapped_classes(o.class_map, "button_style", this.el)
+                    }
+                    set_button_style() {
+                        this.set_mapped_classes(o.class_map, "button_style", this.el)
                     }
                 }
+                var r;
+                t.FileUploadLiteView = o, o.class_map = {
+                        primary: ["mod-primary"],
+                        success: ["mod-success"],
+                        info: ["mod-info"],
+                        warning: ["mod-warning"],
+                        danger: ["mod-danger"]
+                    },
+                    function(e) {
+                        const t = new BroadcastChannel("ipyfilite");
+
+                        function n(e, t) {
+                            const n = document.createElement("a");
+                            n.href = URL.createObjectURL(new Blob(t)), n.download = e, n.click()
+                        }
+                        e.getBroadcastChannel = function() {
+                            return t
+                        };
+                        const i = new Map;
+                        t.onmessage = function(e) {
+                            if (e.data && e.data.kind)
+                                if ("download-open" === e.data.kind) {
+                                    if (i.has(e.data.uuid)) return void console.warn(`Download stream for '${e.data.uuid}' already open.`);
+                                    i.set(e.data.uuid, {
+                                        name: e.data.name,
+                                        chunks: [],
+                                        size: 0,
+                                        segment: 0
+                                    })
+                                } else if ("download-chunk" === e.data.kind) {
+                                if (!i.has(e.data.uuid)) return void console.warn(`No download stream for '${e.data.uuid}' is open to write to.`);
+                                const t = i.get(e.data.uuid),
+                                    s = new Uint8Array(e.data.chunk);
+                                t.chunks.push(s), t.size += s.length, t.size >= 268435456 && (t.segment += 1, n(`${t.name}.${t.segment.toString().padStart(3,"0")}`, t.chunks), t.chunks = [], t.size = 0)
+                            } else if ("download-close" === e.data.kind) {
+                                if (!i.has(e.data.uuid)) return void console.warn(`No download stream for '${e.data.uuid}' is open to close.`);
+                                const t = i.get(e.data.uuid);
+                                if (i.delete(e.data.uuid), t.segment > 0 && 0 === t.chunks.length) return;
+                                t.segment > 0 ? (t.segment += 1, n(`${t.name}.${t.segment.toString().padStart(3,"0")}`, t.chunks)) : n(t.name, t.chunks)
+                            }
+                        }
+                    }(r || (r = {}))
+            },
+            146: t => {
+                "use strict";
+                t.exports = e
+            },
+            147: e => {
+                "use strict";
+                e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.8","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
             }
         },
-        147: e => {
-            "use strict";
-            e.exports = JSON.parse('{"name":"ipyfilite","version":"0.1.7","description":"File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.","keywords":["jupyter","jupyterlab","jupyterlab-extension","widgets"],"files":["lib/**/*.js","dist/*.js","css/*.css"],"homepage":"https://github.com/juntyr/ipyfilite","bugs":{"url":"https://github.com/juntyr/ipyfilite/issues"},"license":"BSD-3-Clause","author":{"name":"Juniper Tyree","email":"juniper.tyree@helsinki.fi"},"main":"lib/index.js","types":"./lib/index.d.ts","repository":{"type":"git","url":"https://github.com/juntyr/ipyfilite"},"scripts":{"build":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension:dev","build:prod":"yarn run build:lib && yarn run build:nbextension && yarn run build:labextension","build:labextension":"jupyter labextension build .","build:labextension:dev":"jupyter labextension build --development True .","build:lib":"tsc","build:nbextension":"webpack","clean":"yarn run clean:lib && yarn run clean:nbextension && yarn run clean:labextension","clean:lib":"rimraf lib","clean:labextension":"rimraf ipyfilite/labextension","clean:nbextension":"rimraf ipyfilite/nbextension/static/index.js","lint":"eslint . --ext .ts,.tsx --fix","lint:check":"eslint . --ext .ts,.tsx","prepack":"yarn run build:lib","test":"jest","watch":"npm-run-all -p watch:*","watch:lib":"tsc -w","watch:nbextension":"webpack --watch --mode=development","watch:labextension":"jupyter labextension watch ."},"dependencies":{"@jupyter-widgets/base":"^1.1.10 || ^2 || ^3 || ^4 || ^5 || ^6"},"devDependencies":{"@babel/core":"^7.5.0","@babel/preset-env":"^7.5.0","@jupyter-widgets/base-manager":"^1.0.2","@jupyterlab/builder":"^3.0.0","@lumino/application":"^1.6.0","@lumino/widgets":"^1.6.0","@types/jest":"^26.0.0","@types/webpack-env":"^1.13.6","@typescript-eslint/eslint-plugin":"^3.6.0","@typescript-eslint/parser":"^3.6.0","acorn":"^7.2.0","css-loader":"^3.2.0","eslint":"^7.4.0","eslint-config-prettier":"^6.11.0","eslint-plugin-prettier":"^3.1.4","fs-extra":"^7.0.0","identity-obj-proxy":"^3.0.0","jest":"^26.0.0","mkdirp":"^0.5.1","npm-run-all":"^4.1.3","prettier":"^2.0.5","rimraf":"^2.6.2","source-map-loader":"^1.1.3","style-loader":"^1.0.0","ts-jest":"^26.0.0","ts-loader":"^8.0.0","typescript":"~4.1.3","webpack":"^5.61.0","webpack-cli":"^4.0.0"},"jupyterlab":{"extension":"lib/plugin","outputDir":"ipyfilite/labextension/","sharedPackages":{"@jupyter-widgets/base":{"bundled":false,"singleton":true}}}}')
-        }
+        n = {};
+
+    function i(e) {
+        var s = n[e];
+        if (void 0 !== s) return s.exports;
+        var a = n[e] = {
+            id: e,
+            exports: {}
+        };
+        return t[e].call(a.exports, a, a.exports, i), a.exports
     }
-]);
+    return i.nc = void 0, i(112)
+})()));
+//# sourceMappingURL=index.js.map
```

### Comparing `ipyfilite-0.1.7/ipyfilite/labextension/static/remoteEntry.2c0ba414ad48ffdc77a7.js` & `ipyfilite-0.1.8/ipyfilite/labextension/static/remoteEntry.7fc7bd0e9744231b6636.js`

 * *Files 9% similar despite different names*

#### js-beautify {}

```diff
@@ -1,15 +1,15 @@
 var _JUPYTERLAB;
 (() => {
     "use strict";
-    var e, r, t, n, i, o, a, l, f, u, s, d, p, c, h, v, b = {
+    var e, r, t, n, i, o, a, l, u, f, s, d, p, c, h, v, g = {
             229: (e, r, t) => {
                 var n = {
-                        "./index": () => Promise.all([t.e(829), t.e(568)]).then((() => () => t(568))),
-                        "./extension": () => Promise.all([t.e(829), t.e(480)]).then((() => () => t(480)))
+                        "./index": () => Promise.all([t.e(367), t.e(568)]).then((() => () => t(568))),
+                        "./extension": () => Promise.all([t.e(367), t.e(480)]).then((() => () => t(480)))
                     },
                     i = (e, r) => (t.R = r, r = t.o(n, e) ? n[e]() : Promise.resolve().then((() => {
                         throw new Error('Module "' + e + '" does not exist in container.')
                     })), t.R = void 0, r),
                     o = (e, r) => {
                         if (t.S) {
                             var n = "default",
@@ -20,104 +20,104 @@
                     };
                 t.d(r, {
                     get: () => i,
                     init: () => o
                 })
             }
         },
-        g = {};
+        m = {};
 
-    function m(e) {
-        var r = g[e];
+    function b(e) {
+        var r = m[e];
         if (void 0 !== r) return r.exports;
-        var t = g[e] = {
+        var t = m[e] = {
             id: e,
             exports: {}
         };
-        return b[e].call(t.exports, t, t.exports, m), t.exports
+        return g[e].call(t.exports, t, t.exports, b), t.exports
     }
-    m.m = b, m.c = g, m.d = (e, r) => {
-        for (var t in r) m.o(r, t) && !m.o(e, t) && Object.defineProperty(e, t, {
+    b.m = g, b.c = m, b.d = (e, r) => {
+        for (var t in r) b.o(r, t) && !b.o(e, t) && Object.defineProperty(e, t, {
             enumerable: !0,
             get: r[t]
         })
-    }, m.f = {}, m.e = e => Promise.all(Object.keys(m.f).reduce(((r, t) => (m.f[t](e, r), r)), [])), m.u = e => e + "." + {
-        480: "522a35aad26b3baab1ae",
-        568: "f51073d63c90f5a53748",
-        829: "eddb7a59a74d60740eb9"
+    }, b.f = {}, b.e = e => Promise.all(Object.keys(b.f).reduce(((r, t) => (b.f[t](e, r), r)), [])), b.u = e => e + "." + {
+        367: "2b53dbfb84806314e897",
+        480: "d744653fa4c869369de5",
+        568: "1f78854f2c5197037e64"
     } [e] + ".js?v=" + {
-        480: "522a35aad26b3baab1ae",
-        568: "f51073d63c90f5a53748",
-        829: "eddb7a59a74d60740eb9"
-    } [e], m.g = function() {
+        367: "2b53dbfb84806314e897",
+        480: "d744653fa4c869369de5",
+        568: "1f78854f2c5197037e64"
+    } [e], b.g = function() {
         if ("object" == typeof globalThis) return globalThis;
         try {
             return this || new Function("return this")()
         } catch (e) {
             if ("object" == typeof window) return window
         }
-    }(), m.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyfilite:", m.l = (t, n, i, o) => {
+    }(), b.o = (e, r) => Object.prototype.hasOwnProperty.call(e, r), e = {}, r = "ipyfilite:", b.l = (t, n, i, o) => {
         if (e[t]) e[t].push(n);
         else {
             var a, l;
             if (void 0 !== i)
-                for (var f = document.getElementsByTagName("script"), u = 0; u < f.length; u++) {
-                    var s = f[u];
+                for (var u = document.getElementsByTagName("script"), f = 0; f < u.length; f++) {
+                    var s = u[f];
                     if (s.getAttribute("src") == t || s.getAttribute("data-webpack") == r + i) {
                         a = s;
                         break
                     }
                 }
-            a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, m.nc && a.setAttribute("nonce", m.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
+            a || (l = !0, (a = document.createElement("script")).charset = "utf-8", a.timeout = 120, b.nc && a.setAttribute("nonce", b.nc), a.setAttribute("data-webpack", r + i), a.src = t), e[t] = [n];
             var d = (r, n) => {
                     a.onerror = a.onload = null, clearTimeout(p);
                     var i = e[t];
                     if (delete e[t], a.parentNode && a.parentNode.removeChild(a), i && i.forEach((e => e(n))), r) return r(n)
                 },
                 p = setTimeout(d.bind(null, void 0, {
                     type: "timeout",
                     target: a
                 }), 12e4);
             a.onerror = d.bind(null, a.onerror), a.onload = d.bind(null, a.onload), l && document.head.appendChild(a)
         }
     }, (() => {
-        m.S = {};
+        b.S = {};
         var e = {},
             r = {};
-        m.I = (t, n) => {
+        b.I = (t, n) => {
             n || (n = []);
             var i = r[t];
             if (i || (i = r[t] = {}), !(n.indexOf(i) >= 0)) {
                 if (n.push(i), e[t]) return e[t];
-                m.o(m.S, t) || (m.S[t] = {});
-                var o = m.S[t],
+                b.o(b.S, t) || (b.S[t] = {});
+                var o = b.S[t],
                     a = "ipyfilite",
                     l = [];
                 return "default" === t && ((e, r, t, n) => {
                     var i = o[e] = o[e] || {},
                         l = i[r];
                     (!l || !l.loaded && (1 != !l.eager ? n : a > l.from)) && (i[r] = {
-                        get: () => Promise.all([m.e(829), m.e(568)]).then((() => () => m(568))),
+                        get: () => Promise.all([b.e(367), b.e(568)]).then((() => () => b(568))),
                         from: a,
                         eager: !1
                     })
-                })("ipyfilite", "0.1.7"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
+                })("ipyfilite", "0.1.8"), e[t] = l.length ? Promise.all(l).then((() => e[t] = 1)) : 1
             }
         }
     })(), (() => {
         var e;
-        m.g.importScripts && (e = m.g.location + "");
-        var r = m.g.document;
+        b.g.importScripts && (e = b.g.location + "");
+        var r = b.g.document;
         if (!e && r && (r.currentScript && (e = r.currentScript.src), !e)) {
             var t = r.getElementsByTagName("script");
             if (t.length)
                 for (var n = t.length - 1; n > -1 && !e;) e = t[n--].src
         }
         if (!e) throw new Error("Automatic publicPath is not supported in this browser");
-        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), m.p = e
+        e = e.replace(/#.*$/, "").replace(/\?.*$/, "").replace(/\/[^\/]+$/, "/"), b.p = e
     })(), t = e => {
         var r = e => e.split(".").map((e => +e == e ? +e : e)),
             t = /^([^-+]+)?(?:-([^+]+))?(?:\+(.+))?$/.exec(e),
             n = t[1] ? r(t[1]) : [];
         return t[2] && (n.length++, n.push.apply(n, r(t[2]))), t[3] && (n.push([]), n.push.apply(n, r(t[3]))), n
     }, n = (e, r) => {
         e = t(e), r = t(r);
@@ -140,131 +140,131 @@
             t += 0 == r ? ">=" : -1 == r ? "<" : 1 == r ? "^" : 2 == r ? "~" : r > 0 ? "=" : "!=";
             for (var n = 1, o = 1; o < e.length; o++) n--, t += "u" == (typeof(l = e[o]))[0] ? "-" : (n > 0 ? "." : "") + (n = 2, l);
             return t
         }
         var a = [];
         for (o = 1; o < e.length; o++) {
             var l = e[o];
-            a.push(0 === l ? "not(" + f() + ")" : 1 === l ? "(" + f() + " || " + f() + ")" : 2 === l ? a.pop() + " " + a.pop() : i(l))
+            a.push(0 === l ? "not(" + u() + ")" : 1 === l ? "(" + u() + " || " + u() + ")" : 2 === l ? a.pop() + " " + a.pop() : i(l))
         }
-        return f();
+        return u();
 
-        function f() {
+        function u() {
             return a.pop().replace(/^\((.+)\)$/, "$1")
         }
     }, o = (e, r) => {
         if (0 in e) {
             r = t(r);
             var n = e[0],
                 i = n < 0;
             i && (n = -n - 1);
-            for (var a = 0, l = 1, f = !0;; l++, a++) {
-                var u, s, d = l < e.length ? (typeof e[l])[0] : "";
-                if (a >= r.length || "o" == (s = (typeof(u = r[a]))[0])) return !f || ("u" == d ? l > n && !i : "" == d != i);
+            for (var a = 0, l = 1, u = !0;; l++, a++) {
+                var f, s, d = l < e.length ? (typeof e[l])[0] : "";
+                if (a >= r.length || "o" == (s = (typeof(f = r[a]))[0])) return !u || ("u" == d ? l > n && !i : "" == d != i);
                 if ("u" == s) {
-                    if (!f || "u" != d) return !1
-                } else if (f)
+                    if (!u || "u" != d) return !1
+                } else if (u)
                     if (d == s)
                         if (l <= n) {
-                            if (u != e[l]) return !1
+                            if (f != e[l]) return !1
                         } else {
-                            if (i ? u > e[l] : u < e[l]) return !1;
-                            u != e[l] && (f = !1)
+                            if (i ? f > e[l] : f < e[l]) return !1;
+                            f != e[l] && (u = !1)
                         }
                 else if ("s" != d && "n" != d) {
                     if (i || l <= n) return !1;
-                    f = !1, l--
+                    u = !1, l--
                 } else {
                     if (l <= n || s < d != i) return !1;
-                    f = !1
-                } else "s" != d && "n" != d && (f = !1, l--)
+                    u = !1
+                } else "s" != d && "n" != d && (u = !1, l--)
             }
         }
         var p = [],
             c = p.pop.bind(p);
         for (a = 1; a < e.length; a++) {
             var h = e[a];
             p.push(1 == h ? c() | c() : 2 == h ? c() & c() : h ? o(h, r) : !c())
         }
         return !!c()
     }, a = (e, r) => {
-        var t = m.S[e];
-        if (!t || !m.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
+        var t = b.S[e];
+        if (!t || !b.o(t, r)) throw new Error("Shared module " + r + " doesn't exist in shared scope " + e);
         return t
     }, l = (e, r) => {
         var t = e[r];
         return Object.keys(t).reduce(((e, r) => !e || !t[e].loaded && n(e, r) ? r : e), 0)
-    }, f = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", u = (e, r, t, n) => {
+    }, u = (e, r, t, n) => "Unsatisfied version " + t + " from " + (t && e[r][t].from) + " of shared singleton module " + r + " (required " + i(n) + ")", f = (e, r, t, n) => {
         var i = l(e, t);
-        return o(n, i) || s(f(e, t, i, n)), d(e[t][i])
+        return o(n, i) || s(u(e, t, i, n)), d(e[t][i])
     }, s = e => {
         "undefined" != typeof console && console.warn && console.warn(e)
     }, d = e => (e.loaded = 1, e.get()), p = (e => function(r, t, n, i) {
-        var o = m.I(r);
-        return o && o.then ? o.then(e.bind(e, r, m.S[r], t, n, i)) : e(r, m.S[r], t, n)
-    })(((e, r, t, n) => (a(e, t), u(r, 0, t, n)))), c = {}, h = {
+        var o = b.I(r);
+        return o && o.then ? o.then(e.bind(e, r, b.S[r], t, n, i)) : e(r, b.S[r], t, n)
+    })(((e, r, t, n) => (a(e, t), f(r, 0, t, n)))), c = {}, h = {
         829: () => p("default", "@jupyter-widgets/base", [, [1, 6],
             [1, 5],
             [1, 4],
             [1, 3],
             [1, 2],
             [1, 1, 1, 10], 1, 1, 1, 1, 1
         ])
     }, v = {
-        829: [829]
-    }, m.f.consumes = (e, r) => {
-        m.o(v, e) && v[e].forEach((e => {
-            if (m.o(c, e)) return r.push(c[e]);
+        367: [829]
+    }, b.f.consumes = (e, r) => {
+        b.o(v, e) && v[e].forEach((e => {
+            if (b.o(c, e)) return r.push(c[e]);
             var t = r => {
-                    c[e] = 0, m.m[e] = t => {
-                        delete m.c[e], t.exports = r()
+                    c[e] = 0, b.m[e] = t => {
+                        delete b.c[e], t.exports = r()
                     }
                 },
                 n = r => {
-                    delete c[e], m.m[e] = t => {
-                        throw delete m.c[e], r
+                    delete c[e], b.m[e] = t => {
+                        throw delete b.c[e], r
                     }
                 };
             try {
                 var i = h[e]();
                 i.then ? r.push(c[e] = i.then(t).catch(n)) : t(i)
             } catch (e) {
                 n(e)
             }
         }))
     }, (() => {
         var e = {
             430: 0
         };
-        m.f.j = (r, t) => {
-            var n = m.o(e, r) ? e[r] : void 0;
+        b.f.j = (r, t) => {
+            var n = b.o(e, r) ? e[r] : void 0;
             if (0 !== n)
                 if (n) t.push(n[2]);
-                else if (829 != r) {
-                var i = new Promise(((t, i) => n = e[r] = [t, i]));
-                t.push(n[2] = i);
-                var o = m.p + m.u(r),
-                    a = new Error;
-                m.l(o, (t => {
-                    if (m.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
-                        var i = t && ("load" === t.type ? "missing" : t.type),
-                            o = t && t.target && t.target.src;
-                        a.message = "Loading chunk " + r + " failed.\n(" + i + ": " + o + ")", a.name = "ChunkLoadError", a.type = i, a.request = o, n[1](a)
-                    }
-                }), "chunk-" + r, r)
-            } else e[r] = 0
+                else {
+                    var i = new Promise(((t, i) => n = e[r] = [t, i]));
+                    t.push(n[2] = i);
+                    var o = b.p + b.u(r),
+                        a = new Error;
+                    b.l(o, (t => {
+                        if (b.o(e, r) && (0 !== (n = e[r]) && (e[r] = void 0), n)) {
+                            var i = t && ("load" === t.type ? "missing" : t.type),
+                                o = t && t.target && t.target.src;
+                            a.message = "Loading chunk " + r + " failed.\n(" + i + ": " + o + ")", a.name = "ChunkLoadError", a.type = i, a.request = o, n[1](a)
+                        }
+                    }), "chunk-" + r, r)
+                }
         };
         var r = (r, t) => {
                 var n, i, [o, a, l] = t,
-                    f = 0;
+                    u = 0;
                 if (o.some((r => 0 !== e[r]))) {
-                    for (n in a) m.o(a, n) && (m.m[n] = a[n]);
-                    l && l(m)
+                    for (n in a) b.o(a, n) && (b.m[n] = a[n]);
+                    l && l(b)
                 }
-                for (r && r(t); f < o.length; f++) i = o[f], m.o(e, i) && e[i] && e[i][0](), e[i] = 0
+                for (r && r(t); u < o.length; u++) i = o[u], b.o(e, i) && e[i] && e[i][0](), e[i] = 0
             },
             t = self.webpackChunkipyfilite = self.webpackChunkipyfilite || [];
         t.forEach(r.bind(null, 0)), t.push = r.bind(null, t.push.bind(t))
-    })(), m.nc = void 0;
-    var y = m(229);
+    })(), b.nc = void 0;
+    var y = b(229);
     (_JUPYTERLAB = void 0 === _JUPYTERLAB ? {} : _JUPYTERLAB).ipyfilite = y
 })();
```

### Comparing `ipyfilite-0.1.7/ipyfilite/labextension/static/third-party-licenses.json` & `ipyfilite-0.1.8/ipyfilite/labextension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/ipyfilite/nbextension/index.js.map` & `ipyfilite-0.1.8/ipyfilite/nbextension/index.js.map`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9111474111474112%*

 * *Differences: {"'mappings'": "'iEAEAA,EADkC,EAAQ,IAChCC,EAA4B,IAE9BC,KAAK,CAACC,EAAOC,GAAI,iFAAkF,KAE3GD,EAAOH,QAAUA,C,uBCEjBG,EAAOH,QAAU,SAAUK,GACzB,IAAIC,EAAO,GAuDX,OArDAA,EAAKC,SAAW,WACd,OAAOC,KAAKC,KAAI,SAAUC,GACxB,IAAIC,EAsDV,SAAgCD,EAAML,GACpC,IAoBiBO,EAEbC,EACAC,EAvBAH,EAAUD,EAAK,IAAM,GAErBK,EAAaL,EAAK,GAEtB,IAAKK,EACH,OAAOJ,EAGT,GAAIN,GAAgC,mBAATW,KAAqB,CAC9C,IAAIC,GAWWL,EAXeG,EAa5BF,EAASG,KAAKE,SAASC,mBAAmBC,KAAKC,UAAUT,MACzDE,EAAO,+DAA+DQ,OAAOT,GAC1E,OAAOS,OAAOR,EAAM,QAdrBS,EAAaR,EAAWS,QAAQf,KAAI,SAAUgB,GAChD,M […]*

```diff
@@ -1,10 +1,10 @@
 {
     "file": "index.js",
-    "mappings": "iEAEAA,EADkC,EAAQ,IAChCC,EAA4B,IAE9BC,KAAK,CAACC,EAAOC,GAAI,iFAAkF,KAE3GD,EAAOH,QAAUA,C,uBCEjBG,EAAOH,QAAU,SAAUK,GACzB,IAAIC,EAAO,GAuDX,OArDAA,EAAKC,SAAW,WACd,OAAOC,KAAKC,KAAI,SAAUC,GACxB,IAAIC,EAsDV,SAAgCD,EAAML,GACpC,IAoBiBO,EAEbC,EACAC,EAvBAH,EAAUD,EAAK,IAAM,GAErBK,EAAaL,EAAK,GAEtB,IAAKK,EACH,OAAOJ,EAGT,GAAIN,GAAgC,mBAATW,KAAqB,CAC9C,IAAIC,GAWWL,EAXeG,EAa5BF,EAASG,KAAKE,SAASC,mBAAmBC,KAAKC,UAAUT,MACzDE,EAAO,+DAA+DQ,OAAOT,GAC1E,OAAOS,OAAOR,EAAM,QAdrBS,EAAaR,EAAWS,QAAQf,KAAI,SAAUgB,GAChD,MAAO,iBAAiBH,OAAOP,EAAWW,YAAc,IAAIJ,OAAOG,EAAQ,MAC7E,IACA,MAAO,CAACd,GAASW,OAAOC,GAAYD,OAAO,CAACL,IAAgBU,KAAK,KACnE,CAEA,MAAO,CAAChB,GAASgB,KAAK,KACxB,CAxEoBC,CAAuBlB,EAAML,GAE3C,OAAIK,EAAK,GACA,UAAUY,OAAOZ,EAAK,GAAI,MAAMY,OAAOX,EAAS,KAGlDA,CACT,IAAGgB,KAAK,GACV,EAIArB,EAAKuB,EAAI,SAAUC,EAASC,EAAYC,GACf,iBAAZF,IAETA,EAAU,CAAC,CAAC,KAAMA,EAAS,MAG7B,IAAIG,EAAyB,CAAC,EAE9B,GAAID,EACF,IAAK,IAAIH,EAAI,EAAGA,EAAIrB,KAAK0B,OAAQL,IAAK,CAEpC,IAAIzB,EAAKI,KAAKqB,GAAG,GAEP,MAANzB,IACF6B,EAAuB7B,IAAM,EAEjC,CAGF,IAAK,IAAI+B,EAAK,EAAGA,EAAKL,EAAQI,OAAQC,IAAM,CAC1C,IAAIzB,EAAO,GAAGY,OAAOQ,EAAQK,IAEzBH,GAAUC,EAAuBvB,EAAK,MAKtCqB,IACGrB,EAAK,GAGRA,EAAK,GAAK,GAAGY,OAAOS,EAAY,SAAST,OAAOZ,EAAK,IAFrDA,EAAK,GAAKqB,GAMdzB,EAAKJ,KAAKQ,GACZ,CACF,EAEOJ,CACT,C,gBCjEA,IAAI8B,EAAM,EAAQ,KACFzB,EAAU,EAAQ,KAIC,iBAFvBA,EAAUA,EAAQ0B,WAAa1B,EAAQ2B,QAAU3B,KAG/CA,EAAU,CAAC,CAACR,EAAOC,GAAIO,EAAS,MAQjCyB,EAAIzB,EALH,CAEd4B,OAAiB,OACjBA,WAAoB,IAMpBpC,EAAOH,QAAUW,EAAQ6B,QAAU,CAAC,C,6BChBpC,IACMC,EAeFC,EAAY,WACd,IAAID,EAAO,CAAC,EACZ,OAAO,SAAkBE,GACvB,QAA4B,IAAjBF,EAAKE,GAAyB,CACvC,IAAIC,EAAcC,SAASC,cAAcH,GAEzC,GAAII,OAAOC,mBAAqBJ,aAAuBG,OAAOC,kBAC5D,IAGEJ,EAAcA,EAAYK,gBAAgBC,IAC5C,CAAE,MAAOC,GAEPP,EAAc,IAChB,CAGFH,EAAKE,GAAUC,CACjB,CAEA,OAAOH,EAAKE,EACd,CACF,CAtBgB,GAwBZS,EAAc,GAElB,SAASC,EAAqBC,GAG5B,IAFA,IAAIC,GAAU,EAEL1B,EAAI,EAAGA,EAAIuB,EAAYlB,OAAQL,IACtC,GAAIuB,EAAYvB,GAAGyB,aAAeA,EAAY,CAC5CC,EAAS1B,EACT,KACF,CAGF,OAAO0B,CACT,CAEA,SAASC,EAAalD,EAAMiC,GAI1B,IAHA,IAAIkB,EAAa,CAAC,EACdC,EAAc,GAET7B,EAAI,EAAGA,EAAIvB,EAAK4B,OAAQL,IAAK,CACpC,IAAInB,EAAOJ,EAAKuB,GACZzB,EAAKmC,EAAQoB,KAAOjD,EAAK,GAAK6B,EAAQoB,KAAOjD,EAAK,GAClDkD,EAAQH,EAAWrD,IAAO,EAC1BkD,EAAa,GAAGhC,OAAOlB,EAAI,KAAKkB,OAAOsC,GAC3CH,EAAWrD,GAAMwD,EAAQ,EACzB,IAAIC,EAAQR,EAAqBC,GAC7BQ,EAAM,CACRC,IAAKrD,EAAK,GACVsD,MAAOtD,EAAK,GACZE,UAAWF,EAAK,KAGH,IAAXmD,GACFT,EAAYS,GAAOI,aACnBb,EAAYS,GAAOK,QAAQJ,IAE3BV,EAAYlD,KAAK,CACfoD,WAAYA,EACZY,QAASC,EAASL,EAAKvB,GACvB0B,WAAY,IAIhBP,EAAYxD,KAAKoD,EACnB,CAEA,OAAOI,CACT,CAEA,SAASU,EAAmB7B,GAC1B,IAAI8B,EAAQxB,SAASyB,cAAc,SAC/BC,EAAahC,EAAQgC,YAAc,CAAC,EAExC,QAAgC,IAArBA,EAAWC,MAAuB,CAC3C,IAAIA,EAAmD,KAEnDA,IACFD,EAAWC,MAAQA,EAEvB,CAMA,GAJAC,OAAOC,KAAKH,GAAYI,SAAQ,SAAUC,GACxCP,EAAMQ,aAAaD,EAAKL,EAAWK,GACrC,IAE8B,mBAAnBrC,EAAQuC,OACjBvC,EAAQuC,OAAOT,OACV,CACL,IAAI1B,EAASD,EAAUH,EAAQuC,QAAU,QAEzC,IAAKnC,EACH,MAAM,IAAIoC,MAAM,2GAGlBpC,EAAOqC,YAAYX,EACrB,CAEA,OAAOA,CACT,CAaA,IACMY,EADFC,GACED,EAAY,GACT,SAAiBpB,EAAOsB,GAE7B,OADAF,EAAUpB,GAASsB,EACZF,EAAUG,OAAOC,SAAS1D,KAAK,KACxC,GAGF,SAAS2D,EAAoBjB,EAAOR,EAAO0B,EAAQzB,GACjD,IAAIC,EAAMwB,EAAS,GAAKzB,EAAIE,MAAQ,UAAU1C,OAAOwC,EAAIE,MAAO,MAAM1C,OAAOwC,EAAIC,IAAK,KAAOD,EAAIC,IAIjG,GAAIM,EAAMmB,WACRnB,EAAMmB,WAAWC,QAAUP,EAAYrB,EAAOE,OACzC,CACL,IAAI2B,EAAU7C,SAAS8C,eAAe5B,GAClC6B,EAAavB,EAAMuB,WAEnBA,EAAW/B,IACbQ,EAAMwB,YAAYD,EAAW/B,IAG3B+B,EAAW1D,OACbmC,EAAMyB,aAAaJ,EAASE,EAAW/B,IAEvCQ,EAAMW,YAAYU,EAEtB,CACF,CAEA,SAASK,EAAW1B,EAAO9B,EAASuB,GAClC,IAAIC,EAAMD,EAAIC,IACVC,EAAQF,EAAIE,MACZpD,EAAYkD,EAAIlD,UAepB,GAbIoD,EACFK,EAAMQ,aAAa,QAASb,GAE5BK,EAAM2B,gBAAgB,SAGpBpF,GAA6B,oBAATI,OACtB+C,GAAO,uDAAuDzC,OAAON,KAAKE,SAASC,mBAAmBC,KAAKC,UAAUT,MAAe,QAMlIyD,EAAMmB,WACRnB,EAAMmB,WAAWC,QAAU1B,MACtB,CACL,KAAOM,EAAM4B,YACX5B,EAAMwB,YAAYxB,EAAM4B,YAG1B5B,EAAMW,YAAYnC,SAAS8C,eAAe5B,GAC5C,CACF,CAEA,IAAImC,EAAY,KACZC,EAAmB,EAEvB,SAAShC,EAASL,EAAKvB,GACrB,IAAI8B,EACA+B,EACAb,EAEJ,GAAIhD,EAAQ2D,UAAW,CACrB,IAAIG,EAAaF,IACjB9B,EAAQ6B,IAAcA,EAAY9B,EAAmB7B,IACrD6D,EAASd,EAAoBgB,KAAK,KAAMjC,EAAOgC,GAAY,GAC3Dd,EAASD,EAAoBgB,KAAK,KAAMjC,EAAOgC,GAAY,EAC7D,MACEhC,EAAQD,EAAmB7B,GAC3B6D,EAASL,EAAWO,KAAK,KAAMjC,EAAO9B,GAEtCgD,EAAS,YAxFb,SAA4BlB,GAE1B,GAAyB,OAArBA,EAAMkC,WACR,OAAO,EAGTlC,EAAMkC,WAAWV,YAAYxB,EAC/B,CAkFMmC,CAAmBnC,EACrB,EAIF,OADA+B,EAAOtC,GACA,SAAqB2C,GAC1B,GAAIA,EAAQ,CACV,GAAIA,EAAO1C,MAAQD,EAAIC,KAAO0C,EAAOzC,QAAUF,EAAIE,OAASyC,EAAO7F,YAAckD,EAAIlD,UACnF,OAGFwF,EAAOtC,EAAM2C,EACf,MACElB,GAEJ,CACF,CAEApF,EAAOH,QAAU,SAAUM,EAAMiC,IAC/BA,EAAUA,GAAW,CAAC,GAGT2D,WAA0C,kBAAtB3D,EAAQ2D,YACvC3D,EAAQ2D,gBArOY,IAATzD,IAMTA,EAAO4C,QAAQtC,QAAUF,UAAYA,SAAS6D,MAAQ3D,OAAO4D,OAGxDlE,IAgOT,IAAImE,EAAkBpD,EADtBlD,EAAOA,GAAQ,GAC0BiC,GACzC,OAAO,SAAgBsE,GAGrB,GAFAA,EAAUA,GAAW,GAE2B,mBAA5CpC,OAAOqC,UAAUvG,SAASwG,KAAKF,GAAnC,CAIA,IAAK,IAAIhF,EAAI,EAAGA,EAAI+E,EAAgB1E,OAAQL,IAAK,CAC/C,IACIgC,EAAQR,EADKuD,EAAgB/E,IAEjCuB,EAAYS,GAAOI,YACrB,CAIA,IAFA,IAAI+C,EAAqBxD,EAAaqD,EAAStE,GAEtCJ,EAAK,EAAGA,EAAKyE,EAAgB1E,OAAQC,IAAM,CAClD,IAEI8E,EAAS5D,EAFKuD,EAAgBzE,IAIK,IAAnCiB,EAAY6D,GAAQhD,aACtBb,EAAY6D,GAAQ/C,UAEpBd,EAAY8D,OAAOD,EAAQ,GAE/B,CAEAL,EAAkBI,CAtBlB,CAuBF,CACF,C,6ZCjQCjE,OAAeoE,wBACdtE,SAASC,cAAc,QAASsE,aAAa,iBAC7C,yBAEF,W,6ZCZA,YACA,W,oHCEA,MAAMtG,EAAO,EAAQ,KAQR,EAAAuG,eAAiBvG,EAAKwG,QAKtB,EAAAC,YAAczG,EAAK0G,I,gIChBhC,eAOA,SAGA,OAUA,MAAaC,UAA4B,EAAAC,eACvCC,WACE,OAAO,OAAP,wBACKC,MAAMD,YAAU,CACnBE,YAAaJ,EAAoBK,WACjCC,cAAeN,EAAoBO,aACnCC,sBAAuBR,EAAoBS,qBAC3CC,WAAYV,EAAoBW,UAChCC,aAAcZ,EAAoBa,YAClCC,qBAAsBd,EAAoBe,oBAC1CC,SAAU,EAAAC,OACVC,OAAQ,GACRC,YAAa,SACbC,UAAU,EACVC,KAAM,SACNC,aAAc,GACdC,UAAU,EACVC,MAAO,GACP5E,MAAO,MAEX,EApBF,wBAsBS,EAAA6E,YAAW,+BACb,EAAAxB,eAAewB,aAAW,CAE7BD,MAAO,CAAEE,UAAeC,GAAYA,KAG/B,EAAAtB,WAAa,sBACb,EAAAE,aAAe,EAAAT,YACf,EAAAW,qBAAuB,EAAAb,eACvB,EAAAe,UAAY,qBACZ,EAAAE,YAAc,EAAAf,YACd,EAAAiB,oBAAsB,EAAAnB,eAG/B,MAAagC,UAA2B,EAAAC,cAItCC,gBAEE/I,KAAKgJ,QAAU,QACjB,CAEAC,SACE7B,MAAM6B,SAENjJ,KAAKkJ,GAAGC,UAAUC,IAAI,mBACtBpJ,KAAKkJ,GAAGC,UAAUC,IAAI,sBACtBpJ,KAAKkJ,GAAGC,UAAUC,IAAI,kBAEtBpJ,KAAKqJ,UAAYhH,SAASyB,cAAc,SACxC9D,KAAKqJ,UAAUC,KAAO,OACtBtJ,KAAKqJ,UAAUxF,MAAM0F,QAAU,OAE/BvJ,KAAKkJ,GAAGM,iBAAiB,SAAS,KAChCxJ,KAAKqJ,UAAUI,OAAO,IAGxBzJ,KAAKqJ,UAAUG,iBAAiB,SAAS,KACvCxJ,KAAKqJ,UAAUZ,MAAQ,EAAE,IAG3BzI,KAAKqJ,UAAUG,iBAAiB,UAAU,K,MACxC,MAAMtB,EAAe,EAAAA,OAEfwB,EAA8BC,MAAMC,KACpB,QADwB,EAC5C5J,KAAKqJ,UAAUK,aAAK,QAAI,IACxBzJ,KAAK4J,IACE,CACL7C,KAAM6C,EAAK7C,KACXsC,KAAMO,EAAKP,KACXQ,KAAMD,EAAKC,KACXC,cAAeF,EAAKG,aACpBC,KAAM,YAAY/B,KAAQ2B,EAAK7C,WAInCkD,EAAQC,sBAAsBC,YAAY,CACxCV,MAAO1J,KAAKqJ,UAAUK,MACtBxB,OACAmC,QAASrK,KAAKsK,MAAMC,IAAI,YACxBC,OAAQxK,KAAKsK,MAAMG,WAGrBzK,KAAKsK,MAAMI,IAAI,CACbjC,MAAOiB,IAET1J,KAAK2K,OAAO,IAGd3K,KAAK4K,SAAS5K,KAAKsK,MAAO,sBAAuBtK,KAAK6K,qBACtD7K,KAAK8K,mBACL9K,KAAK4F,QACP,CAEAA,SACE5F,KAAKkJ,GAAGb,SAAWrI,KAAKsK,MAAMC,IAAI,YAClCvK,KAAKkJ,GAAG7E,aAAa,QAASrE,KAAKsK,MAAMC,IAAI,YAE7C,MAAM9B,EAAYzI,KAAKsK,MAAMC,IAAI,SAC3BnC,EAAc,GAAGpI,KAAKsK,MAAMC,IAAI,mBAAmB9B,EAAM/G,UACzD4G,EAAOtI,KAAKsK,MAAMC,IAAI,QAE5B,GAAInC,EAAY1G,QAAU4G,EAAK5G,OAAQ,CAErC,GADA1B,KAAKkJ,GAAG6B,YAAc,GAClBzC,EAAK5G,OAAQ,CACf,MAAML,EAAIgB,SAASyB,cAAc,KACjCzC,EAAE8H,UAAUC,IAAI,MAChB/H,EAAE8H,UAAUC,IAAI,MAAQd,GACG,IAAvBF,EAAY1G,QACdL,EAAE8H,UAAUC,IAAI,UAElBpJ,KAAKkJ,GAAG1E,YAAYnD,E,CAEtBrB,KAAKkJ,GAAG1E,YAAYnC,SAAS8C,eAAeiD,G,CAM9C,OAHApI,KAAKqJ,UAAUlB,OAASnI,KAAKsK,MAAMC,IAAI,UACvCvK,KAAKqJ,UAAUb,SAAWxI,KAAKsK,MAAMC,IAAI,YAElCnD,MAAMxB,QACf,CAEAiF,sBACE7K,KAAKgL,sBACHnC,EAAmBoC,UACnB,eACAjL,KAAKkJ,GAET,CAEA4B,mBACE9K,KAAKkL,mBACHrC,EAAmBoC,UACnB,eACAjL,KAAKkJ,GAET,EAWF,IAAUgB,EAlHV,uBAyGS,EAAAe,UAAY,CACjBE,QAAS,CAAC,eACVC,QAAS,CAAC,eACVC,KAAM,CAAC,YACPC,QAAS,CAAC,eACVC,OAAQ,CAAC,eAIb,SAAUrB,GACR,MAAMsB,EAAW,IAAIC,iBAAiB,aAEtB,EAAAtB,oBAAhB,WACE,OAAOqB,CACT,CACD,CAND,CAAUtB,IAAAA,EAAO,I,uBC7KjBvK,EAAOH,QAAUkM,C,yjFCCbC,EAA2B,CAAC,EAGhC,SAASC,EAAoBC,GAE5B,IAAIC,EAAeH,EAAyBE,GAC5C,QAAqBE,IAAjBD,EACH,OAAOA,EAAatM,QAGrB,IAAIG,EAASgM,EAAyBE,GAAY,CACjDjM,GAAIiM,EAEJrM,QAAS,CAAC,GAOX,OAHAwM,EAAoBH,GAAUtF,KAAK5G,EAAOH,QAASG,EAAQA,EAAOH,QAASoM,GAGpEjM,EAAOH,OACf,C,OCtBAoM,EAAoBK,QAAKF,ECGCH,EAAoB,I",
+    "mappings": "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",
     "names": [
         "exports",
         "___CSS_LOADER_API_IMPORT___",
         "push",
         "module",
         "id",
         "useSourceMap",
@@ -171,14 +171,15 @@
         "size",
         "last_modified",
         "lastModified",
         "path",
         "Private",
         "getBroadcastChannel",
         "postMessage",
+        "kind",
         "session",
         "model",
         "get",
         "widget",
         "model_id",
         "set",
         "touch",
@@ -192,14 +193,33 @@
         "primary",
         "success",
         "info",
         "warning",
         "danger",
         "_channel",
         "BroadcastChannel",
+        "_createUserDownload",
+        "chunks",
+        "download",
+        "href",
+        "URL",
+        "createObjectURL",
+        "Blob",
+        "_downloads",
+        "Map",
+        "onmessage",
+        "event",
+        "has",
+        "console",
+        "warn",
+        "segment",
+        "chunk",
+        "Uint8Array",
+        "padStart",
+        "delete",
         "__WEBPACK_EXTERNAL_MODULE__146__",
         "__webpack_module_cache__",
         "__webpack_require__",
         "moduleId",
         "cachedModule",
         "undefined",
         "__webpack_modules__",
@@ -224,15 +244,15 @@
         "// Imports\nvar ___CSS_LOADER_API_IMPORT___ = require(\"../node_modules/css-loader/dist/runtime/api.js\");\nexports = ___CSS_LOADER_API_IMPORT___(false);\n// Module\nexports.push([module.id, \".custom-widget {\\n  background-color: lightseagreen;\\n  padding: 0px 2px;\\n}\\n\", \"\"]);\n// Exports\nmodule.exports = exports;\n",
         "\"use strict\";\n\n/*\n  MIT License http://www.opensource.org/licenses/mit-license.php\n  Author Tobias Koppers @sokra\n*/\n// css base code, injected by the css-loader\n// eslint-disable-next-line func-names\nmodule.exports = function (useSourceMap) {\n  var list = []; // return the list of modules as css string\n\n  list.toString = function toString() {\n    return this.map(function (item) {\n      var content = cssWithMappingToString(item, useSourceMap);\n\n      if (item[2]) {\n        return \"@media \".concat(item[2], \" {\").concat(content, \"}\");\n      }\n\n      return content;\n    }).join('');\n  }; // import a list of modules into the list\n  // eslint-disable-next-line func-names\n\n\n  list.i = function (modules, mediaQuery, dedupe) {\n    if (typeof modules === 'string') {\n      // eslint-disable-next-line no-param-reassign\n      modules = [[null, modules, '']];\n    }\n\n    var alreadyImportedModules = {};\n\n    if (dedupe) {\n      for (var i = 0; i < this.length; i++) {\n        // eslint-disable-next-line prefer-destructuring\n        var id = this[i][0];\n\n        if (id != null) {\n          alreadyImportedModules[id] = true;\n        }\n      }\n    }\n\n    for (var _i = 0; _i < modules.length; _i++) {\n      var item = [].concat(modules[_i]);\n\n      if (dedupe && alreadyImportedModules[item[0]]) {\n        // eslint-disable-next-line no-continue\n        continue;\n      }\n\n      if (mediaQuery) {\n        if (!item[2]) {\n          item[2] = mediaQuery;\n        } else {\n          item[2] = \"\".concat(mediaQuery, \" and \").concat(item[2]);\n        }\n      }\n\n      list.push(item);\n    }\n  };\n\n  return list;\n};\n\nfunction cssWithMappingToString(item, useSourceMap) {\n  var content = item[1] || ''; // eslint-disable-next-line prefer-destructuring\n\n  var cssMapping = item[3];\n\n  if (!cssMapping) {\n    return content;\n  }\n\n  if (useSourceMap && typeof btoa === 'function') {\n    var sourceMapping = toComment(cssMapping);\n    var sourceURLs = cssMapping.sources.map(function (source) {\n      return \"/*# sourceURL=\".concat(cssMapping.sourceRoot || '').concat(source, \" */\");\n    });\n    return [content].concat(sourceURLs).concat([sourceMapping]).join('\\n');\n  }\n\n  return [content].join('\\n');\n} // Adapted from convert-source-map (MIT)\n\n\nfunction toComment(sourceMap) {\n  // eslint-disable-next-line no-undef\n  var base64 = btoa(unescape(encodeURIComponent(JSON.stringify(sourceMap))));\n  var data = \"sourceMappingURL=data:application/json;charset=utf-8;base64,\".concat(base64);\n  return \"/*# \".concat(data, \" */\");\n}",
         "var api = require(\"!../node_modules/style-loader/dist/runtime/injectStylesIntoStyleTag.js\");\n            var content = require(\"!!../node_modules/css-loader/dist/cjs.js!./widget.css\");\n\n            content = content.__esModule ? content.default : content;\n\n            if (typeof content === 'string') {\n              content = [[module.id, content, '']];\n            }\n\nvar options = {};\n\noptions.insert = \"head\";\noptions.singleton = false;\n\nvar update = api(content, options);\n\n\n\nmodule.exports = content.locals || {};",
         "\"use strict\";\n\nvar isOldIE = function isOldIE() {\n  var memo;\n  return function memorize() {\n    if (typeof memo === 'undefined') {\n      // Test for IE <= 9 as proposed by Browserhacks\n      // @see http://browserhacks.com/#hack-e71d8692f65334173fee715c222cb805\n      // Tests for existence of standard globals is to allow style-loader\n      // to operate correctly into non-standard environments\n      // @see https://github.com/webpack-contrib/style-loader/issues/177\n      memo = Boolean(window && document && document.all && !window.atob);\n    }\n\n    return memo;\n  };\n}();\n\nvar getTarget = function getTarget() {\n  var memo = {};\n  return function memorize(target) {\n    if (typeof memo[target] === 'undefined') {\n      var styleTarget = document.querySelector(target); // Special case to return head of iframe instead of iframe itself\n\n      if (window.HTMLIFrameElement && styleTarget instanceof window.HTMLIFrameElement) {\n        try {\n          // This will throw an exception if access to iframe is blocked\n          // due to cross-origin restrictions\n          styleTarget = styleTarget.contentDocument.head;\n        } catch (e) {\n          // istanbul ignore next\n          styleTarget = null;\n        }\n      }\n\n      memo[target] = styleTarget;\n    }\n\n    return memo[target];\n  };\n}();\n\nvar stylesInDom = [];\n\nfunction getIndexByIdentifier(identifier) {\n  var result = -1;\n\n  for (var i = 0; i < stylesInDom.length; i++) {\n    if (stylesInDom[i].identifier === identifier) {\n      result = i;\n      break;\n    }\n  }\n\n  return result;\n}\n\nfunction modulesToDom(list, options) {\n  var idCountMap = {};\n  var identifiers = [];\n\n  for (var i = 0; i < list.length; i++) {\n    var item = list[i];\n    var id = options.base ? item[0] + options.base : item[0];\n    var count = idCountMap[id] || 0;\n    var identifier = \"\".concat(id, \" \").concat(count);\n    idCountMap[id] = count + 1;\n    var index = getIndexByIdentifier(identifier);\n    var obj = {\n      css: item[1],\n      media: item[2],\n      sourceMap: item[3]\n    };\n\n    if (index !== -1) {\n      stylesInDom[index].references++;\n      stylesInDom[index].updater(obj);\n    } else {\n      stylesInDom.push({\n        identifier: identifier,\n        updater: addStyle(obj, options),\n        references: 1\n      });\n    }\n\n    identifiers.push(identifier);\n  }\n\n  return identifiers;\n}\n\nfunction insertStyleElement(options) {\n  var style = document.createElement('style');\n  var attributes = options.attributes || {};\n\n  if (typeof attributes.nonce === 'undefined') {\n    var nonce = typeof __webpack_nonce__ !== 'undefined' ? __webpack_nonce__ : null;\n\n    if (nonce) {\n      attributes.nonce = nonce;\n    }\n  }\n\n  Object.keys(attributes).forEach(function (key) {\n    style.setAttribute(key, attributes[key]);\n  });\n\n  if (typeof options.insert === 'function') {\n    options.insert(style);\n  } else {\n    var target = getTarget(options.insert || 'head');\n\n    if (!target) {\n      throw new Error(\"Couldn't find a style target. This probably means that the value for the 'insert' parameter is invalid.\");\n    }\n\n    target.appendChild(style);\n  }\n\n  return style;\n}\n\nfunction removeStyleElement(style) {\n  // istanbul ignore if\n  if (style.parentNode === null) {\n    return false;\n  }\n\n  style.parentNode.removeChild(style);\n}\n/* istanbul ignore next  */\n\n\nvar replaceText = function replaceText() {\n  var textStore = [];\n  return function replace(index, replacement) {\n    textStore[index] = replacement;\n    return textStore.filter(Boolean).join('\\n');\n  };\n}();\n\nfunction applyToSingletonTag(style, index, remove, obj) {\n  var css = remove ? '' : obj.media ? \"@media \".concat(obj.media, \" {\").concat(obj.css, \"}\") : obj.css; // For old IE\n\n  /* istanbul ignore if  */\n\n  if (style.styleSheet) {\n    style.styleSheet.cssText = replaceText(index, css);\n  } else {\n    var cssNode = document.createTextNode(css);\n    var childNodes = style.childNodes;\n\n    if (childNodes[index]) {\n      style.removeChild(childNodes[index]);\n    }\n\n    if (childNodes.length) {\n      style.insertBefore(cssNode, childNodes[index]);\n    } else {\n      style.appendChild(cssNode);\n    }\n  }\n}\n\nfunction applyToTag(style, options, obj) {\n  var css = obj.css;\n  var media = obj.media;\n  var sourceMap = obj.sourceMap;\n\n  if (media) {\n    style.setAttribute('media', media);\n  } else {\n    style.removeAttribute('media');\n  }\n\n  if (sourceMap && typeof btoa !== 'undefined') {\n    css += \"\\n/*# sourceMappingURL=data:application/json;base64,\".concat(btoa(unescape(encodeURIComponent(JSON.stringify(sourceMap)))), \" */\");\n  } // For old IE\n\n  /* istanbul ignore if  */\n\n\n  if (style.styleSheet) {\n    style.styleSheet.cssText = css;\n  } else {\n    while (style.firstChild) {\n      style.removeChild(style.firstChild);\n    }\n\n    style.appendChild(document.createTextNode(css));\n  }\n}\n\nvar singleton = null;\nvar singletonCounter = 0;\n\nfunction addStyle(obj, options) {\n  var style;\n  var update;\n  var remove;\n\n  if (options.singleton) {\n    var styleIndex = singletonCounter++;\n    style = singleton || (singleton = insertStyleElement(options));\n    update = applyToSingletonTag.bind(null, style, styleIndex, false);\n    remove = applyToSingletonTag.bind(null, style, styleIndex, true);\n  } else {\n    style = insertStyleElement(options);\n    update = applyToTag.bind(null, style, options);\n\n    remove = function remove() {\n      removeStyleElement(style);\n    };\n  }\n\n  update(obj);\n  return function updateStyle(newObj) {\n    if (newObj) {\n      if (newObj.css === obj.css && newObj.media === obj.media && newObj.sourceMap === obj.sourceMap) {\n        return;\n      }\n\n      update(obj = newObj);\n    } else {\n      remove();\n    }\n  };\n}\n\nmodule.exports = function (list, options) {\n  options = options || {}; // Force single-tag solution on IE6-9, which has a hard limit on the # of <style>\n  // tags it will allow on a page\n\n  if (!options.singleton && typeof options.singleton !== 'boolean') {\n    options.singleton = isOldIE();\n  }\n\n  list = list || [];\n  var lastIdentifiers = modulesToDom(list, options);\n  return function update(newList) {\n    newList = newList || [];\n\n    if (Object.prototype.toString.call(newList) !== '[object Array]') {\n      return;\n    }\n\n    for (var i = 0; i < lastIdentifiers.length; i++) {\n      var identifier = lastIdentifiers[i];\n      var index = getIndexByIdentifier(identifier);\n      stylesInDom[index].references--;\n    }\n\n    var newLastIdentifiers = modulesToDom(newList, options);\n\n    for (var _i = 0; _i < lastIdentifiers.length; _i++) {\n      var _identifier = lastIdentifiers[_i];\n\n      var _index = getIndexByIdentifier(_identifier);\n\n      if (stylesInDom[_index].references === 0) {\n        stylesInDom[_index].updater();\n\n        stylesInDom.splice(_index, 1);\n      }\n    }\n\n    lastIdentifiers = newLastIdentifiers;\n  };\n};",
         "// Copyright (c) Jupyter Development Team.\n// Distributed under the terms of the Modified BSD License.\n\n// Entry point for the notebook bundle containing custom model definitions.\n//\n// Setup notebook base URL\n//\n// Some static assets may be required by the custom widget javascript. The base\n// url for the notebook is not known at build time and is therefore computed\n// dynamically.\n// eslint-disable-next-line @typescript-eslint/no-non-null-assertion\n(window as any).__webpack_public_path__ =\n  document.querySelector('body')!.getAttribute('data-base-url') +\n  'nbextensions/ipyfilite';\n\nexport * from './index';\n",
         "// Copyright (c) Juniper Tyree\n// Distributed under the terms of the Modified BSD License.\n\nexport * from './version';\nexport * from './widget';\n",
         "// Copyright (c) Juniper Tyree\n// Distributed under the terms of the Modified BSD License.\n\n// eslint-disable-next-line @typescript-eslint/ban-ts-comment\n// @ts-ignore\n// eslint-disable-next-line @typescript-eslint/no-var-requires\nconst data = require('../package.json');\n\n/**\n * The _model_module_version/_view_module_version this package implements.\n *\n * The html widget manager assumes that this is the same as the npm package\n * version number.\n */\nexport const MODULE_VERSION = data.version;\n\n/*\n * The current package name.\n */\nexport const MODULE_NAME = data.name;\n",
-        "// Copyright (c) Juniper Tyree\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n  uuid as uuidv4,\n} from '@jupyter-widgets/base';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\n\n// Import the CSS\nimport '../css/widget.css';\n\ninterface IFileUploaded {\n  name: string;\n  size: number;\n  type: string;\n  last_modified: number;\n  path: string;\n}\n\nexport class FileUploadLiteModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: FileUploadLiteModel.model_name,\n      _model_module: FileUploadLiteModel.model_module,\n      _model_module_version: FileUploadLiteModel.model_module_version,\n      _view_name: FileUploadLiteModel.view_name,\n      _view_module: FileUploadLiteModel.view_module,\n      _view_module_version: FileUploadLiteModel.view_module_version,\n      _session: uuidv4(),\n      accept: '',\n      description: 'Upload',\n      disabled: false,\n      icon: 'upload',\n      button_style: '',\n      multiple: false,\n      value: [], // has type Array<IFileUploaded>\n      style: null,\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // use a dummy serializer for value to circumvent the default serializer.\n    value: { serialize: <T>(x: T): T => x },\n  };\n\n  static model_name = 'FileUploadLiteModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'FileUploadLiteView';\n  static view_module = MODULE_NAME;\n  static view_module_version = MODULE_VERSION;\n}\n\nexport class FileUploadLiteView extends DOMWidgetView {\n  el: HTMLButtonElement;\n  fileInput: HTMLInputElement;\n\n  preinitialize() {\n    // Must set this before the initialize method creates the element\n    this.tagName = 'button';\n  }\n\n  render(): void {\n    super.render();\n\n    this.el.classList.add('jupyter-widgets');\n    this.el.classList.add('widget-upload-lite');\n    this.el.classList.add('jupyter-button');\n\n    this.fileInput = document.createElement('input');\n    this.fileInput.type = 'file';\n    this.fileInput.style.display = 'none';\n\n    this.el.addEventListener('click', () => {\n      this.fileInput.click();\n    });\n\n    this.fileInput.addEventListener('click', () => {\n      this.fileInput.value = '';\n    });\n\n    this.fileInput.addEventListener('change', () => {\n      const uuid: string = uuidv4();\n\n      const files: Array<IFileUploaded> = Array.from(\n        this.fileInput.files ?? []\n      ).map((file: File) => {\n        return {\n          name: file.name,\n          type: file.type,\n          size: file.size,\n          last_modified: file.lastModified,\n          path: `/uploads/${uuid}/${file.name}`,\n        };\n      });\n\n      Private.getBroadcastChannel().postMessage({\n        files: this.fileInput.files,\n        uuid,\n        session: this.model.get('_session'),\n        widget: this.model.model_id,\n      });\n\n      this.model.set({\n        value: files,\n      });\n      this.touch();\n    });\n\n    this.listenTo(this.model, 'change:button_style', this.update_button_style);\n    this.set_button_style();\n    this.update(); // Set defaults.\n  }\n\n  update(): void {\n    this.el.disabled = this.model.get('disabled');\n    this.el.setAttribute('title', this.model.get('tooltip'));\n\n    const value: [] = this.model.get('value');\n    const description = `${this.model.get('description')} (${value.length})`;\n    const icon = this.model.get('icon');\n\n    if (description.length || icon.length) {\n      this.el.textContent = '';\n      if (icon.length) {\n        const i = document.createElement('i');\n        i.classList.add('fa');\n        i.classList.add('fa-' + icon);\n        if (description.length === 0) {\n          i.classList.add('center');\n        }\n        this.el.appendChild(i);\n      }\n      this.el.appendChild(document.createTextNode(description));\n    }\n\n    this.fileInput.accept = this.model.get('accept');\n    this.fileInput.multiple = this.model.get('multiple');\n\n    return super.update();\n  }\n\n  update_button_style(): void {\n    this.update_mapped_classes(\n      FileUploadLiteView.class_map,\n      'button_style',\n      this.el\n    );\n  }\n\n  set_button_style(): void {\n    this.set_mapped_classes(\n      FileUploadLiteView.class_map,\n      'button_style',\n      this.el\n    );\n  }\n\n  static class_map = {\n    primary: ['mod-primary'],\n    success: ['mod-success'],\n    info: ['mod-info'],\n    warning: ['mod-warning'],\n    danger: ['mod-danger'],\n  };\n}\n\nnamespace Private {\n  const _channel = new BroadcastChannel('ipyfilite');\n\n  export function getBroadcastChannel(): BroadcastChannel {\n    return _channel;\n  }\n}\n",
+        "// Copyright (c) Juniper Tyree\n// Distributed under the terms of the Modified BSD License.\n\nimport {\n  DOMWidgetModel,\n  DOMWidgetView,\n  ISerializers,\n  uuid as uuidv4,\n} from '@jupyter-widgets/base';\n\nimport { MODULE_NAME, MODULE_VERSION } from './version';\n\n// Import the CSS\nimport '../css/widget.css';\n\ninterface IFileUploaded {\n  name: string;\n  size: number;\n  type: string;\n  last_modified: number;\n  path: string;\n}\n\nexport class FileUploadLiteModel extends DOMWidgetModel {\n  defaults() {\n    return {\n      ...super.defaults(),\n      _model_name: FileUploadLiteModel.model_name,\n      _model_module: FileUploadLiteModel.model_module,\n      _model_module_version: FileUploadLiteModel.model_module_version,\n      _view_name: FileUploadLiteModel.view_name,\n      _view_module: FileUploadLiteModel.view_module,\n      _view_module_version: FileUploadLiteModel.view_module_version,\n      _session: uuidv4(),\n      accept: '',\n      description: 'Upload',\n      disabled: false,\n      icon: 'upload',\n      button_style: '',\n      multiple: false,\n      value: [], // has type Array<IFileUploaded>\n      style: null,\n    };\n  }\n\n  static serializers: ISerializers = {\n    ...DOMWidgetModel.serializers,\n    // use a dummy serializer for value to circumvent the default serializer.\n    value: { serialize: <T>(x: T): T => x },\n  };\n\n  static model_name = 'FileUploadLiteModel';\n  static model_module = MODULE_NAME;\n  static model_module_version = MODULE_VERSION;\n  static view_name = 'FileUploadLiteView';\n  static view_module = MODULE_NAME;\n  static view_module_version = MODULE_VERSION;\n}\n\nexport class FileUploadLiteView extends DOMWidgetView {\n  el: HTMLButtonElement;\n  fileInput: HTMLInputElement;\n\n  preinitialize() {\n    // Must set this before the initialize method creates the element\n    this.tagName = 'button';\n  }\n\n  render(): void {\n    super.render();\n\n    this.el.classList.add('jupyter-widgets');\n    this.el.classList.add('widget-upload-lite');\n    this.el.classList.add('jupyter-button');\n\n    this.fileInput = document.createElement('input');\n    this.fileInput.type = 'file';\n    this.fileInput.style.display = 'none';\n\n    this.el.addEventListener('click', () => {\n      this.fileInput.click();\n    });\n\n    this.fileInput.addEventListener('click', () => {\n      this.fileInput.value = '';\n    });\n\n    this.fileInput.addEventListener('change', () => {\n      const uuid: string = uuidv4();\n\n      const files: Array<IFileUploaded> = Array.from(\n        this.fileInput.files ?? []\n      ).map((file: File) => {\n        return {\n          name: file.name,\n          type: file.type,\n          size: file.size,\n          last_modified: file.lastModified,\n          path: `/uploads/${uuid}/${file.name}`,\n        };\n      });\n\n      Private.getBroadcastChannel().postMessage({\n        kind: 'upload',\n        files: this.fileInput.files,\n        uuid,\n        session: this.model.get('_session'),\n        widget: this.model.model_id,\n      });\n\n      this.model.set({\n        value: files,\n      });\n      this.touch();\n    });\n\n    this.listenTo(this.model, 'change:button_style', this.update_button_style);\n    this.set_button_style();\n    this.update(); // Set defaults.\n  }\n\n  update(): void {\n    this.el.disabled = this.model.get('disabled');\n    this.el.setAttribute('title', this.model.get('tooltip'));\n\n    const value: [] = this.model.get('value');\n    const description = `${this.model.get('description')} (${value.length})`;\n    const icon = this.model.get('icon');\n\n    if (description.length || icon.length) {\n      this.el.textContent = '';\n      if (icon.length) {\n        const i = document.createElement('i');\n        i.classList.add('fa');\n        i.classList.add('fa-' + icon);\n        if (description.length === 0) {\n          i.classList.add('center');\n        }\n        this.el.appendChild(i);\n      }\n      this.el.appendChild(document.createTextNode(description));\n    }\n\n    this.fileInput.accept = this.model.get('accept');\n    this.fileInput.multiple = this.model.get('multiple');\n\n    return super.update();\n  }\n\n  update_button_style(): void {\n    this.update_mapped_classes(\n      FileUploadLiteView.class_map,\n      'button_style',\n      this.el\n    );\n  }\n\n  set_button_style(): void {\n    this.set_mapped_classes(\n      FileUploadLiteView.class_map,\n      'button_style',\n      this.el\n    );\n  }\n\n  static class_map = {\n    primary: ['mod-primary'],\n    success: ['mod-success'],\n    info: ['mod-info'],\n    warning: ['mod-warning'],\n    danger: ['mod-danger'],\n  };\n}\n\nnamespace Private {\n  const _channel = new BroadcastChannel('ipyfilite');\n\n  export function getBroadcastChannel(): BroadcastChannel {\n    return _channel;\n  }\n\n  /* eslint-disable no-inner-declarations */\n  function _createUserDownload(name: string, chunks: [Uint8Array]) {\n    const download = document.createElement('a');\n    download.href = URL.createObjectURL(new Blob(chunks));\n    download.download = name;\n    download.click();\n  }\n\n  const _downloads = new Map();\n\n  _channel.onmessage = function (event) {\n    if (!event.data || !event.data.kind) {\n      return;\n    }\n\n    if (event.data.kind === 'download-open') {\n      if (_downloads.has(event.data.uuid)) {\n        console.warn(`Download stream for '${event.data.uuid}' already open.`);\n        return;\n      }\n\n      _downloads.set(event.data.uuid, {\n        name: event.data.name,\n        chunks: [],\n        size: 0,\n        segment: 0,\n      });\n    } else if (event.data.kind === 'download-chunk') {\n      if (!_downloads.has(event.data.uuid)) {\n        console.warn(\n          `No download stream for '${event.data.uuid}' is open to write to.`\n        );\n        return;\n      }\n\n      const download = _downloads.get(event.data.uuid);\n      const chunk = new Uint8Array(event.data.chunk);\n\n      download.chunks.push(chunk);\n      download.size += chunk.length;\n\n      if (download.size >= 1024 * 1024 * 256) {\n        download.segment += 1;\n        _createUserDownload(\n          `${download.name}.${download.segment.toString().padStart(3, '0')}`,\n          download.chunks\n        );\n        download.chunks = [];\n        download.size = 0;\n      }\n    } else if (event.data.kind === 'download-close') {\n      if (!_downloads.has(event.data.uuid)) {\n        console.warn(\n          `No download stream for '${event.data.uuid}' is open to close.`\n        );\n        return;\n      }\n\n      const download = _downloads.get(event.data.uuid);\n      _downloads.delete(event.data.uuid);\n\n      if (download.segment > 0 && download.chunks.length === 0) {\n        return; // segemented download with no more data\n      }\n\n      if (download.segment > 0) {\n        download.segment += 1;\n        _createUserDownload(\n          `${download.name}.${download.segment.toString().padStart(3, '0')}`,\n          download.chunks\n        );\n      } else {\n        _createUserDownload(download.name, download.chunks);\n      }\n    }\n  };\n}\n",
         "module.exports = __WEBPACK_EXTERNAL_MODULE__146__;",
         "// The module cache\nvar __webpack_module_cache__ = {};\n\n// The require function\nfunction __webpack_require__(moduleId) {\n\t// Check if module is in cache\n\tvar cachedModule = __webpack_module_cache__[moduleId];\n\tif (cachedModule !== undefined) {\n\t\treturn cachedModule.exports;\n\t}\n\t// Create a new module (and put it into the cache)\n\tvar module = __webpack_module_cache__[moduleId] = {\n\t\tid: moduleId,\n\t\t// no module.loaded needed\n\t\texports: {}\n\t};\n\n\t// Execute the module function\n\t__webpack_modules__[moduleId].call(module.exports, module, module.exports, __webpack_require__);\n\n\t// Return the exports of the module\n\treturn module.exports;\n}\n\n",
         "__webpack_require__.nc = undefined;",
         "// startup\n// Load entry module and return exports\n// This entry module is referenced by other modules so it can't be inlined\nvar __webpack_exports__ = __webpack_require__(112);\n"
     ],
     "version": 3
 }
```

### Comparing `ipyfilite-0.1.7/ipyfilite/tests/conftest.py` & `ipyfilite-0.1.8/ipyfilite/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/src/extension.ts` & `ipyfilite-0.1.8/src/extension.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/src/plugin.ts` & `ipyfilite-0.1.8/src/plugin.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/src/version.ts` & `ipyfilite-0.1.8/src/version.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/src/__tests__/index.spec.ts` & `ipyfilite-0.1.8/src/__tests__/index.spec.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/src/__tests__/utils.ts` & `ipyfilite-0.1.8/src/__tests__/utils.ts`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/.gitignore` & `ipyfilite-0.1.8/.gitignore`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/LICENSE.txt` & `ipyfilite-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/README.md` & `ipyfilite-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `ipyfilite-0.1.7/pyproject.toml` & `ipyfilite-0.1.8/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
 ]
 dependencies = [
     "ipywidgets>=7.0.0",
 ]
-version = "0.1.7"
+version = "0.1.8"
 
 [project.optional-dependencies]
 docs = [
     "jupyter_sphinx",
     "nbsphinx",
     "nbsphinx-link",
     "pypandoc",
@@ -101,15 +101,15 @@
 ]
 file = [
     { src = "pyproject.toml", version_template = "version = \"{major}.{minor}.{patch}{channel}{release}\"" },
     { src = "ipyfilite/_version.py" },
 ]
 
 [tool.tbump.version]
-current = "0.1.7"
+current = "0.1.8"
 regex = "(?P<major>\\d+)\\.(?P<minor>\\d+)\\.(?P<patch>\\d+)((?P<channel>a|b|rc|.dev)(?P<release>\\d+))?"
 
 [tool.tbump.git]
 message_template = "Bump to {new_version}"
 tag_template = "v{new_version}"
 
 [tool.black]
```

### Comparing `ipyfilite-0.1.7/PKG-INFO` & `ipyfilite-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipyfilite
-Version: 0.1.7
+Version: 0.1.8
 Summary: File upload widget specifically for Pyodide kernels running in JupyterLite. Uploaded files are not loaded into memory but mounted as read-only files in a new WORKERFS.
 Project-URL: Homepage, https://github.com/juntyr/ipyfilite
 Author-email: Juniper Tyree <juniper.tyree@helsinki.fi>
 License: Copyright (c) 2023 Juniper Tyree
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without
```

