# Comparing `tmp/arrow_pd_parser-1.3.7.tar.gz` & `tmp/arrow_pd_parser-1.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arrow_pd_parser-1.3.7.tar", max compression
+gzip compressed data, was "arrow_pd_parser-1.3.8.tar", max compression
```

## Comparing `arrow_pd_parser-1.3.7.tar` & `arrow_pd_parser-1.3.8.tar`

### file list

```diff
@@ -1,14 +1,13 @@
--rw-r--r--   0        0        0    12064 2023-02-06 16:44:31.133999 arrow_pd_parser-1.3.7/README.md
--rw-r--r--   0        0        0       22 2023-02-06 16:44:31.133999 arrow_pd_parser-1.3.7/arrow_pd_parser/__init__.py
--rw-r--r--   0        0        0    13642 2023-02-06 16:44:31.133999 arrow_pd_parser-1.3.7/arrow_pd_parser/_arrow_parsers.py
--rw-r--r--   0        0        0     4059 2023-02-06 16:44:31.133999 arrow_pd_parser-1.3.7/arrow_pd_parser/_export.py
--rw-r--r--   0        0        0    14573 2023-02-06 16:44:31.133999 arrow_pd_parser-1.3.7/arrow_pd_parser/_readers.py
--rw-r--r--   0        0        0    13996 2023-02-06 16:44:31.133999 arrow_pd_parser-1.3.7/arrow_pd_parser/_writers.py
--rw-r--r--   0        0        0    10434 2023-02-06 16:44:31.133999 arrow_pd_parser-1.3.7/arrow_pd_parser/caster.py
--rw-r--r--   0        0        0     4413 2023-02-06 16:44:31.133999 arrow_pd_parser-1.3.7/arrow_pd_parser/pa_pd.py
--rw-r--r--   0        0        0     2839 2023-02-06 16:44:31.133999 arrow_pd_parser-1.3.7/arrow_pd_parser/reader.py
--rw-r--r--   0        0        0     3815 2023-02-06 16:44:31.133999 arrow_pd_parser-1.3.7/arrow_pd_parser/utils.py
--rw-r--r--   0        0        0     1580 2023-02-06 16:44:31.133999 arrow_pd_parser-1.3.7/arrow_pd_parser/writer.py
--rw-r--r--   0        0        0     1443 2023-02-06 16:44:31.133999 arrow_pd_parser-1.3.7/pyproject.toml
--rw-r--r--   0        0        0    13160 1970-01-01 00:00:00.000000 arrow_pd_parser-1.3.7/setup.py
--rw-r--r--   0        0        0    12859 1970-01-01 00:00:00.000000 arrow_pd_parser-1.3.7/PKG-INFO
+-rw-r--r--   0        0        0    12064 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/README.md
+-rw-r--r--   0        0        0       22 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/__init__.py
+-rw-r--r--   0        0        0    13642 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/_arrow_parsers.py
+-rw-r--r--   0        0        0     4059 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/_export.py
+-rw-r--r--   0        0        0    14789 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/_readers.py
+-rw-r--r--   0        0        0    14430 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/_writers.py
+-rw-r--r--   0        0        0    10434 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/caster.py
+-rw-r--r--   0        0        0     4413 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/pa_pd.py
+-rw-r--r--   0        0        0     2839 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/reader.py
+-rw-r--r--   0        0        0     3815 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/utils.py
+-rw-r--r--   0        0        0     1580 2023-06-13 12:04:04.636680 arrow_pd_parser-1.3.8/arrow_pd_parser/writer.py
+-rw-r--r--   0        0        0     1460 2023-06-13 12:04:04.640679 arrow_pd_parser-1.3.8/pyproject.toml
+-rw-r--r--   0        0        0    12859 1970-01-01 00:00:00.000000 arrow_pd_parser-1.3.8/PKG-INFO
```

### Comparing `arrow_pd_parser-1.3.7/README.md` & `arrow_pd_parser-1.3.8/README.md`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.7/arrow_pd_parser/_arrow_parsers.py` & `arrow_pd_parser-1.3.8/arrow_pd_parser/_arrow_parsers.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.7/arrow_pd_parser/_export.py` & `arrow_pd_parser-1.3.8/arrow_pd_parser/_export.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.7/arrow_pd_parser/_readers.py` & `arrow_pd_parser-1.3.8/arrow_pd_parser/_readers.py`

 * *Files 5% similar despite different names*

