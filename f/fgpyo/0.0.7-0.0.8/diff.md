# Comparing `tmp/fgpyo-0.0.7.tar.gz` & `tmp/fgpyo-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fgpyo-0.0.7.tar", max compression
+gzip compressed data, was "fgpyo-0.0.8.tar", max compression
```

## Comparing `fgpyo-0.0.7.tar` & `fgpyo-0.0.8.tar`

### file list

```diff
@@ -1,39 +1,41 @@
--rw-r--r--   0        0        0     1634 2022-12-03 22:17:56.407543 fgpyo-0.0.7/LICENSE
--rw-r--r--   0        0        0     2407 2023-03-09 22:41:56.010256 fgpyo-0.0.7/README.md
--rw-r--r--   0        0        0        0 2022-09-21 20:22:00.331481 fgpyo-0.0.7/fgpyo/__init__.py
--rw-r--r--   0        0        0     4531 2022-12-03 22:17:56.408040 fgpyo-0.0.7/fgpyo/collections/__init__.py
--rw-r--r--   0        0        0        0 2022-12-03 22:17:56.408102 fgpyo-0.0.7/fgpyo/collections/tests/__init__.py
--rw-r--r--   0        0        0     1637 2022-12-03 22:17:56.408182 fgpyo-0.0.7/fgpyo/collections/tests/test_peekable_iterator.py
--rw-r--r--   0        0        0        0 2023-03-09 17:27:05.109876 fgpyo-0.0.7/fgpyo/fasta/__init__.py
--rwxr-xr-x   0        0        0     8003 2023-03-09 22:41:56.011875 fgpyo-0.0.7/fgpyo/fasta/builder.py
--rw-r--r--   0        0        0        0 2023-03-09 17:27:05.110130 fgpyo-0.0.7/fgpyo/fasta/tests/__init__.py
--rw-r--r--   0        0        0     2347 2023-03-09 17:48:41.932129 fgpyo-0.0.7/fgpyo/fasta/tests/test_builder.py
--rw-r--r--   0        0        0     6634 2023-04-06 00:36:59.022924 fgpyo-0.0.7/fgpyo/io/__init__.py
--rw-r--r--   0        0        0        0 2023-04-06 00:36:59.023026 fgpyo-0.0.7/fgpyo/io/tests/_init__.py
--rw-r--r--   0        0        0     4498 2023-04-06 00:36:59.023186 fgpyo-0.0.7/fgpyo/io/tests/test_io.py
--rw-r--r--   0        0        0    13880 2022-12-03 22:17:56.408348 fgpyo-0.0.7/fgpyo/read_structure.py
--rw-r--r--   0        0        0    32206 2023-04-06 00:36:59.024010 fgpyo-0.0.7/fgpyo/sam/__init__.py
--rwxr-xr-x   0        0        0    24169 2023-03-09 22:41:56.012913 fgpyo-0.0.7/fgpyo/sam/builder.py
--rwxr-xr-x   0        0        0    16792 2022-12-03 22:17:56.408875 fgpyo-0.0.7/fgpyo/sam/clipping.py
--rw-r--r--   0        0        0        0 2022-12-03 22:17:56.408952 fgpyo-0.0.7/fgpyo/sam/tests/__init__.py
--rwxr-xr-x   0        0        0     3461 2022-12-03 22:17:56.409074 fgpyo-0.0.7/fgpyo/sam/tests/data/valid.sam
--rwxr-xr-x   0        0        0     8442 2022-12-03 22:17:56.409168 fgpyo-0.0.7/fgpyo/sam/tests/test_builder.py
--rwxr-xr-x   0        0        0    15087 2022-12-03 22:17:56.409255 fgpyo-0.0.7/fgpyo/sam/tests/test_clipping.py
--rwxr-xr-x   0        0        0    12375 2022-12-03 22:17:56.409351 fgpyo-0.0.7/fgpyo/sam/tests/test_sam.py
--rw-r--r--   0        0        0     1632 2022-12-03 22:17:56.409441 fgpyo-0.0.7/fgpyo/sam/tests/test_supplementary_alignments.py
--rw-r--r--   0        0        0     2556 2022-12-03 22:17:56.409513 fgpyo-0.0.7/fgpyo/sam/tests/test_template_iterator.py
--rw-r--r--   0        0        0     1527 2022-12-03 22:17:56.409587 fgpyo-0.0.7/fgpyo/sequence.py
--rw-r--r--   0        0        0        0 2022-09-21 20:22:00.331711 fgpyo-0.0.7/fgpyo/tests/__init__.py
--rw-r--r--   0        0        0     9836 2023-03-09 22:41:56.013388 fgpyo-0.0.7/fgpyo/tests/test_read_structure.py
--rw-r--r--   0        0        0      473 2022-12-03 22:17:56.409782 fgpyo-0.0.7/fgpyo/tests/test_sequence.py
--rw-r--r--   0        0        0    12032 2023-03-09 17:48:41.932554 fgpyo-0.0.7/fgpyo/util/inspect.py
--rw-r--r--   0        0        0     6516 2023-04-06 00:36:59.025037 fgpyo-0.0.7/fgpyo/util/logging.py
--rw-r--r--   0        0        0     8685 2023-03-09 17:27:05.111399 fgpyo-0.0.7/fgpyo/util/metric.py
--rw-r--r--   0        0        0      822 2023-03-09 22:41:58.353824 fgpyo-0.0.7/fgpyo/util/string.py
--rw-r--r--   0        0        0        0 2022-09-21 20:22:00.332437 fgpyo-0.0.7/fgpyo/util/tests/__init__.py
--rw-r--r--   0        0        0     1792 2023-04-06 00:36:59.025261 fgpyo-0.0.7/fgpyo/util/tests/test_logging.py
--rw-r--r--   0        0        0     6826 2023-03-09 17:48:41.933010 fgpyo-0.0.7/fgpyo/util/tests/test_metric.py
--rw-r--r--   0        0        0      581 2023-03-09 22:41:58.354037 fgpyo-0.0.7/fgpyo/util/tests/test_string.py
--rw-r--r--   0        0        0     6323 2023-03-09 17:48:41.933185 fgpyo-0.0.7/fgpyo/util/types.py
--rw-r--r--   0        0        0     1395 2023-04-06 00:39:38.283578 fgpyo-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     3837 1970-01-01 00:00:00.000000 fgpyo-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1634 2022-12-03 22:17:56.407543 fgpyo-0.0.8/LICENSE
+-rw-r--r--   0        0        0     2407 2023-03-09 22:41:56.010256 fgpyo-0.0.8/README.md
+-rw-r--r--   0        0        0        0 2022-09-21 20:22:00.331481 fgpyo-0.0.8/fgpyo/__init__.py
+-rw-r--r--   0        0        0     4531 2022-12-03 22:17:56.408040 fgpyo-0.0.8/fgpyo/collections/__init__.py
+-rw-r--r--   0        0        0        0 2022-12-03 22:17:56.408102 fgpyo-0.0.8/fgpyo/collections/tests/__init__.py
+-rw-r--r--   0        0        0     1637 2022-12-03 22:17:56.408182 fgpyo-0.0.8/fgpyo/collections/tests/test_peekable_iterator.py
+-rw-r--r--   0        0        0        0 2023-03-09 17:27:05.109876 fgpyo-0.0.8/fgpyo/fasta/__init__.py
+-rwxr-xr-x   0        0        0     8003 2023-03-09 22:41:56.011875 fgpyo-0.0.8/fgpyo/fasta/builder.py
+-rw-r--r--   0        0        0        0 2023-03-09 17:27:05.110130 fgpyo-0.0.8/fgpyo/fasta/tests/__init__.py
+-rw-r--r--   0        0        0     2347 2023-03-09 17:48:41.932129 fgpyo-0.0.8/fgpyo/fasta/tests/test_builder.py
+-rw-r--r--   0        0        0     6634 2023-04-06 00:36:59.022924 fgpyo-0.0.8/fgpyo/io/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-06 00:36:59.023026 fgpyo-0.0.8/fgpyo/io/tests/_init__.py
+-rw-r--r--   0        0        0     4498 2023-04-06 00:36:59.023186 fgpyo-0.0.8/fgpyo/io/tests/test_io.py
+-rw-r--r--   0        0        0    13880 2022-12-03 22:17:56.408348 fgpyo-0.0.8/fgpyo/read_structure.py
+-rw-r--r--   0        0        0    32592 2023-06-13 18:15:00.456247 fgpyo-0.0.8/fgpyo/sam/__init__.py
+-rwxr-xr-x   0        0        0    24169 2023-03-09 22:41:56.012913 fgpyo-0.0.8/fgpyo/sam/builder.py
+-rwxr-xr-x   0        0        0    16792 2022-12-03 22:17:56.408875 fgpyo-0.0.8/fgpyo/sam/clipping.py
+-rw-r--r--   0        0        0        0 2022-12-03 22:17:56.408952 fgpyo-0.0.8/fgpyo/sam/tests/__init__.py
+-rwxr-xr-x   0        0        0      282 2023-04-26 23:11:38.813727 fgpyo-0.0.8/fgpyo/sam/tests/data/unmapped.sam
+-rwxr-xr-x   0        0        0     3461 2022-12-03 22:17:56.409074 fgpyo-0.0.8/fgpyo/sam/tests/data/valid.sam
+-rwxr-xr-x   0        0        0     8442 2022-12-03 22:17:56.409168 fgpyo-0.0.8/fgpyo/sam/tests/test_builder.py
+-rwxr-xr-x   0        0        0    15087 2022-12-03 22:17:56.409255 fgpyo-0.0.8/fgpyo/sam/tests/test_clipping.py
+-rwxr-xr-x   0        0        0    12709 2023-04-26 23:11:38.814586 fgpyo-0.0.8/fgpyo/sam/tests/test_sam.py
+-rw-r--r--   0        0        0     1632 2022-12-03 22:17:56.409441 fgpyo-0.0.8/fgpyo/sam/tests/test_supplementary_alignments.py
+-rw-r--r--   0        0        0     2556 2022-12-03 22:17:56.409513 fgpyo-0.0.8/fgpyo/sam/tests/test_template_iterator.py
+-rw-r--r--   0        0        0     1527 2022-12-03 22:17:56.409587 fgpyo-0.0.8/fgpyo/sequence.py
+-rw-r--r--   0        0        0        0 2022-09-21 20:22:00.331711 fgpyo-0.0.8/fgpyo/tests/__init__.py
+-rw-r--r--   0        0        0     9836 2023-03-09 22:41:56.013388 fgpyo-0.0.8/fgpyo/tests/test_read_structure.py
+-rw-r--r--   0        0        0      473 2022-12-03 22:17:56.409782 fgpyo-0.0.8/fgpyo/tests/test_sequence.py
+-rw-r--r--   0        0        0    12032 2023-03-09 17:48:41.932554 fgpyo-0.0.8/fgpyo/util/inspect.py
+-rw-r--r--   0        0        0     6516 2023-04-06 00:36:59.025037 fgpyo-0.0.8/fgpyo/util/logging.py
+-rw-r--r--   0        0        0     8685 2023-03-09 17:27:05.111399 fgpyo-0.0.8/fgpyo/util/metric.py
+-rw-r--r--   0        0        0      822 2023-03-09 22:41:58.353824 fgpyo-0.0.8/fgpyo/util/string.py
+-rw-r--r--   0        0        0        0 2022-09-21 20:22:00.332437 fgpyo-0.0.8/fgpyo/util/tests/__init__.py
+-rw-r--r--   0        0        0     1792 2023-04-06 00:36:59.025261 fgpyo-0.0.8/fgpyo/util/tests/test_logging.py
+-rw-r--r--   0        0        0     6826 2023-03-09 17:48:41.933010 fgpyo-0.0.8/fgpyo/util/tests/test_metric.py
+-rw-r--r--   0        0        0      581 2023-03-09 22:41:58.354037 fgpyo-0.0.8/fgpyo/util/tests/test_string.py
+-rw-r--r--   0        0        0     6323 2023-03-09 17:48:41.933185 fgpyo-0.0.8/fgpyo/util/types.py
+-rw-r--r--   0        0        0     1395 2023-06-13 18:15:47.697644 fgpyo-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     3550 2023-06-13 18:16:39.147053 fgpyo-0.0.8/setup.py
+-rw-r--r--   0        0        0     3735 2023-06-13 18:16:39.147309 fgpyo-0.0.8/PKG-INFO
```

### Comparing `fgpyo-0.0.7/LICENSE` & `fgpyo-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/README.md` & `fgpyo-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/collections/__init__.py` & `fgpyo-0.0.8/fgpyo/collections/__init__.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/collections/tests/test_peekable_iterator.py` & `fgpyo-0.0.8/fgpyo/collections/tests/test_peekable_iterator.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/fasta/builder.py` & `fgpyo-0.0.8/fgpyo/fasta/builder.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/fasta/tests/test_builder.py` & `fgpyo-0.0.8/fgpyo/fasta/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/io/__init__.py` & `fgpyo-0.0.8/fgpyo/io/__init__.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/io/tests/test_io.py` & `fgpyo-0.0.8/fgpyo/io/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/read_structure.py` & `fgpyo-0.0.8/fgpyo/read_structure.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/sam/__init__.py` & `fgpyo-0.0.8/fgpyo/sam/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -215,23 +215,28 @@
         try:
             return next(iter([tpe for tpe in SamFileType if tpe.extension == ext]))
         except StopIteration:
             raise ValueError(f"Could not infer file type from {path}")
 
 
 def _pysam_open(
-    path: SamPath, open_for_reading: bool, file_type: Optional[SamFileType] = None, **kwargs: Any
+    path: SamPath,
+    open_for_reading: bool,
+    file_type: Optional[SamFileType] = None,
+    unmapped: bool = False,
+    **kwargs: Any,
 ) -> SamFile:
     """Opens a SAM/BAM/CRAM for reading or writing.
 
     Args:
         path: a file handle or path to the SAM/BAM/CRAM to read or write.
         open_for_reading: True to open for reading, false otherwise.
         file_type: the file type to assume when opening the file.  If None, then the file type
             will be auto-detected for reading and must be a path-like object for writing.
+        unmapped: True if the file is unmapped and has no sequence dictionary, False otherwise.
         kwargs: any keyword arguments to be passed to
         :class:`~pysam.AlignmentFile`; may not include "mode".
     """
 
     if isinstance(path, (str, Path)):  # type: ignore
         file_type = file_type or SamFileType.from_path(path)
         path = str(path)
