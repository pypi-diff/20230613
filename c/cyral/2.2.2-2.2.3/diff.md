# Comparing `tmp/cyral-2.2.2.tar.gz` & `tmp/cyral-2.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyral-2.2.2.tar", max compression
+gzip compressed data, was "cyral-2.2.3.tar", max compression
```

## Comparing `cyral-2.2.2.tar` & `cyral-2.2.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     2113 2023-03-27 17:45:28.532629 cyral-2.2.2/DOC.md
--rw-r--r--   0        0        0        0 2022-08-30 17:38:27.223884 cyral-2.2.2/cyral/__init__.py
--rw-r--r--   0        0        0        0 2022-08-30 17:38:27.224635 cyral-2.2.2/cyral/cli/__init__.py
--rw-r--r--   0        0        0    19930 2023-03-27 17:45:28.534180 cyral-2.2.2/cyral/cli/__main__.py
--rw-r--r--   0        0        0     7439 2023-05-02 22:31:23.634262 cyral-2.2.2/cyral/cli/_aws.py
--rw-r--r--   0        0        0     1829 2022-09-15 23:46:59.079990 cyral-2.2.2/cyral/cli/_pgpass.py
--rw-r--r--   0        0        0        0 2022-08-30 17:38:27.225843 cyral-2.2.2/cyral/sdk/__init__.py
--rw-r--r--   0        0        0      421 2023-03-27 17:45:28.534806 cyral-2.2.2/cyral/sdk/api/__init__.py
--rw-r--r--   0        0        0     1886 2022-09-14 01:07:35.570728 cyral-2.2.2/cyral/sdk/api/access_info.py
--rw-r--r--   0        0        0      424 2022-09-14 01:07:35.571081 cyral-2.2.2/cyral/sdk/api/access_token.py
--rw-r--r--   0        0        0      498 2022-09-14 02:51:19.645357 cyral-2.2.2/cyral/sdk/api/ca_bundle.py
--rw-r--r--   0        0        0     1829 2023-03-27 17:45:28.535153 cyral-2.2.2/cyral/sdk/api/resource.py
--rw-r--r--   0        0        0     4281 2023-04-05 17:08:15.700127 cyral-2.2.2/cyral/sdk/api/sidecar.py
--rw-r--r--   0        0        0      483 2022-09-14 01:07:35.572429 cyral-2.2.2/cyral/sdk/api/user.py
--rwxr-xr-x   0        0        0    11851 2023-03-07 19:03:36.429388 cyral-2.2.2/cyral/sdk/client.py
--rw-r--r--   0        0        0      730 2023-05-02 22:31:23.635205 cyral-2.2.2/pyproject.toml
--rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 cyral-2.2.2/setup.py
--rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 cyral-2.2.2/PKG-INFO
+-rw-r--r--   0        0        0     2113 2023-03-27 17:45:28.532629 cyral-2.2.3/DOC.md
+-rw-r--r--   0        0        0        0 2022-08-30 17:38:27.223884 cyral-2.2.3/cyral/__init__.py
+-rw-r--r--   0        0        0        0 2022-08-30 17:38:27.224635 cyral-2.2.3/cyral/cli/__init__.py
+-rw-r--r--   0        0        0    19951 2023-05-30 02:39:24.364368 cyral-2.2.3/cyral/cli/__main__.py
+-rw-r--r--   0        0        0     7439 2023-05-02 22:31:23.634262 cyral-2.2.3/cyral/cli/_aws.py
+-rw-r--r--   0        0        0     1829 2022-09-15 23:46:59.079990 cyral-2.2.3/cyral/cli/_pgpass.py
+-rw-r--r--   0        0        0        0 2022-08-30 17:38:27.225843 cyral-2.2.3/cyral/sdk/__init__.py
+-rw-r--r--   0        0        0      421 2023-03-27 17:45:28.534806 cyral-2.2.3/cyral/sdk/api/__init__.py
+-rw-r--r--   0        0        0     1886 2022-09-14 01:07:35.570728 cyral-2.2.3/cyral/sdk/api/access_info.py
+-rw-r--r--   0        0        0      424 2022-09-14 01:07:35.571081 cyral-2.2.3/cyral/sdk/api/access_token.py
+-rw-r--r--   0        0        0      887 2023-05-30 02:39:24.365394 cyral-2.2.3/cyral/sdk/api/ca_bundle.py
+-rw-r--r--   0        0        0     1829 2023-03-27 17:45:28.535153 cyral-2.2.3/cyral/sdk/api/resource.py
+-rw-r--r--   0        0        0     4281 2023-04-05 17:08:15.700127 cyral-2.2.3/cyral/sdk/api/sidecar.py
+-rw-r--r--   0        0        0      483 2022-09-14 01:07:35.572429 cyral-2.2.3/cyral/sdk/api/user.py
+-rwxr-xr-x   0        0        0    11851 2023-03-07 19:03:36.429388 cyral-2.2.3/cyral/sdk/client.py
+-rw-r--r--   0        0        0      730 2023-05-30 02:39:24.366135 cyral-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3011 1970-01-01 00:00:00.000000 cyral-2.2.3/setup.py
+-rw-r--r--   0        0        0     2707 1970-01-01 00:00:00.000000 cyral-2.2.3/PKG-INFO
```

### Comparing `cyral-2.2.2/DOC.md` & `cyral-2.2.3/DOC.md`

 * *Files identical despite different names*

### Comparing `cyral-2.2.2/cyral/cli/__main__.py` & `cyral-2.2.3/cyral/cli/__main__.py`

 * *Files 0% similar despite different names*

```diff
@@ -362,15 +362,15 @@
     binding_info = sidecar_client.get_binding(sidecar_id, binding_id)
     user_email = UserClient(cyral_client).get_current_user()["email"]
     token = AccessTokenClient(cyral_client).get()
     sidecar_address = (
         f"{SidecarClient.endpoint(sidecar_info)}:"
         + f"{sidecar_client.port_for_binding(sidecar_id, binding_info, True)}"
     )
