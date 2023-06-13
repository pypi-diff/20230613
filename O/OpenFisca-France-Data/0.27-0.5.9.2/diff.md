# Comparing `tmp/OpenFisca-France-Data-0.27.tar.gz` & `tmp/OpenFisca_France_Data-0.5.9.2-py2-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "OpenFisca-France-Data-0.27.tar", last modified: Tue Jun 13 07:29:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

