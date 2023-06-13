# Comparing `tmp/netzip-0.1.tar.gz` & `tmp/netzip-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netzip-0.1.tar", last modified: Fri Jun  9 09:44:37 2023, max compression
+gzip compressed data, was "netzip-0.2.tar", last modified: Tue Jun 13 16:29:40 2023, max compression
```

## Comparing `netzip-0.1.tar` & `netzip-0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:44:37.331382 netzip-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-09 09:43:57.000000 netzip-0.1/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:44:37.327382 netzip-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:44:37.331382 netzip-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-09 09:43:57.000000 netzip-0.1/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-09 09:43:57.000000 netzip-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-09 09:43:57.000000 netzip-0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-09 09:44:37.331382 netzip-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-09 09:43:57.000000 netzip-0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-06-09 09:43:57.000000 netzip-0.1/noxfile.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-09 09:43:57.000000 netzip-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-09 09:44:37.331382 netzip-0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:44:37.331382 netzip-0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:44:37.331382 netzip-0.1/src/netzip.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-09 09:44:37.000000 netzip-0.1/src/netzip.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-09 09:44:37.000000 netzip-0.1/src/netzip.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:44:37.000000 netzip-0.1/src/netzip.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-09 09:44:37.000000 netzip-0.1/src/netzip.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     9467 2023-06-09 09:43:57.000000 netzip-0.1/src/netzip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-09 09:44:37.331382 netzip-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-06-09 09:43:57.000000 netzip-0.1/tests/test_netzip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:40.834752 netzip-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      179 2023-06-13 16:29:16.000000 netzip-0.2/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:40.834752 netzip-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:40.834752 netzip-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      561 2023-06-13 16:29:16.000000 netzip-0.2/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-13 16:29:16.000000 netzip-0.2/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-13 16:29:16.000000 netzip-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-13 16:29:16.000000 netzip-0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-13 16:29:40.834752 netzip-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      220 2023-06-13 16:29:16.000000 netzip-0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-13 16:29:16.000000 netzip-0.2/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)      538 2023-06-13 16:29:16.000000 netzip-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 16:29:40.834752 netzip-0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:40.834752 netzip-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:40.834752 netzip-0.2/src/netzip.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-06-13 16:29:40.000000 netzip-0.2/src/netzip.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-06-13 16:29:40.000000 netzip-0.2/src/netzip.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:29:40.000000 netzip-0.2/src/netzip.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 16:29:40.000000 netzip-0.2/src/netzip.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    13702 2023-06-13 16:29:16.000000 netzip-0.2/src/netzip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 16:29:40.834752 netzip-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1603 2023-06-13 16:29:16.000000 netzip-0.2/tests/test_netzip.py
```

### Comparing `netzip-0.1/.github/workflows/release.yml` & `netzip-0.2/.github/workflows/release.yml`

 * *Files 24% similar despite different names*

```diff
@@ -7,34 +7,27 @@
 
 jobs:
   release:
     runs-on: ubuntu-latest
 
     environment:
       name: release
-      url: https://pypi.org/p/netzip
+      url: https://pypi.org/project/netzip/
 
     permissions:
       id-token: write
 
     steps:
-      - name: Checkout code
+      - name: Checkout
         uses: actions/checkout@v3
 
-      - name: Setup Nox
-        uses: wntrblm/nox@2022.8.7
-        with:
-         python-versions: "3.8, 3.9, 3.10, 3.11"
-
-      - name: Install dependencies
-        run: |
-          python -m pip install --upgrade pip
-          python -m pip install nox build
+      - name: Install Nox
+        run: pipx install nox
 
       - name: Run tests
         run: nox --session tests
 
       - name: Build packages
-        run: python -m build
+        run: nox --session build
 
       - name: Publish to PyPI
         uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `netzip-0.1/LICENSE.txt` & `netzip-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `netzip-0.1/pyproject.toml` & `netzip-0.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,12 +15,12 @@
 
 [tool.setuptools.packages.find]
 where = ["src"]
 
 [tool.setuptools_scm]
 
 [tool.pytest.ini_options]
-addopts = "-ra --quiet"
+addopts = "-rfEP --quiet"
 testpaths = ["tests"]
 
 [tool.isort]
 profile = "black"
