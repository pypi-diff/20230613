# Comparing `tmp/algokit_client_generator-1.0.0b1-py3-none-any.whl.zip` & `tmp/algokit_client_generator-1.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 18236 bytes, number of entries: 14
+Zip file size: 18227 bytes, number of entries: 14
 -rw-r--r--  2.0 unx       91 b- defN 80-Jan-01 00:00 algokit_client_generator/__init__.py
 -rw-r--r--  2.0 unx       54 b- defN 80-Jan-01 00:00 algokit_client_generator/__main__.py
 -rw-r--r--  2.0 unx     2550 b- defN 80-Jan-01 00:00 algokit_client_generator/cli.py
 -rw-r--r--  2.0 unx     3199 b- defN 80-Jan-01 00:00 algokit_client_generator/document.py
 -rw-r--r--  2.0 unx    36317 b- defN 80-Jan-01 00:00 algokit_client_generator/generator.py
 -rw-r--r--  2.0 unx        0 b- defN 80-Jan-01 00:00 algokit_client_generator/py.typed
 -rw-r--r--  2.0 unx     7466 b- defN 80-Jan-01 00:00 algokit_client_generator/spec.py
--rw-r--r--  2.0 unx     4303 b- defN 80-Jan-01 00:00 algokit_client_generator/utils.py
+-rw-r--r--  2.0 unx     4372 b- defN 80-Jan-01 00:00 algokit_client_generator/utils.py
 -rw-r--r--  2.0 unx      995 b- defN 80-Jan-01 00:00 algokit_client_generator/writer.py
--rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.0b1.dist-info/LICENSE
--rw-r--r--  2.0 unx     4756 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.0b1.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.0b1.dist-info/WHEEL
--rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.0b1.dist-info/entry_points.txt
-?rw-r--r--  2.0 unx     1298 b- defN 16-Jan-01 00:00 algokit_client_generator-1.0.0b1.dist-info/RECORD
-14 files, 62260 bytes uncompressed, 16020 bytes compressed:  74.3%
+-rw-r--r--  2.0 unx     1076 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4754 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       67 b- defN 80-Jan-01 00:00 algokit_client_generator-1.0.1.dist-info/entry_points.txt
+?rw-r--r--  2.0 unx     1288 b- defN 16-Jan-01 00:00 algokit_client_generator-1.0.1.dist-info/RECORD
+14 files, 62317 bytes uncompressed, 16031 bytes compressed:  74.3%
```

## zipnote {}

```diff
@@ -21,23 +21,23 @@
 
 Filename: algokit_client_generator/utils.py
 Comment: 
 
 Filename: algokit_client_generator/writer.py
 Comment: 
 
-Filename: algokit_client_generator-1.0.0b1.dist-info/LICENSE
+Filename: algokit_client_generator-1.0.1.dist-info/LICENSE
 Comment: 
 
-Filename: algokit_client_generator-1.0.0b1.dist-info/METADATA
+Filename: algokit_client_generator-1.0.1.dist-info/METADATA
 Comment: 
 
-Filename: algokit_client_generator-1.0.0b1.dist-info/WHEEL
+Filename: algokit_client_generator-1.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: algokit_client_generator-1.0.0b1.dist-info/entry_points.txt
+Filename: algokit_client_generator-1.0.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: algokit_client_generator-1.0.0b1.dist-info/RECORD
+Filename: algokit_client_generator-1.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## algokit_client_generator/utils.py

```diff
@@ -58,14 +58,16 @@
 
 def map_abi_type_to_python(abi_type_str: str) -> str:
     if abi_type_str == "void":
         return "None"
     if abi.is_abi_transaction_type(abi_type_str):
         # TODO: generic TransactionWithSigner and/or allow unsigned types signed with signer used in transaction
         return "TransactionWithSigner"
+    if abi.is_abi_reference_type(abi_type_str):
+        return "int"
     abi_type = abi.ABIType.from_string(abi_type_str)
     return abi_type_to_python(abi_type)
 
 
 def get_unique_symbol_by_incrementing(existing_symbols: set[str], base_name: str) -> str:
     suffix = 0
     while True:
```

## Comparing `algokit_client_generator-1.0.0b1.dist-info/LICENSE` & `algokit_client_generator-1.0.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `algokit_client_generator-1.0.0b1.dist-info/METADATA` & `algokit_client_generator-1.0.1.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: algokit-client-generator
-Version: 1.0.0b1
+Version: 1.0.1
 Summary: Algorand typed client Generator
 License: MIT
 Author: Algorand Foundation
 Author-email: contact@algorand.foundation
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

