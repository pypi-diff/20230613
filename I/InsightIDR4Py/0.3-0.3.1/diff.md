# Comparing `tmp/InsightIDR4Py-0.3.tar.gz` & `tmp/InsightIDR4Py-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "InsightIDR4Py-0.3.tar", last modified: Tue May 23 21:28:50 2023, max compression
+gzip compressed data, was "InsightIDR4Py-0.3.1.tar", last modified: Tue Jun 13 17:27:06 2023, max compression
```

## Comparing `InsightIDR4Py-0.3.tar` & `InsightIDR4Py-0.3.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-23 21:28:50.198984 InsightIDR4Py-0.3/
-drwxrwxrwx   0        0        0        0 2023-05-23 21:28:50.198984 InsightIDR4Py-0.3/InsightIDR4Py.egg-info/
--rw-rw-rw-   0        0        0     6046 2023-05-23 21:28:49.000000 InsightIDR4Py-0.3/InsightIDR4Py.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      252 2023-05-23 21:28:50.000000 InsightIDR4Py-0.3/InsightIDR4Py.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-23 21:28:49.000000 InsightIDR4Py-0.3/InsightIDR4Py.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-23 21:28:49.000000 InsightIDR4Py-0.3/InsightIDR4Py.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-05-23 21:28:49.000000 InsightIDR4Py-0.3/InsightIDR4Py.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    25652 2023-05-23 21:22:05.000000 InsightIDR4Py-0.3/InsightIDR4Py.py
--rw-rw-rw-   0        0        0     1092 2023-05-22 16:57:04.000000 InsightIDR4Py-0.3/LICENSE
--rw-rw-rw-   0        0        0     6046 2023-05-23 21:28:50.207170 InsightIDR4Py-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     5628 2023-05-23 21:27:27.000000 InsightIDR4Py-0.3/README.md
--rw-rw-rw-   0        0        0       99 2023-05-22 16:55:58.000000 InsightIDR4Py-0.3/pyproject.toml
--rw-rw-rw-   0        0        0      111 2023-05-23 21:28:50.207170 InsightIDR4Py-0.3/setup.cfg
--rw-rw-rw-   0        0        0      692 2023-05-23 21:27:49.000000 InsightIDR4Py-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 17:27:06.865500 InsightIDR4Py-0.3.1/
+drwxrwxrwx   0        0        0        0 2023-06-13 17:27:06.865500 InsightIDR4Py-0.3.1/InsightIDR4Py.egg-info/
+-rw-rw-rw-   0        0        0     6773 2023-06-13 17:27:06.000000 InsightIDR4Py-0.3.1/InsightIDR4Py.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      252 2023-06-13 17:27:06.000000 InsightIDR4Py-0.3.1/InsightIDR4Py.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 17:27:06.000000 InsightIDR4Py-0.3.1/InsightIDR4Py.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-06-13 17:27:06.000000 InsightIDR4Py-0.3.1/InsightIDR4Py.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-13 17:27:06.000000 InsightIDR4Py-0.3.1/InsightIDR4Py.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    32029 2023-06-13 17:12:23.000000 InsightIDR4Py-0.3.1/InsightIDR4Py.py
+-rw-rw-rw-   0        0        0     1092 2023-06-11 15:44:50.000000 InsightIDR4Py-0.3.1/LICENSE
+-rw-rw-rw-   0        0        0     6773 2023-06-13 17:27:06.865500 InsightIDR4Py-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     6346 2023-06-13 17:22:33.000000 InsightIDR4Py-0.3.1/README.md
+-rw-rw-rw-   0        0        0       99 2023-06-11 15:44:50.000000 InsightIDR4Py-0.3.1/pyproject.toml
+-rw-rw-rw-   0        0        0      111 2023-06-13 17:27:06.865500 InsightIDR4Py-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0      702 2023-06-13 17:25:52.000000 InsightIDR4Py-0.3.1/setup.py
```

### Comparing `InsightIDR4Py-0.3/InsightIDR4Py.egg-info/PKG-INFO` & `InsightIDR4Py-0.3.1/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,50 +1,56 @@
-Metadata-Version: 2.1
-Name: InsightIDR4Py
-Version: 0.3
-Summary: A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.
-Home-page: https://github.com/mbabinski/InsightIDR4Py
-Author: Micah Babinski
-Author-email: m.babinski.88@gmail.com
-License: MIT
-Keywords: Rapid7,InsightIDR,SIEM,Logsearch,Investigations,Threats
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # InsightIDR4Py
 A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.
 
