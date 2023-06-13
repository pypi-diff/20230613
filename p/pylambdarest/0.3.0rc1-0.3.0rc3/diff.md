# Comparing `tmp/pylambdarest-0.3.0rc1.tar.gz` & `tmp/pylambdarest-0.3.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pylambdarest-0.3.0rc1.tar", max compression
+gzip compressed data, was "pylambdarest-0.3.0rc3.tar", max compression
```

## Comparing `pylambdarest-0.3.0rc1.tar` & `pylambdarest-0.3.0rc3.tar`

### file list

```diff
@@ -1,10 +1,9 @@
--rw-r--r--   0        0        0     1072 2022-11-01 22:04:54.964182 pylambdarest-0.3.0rc1/LICENSE
--rw-r--r--   0        0        0     6093 2022-11-01 22:04:54.964182 pylambdarest-0.3.0rc1/README.md
--rw-r--r--   0        0        0      182 2022-11-01 22:04:54.968182 pylambdarest-0.3.0rc1/pylambdarest/__init__.py
--rw-r--r--   0        0        0     8634 2022-11-01 22:04:54.968182 pylambdarest-0.3.0rc1/pylambdarest/applications.py
--rw-r--r--   0        0        0     1794 2022-11-01 22:04:54.968182 pylambdarest-0.3.0rc1/pylambdarest/config.py
--rw-r--r--   0        0        0      257 2022-11-01 22:04:54.968182 pylambdarest-0.3.0rc1/pylambdarest/exceptions.py
--rw-r--r--   0        0        0     2870 2022-11-01 22:04:54.968182 pylambdarest-0.3.0rc1/pylambdarest/request.py
--rw-r--r--   0        0        0     1364 2022-11-01 22:04:54.968182 pylambdarest-0.3.0rc1/pyproject.toml
--rw-r--r--   0        0        0     7090 1970-01-01 00:00:00.000000 pylambdarest-0.3.0rc1/setup.py
--rw-r--r--   0        0        0     7131 1970-01-01 00:00:00.000000 pylambdarest-0.3.0rc1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/LICENSE
+-rw-r--r--   0        0        0     6093 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/README.md
+-rw-r--r--   0        0        0      182 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/pylambdarest/__init__.py
+-rw-r--r--   0        0        0     8723 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/pylambdarest/applications.py
+-rw-r--r--   0        0        0     2043 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/pylambdarest/config.py
+-rw-r--r--   0        0        0      257 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/pylambdarest/exceptions.py
+-rw-r--r--   0        0        0     2870 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/pylambdarest/request.py
+-rw-r--r--   0        0        0     1364 2023-06-13 12:59:05.884157 pylambdarest-0.3.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     7083 1970-01-01 00:00:00.000000 pylambdarest-0.3.0rc3/PKG-INFO
```

### Comparing `pylambdarest-0.3.0rc1/LICENSE` & `pylambdarest-0.3.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `pylambdarest-0.3.0rc1/README.md` & `pylambdarest-0.3.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `pylambdarest-0.3.0rc1/pylambdarest/applications.py` & `pylambdarest-0.3.0rc3/pylambdarest/applications.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,16 @@
         response: Dict[str, Any] = {"statusCode": code}
 
         if body is not None:
             response["body"] = json.dumps(body)
 
         if self.config.ALLOW_CORS:
             response["headers"] = {
-                "Access-Control-Allow-Origin": self.config.CORS_ORIGIN
+                "Access-Control-Allow-Origin": self.config.CORS_ORIGIN,
+                "Access-Control-Allow-Credentials": self.config.CORS_ALLOW_CREDENTIALS,
             }
 
         if headers is not None:
             response["headers"] = {**response.get("headers", {}), **headers}
 
         return response
```

### Comparing `pylambdarest-0.3.0rc1/pylambdarest/request.py` & `pylambdarest-0.3.0rc3/pylambdarest/request.py`

 * *Files identical despite different names*

### Comparing `pylambdarest-0.3.0rc1/pyproject.toml` & `pylambdarest-0.3.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pylambdarest"
-version = "0.3.0rc1"
+version = "0.3.0rc3"
 license = "MIT"
 description = "Lightweight framework for building REST API using AWS Lambda + API Gateway"
 authors = ["Marwan Debbiche (Macbook Pro) <marwan.debbiche@gmail.com>"]
 homepage = "https://github.com/MarwanDebbiche/pylambdarest"
 repository = "https://github.com/MarwanDebbiche/pylambdarest"
 documentation = "https://pylambdarest.readthedocs.io"
 readme = "README.md"
