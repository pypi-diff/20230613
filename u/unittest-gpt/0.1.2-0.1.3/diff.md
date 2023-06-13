# Comparing `tmp/unittest_gpt-0.1.2.tar.gz` & `tmp/unittest_gpt-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unittest_gpt-0.1.2.tar", max compression
+gzip compressed data, was "unittest_gpt-0.1.3.tar", max compression
```

## Comparing `unittest_gpt-0.1.2.tar` & `unittest_gpt-0.1.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1075 2023-06-13 19:08:18.775053 unittest_gpt-0.1.2/LICENSE
--rw-r--r--   0        0        0     5259 2023-06-13 03:30:38.442316 unittest_gpt-0.1.2/README.md
--rw-r--r--   0        0        0      459 2023-06-13 19:17:51.108215 unittest_gpt-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1483 2023-06-13 03:30:38.443043 unittest_gpt-0.1.2/src/file_utils.py
--rw-r--r--   0        0        0     8646 2023-06-13 19:17:00.858844 unittest_gpt-0.1.2/src/unit_test_agent.py
--rw-r--r--   0        0        0     5843 1970-01-01 00:00:00.000000 unittest_gpt-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1075 2023-06-13 19:08:18.775053 unittest_gpt-0.1.3/LICENSE
+-rw-r--r--   0        0        0     5259 2023-06-13 03:30:38.442316 unittest_gpt-0.1.3/README.md
+-rw-r--r--   0        0        0      459 2023-06-13 20:06:10.137703 unittest_gpt-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1483 2023-06-13 03:30:38.443043 unittest_gpt-0.1.3/src/file_utils.py
+-rw-r--r--   0        0        0     8646 2023-06-13 20:05:49.706727 unittest_gpt-0.1.3/src/unit_test_agent.py
+-rw-r--r--   0        0        0     5843 1970-01-01 00:00:00.000000 unittest_gpt-0.1.3/PKG-INFO
```

### Comparing `unittest_gpt-0.1.2/LICENSE` & `unittest_gpt-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unittest_gpt-0.1.2/README.md` & `unittest_gpt-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `unittest_gpt-0.1.2/src/file_utils.py` & `unittest_gpt-0.1.3/src/file_utils.py`

 * *Files identical despite different names*

### Comparing `unittest_gpt-0.1.2/src/unit_test_agent.py` & `unittest_gpt-0.1.3/src/unit_test_agent.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
             # Generate the test case code
             test_case_code = self.generate_test_case_code(file_contents, file_name, test_file_name,
                                                           source_file_path)
             test_case_code = self.get_cleaned_code(test_case_code)
             formatted_code = autopep8.fix_code(test_case_code)
 
             # Get the path to the parent directory of the "src" director
-            project_directory = os.path.dirname(os.getcwd())
+            project_directory = os.path.abspath(os.getcwd())
 
             # Create the "tests" directory if it doesn't exist
             tests_directory = os.path.join(project_directory, 'tests')
 
             # Create the tests directory if it doesn't exist
             if not os.path.exists(tests_directory):
                 os.makedirs(tests_directory)
@@ -90,15 +90,15 @@
         code_block = code[start_index + 3: end_index]
 
         # Remove leading and trail  ing whitespace
         code = code_block.strip()
         return code
 
     def create_tests_init_file(self):
-        project_directory = os.path.dirname(os.getcwd())
+        project_directory = os.path.abspath(os.getcwd())
 
         # Create the "tests" directory if it doesn't exist
         tests_directory = os.path.join(project_directory, 'tests')
 
         if not os.path.exists(tests_directory):  # Check if the tests directory doesn't exist
             os.makedirs(tests_directory)  # Create the tests directory if it doesn't exist
```

### Comparing `unittest_gpt-0.1.2/PKG-INFO` & `unittest_gpt-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unittest-gpt
-Version: 0.1.2
+Version: 0.1.3
 Summary: Auto generate unit test using PyTest and Gpt
 License: MIT
 Author: Akshay Lingamaneni
 Requires-Python: >=3.11,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

