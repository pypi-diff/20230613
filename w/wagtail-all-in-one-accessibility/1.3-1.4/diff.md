# Comparing `tmp/wagtail-all-in-one-accessibility-1.3.tar.gz` & `tmp/wagtail-all-in-one-accessibility-1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wagtail-all-in-one-accessibility-1.3.tar", last modified: Tue Jun 13 09:34:57 2023, max compression
+gzip compressed data, was "wagtail-all-in-one-accessibility-1.4.tar", last modified: Tue Jun 13 09:36:10 2023, max compression
```

## Comparing `wagtail-all-in-one-accessibility-1.3.tar` & `wagtail-all-in-one-accessibility-1.4.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 09:34:57.809566 wagtail-all-in-one-accessibility-1.3/
--rw-rw-rw-   0        0        0     4070 2023-06-13 09:34:57.809566 wagtail-all-in-one-accessibility-1.3/PKG-INFO
--rw-rw-rw-   0        0        0     3097 2023-06-13 09:22:45.000000 wagtail-all-in-one-accessibility-1.3/Readme.md
-drwxrwxrwx   0        0        0        0 2023-06-13 09:34:57.777382 wagtail-all-in-one-accessibility-1.3/search/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.3/search/__init__.py
--rw-rw-rw-   0        0        0     1057 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.3/search/views.py
--rw-rw-rw-   0        0        0     1008 2023-06-13 09:34:57.810592 wagtail-all-in-one-accessibility-1.3/setup.cfg
--rw-rw-rw-   0        0        0       82 2023-06-13 09:33:53.000000 wagtail-all-in-one-accessibility-1.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:34:57.783678 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/
--rw-rw-rw-   0        0        0        0 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/__init__.py
--rw-rw-rw-   0        0        0     1042 2023-06-12 10:02:50.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/admin.py
--rw-rw-rw-   0        0        0      198 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/apps.py
--rw-rw-rw-   0        0        0     1138 2023-06-12 13:12:27.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/context_processors.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:34:57.800622 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/migrations/
--rw-rw-rw-   0        0        0     2067 2023-06-12 10:04:21.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/migrations/0001_initial.py
--rw-rw-rw-   0        0        0      648 2023-06-12 12:22:09.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/migrations/0002_alter_wagtail_all_in_one_accessibility_aioa_license_key.py
--rw-rw-rw-   0        0        0        0 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/migrations/__init__.py
--rw-rw-rw-   0        0        0     1921 2023-06-12 13:12:35.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/models.py
--rw-rw-rw-   0        0        0       63 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/tests.py
--rw-rw-rw-   0        0        0      548 2023-06-12 10:03:16.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/urls.py
--rw-rw-rw-   0        0        0      108 2023-06-12 10:02:19.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/views.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:34:57.787670 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility.egg-info/
--rw-rw-rw-   0        0        0     4070 2023-06-13 09:34:57.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1134 2023-06-13 09:34:57.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 09:34:57.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       35 2023-06-13 09:34:57.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility.egg-info/requires.txt
--rw-rw-rw-   0        0        0       56 2023-06-13 09:34:57.000000 wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-06-13 09:34:57.803582 wagtail-all-in-one-accessibility-1.3/wagtail_package/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.3/wagtail_package/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-13 09:34:57.809566 wagtail-all-in-one-accessibility-1.3/wagtail_package/settings/
--rw-rw-rw-   0        0        0        0 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.3/wagtail_package/settings/__init__.py
--rw-rw-rw-   0        0        0     4791 2023-06-12 12:18:51.000000 wagtail-all-in-one-accessibility-1.3/wagtail_package/settings/base.py
--rw-rw-rw-   0        0        0      478 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.3/wagtail_package/settings/dev.py
--rw-rw-rw-   0        0        0      103 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.3/wagtail_package/settings/production.py
--rw-rw-rw-   0        0        0     1447 2023-06-12 10:07:02.000000 wagtail-all-in-one-accessibility-1.3/wagtail_package/urls.py
--rw-rw-rw-   0        0        0      427 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.3/wagtail_package/wsgi.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:36:10.431222 wagtail-all-in-one-accessibility-1.4/
+-rw-rw-rw-   0        0        0     4071 2023-06-13 09:36:10.431222 wagtail-all-in-one-accessibility-1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     3098 2023-06-13 09:35:57.000000 wagtail-all-in-one-accessibility-1.4/Readme.md
+drwxrwxrwx   0        0        0        0 2023-06-13 09:36:10.387379 wagtail-all-in-one-accessibility-1.4/search/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.4/search/__init__.py
+-rw-rw-rw-   0        0        0     1057 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.4/search/views.py
+-rw-rw-rw-   0        0        0     1008 2023-06-13 09:36:10.432219 wagtail-all-in-one-accessibility-1.4/setup.cfg
+-rw-rw-rw-   0        0        0       82 2023-06-13 09:33:53.000000 wagtail-all-in-one-accessibility-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:36:10.396354 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/
+-rw-rw-rw-   0        0        0        0 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/__init__.py
+-rw-rw-rw-   0        0        0     1042 2023-06-12 10:02:50.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/admin.py
+-rw-rw-rw-   0        0        0      198 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/apps.py
+-rw-rw-rw-   0        0        0     1138 2023-06-12 13:12:27.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/context_processors.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:36:10.418256 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/migrations/
+-rw-rw-rw-   0        0        0     2067 2023-06-12 10:04:21.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/migrations/0001_initial.py
+-rw-rw-rw-   0        0        0      648 2023-06-12 12:22:09.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/migrations/0002_alter_wagtail_all_in_one_accessibility_aioa_license_key.py
+-rw-rw-rw-   0        0        0        0 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/migrations/__init__.py
+-rw-rw-rw-   0        0        0     1921 2023-06-12 13:12:35.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/models.py
+-rw-rw-rw-   0        0        0       63 2023-06-12 10:01:23.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/tests.py
+-rw-rw-rw-   0        0        0      548 2023-06-12 10:03:16.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/urls.py
+-rw-rw-rw-   0        0        0      108 2023-06-12 10:02:19.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/views.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:36:10.400343 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility.egg-info/
+-rw-rw-rw-   0        0        0     4071 2023-06-13 09:36:10.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1134 2023-06-13 09:36:10.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 09:36:10.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       35 2023-06-13 09:36:10.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       56 2023-06-13 09:36:10.000000 wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-13 09:36:10.424240 wagtail-all-in-one-accessibility-1.4/wagtail_package/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.4/wagtail_package/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-13 09:36:10.430224 wagtail-all-in-one-accessibility-1.4/wagtail_package/settings/
+-rw-rw-rw-   0        0        0        0 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.4/wagtail_package/settings/__init__.py
+-rw-rw-rw-   0        0        0     4791 2023-06-12 12:18:51.000000 wagtail-all-in-one-accessibility-1.4/wagtail_package/settings/base.py
+-rw-rw-rw-   0        0        0      478 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.4/wagtail_package/settings/dev.py
+-rw-rw-rw-   0        0        0      103 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.4/wagtail_package/settings/production.py
+-rw-rw-rw-   0        0        0     1447 2023-06-12 10:07:02.000000 wagtail-all-in-one-accessibility-1.4/wagtail_package/urls.py
+-rw-rw-rw-   0        0        0      427 2023-06-12 09:56:54.000000 wagtail-all-in-one-accessibility-1.4/wagtail_package/wsgi.py
```

### Comparing `wagtail-all-in-one-accessibility-1.3/PKG-INFO` & `wagtail-all-in-one-accessibility-1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-all-in-one-accessibility
-Version: 1.3
+Version: 1.4
 Summary: All in One Accessibility that helps organizations enhance the accessibility and usability of their website
 Home-page: https://www.skynettechnologies.com
 Author: Skynet Technologies USA LLC
 Author-email: developer3@skynettechnologies.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -78,15 +78,15 @@
             ],
         },
     },
 ]
 ```
 
 ### Base.html
-Just add this tag in your base.html footer(your main template of django website) `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`:
+Just add this tag in your base.html footer(your main template of wagtail website) `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`:
 ```python
   <footer>
     <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
   </footer>
 ```
 
 ### Migrate
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-all-in-one-accessibility Version: 1.3
+Metadata-Version: 2.1 Name: wagtail-all-in-one-accessibility Version: 1.4
 Summary: All in One Accessibility that helps organizations enhance the
 accessibility and usability of their website Home-page: https://
 www.skynettechnologies.com Author: Skynet Technologies USA LLC Author-email:
 developer3@skynettechnologies.com Classifier: Environment :: Web Environment
 Classifier: Framework :: Django Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
@@ -41,12 +41,12 @@
 Settings.TEMPLATES Just add
 `wagtail_all_in_one_accessibility.context_processors.admin_AIOA` in your
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'wagtail_all_in_one_accessibility.context_processors.admin_AIOA', ], }, }, ]
 ``` ### Base.html Just add this tag in your base.html footer(your main template
