# Comparing `tmp/django_admin_chart-1.0.0.tar.gz` & `tmp/django_admin_chart-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_admin_chart-1.0.0.tar", last modified: Tue Jun 13 05:16:00 2023, max compression
+gzip compressed data, was "django_admin_chart-1.0.1.tar", last modified: Tue Jun 13 08:04:09 2023, max compression
```

## Comparing `django_admin_chart-1.0.0.tar` & `django_admin_chart-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-06-13 05:16:00.221862 django_admin_chart-1.0.0/
--rw-rw-rw-   0        0        0     1082 2023-06-08 09:41:53.000000 django_admin_chart-1.0.0/LICENSE
--rw-rw-rw-   0        0        0      266 2023-06-13 05:16:00.220885 django_admin_chart-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0      111 2023-06-12 02:33:17.000000 django_admin_chart-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2023-06-13 05:16:00.156448 django_admin_chart-1.0.0/django_admin_chart/
--rw-rw-rw-   0        0        0        0 2023-06-08 09:39:31.000000 django_admin_chart-1.0.0/django_admin_chart/__init__.py
--rw-rw-rw-   0        0        0     1120 2023-06-13 02:37:17.000000 django_admin_chart-1.0.0/django_admin_chart/chart.py
--rw-rw-rw-   0        0        0      146 2023-06-07 03:11:51.000000 django_admin_chart-1.0.0/django_admin_chart/chart_base.py
--rw-rw-rw-   0        0        0      595 2023-01-29 03:42:10.000000 django_admin_chart-1.0.0/django_admin_chart/chart_color.py
--rw-rw-rw-   0        0        0     1567 2023-06-13 02:37:17.000000 django_admin_chart-1.0.0/django_admin_chart/chart_render.py
--rw-rw-rw-   0        0        0      350 2023-06-13 05:04:40.000000 django_admin_chart-1.0.0/django_admin_chart/statistics.py
-drwxrwxrwx   0        0        0        0 2023-06-13 05:16:00.137898 django_admin_chart-1.0.0/django_admin_chart/templates/
-drwxrwxrwx   0        0        0        0 2023-06-13 05:16:00.178907 django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/
-drwxrwxrwx   0        0        0        0 2023-06-13 05:16:00.181833 django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/components/
--rw-rw-rw-   0        0        0     2986 2023-01-29 03:42:10.000000 django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/components/chart_statistics.html
--rw-rw-rw-   0        0        0     2911 2023-06-13 02:37:17.000000 django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/duel_bar_chart.html
--rw-rw-rw-   0        0        0     2306 2023-06-13 02:37:17.000000 django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/one_bar_chart.html
--rw-rw-rw-   0        0        0     2960 2023-06-13 02:37:17.000000 django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/one_bar_one_pie_chart.html
-drwxrwxrwx   0        0        0        0 2023-06-13 05:16:00.218933 django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/widgets/
--rw-rw-rw-   0        0        0       79 2023-01-29 03:42:10.000000 django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/widgets/button.html
--rw-rw-rw-   0        0        0       85 2023-01-29 03:42:10.000000 django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/widgets/chart_bar.html
--rw-rw-rw-   0        0        0       85 2023-01-29 03:42:10.000000 django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/widgets/chart_pie.html
--rw-rw-rw-   0        0        0       97 2023-01-29 03:42:10.000000 django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/widgets/select.html
-drwxrwxrwx   0        0        0        0 2023-06-13 05:16:00.173046 django_admin_chart-1.0.0/django_admin_chart.egg-info/
--rw-rw-rw-   0        0        0      266 2023-06-13 05:15:59.000000 django_admin_chart-1.0.0/django_admin_chart.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      998 2023-06-13 05:16:00.000000 django_admin_chart-1.0.0/django_admin_chart.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-13 05:15:59.000000 django_admin_chart-1.0.0/django_admin_chart.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-06-13 05:15:59.000000 django_admin_chart-1.0.0/django_admin_chart.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-06-13 05:15:59.000000 django_admin_chart-1.0.0/django_admin_chart.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-06-13 05:16:00.222839 django_admin_chart-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0      749 2023-06-13 05:14:28.000000 django_admin_chart-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:09.705877 django_admin_chart-1.0.1/
+-rw-rw-rw-   0        0        0     1082 2023-06-08 09:41:53.000000 django_admin_chart-1.0.1/LICENSE
+-rw-rw-rw-   0        0        0      266 2023-06-13 08:04:09.704878 django_admin_chart-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0      111 2023-06-12 02:33:17.000000 django_admin_chart-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:09.644204 django_admin_chart-1.0.1/django_admin_chart/
+-rw-rw-rw-   0        0        0        0 2023-06-08 09:39:31.000000 django_admin_chart-1.0.1/django_admin_chart/__init__.py
+-rw-rw-rw-   0        0        0     1126 2023-06-13 07:09:25.000000 django_admin_chart-1.0.1/django_admin_chart/chart.py
+-rw-rw-rw-   0        0        0      146 2023-06-07 03:11:51.000000 django_admin_chart-1.0.1/django_admin_chart/chart_base.py
+-rw-rw-rw-   0        0        0      595 2023-01-29 03:42:10.000000 django_admin_chart-1.0.1/django_admin_chart/chart_color.py
+-rw-rw-rw-   0        0        0     1567 2023-06-13 02:37:17.000000 django_admin_chart-1.0.1/django_admin_chart/chart_render.py
+-rw-rw-rw-   0        0        0      350 2023-06-13 05:04:40.000000 django_admin_chart-1.0.1/django_admin_chart/statistics.py
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:09.610361 django_admin_chart-1.0.1/django_admin_chart/templates/
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:09.667192 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:09.681892 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/components/
+-rw-rw-rw-   0        0        0     2986 2023-01-29 03:42:10.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/components/chart_statistics.html
+-rw-rw-rw-   0        0        0     2919 2023-06-13 07:02:01.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/duel_bar_chart.html
+-rw-rw-rw-   0        0        0     2314 2023-06-13 07:02:01.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/one_bar_chart.html
+-rw-rw-rw-   0        0        0     2968 2023-06-13 07:02:01.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/one_bar_one_pie_chart.html
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:09.702878 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/widgets/
+-rw-rw-rw-   0        0        0       79 2023-01-29 03:42:10.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/widgets/button.html
+-rw-rw-rw-   0        0        0       85 2023-01-29 03:42:10.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/widgets/chart_bar.html
+-rw-rw-rw-   0        0        0       85 2023-01-29 03:42:10.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/widgets/chart_pie.html
+-rw-rw-rw-   0        0        0       97 2023-01-29 03:42:10.000000 django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/widgets/select.html
+drwxrwxrwx   0        0        0        0 2023-06-13 08:04:09.662194 django_admin_chart-1.0.1/django_admin_chart.egg-info/
+-rw-rw-rw-   0        0        0      266 2023-06-13 08:04:09.000000 django_admin_chart-1.0.1/django_admin_chart.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      998 2023-06-13 08:04:09.000000 django_admin_chart-1.0.1/django_admin_chart.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 08:04:09.000000 django_admin_chart-1.0.1/django_admin_chart.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 08:04:09.000000 django_admin_chart-1.0.1/django_admin_chart.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-06-13 08:04:09.000000 django_admin_chart-1.0.1/django_admin_chart.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 08:04:09.705877 django_admin_chart-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0      749 2023-06-13 07:02:01.000000 django_admin_chart-1.0.1/setup.py
```

### Comparing `django_admin_chart-1.0.0/LICENSE` & `django_admin_chart-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `django_admin_chart-1.0.0/django_admin_chart/chart.py` & `django_admin_chart-1.0.1/django_admin_chart/chart.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,18 +21,18 @@
         extra_context['select_filter'] = self.chart_select_filter
 
         self.change_list_template = self.chart_template
 
         return super().changelist_view(request, extra_context=extra_context)
 
 
-class SingleChartAdmin(ChartAdmin):
+class SingleBarChartAdmin(ChartAdmin):
     chart_template = 'django_admin_chart/one_bar_chart.html'
 
 
-class DuelChartAdmin(ChartAdmin):
+class DuelBarChartAdmin(ChartAdmin):
     chart_template = 'django_admin_chart/duel_bar_chart.html'
 
 
 class BarAndPieChartAdmin(ChartAdmin):
     chart_template = 'django_admin_chart/one_bar_one_pie_chart.html'
     # raise ValueError('Chart filter url not found.')
```

