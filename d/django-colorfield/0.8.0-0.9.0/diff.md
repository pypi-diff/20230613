# Comparing `tmp/django-colorfield-0.8.0.tar.gz` & `tmp/django-colorfield-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-colorfield-0.8.0.tar", last modified: Fri Dec  2 09:51:04 2022, max compression
+gzip compressed data, was "django-colorfield-0.9.0.tar", last modified: Tue Jun 13 07:55:13 2023, max compression
```

## Comparing `django-colorfield-0.8.0.tar` & `django-colorfield-0.9.0.tar`

### file list

```diff
@@ -1,31 +1,45 @@
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-12-02 09:51:04.872027 django-colorfield-0.8.0/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1094 2022-12-02 09:44:41.000000 django-colorfield-0.8.0/LICENSE.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      117 2020-08-27 08:05:11.000000 django-colorfield-0.8.0/MANIFEST.in
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     9837 2022-12-02 09:51:04.872273 django-colorfield-0.8.0/PKG-INFO
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     6768 2022-10-24 08:38:11.000000 django-colorfield-0.8.0/README.md
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-12-02 09:51:04.865060 django-colorfield-0.8.0/colorfield/
--rwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2020-08-27 08:05:11.000000 django-colorfield-0.8.0/colorfield/__init__.py
--rwxr-xr-x   0 fabiocaccamo   (501) staff       (20)     4715 2022-12-02 09:44:41.000000 django-colorfield-0.8.0/colorfield/fields.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1059 2022-12-02 09:44:41.000000 django-colorfield-0.8.0/colorfield/serializers.py
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-12-02 09:51:04.860463 django-colorfield-0.8.0/colorfield/static/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-12-02 09:51:04.865394 django-colorfield-0.8.0/colorfield/static/colorfield/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      408 2021-10-08 14:53:36.000000 django-colorfield-0.8.0/colorfield/static/colorfield/colorfield.js
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-12-02 09:51:04.868017 django-colorfield-0.8.0/colorfield/static/colorfield/jscolor/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)   102106 2021-01-14 08:56:48.000000 django-colorfield-0.8.0/colorfield/static/colorfield/jscolor/jscolor.js
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)    61235 2021-01-14 08:56:48.000000 django-colorfield-0.8.0/colorfield/static/colorfield/jscolor/jscolor.min.js
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-12-02 09:51:04.860898 django-colorfield-0.8.0/colorfield/templates/
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-12-02 09:51:04.869430 django-colorfield-0.8.0/colorfield/templates/colorfield/
--rwxr-xr-x   0 fabiocaccamo   (501) staff       (20)      524 2022-07-19 08:16:07.000000 django-colorfield-0.8.0/colorfield/templates/colorfield/color.html
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      576 2022-12-02 09:44:41.000000 django-colorfield-0.8.0/colorfield/utils.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      492 2022-12-02 09:44:41.000000 django-colorfield-0.8.0/colorfield/validators.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)       22 2022-12-02 09:50:06.000000 django-colorfield-0.8.0/colorfield/version.py
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     1024 2022-12-02 09:44:41.000000 django-colorfield-0.8.0/colorfield/widgets.py
-drwxr-xr-x   0 fabiocaccamo   (501) staff       (20)        0 2022-12-02 09:51:04.871760 django-colorfield-0.8.0/django_colorfield.egg-info/
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     9837 2022-12-02 09:51:04.000000 django-colorfield-0.8.0/django_colorfield.egg-info/PKG-INFO
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      616 2022-12-02 09:51:04.000000 django-colorfield-0.8.0/django_colorfield.egg-info/SOURCES.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)        1 2022-12-02 09:51:04.000000 django-colorfield-0.8.0/django_colorfield.egg-info/dependency_links.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)       14 2022-12-02 09:51:04.000000 django-colorfield-0.8.0/django_colorfield.egg-info/requires.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)       11 2022-12-02 09:51:04.000000 django-colorfield-0.8.0/django_colorfield.egg-info/top_level.txt
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)      178 2022-10-24 08:37:37.000000 django-colorfield-0.8.0/pyproject.toml
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)       79 2022-12-02 09:51:04.872783 django-colorfield-0.8.0/setup.cfg
--rw-r--r--   0 fabiocaccamo   (501) staff       (20)     2662 2022-12-02 09:47:05.000000 django-colorfield-0.8.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:55:13.476864 django-colorfield-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-06-13 07:55:13.476864 django-colorfield-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6755 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:55:13.472864 django-colorfield-0.9.0/colorfield/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      273 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4685 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:55:13.468864 django-colorfield-0.9.0/colorfield/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:55:13.468864 django-colorfield-0.9.0/colorfield/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:55:13.472864 django-colorfield-0.9.0/colorfield/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      380 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:55:13.468864 django-colorfield-0.9.0/colorfield/locale/it/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:55:13.472864 django-colorfield-0.9.0/colorfield/locale/it/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/serializers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:55:13.472864 django-colorfield-0.9.0/colorfield/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:55:13.476864 django-colorfield-0.9.0/colorfield/static/colorfield/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/static/colorfield/colorfield.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:55:13.476864 django-colorfield-0.9.0/colorfield/static/colorfield/jscolor/
+-rw-r--r--   0 runner    (1001) docker     (123)   102106 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/static/colorfield/jscolor/jscolor.js
+-rw-r--r--   0 runner    (1001) docker     (123)    61235 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/static/colorfield/jscolor/jscolor.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:55:13.472864 django-colorfield-0.9.0/colorfield/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:55:13.476864 django-colorfield-0.9.0/colorfield/templates/colorfield/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      524 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/templates/colorfield/color.html
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      492 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/colorfield/widgets.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:55:13.476864 django-colorfield-0.9.0/django_colorfield.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9756 2023-06-13 07:55:13.000000 django-colorfield-0.9.0/django_colorfield.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      871 2023-06-13 07:55:13.000000 django-colorfield-0.9.0/django_colorfield.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:55:13.000000 django-colorfield-0.9.0/django_colorfield.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-06-13 07:55:13.000000 django-colorfield-0.9.0/django_colorfield.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-06-13 07:55:13.000000 django-colorfield-0.9.0/django_colorfield.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2430 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 07:55:13.476864 django-colorfield-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:55:13.476864 django-colorfield-0.9.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5524 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/tests/test_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3747 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/tests/test_serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-06-13 07:54:58.000000 django-colorfield-0.9.0/tests/test_widgets.py
```

### Comparing `django-colorfield-0.8.0/LICENSE.txt` & `django-colorfield-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `django-colorfield-0.8.0/PKG-INFO` & `django-colorfield-0.9.0/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,205 +1,227 @@
 Metadata-Version: 2.1
 Name: django-colorfield
-Version: 0.8.0
-Summary: simple color field for your models with a nice color-picker in the admin-interface.
-Home-page: https://github.com/fabiocaccamo/django-colorfield
-Author: Jared Forsyth, Fabio Caccamo
-Author-email: jared@jaredforsyth.com, fabio.caccamo@gmail.com
-License: MIT
-Download-URL: https://github.com/fabiocaccamo/django-colorfield/archive/0.8.0.tar.gz
+Version: 0.9.0
+Summary: color field for django models with a nice color-picker in the admin.
+Author-email: Jared Forsyth <jared@jaredforsyth.com>, Fabio Caccamo <fabio.caccamo@gmail.com>
+Maintainer-email: Fabio Caccamo <fabio.caccamo@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2013-present Jared Forsyth / Fabio Caccamo
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/fabiocaccamo/django-colorfield
+Project-URL: Download, https://github.com/fabiocaccamo/django-colorfield/releases
 Project-URL: Documentation, https://github.com/fabiocaccamo/django-colorfield#readme
 Project-URL: Issues, https://github.com/fabiocaccamo/django-colorfield/issues
 Project-URL: Funding, https://github.com/sponsors/fabiocaccamo/
 Project-URL: Twitter, https://twitter.com/fabiocaccamo
-Description: [![](https://img.shields.io/pypi/pyversions/django-colorfield.svg?color=3776AB&logo=python&logoColor=white)](https://www.python.org/)
-        [![](https://img.shields.io/pypi/djversions/django-colorfield?color=0C4B33&logo=django&logoColor=white&label=django)](https://www.djangoproject.com/)
-        
-        [![](https://img.shields.io/pypi/v/django-colorfield.svg?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/django-colorfield/)
-        [![](https://pepy.tech/badge/django-colorfield/month)](https://pepy.tech/project/django-colorfield)
-        [![](https://img.shields.io/github/stars/fabiocaccamo/django-colorfield?logo=github)](https://github.com/fabiocaccamo/django-colorfield/)
-        [![](https://badges.pufler.dev/visits/fabiocaccamo/django-colorfield?label=visitors&color=blue)](https://badges.pufler.dev)
-        [![](https://img.shields.io/pypi/l/django-colorfield.svg?color=blue)](https://github.com/fabiocaccamo/django-colorfield/blob/master/LICENSE.txt)
-        
-        [![](https://results.pre-commit.ci/badge/github/fabiocaccamo/django-colorfield/master.svg)](https://results.pre-commit.ci/latest/github/fabiocaccamo/django-colorfield/master)
-        [![](https://img.shields.io/github/workflow/status/fabiocaccamo/django-colorfield/Test%20package?label=build&logo=github)](https://github.com/fabiocaccamo/django-colorfield)
-        [![](https://img.shields.io/codecov/c/gh/fabiocaccamo/django-colorfield?logo=codecov)](https://codecov.io/gh/fabiocaccamo/django-colorfield)
-        [![](https://img.shields.io/codacy/grade/194566618f424a819ce43450ea0af081?logo=codacy)](https://www.codacy.com/app/fabiocaccamo/django-colorfield)
-        [![](https://img.shields.io/codeclimate/maintainability/fabiocaccamo/django-colorfield?logo=code-climate)](https://codeclimate.com/github/fabiocaccamo/django-colorfield/)
-        [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        # django-colorfield
-        simple color field for your models with a nice color-picker in the admin-interface.
-        
-        ![django-colorfield-hex](https://user-images.githubusercontent.com/7900305/104512324-51ed0f80-55ee-11eb-9144-de03d922c2ce.png)
-        ![django-colorfield-hexa](https://user-images.githubusercontent.com/7900305/104512063-ec991e80-55ed-11eb-95b6-9174ac3f4f38.png)
-        
-        ---
-        
-        ## Installation
-        -   Run `pip install django-colorfield`
-        -   Add `colorfield` to `settings.INSTALLED_APPS`
-        -   Run `python manage.py collectstatic`
-        -   Restart your application server
-        
-        ---
-        
-        ## Usage
-        
-        ### Settings
-        This package doesn't need any setting.
-        
-        ### Models
-        Just add color field(s) to your models like this:
-        
-        ```python
-        from colorfield.fields import ColorField
-        from django.db import models
-        
-        class MyModel(model.Model):
-            color = ColorField(default='#FF0000')
-        ```
-        
-        ### Field Options
-        These are the supported custom options: [`format`](#format), [`image_field`](#image_field), [`samples`](#samples)
-        
-        #### format
-        
-        The following formats are supported: `hex` *(default)*, `hexa`.
-        
-        ```python
-        from colorfield.fields import ColorField
-        from django.db import models
-        
-        class MyModel(model.Model):
-            color = ColorField(format="hexa")
-        ```
-        
-        #### image_field
-        
-        It is possible to auto-populate the field value getting the color from an image using the `image_field` option.
-        
-        The color will be calculated from the **top-left pixel** color of the image each time the model instance is saved.
-        
-        ```python
-        from colorfield.fields import ColorField
-        from django.db import models
-        
-        class MyModel(model.Model):
-            image = models.ImageField(upload_to="images")
-            color = ColorField(image_field="image")
-        ```
-        
-        #### samples
-        
-        It is possible to provide a palette of colors to choose from to the widget using the `samples` option.
-        
-        This option **is not restrictive** (on the contrary of `choices` option), it is also possible to choose another color from the spectrum.
-        
-        ![django-colorfield-samples](https://user-images.githubusercontent.com/7900305/104512178-194d3600-55ee-11eb-8cba-91cca156da06.png)
-        
-        ```python
-        from colorfield.fields import ColorField
-        from django.db import models
-        
-        class MyModel(model.Model):
-        
-            COLOR_PALETTE = [
-                ("#FFFFFF", "white", ),
-                ("#000000", "black", ),
-            ]
-        
-            # not restrictive, allows the selection of another color from the spectrum.
-            color = ColorField(samples=COLOR_PALETTE)
-        
-            # restrictive, it is mandatory to choose a color from the palette
-            color = ColorField(choices=COLOR_PALETTE)
-        ```
-        
-        ### Admin
-        The admin will kindly provide a simple [color picker](http://jscolor.com/) for all color fields. :)
-        
-        ---
-        
-        ## Testing
-        ```bash
-        # clone repository
-        git clone https://github.com/fabiocaccamo/django-colorfield.git && cd django-colorfield
-        
-        # create virtualenv and activate it
-        python -m venv venv && . venv/bin/activate
-        
-        # upgrade pip
-        python -m pip install --upgrade pip
-        
-        # install requirements
-        pip install -r requirements.txt -r requirements-test.txt
-        
-        # run tests
-        tox
-        # or
-        python setup.py test
-        # or
-        python -m django test --settings "tests.settings"
-        ```
-        ---
-        
-        ## Credits
-        Originally developed by [Jared Forsyth](https://github.com/jaredly)
-        
-        ---
-        
-        ## License
-        Released under [MIT License](LICENSE.txt).
-        
-        ---
-        
-        ## Supporting
-        
-        - :star: Star this project on [GitHub](https://github.com/fabiocaccamo/django-colorfield)
-        - :octocat: Follow me on [GitHub](https://github.com/fabiocaccamo)
-        - :blue_heart: Follow me on [Twitter](https://twitter.com/fabiocaccamo)
-        - :moneybag: Sponsor me on [Github](https://github.com/sponsors/fabiocaccamo)
-        
-        ## See also
-        
-        - [`django-admin-interface`](https://github.com/fabiocaccamo/django-admin-interface) - the default admin interface made customizable by the admin itself. popup windows replaced by modals. 🧙 ⚡
-        
-        - [`django-extra-settings`](https://github.com/fabiocaccamo/django-extra-settings) - config and manage typed extra settings using just the django admin. ⚙️
-        
-        - [`django-maintenance-mode`](https://github.com/fabiocaccamo/django-maintenance-mode) - shows a 503 error page when maintenance-mode is on. 🚧 🛠️
-        
-        - [`django-redirects`](https://github.com/fabiocaccamo/django-redirects) - redirects with full control. ↪️
-        
-        - [`django-treenode`](https://github.com/fabiocaccamo/django-treenode) - probably the best abstract model / admin for your tree based stuff. 🌳
-        
-        - [`python-benedict`](https://github.com/fabiocaccamo/python-benedict) - dict subclass with keylist/keypath support, I/O shortcuts (base64, csv, json, pickle, plist, query-string, toml, xml, yaml) and many utilities. 📘
-        
-        - [`python-codicefiscale`](https://github.com/fabiocaccamo/python-codicefiscale) - encode/decode Italian fiscal codes - codifica/decodifica del Codice Fiscale. 🇮🇹 💳
-        
-        - [`python-fontbro`](https://github.com/fabiocaccamo/python-fontbro) - friendly font operations. 🧢
-        
-        - [`python-fsutil`](https://github.com/fabiocaccamo/python-fsutil) - file-system utilities for lazy devs. 🧟‍♂️
-        
 Keywords: django,colorfield,colorpicker,color,field,picker,chooser,admin,python
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
-Requires: django (>=2.2)
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![](https://img.shields.io/pypi/pyversions/django-colorfield.svg?color=3776AB&logo=python&logoColor=white)](https://www.python.org/)
+[![](https://img.shields.io/pypi/djversions/django-colorfield?color=0C4B33&logo=django&logoColor=white&label=django)](https://www.djangoproject.com/)
+
+[![](https://img.shields.io/pypi/v/django-colorfield.svg?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/django-colorfield/)
+[![](https://pepy.tech/badge/django-colorfield/month)](https://pepy.tech/project/django-colorfield)
+[![](https://img.shields.io/github/stars/fabiocaccamo/django-colorfield?logo=github)](https://github.com/fabiocaccamo/django-colorfield/stargazers)
+[![](https://img.shields.io/pypi/l/django-colorfield.svg?color=blue)](https://github.com/fabiocaccamo/django-colorfield/blob/main/LICENSE.txt)
+
+[![](https://results.pre-commit.ci/badge/github/fabiocaccamo/django-colorfield/main.svg)](https://results.pre-commit.ci/latest/github/fabiocaccamo/django-colorfield/main)
+[![](https://img.shields.io/github/actions/workflow/status/fabiocaccamo/django-colorfield/test-package.yml?branch=main&label=build&logo=github)](https://github.com/fabiocaccamo/django-colorfield)
+[![](https://img.shields.io/codecov/c/gh/fabiocaccamo/django-colorfield?logo=codecov)](https://codecov.io/gh/fabiocaccamo/django-colorfield)
+[![](https://img.shields.io/codacy/grade/194566618f424a819ce43450ea0af081?logo=codacy)](https://www.codacy.com/app/fabiocaccamo/django-colorfield)
+[![](https://img.shields.io/codeclimate/maintainability/fabiocaccamo/django-colorfield?logo=code-climate)](https://codeclimate.com/github/fabiocaccamo/django-colorfield/)
+[![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+# django-colorfield
+simple color field for your models with a nice color-picker in the admin-interface.
+
+![django-colorfield-hex](https://user-images.githubusercontent.com/7900305/104512324-51ed0f80-55ee-11eb-9144-de03d922c2ce.png)
+![django-colorfield-hexa](https://user-images.githubusercontent.com/7900305/104512063-ec991e80-55ed-11eb-95b6-9174ac3f4f38.png)
+
+---
+
+## Installation
+-   Run `pip install django-colorfield`
+-   Add `colorfield` to `settings.INSTALLED_APPS`
+-   Run `python manage.py collectstatic`
+-   Restart your application server
+
+---
+
+## Usage
+
+### Settings
+This package doesn't need any setting.
+
+### Models
+Just add color field(s) to your models like this:
+
+```python
+from colorfield.fields import ColorField
+from django.db import models
+
+class MyModel(model.Model):
+    color = ColorField(default='#FF0000')
+```
+
+### Field Options
+These are the supported custom options: [`format`](#format), [`image_field`](#image_field), [`samples`](#samples)
+
+#### format
+
+The following formats are supported: `hex` *(default)*, `hexa`.
+
+```python
+from colorfield.fields import ColorField
+from django.db import models
+
+class MyModel(model.Model):
+    color = ColorField(format="hexa")
+```
+
+#### image_field
+
+It is possible to auto-populate the field value getting the color from an image using the `image_field` option.
+
+The color will be calculated from the **top-left pixel** color of the image each time the model instance is saved.
+
+```python
+from colorfield.fields import ColorField
+from django.db import models
+
+class MyModel(model.Model):
+    image = models.ImageField(upload_to="images")
+    color = ColorField(image_field="image")
+```
+
+#### samples
+
+It is possible to provide a palette of colors to choose from to the widget using the `samples` option.
+
+This option **is not restrictive** (on the contrary of `choices` option), it is also possible to choose another color from the spectrum.
+
+![django-colorfield-samples](https://user-images.githubusercontent.com/7900305/104512178-194d3600-55ee-11eb-8cba-91cca156da06.png)
+
+```python
+from colorfield.fields import ColorField
+from django.db import models
+
+class MyModel(model.Model):
+
+    COLOR_PALETTE = [
+        ("#FFFFFF", "white", ),
+        ("#000000", "black", ),
+    ]
+
+    # not restrictive, allows the selection of another color from the spectrum.
+    color = ColorField(samples=COLOR_PALETTE)
+
+    # restrictive, it is mandatory to choose a color from the palette
+    color = ColorField(choices=COLOR_PALETTE)
+```
+
+### Admin
+The admin will kindly provide a simple [color picker](http://jscolor.com/) for all color fields. :)
+
+---
+
+## Testing
+```bash
+# clone repository
+git clone https://github.com/fabiocaccamo/django-colorfield.git && cd django-colorfield
+
+# create virtualenv and activate it
+python -m venv venv && . venv/bin/activate
+
+# upgrade pip
+python -m pip install --upgrade pip
+
+# install requirements
+pip install -r requirements.txt -r requirements-test.txt
+
+# install pre-commit to run formatters and linters
+pre-commit install --install-hooks
+
+# run tests
+tox
+# or
+python runtests.py
+# or
+python -m django test --settings "tests.settings"
+```
+---
+
+## Credits
+Originally developed by [Jared Forsyth](https://github.com/jaredly)
+
+---
+
+## License
+Released under [MIT License](LICENSE.txt).
+
+---
+
+## Supporting
+
+- :star: Star this project on [GitHub](https://github.com/fabiocaccamo/django-colorfield)
+- :octocat: Follow me on [GitHub](https://github.com/fabiocaccamo)
+- :blue_heart: Follow me on [Twitter](https://twitter.com/fabiocaccamo)
+- :moneybag: Sponsor me on [Github](https://github.com/sponsors/fabiocaccamo)
+
+## See also
+
+- [`django-admin-interface`](https://github.com/fabiocaccamo/django-admin-interface) - the default admin interface made customizable by the admin itself. popup windows replaced by modals. 🧙 ⚡
+
+- [`django-extra-settings`](https://github.com/fabiocaccamo/django-extra-settings) - config and manage typed extra settings using just the django admin. ⚙️
+
+- [`django-maintenance-mode`](https://github.com/fabiocaccamo/django-maintenance-mode) - shows a 503 error page when maintenance-mode is on. 🚧 🛠️
+
+- [`django-redirects`](https://github.com/fabiocaccamo/django-redirects) - redirects with full control. ↪️
+
+- [`django-treenode`](https://github.com/fabiocaccamo/django-treenode) - probably the best abstract model / admin for your tree based stuff. 🌳
+
+- [`python-benedict`](https://github.com/fabiocaccamo/python-benedict) - dict subclass with keylist/keypath support, I/O shortcuts (base64, csv, json, pickle, plist, query-string, toml, xml, yaml) and many utilities. 📘
+
+- [`python-codicefiscale`](https://github.com/fabiocaccamo/python-codicefiscale) - encode/decode Italian fiscal codes - codifica/decodifica del Codice Fiscale. 🇮🇹 💳
+
+- [`python-fontbro`](https://github.com/fabiocaccamo/python-fontbro) - friendly font operations. 🧢
+
+- [`python-fsutil`](https://github.com/fabiocaccamo/python-fsutil) - file-system utilities for lazy devs. 🧟‍♂️
```