-of django website) `
+of wagtail website) `
 `: ```python
   ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
 Restart Restart your app server with this command and check the admin panel the
 model is ready to use ```python python manage.py runserver ```
```

### Comparing `wagtail-all-in-one-accessibility-1.3/Readme.md` & `wagtail-all-in-one-accessibility-1.4/Readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             ],
         },
     },
 ]
 ```
 
 ### Base.html
-Just add this tag in your base.html footer(your main template of django website) `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`:
+Just add this tag in your base.html footer(your main template of wagtail website) `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`:
 ```python
   <footer>
     <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
   </footer>
 ```
 
 ### Migrate
```

#### html2text {}

```diff
@@ -28,12 +28,12 @@
 Settings.TEMPLATES Just add
 `wagtail_all_in_one_accessibility.context_processors.admin_AIOA` in your
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'wagtail_all_in_one_accessibility.context_processors.admin_AIOA', ], }, }, ]
 ``` ### Base.html Just add this tag in your base.html footer(your main template
-of django website) `
+of wagtail website) `
 `: ```python
   ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
 Restart Restart your app server with this command and check the admin panel the
 model is ready to use ```python python manage.py runserver ```
```

### Comparing `wagtail-all-in-one-accessibility-1.3/search/views.py` & `wagtail-all-in-one-accessibility-1.4/search/views.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.3/setup.cfg` & `wagtail-all-in-one-accessibility-1.4/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2077 6167 7461 696c 2d61 6c6c 2d69   = wagtail-all-i
 00000020: 6e2d 6f6e 652d 6163 6365 7373 6962 696c  n-one-accessibil
 00000030: 6974 790d 0a76 6572 7369 6f6e 203d 2031  ity..version = 1
