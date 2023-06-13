# Comparing `tmp/django_admin_chart-1.0.1.tar.gz` & `tmp/django_admin_chart-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_admin_chart-1.0.1.tar", last modified: Tue Jun 13 08:04:09 2023, max compression
+gzip compressed data, was "django_admin_chart-1.0.2.tar", last modified: Tue Jun 13 08:08:07 2023, max compression
```

## Comparing `django_admin_chart-1.0.1.tar` & `django_admin_chart-1.0.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:09.705877 django_admin_chart-1.0.1/
--rw-rw-rw-   0        0        0     1082 2023-06-08 09:41:53.000000 django_admin_chart-1.0.1/LICENSE
--rw-rw-rw-   0        0        0      266 2023-06-13 08:04:09.704878 django_admin_chart-1.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      111 2023-06-12 02:33:17.000000 django_admin_chart-1.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:09.644204 django_admin_chart-1.0.1/django_admin_chart/
--rw-rw-rw-   0        0        0        0 2023-06-08 09:39:31.000000 django_admin_chart-1.0.1/django_admin_chart/__init__.py
--rw-rw-rw-   0        0        0     1126 2023-06-13 07:09:25.000000 django_admin_chart-1.0.1/django_admin_chart/chart.py
--rw-rw-rw-   0        0        0      146 2023-06-07 03:11:51.000000 django_admin_chart-1.0.1/django_admin_chart/chart_base.py
--rw-rw-rw-   0        0        0      595 2023-01-29 03:42:10.000000 django_admin_chart-1.0.1/django_admin_chart/chart_color.py
--rw-rw-rw-   0        0        0     1567 2023-06-13 02:37:17.000000 django_admin_chart-1.0.1/django_admin_chart/chart_render.py
--rw-rw-rw-   0        0        0      350 2023-06-13 05:04:40.000000 django_admin_chart-1.0.1/django_admin_chart/statistics.py
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:09.610361 django_admin_chart-1.0.1/django_admin_chart/templates/
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:09.667192 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:09.681892 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/components/
--rw-rw-rw-   0        0        0     2986 2023-01-29 03:42:10.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/components/chart_statistics.html
--rw-rw-rw-   0        0        0     2919 2023-06-13 07:02:01.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/duel_bar_chart.html
--rw-rw-rw-   0        0        0     2314 2023-06-13 07:02:01.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/one_bar_chart.html
--rw-rw-rw-   0        0        0     2968 2023-06-13 07:02:01.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/one_bar_one_pie_chart.html
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:09.702878 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/widgets/
--rw-rw-rw-   0        0        0       79 2023-01-29 03:42:10.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/widgets/button.html
--rw-rw-rw-   0        0        0       85 2023-01-29 03:42:10.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/widgets/chart_bar.html
--rw-rw-rw-   0        0        0       85 2023-01-29 03:42:10.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/widgets/chart_pie.html
--rw-rw-rw-   0        0        0       97 2023-01-29 03:42:10.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/widgets/select.html
-drwxrwxrwx   0        0        0        0 2023-06-13 08:04:09.662194 django_admin_chart-1.0.1/django_admin_chart.egg-info/
--rw-rw-rw-   0        0        0      266 2023-06-13 08:04:09.000000 django_admin_chart-1.0.1/django_admin_chart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      998 2023-06-13 08:04:09.000000 django_admin_chart-1.0.1/django_admin_chart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 08:04:09.000000 django_admin_chart-1.0.1/django_admin_chart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-13 08:04:09.000000 django_admin_chart-1.0.1/django_admin_chart.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-13 08:04:09.000000 django_admin_chart-1.0.1/django_admin_chart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 08:04:09.705877 django_admin_chart-1.0.1/setup.cfg
--rw-rw-rw-   0        0        0      749 2023-06-13 07:02:01.000000 django_admin_chart-1.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:08:07.759128 django_admin_chart-1.0.2/
+-rw-rw-rw-   0        0        0     1082 2023-06-08 09:41:53.000000 django_admin_chart-1.0.2/LICENSE
+-rw-rw-rw-   0        0        0      266 2023-06-13 08:08:07.758129 django_admin_chart-1.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      111 2023-06-12 02:33:17.000000 django_admin_chart-1.0.2/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 08:08:07.722133 django_admin_chart-1.0.2/django_admin_chart/
+-rw-rw-rw-   0        0        0        0 2023-06-08 09:39:31.000000 django_admin_chart-1.0.2/django_admin_chart/__init__.py
+-rw-rw-rw-   0        0        0     1126 2023-06-13 07:09:25.000000 django_admin_chart-1.0.2/django_admin_chart/chart.py
+-rw-rw-rw-   0        0        0      146 2023-06-07 03:11:51.000000 django_admin_chart-1.0.2/django_admin_chart/chart_base.py
+-rw-rw-rw-   0        0        0      595 2023-01-29 03:42:10.000000 django_admin_chart-1.0.2/django_admin_chart/chart_color.py
+-rw-rw-rw-   0        0        0     1567 2023-06-13 02:37:17.000000 django_admin_chart-1.0.2/django_admin_chart/chart_render.py
+-rw-rw-rw-   0        0        0      350 2023-06-13 05:04:40.000000 django_admin_chart-1.0.2/django_admin_chart/statistics.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:08:07.706661 django_admin_chart-1.0.2/django_admin_chart/templates/
+drwxrwxrwx   0        0        0        0 2023-06-13 08:08:07.750120 django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/
+drwxrwxrwx   0        0        0        0 2023-06-13 08:08:07.751119 django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/components/
+-rw-rw-rw-   0        0        0     2986 2023-01-29 03:42:10.000000 django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/components/chart_statistics.html
+-rw-rw-rw-   0        0        0     2919 2023-06-13 07:02:01.000000 django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/duel_bar_chart.html
+-rw-rw-rw-   0        0        0     2314 2023-06-13 07:02:01.000000 django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/one_bar_chart.html
+-rw-rw-rw-   0        0        0     2968 2023-06-13 07:02:01.000000 django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/one_bar_one_pie_chart.html
+drwxrwxrwx   0        0        0        0 2023-06-13 08:08:07.757133 django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/widgets/
+-rw-rw-rw-   0        0        0       79 2023-01-29 03:42:10.000000 django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/widgets/button.html
+-rw-rw-rw-   0        0        0       85 2023-01-29 03:42:10.000000 django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/widgets/chart_bar.html
+-rw-rw-rw-   0        0        0       85 2023-01-29 03:42:10.000000 django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/widgets/chart_pie.html
+-rw-rw-rw-   0        0        0       97 2023-01-29 03:42:10.000000 django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/widgets/select.html
+drwxrwxrwx   0        0        0        0 2023-06-13 08:08:07.744122 django_admin_chart-1.0.2/django_admin_chart.egg-info/
+-rw-rw-rw-   0        0        0      266 2023-06-13 08:08:07.000000 django_admin_chart-1.0.2/django_admin_chart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      998 2023-06-13 08:08:07.000000 django_admin_chart-1.0.2/django_admin_chart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 08:08:07.000000 django_admin_chart-1.0.2/django_admin_chart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 08:08:07.000000 django_admin_chart-1.0.2/django_admin_chart.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-13 08:08:07.000000 django_admin_chart-1.0.2/django_admin_chart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 08:08:07.760112 django_admin_chart-1.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-06-13 08:07:58.000000 django_admin_chart-1.0.2/setup.py
```

### Comparing `django_admin_chart-1.0.1/LICENSE` & `django_admin_chart-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `django_admin_chart-1.0.1/django_admin_chart/chart.py` & `django_admin_chart-1.0.2/django_admin_chart/chart.py`

 * *Files identical despite different names*

