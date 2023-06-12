# Comparing `tmp/unigui-1.5.0.tar.gz` & `tmp/unigui-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unigui-1.5.0.tar", last modified: Sun Jun 11 15:00:39 2023, max compression
+gzip compressed data, was "dist/unigui-1.5.1.tar", last modified: Mon Jun 12 23:15:48 2023, max compression
```

## Comparing `unigui-1.5.0.tar` & `unigui-1.5.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui/
--rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.5.0/unigui/manager.py
--rw-rw-r--   0 george    (1000) george    (1000)     8604 2023-06-11 00:11:43.000000 unigui-1.5.0/unigui/guielements.py
--rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.5.0/unigui/userset.py
--rw-rw-r--   0 george    (1000) george    (1000)     3654 2023-06-11 14:56:41.000000 unigui-1.5.0/unigui/server.py
--rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.5.0/unigui/__init__.py
--rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.5.0/unigui/utils.py
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui/web/
--rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/favicon.ico
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui/web/css/
--rw-rw-r--   0 george    (1000) george    (1000)        0 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/css/app.31d6cfe0.css
--rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/css/523.c9159919.css
--rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/css/vendor.49a52e8f.css
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui/web/icons/
--rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/icons/favicon-96x96.png
--rw-rw-r--   0 george    (1000) george    (1000)      859 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/icons/favicon-16x16.png
--rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/icons/favicon-32x32.png
--rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/icons/favicon-128x128.png
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui/web/fonts/
--rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
--rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
--rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
--rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui/web/js/
--rw-rw-r--   0 george    (1000) george    (1000)    43017 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/js/523.37de2173.js
--rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/js/430.591e9a73.js
--rw-rw-r--   0 george    (1000) george    (1000)     5868 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/js/app.44bf7c5c.js
--rw-rw-r--   0 george    (1000) george    (1000)      763 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/js/193.283445be.js
--rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/js/vendor.3e8714c2.js
--rw-rw-r--   0 george    (1000) george    (1000)      907 2023-06-11 14:19:27.000000 unigui-1.5.0/unigui/web/index.html
--rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.5.0/LICENSE
--rw-rw-r--   0 george    (1000) george    (1000)      585 2023-06-11 14:59:42.000000 unigui-1.5.0/setup.py
--rw-rw-r--   0 george    (1000) george    (1000)    19452 2023-06-11 15:00:39.000000 unigui-1.5.0/PKG-INFO
--rw-rw-r--   0 george    (1000) george    (1000)       38 2023-06-11 15:00:39.000000 unigui-1.5.0/setup.cfg
--rw-rw-r--   0 george    (1000) george    (1000)    19162 2023-05-24 11:05:25.000000 unigui-1.5.0/README.md
--rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.5.0/MANIFEST.in
-drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui.egg-info/
--rw-rw-r--   0 george    (1000) george    (1000)       30 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui.egg-info/requires.txt
--rw-r--r--   0 george    (1000) george    (1000)        1 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui.egg-info/dependency_links.txt
--rw-r--r--   0 george    (1000) george    (1000)    19452 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui.egg-info/PKG-INFO
--rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.5.0/unigui.egg-info/not-zip-safe
--rw-r--r--   0 george    (1000) george    (1000)     1223 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui.egg-info/SOURCES.txt
--rw-r--r--   0 george    (1000) george    (1000)        7 2023-06-11 15:00:39.000000 unigui-1.5.0/unigui.egg-info/top_level.txt
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:15:48.000000 unigui-1.5.1/
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:15:48.000000 unigui-1.5.1/unigui/
+-rw-r--r--   0 george    (1000) george    (1000)    13618 2022-05-05 16:57:28.000000 unigui-1.5.1/unigui/manager.py
+-rw-rw-r--   0 george    (1000) george    (1000)     9105 2023-06-12 23:03:24.000000 unigui-1.5.1/unigui/guielements.py
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2020-12-07 05:58:08.000000 unigui-1.5.1/unigui/userset.py
+-rw-rw-r--   0 george    (1000) george    (1000)     3654 2023-06-11 14:56:41.000000 unigui-1.5.1/unigui/server.py
+-rw-rw-r--   0 george    (1000) george    (1000)      132 2022-02-12 20:42:49.000000 unigui-1.5.1/unigui/__init__.py
+-rw-r--r--   0 george    (1000) george    (1000)     2579 2021-11-25 07:29:21.000000 unigui-1.5.1/unigui/utils.py
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:15:48.000000 unigui-1.5.1/unigui/web/
+-rw-rw-r--   0 george    (1000) george    (1000)    64483 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/favicon.ico
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:15:48.000000 unigui-1.5.1/unigui/web/css/
+-rw-rw-r--   0 george    (1000) george    (1000)        0 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/css/app.31d6cfe0.css
+-rw-rw-r--   0 george    (1000) george    (1000)   219590 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/css/vendor.49a52e8f.css
+-rw-rw-r--   0 george    (1000) george    (1000)     3267 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/css/361.c9159919.css
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:15:48.000000 unigui-1.5.1/unigui/web/icons/
+-rw-rw-r--   0 george    (1000) george    (1000)     9643 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/icons/favicon-96x96.png
+-rw-rw-r--   0 george    (1000) george    (1000)      859 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/icons/favicon-16x16.png
+-rw-rw-r--   0 george    (1000) george    (1000)     2039 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/icons/favicon-32x32.png
+-rw-rw-r--   0 george    (1000) george    (1000)    12324 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/icons/favicon-128x128.png
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:15:48.000000 unigui-1.5.1/unigui/web/fonts/
+-rw-rw-r--   0 george    (1000) george    (1000)   164912 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20344 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20416 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20408 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20424 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
+-rw-rw-r--   0 george    (1000) george    (1000)    20544 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
+-rw-rw-r--   0 george    (1000) george    (1000)   128360 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
+-rw-rw-r--   0 george    (1000) george    (1000)    20436 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:15:48.000000 unigui-1.5.1/unigui/web/js/
+-rw-rw-r--   0 george    (1000) george    (1000)    43129 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/js/361.78add75c.js
+-rw-rw-r--   0 george    (1000) george    (1000)     6560 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/js/430.591e9a73.js
+-rw-rw-r--   0 george    (1000) george    (1000)     5867 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/js/app.6ab35062.js
+-rw-rw-r--   0 george    (1000) george    (1000)      763 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/js/193.283445be.js
+-rw-rw-r--   0 george    (1000) george    (1000)  1431597 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/js/vendor.3e8714c2.js
+-rw-rw-r--   0 george    (1000) george    (1000)      907 2023-06-12 23:10:20.000000 unigui-1.5.1/unigui/web/index.html
+-rw-r--r--   0 george    (1000) george    (1000)     1073 2020-12-06 13:19:46.000000 unigui-1.5.1/LICENSE
+-rw-rw-r--   0 george    (1000) george    (1000)      585 2023-06-12 23:15:37.000000 unigui-1.5.1/setup.py
+-rw-rw-r--   0 george    (1000) george    (1000)    19452 2023-06-12 23:15:48.000000 unigui-1.5.1/PKG-INFO
+-rw-rw-r--   0 george    (1000) george    (1000)       38 2023-06-12 23:15:48.000000 unigui-1.5.1/setup.cfg
+-rw-rw-r--   0 george    (1000) george    (1000)    19162 2023-05-24 11:05:25.000000 unigui-1.5.1/README.md
+-rw-rw-r--   0 george    (1000) george    (1000)       43 2021-04-23 05:55:14.000000 unigui-1.5.1/MANIFEST.in
+drwxrwxr-x   0 george    (1000) george    (1000)        0 2023-06-12 23:15:48.000000 unigui-1.5.1/unigui.egg-info/
+-rw-rw-r--   0 george    (1000) george    (1000)       30 2023-06-12 23:15:48.000000 unigui-1.5.1/unigui.egg-info/requires.txt
+-rw-r--r--   0 george    (1000) george    (1000)        1 2023-06-12 23:15:48.000000 unigui-1.5.1/unigui.egg-info/dependency_links.txt
+-rw-r--r--   0 george    (1000) george    (1000)    19452 2023-06-12 23:15:48.000000 unigui-1.5.1/unigui.egg-info/PKG-INFO
+-rw-r--r--   0 george    (1000) george    (1000)        1 2020-12-06 17:27:14.000000 unigui-1.5.1/unigui.egg-info/not-zip-safe
+-rw-r--r--   0 george    (1000) george    (1000)     1223 2023-06-12 23:15:48.000000 unigui-1.5.1/unigui.egg-info/SOURCES.txt
+-rw-r--r--   0 george    (1000) george    (1000)        7 2023-06-12 23:15:48.000000 unigui-1.5.1/unigui.egg-info/top_level.txt
```

### Comparing `unigui-1.5.0/unigui/manager.py` & `unigui-1.5.1/unigui/manager.py`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/guielements.py` & `unigui-1.5.1/unigui/guielements.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,14 +27,27 @@
         if hasattr(self, 'changed'):
             self.changed(self, value)
         else:
             self.value = value
 
 Line = Gui("Line", type = 'line')
 
+def smart_complete(lst, min_input_length = 2, max_output_length = 10):
+    di = {it: it.lower() for it in lst}
+    def complete(gui, ustr):
+        if len(ustr) < min_input_length:
+            return []
+        ustr = ustr.lower()
+        arr = [(itlow.find(ustr), it) for it, itlow in di.items() if itlow.find(ustr) != -1]
+        arr.sort(key=lambda e: e[0])
+        if len(arr) > max_output_length:
+            arr = arr[: max_output_length]
+        return [e[1] for e in arr]
+    return complete
+
 class Edit(Gui):
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)        
         if 'type' not in kwargs:
             self.type =  'autoedit' if 'complete' in kwargs else 'edit'
         self.check('value')
```

