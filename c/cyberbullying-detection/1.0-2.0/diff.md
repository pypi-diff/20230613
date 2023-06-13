# Comparing `tmp/cyberbullying_detection-1.0.tar.gz` & `tmp/cyberbullying_detection-2.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyberbullying_detection-1.0.tar", last modified: Fri May 26 08:04:18 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

