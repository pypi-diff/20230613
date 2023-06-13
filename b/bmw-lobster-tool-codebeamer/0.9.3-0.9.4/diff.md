# Comparing `tmp/bmw-lobster-tool-codebeamer-0.9.3.tar.gz` & `tmp/bmw-lobster-tool-codebeamer-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bmw-lobster-tool-codebeamer-0.9.3.tar", last modified: Tue May  9 09:58:20 2023, max compression
+gzip compressed data, was "bmw-lobster-tool-codebeamer-0.9.4.tar", last modified: Tue Jun 13 09:18:56 2023, max compression
```

## Comparing `bmw-lobster-tool-codebeamer-0.9.3.tar` & `bmw-lobster-tool-codebeamer-0.9.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:20.468663 bmw-lobster-tool-codebeamer-0.9.3/
--rw-r--r--   0 florian   (1000) florian   (1000)     1754 2023-05-09 09:58:20.464662 bmw-lobster-tool-codebeamer-0.9.3/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      814 2023-05-08 15:03:18.000000 bmw-lobster-tool-codebeamer-0.9.3/README.md
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:20.464662 bmw-lobster-tool-codebeamer-0.9.3/bmw_lobster_tool_codebeamer.egg-info/
--rw-r--r--   0 florian   (1000) florian   (1000)     1754 2023-05-09 09:58:20.000000 bmw-lobster-tool-codebeamer-0.9.3/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO
--rw-r--r--   0 florian   (1000) florian   (1000)      402 2023-05-09 09:58:20.000000 bmw-lobster-tool-codebeamer-0.9.3/bmw_lobster_tool_codebeamer.egg-info/SOURCES.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-05-09 09:58:20.000000 bmw-lobster-tool-codebeamer-0.9.3/bmw_lobster_tool_codebeamer.egg-info/dependency_links.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       80 2023-05-09 09:58:20.000000 bmw-lobster-tool-codebeamer-0.9.3/bmw_lobster_tool_codebeamer.egg-info/entry_points.txt
--rw-r--r--   0 florian   (1000) florian   (1000)       39 2023-05-09 09:58:20.000000 bmw-lobster-tool-codebeamer-0.9.3/bmw_lobster_tool_codebeamer.egg-info/requires.txt
--rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-05-09 09:58:20.000000 bmw-lobster-tool-codebeamer-0.9.3/bmw_lobster_tool_codebeamer.egg-info/top_level.txt
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:20.464662 bmw-lobster-tool-codebeamer-0.9.3/lobster/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:20.464662 bmw-lobster-tool-codebeamer-0.9.3/lobster/tools/
-drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:20.464662 bmw-lobster-tool-codebeamer-0.9.3/lobster/tools/codebeamer/
--rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-05-09 09:58:20.000000 bmw-lobster-tool-codebeamer-0.9.3/lobster/tools/codebeamer/__init__.py
--rwxr-xr-x   0 florian   (1000) florian   (1000)     7902 2023-05-09 09:58:20.000000 bmw-lobster-tool-codebeamer-0.9.3/lobster/tools/codebeamer/codebeamer.py
--rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-05-09 09:58:20.468663 bmw-lobster-tool-codebeamer-0.9.3/setup.cfg
--rw-r--r--   0 florian   (1000) florian   (1000)     2296 2023-05-08 15:03:18.000000 bmw-lobster-tool-codebeamer-0.9.3/setup.py
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.841244 bmw-lobster-tool-codebeamer-0.9.4/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1756 2023-06-13 09:18:56.841244 bmw-lobster-tool-codebeamer-0.9.4/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      816 2023-06-13 09:17:37.000000 bmw-lobster-tool-codebeamer-0.9.4/README.md
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.841244 bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/
+-rw-r--r--   0 florian   (1000) florian   (1000)     1756 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO
+-rw-r--r--   0 florian   (1000) florian   (1000)      402 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/SOURCES.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        1 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/dependency_links.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       80 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/entry_points.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)       39 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/requires.txt
+-rw-r--r--   0 florian   (1000) florian   (1000)        8 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/top_level.txt
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.837244 bmw-lobster-tool-codebeamer-0.9.4/lobster/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.837244 bmw-lobster-tool-codebeamer-0.9.4/lobster/tools/
+drwxr-xr-x   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.841244 bmw-lobster-tool-codebeamer-0.9.4/lobster/tools/codebeamer/
+-rw-r--r--   0 florian   (1000) florian   (1000)        0 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/lobster/tools/codebeamer/__init__.py
+-rwxr-xr-x   0 florian   (1000) florian   (1000)     9495 2023-06-13 09:18:56.000000 bmw-lobster-tool-codebeamer-0.9.4/lobster/tools/codebeamer/codebeamer.py
+-rw-r--r--   0 florian   (1000) florian   (1000)       38 2023-06-13 09:18:56.841244 bmw-lobster-tool-codebeamer-0.9.4/setup.cfg
+-rw-r--r--   0 florian   (1000) florian   (1000)     2296 2023-05-08 15:03:18.000000 bmw-lobster-tool-codebeamer-0.9.4/setup.py
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.3/PKG-INFO` & `bmw-lobster-tool-codebeamer-0.9.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-codebeamer
-Version: 0.9.3
+Version: 0.9.4
 Summary: LOBSTER Tool for Codebeamer
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
@@ -16,16 +16,16 @@
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 
 # LOBSTER
 
