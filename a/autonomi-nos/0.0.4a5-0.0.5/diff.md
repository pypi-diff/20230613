# Comparing `tmp/autonomi-nos-0.0.4a5.tar.gz` & `tmp/autonomi_nos-0.0.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autonomi-nos-0.0.4a5.tar", last modified: Tue May 30 19:24:33 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

