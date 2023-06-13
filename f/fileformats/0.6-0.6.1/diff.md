# Comparing `tmp/fileformats-0.6.tar.gz` & `tmp/fileformats-0.6.1.tar.gz`

## Comparing `fileformats-0.6.tar` & `fileformats-0.6.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/archive/__init__.py
--rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/archive/converters.py
--rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/archive/tests/test_archive_converters.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/audio/__init__.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/__init__.py
--rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/_version.py
--rw-r--r--   0        0        0    41119 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/base.py
--rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/converter.py
--rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/exceptions.py
--rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/mark.py
--rw-r--r--   0        0        0    24541 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/mixin.py
--rw-r--r--   0        0        0    10881 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/utils.py
--rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/tests/test_classifiers.py
--rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/tests/test_converter.py
--rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/tests/test_detection.py
--rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/tests/test_general.py
--rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/tests/test_mime.py
--rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/tests/test_mixin.py
--rw-r--r--   0        0        0     5899 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/core/tests/test_utils.py
--rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/document/__init__.py
--rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/field/__init__.py
--rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/field/tests/test_fields.py
--rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/field/tests/test_fields_mime.py
--rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/generic/__init__.py
--rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/image/__init__.py
--rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/image/base.py
--rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/image/converters.py
--rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/image/raster.py
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/image/vector.py
--rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/image/tests/test_image_converters.py
--rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/image/tests/test_image_raster.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/misc/__init__.py
--rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/misc/medical.py
--rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/numeric/__init__.py
--rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/serialization/__init__.py
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/serialization/converters.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/serialization/tests/test_serialization_converters.py
--rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/text/__init__.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.6/fileformats/video/__init__.py
--rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.6/.gitignore
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.6/AUTHORS
--rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.6/LICENSE
--rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.6/README.rst
--rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fileformats-0.6/pyproject.toml
--rw-r--r--   0        0        0    22510 2020-02-02 00:00:00.000000 fileformats-0.6/PKG-INFO
+-rw-r--r--   0        0        0     1342 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/archive/__init__.py
+-rw-r--r--   0        0        0     8869 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/archive/converters.py
+-rw-r--r--   0        0        0     2515 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/archive/tests/test_archive_converters.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/audio/__init__.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/_version.py
+-rw-r--r--   0        0        0    41153 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/base.py
+-rw-r--r--   0        0        0     5584 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/converter.py
+-rw-r--r--   0        0        0      486 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/exceptions.py
+-rw-r--r--   0        0        0     4609 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/mark.py
+-rw-r--r--   0        0        0    24541 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/mixin.py
+-rw-r--r--   0        0        0    10881 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/utils.py
+-rw-r--r--   0        0        0     8171 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/tests/test_classifiers.py
+-rw-r--r--   0        0        0     3990 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/tests/test_converter.py
+-rw-r--r--   0        0        0     5998 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/tests/test_detection.py
+-rw-r--r--   0        0        0     3336 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/tests/test_general.py
+-rw-r--r--   0        0        0      521 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/tests/test_mime.py
+-rw-r--r--   0        0        0     7043 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/tests/test_mixin.py
+-rw-r--r--   0        0        0     5884 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/core/tests/test_utils.py
+-rw-r--r--   0        0        0      773 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/document/__init__.py
+-rw-r--r--   0        0        0     4843 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/field/__init__.py
+-rw-r--r--   0        0        0     2205 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/field/tests/test_fields.py
+-rw-r--r--   0        0        0      733 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/field/tests/test_fields_mime.py
+-rw-r--r--   0        0        0     7937 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/generic/__init__.py
+-rw-r--r--   0        0        0      130 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/image/__init__.py
+-rw-r--r--   0        0        0      103 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/image/base.py
+-rw-r--r--   0        0        0      891 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/image/converters.py
+-rw-r--r--   0        0        0     1893 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/image/raster.py
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/image/vector.py
+-rw-r--r--   0        0        0      536 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/image/tests/test_image_converters.py
+-rw-r--r--   0        0        0      569 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/image/tests/test_image_raster.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/misc/__init__.py
+-rw-r--r--   0        0        0      305 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/misc/medical.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/numeric/__init__.py
+-rw-r--r--   0        0        0     2159 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/serialization/__init__.py
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/serialization/converters.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/serialization/tests/test_serialization_converters.py
+-rw-r--r--   0        0        0      691 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/text/__init__.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 fileformats-0.6.1/fileformats/video/__init__.py
+-rw-r--r--   0        0        0      242 2020-02-02 00:00:00.000000 fileformats-0.6.1/.gitignore
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 fileformats-0.6.1/AUTHORS
+-rw-r--r--   0        0        0    14222 2020-02-02 00:00:00.000000 fileformats-0.6.1/LICENSE
+-rw-r--r--   0        0        0     5235 2020-02-02 00:00:00.000000 fileformats-0.6.1/README.rst
+-rw-r--r--   0        0        0     2458 2020-02-02 00:00:00.000000 fileformats-0.6.1/pyproject.toml
+-rw-r--r--   0        0        0    22512 2020-02-02 00:00:00.000000 fileformats-0.6.1/PKG-INFO
```

### Comparing `fileformats-0.6/fileformats/archive/__init__.py` & `fileformats-0.6.1/fileformats/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/archive/converters.py` & `fileformats-0.6.1/fileformats/archive/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/archive/tests/test_archive_converters.py` & `fileformats-0.6.1/fileformats/archive/tests/test_archive_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/audio/__init__.py` & `fileformats-0.6.1/fileformats/audio/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/core/base.py` & `fileformats-0.6.1/fileformats/core/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -469,15 +469,15 @@
             try:
                 klass_attr.__annotations__[CHECK_ANNOTATION]
             except (AttributeError, KeyError):
                 pass
             else:
                 yield attr_name
 
