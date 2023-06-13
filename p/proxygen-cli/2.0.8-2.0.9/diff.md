# Comparing `tmp/proxygen_cli-2.0.8.tar.gz` & `tmp/proxygen_cli-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proxygen_cli-2.0.8.tar", max compression
+gzip compressed data, was "proxygen_cli-2.0.9.tar", max compression
```

## Comparing `proxygen_cli-2.0.8.tar` & `proxygen_cli-2.0.9.tar`

### file list

```diff
@@ -1,21 +1,22 @@
--rw-r--r--   0        0        0     1191 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/README.md
--rw-r--r--   0        0        0      229 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/__init__.py
--rw-r--r--   0        0        0     1509 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/cli/command_credentials.py
--rw-r--r--   0        0        0     3706 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/cli/command_instance.py
--rw-r--r--   0        0        0     1417 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/cli/command_main.py
--rw-r--r--   0        0        0     3662 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/cli/command_secret.py
--rw-r--r--   0        0        0     1852 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/cli/command_settings.py
--rw-r--r--   0        0        0     2716 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/cli/command_spec.py
--rw-r--r--   0        0        0     5620 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/lib/auth.py
--rw-r--r--   0        0        0      208 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/lib/constants.py
--rw-r--r--   0        0        0     3277 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/lib/credentials.py
--rw-r--r--   0        0        0     1018 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/lib/dot_proxygen.py
--rw-r--r--   0        0        0     1562 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/lib/output.py
--rw-r--r--   0        0        0     5066 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/lib/proxygen_api.py
--rw-r--r--   0        0        0      857 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/lib/settings.py
--rw-r--r--   0        0        0     2683 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/lib/spec.py
--rw-r--r--   0        0        0     1042 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/lib/spec_server.py
--rw-r--r--   0        0        0      520 2023-02-09 13:54:31.674148 proxygen_cli-2.0.8/proxygen_cli/lib/version.py
--rw-r--r--   0        0        0      662 2023-02-09 13:54:31.678149 proxygen_cli-2.0.8/pyproject.toml
--rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 proxygen_cli-2.0.8/setup.py
--rw-r--r--   0        0        0     2165 1970-01-01 00:00:00.000000 proxygen_cli-2.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1191 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/README.md
+-rw-r--r--   0        0        0      229 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/__init__.py
+-rw-r--r--   0        0        0     1509 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/cli/command_credentials.py
+-rw-r--r--   0        0        0     1167 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/cli/command_docker.py
+-rw-r--r--   0        0        0     3706 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/cli/command_instance.py
+-rw-r--r--   0        0        0      958 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/cli/command_main.py
+-rw-r--r--   0        0        0     3662 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/cli/command_secret.py
+-rw-r--r--   0        0        0     1852 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/cli/command_settings.py
+-rw-r--r--   0        0        0     2716 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/cli/command_spec.py
+-rw-r--r--   0        0        0     5620 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/lib/auth.py
+-rw-r--r--   0        0        0      208 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/lib/constants.py
+-rw-r--r--   0        0        0     3277 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/lib/credentials.py
+-rw-r--r--   0        0        0     1018 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/lib/dot_proxygen.py
+-rw-r--r--   0        0        0     1562 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/lib/output.py
+-rw-r--r--   0        0        0     5066 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/lib/proxygen_api.py
+-rw-r--r--   0        0        0      857 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/lib/settings.py
+-rw-r--r--   0        0        0     3037 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/lib/spec.py
+-rw-r--r--   0        0        0     1042 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/lib/spec_server.py
+-rw-r--r--   0        0        0      520 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/proxygen_cli/lib/version.py
+-rw-r--r--   0        0        0      662 2023-02-09 16:03:35.465282 proxygen_cli-2.0.9/pyproject.toml
+-rw-r--r--   0        0        0     2294 1970-01-01 00:00:00.000000 proxygen_cli-2.0.9/setup.py
+-rw-r--r--   0        0        0     2165 1970-01-01 00:00:00.000000 proxygen_cli-2.0.9/PKG-INFO
```

### Comparing `proxygen_cli-2.0.8/README.md` & `proxygen_cli-2.0.9/README.md`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.0.8/proxygen_cli/cli/command_credentials.py` & `proxygen_cli-2.0.9/proxygen_cli/cli/command_credentials.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.0.8/proxygen_cli/cli/command_instance.py` & `proxygen_cli-2.0.9/proxygen_cli/cli/command_instance.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.0.8/proxygen_cli/cli/command_secret.py` & `proxygen_cli-2.0.9/proxygen_cli/cli/command_secret.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.0.8/proxygen_cli/cli/command_settings.py` & `proxygen_cli-2.0.9/proxygen_cli/cli/command_settings.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.0.8/proxygen_cli/cli/command_spec.py` & `proxygen_cli-2.0.9/proxygen_cli/cli/command_spec.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.0.8/proxygen_cli/lib/auth.py` & `proxygen_cli-2.0.9/proxygen_cli/lib/auth.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.0.8/proxygen_cli/lib/credentials.py` & `proxygen_cli-2.0.9/proxygen_cli/lib/credentials.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.0.8/proxygen_cli/lib/dot_proxygen.py` & `proxygen_cli-2.0.9/proxygen_cli/lib/dot_proxygen.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.0.8/proxygen_cli/lib/output.py` & `proxygen_cli-2.0.9/proxygen_cli/lib/output.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.0.8/proxygen_cli/lib/proxygen_api.py` & `proxygen_cli-2.0.9/proxygen_cli/lib/proxygen_api.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.0.8/proxygen_cli/lib/settings.py` & `proxygen_cli-2.0.9/proxygen_cli/lib/settings.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.0.8/proxygen_cli/lib/spec.py` & `proxygen_cli-2.0.9/proxygen_cli/lib/spec.py`

 * *Files 6% similar despite different names*

