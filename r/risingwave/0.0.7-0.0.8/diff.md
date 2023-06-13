# Comparing `tmp/risingwave-0.0.7.tar.gz` & `tmp/risingwave-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "risingwave-0.0.7.tar", last modified: Wed May 17 02:34:30 2023, max compression
+gzip compressed data, was "risingwave-0.0.8.tar", last modified: Tue Jun 13 10:36:45 2023, max compression
```

## Comparing `risingwave-0.0.7.tar` & `risingwave-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-05-17 02:34:30.191217 risingwave-0.0.7/
--rw-r--r--   0 wangrunji   (501) staff       (20)     2215 2023-05-17 02:34:30.191094 risingwave-0.0.7/PKG-INFO
--rw-r--r--   0 wangrunji   (501) staff       (20)     1859 2023-03-27 03:26:39.000000 risingwave-0.0.7/README.md
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-05-17 02:34:30.190368 risingwave-0.0.7/risingwave/
--rw-r--r--   0 wangrunji   (501) staff       (20)        0 2023-03-17 09:49:44.000000 risingwave-0.0.7/risingwave/__init__.py
--rw-r--r--   0 wangrunji   (501) staff       (20)     3120 2023-05-17 02:33:59.000000 risingwave-0.0.7/risingwave/test_udf.py
--rw-r--r--   0 wangrunji   (501) staff       (20)    13189 2023-05-17 02:33:59.000000 risingwave-0.0.7/risingwave/udf.py
-drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-05-17 02:34:30.190934 risingwave-0.0.7/risingwave.egg-info/
--rw-r--r--   0 wangrunji   (501) staff       (20)     2215 2023-05-17 02:34:30.000000 risingwave-0.0.7/risingwave.egg-info/PKG-INFO
--rw-r--r--   0 wangrunji   (501) staff       (20)      251 2023-05-17 02:34:30.000000 risingwave-0.0.7/risingwave.egg-info/SOURCES.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)        1 2023-05-17 02:34:30.000000 risingwave-0.0.7/risingwave.egg-info/dependency_links.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)       23 2023-05-17 02:34:30.000000 risingwave-0.0.7/risingwave.egg-info/requires.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)       11 2023-05-17 02:34:30.000000 risingwave-0.0.7/risingwave.egg-info/top_level.txt
--rw-r--r--   0 wangrunji   (501) staff       (20)       38 2023-05-17 02:34:30.191248 risingwave-0.0.7/setup.cfg
--rw-r--r--   0 wangrunji   (501) staff       (20)      661 2023-05-17 02:33:59.000000 risingwave-0.0.7/setup.py
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-06-13 10:36:45.251929 risingwave-0.0.8/
+-rw-r--r--   0 wangrunji   (501) staff       (20)     2215 2023-06-13 10:36:45.251782 risingwave-0.0.8/PKG-INFO
+-rw-r--r--   0 wangrunji   (501) staff       (20)     1859 2023-03-27 03:26:39.000000 risingwave-0.0.8/README.md
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-06-13 10:36:45.250857 risingwave-0.0.8/risingwave/
+-rw-r--r--   0 wangrunji   (501) staff       (20)        0 2023-03-17 09:49:44.000000 risingwave-0.0.8/risingwave/__init__.py
+-rw-r--r--   0 wangrunji   (501) staff       (20)     3120 2023-05-18 08:37:35.000000 risingwave-0.0.8/risingwave/test_udf.py
+-rw-r--r--   0 wangrunji   (501) staff       (20)    13962 2023-06-13 10:35:58.000000 risingwave-0.0.8/risingwave/udf.py
+drwxr-xr-x   0 wangrunji   (501) staff       (20)        0 2023-06-13 10:36:45.251560 risingwave-0.0.8/risingwave.egg-info/
+-rw-r--r--   0 wangrunji   (501) staff       (20)     2215 2023-06-13 10:36:45.000000 risingwave-0.0.8/risingwave.egg-info/PKG-INFO
+-rw-r--r--   0 wangrunji   (501) staff       (20)      251 2023-06-13 10:36:45.000000 risingwave-0.0.8/risingwave.egg-info/SOURCES.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)        1 2023-06-13 10:36:45.000000 risingwave-0.0.8/risingwave.egg-info/dependency_links.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)       23 2023-06-13 10:36:45.000000 risingwave-0.0.8/risingwave.egg-info/requires.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)       11 2023-06-13 10:36:45.000000 risingwave-0.0.8/risingwave.egg-info/top_level.txt
+-rw-r--r--   0 wangrunji   (501) staff       (20)       38 2023-06-13 10:36:45.251987 risingwave-0.0.8/setup.cfg
+-rw-r--r--   0 wangrunji   (501) staff       (20)      647 2023-06-13 10:35:58.000000 risingwave-0.0.8/setup.py
```

### Comparing `risingwave-0.0.7/PKG-INFO` & `risingwave-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risingwave
-Version: 0.0.7
+Version: 0.0.8
 Summary: RisingWave Python API
 Home-page: https://github.com/risingwavelabs/risingwave
 Author: RisingWave Labs
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `risingwave-0.0.7/README.md` & `risingwave-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `risingwave-0.0.7/risingwave/test_udf.py` & `risingwave-0.0.8/risingwave/test_udf.py`

 * *Files identical despite different names*

### Comparing `risingwave-0.0.7/risingwave/udf.py` & `risingwave-0.0.8/risingwave/udf.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,55 +31,79 @@
     """
     Base interface for user-defined scalar function. A user-defined scalar functions maps zero, one,
     or multiple scalar values to a new scalar value.
     """
 
     def __init__(self, *args, **kwargs):
         self._io_threads = kwargs.pop("io_threads")
