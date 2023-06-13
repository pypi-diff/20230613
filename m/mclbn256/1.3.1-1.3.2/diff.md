# Comparing `tmp/mclbn256-1.3.1-py3-none-win_amd64.whl.zip` & `tmp/mclbn256-1.3.2-py3-none-win_amd64.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 1477746 bytes, number of entries: 7
--rw-r--r--  2.0 unx  1469718 b- stor 23-May-02 03:43 mclbn256/mclbn256.py
--rw-r--r--  2.0 unx       45 b- stor 23-May-02 03:43 mclbn256/__init__.py
-?rw-------  2.0 unx     3658 b- stor 23-May-02 03:43 mclbn256-1.3.1.dist-info/METADATA
-?rw-------  2.0 unx       85 b- stor 23-May-02 03:43 mclbn256-1.3.1.dist-info/WHEEL
-?rw-------  2.0 unx        9 b- stor 23-May-02 03:43 mclbn256-1.3.1.dist-info/top_level.txt
-?rw-------  2.0 unx      595 b- stor 23-May-02 03:43 mclbn256-1.3.1.dist-info/RECORD
-?rw-------  2.0 unx     2674 b- stor 23-May-02 03:43 mclbn256-1.3.1.dist-info/LICENSE
-7 files, 1476784 bytes uncompressed, 1476784 bytes compressed:  0.0%
+Zip file size: 1478200 bytes, number of entries: 7
+-rw-r--r--  2.0 unx  1470172 b- stor 23-Jun-06 14:04 mclbn256/mclbn256.py
+-rw-r--r--  2.0 unx       45 b- stor 23-Jun-06 14:04 mclbn256/__init__.py
+?rw-------  2.0 unx     3658 b- stor 23-Jun-06 14:04 mclbn256-1.3.2.dist-info/METADATA
+?rw-------  2.0 unx       85 b- stor 23-Jun-06 14:04 mclbn256-1.3.2.dist-info/WHEEL
+?rw-------  2.0 unx        9 b- stor 23-Jun-06 14:04 mclbn256-1.3.2.dist-info/top_level.txt
+?rw-------  2.0 unx      595 b- stor 23-Jun-06 14:04 mclbn256-1.3.2.dist-info/RECORD
+?rw-------  2.0 unx     2674 b- stor 23-Jun-06 14:04 mclbn256-1.3.2.dist-info/LICENSE
+7 files, 1477238 bytes uncompressed, 1477238 bytes compressed:  0.0%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: mclbn256/mclbn256.py
 Comment: 
 
 Filename: mclbn256/__init__.py
 Comment: 
 
-Filename: mclbn256-1.3.1.dist-info/METADATA
+Filename: mclbn256-1.3.2.dist-info/METADATA
 Comment: 
 
-Filename: mclbn256-1.3.1.dist-info/WHEEL
+Filename: mclbn256-1.3.2.dist-info/WHEEL
 Comment: 
 
-Filename: mclbn256-1.3.1.dist-info/top_level.txt
+Filename: mclbn256-1.3.2.dist-info/top_level.txt
 Comment: 
 
-Filename: mclbn256-1.3.1.dist-info/RECORD
+Filename: mclbn256-1.3.2.dist-info/RECORD
 Comment: 
 
-Filename: mclbn256-1.3.1.dist-info/LICENSE
+Filename: mclbn256-1.3.2.dist-info/LICENSE
 Comment: 
 
 Zip file comment:
```

## mclbn256/mclbn256.py

```diff
@@ -22,27 +22,40 @@
 
 # Generate a temporary folder structure on disk to which to write the mcl binaries.
 temp_dir = tempfile.TemporaryDirectory()  # pylint: disable=consider-using-with
 LOADER_TEMP_PATH = temp_dir.name
 if False: print(LOADER_TEMP_PATH)
 os.makedirs(os.path.join(LOADER_TEMP_PATH, 'lib'))
 LIB_EXT = ".dll" if pl == "Windows" else ".dylib" if pl == "Darwin" else ".so"
-fd_libmcl = open(os.path.join(LOADER_TEMP_PATH, 'lib', 'libmcl'+LIB_EXT), "wb")
+if len(mcl_bs) > 0: fd_libmcl = open(os.path.join(LOADER_TEMP_PATH, 'lib', 'libmcl'+LIB_EXT), "wb")
 fd_libmclbn256 = open(os.path.join(LOADER_TEMP_PATH, 'libmclbn256'+LIB_EXT), "wb")
-fd_libmcl.write(mcl_bs)
+if len(mcl_bs) > 0: fd_libmcl.write(mcl_bs)
 fd_libmclbn256.write(mclbn256_bs)
+
 # Close temp file to avoid multiprocess access error on Windows
-fd_libmcl.close()
+if len(mcl_bs) > 0: fd_libmcl.close()
 fd_libmclbn256.close()
 # Manual cleanup is optional, but saves ~1mb of space on dist immediately after being called.
 cleanup = temp_dir.cleanup
 
+loaded_libraries = {}
+if len(mcl_bs) > 0:
+    loaded_libraries['libmcl'] \
+        = cdll.LoadLibrary(os.path.join(LOADER_TEMP_PATH, os.path.join('lib', 'libmcl'+LIB_EXT)))
+loaded_libraries['libmclbn256'] \
+        = cdll.LoadLibrary(os.path.join(LOADER_TEMP_PATH, 'libmclbn256'+LIB_EXT))
+
 def load_library(path_name):
-    return cdll.LoadLibrary(os.path.join(LOADER_TEMP_PATH, path_name+LIB_EXT))
+    return loaded_libraries[path_name]
+      #cdll.LoadLibrary(os.path.join(LOADER_TEMP_PATH, path_name+LIB_EXT))
+
 
+cleanup()
+#print('Python has cleaned up mclbn256.')
+#print('end.')
 
 #
 # Define constants needed to replace the C headers
 #
 mclBn_CurveFp254BNb = 0
 EMBEDDING_DEGREE = 12
 DIMENSIONALITY = 3
```

## Comparing `mclbn256-1.3.1.dist-info/METADATA` & `mclbn256-1.3.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mclbn256
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python bindings for the BN254/256 pairing-friendly curve supported by the MCl library.
 Home-page: https://github.com/nthparty/mclbn256
 Author: Wyatt Howe
 Author-email: Wyatt@nthparty.com
 /issues
 License: None
 Classifier: Programming Language :: Python :: 3
```

## Comparing `mclbn256-1.3.1.dist-info/LICENSE` & `mclbn256-1.3.2.dist-info/LICENSE`

 * *Files identical despite different names*

