# Comparing `tmp/rpm_head_signing-1.7.tar.gz` & `tmp/rpm_head_signing-1.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rpm_head_signing-1.7.tar", last modified: Mon Oct 25 16:20:50 2021, max compression
+gzip compressed data, was "rpm_head_signing-1.7.1.tar", last modified: Tue Jun 13 20:57:48 2023, max compression
```

## Comparing `rpm_head_signing-1.7.tar` & `rpm_head_signing-1.7.1.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 16:20:50.063568 rpm_head_signing-1.7/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-10-25 16:20:50.063568 rpm_head_signing-1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      468 2021-10-25 16:20:49.000000 rpm_head_signing-1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 16:20:50.063568 rpm_head_signing-1.7/rpm_head_signing/
--rw-r--r--   0 runner    (1001) docker     (121)      330 2021-10-25 16:20:49.000000 rpm_head_signing-1.7/rpm_head_signing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2282 2021-10-25 16:20:49.000000 rpm_head_signing-1.7/rpm_head_signing/determine.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2431 2021-10-25 16:20:49.000000 rpm_head_signing-1.7/rpm_head_signing/extract_header.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     4896 2021-10-25 16:20:49.000000 rpm_head_signing-1.7/rpm_head_signing/extract_rpm_with_filesigs.py
--rw-r--r--   0 runner    (1001) docker     (121)     2350 2021-10-25 16:20:49.000000 rpm_head_signing-1.7/rpm_head_signing/extract_signature_and_ima_info.py
--rw-r--r--   0 runner    (1001) docker     (121)      622 2021-10-25 16:20:49.000000 rpm_head_signing-1.7/rpm_head_signing/fix_signatures.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2695 2021-10-25 16:20:49.000000 rpm_head_signing-1.7/rpm_head_signing/insert_signature.py
--rw-r--r--   0 runner    (1001) docker     (121)    24425 2021-10-25 16:20:49.000000 rpm_head_signing-1.7/rpm_head_signing/insertlib.c
--rwxr-xr-x   0 runner    (1001) docker     (121)     7597 2021-10-25 16:20:49.000000 rpm_head_signing-1.7/rpm_head_signing/verify_rpm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-10-25 16:20:50.063568 rpm_head_signing-1.7/rpm_head_signing.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      188 2021-10-25 16:20:50.000000 rpm_head_signing-1.7/rpm_head_signing.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      544 2021-10-25 16:20:50.000000 rpm_head_signing-1.7/rpm_head_signing.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-10-25 16:20:50.000000 rpm_head_signing-1.7/rpm_head_signing.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       84 2021-10-25 16:20:50.000000 rpm_head_signing-1.7/rpm_head_signing.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       27 2021-10-25 16:20:50.000000 rpm_head_signing-1.7/rpm_head_signing.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2021-10-25 16:20:50.063568 rpm_head_signing-1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1191 2021-10-25 16:20:49.000000 rpm_head_signing-1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:57:48.991057 rpm_head_signing-1.7.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1062 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-13 20:57:48.991057 rpm_head_signing-1.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:57:48.991057 rpm_head_signing-1.7.1/rpm_head_signing/
+-rw-r--r--   0 runner    (1001) docker     (123)      330 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/rpm_head_signing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2282 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/rpm_head_signing/determine.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2442 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/rpm_head_signing/extract_header.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4896 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/rpm_head_signing/extract_rpm_with_filesigs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2350 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/rpm_head_signing/extract_signature_and_ima_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/rpm_head_signing/fix_signatures.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2695 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/rpm_head_signing/insert_signature.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24449 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/rpm_head_signing/insertlib.c
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7595 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/rpm_head_signing/verify_rpm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 20:57:48.991057 rpm_head_signing-1.7.1/rpm_head_signing.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      163 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/rpm_head_signing.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      552 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/rpm_head_signing.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/rpm_head_signing.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/rpm_head_signing.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/rpm_head_signing.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 20:57:48.991057 rpm_head_signing-1.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1193 2023-06-13 20:57:48.000000 rpm_head_signing-1.7.1/setup.py
```

### Comparing `rpm_head_signing-1.7/rpm_head_signing/determine.py` & `rpm_head_signing-1.7.1/rpm_head_signing/determine.py`

 * *Files identical despite different names*

### Comparing `rpm_head_signing-1.7/rpm_head_signing/extract_header.py` & `rpm_head_signing-1.7.1/rpm_head_signing/extract_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
     if not rawhdr.index.get(RPMTAG_PAYLOADDIGEST):
         raise NonHeaderSignablePackage("This package cannot be headersigned")
 
 
 def extract_header(input_path, header_out_path, digest_out_path):
     (sig_start, sig_size) = find_rpm_sighdr(input_path)
     hdr_start = sig_start + sig_size
