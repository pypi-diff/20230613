# Comparing `tmp/gardener-cicd-dso-1.2071.0.tar.gz` & `tmp/gardener-cicd-dso-1.2072.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gardener-cicd-dso-1.2071.0.tar", last modified: Tue Jun 13 04:34:35 2023, max compression
+gzip compressed data, was "gardener-cicd-dso-1.2072.0.tar", last modified: Tue Jun 13 09:03:48 2023, max compression
```

## Comparing `gardener-cicd-dso-1.2071.0.tar` & `gardener-cicd-dso-1.2072.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 04:34:35.431461 gardener-cicd-dso-1.2071.0/
--rw-r--r--   0 root         (0) root         (0)    16830 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/LICENSE.md
--rw-r--r--   0 root         (0) root         (0)      132 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/NOTICE.md
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-13 04:34:35.431461 gardener-cicd-dso-1.2071.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1820 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 04:34:35.427461 gardener-cicd-dso-1.2071.0/checkmarx/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/checkmarx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7623 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/checkmarx/client.py
--rw-r--r--   0 root         (0) root         (0)     3746 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/checkmarx/model.py
--rw-r--r--   0 root         (0) root         (0)     7006 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/checkmarx/project.py
--rw-r--r--   0 root         (0) root         (0)     5790 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/checkmarx/tablefmt.py
--rw-r--r--   0 root         (0) root         (0)    17856 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/checkmarx/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 04:34:35.427461 gardener-cicd-dso-1.2071.0/clamav/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/clamav/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5287 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/clamav/client.py
--rw-r--r--   0 root         (0) root         (0)     8057 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/clamav/cnudie.py
--rw-r--r--   0 root         (0) root         (0)     2252 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/clamav/model.py
--rw-r--r--   0 root         (0) root         (0)     1528 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/clamav/report.py
--rw-r--r--   0 root         (0) root         (0)     1690 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/clamav/routes.py
--rw-r--r--   0 root         (0) root         (0)     7469 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/clamav/scan.py
--rw-r--r--   0 root         (0) root         (0)     6577 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/clamav/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 04:34:35.427461 gardener-cicd-dso-1.2071.0/gardener_cicd_dso.egg-info/
--rw-r--r--   0 root         (0) root         (0)      171 2023-06-13 04:34:35.000000 gardener-cicd-dso-1.2071.0/gardener_cicd_dso.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      688 2023-06-13 04:34:35.000000 gardener-cicd-dso-1.2071.0/gardener_cicd_dso.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 04:34:35.000000 gardener-cicd-dso-1.2071.0/gardener_cicd_dso.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-06-13 04:34:35.000000 gardener-cicd-dso-1.2071.0/gardener_cicd_dso.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-06-13 04:34:35.000000 gardener-cicd-dso-1.2071.0/gardener_cicd_dso.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 04:34:35.431461 gardener-cicd-dso-1.2071.0/protecode/
--rw-r--r--   0 root         (0) root         (0)      740 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/protecode/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5756 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/protecode/assessments.py
--rw-r--r--   0 root         (0) root         (0)    17050 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/protecode/client.py
--rw-r--r--   0 root         (0) root         (0)    12151 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/protecode/model.py
--rw-r--r--   0 root         (0) root         (0)     4254 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/protecode/report.py
--rw-r--r--   0 root         (0) root         (0)     3594 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/protecode/rescore.py
--rw-r--r--   0 root         (0) root         (0)    24726 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/protecode/scanning.py
--rw-r--r--   0 root         (0) root         (0)     8437 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/protecode/util.py
--rw-r--r--   0 root         (0) root         (0)      174 2023-06-13 04:34:35.431461 gardener-cicd-dso-1.2071.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      673 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/setup.dso.py
--rw-r--r--   0 root         (0) root         (0)     2096 2023-06-13 04:33:41.000000 gardener-cicd-dso-1.2071.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:03:48.219441 gardener-cicd-dso-1.2072.0/
+-rw-r--r--   0 root         (0) root         (0)    16830 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/LICENSE.md
+-rw-r--r--   0 root         (0) root         (0)      132 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/NOTICE.md
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-13 09:03:48.219441 gardener-cicd-dso-1.2072.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1820 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:03:48.215440 gardener-cicd-dso-1.2072.0/checkmarx/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/checkmarx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7623 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/checkmarx/client.py
+-rw-r--r--   0 root         (0) root         (0)     3746 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/checkmarx/model.py
+-rw-r--r--   0 root         (0) root         (0)     7006 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/checkmarx/project.py
+-rw-r--r--   0 root         (0) root         (0)     5790 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/checkmarx/tablefmt.py
+-rw-r--r--   0 root         (0) root         (0)    17856 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/checkmarx/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:03:48.215440 gardener-cicd-dso-1.2072.0/clamav/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/clamav/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5287 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/clamav/client.py
+-rw-r--r--   0 root         (0) root         (0)     8057 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/clamav/cnudie.py
+-rw-r--r--   0 root         (0) root         (0)     2252 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/clamav/model.py
+-rw-r--r--   0 root         (0) root         (0)     1528 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/clamav/report.py
+-rw-r--r--   0 root         (0) root         (0)     1690 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/clamav/routes.py
+-rw-r--r--   0 root         (0) root         (0)     7469 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/clamav/scan.py
+-rw-r--r--   0 root         (0) root         (0)     6577 2023-06-13 09:03:03.000000 gardener-cicd-dso-1.2072.0/clamav/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:03:48.215440 gardener-cicd-dso-1.2072.0/gardener_cicd_dso.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      171 2023-06-13 09:03:48.000000 gardener-cicd-dso-1.2072.0/gardener_cicd_dso.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      688 2023-06-13 09:03:48.000000 gardener-cicd-dso-1.2072.0/gardener_cicd_dso.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 09:03:48.000000 gardener-cicd-dso-1.2072.0/gardener_cicd_dso.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-06-13 09:03:48.000000 gardener-cicd-dso-1.2072.0/gardener_cicd_dso.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-06-13 09:03:48.000000 gardener-cicd-dso-1.2072.0/gardener_cicd_dso.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 09:03:48.215440 gardener-cicd-dso-1.2072.0/protecode/
+-rw-r--r--   0 root         (0) root         (0)      740 2023-06-13 09:03:04.000000 gardener-cicd-dso-1.2072.0/protecode/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5756 2023-06-13 09:03:04.000000 gardener-cicd-dso-1.2072.0/protecode/assessments.py
+-rw-r--r--   0 root         (0) root         (0)    17050 2023-06-13 09:03:04.000000 gardener-cicd-dso-1.2072.0/protecode/client.py
+-rw-r--r--   0 root         (0) root         (0)    12151 2023-06-13 09:03:04.000000 gardener-cicd-dso-1.2072.0/protecode/model.py
+-rw-r--r--   0 root         (0) root         (0)     4254 2023-06-13 09:03:04.000000 gardener-cicd-dso-1.2072.0/protecode/report.py
+-rw-r--r--   0 root         (0) root         (0)     3651 2023-06-13 09:03:04.000000 gardener-cicd-dso-1.2072.0/protecode/rescore.py
+-rw-r--r--   0 root         (0) root         (0)    24726 2023-06-13 09:03:04.000000 gardener-cicd-dso-1.2072.0/protecode/scanning.py
+-rw-r--r--   0 root         (0) root         (0)     8437 2023-06-13 09:03:04.000000 gardener-cicd-dso-1.2072.0/protecode/util.py
+-rw-r--r--   0 root         (0) root         (0)      174 2023-06-13 09:03:48.219441 gardener-cicd-dso-1.2072.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      673 2023-06-13 09:03:04.000000 gardener-cicd-dso-1.2072.0/setup.dso.py
+-rw-r--r--   0 root         (0) root         (0)     2096 2023-06-13 09:03:04.000000 gardener-cicd-dso-1.2072.0/setup.py
```

### Comparing `gardener-cicd-dso-1.2071.0/LICENSE.md` & `gardener-cicd-dso-1.2072.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/README.md` & `gardener-cicd-dso-1.2072.0/README.md`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/checkmarx/__init__.py` & `gardener-cicd-dso-1.2072.0/checkmarx/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/checkmarx/client.py` & `gardener-cicd-dso-1.2072.0/checkmarx/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/checkmarx/model.py` & `gardener-cicd-dso-1.2072.0/checkmarx/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/checkmarx/project.py` & `gardener-cicd-dso-1.2072.0/checkmarx/project.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/checkmarx/tablefmt.py` & `gardener-cicd-dso-1.2072.0/checkmarx/tablefmt.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/checkmarx/util.py` & `gardener-cicd-dso-1.2072.0/checkmarx/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/clamav/__init__.py` & `gardener-cicd-dso-1.2072.0/clamav/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/clamav/client.py` & `gardener-cicd-dso-1.2072.0/clamav/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/clamav/cnudie.py` & `gardener-cicd-dso-1.2072.0/clamav/cnudie.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/clamav/model.py` & `gardener-cicd-dso-1.2072.0/clamav/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/clamav/report.py` & `gardener-cicd-dso-1.2072.0/clamav/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/clamav/routes.py` & `gardener-cicd-dso-1.2072.0/clamav/routes.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/clamav/scan.py` & `gardener-cicd-dso-1.2072.0/clamav/scan.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/clamav/util.py` & `gardener-cicd-dso-1.2072.0/clamav/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/gardener_cicd_dso.egg-info/SOURCES.txt` & `gardener-cicd-dso-1.2072.0/gardener_cicd_dso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/protecode/__init__.py` & `gardener-cicd-dso-1.2072.0/protecode/__init__.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/protecode/assessments.py` & `gardener-cicd-dso-1.2072.0/protecode/assessments.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/protecode/client.py` & `gardener-cicd-dso-1.2072.0/protecode/client.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/protecode/model.py` & `gardener-cicd-dso-1.2072.0/protecode/model.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/protecode/report.py` & `gardener-cicd-dso-1.2072.0/protecode/report.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/protecode/rescore.py` & `gardener-cicd-dso-1.2072.0/protecode/rescore.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,14 +50,16 @@
     components_with_vulnerabilities = [c for c in all_components if tuple(c.vulnerabilities())]
 
     components_with_vulnerabilities = sorted(
         components_with_vulnerabilities,
         key=lambda c: c.name()
     )
 
+    is_fetch_required = False
+
     for c in components_with_vulnerabilities:
         if not c.version():
             continue # do not inject dummy-versions in fully automated mode, yet
 
         vulns_to_assess = []
 
         for v in c.vulnerabilities():
@@ -84,24 +86,25 @@
             )
 
             if rescored is dso.cvss.CVESeverity.NONE:
                 vulns_to_assess.append(v)
 
         if vulns_to_assess:
             logger.info(f'{len(vulns_to_assess)=}: {[v.cve() for v in vulns_to_assess]}')
+            is_fetch_required = True
             bdba_client.add_triage_raw({
                 'component': c.name(),
                 'version': c.version(),
                 'vulns': [v.cve() for v in vulns_to_assess],
                 'scope': protecode.model.TriageScope.RESULT.value,
                 'reason': 'OT',
                 'description': 'auto-assessed as irrelevant based on cve-categorisation',
                 'product_id': product_id,
             })
 
-    if vulns_to_assess:
+    if is_fetch_required:
         logger.info('retrieving result again from bdba (this may take a while)')
         scan_result = bdba_client.wait_for_scan_result(
-            product_id=scan_result.product_id()
+            product_id=product_id,
         )
 
     return scan_result
```

### Comparing `gardener-cicd-dso-1.2071.0/protecode/scanning.py` & `gardener-cicd-dso-1.2072.0/protecode/scanning.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/protecode/util.py` & `gardener-cicd-dso-1.2072.0/protecode/util.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/setup.dso.py` & `gardener-cicd-dso-1.2072.0/setup.dso.py`

 * *Files identical despite different names*

### Comparing `gardener-cicd-dso-1.2071.0/setup.py` & `gardener-cicd-dso-1.2072.0/setup.py`

 * *Files identical despite different names*

