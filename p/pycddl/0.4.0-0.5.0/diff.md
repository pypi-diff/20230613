# Comparing `tmp/pycddl-0.4.0.tar.gz` & `tmp/pycddl-0.5.0.tar.gz`

## Comparing `pycddl-0.4.0.tar` & `pycddl-0.5.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0      679 1970-01-01 00:00:00.000000 pycddl-0.4.0/Cargo.toml
--rw-rw-rw-   0        0        0      239 2023-01-05 23:15:33.000000 pycddl-0.4.0/.bumpversion.cfg
--rw-rw-rw-   0        0        0       46 2023-01-05 23:15:33.000000 pycddl-0.4.0/.dir-locals.el
--rw-rw-rw-   0        0        0       50 2023-01-05 23:15:33.000000 pycddl-0.4.0/.flake8
--rw-rw-rw-   0        0        0       31 2023-01-05 23:15:33.000000 pycddl-0.4.0/.gitignore
--rw-rw-rw-   0        0        0     2148 2023-01-05 23:15:33.000000 pycddl-0.4.0/.gitlab-ci.yml
--rw-rw-rw-   0        0        0     1079 2023-01-05 23:15:33.000000 pycddl-0.4.0/LICENSE
--rw-rw-rw-   0        0        0       58 2023-01-05 23:15:33.000000 pycddl-0.4.0/Makefile
--rw-rw-rw-   0        0        0     2156 2023-01-05 23:15:33.000000 pycddl-0.4.0/README.md
--rw-rw-rw-   0        0        0      795 2023-01-05 23:15:33.000000 pycddl-0.4.0/RELEASE.md
--rw-rw-rw-   0        0        0      116 2023-01-05 23:15:33.000000 pycddl-0.4.0/build.rs
--rw-rw-rw-   0        0        0     1243 2023-01-05 23:15:33.000000 pycddl-0.4.0/pyproject.toml
--rw-rw-rw-   0        0        0      773 2023-01-05 23:15:33.000000 pycddl-0.4.0/pysrc/pycddl/__init__.py
--rw-rw-rw-   0        0        0       45 2023-01-05 23:15:33.000000 pycddl-0.4.0/requirements-dev.txt
--rw-rw-rw-   0        0        0       63 2023-01-05 23:15:33.000000 pycddl-0.4.0/rust-toolchain.toml
--rw-rw-rw-   0        0        0     3608 2023-01-05 23:15:33.000000 pycddl-0.4.0/src/lib.rs
--rw-rw-rw-   0        0        0        0 2023-01-05 23:15:33.000000 pycddl-0.4.0/tests/__init__.py
--rw-rw-rw-   0        0        0      616 2023-01-05 23:15:33.000000 pycddl-0.4.0/tests/test_benchmarks.py
--rw-rw-rw-   0        0        0     6456 2023-01-05 23:15:33.000000 pycddl-0.4.0/tests/test_cddl.py
--rw-rw-rw-   0        0        0      820 2023-01-05 23:15:33.000000 pycddl-0.4.0/tests/utils.py
--rw-rw-rw-   0        0        0    33814 2023-01-05 23:15:33.000000 pycddl-0.4.0/Cargo.lock
--rw-r--r--   0        0        0     2469 1970-01-01 00:00:00.000000 pycddl-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0      678 1970-01-01 00:00:00.000000 pycddl-0.5.0/Cargo.toml
+-rw-rw-rw-   0        0        0      239 2023-06-13 21:10:07.000000 pycddl-0.5.0/.bumpversion.cfg
+-rw-rw-rw-   0        0        0       46 2023-06-13 21:10:07.000000 pycddl-0.5.0/.dir-locals.el
+-rw-rw-rw-   0        0        0       50 2023-06-13 21:10:07.000000 pycddl-0.5.0/.flake8
+-rw-rw-rw-   0        0        0       31 2023-06-13 21:10:07.000000 pycddl-0.5.0/.gitignore
+-rw-rw-rw-   0        0        0     2457 2023-06-13 21:10:07.000000 pycddl-0.5.0/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0     1079 2023-06-13 21:10:07.000000 pycddl-0.5.0/LICENSE
+-rw-rw-rw-   0        0        0       58 2023-06-13 21:10:07.000000 pycddl-0.5.0/Makefile
+-rw-rw-rw-   0        0        0     2223 2023-06-13 21:10:07.000000 pycddl-0.5.0/README.md
+-rw-rw-rw-   0        0        0      795 2023-06-13 21:10:07.000000 pycddl-0.5.0/RELEASE.md
+-rw-rw-rw-   0        0        0      116 2023-06-13 21:10:07.000000 pycddl-0.5.0/build.rs
+-rw-rw-rw-   0        0        0     1352 2023-06-13 21:10:07.000000 pycddl-0.5.0/pyproject.toml
+-rw-rw-rw-   0        0        0      773 2023-06-13 21:10:07.000000 pycddl-0.5.0/pysrc/pycddl/__init__.py
+-rw-rw-rw-   0        0        0       45 2023-06-13 21:10:07.000000 pycddl-0.5.0/requirements-dev.txt
+-rw-rw-rw-   0        0        0       63 2023-06-13 21:10:07.000000 pycddl-0.5.0/rust-toolchain.toml
+-rw-rw-rw-   0        0        0     3735 2023-06-13 21:10:07.000000 pycddl-0.5.0/src/lib.rs
+-rw-rw-rw-   0        0        0        0 2023-06-13 21:10:07.000000 pycddl-0.5.0/tests/__init__.py
+-rw-rw-rw-   0        0        0      616 2023-06-13 21:10:07.000000 pycddl-0.5.0/tests/test_benchmarks.py
+-rw-rw-rw-   0        0        0     6456 2023-06-13 21:10:07.000000 pycddl-0.5.0/tests/test_cddl.py
+-rw-rw-rw-   0        0        0      820 2023-06-13 21:10:07.000000 pycddl-0.5.0/tests/utils.py
+-rw-rw-rw-   0        0        0    32557 2023-06-13 21:10:07.000000 pycddl-0.5.0/Cargo.lock
+-rw-r--r--   0        0        0     2536 1970-01-01 00:00:00.000000 pycddl-0.5.0/PKG-INFO
```

### Comparing `pycddl-0.4.0/Cargo.toml` & `pycddl-0.5.0/Cargo.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pycddl"
-version = "0.4.0"  # pycddl version, for bumpversion
+version = "0.5.0"  # pycddl version, for bumpversion
 edition = "2021"
 license = "MIT"
 authors = ["Tahoe-LAFS project"]
 description = "Validate CBOR documents using CDDL schema language"
 homepage = "https://gitlab.com/tahoe-lafs/pycddl"
 readme = "README.md"
 
