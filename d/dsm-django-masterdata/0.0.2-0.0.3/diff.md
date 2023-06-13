# Comparing `tmp/dsm_django_masterdata-0.0.2.tar.gz` & `tmp/dsm_django_masterdata-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dsm_django_masterdata-0.0.2.tar", last modified: Mon Jun 12 15:36:22 2023, max compression
+gzip compressed data, was "dsm_django_masterdata-0.0.3.tar", last modified: Tue Jun 13 15:58:35 2023, max compression
```

## Comparing `dsm_django_masterdata-0.0.2.tar` & `dsm_django_masterdata-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:36:22.201526 dsm_django_masterdata-0.0.2/
--rw-r--r--   0 naii       (501) staff       (20)      995 2023-06-12 15:36:22.200716 dsm_django_masterdata-0.0.2/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      386 2023-06-12 15:35:40.000000 dsm_django_masterdata-0.0.2/README.md
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:36:22.192579 dsm_django_masterdata-0.0.2/dsm_django_masterdata/
--rw-r--r--   0 naii       (501) staff       (20)      153 2023-06-12 15:36:06.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)      165 2023-06-12 15:30:14.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/apps.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:36:22.198243 dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/
--rw-r--r--   0 naii       (501) staff       (20)        0 2023-06-12 09:43:46.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)      327 2023-06-12 10:06:08.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/admin.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:36:22.199945 dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/migrations/
--rw-r--r--   0 naii       (501) staff       (20)     1093 2023-06-12 15:25:37.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/migrations/0001_initial.py
--rw-r--r--   0 naii       (501) staff       (20)        0 2023-06-12 09:50:06.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/migrations/__init__.py
--rw-r--r--   0 naii       (501) staff       (20)      395 2023-06-12 11:19:07.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/models.py
--rw-r--r--   0 naii       (501) staff       (20)       60 2023-06-12 09:43:33.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata/tests.py
-drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-12 15:36:22.196671 dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/
--rw-r--r--   0 naii       (501) staff       (20)      995 2023-06-12 15:36:22.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/PKG-INFO
--rw-r--r--   0 naii       (501) staff       (20)      563 2023-06-12 15:36:22.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/SOURCES.txt
--rw-r--r--   0 naii       (501) staff       (20)        1 2023-06-12 15:36:22.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/dependency_links.txt
--rw-r--r--   0 naii       (501) staff       (20)       15 2023-06-12 15:36:22.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/requires.txt
--rw-r--r--   0 naii       (501) staff       (20)       22 2023-06-12 15:36:22.000000 dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/top_level.txt
--rw-r--r--   0 naii       (501) staff       (20)       38 2023-06-12 15:36:22.201715 dsm_django_masterdata-0.0.2/setup.cfg
--rw-r--r--   0 naii       (501) staff       (20)     1315 2023-06-12 15:36:16.000000 dsm_django_masterdata-0.0.2/setup.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-13 15:58:35.193173 dsm_django_masterdata-0.0.3/
+-rw-r--r--   0 naii       (501) staff       (20)     1181 2023-06-13 15:58:35.192609 dsm_django_masterdata-0.0.3/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      572 2023-06-13 15:58:01.000000 dsm_django_masterdata-0.0.3/README.md
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-13 15:58:35.182496 dsm_django_masterdata-0.0.3/dsm_django_masterdata/
+-rw-r--r--   0 naii       (501) staff       (20)      153 2023-06-13 15:58:26.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      291 2023-06-13 15:49:04.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/apps.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-13 15:58:35.188667 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/
+-rw-r--r--   0 naii       (501) staff       (20)        0 2023-06-12 09:43:46.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      327 2023-06-12 10:06:08.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/admin.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-13 15:58:35.191670 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/migrations/
+-rw-r--r--   0 naii       (501) staff       (20)     1110 2023-06-13 15:54:02.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/migrations/0001_initial.py
+-rw-r--r--   0 naii       (501) staff       (20)      337 2023-06-13 15:50:16.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/migrations/0002_alter_hscode_options.py
+-rw-r--r--   0 naii       (501) staff       (20)        0 2023-06-12 09:50:06.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/migrations/__init__.py
+-rw-r--r--   0 naii       (501) staff       (20)      395 2023-06-12 11:19:07.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/models.py
+-rw-r--r--   0 naii       (501) staff       (20)       60 2023-06-12 09:43:33.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata/tests.py
+drwxr-xr-x   0 naii       (501) staff       (20)        0 2023-06-13 15:58:35.187108 dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/
+-rw-r--r--   0 naii       (501) staff       (20)     1181 2023-06-13 15:58:35.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/PKG-INFO
+-rw-r--r--   0 naii       (501) staff       (20)      632 2023-06-13 15:58:35.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/SOURCES.txt
+-rw-r--r--   0 naii       (501) staff       (20)        1 2023-06-13 15:58:35.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/dependency_links.txt
+-rw-r--r--   0 naii       (501) staff       (20)       15 2023-06-13 15:58:35.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/requires.txt
+-rw-r--r--   0 naii       (501) staff       (20)       22 2023-06-13 15:58:35.000000 dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/top_level.txt
+-rw-r--r--   0 naii       (501) staff       (20)       38 2023-06-13 15:58:35.193343 dsm_django_masterdata-0.0.3/setup.cfg
+-rw-r--r--   0 naii       (501) staff       (20)     1315 2023-06-13 15:58:12.000000 dsm_django_masterdata-0.0.3/setup.py
```

### Comparing `dsm_django_masterdata-0.0.2/PKG-INFO` & `dsm_django_masterdata-0.0.3/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 Metadata-Version: 2.1
 Name: dsm_django_masterdata
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple way to use Master Data in django project.
 Home-page: https://github.com/storemesh/masterdata/tree/django-app
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
 # Django Master data
