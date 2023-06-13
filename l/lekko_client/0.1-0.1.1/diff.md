# Comparing `tmp/lekko_client-0.1.tar.gz` & `tmp/lekko_client-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lekko_client-0.1.tar", last modified: Wed May  3 23:31:42 2023, max compression
+gzip compressed data, was "lekko_client-0.1.1.tar", last modified: Tue Jun 13 19:53:15 2023, max compression
```

## Comparing `lekko_client-0.1.tar` & `lekko_client-0.1.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1127 2023-05-03 23:03:04.216499 lekko_client-0.1/.github/workflows/ci.yaml
--rw-r--r--   0        0        0     3078 2023-04-21 20:20:24.420901 lekko_client-0.1/.gitignore
--rw-r--r--   0        0        0    11357 2023-04-21 20:20:24.421086 lekko_client-0.1/LICENSE
--rw-r--r--   0        0        0      607 2023-05-03 23:03:04.216872 lekko_client-0.1/Makefile
--rw-r--r--   0        0        0       12 2023-04-21 20:20:24.421180 lekko_client-0.1/README.md
--rw-r--r--   0        0        0      233 2023-05-03 18:55:48.352789 lekko_client-0.1/buf.gen.yaml
--rw-r--r--   0        0        0     2297 2023-05-03 18:55:48.353119 lekko_client-0.1/example.py
--rw-r--r--   0        0        0      243 2023-05-03 18:55:48.353448 lekko_client-0.1/lekko_client/__init__.py
--rw-r--r--   0        0        0     7353 2023-05-03 22:29:42.588741 lekko_client-0.1/lekko_client/client.py
--rw-r--r--   0        0        0      279 2023-05-03 18:55:48.354020 lekko_client-0.1/lekko_client/exceptions.py
--rw-r--r--   0        0        0     9857 2023-05-03 21:16:43.938055 lekko_client-0.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.py
--rw-r--r--   0        0        0    18544 2023-05-03 20:42:34.599769 lekko_client-0.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.pyi
--rw-r--r--   0        0        0    16283 2023-05-03 21:16:43.938327 lekko_client-0.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2_grpc.py
--rw-r--r--   0        0        0     1753 2023-05-03 18:55:48.354697 lekko_client-0.1/lekko_client/helpers.py
--rw-r--r--   0        0        0      770 2023-05-03 23:09:29.307949 lekko_client-0.1/pyproject.toml
--rw-r--r--   0        0        0       61 2023-04-26 23:47:06.221249 lekko_client-0.1/requirements.txt
--rw-r--r--   0        0        0     2086 2023-05-03 21:16:43.938569 lekko_client-0.1/tests/conftest.py
--rw-r--r--   0        0        0     1888 2023-05-03 18:55:48.355229 lekko_client-0.1/tests/mock_server.py
--rw-r--r--   0        0        0       40 2023-05-03 18:55:48.355400 lekko_client-0.1/tests/requirements.txt
--rw-r--r--   0        0        0     2398 2023-05-03 21:16:43.938766 lekko_client-0.1/tests/test_client.py
--rw-r--r--   0        0        0      913 2023-05-03 23:03:04.217147 lekko_client-0.1/tox.ini
--rw-r--r--   0        0        0      542 1970-01-01 00:00:00.000000 lekko_client-0.1/PKG-INFO
+-rw-r--r--   0        0        0     1127 2023-05-03 23:03:04.216499 lekko_client-0.1.1/.github/workflows/ci.yaml
+-rw-r--r--   0        0        0     3078 2023-04-21 20:20:24.420901 lekko_client-0.1.1/.gitignore
+-rw-r--r--   0        0        0    11357 2023-04-21 20:20:24.421086 lekko_client-0.1.1/LICENSE
+-rw-r--r--   0        0        0      607 2023-05-03 23:03:04.216872 lekko_client-0.1.1/Makefile
+-rw-r--r--   0        0        0       12 2023-04-21 20:20:24.421180 lekko_client-0.1.1/README.md
+-rw-r--r--   0        0        0      233 2023-05-03 18:55:48.352789 lekko_client-0.1.1/buf.gen.yaml
+-rw-r--r--   0        0        0     2368 2023-05-28 18:43:00.488488 lekko_client-0.1.1/example.py
+-rw-r--r--   0        0        0      245 2023-06-13 19:52:16.322836 lekko_client-0.1.1/lekko_client/__init__.py
+-rw-r--r--   0        0        0     7353 2023-05-03 22:29:42.588741 lekko_client-0.1.1/lekko_client/client.py
+-rw-r--r--   0        0        0      279 2023-05-03 18:55:48.354020 lekko_client-0.1.1/lekko_client/exceptions.py
+-rw-r--r--   0        0        0     9857 2023-05-03 21:16:43.938055 lekko_client-0.1.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.py
+-rw-r--r--   0        0        0    18544 2023-05-03 20:42:34.599769 lekko_client-0.1.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.pyi
+-rw-r--r--   0        0        0    16283 2023-05-03 21:16:43.938327 lekko_client-0.1.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2_grpc.py
+-rw-r--r--   0        0        0     1761 2023-05-31 18:07:52.219437 lekko_client-0.1.1/lekko_client/helpers.py
+-rw-r--r--   0        0        0      753 2023-05-28 18:42:56.475381 lekko_client-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       61 2023-04-26 23:47:06.221249 lekko_client-0.1.1/requirements.txt
+-rw-r--r--   0        0        0     2086 2023-05-28 18:50:58.132098 lekko_client-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0     1888 2023-05-03 18:55:48.355229 lekko_client-0.1.1/tests/mock_server.py
+-rw-r--r--   0        0        0       40 2023-05-03 18:55:48.355400 lekko_client-0.1.1/tests/requirements.txt
+-rw-r--r--   0        0        0     2456 2023-05-31 18:07:52.219638 lekko_client-0.1.1/tests/test_client.py
+-rw-r--r--   0        0        0      913 2023-05-03 23:03:04.217147 lekko_client-0.1.1/tox.ini
+-rw-r--r--   0        0        0      500 1970-01-01 00:00:00.000000 lekko_client-0.1.1/PKG-INFO
```

### Comparing `lekko_client-0.1/.github/workflows/ci.yaml` & `lekko_client-0.1.1/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1/.gitignore` & `lekko_client-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1/LICENSE` & `lekko_client-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1/Makefile` & `lekko_client-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1/example.py` & `lekko_client-0.1.1/example.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 
 if __name__ == "__main__":
     parser = argparse.ArgumentParser()
     parser.add_argument("--apikey", type=str)
     parser.add_argument("--sidecar", action="store_true")
     parser.add_argument("--owner", type=str)
     parser.add_argument("--repo", type=str)
