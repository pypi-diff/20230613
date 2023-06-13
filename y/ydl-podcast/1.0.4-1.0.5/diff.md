# Comparing `tmp/ydl_podcast-1.0.4.tar.gz` & `tmp/ydl_podcast-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydl_podcast-1.0.4.tar", max compression
+gzip compressed data, was "ydl_podcast-1.0.5.tar", max compression
```

## Comparing `ydl_podcast-1.0.4.tar` & `ydl_podcast-1.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1102 2023-06-12 02:15:43.271076 ydl_podcast-1.0.4/LICENSE
--rw-r--r--   0        0        0     2748 2023-06-12 02:15:43.271076 ydl_podcast-1.0.4/README.md
--rw-r--r--   0        0        0      895 2023-06-12 02:23:54.572619 ydl_podcast-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    12290 2023-06-12 02:15:43.271076 ydl_podcast-1.0.4/ydl_podcast/__init__.py
--rwxr-xr-x   0        0        0     1830 2023-06-12 02:15:43.271076 ydl_podcast-1.0.4/ydl_podcast/__main__.py
--rw-r--r--   0        0        0      990 2023-06-12 02:15:43.271076 ydl_podcast-1.0.4/ydl_podcast/template.py
--rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 ydl_podcast-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-06-12 02:15:43.271076 ydl_podcast-1.0.5/LICENSE
+-rw-r--r--   0        0        0     2748 2023-06-12 02:15:43.271076 ydl_podcast-1.0.5/README.md
+-rw-r--r--   0        0        0      895 2023-06-13 00:43:53.005552 ydl_podcast-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    12211 2023-06-13 00:43:53.005552 ydl_podcast-1.0.5/ydl_podcast/__init__.py
+-rwxr-xr-x   0        0        0     1830 2023-06-12 02:15:43.271076 ydl_podcast-1.0.5/ydl_podcast/__main__.py
+-rw-r--r--   0        0        0      990 2023-06-12 02:15:43.271076 ydl_podcast-1.0.5/ydl_podcast/template.py
+-rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 ydl_podcast-1.0.5/PKG-INFO
```

### Comparing `ydl_podcast-1.0.4/LICENSE` & `ydl_podcast-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.4/README.md` & `ydl_podcast-1.0.5/README.md`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.4/pyproject.toml` & `ydl_podcast-1.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ydl-podcast"
-version = "1.0.4"
+version = "1.0.5"
 description = "A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl"
 license = "MIT"
 authors = ["nbr23 <max@23.tf>"]
 homepage = "https://github.com/nbr23/ydl-podcast"
 repository = "https://github.com/nbr23/ydl-podcast"
 keywords = ["podcast", "youtube-dl"]
 readme = "README.md"
```

### Comparing `ydl_podcast-1.0.4/ydl_podcast/__init__.py` & `ydl_podcast-1.0.5/ydl_podcast/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -179,41 +179,38 @@
             options["format"] = sub["format"]
 
     for key in sub.get("ydl_options", {}):
         options[key] = sub["ydl_options"][key]
 
     return options
 
-def get_podcast_icon(ydl_mod, sub, metadata, options):
+def get_podcast_icon(ydl_mod, sub, metadata):
     # check if it already exists
     icon_filepath = os.path.join(sub["output_dir"], sub["name"], "icon.jpg")
     if os.path.isfile(icon_filepath):
         return
 
     # get the channel's about  metadata
     channel_url = metadata.get("uploader_url")
     if channel_url is None:
         return
-    my_options = options.copy()
-    my_options.update(
-        {
+    options =  {
         "quiet": False,
         "ignoreerrors": True,
         "extract_flat": "in_playlist",
         "writethumbnail": True,
         "filename_template": "icon.jpg",
         "outtmpl": os.path.join(
             sub["output_dir"], sub["name"], 'icon.jpg'
         ),
         "writeinfojson": False,
-        }
-    )
+    }
 
     output = io.StringIO()
-    with ydl_mod.YoutubeDL(my_options) as ydl:
+    with ydl_mod.YoutubeDL(options) as ydl:
         try:
             if hasattr(ydl, "_out_files"):
                 ydl._out_files.out = output
                 ydl._out_files.error = io.StringIO()
             else:
                 ydl._screen_file = output
                 ydl._err_file = io.StringIO()
@@ -225,15 +222,15 @@
 def download(ydl_mod, sub):
     downloaded = []
     options = process_options(ydl_mod, sub)
     metadata = get_metadata(ydl_mod, sub["url"], options, sub["quiet"])
     entries = metadata.get("entries", [])
 
     # Handle podcast icon
-    get_podcast_icon(ydl_mod, sub, metadata, options)
+    get_podcast_icon(ydl_mod, sub, metadata)
 
     # Filter out older entries
     if sub["download_last"] is not None and not sub.get("initialize", False):
         entries = entries[: sub["download_last"]]
 
     # Go through entries and download them
     for i, md in enumerate(entries):
```

### Comparing `ydl_podcast-1.0.4/ydl_podcast/__main__.py` & `ydl_podcast-1.0.5/ydl_podcast/__main__.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.4/ydl_podcast/template.py` & `ydl_podcast-1.0.5/ydl_podcast/template.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.4/PKG-INFO` & `ydl_podcast-1.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydl-podcast
-Version: 1.0.4
+Version: 1.0.5
 Summary: A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl
 Home-page: https://github.com/nbr23/ydl-podcast
 License: MIT
 Keywords: podcast,youtube-dl
 Author: nbr23
 Author-email: max@23.tf
 Requires-Python: >=3.7,<4.0
```

