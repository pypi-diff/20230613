# Comparing `tmp/cmem_cmempy-23.1.tar.gz` & `tmp/cmem_cmempy-23.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cmem_cmempy-23.1.tar", max compression
+gzip compressed data, was "cmem_cmempy-23.1.1.tar", max compression
```

## Comparing `cmem_cmempy-23.1.tar` & `cmem_cmempy-23.1.1.tar`

### file list

```diff
@@ -1,55 +1,55 @@
--rw-r--r--   0        0        0    11357 2023-01-18 07:28:45.599930 cmem_cmempy-23.1/LICENSE
--rw-r--r--   0        0        0      651 2023-04-24 07:06:13.952436 cmem_cmempy-23.1/README-public.md
--rw-r--r--   0        0        0      110 2023-04-24 07:06:13.952744 cmem_cmempy-23.1/cmem/__init__.py
--rw-r--r--   0        0        0       40 2023-04-24 07:06:13.952818 cmem_cmempy-23.1/cmem/cmempy/__init__.py
--rw-r--r--   0        0        0     4456 2023-04-24 07:06:13.953043 cmem_cmempy-23.1/cmem/cmempy/api.py
--rw-r--r--   0        0        0     4970 2023-04-24 07:06:13.953161 cmem_cmempy-23.1/cmem/cmempy/config.py
--rw-r--r--   0        0        0     1062 2023-04-24 07:06:13.953244 cmem_cmempy-23.1/cmem/cmempy/custom_tasks/__init__.py
--rw-r--r--   0        0        0       36 2023-04-24 07:06:13.953307 cmem_cmempy-23.1/cmem/cmempy/dp/__init__.py
--rw-r--r--   0        0        0     1029 2023-04-24 07:06:13.953384 cmem_cmempy-23.1/cmem/cmempy/dp/admin/__init__.py
--rw-r--r--   0        0        0     1014 2023-04-24 07:06:13.953446 cmem_cmempy-23.1/cmem/cmempy/dp/admin/backup.py
--rw-r--r--   0        0        0       42 2023-04-24 07:06:13.953524 cmem_cmempy-23.1/cmem/cmempy/dp/authorization/__init__.py
--rw-r--r--   0        0        0     1232 2023-04-24 07:06:13.953586 cmem_cmempy-23.1/cmem/cmempy/dp/authorization/conditions.py
--rw-r--r--   0        0        0      477 2023-04-24 07:06:13.953641 cmem_cmempy-23.1/cmem/cmempy/dp/authorization/refresh.py
--rw-r--r--   0        0        0      380 2023-04-24 07:06:13.953720 cmem_cmempy-23.1/cmem/cmempy/dp/proxy/__init__.py
--rw-r--r--   0        0        0     6036 2023-04-24 07:06:13.953793 cmem_cmempy-23.1/cmem/cmempy/dp/proxy/graph.py
--rw-r--r--   0        0        0     4159 2023-04-24 07:06:13.953863 cmem_cmempy-23.1/cmem/cmempy/dp/proxy/sparql.py
--rw-r--r--   0        0        0     1244 2023-04-24 07:06:13.953918 cmem_cmempy-23.1/cmem/cmempy/dp/proxy/update.py
--rw-r--r--   0        0        0     1011 2023-04-24 07:06:13.954002 cmem_cmempy-23.1/cmem/cmempy/dp/titles/__init__.py
--rw-r--r--   0        0        0     5905 2023-04-24 07:06:13.954105 cmem_cmempy-23.1/cmem/cmempy/health/__init__.py
--rw-r--r--   0        0        0      519 2023-04-24 07:06:13.954373 cmem_cmempy-23.1/cmem/cmempy/keycloak/group.py
--rw-r--r--   0        0        0     3630 2023-04-24 07:06:13.954464 cmem_cmempy-23.1/cmem/cmempy/keycloak/user.py
--rw-r--r--   0        0        0       31 2023-04-24 07:06:13.954530 cmem_cmempy-23.1/cmem/cmempy/linking/__init__.py
--rw-r--r--   0        0        0     2588 2023-04-24 07:06:13.954585 cmem_cmempy-23.1/cmem/cmempy/linking/linkingtask.py
--rw-r--r--   0        0        0       26 2023-04-24 07:06:13.954658 cmem_cmempy-23.1/cmem/cmempy/plugins/__init__.py
--rw-r--r--   0        0        0     1939 2023-04-24 07:06:13.954716 cmem_cmempy-23.1/cmem/cmempy/plugins/marshalling.py
--rw-r--r--   0        0        0    11190 2023-04-24 07:06:13.955001 cmem_cmempy-23.1/cmem/cmempy/queries/__init__.py
--rw-r--r--   0        0        0       33 2023-04-24 07:06:13.955070 cmem_cmempy-23.1/cmem/cmempy/transform/__init__.py
--rw-r--r--   0        0        0     1090 2023-04-24 07:06:13.955142 cmem_cmempy-23.1/cmem/cmempy/transform/rules/__init__.py
--rw-r--r--   0        0        0     1075 2023-04-24 07:06:13.955192 cmem_cmempy-23.1/cmem/cmempy/transform/rules/transformationrule.py
--rw-r--r--   0        0        0     1240 2023-04-24 07:06:13.955247 cmem_cmempy-23.1/cmem/cmempy/transform/transformationtask.py
--rw-r--r--   0        0        0     3597 2023-04-24 07:06:13.955338 cmem_cmempy-23.1/cmem/cmempy/vocabularies/__init__.py
--rw-r--r--   0        0        0      500 2023-04-24 07:06:13.955412 cmem_cmempy-23.1/cmem/cmempy/workflow/__init__.py
--rw-r--r--   0        0        0     4502 2023-04-24 07:06:13.955473 cmem_cmempy-23.1/cmem/cmempy/workflow/workflow.py
--rw-r--r--   0        0        0      131 2023-04-24 07:06:13.955517 cmem_cmempy-23.1/cmem/cmempy/workflow/workflows.py
--rw-r--r--   0        0        0     1873 2023-04-24 07:06:13.955597 cmem_cmempy-23.1/cmem/cmempy/workspace/__init__.py
--rw-r--r--   0        0        0      340 2023-04-24 07:06:13.955666 cmem_cmempy-23.1/cmem/cmempy/workspace/activities/__init__.py
--rw-r--r--   0        0        0      914 2023-04-24 07:06:13.955719 cmem_cmempy-23.1/cmem/cmempy/workspace/activities/projectactivities.py
--rw-r--r--   0        0        0     2281 2023-04-24 07:06:13.955774 cmem_cmempy-23.1/cmem/cmempy/workspace/activities/projectactivity.py
--rw-r--r--   0        0        0     3164 2023-04-24 07:06:13.955836 cmem_cmempy-23.1/cmem/cmempy/workspace/activities/taskactivities.py
--rw-r--r--   0        0        0     2323 2023-04-24 07:06:13.955884 cmem_cmempy-23.1/cmem/cmempy/workspace/activities/taskactivity.py
--rw-r--r--   0        0        0      744 2023-04-24 07:06:13.955973 cmem_cmempy-23.1/cmem/cmempy/workspace/export_/__init__.py
--rw-r--r--   0        0        0     1540 2023-04-24 07:06:13.956048 cmem_cmempy-23.1/cmem/cmempy/workspace/import_/__init__.py
--rw-r--r--   0        0        0      454 2023-04-24 07:06:13.956113 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/__init__.py
--rw-r--r--   0        0        0       45 2023-04-24 07:06:13.956183 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/datasets/__init__.py
--rw-r--r--   0        0        0     2369 2023-04-24 07:06:13.956242 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/datasets/dataset.py
--rw-r--r--   0        0        0      748 2023-04-24 07:06:13.956330 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/export_.py
--rw-r--r--   0        0        0     4945 2023-04-24 07:06:13.956394 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/import_.py
--rw-r--r--   0        0        0     2007 2023-04-24 07:06:13.956449 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/project.py
--rw-r--r--   0        0        0      960 2023-04-24 07:06:13.956713 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/resources/__init__.py
--rw-r--r--   0        0        0     6089 2023-04-24 07:06:13.956822 cmem_cmempy-23.1/cmem/cmempy/workspace/projects/resources/resource.py
--rw-r--r--   0        0        0     2292 2023-04-24 07:06:13.956887 cmem_cmempy-23.1/cmem/cmempy/workspace/python.py
--rw-r--r--   0        0        0     1075 2023-04-24 07:06:13.956970 cmem_cmempy-23.1/cmem/cmempy/workspace/search/__init__.py
--rw-r--r--   0        0        0     1078 2023-04-24 07:06:13.957053 cmem_cmempy-23.1/cmem/cmempy/workspace/tasks/__init__.py
--rw-r--r--   0        0        0     2048 2023-04-24 11:55:27.286209 cmem_cmempy-23.1/pyproject.toml
--rw-r--r--   0        0        0     2005 1970-01-01 00:00:00.000000 cmem_cmempy-23.1/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-01-04 14:59:14.088341 cmem_cmempy-23.1.1/LICENSE
+-rw-r--r--   0        0        0      651 2023-06-13 18:26:21.198608 cmem_cmempy-23.1.1/README-public.md
+-rw-r--r--   0        0        0      110 2023-01-04 14:59:14.088607 cmem_cmempy-23.1.1/cmem/__init__.py
+-rw-r--r--   0        0        0       40 2023-01-04 14:59:14.088681 cmem_cmempy-23.1.1/cmem/cmempy/__init__.py
+-rw-r--r--   0        0        0     4456 2023-04-27 06:10:06.372985 cmem_cmempy-23.1.1/cmem/cmempy/api.py
+-rw-r--r--   0        0        0     4970 2023-04-27 06:10:06.373356 cmem_cmempy-23.1.1/cmem/cmempy/config.py
+-rw-r--r--   0        0        0     1062 2023-01-04 14:59:14.088909 cmem_cmempy-23.1.1/cmem/cmempy/custom_tasks/__init__.py
+-rw-r--r--   0        0        0       36 2023-01-04 14:59:14.088982 cmem_cmempy-23.1.1/cmem/cmempy/dp/__init__.py
+-rw-r--r--   0        0        0     1029 2023-01-04 14:59:14.089065 cmem_cmempy-23.1.1/cmem/cmempy/dp/admin/__init__.py
+-rw-r--r--   0        0        0     1014 2023-01-04 14:59:14.089117 cmem_cmempy-23.1.1/cmem/cmempy/dp/admin/backup.py
+-rw-r--r--   0        0        0       42 2023-01-04 14:59:14.089196 cmem_cmempy-23.1.1/cmem/cmempy/dp/authorization/__init__.py
+-rw-r--r--   0        0        0     1232 2023-01-04 14:59:14.089259 cmem_cmempy-23.1.1/cmem/cmempy/dp/authorization/conditions.py
+-rw-r--r--   0        0        0      477 2023-01-04 14:59:14.089322 cmem_cmempy-23.1.1/cmem/cmempy/dp/authorization/refresh.py
+-rw-r--r--   0        0        0      380 2023-01-04 14:59:14.089401 cmem_cmempy-23.1.1/cmem/cmempy/dp/proxy/__init__.py
+-rw-r--r--   0        0        0     6036 2023-01-04 14:59:14.089475 cmem_cmempy-23.1.1/cmem/cmempy/dp/proxy/graph.py
+-rw-r--r--   0        0        0     4159 2023-01-04 14:59:14.089530 cmem_cmempy-23.1.1/cmem/cmempy/dp/proxy/sparql.py
+-rw-r--r--   0        0        0     1244 2023-01-04 14:59:14.089583 cmem_cmempy-23.1.1/cmem/cmempy/dp/proxy/update.py
+-rw-r--r--   0        0        0     1011 2023-01-04 14:59:14.089671 cmem_cmempy-23.1.1/cmem/cmempy/dp/titles/__init__.py
+-rw-r--r--   0        0        0     5905 2023-01-04 14:59:14.089779 cmem_cmempy-23.1.1/cmem/cmempy/health/__init__.py
+-rw-r--r--   0        0        0      519 2023-04-27 06:10:06.373437 cmem_cmempy-23.1.1/cmem/cmempy/keycloak/group.py
+-rw-r--r--   0        0        0     3630 2023-06-13 18:49:23.475724 cmem_cmempy-23.1.1/cmem/cmempy/keycloak/user.py
+-rw-r--r--   0        0        0       31 2023-01-04 14:59:14.089861 cmem_cmempy-23.1.1/cmem/cmempy/linking/__init__.py
+-rw-r--r--   0        0        0     2588 2023-01-04 14:59:14.089928 cmem_cmempy-23.1.1/cmem/cmempy/linking/linkingtask.py
+-rw-r--r--   0        0        0       26 2023-01-04 14:59:14.090002 cmem_cmempy-23.1.1/cmem/cmempy/plugins/__init__.py
+-rw-r--r--   0        0        0     1939 2023-01-04 14:59:14.090063 cmem_cmempy-23.1.1/cmem/cmempy/plugins/marshalling.py
+-rw-r--r--   0        0        0    11190 2023-04-27 06:10:06.373634 cmem_cmempy-23.1.1/cmem/cmempy/queries/__init__.py
+-rw-r--r--   0        0        0       33 2023-01-04 14:59:14.090285 cmem_cmempy-23.1.1/cmem/cmempy/transform/__init__.py
+-rw-r--r--   0        0        0     1090 2023-01-04 14:59:14.090388 cmem_cmempy-23.1.1/cmem/cmempy/transform/rules/__init__.py
+-rw-r--r--   0        0        0     1075 2023-01-04 14:59:14.090439 cmem_cmempy-23.1.1/cmem/cmempy/transform/rules/transformationrule.py
+-rw-r--r--   0        0        0     1240 2023-01-04 14:59:14.090495 cmem_cmempy-23.1.1/cmem/cmempy/transform/transformationtask.py
+-rw-r--r--   0        0        0     3597 2023-01-05 19:05:10.883204 cmem_cmempy-23.1.1/cmem/cmempy/vocabularies/__init__.py
+-rw-r--r--   0        0        0      500 2023-01-04 14:59:14.090681 cmem_cmempy-23.1.1/cmem/cmempy/workflow/__init__.py
+-rw-r--r--   0        0        0     4502 2023-01-04 14:59:14.090748 cmem_cmempy-23.1.1/cmem/cmempy/workflow/workflow.py
+-rw-r--r--   0        0        0      131 2023-01-04 14:59:14.090794 cmem_cmempy-23.1.1/cmem/cmempy/workflow/workflows.py
+-rw-r--r--   0        0        0     1873 2023-01-04 14:59:14.090883 cmem_cmempy-23.1.1/cmem/cmempy/workspace/__init__.py
+-rw-r--r--   0        0        0      340 2023-01-04 14:59:14.090960 cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/__init__.py
+-rw-r--r--   0        0        0      914 2023-01-04 14:59:14.091021 cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/projectactivities.py
+-rw-r--r--   0        0        0     2281 2023-01-04 14:59:14.091080 cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/projectactivity.py
+-rw-r--r--   0        0        0     3164 2023-01-04 14:59:14.091146 cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/taskactivities.py
+-rw-r--r--   0        0        0     2323 2023-01-04 14:59:14.091194 cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/taskactivity.py
+-rw-r--r--   0        0        0      744 2023-01-04 14:59:14.091271 cmem_cmempy-23.1.1/cmem/cmempy/workspace/export_/__init__.py
+-rw-r--r--   0        0        0     1540 2023-01-04 14:59:14.091352 cmem_cmempy-23.1.1/cmem/cmempy/workspace/import_/__init__.py
+-rw-r--r--   0        0        0      454 2023-01-04 14:59:14.091425 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/__init__.py
+-rw-r--r--   0        0        0       45 2023-01-04 14:59:14.091506 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/datasets/__init__.py
+-rw-r--r--   0        0        0     2369 2023-01-04 14:59:14.091570 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/datasets/dataset.py
+-rw-r--r--   0        0        0      748 2023-01-04 14:59:14.091621 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/export_.py
+-rw-r--r--   0        0        0     4945 2023-01-04 14:59:14.091685 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/import_.py
+-rw-r--r--   0        0        0     2007 2023-01-04 14:59:14.091735 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/project.py
+-rw-r--r--   0        0        0      960 2023-04-27 06:10:06.373750 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/resources/__init__.py
+-rw-r--r--   0        0        0     6089 2023-04-27 06:10:06.373861 cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/resources/resource.py
+-rw-r--r--   0        0        0     2292 2023-01-04 14:59:14.091934 cmem_cmempy-23.1.1/cmem/cmempy/workspace/python.py
+-rw-r--r--   0        0        0     1075 2023-01-04 14:59:14.092020 cmem_cmempy-23.1.1/cmem/cmempy/workspace/search/__init__.py
+-rw-r--r--   0        0        0     1078 2023-01-04 14:59:14.092095 cmem_cmempy-23.1.1/cmem/cmempy/workspace/tasks/__init__.py
+-rw-r--r--   0        0        0     2042 2023-06-13 18:49:40.640308 cmem_cmempy-23.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1938 1970-01-01 00:00:00.000000 cmem_cmempy-23.1.1/PKG-INFO
```

### Comparing `cmem_cmempy-23.1/LICENSE` & `cmem_cmempy-23.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/README-public.md` & `cmem_cmempy-23.1.1/README-public.md`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/api.py` & `cmem_cmempy-23.1.1/cmem/cmempy/api.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/config.py` & `cmem_cmempy-23.1.1/cmem/cmempy/config.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/custom_tasks/__init__.py` & `cmem_cmempy-23.1.1/cmem/cmempy/custom_tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/dp/admin/__init__.py` & `cmem_cmempy-23.1.1/cmem/cmempy/dp/admin/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/dp/admin/backup.py` & `cmem_cmempy-23.1.1/cmem/cmempy/dp/admin/backup.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/dp/authorization/conditions.py` & `cmem_cmempy-23.1.1/cmem/cmempy/dp/authorization/conditions.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/dp/proxy/graph.py` & `cmem_cmempy-23.1.1/cmem/cmempy/dp/proxy/graph.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/dp/proxy/sparql.py` & `cmem_cmempy-23.1.1/cmem/cmempy/dp/proxy/sparql.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/dp/proxy/update.py` & `cmem_cmempy-23.1.1/cmem/cmempy/dp/proxy/update.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/dp/titles/__init__.py` & `cmem_cmempy-23.1.1/cmem/cmempy/dp/titles/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/health/__init__.py` & `cmem_cmempy-23.1.1/cmem/cmempy/health/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/keycloak/group.py` & `cmem_cmempy-23.1.1/cmem/cmempy/keycloak/group.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/keycloak/user.py` & `cmem_cmempy-23.1.1/cmem/cmempy/keycloak/user.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/linking/linkingtask.py` & `cmem_cmempy-23.1.1/cmem/cmempy/linking/linkingtask.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/plugins/marshalling.py` & `cmem_cmempy-23.1.1/cmem/cmempy/plugins/marshalling.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/queries/__init__.py` & `cmem_cmempy-23.1.1/cmem/cmempy/queries/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/transform/rules/__init__.py` & `cmem_cmempy-23.1.1/cmem/cmempy/transform/rules/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/transform/rules/transformationrule.py` & `cmem_cmempy-23.1.1/cmem/cmempy/transform/rules/transformationrule.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/transform/transformationtask.py` & `cmem_cmempy-23.1.1/cmem/cmempy/transform/transformationtask.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/vocabularies/__init__.py` & `cmem_cmempy-23.1.1/cmem/cmempy/vocabularies/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workflow/workflow.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workflow/workflow.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/__init__.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/activities/projectactivities.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/projectactivities.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/activities/projectactivity.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/projectactivity.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/activities/taskactivities.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/taskactivities.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/activities/taskactivity.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/activities/taskactivity.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/export_/__init__.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/export_/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/import_/__init__.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/import_/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/projects/datasets/dataset.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/projects/export_.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/export_.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/projects/import_.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/import_.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/projects/project.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/project.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/projects/resources/__init__.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/projects/resources/resource.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/projects/resources/resource.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/python.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/python.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/search/__init__.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/search/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/cmem/cmempy/workspace/tasks/__init__.py` & `cmem_cmempy-23.1.1/cmem/cmempy/workspace/tasks/__init__.py`

 * *Files identical despite different names*