-    ca_bundle = CABundleClient(cyral_client).get()
+    ca_bundle = CABundleClient(cyral_client).get(sidecar_id=sidecar_id)
     if not s3_proxy_is_configured(aws_profile):
         user_input = ""
         if not autoconfigure:
             user_input = input(
                 "S3 proxy settings are not correctly configured to work "
                 "with Cyral.\nProceed with the configuration first? [y/n] "
             )
```

### Comparing `cyral-2.2.2/cyral/cli/_aws.py` & `cyral-2.2.3/cyral/cli/_aws.py`

 * *Files identical despite different names*

### Comparing `cyral-2.2.2/cyral/cli/_pgpass.py` & `cyral-2.2.3/cyral/cli/_pgpass.py`

 * *Files identical despite different names*

### Comparing `cyral-2.2.2/cyral/sdk/api/access_info.py` & `cyral-2.2.3/cyral/sdk/api/access_info.py`

 * *Files identical despite different names*

### Comparing `cyral-2.2.2/cyral/sdk/api/resource.py` & `cyral-2.2.3/cyral/sdk/api/resource.py`

 * *Files identical despite different names*

### Comparing `cyral-2.2.2/cyral/sdk/api/sidecar.py` & `cyral-2.2.3/cyral/sdk/api/sidecar.py`

 * *Files identical despite different names*

### Comparing `cyral-2.2.2/cyral/sdk/client.py` & `cyral-2.2.3/cyral/sdk/client.py`

 * *Files identical despite different names*

### Comparing `cyral-2.2.2/pyproject.toml` & `cyral-2.2.3/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 [tool.poetry]
 name = "cyral"
-version = "2.2.2"
+version = "2.2.3"
 description = "The Cyral CLI tool"
 license = "MIT"
 authors = [
 	"Deepak Gupta <deepak@cyral.com>",
 	"Pedro Carvalho <pcarvalho@cyral.com>",
 ]
 readme = "DOC.md"
 
 [tool.poetry.dependencies]
 click = "^8.1"
 oauthlib = "^3.2"
 python = "^3.9"
