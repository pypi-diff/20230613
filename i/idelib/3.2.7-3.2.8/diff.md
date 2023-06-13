# Comparing `tmp/idelib-3.2.7.tar.gz` & `tmp/idelib-3.2.8-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idelib-3.2.7.tar", last modified: Tue Dec 13 21:46:05 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

