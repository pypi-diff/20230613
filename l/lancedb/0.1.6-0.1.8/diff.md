# Comparing `tmp/lancedb-0.1.6.tar.gz` & `tmp/lancedb-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lancedb-0.1.6.tar", last modified: Tue Jun  6 01:22:06 2023, max compression
+gzip compressed data, was "lancedb-0.1.8.tar", last modified: Mon Jun 12 22:36:00 2023, max compression
```

## Comparing `lancedb-0.1.6.tar` & `lancedb-0.1.8.tar`

### file list

```diff
@@ -1,21 +1,31 @@
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-06 01:22:06.577658 lancedb-0.1.6/
--rw-r--r--   0 changshe   (501) staff       (20)     1004 2023-06-06 01:22:06.577554 lancedb-0.1.6/PKG-INFO
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-06 01:22:06.576879 lancedb-0.1.6/lancedb/
--rw-r--r--   0 changshe   (501) staff       (20)      922 2023-05-05 18:26:36.000000 lancedb-0.1.6/lancedb/__init__.py
--rw-r--r--   0 changshe   (501) staff       (20)      889 2023-05-05 18:26:36.000000 lancedb-0.1.6/lancedb/common.py
--rw-r--r--   0 changshe   (501) staff       (20)     2981 2023-05-05 01:55:15.000000 lancedb-0.1.6/lancedb/context.py
--rw-r--r--   0 changshe   (501) staff       (20)     4134 2023-06-02 16:16:59.000000 lancedb-0.1.6/lancedb/db.py
--rw-r--r--   0 changshe   (501) staff       (20)     3758 2023-05-05 18:26:42.000000 lancedb-0.1.6/lancedb/embeddings.py
--rw-r--r--   0 changshe   (501) staff       (20)     3895 2023-06-06 01:19:03.000000 lancedb-0.1.6/lancedb/fts.py
--rw-r--r--   0 changshe   (501) staff       (20)     4936 2023-06-06 01:19:03.000000 lancedb-0.1.6/lancedb/query.py
--rw-r--r--   0 changshe   (501) staff       (20)     8861 2023-06-02 16:16:59.000000 lancedb-0.1.6/lancedb/table.py
--rw-r--r--   0 changshe   (501) staff       (20)     1800 2023-06-02 16:16:59.000000 lancedb-0.1.6/lancedb/util.py
-drwxr-xr-x   0 changshe   (501) staff       (20)        0 2023-06-06 01:22:06.577387 lancedb-0.1.6/lancedb.egg-info/
--rw-r--r--   0 changshe   (501) staff       (20)     1004 2023-06-06 01:22:06.000000 lancedb-0.1.6/lancedb.egg-info/PKG-INFO
--rw-r--r--   0 changshe   (501) staff       (20)      335 2023-06-06 01:22:06.000000 lancedb-0.1.6/lancedb.egg-info/SOURCES.txt
--rw-r--r--   0 changshe   (501) staff       (20)        1 2023-06-06 01:22:06.000000 lancedb-0.1.6/lancedb.egg-info/dependency_links.txt
--rw-r--r--   0 changshe   (501) staff       (20)      163 2023-06-06 01:22:06.000000 lancedb-0.1.6/lancedb.egg-info/requires.txt
--rw-r--r--   0 changshe   (501) staff       (20)        8 2023-06-06 01:22:06.000000 lancedb-0.1.6/lancedb.egg-info/top_level.txt
--rw-r--r--   0 changshe   (501) staff       (20)     1349 2023-06-06 01:19:17.000000 lancedb-0.1.6/pyproject.toml
--rw-r--r--   0 changshe   (501) staff       (20)       38 2023-06-06 01:22:06.577694 lancedb-0.1.6/setup.cfg
--rw-r--r--   0 changshe   (501) staff       (20)      660 2023-05-05 01:55:15.000000 lancedb-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:36:00.097548 lancedb-0.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-12 22:36:00.093548 lancedb-0.1.8/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:36:00.093548 lancedb-0.1.8/lancedb/
+-rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7013 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3963 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/fts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6282 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/query.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10879 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1800 2023-06-12 22:35:55.000000 lancedb-0.1.8/lancedb/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:36:00.093548 lancedb-0.1.8/lancedb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-06-12 22:36:00.000000 lancedb-0.1.8/lancedb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-06-12 22:36:00.000000 lancedb-0.1.8/lancedb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-12 22:36:00.000000 lancedb-0.1.8/lancedb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-12 22:36:00.000000 lancedb-0.1.8/lancedb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-12 22:36:00.000000 lancedb-0.1.8/lancedb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1360 2023-06-12 22:35:55.000000 lancedb-0.1.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-12 22:36:00.097548 lancedb-0.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-06-12 22:35:55.000000 lancedb-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-12 22:36:00.093548 lancedb-0.1.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3338 2023-06-12 22:35:55.000000 lancedb-0.1.8/tests/test_db.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1526 2023-06-12 22:35:55.000000 lancedb-0.1.8/tests/test_embeddings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-12 22:35:55.000000 lancedb-0.1.8/tests/test_fts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-06-12 22:35:55.000000 lancedb-0.1.8/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-06-12 22:35:55.000000 lancedb-0.1.8/tests/test_query.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-06-12 22:35:55.000000 lancedb-0.1.8/tests/test_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-06-12 22:35:55.000000 lancedb-0.1.8/tests/test_util.py
```

### Comparing `lancedb-0.1.6/PKG-INFO` & `lancedb-0.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1.6
+Version: 0.1.8
 Summary: lancedb
 Author-email: LanceDB Devs <dev@lancedb.com>
 Project-URL: repository, https://github.com/lancedb/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.1.6/lancedb/__init__.py` & `lancedb-0.1.8/lancedb/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,12 +18,25 @@
     """Connect to a LanceDB instance at the given URI
 
     Parameters
     ----------
     uri: str or Path
         The uri of the database.
 
+    Examples
+    --------
+
+    For a local directory, provide a path for the database:
+
+    >>> import lancedb
+    >>> db = lancedb.connect("~/.lancedb")
+
+    For object storage, use a URI prefix:
+
+    >>> db = lancedb.connect("s3://my-bucket/lancedb")
+
     Returns
     -------
-    A connection to a LanceDB database.
+    conn : LanceDBConnection
+        A connection to a LanceDB database.
     """
     return LanceDBConnection(uri)