### Comparing `unigui-1.5.0/unigui/server.py` & `unigui-1.5.1/unigui/server.py`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/utils.py` & `unigui-1.5.1/unigui/utils.py`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/favicon.ico` & `unigui-1.5.1/unigui/web/favicon.ico`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/css/523.c9159919.css` & `unigui-1.5.1/unigui/web/css/361.c9159919.css`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/css/vendor.49a52e8f.css` & `unigui-1.5.1/unigui/web/css/vendor.49a52e8f.css`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/icons/favicon-96x96.png` & `unigui-1.5.1/unigui/web/icons/favicon-96x96.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/icons/favicon-16x16.png` & `unigui-1.5.1/unigui/web/icons/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/icons/favicon-32x32.png` & `unigui-1.5.1/unigui/web/icons/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/icons/favicon-128x128.png` & `unigui-1.5.1/unigui/web/icons/favicon-128x128.png`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff` & `unigui-1.5.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff` & `unigui-1.5.1/unigui/web/fonts/KFOmCnqEu92Fr1Mu4mxM.f1e2a767.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff` & `unigui-1.5.1/unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff` & `unigui-1.5.1/unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff` & `unigui-1.5.1/unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff` & `unigui-1.5.1/unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2` & `unigui-1.5.1/unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff` & `unigui-1.5.1/unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/js/523.37de2173.js` & `unigui-1.5.1/unigui/web/js/361.78add75c.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -1,11 +1,11 @@
 "use strict";
 (globalThis["webpackChunkuniqua"] = globalThis["webpackChunkuniqua"] || []).push([
-    [523], {
-        1523: (e, t, a) => {
+    [361], {
+        361: (e, t, a) => {
             a.r(t), a.d(t, {
                 default: () => Gt
             });
             var l = a(3673),
                 s = a(2323);
             const i = (0, l._)("div", {
                 class: "q-pa-lg"
@@ -1163,15 +1163,15 @@
                     },
                     append() {
                         let e = this.data.rows,
                             t = e.length,
                             a = this;
                         z(this, [t, this.search], (function(l) {
                             if (!Array.isArray(l)) return h.error(l);
-                            p && console.log("added row", l), a.search = "", a.data.value = t, e.push(l), setTimeout((() => {
+                            p && console.log("added row", l), a.search = "", e.push(l), setTimeout((() => {
                                 let e = a.rows;
                                 a.selected = [e[t]], a.showSelected(), a.editMode || a.switchEdit(), a.select(e[t], 0)
                             }), 100)
                         }), "+")
                     },
                     showSelected() {
                         let e = this.$refs.table;
@@ -1203,15 +1203,16 @@
                             for (let t of this.selected) e.splice(t.iiid, 1)
                         }
                         this.selected = []
                     }
                 },
                 watch: {
                     selected(e) {
-                        Ae(this.updated, this.selected) || (this.sendMessage("=", this.value), this.updated = this.selected), this.data.show && this.showSelected()
+                        const t = this.data;
+                        Ae(this.updated, this.selected) || (this.sendMessage("=", this.selected.length ? this.selected[0].iiid : null), this.updated = this.selected), t.show && (this.showSelected(), t.show = !1), this.editMode && this.selected.length && (t.value = this.selected[0].iiid)
                     }
                 },
                 computed: {
                     redit() {
                         return console.log("redit", this.editMode && this.selected.length ? this.selected[0].iiid : null), this.editMode && this.selected.length ? this.selected[0].iiid : null
                     },
                     editable() {
```

### Comparing `unigui-1.5.0/unigui/web/js/430.591e9a73.js` & `unigui-1.5.1/unigui/web/js/430.591e9a73.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/js/app.44bf7c5c.js` & `unigui-1.5.1/unigui/web/js/app.6ab35062.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -22,15 +22,15 @@
                         ["render", l]
                     ]),
                     d = c;
                 var p = r(3340),
                     f = r(8339);
                 const h = [{
                         path: "/",
-                        component: () => Promise.all([r.e(736), r.e(523)]).then(r.bind(r, 1523)),
+                        component: () => Promise.all([r.e(736), r.e(361)]).then(r.bind(r, 361)),
                         children: [{
                             path: "",
                             component: () => Promise.all([r.e(736), r.e(430)]).then(r.bind(r, 6430))
                         }]
                     }, {
                         path: "/:catchAll(.*)*",
                         component: () => Promise.all([r.e(736), r.e(193)]).then(r.bind(r, 2193))
@@ -159,24 +159,24 @@
             })
         }
     })(), (() => {
         r.f = {}, r.e = e => Promise.all(Object.keys(r.f).reduce(((t, n) => (r.f[n](e, t), t)), []))
     })(), (() => {
         r.u = e => "js/" + e + "." + {
             193: "283445be",
-            430: "591e9a73",
-            523: "37de2173"
+            361: "78add75c",
+            430: "591e9a73"
         } [e] + ".js"
     })(), (() => {
         r.miniCssF = e => "css/" + ({
             143: "app",
             736: "vendor"
         } [e] || e) + "." + {
             143: "31d6cfe0",
-            523: "c9159919",
+            361: "c9159919",
             736: "49a52e8f"
         } [e] + ".css"
     })(), (() => {
         r.g = function() {
             if ("object" === typeof globalThis) return globalThis;
             try {
                 return this || new Function("return this")()
@@ -260,15 +260,15 @@
                 e(n, l, o, a)
             })),
             o = {
                 143: 0
             };
         r.f.miniCss = (e, t) => {
             var r = {
-                523: 1
+                361: 1
             };
             o[e] ? t.push(o[e]) : 0 !== o[e] && r[e] && t.push(o[e] = n(e).then((() => {
                 o[e] = 0
             }), (t => {
                 throw delete o[e], t
             })))
         }
```

### Comparing `unigui-1.5.0/unigui/web/js/193.283445be.js` & `unigui-1.5.1/unigui/web/js/193.283445be.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/js/vendor.3e8714c2.js` & `unigui-1.5.1/unigui/web/js/vendor.3e8714c2.js`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui/web/index.html` & `unigui-1.5.1/unigui/web/index.html`

 * *Files 2% similar despite different names*

```diff
@@ -1 +1 @@
-<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.44bf7c5c.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
+<!DOCTYPE html><html><head><title>Unigui</title><meta charset=utf-8><meta name=description content="Unigui on Quasar"><meta name=format-detection content="telephone=no"><meta name=msapplication-tap-highlight content=no><meta name=viewport content="user-scalable=no,initial-scale=1,maximum-scale=1,minimum-scale=1,width=device-width"><link rel=icon type=image/png sizes=128x128 href=icons/favicon-128x128.png><link rel=icon type=image/png sizes=96x96 href=icons/favicon-96x96.png><link rel=icon type=image/png sizes=32x32 href=icons/favicon-32x32.png><link rel=icon type=image/png sizes=16x16 href=icons/favicon-16x16.png><link rel=icon type=image/ico href=favicon.ico><script defer src=js/vendor.3e8714c2.js></script><script defer src=js/app.6ab35062.js></script><link href=css/vendor.49a52e8f.css rel=stylesheet><link href=css/app.31d6cfe0.css rel=stylesheet></head><body><div id=q-app></div></body></html>
```

### Comparing `unigui-1.5.0/LICENSE` & `unigui-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/setup.py` & `unigui-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
  
 setup(name='unigui',
-      version='1.5.0',      
+      version='1.5.1',      
       license='MIT',
       author='Georgii Dernovyi',
       author_email='g.dernovoy@gmail.com',
       description='Unigui - Universal app browser',
       packages=find_packages(exclude=['tests']),
       long_description=open('README.md').read(),
       long_description_content_type="text/markdown",
```

### Comparing `unigui-1.5.0/PKG-INFO` & `unigui-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.5.0
+Version: 1.5.1
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.5.0/README.md` & `unigui-1.5.1/README.md`

 * *Files identical despite different names*

### Comparing `unigui-1.5.0/unigui.egg-info/PKG-INFO` & `unigui-1.5.1/unigui.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unigui
-Version: 1.5.0
+Version: 1.5.1
 Summary: Unigui - Universal app browser
 Home-page: https://github.com/Claus1/unigui
 Author: Georgii Dernovyi
 Author-email: g.dernovoy@gmail.com
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `unigui-1.5.0/unigui.egg-info/SOURCES.txt` & `unigui-1.5.1/unigui.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 unigui.egg-info/SOURCES.txt
 unigui.egg-info/dependency_links.txt
 unigui.egg-info/not-zip-safe
 unigui.egg-info/requires.txt
 unigui.egg-info/top_level.txt
 unigui/web/favicon.ico
 unigui/web/index.html
-unigui/web/css/523.c9159919.css
+unigui/web/css/361.c9159919.css
 unigui/web/css/app.31d6cfe0.css
 unigui/web/css/vendor.49a52e8f.css
 unigui/web/fonts/KFOkCnqEu92Fr1MmgVxIIzQ.68bb21d0.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmEU9fBBc-.48af7707.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmSU5fBBc-.c2f7ab22.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmWUlfBBc-.77ecb942.woff
 unigui/web/fonts/KFOlCnqEu92Fr1MmYUtfBBc-.f5677eb2.woff
@@ -28,11 +28,11 @@
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNa.4d73cb90.woff
 unigui/web/fonts/flUhRq6tzZclQEJ-Vdg-IuiaDsNcIhQ8tQ.0383092b.woff2
 unigui/web/icons/favicon-128x128.png
 unigui/web/icons/favicon-16x16.png
 unigui/web/icons/favicon-32x32.png
 unigui/web/icons/favicon-96x96.png
 unigui/web/js/193.283445be.js
+unigui/web/js/361.78add75c.js
 unigui/web/js/430.591e9a73.js
-unigui/web/js/523.37de2173.js
-unigui/web/js/app.44bf7c5c.js
+unigui/web/js/app.6ab35062.js
 unigui/web/js/vendor.3e8714c2.js
```

