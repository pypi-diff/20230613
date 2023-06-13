# Comparing `tmp/lifeguard-k8s-1.1.0.tar.gz` & `tmp/lifeguard-k8s-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lifeguard-k8s-1.1.0.tar", last modified: Wed Jun  7 19:45:55 2023, max compression
+gzip compressed data, was "lifeguard-k8s-1.2.0.tar", last modified: Tue Jun 13 19:10:47 2023, max compression
```

## Comparing `lifeguard-k8s-1.1.0.tar` & `lifeguard-k8s-1.2.0.tar`

### file list

```diff
@@ -1,30 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.801562 lifeguard-k8s-1.1.0/lifeguard_k8s/
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/lifeguard_k8s/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/lifeguard_k8s/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/lifeguard_k8s/actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/lifeguard_k8s/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/lifeguard_k8s/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2289 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/lifeguard_k8s/infrastructure/pods.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/lifeguard_k8s/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/lifeguard_k8s/validations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/lifeguard_k8s/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/lifeguard_k8s/validations/pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/lifeguard_k8s.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-07 19:45:55.000000 lifeguard-k8s-1.1.0/lifeguard_k8s.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-07 19:45:55.000000 lifeguard-k8s-1.1.0/lifeguard_k8s.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-07 19:45:55.000000 lifeguard-k8s-1.1.0/lifeguard_k8s.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-07 19:45:55.000000 lifeguard-k8s-1.1.0/lifeguard_k8s.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-07 19:45:55.000000 lifeguard-k8s-1.1.0/lifeguard_k8s.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/tests/infrastructure/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/tests/infrastructure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/tests/infrastructure/test_pods.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:55.805562 lifeguard-k8s-1.1.0/tests/validations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/tests/validations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-07 19:45:28.000000 lifeguard-k8s-1.1.0/tests/validations/test_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.995016 lifeguard-k8s-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-13 19:10:47.995016 lifeguard-k8s-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.991016 lifeguard-k8s-1.2.0/lifeguard_k8s/
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.991016 lifeguard-k8s-1.2.0/lifeguard_k8s/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/actions/pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.991016 lifeguard-k8s-1.2.0/lifeguard_k8s/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/infrastructure/pods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.991016 lifeguard-k8s-1.2.0/lifeguard_k8s/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/lifeguard_k8s/validations/pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.991016 lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2154 2023-06-13 19:10:47.000000 lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-06-13 19:10:47.000000 lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 19:10:47.000000 lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-06-13 19:10:47.000000 lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 19:10:47.000000 lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 19:10:47.995016 lifeguard-k8s-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.991016 lifeguard-k8s-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.995016 lifeguard-k8s-1.2.0/tests/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/tests/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/tests/actions/test_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.995016 lifeguard-k8s-1.2.0/tests/infrastructure/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/tests/infrastructure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8037 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/tests/infrastructure/test_pods.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:47.995016 lifeguard-k8s-1.2.0/tests/validations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/tests/validations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4155 2023-06-13 19:10:19.000000 lifeguard-k8s-1.2.0/tests/validations/test_pods.py
```

### Comparing `lifeguard-k8s-1.1.0/lifeguard_k8s/infrastructure/pods.py` & `lifeguard-k8s-1.2.0/lifeguard_k8s/infrastructure/pods.py`

 * *Files 15% similar despite different names*

```diff
@@ -48,14 +48,19 @@
                     not_running_pods.append(pod.metadata.name)
             else:
                 not_running_pods.append(pod.metadata.name)
 
     return not_running_pods
 
 
