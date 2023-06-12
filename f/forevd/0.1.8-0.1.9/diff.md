# Comparing `tmp/forevd-0.1.8.tar.gz` & `tmp/forevd-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forevd-0.1.8.tar", max compression
+gzip compressed data, was "forevd-0.1.9.tar", max compression
```

## Comparing `forevd-0.1.8.tar` & `forevd-0.1.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    11357 2023-06-12 16:29:28.917774 forevd-0.1.8/LICENSE
--rw-r--r--   0        0        0     4065 2023-06-12 16:29:28.917774 forevd-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/__init__.py
--rw-r--r--   0        0        0     5879 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/__main__.py
--rw-r--r--   0        0        0     1543 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/apache/__init__.py
--rw-r--r--   0        0        0     4777 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/apache/httpd.conf
--rw-r--r--   0        0        0      216 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/app.py
--rw-r--r--   0        0        0        0 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/resources/__init__.py
--rw-r--r--   0        0        0        0 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/resources/logging/__init__.py
--rw-r--r--   0        0        0      387 2023-06-12 16:29:28.921774 forevd-0.1.8/forevd/resources/logging/cli.conf
--rw-r--r--   0        0        0      884 2023-06-12 16:29:28.921774 forevd-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     4770 1970-01-01 00:00:00.000000 forevd-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-06-12 22:39:08.047007 forevd-0.1.9/LICENSE
+-rw-r--r--   0        0        0     4065 2023-06-12 22:39:08.047007 forevd-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/__init__.py
+-rw-r--r--   0        0        0     6247 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/__main__.py
+-rw-r--r--   0        0        0     1543 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/apache/__init__.py
+-rw-r--r--   0        0        0     4836 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/apache/httpd.conf
+-rw-r--r--   0        0        0      216 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/app.py
+-rw-r--r--   0        0        0        0 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/resources/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/resources/logging/__init__.py
+-rw-r--r--   0        0        0      387 2023-06-12 22:39:08.047007 forevd-0.1.9/forevd/resources/logging/cli.conf
+-rw-r--r--   0        0        0      884 2023-06-12 22:39:08.047007 forevd-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     4770 1970-01-01 00:00:00.000000 forevd-0.1.9/PKG-INFO
```

### Comparing `forevd-0.1.8/LICENSE` & `forevd-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `forevd-0.1.8/README.md` & `forevd-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `forevd-0.1.8/forevd/__main__.py` & `forevd-0.1.9/forevd/__main__.py`

 * *Files 13% similar despite different names*

```diff
@@ -36,15 +36,20 @@
         if config["path"] == path:
             return config
 
     return None
 
 
 def _nomalize_locations(
-    locations: dict, backend: str, location: str, mtls: bool, http_methods: list
+    locations: dict,
+    backend: str,
+    location: str,
+    mtls: bool,
+    http_methods: list,
+    set_access_token: bool,
 ):
     if not locations:
         locations = []
 
     endpoints = [conf["path"] for conf in locations]
 
     missing_cli_loc = False
@@ -60,14 +65,16 @@
 
         if "backend" not in config:
             config["backend"] = backend
         if "mtls" not in config:
             config["mtls"] = mtls
         if "http_methods" not in config:
             config["http_methods"] = http_methods
+        if "set_access_token" not in config:
+            config["set_access_token"] = set_access_token
 
         if missing_cli_loc:
             locations.append(config)
 
     _LOGGER.debug(f"locations: {locations}")
 
     return locations
@@ -171,14 +178,21 @@
     help="Define the server name, else it uses $HOSTNAME",
     type=str,
     show_default=True,
     default=_DEFAULT_HOSTNAME,
     envvar="FOREVD_HOSTNAME",
 )
 @click.option(
+    "--set-access-token/--no-set-access-token",
+    "set_access_token",
+    help="Set the access token",
+    is_flag=True,
+    default=True,
+)
+@click.option(
     "--var-dir",
     help="The backend of this reverse proxy will front, e.g. http://localhost:8080/foo",
     type=click.Path(),
     default=_DEFAULT_VAR_DIR,
     show_default=True,
 )
 # pylint: disable=too-many-arguments,too-many-locals
@@ -198,14 +212,15 @@
     ldap,
     listen,
     location,
     locations,
     mtls,
     oidc,
     server_name,
+    set_access_token,
     var_dir,
 ):
     """forevd is a forward/reverse proxy, primarily used as a sidecar for REST or any HTTP/s apps."""
     _setup_logging(debug)
 
     if (not backend or not location) and not locations:
         raise click.UsageError("You must supply a --backend and --location or --locations")
@@ -218,15 +233,17 @@
         "access_log": access_log,
         "ca_cert": ca_cert,
         "cert": cert,
         "cert_key": cert_key,
         "httpd_include": httpd_include,
         "debug": debug,
         "ldap": ldap,
-        "locations": _nomalize_locations(locations, backend, location, mtls, http_methods),
+        "locations": _nomalize_locations(
+            locations, backend, location, mtls, http_methods, set_access_token
+        ),
         "listen": listen,
         "oidc": oidc,
         "server_name": server_name,
     }
     _LOGGER.debug(f"config: {config}")
 
     mod = importlib.import_module(f"forevd.{backend_type}")
```

### Comparing `forevd-0.1.8/forevd/apache/__init__.py` & `forevd-0.1.9/forevd/apache/__init__.py`

 * *Files identical despite different names*

### Comparing `forevd-0.1.8/forevd/apache/httpd.conf` & `forevd-0.1.9/forevd/apache/httpd.conf`

 * *Files 2% similar despite different names*

```diff
@@ -134,16 +134,18 @@
     RequestHeader set X-Remote-User %{SSL_CLIENT_S_DN_CN}e
     RequestHeader set X-SSL-certificate "%{SSL_CLIENT_CERT}s" "expr=-n %{SSL_CLIENT_CERT}"
     {% endif %}
 
     {% if oidc -%}
     AuthType openid-connect
     RequestHeader set X-Remote-User %{REMOTE_USER}s "expr=-n %{REMOTE_USER}"
+    {% if location["set_access_token"] -%}
     RequestHeader set Authorization "Bearer %{OIDC_access_token}e" env=OIDC_access_token
     {% endif %}
+    {% endif %}
 
     {% if "ldap" in location["authz"] -%}
     AuthLDAPURL {{ location["authz"]["ldap"]["url"] }}
     AuthLDAPBindDN {{ location["authz"]["ldap"]["bind-dn"] }}
     AuthLDAPBindPassword {{ location["authz"]["ldap"]["bind-pw"] }}
     {% endif %}
```

### Comparing `forevd-0.1.8/pyproject.toml` & `forevd-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "forevd"
-version = "0.1.8"
+version = "0.1.9"
 description = "Forward and reverse proxy using apache or nginx"
 authors = ["Erick Bourgeois <erick@jeb.ca>"]
 license = "LICENSE"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `forevd-0.1.8/PKG-INFO` & `forevd-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: forevd
-Version: 0.1.8
+Version: 0.1.9
 Summary: Forward and reverse proxy using apache or nginx
 License: LICENSE
 Author: Erick Bourgeois
 Author-email: erick@jeb.ca
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

