# Comparing `tmp/cargo2rpm-0.1.4.tar.gz` & `tmp/cargo2rpm-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cargo2rpm-0.1.4.tar", last modified: Wed May 10 15:47:51 2023, max compression
+gzip compressed data, was "cargo2rpm-0.1.5.tar", last modified: Tue Jun 13 00:10:08 2023, max compression
```

## Comparing `cargo2rpm-0.1.4.tar` & `cargo2rpm-0.1.5.tar`

### file list

```diff
@@ -1,52 +1,56 @@
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-05-10 15:47:51.111456 cargo2rpm-0.1.4/
--rw-r--r--   0 deca      (1000) deca      (1000)     1059 2023-02-02 16:39:47.000000 cargo2rpm-0.1.4/LICENSE
--rw-rw-r--   0 deca      (1000) deca      (1000)       50 2023-02-06 21:47:33.000000 cargo2rpm-0.1.4/MANIFEST.in
--rw-r--r--   0 deca      (1000) deca      (1000)     1920 2023-05-10 15:47:51.111456 cargo2rpm-0.1.4/PKG-INFO
--rw-r--r--   0 deca      (1000) deca      (1000)     1142 2023-02-12 23:57:41.000000 cargo2rpm-0.1.4/README.md
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-05-10 15:47:51.108456 cargo2rpm-0.1.4/cargo2rpm/
--rw-r--r--   0 deca      (1000) deca      (1000)      497 2023-05-10 15:46:37.000000 cargo2rpm-0.1.4/cargo2rpm/__init__.py
--rw-r--r--   0 deca      (1000) deca      (1000)     7132 2023-02-14 13:59:22.000000 cargo2rpm-0.1.4/cargo2rpm/__main__.py
--rw-r--r--   0 deca      (1000) deca      (1000)     5010 2023-04-15 10:37:18.000000 cargo2rpm-0.1.4/cargo2rpm/cli.py
--rw-r--r--   0 deca      (1000) deca      (1000)    24552 2023-03-03 16:38:35.000000 cargo2rpm-0.1.4/cargo2rpm/metadata.py
--rw-r--r--   0 deca      (1000) deca      (1000)    15400 2023-03-02 22:37:18.000000 cargo2rpm-0.1.4/cargo2rpm/rpm.py
--rw-r--r--   0 deca      (1000) deca      (1000)    17634 2023-02-12 22:52:52.000000 cargo2rpm-0.1.4/cargo2rpm/semver.py
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-05-10 15:47:51.111456 cargo2rpm-0.1.4/cargo2rpm/testdata/
--rw-r--r--   0 deca      (1000) deca      (1000)     6403 2023-02-04 15:25:02.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/ahash-0.8.3.json
--rw-r--r--   0 deca      (1000) deca      (1000)     4690 2023-02-04 15:26:13.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/assert_cmd-2.0.8.json
--rw-r--r--   0 deca      (1000) deca      (1000)     3989 2023-02-04 15:27:28.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/assert_fs-1.0.10.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2177 2023-02-04 11:54:43.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/autocfg-1.1.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     4792 2023-02-04 15:28:23.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/bstr-1.2.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2078 2023-02-04 11:53:09.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/cfg-if-1.0.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)    21085 2023-02-04 15:28:56.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/clap-4.1.4.json
--rw-r--r--   0 deca      (1000) deca      (1000)    19710 2023-02-07 16:19:07.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/fapolicy-analyzer-0.6.8.json
--rw-r--r--   0 deca      (1000) deca      (1000)     6679 2023-02-04 15:29:26.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/gstreamer-0.19.7.json
--rw-r--r--   0 deca      (1000) deca      (1000)     3706 2023-02-04 15:30:03.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/human-panic-1.1.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     7484 2023-02-08 15:04:25.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/hyperfine-1.15.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     7821 2023-02-07 16:31:01.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/libblkio-1.2.2.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2126 2023-02-04 11:52:04.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/libc-0.2.139.json
--rw-r--r--   0 deca      (1000) deca      (1000)     4674 2023-02-04 15:30:40.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/predicates-2.1.5.json
--rw-r--r--   0 deca      (1000) deca      (1000)     3363 2023-02-04 11:53:39.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/proc-macro2-1.0.50.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2537 2023-02-04 11:52:34.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/quote-1.0.23.json
--rw-r--r--   0 deca      (1000) deca      (1000)     3523 2023-02-04 11:44:15.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/rand-0.8.5.json
--rw-r--r--   0 deca      (1000) deca      (1000)     1963 2023-02-04 11:45:17.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/rand_core-0.6.4.json
--rw-r--r--   0 deca      (1000) deca      (1000)     4188 2023-02-07 16:26:50.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/rpm-sequoia-1.2.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     9928 2023-02-04 15:31:49.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/rust_decimal-1.28.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)    10741 2023-02-08 12:38:58.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/rustix-0.36.8.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2116 2023-02-04 11:54:11.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/serde-1.0.152.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2562 2023-02-10 16:01:12.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/serde_derive-1.0.152.json
--rw-r--r--   0 deca      (1000) deca      (1000)    10844 2023-02-04 11:36:50.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/syn-1.0.107.json
--rw-r--r--   0 deca      (1000) deca      (1000)     6240 2023-02-04 15:32:38.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/time-0.3.17.json
--rw-r--r--   0 deca      (1000) deca      (1000)    32900 2023-02-08 13:03:00.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/tokio-1.25.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)     2131 2023-02-04 11:55:18.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/unicode-xid-0.2.4.json
--rw-r--r--   0 deca      (1000) deca      (1000)    12152 2023-02-04 15:33:09.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/zbus-3.8.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)    41849 2023-02-04 15:42:40.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/zola-0.16.1.json
--rw-r--r--   0 deca      (1000) deca      (1000)     6485 2023-02-08 15:04:53.000000 cargo2rpm-0.1.4/cargo2rpm/testdata/zoxide-0.9.0.json
--rw-r--r--   0 deca      (1000) deca      (1000)      766 2023-02-12 21:25:39.000000 cargo2rpm-0.1.4/cargo2rpm/utils.py
-drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-05-10 15:47:51.108456 cargo2rpm-0.1.4/cargo2rpm.egg-info/
--rw-r--r--   0 deca      (1000) deca      (1000)     1920 2023-05-10 15:47:51.000000 cargo2rpm-0.1.4/cargo2rpm.egg-info/PKG-INFO
--rw-r--r--   0 deca      (1000) deca      (1000)     1534 2023-05-10 15:47:51.000000 cargo2rpm-0.1.4/cargo2rpm.egg-info/SOURCES.txt
--rw-r--r--   0 deca      (1000) deca      (1000)        1 2023-05-10 15:47:51.000000 cargo2rpm-0.1.4/cargo2rpm.egg-info/dependency_links.txt
--rw-r--r--   0 deca      (1000) deca      (1000)       54 2023-05-10 15:47:51.000000 cargo2rpm-0.1.4/cargo2rpm.egg-info/entry_points.txt
--rw-r--r--   0 deca      (1000) deca      (1000)       10 2023-05-10 15:47:51.000000 cargo2rpm-0.1.4/cargo2rpm.egg-info/top_level.txt
--rw-r--r--   0 deca      (1000) deca      (1000)      161 2023-02-02 00:36:19.000000 cargo2rpm-0.1.4/pyproject.toml
--rw-r--r--   0 deca      (1000) deca      (1000)      893 2023-05-10 15:47:51.111456 cargo2rpm-0.1.4/setup.cfg
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-06-13 00:10:08.660513 cargo2rpm-0.1.5/
+-rw-r--r--   0 deca      (1000) deca      (1000)     1059 2023-02-02 16:39:47.000000 cargo2rpm-0.1.5/LICENSE
+-rw-rw-r--   0 deca      (1000) deca      (1000)       50 2023-02-06 21:47:33.000000 cargo2rpm-0.1.5/MANIFEST.in
+-rw-r--r--   0 deca      (1000) deca      (1000)     1920 2023-06-13 00:10:08.660513 cargo2rpm-0.1.5/PKG-INFO
+-rw-r--r--   0 deca      (1000) deca      (1000)     1142 2023-02-12 23:57:41.000000 cargo2rpm-0.1.5/README.md
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-06-13 00:10:08.657513 cargo2rpm-0.1.5/cargo2rpm/
+-rw-r--r--   0 deca      (1000) deca      (1000)      497 2023-06-13 00:08:14.000000 cargo2rpm-0.1.5/cargo2rpm/__init__.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     7132 2023-02-14 13:59:22.000000 cargo2rpm-0.1.5/cargo2rpm/__main__.py
+-rw-r--r--   0 deca      (1000) deca      (1000)     5010 2023-04-15 10:37:18.000000 cargo2rpm-0.1.5/cargo2rpm/cli.py
+-rw-r--r--   0 deca      (1000) deca      (1000)    24552 2023-03-03 16:38:35.000000 cargo2rpm-0.1.5/cargo2rpm/metadata.py
+-rw-r--r--   0 deca      (1000) deca      (1000)    15915 2023-06-12 23:49:45.000000 cargo2rpm-0.1.5/cargo2rpm/rpm.py
+-rw-r--r--   0 deca      (1000) deca      (1000)    17634 2023-02-12 22:52:52.000000 cargo2rpm-0.1.5/cargo2rpm/semver.py
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-06-13 00:10:08.660513 cargo2rpm-0.1.5/cargo2rpm/testdata/
+-rw-r--r--   0 deca      (1000) deca      (1000)     6403 2023-02-04 15:25:02.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/ahash-0.8.3.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2134 2023-06-12 20:40:02.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/aho-corasick-1.0.2.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     4690 2023-02-04 15:26:13.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/assert_cmd-2.0.8.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     3989 2023-02-04 15:27:28.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/assert_fs-1.0.10.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2177 2023-02-04 11:54:43.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/autocfg-1.1.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     4792 2023-02-04 15:28:23.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/bstr-1.2.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2078 2023-02-04 11:53:09.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/cfg-if-1.0.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    21085 2023-02-04 15:28:56.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/clap-4.1.4.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    19710 2023-02-07 16:19:07.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/fapolicy-analyzer-0.6.8.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     6679 2023-02-04 15:29:26.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/gstreamer-0.19.7.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     3706 2023-02-04 15:30:03.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/human-panic-1.1.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     7484 2023-02-08 15:04:25.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/hyperfine-1.15.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     5189 2023-06-12 20:41:15.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/iri-string-0.7.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     7821 2023-02-07 16:31:01.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/libblkio-1.2.2.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2126 2023-02-04 11:52:04.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/libc-0.2.139.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     4674 2023-02-04 15:30:40.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/predicates-2.1.5.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     3363 2023-02-04 11:53:39.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/proc-macro2-1.0.50.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2537 2023-02-04 11:52:34.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/quote-1.0.23.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     3523 2023-02-04 11:44:15.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/rand-0.8.5.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     1963 2023-02-04 11:45:17.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/rand_core-0.6.4.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     6593 2023-06-12 20:40:35.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/regex-1.8.4.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     1816 2023-06-12 20:40:57.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/regex-syntax-0.7.2.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     4188 2023-02-07 16:26:50.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/rpm-sequoia-1.2.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     9928 2023-02-04 15:31:49.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/rust_decimal-1.28.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    10741 2023-02-08 12:38:58.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/rustix-0.36.8.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2116 2023-02-04 11:54:11.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/serde-1.0.152.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2562 2023-02-10 16:01:12.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/serde_derive-1.0.152.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    10844 2023-02-04 11:36:50.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/syn-1.0.107.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     6240 2023-02-04 15:32:38.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/time-0.3.17.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    32900 2023-02-08 13:03:00.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/tokio-1.25.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     2131 2023-02-04 11:55:18.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/unicode-xid-0.2.4.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    12152 2023-02-04 15:33:09.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/zbus-3.8.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)    41849 2023-02-04 15:42:40.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/zola-0.16.1.json
+-rw-r--r--   0 deca      (1000) deca      (1000)     6485 2023-02-08 15:04:53.000000 cargo2rpm-0.1.5/cargo2rpm/testdata/zoxide-0.9.0.json
+-rw-r--r--   0 deca      (1000) deca      (1000)      766 2023-02-12 21:25:39.000000 cargo2rpm-0.1.5/cargo2rpm/utils.py
+drwxr-xr-x   0 deca      (1000) deca      (1000)        0 2023-06-13 00:10:08.657513 cargo2rpm-0.1.5/cargo2rpm.egg-info/
+-rw-r--r--   0 deca      (1000) deca      (1000)     1920 2023-06-13 00:10:08.000000 cargo2rpm-0.1.5/cargo2rpm.egg-info/PKG-INFO
+-rw-r--r--   0 deca      (1000) deca      (1000)     1697 2023-06-13 00:10:08.000000 cargo2rpm-0.1.5/cargo2rpm.egg-info/SOURCES.txt
+-rw-r--r--   0 deca      (1000) deca      (1000)        1 2023-06-13 00:10:08.000000 cargo2rpm-0.1.5/cargo2rpm.egg-info/dependency_links.txt
+-rw-r--r--   0 deca      (1000) deca      (1000)       54 2023-06-13 00:10:08.000000 cargo2rpm-0.1.5/cargo2rpm.egg-info/entry_points.txt
+-rw-r--r--   0 deca      (1000) deca      (1000)       10 2023-06-13 00:10:08.000000 cargo2rpm-0.1.5/cargo2rpm.egg-info/top_level.txt
+-rw-r--r--   0 deca      (1000) deca      (1000)      161 2023-02-02 00:36:19.000000 cargo2rpm-0.1.5/pyproject.toml
+-rw-r--r--   0 deca      (1000) deca      (1000)      893 2023-06-13 00:10:08.660513 cargo2rpm-0.1.5/setup.cfg
```

### Comparing `cargo2rpm-0.1.4/LICENSE` & `cargo2rpm-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/PKG-INFO` & `cargo2rpm-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cargo2rpm
-Version: 0.1.4
+Version: 0.1.5
 Summary: Translation layer between cargo and RPM
 Home-page: https://pagure.io/fedora-rust/cargo2rpm
 Author: Fedora Rust SIG
 Author-email: rust@lists.fedoraproject.org
 License: MIT
 Keywords: rpm,cargo,rust
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cargo2rpm-0.1.4/README.md` & `cargo2rpm-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/__main__.py` & `cargo2rpm-0.1.5/cargo2rpm/__main__.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/cli.py` & `cargo2rpm-0.1.5/cargo2rpm/cli.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/metadata.py` & `cargo2rpm-0.1.5/cargo2rpm/metadata.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/rpm.py` & `cargo2rpm-0.1.5/cargo2rpm/rpm.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,28 +107,33 @@
 
     # features unconditionally enabled by feature dependencies
     for (name, other_features) in other_enabled.items():
         features = deps_enabled_features.get(name) or set()
         features.update(other_features)
         deps_enabled_features[name] = features
 
