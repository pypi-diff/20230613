# Comparing `tmp/everinfer-0.1.7.tar.gz` & `tmp/everinfer-0.1.8-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "everinfer-0.1.7.tar", last modified: Sat Nov 26 13:03:41 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