-requests = "^2.28"
+requests = "^2.31"
 columnar = "^1.4"
 awscli = "^1.25"
 
 [tool.poetry.dev-dependencies]
-types-requests = "^2.28"
+types-requests = "^2.31"
 typing_extensions = "^4.3"
 types-setuptools = "^65.3"
 types-PyYAML = "^6.0"
 mypy = "^0.971"
 pylint = "^2.14"
 flake8 = "^5.0"
 black = "^22.6"
```

### Comparing `cyral-2.2.2/setup.py` & `cyral-2.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 {'': ['*']}
 
 install_requires = \
 ['awscli>=1.25,<2.0',
  'click>=8.1,<9.0',
  'columnar>=1.4,<2.0',
  'oauthlib>=3.2,<4.0',
- 'requests>=2.28,<3.0']
+ 'requests>=2.31,<3.0']
 
 entry_points = \
 {'console_scripts': ['cyral = cyral.cli.__main__:main']}
 
 setup_kwargs = {
     'name': 'cyral',
-    'version': '2.2.2',
+    'version': '2.2.3',
     'description': 'The Cyral CLI tool',
     'long_description': '# The Cyral CLI Tool\n\nUse this tool to obtain credentials for accessing a data repo via the Cyral sidecar.\n\n**Note 1** This tool does not work with Cyral versions before 3.0. If you are using an\nolder version of Cyral, please use the [gimme-db-token](https://pypi.org/project/cyral-gimme-db-token/)\ntool instead.\n\n**Note 2** Use version 1.x of this tool for Cyral version 3.X and version 2.x for Cyral version 4.X and greater.\n\n## Usage\n\n```\ncyral <global options> <command> <subcommand> <command options>\n```\n\nFor detailed usage instructions:\n\n```bash\ncyral --help\n```\n\n### Global Options\n\n- `--cp-address <control plane address>` Cyral Control Plane Address, e.g., `mycompany.app.cyral.com` (the address may need a :8000 suffix in some cases).\n- `--idp <idp alias>` The identity provider to use for authentication.\n- `--offline-access` Obtain a long-lived offline access token for authentication to the control plane.\n- `--no-stored-creds` Do not store or use a stored refresh token.\n- `--realm` The authentication realm in the Cyral control plane. This is usually not needed. Please contact Cyral Support for help if authentication is failing without this option.\n- `--version` Show package version and exit.\n- `--help` Show command help.\n\n### Top Level Commands\n\n### `access`\n\nTools for accessing different options on the cyral CP\n\nIt has the following subcommands:\n\n- `token` Print a token for authenticating to a repo using your email address as user name.\n- `repo` Show list of accessible data repos and print connection information for the selected repo.\n  + Use `--type`, `--tag`, `--name` options to specify repo filters.\n- `s3` Write configuration needed to access S3 to AWS config files.\n- `pg` Write configuration needed to access selected postgres database to `.pgpass` file.\n\n### `sidecar` \n\nTools for interacting with the Cyral sidecars\n\nIt has the following subcommands:\n\n- `get` Get information for a sidecar or sidecars.\n- `set` Set options on a sidecar.\n\n#### `set`\n\nSet options for a Cyral sidecar. It has the following subcommands:\n\n- `log-level` Sets the log level for sidecar service(s).\n\n',
     'author': 'Deepak Gupta',
     'author_email': 'deepak@cyral.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `cyral-2.2.2/PKG-INFO` & `cyral-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cyral
-Version: 2.2.2
+Version: 2.2.3
 Summary: The Cyral CLI tool
 License: MIT
 Author: Deepak Gupta
 Author-email: deepak@cyral.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: awscli (>=1.25,<2.0)
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: columnar (>=1.4,<2.0)
 Requires-Dist: oauthlib (>=3.2,<4.0)
-Requires-Dist: requests (>=2.28,<3.0)
+Requires-Dist: requests (>=2.31,<3.0)
 Description-Content-Type: text/markdown
 
 # The Cyral CLI Tool
 
 Use this tool to obtain credentials for accessing a data repo via the Cyral sidecar.
 
 **Note 1** This tool does not work with Cyral versions before 3.0. If you are using an
```