+        if "default" in features:
+            deps_default_features[name] = True
+
     # features conditionally enabled by feature dependencies
     for (name, other_features) in other_conditional.items():
         if name in enabled or CARGO_BUGGY_RESOLVER:
             features = deps_enabled_features.get(name) or set()
             features.update(other_features)
             deps_enabled_features[name] = features
 
         if name not in enabled and CARGO_BUGGY_RESOLVER:
-            defaults = False
+            defaults = deps_default_features.get(name) or False
             if dep := normal_optional.get(name):
                 defaults = defaults or dep.uses_default_features
+                additional_features = dep.features
             if dep := build_optional.get(name):
                 defaults = defaults or dep.uses_default_features
-            workarounds[name] = (other_features, defaults)
+                additional_features = dep.features
+            workarounds[name] = (set.union(other_features, additional_features), defaults)
 
     # collect dependencies taking into account which features are enabled
     brs = set()
 
     # normal dependencies
     for (name, dep) in normal.items():
         if dep.path:
@@ -191,17 +196,25 @@
                 brs.add(dep.to_rpm(None))
             for feature in deps_enabled_features[name]:
                 brs.add(dep.to_rpm(feature))
 
     # workarounds
     for (name, (features, defaults)) in workarounds.items():
         if dep := normal_optional.get(name):