-0. install dsm_master
+0. install dsm-django-masterdata
 ```
-pip install dsm_master
+pip install pip install dsm-django-masterdata
 ```
 1. install django app in `settings.py`
 ```python
 INSTALLED_APPS = [
     ...
     'dsm_django_masterdata.hscode',
+    'dsm_django_masterdata.area',
     ...
 ]
 ```
 
 2. migrate database
 ```
 python manage.py migrate
 ```
 
 3. check data in admin page
 
 ## How to use
+- HScode
 ```python
-from dsm_master.hscode.models import HScode
+from dsm_django_masterdata.hscode.models import HScode
 hs_code = HScode.objects.all()
 ```
+- Area
+```python
+from dsm_django_masterdata.area.models import Area
+area = Area.objects.all()
+```
```

### Comparing `dsm_django_masterdata-0.0.2/dsm_django_masterdata/hscode/migrations/0001_initial.py` & `dsm_django_masterdata-0.0.3/dsm_django_masterdata/hscode/migrations/0001_initial.py`

 * *Files 16% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 def get_hscode(apps, schema_editor):
     print(f"Get hscode from {hscode_url}")
     df = pd.read_parquet(hscode_url, engine='pyarrow')
     bluck = [HScode(**elm) for elm in df.to_dict('records')]
     with transaction.atomic():
         HScode.objects.bulk_create(bluck)
-    print("Import hscode to HScode, Sucessful!")
+    print(f"Import hscode to HScode, Sucessful! => {len(bluck)}")
 
 class Migration(migrations.Migration):
 
     initial = True
 
     dependencies = [
     ]
```

### Comparing `dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/PKG-INFO` & `dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,42 +1,49 @@
 Metadata-Version: 2.1
 Name: dsm-django-masterdata
-Version: 0.0.2
+Version: 0.0.3
 Summary: A simple way to use Master Data in django project.
 Home-page: https://github.com/storemesh/masterdata/tree/django-app
 Author: DigitalStoreMesh Co.,Ltd
 Author-email: contact@storemesh.com
 License: MIT License
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
 
 # Django Master data
-0. install dsm_master
+0. install dsm-django-masterdata
 ```
-pip install dsm_master
+pip install pip install dsm-django-masterdata
 ```
 1. install django app in `settings.py`
 ```python
 INSTALLED_APPS = [
     ...
     'dsm_django_masterdata.hscode',
+    'dsm_django_masterdata.area',
     ...
 ]
 ```
 
 2. migrate database
 ```
 python manage.py migrate
 ```
 
 3. check data in admin page
 
 ## How to use
+- HScode
 ```python
-from dsm_master.hscode.models import HScode
+from dsm_django_masterdata.hscode.models import HScode
 hs_code = HScode.objects.all()
 ```
+- Area
+```python
+from dsm_django_masterdata.area.models import Area
+area = Area.objects.all()
+```
```

### Comparing `dsm_django_masterdata-0.0.2/dsm_django_masterdata.egg-info/SOURCES.txt` & `dsm_django_masterdata-0.0.3/dsm_django_masterdata.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -8,8 +8,9 @@
 dsm_django_masterdata.egg-info/dependency_links.txt
 dsm_django_masterdata.egg-info/requires.txt
 dsm_django_masterdata.egg-info/top_level.txt
 dsm_django_masterdata/hscode/__init__.py
 dsm_django_masterdata/hscode/admin.py
 dsm_django_masterdata/hscode/models.py
 dsm_django_masterdata/hscode/migrations/0001_initial.py
+dsm_django_masterdata/hscode/migrations/0002_alter_hscode_options.py
 dsm_django_masterdata/hscode/migrations/__init__.py
```

### Comparing `dsm_django_masterdata-0.0.2/setup.py` & `dsm_django_masterdata-0.0.3/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 # allow setup.py to be run from any path
 os.chdir(os.path.normpath(os.path.join(os.path.abspath(__file__), os.pardir)))
 
 
 setup(
     name='dsm_django_masterdata',
-    version='0.0.2',
+    version='0.0.3',
     url='https://github.com/storemesh/masterdata/tree/django-app',
     packages=find_packages(),
     include_package_data=True,
     license='MIT License',
     description='A simple way to use Master Data in django project.',
     long_description=README,
     long_description_content_type='text/markdown',
```

