# Comparing `tmp/diveplane-reactor-api-2.4.3.tar.gz` & `tmp/diveplane_reactor_api-2.5.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "diveplane-reactor-api-2.4.3.tar", last modified: Thu Jun  8 06:55:46 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

