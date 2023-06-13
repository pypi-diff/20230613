# Comparing `tmp/tcfetch-0.1.tar.gz` & `tmp/tcfetch-0.3.1.tar.gz`

## Comparing `tcfetch-0.1.tar` & `tcfetch-0.3.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0      513 1970-01-01 00:00:00.000000 tcfetch-0.1/local_dependencies/tc-fetch/Cargo.toml
--rw-r--r--   0     1001      123     2459 2023-06-06 17:54:25.000000 tcfetch-0.1/local_dependencies/tc-fetch/.github/workflows/python.yml
--rw-r--r--   0     1001      123       49 2023-06-06 17:54:25.000000 tcfetch-0.1/local_dependencies/tc-fetch/.gitignore
--rw-r--r--   0     1001      123     1500 2023-06-06 17:54:25.000000 tcfetch-0.1/local_dependencies/tc-fetch/LICENSE.md
--rw-r--r--   0     1001      123     1709 2023-06-06 17:54:25.000000 tcfetch-0.1/local_dependencies/tc-fetch/README.md
--rw-r--r--   0     1001      123       10 2023-06-06 17:54:52.000000 tcfetch-0.1/local_dependencies/tc-fetch/dist/tcfetch-0.1.tar.gz
--rw-r--r--   0     1001      123     4269 2023-06-06 17:54:25.000000 tcfetch-0.1/local_dependencies/tc-fetch/src/gh.rs
--rw-r--r--   0     1001      123     1614 2023-06-06 17:54:25.000000 tcfetch-0.1/local_dependencies/tc-fetch/src/ghwpt.rs
--rw-r--r--   0     1001      123     3141 2023-06-06 17:54:25.000000 tcfetch-0.1/local_dependencies/tc-fetch/src/hgmo.rs
--rw-r--r--   0     1001      123     5390 2023-06-06 17:54:25.000000 tcfetch-0.1/local_dependencies/tc-fetch/src/lib.rs
--rw-r--r--   0     1001      123     3038 2023-06-06 17:54:25.000000 tcfetch-0.1/local_dependencies/tc-fetch/src/main.rs
--rw-r--r--   0     1001      123     5270 2023-06-06 17:54:25.000000 tcfetch-0.1/local_dependencies/tc-fetch/src/taskcluster.rs
--rw-r--r--   0     1001      123     1417 2023-06-06 17:54:25.000000 tcfetch-0.1/local_dependencies/tc-fetch/src/utils.rs
--rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 tcfetch-0.1/Cargo.toml
--rw-r--r--   0     1001      123     2807 2023-06-06 17:54:25.000000 tcfetch-0.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      123      685 2023-06-06 17:54:25.000000 tcfetch-0.1/.gitignore
--rw-r--r--   0     1001      123      535 2023-06-06 17:54:25.000000 tcfetch-0.1/pyproject.toml
--rw-r--r--   0     1001      123     2139 2023-06-06 17:54:25.000000 tcfetch-0.1/src/lib.rs
--rw-r--r--   0     1001      123    31883 2023-06-06 17:54:50.000000 tcfetch-0.1/Cargo.lock
--rw-r--r--   0        0        0      332 1970-01-01 00:00:00.000000 tcfetch-0.1/PKG-INFO
+-rw-r--r--   0        0        0      521 1970-01-01 00:00:00.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/Cargo.toml
+-rw-r--r--   0     1001      123     2459 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/.github/workflows/python.yml
+-rw-r--r--   0     1001      123       49 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/.gitignore
+-rw-r--r--   0     1001      123     1500 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/LICENSE.md
+-rw-r--r--   0     1001      123     1709 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/README.md
+-rw-r--r--   0     1001      123       10 2023-06-13 07:18:12.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/dist/tcfetch-0.3.1.tar.gz
+-rw-r--r--   0     1001      123     4269 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/src/gh.rs
+-rw-r--r--   0     1001      123     1614 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/src/ghwpt.rs
+-rw-r--r--   0     1001      123     3141 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/src/hgmo.rs
+-rw-r--r--   0     1001      123     5390 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/src/lib.rs
+-rw-r--r--   0     1001      123     3038 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/src/main.rs
+-rw-r--r--   0     1001      123     5270 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/src/taskcluster.rs
+-rw-r--r--   0     1001      123     1417 2023-06-13 07:16:01.000000 tcfetch-0.3.1/local_dependencies/tc-fetch/src/utils.rs
+-rw-r--r--   0        0        0      290 1970-01-01 00:00:00.000000 tcfetch-0.3.1/Cargo.toml
+-rw-r--r--   0     1001      123     2807 2023-06-13 07:16:01.000000 tcfetch-0.3.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      123      685 2023-06-13 07:16:01.000000 tcfetch-0.3.1/.gitignore
+-rw-r--r--   0     1001      123      537 2023-06-13 07:16:01.000000 tcfetch-0.3.1/pyproject.toml
+-rw-r--r--   0     1001      123     2139 2023-06-13 07:16:01.000000 tcfetch-0.3.1/src/lib.rs
+-rw-r--r--   0     1001      123    33086 2023-06-13 07:18:10.000000 tcfetch-0.3.1/Cargo.lock
+-rw-r--r--   0        0        0      334 1970-01-01 00:00:00.000000 tcfetch-0.3.1/PKG-INFO
```

### Comparing `tcfetch-0.1/local_dependencies/tc-fetch/Cargo.toml` & `tcfetch-0.3.1/local_dependencies/tc-fetch/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "tc-fetch"
-version = "0.3.0"
+version = "0.3.1"
 authors = ["James Graham <james@hoppipolla.co.uk>"]
 description="Download taskcluster artifacts"
 readme = "README.md"
 edition = "2021"
 license = "BSD-3-Clause"
 
 [lib]