@@ -247,27 +252,33 @@
     # writing since we can let pysam auto-recognize the file type when reading.  See discussion:
     # https://github.com/pysam-developers/pysam/issues/655
     if file_type is not None:
         kwargs["mode"] = "r" if open_for_reading else "w" + file_type.mode
     else:
         assert open_for_reading, "Bug: file_type was None but open_for_reading was False"
 
+    if unmapped and open_for_reading:
+        kwargs["check_sq"] = False
+
     # Open it!
     return pysam.AlignmentFile(path, **kwargs)
 
 
-def reader(path: SamPath, file_type: Optional[SamFileType] = None) -> SamFile:
+def reader(
+    path: SamPath, file_type: Optional[SamFileType] = None, unmapped: bool = False
+) -> SamFile:
     """Opens a SAM/BAM/CRAM for reading.
 
     Args:
         path: a file handle or path to the SAM/BAM/CRAM to read or write.
         file_type: the file type to assume when opening the file.  If None, then the file
             type will be auto-detected.
+        unmapped: True if the file is unmapped and has no sequence dictionary, False otherwise.
     """
-    return _pysam_open(path=path, open_for_reading=True, file_type=file_type)
+    return _pysam_open(path=path, open_for_reading=True, file_type=file_type, unmapped=unmapped)
 
 
 def writer(
     path: SamPath,
     header: Union[str, Dict[str, Any], SamHeader],
     file_type: Optional[SamFileType] = None,
 ) -> SamFile:
