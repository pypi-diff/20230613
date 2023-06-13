# Comparing `tmp/solidityscan-0.1.4.tar.gz` & `tmp/solidityscan-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "solidityscan-0.1.4.tar", last modified: Thu Jun  8 10:39:26 2023, max compression
+gzip compressed data, was "solidityscan-0.1.6.tar", last modified: Mon Jun 12 12:41:50 2023, max compression
```

## Comparing `solidityscan-0.1.4.tar` & `solidityscan-0.1.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-08 10:39:26.140337 solidityscan-0.1.4/
--rw-r--r--   0 manosriram   (501) staff       (20)      272 2023-06-08 10:39:26.140198 solidityscan-0.1.4/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)       55 2023-05-15 17:56:15.000000 solidityscan-0.1.4/README.md
--rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-06-08 10:39:26.140376 solidityscan-0.1.4/setup.cfg
--rw-r--r--   0 manosriram   (501) staff       (20)     1290 2023-06-08 10:39:12.000000 solidityscan-0.1.4/setup.py
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-08 10:39:26.139279 solidityscan-0.1.4/solidityscan.egg-info/
--rw-r--r--   0 manosriram   (501) staff       (20)      272 2023-06-08 10:39:26.000000 solidityscan-0.1.4/solidityscan.egg-info/PKG-INFO
--rw-r--r--   0 manosriram   (501) staff       (20)      415 2023-06-08 10:39:26.000000 solidityscan-0.1.4/solidityscan.egg-info/SOURCES.txt
--rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-06-08 10:39:26.000000 solidityscan-0.1.4/solidityscan.egg-info/dependency_links.txt
--rw-r--r--   0 manosriram   (501) staff       (20)       74 2023-06-08 10:39:26.000000 solidityscan-0.1.4/solidityscan.egg-info/entry_points.txt
--rw-r--r--   0 manosriram   (501) staff       (20)      387 2023-06-08 10:39:26.000000 solidityscan-0.1.4/solidityscan.egg-info/requires.txt
--rw-r--r--   0 manosriram   (501) staff       (20)       19 2023-06-08 10:39:26.000000 solidityscan-0.1.4/solidityscan.egg-info/top_level.txt
-drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-08 10:39:26.140010 solidityscan-0.1.4/solidityscan_agent/
--rw-r--r--   0 manosriram   (501) staff       (20)     3352 2023-06-08 10:37:57.000000 solidityscan-0.1.4/solidityscan_agent/__init__.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1833 2023-06-08 10:37:59.000000 solidityscan-0.1.4/solidityscan_agent/config.py
--rw-r--r--   0 manosriram   (501) staff       (20)      211 2023-06-06 06:05:13.000000 solidityscan-0.1.4/solidityscan_agent/constants.py
--rw-r--r--   0 manosriram   (501) staff       (20)     1356 2023-06-08 10:38:02.000000 solidityscan-0.1.4/solidityscan_agent/exceptions.py
--rw-r--r--   0 manosriram   (501) staff       (20)      916 2023-06-08 10:38:07.000000 solidityscan-0.1.4/solidityscan_agent/lang.py
--rw-r--r--   0 manosriram   (501) staff       (20)     2872 2023-06-08 10:38:09.000000 solidityscan-0.1.4/solidityscan_agent/scan.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-12 12:41:50.725841 solidityscan-0.1.6/
+-rw-r--r--   0 manosriram   (501) staff       (20)      272 2023-06-12 12:41:50.725685 solidityscan-0.1.6/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)       55 2023-05-15 17:56:15.000000 solidityscan-0.1.6/README.md
+-rw-r--r--   0 manosriram   (501) staff       (20)       38 2023-06-12 12:41:50.725879 solidityscan-0.1.6/setup.cfg
+-rw-r--r--   0 manosriram   (501) staff       (20)     1290 2023-06-12 12:40:47.000000 solidityscan-0.1.6/setup.py
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-12 12:41:50.724626 solidityscan-0.1.6/solidityscan.egg-info/
+-rw-r--r--   0 manosriram   (501) staff       (20)      272 2023-06-12 12:41:50.000000 solidityscan-0.1.6/solidityscan.egg-info/PKG-INFO
+-rw-r--r--   0 manosriram   (501) staff       (20)      444 2023-06-12 12:41:50.000000 solidityscan-0.1.6/solidityscan.egg-info/SOURCES.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)        1 2023-06-12 12:41:50.000000 solidityscan-0.1.6/solidityscan.egg-info/dependency_links.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       74 2023-06-12 12:41:50.000000 solidityscan-0.1.6/solidityscan.egg-info/entry_points.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)      387 2023-06-12 12:41:50.000000 solidityscan-0.1.6/solidityscan.egg-info/requires.txt
+-rw-r--r--   0 manosriram   (501) staff       (20)       19 2023-06-12 12:41:50.000000 solidityscan-0.1.6/solidityscan.egg-info/top_level.txt
+drwxr-xr-x   0 manosriram   (501) staff       (20)        0 2023-06-12 12:41:50.725503 solidityscan-0.1.6/solidityscan_agent/
+-rw-r--r--   0 manosriram   (501) staff       (20)     4084 2023-06-12 12:39:05.000000 solidityscan-0.1.6/solidityscan_agent/__init__.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1833 2023-06-12 12:35:16.000000 solidityscan-0.1.6/solidityscan_agent/config.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      211 2023-06-06 06:05:13.000000 solidityscan-0.1.6/solidityscan_agent/constants.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1606 2023-06-12 12:25:13.000000 solidityscan-0.1.6/solidityscan_agent/exceptions.py
+-rw-r--r--   0 manosriram   (501) staff       (20)      916 2023-06-12 12:35:24.000000 solidityscan-0.1.6/solidityscan_agent/lang.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     1217 2023-06-12 12:35:34.000000 solidityscan-0.1.6/solidityscan_agent/report.py
+-rw-r--r--   0 manosriram   (501) staff       (20)     2872 2023-06-12 12:35:41.000000 solidityscan-0.1.6/solidityscan_agent/scan.py
```

### Comparing `solidityscan-0.1.4/setup.py` & `solidityscan-0.1.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import os
 
 def readme():
     with open(os.path.join(os.path.dirname(__file__), 'README.md')) as f:
         return f.read()
 
 setup(name="solidityscan",
-      version="0.1.4",
+      version="0.1.6",
       description="Get your smart contracts audited by a smarter tool",
       long_description=readme(),
       long_description_content_type='text/markdown',
       url="https://solidityscan.com",
       entry_points={
         'console_scripts': [
             'solidityscan=solidityscan_agent.__init__:solidityscan',
```

### Comparing `solidityscan-0.1.4/solidityscan_agent/__init__.py` & `solidityscan-0.1.6/solidityscan_agent/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import click
 
 from solidityscan_agent.config import Config
+from solidityscan_agent.report import Report
 from solidityscan_agent.scan import Scan
 
 """
     each command is mapped to @config.command()
     commands can be grouped. a group can be created by mapping the method to @config.group()
 """
 
@@ -74,9 +75,26 @@
         if not contract_chain:
             raise click.UsageError("-contract-chain flag is required")
         if not contract_platform:
             raise click.UsageError("-contract-platform flag is required")
         
         s.block_scan(contract_address, contract_chain, contract_platform, rescan, token)
 
+@solidityscan.command()
+@click.option("--report-type", "-r", required=True, type=click.Choice(["generate"]), prompt=False, help="report command")
+@click.option("-project-id", required=False, help="project id to generate report for")
+@click.option("-scan-id", required=False, help="scan associated with the project")
+def report(report_type, project_id, scan_id):
+    """perform report related actions"""
+
+    r = Report()
+
+    if report_type == "generate":
+        if not project_id:
+            raise click.UsageError("-project-id flag is required")
+        if not scan_id:
+            raise click.UsageError("-scan-id flag is required")
+
+        r.generate_report(project_id, scan_id)
+
 if __name__ == "__main__":
     solidityscan()
```

### Comparing `solidityscan-0.1.4/solidityscan_agent/config.py` & `solidityscan-0.1.6/solidityscan_agent/config.py`

 * *Files identical despite different names*

### Comparing `solidityscan-0.1.4/solidityscan_agent/exceptions.py` & `solidityscan-0.1.6/solidityscan_agent/exceptions.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,14 +21,20 @@
 
 class ScanFailed(Exception):
     def __init__(self, err_payload={"status": "failed", "message": "internal server error"}) -> None:
         err_payload = ErrorLanguageMapper().translate(err_payload)
 
         super().__init__(err_payload)
 
+class ReportGenerationFailed(Exception):
+    def __init__(self, err_payload={"status": "failed", "message": "internal server error"}) -> None:
+        err_payload = ErrorLanguageMapper().translate(err_payload)
+
+        super().__init__(err_payload)
+
 class HostNotReachable(Exception):
     @staticmethod
     def get_err_code():
         err_code = "ERR_1001"
         return err_code
 
     @staticmethod
```

### Comparing `solidityscan-0.1.4/solidityscan_agent/lang.py` & `solidityscan-0.1.6/solidityscan_agent/lang.py`

 * *Files identical despite different names*

### Comparing `solidityscan-0.1.4/solidityscan_agent/scan.py` & `solidityscan-0.1.6/solidityscan_agent/scan.py`

 * *Files identical despite different names*