+def delete_a_pod(namespace, pod_name):
+    v1 = _get_clients()
+    v1.delete_namespaced_pod(pod_name, namespace)
+
+
 def get_events_from_pod(namespace, pod_name):
     v1 = _get_clients()
     events = v1.list_namespaced_event(
         namespace, field_selector=f"involvedObject.name={pod_name}"
     )
     return [
         {"event_type": item.type, "message": item.message, "reason": item.reason}
```

### Comparing `lifeguard-k8s-1.1.0/lifeguard_k8s/settings.py` & `lifeguard-k8s-1.2.0/lifeguard_k8s/settings.py`

 * *Files identical despite different names*

### Comparing `lifeguard-k8s-1.1.0/lifeguard_k8s/validations/pods.py` & `lifeguard-k8s-1.2.0/lifeguard_k8s/validations/pods.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     else:
         details["traceback"].append(None)
 
 
 def pods_validation(namespace):
     status = NORMAL
 
-    details = {"pods": [], "traceback": []}
+    details = {"pods": [], "traceback": [], "namespace": namespace}
 
     if namespace not in IN_REVIEW:
         IN_REVIEW[namespace] = []
 
     pods = get_not_running_pods(namespace)
     if pods:
         for pod in pods:
```

### Comparing `lifeguard-k8s-1.1.0/lifeguard_k8s.egg-info/SOURCES.txt` & `lifeguard-k8s-1.2.0/lifeguard_k8s.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -4,16 +4,19 @@
 lifeguard_k8s/settings.py
 lifeguard_k8s.egg-info/PKG-INFO
 lifeguard_k8s.egg-info/SOURCES.txt
 lifeguard_k8s.egg-info/dependency_links.txt
 lifeguard_k8s.egg-info/requires.txt
 lifeguard_k8s.egg-info/top_level.txt
 lifeguard_k8s/actions/__init__.py
+lifeguard_k8s/actions/pods.py
 lifeguard_k8s/infrastructure/__init__.py
 lifeguard_k8s/infrastructure/pods.py
 lifeguard_k8s/validations/__init__.py
 lifeguard_k8s/validations/pods.py
 tests/__init__.py
+tests/actions/__init__.py
+tests/actions/test_pods.py
 tests/infrastructure/__init__.py
 tests/infrastructure/test_pods.py
 tests/validations/__init__.py
 tests/validations/test_pods.py
```

### Comparing `lifeguard-k8s-1.1.0/setup.py` & `lifeguard-k8s-1.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="lifeguard-k8s",
-    version="1.1.0",
+    version="1.2.0",
     url="https://github.com/LifeguardSystem/lifeguard-k8s",
     author="Diego Rubin",
     author_email="contact@diegorubin.dev",
     license="GPL2",
     scripts=[],
     include_package_data=True,
     description="Lifeguard integration with Kubernetes",
```

### Comparing `lifeguard-k8s-1.1.0/tests/infrastructure/test_pods.py` & `lifeguard-k8s-1.2.0/tests/infrastructure/test_pods.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 from unittest.mock import patch, MagicMock
 
 from lifeguard_k8s.infrastructure.pods import (
     get_not_running_pods,
     get_events_from_pod,
     get_last_error_event_from_pod,
     get_logs_from_pod,
+    delete_a_pod,
 )
 
 
 def build_pod(status, container_status, pod_name, kind="ReplicaSet"):
     container_statuses = MagicMock(name="container_statuses")
     container_statuses.ready = container_status
 
@@ -197,7 +198,17 @@
         "lifeguard_k8s.infrastructure.pods.LIFEGUARD_KUBERNETES_READ_LOG_MAX_SIZE", 10
     )
     def test_get_logs_from_pod_with_limited_size(self, mock_client, mock_config):
         mock_client.CoreV1Api.return_value.read_namespaced_pod_log.return_value = """
 a big log that will be limited
 send only last 10 characters"""
         self.assertEqual(get_logs_from_pod("namespace", "pod_name"), "characters")
+
+    @patch("lifeguard_k8s.infrastructure.pods.config")
+    @patch("lifeguard_k8s.infrastructure.pods.client")
+    def test_delete_a_pod(self, mock_client, mock_config):
+        mock_client.CoreV1Api.return_value.delete_namespaced_pod.return_value = None
+        delete_a_pod("namespace", "pod_name")
+
+        mock_client.CoreV1Api.return_value.delete_namespaced_pod.assert_called_with(
+            "pod_name", "namespace"
+        )
```

### Comparing `lifeguard-k8s-1.1.0/tests/validations/test_pods.py` & `lifeguard-k8s-1.2.0/tests/validations/test_pods.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,25 +11,29 @@
     def test_normal_response(self, mock_get_not_running_pods):
         mock_get_not_running_pods.return_value = []
 
         response = pods_validation("namespace")
 
         mock_get_not_running_pods.assert_called_with("namespace")
         self.assertEqual(response.status, NORMAL)