@@ -283,15 +294,17 @@
         file_type: the file type to assume when opening the file.  If None, then the
             filetype will be auto-detected and must be a path-like object.
     """
     # Set the header for pysam's AlignmentFile
     key = "text" if isinstance(header, str) else "header"
     kwargs = {key: header}
 
-    return _pysam_open(path=path, open_for_reading=False, file_type=file_type, **kwargs)
+    return _pysam_open(
+        path=path, open_for_reading=False, file_type=file_type, unmapped=False, **kwargs
+    )
 
 
 class _CigarOpUtil:
     """Some useful constants to speed up methods on CigarOp"""
 
     """A dictionary from the cigar op code to the cigar op char.
```

### Comparing `fgpyo-0.0.7/fgpyo/sam/builder.py` & `fgpyo-0.0.8/fgpyo/sam/builder.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/sam/clipping.py` & `fgpyo-0.0.8/fgpyo/sam/clipping.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/sam/tests/data/valid.sam` & `fgpyo-0.0.8/fgpyo/sam/tests/data/valid.sam`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/sam/tests/test_builder.py` & `fgpyo-0.0.8/fgpyo/sam/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/sam/tests/test_clipping.py` & `fgpyo-0.0.8/fgpyo/sam/tests/test_clipping.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/sam/tests/test_sam.py` & `fgpyo-0.0.8/fgpyo/sam/tests/test_sam.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,14 +55,19 @@
                 num_read += 1
                 fh_out.write(rec)
     assert num_read == 8
     yield bam
     bam.unlink()
 
 
+@pytest.fixture
+def unmapped_sam() -> Path:
+    return Path(__file__).parent / "data" / "unmapped.sam"
+
+
 @pytest.fixture(scope="function")
 def in_path(request: Any, valid_sam: Path, valid_bam: Path) -> Path:
     """A fixture for test_sam_file_open_reading to modify in_path prior to executing.
 
     Returns:
          the path corresponding to the given file type (i.e. SAM or BAM).
     """
@@ -97,14 +102,19 @@
 
 
 def test_sam_file_open_reading_with_reader(valid_sam: Path) -> None:
     with sam.reader(path=valid_sam, file_type=None) as samfile:
         assert sum(1 for _ in samfile) == 8
 
 
+def test_unmapped_sam_file_open_reading_with_reader(unmapped_sam: Path) -> None:
+    with sam.reader(path=unmapped_sam, unmapped=True) as samfile:
+        assert len([read for read in samfile.fetch() if read.is_unmapped]) == 1
+
+
 @pytest.fixture
 def expected_records(valid_sam: Path) -> List[pysam.AlignedSegment]:
     """Returns the records that are found in the valid_sam."""
     with sam.reader(valid_sam) as fh:
         return [r for r in fh]
```

