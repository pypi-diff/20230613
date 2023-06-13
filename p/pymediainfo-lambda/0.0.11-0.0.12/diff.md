# Comparing `tmp/pymediainfo_lambda-0.0.11-py3-none-win_amd64.whl.zip` & `tmp/pymediainfo_lambda-0.0.12-py3-none-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,18 @@
-Zip file size: 2726721 bytes, number of entries: 10
--rw-rw-rw-  2.0 fat  6588320 b- defN 22-Oct-04 17:51 pymediainfo/MediaInfo.dll
--rw-rw-rw-  2.0 fat    21461 b- defN 23-Jun-13 06:46 pymediainfo/__init__.py
--rw-rw-rw-  2.0 fat     4849 b- defN 22-Oct-04 17:31 pymediainfo_lambda-0.0.11.data/data/docs/License.html
--rw-rw-rw-  2.0 fat      143 b- defN 23-Jun-13 06:47 pymediainfo_lambda-0.0.11.dist-info/AUTHORS
--rw-rw-rw-  2.0 fat     1213 b- defN 23-Jun-13 06:47 pymediainfo_lambda-0.0.11.dist-info/LICENSE
--rw-rw-rw-  2.0 fat     2175 b- defN 23-Jun-13 06:47 pymediainfo_lambda-0.0.11.dist-info/METADATA
--rw-rw-rw-  2.0 fat       99 b- defN 23-Jun-13 06:47 pymediainfo_lambda-0.0.11.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        1 b- defN 23-Jun-13 06:47 pymediainfo_lambda-0.0.11.dist-info/namespace_packages.txt
--rw-rw-rw-  2.0 fat       12 b- defN 23-Jun-13 06:47 pymediainfo_lambda-0.0.11.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      933 b- defN 23-Jun-13 06:47 pymediainfo_lambda-0.0.11.dist-info/RECORD
-10 files, 6619206 bytes uncompressed, 2725097 bytes compressed:  58.8%
+Zip file size: 6202760 bytes, number of entries: 16
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:56 pymediainfo_lambda-0.0.12.data/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:56 pymediainfo_lambda.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:56 pymediainfo_lambda-0.0.12.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:56 pymediainfo/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:56 pymediainfo_lambda-0.0.12.data/data/
+drwxr-xr-x  2.0 unx        0 b- stor 23-Jun-13 06:56 pymediainfo_lambda-0.0.12.data/data/docs/
+-rw-r--r--  2.0 unx     1328 b- defN 23-Jun-13 06:56 pymediainfo_lambda-0.0.12.data/data/docs/LICENSE
+-rw-r--r--  2.0 unx       12 b- defN 23-Jun-13 06:56 pymediainfo_lambda-0.0.12.dist-info/top_level.txt
+-rw-r--r--  2.0 unx     2077 b- defN 23-Jun-13 06:56 pymediainfo_lambda-0.0.12.dist-info/METADATA
+-rw-r--r--  2.0 unx      146 b- defN 23-Jun-13 06:56 pymediainfo_lambda-0.0.12.dist-info/WHEEL
+-rw-r--r--  2.0 unx      143 b- defN 23-Jun-13 06:56 pymediainfo_lambda-0.0.12.dist-info/AUTHORS
+-rw-r--r--  2.0 unx     1213 b- defN 23-Jun-13 06:56 pymediainfo_lambda-0.0.12.dist-info/LICENSE
+-rw-rw-r--  2.0 unx      944 b- defN 23-Jun-13 06:56 pymediainfo_lambda-0.0.12.dist-info/RECORD
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-13 06:56 pymediainfo_lambda-0.0.12.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx    21461 b- defN 23-Jun-13 06:56 pymediainfo/__init__.py
+-rwxr-xr-x  2.0 unx 16847464 b- defN 23-Jun-13 06:56 pymediainfo/libmediainfo.so.0
+16 files, 16874789 bytes uncompressed, 6200322 bytes compressed:  63.3%
```

## zipnote {}

```diff
@@ -1,31 +1,49 @@
-Filename: pymediainfo/MediaInfo.dll
+Filename: pymediainfo_lambda-0.0.12.data/
 Comment: 
 
-Filename: pymediainfo/__init__.py
+Filename: pymediainfo_lambda.libs/
+Comment: 
+
+Filename: pymediainfo_lambda-0.0.12.dist-info/
+Comment: 
+
+Filename: pymediainfo/
+Comment: 
+
+Filename: pymediainfo_lambda-0.0.12.data/data/
 Comment: 
 
-Filename: pymediainfo_lambda-0.0.11.data/data/docs/License.html
+Filename: pymediainfo_lambda-0.0.12.data/data/docs/
 Comment: 
 
-Filename: pymediainfo_lambda-0.0.11.dist-info/AUTHORS
+Filename: pymediainfo_lambda-0.0.12.data/data/docs/LICENSE
 Comment: 
 
