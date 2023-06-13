# Comparing `tmp/django-proemail-template-0.2.3.tar.gz` & `tmp/django-proemail-template-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-proemail-template-0.2.3.tar", last modified: Fri Jun  2 16:26:23 2023, max compression
+gzip compressed data, was "django-proemail-template-0.2.4.tar", last modified: Tue Jun 13 16:33:59 2023, max compression
```

## Comparing `django-proemail-template-0.2.3.tar` & `django-proemail-template-0.2.4.tar`

### file list

```diff
@@ -1,25 +1,26 @@
-drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:26:23.831401 django-proemail-template-0.2.3/
-drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:26:23.829312 django-proemail-template-0.2.3/EmailTemplate/
--rw-r--r--   0 teppss     (501) staff       (20)        0 2022-04-05 14:10:09.000000 django-proemail-template-0.2.3/EmailTemplate/__init__.py
--rw-r--r--   0 teppss     (501) staff       (20)      706 2023-06-02 16:23:37.000000 django-proemail-template-0.2.3/EmailTemplate/admin.py
-drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:26:23.830647 django-proemail-template-0.2.3/EmailTemplate/migrations/
--rw-r--r--   0 teppss     (501) staff       (20)     1232 2022-04-05 14:05:32.000000 django-proemail-template-0.2.3/EmailTemplate/migrations/0001_initial.py
--rw-r--r--   0 teppss     (501) staff       (20)      445 2022-04-05 14:05:32.000000 django-proemail-template-0.2.3/EmailTemplate/migrations/0002_auto_20190719_1354.py
--rw-r--r--   0 teppss     (501) staff       (20)      482 2022-04-05 14:05:32.000000 django-proemail-template-0.2.3/EmailTemplate/migrations/0003_auto_20190719_1358.py
--rw-r--r--   0 teppss     (501) staff       (20)      445 2022-04-05 14:05:32.000000 django-proemail-template-0.2.3/EmailTemplate/migrations/0004_auto_20210226_0911.py
--rw-r--r--   0 teppss     (501) staff       (20)      637 2022-04-05 14:12:58.000000 django-proemail-template-0.2.3/EmailTemplate/migrations/0005_emailtemplate_bcc_emailtemplate_cc.py
--rw-r--r--   0 teppss     (501) staff       (20)        0 2022-04-05 14:05:32.000000 django-proemail-template-0.2.3/EmailTemplate/migrations/__init__.py
--rw-r--r--   0 teppss     (501) staff       (20)     5468 2023-06-02 16:16:34.000000 django-proemail-template-0.2.3/EmailTemplate/models.py
--rw-r--r--   0 teppss     (501) staff       (20)      449 2021-02-26 09:04:46.000000 django-proemail-template-0.2.3/EmailTemplate/tests.py
--rw-r--r--   0 teppss     (501) staff       (20)       63 2018-11-14 15:29:47.000000 django-proemail-template-0.2.3/EmailTemplate/views.py
--rw-r--r--   0 teppss     (501) staff       (20)     1065 2019-07-12 02:22:08.000000 django-proemail-template-0.2.3/LICENSE
--rw-r--r--   0 teppss     (501) staff       (20)       60 2022-05-19 14:16:14.000000 django-proemail-template-0.2.3/MANIFEST.in
--rw-r--r--   0 teppss     (501) staff       (20)     1803 2023-06-02 16:26:23.831287 django-proemail-template-0.2.3/PKG-INFO
--rw-r--r--   0 teppss     (501) staff       (20)      979 2020-02-01 09:44:20.000000 django-proemail-template-0.2.3/README.rst
-drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-02 16:26:23.831120 django-proemail-template-0.2.3/django_proemail_template.egg-info/
--rw-r--r--   0 teppss     (501) staff       (20)     1803 2023-06-02 16:26:23.000000 django-proemail-template-0.2.3/django_proemail_template.egg-info/PKG-INFO
--rw-r--r--   0 teppss     (501) staff       (20)      652 2023-06-02 16:26:23.000000 django-proemail-template-0.2.3/django_proemail_template.egg-info/SOURCES.txt
--rw-r--r--   0 teppss     (501) staff       (20)        1 2023-06-02 16:26:23.000000 django-proemail-template-0.2.3/django_proemail_template.egg-info/dependency_links.txt
--rw-r--r--   0 teppss     (501) staff       (20)       14 2023-06-02 16:26:23.000000 django-proemail-template-0.2.3/django_proemail_template.egg-info/top_level.txt
--rw-r--r--   0 teppss     (501) staff       (20)       38 2023-06-02 16:26:23.831436 django-proemail-template-0.2.3/setup.cfg
--rw-r--r--   0 teppss     (501) staff       (20)     1191 2023-06-02 16:26:20.000000 django-proemail-template-0.2.3/setup.py
+drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-13 16:33:59.136359 django-proemail-template-0.2.4/
+drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-13 16:33:59.132922 django-proemail-template-0.2.4/EmailTemplate/
+-rw-r--r--   0 teppss     (501) staff       (20)        0 2022-04-05 14:10:09.000000 django-proemail-template-0.2.4/EmailTemplate/__init__.py
+-rw-r--r--   0 teppss     (501) staff       (20)      706 2023-06-02 16:23:37.000000 django-proemail-template-0.2.4/EmailTemplate/admin.py
+drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-13 16:33:59.134917 django-proemail-template-0.2.4/EmailTemplate/migrations/
+-rw-r--r--   0 teppss     (501) staff       (20)     1232 2022-04-05 14:05:32.000000 django-proemail-template-0.2.4/EmailTemplate/migrations/0001_initial.py
+-rw-r--r--   0 teppss     (501) staff       (20)      445 2022-04-05 14:05:32.000000 django-proemail-template-0.2.4/EmailTemplate/migrations/0002_auto_20190719_1354.py
+-rw-r--r--   0 teppss     (501) staff       (20)      482 2022-04-05 14:05:32.000000 django-proemail-template-0.2.4/EmailTemplate/migrations/0003_auto_20190719_1358.py
+-rw-r--r--   0 teppss     (501) staff       (20)      445 2022-04-05 14:05:32.000000 django-proemail-template-0.2.4/EmailTemplate/migrations/0004_auto_20210226_0911.py
+-rw-r--r--   0 teppss     (501) staff       (20)      637 2022-04-05 14:12:58.000000 django-proemail-template-0.2.4/EmailTemplate/migrations/0005_emailtemplate_bcc_emailtemplate_cc.py
+-rw-r--r--   0 teppss     (501) staff       (20)     1469 2023-06-13 16:31:12.000000 django-proemail-template-0.2.4/EmailTemplate/migrations/0006_emaillog.py
+-rw-r--r--   0 teppss     (501) staff       (20)        0 2022-04-05 14:05:32.000000 django-proemail-template-0.2.4/EmailTemplate/migrations/__init__.py
+-rw-r--r--   0 teppss     (501) staff       (20)     5468 2023-06-02 16:16:34.000000 django-proemail-template-0.2.4/EmailTemplate/models.py
+-rw-r--r--   0 teppss     (501) staff       (20)      449 2021-02-26 09:04:46.000000 django-proemail-template-0.2.4/EmailTemplate/tests.py
+-rw-r--r--   0 teppss     (501) staff       (20)       63 2018-11-14 15:29:47.000000 django-proemail-template-0.2.4/EmailTemplate/views.py
+-rw-r--r--   0 teppss     (501) staff       (20)     1065 2019-07-12 02:22:08.000000 django-proemail-template-0.2.4/LICENSE
+-rw-r--r--   0 teppss     (501) staff       (20)       60 2022-05-19 14:16:14.000000 django-proemail-template-0.2.4/MANIFEST.in
+-rw-r--r--   0 teppss     (501) staff       (20)     1803 2023-06-13 16:33:59.136207 django-proemail-template-0.2.4/PKG-INFO
+-rw-r--r--   0 teppss     (501) staff       (20)      979 2020-02-01 09:44:20.000000 django-proemail-template-0.2.4/README.rst
+drwxr-xr-x   0 teppss     (501) staff       (20)        0 2023-06-13 16:33:59.135868 django-proemail-template-0.2.4/django_proemail_template.egg-info/
+-rw-r--r--   0 teppss     (501) staff       (20)     1803 2023-06-13 16:33:59.000000 django-proemail-template-0.2.4/django_proemail_template.egg-info/PKG-INFO
+-rw-r--r--   0 teppss     (501) staff       (20)      694 2023-06-13 16:33:59.000000 django-proemail-template-0.2.4/django_proemail_template.egg-info/SOURCES.txt
+-rw-r--r--   0 teppss     (501) staff       (20)        1 2023-06-13 16:33:59.000000 django-proemail-template-0.2.4/django_proemail_template.egg-info/dependency_links.txt
+-rw-r--r--   0 teppss     (501) staff       (20)       14 2023-06-13 16:33:59.000000 django-proemail-template-0.2.4/django_proemail_template.egg-info/top_level.txt
+-rw-r--r--   0 teppss     (501) staff       (20)       38 2023-06-13 16:33:59.136501 django-proemail-template-0.2.4/setup.cfg
+-rw-r--r--   0 teppss     (501) staff       (20)     1191 2023-06-13 16:31:56.000000 django-proemail-template-0.2.4/setup.py
```

### Comparing `django-proemail-template-0.2.3/EmailTemplate/admin.py` & `django-proemail-template-0.2.4/EmailTemplate/admin.py`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.2.3/EmailTemplate/migrations/0001_initial.py` & `django-proemail-template-0.2.4/EmailTemplate/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.2.3/EmailTemplate/migrations/0005_emailtemplate_bcc_emailtemplate_cc.py` & `django-proemail-template-0.2.4/EmailTemplate/migrations/0005_emailtemplate_bcc_emailtemplate_cc.py`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.2.3/EmailTemplate/models.py` & `django-proemail-template-0.2.4/EmailTemplate/models.py`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.2.3/LICENSE` & `django-proemail-template-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.2.3/PKG-INFO` & `django-proemail-template-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-proemail-template
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple Django app to send emails
 Home-page: https://github.com/iwalucas/django-email-template/
 Author: Lucas
 Author-email: teppss@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-proemail-template-0.2.3/README.rst` & `django-proemail-template-0.2.4/README.rst`

 * *Files identical despite different names*

