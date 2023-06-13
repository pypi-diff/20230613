# Comparing `tmp/schema_enforcer-1.2.0.tar.gz` & `tmp/schema_enforcer-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schema_enforcer-1.2.0.tar", max compression
+gzip compressed data, was "schema_enforcer-1.2.1.tar", max compression
```

## Comparing `schema_enforcer-1.2.0.tar` & `schema_enforcer-1.2.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0     2303 2023-06-06 15:46:54.991255 schema_enforcer-1.2.0/CHANGELOG.md
--rw-r--r--   0        0        0      602 2023-06-06 15:46:54.991255 schema_enforcer-1.2.0/LICENSE
--rwxr-xr-x   0        0        0    10213 2023-06-06 15:46:54.991255 schema_enforcer-1.2.0/README.md
--rwxr-xr-x   0        0        0     2125 2023-06-06 15:47:05.143261 schema_enforcer-1.2.0/pyproject.toml
--rw-r--r--   0        0        0       86 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/__init__.py
--rw-r--r--   0        0        0    10605 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/ansible_inventory.py
--rw-r--r--   0        0        0    12629 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/cli.py
--rw-r--r--   0        0        0     4038 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/config.py
--rw-r--r--   0        0        0     1384 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/exceptions.py
--rw-r--r--   0        0        0     6980 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/instances/file.py
--rw-r--r--   0        0        0     6183 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/schemas/jsonschema.py
--rw-r--r--   0        0        0    13446 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/schemas/manager.py
--rw-r--r--   0        0        0     4022 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/schemas/validator.py
--rwxr-xr-x   0        0        0    18375 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/utils.py
--rw-r--r--   0        0        0     2608 2023-06-06 15:46:54.995255 schema_enforcer-1.2.0/schema_enforcer/validation.py
--rw-r--r--   0        0        0    11611 1970-01-01 00:00:00.000000 schema_enforcer-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     2374 2023-06-13 15:24:24.105442 schema_enforcer-1.2.1/CHANGELOG.md
+-rw-r--r--   0        0        0      602 2023-06-13 15:24:24.109443 schema_enforcer-1.2.1/LICENSE
+-rwxr-xr-x   0        0        0    10213 2023-06-13 15:24:24.109443 schema_enforcer-1.2.1/README.md
+-rwxr-xr-x   0        0        0     2126 2023-06-13 15:24:36.510090 schema_enforcer-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0       86 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/__init__.py
+-rw-r--r--   0        0        0    10605 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/ansible_inventory.py
+-rw-r--r--   0        0        0    12628 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/cli.py
+-rw-r--r--   0        0        0     4038 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/config.py
+-rw-r--r--   0        0        0     1384 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/exceptions.py
+-rw-r--r--   0        0        0     6980 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/instances/file.py
+-rw-r--r--   0        0        0     6181 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/schemas/jsonschema.py
+-rw-r--r--   0        0        0    13444 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/schemas/manager.py
+-rw-r--r--   0        0        0     4022 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/schemas/validator.py
+-rwxr-xr-x   0        0        0    18373 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/utils.py
+-rw-r--r--   0        0        0     2608 2023-06-13 15:24:24.113443 schema_enforcer-1.2.1/schema_enforcer/validation.py
+-rw-r--r--   0        0        0    11605 1970-01-01 00:00:00.000000 schema_enforcer-1.2.1/PKG-INFO
```

### Comparing `schema_enforcer-1.2.0/CHANGELOG.md` & `schema_enforcer-1.2.1/CHANGELOG.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # Changelog
 
+## v1.2.1
+
+### Changes
+
+- #152 Update requirement for rich to ^12.5.1
+
 ## v1.2.0 - 2023-06-05
 
 ### Adds
 
 - Support for versions of jsonschema >= 4.6
 
 ### Removes