@@ -14,13 +14,13 @@
 [[bin]]
 name = "tcfetch"
 path = "src/main.rs"
 
 [dependencies]
 clap = "4"
 regex = "1"
-reqwest = {version="0.11", default-features=false, features=["blocking", "rustls-tls"]}
+reqwest = {version="0.11", default-features=false, features=["blocking", "gzip", "rustls-tls"]}
 thiserror = "1"
 scoped_threadpool = "0.1"
 serde = "1"
 serde_derive = "1"
 serde_json = "1"
```

### Comparing `tcfetch-0.1/local_dependencies/tc-fetch/.github/workflows/python.yml` & `tcfetch-0.3.1/local_dependencies/tc-fetch/.github/workflows/python.yml`

 * *Files identical despite different names*

### Comparing `tcfetch-0.1/local_dependencies/tc-fetch/LICENSE.md` & `tcfetch-0.3.1/local_dependencies/tc-fetch/LICENSE.md`

 * *Files identical despite different names*

### Comparing `tcfetch-0.1/local_dependencies/tc-fetch/README.md` & `tcfetch-0.3.1/local_dependencies/tc-fetch/README.md`

 * *Files identical despite different names*

### Comparing `tcfetch-0.1/local_dependencies/tc-fetch/src/gh.rs` & `tcfetch-0.3.1/local_dependencies/tc-fetch/src/gh.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.1/local_dependencies/tc-fetch/src/ghwpt.rs` & `tcfetch-0.3.1/local_dependencies/tc-fetch/src/ghwpt.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.1/local_dependencies/tc-fetch/src/hgmo.rs` & `tcfetch-0.3.1/local_dependencies/tc-fetch/src/hgmo.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.1/local_dependencies/tc-fetch/src/lib.rs` & `tcfetch-0.3.1/local_dependencies/tc-fetch/src/lib.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.1/local_dependencies/tc-fetch/src/main.rs` & `tcfetch-0.3.1/local_dependencies/tc-fetch/src/main.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.1/local_dependencies/tc-fetch/src/taskcluster.rs` & `tcfetch-0.3.1/local_dependencies/tc-fetch/src/taskcluster.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.1/local_dependencies/tc-fetch/src/utils.rs` & `tcfetch-0.3.1/local_dependencies/tc-fetch/src/utils.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.1/.github/workflows/CI.yml` & `tcfetch-0.3.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `tcfetch-0.1/.gitignore` & `tcfetch-0.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `tcfetch-0.1/pyproject.toml` & `tcfetch-0.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "tcfetch"
 description = "Download log files from Taskcluster CI systems"
 author = "James Graham"
 author_email = "james@hoppipolla.co.uk"
 license = "BSD-3-Clause"
