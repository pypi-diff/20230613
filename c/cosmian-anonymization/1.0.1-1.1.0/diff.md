# Comparing `tmp/cosmian_anonymization-1.0.1-py3-none-any.whl.zip` & `tmp/cosmian_anonymization-1.1.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 19952 bytes, number of entries: 11
+Zip file size: 20328 bytes, number of entries: 11
 -rw-r--r--  2.0 unx      169 b- defN 80-Jan-01 00:00 cosmian_anonymization/__init__.py
--rw-r--r--  2.0 unx     7352 b- defN 80-Jan-01 00:00 cosmian_anonymization/anonymize.py
--rw-r--r--  2.0 unx     1763 b- defN 80-Jan-01 00:00 cosmian_anonymization/conversion_helper.py
--rw-r--r--  2.0 unx     3495 b- defN 80-Jan-01 00:00 cosmian_anonymization/method_parser.py
+-rw-r--r--  2.0 unx     8012 b- defN 80-Jan-01 00:00 cosmian_anonymization/anonymize.py
+-rw-r--r--  2.0 unx     1954 b- defN 80-Jan-01 00:00 cosmian_anonymization/conversion_helper.py
+-rw-r--r--  2.0 unx     3628 b- defN 80-Jan-01 00:00 cosmian_anonymization/method_parser.py
 -rw-r--r--  2.0 unx     3784 b- defN 80-Jan-01 00:00 cosmian_anonymization/noise_correlation.py
 -rw-r--r--  2.0 unx     3887 b- defN 80-Jan-01 00:00 cosmian_anonymization/noise_parser.py
--rw-r--r--  2.0 unx    32275 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.0.1.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     1281 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       73 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.0.1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1030 b- defN 16-Jan-01 00:00 cosmian_anonymization-1.0.1.dist-info/RECORD
-11 files, 55197 bytes uncompressed, 18172 bytes compressed:  67.1%
+-rw-r--r--  2.0 unx    32275 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     1500 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       73 b- defN 80-Jan-01 00:00 cosmian_anonymization-1.1.0.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1030 b- defN 16-Jan-01 00:00 cosmian_anonymization-1.1.0.dist-info/RECORD
+11 files, 56400 bytes uncompressed, 18548 bytes compressed:  67.1%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: cosmian_anonymization/noise_correlation.py
 Comment: 
 
 Filename: cosmian_anonymization/noise_parser.py
 Comment: 
 
-Filename: cosmian_anonymization-1.0.1.dist-info/LICENSE.md
+Filename: cosmian_anonymization-1.1.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: cosmian_anonymization-1.0.1.dist-info/METADATA
+Filename: cosmian_anonymization-1.1.0.dist-info/METADATA
 Comment: 
 
-Filename: cosmian_anonymization-1.0.1.dist-info/WHEEL
+Filename: cosmian_anonymization-1.1.0.dist-info/WHEEL
 Comment: 
 
-Filename: cosmian_anonymization-1.0.1.dist-info/entry_points.txt
+Filename: cosmian_anonymization-1.1.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: cosmian_anonymization-1.0.1.dist-info/RECORD
+Filename: cosmian_anonymization-1.1.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cosmian_anonymization/anonymize.py

