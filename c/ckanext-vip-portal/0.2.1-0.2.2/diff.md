# Comparing `tmp/ckanext-vip-portal-0.2.1.tar.gz` & `tmp/ckanext-vip-portal-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext-vip-portal-0.2.1.tar", last modified: Fri Mar  3 00:14:55 2023, max compression
+gzip compressed data, was "ckanext-vip-portal-0.2.2.tar", last modified: Tue Jun 13 11:37:47 2023, max compression
```

## Comparing `ckanext-vip-portal-0.2.1.tar` & `ckanext-vip-portal-0.2.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:14:55.110103 ckanext-vip-portal-0.2.1/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.1/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      212 2023-03-03 00:11:02.000000 ckanext-vip-portal-0.2.1/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3683 2023-03-03 00:14:55.110103 ckanext-vip-portal-0.2.1/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3035 2023-03-02 17:30:47.000000 ckanext-vip-portal-0.2.1/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:14:55.110103 ckanext-vip-portal-0.2.1/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-24 14:50:12.000000 ckanext-vip-portal-0.2.1/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:14:55.110103 ckanext-vip-portal-0.2.1/ckanext/vip_portal/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.1/ckanext/vip_portal/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:14:55.110103 ckanext-vip-portal-0.2.1/ckanext/vip_portal/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      162 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.1/ckanext/vip_portal/assets/script.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.1/ckanext/vip_portal/assets/style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      319 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.1/ckanext/vip_portal/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3319 2023-02-15 12:23:34.000000 ckanext-vip-portal-0.2.1/ckanext/vip_portal/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2332 2023-03-02 17:29:51.000000 ckanext-vip-portal-0.2.1/ckanext/vip_portal/config_declaration.yaml
--rw-r--r--   0 sergey    (1000) sergey    (1000)      850 2023-02-15 12:23:34.000000 ckanext-vip-portal-0.2.1/ckanext/vip_portal/interfaces.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3695 2023-03-02 17:24:19.000000 ckanext-vip-portal-0.2.1/ckanext/vip_portal/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:14:55.110103 ckanext-vip-portal-0.2.1/ckanext/vip_portal/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.1/ckanext/vip_portal/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2022-10-24 17:18:21.000000 ckanext-vip-portal-0.2.1/ckanext/vip_portal/tests/test_plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      958 2023-02-15 12:23:34.000000 ckanext-vip-portal-0.2.1/ckanext/vip_portal/utils.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-03-03 00:14:55.110103 ckanext-vip-portal-0.2.1/ckanext_vip_portal.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3683 2023-03-03 00:14:55.000000 ckanext-vip-portal-0.2.1/ckanext_vip_portal.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)      770 2023-03-03 00:14:55.000000 ckanext-vip-portal-0.2.1/ckanext_vip_portal.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-03-03 00:14:55.000000 ckanext-vip-portal-0.2.1/ckanext_vip_portal.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      127 2023-03-03 00:14:55.000000 ckanext-vip-portal-0.2.1/ckanext_vip_portal.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-03-03 00:14:55.000000 ckanext-vip-portal-0.2.1/ckanext_vip_portal.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)       19 2023-03-03 00:14:55.000000 ckanext-vip-portal-0.2.1/ckanext_vip_portal.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-03-03 00:14:55.000000 ckanext-vip-portal-0.2.1/ckanext_vip_portal.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2927 2023-03-02 17:22:47.000000 ckanext-vip-portal-0.2.1/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1665 2023-03-03 00:14:55.110103 ckanext-vip-portal-0.2.1/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-10-24 14:50:12.000000 ckanext-vip-portal-0.2.1/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-13 11:37:47.685117 ckanext-vip-portal-0.2.2/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34500 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.2/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      212 2023-03-03 00:11:02.000000 ckanext-vip-portal-0.2.2/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3683 2023-06-13 11:37:47.685117 ckanext-vip-portal-0.2.2/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3035 2023-03-02 17:30:47.000000 ckanext-vip-portal-0.2.2/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-13 11:37:47.675117 ckanext-vip-portal-0.2.2/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2022-10-24 14:50:12.000000 ckanext-vip-portal-0.2.2/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-13 11:37:47.675117 ckanext-vip-portal-0.2.2/ckanext/vip_portal/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.2/ckanext/vip_portal/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-13 11:37:47.685117 ckanext-vip-portal-0.2.2/ckanext/vip_portal/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      162 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.2/ckanext/vip_portal/assets/script.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       35 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.2/ckanext/vip_portal/assets/style.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      319 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.2/ckanext/vip_portal/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3350 2023-06-13 11:36:51.000000 ckanext-vip-portal-0.2.2/ckanext/vip_portal/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2332 2023-03-02 17:29:51.000000 ckanext-vip-portal-0.2.2/ckanext/vip_portal/config_declaration.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      850 2023-02-15 12:23:34.000000 ckanext-vip-portal-0.2.2/ckanext/vip_portal/interfaces.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3695 2023-05-21 19:59:13.000000 ckanext-vip-portal-0.2.2/ckanext/vip_portal/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-13 11:37:47.685117 ckanext-vip-portal-0.2.2/ckanext/vip_portal/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2022-10-24 14:00:22.000000 ckanext-vip-portal-0.2.2/ckanext/vip_portal/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      142 2022-10-24 17:18:21.000000 ckanext-vip-portal-0.2.2/ckanext/vip_portal/tests/test_plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      958 2023-02-15 12:23:34.000000 ckanext-vip-portal-0.2.2/ckanext/vip_portal/utils.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2023-06-13 11:37:47.685117 ckanext-vip-portal-0.2.2/ckanext_vip_portal.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3683 2023-06-13 11:37:47.000000 ckanext-vip-portal-0.2.2/ckanext_vip_portal.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      770 2023-06-13 11:37:47.000000 ckanext-vip-portal-0.2.2/ckanext_vip_portal.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2023-06-13 11:37:47.000000 ckanext-vip-portal-0.2.2/ckanext_vip_portal.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      127 2023-06-13 11:37:47.000000 ckanext-vip-portal-0.2.2/ckanext_vip_portal.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-13 11:37:47.000000 ckanext-vip-portal-0.2.2/ckanext_vip_portal.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       19 2023-06-13 11:37:47.000000 ckanext-vip-portal-0.2.2/ckanext_vip_portal.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2023-06-13 11:37:47.000000 ckanext-vip-portal-0.2.2/ckanext_vip_portal.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2927 2023-03-02 17:22:47.000000 ckanext-vip-portal-0.2.2/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1665 2023-06-13 11:37:47.685117 ckanext-vip-portal-0.2.2/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      528 2022-10-24 14:50:12.000000 ckanext-vip-portal-0.2.2/setup.py
```

### Comparing `ckanext-vip-portal-0.2.1/LICENSE` & `ckanext-vip-portal-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.1/PKG-INFO` & `ckanext-vip-portal-0.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-vip-portal
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/DataShades/ckanext-vip-portal
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-vip-portal-0.2.1/README.md` & `ckanext-vip-portal-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.1/ckanext/vip_portal/config.py` & `ckanext-vip-portal-0.2.2/ckanext/vip_portal/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,14 +49,15 @@
     ("user", "logged_out"),
     ("user", "logged_out_page"),
     ("user", "logged_out_redirect"),
 ]
 
 password_reset_endpoints = [
     ("user", "request_reset"),
+    ("user", "perform_reset"),
 ]
 
 register_endpoints = [
     ("user", "register"),
 ]
 
 api_endpoints = [
```

### Comparing `ckanext-vip-portal-0.2.1/ckanext/vip_portal/config_declaration.yaml` & `ckanext-vip-portal-0.2.2/ckanext/vip_portal/config_declaration.yaml`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.1/ckanext/vip_portal/interfaces.py` & `ckanext-vip-portal-0.2.2/ckanext/vip_portal/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.1/ckanext/vip_portal/plugin.py` & `ckanext-vip-portal-0.2.2/ckanext/vip_portal/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.1/ckanext/vip_portal/utils.py` & `ckanext-vip-portal-0.2.2/ckanext/vip_portal/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.1/ckanext_vip_portal.egg-info/PKG-INFO` & `ckanext-vip-portal-0.2.2/ckanext_vip_portal.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-vip-portal
-Version: 0.2.1
+Version: 0.2.2
 Home-page: https://github.com/DataShades/ckanext-vip-portal
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext-vip-portal-0.2.1/ckanext_vip_portal.egg-info/SOURCES.txt` & `ckanext-vip-portal-0.2.2/ckanext_vip_portal.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.1/pyproject.toml` & `ckanext-vip-portal-0.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext-vip-portal-0.2.1/setup.cfg` & `ckanext-vip-portal-0.2.2/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-vip-portal
-version = 0.2.1
+version = 0.2.2
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-vip-portal
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

### Comparing `ckanext-vip-portal-0.2.1/setup.py` & `ckanext-vip-portal-0.2.2/setup.py`

 * *Files identical despite different names*