### Comparing `django_admin_chart-1.0.0/django_admin_chart/chart_color.py` & `django_admin_chart-1.0.1/django_admin_chart/chart_color.py`

 * *Files identical despite different names*

### Comparing `django_admin_chart-1.0.0/django_admin_chart/chart_render.py` & `django_admin_chart-1.0.1/django_admin_chart/chart_render.py`

 * *Files identical despite different names*

### Comparing `django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/components/chart_statistics.html` & `django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/components/chart_statistics.html`

 * *Files identical despite different names*

### Comparing `django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/duel_bar_chart.html` & `django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/duel_bar_chart.html`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
         {% if select_filter %}
             jsonResponse.years.forEach(option => {
                 $("#year").append(new Option(option, option));
             });
             const year = $("#year").children().first().val();
             //
             jsonResponse.{{ select_filter|add:"s" }}.forEach(option => {
-                $("#{{ select_filter }}").append(new Option(option, option));
+                $("#{{ select_filter }}").append(new Option(option.name, option.id));
             });
 
             const select = $("#{{ select_filter }}").children().first().val();
             //
             pyChart.loadChart(chart1, chart1EndPoint + `?year=${year}&{{ select_filter }}=${select}`);
             pyChart.loadChart(chart2, chart2EndPoint + `?year=${year}&{{ select_filter }}=${select}`);
         {% else %}
