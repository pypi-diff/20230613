# Comparing `tmp/duckdb-0.8.1.dev477.tar.gz` & `tmp/duckdb-0.8.1.dev480-cp310-cp310-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/duckdb-0.8.1.dev477.tar", last modified: Mon Jun 12 03:24:38 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