-Filename: pymediainfo_lambda-0.0.11.dist-info/LICENSE
+Filename: pymediainfo_lambda-0.0.12.dist-info/top_level.txt
 Comment: 
 
-Filename: pymediainfo_lambda-0.0.11.dist-info/METADATA
+Filename: pymediainfo_lambda-0.0.12.dist-info/METADATA
 Comment: 
 
-Filename: pymediainfo_lambda-0.0.11.dist-info/WHEEL
+Filename: pymediainfo_lambda-0.0.12.dist-info/WHEEL
 Comment: 
 
-Filename: pymediainfo_lambda-0.0.11.dist-info/namespace_packages.txt
+Filename: pymediainfo_lambda-0.0.12.dist-info/AUTHORS
 Comment: 
 
-Filename: pymediainfo_lambda-0.0.11.dist-info/top_level.txt
+Filename: pymediainfo_lambda-0.0.12.dist-info/LICENSE
+Comment: 
+
+Filename: pymediainfo_lambda-0.0.12.dist-info/RECORD
+Comment: 
+
+Filename: pymediainfo_lambda-0.0.12.dist-info/namespace_packages.txt
+Comment: 
+
+Filename: pymediainfo/__init__.py
 Comment: 
 
-Filename: pymediainfo_lambda-0.0.11.dist-info/RECORD
+Filename: pymediainfo/libmediainfo.so.0
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## Comparing `pymediainfo_lambda-0.0.11.dist-info/LICENSE` & `pymediainfo_lambda-0.0.12.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `pymediainfo_lambda-0.0.11.dist-info/RECORD` & `pymediainfo_lambda-0.0.12.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-pymediainfo/MediaInfo.dll,sha256=TcswXBpN5JrJ5QlR64EXbQmqCt_9UwTjSc3WsdLrhUo,6588320
-pymediainfo/__init__.py,sha256=7nNDIbacBNwkLRZzipX2pGkz-MKT0QRdEHlPOeLD6nI,21461
-pymediainfo_lambda-0.0.11.data/data/docs/License.html,sha256=rmRIMVfVTOyFpoirViJF8M7mRu3OJ-DDW3hrq4Umapk,4849
-pymediainfo_lambda-0.0.11.dist-info/AUTHORS,sha256=38KIOxhqkhfSz4gLaVoQ0g9SsvlJ7nPbflT47JTKWfw,143
-pymediainfo_lambda-0.0.11.dist-info/LICENSE,sha256=MvjTJkPHxeLn1_eZcd3exq0cAVnSbqKSS4g7jUdCgos,1213
-pymediainfo_lambda-0.0.11.dist-info/METADATA,sha256=dONP06ljFlMz90ekPrVtO4fb9Zfsg33bbbpvits4OG0,2175
-pymediainfo_lambda-0.0.11.dist-info/WHEEL,sha256=oOatfxF9lem9vgsF-QTj3e-P_rDgLCmqbWx3sLKdyrE,99
-pymediainfo_lambda-0.0.11.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pymediainfo_lambda-0.0.11.dist-info/top_level.txt,sha256=OKqFwmlXFyPK7eRKNhlIAQot6cXSsvU-BNeG19EqOpk,12
-pymediainfo_lambda-0.0.11.dist-info/RECORD,,
+pymediainfo_lambda-0.0.12.data/data/docs/LICENSE,sha256=zP47VLp4bv45iYTqOLZo04e-zDjxQF5QfgBk8udx3Uo,1328
+pymediainfo_lambda-0.0.12.dist-info/top_level.txt,sha256=OKqFwmlXFyPK7eRKNhlIAQot6cXSsvU-BNeG19EqOpk,12
+pymediainfo_lambda-0.0.12.dist-info/METADATA,sha256=tQJIerjHIbOuTtSJUSwYXioGXpJnAbEybnuzSHPsSVs,2077
+pymediainfo_lambda-0.0.12.dist-info/WHEEL,sha256=V2KjM8jRkjCA0T3Qq1khvRiuI5gyLMwf7zYUWcXbs_4,146
+pymediainfo_lambda-0.0.12.dist-info/AUTHORS,sha256=38KIOxhqkhfSz4gLaVoQ0g9SsvlJ7nPbflT47JTKWfw,143
+pymediainfo_lambda-0.0.12.dist-info/LICENSE,sha256=MvjTJkPHxeLn1_eZcd3exq0cAVnSbqKSS4g7jUdCgos,1213
+pymediainfo_lambda-0.0.12.dist-info/RECORD,,
+pymediainfo_lambda-0.0.12.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pymediainfo/__init__.py,sha256=7nNDIbacBNwkLRZzipX2pGkz-MKT0QRdEHlPOeLD6nI,21461
+pymediainfo/libmediainfo.so.0,sha256=a9Q4qdNR68Ozqc-l30mMwxJUg2I6szetcmy15Sgd33k,16847464
```