-    parser.add_argument("--namespace", type=str)
-    parser.add_argument("--feature", type=str)
+    parser.add_argument("--namespace", type=str, default="default")
+    parser.add_argument("--feature", type=str, default="example")
     parser.add_argument(
         "--feature-type",
         type=str,
         choices=["bool", "int", "float", "str", "json", "proto"],
-        default="str",
+        default="bool",
     )
     parser.add_argument("--proto-type", type=str, default="")
     parser.add_argument("--proto-file", type=str)
     args = parser.parse_args()
 
     client_cls = SidecarClient if args.sidecar else APIClient
     client = client_cls(args.owner, args.repo, args.namespace, api_key=args.apikey)
@@ -48,12 +48,12 @@
                 imported_proto = grpc.protos(args.proto_file)
 
                 if args.proto_type:
                     msg_type = getattr(imported_proto, args.proto_type)
                     val = MessageToDict(client.get_proto_by_type(args.feature, {}, msg_type))
                 else:
                     val = MessageToDict(client.get_proto(args.feature, {}))
-        print(f"Got {val} for feature")
+        print(f"Got {val} for feature {args.namespace}/{args.feature}")
     except LekkoError as e:
         print(f"Failed to get feature: {e}")
         if e.__cause__:
             print(f"Caused by: {e.__cause__}")
