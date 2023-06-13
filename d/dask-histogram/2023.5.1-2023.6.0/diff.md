# Comparing `tmp/dask_histogram-2023.5.1.tar.gz` & `tmp/dask_histogram-2023.6.0.tar.gz`

## Comparing `dask_histogram-2023.5.1.tar` & `dask_histogram-2023.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/src/dask_histogram/__init__.py
--rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/src/dask_histogram/bins.py
--rw-r--r--   0        0        0    29302 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/src/dask_histogram/boost.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/src/dask_histogram/config.py
--rw-r--r--   0        0        0    39941 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/src/dask_histogram/core.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/src/dask_histogram/histogram.yaml
--rw-r--r--   0        0        0      515 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/src/dask_histogram/layers.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/src/dask_histogram/py.typed
--rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/src/dask_histogram/routines.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/src/dask_histogram/sizeof.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/src/dask_histogram/typing.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/src/dask_histogram/version.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/.gitignore
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/LICENSE
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/README.md
--rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/pyproject.toml
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 dask_histogram-2023.5.1/PKG-INFO
+-rw-r--r--   0        0        0      777 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/src/dask_histogram/__init__.py
+-rw-r--r--   0        0        0     6417 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/src/dask_histogram/bins.py
+-rw-r--r--   0        0        0    29302 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/src/dask_histogram/boost.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/src/dask_histogram/config.py
+-rw-r--r--   0        0        0    37967 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/src/dask_histogram/core.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/src/dask_histogram/histogram.yaml
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/src/dask_histogram/layers.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/src/dask_histogram/py.typed
+-rw-r--r--   0        0        0    16836 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/src/dask_histogram/routines.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/src/dask_histogram/sizeof.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/src/dask_histogram/typing.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/src/dask_histogram/version.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/.gitignore
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/LICENSE
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/README.md
+-rw-r--r--   0        0        0     2567 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 dask_histogram-2023.6.0/PKG-INFO
```

### Comparing `dask_histogram-2023.5.1/src/dask_histogram/__init__.py` & `dask_histogram-2023.6.0/src/dask_histogram/__init__.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.5.1/src/dask_histogram/bins.py` & `dask_histogram-2023.6.0/src/dask_histogram/bins.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.5.1/src/dask_histogram/boost.py` & `dask_histogram-2023.6.0/src/dask_histogram/boost.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.5.1/src/dask_histogram/core.py` & `dask_histogram-2023.6.0/src/dask_histogram/core.py`

 * *Files 6% similar despite different names*

```diff
@@ -257,36 +257,29 @@
     weights: Any | None,
     sample: Any | None,
     *,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     import awkward as ak
 
-    thedata = data
-    theweights = weights
-    thesample = sample
-    if isinstance(thedata, ak.Array) and ak.backend(thedata) == "typetracer":
-        thedata.layout._touch_data(recursive=True)
-        thedata = ak.Array(
-            data.layout.form.length_zero_array(highlevel=False), behavior=data.behavior
-        )
-
-    if isinstance(theweights, ak.Array) and ak.backend(theweights) == "typetracer":
-        theweights.layout._touch_data(recursive=True)
-        theweights = ak.Array(
-            weights.layout.form.length_zero_array(highlevel=False),
-            behavior=weights.behavior,
-        )
-
-    if isinstance(thesample, ak.Array) and ak.backend(thesample) == "typetracer":
-        thesample.layout._touch_data(recursive=True)
-        thesample = ak.Array(
-            sample.layout.form.length_zero_array(highlevel=False),
-            behavior=sample.behavior,
-        )
+    thedata = (
+        ak.typetracer.length_zero_if_typetracer(data)
+        if isinstance(data, ak.Array)
+        else data
+    )
+    theweights = (
+        ak.typetracer.length_zero_if_typetracer(weights)
+        if isinstance(weights, ak.Array)
+        else weights
+    )
+    thesample = (
+        ak.typetracer.length_zero_if_typetracer(sample)
+        if isinstance(sample, ak.Array)
+        else sample
+    )
 
     thehist = (
         clone(histref)
         if not isinstance(histref, tuple)
         else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
     )
     return thehist.fill(thedata, weight=theweights, sample=thesample)