-version = "0.1"
+version = "0.3.1"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
```

### Comparing `tcfetch-0.1/src/lib.rs` & `tcfetch-0.3.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `tcfetch-0.1/Cargo.lock` & `tcfetch-0.3.1/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
+name = "adler"
+version = "1.0.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
+
+[[package]]
 name = "aho-corasick"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "43f6cb1bf222025340178f382c426f13757b2960e89779dfcb319c32542a5a41"
 dependencies = [
  "memchr",
 ]
@@ -57,14 +63,27 @@
 checksum = "180abfa45703aebe0093f79badacc01b8fd4ea2e35118747e5811127f926e188"
 dependencies = [
  "anstyle",
  "windows-sys",
 ]
 
 [[package]]
+name = "async-compression"
+version = "0.4.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "5b0122885821398cc923ece939e24d1056a2384ee719432397fa9db87230ff11"
+dependencies = [
+ "flate2",
+ "futures-core",
+ "memchr",
+ "pin-project-lite",
+ "tokio",
+]
+
+[[package]]
 name = "autocfg"
 version = "1.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
 
 [[package]]
 name = "base64"
@@ -100,26 +119,26 @@
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
 [[package]]
 name = "clap"
-version = "4.3.2"
+version = "4.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "401a4694d2bf92537b6867d94de48c4842089645fdcdf6c71865b175d836e9c2"
+checksum = "ca8f255e4b8027970e78db75e78831229c9815fdbfa67eb1a1b777a62e24b4a0"
 dependencies = [
  "clap_builder",
 ]
 
 [[package]]
 name = "clap_builder"
-version = "4.3.1"
+version = "4.3.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "72394f3339a76daf211e57d4bcb374410f3965dcc606dd0e03738c7888766980"
+checksum = "acd4f3c17c83b0ba34ffbc4f8bbd74f079413f747f84a6f89292f138057e36ab"
 dependencies = [
  "anstream",
  "anstyle",
  "bitflags",
  "clap_lex",
  "strsim",
 ]
@@ -133,14 +152,23 @@
 [[package]]
 name = "colorchoice"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "acbf1af155f9b9ef647e42cdc158db4b64a1b61f743629225fde6f3e0be2a7c7"
 
 [[package]]
+name = "crc32fast"
+version = "1.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b540bd8bc810d3885c6ea91e2018302f68baba2129ab3e88f32389ee9370880d"
+dependencies = [
+ "cfg-if",
+]
+
+[[package]]
 name = "encoding_rs"
 version = "0.8.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "071a31f4ee85403370b58aca746f01041ede6f0da2730960ad001edc2b71b394"
 dependencies = [
  "cfg-if",
 ]
@@ -163,14 +191,24 @@
 checksum = "aa68f1b12764fab894d2755d2518754e71b4fd80ecfb822714a1206c2aab39bf"
 dependencies = [
  "cc",
  "libc",
 ]
 
 [[package]]
+name = "flate2"
+version = "1.0.26"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3b9429470923de8e8cbd4d2dc513535400b4b3fef0319fb5c4e1f520a7bef743"
+dependencies = [
+ "crc32fast",
+ "miniz_oxide",
+]
+
+[[package]]
 name = "fnv"
 version = "1.0.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3f9eec918d3f24069decb9af1554cad7c880e2da24a9afd88aca000531ab82c1"
 
 [[package]]
 name = "form_urlencoded"
@@ -399,17 +437,17 @@
 name = "itoa"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "453ad9f582a441959e5f0d088b02ce04cfe8d51a8eaf077f12ac6d3e94164ca6"
 
 [[package]]
 name = "js-sys"
-version = "0.3.63"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2f37a4a5928311ac501dee68b3c7613a1037d0edb30c8e5427bd832d55d1b790"
+checksum = "c5f195fe497f702db0f318b07fdd68edb16955aed830df8363d837542f8f935a"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "libc"
 version = "0.2.146"
@@ -430,17 +468,17 @@
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.18"
+version = "0.4.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "518ef76f2f87365916b142844c16d8fefd85039bc5699050210a7778ee1cd1de"
+checksum = "b06a4cde4c0f271a446782e3eff8de789548ce57dbc8eca9292c27f4a42004b4"
 
 [[package]]
 name = "memchr"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2dffe52ecf27772e601905b7522cb4ef790d2cc203488bbd0e2fe85fcb74566d"
 
@@ -456,14 +494,23 @@
 [[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
+name = "miniz_oxide"
+version = "0.7.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+dependencies = [
+ "adler",
+]
+
+[[package]]
 name = "mio"
 version = "0.8.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "927a765cd3fc26206e66b296465fa9d3e5ab003e651c1b3c060e7956d96b19d2"
 dependencies = [
  "libc",
  "wasi",
@@ -525,17 +572,17 @@
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.59"
+version = "1.0.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6aeca18b86b413c660b781aa319e4e2648a3e6f9eadc9b47e9038e6fe9f3451b"
+checksum = "dec2b086b7a862cf4de201096214fa870344cf922b2b30c167badb3af3195406"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.18.3"
@@ -633,14 +680,15 @@
 
 [[package]]
 name = "reqwest"
 version = "0.11.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cde824a14b7c14f85caff81225f411faacc04a2013f41670f41443742b1c1c55"
 dependencies = [
+ "async-compression",
  "base64",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
@@ -657,14 +705,15 @@
  "rustls",
  "rustls-pemfile",
  "serde",
  "serde_json",
  "serde_urlencoded",
  "tokio",
  "tokio-rustls",
+ "tokio-util",
  "tower-service",
  "url",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
  "webpki-roots",
  "winreg",
@@ -683,17 +732,17 @@
  "untrusted",
  "web-sys",
  "winapi",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.37.19"
+version = "0.37.20"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "acf8729d8542766f1b2cf77eb034d52f40d375bb8b615d0b147089946e16613d"
+checksum = "b96e891d04aa506a6d1f318d2771bcb1c7dfda84e126660ace067c9b474bb2c0"
 dependencies = [
  "bitflags",
  "errno",
  "io-lifetimes",
  "libc",
  "linux-raw-sys",
  "windows-sys",
@@ -756,23 +805,23 @@
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "serde"
-version = "1.0.163"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2113ab51b87a539ae008b5c6c02dc020ffa39afd2d83cffcb3f4eb2722cebec2"
+checksum = "9e8c8cf938e98f769bc164923b06dce91cea1751522f46f8466461af04c9027d"
 
 [[package]]
 name = "serde_derive"
-version = "1.0.163"
+version = "1.0.164"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c805777e3930c8883389c602315a24224bcc738b63905ef87cd1420353ea93e"
+checksum = "d9735b638ccc51c28bf6914d90a2e9725b377144fc612c49a611fddd1b631d68"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.18",
 ]
 
 [[package]]
@@ -861,15 +910,15 @@
 name = "target-lexicon"
 version = "0.12.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd1ba337640d60c3e96bc6f0638a939b9c9a7f2c316a1598c279828b3d1dc8c5"
 
 [[package]]
 name = "tc-fetch"
-version = "0.3.0"
+version = "0.3.1"
 dependencies = [
  "clap",
  "regex",
  "reqwest",
  "scoped_threadpool",
  "serde",
  "serde_derive",
@@ -934,17 +983,17 @@
  "pin-project-lite",
  "socket2",
  "windows-sys",
 ]
 
 [[package]]
 name = "tokio-rustls"
-version = "0.24.0"
+version = "0.24.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e0d409377ff5b1e3ca6437aa86c1eb7d40c134bfec254e44c830defa92669db5"
+checksum = "c28327cf380ac148141087fbfb9de9d7bd4e84ab5d2c28fbc911d753de8a7081"
 dependencies = [
  "rustls",
  "tokio",
 ]
 
 [[package]]
 name = "tokio-util"
@@ -1056,83 +1105,83 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5bba0e8cb82ba49ff4e229459ff22a191bbe9a1cb3a341610c9c33efc27ddf73"
+checksum = "7706a72ab36d8cb1f80ffbf0e071533974a60d0a308d01a5d0375bf60499a342"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "19b04bc93f9d6bdee709f6bd2118f57dd6679cf1176a1af464fca3ab0d66d8fb"
+checksum = "5ef2b6d3c510e9625e5fe6f509ab07d66a760f0885d858736483c32ed7809abd"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
  "syn 2.0.18",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.36"
+version = "0.4.37"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2d1985d03709c53167ce907ff394f5316aa22cb4e12761295c5dc57dacb6297e"
+checksum = "c02dbc21516f9f1f04f187958890d7e6026df8d16540b7ad9492bc34a67cea03"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14d6b024f1a526bb0234f52840389927257beb670610081360e5a03c5df9c258"
+checksum = "dee495e55982a3bd48105a7b947fd2a9b4a8ae3010041b9e0faab3f9cd028f1d"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e128beba882dd1eb6200e1dc92ae6c5dbaa4311aa7bb211ca035779e5efc39f8"
+checksum = "54681b18a46765f095758388f2d0cf16eb8d4169b639ab575a8f5693af210c7b"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 2.0.18",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.86"
+version = "0.2.87"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed9d5b4305409d1fc9482fee2d7f9bcbf24b3972bf59817ef757e23982242a93"
+checksum = "ca6ad05a4870b2bf5fe995117d3728437bd27d7cd5f06f13c17443ef369775a1"
 
 [[package]]
 name = "web-sys"
-version = "0.3.63"
+version = "0.3.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3bdd9ef4e984da1187bf8110c5cf5b845fbc87a23602cdf912386a76fcd3a7c2"
+checksum = "9b85cbef8c220a6abc02aefd892dfc0fc23afb1c6a426316ec33253a3877249b"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "webpki"
```

