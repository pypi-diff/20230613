# Comparing `tmp/python_calamine-0.1.2.tar.gz` & `tmp/python_calamine-0.1.3-pp39-pypy39_pp73-macosx_10_7_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