```diff
@@ -67,25 +67,29 @@
 
     with root_file.open() as f:
         spec = load_templated_yaml(f.read())
 
     for key in pop_keys:
         spec.pop(key, None)
 
-    file_refs = _find_file_refs(spec)
-    spec_dir = root_file.parent.absolute().resolve()
+    # We need this while loop to handle the case where a file a $ref has a $ref inside it.
+    # The first loop replaces the outer ref, but also adds a ref.
+    # This Very Hacky Method can almost certainly be replaced with something more elegant.
+    # but... tomorrow is my last day, so it won't be me doing it.
+    while file_refs := _find_file_refs(spec):
+        spec_dir = root_file.parent.absolute().resolve()
+
+        for keys, file_ref in file_refs:
+            file_path = spec_dir.joinpath(file_ref)
+            if not file_path.exists() or file_path.is_dir():
+                raise click.ClickException(f"Unable to resolve $ref {file_path} at {keys}")
+            with file_path.open() as f:
+                sub_spec = load_templated_yaml(f.read())
 
-    for keys, file_ref in file_refs:
-        file_path = spec_dir.joinpath(file_ref)
-        if not file_path.exists() or file_path.is_dir():
-            raise click.ClickException(f"Unable to resolve $ref {file_path} at {keys}")
-        with file_path.open() as f:
-            sub_spec = load_templated_yaml(f.read())
-
-        spec = _update_obj(spec, keys, sub_spec)
+            spec = _update_obj(spec, keys, sub_spec)
     return spec
 
 
 
 def host(env):
     sub_domain = "api" if env == "prod" else f"{env}.api"
     return f"https://{sub_domain}.service.nhs.uk"
```

### Comparing `proxygen_cli-2.0.8/proxygen_cli/lib/spec_server.py` & `proxygen_cli-2.0.9/proxygen_cli/lib/spec_server.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.0.8/proxygen_cli/lib/version.py` & `proxygen_cli-2.0.9/proxygen_cli/lib/version.py`

 * *Files identical despite different names*

### Comparing `proxygen_cli-2.0.8/pyproject.toml` & `proxygen_cli-2.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proxygen-cli"
-version = "2.0.8"
+version = "2.0.9"
 description = "CLI for interacting with NHSD APIM's proxygen service"
 authors = ["Ben Strutt <ben.strutt1@nhs.net>"]
 readme = "README.md"
 packages = [{include = "proxygen_cli"}]
 repository = "https://github.com/NHSDigital/proxygen-cli"
 
 [tool.poetry.scripts]
```

### Comparing `proxygen_cli-2.0.8/setup.py` & `proxygen_cli-2.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
  'yaspin>=2.2.0,<3.0.0']
 
 entry_points = \
 {'console_scripts': ['proxygen = proxygen_cli.cli.command_main:main']}
 
 setup_kwargs = {
     'name': 'proxygen-cli',
-    'version': '2.0.8',
+    'version': '2.0.9',
     'description': "CLI for interacting with NHSD APIM's proxygen service",
     'long_description': '# proxygen-cli\n\n## Installation\n\nShould be as simple as\n```\npip install proxygen-cli\n```\nThe python package includes an execuatable `proxygen`.\nType `proxygen` to see a list of available commands.\n\n\n## Configuration\n\n### Credentials\n\nAll users should have individual credentials.\n`proxygen-cli` needs to know about them.\n\n```\nproxygen credentials set username <USERNAME>\nproxygen credentials set password <PASSWORD>\n```\n\nThe CLI has its own client credentials, which need to be input.\nContact `deathstar` squad or the `platforms-api-producer-support` slack channel to find out what they are.\n```\nproxgen credentials set client_id <CLIENT_ID>\nproxgen credentials set client_secret <CLIENT_SECRET>\n```\n\n\n### Settings\n`proxygen-cli` needs to know what API you are developing.\n\n```\nproxygen settings set api <API-NAME>\n```\nYour user must have permissions to manipulate instances/secrets/specs for the API you set here.\nIf you do not have sufficient permissions commands will fail.\nIf you believe your permissions are incorrect, contact the `platforms-api-producer-support` channel.\n\n## Commands\nCommands are documented inside the CLI itself.\nType `proxygen` to see a list of available commands.\n',
     'author': 'Ben Strutt',
     'author_email': 'ben.strutt1@nhs.net',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/NHSDigital/proxygen-cli',
```

### Comparing `proxygen_cli-2.0.8/PKG-INFO` & `proxygen_cli-2.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proxygen-cli
-Version: 2.0.8
+Version: 2.0.9
 Summary: CLI for interacting with NHSD APIM's proxygen service
 Home-page: https://github.com/NHSDigital/proxygen-cli
 Author: Ben Strutt
 Author-email: ben.strutt1@nhs.net
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
```