```diff
@@ -1,12 +1,13 @@
 # -*- coding: utf-8 -*-
 import argparse
 import json
-from typing import Dict, Optional
+from typing import Any, Dict, List, Optional
 
+import numpy as np
 import pandas as pd
 from humps import decamelize
 
 from .conversion_helper import convert_config_types
 from .method_parser import create_transformation_function
 from .noise_correlation import NoiseCorrelationTask, parse_noise_correlation_config
 
@@ -81,29 +82,49 @@
 
     if "correlation" in method_options:
         # Correlation is done later in a dedicated function: `apply_correlation_columns`
         return values
 
     # Create a transformation function based on the selected technique.
     transform_func = create_transformation_function(method, method_options)
-    return values.map(transform_func)
 
+    result: List[Any] = []
+    # Apply anonymization to each element
+    for i, val in enumerate(values):
+        try:
+            result.append(transform_func(val))
+        except Exception as e:
+            raise ValueError(f"Error processing `{values.name}` at line {i + 1}:\n{e}")
 
-def apply_correlation_columns(values: pd.Series, task: NoiseCorrelationTask):
+    return result
+
+
+def apply_correlation_columns(values: np.ndarray, task: NoiseCorrelationTask):
     """Apply noise correlation to specified columns in a DataFrame.
 
     Args:
-        values (pd.Series): The values to apply noise correlation to.
+        values (np.ndarray): The values to apply noise correlation to, in the shape (lines, columns).
         task (NoiseCorrelationTask): The task containing column names and transformation function.
 
     Returns:
         pd.DataFrame: The columns with noise correlation applied.
     """
     transform_func = task.generate_transformation()
-    return values.apply(transform_func, axis=1, raw=True)
+
+    result: List[Any] = []
+    # Apply correlated anonymization to both columns line by line
+    for i, line_values in enumerate(values):
+        try:
+            result.append(transform_func(line_values))
+        except Exception as e:
+            raise ValueError(
+                f"Error processing `{task.column_names}` at line {i + 1}:\n{e}"
+            )
+
+    return result
 
 
 def anonymize_dataframe(
     df: pd.DataFrame, config: Dict, inplace: bool = False
 ) -> pd.DataFrame:
     """
     Anonymizes a Pandas DataFrame by applying the specified techniques to selected columns.
@@ -132,15 +153,15 @@
 
     # -- Noise correlation --
     # Read through the config to find all correlation tasks
     noise_corr_tasks = parse_noise_correlation_config(config)
     # Apply correlation on each groups
     for task in noise_corr_tasks.values():
         output_df[task.column_names] = apply_correlation_columns(
-            output_df[task.column_names], task
+            output_df[task.column_names].values, task
         )
 
     # Return the anonymized data
     return output_df
 
 
 def anonymize_from_files(data_path: str, config_path: str, output_path: str) -> None:
```

## cosmian_anonymization/conversion_helper.py

```diff
@@ -37,21 +37,27 @@
     """
     if type not in CONFIG_TYPES_MAPPING:
         raise ValueError(f"Invalid type in config file: {type}.")
 
     target_type = CONFIG_TYPES_MAPPING[type]
 
     # Convert the series to the target type if it's different from the current type
-    converted_values = (
-        values.astype(target_type) if values.dtype != target_type else values
-    )
-
-    if type == "Date":
-        # Convert the series values to RFC3339 format
-        converted_values = converted_values.map(date_to_rfc3339)
+    try:
+        converted_values = (
+            values.astype(target_type) if values.dtype != target_type else values
+        )
+
+        if type == "Date":
+            # Convert the series values to RFC3339 format
+            converted_values = converted_values.map(date_to_rfc3339)
+
+    except Exception:
+        raise ValueError(
+            f"The column `{values.name}` contains elements that could not be converted to {type}."
+        )
 
     return converted_values
 
 
 def date_to_rfc3339(date_str: str) -> str:
     """
     Converts a date string to ISO format with timezone (RFC 3339).
```

## cosmian_anonymization/method_parser.py

```diff
@@ -1,14 +1,16 @@
 # -*- coding: utf-8 -*-
 import os
 from typing import Callable, Dict, Optional
 
+from cloudproof_py.anonymization import DateAggregator
+from cloudproof_py.anonymization import (
+    Hasher as AnoHasher,  # Avoid builtin.Hasher name override
+)
 from cloudproof_py.anonymization import (
-    DateAggregator,
-    Hasher,
     NumberAggregator,
     NumberScaler,
     WordMasker,
     WordPatternMasker,
     WordTokenizer,
 )
 from cloudproof_py.fpe import Alphabet, Float, Integer
@@ -56,15 +58,15 @@
         hash_type (str): The name of the hash function to use.
         salt_value (Optional[str]): An optional salt to use for hashing.
         encoding (str): The encoding to use when converting the input string to bytes.
     """
     salt = None
     if salt_value:
         salt = salt_value.encode(encoding)
-    hasher = Hasher(hash_type, salt)
+    hasher = AnoHasher(hash_type, salt)
 
     return lambda val: hasher.apply_str(val)
 
 
 def create_transformation_function(method_name: str, method_opts: Dict) -> Callable:
     """
     Given a method name and options, returns a callable that applies the desired transformation.
```

## Comparing `cosmian_anonymization-1.0.1.dist-info/LICENSE.md` & `cosmian_anonymization-1.1.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