@@ -13,15 +13,15 @@
 [lib]
 name = "pycddl"
 crate-type = ["cdylib"]
 
 [dependencies]
 cddl = "0.9"
 ciborium = "0.2"
-ouroboros = "0.15"
-pyo3 = { version = "0.17", features = ["extension-module"] }
+self_cell = "1.0"
+pyo3 = { version = "0.19", features = ["extension-module"] }
 
 [build-dependencies]
-pyo3-build-config = { version = "0.17", features = ["resolve-config"] }
+pyo3-build-config = { version = "0.19", features = ["resolve-config"] }
 
 [profile.release]
 lto = "thin"
```

### Comparing `pycddl-0.4.0/.gitlab-ci.yml` & `pycddl-0.5.0/.gitlab-ci.yml`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 stages:
   - test
   - release
 
 # For tagged versions, upload to PyPI
 release:
   stage: release
-  image: python:3.9
+  image: python:3.11
   dependencies:
     - linux
     - macos
     - windows
   only:
     - tags
   script:
@@ -24,15 +24,15 @@
     - mkdir -p wheelhouse
     - mv target/wheels/*.tar.gz wheelhouse/
     # Upload:
     - maturin upload --username "__token__" wheelhouse/*
 
 
 linux:
-  image: python:3.9
+  image: python:3.11
   only:
     - main
     - merge_requests
     - tags
   stage: test
 
   # Run Docker, so cibuildwheel can use it.
@@ -40,57 +40,68 @@
     - name: docker:dind
 
   # Tell Docker client where to find it.
   variables:
     DOCKER_HOST: tcp://docker:2375/
     DOCKER_DRIVER: overlay2
     DOCKER_TLS_CERTDIR: ""
-    CIBW_BUILD: "pp3*-manylinux_x86_64 cp3*_x86_64"
-    CIBW_SKIP: "pp37*"
   script:
     - curl -sSL https://get.docker.com/ | sh
-    - python -m pip install cibuildwheel==2.11.3
+    - python -m pip install cibuildwheel==2.13.1
     - cibuildwheel --output-dir wheelhouse
 
   artifacts:
     paths:
       - wheelhouse/
 
 
 # https://docs.gitlab.com/ee/ci/runners/saas/macos_saas_runner.html
 macos:
+  only:
+    - main
+    - merge_requests
+    - tags
+  stage: test
   tags:
-    - shared-macos-amd64
-  image: macos-11-xcode-12
+    - saas-macos-medium-m1
+  image: macos-12-xcode-14
 
   variables:
-    CIBW_BUILD: "cp3*"
-    MACOSX_DEPLOYMENT_TARGET: "10.15"
+    MACOSX_DEPLOYMENT_TARGET: "11.0"
+    ARCHFLAGS: " -arch x86_64 -arch arm64"
+    # Can't be set in pyproject.toml, alas
+    CIBW_ARCHS_MACOS: "universal2"
 
   script:
     - python -m pip install --upgrade pip
-    - python -m pip install cibuildwheel
+    - python -m pip install cibuildwheel==2.13.1
     - python -m cibuildwheel --output-dir wheelhouse
 
   artifacts:
     paths:
       - wheelhouse/
 
 windows:
+  only:
+    - main
+    - merge_requests
+    - tags
   stage: test
   tags:
     - shared-windows
     - windows
     - windows-1809
 
-  variables:
-    CIBW_BUILD: "cp3*"
-
   script:
+    - Import-Module "$env:ChocolateyInstall\helpers\chocolateyProfile.psm1"
     - choco install -y python --version=3.9.9
+    - choco install -y rustup.install
+    - refreshenv
+    - rustup toolchain install stable-msvc
     - refreshenv
-    - c:\python39\scripts\pip install cibuildwheel==2.10.2
+    - cargo --version
+    - c:\python39\scripts\pip install cibuildwheel==2.13.1
     - c:\python39\scripts\cibuildwheel --output-dir wheelhouse
 
   artifacts:
     paths:
       - wheelhouse/
```