### Comparing `django-colorfield-0.8.0/README.md` & `django-colorfield-0.9.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 [![](https://img.shields.io/pypi/pyversions/django-colorfield.svg?color=3776AB&logo=python&logoColor=white)](https://www.python.org/)
 [![](https://img.shields.io/pypi/djversions/django-colorfield?color=0C4B33&logo=django&logoColor=white&label=django)](https://www.djangoproject.com/)
 
 [![](https://img.shields.io/pypi/v/django-colorfield.svg?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/django-colorfield/)
 [![](https://pepy.tech/badge/django-colorfield/month)](https://pepy.tech/project/django-colorfield)
-[![](https://img.shields.io/github/stars/fabiocaccamo/django-colorfield?logo=github)](https://github.com/fabiocaccamo/django-colorfield/)
-[![](https://badges.pufler.dev/visits/fabiocaccamo/django-colorfield?label=visitors&color=blue)](https://badges.pufler.dev)
-[![](https://img.shields.io/pypi/l/django-colorfield.svg?color=blue)](https://github.com/fabiocaccamo/django-colorfield/blob/master/LICENSE.txt)
+[![](https://img.shields.io/github/stars/fabiocaccamo/django-colorfield?logo=github)](https://github.com/fabiocaccamo/django-colorfield/stargazers)
+[![](https://img.shields.io/pypi/l/django-colorfield.svg?color=blue)](https://github.com/fabiocaccamo/django-colorfield/blob/main/LICENSE.txt)
 
-[![](https://results.pre-commit.ci/badge/github/fabiocaccamo/django-colorfield/master.svg)](https://results.pre-commit.ci/latest/github/fabiocaccamo/django-colorfield/master)
-[![](https://img.shields.io/github/workflow/status/fabiocaccamo/django-colorfield/Test%20package?label=build&logo=github)](https://github.com/fabiocaccamo/django-colorfield)
+[![](https://results.pre-commit.ci/badge/github/fabiocaccamo/django-colorfield/main.svg)](https://results.pre-commit.ci/latest/github/fabiocaccamo/django-colorfield/main)
+[![](https://img.shields.io/github/actions/workflow/status/fabiocaccamo/django-colorfield/test-package.yml?branch=main&label=build&logo=github)](https://github.com/fabiocaccamo/django-colorfield)
 [![](https://img.shields.io/codecov/c/gh/fabiocaccamo/django-colorfield?logo=codecov)](https://codecov.io/gh/fabiocaccamo/django-colorfield)
 [![](https://img.shields.io/codacy/grade/194566618f424a819ce43450ea0af081?logo=codacy)](https://www.codacy.com/app/fabiocaccamo/django-colorfield)
 [![](https://img.shields.io/codeclimate/maintainability/fabiocaccamo/django-colorfield?logo=code-climate)](https://codeclimate.com/github/fabiocaccamo/django-colorfield/)
 [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # django-colorfield
 simple color field for your models with a nice color-picker in the admin-interface.
@@ -117,18 +116,21 @@
 
 # upgrade pip
 python -m pip install --upgrade pip
 
 # install requirements
 pip install -r requirements.txt -r requirements-test.txt
 
+# install pre-commit to run formatters and linters
+pre-commit install --install-hooks
+
 # run tests
 tox
 # or
-python setup.py test
+python runtests.py
 # or
 python -m django test --settings "tests.settings"
 ```
 ---
 
 ## Credits
 Originally developed by [Jared Forsyth](https://github.com/jaredly)
```

### Comparing `django-colorfield-0.8.0/colorfield/fields.py` & `django-colorfield-0.9.0/colorfield/fields.py`

 * *Files 15% similar despite different names*

```diff
@@ -8,38 +8,37 @@
 
 VALIDATORS_PER_FORMAT = {"hex": color_hex_validator, "hexa": color_hexa_validator}
 
 DEFAULT_PER_FORMAT = {"hex": "#FFFFFF", "hexa": "#FFFFFFFF"}
 
 
 class ColorField(CharField):
-
     default_validators = []
 
     def __init__(self, *args, **kwargs):
         # works like Django choices, but does not restrict input to the given choices
         self.samples = kwargs.pop("samples", None)
         self.format = kwargs.pop("format", "hex").lower()
         if self.format not in ["hex", "hexa"]:
-            raise ValueError("Unsupported color format: {}".format(self.format))
+            raise ValueError(f"Unsupported color format: {self.format}")
         self.default_validators = [VALIDATORS_PER_FORMAT[self.format]]
 
         self.image_field = kwargs.pop("image_field", None)
         if self.image_field:
             kwargs.setdefault("blank", True)
 
         kwargs.setdefault("max_length", 18)
         if kwargs.get("null"):
             kwargs.setdefault("blank", True)
             kwargs.setdefault("default", None)
         elif kwargs.get("blank"):
             kwargs.setdefault("default", "")
         else:
             kwargs.setdefault("default", DEFAULT_PER_FORMAT[self.format])
-        super(ColorField, self).__init__(*args, **kwargs)
+        super().__init__(*args, **kwargs)
 
         if self.choices and self.samples:
             raise ImproperlyConfigured(
                 "Invalid options: 'choices' and 'samples' are mutually exclusive, "
                 "you can set only one of the two for a ColorField instance."
             )
 
@@ -51,29 +50,30 @@
         elif self.samples:
             palette = [choice[0] for choice in self.samples]
         kwargs["widget"] = ColorWidget(
             attrs={
                 "default": self.get_default(),
                 "format": self.format,
                 "palette": palette,
-                # # this will be used to hide the widget color spectrum if choices is defined:
+                # # TODO: in case choices is defined,
+                # # this will be used to hide the widget color spectrum
                 # 'palette_choices_only': bool(self.choices),
             }
         )
-        return super(ColorField, self).formfield(**kwargs)
+        return super().formfield(**kwargs)
 
     def contribute_to_class(self, cls, name, **kwargs):
-        super(ColorField, self).contribute_to_class(cls, name, **kwargs)
+        super().contribute_to_class(cls, name, **kwargs)
         if cls._meta.abstract:
             return
         if self.image_field:
             signals.post_save.connect(self._update_from_image_field, sender=cls)
 
     def deconstruct(self):
-        name, path, args, kwargs = super(ColorField, self).deconstruct()
+        name, path, args, kwargs = super().deconstruct()
         kwargs["samples"] = self.samples
         kwargs["image_field"] = self.image_field
         return name, path, args, kwargs
 
     def _get_image_field_color(self, instance):
         color = ""
         image_file = getattr(instance, self.image_field)
@@ -87,22 +87,22 @@
         if not instance or not instance.pk or not self.image_field:
             return
         # check if the field is a valid ImageField
         try:
             field_cls = instance._meta.get_field(self.image_field)
             if not isinstance(field_cls, ImageField):
                 raise ImproperlyConfigured(
-                    'Invalid "image_field" field type, '
-                    'expected an instance of "models.ImageField".'
+                    "Invalid 'image_field' field type, "
+                    "expected an instance of 'models.ImageField'."
                 )
-        except FieldDoesNotExist:
+        except FieldDoesNotExist as error:
             raise ImproperlyConfigured(
-                'Invalid "image_field" field name, '
-                '"{}" field not found.'.format(self.image_field)
-            )
+                "Invalid 'image_field' field name, "
+                f"{self.image_field!r} field not found."
+            ) from error
         # update value from picking color from image field
         color = self._get_image_field_color(instance)
         color_field_name = self.attname
         color_field_value = getattr(instance, color_field_name, None)
         if color_field_value != color and color:
             color_field_value = color or self.default
             # update in-memory value
```

### Comparing `django-colorfield-0.8.0/colorfield/serializers.py` & `django-colorfield-0.9.0/colorfield/serializers.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 except ImportError:
     ModuleNotFoundError("Django REST Framework is not installed.")
 
 from colorfield.validators import color_hex_validator, color_hexa_validator
 
 
 class ColorField(CharField):
-
     default_error_messages = {
         "invalid": [
             color_hex_validator.message,
             color_hexa_validator.message,
         ]
     }
```

### Comparing `django-colorfield-0.8.0/colorfield/static/colorfield/jscolor/jscolor.js` & `django-colorfield-0.9.0/colorfield/static/colorfield/jscolor/jscolor.js`

 * *Files identical despite different names*

### Comparing `django-colorfield-0.8.0/colorfield/static/colorfield/jscolor/jscolor.min.js` & `django-colorfield-0.9.0/colorfield/static/colorfield/jscolor/jscolor.min.js`

 * *Files identical despite different names*

### Comparing `django-colorfield-0.8.0/colorfield/templates/colorfield/color.html` & `django-colorfield-0.9.0/colorfield/templates/colorfield/color.html`

 * *Files identical despite different names*

### Comparing `django-colorfield-0.8.0/colorfield/utils.py` & `django-colorfield-0.9.0/colorfield/utils.py`

 * *Files identical despite different names*

### Comparing `django-colorfield-0.8.0/colorfield/widgets.py` & `django-colorfield-0.9.0/colorfield/widgets.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from django.conf import settings
 from django.forms import TextInput
 from django.template.loader import render_to_string
 
 
 class ColorWidget(TextInput):
-
     template_name = "colorfield/color.html"
 
     class Media:
         if settings.DEBUG:
             js = [
                 "colorfield/jscolor/jscolor.js",
                 "colorfield/colorfield.js",
```

### Comparing `django-colorfield-0.8.0/django_colorfield.egg-info/PKG-INFO` & `django-colorfield-0.9.0/django_colorfield.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,205 +1,227 @@
 Metadata-Version: 2.1
 Name: django-colorfield
-Version: 0.8.0
-Summary: simple color field for your models with a nice color-picker in the admin-interface.
-Home-page: https://github.com/fabiocaccamo/django-colorfield
-Author: Jared Forsyth, Fabio Caccamo
-Author-email: jared@jaredforsyth.com, fabio.caccamo@gmail.com
-License: MIT
-Download-URL: https://github.com/fabiocaccamo/django-colorfield/archive/0.8.0.tar.gz
+Version: 0.9.0
+Summary: color field for django models with a nice color-picker in the admin.
+Author-email: Jared Forsyth <jared@jaredforsyth.com>, Fabio Caccamo <fabio.caccamo@gmail.com>
+Maintainer-email: Fabio Caccamo <fabio.caccamo@gmail.com>
+License: MIT License
+        
+        Copyright (c) 2013-present Jared Forsyth / Fabio Caccamo
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/fabiocaccamo/django-colorfield
+Project-URL: Download, https://github.com/fabiocaccamo/django-colorfield/releases
 Project-URL: Documentation, https://github.com/fabiocaccamo/django-colorfield#readme
 Project-URL: Issues, https://github.com/fabiocaccamo/django-colorfield/issues
 Project-URL: Funding, https://github.com/sponsors/fabiocaccamo/
 Project-URL: Twitter, https://twitter.com/fabiocaccamo
-Description: [![](https://img.shields.io/pypi/pyversions/django-colorfield.svg?color=3776AB&logo=python&logoColor=white)](https://www.python.org/)
-        [![](https://img.shields.io/pypi/djversions/django-colorfield?color=0C4B33&logo=django&logoColor=white&label=django)](https://www.djangoproject.com/)
-        
-        [![](https://img.shields.io/pypi/v/django-colorfield.svg?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/django-colorfield/)
-        [![](https://pepy.tech/badge/django-colorfield/month)](https://pepy.tech/project/django-colorfield)
-        [![](https://img.shields.io/github/stars/fabiocaccamo/django-colorfield?logo=github)](https://github.com/fabiocaccamo/django-colorfield/)
-        [![](https://badges.pufler.dev/visits/fabiocaccamo/django-colorfield?label=visitors&color=blue)](https://badges.pufler.dev)
-        [![](https://img.shields.io/pypi/l/django-colorfield.svg?color=blue)](https://github.com/fabiocaccamo/django-colorfield/blob/master/LICENSE.txt)
-        
-        [![](https://results.pre-commit.ci/badge/github/fabiocaccamo/django-colorfield/master.svg)](https://results.pre-commit.ci/latest/github/fabiocaccamo/django-colorfield/master)
-        [![](https://img.shields.io/github/workflow/status/fabiocaccamo/django-colorfield/Test%20package?label=build&logo=github)](https://github.com/fabiocaccamo/django-colorfield)
-        [![](https://img.shields.io/codecov/c/gh/fabiocaccamo/django-colorfield?logo=codecov)](https://codecov.io/gh/fabiocaccamo/django-colorfield)
-        [![](https://img.shields.io/codacy/grade/194566618f424a819ce43450ea0af081?logo=codacy)](https://www.codacy.com/app/fabiocaccamo/django-colorfield)
-        [![](https://img.shields.io/codeclimate/maintainability/fabiocaccamo/django-colorfield?logo=code-climate)](https://codeclimate.com/github/fabiocaccamo/django-colorfield/)
-        [![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
-        
-        # django-colorfield
-        simple color field for your models with a nice color-picker in the admin-interface.
-        
-        ![django-colorfield-hex](https://user-images.githubusercontent.com/7900305/104512324-51ed0f80-55ee-11eb-9144-de03d922c2ce.png)
-        ![django-colorfield-hexa](https://user-images.githubusercontent.com/7900305/104512063-ec991e80-55ed-11eb-95b6-9174ac3f4f38.png)
-        
-        ---
-        
-        ## Installation
-        -   Run `pip install django-colorfield`
-        -   Add `colorfield` to `settings.INSTALLED_APPS`
-        -   Run `python manage.py collectstatic`
-        -   Restart your application server
-        
-        ---
-        
-        ## Usage
-        
-        ### Settings
-        This package doesn't need any setting.
-        
-        ### Models
-        Just add color field(s) to your models like this:
-        
-        ```python
-        from colorfield.fields import ColorField
-        from django.db import models
-        
-        class MyModel(model.Model):
-            color = ColorField(default='#FF0000')
-        ```
-        
-        ### Field Options
-        These are the supported custom options: [`format`](#format), [`image_field`](#image_field), [`samples`](#samples)
-        
-        #### format
-        
-        The following formats are supported: `hex` *(default)*, `hexa`.
-        
-        ```python
-        from colorfield.fields import ColorField
-        from django.db import models
-        
-        class MyModel(model.Model):
-            color = ColorField(format="hexa")
-        ```
-        
-        #### image_field
-        
-        It is possible to auto-populate the field value getting the color from an image using the `image_field` option.
-        
-        The color will be calculated from the **top-left pixel** color of the image each time the model instance is saved.
-        
-        ```python
-        from colorfield.fields import ColorField
-        from django.db import models
-        
-        class MyModel(model.Model):
-            image = models.ImageField(upload_to="images")
-            color = ColorField(image_field="image")
-        ```
-        
-        #### samples
-        
-        It is possible to provide a palette of colors to choose from to the widget using the `samples` option.
-        
-        This option **is not restrictive** (on the contrary of `choices` option), it is also possible to choose another color from the spectrum.
-        
-        ![django-colorfield-samples](https://user-images.githubusercontent.com/7900305/104512178-194d3600-55ee-11eb-8cba-91cca156da06.png)
-        
-        ```python
-        from colorfield.fields import ColorField
-        from django.db import models
-        
-        class MyModel(model.Model):
-        
-            COLOR_PALETTE = [
-                ("#FFFFFF", "white", ),
-                ("#000000", "black", ),
-            ]
-        
-            # not restrictive, allows the selection of another color from the spectrum.
-            color = ColorField(samples=COLOR_PALETTE)
-        
-            # restrictive, it is mandatory to choose a color from the palette
-            color = ColorField(choices=COLOR_PALETTE)
-        ```
-        
-        ### Admin
-        The admin will kindly provide a simple [color picker](http://jscolor.com/) for all color fields. :)
-        
-        ---
-        
-        ## Testing
-        ```bash
-        # clone repository
-        git clone https://github.com/fabiocaccamo/django-colorfield.git && cd django-colorfield
-        
-        # create virtualenv and activate it
-        python -m venv venv && . venv/bin/activate
-        
-        # upgrade pip
-        python -m pip install --upgrade pip
-        
-        # install requirements
-        pip install -r requirements.txt -r requirements-test.txt
-        
-        # run tests
-        tox
-        # or
-        python setup.py test
-        # or
-        python -m django test --settings "tests.settings"
-        ```
-        ---
-        
-        ## Credits
-        Originally developed by [Jared Forsyth](https://github.com/jaredly)
-        
-        ---
-        
-        ## License
-        Released under [MIT License](LICENSE.txt).
-        
-        ---
-        
-        ## Supporting
-        
-        - :star: Star this project on [GitHub](https://github.com/fabiocaccamo/django-colorfield)
-        - :octocat: Follow me on [GitHub](https://github.com/fabiocaccamo)
-        - :blue_heart: Follow me on [Twitter](https://twitter.com/fabiocaccamo)
-        - :moneybag: Sponsor me on [Github](https://github.com/sponsors/fabiocaccamo)
-        
-        ## See also
-        
-        - [`django-admin-interface`](https://github.com/fabiocaccamo/django-admin-interface) - the default admin interface made customizable by the admin itself. popup windows replaced by modals. 🧙 ⚡
-        
-        - [`django-extra-settings`](https://github.com/fabiocaccamo/django-extra-settings) - config and manage typed extra settings using just the django admin. ⚙️
-        
-        - [`django-maintenance-mode`](https://github.com/fabiocaccamo/django-maintenance-mode) - shows a 503 error page when maintenance-mode is on. 🚧 🛠️
-        
-        - [`django-redirects`](https://github.com/fabiocaccamo/django-redirects) - redirects with full control. ↪️
-        
-        - [`django-treenode`](https://github.com/fabiocaccamo/django-treenode) - probably the best abstract model / admin for your tree based stuff. 🌳
-        
-        - [`python-benedict`](https://github.com/fabiocaccamo/python-benedict) - dict subclass with keylist/keypath support, I/O shortcuts (base64, csv, json, pickle, plist, query-string, toml, xml, yaml) and many utilities. 📘
-        
-        - [`python-codicefiscale`](https://github.com/fabiocaccamo/python-codicefiscale) - encode/decode Italian fiscal codes - codifica/decodifica del Codice Fiscale. 🇮🇹 💳
-        
-        - [`python-fontbro`](https://github.com/fabiocaccamo/python-fontbro) - friendly font operations. 🧢
-        
-        - [`python-fsutil`](https://github.com/fabiocaccamo/python-fsutil) - file-system utilities for lazy devs. 🧟‍♂️
-        
 Keywords: django,colorfield,colorpicker,color,field,picker,chooser,admin,python
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
-Classifier: Framework :: Django :: 2.2
 Classifier: Framework :: Django :: 3.0
 Classifier: Framework :: Django :: 3.1
 Classifier: Framework :: Django :: 3.2
 Classifier: Framework :: Django :: 4.0
 Classifier: Framework :: Django :: 4.1
+Classifier: Framework :: Django :: 4.2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Build Tools
-Requires: django (>=2.2)
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+[![](https://img.shields.io/pypi/pyversions/django-colorfield.svg?color=3776AB&logo=python&logoColor=white)](https://www.python.org/)
+[![](https://img.shields.io/pypi/djversions/django-colorfield?color=0C4B33&logo=django&logoColor=white&label=django)](https://www.djangoproject.com/)
+
+[![](https://img.shields.io/pypi/v/django-colorfield.svg?color=blue&logo=pypi&logoColor=white)](https://pypi.org/project/django-colorfield/)
+[![](https://pepy.tech/badge/django-colorfield/month)](https://pepy.tech/project/django-colorfield)
+[![](https://img.shields.io/github/stars/fabiocaccamo/django-colorfield?logo=github)](https://github.com/fabiocaccamo/django-colorfield/stargazers)
+[![](https://img.shields.io/pypi/l/django-colorfield.svg?color=blue)](https://github.com/fabiocaccamo/django-colorfield/blob/main/LICENSE.txt)
+
+[![](https://results.pre-commit.ci/badge/github/fabiocaccamo/django-colorfield/main.svg)](https://results.pre-commit.ci/latest/github/fabiocaccamo/django-colorfield/main)
+[![](https://img.shields.io/github/actions/workflow/status/fabiocaccamo/django-colorfield/test-package.yml?branch=main&label=build&logo=github)](https://github.com/fabiocaccamo/django-colorfield)
+[![](https://img.shields.io/codecov/c/gh/fabiocaccamo/django-colorfield?logo=codecov)](https://codecov.io/gh/fabiocaccamo/django-colorfield)
+[![](https://img.shields.io/codacy/grade/194566618f424a819ce43450ea0af081?logo=codacy)](https://www.codacy.com/app/fabiocaccamo/django-colorfield)
+[![](https://img.shields.io/codeclimate/maintainability/fabiocaccamo/django-colorfield?logo=code-climate)](https://codeclimate.com/github/fabiocaccamo/django-colorfield/)
+[![](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+
+# django-colorfield
+simple color field for your models with a nice color-picker in the admin-interface.
+
+![django-colorfield-hex](https://user-images.githubusercontent.com/7900305/104512324-51ed0f80-55ee-11eb-9144-de03d922c2ce.png)
+![django-colorfield-hexa](https://user-images.githubusercontent.com/7900305/104512063-ec991e80-55ed-11eb-95b6-9174ac3f4f38.png)
+
+---
+
+## Installation
+-   Run `pip install django-colorfield`
+-   Add `colorfield` to `settings.INSTALLED_APPS`
+-   Run `python manage.py collectstatic`
+-   Restart your application server
+
+---
+
+## Usage
+
+### Settings
+This package doesn't need any setting.
+
+### Models
+Just add color field(s) to your models like this:
+
+```python
+from colorfield.fields import ColorField
+from django.db import models
+
+class MyModel(model.Model):
+    color = ColorField(default='#FF0000')
+```
+
+### Field Options
+These are the supported custom options: [`format`](#format), [`image_field`](#image_field), [`samples`](#samples)
+
+#### format
+
+The following formats are supported: `hex` *(default)*, `hexa`.
+
+```python
+from colorfield.fields import ColorField
+from django.db import models
+
+class MyModel(model.Model):
+    color = ColorField(format="hexa")
+```
+
+#### image_field
+
+It is possible to auto-populate the field value getting the color from an image using the `image_field` option.
+
+The color will be calculated from the **top-left pixel** color of the image each time the model instance is saved.
+
+```python
+from colorfield.fields import ColorField
+from django.db import models
+
+class MyModel(model.Model):
+    image = models.ImageField(upload_to="images")
+    color = ColorField(image_field="image")
+```
+
+#### samples
+
+It is possible to provide a palette of colors to choose from to the widget using the `samples` option.
+
+This option **is not restrictive** (on the contrary of `choices` option), it is also possible to choose another color from the spectrum.
+
+![django-colorfield-samples](https://user-images.githubusercontent.com/7900305/104512178-194d3600-55ee-11eb-8cba-91cca156da06.png)
+
+```python
+from colorfield.fields import ColorField
+from django.db import models
+
+class MyModel(model.Model):
+
+    COLOR_PALETTE = [
+        ("#FFFFFF", "white", ),
+        ("#000000", "black", ),
+    ]
+
+    # not restrictive, allows the selection of another color from the spectrum.
+    color = ColorField(samples=COLOR_PALETTE)
+
+    # restrictive, it is mandatory to choose a color from the palette
+    color = ColorField(choices=COLOR_PALETTE)
+```
+
+### Admin
+The admin will kindly provide a simple [color picker](http://jscolor.com/) for all color fields. :)
+
+---
+
+## Testing
+```bash
+# clone repository
+git clone https://github.com/fabiocaccamo/django-colorfield.git && cd django-colorfield
+
+# create virtualenv and activate it
+python -m venv venv && . venv/bin/activate
+
+# upgrade pip
+python -m pip install --upgrade pip
+
+# install requirements
+pip install -r requirements.txt -r requirements-test.txt
+
+# install pre-commit to run formatters and linters
+pre-commit install --install-hooks
+
+# run tests
+tox
+# or
+python runtests.py
+# or
+python -m django test --settings "tests.settings"
+```
+---
+
+## Credits
+Originally developed by [Jared Forsyth](https://github.com/jaredly)
+
+---
+
+## License
+Released under [MIT License](LICENSE.txt).
+
+---
+
+## Supporting
+
+- :star: Star this project on [GitHub](https://github.com/fabiocaccamo/django-colorfield)
+- :octocat: Follow me on [GitHub](https://github.com/fabiocaccamo)
+- :blue_heart: Follow me on [Twitter](https://twitter.com/fabiocaccamo)
+- :moneybag: Sponsor me on [Github](https://github.com/sponsors/fabiocaccamo)
+
+## See also
+
+- [`django-admin-interface`](https://github.com/fabiocaccamo/django-admin-interface) - the default admin interface made customizable by the admin itself. popup windows replaced by modals. 🧙 ⚡
+
+- [`django-extra-settings`](https://github.com/fabiocaccamo/django-extra-settings) - config and manage typed extra settings using just the django admin. ⚙️
+
+- [`django-maintenance-mode`](https://github.com/fabiocaccamo/django-maintenance-mode) - shows a 503 error page when maintenance-mode is on. 🚧 🛠️
+
+- [`django-redirects`](https://github.com/fabiocaccamo/django-redirects) - redirects with full control. ↪️
+
+- [`django-treenode`](https://github.com/fabiocaccamo/django-treenode) - probably the best abstract model / admin for your tree based stuff. 🌳
+
+- [`python-benedict`](https://github.com/fabiocaccamo/python-benedict) - dict subclass with keylist/keypath support, I/O shortcuts (base64, csv, json, pickle, plist, query-string, toml, xml, yaml) and many utilities. 📘
+
+- [`python-codicefiscale`](https://github.com/fabiocaccamo/python-codicefiscale) - encode/decode Italian fiscal codes - codifica/decodifica del Codice Fiscale. 🇮🇹 💳
+
+- [`python-fontbro`](https://github.com/fabiocaccamo/python-fontbro) - friendly font operations. 🧢
+
+- [`python-fsutil`](https://github.com/fabiocaccamo/python-fsutil) - file-system utilities for lazy devs. 🧟‍♂️
```

### Comparing `django-colorfield-0.8.0/setup.py` & `django-colorfield-0.9.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,79 +1,101 @@
-#!/usr/bin/env python
+[build-system]
+requires = ["setuptools"]
+build-backend = "setuptools.build_meta"
 
-import os
-import sys
+[project]
+name = "django-colorfield"
+description = "color field for django models with a nice color-picker in the admin."
+authors = [
+    { name = "Jared Forsyth", email = "jared@jaredforsyth.com" },
+    { name = "Fabio Caccamo", email = "fabio.caccamo@gmail.com" },
+]
+keywords = [
+    "django",
+    "colorfield",
+    "colorpicker",
+    "color",
+    "field",
+    "picker",
+    "chooser",
+    "admin",
+    "python",
+]
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Environment :: Web Environment",
+    "Framework :: Django",
+    "Framework :: Django :: 3.0",
+    "Framework :: Django :: 3.1",
+    "Framework :: Django :: 3.2",
+    "Framework :: Django :: 4.0",
+    "Framework :: Django :: 4.1",
+    "Framework :: Django :: 4.2",
+    "Intended Audience :: Developers",
+    "License :: OSI Approved :: MIT License",
+    "Natural Language :: English",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: Software Development :: Build Tools",
+]
+dependencies = [
+    "Pillow (>= 9.0.0)",
+]
+dynamic = ["version"]
+maintainers = [
+    { name = "Fabio Caccamo", email = "fabio.caccamo@gmail.com" },
+]
 
-from setuptools import find_packages, setup
+[project.readme]
+file = "README.md"
+content-type = "text/markdown"
 
-exec(open("colorfield/version.py").read())
+[project.license]
+file = "LICENSE.txt"
+content-type = "text/plain"
 
-github_url = "https://github.com/fabiocaccamo"
-sponsor_url = "https://github.com/sponsors/fabiocaccamo/"
-twitter_url = "https://twitter.com/fabiocaccamo"
-package_name = "django-colorfield"
-package_url = "{}/{}".format(github_url, package_name)
-package_path = os.path.abspath(os.path.dirname(__file__))
-long_description_file_path = os.path.join(package_path, "README.md")
-long_description_content_type = "text/markdown"
-long_description = ""
-try:
-    with open(long_description_file_path, "r", encoding="utf-8") as f:
-        long_description = f.read()
-except IOError:
-    pass
-
-setup(
-    name=package_name,
-    packages=find_packages(exclude=["contrib", "docs", "tests*"]),
-    include_package_data=True,
-    version=__version__,
-    description="simple color field for your models with a nice color-picker in the admin-interface.",
-    long_description=long_description,
-    long_description_content_type=long_description_content_type,
-    author="Jared Forsyth, Fabio Caccamo",
-    author_email="jared@jaredforsyth.com, fabio.caccamo@gmail.com",
-    url=package_url,
-    download_url="{}/archive/{}.tar.gz".format(package_url, __version__),
-    project_urls={
-        "Documentation": "{}#readme".format(package_url),
-        "Issues": "{}/issues".format(package_url),
-        "Funding": sponsor_url,
-        "Twitter": twitter_url,
-    },
-    keywords=[
-        "django",
-        "colorfield",
-        "colorpicker",
-        "color",
-        "field",
-        "picker",
-        "chooser",
-        "admin",
-        "python",
-    ],
-    requires=["django (>=2.2)"],
-    install_requires=["Pillow (>=9.0.0)"],
-    classifiers=[
-        "Development Status :: 5 - Production/Stable",
-        "Environment :: Web Environment",
-        "Framework :: Django",
-        "Framework :: Django :: 2.2",
-        "Framework :: Django :: 3.0",
-        "Framework :: Django :: 3.1",
-        "Framework :: Django :: 3.2",
-        "Framework :: Django :: 4.0",
-        "Framework :: Django :: 4.1",
-        "Intended Audience :: Developers",
-        "License :: OSI Approved :: MIT License",
-        "Natural Language :: English",
-        "Operating System :: OS Independent",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "Topic :: Software Development :: Build Tools",
-    ],
-    license="MIT",
-    test_suite="runtests.runtests",
-)
+[project.urls]
+Homepage = "https://github.com/fabiocaccamo/django-colorfield"
+Download = "https://github.com/fabiocaccamo/django-colorfield/releases"
+Documentation = "https://github.com/fabiocaccamo/django-colorfield#readme"
+Issues = "https://github.com/fabiocaccamo/django-colorfield/issues"
+Funding = "https://github.com/sponsors/fabiocaccamo/"
+Twitter = "https://twitter.com/fabiocaccamo"
+
+[tool.black]
+line-length = 88
+include = '\.pyi?$'
+exclude = '''
+/(
+    \.git
+  | \.hg
+  | \.mypy_cache
+  | \.tox
+  | \.venv
+  | _build
+  | buck-out
+  | build
+  | dist
+  | venv
+)/
+'''
+
+[tool.isort]
+profile = "black"
+
+[tool.ruff]
+ignore = []
+line-length = 88
+select = ["B", "B9", "C", "E", "F", "W"]
+
+[tool.ruff.mccabe]
+max-complexity = 10
+
+[tool.setuptools.packages.find]
+include = ["colorfield*"]
+
+[tool.setuptools.dynamic.version]
+attr = "colorfield.metadata.__version__"
```