-        self.assertEqual(response.details, {"pods": [], "traceback": []})
+        self.assertEqual(
+            response.details, {"pods": [], "traceback": [], "namespace": "namespace"}
+        )
         self.assertEqual(response.settings, None)
 
     @patch("lifeguard_k8s.validations.pods.get_not_running_pods")
     def test_normal_response_on_first_error(self, mock_get_not_running_pods):
         mock_get_not_running_pods.return_value = ["pod"]
 
         response = pods_validation("namespace")
 
         self.assertEqual(response.status, NORMAL)
-        self.assertEqual(response.details, {"pods": [], "traceback": []})
+        self.assertEqual(
+            response.details, {"pods": [], "traceback": [], "namespace": "namespace"}
+        )
         self.assertEqual(response.settings, None)
 
     @patch("lifeguard_k8s.validations.pods.IN_REVIEW", {"namespace": ["pod"]})
     @patch("lifeguard_k8s.validations.pods.get_not_running_pods")
     @patch("lifeguard_k8s.validations.pods.get_last_error_event_from_pod")
     def test_error_response_on_second_error(
         self, mock_last_error_event_from_pod, mock_get_not_running_pods
@@ -37,15 +41,16 @@
         mock_get_not_running_pods.return_value = ["pod"]
         mock_last_error_event_from_pod.return_value = {"message": "error message"}
 
         response = pods_validation("namespace")
 
         self.assertEqual(response.status, PROBLEM)
         self.assertEqual(
-            response.details, {"pods": ["pod"], "traceback": ["error message"]}
+            response.details,
+            {"pods": ["pod"], "traceback": ["error message"], "namespace": "namespace"},
         )
 
     @patch("lifeguard_k8s.validations.pods.IN_REVIEW", {"namespace": ["pod"]})
     @patch("lifeguard_k8s.validations.pods.get_not_running_pods")
     @patch("lifeguard_k8s.validations.pods.get_last_error_event_from_pod")
     @patch("lifeguard_k8s.validations.pods.get_logs_from_pod")
     def test_error_response_on_second_error_with_log_usage(
@@ -60,29 +65,35 @@
         }
 
         mock_get_logs_from_pod.return_value = "log"
 
         response = pods_validation("namespace")
 
         self.assertEqual(response.status, PROBLEM)
-        self.assertEqual(response.details, {"pods": ["pod"], "traceback": ["log"]})
+        self.assertEqual(
+            response.details,
+            {"pods": ["pod"], "traceback": ["log"], "namespace": "namespace"},
+        )
 
     @patch("lifeguard_k8s.validations.pods.IN_REVIEW", {"namespace": ["pod"]})
     @patch("lifeguard_k8s.validations.pods.get_not_running_pods")
     @patch("lifeguard_k8s.validations.pods.get_last_error_event_from_pod")
     def test_error_response_on_second_error_without_traceback(
         self, mock_last_error_event_from_pod, mock_get_not_running_pods
     ):
         mock_get_not_running_pods.return_value = ["pod"]
         mock_last_error_event_from_pod.return_value = None
 
         response = pods_validation("namespace")
 
         self.assertEqual(response.status, PROBLEM)
-        self.assertEqual(response.details, {"pods": ["pod"], "traceback": [None]})
+        self.assertEqual(
+            response.details,
+            {"pods": ["pod"], "traceback": [None], "namespace": "namespace"},
+        )
         self.assertEqual(response.settings, None)
 
     @patch("lifeguard_k8s.validations.pods.IN_REVIEW", {"namespace": ["pod"]})
     @patch("lifeguard_k8s.validations.pods.get_not_running_pods")
     def test_normal_on_first_error_after_normalized(self, mock_get_not_running_pods):
         mock_get_not_running_pods.return_value = []
```

