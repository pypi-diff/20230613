# Comparing `tmp/grpcio-channelz-1.55.0rc1.tar.gz` & `tmp/grpcio_channelz-1.56.0rc2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grpcio-channelz-1.55.0rc1.tar", last modified: Wed Apr 26 10:35:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

