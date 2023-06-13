# Comparing `tmp/ydl_podcast-1.0.5.tar.gz` & `tmp/ydl_podcast-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ydl_podcast-1.0.5.tar", max compression
+gzip compressed data, was "ydl_podcast-1.0.6.tar", max compression
```

## Comparing `ydl_podcast-1.0.5.tar` & `ydl_podcast-1.0.6.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1102 2023-06-12 02:15:43.271076 ydl_podcast-1.0.5/LICENSE
--rw-r--r--   0        0        0     2748 2023-06-12 02:15:43.271076 ydl_podcast-1.0.5/README.md
--rw-r--r--   0        0        0      895 2023-06-13 00:43:53.005552 ydl_podcast-1.0.5/pyproject.toml
--rw-r--r--   0        0        0    12211 2023-06-13 00:43:53.005552 ydl_podcast-1.0.5/ydl_podcast/__init__.py
--rwxr-xr-x   0        0        0     1830 2023-06-12 02:15:43.271076 ydl_podcast-1.0.5/ydl_podcast/__main__.py
--rw-r--r--   0        0        0      990 2023-06-12 02:15:43.271076 ydl_podcast-1.0.5/ydl_podcast/template.py
--rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 ydl_podcast-1.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-06-12 02:15:43.271076 ydl_podcast-1.0.6/LICENSE
+-rw-r--r--   0        0        0     2748 2023-06-12 02:15:43.271076 ydl_podcast-1.0.6/README.md
+-rw-r--r--   0        0        0      895 2023-06-13 00:52:22.549108 ydl_podcast-1.0.6/pyproject.toml
+-rw-r--r--   0        0        0    12211 2023-06-13 00:43:53.005552 ydl_podcast-1.0.6/ydl_podcast/__init__.py
+-rwxr-xr-x   0        0        0     1830 2023-06-12 02:15:43.271076 ydl_podcast-1.0.6/ydl_podcast/__main__.py
+-rw-r--r--   0        0        0      982 2023-06-13 00:52:22.553108 ydl_podcast-1.0.6/ydl_podcast/template.py
+-rw-r--r--   0        0        0     3836 1970-01-01 00:00:00.000000 ydl_podcast-1.0.6/PKG-INFO
```

### Comparing `ydl_podcast-1.0.5/LICENSE` & `ydl_podcast-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.5/README.md` & `ydl_podcast-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.5/pyproject.toml` & `ydl_podcast-1.0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ydl-podcast"
-version = "1.0.5"
+version = "1.0.6"
 description = "A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl"
 license = "MIT"
 authors = ["nbr23 <max@23.tf>"]
 homepage = "https://github.com/nbr23/ydl-podcast"
 repository = "https://github.com/nbr23/ydl-podcast"
 keywords = ["podcast", "youtube-dl"]
 readme = "README.md"
```

### Comparing `ydl_podcast-1.0.5/ydl_podcast/__init__.py` & `ydl_podcast-1.0.6/ydl_podcast/__init__.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.5/ydl_podcast/__main__.py` & `ydl_podcast-1.0.6/ydl_podcast/__main__.py`

 * *Files identical despite different names*

### Comparing `ydl_podcast-1.0.5/ydl_podcast/template.py` & `ydl_podcast-1.0.6/ydl_podcast/template.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ATOM_TMPL = """<?xml version="1.0"?>
 <rss version="2.0" xmlns:itunes="http://www.itunes.com/dtds/podcast-1.0.dtd">
   <channel>
     <updated>{{ last_update }}</updated>
     <title>{{ channel_title }}</title>
     <link href="{{ channel_link }}" rel="self" type="application/rss+xml"/>
-    {% if icon_url != None %}
+    {% if icon_url %}
     <itunes:image href="{{ icon_url }}"/>
     {% endif %}
 
 
 {% for item in items %}
     <item>
       <id>{{ item.id }}</id>
```

#### html2text {}

```diff
@@ -1,6 +1,6 @@
 ATOM_TMPL = """<?xml version="1.0"?>   {{ last_update }}
- {% if icon_url != None %}  {% endif %} {% for item in items %}  {{ item.id }}
+ {% if icon_url %}  {% endif %} {% for item in items %}  {{ item.id }}
  {% if item.pubDate != None %}{{ item.pubDate }}{% endif %} {% if
 item.thumbnail != None %}{% endif %} {% if item.description != None %}
 CDATA[{{ item.description }}]]> {% endif %} {% if item.duration != None %}{
 { item.duration }}{% endif %}  {% endfor %}   """
```

### Comparing `ydl_podcast-1.0.5/PKG-INFO` & `ydl_podcast-1.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ydl-podcast
-Version: 1.0.5
+Version: 1.0.6
 Summary: A simple tool to generate Podcast-like RSS feeds from youtube (or other youtube-dl supported services) channels, using youtube-dl
 Home-page: https://github.com/nbr23/ydl-podcast
 License: MIT
 Keywords: podcast,youtube-dl
 Author: nbr23
 Author-email: max@23.tf
 Requires-Python: >=3.7,<4.0
```