### Comparing `fgpyo-0.0.7/fgpyo/sam/tests/test_supplementary_alignments.py` & `fgpyo-0.0.8/fgpyo/sam/tests/test_supplementary_alignments.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/sam/tests/test_template_iterator.py` & `fgpyo-0.0.8/fgpyo/sam/tests/test_template_iterator.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/sequence.py` & `fgpyo-0.0.8/fgpyo/sequence.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/tests/test_read_structure.py` & `fgpyo-0.0.8/fgpyo/tests/test_read_structure.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/util/inspect.py` & `fgpyo-0.0.8/fgpyo/util/inspect.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/util/logging.py` & `fgpyo-0.0.8/fgpyo/util/logging.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/util/metric.py` & `fgpyo-0.0.8/fgpyo/util/metric.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/util/string.py` & `fgpyo-0.0.8/fgpyo/util/string.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/util/tests/test_logging.py` & `fgpyo-0.0.8/fgpyo/util/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/util/tests/test_metric.py` & `fgpyo-0.0.8/fgpyo/util/tests/test_metric.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/util/tests/test_string.py` & `fgpyo-0.0.8/fgpyo/util/tests/test_string.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/fgpyo/util/types.py` & `fgpyo-0.0.8/fgpyo/util/types.py`

 * *Files identical despite different names*