-00000040: 2e33 0d0a 6465 7363 7269 7074 696f 6e20  .3..description 
+00000040: 2e34 0d0a 6465 7363 7269 7074 696f 6e20  .4..description 
 00000050: 3d20 416c 6c20 696e 204f 6e65 2041 6363  = All in One Acc
 00000060: 6573 7369 6269 6c69 7479 2074 6861 7420  essibility that 
 00000070: 6865 6c70 7320 6f72 6761 6e69 7a61 7469  helps organizati
 00000080: 6f6e 7320 656e 6861 6e63 6520 7468 6520  ons enhance the 
 00000090: 6163 6365 7373 6962 696c 6974 7920 616e  accessibility an
 000000a0: 6420 7573 6162 696c 6974 7920 6f66 2074  d usability of t
 000000b0: 6865 6972 2077 6562 7369 7465 0d0a 6c6f  heir website..lo
```

### Comparing `wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/admin.py` & `wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/admin.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/context_processors.py` & `wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/context_processors.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/migrations/0001_initial.py` & `wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/migrations/0002_alter_wagtail_all_in_one_accessibility_aioa_license_key.py` & `wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/migrations/0002_alter_wagtail_all_in_one_accessibility_aioa_license_key.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/models.py` & `wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/models.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility/urls.py` & `wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility/urls.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility.egg-info/PKG-INFO` & `wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wagtail-all-in-one-accessibility
-Version: 1.3
+Version: 1.4
 Summary: All in One Accessibility that helps organizations enhance the accessibility and usability of their website
 Home-page: https://www.skynettechnologies.com
 Author: Skynet Technologies USA LLC
 Author-email: developer3@skynettechnologies.com
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
@@ -78,15 +78,15 @@
             ],
         },
     },
 ]
 ```
 
 ### Base.html
-Just add this tag in your base.html footer(your main template of django website) `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`:
+Just add this tag in your base.html footer(your main template of wagtail website) `<script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>`:
 ```python
   <footer>
     <script id="aioa-adawidget" src="{{ AIOA_URL }}"></script>
   </footer>
 ```
 
 ### Migrate
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: wagtail-all-in-one-accessibility Version: 1.3
+Metadata-Version: 2.1 Name: wagtail-all-in-one-accessibility Version: 1.4
 Summary: All in One Accessibility that helps organizations enhance the
 accessibility and usability of their website Home-page: https://
 www.skynettechnologies.com Author: Skynet Technologies USA LLC Author-email:
 developer3@skynettechnologies.com Classifier: Environment :: Web Environment
 Classifier: Framework :: Django Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License Classifier: Operating System
 :: OS Independent Classifier: Programming Language :: Python Classifier:
@@ -41,12 +41,12 @@
 Settings.TEMPLATES Just add
 `wagtail_all_in_one_accessibility.context_processors.admin_AIOA` in your
 setting.TEMPLATES: ```python TEMPLATES = [ { 'BACKEND':
 'django.template.backends.django.DjangoTemplates', 'DIRS': [], 'APP_DIRS':
 True, 'OPTIONS': { 'context_processors':
 [ 'wagtail_all_in_one_accessibility.context_processors.admin_AIOA', ], }, }, ]
 ``` ### Base.html Just add this tag in your base.html footer(your main template
-of django website) `
+of wagtail website) `
 `: ```python
   ``` ### Migrate Migrate your app ```python python manage.py migrate ``` ###
 Restart Restart your app server with this command and check the admin panel the
 model is ready to use ```python python manage.py runserver ```
```

### Comparing `wagtail-all-in-one-accessibility-1.3/wagtail_all_in_one_accessibility.egg-info/SOURCES.txt` & `wagtail-all-in-one-accessibility-1.4/wagtail_all_in_one_accessibility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.3/wagtail_package/settings/base.py` & `wagtail-all-in-one-accessibility-1.4/wagtail_package/settings/base.py`

 * *Files identical despite different names*

### Comparing `wagtail-all-in-one-accessibility-1.3/wagtail_package/urls.py` & `wagtail-all-in-one-accessibility-1.4/wagtail_package/urls.py`

 * *Files identical despite different names*