-        self._executor = ThreadPoolExecutor(max_workers=self._io_threads) if self._io_threads is not None else None
+        self._executor = (
+            ThreadPoolExecutor(max_workers=self._io_threads)
+            if self._io_threads is not None
+            else None
+        )
         super().__init__(*args, **kwargs)
 
     def eval(self, *args) -> Any:
         """
         Method which defines the logic of the scalar function.
         """
         pass
 
     def eval_batch(self, batch: pa.RecordBatch) -> Iterator[pa.RecordBatch]:
         # parse value from json string for jsonb columns
         inputs = [[v.as_py() for v in array] for array in batch]
         inputs = [
-            _process_input_array(array, type)
+            _process_func(pa.list_(type), False)(array)
             for array, type in zip(inputs, self._input_schema.types)
         ]
         if self._executor is not None:
             # evaluate the function for each row
-            tasks = [self._executor.submit(self._func, *[col[i] for col in inputs])
-                    for i in range(batch.num_rows)]
-            column = [future.result() for future in concurrent.futures.as_completed(tasks)]
+            tasks = [
+                self._executor.submit(self._func, *[col[i] for col in inputs])
+                for i in range(batch.num_rows)
+            ]
+            column = [
+                future.result() for future in concurrent.futures.as_completed(tasks)
+            ]
         else:
             # evaluate the function for each row
-            column = [self.eval(*[col[i] for col in inputs]) for i in range(batch.num_rows)]
+            column = [
+                self.eval(*[col[i] for col in inputs]) for i in range(batch.num_rows)
+            ]
+
+        column = _process_func(pa.list_(self._result_schema.types[0]), True)(column)
 
-        # convert value to json for jsonb columns
-        if self._result_schema.types[0] == pa.large_string():
-            column = [(json.dumps(v) if v is not None else None) for v in column]
         array = pa.array(column, type=self._result_schema.types[0])
         yield pa.RecordBatch.from_arrays([array], schema=self._result_schema)
 
 
-def _process_input_array(array: list, type: pa.DataType) -> list:
+def _process_func(type: pa.DataType, output: bool) -> Callable:
+    """Return a function to process input or output value."""
     if pa.types.is_list(type):
-        return [
-            (_process_input_array(v, type.value_type) if v is not None else None)
-            for v in array
-        ]
+        func = _process_func(type.value_type, output)
+        return lambda array: [(func(v) if v is not None else None) for v in array]
+    if pa.types.is_struct(type):
+        funcs = [_process_func(field.type, output) for field in type]
+        if output:
+            return lambda tup: tuple(
+                (func(v) if v is not None else None) for v, func in zip(tup, funcs)
+            )
+        else:
+            # the input value of struct type is a dict
+            # we convert it into tuple here
+            return lambda map: tuple(
+                (func(v) if v is not None else None)
+                for v, func in zip(map.values(), funcs)
+            )
     if pa.types.is_large_string(type):
-        return [(json.loads(v) if v is not None else None) for v in array]
-    return array
+        if output:
+            return lambda v: json.dumps(v)
+        else:
+            return lambda v: json.loads(v)
+    return lambda v: v
 
 
 class TableFunction(UserDefinedFunction):
     """
     Base interface for user-defined table function. A user-defined table functions maps zero, one,
     or multiple scalar values to a new table value.
     """
@@ -103,19 +127,18 @@
                 self.schema = schema
                 self.columns = [[] for _ in self.schema.types]
 
             def len(self) -> int:
                 """Returns the number of rows in the RecordBatch being built."""
                 return len(self.columns[0])
 