```

### Comparing `lancedb-0.1.6/lancedb/common.py` & `lancedb-0.1.8/lancedb/common.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.6/lancedb/embeddings.py` & `lancedb-0.1.8/lancedb/embeddings.py`

 * *Files 26% similar despite different names*

```diff
@@ -25,15 +25,39 @@
 def with_embeddings(
     func: Callable,
     data: Union[pa.Table, pd.DataFrame],
     column: str = "text",
     wrap_api: bool = True,
     show_progress: bool = False,
     batch_size: int = 1000,
-):
+) -> pa.Table:
+    """Add a vector column to a table using the given embedding function.
+
+    The new columns will be called "vector".
+
+    Parameters
+    ----------
+    func : Callable
+        A function that takes a list of strings and returns a list of vectors.
+    data : pa.Table or pd.DataFrame
+        The data to add an embedding column to.
+    column : str, default "text"
+        The name of the column to use as input to the embedding function.
+    wrap_api : bool, default True
+        Whether to wrap the embedding function in a retry and rate limiter.
+    show_progress : bool, default False
+        Whether to show a progress bar.
+    batch_size : int, default 1000
+        The number of row values to pass to each call of the embedding function.
+
+    Returns
+    -------
+    pa.Table
+        The input table with a new column called "vector" containing the embeddings.
+    """
     func = EmbeddingFunction(func)
     if wrap_api:
         func = func.retry().rate_limit()
     func = func.batch_size(batch_size)
     if show_progress:
         func = func.show_progress()
     if isinstance(data, pd.DataFrame):
```

### Comparing `lancedb-0.1.6/lancedb/fts.py` & `lancedb-0.1.8/lancedb/fts.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,19 @@
     ----------
     index : tantivy.Index
         The index object
     table : LanceTable
         The table to index
     fields : List[str]
         List of fields to index