### Comparing `fgpyo-0.0.7/pyproject.toml` & `fgpyo-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fgpyo"
-version = "0.0.7"
+version = "0.0.8"
 description = "Python bioinformatics and genomics library"
 authors = ["Nils Homer", "Tim Fennell", "Nathan Roach"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/fulcrumgenomics/fgpyo"
 repository = "https://github.com/fulcrumgenomics/fgpyo"
 keywords = ["bioinformatics"]
```

### Comparing `fgpyo-0.0.7/PKG-INFO` & `fgpyo-0.0.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,36 @@
 Metadata-Version: 2.1
 Name: fgpyo
-Version: 0.0.7
+Version: 0.0.8
 Summary: Python bioinformatics and genomics library
 Home-page: https://github.com/fulcrumgenomics/fgpyo
 License: MIT
 Keywords: bioinformatics
 Author: Nils Homer
 Requires-Python: >=3.7.0,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Software Development :: Documentation
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: docs
 Requires-Dist: attrs (>=19.3.0)
 Requires-Dist: pysam (>=0.20.0)
-Requires-Dist: sphinx (==4.3.1) ; extra == "docs"
-Requires-Dist: typing_extensions (>=3.7.4) ; python_version < "3.8"
-Requires-Dist: typing_inspect (>=0.3.1) ; python_version < "3.8"
+Requires-Dist: sphinx (==4.3.1); extra == "docs"
+Requires-Dist: typing_extensions (>=3.7.4); python_version < "3.8"
+Requires-Dist: typing_inspect (>=0.3.1); python_version < "3.8"
 Project-URL: Repository, https://github.com/fulcrumgenomics/fgpyo
 Description-Content-Type: text/markdown
 
 
 [![Language][language-badge]][language-link]
 [![Code Style][code-style-badge]][code-style-link]
 [![Type Checked][type-checking-badge]][type-checking-link]
```