### Comparing `django_admin_chart-1.0.1/django_admin_chart/chart_color.py` & `django_admin_chart-1.0.2/django_admin_chart/chart_color.py`

 * *Files identical despite different names*

### Comparing `django_admin_chart-1.0.1/django_admin_chart/chart_render.py` & `django_admin_chart-1.0.2/django_admin_chart/chart_render.py`

 * *Files identical despite different names*

### Comparing `django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/components/chart_statistics.html` & `django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/components/chart_statistics.html`

 * *Files identical despite different names*

### Comparing `django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/duel_bar_chart.html` & `django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/duel_bar_chart.html`

 * *Files identical despite different names*

### Comparing `django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/one_bar_chart.html` & `django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/one_bar_chart.html`

 * *Files identical despite different names*

### Comparing `django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/one_bar_one_pie_chart.html` & `django_admin_chart-1.0.2/django_admin_chart/templates/django_admin_chart/one_bar_one_pie_chart.html`

 * *Files identical despite different names*

### Comparing `django_admin_chart-1.0.1/django_admin_chart.egg-info/SOURCES.txt` & `django_admin_chart-1.0.2/django_admin_chart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_admin_chart-1.0.1/setup.py` & `django_admin_chart-1.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django_admin_chart',
-    version='1.0.1',
+    version='1.0.2',
     description='django admin chart',
     long_description='django admin chart',
     author='ReimiBeta',
     author_email='reimi846@gmail.com',
-    url='https://github.com/reimibeta/django_html_render',
+    url='https://github.com/reimibeta/django_admin_chart',
     license='MIT',
     packages=find_packages(),
     # py_modules=['image_compress',],
     install_requires=[
         # other dependencies
         'Django==4.1.7'
     ],
```