```diff
@@ -181,14 +181,19 @@
             # If metadata is provided force
             # str read in ready for type conversion
             if "low_memory" not in kwargs:
                 kwargs["low_memory"] = False
             if "dtype" not in kwargs:
                 kwargs["dtype"] = str
 
+        if "ignore_unnamed_columns" in kwargs:
+            if "usecols" not in kwargs:
+                kwargs["usecols"] = lambda c: not c.startswith("Unnamed:")
+            _ = kwargs.pop("ignore_unnamed_columns")
+
         if is_s3_filepath(input_path):
             reader = wr.s3.read_csv
         else:
             reader = pd.read_csv
 
         if is_iterable:
             df = self._read_iterable(
```

### Comparing `arrow_pd_parser-1.3.7/arrow_pd_parser/_writers.py` & `arrow_pd_parser-1.3.8/arrow_pd_parser/_writers.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 from abc import ABC, abstractmethod
 from dataclasses import dataclass, field
 from typing import IO, Dict, Iterable, List, Union
 
 import numpy as np
 import pandas as pd
 import pyarrow as pa
+import pyarrow.fs as fs
 import pyarrow.parquet as pq
 import smart_open
 from mojap_metadata import Metadata
 from mojap_metadata.converters.arrow_converter import ArrowConverter
 
 from arrow_pd_parser.utils import (
     EngineNotImplementedError,
@@ -321,15 +322,28 @@
         with pq.ParquetWriter(
             where=output_path, schema=table.schema, **kwargs
         ) as parquet_writer:
             parquet_writer.write_table(table)
             for chunk in df:
                 table = pa.Table.from_pandas(chunk, schema=arrow_schema)
                 parquet_writer.write_table(table)
-        written_arrow_schema = pq.read_schema(output_path)
+
+        if output_path.startswith("s3://"):
+            s3 = fs.S3FileSystem(
+                region=os.getenv(
+                    "AWS_REGION", os.getenv("AWS_DEFAULT_REGION", "eu-west-1")
+                )
+            )
+            pa_pth = output_path.replace("s3://", "")
+            with s3.open_input_file(pa_pth) as file:
+                written_arrow_schema = pq.read_schema(file)
+
+        else:
+            written_arrow_schema = pq.read_schema(output_path)
+
         if arrow_schema:
             mismatched_types = {}
             for i, written_col in enumerate(written_arrow_schema):
                 schema_col = arrow_schema[i]
                 if not written_col.equals(schema_col):
                     mismatched_types[written_col.name] = {
                         "type_in_schema": schema_col.type,
@@ -352,15 +366,14 @@
         self._write(engine="pyarrow", **kwargs)
 
 
 def get_writer_for_file_format(
     file_format: Union[FileFormat, str],
     writer_engine: str = None,
 ) -> DataFrameFileWriter:
-
     # Convert to enum
     if isinstance(file_format, str):
         file_format = FileFormat.from_string(file_format)
 
     implemented_engines = ["pandas", "arrow"]
     default_engines = {
         FileFormat.CSV: "pandas",
```

### Comparing `arrow_pd_parser-1.3.7/arrow_pd_parser/caster.py` & `arrow_pd_parser-1.3.8/arrow_pd_parser/caster.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.7/arrow_pd_parser/pa_pd.py` & `arrow_pd_parser-1.3.8/arrow_pd_parser/pa_pd.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.7/arrow_pd_parser/reader.py` & `arrow_pd_parser-1.3.8/arrow_pd_parser/reader.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.7/arrow_pd_parser/utils.py` & `arrow_pd_parser-1.3.8/arrow_pd_parser/utils.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.7/arrow_pd_parser/writer.py` & `arrow_pd_parser-1.3.8/arrow_pd_parser/writer.py`

 * *Files identical despite different names*

### Comparing `arrow_pd_parser-1.3.7/pyproject.toml` & `arrow_pd_parser-1.3.8/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arrow_pd_parser"
-version = "1.3.7"
+version = "1.3.8"
 description = "MoJ arrow-pd-parser"
 authors = ["Karik Isichei <karik.isichei@digital.justice.gov.uk>",
            "Alec Johnson <alec.johnson@digital.justice.gov.uk>",
            "Kimberley Brett <kimberley.brett@digital.justice.gov.uk>",
            "Thomas Hirsch <thomas.hirsch@digital.justice.gov.uk>",
            "Jacob Browning <jacob.browning@digital.justice.gov.uk>",
            "Jacob Hamblin-Pyke <jacob.hamblin-pyke@digital.justice.gov.uk>",
@@ -30,11 +30,12 @@
 [tool.poetry.dev-dependencies]
 pytest = ">=6.1"
 flake8 = "^3.8.4"
 black = ">=21.8b0"
 yamllint = ">=1.26.3"
 toml = "^0.10.2"
 pre-commit = "^2.19.0"
+moto = ">=3.1.6"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `arrow_pd_parser-1.3.7/setup.py` & `arrow_pd_parser-1.3.8/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,34 +1,292 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: arrow-pd-parser
+Version: 1.3.8
+Summary: MoJ arrow-pd-parser
+Home-page: https://github.com/moj-analytical-services/mojap-arrow-pd-parser
+Author: Karik Isichei
+Author-email: karik.isichei@digital.justice.gov.uk
+Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: awswrangler (>=2.4.0)
+Requires-Dist: mojap-metadata[arrow] (>=1.10.0,<2.0.0)
+Requires-Dist: pandas (>=1.2)
+Requires-Dist: pyarrow (>=6.0.0)
+Requires-Dist: smart-open (>=5.2.1,<6.0.0)
+Project-URL: Repository, https://github.com/moj-analytical-services/mojap-arrow-pd-parser
+Description-Content-Type: text/markdown
 
-packages = \
-['arrow_pd_parser']
+# mojap-arrow-pd-parser
 
-package_data = \
-{'': ['*']}
+Using pyArrow/Pandas to read CSV, JSONL and Parquet ensuring that you get the best representation of the column types in the resulting Pandas dataframe. Also ensures data type conformance by maintaining column types when reading and writing data back into Pandas (even when round tripping across multiple data types).
 
-install_requires = \
-['awswrangler>=2.4.0',
- 'mojap-metadata[arrow]>=1.10.0,<2.0.0',
- 'pandas>=1.2',
- 'pyarrow>=6.0.0',
- 'smart-open>=5.2.1,<6.0.0']
-
-setup_kwargs = {
-    'name': 'arrow-pd-parser',
-    'version': '1.3.7',
-    'description': 'MoJ arrow-pd-parser',
-    'long_description': '# mojap-arrow-pd-parser\n\nUsing pyArrow/Pandas to read CSV, JSONL and Parquet ensuring that you get the best representation of the column types in the resulting Pandas dataframe. Also ensures data type conformance by maintaining column types when reading and writing data back into Pandas (even when round tripping across multiple data types).\n\nThis package also can read in data given an [MoJ-Metadata](https://github.com/moj-analytical-services/mojap-metadata) schema again to result in a Pandas dataframe that best represents the provided schema.\n\nCan also be used to write data back to supported formats using Pandas (for CSV/JSONL) and PyArrow (for Parquet).\n\n## Installation\n\n```\npip install arrow-pd-parser\n```\n\nor via GitHub\n\n```\npip install arrow-pd-parser @ git+https://github.com/moj-analytical-services/mojap-arrow-pd-parser\n```\n\n## Basic Usage\n\nThis package uses `PyArrow` and/or `Pandas` to parse CSVs, JSONL and Parquet files and convert them to a Pandas Dataframe that are the best representation of those datatypes and ensure conformance between them. Also can write data back into the above formats to still maintain conformance to the provided schema.\n\n```python\nfrom arrow_pd_parser import reader, writer\n\ndf1 = reader.read("tests/data/all_types.csv")\ndf1.dtypes\n\n# i                     Int64\n# my_bool             boolean\n# my_nullable_bool    boolean\n#\xa0my_date              object\n# my_datetime          object\n# my_int                Int64\n# my_string            string\n\ndf2 = reader.read("tests/data/all_types.jsonl")\ndf2.dtypes # Note that Pandas struggles with nullable booleans when it reads JSONL (hence it is an Int64)\n\n# Write the dataframe to parquet\n# note deafult settings for the parquet writer is to\n# compress using snappy. (compression is not inferred from filepath but may do in future releases)\nwriter.write(df1, "new_output.snappy.parquet")\n```\n\nNote that the default behavior of this package is to utilise the new pandas datatypes for Integers, Booleans and Strings that represent Nulls as `pd.NA()`. Dates are returned as nullable objects of `datetime.date()` type and timestamps are `datetime.datetime()`. By default we enforce these types instead of the native pandas timestamp as the indexing for the Pandas timestamp is nanoseconds and can cause dates to be out of bounds. See the [timestamps](#timestamps) section for more details.\n\nThe `reader.read()` method will infer what the file format is based on the extension of your filepath failing that it will take the format from your metadata if provided. By default the reader.read() will use the following readers for the prescribed file format.\n\n| Data Type | Reader | Writer |\n|-----------|--------|--------|\n| CSV       | Pandas | Pandas |\n| JSONL     | Pandas | Pandas |\n| Parquet   | Arrow  | Arrow  |\n\nYou can also specify the file format in the reader and writer function or specify the reader type:\n\n```python\nfrom arrow_pd_parser import reader, writer\n\n# Specifying the reader\n#\xa0Both reader statements are equivalent and call the same readers\n# under the hood\ndf1 = reader.read("tests/data/all_types.csv", file_format="csv")\ndf2 = reader.csv.read("tests/data/all_types.csv")\n\n# You can also pass the reader args to the reader as kwargs\ndf3 = reader.csv.read("tests/data/all_types.csv", nrows = 2)\n\n# The writer API has the same functionality\nwriter.write(df1, file_format="parquet")\nwriter.parquet.write(df1)\n```\n\n### Use of Metadata\n\nThe main usefulness of this repo comes from specifying metadata for the data you want. We are going to focus on CSV and JSONL in this section as Parquet becomes a bit more nuanced as it encodes data types (unlike CSV and JSONL that can be more vague).\n\nWhen reading and writing you can specify metadata (using our [metadata schema definitions](https://github.com/moj-analytical-services/mojap-metadata)) to ensure the data read into pandas conforms.\n\n```python\nfrom arrow_pd_parser import reader\n\n# If no meta is provided we let the reader infer type\ndf1 = reader.read("tests/data/all_types.csv")\ndf1.dtypes\n\n# i                     Int64\n# my_bool             boolean\n# my_nullable_bool    boolean\n#\xa0my_date              object\n# my_datetime          object\n# my_int                Int64\n# my_string            string\n\n# If metadata is provided we ensure conformance\nmeta = {\n    "columns": [\n        {"name": "my_bool", "type": "string"},\n        {"name": "my_nullable_bool", "type": "bool"},\n        {"name": "my_date", "type": "string"},\n        {"name": "my_datetime", "type": "string"},\n        {"name": "my_int", "type": "float64"},\n        {"name": "my_string", "type": "string"}\n    ]\n}\ndf2 = reader.read("tests/data/all_types.csv", metadata=meta)\ndf2.dtypes\n\n# i                     Int64\n# my_bool              string\n# my_nullable_bool    boolean\n#\xa0my_date              string\n# my_datetime          string\n# my_int              float64\n# my_string            string\n\ndf3 = reader.read("tests/data/all_types.jsonl", metadata=meta)\ndf3.dtypes\n\nassert df2.dtypes.to_list() == df3.dtypes.to_list()\n```\n\nAs of the v1 release we expect the API for reading and writing will remain the same but will still be lacking in how the caster works (what is called under the hood when casting the data to the prescribed metadata). The caster should improve with subsequent releases.\n\n## Advanced Usage\n\n### Parameterising your reader and writer\n\nWhen using the `reader.read()` or `writer.write()` it pulls the default method with their default settings. However, if you want to customise your reader/writer you can do.\n\n\n#### Passing arguments to the reader\n\nYou can pass arguments to the underlying reader that is used to read data in. In the example below we use the nrows arg in pd.`pd.read_csv` that is used for our underlying reader.\n\n```python\nfrom arrow_pd_parser import reader\n\n# Passing args to the read function.\ndf = reader.csv.read("tests/data/all_types.jsonl", nrows=1000)\n```\n\n#### Reader and Writer settings\n\nThe readers and writers have some settings that you can use to configure how it reads/writes data. One of the main settings is how we deal with Pandas types. We default to the new pandas Series types: `StringDtype` for `string`, `BooleanDtype` for `bool` and `Int64Dtype` for `integer`. We also force dates and timestamps to be a series of objects (see the Timestamp section below)[#Reader-Pandas-Timestamps]. To change what pandas types to use you can change the reader settings:\n\n```python\nfrom arrow_pd_parser.reader import csv\nfrom io import StringIO\n\ncsv.pd_integer = False\ncsv.pd_string = False\ncsv.bool_map = {"Yes": True, "No": False}\n\ndata = """\nint_col,str_col,bool_col\n1,"Hello, mate",Yes\n2,Hi,No\n"""\nmeta = {\n    "columns": [\n        {"name": "int_col", "type": "int64"},\n        {"name": "str_col", "type": "string"},\n        {"name": "bool_col", "type": "bool"},\n    ]\n}\nf = StringIO(data)\ndf = csv.read(f, metadata = meta)\ndf.dtypes\n# int_col       int64\n# str_col      object\n# bool_col    boolean\n```\n\n####\xa0Using your own reader\n\nIf you wanted to create your own instance of a reader that wasn\'t the default provided you can.\n\n```python\nfrom arrow_pd_parser.reader import PandasCsvReader, csv\n\n\n# But you can also create your own and init the settings\nspecific_csv = PandasCsvReader(\n    pd_integer = False,\n    pd_string = False,\n    bool_map = {"Yes": True, "No": False}\n)\n\n# This may come in handy if you want to have two instances of a CSV reader with different settings\ndf1 = csv.read("tests/data/all_types.csv") # default reader\ndf2 = specific_csv.read("tests/data/all_types.csv")\n```\n\n#### Reading and Writing Parquet\n\nThe default parquet reader and writer uses Arrow under the hood. This also means it uses a different method for casting datatypes (it is done in Arrow not with Pandas). Because parquet is stricter, most likely if there is a deviation from your metadata it will fail to cast. When you provide metadata to the reader and writer, the API forces the data to that metadata. This makes sense for CSV and JSONL, but may make less sense for parquet. Therefore when using the parquet reader and writer you might want to consider if you want to provide your metadata. This may still be advantagous to check that the parquet matches metadata schema you have for the data.\n\nIn some cases (see [this issue](https://github.com/apache/arrow/issues/15032)) pyarrow will silently convert some data types when writing a parquet file, overriding the provided metadata. The `writer` will raise a warning if this happens, and you may wish to update your metdata so it matches the type that arrow expects.\n\n```python\nfrom arrow_pd_parser import reader, writer\n\n# Note all readers (CSV, JSONL and Parquet) support S3 paths in the following way\ndf = reader.parquet.read("s3://bucket/in.snappy.parquet")\nwriter.parquet.write("s3://bucket/out.snappy.parquet")\n\nprint(writer.parquet.compression, writer.parquet.version)\n# The default settings for the Parquet writer are snappy compression and version = \'2.0\'\n# These are passed to the arrow parquet write method but can either be changed by setting the\n# properties or by passing them as kwargs (which will super seed the default properties) e.g.\nwriter.parquet.write("s3://bucket/out.parquet", compression=None, version=\'1.0\')\n```\n\n#### Pandas Timestamps\n\nWhen metadata is provided (or for all Arrow Readers without metadata) we default to dates and datetimes as a series of objects rather than the Pandas timestamps this is because Pandas timestamps (currently) only support nanosecond resolution which is not ideal for a lot of timestamps as the range can be often too small.\n\n```python\nimport pandas as pd\npd.Timestamp.min # Timestamp(\'1677-09-22 00:12:43.145225\')\n\npd.Timestamp.max # Timestamp(\'2262-04-11 23:47:16.854775807\')\n```\n\nWhereas Spark 3.0 (for example) allows timestamps from `0001-01-01 00:00:00` to `9999-12-31 23:59:59.999999` ([source](https://databricks.com/blog/2020/07/22/a-comprehensive-look-at-dates-and-timestamps-in-apache-spark-3-0.html)). By default we do not allow Timestamps for this reason instead we use the python native datetime class as default for our types (wrapped in a Pandas object column type). Users can specify other Pandas date/timestamp using the `pd_timestamp_type` parameter which can either be `object` (default), `pd_timestamp` or `pd_period`.\n\nWhen setting `pd_timestamp_type=pd_period` pd_arrow_parser will identify the correct pandas period resolution based on the arrow column type.\n\n```python\nfrom arrow_pd_parser.reader import csv\n\n# The Pandas Period\ncsv.pd_timestamp_type="pd_period"\ndf = csv.read("tests/data/datetime_type.csv")\ndf.my_datetime.dtype # "period[S]"\n\n# Use pandas timestamp\ncsv.pd_timestamp_type="pd_timestamp"\ndf = csv.read("tests/data/datetime_type.csv")\ndf.my_datetime.dtype # dtype(\'<M8[ns]\')\n```\n\n#### Reading and writing large datasets\n\nDatasets that are too large to fit into memory can be read in chunks. If the `chunksize` parameter is given to `reader.read` then an iterator of dataframes is returned rather than a single dataframe. `chunksize` can be an integer indicating the number of rows each chunk contains, or a string indicating the amount of memory each chunk should fill, e.g. "1 GB". Note that the memory size should not fill available memory as some overhead is required for reading and writing. The `writer.write` function can then use these iterators instead of a dataframe.\n\n```python\nfrom arrow_pd_parser import reader, writer\n\ndf_iter = reader.read("s3://my_bucket/csv_data/my_table.csv", chunksize=10000)\nwriter.write(df_iter, "s3://my_bucket/parquet_data/my_table.parquet")\n```\n\nIf the dataframe needs transforming before writing then use a generator.\n\n```python\nfrom arrow_pd_parser import reader, writer\n\ndef transform(df):\n    # do something\n    return df\n\ndf_iter = reader.read("s3://my_bucket/csv_data/my_table.csv", chunksize="500MB")\n# Using a generator comprehension\ndf_transformed_iter = (transform(df) for df in df_iter)\nwriter.write(df_transformed_iter, "s3://my_bucket/parquet_data/my_transformed_table.parquet")\n```\n',
-    'author': 'Karik Isichei',
-    'author_email': 'karik.isichei@digital.justice.gov.uk',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/moj-analytical-services/mojap-arrow-pd-parser',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
+This package also can read in data given an [MoJ-Metadata](https://github.com/moj-analytical-services/mojap-metadata) schema again to result in a Pandas dataframe that best represents the provided schema.
+
+Can also be used to write data back to supported formats using Pandas (for CSV/JSONL) and PyArrow (for Parquet).
+
+## Installation
+
+```
+pip install arrow-pd-parser
+```
+
+or via GitHub
+
+```
+pip install arrow-pd-parser @ git+https://github.com/moj-analytical-services/mojap-arrow-pd-parser
+```
+
+## Basic Usage
+
+This package uses `PyArrow` and/or `Pandas` to parse CSVs, JSONL and Parquet files and convert them to a Pandas Dataframe that are the best representation of those datatypes and ensure conformance between them. Also can write data back into the above formats to still maintain conformance to the provided schema.
+
+```python
+from arrow_pd_parser import reader, writer
+
+df1 = reader.read("tests/data/all_types.csv")
+df1.dtypes
+
+# i                     Int64
+# my_bool             boolean
+# my_nullable_bool    boolean
+# my_date              object
+# my_datetime          object
+# my_int                Int64
+# my_string            string
+
+df2 = reader.read("tests/data/all_types.jsonl")
+df2.dtypes # Note that Pandas struggles with nullable booleans when it reads JSONL (hence it is an Int64)
+
+# Write the dataframe to parquet
+# note deafult settings for the parquet writer is to
+# compress using snappy. (compression is not inferred from filepath but may do in future releases)
+writer.write(df1, "new_output.snappy.parquet")
+```
+
+Note that the default behavior of this package is to utilise the new pandas datatypes for Integers, Booleans and Strings that represent Nulls as `pd.NA()`. Dates are returned as nullable objects of `datetime.date()` type and timestamps are `datetime.datetime()`. By default we enforce these types instead of the native pandas timestamp as the indexing for the Pandas timestamp is nanoseconds and can cause dates to be out of bounds. See the [timestamps](#timestamps) section for more details.
+
+The `reader.read()` method will infer what the file format is based on the extension of your filepath failing that it will take the format from your metadata if provided. By default the reader.read() will use the following readers for the prescribed file format.
+
+| Data Type | Reader | Writer |
+|-----------|--------|--------|
+| CSV       | Pandas | Pandas |
+| JSONL     | Pandas | Pandas |
+| Parquet   | Arrow  | Arrow  |
+
+You can also specify the file format in the reader and writer function or specify the reader type:
+
+```python
+from arrow_pd_parser import reader, writer
+
+# Specifying the reader
+# Both reader statements are equivalent and call the same readers
+# under the hood
+df1 = reader.read("tests/data/all_types.csv", file_format="csv")
+df2 = reader.csv.read("tests/data/all_types.csv")
+
+# You can also pass the reader args to the reader as kwargs
+df3 = reader.csv.read("tests/data/all_types.csv", nrows = 2)
+
+# The writer API has the same functionality
+writer.write(df1, file_format="parquet")
+writer.parquet.write(df1)
+```
+
+### Use of Metadata
+
+The main usefulness of this repo comes from specifying metadata for the data you want. We are going to focus on CSV and JSONL in this section as Parquet becomes a bit more nuanced as it encodes data types (unlike CSV and JSONL that can be more vague).
+
+When reading and writing you can specify metadata (using our [metadata schema definitions](https://github.com/moj-analytical-services/mojap-metadata)) to ensure the data read into pandas conforms.
+
+```python
+from arrow_pd_parser import reader
+
+# If no meta is provided we let the reader infer type
+df1 = reader.read("tests/data/all_types.csv")
+df1.dtypes
+
+# i                     Int64
+# my_bool             boolean
+# my_nullable_bool    boolean
+# my_date              object
+# my_datetime          object
+# my_int                Int64
+# my_string            string
+
+# If metadata is provided we ensure conformance
+meta = {
+    "columns": [
+        {"name": "my_bool", "type": "string"},
+        {"name": "my_nullable_bool", "type": "bool"},
+        {"name": "my_date", "type": "string"},
+        {"name": "my_datetime", "type": "string"},
+        {"name": "my_int", "type": "float64"},
+        {"name": "my_string", "type": "string"}
+    ]
 }
+df2 = reader.read("tests/data/all_types.csv", metadata=meta)
+df2.dtypes
+
+# i                     Int64
+# my_bool              string
+# my_nullable_bool    boolean
+# my_date              string
+# my_datetime          string
+# my_int              float64
+# my_string            string
+
+df3 = reader.read("tests/data/all_types.jsonl", metadata=meta)
+df3.dtypes
+
+assert df2.dtypes.to_list() == df3.dtypes.to_list()
+```
+
+As of the v1 release we expect the API for reading and writing will remain the same but will still be lacking in how the caster works (what is called under the hood when casting the data to the prescribed metadata). The caster should improve with subsequent releases.
+
+## Advanced Usage
+
+### Parameterising your reader and writer
+
+When using the `reader.read()` or `writer.write()` it pulls the default method with their default settings. However, if you want to customise your reader/writer you can do.
+
+
+#### Passing arguments to the reader
+
+You can pass arguments to the underlying reader that is used to read data in. In the example below we use the nrows arg in pd.`pd.read_csv` that is used for our underlying reader.
+
+```python
+from arrow_pd_parser import reader
+
+# Passing args to the read function.
+df = reader.csv.read("tests/data/all_types.jsonl", nrows=1000)
+```
+
+#### Reader and Writer settings
+
+The readers and writers have some settings that you can use to configure how it reads/writes data. One of the main settings is how we deal with Pandas types. We default to the new pandas Series types: `StringDtype` for `string`, `BooleanDtype` for `bool` and `Int64Dtype` for `integer`. We also force dates and timestamps to be a series of objects (see the Timestamp section below)[#Reader-Pandas-Timestamps]. To change what pandas types to use you can change the reader settings:
+
+```python
+from arrow_pd_parser.reader import csv
+from io import StringIO
+
+csv.pd_integer = False
+csv.pd_string = False
+csv.bool_map = {"Yes": True, "No": False}
+
+data = """
+int_col,str_col,bool_col
+1,"Hello, mate",Yes
+2,Hi,No
+"""
+meta = {
+    "columns": [
+        {"name": "int_col", "type": "int64"},
+        {"name": "str_col", "type": "string"},
+        {"name": "bool_col", "type": "bool"},
+    ]
+}
+f = StringIO(data)
+df = csv.read(f, metadata = meta)
+df.dtypes
+# int_col       int64
+# str_col      object
+# bool_col    boolean
+```
+
+#### Using your own reader
+
+If you wanted to create your own instance of a reader that wasn't the default provided you can.
+
+```python
+from arrow_pd_parser.reader import PandasCsvReader, csv
+
+
+# But you can also create your own and init the settings
+specific_csv = PandasCsvReader(
+    pd_integer = False,
+    pd_string = False,
+    bool_map = {"Yes": True, "No": False}
+)
+
+# This may come in handy if you want to have two instances of a CSV reader with different settings
+df1 = csv.read("tests/data/all_types.csv") # default reader
+df2 = specific_csv.read("tests/data/all_types.csv")
+```
+
+#### Reading and Writing Parquet
+
+The default parquet reader and writer uses Arrow under the hood. This also means it uses a different method for casting datatypes (it is done in Arrow not with Pandas). Because parquet is stricter, most likely if there is a deviation from your metadata it will fail to cast. When you provide metadata to the reader and writer, the API forces the data to that metadata. This makes sense for CSV and JSONL, but may make less sense for parquet. Therefore when using the parquet reader and writer you might want to consider if you want to provide your metadata. This may still be advantagous to check that the parquet matches metadata schema you have for the data.
+
+In some cases (see [this issue](https://github.com/apache/arrow/issues/15032)) pyarrow will silently convert some data types when writing a parquet file, overriding the provided metadata. The `writer` will raise a warning if this happens, and you may wish to update your metdata so it matches the type that arrow expects.
+
+```python
+from arrow_pd_parser import reader, writer
+
+# Note all readers (CSV, JSONL and Parquet) support S3 paths in the following way
+df = reader.parquet.read("s3://bucket/in.snappy.parquet")
+writer.parquet.write("s3://bucket/out.snappy.parquet")
+
+print(writer.parquet.compression, writer.parquet.version)
+# The default settings for the Parquet writer are snappy compression and version = '2.0'
+# These are passed to the arrow parquet write method but can either be changed by setting the
+# properties or by passing them as kwargs (which will super seed the default properties) e.g.
+writer.parquet.write("s3://bucket/out.parquet", compression=None, version='1.0')
+```
+
+#### Pandas Timestamps
+
+When metadata is provided (or for all Arrow Readers without metadata) we default to dates and datetimes as a series of objects rather than the Pandas timestamps this is because Pandas timestamps (currently) only support nanosecond resolution which is not ideal for a lot of timestamps as the range can be often too small.
+
+```python
+import pandas as pd
+pd.Timestamp.min # Timestamp('1677-09-22 00:12:43.145225')
+
+pd.Timestamp.max # Timestamp('2262-04-11 23:47:16.854775807')
+```
+
+Whereas Spark 3.0 (for example) allows timestamps from `0001-01-01 00:00:00` to `9999-12-31 23:59:59.999999` ([source](https://databricks.com/blog/2020/07/22/a-comprehensive-look-at-dates-and-timestamps-in-apache-spark-3-0.html)). By default we do not allow Timestamps for this reason instead we use the python native datetime class as default for our types (wrapped in a Pandas object column type). Users can specify other Pandas date/timestamp using the `pd_timestamp_type` parameter which can either be `object` (default), `pd_timestamp` or `pd_period`.
+
+When setting `pd_timestamp_type=pd_period` pd_arrow_parser will identify the correct pandas period resolution based on the arrow column type.
+
+```python
+from arrow_pd_parser.reader import csv
+
+# The Pandas Period
+csv.pd_timestamp_type="pd_period"
+df = csv.read("tests/data/datetime_type.csv")
+df.my_datetime.dtype # "period[S]"
+
+# Use pandas timestamp
+csv.pd_timestamp_type="pd_timestamp"
+df = csv.read("tests/data/datetime_type.csv")
+df.my_datetime.dtype # dtype('<M8[ns]')
+```
+
+#### Reading and writing large datasets
+
+Datasets that are too large to fit into memory can be read in chunks. If the `chunksize` parameter is given to `reader.read` then an iterator of dataframes is returned rather than a single dataframe. `chunksize` can be an integer indicating the number of rows each chunk contains, or a string indicating the amount of memory each chunk should fill, e.g. "1 GB". Note that the memory size should not fill available memory as some overhead is required for reading and writing. The `writer.write` function can then use these iterators instead of a dataframe.
+
+```python
+from arrow_pd_parser import reader, writer
+
+df_iter = reader.read("s3://my_bucket/csv_data/my_table.csv", chunksize=10000)
+writer.write(df_iter, "s3://my_bucket/parquet_data/my_table.parquet")
+```
+
+If the dataframe needs transforming before writing then use a generator.
+
+```python
+from arrow_pd_parser import reader, writer
+
+def transform(df):
+    # do something
+    return df
 
+df_iter = reader.read("s3://my_bucket/csv_data/my_table.csv", chunksize="500MB")
+# Using a generator comprehension
+df_transformed_iter = (transform(df) for df in df_iter)
+writer.write(df_transformed_iter, "s3://my_bucket/parquet_data/my_transformed_table.parquet")
+```
 
-setup(**setup_kwargs)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