### Comparing `django-proemail-template-0.2.3/django_proemail_template.egg-info/PKG-INFO` & `django-proemail-template-0.2.4/django_proemail_template.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-proemail-template
-Version: 0.2.3
+Version: 0.2.4
 Summary: A simple Django app to send emails
 Home-page: https://github.com/iwalucas/django-email-template/
 Author: Lucas
 Author-email: teppss@gmail.com
 License: MIT License
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

### Comparing `django-proemail-template-0.2.3/django_proemail_template.egg-info/SOURCES.txt` & `django-proemail-template-0.2.4/django_proemail_template.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -8,12 +8,13 @@
 EmailTemplate/tests.py
 EmailTemplate/views.py
 EmailTemplate/migrations/0001_initial.py
 EmailTemplate/migrations/0002_auto_20190719_1354.py
 EmailTemplate/migrations/0003_auto_20190719_1358.py
 EmailTemplate/migrations/0004_auto_20210226_0911.py
 EmailTemplate/migrations/0005_emailtemplate_bcc_emailtemplate_cc.py
+EmailTemplate/migrations/0006_emaillog.py
 EmailTemplate/migrations/__init__.py
 django_proemail_template.egg-info/PKG-INFO
 django_proemail_template.egg-info/SOURCES.txt
 django_proemail_template.egg-info/dependency_links.txt
 django_proemail_template.egg-info/top_level.txt
```

### Comparing `django-proemail-template-0.2.3/setup.py` & `django-proemail-template-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     README = readme.read()
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 setup(
     name='django-proemail-template',
-    version='0.2.3',
+    version='0.2.4',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A simple Django app to send emails',
     long_description=README,
     url='https://github.com/iwalucas/django-email-template/',
     author='Lucas',
```