-    def copy_to(
+    def copy(
         self,
         dest_dir: Path,
         stem: ty.Optional[str] = None,
         link_type: ty.Optional[str] = None,
         trim: bool = True,
         make_dirs: bool = False,
         overwrite: bool = False,
@@ -560,14 +560,18 @@
             if fspath.is_dir():
                 copy_dir(fspath, new_path)
             else:
                 copy_file(fspath, new_path)
             new_paths.append(new_path)
         return type(self)(new_paths)
 
+    def copy_to(self, *args, **kwargs):
+        """For b/w compatibility (temporary message)"""
+        return self.copy(*args, **kwargs)
+
     def select_by_ext(
         self, fileformat: ty.Optional[type] = None, allow_none: bool = False
     ) -> Path:
         """Selects a single path from a set of file-system paths based on the file
         extension
 
         Parameters
@@ -1036,25 +1040,25 @@
         for path, bytes_iter in self.byte_chunks(**kwargs):
             crypto_obj = crypto()
             for bytes_str in bytes_iter:
                 crypto_obj.update(bytes_str)
             file_hashes[str(path)] = crypto_obj.hexdigest()
         return file_hashes
 
-    def __bytes_repr__(self, cache, mode=None):  # pylint: disable=unused-argument
+    def __bytes_repr__(
+        self, cache: dict
+    ) -> ty.Iterable[bytes]:  # pylint: disable=unused-argument
         """Provided for compatibility with Pydra's hashing function, return the contents
         of all the files in the file-set in chunks
 
         Parameters
         ----------
-        cache : pydra.utils.hash.Cache
+        cache : dict
             an object passed around by Pydra's hashing function to store cached versions
             of previously hashed objects, to allow recursive structures
-        mode : int, optional
-            a flag used to specify the mode used to generate the bytes representation
 
         Yields
         ------
         bytes
             a chunk of bytes of length FILE_CHUNK_LEN_DEFAULT from the contents of all
             files in the file-set.
         """
```

### Comparing `fileformats-0.6/fileformats/core/converter.py` & `fileformats-0.6.1/fileformats/core/converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/core/mark.py` & `fileformats-0.6.1/fileformats/core/mark.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/core/mixin.py` & `fileformats-0.6.1/fileformats/core/mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/core/utils.py` & `fileformats-0.6.1/fileformats/core/utils.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/core/tests/test_classifiers.py` & `fileformats-0.6.1/fileformats/core/tests/test_classifiers.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/core/tests/test_converter.py` & `fileformats-0.6.1/fileformats/core/tests/test_converter.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/core/tests/test_detection.py` & `fileformats-0.6.1/fileformats/core/tests/test_detection.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/core/tests/test_general.py` & `fileformats-0.6.1/fileformats/core/tests/test_general.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/core/tests/test_mime.py` & `fileformats-0.6.1/fileformats/core/tests/test_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/core/tests/test_mixin.py` & `fileformats-0.6.1/fileformats/core/tests/test_mixin.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/core/tests/test_utils.py` & `fileformats-0.6.1/fileformats/core/tests/test_utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,42 +62,42 @@
 def dest_dir(work_dir):
     dest_dir = work_dir / "new-dir"
     dest_dir.mkdir()
     return dest_dir
 
 
 def test_copy(fsobject: FsObject, dest_dir: Path):
-    cpy = fsobject.copy_to(dest_dir)
+    cpy = fsobject.copy(dest_dir)
     assert all(p.parent == dest_dir for p in cpy.fspaths)
     assert set(p.name for p in cpy.fspaths) == set(p.name for p in fsobject.fspaths)
     assert cpy.hash() == fsobject.hash()
 
 
 def test_copy_symlink(fsobject: FsObject, dest_dir: Path):
-    cpy = fsobject.copy_to(dest_dir, link_type="symbolic")
+    cpy = fsobject.copy(dest_dir, link_type="symbolic")
     assert all(p.parent == dest_dir for p in cpy.fspaths)
     assert set(p.name for p in cpy.fspaths) == set(p.name for p in fsobject.fspaths)
     assert set(p.is_symlink() for p in cpy.fspaths)
     assert cpy.hash() == fsobject.hash()
 
 
 def test_copy_hardlink(fsobject: FsObject, dest_dir: Path):
-    cpy = fsobject.copy_to(dest_dir, link_type="hard")
+    cpy = fsobject.copy(dest_dir, link_type="hard")
     assert all(p.parent == dest_dir for p in cpy.fspaths)
     assert set(p.name for p in cpy.fspaths) == set(p.name for p in fsobject.fspaths)
     assert all(
         os.path.samefile(c, o)
         for c, o in zip(sorted(cpy.fspaths), sorted(fsobject.fspaths))
         if o.is_file()
     )
     assert cpy.hash() == fsobject.hash()
 
 
 def test_copy_with_rename(foo_file, dest_dir):
-    cpy = foo_file.copy_to(dest_dir, stem="new")
+    cpy = foo_file.copy(dest_dir, stem="new")
     assert cpy.fspath.name == "new.foo"
     assert cpy.header.fspath.name == "new.bar"
 
 
 def test_copy_ext(work_dir):
     assert (
         File.copy_ext(work_dir / "x.foo.bar", work_dir / "y") == work_dir / "y.foo.bar"
@@ -203,9 +203,9 @@
 
 
 def test_hash_files(fsobject: FsObject, work_dir: Path, dest_dir: Path):
     file_hashes = fsobject.hash_files(relative_to=work_dir)
     assert sorted(Path(p) for p in file_hashes) == sorted(
         p.relative_to(work_dir) for p in fsobject.all_file_paths
     )
-    cpy = fsobject.copy_to(dest_dir)
+    cpy = fsobject.copy(dest_dir)
     assert cpy.hash_files() == fsobject.hash_files()
```

### Comparing `fileformats-0.6/fileformats/document/__init__.py` & `fileformats-0.6.1/fileformats/document/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/field/__init__.py` & `fileformats-0.6.1/fileformats/field/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/field/tests/test_fields.py` & `fileformats-0.6.1/fileformats/field/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/field/tests/test_fields_mime.py` & `fileformats-0.6.1/fileformats/field/tests/test_fields_mime.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/generic/__init__.py` & `fileformats-0.6.1/fileformats/generic/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/image/converters.py` & `fileformats-0.6.1/fileformats/image/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/image/raster.py` & `fileformats-0.6.1/fileformats/image/raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/image/tests/test_image_converters.py` & `fileformats-0.6.1/fileformats/image/tests/test_image_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/image/tests/test_image_raster.py` & `fileformats-0.6.1/fileformats/image/tests/test_image_raster.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/serialization/__init__.py` & `fileformats-0.6.1/fileformats/serialization/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/serialization/converters.py` & `fileformats-0.6.1/fileformats/serialization/converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/serialization/tests/test_serialization_converters.py` & `fileformats-0.6.1/fileformats/serialization/tests/test_serialization_converters.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/fileformats/text/__init__.py` & `fileformats-0.6.1/fileformats/text/__init__.py`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/LICENSE` & `fileformats-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/README.rst` & `fileformats-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/pyproject.toml` & `fileformats-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `fileformats-0.6/PKG-INFO` & `fileformats-0.6.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fileformats
-Version: 0.6
+Version: 0.6.1
 Summary: Classes for representing different file formats in Python classes for use in type hinting in data workflows
 Project-URL: repository, https://github.com/ArcanaFramework/fileformats
 Author-email: "Thomas G. Close" <tom.g.close@gmail.com>
 Maintainer-email: "Thomas G. Close" <tom.g.close@gmail.com>
 License: Creative Commons Attribution 4.0 International Public License
         By exercising the Licensed Rights (defined below), You accept and agree to be bound by the terms and conditions of this Creative Commons Attribution 4.0 International Public License ("Public License"). To the extent this Public License may be interpreted as a contract, You are granted the Licensed Rights in consideration of Your acceptance of these terms and conditions, and the Licensor grants You such rights in consideration of benefits the Licensor receives from making the Licensed Material available under these terms and conditions.
```

