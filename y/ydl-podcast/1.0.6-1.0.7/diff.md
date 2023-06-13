# Comparing `tmp/ydl_podcast-1.0.6.tar.gz` & `tmp/ydl_podcast-1.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydl_podcast-1.0.6.tar", max compression
+gzip compressed data, was "ydl_podcast-1.0.7.tar", max compression
```

## Comparing `ydl_podcast-1.0.6.tar` & `ydl_podcast-1.0.7.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1102 2023-06-12 02:15:43.271076 ydl_podcast-1.0.6/LICENSE
--rw-r--r--   0        0        0     2748 2023-06-12 02:15:43.271076 ydl_podcast-1.0.6/README.md
--rw-r--r--   0        0        0      895 2023-06-13 00:52:22.549108 ydl_podcast-1.0.6/pyproject.toml
--rw-r--r--   0        0        0    12211 2023-06-13 00:43:53.005552 ydl_podcast-1.0.6/ydl_podcast/__init__.py
--rwxr-xr-x   0        0        0     1830 2023-06-12 02:15:43.271076 ydl_podcast-1.0.6/ydl_podcast/__main__.py
--rw-r--r--   0        0        0      982 2023-06-13 00:52:22.553108 ydl_podcast-1.0.6/ydl_podcast/template.py
--rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 ydl_podcast-1.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-06-12 02:15:43.271076 ydl_podcast-1.0.7/LICENSE
+-rw-r--r--   0        0        0     2748 2023-06-12 02:15:43.271076 ydl_podcast-1.0.7/README.md
+-rw-r--r--   0        0        0      895 2023-06-13 13:18:24.930680 ydl_podcast-1.0.7/pyproject.toml
+-rw-r--r--   0        0        0    12630 2023-06-13 13:17:25.297576 ydl_podcast-1.0.7/ydl_podcast/__init__.py
+-rwxr-xr-x   0        0        0     1830 2023-06-12 02:15:43.271076 ydl_podcast-1.0.7/ydl_podcast/__main__.py
+-rw-r--r--   0        0        0      982 2023-06-13 00:52:22.553108 ydl_podcast-1.0.7/ydl_podcast/template.py
+-rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 ydl_podcast-1.0.7/PKG-INFO
```

### Comparing `ydl_podcast-1.0.6/LICENSE` & `ydl_podcast-1.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.6/README.md` & `ydl_podcast-1.0.7/README.md`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.6/pyproject.toml` & `ydl_podcast-1.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ydl-podcast"
-version = "1.0.6"
+version = "1.0.7"
 description = "A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl"
 license = "MIT"
 authors = ["nbr23 <max@23.tf>"]
 homepage = "https://github.com/nbr23/ydl-podcast"
 repository = "https://github.com/nbr23/ydl-podcast"
 keywords = ["podcast", "youtube-dl"]
 readme = "README.md"
```

### Comparing `ydl_podcast-1.0.6/ydl_podcast/__init__.py` & `ydl_podcast-1.0.7/ydl_podcast/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -38,23 +38,32 @@
 def metadata_file_extension(metadata, data_path, basename):
     if "audio only" in metadata["format"] and os.path.isfile(
         os.path.join(data_path, "%s.%s" % (basename, metadata["acodec"]))
     ):
         return metadata["acodec"]
     return metadata["ext"]
 
+def get_real_thumbnail_ext(metadata_path, default_ext):
+    path = os.path.dirname(metadata_path)
+    basename = ".".join(os.path.basename(metadata_path).split(".")[:-2])
+    extensions = [default_ext, "jpg", "jpeg", "png", "webp"]
+    for ext in extensions:
+        if os.path.isfile(os.path.join(path, "%s.%s" % (basename, ext))):
+            return ext
+    return default_ext
+
 
 def metadata_parse(metadata_path):
     with open(metadata_path) as metadata:
         mdjs = json.load(metadata)
         basename = ".".join(os.path.basename(metadata_path).split(".")[:-2])
         path = os.path.dirname(metadata_path)
         thumbnail_file = None
         if mdjs.get("thumbnail") is not None:
-            thumb_ext = mdjs["thumbnail"].split(".")[-1]
+            thumb_ext = get_real_thumbnail_ext(metadata_path, mdjs["thumbnail"].split(".")[-1])
             thumbnail_file = "%s.%s" % (basename, thumb_ext)
         extension = metadata_file_extension(mdjs, path, basename)
         if not os.path.isfile(os.path.join(path, "%s.%s" % (basename, extension))):
             with os.scandir(path) as directory:
                 for f in directory:
                     ext = f.name.split(".")[-1]
                     if (
```

### Comparing `ydl_podcast-1.0.6/ydl_podcast/__main__.py` & `ydl_podcast-1.0.7/ydl_podcast/__main__.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.6/ydl_podcast/template.py` & `ydl_podcast-1.0.7/ydl_podcast/template.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.6/PKG-INFO` & `ydl_podcast-1.0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydl-podcast
-Version: 1.0.6
+Version: 1.0.7
 Summary: A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl
 Home-page: https://github.com/nbr23/ydl-podcast
 License: MIT
 Keywords: podcast,youtube-dl
 Author: nbr23
 Author-email: max@23.tf
 Requires-Python: >=3.7,<4.0
```