### Comparing `cmem_cmempy-23.1/pyproject.toml` & `cmem_cmempy-23.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.poetry]
 name = "cmem-cmempy"
-version = "23.1"
+version = "23.1.1"
 license = "Apache-2.0"
-description = "API wrapper for eccenca Corporate Memory"
+description = "API for eccenca Corporate Memory"
 authors = ["eccenca GmbH <cmempy-developer@eccenca.com>"]
 maintainers = ["Sebastian Tramp <sebastian.tramp@eccenca.com>"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "Intended Audience :: Science/Research",
     "Intended Audience :: System Administrators",
@@ -21,19 +21,19 @@
 readme = "README-public.md"
 packages = [
     { include = "cmem" }
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-certifi = "^2022.12.7"
+certifi = ">=2023.5.7"
 pyparsing = "^3.0.9"
 pysocks = "^1.7.1"
-rdflib = "^6.2.0"
-requests = "^2.28.1"
+rdflib = "^6.3.2"
+requests = "^2.31.0"
 requests-toolbelt = "^0.10.1"
 six = "^1.16.0"
 
 [tool.poetry.group.dev.dependencies]
 bandit = "^1.7.2"
 black = "^22.1.0"
 coverage = "^6.3.2"
```

### Comparing `cmem_cmempy-23.1/PKG-INFO` & `cmem_cmempy-23.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: cmem-cmempy
-Version: 23.1
-Summary: API wrapper for eccenca Corporate Memory
+Version: 23.1.1
+Summary: API for eccenca Corporate Memory
 Home-page: https://eccenca.com/go/cmempy
 License: Apache-2.0
 Author: eccenca GmbH
 Author-email: cmempy-developer@eccenca.com
 Maintainer: Sebastian Tramp
 Maintainer-email: sebastian.tramp@eccenca.com
 Requires-Python: >=3.9,<4.0
@@ -15,23 +15,22 @@
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Testing
 Classifier: Topic :: Utilities
-Requires-Dist: certifi (>=2022.12.7,<2023.0.0)
+Requires-Dist: certifi (>=2023.5.7)
 Requires-Dist: pyparsing (>=3.0.9,<4.0.0)
 Requires-Dist: pysocks (>=1.7.1,<2.0.0)
-Requires-Dist: rdflib (>=6.2.0,<7.0.0)
-Requires-Dist: requests (>=2.28.1,<3.0.0)
+Requires-Dist: rdflib (>=6.3.2,<7.0.0)
+Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: requests-toolbelt (>=0.10.1,<0.11.0)
 Requires-Dist: six (>=1.16.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # cmempy
 
 cmempy is a Python API wrapper for [eccenca Corporate Memory](https://documentation.eccenca.com/).
```