-InsightIDR4Py allows analysts to query log data from Rapid7 [InsightIDR](https://docs.rapid7.com/insightidr/), analyze it within Python, and/or feed it to other APIs like VirusTotal, AbuseIPDB, or others. This tool handles some of the challenges and complexities of using the InsightIDR REST API, including polling queries in progress, paginated responses, handling the JSON output, and time range queries.
+InsightIDR4Py allows users to perform numerous actions within Rapid7 [InsightIDR](https://docs.rapid7.com/insightidr/). This tool handles some of the challenges and complexities of using the InsightIDR REST API, including polling queries in progress, paginated responses, handling the JSON output, and time range queries.
+
+These capabilities can be particularly useful for automating processes, integrating log data with other APIs (like VirusTotal), managing content in the InsightIDR platform, and performing multi-tenant workflows (for instance, updating content across tenants for consistency, or copying content from one InsightIDR tenant to another). For some ideas on how InsightIDR4Py can be used, check out this [blog post](https://micahbabinski.medium.com/button-pusher-to-masterbuilder-automating-siem-workflows-3f51874a80e) where I cover some use cases.
+
+The API capabilities provided by InsightIDR4Py include:
+## Logsearch
+* Query Events
+* Query Groups
+
+## Saved Queries
+* List Saved Queries
+* Get a Saved Query
+* Create Saved Query
+* Replace a Saved Query
+* Update a Saved Query
+* Delete a Saved Query
+
+## Custom Alerts*
+* List Custom Alerts
+* Get a Custom Alert
+* Create Custom Alert
+* Replace a Custom Alert
+* Update a Custom Alert
+* Delete a Custom Alert
+
+*Only pattern detection alerts are supported currently.
 
-InsightIDR4Py also offers access to some of the additional APIs in the InsightIDR ecosystem. These include:
 ## Investigations
 * List Investigations
 * Get an Investigation
 * Create Investigation
 * Close Investigations in Bulk
 * List Alerts by Investigation
 * List Rapid7 Product Alerts by Investigation
 * Update Investigation
 * List Comments on an Investigation
 * Create Comment
 * Delete Comment
+
 ## Threats
 * Create Threat
 * Add Indicators to Threat
 * Replace Threat Indicators
 * Delete Threat
-## Saved Queries
-* List Saved Queries
-* Get a Saved Query
-* Create Saved Query
-* Replace a Saved Query
-* Update a Saved Query
-* Delete a Saved Query
 
-Happy analyzing!:monocle_face:
+Happy analyzing :monocle_face: and happy administering! :hammer:
 
 # Installation
 InsightIDR4Py is available on [PyPI](https://pypi.org/project/InsightIDR4Py/) and can be installed using:
 ```
 pip install InsightIDR4Py
 ```
 
@@ -153,8 +159,8 @@
 	print("----------")
 ```
 
 # License
 This repository is licensed under an [MIT license](https://github.com/mbabinski/InsightIDR4Py/blob/main/LICENSE), which grants extensive permission to use this material however you wish.
 
 # Contributing
-You are welcome to contribute however you wish! I appreciate feedback in any format.
+You are welcome to contribute however you wish! I appreciate feedback in any format.
```

### Comparing `InsightIDR4Py-0.3/InsightIDR4Py.py` & `InsightIDR4Py-0.3.1/InsightIDR4Py.py`

 * *Files 21% similar despite different names*

```diff
@@ -27,14 +27,15 @@
             self.region = region
         self.logs_url = "https://{}.rest.logs.insight.rapid7.com/query/logs/".format(self.region)
         self.query_url = "https://{}.rest.logs.insight.rapid7.com/query/".format(self.region)
         self.log_mgmt_url = "https://{}.api.insight.rapid7.com/log_search/management/logs/".format(self.region)
         self.investigations_url = "https://{}.api.insight.rapid7.com/idr/v2/investigations/".format(self.region)
         self.comments_url = "https://{}.api.insight.rapid7.com/idr/v1/comments/".format(self.region)
         self.threat_url = "https://{}.api.insight.rapid7.com/idr/v1/customthreats/".format(self.region)
+        self.mgmt_url = "https://{}.rest.logs.insight.rapid7.com/management/".format(self.region)
 
     def _get_region(self):
         """
         This method cycles through available API regions, making a call to the log management URL with each
         region until a successful call indicates the correct region. If you already know your region, simply
         pass that in when creating the InsightIDR object.
         """
@@ -507,16 +508,195 @@
         """
         data = {"reason": reason}
         url = self.threat_url + "/key/{}/delete".format(threat_key)
         response = self.session.post(url, json=data)
         result = response.json()
 
         return result
-        
-        
+
+    def ListCustomAlerts(self):
+        """
+        Lists all 'Tags' aka alerts, associated with the account.
+        """
+        url = self.mgmt_url + "tags"
+        response = self.session.get(url)
+        result = response.json()
+        alerts = result["tags"]
+
+        return alerts
+
+    def GetCustomAlert(self, custom_alert_id):
+        """
+        Retrieve a single custom alert by its ID value
+        """
+        url = self.mgmt_url + "tags/{}".format(custom_alert_id)
+        response = self.session.get(url)
+        result = response.json()
+        alert = result["tag"]
+
+        return alert
+
+    def CreateCustomAlert(self, name, logsource, query, description="", actions=[], labels=[],
+                                          priority="low"):
+        """
+        Create a custom alert. If log source is set to an array of logsource IDs, these will be used. If a logset name is provided,
+        the log IDs for this log set will be retrieved and used.
+        """
+        # validate input
+        if not priority.lower() in ("low", "medium", "high", "critical"):
+            raise ValueError("Priority must be one of [low, medium, high, critical]!")
+
+        # map alert priority to numeric value
+        priority_mapping = {
+            "low": 1,
+            "medium": 2,
+            "high": 3,
+            "critical": 4
+        }
+        priority = priority_mapping[priority.lower()]
+
+        # list logsource IDs
+        if type(logsource) == list:
+            logsource_ids = [{"id": item} for item in logsource]
+        else:
+            logsource_ids = [{"id": item} for item in self.ListLogIdsByLogSetName(logsource)]
+
+        # format parameters
+        data = {
+            "tag": {
+                "name": name,
+                "sources": logsource_ids,
+                "type": "Alert",
+                "leql": {"statement": query},
+                "description": description,
+                "actions": actions,
+                "labels": labels,
+                "priority": priority
+            }
+        }
+
+        # send request
+        self.session.headers["Content-type"] = "application/json"
+        url = self.mgmt_url + "tags"
+        response = self.session.post(url, json=data)
+        result = response.json()
+
+        return result
+
+    def ReplaceCustomAlert(self, alert_id, name, logsource, query, description="", actions=[], labels=[],
+                           priority="low"):
+        """
+        Replaces a custom alert identified by the alert_id value. If log source is set to an array of logsource IDs, these will be used.
+        If a logset name is provided, the log IDs for this log set will be retrieved and used.
+        """
+        # validate input
+        if not priority.lower() in ("low", "medium", "high", "critical"):
+            raise ValueError("Priority must be one of [low, medium, high, critical]!")
+
+        # map alert priority to numeric value
+        priority_mapping = {
+            "low": 1,
+            "medium": 2,
+            "high": 3,
+            "critical": 4
+        }
+        priority = priority_mapping[priority.lower()]
+
+        # list logsource IDs
+        if type(logsource) == list:
+            logsource_ids = [{"id": item} for item in logsource]
+        else:
+            logsource_ids = [{"id": item} for item in self.ListLogIdsByLogSetName(logsource)]
+
+        # format parameters
+        data = {
+            "tag": {
+                "name": name,
+                "sources": logsource_ids,
+                "type": "Alert",
+                "leql": {"statement": query},
+                "description": description,
+                "actions": actions,
+                "labels": labels,
+                "priority": priority
+            }
+        }
+
+        # send request
+        self.session.headers["Content-type"] = "application/json"
+        url = self.mgmt_url + "tags/{}".format(alert_id)
+        response = self.session.put(url, json=data)
+        result = response.json()
+
+        return result
+
+    def UpdateCustomAlert(self, alert_id, name=None, logsource=None, query=None, description=None, actions=None, labels=None,
+                          priority=None):
+        """
+        Updates any user-specified element of a custom alert, identified by the alert_id
+        """
+        if priority:
+            # validate input
+            if not priority.lower() in ("low", "medium", "high", "critical"):
+                raise ValueError("Priority must be one of [low, medium, high, critical]!")
+
+            # map alert priority to numeric value
+            priority_mapping = {
+                "low": 1,
+                "medium": 2,
+                "high": 3,
+                "critical": 4
+            }
+            priority = priority_mapping[priority.lower()]
+
+        # list logsource IDs
+        if logsource:
+            if type(logsource) == list:
+                logsource_ids = [{"id": item} for item in logsource]
+            else:
+                logsource_ids = [{"id": item} for item in self.ListLogIdsByLogSetName(logsource)]
+        else:
+            logsource_ids = None
+
+        if query:
+            leql_obj = {"statement": query}
+        else:
+            leql_obj = None
+
+        # format parameters
+        params = {
+            "name": name,
+            "sources": logsource_ids,
+            "type": "Alert",
+            "leql": leql_obj,
+            "description": description,
+            "actions": actions,
+            "labels": labels,
+            "priority": priority
+        }
+        params = {k:v for k, v in params.items() if v}
+        data = {"tag": params}
+
+        # send request
+        self.session.headers["Content-type"] = "application/json"
+        url = self.mgmt_url + "tags/{}".format(alert_id)
+        response = self.session.patch(url, json=data)
+        result = response.json()
+
+        return result
+
+    def DeleteCustomAlert(self, alert_id):
+        """
+        Deletes the custom alert identified by the alert_id
+        """
+        url = self.mgmt_url + "tags/{}".format(alert_id)
+        response = self.session.delete(url)
+
+        return response
+                
     def ListSavedQueries(self):
         """
         Lists saved queries in the InsightIDR platform.
         """
         url = self.query_url + "saved_queries"
         response = self.session.get(url)
         result = response.json()
@@ -562,15 +742,15 @@
                     "statement": query,
                     "during": during
                     },
                 "logs": log_ids
                 }
             }
 
-        # make the reuest
+        # make the request
         url = self.query_url + "saved_queries"
         response = self.session.post(url, json=data)
         result = response.json()
 
         return result
 
     def ReplaceSavedQuery(self, saved_query_id, name, query, logset_name=None, time_range=None, from_time=None, to_time=None):
```

### Comparing `InsightIDR4Py-0.3/LICENSE` & `InsightIDR4Py-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `InsightIDR4Py-0.3/PKG-INFO` & `InsightIDR4Py-0.3.1/InsightIDR4Py.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,68 @@
 Metadata-Version: 2.1
 Name: InsightIDR4Py
-Version: 0.3
+Version: 0.3.1
 Summary: A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.
 Home-page: https://github.com/mbabinski/InsightIDR4Py
 Author: Micah Babinski
 Author-email: m.babinski.88@gmail.com
 License: MIT
-Keywords: Rapid7,InsightIDR,SIEM,Logsearch,Investigations,Threats
+Keywords: Rapid7,InsightIDR,SIEM,Logsearch,Investigations,Threats,Alerts
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # InsightIDR4Py
 A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.
 
-InsightIDR4Py allows analysts to query log data from Rapid7 [InsightIDR](https://docs.rapid7.com/insightidr/), analyze it within Python, and/or feed it to other APIs like VirusTotal, AbuseIPDB, or others. This tool handles some of the challenges and complexities of using the InsightIDR REST API, including polling queries in progress, paginated responses, handling the JSON output, and time range queries.
+InsightIDR4Py allows users to perform numerous actions within Rapid7 [InsightIDR](https://docs.rapid7.com/insightidr/). This tool handles some of the challenges and complexities of using the InsightIDR REST API, including polling queries in progress, paginated responses, handling the JSON output, and time range queries.
+
+These capabilities can be particularly useful for automating processes, integrating log data with other APIs (like VirusTotal), managing content in the InsightIDR platform, and performing multi-tenant workflows (for instance, updating content across tenants for consistency, or copying content from one InsightIDR tenant to another). For some ideas on how InsightIDR4Py can be used, check out this [blog post](https://micahbabinski.medium.com/button-pusher-to-masterbuilder-automating-siem-workflows-3f51874a80e) where I cover some use cases.
+
+The API capabilities provided by InsightIDR4Py include:
+## Logsearch
+* Query Events
+* Query Groups
+
+## Saved Queries
+* List Saved Queries
+* Get a Saved Query
+* Create Saved Query
+* Replace a Saved Query
+* Update a Saved Query
+* Delete a Saved Query
+
+## Custom Alerts*
+* List Custom Alerts
+* Get a Custom Alert
+* Create Custom Alert
+* Replace a Custom Alert
+* Update a Custom Alert
+* Delete a Custom Alert
+
+*Only pattern detection alerts are supported currently.
 
-InsightIDR4Py also offers access to some of the additional APIs in the InsightIDR ecosystem. These include:
 ## Investigations
 * List Investigations
 * Get an Investigation
 * Create Investigation
 * Close Investigations in Bulk
 * List Alerts by Investigation
 * List Rapid7 Product Alerts by Investigation
 * Update Investigation
 * List Comments on an Investigation
 * Create Comment
 * Delete Comment
+
 ## Threats
 * Create Threat
 * Add Indicators to Threat
 * Replace Threat Indicators
 * Delete Threat
-## Saved Queries
-* List Saved Queries
-* Get a Saved Query
-* Create Saved Query
-* Replace a Saved Query
-* Update a Saved Query
-* Delete a Saved Query
 
-Happy analyzing!:monocle_face:
+Happy analyzing :monocle_face: and happy administering! :hammer:
 
 # Installation
 InsightIDR4Py is available on [PyPI](https://pypi.org/project/InsightIDR4Py/) and can be installed using:
 ```
 pip install InsightIDR4Py
 ```
```

### Comparing `InsightIDR4Py-0.3/README.md` & `InsightIDR4Py-0.3.1/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,68 @@
+Metadata-Version: 2.1
+Name: InsightIDR4Py
+Version: 0.3.1
+Summary: A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.
+Home-page: https://github.com/mbabinski/InsightIDR4Py
+Author: Micah Babinski
+Author-email: m.babinski.88@gmail.com
+License: MIT
+Keywords: Rapid7,InsightIDR,SIEM,Logsearch,Investigations,Threats,Alerts
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # InsightIDR4Py
 A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.
 
-InsightIDR4Py allows analysts to query log data from Rapid7 [InsightIDR](https://docs.rapid7.com/insightidr/), analyze it within Python, and/or feed it to other APIs like VirusTotal, AbuseIPDB, or others. This tool handles some of the challenges and complexities of using the InsightIDR REST API, including polling queries in progress, paginated responses, handling the JSON output, and time range queries.
+InsightIDR4Py allows users to perform numerous actions within Rapid7 [InsightIDR](https://docs.rapid7.com/insightidr/). This tool handles some of the challenges and complexities of using the InsightIDR REST API, including polling queries in progress, paginated responses, handling the JSON output, and time range queries.
+
+These capabilities can be particularly useful for automating processes, integrating log data with other APIs (like VirusTotal), managing content in the InsightIDR platform, and performing multi-tenant workflows (for instance, updating content across tenants for consistency, or copying content from one InsightIDR tenant to another). For some ideas on how InsightIDR4Py can be used, check out this [blog post](https://micahbabinski.medium.com/button-pusher-to-masterbuilder-automating-siem-workflows-3f51874a80e) where I cover some use cases.
+
+The API capabilities provided by InsightIDR4Py include:
+## Logsearch
+* Query Events
+* Query Groups
+
+## Saved Queries
+* List Saved Queries
+* Get a Saved Query
+* Create Saved Query
+* Replace a Saved Query
+* Update a Saved Query
+* Delete a Saved Query
+
+## Custom Alerts*
+* List Custom Alerts
+* Get a Custom Alert
+* Create Custom Alert
+* Replace a Custom Alert
+* Update a Custom Alert
+* Delete a Custom Alert
+
+*Only pattern detection alerts are supported currently.
 
-InsightIDR4Py also offers access to some of the additional APIs in the InsightIDR ecosystem. These include:
 ## Investigations
 * List Investigations
 * Get an Investigation
 * Create Investigation
 * Close Investigations in Bulk
 * List Alerts by Investigation
 * List Rapid7 Product Alerts by Investigation
 * Update Investigation
 * List Comments on an Investigation
 * Create Comment
 * Delete Comment
+
 ## Threats
 * Create Threat
 * Add Indicators to Threat
 * Replace Threat Indicators
 * Delete Threat
-## Saved Queries
-* List Saved Queries
-* Get a Saved Query
-* Create Saved Query
-* Replace a Saved Query
-* Update a Saved Query
-* Delete a Saved Query
 
-Happy analyzing!:monocle_face:
+Happy analyzing :monocle_face: and happy administering! :hammer:
 
 # Installation
 InsightIDR4Py is available on [PyPI](https://pypi.org/project/InsightIDR4Py/) and can be installed using:
 ```
 pip install InsightIDR4Py
 ```
 
@@ -141,8 +171,8 @@
 	print("----------")
 ```
 
 # License
 This repository is licensed under an [MIT license](https://github.com/mbabinski/InsightIDR4Py/blob/main/LICENSE), which grants extensive permission to use this material however you wish.
 
 # Contributing
-You are welcome to contribute however you wish! I appreciate feedback in any format.
+You are welcome to contribute however you wish! I appreciate feedback in any format.
```

### Comparing `InsightIDR4Py-0.3/setup.py` & `InsightIDR4Py-0.3.1/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="InsightIDR4Py",
-    version="0.3",
+    version="0.3.1",
     description="A Python client allowing simplified interaction with Rapid7's InsightIDR REST API.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     author="Micah Babinski",
     author_email="m.babinski.88@gmail.com",
     py_modules=["InsightIDR4Py"],
     url="https://github.com/mbabinski/InsightIDR4Py",
-    keywords="Rapid7, InsightIDR, SIEM, Logsearch, Investigations, Threats",
+    keywords="Rapid7, InsightIDR, SIEM, Logsearch, Investigations, Threats, Alerts",
     install_requires=[
           "requests",
       ],
 
 )
```