```

### Comparing `netzip-0.1/src/netzip.py` & `netzip-0.2/src/netzip.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,55 +2,61 @@
 
 See https://pkware.cachefly.net/webdocs/casestudies/APPNOTE.TXT
 for the ZIP file format specification.
 """
 
 import collections.abc
 import io
+import itertools
 import struct
 import zlib
 from dataclasses import dataclass
-from typing import ClassVar, Dict, Iterable, Tuple
+from typing import Any, ClassVar, Dict, Iterable, Tuple
 
 _MULTI_DISK_ERROR = ValueError("multi-disk ZIP archives are not supported")
 _ENCRYPTED_ERROR = ValueError("encrypted ZIP archives are not supported")
 _COMPRESSED_ERROR = ValueError("compressed ZIP archives are not supported")
-_ZIP64_ERROR = NotImplementedError("ZIP64 archives are not implemented yet")
 
 
 def _validate_signature(name: str, *, want: bytes, got: bytes) -> None:
     """Validate a ZIP file signature."""
     if want != got:
         raise ValueError(f"invalid {name} signature: want {want}, got {got}")
 
 
-def _fullread(buf, size: int = -1) -> bytes:
-    """Read exactly `size` bytes from `buf`, or raise EOFError.
-
-    If size is negative, read until EOF.
-    """
+def _fullread(buf, size: int) -> bytes:
+    """Read exactly `size` bytes from `buf`, or raise EOFError."""
     data = buf.read(size)
-    if size >= 0 and len(data) != size:
+    if len(data) != size:
         raise EOFError(f"requested {size} bytes, got {len(data)}")
     return data
 
 
-def _unpackbuf(format, buf) -> Tuple:
+def _unpackbuf(format: str, buf) -> Tuple:
     """Unpack a struct from buffer.
 
     Read the required number of bytes from `buf` and unpack them according to `format`.
     """
     return struct.unpack(format, _fullread(buf, struct.calcsize(format)))
 
 
 # region File format data structures
 
 
-## Fields in the following data structures are separated into two groups:
-## fixed-size and variable-size ones.
+# The following data structures are defined in the ZIP file format specification.
+
+# Some fields are omitted because they are not used by this implementation, and parsing
+# them would add extra I/O, which is undesirable for network access.
+
+# Each data structure has a `read` classmethod that reads the structure from a buffer.
+# The `validate` method checks that the structure is valid and can be used by this
+# implementation.
+
+# Fields in all data structures have default values because they cannot be created
+# in a single step: almost all structures contain some variable-length fields.
 
 
 @dataclass
 class _EocdRecord:
     """End of central directory record."""
 
     signature: bytes = b""
@@ -66,36 +72,142 @@
 
     SIGNATURE: ClassVar[bytes] = b"PK\x05\x06"
     STRUCT_FORMAT: ClassVar[str] = "<4s4H2LH"
     MAX_SIZE: ClassVar[int] = struct.calcsize(STRUCT_FORMAT) + 0xFFFF
 
     @classmethod
     def read(cls, buf) -> "_EocdRecord":
-        """Read an end of central directory record from `buf`."""
         inst = cls(*_unpackbuf(cls.STRUCT_FORMAT, buf))
         inst.comment = _fullread(buf, inst.comment_size)
         inst.validate()
         return inst
 
     def validate(self) -> None:
         _validate_signature(
-            "end of central directory", want=self.SIGNATURE, got=self.signature
+            "end of central directory record", want=self.SIGNATURE, got=self.signature
         )
         if (
             self.this_disk_number != 0
             or self.start_disk_number != 0
             or self.this_record_count != self.total_record_count
         ):
             raise _MULTI_DISK_ERROR
-        if (
-            self.total_record_count == 0xFFFF
+
+    def is_zip64(self) -> bool:
+        return (
+            self.this_disk_number == 0xFFFF
+            or self.start_disk_number == 0xFFFF
+            or self.this_record_count == 0xFFFF
+            or self.total_record_count == 0xFFFF
             or self.central_directory_size == 0xFFFFFFFF
             or self.central_directory_offset == 0xFFFFFFFF
+        )
+
+
+@dataclass
+class _Zip64EocdRecord:
+    """End of central directory record for ZIP64 archives."""
+
+    signature: bytes = b""
+    size: int = 0
+    version_created: int = 0
+    version_needed: int = 0
+    this_disk_number: int = 0
+    start_disk_number: int = 0
+    this_record_count: int = 0
+    total_record_count: int = 0
+    central_directory_size: int = 0
+    central_directory_offset: int = 0
+
+    SIGNATURE: ClassVar[bytes] = b"PK\x06\x06"
+    STRUCT_FORMAT: ClassVar[str] = "<4sQ2H2L4Q"
+    SIZE: ClassVar[int] = struct.calcsize(STRUCT_FORMAT)
+
+    @classmethod
+    def read(cls, buf) -> "_Zip64EocdRecord":
+        inst = cls(*_unpackbuf(cls.STRUCT_FORMAT, buf))
+        inst.validate()
+        return inst
+
+    def validate(self) -> None:
+        _validate_signature(
+            "ZIP64 end of central directory record",
+            want=self.SIGNATURE,
+            got=self.signature,
+        )
+        if (
+            self.this_disk_number != 0
+            or self.start_disk_number != 0
+            or self.this_record_count != self.total_record_count
         ):
-            raise _ZIP64_ERROR
+            raise _MULTI_DISK_ERROR
+
+
+@dataclass
+class _Zip64EocdLocator:
+    """Location of the ZIP64 end of central directory."""
+
+    signature: bytes = b""
+    eocd_disk_number: int = 0
+    eocd_offset: int = 0
+    total_disk_count: int = 0
+
+    SIGNATURE: ClassVar[bytes] = b"PK\x06\x07"
+    STRUCT_FORMAT: ClassVar[str] = "<4sLQL"
+    SIZE: ClassVar[int] = struct.calcsize(STRUCT_FORMAT)
+
+    @classmethod
+    def read(cls, buf) -> "_Zip64EocdLocator":
+        inst = cls(*_unpackbuf(cls.STRUCT_FORMAT, buf))
+        inst.validate()
+        return inst
+
+    def validate(self) -> None:
+        _validate_signature(
+            "ZIP64 end of central directory locator",
+            want=self.SIGNATURE,
+            got=self.signature,
+        )
+        if self.eocd_disk_number != 0 or self.total_disk_count != 1:
+            raise _MULTI_DISK_ERROR
+
+
+def _read_zip64_extinfo(block) -> Dict[str, Any]:
+    """Read ZIP64 extended information extra field from the 'extra' field block.
+
+    Return dict with values found in the extra block, and keys corresponding
+    to field names in _CdFileHeader and _LocalFileHeader.
+    """
+    buf = io.BytesIO(block)
+
+    while buf.tell() < len(block):
+        header, size = _unpackbuf("<2H", buf)
+        if header != 0x0001:
+            buf.seek(size, io.SEEK_CUR)
+            continue
+
+        formats = dict(
+            uncompressed_size="<Q",
+            compressed_size="<Q",
+            local_header_offset="<Q",
+            disk_number="<L",
+        )
+        if size not in itertools.accumulate(map(struct.calcsize, formats.values())):
+            raise ValueError("invalid ZIP64 extended information extra field")
+
+        fields = {}
+        ext_block = _fullread(buf, size)
+        ext_buf = io.BytesIO(ext_block)
+        for name, fmt in formats.items():
+            if ext_buf.tell() >= len(ext_block):
+                break
+            fields[name] = _unpackbuf(fmt, ext_buf)[0]
+        return fields
+
+    return {}
 
 
 @dataclass
 class _CdFileHeader:
     """File metadata that is stored in the central directory."""
 
     signature: bytes = b""
@@ -122,37 +234,43 @@
     SIGNATURE: ClassVar[bytes] = b"PK\x01\x02"
     STRUCT_FORMAT: ClassVar[str] = "<4s6H3L5H2L"
 
     @classmethod
     def read(cls, buf) -> "_CdFileHeader":
         inst = cls(*_unpackbuf(cls.STRUCT_FORMAT, buf))
         inst.filename = _fullread(buf, inst.filename_size)
-        _fullread(buf, inst.extra_size)
+        extra_block = _fullread(buf, inst.extra_size)
         inst.comment = _fullread(buf, inst.comment_size)
+        if inst.is_zip64():
+            for name, value in _read_zip64_extinfo(extra_block).items():
+                setattr(inst, name, value)
         inst.validate()
         return inst
 
     def validate(self) -> None:
         _validate_signature(
-            "central directory ", want=self.SIGNATURE, got=self.signature
+            "central directory file header", want=self.SIGNATURE, got=self.signature
         )
         if self.flags & 0x0001:
             raise _ENCRYPTED_ERROR
         if (
             self.compression_method != 0
             or self.compressed_size != self.uncompressed_size
         ):
             raise _COMPRESSED_ERROR
         if self.disk_number != 0:
             raise _MULTI_DISK_ERROR
-        if (
-            self.uncompressed_size == 0xFFFFFFFF
+
+    def is_zip64(self) -> bool:
+        return (
+            self.compressed_size == 0xFFFFFFFF
+            or self.uncompressed_size == 0xFFFFFFFF
+            or self.disk_number == 0xFFFF
             or self.local_header_offset == 0xFFFFFFFF
-        ):
-            raise _ZIP64_ERROR
+        )
 
 
 @dataclass
 class _LocalFileHeader:
     """File metadata that precedes the actual file data."""
 
     signature: bytes = b""
@@ -173,31 +291,37 @@
     STRUCT_FORMAT: ClassVar[str] = "<4s5H3L2H"
     MAX_SIZE: ClassVar[int] = struct.calcsize(STRUCT_FORMAT) + 2 * 0xFFFF
 
     @classmethod
     def read(cls, buf) -> "_LocalFileHeader":
         inst = cls(*_unpackbuf(cls.STRUCT_FORMAT, buf))
         inst.filename = _fullread(buf, inst.filename_size)
-        _fullread(buf, inst.extra_size)
+        extra_block = _fullread(buf, inst.extra_size)
+        if inst.is_zip64():
+            for name, value in _read_zip64_extinfo(extra_block).items():
+                setattr(inst, name, value)
         inst.validate()
         return inst
 
     def validate(self) -> None:
         _validate_signature(
             "local file header", want=self.SIGNATURE, got=self.signature
         )
         if self.flags & 0x0001:
             raise _ENCRYPTED_ERROR
         if (
             self.compression_method != 0
             or self.compressed_size != self.uncompressed_size
         ):
             raise _COMPRESSED_ERROR
-        if self.uncompressed_size == 0xFFFFFFFF:
-            raise _ZIP64_ERROR
+
+    def is_zip64(self) -> bool:
+        return (
+            self.compressed_size == 0xFFFFFFFF or self.uncompressed_size == 0xFFFFFFFF
+        )
 
 
 # endregion
 
 
 @dataclass
 class _FileInfo:
@@ -230,41 +354,45 @@
             )
         if buf.read(1):
             raise ValueError("central directory contains more data than expected")
         return d
 
     def validate_header(self, header: _LocalFileHeader) -> None:
         """Validate against local file header."""
-        if self.size != header.uncompressed_size:
-            raise ValueError("size mismatch")
-        if self.crc32 != header.crc32:
-            raise ValueError("CRC32 mismatch")
-
-    def validate_payload(self, payload: bytes) -> None:
-        """Validate against file payload."""
-        if self.size != len(payload):
-            raise ValueError("size mismatch")
-        if self.crc32 != zlib.crc32(payload):
-            raise ValueError("CRC32 mismatch")
+        if self.size != header.uncompressed_size or self.crc32 != header.crc32:
+            raise ValueError(
+                "local file header and central directory file header contain different metadata"
+            )
 
 
 def _read_metadata(source: io.BufferedIOBase) -> Dict[bytes, _FileInfo]:
     """Parse ZIP metadata from source.
 
     Returns:
         Mapping of file names to file info records.
     """
-    source.seek(-_EocdRecord.MAX_SIZE, io.SEEK_END)
+    source.seek(0, io.SEEK_END)
+    size = source.tell()
+
+    source.seek(max(0, size - _EocdRecord.MAX_SIZE - _Zip64EocdLocator.SIZE))
     eocd_block = source.read()
 
     eocd_start = eocd_block.rfind(_EocdRecord.SIGNATURE)
     if eocd_start < 0:
         raise ValueError("end of central directory record not found")
     eocd = _EocdRecord.read(io.BytesIO(eocd_block[eocd_start:]))
 
+    if eocd.is_zip64():
+        loc_block = eocd_block[max(0, eocd_start - _Zip64EocdLocator.SIZE) : eocd_start]
+        loc = _Zip64EocdLocator.read(io.BytesIO(loc_block))
+
+        source.seek(loc.eocd_offset)
+        eocd64_block = source.read(_Zip64EocdRecord.SIZE)
+        eocd = _Zip64EocdRecord.read(io.BytesIO(eocd64_block))
+
     source.seek(eocd.central_directory_offset)
     cd_block = source.read(eocd.central_directory_size)
 
     return _FileInfo.readmany(io.BytesIO(cd_block), eocd.total_record_count)
 
 
 class ZipReader(collections.abc.Mapping):
@@ -283,16 +411,17 @@
         """Return contents of a file with the given name."""
         info = self._files[name]
 
         self._source.seek(info.offset)
         buf = io.BytesIO(self._source.read(info.max_block_size))
 
         info.validate_header(_LocalFileHeader.read(buf))
-        data = buf.read(info.size)
-        info.validate_payload(data)
+        data = _fullread(buf, info.size)
+        if info.crc32 != zlib.crc32(data):
+            raise ValueError("CRC32 mismatch")
         return data
 
     def __iter__(self) -> Iterable[bytes]:
         """Return file names in this archive, in unspecified order."""
         return iter(self._files)
 
     def __len__(self) -> int:
```

