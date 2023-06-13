# Comparing `tmp/cirq_ft-1.2.0.dev20230611062534-py3-none-any.whl.zip` & `tmp/cirq_ft-1.2.0.dev20230613031912-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 7328 bytes, number of entries: 8
--rw-r--r--  2.0 unx      626 b- defN 23-Jun-11 06:25 cirq_ft/__init__.py
--rw-r--r--  2.0 unx       40 b- defN 23-Jun-11 06:25 cirq_ft/_version.py
--rw-r--r--  2.0 unx      696 b- defN 23-Jun-11 06:25 cirq_ft/dropme_blank_test.py
--rw-r--r--  2.0 unx    11357 b- defN 23-Jun-11 06:25 cirq_ft-1.2.0.dev20230611062534.dist-info/LICENSE
--rw-r--r--  2.0 unx     1443 b- defN 23-Jun-11 06:25 cirq_ft-1.2.0.dev20230611062534.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-11 06:25 cirq_ft-1.2.0.dev20230611062534.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jun-11 06:25 cirq_ft-1.2.0.dev20230611062534.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      709 b- defN 23-Jun-11 06:25 cirq_ft-1.2.0.dev20230611062534.dist-info/RECORD
-8 files, 14971 bytes uncompressed, 6068 bytes compressed:  59.5%
+Zip file size: 7326 bytes, number of entries: 8
+-rw-r--r--  2.0 unx      626 b- defN 23-Jun-13 03:19 cirq_ft/__init__.py
+-rw-r--r--  2.0 unx       40 b- defN 23-Jun-13 03:19 cirq_ft/_version.py
+-rw-r--r--  2.0 unx      696 b- defN 23-Jun-13 03:19 cirq_ft/dropme_blank_test.py
+-rw-r--r--  2.0 unx    11357 b- defN 23-Jun-13 03:19 cirq_ft-1.2.0.dev20230613031912.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1443 b- defN 23-Jun-13 03:19 cirq_ft-1.2.0.dev20230613031912.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-13 03:19 cirq_ft-1.2.0.dev20230613031912.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-Jun-13 03:19 cirq_ft-1.2.0.dev20230613031912.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      709 b- defN 23-Jun-13 03:19 cirq_ft-1.2.0.dev20230613031912.dist-info/RECORD
+8 files, 14971 bytes uncompressed, 6066 bytes compressed:  59.5%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: cirq_ft/_version.py
 Comment: 
 
 Filename: cirq_ft/dropme_blank_test.py
 Comment: 
 
-Filename: cirq_ft-1.2.0.dev20230611062534.dist-info/LICENSE
+Filename: cirq_ft-1.2.0.dev20230613031912.dist-info/LICENSE
 Comment: 
 
-Filename: cirq_ft-1.2.0.dev20230611062534.dist-info/METADATA
+Filename: cirq_ft-1.2.0.dev20230613031912.dist-info/METADATA
 Comment: 
 
-Filename: cirq_ft-1.2.0.dev20230611062534.dist-info/WHEEL
+Filename: cirq_ft-1.2.0.dev20230613031912.dist-info/WHEEL
 Comment: 
 
-Filename: cirq_ft-1.2.0.dev20230611062534.dist-info/top_level.txt
+Filename: cirq_ft-1.2.0.dev20230613031912.dist-info/top_level.txt
 Comment: 
 
-Filename: cirq_ft-1.2.0.dev20230611062534.dist-info/RECORD
+Filename: cirq_ft-1.2.0.dev20230613031912.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## cirq_ft/_version.py

```diff
@@ -1 +1 @@
-__version__ = "1.2.0.dev20230611062534"
+__version__ = "1.2.0.dev20230613031912"
```

## Comparing `cirq_ft-1.2.0.dev20230611062534.dist-info/LICENSE` & `cirq_ft-1.2.0.dev20230613031912.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `cirq_ft-1.2.0.dev20230611062534.dist-info/METADATA` & `cirq_ft-1.2.0.dev20230613031912.dist-info/METADATA`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: cirq-ft
-Version: 1.2.0.dev20230611062534
+Version: 1.2.0.dev20230613031912
 Summary: A Cirq package for fault-tolerant algorithms
 Home-page: http://github.com/quantumlib/cirq
 Author: The Cirq Developers
 Author-email: cirq-dev@googlegroups.com
 License: Apache 2
 Platform: UNKNOWN
 Requires-Python: >=3.7.0
-Requires-Dist: cirq-core (==1.2.0.dev20230611062534)
+Requires-Dist: cirq-core (==1.2.0.dev20230613031912)
 
 **This is a development version of Cirq-ft and may be unstable.**
 
 **For the latest stable release of Cirq-ft see**
 `here <https://pypi.org/project/cirq-ft>`__.
 
 .. image:: https://raw.githubusercontent.com/quantumlib/Cirq/master/docs/images/Cirq_logo_color.png
```

## Comparing `cirq_ft-1.2.0.dev20230611062534.dist-info/RECORD` & `cirq_ft-1.2.0.dev20230613031912.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 cirq_ft/__init__.py,sha256=-bKSYRapFilweJCnQsU1TliTfqaNAFt9sVHVujMUR9w,626
-cirq_ft/_version.py,sha256=N98u5E2zf9hFXz9U_pMrvayF3ZABRLQ5JOmaF9HIedo,40
+cirq_ft/_version.py,sha256=m_MU6Nvvwz2W1B7BB7lg_aXdT5Nj4twyW62ghaoAFak,40
 cirq_ft/dropme_blank_test.py,sha256=yshtLfaYV61ePqWkMNLHQSYSwgQDMngqwG9uvulTTwU,696
-cirq_ft-1.2.0.dev20230611062534.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
-cirq_ft-1.2.0.dev20230611062534.dist-info/METADATA,sha256=BiC47Jr6zgdzKBCCZzI3IbuScmlKLK5PCcjTkabxVug,1443
-cirq_ft-1.2.0.dev20230611062534.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-cirq_ft-1.2.0.dev20230611062534.dist-info/top_level.txt,sha256=H8KJHkgeicc6P99pLIx51PGnLymjmgmVoKeeGGZxP_M,8
-cirq_ft-1.2.0.dev20230611062534.dist-info/RECORD,,
+cirq_ft-1.2.0.dev20230613031912.dist-info/LICENSE,sha256=tAkwu8-AdEyGxGoSvJ2gVmQdcicWw3j1ZZueVV74M-E,11357
+cirq_ft-1.2.0.dev20230613031912.dist-info/METADATA,sha256=nQ7GWqFbOgyfqxW8UWfkuUtOzLjirmVjjJ8GFxgp9OE,1443
+cirq_ft-1.2.0.dev20230613031912.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+cirq_ft-1.2.0.dev20230613031912.dist-info/top_level.txt,sha256=H8KJHkgeicc6P99pLIx51PGnLymjmgmVoKeeGGZxP_M,8
+cirq_ft-1.2.0.dev20230613031912.dist-info/RECORD,,
```

