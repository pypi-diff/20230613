# Comparing `tmp/django-template-partials-23.1.tar.gz` & `tmp/django-template-partials-23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-template-partials-23.1.tar", last modified: Sat Jun 10 08:11:07 2023, max compression
+gzip compressed data, was "django-template-partials-23.2.tar", last modified: Tue Jun 13 15:31:11 2023, max compression
```

## Comparing `django-template-partials-23.1.tar` & `django-template-partials-23.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
--rw-r--r--   0        0        0       12 2023-06-10 08:10:09.840430 django-template-partials-23.1/.gitignore
--rw-r--r--   0        0        0      133 2023-06-10 07:15:27.155706 django-template-partials-23.1/.vscode/settings.json
--rw-r--r--   0        0        0     1081 2023-05-17 17:27:47.027110 django-template-partials-23.1/LICENSE
--rw-r--r--   0        0        0     2391 2023-06-10 08:06:13.659056 django-template-partials-23.1/README.md
--rw-r--r--   0        0        0      213 2023-06-10 08:07:19.133058 django-template-partials-23.1/justfile
--rw-r--r--   0        0        0      706 2023-06-10 08:09:04.575213 django-template-partials-23.1/pyproject.toml
--rw-r--r--   0        0        0      121 2023-06-10 08:06:27.533153 django-template-partials-23.1/src/template_partials/__init__.py
--rw-r--r--   0        0        0     2013 2023-06-10 07:52:39.943743 django-template-partials-23.1/src/template_partials/loader.py
--rw-r--r--   0        0        0        0 2023-06-10 07:14:20.655108 django-template-partials-23.1/src/template_partials/templatetags/__init__.py
--rw-r--r--   0        0        0     3120 2023-06-10 07:34:55.088077 django-template-partials-23.1/src/template_partials/templatetags/partials.py
--rw-r--r--   0        0        0        0 2023-06-10 07:31:47.903235 django-template-partials-23.1/tests/__init__.py
--rw-r--r--   0        0        0     1211 2023-06-10 07:48:57.417739 django-template-partials-23.1/tests/settings.py
--rw-r--r--   0        0        0       37 2023-06-10 07:39:17.702320 django-template-partials-23.1/tests/templates/base.html
--rw-r--r--   0        0        0      205 2023-06-10 07:40:08.278885 django-template-partials-23.1/tests/templates/example.html
--rw-r--r--   0        0        0     1131 2023-06-10 07:50:15.127276 django-template-partials-23.1/tests/tests.py
--rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 django-template-partials-23.1/PKG-INFO
+-rw-r--r--   0        0        0       12 2023-06-10 08:10:09.840430 django-template-partials-23.2/.gitignore
+-rw-r--r--   0        0        0      133 2023-06-10 07:15:27.155706 django-template-partials-23.2/.vscode/settings.json
+-rw-r--r--   0        0        0     1081 2023-05-17 17:27:47.027110 django-template-partials-23.2/LICENSE
+-rw-r--r--   0        0        0     2391 2023-06-10 08:06:13.659056 django-template-partials-23.2/README.md
+-rw-r--r--   0        0        0      213 2023-06-10 08:07:19.133058 django-template-partials-23.2/justfile
+-rw-r--r--   0        0        0      706 2023-06-10 08:09:04.575213 django-template-partials-23.2/pyproject.toml
+-rw-r--r--   0        0        0      121 2023-06-13 15:30:22.931172 django-template-partials-23.2/src/template_partials/__init__.py
+-rw-r--r--   0        0        0     2013 2023-06-10 07:52:39.943743 django-template-partials-23.2/src/template_partials/loader.py
+-rw-r--r--   0        0        0        0 2023-06-10 07:14:20.655108 django-template-partials-23.2/src/template_partials/templatetags/__init__.py
+-rw-r--r--   0        0        0     3312 2023-06-13 15:28:51.430156 django-template-partials-23.2/src/template_partials/templatetags/partials.py
+-rw-r--r--   0        0        0        0 2023-06-10 07:31:47.903235 django-template-partials-23.2/tests/__init__.py
+-rw-r--r--   0        0        0     1211 2023-06-10 07:48:57.417739 django-template-partials-23.2/tests/settings.py
+-rw-r--r--   0        0        0       37 2023-06-10 07:39:17.702320 django-template-partials-23.2/tests/templates/base.html
+-rw-r--r--   0        0        0      160 2023-06-13 15:27:32.435120 django-template-partials-23.2/tests/templates/debug.html
+-rw-r--r--   0        0        0      205 2023-06-10 07:40:08.278885 django-template-partials-23.2/tests/templates/example.html
+-rw-r--r--   0        0        0     1628 2023-06-13 15:27:32.435346 django-template-partials-23.2/tests/tests.py
+-rw-r--r--   0        0        0      499 1970-01-01 00:00:00.000000 django-template-partials-23.2/PKG-INFO
```

### Comparing `django-template-partials-23.1/LICENSE` & `django-template-partials-23.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django-template-partials-23.1/README.md` & `django-template-partials-23.2/README.md`

 * *Files identical despite different names*

### Comparing `django-template-partials-23.1/pyproject.toml` & `django-template-partials-23.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `django-template-partials-23.1/src/template_partials/loader.py` & `django-template-partials-23.2/src/template_partials/loader.py`

 * *Files identical despite different names*

### Comparing `django-template-partials-23.1/src/template_partials/templatetags/partials.py` & `django-template-partials-23.2/src/template_partials/templatetags/partials.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,18 @@
     """
 
     def __init__(self, nodelist, origin, name):
         self.nodelist = nodelist
         self.origin = origin
         self.name = name
 
+    def get_exception_info(self, exception, token):
+        template = self.origin.loader.get_template(self.origin.template_name)
+        return template.get_exception_info(exception, token)
+
     def render(self, context):
         "Display stage -- can be called many times"
         with context.render_context.push_state(self):
             if context.template is None:
                 with context.bind_template(self):
                     context.template_name = self.name
                     return self.nodelist.render(context)
```

### Comparing `django-template-partials-23.1/tests/settings.py` & `django-template-partials-23.2/tests/settings.py`

 * *Files identical despite different names*

### Comparing `django-template-partials-23.1/tests/tests.py` & `django-template-partials-23.2/tests/tests.py`

 * *Files 11% similar despite different names*

```diff
@@ -28,7 +28,20 @@
 
     def test_just_partial_from_loader(self):
         engine = engines["django"]
         template = engine.get_template("example.html#test-partial")
         rendered = template.render()
 
         self.assertEqual("TEST-PARTIAL-CONTENT", rendered.strip())
+
+    def test_debug_template(self):
+        class LazyExceptionObject:
+            def __str__(self):
+                raise Exception("Test exception")
+            
+        engine = engines["django"]
+        template = engine.get_template("debug.html")
+        try:
+            template.render({'exception': LazyExceptionObject()})
+        except Exception as e:
+            self.assertEqual(e.template_debug['message'], "Test exception")
+            self.assertEqual(e.template_debug['line'], 4)
```