```

### Comparing `lekko_client-0.1/lekko_client/client.py` & `lekko_client-0.1.1/lekko_client/client.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.py` & `lekko_client-0.1.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.pyi` & `lekko_client-0.1.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2.pyi`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2_grpc.py` & `lekko_client-0.1.1/lekko_client/gen/lekko/client/v1beta1/configuration_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1/lekko_client/helpers.py` & `lekko_client-0.1.1/lekko_client/helpers.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         elif isinstance(val, int):
             return Value(int_value=val)
         elif isinstance(val, float):
             return Value(double_value=val)
         else:
             return Value(string_value=str(val))
 
-    return {k: convert_value(v) for k, v in context}
+    return {k: convert_value(v) for k, v in context.items()}
 
 
 class ApiKeyInterceptor(ClientInterceptor):
     """A test interceptor that injects invocation metadata."""
 
     def __init__(self, api_key):
         self.api_key = api_key
```

### Comparing `lekko_client-0.1/pyproject.toml` & `lekko_client-0.1.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -15,15 +15,14 @@
   'grpcio-tools ~= 1.32',
   'grpc-interceptor ~= 0.15',
 ]
 
 [project.optional-dependencies]
 dev = [
   'tox ~= 4.5',
-  'flit ~= 3.8',
 ]
 
 [project.urls]
 Home = "https://github.com/lekkodev/python-sdk"
 
 [tool.ruff]
 extend-exclude = ["gen"]
```

### Comparing `lekko_client-0.1/tests/conftest.py` & `lekko_client-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1/tests/mock_server.py` & `lekko_client-0.1.1/tests/mock_server.py`

 * *Files identical despite different names*

### Comparing `lekko_client-0.1/tests/test_client.py` & `lekko_client-0.1.1/tests/test_client.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,56 +9,56 @@
         test_server.MockRequestResponse("Register", messages.RegisterResponse),
         test_server.MockRequestResponse("GetBoolValue", messages.GetBoolValueResponse(value=True)),
     ]
 
     test_server.mock_async_responses(requests)
 
     client = SidecarClient("owner", "repo", "namespace", "lekko_apikey123")
-    resp = client.get_bool("val", {})
+    resp = client.get_bool("val", {"context": True})
 
     assert resp is True
 
 
 def test_get_int(test_server):
     requests = [
         test_server.MockRequestResponse("Register", messages.RegisterResponse),
         test_server.MockRequestResponse("GetIntValue", messages.GetIntValueResponse(value=10)),
     ]
 
     test_server.mock_async_responses(requests)
 
     client = SidecarClient("owner", "repo", "namespace", "lekko_apikey123")
-    resp = client.get_int("val", {})
+    resp = client.get_int("val", {"context": 5})
 
     assert resp == 10
 
 
 def test_get_float(test_server):
     requests = [
         test_server.MockRequestResponse("Register", messages.RegisterResponse),
         test_server.MockRequestResponse("GetFloatValue", messages.GetFloatValueResponse(value=1.5)),
     ]
 
     test_server.mock_async_responses(requests)
 
     client = SidecarClient("owner", "repo", "namespace", "lekko_apikey123")
-    resp = client.get_float("val", {})
+    resp = client.get_float("val", {"context": 2.5})
 
     assert resp == 1.5
 
 
 def test_get_string(test_server):
     requests = [
         test_server.MockRequestResponse("Register", messages.RegisterResponse),
         test_server.MockRequestResponse("GetStringValue", messages.GetStringValueResponse(value="feature value")),
     ]
     test_server.mock_async_responses(requests)
 
     client = SidecarClient("owner", "repo", "namespace", "lekko_apikey123")
-    resp = client.get_string("val", {})
+    resp = client.get_string("val", {"conext": "hello"})
 
     assert resp == "feature value"
 
 
 def test_get_json(test_server):
     expected = {"key": "value", "int_key": 1}
     requests = [
```

### Comparing `lekko_client-0.1/tox.ini` & `lekko_client-0.1.1/tox.ini`

 * *Files identical despite different names*