### Comparing `pycddl-0.4.0/LICENSE` & `pycddl-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pycddl-0.4.0/README.md` & `pycddl-0.5.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -25,14 +25,19 @@
 In order to reduce memory usage, you can pass in any Python object that implements the buffer API and stores bytes, e.g. a `memoryview()` or a `mmap` object.
 
 **The passed-in object must be read-only, and the data must not change during validation!**
 If you mutate the data while validation is happening the result can be memory corruption or other [undefined behavior](https://stackoverflow.com/questions/18506029/can-undefined-behavior-erase-the-hard-drive#comment27209771_18506029).
 
 ## Release notes
 
+### 0.5.0
+
+* Support for ARM macOS.
+* Dropped Python 3.7 support.
+
 ### 0.4.1
 
 * Test fixes, with no user-relevant changes.
 
 ### 0.4.0
 
 * `validate_cbor()` now accepts read-only buffers, not just `bytes`. This is useful if you want to e.g. validate a large file, since you can `mmap()` it.
```

### Comparing `pycddl-0.4.0/RELEASE.md` & `pycddl-0.5.0/RELEASE.md`

 * *Files identical despite different names*

### Comparing `pycddl-0.4.0/pysrc/pycddl/__init__.py` & `pycddl-0.5.0/pysrc/pycddl/__init__.py`

 * *Files identical despite different names*

### Comparing `pycddl-0.4.0/src/lib.rs` & `pycddl-0.5.0/src/lib.rs`

 * *Files 6% similar despite different names*

```diff
@@ -1,55 +1,55 @@
 use cddl::{
     ast::CDDL,
     validator::{cbor::CBORValidator, Validator},
 };
-use ouroboros::self_referencing;
 use pyo3::{
     buffer::{PyBuffer, ReadOnlyCell},
     create_exception,
     exceptions::{PyException, PyTypeError, PyValueError},
     prelude::*,
 };
+use self_cell::self_cell;
 use std::mem::size_of;
 
+/// A CDDL schema that can be used to validate CBOR documents.
 #[pyclass]
 struct Schema {
-    // We need to do a song-and-dance with an inner struct because #[pyclass]
-    // doesn't like generic classes, and #[pyclass] and #[self_referencing]
-    // conflict.
+    // We need to do a song-and-dance with an inner struct so we don't have to
+    // worry about how the self_cell! macro and PyO3 macros interact.
     inner: SchemaImpl,
 }
 
-#[self_referencing]
-struct SchemaImpl {
-    // Keep around the underlying data.
-    schema_string: String,
-    // The parsed schema:
-    #[borrows(schema_string)]
-    #[covariant]
-    schema: CDDL<'this>,
+self_cell! {
+    struct SchemaImpl {
+        // Keep around the underlying data.
+        owner: String,
+
+        // The parsed schema:
+        #[covariant]
+        dependent: CDDL,
+    }
 }
 
 #[pymethods]
 impl Schema {
+    /// Create a new ``Schema`` given a string with the CDDL specification.
     #[new]
     fn new(schema_string: String) -> PyResult<Self> {
-        let inner = SchemaImplTryBuilder {
-            schema_string,
-            schema_builder: |s: &String| CDDL::from_slice(s.as_bytes()),
-        }
-        .try_build()
-        .map_err(PyValueError::new_err)?;
+        let inner = SchemaImpl::try_new(schema_string, |s: &String| CDDL::from_slice(s.as_bytes()))
+            .map_err(PyValueError::new_err)?;
         Ok(Schema { inner })
     }
 
     fn __repr__(&self) -> String {
-        format!(r#"Schema("""{}""")"#, self.inner.borrow_schema_string())
+        format!(r#"Schema("""{}""")"#, self.inner.borrow_owner())
     }
 
+    /// Validate a CBOR document in string format, throwing a ``ValidateError``
+    /// if validation failed.
     fn validate_cbor(&self, py: Python<'_>, cbor: &PyAny) -> PyResult<()> {
         let buffer = PyBuffer::<u8>::get(cbor)?;
         // PyPy has weird issues with this flag.
         if !cfg!(PyPy) && !buffer.readonly() {
             return Err(PyValueError::new_err("Must be a read-only byte buffer (and you should never mutate it during validation)"));
         }
         let slice = buffer
@@ -72,15 +72,15 @@
         let (before, cbor, after) = unsafe { slice.align_to::<u8>() };
         assert_eq!(before.len(), 0);
         assert_eq!(after.len(), 0);
 
         let validate = || {
             let document_size = cbor.len();
             let cbor: ciborium::value::Value = ciborium::de::from_reader(cbor)?;
-            let schema = self.inner.borrow_schema();
+            let schema = self.inner.borrow_dependent();
             let mut cv = CBORValidator::new(schema, cbor, None);
             if document_size > 10 * 1024 {
                 // For larger documents, parsing can get expensive, so release
                 // the GIL to enable parallelism.
                 Python::allow_threads(py, || cv.validate())?;
             } else {
                 cv.validate()?;
```

### Comparing `pycddl-0.4.0/tests/test_benchmarks.py` & `pycddl-0.5.0/tests/test_benchmarks.py`

 * *Files identical despite different names*

### Comparing `pycddl-0.4.0/tests/test_cddl.py` & `pycddl-0.5.0/tests/test_cddl.py`

 * *Files identical despite different names*

### Comparing `pycddl-0.4.0/tests/utils.py` & `pycddl-0.5.0/tests/utils.py`

 * *Files identical despite different names*

### Comparing `pycddl-0.4.0/Cargo.lock` & `pycddl-0.5.0/Cargo.lock`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,12 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
-name = "Inflector"
-version = "0.11.4"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fe438c63458706e03479442743baae6c88256498e6431708f6dfc520a26515d3"
-
-[[package]]
 name = "abnf"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "33741baa462d86e43fdec5e8ffca7c6ac82847ad06cbfb382c1bdbf527de9e6b"
 dependencies = [
  "abnf-core",
  "nom",
@@ -36,18 +30,18 @@
  "abnf",
  "indexmap",
  "itertools",
  "pretty",
 ]
 
 [[package]]
-name = "aliasable"
-version = "0.1.3"
+name = "android-tzdata"
+version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "250f629c0161ad8107cf89319e990051fae62832fd343083bea452d93e2205fd"
+checksum = "e999941b234f3131b00bc13c22d06e8c5ff726d1b6318ac7eb276997bbb4fef0"
 
 [[package]]
 name = "android_system_properties"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
@@ -102,32 +96,32 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "block-buffer"
-version = "0.10.3"
+version = "0.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69cce20737498f97b993470a6e536b8523f0af7892a4f928cceb1ac5e52ebe7e"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
 dependencies = [
  "generic-array",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.11.1"
+version = "3.13.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "572f695136211188308f16ad2ca5c851a712c464060ae6974944458eb83880ba"
+checksum = "a3e2c3daef883ecc1b5d58c15adae93470a91d425f3532ba1695849656af3fc1"
 
 [[package]]
 name = "cc"
-version = "1.0.78"
+version = "1.0.79"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a20104e2335ce8a659d6dd92a51a767a0c062599c73b343fd152cb401e828c3d"
+checksum = "50d30906286121d95be3d479533b458f87493b30a4b5f79a607db8f5d11aa91f"
 
 [[package]]
 name = "cddl"
 version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "286a21bdd91f4cab45c26ae7310f73aedf1e8f6fe21e210d220c449991c7fcf4"
 dependencies = [
@@ -145,15 +139,15 @@
  "hexf-parse",
  "itertools",
  "lexical-core",
  "log",
  "pest_meta",
  "pest_vm",
  "regex",
- "regex-syntax",
+ "regex-syntax 0.6.29",
  "serde",
  "serde-wasm-bindgen",
  "serde_json",
  "simplelog",
  "uriparse",
  "wasm-bindgen",
 ]
@@ -162,82 +156,82 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "chrono"
-version = "0.4.23"
+version = "0.4.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "16b0a3d9ed01224b22057780a37bb8c5dbfe1be8ba48678e7bf57ec4b385411f"
+checksum = "ec837a71355b28f6556dbd569b37b3f363091c0bd4b2e735674521b4c5fd9bc5"
 dependencies = [
+ "android-tzdata",
  "iana-time-zone",
  "js-sys",
- "num-integer",
  "num-traits",
  "time",
  "wasm-bindgen",
  "winapi",
 ]
 
 [[package]]
 name = "ciborium"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b0c137568cc60b904a7724001b35ce2630fd00d5d84805fbb608ab89509d788f"
+checksum = "effd91f6c78e5a4ace8a5d3c0b6bfaec9e2baaef55f3efc00e45fb2e477ee926"
 dependencies = [
  "ciborium-io",
  "ciborium-ll",
  "serde",
 ]
 
 [[package]]
 name = "ciborium-io"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "346de753af073cc87b52b2083a506b38ac176a44cfb05497b622e27be899b369"
+checksum = "cdf919175532b369853f5d5e20b26b43112613fd6fe7aee757e35f7a44642656"
 
 [[package]]
 name = "ciborium-ll"
-version = "0.2.0"
+version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "213030a2b5a4e0c0892b6652260cf6ccac84827b83a85a534e178e3906c4cf1b"
+checksum = "defaa24ecc093c77630e6c15e17c51f5e187bf35ee514f4e2d67baaa96dae22b"
 dependencies = [
  "ciborium-io",
  "half",
 ]
 
 [[package]]
 name = "clap"
-version = "3.2.23"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "71655c45cb9845d3270c9d6df84ebe72b4dad3c2ba3f7023ad47c144e4e473a5"
+checksum = "4ea181bf566f71cb9a5d17a59e1871af638180a18fb0035c92ae62b705207123"
 dependencies = [
  "atty",
  "bitflags",
  "clap_derive",
  "clap_lex",
  "indexmap",
  "once_cell",
  "strsim",
  "termcolor",
  "textwrap",
 ]
 
 [[package]]
 name = "clap_derive"
-version = "3.2.18"
+version = "3.2.25"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ea0c8bce528c4be4da13ea6fead8965e95b6073585a2f05204bd8f4119f82a65"
+checksum = "ae6371b8bdc8b7d3959e9cf7b22d4435ef3e79e138688421ec654acf8c81b008"
 dependencies = [
  "heck",
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "clap_lex"
 version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2850f2f5a82cbf437dd5af4d49848fbdfc27c157c3d010345776f952765261c5"
@@ -263,23 +257,23 @@
 dependencies = [
  "cfg-if",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.3"
+version = "0.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5827cebf4670468b8772dd191856768aedcb1b0278a04f989f7766351917b9dc"
+checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
 
 [[package]]
 name = "cpufeatures"
-version = "0.2.5"
+version = "0.2.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28d997bd5e24a5928dd43e46dc529867e207907fe0b239c3477d924f7f2ca320"
+checksum = "3e4c1eaa2012c47becbbad2ab175484c2a84d1185b566fb2cc5b8707343dfe58"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "crossterm"
 version = "0.25.0"
@@ -294,17 +288,17 @@
  "signal-hook",
  "signal-hook-mio",
  "winapi",
 ]
 
 [[package]]
 name = "crossterm_winapi"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2ae1b35a484aa10e07fe0638d02301c5ad24de82d310ccbd2f3693da5f09bf1c"
+checksum = "acdd7c62a3665c7f6830a51635d9ac9b23ed385797f70a83bb8bafe9c572ab2b"
 dependencies = [
  "winapi",
 ]
 
 [[package]]
 name = "crypto-common"
 version = "0.1.6"
@@ -312,95 +306,51 @@
 checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
 dependencies = [
  "generic-array",
  "typenum",
 ]
 
 [[package]]
-name = "cxx"
-version = "1.0.85"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5add3fc1717409d029b20c5b6903fc0c0b02fa6741d820054f4a2efa5e5816fd"
-dependencies = [
- "cc",
- "cxxbridge-flags",
- "cxxbridge-macro",
- "link-cplusplus",
-]
-
-[[package]]
-name = "cxx-build"
-version = "1.0.85"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4c87959ba14bc6fbc61df77c3fcfe180fc32b93538c4f1031dd802ccb5f2ff0"
-dependencies = [
- "cc",
- "codespan-reporting",
- "once_cell",
- "proc-macro2",
- "quote",
- "scratch",
- "syn",
-]
-
-[[package]]
-name = "cxxbridge-flags"
-version = "1.0.85"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "69a3e162fde4e594ed2b07d0f83c6c67b745e7f28ce58c6df5e6b6bef99dfb59"
-
-[[package]]
-name = "cxxbridge-macro"
-version = "1.0.85"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3e7e2adeb6a0d4a282e581096b06e1791532b7d576dcde5ccd9382acf55db8e6"
-dependencies = [
- "proc-macro2",
- "quote",
- "syn",
-]
-
-[[package]]
 name = "digest"
-version = "0.10.6"
+version = "0.10.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8168378f4e5023e7218c89c891c0fd8ecdb5e5e4f18cb78f38cf245dd021e76f"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
 dependencies = [
  "block-buffer",
  "crypto-common",
 ]
 
 [[package]]
 name = "displaydoc"
-version = "0.2.3"
+version = "0.2.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3bf95dc3f046b9da4f2d51833c0d3547d8564ef6910f5c1ed130306a75b92886"
+checksum = "487585f4d0c6655fe74905e2504d8ad6908e4db67f744eb140876906c2f3175d"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "either"
-version = "1.8.0"
+version = "1.8.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "90e5c1c8368803113bf0c9584fc495a58b86dc8a29edbf8fe877d21d9507e797"
+checksum = "7fcaabb2fef8c910e7f4c7ce9f67a1283a1715879a7c230ca9d6d1ae31f16d91"
 
 [[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "generic-array"
-version = "0.14.6"
+version = "0.14.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bff49e947297f3312447abdca79f45f4738097cc82b06e72054d2223f601f1b9"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
 dependencies = [
  "typenum",
  "version_check",
 ]
 
 [[package]]
 name = "half"
@@ -412,17 +362,17 @@
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 
 [[package]]
 name = "heck"
-version = "0.4.0"
+version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2540771e65fc8cb83cd6e8a237f70c319bd5c29f78ed1084ba5d50eeac86f7f9"
+checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
 version = "0.1.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "62b467343b94ba476dcb2500d242dadbb39557df889310ac77c5d99100aaac33"
 dependencies = [
@@ -433,72 +383,71 @@
 name = "hexf-parse"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dfa686283ad6dd069f105e5ab091b04c62850d3e4cf5d67debad1933f55023df"
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.53"
+version = "0.1.57"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "64c122667b287044802d6ce17ee2ddf13207ed924c712de9a66a5814d5b64765"
+checksum = "2fad5b825842d2b38bd206f3e81d6957625fd7f0a361e345c30e01a0ae2dd613"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
- "winapi",
+ "windows",
 ]
 
 [[package]]
 name = "iana-time-zone-haiku"
-version = "0.1.1"
+version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0703ae284fc167426161c2e3f1da3ea71d94b21bedbcc9494e92b28e334e3dca"
+checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
- "cxx",
- "cxx-build",
+ "cc",
 ]
 
 [[package]]
 name = "indexmap"
-version = "1.9.2"
+version = "1.9.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1885e79c1fc4b10f0e172c475f458b7f7b93061064d98c3293e98c5ba0c8b399"
+checksum = "bd070e393353796e801d209ad339e89596eb4c8d430d18ede6a1cced8fafbd99"
 dependencies = [
  "autocfg",
  "hashbrown",
 ]
 
 [[package]]
 name = "indoc"
-version = "1.0.8"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da2d6f23ffea9d7e76c53eee25dfb67bcd8fde7f1198b0855350698c9f07c780"
+checksum = "bfa799dd5ed20a7e349f3b4639aa80d74549c81716d9ec4f994c9b5815598306"
 
 [[package]]
 name = "itertools"
 version = "0.10.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "b0fd2260e829bddf4cb6ea802289de2f86d6a7a690192fbe91b3f46e0f2c8473"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.5"
+version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fad582f4b9e86b6caa621cabeb0963332d92eea04729ab12892c2533951e6440"
+checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.60"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "49409df3e3bf0856b916e2ceaca09ee28e6871cf7d9ce97a692cacfdb2a25a47"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lazy_static"
 version = "1.4.0"
@@ -567,192 +516,147 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.138"
+version = "0.2.146"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "db6d7e329c562c5dfab7a46a2afabc8b987ab9a4834c9d1ca04dc54c1546cef8"
-
-[[package]]
-name = "link-cplusplus"
-version = "1.0.8"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ecd207c9c713c34f95a097a5b029ac2ce6010530c7b49d7fea24d977dede04f5"
-dependencies = [
- "cc",
-]
+checksum = "f92be4933c13fd498862a9e02a3055f8a8d9c039ce33db97306fd5a6caa7f29b"
 
 [[package]]
 name = "lock_api"
-version = "0.4.9"
+version = "0.4.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "435011366fe56583b16cf956f9df0095b405b82d76425bc8981c0e22e60ec4df"
+checksum = "c1cc9717a20b1bb222f333e6a92fd32f7d8a18ddc5a3191a11af45dcbf4dcd16"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.17"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "abb12e687cfb44aa40f41fc3978ef76448f9b6038cad6aef4259d3c095a2382e"
-dependencies = [
- "cfg-if",
-]
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
 [[package]]
 name = "memoffset"
-version = "0.6.5"
+version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aa361d4faea93603064a027415f07bd8e1d5c88c9fbf68bf56a285428fd79ce"
+checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "minimal-lexical"
 version = "0.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "68354c5c6bd36d73ff3feceb05efa59b6acb7626617f4962be322a825e61f79a"
 
 [[package]]
 name = "mio"
-version = "0.8.5"
+version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5d732bc30207a6423068df043e3d02e0735b155ad7ce1a6f76fe2baa5b158de"
+checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
  "log",
  "wasi 0.11.0+wasi-snapshot-preview1",
  "windows-sys",
 ]
 
 [[package]]
 name = "nom"
-version = "7.1.1"
+version = "7.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a8903e5a29a317527874d0402f867152a3d21c908bb0b933e416c65e301d4c36"
+checksum = "d273983c5a657a70a3e8f2a01329822f3b8c8172b73826411a55751e404a0a4a"
 dependencies = [
  "memchr",
  "minimal-lexical",
 ]
 
 [[package]]
-name = "num-integer"
-version = "0.1.45"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
-dependencies = [
- "autocfg",
- "num-traits",
-]
-
-[[package]]
 name = "num-traits"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "578ede34cf02f8924ab9447f50c28075b4d3e5b269972345e7e0372b38c6cdcd"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.16.0"
+version = "1.18.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "86f0b0d4bf799edbc74508c1e8bf170ff5f41238e5f8225603ca7caaae2b7860"
+checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
 
 [[package]]
 name = "os_str_bytes"
-version = "6.4.1"
+version = "6.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b7820b9daea5457c9f21c69448905d723fbd21136ccf521748f23fd49e723ee"
-
-[[package]]
-name = "ouroboros"
-version = "0.15.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dfbb50b356159620db6ac971c6d5c9ab788c9cc38a6f49619fca2a27acb062ca"
-dependencies = [
- "aliasable",
- "ouroboros_macro",
-]
-
-[[package]]
-name = "ouroboros_macro"
-version = "0.15.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4a0d9d1a6191c4f391f87219d1ea42b23f09ee84d64763cd05ee6ea88d9f384d"
-dependencies = [
- "Inflector",
- "proc-macro-error",
- "proc-macro2",
- "quote",
- "syn",
-]
+checksum = "4d5d9eb14b174ee9aa2ef96dc2b94637a2d4b6e7cb873c7e171f0c20c6cf3eac"
 
 [[package]]
 name = "parking_lot"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3742b2c103b9f06bc9fff0a37ff4912935851bee6d36f3c02bcc755bcfec228f"
 dependencies = [
  "lock_api",
  "parking_lot_core",
 ]
 
 [[package]]
 name = "parking_lot_core"
-version = "0.9.5"
+version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff9f3fef3968a3ec5945535ed654cb38ff72d7495a25619e2247fb15a2ed9ba"
+checksum = "93f00c865fe7cabf650081affecd3871070f26767e7b2070a3ffae14c654b447"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-sys",
+ "windows-targets",
 ]
 
 [[package]]
 name = "pest"
-version = "2.5.1"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "cc8bed3549e0f9b0a2a78bf7c0018237a2cdf085eecbbc048e52612438e4e9d0"
+checksum = "e68e84bfb01f0507134eac1e9b410a12ba379d064eab48c50ba4ce329a527b70"
 dependencies = [
  "thiserror",
  "ucd-trie",
 ]
 
 [[package]]
 name = "pest_meta"
-version = "2.5.1"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fec8605d59fc2ae0c6c1aefc0c7c7a9769732017c0ce07f7a9cfffa7b4404f20"
+checksum = "745a452f8eb71e39ffd8ee32b3c5f51d03845f99786fa9b68db6ff509c505411"
 dependencies = [
  "once_cell",
  "pest",
- "sha1",
+ "sha2",
 ]
 
 [[package]]
 name = "pest_vm"
-version = "2.5.1"
+version = "2.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2dae921424fe86cfd367fa0050c43347ddc0c1c8ecb149ae889066176b5ba2ee"
+checksum = "910fc201ae72f3391e17ef56d12d95d7d537d68bdf572758edaca76c9349624f"
 dependencies = [
  "pest",
  "pest_meta",
 ]
 
 [[package]]
 name = "pretty"
@@ -771,15 +675,15 @@
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "da25490ff9892aab3fcf7c36f08cfb902dd3e71ca0f9f9517bea02a73a5ce38c"
 dependencies = [
  "proc-macro-error-attr",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro-error-attr"
 version = "1.0.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -788,148 +692,154 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.49"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "57a8eca9f9c4ffde41714334dee777596264c7825420f521abc92b5b5deb63a5"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pycddl"
-version = "0.4.0"
+version = "0.5.0"
 dependencies = [
  "cddl",
  "ciborium",
- "ouroboros",
  "pyo3",
  "pyo3-build-config",
+ "self_cell",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "268be0c73583c183f2b14052337465768c07726936a260f480f0857cb95ba543"
+checksum = "cffef52f74ec3b1a1baf295d9b8fcc3070327aefc39a6d00656b13c1d0b8885c"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "28fcd1e73f06ec85bf3280c48c67e731d8290ad3d730f8be9dc07946923005c8"
+checksum = "713eccf888fb05f1a96eb78c0dbc51907fee42b3377272dc902eb38985f418d5"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f6cb136e222e49115b3c51c32792886defbfb0adead26a688142b346a0b9ffc"
+checksum = "5b2ecbdcfb01cbbf56e179ce969a048fd7305a66d4cdf3303e0da09d69afe4c3"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "94144a1266e236b1c932682136dc35a9dee8d3589728f68130c7c3861ef96b28"
+checksum = "b78fdc0899f2ea781c463679b20cb08af9247febc8d052de941951024cd8aea0"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.17.3"
+version = "0.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8df9be978a2d2f0cdebabb03206ed73b11314701a5bfe71b0d753b81997777f"
+checksum = "60da7b84f1227c3e2fe7593505de274dcf4c8928b4e0a1c23d551a14e4e80a0f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 1.0.109",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.23"
+version = "1.0.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8856d8364d252a14d474036ea1358d63c9e6965c8e5c1885c18f73d70bff9c7b"
+checksum = "1b9ab9c7eadfd8df19006f1cf1a4aed13540ed5cbc047010ece5826e10825488"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
-version = "0.2.16"
+version = "0.3.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb5a58c1855b4b6819d59012155603f0b22ad30cad752600aadfcb695265519a"
+checksum = "567664f262709473930a4bf9e51bf2ebf3348f2e748ccc50dea20646858f8f29"
 dependencies = [
  "bitflags",
 ]
 
 [[package]]
 name = "regex"
-version = "1.7.0"
+version = "1.8.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e076559ef8e241f2ae3479e36f97bd5741c0330689e217ad51ce2c76808b868a"
+checksum = "d0ab3ca65655bb1e41f2a8c8cd662eb4fb035e67c3f78da1d61dffe89d07300f"
 dependencies = [
- "regex-syntax",
+ "regex-syntax 0.7.2",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.6.28"
+version = "0.6.29"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f162c6dd7b008981e4d40210aca20b4bd0f9b60ca9271061b07f78537722f2e1"
+
+[[package]]
+name = "regex-syntax"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "456c603be3e8d448b072f410900c09faf164fbce2d480456f50eea6e25f9c848"
+checksum = "436b050e76ed2903236f032a59761c1eb99e1b0aead2c257922771dab1fc8c78"
 
 [[package]]
 name = "ryu"
-version = "1.0.12"
+version = "1.0.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b4b9743ed687d4b4bcedf9ff5eaa7398495ae14e61cba0a295704edbc7decde"
+checksum = "f91339c0467de62360649f8d3e185ca8de4224ff281f66000de5eb2a77a79041"
 
 [[package]]
 name = "scopeguard"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d29ab0c6d3fc0ee92fe66e2d99f700eab17a8d57d1c1d3b748380fb20baa78cd"
 
 [[package]]
-name = "scratch"
-version = "1.0.3"
+name = "self_cell"
+version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ddccb15bcce173023b3fedd9436f882a0739b8dfb45e4f6b6002bee5929f61b2"
+checksum = "4a3926e239738d36060909ffe6f511502f92149a45a1fade7fe031cb2d33e88b"
 
 [[package]]
 name = "serde"
-version = "1.0.151"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "97fed41fc1a24994d044e6db6935e69511a1153b52c15eb42493b26fa87feba0"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde-wasm-bindgen"
 version = "0.4.5"
@@ -939,50 +849,50 @@
  "js-sys",
  "serde",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.151"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "255abe9a125a985c05190d687b320c12f9b1f0b99445e608c21ba0782c719ad8"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.91"
+version = "1.0.96"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "877c235533714907a8c2464236f5c4b2a17262ef1bd71f38f35ea592c8da6883"
+checksum = "057d394a50403bcac12672b2b18fb387ab6d289d957dab67dd201875391e52f1"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
-name = "sha1"
-version = "0.10.5"
+name = "sha2"
+version = "0.10.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f04293dc80c3993519f2d7f6f511707ee7094fe0c6d3406feb330cdb3540eba3"
+checksum = "82e6b795fe2e3b1e845bafcb27aa35405c4d47cdfc92af5fc8d3002f76cebdc0"
 dependencies = [
  "cfg-if",
  "cpufeatures",
  "digest",
 ]
 
 [[package]]
 name = "signal-hook"
-version = "0.3.14"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a253b5e89e2698464fc26b545c9edceb338e18a89effeeecfea192c3025be29d"
+checksum = "732768f1176d21d09e076c23a93123d40bba92d50c4058da34d45c8de8e682b9"
 dependencies = [
  "libc",
  "signal-hook-registry",
 ]
 
 [[package]]
 name = "signal-hook-mio"
@@ -993,17 +903,17 @@
  "libc",
  "mio",
  "signal-hook",
 ]
 
 [[package]]
 name = "signal-hook-registry"
-version = "1.4.0"
+version = "1.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e51e73328dc4ac0c7ccbda3a494dfa03df1de2f46018127f60c693f2648455b0"
+checksum = "d8229b473baa5980ac72ef434c4415e70c4b5e71b423043adb4ba059f89c99a1"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "simplelog"
 version = "0.11.2"
@@ -1031,28 +941,39 @@
 name = "strsim"
 version = "0.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "73473c0e59e6d5812c5dfe2a064a6444949f089e20eec9a2e5506596494e4623"
 
 [[package]]
 name = "syn"
-version = "1.0.107"
+version = "1.0.109"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1f4064b5b16e03ae50984a5a8ed5d4f8803e6bc1fd170a3cda91a1be4b18e3f5"
+checksum = "72b64191b275b66ffe2469e8af2c1cfe3bafa67b529ead792a6d0160888b4237"
+dependencies = [
+ "proc-macro2",
+ "quote",
+ "unicode-ident",
+]
+
+[[package]]
+name = "syn"
+version = "2.0.18"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "32d41677bcbe24c20c52e7c70b0d8db04134c5d1066bf98662e2871ad200ea3e"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.5"
+version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9410d0f6853b1d94f0e519fb95df60f29d2c1eff2d921ffdf01a4c8a3b54f12d"
+checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "termcolor"
 version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bab24d30b911b2376f3a13cc2cd443142f0c81dda04c118693e35b3835757755"
 dependencies = [
@@ -1063,30 +984,30 @@
 name = "textwrap"
 version = "0.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "222a222a5bfe1bba4a77b45ec488a741b3cb8872e5e499451fd7d0129c9c7c3d"
 
 [[package]]
 name = "thiserror"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6a9cd18aa97d5c45c6603caea1da6628790b37f7a34b6ca89522331c5180fed0"
+checksum = "978c9a314bd8dc99be594bc3c175faaa9794be04a5a5e153caba6915336cebac"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.38"
+version = "1.0.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1fb327af4685e4d03fa8cbcf1716380da910eeb2bb8be417e7f9fd3fb164f36f"
+checksum = "f9456a42c5b0d803c8cd86e73dd7cc9edd429499f37a3550d286d5e86720569f"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
 ]
 
 [[package]]
 name = "time"
 version = "0.1.45"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1b797afad3f312d1c66a56d11d0316f916356d11bd158fbc6ca6389ff6bf805a"
@@ -1094,17 +1015,17 @@
  "libc",
  "wasi 0.10.0+wasi-snapshot-preview1",
  "winapi",
 ]
 
 [[package]]
 name = "typed-arena"
-version = "2.0.1"
+version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0685c84d5d54d1c26f7d3eb96cd41550adb97baed141a761cf335d3d33bcd0ae"
+checksum = "6af6ae20167a9ece4bcb41af5b80f8a1f1df981f6391189ce00fd257af04126a"
 
 [[package]]
 name = "typenum"
 version = "1.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "497961ef93d974e23eb6f433eb5fe1b7930b659f06d12dec6fc44a8f554c0bba"
 
@@ -1112,23 +1033,23 @@
 name = "ucd-trie"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9e79c4d996edb816c91e4308506774452e55e95c3c9de07b6729e17e15a5ef81"
 
 [[package]]
 name = "unicode-ident"
-version = "1.0.6"
+version = "1.0.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84a22b9f218b40614adcb3f4ff08b703773ad44fa9423e4e0d346d5db86e4ebc"
+checksum = "b15811caf2415fb889178633e7724bad2509101cde276048e013b9def5e51fa0"
 
 [[package]]
 name = "unicode-segmentation"
-version = "1.10.0"
+version = "1.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0fdbf052a0783de01e944a6ce7a8cb939e295b1e7be835a1112c3b9a7f047a5a"
+checksum = "1dd624098567895118886609431a7c3b8f516e41d30e0643f03d94592a147e36"
 
 [[package]]
 name = "unicode-width"
 version = "0.1.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c0edd1e5b14653f783770bce4a4dabb4a5108a5370a5f5d8cfe8710c361f6c8b"
 
@@ -1164,65 +1085,65 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eaf9f5aceeec8be17c128b2e93e031fb8a4d469bb9c4ae2d7dc1888b26887268"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4c8ffb332579b0557b52d268b91feab8df3615f265d5270fec2a8c95b17c1142"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "052be0f94026e6cbc75cdefc9bae13fd6052cdcaf532fa6c45e7ae33a1e6c810"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "07bc0c051dc5f23e307b13285f9d75df86bfdf816c5721e573dec1f9b8aa193c"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn",
+ "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.83"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c38c045535d93ec4f0b4defec448e4291638ee608530863b1e2ba115d4fff7f"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "winapi"
 version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c839a674fcd7a98952e593242ea400abe93992746761e38641405d28b00f419"
 dependencies = [
@@ -1248,62 +1169,80 @@
 [[package]]
 name = "winapi-x86_64-pc-windows-gnu"
 version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "712e227841d057c1ee1cd2fb22fa7e5a5461ae8e48fa2ca79ec42cfc1931183f"
 
 [[package]]
+name = "windows"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e686886bc078bc1b0b600cac0147aadb815089b6e4da64016cbd754b6342700f"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
 name = "windows-sys"
-version = "0.42.0"
+version = "0.48.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
+dependencies = [
+ "windows-targets",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a3e1820f08b8513f676f7ab6c1f99ff312fb97b553d30ff4dd86f9f15728aa7"
+checksum = "7b1eb6f0cd7c80c79759c929114ef071b87354ce476d9d94271031c0497adfd5"
 dependencies = [
  "windows_aarch64_gnullvm",
  "windows_aarch64_msvc",
  "windows_i686_gnu",
  "windows_i686_msvc",
  "windows_x86_64_gnu",
  "windows_x86_64_gnullvm",
  "windows_x86_64_msvc",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "41d2aa71f6f0cbe00ae5167d90ef3cfe66527d6f613ca78ac8024c3ccab9a19e"
+checksum = "91ae572e1b79dba883e0d315474df7305d12f569b400fcf90581b06062f7e1bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd0f252f5a35cac83d6311b2e795981f5ee6e67eb1f9a7f64eb4500fbc4dcdb4"
+checksum = "b2ef27e0d7bdfcfc7b868b317c1d32c641a6fe4629c171b8928c7b08d98d7cf3"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fbeae19f6716841636c28d695375df17562ca208b2b7d0dc47635a50ae6c5de7"
+checksum = "622a1962a7db830d6fd0a69683c80a18fda201879f0f447f065a3b7467daa241"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "84c12f65daa39dd2babe6e442988fc329d6243fdce47d7d2d155b8d874862246"
+checksum = "4542c6e364ce21bf45d69fdd2a8e455fa38d316158cfd43b3ac1c5b1b19f8e00"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf7b1b21b5362cbc318f686150e5bcea75ecedc74dd157d874d754a2ca44b0ed"
+checksum = "ca2b8a661f7628cbd23440e50b05d705db3686f894fc9580820623656af974b1"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "09d525d2ba30eeb3297665bd434a54297e4170c7f1a44cad4ef58095b4cd2028"
+checksum = "7896dbc1f41e08872e9d5e8f8baa8fdd2677f29468c4e156210174edc7f7b953"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.42.0"
+version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f40009d85759725a34da6d89a94e63d7bdc50a862acf0dbc7c8e488f1edcb6f5"
+checksum = "1a515f5799fe4961cb532f983ce2b23082366b898e52ffbce459c86f67c8378a"
```

### Comparing `pycddl-0.4.0/PKG-INFO` & `pycddl-0.5.0/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: pycddl
-Version: 0.4.0
+Version: 0.5.0
 License-File: LICENSE
 Summary: Validate CBOR documents using CDDL schema language
 Home-Page: https://gitlab.com/tahoe-lafs/pycddl
 Author: Tahoe-LAFS project
 License: MIT
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 # PyCDDL: A CDDL validation library for Python
 
 [CDDL](https://www.rfc-editor.org/rfc/rfc8610.html) is a schema language for the CBOR serialization format.
 `pycddl` allows you to validate CBOR documents match a particular CDDL schema, based on the Rust [`cddl`](https://github.com/anweiss/cddl) library.
 
@@ -36,14 +36,19 @@
 In order to reduce memory usage, you can pass in any Python object that implements the buffer API and stores bytes, e.g. a `memoryview()` or a `mmap` object.
 
 **The passed-in object must be read-only, and the data must not change during validation!**
 If you mutate the data while validation is happening the result can be memory corruption or other [undefined behavior](https://stackoverflow.com/questions/18506029/can-undefined-behavior-erase-the-hard-drive#comment27209771_18506029).
 
 ## Release notes
 
+### 0.5.0
+
+* Support for ARM macOS.
+* Dropped Python 3.7 support.
+
 ### 0.4.1
 
 * Test fixes, with no user-relevant changes.
 
 ### 0.4.0
 
 * `validate_cbor()` now accepts read-only buffers, not just `bytes`. This is useful if you want to e.g. validate a large file, since you can `mmap()` it.
```

