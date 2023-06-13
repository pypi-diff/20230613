# Comparing `tmp/pep440_rs-0.3.7.tar.gz` & `tmp/pep440_rs-0.3.9.tar.gz`

## Comparing `pep440_rs-0.3.7.tar` & `pep440_rs-0.3.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 pep440_rs-0.3.7/Cargo.toml
--rw-r--r--   0      501       20      901 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/Changelog.md
--rw-r--r--   0      501       20    10173 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/License-Apache
--rw-r--r--   0      501       20     1293 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/License-BSD
--rw-r--r--   0      501       20     2981 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/Readme.md
--rw-r--r--   0      501       20      312 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/pyproject.toml
--rw-r--r--   0      501       20     2105 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/python/Readme.md
--rw-r--r--   0      501       20     4043 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/src/lib.rs
--rw-r--r--   0      501       20    39609 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/src/version.rs
--rw-r--r--   0      501       20    42546 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/src/version_specifier.rs
--rw-r--r--   0      501       20    10916 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/Cargo.lock
--rw-r--r--   0      501       20     1131 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/python/pep440_rs/__init__.pyi
--rw-r--r--   0      501       20      534 2023-05-07 15:06:08.000000 pep440_rs-0.3.7/python/pep440_rs/__init__.py
--rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 pep440_rs-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0      880 1970-01-01 00:00:00.000000 pep440_rs-0.3.9/Cargo.toml
+-rw-r--r--   0      501       20     1033 2023-05-08 17:05:18.000000 pep440_rs-0.3.9/Changelog.md
+-rw-r--r--   0      501       20    10173 2023-05-08 17:05:18.000000 pep440_rs-0.3.9/License-Apache
+-rw-r--r--   0      501       20     1293 2023-05-08 17:05:18.000000 pep440_rs-0.3.9/License-BSD
+-rw-r--r--   0      501       20     2981 2023-05-08 17:05:18.000000 pep440_rs-0.3.9/Readme.md
+-rw-r--r--   0      501       20      312 2023-05-08 17:05:18.000000 pep440_rs-0.3.9/pyproject.toml
+-rw-r--r--   0      501       20     2105 2023-05-08 17:05:18.000000 pep440_rs-0.3.9/python/Readme.md
+-rw-r--r--   0      501       20     4043 2023-05-08 17:05:18.000000 pep440_rs-0.3.9/src/lib.rs
+-rw-r--r--   0      501       20    39609 2023-05-08 17:05:18.000000 pep440_rs-0.3.9/src/version.rs
+-rw-r--r--   0      501       20    42546 2023-05-08 17:05:18.000000 pep440_rs-0.3.9/src/version_specifier.rs
+-rw-r--r--   0      501       20    10916 2023-05-08 17:05:18.000000 pep440_rs-0.3.9/Cargo.lock
+-rw-r--r--   0      501       20     1131 2023-05-08 17:05:18.000000 pep440_rs-0.3.9/python/pep440_rs/__init__.pyi
+-rw-r--r--   0      501       20      534 2023-05-08 17:05:18.000000 pep440_rs-0.3.9/python/pep440_rs/__init__.py
+-rw-r--r--   0        0        0     2410 1970-01-01 00:00:00.000000 pep440_rs-0.3.9/PKG-INFO
```

### Comparing `pep440_rs-0.3.7/Cargo.toml` & `pep440_rs-0.3.9/Cargo.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pep440_rs"
-version = "0.3.7"
+version = "0.3.9"
 description = "A library for python version numbers and specifiers, implementing PEP 440"
 edition = "2021"
 include = ["/src", "Changelog.md", "License-Apache", "License-BSD", "Readme.md", "pyproject.toml"]
 # Same license as pypa/packaging where the tests are from
 license = "Apache-2.0 OR BSD-2-Clause"
 repository = "https://github.com/konstin/pep440-rs"
 readme = "Readme.md"
```

### Comparing `pep440_rs-0.3.7/License-Apache` & `pep440_rs-0.3.9/License-Apache`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.7/License-BSD` & `pep440_rs-0.3.9/License-BSD`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.7/Readme.md` & `pep440_rs-0.3.9/Readme.md`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.7/python/Readme.md` & `pep440_rs-0.3.9/python/Readme.md`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.7/src/lib.rs` & `pep440_rs-0.3.9/src/lib.rs`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.7/src/version.rs` & `pep440_rs-0.3.9/src/version.rs`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.7/src/version_specifier.rs` & `pep440_rs-0.3.9/src/version_specifier.rs`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.7/Cargo.lock` & `pep440_rs-0.3.9/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -45,17 +45,17 @@
 name = "lazy_static"
 version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e2abad23fbc42b3700f2f279844dc832adb2b2eb069b2df918f455c4e18cc646"
 
 [[package]]
 name = "libc"
-version = "0.2.143"
+version = "0.2.144"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "edc207893e85c5d6be840e969b496b53d94cec8be2d501b214f50daa97fa8024"
+checksum = "2b00cc1c228a6782d0f076e7b232802e0c5689d41bb5df366f2a6b6621cfdfe1"
 
 [[package]]
 name = "lock_api"
 version = "0.4.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
 dependencies = [
@@ -105,15 +105,15 @@
  "redox_syscall",
  "smallvec",
  "windows-sys",
 ]
 
 [[package]]
 name = "pep440_rs"
-version = "0.3.7"
+version = "0.3.9"
 dependencies = [
  "indoc 2.0.1",
  "lazy_static",
  "pyo3",
  "regex",
  "serde",
  "tracing",
@@ -193,17 +193,17 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.26"
+version = "1.0.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4424af4bf778aae2051a77b60283332f386554255d722233d09fbfc7e30da2fc"
+checksum = "8f4f29d145265ec1c483c7c654450edde0bfe043d3938d6972630663356d9500"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.2.16"
```

### Comparing `pep440_rs-0.3.7/python/pep440_rs/__init__.pyi` & `pep440_rs-0.3.9/python/pep440_rs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.7/python/pep440_rs/__init__.py` & `pep440_rs-0.3.9/python/pep440_rs/__init__.py`

 * *Files identical despite different names*

### Comparing `pep440_rs-0.3.7/PKG-INFO` & `pep440_rs-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pep440_rs
-Version: 0.3.7
+Version: 0.3.9
 Summary: A library for python version numbers and specifiers, implementing PEP 440
 License: Apache-2.0 OR BSD-2-Clause
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source Code, https://github.com/konstin/pep440-rs
 
 # PEP440 in rust
```