```

### Comparing `django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/one_bar_chart.html` & `django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/one_bar_chart.html`

 * *Files 5% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 
             jsonResponse.years.forEach(option => {
                 $("#year").append(new Option(option, option));
             });
             const year = $("#year").children().first().val();
             //
             jsonResponse.{{ select_filter|add:"s" }}.forEach(option => {
-                $("#{{ select_filter }}").append(new Option(option, option));
+                $("#{{ select_filter }}").append(new Option(option.name, option.id));
             });
 
             const select = $("#{{ select_filter }}").children().first().val();
             //
             pyChart.loadChart(chart, chartEndPoint + `?year=${year}&{{ select_filter }}=${select}`);
 
         {% else %}
```

### Comparing `django_admin_chart-1.0.0/django_admin_chart/templates/django_admin_chart/one_bar_one_pie_chart.html` & `django_admin_chart-1.0.1/django_admin_chart/templates/django_admin_chart/one_bar_one_pie_chart.html`

 * *Files 0% similar despite different names*

```diff
@@ -36,15 +36,15 @@
         {% if select_filter %}
             jsonResponse.years.forEach(option => {
                 $("#year").append(new Option(option, option));
             });
             const year = $("#year").children().first().val();
             //
             jsonResponse.{{ select_filter|add:"s" }}.forEach(option => {
-                $("#{{ select_filter }}").append(new Option(option, option));
+                $("#{{ select_filter }}").append(new Option(option.name, option.id));
             });
 
             const select = $("#{{ select_filter }}").children().first().val();
             //
             pyChart.loadChart(barChart, barChartEndPoint + `?year=${year}&{{ select_filter }}=${select}`);
             pyChart.loadChart(pieChart, pieChartEndPoint + `?year=${year}&{{ select_filter }}=${select}`);
         {% else %}
```

### Comparing `django_admin_chart-1.0.0/django_admin_chart.egg-info/SOURCES.txt` & `django_admin_chart-1.0.1/django_admin_chart.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `django_admin_chart-1.0.0/setup.py` & `django_admin_chart-1.0.1/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='django_admin_chart',
-    version='1.0.0',
+    version='1.0.1',
     description='django admin chart',
     long_description='django admin chart',
     author='ReimiBeta',
     author_email='reimi846@gmail.com',
     url='https://github.com/reimibeta/django_html_render',
     license='MIT',
     packages=find_packages(),
```