-            def append(self, index: int, args: Tuple):
+            def append(self, index: int, value: Any):
                 """Appends a new row to the RecordBatch being built."""
                 self.columns[0].append(index)
-                for column, val in zip(self.columns[1:], args):
-                    column.append(val)
+                self.columns[1].append(value)
 
             def build(self) -> pa.RecordBatch:
                 """Builds the RecordBatch from the accumulated data and clears the state."""
                 # Convert the columns to arrow arrays
                 arrays = [
                     pa.array(col, type)
                     for col, type in zip(self.columns, self.schema.types)
@@ -125,18 +148,16 @@
                 return pa.RecordBatch.from_arrays(arrays, schema=self.schema)
 
         builder = RecordBatchBuilder(self._result_schema)
 
         # Iterate through rows in the input RecordBatch
         for row_index in range(batch.num_rows):
             row = tuple(column[row_index].as_py() for column in batch)
-            for result_row in self.eval(*row):
-                if not isinstance(result_row, tuple):
-                    result_row = (result_row,)
-                builder.append(row_index, result_row)
+            for result in self.eval(*row):
+                builder.append(row_index, result)
                 if builder.len() == self.BATCH_SIZE:
                     yield builder.build()
         if builder.len() != 0:
             yield builder.build()
 
 
 class UserDefinedScalarFunctionWrapper(ScalarFunction):
@@ -162,43 +183,52 @@
 
     def __call__(self, *args):
         return self._func(*args)
 
     def eval(self, *args):
         return self._func(*args)
 
+
 class UserDefinedTableFunctionWrapper(TableFunction):
     """
     Base Wrapper for Python user-defined table function.
     """
 
     _func: Callable
 
     def __init__(self, func, input_types, result_types, name=None):
         self._func = func
+        self._name = name or (
+            func.__name__ if hasattr(func, "__name__") else func.__class__.__name__
+        )
         self._input_schema = pa.schema(
             zip(
                 inspect.getfullargspec(func)[0],
                 [_to_data_type(t) for t in _to_list(input_types)],
             )
         )
         self._result_schema = pa.schema(
-            [("row_index", pa.int64())]
-            + [("", _to_data_type(t)) for t in _to_list(result_types)]
-        )
-        self._name = name or (
-            func.__name__ if hasattr(func, "__name__") else func.__class__.__name__
+            [
+                ("row_index", pa.int32()),
+                (
+                    self._name,
+                    pa.struct([("", _to_data_type(t)) for t in result_types])
+                    if isinstance(result_types, list)
+                    else _to_data_type(result_types),
+                ),
+            ]
         )
 
     def __call__(self, *args):
         return self._func(*args)
 
     def eval(self, *args):
         return self._func(*args)
 
+
 def _to_list(x):
     if isinstance(x, list):
         return x
     else:
         return [x]
 
 
@@ -232,17 +262,21 @@
     def external_api(x):
         response = requests.get(my_endpoint + '?param=' + x)
         return response["data"]
     ```
     """
 
     if io_threads is not None and io_threads > 1:
-        return lambda f: UserDefinedScalarFunctionWrapper(f, input_types, result_type, name, io_threads=io_threads)
+        return lambda f: UserDefinedScalarFunctionWrapper(
+            f, input_types, result_type, name, io_threads=io_threads
+        )
     else:
-        return lambda f: UserDefinedScalarFunctionWrapper(f, input_types, result_type, name)
+        return lambda f: UserDefinedScalarFunctionWrapper(
+            f, input_types, result_type, name
+        )
 
 
 def udtf(
     input_types: Union[List[Union[str, pa.DataType]], Union[str, pa.DataType]],
     result_types: Union[List[Union[str, pa.DataType]], Union[str, pa.DataType]],
     name: Optional[str] = None,
 ) -> Callable:
```

### Comparing `risingwave-0.0.7/risingwave.egg-info/PKG-INFO` & `risingwave-0.0.8/risingwave.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: risingwave
-Version: 0.0.7
+Version: 0.0.8
 Summary: RisingWave Python API
 Home-page: https://github.com/risingwavelabs/risingwave
 Author: RisingWave Labs
 Classifier: Programming Language :: Python
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `risingwave-0.0.7/setup.py` & `risingwave-0.0.8/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="risingwave",
-    version="0.0.7",
+    version="0.0.8",
     author="RisingWave Labs",
     description="RisingWave Python API",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/risingwavelabs/risingwave",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python",
         "License :: OSI Approved :: Apache Software License",
     ],
     python_requires=">=3.8",
-    install_requires=['pyarrow'],
-    extras_require={
-        'test': ['pytest']
-    },
+    install_requires=["pyarrow"],
+    extras_require={"test": ["pytest"]},
 )
```