-    hdr_size = rpm_hdr_size(input_path, hdr_start)
+    hdr_size = rpm_hdr_size(input_path, hdr_start, pad=False)
 
     if digest_out_path:
         rpm_hdr = get_rpm_header(input_path)
         file_digestalgo, file_digests = _get_filedigests(rpm_hdr)
         file_digests = set(file_digests)
 
     with open(input_path, "rb") as f:
```

### Comparing `rpm_head_signing-1.7/rpm_head_signing/extract_rpm_with_filesigs.py` & `rpm_head_signing-1.7.1/rpm_head_signing/extract_rpm_with_filesigs.py`

 * *Files identical despite different names*

### Comparing `rpm_head_signing-1.7/rpm_head_signing/extract_signature_and_ima_info.py` & `rpm_head_signing-1.7.1/rpm_head_signing/extract_signature_and_ima_info.py`

 * *Files identical despite different names*

### Comparing `rpm_head_signing-1.7/rpm_head_signing/fix_signatures.py` & `rpm_head_signing-1.7.1/rpm_head_signing/fix_signatures.py`

 * *Files identical despite different names*

### Comparing `rpm_head_signing-1.7/rpm_head_signing/insert_signature.py` & `rpm_head_signing-1.7.1/rpm_head_signing/insert_signature.py`

 * *Files identical despite different names*

### Comparing `rpm_head_signing-1.7/rpm_head_signing/insertlib.c` & `rpm_head_signing-1.7.1/rpm_head_signing/insertlib.c`

 * *Files 0% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #include <asm/byteorder.h>
 
 #include <rpm/rpmtypes.h>
 #include <rpm/rpmlib.h>
 #include <rpm/rpmstring.h>
 #include <rpm/rpmfileutil.h>
 #include <rpm/rpmfi.h>
+#include <rpm/rpmpgp.h>
 
 // Functions that are in librpm but are not in the headers
 // This one function is identical from 4.11 onwards...
 int rpmWriteSignature(FD_t fd, Header sigh);
 
 #if defined(RPM_415)
```

### Comparing `rpm_head_signing-1.7/rpm_head_signing/verify_rpm.py` & `rpm_head_signing-1.7.1/rpm_head_signing/verify_rpm.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,15 +112,15 @@
             logging.debug("Extracting RPM into %s...", extracted_dir)
             rpm_head_signing.extract_rpm_with_filesigs(
                 rpm_path,
                 extracted_dir,
             )
             logging.debug("Extracted RPM, verifying signatures...")
 
-            for (where, _, fnames) in os.walk(extracted_dir):
+            for where, _, fnames in os.walk(extracted_dir):
                 for fname in fnames:
                     file_path = os.path.join(where, fname)
                     if os.path.islink(file_path):
                         logging.debug("Skipping symbolic link at %s", file_path)
                         continue
                     logging.debug("Verifying file %s ...", file_path)
```

### Comparing `rpm_head_signing-1.7/rpm_head_signing.egg-info/SOURCES.txt` & `rpm_head_signing-1.7.1/rpm_head_signing.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 README.md
 setup.py
 rpm_head_signing/__init__.py
 rpm_head_signing/determine.py
 rpm_head_signing/extract_header.py
 rpm_head_signing/extract_rpm_with_filesigs.py
 rpm_head_signing/extract_signature_and_ima_info.py
```

### Comparing `rpm_head_signing-1.7/setup.py` & `rpm_head_signing-1.7.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     sources=["rpm_head_signing/insertlib.c"],
     extra_compile_args=["-Wall", "-Werror"],
     define_macros=ext_defines,
 )
 
 setup(
     name="rpm_head_signing",
-    version="1.7",
+    version="1.7.1",
     packages=["rpm_head_signing"],
     ext_package="rpm_head_signing",
     ext_modules=[insertlib],
     entry_points={
         "console_scripts": [
             "verify-rpm-ima-signatures=rpm_head_signing.verify_rpm:__main__",
         ],
```