```

### Comparing `schema_enforcer-1.2.0/LICENSE` & `schema_enforcer-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.0/README.md` & `schema_enforcer-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.0/pyproject.toml` & `schema_enforcer-1.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "schema-enforcer"
-version = "v1.2.0"
+version = "v1.2.1"
 description = "Tool/Framework for testing structured data against schema definitions"
 authors = ["Network to Code, LLC <info@networktocode.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/networktocode/schema-enforcer"
 repository = "https://github.com/networktocode/schema-enforcer"
 include = [
@@ -18,15 +18,15 @@
 click = "^7.1 || ^8.0"
 termcolor = "^1.1"
 toml = "^0.10"
 "ruamel.yaml" = "^0.16 || ^0.17"
 jinja2 = ">=2.11"
 jsonref = "^0.2"
 pydantic = "^1.6"
-rich = "^9.5"
+rich = ">=9.5"
 jsonpointer = "^2.1"
 jmespath = "^0.10"
 ansible = { version = "^2.10.0", optional = true }
 ansible-base = { version = "^2.10.0", optional = true }
 jsonschema = {version = "^4.6", extras = ["format-nongpl"]}
 
 [tool.poetry.extras]
```

### Comparing `schema_enforcer-1.2.0/schema_enforcer/ansible_inventory.py` & `schema_enforcer-1.2.1/schema_enforcer/ansible_inventory.py`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.0/schema_enforcer/cli.py` & `schema_enforcer-1.2.1/schema_enforcer/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,15 +79,14 @@
     if show_checks:
         ifm.print_schema_mapping()
         sys.exit(0)
 
     error_exists = False
     for instance in ifm.instances:
         for result in instance.validate(smgr, strict):
-
             result.instance_type = "FILE"
             result.instance_name = instance.filename
             result.instance_location = instance.path
 
             if not result.passed():
                 error_exists = True
                 result.print()
```

### Comparing `schema_enforcer-1.2.0/schema_enforcer/config.py` & `schema_enforcer-1.2.1/schema_enforcer/config.py`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.0/schema_enforcer/exceptions.py` & `schema_enforcer-1.2.1/schema_enforcer/exceptions.py`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.0/schema_enforcer/instances/file.py` & `schema_enforcer-1.2.1/schema_enforcer/instances/file.py`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.0/schema_enforcer/schemas/jsonschema.py` & `schema_enforcer-1.2.1/schema_enforcer/schemas/jsonschema.py`

 * *Files 0% similar despite different names*

```diff
@@ -52,15 +52,14 @@
         if strict:
             validator = self.__get_strict_validator()
         else:
             validator = self.__get_validator()
 
         has_error = False
         for err in validator.iter_errors(data):
-
             has_error = True
             self.add_validation_error(err.message, absolute_path=list(err.absolute_path))
 
         if not has_error:
             self.add_validation_pass()
         return self.get_results()
 
@@ -133,15 +132,14 @@
             List[ValidationResult]: A list of validation result objects.
         """
         validator = Draft7Validator(v7schema, format_checker=self.format_checker)
 
         results = []
         has_error = False
         for err in validator.iter_errors(self.data):
-
             has_error = True
 
             results.append(
                 ValidationResult(
                     schema_id=self.id,
                     result=RESULT_FAIL,
                     message=err.message,
```

### Comparing `schema_enforcer-1.2.0/schema_enforcer/schemas/manager.py` & `schema_enforcer-1.2.1/schema_enforcer/schemas/manager.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,14 @@
           - schema must be Draft7 valid.
           - Valid tests must pass.
           - Invalid tests must pass.
         """
         error_exists = False
 
         for schema_id, schema in self.iter_schemas():
-
             schema_valid = schema.check_if_valid()
             valid_results = self.test_schema_valid(schema_id)
             invalid_results = self.test_schema_invalid(schema_id)
 
             for result in schema_valid + valid_results + invalid_results:
                 if not result.passed():
                     error_exists = True
@@ -160,15 +159,14 @@
             excluded_filenames=[],
             return_dir=True,
         )
 
         results = []
 
         for root, filename in valid_files:
-
             test_data = load_file(os.path.join(root, filename))
 
             for result in schema.validate(test_data, strict=strict):
                 result.instance_name = filename
                 result.instance_location = root
                 result.instance_type = "TEST"
                 results.append(result)
```

### Comparing `schema_enforcer-1.2.0/schema_enforcer/schemas/validator.py` & `schema_enforcer-1.2.1/schema_enforcer/schemas/validator.py`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.0/schema_enforcer/utils.py` & `schema_enforcer-1.2.1/schema_enforcer/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -343,15 +343,14 @@
             except AttributeError:
                 error(f"Failed to find python package `{search_directory}' for loading {search_directory}/schemas/")
                 continue
 
             search_directory = directory
 
         for root, dirs, files in os.walk(search_directory):  # pylint: disable=W0612
-
             if is_part_of_excluded_dirs(root):
                 continue
 
             for file in files:
                 # Extract the extension of the file and check if the extension matches the list
                 _, ext = os.path.splitext(file)
                 if ext in file_extensions:
@@ -433,15 +432,14 @@
         filename (str): Full filename of the file to search and load, without the extension.
         formats (List[str]): List of formats to search.
 
     Returns:
         dict, list or None: content of the file in a python variable. None if no file could be found.
     """
     for ext in formats:
-
         file_ext = f"{filename}.{ext}"
         if not os.path.isfile(file_ext):
             continue
 
         data = load_file(file_ext)
         return data
```

### Comparing `schema_enforcer-1.2.0/schema_enforcer/validation.py` & `schema_enforcer-1.2.1/schema_enforcer/validation.py`

 * *Files identical despite different names*

### Comparing `schema_enforcer-1.2.0/PKG-INFO` & `schema_enforcer-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schema-enforcer
-Version: 1.2.0
+Version: 1.2.1
 Summary: Tool/Framework for testing structured data against schema definitions
 Home-page: https://github.com/networktocode/schema-enforcer
 License: Apache-2.0
 Author: Network to Code, LLC
 Author-email: info@networktocode.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,15 +21,15 @@
 Requires-Dist: click (>=7.1,<9.0)
 Requires-Dist: jinja2 (>=2.11)
 Requires-Dist: jmespath (>=0.10,<0.11)
 Requires-Dist: jsonpointer (>=2.1,<3.0)
 Requires-Dist: jsonref (>=0.2,<0.3)
 Requires-Dist: jsonschema[format-nongpl] (>=4.6,<5.0)
 Requires-Dist: pydantic (>=1.6,<2.0)
-Requires-Dist: rich (>=9.5,<10.0)
+Requires-Dist: rich (>=9.5)
 Requires-Dist: ruamel.yaml (>=0.16,<0.18)
 Requires-Dist: termcolor (>=1.1,<2.0)
 Requires-Dist: toml (>=0.10,<0.11)
 Project-URL: Repository, https://github.com/networktocode/schema-enforcer
 Description-Content-Type: text/markdown
 
 # Schema Enforcer
```

