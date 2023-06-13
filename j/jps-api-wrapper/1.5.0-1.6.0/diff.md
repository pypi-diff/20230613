# Comparing `tmp/jps_api_wrapper-1.5.0.tar.gz` & `tmp/jps_api_wrapper-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jps_api_wrapper-1.5.0.tar", last modified: Tue Apr 25 16:37:28 2023, max compression
+gzip compressed data, was "jps_api_wrapper-1.6.0.tar", last modified: Tue Jun 13 16:27:06 2023, max compression
```

## Comparing `jps_api_wrapper-1.5.0.tar` & `jps_api_wrapper-1.6.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:37:28.788352 jps_api_wrapper-1.5.0/
--rw-rw-rw-   0 root         (0) root         (0)     1068 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     8112 2023-04-25 16:37:28.788352 jps_api_wrapper-1.5.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     6635 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/README.md
--rw-rw-rw-   0 root         (0) root         (0)      136 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      757 2023-04-25 16:37:28.789352 jps_api_wrapper-1.5.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:37:28.784352 jps_api_wrapper-1.5.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:37:28.786352 jps_api_wrapper-1.5.0/src/jps_api_wrapper/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-25 16:37:01.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)   262861 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper/classic.py
--rw-rw-rw-   0 root         (0) root         (0)   309635 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper/pro.py
--rw-rw-rw-   0 root         (0) root         (0)    13172 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper/request_builder.py
--rw-rw-rw-   0 root         (0) root         (0)     6752 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:37:28.787352 jps_api_wrapper-1.5.0/src/jps_api_wrapper.egg-info/
--rw-r--r--   0 root         (0) root         (0)     8112 2023-04-25 16:37:28.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      454 2023-04-25 16:37:28.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-25 16:37:28.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       30 2023-04-25 16:37:28.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-04-25 16:37:28.000000 jps_api_wrapper-1.5.0/src/jps_api_wrapper.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-25 16:37:28.787352 jps_api_wrapper-1.5.0/tests/
--rw-rw-rw-   0 root         (0) root         (0)   290397 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/tests/test_classic.py
--rw-rw-rw-   0 root         (0) root         (0)   209507 2023-04-25 16:26:12.000000 jps_api_wrapper-1.5.0/tests/test_pro.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:27:06.857386 jps_api_wrapper-1.6.0/
+-rw-rw-rw-   0 root         (0) root         (0)     1068 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     8112 2023-06-13 16:27:06.857386 jps_api_wrapper-1.6.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     6635 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/README.md
+-rw-rw-rw-   0 root         (0) root         (0)      136 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)      757 2023-06-13 16:27:06.858386 jps_api_wrapper-1.6.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:27:06.853386 jps_api_wrapper-1.6.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:27:06.855386 jps_api_wrapper-1.6.0/src/jps_api_wrapper/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-13 16:26:40.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)   262861 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper/classic.py
+-rw-rw-rw-   0 root         (0) root         (0)   312452 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper/pro.py
+-rw-rw-rw-   0 root         (0) root         (0)    13172 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper/request_builder.py
+-rw-rw-rw-   0 root         (0) root         (0)     6752 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:27:06.856386 jps_api_wrapper-1.6.0/src/jps_api_wrapper.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     8112 2023-06-13 16:27:06.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      454 2023-06-13 16:27:06.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-13 16:27:06.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       30 2023-06-13 16:27:06.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-13 16:27:06.000000 jps_api_wrapper-1.6.0/src/jps_api_wrapper.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-13 16:27:06.856386 jps_api_wrapper-1.6.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)   290397 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/tests/test_classic.py
+-rw-rw-rw-   0 root         (0) root         (0)   211163 2023-06-13 16:07:00.000000 jps_api_wrapper-1.6.0/tests/test_pro.py
```

### Comparing `jps_api_wrapper-1.5.0/LICENSE` & `jps_api_wrapper-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.5.0/PKG-INFO` & `jps_api_wrapper-1.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jps_api_wrapper
-Version: 1.5.0
+Version: 1.6.0
 Summary: Jamf Pro Server API Python wrapper
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
```

### Comparing `jps_api_wrapper-1.5.0/README.md` & `jps_api_wrapper-1.6.0/README.md`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.5.0/setup.cfg` & `jps_api_wrapper-1.6.0/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = jps_api_wrapper
-version = 1.5.0
+version = 1.6.0
 description = Jamf Pro Server API Python wrapper
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 readme = README.md
 license = MIT
 classifiers = 
 	License :: OSI Approved :: MIT License
```

