# Comparing `tmp/stmd-0.0b2.tar.gz` & `tmp/stmd-0.0b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stmd-0.0b2.tar", last modified: Wed May 24 06:50:17 2023, max compression
+gzip compressed data, was "stmd-0.0b3.tar", last modified: Tue Jun 13 01:41:37 2023, max compression
```

## Comparing `stmd-0.0b2.tar` & `stmd-0.0b3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-05-24 06:50:17.594716 stmd-0.0b2/
--rw-r--r--   0 anon      (1000) wheel      (998)      266 2023-05-24 06:50:17.594716 stmd-0.0b2/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)       33 2023-05-24 06:40:46.000000 stmd-0.0b2/README.md
--rw-r--r--   0 anon      (1000) wheel      (998)      455 2023-05-24 06:49:20.000000 stmd-0.0b2/pyproject.toml
--rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-05-24 06:50:17.594716 stmd-0.0b2/setup.cfg
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-05-24 06:50:17.594716 stmd-0.0b2/src/
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-05-24 06:50:17.594716 stmd-0.0b2/src/stmd/
--rw-r--r--   0 anon      (1000) wheel      (998)       23 2023-05-14 06:53:15.000000 stmd-0.0b2/src/stmd/__init__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1772 2023-05-24 06:47:16.000000 stmd-0.0b2/src/stmd/__main__.py
--rwxr-xr-x   0 anon      (1000) wheel      (998)     1139 2023-05-24 06:45:01.000000 stmd-0.0b2/src/stmd/options.py
-drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-05-24 06:50:17.594716 stmd-0.0b2/src/stmd.egg-info/
--rw-r--r--   0 anon      (1000) wheel      (998)      266 2023-05-24 06:50:17.000000 stmd-0.0b2/src/stmd.egg-info/PKG-INFO
--rw-r--r--   0 anon      (1000) wheel      (998)      249 2023-05-24 06:50:17.000000 stmd-0.0b2/src/stmd.egg-info/SOURCES.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-05-24 06:50:17.000000 stmd-0.0b2/src/stmd.egg-info/dependency_links.txt
--rw-r--r--   0 anon      (1000) wheel      (998)       44 2023-05-24 06:50:17.000000 stmd-0.0b2/src/stmd.egg-info/entry_points.txt
--rw-r--r--   0 anon      (1000) wheel      (998)        5 2023-05-24 06:50:17.000000 stmd-0.0b2/src/stmd.egg-info/top_level.txt
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-13 01:41:37.661646 stmd-0.0b3/
+-rw-r--r--   0 anon      (1000) wheel      (998)      266 2023-06-13 01:41:37.661646 stmd-0.0b3/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)       33 2023-05-24 06:40:46.000000 stmd-0.0b3/README.md
+-rw-r--r--   0 anon      (1000) wheel      (998)      438 2023-06-13 01:41:10.000000 stmd-0.0b3/pyproject.toml
+-rw-r--r--   0 anon      (1000) wheel      (998)       38 2023-06-13 01:41:37.661646 stmd-0.0b3/setup.cfg
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-13 01:41:37.658313 stmd-0.0b3/src/
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-13 01:41:37.661646 stmd-0.0b3/src/stmd/
+-rw-r--r--   0 anon      (1000) wheel      (998)       23 2023-05-14 06:53:15.000000 stmd-0.0b3/src/stmd/__init__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     2116 2023-06-13 01:40:51.000000 stmd-0.0b3/src/stmd/__main__.py
+-rwxr-xr-x   0 anon      (1000) wheel      (998)     1139 2023-05-24 06:45:01.000000 stmd-0.0b3/src/stmd/options.py
+drwxr-xr-x   0 anon      (1000) wheel      (998)        0 2023-06-13 01:41:37.661646 stmd-0.0b3/src/stmd.egg-info/
+-rw-r--r--   0 anon      (1000) wheel      (998)      266 2023-06-13 01:41:37.000000 stmd-0.0b3/src/stmd.egg-info/PKG-INFO
+-rw-r--r--   0 anon      (1000) wheel      (998)      249 2023-06-13 01:41:37.000000 stmd-0.0b3/src/stmd.egg-info/SOURCES.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        1 2023-06-13 01:41:37.000000 stmd-0.0b3/src/stmd.egg-info/dependency_links.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)       44 2023-06-13 01:41:37.000000 stmd-0.0b3/src/stmd.egg-info/entry_points.txt
+-rw-r--r--   0 anon      (1000) wheel      (998)        5 2023-06-13 01:41:37.000000 stmd-0.0b3/src/stmd.egg-info/top_level.txt
```

### Comparing `stmd-0.0b2/src/stmd/__main__.py` & `stmd-0.0b3/src/stmd/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,14 +7,29 @@
 
 
 def mkdir(asOutput: str):
     # TODO make output dir as needed
     pass
 
 
+def appendUrl(
+    asBaseUrl: str,
+    alUrls: list[str],
+    asUrl: str,
+):
+    if len(asUrl.split("://")) < 2:
+        if asUrl.startswith("/"):
+            storeUrl = asBaseUrl + asUrl
+        else:
+            storeUrl = asBaseUrl + "/" + asUrl
+    else:
+        storeUrl = asUrl
+    alUrls.append(storeUrl)
+
+
 def writeUrl(
     asUrl: str,
     asOutput: str,
     abCode: bool,
     asTitle: str = "",
 ):
     h = h2t.HTML2Text()
@@ -45,19 +60,19 @@
     response = requests.get(asBaseUrl)
     soup = BS(response.text, "html.parser")
     urls = []
     for url in soup.findAll("a"):
         if abMatch:
             try:
                 if asMatch in url["href"]:
-                    urls.append(url)
+                    appendUrl(asBaseUrl, urls, url)
             except KeyError:
                 continue
         else:
-            urls.append(url)
+            appendUrl(asBaseUrl, urls, url)
     return urls
 
 
 def main():
     args = get_opts()
     # set vars
     bScrapeAll = args.all
```

### Comparing `stmd-0.0b2/src/stmd/options.py` & `stmd-0.0b3/src/stmd/options.py`

 * *Files identical despite different names*