+
+    Returns
+    -------
+    int
+        The number of rows indexed
     """
     # first check the fields exist and are string or large string type
     for name in fields:
         f = table.schema.field(name)  # raises KeyError if not found
         if not pa.types.is_string(f.type) and not pa.types.is_large_string(f.type):
             raise TypeError(f"Field {name} is not a string type")
```

### Comparing `lancedb-0.1.6/lancedb/table.py` & `lancedb-0.1.8/lancedb/table.py`

 * *Files 12% similar despite different names*

```diff
@@ -43,14 +43,48 @@
         raise TypeError(f"Unsupported data type: {type(data)}")
     return data
 
 
 class LanceTable:
     """
     A table in a LanceDB database.
+
+    Examples
+    --------
+
+    Create using [LanceDBConnection.create_table][lancedb.LanceDBConnection.create_table]
+    (more examples in that method's documentation).
+
+    >>> import lancedb
+    >>> db = lancedb.connect("./.lancedb")
+    >>> table = db.create_table("my_table", data=[{"vector": [1.1, 1.2], "b": 2}])
+    >>> table.head()
+    pyarrow.Table
+    vector: fixed_size_list<item: float>[2]
+      child 0, item: float
+    b: int64
+    ----
+    vector: [[[1.1,1.2]]]
+    b: [[2]]
+
+    Can append new data with [LanceTable.add][lancedb.table.LanceTable.add].
+
+    >>> table.add([{"vector": [0.5, 1.3], "b": 4}])
+    2
+
+    Can query the table with [LanceTable.search][lancedb.table.LanceTable.search].
+
+    >>> table.search([0.4, 0.4]).select(["b"]).to_df()
+       b      vector  score
+    0  4  [0.5, 1.3]   0.82
+    1  2  [1.1, 1.2]   1.13
+
+    Search queries are much faster when an index is created. See
+    [LanceTable.create_index][lancedb.table.LanceTable.create_index].
+
     """
 
     def __init__(
         self, connection: "lancedb.db.LanceDBConnection", name: str, version: int = None
     ):
         self._conn = connection
         self.name = name
@@ -60,28 +94,60 @@
         try:
             del self.__dict__["_dataset"]
         except AttributeError:
             pass
 
     @property
     def schema(self) -> pa.Schema:
-        """Return the schema of the table."""
+        """Return the schema of the table.
+
+        Returns
+        -------
+        pa.Schema
+            A PyArrow schema object."""
         return self._dataset.schema
 
     def list_versions(self):
         """List all versions of the table"""
         return self._dataset.versions()
 
     @property
-    def version(self):
+    def version(self) -> int:
         """Get the current version of the table"""
         return self._dataset.version
 
     def checkout(self, version: int):
-        """Checkout a version of the table"""
+        """Checkout a version of the table. This is an in-place operation.
+
+        This allows viewing previous versions of the table.
+
+        Parameters
+        ----------
+        version : int
+            The version to checkout.
+
+        Examples
+        --------
+        >>> import lancedb
+        >>> db = lancedb.connect("./.lancedb")
+        >>> table = db.create_table("my_table", [{"vector": [1.1, 0.9], "type": "vector"}])
+        >>> table.version
+        1
+        >>> table.to_pandas()
+               vector    type
+        0  [1.1, 0.9]  vector
+        >>> table.add([{"vector": [0.5, 0.2], "type": "vector"}])
+        2
+        >>> table.version
+        2
+        >>> table.checkout(1)
+        >>> table.to_pandas()
+               vector    type
+        0  [1.1, 0.9]  vector
+        """
         max_ver = max([v["version"] for v in self._dataset.versions()])
         if version < 1 or version > max_ver:
             raise ValueError(f"Invalid version {version}")
         self._version = version
         self._reset_dataset()
 
     def __len__(self):
@@ -94,19 +160,28 @@
         return self.__repr__()
 
     def head(self, n=5) -> pa.Table:
         """Return the first n rows of the table."""
         return self._dataset.head(n)
 
     def to_pandas(self) -> pd.DataFrame:
-        """Return the table as a pandas DataFrame."""
+        """Return the table as a pandas DataFrame.
+
+        Returns
+        -------
+        pd.DataFrame
+        """
         return self.to_arrow().to_pandas()
 
     def to_arrow(self) -> pa.Table:
-        """Return the table as a pyarrow Table."""
+        """Return the table as a pyarrow Table.
+
+        Returns
+        -------
+        pa.Table"""
         return self._dataset.to_table()
 
     @property
     def _dataset_uri(self) -> str:
         return os.path.join(self._conn.uri, f"{self.name}.lance")
 
     def create_index(self, metric="L2", num_partitions=256, num_sub_vectors=96):
@@ -171,15 +246,16 @@
             The data to insert into the table.
         mode: str
             The mode to use when writing the data. Valid values are
             "append" and "overwrite".
 
         Returns
         -------
-        The number of vectors added to the table.
+        int
+            The number of vectors in the table.
         """
         data = _sanitize_data(data, self.schema)
         lance.write_dataset(data, self._dataset_uri, mode=mode)
         self._reset_dataset()
         return len(self)
 
     def search(self, query: Union[VEC, str]) -> LanceQueryBuilder:
@@ -189,18 +265,19 @@
         Parameters
         ----------
         query: list, np.ndarray
             The query vector.
 
         Returns
         -------
-        A LanceQueryBuilder object representing the query.
-        Once executed, the query returns selected columns, the vector,
-        and also the "score" column which is the distance between the query
-        vector and the returned vector.
+        LanceQueryBuilder
+            A query builder object representing the query.
+            Once executed, the query returns selected columns, the vector,
+            and also the "score" column which is the distance between the query
+            vector and the returned vector.
         """
         if isinstance(query, str):
             # fts
             return LanceFtsQueryBuilder(self, query)
 
         if isinstance(query, list):
             query = np.array(query)
@@ -261,8 +338,10 @@
     if not pa.types.is_list(vec_arr.type):
         raise TypeError(f"Unsupported vector column type: {vec_arr.type}")
     values = vec_arr.values
     if not pa.types.is_float32(values.type):
         values = values.cast(pa.float32())
     list_size = len(values) / len(data)
     vec_arr = pa.FixedSizeListArray.from_arrays(values, list_size)
-    return data.set_column(data.column_names.index(vector_column_name), vector_column_name, vec_arr)
+    return data.set_column(
+        data.column_names.index(vector_column_name), vector_column_name, vec_arr
+    )
```

### Comparing `lancedb-0.1.6/lancedb/util.py` & `lancedb-0.1.8/lancedb/util.py`

 * *Files identical despite different names*

### Comparing `lancedb-0.1.6/lancedb.egg-info/PKG-INFO` & `lancedb-0.1.8/lancedb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lancedb
-Version: 0.1.6
+Version: 0.1.8
 Summary: lancedb
 Author-email: LanceDB Devs <dev@lancedb.com>
 Project-URL: repository, https://github.com/lancedb/lancedb
 Keywords: data-format,data-science,machine-learning,arrow,data-analytics
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
```

### Comparing `lancedb-0.1.6/pyproject.toml` & `lancedb-0.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "lancedb"
-version = "0.1.6"
-dependencies = ["pylance>=0.4.17", "ratelimiter", "retry", "tqdm"]
+version = "0.1.8"
+dependencies = ["pylance>=0.4.20", "ratelimiter", "retry", "tqdm"]
 description = "lancedb"
 authors = [
     { name = "LanceDB Devs", email = "dev@lancedb.com" },
 ]
 license = { file = "LICENSE" }
 readme = "README.md"
 requires-python = ">=3.8"
@@ -33,15 +33,15 @@
 ]
 
 [project.urls]
 repository = "https://github.com/lancedb/lancedb"
 
 [project.optional-dependencies]
 tests = [
-    "pytest", "pytest-mock"
+    "pytest", "pytest-mock", "doctest"
 ]
 dev = [
     "ruff", "pre-commit", "black"
 ]
 docs = [
     "mkdocs", "mkdocs-jupyter", "mkdocs-material", "mkdocstrings[python]"
 ]
```

### Comparing `lancedb-0.1.6/setup.py` & `lancedb-0.1.8/setup.py`

 * *Files identical despite different names*