-The **L**ightweight **O**pen **B**MW **S**oftware **T**racability
-**E**vidence **R**eport allows you to demonstrate software tracability
+The **L**ightweight **O**pen **B**MW **S**oftware **T**raceability
+**E**vidence **R**eport allows you to demonstrate software traceability
 and requirements coverage, which is essential for meeting standards
 such as ISO 26262.
 
 This package contains a tool to interface with the proprietary
 requirements management tool
 [Codebeamer](https://intland.com/codebeamer).
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.3/README.md` & `bmw-lobster-tool-codebeamer-0.9.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # LOBSTER
 
-The **L**ightweight **O**pen **B**MW **S**oftware **T**racability
-**E**vidence **R**eport allows you to demonstrate software tracability
+The **L**ightweight **O**pen **B**MW **S**oftware **T**raceability
+**E**vidence **R**eport allows you to demonstrate software traceability
 and requirements coverage, which is essential for meeting standards
 such as ISO 26262.
 
 This package contains a tool to interface with the proprietary
 requirements management tool
 [Codebeamer](https://intland.com/codebeamer).
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.3/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO` & `bmw-lobster-tool-codebeamer-0.9.4/bmw_lobster_tool_codebeamer.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bmw-lobster-tool-codebeamer
-Version: 0.9.3
+Version: 0.9.4
 Summary: LOBSTER Tool for Codebeamer
 Home-page: https://github.com/bmw-software-engineering/lobster
 Author: Bayerische Motoren Werke Aktiengesellschaft (BMW AG)
 Author-email: florian.schanda@bmw.de
 License: GNU Affero General Public License v3
 Project-URL: Bug Tracker, https://github.com/bmw-software-engineering/lobster/issues
 Project-URL: Documentation, https://github.com/pages/bmw-software-engineering/lobster/
@@ -16,16 +16,16 @@
 Classifier: Topic :: Documentation
 Classifier: Topic :: Software Development
 Requires-Python: >=3.7, <4
 Description-Content-Type: text/markdown
 
 # LOBSTER
 
-The **L**ightweight **O**pen **B**MW **S**oftware **T**racability
-**E**vidence **R**eport allows you to demonstrate software tracability
+The **L**ightweight **O**pen **B**MW **S**oftware **T**raceability
+**E**vidence **R**eport allows you to demonstrate software traceability
 and requirements coverage, which is essential for meeting standards
 such as ISO 26262.
 
 This package contains a tool to interface with the proprietary
 requirements management tool
 [Codebeamer](https://intland.com/codebeamer).
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.3/lobster/tools/codebeamer/codebeamer.py` & `bmw-lobster-tool-codebeamer-0.9.4/lobster/tools/codebeamer/codebeamer.py`

 * *Files 16% similar despite different names*

```diff
@@ -95,14 +95,48 @@
         if len(rv) == data["total"]:
             break
         page_id += 1
 
     return rv
 
 
+def get_query(mh, cb_config, query_id):
+    assert isinstance(mh, Message_Handler)
+    assert isinstance(cb_config, dict)
+    assert isinstance(query_id, int)
+    rv = []
+    page_id = 1
+    total_items = None
+
+    while total_items is None or len(rv) < total_items:
+        print("Fetching page %u of query..." % page_id)
+        data = query_cb_single(cb_config,
+                               "%s/query/%u/page/%u?pagesize=100" %
+                               (cb_config["base"],
+                                query_id,
+                                page_id))
+        assert len(data) == 1
+        data = data["trackerItems"]
+
+        assert page_id == data["page"]
+        if page_id == 1:
+            total_items = data["total"]
+        else:
+            assert total_items == data["total"]
+
+        rv += [to_lobster(cb_config, cb_item)
+               for cb_item in data["items"]]
+
+        page_id += 1
+
+    assert total_items == len(rv)
+
+    return rv
+
+
 def to_lobster(cb_config, cb_item):
     assert isinstance(cb_config, dict)
     assert isinstance(cb_item, dict) and "id" in cb_item
 
     # This looks like it's business logic, maybe we should make this
     # configurable?
 
@@ -171,14 +205,17 @@
 def main():
     ap = argparse.ArgumentParser()
 
     modes = ap.add_mutually_exclusive_group()
     modes.add_argument("--import-tagged",
                        metavar="LOBSTER_FILE",
                        default=None)
+    modes.add_argument("--import-query",
+                       metavar="CB_QUERY_ID",
+                       default=None)
 
     ap.add_argument("--cb-root", default=os.environ.get("CB_ROOT", None))
     ap.add_argument("--cb-user", default=os.environ.get("CB_USERNAME", None))
     ap.add_argument("--cb-pass", default=os.environ.get("CB_PASSWORD", None))
     ap.add_argument("--out", default=None)
     options = ap.parse_args()
 
@@ -215,31 +252,44 @@
                     else:
                         mh.warning(item.location,
                                    "invalid codebeamer reference to %i" %
                                    item_id)
                 except ValueError:
                     pass
 
+    elif options.import_query:
+        try:
+            query_id = int(options.import_query)
+        except ValueError:
+            ap.error("query-id must be an integer")
+        if query_id < 1:
+            ap.error("query-id must be a positive")
+
     cb_config = {
         "root" : options.cb_root,
         "base" : "%s/cb/rest" % options.cb_root,
         "user" : options.cb_user,
         "pass" : options.cb_pass,
     }
 
     try:
-        items = import_tagged(mh, cb_config, items_to_import)
+        if options.import_tagged:
+            items = import_tagged(mh, cb_config, items_to_import)
+        elif options.import_query:
+            items = get_query(mh, cb_config, query_id)
     except LOBSTER_Error:
         return 1
 
     if options.out is None:
         lobster_write(sys.stdout, Requirement, "lobster_codebeamer", items)
         print()
     else:
         with open(options.out, "w", encoding="UTF-8") as fd:
             lobster_write(fd, Requirement, "lobster_codebeamer", items)
+        print("Written %u requirements to %s" % (len(items),
+                                                 options.out))
 
     return 0
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `bmw-lobster-tool-codebeamer-0.9.3/setup.py` & `bmw-lobster-tool-codebeamer-0.9.4/setup.py`

 * *Files identical despite different names*