+            if defaults:
+                brs.add(dep.to_rpm("default"))
+            else:
+                brs.add(dep.to_rpm(None))
             for feature in features:
                 brs.add(dep.to_rpm(feature))
         if dep := build_optional.get(name):
+            if defaults:
+                brs.add(dep.to_rpm("default"))
+            else:
+                brs.add(dep.to_rpm(None))
             for feature in features:
                 brs.add(dep.to_rpm(feature))
 
     return brs
 
 
 def workspace_buildrequires(metadata: Metadata, flags: FeatureFlags, with_dev_deps: bool) -> set[str]:
```

### Comparing `cargo2rpm-0.1.4/cargo2rpm/semver.py` & `cargo2rpm-0.1.5/cargo2rpm/semver.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/ahash-0.8.3.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/ahash-0.8.3.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/assert_cmd-2.0.8.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/assert_cmd-2.0.8.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/assert_fs-1.0.10.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/assert_fs-1.0.10.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/autocfg-1.1.0.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/autocfg-1.1.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/bstr-1.2.0.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/bstr-1.2.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/cfg-if-1.0.0.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/cfg-if-1.0.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/clap-4.1.4.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/clap-4.1.4.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/fapolicy-analyzer-0.6.8.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/fapolicy-analyzer-0.6.8.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/gstreamer-0.19.7.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/gstreamer-0.19.7.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/human-panic-1.1.0.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/human-panic-1.1.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/hyperfine-1.15.0.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/hyperfine-1.15.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/libblkio-1.2.2.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/libblkio-1.2.2.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/libc-0.2.139.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/libc-0.2.139.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/predicates-2.1.5.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/predicates-2.1.5.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/proc-macro2-1.0.50.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/proc-macro2-1.0.50.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/quote-1.0.23.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/quote-1.0.23.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/rand-0.8.5.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/rand-0.8.5.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/rand_core-0.6.4.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/rand_core-0.6.4.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/rpm-sequoia-1.2.0.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/rpm-sequoia-1.2.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/rust_decimal-1.28.0.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/rust_decimal-1.28.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/rustix-0.36.8.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/rustix-0.36.8.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/serde-1.0.152.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/serde-1.0.152.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/serde_derive-1.0.152.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/serde_derive-1.0.152.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/syn-1.0.107.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/syn-1.0.107.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/time-0.3.17.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/time-0.3.17.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/tokio-1.25.0.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/tokio-1.25.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/unicode-xid-0.2.4.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/unicode-xid-0.2.4.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/zbus-3.8.0.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/zbus-3.8.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/zola-0.16.1.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/zola-0.16.1.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/testdata/zoxide-0.9.0.json` & `cargo2rpm-0.1.5/cargo2rpm/testdata/zoxide-0.9.0.json`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm/utils.py` & `cargo2rpm-0.1.5/cargo2rpm/utils.py`

 * *Files identical despite different names*

