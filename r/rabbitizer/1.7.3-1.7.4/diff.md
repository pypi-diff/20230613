# Comparing `tmp/rabbitizer-1.7.3.tar.gz` & `tmp/rabbitizer-1.7.4-cp37-cp37m-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rabbitizer-1.7.3.tar", last modified: Sat Jun 10 14:55:16 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

