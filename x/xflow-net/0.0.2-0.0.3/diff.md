# Comparing `tmp/xflow-net-0.0.2.tar.gz` & `tmp/xflow_net-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xflow-net-0.0.2.tar", last modified: Tue Jun 13 15:06:00 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

