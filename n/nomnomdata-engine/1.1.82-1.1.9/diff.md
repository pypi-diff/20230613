# Comparing `tmp/nomnomdata_engine-1.1.82.tar.gz` & `tmp/nomnomdata-engine-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomnomdata_engine-1.1.82.tar", max compression
+gzip compressed data, was "nomnomdata-engine-1.1.9.tar", max compression
```

## Comparing `nomnomdata_engine-1.1.82.tar` & `nomnomdata-engine-1.1.9.tar`

### file list

```diff
@@ -1,17 +1,18 @@
--rw-r--r--   0        0        0      702 2023-06-13 17:11:13.468442 nomnomdata_engine-1.1.82/LICENSE
--rw-r--r--   0        0        0       37 2023-06-13 17:11:13.468442 nomnomdata_engine-1.1.82/README.md
--rw-r--r--   0        0        0      432 2023-06-13 17:11:13.468442 nomnomdata_engine-1.1.82/nomnomdata/engine/__init__.py
--rw-r--r--   0        0        0    10061 2023-06-13 17:11:13.468442 nomnomdata_engine-1.1.82/nomnomdata/engine/components.py
--rw-r--r--   0        0        0    72019 2023-06-13 17:11:13.468442 nomnomdata_engine-1.1.82/nomnomdata/engine/connections.py
--rw-r--r--   0        0        0     5598 2023-06-13 17:11:13.469442 nomnomdata_engine-1.1.82/nomnomdata/engine/encoders.py
--rw-r--r--   0        0        0    14368 2023-06-13 17:11:13.469442 nomnomdata_engine-1.1.82/nomnomdata/engine/engine.py
--rw-r--r--   0        0        0      516 2023-06-13 17:11:13.469442 nomnomdata_engine-1.1.82/nomnomdata/engine/errors.py
--rw-r--r--   0        0        0      290 2023-06-13 17:11:13.469442 nomnomdata_engine-1.1.82/nomnomdata/engine/globals.py
--rw-r--r--   0        0        0     2448 2023-06-13 17:11:13.469442 nomnomdata_engine-1.1.82/nomnomdata/engine/logging.py
--rw-r--r--   0        0        0    11023 2023-06-13 17:11:13.469442 nomnomdata_engine-1.1.82/nomnomdata/engine/nominode.py
--rw-r--r--   0        0        0     9574 2023-06-13 17:11:13.469442 nomnomdata_engine-1.1.82/nomnomdata/engine/parameters.py
--rw-r--r--   0        0        0    29217 2023-06-13 17:11:13.469442 nomnomdata_engine-1.1.82/nomnomdata/engine/shared_configs.py
--rw-r--r--   0        0        0     4357 2023-06-13 17:11:13.469442 nomnomdata_engine-1.1.82/nomnomdata/engine/testing.py
--rw-r--r--   0        0        0      162 2023-06-13 17:11:13.470441 nomnomdata_engine-1.1.82/nomnomdata/engine/util.py
--rw-r--r--   0        0        0     1291 2023-06-13 17:11:26.200241 nomnomdata_engine-1.1.82/pyproject.toml
--rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 nomnomdata_engine-1.1.82/PKG-INFO
+-rw-r--r--   0        0        0      702 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/LICENSE
+-rw-r--r--   0        0        0       40 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/README.md
+-rw-r--r--   0        0        0      432 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/__init__.py
+-rw-r--r--   0        0        0     9869 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/components.py
+-rw-r--r--   0        0        0    30556 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/connections.py
+-rw-r--r--   0        0        0     5426 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/encoders.py
+-rw-r--r--   0        0        0    14368 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/engine.py
+-rw-r--r--   0        0        0      516 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/errors.py
+-rw-r--r--   0        0        0      290 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/globals.py
+-rw-r--r--   0        0        0     2448 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/logging.py
+-rw-r--r--   0        0        0    11023 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/nominode.py
+-rw-r--r--   0        0        0     9574 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/parameters.py
+-rw-r--r--   0        0        0    15475 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/shared_configs.py
+-rw-r--r--   0        0        0     4357 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/testing.py
+-rw-r--r--   0        0        0      162 2021-03-23 15:35:19.464848 nomnomdata-engine-1.1.9/nomnomdata/engine/util.py
+-rw-r--r--   0        0        0     1269 2021-03-23 15:35:41.196843 nomnomdata-engine-1.1.9/pyproject.toml
+-rw-r--r--   0        0        0      907 2021-03-23 15:35:42.349421 nomnomdata-engine-1.1.9/setup.py
+-rw-r--r--   0        0        0      995 2021-03-23 15:35:42.349753 nomnomdata-engine-1.1.9/PKG-INFO
```

### Comparing `nomnomdata_engine-1.1.82/LICENSE` & `nomnomdata-engine-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.82/nomnomdata/engine/components.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/components.py`

 * *Files 5% similar despite different names*

```diff
@@ -31,20 +31,14 @@
     def dump(self, val):
         return val
 
     def load(self, val):
         return val
 
 