@@ -294,22 +287,20 @@
 
 def _blocked_dak_ma(
     *data: Any,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     import awkward as ak
 
-    thedata = list(data)
-    for idata, adatum in enumerate(thedata):
-        if isinstance(adatum, ak.Array) and ak.backend(adatum) == "typetracer":
-            adatum.layout._touch_data(recursive=True)
-            thedata[idata] = ak.Array(
-                adatum.layout.form.length_zero_array(highlevel=False),
-                behavior=adatum.behavior,
-            )
+    thedata = [
+        ak.typetracer.length_zero_if_typetracer(datum)
+        if isinstance(datum, ak.Array)
+        else datum
+        for datum in data
+    ]
 
     thehist = (
         clone(histref)
         if not isinstance(histref, tuple)
         else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
     )
     return thehist.fill(*tuple(thedata))
@@ -317,30 +308,25 @@
 
 def _blocked_dak_ma_w(
     *data: Any,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     import awkward as ak
 
-    thedata = list(data[:-1])
-    theweights = data[-1]
-    for idata, adatum in enumerate(thedata):
-        if isinstance(adatum, ak.Array) and ak.backend(adatum) == "typetracer":
-            adatum.layout._touch_data(recursive=True)
-            thedata[idata] = ak.Array(
-                adatum.layout.form.length_zero_array(highlevel=False),
-                behavior=adatum.behavior,
-            )
-
-    if isinstance(theweights, ak.Array) and ak.backend(theweights) == "typetracer":
-        theweights.layout._touch_data(recursive=True)
-        theweights = ak.Array(
-            data[-1].layout.form.length_zero_array(highlevel=False),
-            behavior=data[-1].behavior,
-        )
+    thedata = [
+        ak.typetracer.length_zero_if_typetracer(datum)
+        if isinstance(datum, ak.Array)
+        else datum
+        for datum in data[:-1]
+    ]
+    theweights = (
+        ak.typetracer.length_zero_if_typetracer(data[-1])
+        if isinstance(data[-1], ak.Array)
+        else data[-1]
+    )
 
     thehist = (
         clone(histref)
         if not isinstance(histref, tuple)
         else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
     )
     return thehist.fill(*tuple(thedata), weight=theweights)
@@ -348,30 +334,25 @@
 
 def _blocked_dak_ma_s(
     *data: Any,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     import awkward as ak
 
-    thedata = list(data[:-1])
-    thesample = data[-1]
-    for idata, adatum in enumerate(thedata):
-        if isinstance(adatum, ak.Array) and ak.backend(adatum) == "typetracer":
-            adatum.layout._touch_data(recursive=True)
-            thedata[idata] = ak.Array(
-                adatum.layout.form.length_zero_array(highlevel=False),
-                behavior=adatum.behavior,
-            )
-
-    if isinstance(thesample, ak.Array) and ak.backend(thesample) == "typetracer":
-        thesample.layout._touch_data(recursive=True)
-        thesample = ak.Array(
-            data[-1].layout.form.length_zero_array(highlevel=False),
-            behavior=data[-1].behavior,
-        )
+    thedata = [
+        ak.typetracer.length_zero_if_typetracer(datum)
+        if isinstance(datum, ak.Array)
+        else datum
+        for datum in data[:-1]
+    ]
+    thesample = (
+        ak.typetracer.length_zero_if_typetracer(data[-1])
+        if isinstance(data[-1], ak.Array)
+        else data[-1]
+    )
 
     thehist = (
         clone(histref)
         if not isinstance(histref, tuple)
         else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
     )
     return thehist.fill(*tuple(thedata), sample=thesample)
@@ -379,38 +360,30 @@
 
 def _blocked_dak_ma_w_s(
     *data: Any,
     histref: bh.Histogram | None = None,
 ) -> bh.Histogram:
     import awkward as ak
 
-    thedata = list(data[:-2])
-    theweights = data[-2]
-    thesample = data[-1]
-    for idata, adatum in enumerate(thedata):
-        if isinstance(adatum, ak.Array) and ak.backend(adatum) == "typetracer":
-            adatum.layout._touch_data(recursive=True)
-            thedata[idata] = ak.Array(
-                adatum.layout.form.length_zero_array(highlevel=False),
-                behavior=adatum.behavior,
-            )
-
-    if isinstance(theweights, ak.Array) and ak.backend(theweights) == "typetracer":
-        theweights.layout._touch_data(recursive=True)
-        theweights = ak.Array(
-            data[-2].layout.form.length_zero_array(highlevel=False),
-            behavior=data[-2].behavior,
-        )
-
-    if isinstance(thesample, ak.Array) and ak.backend(thesample) == "typetracer":
-        thesample.layout._touch_data(recursive=True)
-        thesample = ak.Array(
-            data[-1].layout.form.length_zero_array(highlevel=False),
-            behavior=data[-1].behavior,
-        )
+    thedata = [
+        ak.typetracer.length_zero_if_typetracer(datum)
+        if isinstance(datum, ak.Array)
+        else datum
+        for datum in data[:-2]
+    ]
+    theweights = (
+        ak.typetracer.length_zero_if_typetracer(data[-2])
+        if isinstance(data[-2], ak.Array)
+        else data[-2]
+    )
+    thesample = (
+        ak.typetracer.length_zero_if_typetracer(data[-1])
+        if isinstance(data[-1], ak.Array)
+        else data[-1]
+    )
 
     thehist = (
         clone(histref)
         if not isinstance(histref, tuple)
         else bh.Histogram(*histref[0], storage=histref[1], metadata=histref[2])
     )
     return thehist.fill(*tuple(thedata), weight=theweights, sample=thesample)
```

### Comparing `dask_histogram-2023.5.1/src/dask_histogram/layers.py` & `dask_histogram-2023.6.0/src/dask_histogram/layers.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 from dask.layers import DataFrameTreeReduction
 
 
 class MockableDataFrameTreeReduction(DataFrameTreeReduction):
     def mock(self):
-        return MockableDataFrameTreeReduction(
-            name=self.name,
-            name_input=self.name_input,
-            npartitions_input=1,
-            concat_func=self.concat_func,
-            tree_node_func=self.tree_node_func,
-            finalize_func=self.finalize_func,
-            split_every=self.split_every,
-            tree_node_name=self.tree_node_name,
+        return (
+            MockableDataFrameTreeReduction(
+                name=self.name,
+                name_input=self.name_input,
+                npartitions_input=1,
+                concat_func=self.concat_func,
+                tree_node_func=self.tree_node_func,
+                finalize_func=self.finalize_func,
+                split_every=self.split_every,
+                tree_node_name=self.tree_node_name,
+            ),
+            None,
         )
```

### Comparing `dask_histogram-2023.5.1/src/dask_histogram/routines.py` & `dask_histogram-2023.6.0/src/dask_histogram/routines.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.5.1/src/dask_histogram/sizeof.py` & `dask_histogram-2023.6.0/src/dask_histogram/sizeof.py`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.5.1/.gitignore` & `dask_histogram-2023.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.5.1/LICENSE` & `dask_histogram-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.5.1/README.md` & `dask_histogram-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `dask_histogram-2023.5.1/pyproject.toml` & `dask_histogram-2023.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -31,28 +31,28 @@
 ]
 dynamic = ["version"]
 
 [project.optional-dependencies]
 complete = [
     "dask-sphinx-theme >=3.0.2",
     "dask[array,dataframe]",
-    "dask_awkward >=2023.5.1",
+    "dask_awkward >=2023.6.1",
     "hist",
     "pytest",
     "sphinx >=4.0.0",
 ]
 docs = [
     "dask-sphinx-theme >=3.0.2",
     "dask[array,dataframe]",
-    "dask_awkward >=2023.5.1",
+    "dask_awkward >=2023.6.1",
     "sphinx >=4.0.0",
 ]
 test = [
     "dask[array,dataframe]",
-    "dask_awkward >=2023.5.1",
+    "dask_awkward >=2023.6.1",
     "hist",
     "pytest",
 ]
 
 [project.urls]
 Homepage = "https://github.com/dask-contrib/dask-histogram"
 Documentation = "https://dask-histogram.readthedocs.io/"
```

### Comparing `dask_histogram-2023.5.1/PKG-INFO` & `dask_histogram-2023.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-histogram
-Version: 2023.5.1
+Version: 2023.6.0
 Summary: Histogramming with Dask.
 Project-URL: Homepage, https://github.com/dask-contrib/dask-histogram
 Project-URL: Documentation, https://dask-histogram.readthedocs.io/
 Project-URL: Bug Tracker, https://github.com/dask-contrib/dask-histogram/issues
 Author-email: Doug Davis <ddavis@ddavis.io>
 License: BSD-3-Clause
 License-File: LICENSE
@@ -20,27 +20,27 @@
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Scientific/Engineering :: Physics
 Requires-Python: >=3.8
 Requires-Dist: boost-histogram>=1.3.2
 Requires-Dist: dask>=2021.03.0
 Provides-Extra: complete
-Requires-Dist: dask-awkward>=2023.5.1; extra == 'complete'
+Requires-Dist: dask-awkward>=2023.6.1; extra == 'complete'
 Requires-Dist: dask-sphinx-theme>=3.0.2; extra == 'complete'
 Requires-Dist: dask[array,dataframe]; extra == 'complete'
 Requires-Dist: hist; extra == 'complete'
 Requires-Dist: pytest; extra == 'complete'
 Requires-Dist: sphinx>=4.0.0; extra == 'complete'
 Provides-Extra: docs
-Requires-Dist: dask-awkward>=2023.5.1; extra == 'docs'
+Requires-Dist: dask-awkward>=2023.6.1; extra == 'docs'
 Requires-Dist: dask-sphinx-theme>=3.0.2; extra == 'docs'
 Requires-Dist: dask[array,dataframe]; extra == 'docs'
 Requires-Dist: sphinx>=4.0.0; extra == 'docs'
 Provides-Extra: test
-Requires-Dist: dask-awkward>=2023.5.1; extra == 'test'
+Requires-Dist: dask-awkward>=2023.6.1; extra == 'test'
 Requires-Dist: dask[array,dataframe]; extra == 'test'
 Requires-Dist: hist; extra == 'test'
 Requires-Dist: pytest; extra == 'test'
 Description-Content-Type: text/markdown
 
 # dask-histogram
```