### Comparing `jps_api_wrapper-1.5.0/src/jps_api_wrapper/classic.py` & `jps_api_wrapper-1.6.0/src/jps_api_wrapper/classic.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.5.0/src/jps_api_wrapper/pro.py` & `jps_api_wrapper-1.6.0/src/jps_api_wrapper/pro.py`

 * *Files 1% similar despite different names*

```diff
@@ -2056,14 +2056,17 @@
     computer-prestages
     """
 
     def get_computer_prestages(
         self, page: int = None, page_size: int = None, sort: List[str] = ["id:desc"]
     ) -> dict:
         """
+        .. deprecated:: 1.6.0
+            Use :func:`get_computer_prestages_v2` instead.
+
         Returns sorted and paged computer prestages
 
         :param page: Page to return, default page is 0.
         :param page_size: Page size to return, default page-size is 100.
         :param sort:
             Sorting criteria in the format: property:asc/desc. Default sort
             is id:desc. Multiple sort criteria are supported and must
@@ -2080,14 +2083,42 @@
                 "sort": sort,
             }
         )
         endpoint = "/api/v2/computer-prestages"
 
         return self._get(endpoint, params=params)
 
+    def get_computer_prestages_v2(
+        self, page: int = None, page_size: int = None, sort: List[str] = ["id:desc"]
+    ) -> dict:
+        """
+        Returns sorted and paged computer prestages
+
+        :param page: Page to return, default page is 0.
+        :param page_size: Page size to return, default page-size is 100.
+        :param sort:
+            Sorting criteria in the format: property:asc/desc. Default sort
+            is id:desc. Multiple sort criteria are supported and must
+            be separated with a comma.
+
+            Example: ["id:desc", "enrollmentCustomizationId:asc"]
+
+        :returns: All computer prestages in JSON
+        """
+        params = remove_empty_params(
+            {
+                "page": page,
+                "page-size": page_size,
+                "sort": sort,
+            }
+        )
+        endpoint = "/api/v3/computer-prestages"
+
+        return self._get(endpoint, params=params)
+
     def get_computer_prestage_scopes(self) -> dict:
         """
         Returns all device scopes for all computer prestages
 
         :returns: All computer prestage scopes in JSON
         """
         endpoint = "/api/v2/computer-prestages/scope"
@@ -2098,15 +2129,15 @@
         """
         Returns a computer prestage with the supplied ID
 
         :param id: Computer prestage ID
 
         :returns: Computer prestage information in JSON
         """
-        endpoint = f"/api/v2/computer-prestages/{id}"
+        endpoint = f"/api/v3/computer-prestages/{id}"
 
         return self._get(endpoint)
 
     def get_computer_prestage_scope(self, id: Union[int, str]) -> dict:
         """
         Returns device scope for a specified computer prestage by ID
 
@@ -2157,15 +2188,15 @@
             JSON data to update the computer prestage with. For syntax
             information view `Jamf's documentation.
             <https://developer.jamf.com/jamf-pro/reference/put_v2-computer-prestages-id>`__
         :param id: Computer prestage ID
 
         :returns: Updated computer prestage information in JSON
         """
-        endpoint = f"/api/v2/computer-prestages/{id}"
+        endpoint = f"/api/v3/computer-prestages/{id}"
 
         return self._put(endpoint, data)
 
     def replace_computer_prestage_scope(self, data: dict, id: Union[int, str]) -> dict:
         """
         Replaces device scope for a specified computer prestage
 
@@ -2186,15 +2217,15 @@
         Deletes a computer prestage with the supplied ID
 
         :param id: Computer prestage ID
 
         :returns:
             Success message stating that the computer prestage was deleted
         """
-        endpoint = f"/api/v2/computer-prestages/{id}"
+        endpoint = f"/api/v3/computer-prestages/{id}"
 
         return self._delete(
             endpoint, success_message=f"Computer prestage {id} successfully deleted."
         )
 
     def delete_computer_prestage_scope(self, data: dict, id: Union[int, str]) -> dict:
         """