-class Rule:
-    def __init__(self, name: str = "", value: List[str] = [""]):
-        self.name = name
-        self.value = value
-
-
 class Parameter:
     """
     Parameter for use in a ParameterGroup, also contains options
     to control the look in the Nominode UI
 
     :param type:
         Set the type to allow validation of the parameter and
@@ -80,15 +74,14 @@
         help_header_id: str = None,
         help_md_path: str = None,
         required: bool = False,
         description: str = "",
         default: object = None,
         many: bool = False,
         categories: List[str] = None,
-        show_on: Rule = None,
     ):
         if (
             not isinstance(type, ParameterType)
             and type is not None
             and issubclass(type, ParameterType)
         ):
             raise ValueError(f"{type} is not an instance, perhaps a forgotten ()?")
@@ -114,15 +107,14 @@
         self.required = required
         self.description = description
         if default:
             type.validate(default)
         self.default = default
         self.many = many
         self.categories = [{"name": val} for val in categories] if categories else None
-        self.show_on = show_on
 
     def validate(self, value: Any):
         self._verify_required(value)
         if self.many and value is not None:
             for v in value:
                 self._validate(v)
         else:
```

### Comparing `nomnomdata_engine-1.1.82/nomnomdata/engine/encoders.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/encoders.py`

 * *Files 2% similar despite different names*

```diff
@@ -115,19 +115,14 @@
             result["help"] = p.help
         if p.default:
             result["default"] = p.type.dump(p.default)
         if p.many:
             result["many"] = p.many
         if p.categories:
             result["categories"] = p.categories
-        if p.show_on:
-            result["show_on"] = {
-                "parameter_name": p.show_on.name,
-                "parameter_value": p.show_on.value,
-            }
         if isinstance(p.type, Connection):
             result.update(self.serialize_connection_parameter(p.type))
         elif isinstance(p.type, SharedConfig):
             result.update(self.serialize_shared_config_parameter(p.type))
         else:
             result.update(self.serialize_parameter_type(p.type))
         return result
```

### Comparing `nomnomdata_engine-1.1.82/nomnomdata/engine/engine.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/engine.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.82/nomnomdata/engine/errors.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/errors.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.82/nomnomdata/engine/logging.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/logging.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.82/nomnomdata/engine/nominode.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/nominode.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.82/nomnomdata/engine/parameters.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.82/nomnomdata/engine/shared_configs.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/shared_configs.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,141 +1,9 @@
 from nomnomdata.engine.components import Parameter, ParameterGroup, SharedConfig
-from nomnomdata.engine.parameters import Boolean, Code, Enum, Int, Nested, String
-
-DOSpace = SharedConfig(
-    shared_config_type_uuid="DOSPC-NND3C",
-    description="DigitalOcean Space configuration parameters.",
-    alias="DigitalOcean Space",
-    categories=["DigitalOcean", "Spaces"],
-    parameter_groups=[
-        ParameterGroup(
-            Parameter(
-                name="space",
-                display_name="Space Name",
-                description="Specify the name of the Space.",
-                type=String(),
-                required=True,
-            ),
-            Parameter(
-                name="region",
-                display_name="Region",
-                description="Specify the region where the Space exists.",
-                type=String(),
-                required=True,
-            ),
-            Parameter(
-                name="path_prefix",
-                display_name="Path Prefix",
-                description="Optional. Specify a path that will be prepended to the path specified in a Task to form the full path where files will be stored within the Space.",
-                required=False,
-                type=String(),
-            ),
-            Parameter(
-                name="temp_path",
-                display_name="Temp Path",
-                description="Optional. Specify a full path within the Space where temporary files can be written.",
-                required=False,
-                type=String(),
-            ),
-            name="do_space_parameters",
-            display_name="Space Parameters",
-            description="",
-        ),
-    ],
-)
-
-FileFormat = SharedConfig(
-    shared_config_type_uuid="FFILE-FMTSC",
-    description="Flat file format configuration parameters.",
-    alias="File Format",
-    categories=["CSV", "Delimited", "JSON"],
-    parameter_groups=[
-        ParameterGroup(
-            Parameter(
-                name="file_name",
-                display_name="File Name",
-                description="Specify the non-dynamic portion of the file name.",
-                type=String(),
-                required=False,
-            ),
-            Parameter(
-                name="allow_overwrite",
-                display_name="Allow Overwrite",
-                description="Specify whether or not existing files should be overwritten.",
-                required=False,
-                type=Boolean(),
-                default=False,
-            ),
-            Parameter(
-                name="compression",
-                display_name="Compression Format",
-                description="Select the compression, if any, applied to the files.",
-                type=Enum(choices=["None", "gzip", "zip", "bzip2"]),
-                required=False,
-                default="None",
-            ),
-            Parameter(
-                name="format_type",
-                display_name="Data Format",
-                description="Select the format of the data in the files.",
-                type=Enum(choices=["JSON", "Delimited"]),
-                required=False,
-                default="JSON",
-            ),
-            Parameter(
-                name="add_quotes",
-                display_name="Add Quotes",
-                description="Specify whether or not string data values should be enclosed in files with delimited data format.",
-                required=False,
-                type=Boolean(),
-                default=False,
-            ),
-            Parameter(
-                name="quote_char",
-                display_name="Quote Character",
-                description="Specify the character used enclose string data values in files with delimited data format, if Add Quotes is enabled.",
-                type=String(),
-                required=False,
-            ),
-            Parameter(
-                name="delimiter_char",
-                display_name="Delimiter",
-                description="Specify the character used to separate data values in files with delimited data format.",
-                type=String(),
-                required=False,
-            ),
-            Parameter(
-                name="escape_char",
-                display_name="Escape Character",
-                description="Specify the character used to represent an escaped value in files with delimited data format.",
-                type=String(),
-                required=False,
-            ),
-            Parameter(
-                name="null_value",
-                display_name="Null Value",
-                description="Specify the characters used to represent a null value in files with delimited data format.",
-                type=String(),
-                required=False,
-            ),
-            Parameter(
-                name="append_date",
-                display_name="Append Date",
-                description="Enable to append the creation date to the file name.",
-                type=Boolean(),
-                required=False,
-                default=False,
-                help_header_id="Append Date",
-            ),
-            name="file_format_parameters",
-            display_name="File Format Parameters",
-            description="",
-        ),
-    ],
-)
+from nomnomdata.engine.parameters import Code, Enum, Int, Nested, String
 
 FirebaseToDatabase = SharedConfig(
     shared_config_type_uuid="FB2DB-NND3C",
     description="Firebase collection to a relational database table configuration parameters.",
     alias="Firebase to Relational Database",
     categories=[
         "Firebase",
@@ -264,55 +132,14 @@
             name="additional_parameters",
             display_name="Additional Parameters",
             description="Any additional parameters not described above.",
         ),
     ],
 )
 
-S3Bucket = SharedConfig(
-    shared_config_type_uuid="S3BKT-NND3C",
-    description="AWS S3 Bucket configuration parameters.",
-    alias="S3 Bucket",
-    categories=["Amazon", "AWS", "S3"],
-    parameter_groups=[
-        ParameterGroup(
-            Parameter(
-                name="bucket",
-                display_name="Bucket Name",
-                description="Specify the name of the S3 Bucket.",
-                type=String(),
-                required=True,
-            ),
-            Parameter(
-                name="region",
-                display_name="Region",
-                description="Optional. Specify the region where the Bucket exists.",
-                type=String(),
-                required=False,
-            ),
-            Parameter(
-                name="path_prefix",
-                display_name="Path Prefix",
-                description="Optional. Specify a path that will be prepended to the path specified in a Task to form the full path where files will be stored within the Bucket.",
-                required=False,
-                type=String(),
-            ),
-            Parameter(
-                name="temp_path",
-                display_name="Temp Path",
-                description="Optional. Specify a full path within the Bucket where temporary files can be written.",
-                required=False,
-                type=String(),
-            ),
-            name="s3_bucket_parameters",
-            display_name="Bucket Parameters",
-            description="",
-        ),
-    ],
-)
 
 S3FileToDatabase = SharedConfig(
     shared_config_type_uuid="S3BTK-DB3MD",
     alias="S3 to Relational Database Load Options",
     description="Information needed when loading data from files stored on S3 into a relational database.",
     categories=[
         "S3",
@@ -345,35 +172,26 @@
             Parameter(
                 name="s3_temp_space",
                 display_name="Temporary File Storage Path",
                 description="Specify the path within the S3 bucket where manifest files can be created.  If blank, nnd_tmp will be used.",
                 type=String(max=2048),
                 required=False,
             ),
-            Parameter(
-                name="region",
-                display_name="Region",
-                description="Optional. Specify the region where the Bucket exists.",
-                type=String(),
-                required=False,
-            ),
             name="s3_parameters",
             display_name="S3 Parameters",
             description="Information about the S3 location where the files reside.",
         ),
         ParameterGroup(
             Parameter(
                 name="load_pattern",
                 display_name="Load Pattern",
                 description="Select which pattern to use when loading the data from the files.",
                 type=Enum(
                     choices=[
                         "INSERT",
-                        "DELETE_ALL_INSERT_ALL",
-                        "DELETE_ALL_INSERT_LAST",
                         "DELETE_INSERT",
                         "DELETE_INSERT_BATCH",
                         "DROP_AND_RECREATE",
                         "INSERT_IF_NOT_EXISTS",
                         "TRUNCATE_LOAD_ALL",
                         "TRUNCATE_LOAD_LAST",
                         "UPDATE_INSERT",
@@ -382,29 +200,29 @@
                 ),
                 default="INSERT",
             ),
             Parameter(
                 name="file_type",
                 display_name="Data Format",
                 description="Select the format of the data in the files.",
-                type=Enum(choices=["JSON", "Delimited", "PARQUET"]),
+                type=Enum(choices=["JSON", "Delimited"]),
                 default="JSON",
             ),
             Parameter(
                 name="compression",
                 display_name="Compression Format",
                 description="Select the compression, if any, applied to the files.",
-                type=Enum(choices=["None", "gzip", "zip", "bzip2"]),
+                type=Enum(choices=["None", "gzip", "zip", "bzip"]),
                 default="None",
             ),
             Parameter(
                 name="delimiter",
                 display_name="Delimiter",
                 description="Specify the character used to separate data values in files with delimited data format.",
-                type=String(max=5),
+                type=String(max=2),
                 required=False,
             ),
             Parameter(
                 name="null_value",
                 display_name="Null Value",
                 description="Specify the characters used to represent a null value in files with delimited data format.",
                 type=String(max=8),
@@ -417,15 +235,15 @@
                 type=String(max=2),
                 required=False,
             ),
             Parameter(
                 name="header_rows",
                 display_name="Header Rows",
                 description="Specify the number of lines to skip before the first row of data in files with delimited data format.",
-                type=Int(),
+                type=Int,
                 required=False,
             ),
             name="load_parameters",
             display_name="Load Parameters",
             description="Options describing how the data from the files should be loaded.",
         ),
         ParameterGroup(
@@ -454,32 +272,26 @@
                 name="merge_key",
                 display_name="Merge Keys",
                 description="Optional. Specify one or more column names, with commas between each name, whose combined values will be used to identify rows of data that will be merged together.",
                 type=String(max=2048),
                 required=False,
             ),
             Parameter(
-                name="upsert_sort_key",
-                display_name="Upsert Sort Keys",
-                description="Optional. Specify one or more column names, with commas between each name, whose combined values will be used to set the order priority of rows of data that will be merged together.",
-                type=String(max=2048),
-                required=False,
-            ),
-            Parameter(
                 name="merge_type",
                 display_name="Merge Strategy",
                 description="If column names are specified in the Merge Keys field, then rows with matching merge key values will be combined according to the strategy selected.",
                 type=Enum(choices=["DISTINCT", "LOAD_ALL"]),
                 default="DISTINCT",
                 required=False,
             ),
             name="key_parameters",
             display_name="Key Parameters",
             description="Columns used to partition, sort, identify and merge data.",
         ),
+        # MANY TYPES ARE NOT PART OF PARAMETER GROUPS FOR SHARED OBJECTS
         Parameter(
             name="column_parameters",
             display_name="Column Parameters",
             description="Details about each column within the relational database.",
             required=True,
             many=True,
             type=Nested(
@@ -541,177 +353,7 @@
             ),
             name="additional_parameters",
             display_name="Additional Parameters",
             description="",
         ),
     ],
 )
-
-
-SQLToBigQueryParameters = SharedConfig(
-    shared_config_type_uuid="SQLRW-BIGQRY",
-    alias="SQL to BigQuery Load Options",
-    description="Information needed when loading data from an SQL table into a BigQuery table.",
-    categories=["Google", "BigQuery", "SQL"],
-    parameter_groups=[
-        ParameterGroup(
-            Parameter(
-                name="strategy",
-                display_name="Load Pattern",
-                description="Select which pattern to use when loading the data.",
-                type=Enum(choices=["Append", "Overwrite", "Upsert"]),
-                required=False,
-                default="Append",
-                help_header_id="Load Pattern",
-            ),
-            Parameter(
-                name="upsert_column",
-                display_name="Merge Keys",
-                description="Optional. Specify one or more column names, with commas between each name, whose combined values will be used to identify rows of data that will be merged together.",
-                type=String(),
-                required=False,
-                help_header_id="Merge Keys",
-            ),
-            Parameter(
-                name="fields_mapping_autodetect",
-                display_name="Autodetect Column Mappings",
-                description="Automatically create the BigQuery table description.",
-                type=Boolean(),
-                required=False,
-                default=True,
-                help_header_id="Autodetect Column Mappings",
-            ),
-            Parameter(
-                name="add_default_fields",
-                display_name="Add Nom Nom Data Columns",
-                description="Add the nnd_updated and nnd_created columns to the BigQuery table.",
-                type=Boolean(),
-                required=False,
-                default=True,
-                help_header_id="Add Nom Nom Data Columns",
-            ),
-            Parameter(
-                name="column_parameters",
-                display_name="Column Parameters",
-                description="Details about each column within the tables.",
-                required=True,
-                many=True,
-                type=Nested(
-                    Parameter(
-                        name="sql_row",
-                        display_name="SQL Column Name",
-                        description="Specify the name of the column.",
-                        type=String(max=128),
-                        required=True,
-                    ),
-                    Parameter(
-                        name="bigquery_row",
-                        display_name="BigQuery Column Name",
-                        description="Specify the name of the column.",
-                        type=String(max=128),
-                        required=True,
-                    ),
-                    Parameter(
-                        name="bigquery_row_type",
-                        display_name="BigQuery Column Type",
-                        description="Specify the type of the column.",
-                        type=Enum(
-                            choices=[
-                                "STRING",
-                                "BIGNUMERIC",
-                                "BOOL",
-                                "BYTES",
-                                "DATE",
-                                "DATETIME",
-                                "FLOAT64",
-                                "GEOGRAPHY",
-                                "INT64",
-                                "JSON",
-                                "NUMERIC",
-                                "STRING",
-                                "TIME",
-                                "TIMESTAMP",
-                            ]
-                        ),
-                        required=True,
-                    ),
-                ),
-            ),
-        ),
-    ],
-)
-
-
-VultrObjectStore = SharedConfig(
-    shared_config_type_uuid="VULTR-OBJSR",
-    description="Vultr Object Storage Bucket configuration parameters.",
-    alias="Vultr Object Storage Bucket",
-    categories=["Vultr", "Object Storage"],
-    parameter_groups=[
-        ParameterGroup(
-            Parameter(
-                name="bucket",
-                display_name="Bucket Name",
-                description="Specify the name of the Bucket.",
-                type=String(),
-                required=True,
-            ),
-            Parameter(
-                name="region",
-                display_name="Region",
-                description="Specify the region where the Bucket exists.",
-                type=Enum(choices=["ewr1"]),
-                default="ewr1",
-                required=True,
-            ),
-            Parameter(
-                name="path_prefix",
-                display_name="Path Prefix",
-                description="Optional. Specify a path that will be prepended to the path specified in a Task to form the full path where files will be stored within the Bucket.",
-                required=False,
-                type=String(),
-            ),
-            Parameter(
-                name="temp_path",
-                display_name="Temp Path",
-                description="Optional. Specify a full path within the Bucket where temporary files can be written.",
-                required=False,
-                type=String(),
-            ),
-            name="vultr_object_storage_parameters",
-            display_name="Vultr Object Storage Parameters",
-            description="",
-        ),
-    ],
-)
-
-KeyValue = SharedConfig(
-    shared_config_type_uuid="GENRIC-KEYVAL",
-    alias="Key and Value Pairs",
-    description="One or more sets of key and value string pairs.",
-    categories=[],
-    parameter_groups=[
-        Parameter(
-            name="key_values",
-            display_name="Pairs",
-            description="",
-            required=True,
-            many=True,
-            type=Nested(
-                Parameter(
-                    name="key",
-                    display_name="Key",
-                    description="Specify a key name.",
-                    type=String(),
-                    required=True,
-                ),
-                Parameter(
-                    name="value",
-                    display_name="Value",
-                    description="Specify the value that corresponds to the key specified.",
-                    type=String(),
-                    required=True,
-                ),
-            ),
-        ),
-    ],
-)
```

### Comparing `nomnomdata_engine-1.1.82/nomnomdata/engine/testing.py` & `nomnomdata-engine-1.1.9/nomnomdata/engine/testing.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.82/pyproject.toml` & `nomnomdata-engine-1.1.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -4,25 +4,24 @@
 license = "LGPL-3.0-only"
 name = "nomnomdata-engine"
 packages = [
   {include = "nomnomdata"},
 ]
 readme = "README.md"
 repository = "https://gitlab.com/nomnomdata/tools/nomnomdata-engine"
-version = "1.1.82"
+version = "1.1.9"
 
 [tool.poetry.dependencies]
 dunamai = "^1.1.0"
 httmock = "^1.3.0"
 nomnomdata-cli = "^0.1.7"
 python = "^3.7"
 pyyaml = "^5.3.1"
 requests = "^2.23.0"
 wrapt = "^1.12.1"
-MarkupSafe = "2.0.1"
 
 [tool.poetry.dev-dependencies]
 genson = "^1.2.1"
 pytest = "^6.0.1"
 pytest-cov = "^2.10.0"
 pytest-snapshot = "^0.4.2"
```

### Comparing `nomnomdata_engine-1.1.82/PKG-INFO` & `nomnomdata-engine-1.1.9/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 Metadata-Version: 2.1
 Name: nomnomdata-engine
-Version: 1.1.82
+Version: 1.1.9
 Summary: Package containing tooling for developing nominode engines
 Home-page: https://gitlab.com/nomnomdata/tools/nomnomdata-engine
 License: LGPL-3.0-only
 Author: Nom Nom Data Inc
 Author-email: info@nomnomdata.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: MarkupSafe (==2.0.1)
 Requires-Dist: dunamai (>=1.1.0,<2.0.0)
 Requires-Dist: httmock (>=1.3.0,<2.0.0)
 Requires-Dist: nomnomdata-cli (>=0.1.7,<0.2.0)
 Requires-Dist: pyyaml (>=5.3.1,<6.0.0)
 Requires-Dist: requests (>=2.23.0,<3.0.0)
 Requires-Dist: wrapt (>=1.12.1,<2.0.0)
 Project-URL: Repository, https://gitlab.com/nomnomdata/tools/nomnomdata-engine
 Description-Content-Type: text/markdown
 
-Package for developing Nominode apps
+Package for developing nominode engines
```