### Comparing `cargo2rpm-0.1.4/cargo2rpm.egg-info/PKG-INFO` & `cargo2rpm-0.1.5/cargo2rpm.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cargo2rpm
-Version: 0.1.4
+Version: 0.1.5
 Summary: Translation layer between cargo and RPM
 Home-page: https://pagure.io/fedora-rust/cargo2rpm
 Author: Fedora Rust SIG
 Author-email: rust@lists.fedoraproject.org
 License: MIT
 Keywords: rpm,cargo,rust
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `cargo2rpm-0.1.4/cargo2rpm.egg-info/SOURCES.txt` & `cargo2rpm-0.1.5/cargo2rpm.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,31 +12,35 @@
 cargo2rpm/utils.py
 cargo2rpm.egg-info/PKG-INFO
 cargo2rpm.egg-info/SOURCES.txt
 cargo2rpm.egg-info/dependency_links.txt
 cargo2rpm.egg-info/entry_points.txt
 cargo2rpm.egg-info/top_level.txt
 cargo2rpm/testdata/ahash-0.8.3.json
+cargo2rpm/testdata/aho-corasick-1.0.2.json
 cargo2rpm/testdata/assert_cmd-2.0.8.json
 cargo2rpm/testdata/assert_fs-1.0.10.json
 cargo2rpm/testdata/autocfg-1.1.0.json
 cargo2rpm/testdata/bstr-1.2.0.json
 cargo2rpm/testdata/cfg-if-1.0.0.json
 cargo2rpm/testdata/clap-4.1.4.json
 cargo2rpm/testdata/fapolicy-analyzer-0.6.8.json
 cargo2rpm/testdata/gstreamer-0.19.7.json
 cargo2rpm/testdata/human-panic-1.1.0.json
 cargo2rpm/testdata/hyperfine-1.15.0.json
+cargo2rpm/testdata/iri-string-0.7.0.json
 cargo2rpm/testdata/libblkio-1.2.2.json
 cargo2rpm/testdata/libc-0.2.139.json
 cargo2rpm/testdata/predicates-2.1.5.json
 cargo2rpm/testdata/proc-macro2-1.0.50.json
 cargo2rpm/testdata/quote-1.0.23.json
 cargo2rpm/testdata/rand-0.8.5.json
 cargo2rpm/testdata/rand_core-0.6.4.json
+cargo2rpm/testdata/regex-1.8.4.json
+cargo2rpm/testdata/regex-syntax-0.7.2.json
 cargo2rpm/testdata/rpm-sequoia-1.2.0.json
 cargo2rpm/testdata/rust_decimal-1.28.0.json
 cargo2rpm/testdata/rustix-0.36.8.json
 cargo2rpm/testdata/serde-1.0.152.json
 cargo2rpm/testdata/serde_derive-1.0.152.json
 cargo2rpm/testdata/syn-1.0.107.json
 cargo2rpm/testdata/time-0.3.17.json
```

### Comparing `cargo2rpm-0.1.4/setup.cfg` & `cargo2rpm-0.1.5/setup.cfg`

 * *Files identical despite different names*