```

### Comparing `pylambdarest-0.3.0rc1/setup.py` & `pylambdarest-0.3.0rc3/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,30 +1,235 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pylambdarest
+Version: 0.3.0rc3
+Summary: Lightweight framework for building REST API using AWS Lambda + API Gateway
+Home-page: https://github.com/MarwanDebbiche/pylambdarest
+License: MIT
+Keywords: aws-lambda,serverless,api-gateway,rest-api
+Author: Marwan Debbiche (Macbook Pro)
+Author-email: marwan.debbiche@gmail.com
+Requires-Python: >=3.7.2,<4.0.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: jsonschema (>=3.2.0,<4.0.0)
+Requires-Dist: simplejson (>=3.17.2,<4.0.0)
+Project-URL: Documentation, https://pylambdarest.readthedocs.io
+Project-URL: Repository, https://github.com/MarwanDebbiche/pylambdarest
+Description-Content-Type: text/markdown
 
-packages = \
-['pylambdarest']
+# pylambdarest
 
-package_data = \
-{'': ['*']}
+[![CI/CD Status](https://github.com/MarwanDebbiche/pylambdarest/workflows/CI%2FCD/badge.svg?branch=master)](https://github.com/MarwanDebbiche/pylambdarest/actions?query=branch:master)
+[![Coverage Status](https://coveralls.io/repos/github/MarwanDebbiche/pylambdarest/badge.svg?branch=master)](https://coveralls.io/github/MarwanDebbiche/pylambdarest?branch=master)
+[![Latest Version](https://img.shields.io/pypi/v/pylambdarest.svg?color=blue)](https://pypi.python.org/pypi/pylambdarest)
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/pylambdarest?label=pypi%20downloads)](https://pypi.org/project/pylambdarest/)
+![License](https://img.shields.io/github/license/MarwanDebbiche/pylambdarest)
 
-install_requires = \
-['jsonschema>=3.2.0,<4.0.0', 'simplejson>=3.17.2,<4.0.0']
-
-setup_kwargs = {
-    'name': 'pylambdarest',
-    'version': '0.3.0rc1',
-    'description': 'Lightweight framework for building REST API using AWS Lambda + API Gateway',
-    'long_description': '# pylambdarest\n\n[![CI/CD Status](https://github.com/MarwanDebbiche/pylambdarest/workflows/CI%2FCD/badge.svg?branch=master)](https://github.com/MarwanDebbiche/pylambdarest/actions?query=branch:master)\n[![Coverage Status](https://coveralls.io/repos/github/MarwanDebbiche/pylambdarest/badge.svg?branch=master)](https://coveralls.io/github/MarwanDebbiche/pylambdarest?branch=master)\n[![Latest Version](https://img.shields.io/pypi/v/pylambdarest.svg?color=blue)](https://pypi.python.org/pypi/pylambdarest)\n[![PyPI - Downloads](https://img.shields.io/pypi/dm/pylambdarest?label=pypi%20downloads)](https://pypi.org/project/pylambdarest/)\n![License](https://img.shields.io/github/license/MarwanDebbiche/pylambdarest)\n\npylambdarest is a lightweight opinionated framework for building REST API using [AWS Lambda](https://aws.amazon.com/lambda/) and [API Gateway](https://aws.amazon.com/api-gateway/).\n\n## Motivation\n\nWhy another framework ?\n\nWhen using API Gateway and python Lambda functions, one common pattern is to have a unique Lambda function triggered by a proxy API Gateway resource. The Lambda then uses a framework like [Flask](https://flask.palletsprojects.com/en/1.1.x/) to do all the routing. In an API Gateway + Lambda context, I feel like **the routing should be handled by API Gateway itself**, then forwarding the request to specific Lambda functions for each resource or endpoint.\n\n## Features\n\n- No routing. Yes, this is a feature. Routing should be handled by API Gateway.\n- API Gateway event parsing (including request body and path parameters).\n- Cleaner syntax.\n- Optional body schema and query parameters validation.\n- Optional authentication using JWT Bearet token.\n\n## Installation\n\nInstall the package from PyPI using pip:\n\n```\n$ pip install pylambdarest\n```\n\npylambdarest should also be included in the deployment package of your Lambda functions.\n\n## Getting started\n\npylambdarest provides a `@route` decorator to parse the API Gateway event into a `Request` object available in the handler function as an argument. It also formats the handler\'s output to the expected Lambda + API Gateway format seamlessly.\n\nTurning this:\n\n```python\nimport json\n\ndef handler(event, context):\n    body = json.loads(event["body"])\n    query_params = event["queryStringParameters"]\n    path_params = event["pathParameters"]\n\n    return {\n        "statusCode": 200,\n        "body": json.dumps({\n            "message": f"Hello from AWS Lambda {body[\'name\']}!!"\n        })\n    }\n\n```\n\nInto this:\n\n```python\nfrom pylambdarest import App\n\napp = App()\n\n@app.route()\ndef handler(request):\n    body = request.json\n    query_params = request.query_params\n    path_params = request.path_params\n\n    return 200, {"message": f"Hello from AWS Lambda {body[\'name\']}!!"}\n```\n\nYou can still access the original `event` and `context` arguments from the handler:\n\n```python\n@app.route()\ndef handler(request, event, context):\n    print(event)\n    body = request.json\n\n    return 200, {"message": f"Hello from AWS Lambda {body[\'name\']}!!"}\n```\n\n<br/>\n\nPath parameters defined in API Gateway can also be accessed directly as function argument:\n\n<br/>\n\n![api-gateway-path-params](https://raw.githubusercontent.com/MarwanDebbiche/pylambdarest/master/images/api-gateway-path-params.png)\n\n```python\n@app.route()\ndef get_user(user_id):\n    print(user_id)\n\n    # get user from db\n    user = {"id": user_id, "name": "John Doe"}\n\n    return 200, user\n```\n\n## Schema Validation\n\npylambdarest optionally provides schema validation using [jsonschema](https://github.com/Julian/jsonschema):\n\n```python\nuser_schema = {\n    "type": "object",\n    "properties": {\n        "name": {"type": "string"}\n    },\n    "required": ["name"],\n    "additionalProperties": False\n}\n\n@app.route(body_schema=user_schema)\ndef create_user(request):\n    # If the request\'s body does not\n    # satisfy the user_schema,\n    # a 400 will be returned\n\n    # Create user here\n\n    return 201\n\n\nquery_params_schema = {\n    "type": "object",\n    "properties": {\n        # Only string types are allowed for query parameters.\n        # Types casting should be done in the handler.\n        "page": {"type": "string"}\n    },\n    "additionalProperties": False\n}\n\n@app.route(query_params_schema=query_params_schema)\ndef get_users(request):\n    page = int(request.query_params.get("page", 1))\n\n    # request users in db\n    users = [\n        {"userId": i}\n        for i in range((page - 1) * 50, page * 50)\n    ]\n\n    return 200, users\n```\n\n## Authentication\n\n### Using JWT Bearer Token\n\n```python\nfrom datetime import datetime, timedelta, timezone\nimport jwt\nfrom pylambdarest import App, Request\n\nconfig = {"AUTH_SCHEME": "JWT_BEARER", "JWT_SECRET": "secret"}\n\napp = App(config=config)\n\n\nauth_schema = {\n    "type": "object",\n    "properties": {"username": {"type": "string"}, "password": {"type": "string"}},\n    "required": ["username", "password"],\n    "additionalProperties": False,\n}\n\n# POST /auth\n\n@app.route(body_schema=auth_schema)\ndef auth(request: Request):\n    username = request.json["username"]\n    password = request.json["password"]\n\n    # compare password and hash (stored in db) here\n\n    token = jwt.encode(\n        {\n            "exp": datetime.now(tz=timezone.utc) + timedelta(seconds=300),\n            "username": username,\n        },\n        config["JWT_SECRET"],\n    )\n\n    return 200, {"token": token}\n\n# GET /hello\n\n@app.route(restricted=True)\ndef hello(jwt_payload):\n    # This route is protected and a 401 error returned\n    # If the JWT is missing from the Authorization header\n\n    # The JWT payload is available as a \'jwt_payload\' argument.\n\n    return 200, {"message": "Hello from Pylambdarest"}\n\n```\n\n## Example\n\nYou can look at the [sample](https://github.com/MarwanDebbiche/pylambdarest/tree/master/sample) for a minimal pylambdarest API.\n\nIn this sample, we use the [serverless](https://www.serverless.com/) framework to declare the API Gateway -> Lambda routing\n\nThe packaging of the Lambda functions is done using the [serverless-python-requirements](https://github.com/UnitedIncome/serverless-python-requirements) plugin.\n',
-    'author': 'Marwan Debbiche (Macbook Pro)',
-    'author_email': 'marwan.debbiche@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/MarwanDebbiche/pylambdarest',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.7.2,<4.0.0',
+pylambdarest is a lightweight opinionated framework for building REST API using [AWS Lambda](https://aws.amazon.com/lambda/) and [API Gateway](https://aws.amazon.com/api-gateway/).
+
+## Motivation
+
+Why another framework ?
+
+When using API Gateway and python Lambda functions, one common pattern is to have a unique Lambda function triggered by a proxy API Gateway resource. The Lambda then uses a framework like [Flask](https://flask.palletsprojects.com/en/1.1.x/) to do all the routing. In an API Gateway + Lambda context, I feel like **the routing should be handled by API Gateway itself**, then forwarding the request to specific Lambda functions for each resource or endpoint.
+
+## Features
+
+- No routing. Yes, this is a feature. Routing should be handled by API Gateway.
+- API Gateway event parsing (including request body and path parameters).
+- Cleaner syntax.
+- Optional body schema and query parameters validation.
+- Optional authentication using JWT Bearet token.
+
+## Installation
+
+Install the package from PyPI using pip:
+
+```
+$ pip install pylambdarest
+```
+
+pylambdarest should also be included in the deployment package of your Lambda functions.
+
+## Getting started
+
+pylambdarest provides a `@route` decorator to parse the API Gateway event into a `Request` object available in the handler function as an argument. It also formats the handler's output to the expected Lambda + API Gateway format seamlessly.
+
+Turning this:
+
+```python
+import json
+
+def handler(event, context):
+    body = json.loads(event["body"])
+    query_params = event["queryStringParameters"]
+    path_params = event["pathParameters"]
+
+    return {
+        "statusCode": 200,
+        "body": json.dumps({
+            "message": f"Hello from AWS Lambda {body['name']}!!"
+        })
+    }
+
+```
+
+Into this:
+
+```python
+from pylambdarest import App
+
+app = App()
+
+@app.route()
+def handler(request):
+    body = request.json
+    query_params = request.query_params
+    path_params = request.path_params
+
+    return 200, {"message": f"Hello from AWS Lambda {body['name']}!!"}
+```
+
+You can still access the original `event` and `context` arguments from the handler:
+
+```python
+@app.route()
+def handler(request, event, context):
+    print(event)
+    body = request.json
+
+    return 200, {"message": f"Hello from AWS Lambda {body['name']}!!"}
+```
+
+<br/>
+
+Path parameters defined in API Gateway can also be accessed directly as function argument:
+
+<br/>
+
+![api-gateway-path-params](https://raw.githubusercontent.com/MarwanDebbiche/pylambdarest/master/images/api-gateway-path-params.png)
+
+```python
+@app.route()
+def get_user(user_id):
+    print(user_id)
+
+    # get user from db
+    user = {"id": user_id, "name": "John Doe"}
+
+    return 200, user
+```
+
+## Schema Validation
+
+pylambdarest optionally provides schema validation using [jsonschema](https://github.com/Julian/jsonschema):
+
+```python
+user_schema = {
+    "type": "object",
+    "properties": {
+        "name": {"type": "string"}
+    },
+    "required": ["name"],
+    "additionalProperties": False
+}
+
+@app.route(body_schema=user_schema)
+def create_user(request):
+    # If the request's body does not
+    # satisfy the user_schema,
+    # a 400 will be returned
+
+    # Create user here
+
+    return 201
+
+
+query_params_schema = {
+    "type": "object",
+    "properties": {
+        # Only string types are allowed for query parameters.
+        # Types casting should be done in the handler.
+        "page": {"type": "string"}
+    },
+    "additionalProperties": False
+}
+
+@app.route(query_params_schema=query_params_schema)
+def get_users(request):
+    page = int(request.query_params.get("page", 1))
+
+    # request users in db
+    users = [
+        {"userId": i}
+        for i in range((page - 1) * 50, page * 50)
+    ]
+
+    return 200, users
+```
+
+## Authentication
+
+### Using JWT Bearer Token
+
+```python
+from datetime import datetime, timedelta, timezone
+import jwt
+from pylambdarest import App, Request
+
+config = {"AUTH_SCHEME": "JWT_BEARER", "JWT_SECRET": "secret"}
+
+app = App(config=config)
+
+
+auth_schema = {
+    "type": "object",
+    "properties": {"username": {"type": "string"}, "password": {"type": "string"}},
+    "required": ["username", "password"],
+    "additionalProperties": False,
 }
 
+# POST /auth
+
+@app.route(body_schema=auth_schema)
+def auth(request: Request):
+    username = request.json["username"]
+    password = request.json["password"]
+
+    # compare password and hash (stored in db) here
+
+    token = jwt.encode(
+        {
+            "exp": datetime.now(tz=timezone.utc) + timedelta(seconds=300),
+            "username": username,
+        },
+        config["JWT_SECRET"],
+    )
+
+    return 200, {"token": token}
+
+# GET /hello
+
+@app.route(restricted=True)
+def hello(jwt_payload):
+    # This route is protected and a 401 error returned
+    # If the JWT is missing from the Authorization header
+
+    # The JWT payload is available as a 'jwt_payload' argument.
+
+    return 200, {"message": "Hello from Pylambdarest"}
+
+```
+
+## Example
+
+You can look at the [sample](https://github.com/MarwanDebbiche/pylambdarest/tree/master/sample) for a minimal pylambdarest API.
+
+In this sample, we use the [serverless](https://www.serverless.com/) framework to declare the API Gateway -> Lambda routing
+
+The packaging of the Lambda functions is done using the [serverless-python-requirements](https://github.com/UnitedIncome/serverless-python-requirements) plugin.
 
-setup(**setup_kwargs)
```

