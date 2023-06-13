# Comparing `tmp/webargs-sanic-2.2.0.tar.gz` & `tmp/webargs_sanic-2.3.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webargs-sanic-2.2.0.tar", last modified: Sun Oct 17 14:39:56 2021, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

