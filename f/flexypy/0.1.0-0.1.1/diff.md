# Comparing `tmp/flexypy-0.1.0.tar.gz` & `tmp/flexypy-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexypy-0.1.0.tar", last modified: Mon Jun 12 15:52:02 2023, max compression
+gzip compressed data, was "flexypy-0.1.1.tar", last modified: Tue Jun 13 18:31:49 2023, max compression
```

## Comparing `flexypy-0.1.0.tar` & `flexypy-0.1.1.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.266679 flexypy-0.1.0/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-06-12 15:52:02.266679 flexypy-0.1.0/PKG-INFO
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.230679 flexypy-0.1.0/flexypy/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:08:21.000000 flexypy-0.1.0/flexypy/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      211 2023-04-16 08:03:04.000000 flexypy-0.1.0/flexypy/cli.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.254679 flexypy-0.1.0/flexypy/exceptions/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:11.000000 flexypy-0.1.0/flexypy/exceptions/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      222 2023-04-13 06:56:05.000000 flexypy-0.1.0/flexypy/exceptions/baseexceptions.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      250 2023-04-17 09:30:54.000000 flexypy-0.1.0/flexypy/exceptions/extension.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      238 2023-04-17 10:37:47.000000 flexypy-0.1.0/flexypy/exceptions/render.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      263 2023-04-14 07:24:29.000000 flexypy-0.1.0/flexypy/exceptions/routing.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:25.000000 flexypy-0.1.0/flexypy/exceptions/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.254679 flexypy-0.1.0/flexypy/exceptions/web/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:56:03.000000 flexypy-0.1.0/flexypy/exceptions/web/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      128 2023-04-13 07:16:15.000000 flexypy-0.1.0/flexypy/exceptions/web/baseexseptions.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      583 2023-04-13 07:27:17.000000 flexypy-0.1.0/flexypy/exceptions/web/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.254679 flexypy-0.1.0/flexypy/generate_templates/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:53:58.000000 flexypy-0.1.0/flexypy/generate_templates/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      953 2023-04-27 09:44:58.000000 flexypy-0.1.0/flexypy/generate_templates/generator.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.254679 flexypy-0.1.0/flexypy/generate_templates/templates/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-16 08:46:07.000000 flexypy-0.1.0/flexypy/generate_templates/templates/__init__.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.262679 flexypy-0.1.0/flexypy/generate_templates/templates/config/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:54:20.000000 flexypy-0.1.0/flexypy/generate_templates/templates/config/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       86 2023-04-23 08:22:28.000000 flexypy-0.1.0/flexypy/generate_templates/templates/config/apps.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      209 2023-04-15 14:55:12.000000 flexypy-0.1.0/flexypy/generate_templates/templates/config/dirs.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      201 2023-04-23 08:23:04.000000 flexypy-0.1.0/flexypy/generate_templates/templates/main.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.266679 flexypy-0.1.0/flexypy/http/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:09:44.000000 flexypy-0.1.0/flexypy/http/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      992 2023-04-22 20:19:57.000000 flexypy-0.1.0/flexypy/http/cookie.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     2552 2023-06-12 15:43:55.000000 flexypy-0.1.0/flexypy/http/request.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     2645 2023-04-27 09:44:59.000000 flexypy-0.1.0/flexypy/http/routing.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)    10059 2023-06-12 15:35:09.000000 flexypy-0.1.0/flexypy/http/server.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.266679 flexypy-0.1.0/flexypy/http/template/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 14:52:16.000000 flexypy-0.1.0/flexypy/http/template/__init__.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.266679 flexypy-0.1.0/flexypy/http/template/extensions/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 16:12:24.000000 flexypy-0.1.0/flexypy/http/template/extensions/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      764 2023-04-27 09:44:58.000000 flexypy-0.1.0/flexypy/http/template/extensions/base_extension.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      548 2023-04-17 09:32:56.000000 flexypy-0.1.0/flexypy/http/template/extensions/template_ext.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     3368 2023-04-17 10:37:47.000000 flexypy-0.1.0/flexypy/http/template/render.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.266679 flexypy-0.1.0/flexypy/middlewares/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 09:42:14.000000 flexypy-0.1.0/flexypy/middlewares/__init__.py
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      327 2023-04-15 11:09:28.000000 flexypy-0.1.0/flexypy/middlewares/mddl.py
-drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-12 15:52:02.250679 flexypy-0.1.0/flexypy.egg-info/
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-06-12 15:52:02.000000 flexypy-0.1.0/flexypy.egg-info/PKG-INFO
--rw-rw-r--   0 uwine     (1000) uwine     (1000)     1223 2023-06-12 15:52:02.000000 flexypy-0.1.0/flexypy.egg-info/SOURCES.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        1 2023-06-12 15:52:02.000000 flexypy-0.1.0/flexypy.egg-info/dependency_links.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       34 2023-06-12 15:52:02.000000 flexypy-0.1.0/flexypy.egg-info/requires.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)        8 2023-06-12 15:52:02.000000 flexypy-0.1.0/flexypy.egg-info/top_level.txt
--rw-rw-r--   0 uwine     (1000) uwine     (1000)      405 2023-06-12 15:47:57.000000 flexypy-0.1.0/pyproject.toml
--rw-rw-r--   0 uwine     (1000) uwine     (1000)       38 2023-06-12 15:52:02.266679 flexypy-0.1.0/setup.cfg
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-13 18:31:49.584196 flexypy-0.1.1/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-06-13 18:31:49.584196 flexypy-0.1.1/PKG-INFO
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-13 18:31:49.320128 flexypy-0.1.1/flexypy/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:08:21.000000 flexypy-0.1.1/flexypy/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      211 2023-04-16 08:03:04.000000 flexypy-0.1.1/flexypy/cli.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-13 18:31:49.436158 flexypy-0.1.1/flexypy/exceptions/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:11.000000 flexypy-0.1.1/flexypy/exceptions/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      222 2023-04-13 06:56:05.000000 flexypy-0.1.1/flexypy/exceptions/baseexceptions.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      250 2023-04-17 09:30:54.000000 flexypy-0.1.1/flexypy/exceptions/extension.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      238 2023-04-17 10:37:47.000000 flexypy-0.1.1/flexypy/exceptions/render.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      263 2023-04-14 07:24:29.000000 flexypy-0.1.1/flexypy/exceptions/routing.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:52:25.000000 flexypy-0.1.1/flexypy/exceptions/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-13 18:31:49.436158 flexypy-0.1.1/flexypy/exceptions/web/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-13 06:56:03.000000 flexypy-0.1.1/flexypy/exceptions/web/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      128 2023-04-13 07:16:15.000000 flexypy-0.1.1/flexypy/exceptions/web/baseexseptions.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      583 2023-04-13 07:27:17.000000 flexypy-0.1.1/flexypy/exceptions/web/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-13 18:31:49.452162 flexypy-0.1.1/flexypy/generate_templates/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:53:58.000000 flexypy-0.1.1/flexypy/generate_templates/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      953 2023-04-27 09:44:58.000000 flexypy-0.1.1/flexypy/generate_templates/generator.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-13 18:31:49.464165 flexypy-0.1.1/flexypy/generate_templates/templates/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-16 08:46:07.000000 flexypy-0.1.1/flexypy/generate_templates/templates/__init__.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-13 18:31:49.484171 flexypy-0.1.1/flexypy/generate_templates/templates/config/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 14:54:20.000000 flexypy-0.1.1/flexypy/generate_templates/templates/config/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       86 2023-04-23 08:22:28.000000 flexypy-0.1.1/flexypy/generate_templates/templates/config/apps.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      209 2023-04-15 14:55:12.000000 flexypy-0.1.1/flexypy/generate_templates/templates/config/dirs.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      201 2023-04-23 08:23:04.000000 flexypy-0.1.1/flexypy/generate_templates/templates/main.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-13 18:31:49.548187 flexypy-0.1.1/flexypy/http/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-03-26 16:09:44.000000 flexypy-0.1.1/flexypy/http/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      992 2023-04-22 20:19:57.000000 flexypy-0.1.1/flexypy/http/cookie.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     2552 2023-06-12 15:43:55.000000 flexypy-0.1.1/flexypy/http/request.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     2645 2023-04-27 09:44:59.000000 flexypy-0.1.1/flexypy/http/routing.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)    10281 2023-06-13 18:17:49.000000 flexypy-0.1.1/flexypy/http/server.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-13 18:31:49.548187 flexypy-0.1.1/flexypy/http/template/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 14:52:16.000000 flexypy-0.1.1/flexypy/http/template/__init__.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-13 18:31:49.568192 flexypy-0.1.1/flexypy/http/template/extensions/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-14 16:12:24.000000 flexypy-0.1.1/flexypy/http/template/extensions/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      764 2023-04-27 09:44:58.000000 flexypy-0.1.1/flexypy/http/template/extensions/base_extension.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      548 2023-04-17 09:32:56.000000 flexypy-0.1.1/flexypy/http/template/extensions/template_ext.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     3368 2023-04-17 10:37:47.000000 flexypy-0.1.1/flexypy/http/template/render.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-13 18:31:49.584196 flexypy-0.1.1/flexypy/middlewares/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        0 2023-04-15 09:42:14.000000 flexypy-0.1.1/flexypy/middlewares/__init__.py
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      445 2023-06-13 18:17:00.000000 flexypy-0.1.1/flexypy/middlewares/mddl.py
+drwxrwxr-x   0 uwine     (1000) uwine     (1000)        0 2023-06-13 18:31:49.384144 flexypy-0.1.1/flexypy.egg-info/
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      146 2023-06-13 18:31:49.000000 flexypy-0.1.1/flexypy.egg-info/PKG-INFO
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)     1223 2023-06-13 18:31:49.000000 flexypy-0.1.1/flexypy.egg-info/SOURCES.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        1 2023-06-13 18:31:49.000000 flexypy-0.1.1/flexypy.egg-info/dependency_links.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       34 2023-06-13 18:31:49.000000 flexypy-0.1.1/flexypy.egg-info/requires.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)        8 2023-06-13 18:31:49.000000 flexypy-0.1.1/flexypy.egg-info/top_level.txt
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)      405 2023-06-13 18:31:33.000000 flexypy-0.1.1/pyproject.toml
+-rw-rw-r--   0 uwine     (1000) uwine     (1000)       38 2023-06-13 18:31:49.584196 flexypy-0.1.1/setup.cfg
```

### Comparing `flexypy-0.1.0/flexypy/exceptions/web/server.py` & `flexypy-0.1.1/flexypy/exceptions/web/server.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.1.0/flexypy/generate_templates/generator.py` & `flexypy-0.1.1/flexypy/generate_templates/generator.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.1.0/flexypy/http/cookie.py` & `flexypy-0.1.1/flexypy/http/cookie.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.1.0/flexypy/http/request.py` & `flexypy-0.1.1/flexypy/http/request.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.1.0/flexypy/http/routing.py` & `flexypy-0.1.1/flexypy/http/routing.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.1.0/flexypy/http/server.py` & `flexypy-0.1.1/flexypy/http/server.py`

 * *Files 5% similar despite different names*

```diff
@@ -163,14 +163,19 @@
             global_t_obj = __import__(mddl.replace('/', '.'), fromlist=['middlewares'])
             mddl_list = getattr(global_t_obj, 'middlewares')
 
             for mddl in mddl_list:
                 m: Middleware = mddl(self.request, app)
                 m.start()
                 mddl_app = m.app
+                # set template variables
+                if m.template_kwargs:
+                    for name in m.template_kwargs:
+                        mddl_app.set_template_variables(**{name: m.template_kwargs[name]})
+
                 redirect = MddlRedirect(m.redirect_from, m.redirect_to)
         return [mddl_app, redirect]
 
     def start(self):
         resp = self._route()
         self._set_server_cookie()
```

### Comparing `flexypy-0.1.0/flexypy/http/template/extensions/base_extension.py` & `flexypy-0.1.1/flexypy/http/template/extensions/base_extension.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.1.0/flexypy/http/template/extensions/template_ext.py` & `flexypy-0.1.1/flexypy/http/template/extensions/template_ext.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.1.0/flexypy/http/template/render.py` & `flexypy-0.1.1/flexypy/http/template/render.py`

 * *Files identical despite different names*

### Comparing `flexypy-0.1.0/flexypy.egg-info/SOURCES.txt` & `flexypy-0.1.1/flexypy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