@@ -5088,15 +5119,15 @@
         Updates Local Admin Password auto-deploy feature to be enabled or not.
         When it is enabled (true), all computers will have the
         SetAutoAdminPassword command sent to them automatically.
 
         :param data:
             JSON data to update local admin password settings with. For syntax
             information view `Jamf's documentation.
-            <TODO: Add URL on 10.46 release>`__
+            <https://developer.jamf.com/jamf-pro/reference/put_v2-local-admin-password-settings>`__
 
         :returns: Updated local admin password settings in JSON
         """
         endpoint = "/api/v2/local-admin-password/settings"
 
         return self._put(endpoint, data)
 
@@ -5104,15 +5135,15 @@
         """
         Updates the LAPS password for a device. This will set the password for
         all LAPS capable accounts.
 
         :param data:
             JSON data to update local admin password with. For syntax
             information view `Jamf's documentation.
-            <TODO: Add URL on 10.46 release>`__
+            <https://developer.jamf.com/jamf-pro/reference/put_v2-local-admin-password-clientmanagementid-set-password>`__
         :param clientManagementId: Client management ID of target device
 
         :returns: Information on the updated account in JSON
         """
         endpoint = f"/api/v2/local-admin-password/{clientManagementId}/set-password"
 
         return self._put(endpoint, data)
@@ -6166,24 +6197,62 @@
             failed. This param can be combined with paging and sorting.
 
             Example: 'policyName=="Example name"'
 
         :returns: All patch policies information in JSON
         """
         params = remove_empty_params(
-            {
-                "page": page,
-                "page-size": page_size,
-                "sort": sort,
-            }
+            {"page": page, "page-size": page_size, "sort": sort, "filter": filter}
         )
         endpoint = "/api/v2/patch-policies"
 
         return self._get(endpoint, params=params)
 
+    def get_patch_policies_policy_details(
+        self,
+        page: int = None,
+        page_size: int = None,
+        sort: List[str] = None,
+        filter: str = None,
+    ):
+        """
+        Returns policy details on all patch policies
+
+        :param page: Page to return, default page is 0.
+        :param page_size: Page size to return, default page-size is 100.
+        :param sort:
+            Sorting criteria in the format: property:asc/desc. Default sort is
+            ["id:asc"]. Multiple sort criteria are supported and must be
+            separated with a comma.
+
+            Example: ["id:desc", "name:asc"]
+
+        :param filter:
+            Query in the RSQL format, allowing to filter Patch Policy
+            collection. Default filter is empty query - returning all results
+            for the requested page. Fields allowed in the query: id, name,
+            enabled, targetPatchVersion, deploymentMethod, softwareTitleId,
+            softwareTitleConfigurationId, killAppsDelayMinutes,
+            killAppsMessage, isDowngrade, isPatchUnknownVersion,
+            notificationHeader, selfServiceEnforceDeadline,
+            selfServiceDeadline, installButtonText, selfServiceDescription,
+            iconId, reminderFrequency, reminderEnabled. This param can be
+            combined with paging and sorting.
+
+            Example: 'name == "Example Name"'
+
+        :returns: Policy details for all patch policies in JSON
+        """
+        params = remove_empty_params(
+            {"page": page, "page-size": page_size, "sort": sort, "filter": filter}
+        )
+        endpoint = "/api/v2/patch-policies/policy-details"
+
+        return self._get(endpoint, params=params)
+
     def get_patch_policy_dashboard_v2(self, id: Union[int, str]) -> dict:
         """
         Returns whether or not the requested patch policy is on the dashboard
         by ID
 
         :param id: Patch policy ID
```

### Comparing `jps_api_wrapper-1.5.0/src/jps_api_wrapper/request_builder.py` & `jps_api_wrapper-1.6.0/src/jps_api_wrapper/request_builder.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.5.0/src/jps_api_wrapper/utils.py` & `jps_api_wrapper-1.6.0/src/jps_api_wrapper/utils.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.5.0/src/jps_api_wrapper.egg-info/PKG-INFO` & `jps_api_wrapper-1.6.0/src/jps_api_wrapper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jps-api-wrapper
-Version: 1.5.0
+Version: 1.6.0
 Summary: Jamf Pro Server API Python wrapper
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.6
```

### Comparing `jps_api_wrapper-1.5.0/tests/test_classic.py` & `jps_api_wrapper-1.6.0/tests/test_classic.py`

 * *Files identical despite different names*

### Comparing `jps_api_wrapper-1.5.0/tests/test_pro.py` & `jps_api_wrapper-1.6.0/tests/test_pro.py`

 * *Files 0% similar despite different names*

```diff
@@ -1622,29 +1622,54 @@
     assert (
         pro.get_computer_prestages(0, 100, ["id:desc", "enrollmentCustomizationId:asc"])
         == EXPECTED_JSON
     )
 
 
 @responses.activate
+def test_get_computer_prestages_v2(pro):
+    """
+    Ensures that get_computer_prestages_v2 returns JSON when used with no
+    optional params
+    """
+    responses.add(response_builder("GET", jps_url("/api/v3/computer-prestages")))
+    assert pro.get_computer_prestages_v2() == EXPECTED_JSON
+
+
+@responses.activate
+def test_get_computer_prestages_v2_optional_params(pro):
+    """
+    Ensure that get_computer_prestages_v2 returns JSON when used with all
+    optional params
+    """
+    responses.add(response_builder("GET", jps_url("/api/v3/computer-prestages")))
+    assert (
+        pro.get_computer_prestages_v2(
+            0, 100, ["id:desc", "enrollmentCustomizationId:asc"]
+        )
+        == EXPECTED_JSON
+    )
+
+
+@responses.activate
 def test_get_computer_prestage_scopes(pro):
     """
     Ensures that get_computer_prestage_scopes returns JSON when used
     """
     responses.add(response_builder("GET", jps_url("/api/v2/computer-prestages/scope")))
     assert pro.get_computer_prestage_scopes() == EXPECTED_JSON
 
 
 @responses.activate
 def test_get_computer_prestage(pro):
     """
     Ensures that get_computer_prestage returns JSON when used with required
     params
     """
-    responses.add(response_builder("GET", jps_url("/api/v2/computer-prestages/1001")))
+    responses.add(response_builder("GET", jps_url("/api/v3/computer-prestages/1001")))
     assert pro.get_computer_prestage(1001) == EXPECTED_JSON
 
 
 @responses.activate
 def test_get_computer_prestage_scope(pro):
     """
     Ensures that get_computer_prestage_scope returns JSON when used with
@@ -1680,15 +1705,15 @@
 
 @responses.activate
 def test_update_computer_prestage(pro):
     """
     Ensures that update_computer_prestage returns JSON when completed
     successfully with required params
     """
-    responses.add(response_builder("PUT", jps_url("/api/v2/computer-prestages/1001")))
+    responses.add(response_builder("PUT", jps_url("/api/v3/computer-prestages/1001")))
     assert pro.update_computer_prestage(EXPECTED_JSON, 1001) == EXPECTED_JSON
 
 
 @responses.activate
 def test_replace_computer_prestage_scope(pro):
     """
     Ensures that replace_computer_prestage_scope returns JSON when completed
@@ -1703,15 +1728,15 @@
 @responses.activate
 def test_delete_computer_prestage(pro):
     """
     Ensures that delete_computer_prestage returns a success message str when
     used with required params
     """
     responses.add(
-        response_builder("DELETE", jps_url("/api/v2/computer-prestages/1001"))
+        response_builder("DELETE", jps_url("/api/v3/computer-prestages/1001"))
     )
     assert (
         pro.delete_computer_prestage(1001)
         == "Computer prestage 1001 successfully deleted."
     )
 
 
@@ -4900,15 +4925,46 @@
 @responses.activate
 def test_get_patch_policies_optional_params(pro):
     """
     Ensures that get_patch_policies returns JSON when used with all optional
     params
     """
     responses.add(response_builder("GET", jps_url("/api/v2/patch-policies")))
-    assert pro.get_patch_policies() == EXPECTED_JSON
+    assert (
+        pro.get_patch_policies(
+            0, 100, ["policyName:asc", "id:desc"], 'policyName=="Example name"'
+        )
+        == EXPECTED_JSON
+    )
+
+
+@responses.activate
+def test_get_patch_policies_policy_details(pro):
+    """
+    Ensures that get_patch_policies_policy_details returns JSON when used
+    without optional params
+    """
+    responses.add(
+        response_builder("GET", jps_url("/api/v2/patch-policies/policy-details"))
+    )
+    assert pro.get_patch_policies_policy_details() == EXPECTED_JSON
+
+
+@responses.activate
+def test_get_patch_policies_policy_details_optional_params(pro):
+    """
+    Ensures that get_patch_policies_policy_details returns JSON when used with
+    all optional params
+    """
+    responses.add(
+        response_builder("GET", jps_url("/api/v2/patch-policies/policy-details"))
+    )
+    assert pro.get_patch_policies_policy_details(
+        0, 100, ["id:desc", "name:asc"], 'name == "Example Name"'
+    )
 
 
 @responses.activate
 def test_get_patch_policy_dashboard_v2(pro):
     """
     Ensures that get_patch_policy_dashboard_v2 returns JSON when used with
     required params
```

