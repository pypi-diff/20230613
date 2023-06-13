# Comparing `tmp/revproxy_auth-0.1.6.tar.gz` & `tmp/revproxy_auth-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "revproxy_auth-0.1.6.tar", last modified: Fri May 26 11:53:09 2023, max compression
+gzip compressed data, was "revproxy_auth-0.1.7.tar", last modified: Tue Jun 13 06:47:11 2023, max compression
```

## Comparing `revproxy_auth-0.1.6.tar` & `revproxy_auth-0.1.7.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/revproxy_auth/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/revproxy_auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/revproxy_auth/config-template.yml
--rw-r--r--   0 runner    (1001) docker     (123)    19605 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/revproxy_auth/revproxy_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.917979 revproxy_auth-0.1.6/revproxy_auth/revproxy_auth_static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/revproxy_auth/revproxy_auth_static/css/
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/revproxy_auth/revproxy_auth_static/css/view.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/revproxy_auth/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/revproxy_auth/templates/form.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/revproxy_auth.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-26 11:53:09.000000 revproxy_auth-0.1.6/revproxy_auth.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-26 11:53:09.000000 revproxy_auth-0.1.6/revproxy_auth.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 11:53:09.000000 revproxy_auth-0.1.6/revproxy_auth.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 11:53:09.000000 revproxy_auth-0.1.6/revproxy_auth.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-26 11:53:09.000000 revproxy_auth-0.1.6/revproxy_auth.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 11:53:09.921979 revproxy_auth-0.1.6/tests/data/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/tests/data/config.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/tests/test_000.py
--rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-05-26 11:52:52.000000 revproxy_auth-0.1.6/tests/test_001.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.607762 revproxy_auth-0.1.7/revproxy_auth/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/revproxy_auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/revproxy_auth/config-template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)    19577 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/revproxy_auth/revproxy_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.607762 revproxy_auth-0.1.7/revproxy_auth/revproxy_auth_static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/revproxy_auth/revproxy_auth_static/css/
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/revproxy_auth/revproxy_auth_static/css/view.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/revproxy_auth/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/revproxy_auth/templates/form.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/revproxy_auth.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-06-13 06:47:11.000000 revproxy_auth-0.1.7/revproxy_auth.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 06:47:11.000000 revproxy_auth-0.1.7/revproxy_auth.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 06:47:11.000000 revproxy_auth-0.1.7/revproxy_auth.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-06-13 06:47:11.000000 revproxy_auth-0.1.7/revproxy_auth.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-13 06:47:11.000000 revproxy_auth-0.1.7/revproxy_auth.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 06:47:11.611762 revproxy_auth-0.1.7/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/tests/data/config.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4335 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/tests/test_000.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3535 2023-06-13 06:46:58.000000 revproxy_auth-0.1.7/tests/test_001.py
```

### Comparing `revproxy_auth-0.1.6/PKG-INFO` & `revproxy_auth-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revproxy_auth
-Version: 0.1.6
+Version: 0.1.7
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # revproxy_auth
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
```

### Comparing `revproxy_auth-0.1.6/README.md` & `revproxy_auth-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.6/revproxy_auth/revproxy_auth.py` & `revproxy_auth-0.1.7/revproxy_auth/revproxy_auth.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 """ Class to perform authentication using the synology authmethods """
 import os
 import time
 from urllib import parse
 import json
+import logging
 from pathlib import Path
 import secrets
 import jinja2
 import requests
 from flask import Flask, request, Response, send_from_directory, redirect, Request
 
 from config_yml import Config
-from log_mgr import Logger
 
 COOKIE_LIFE_MINUTES = 15
 
 HTTP_200_OK = 200
 HTTP_501_NOT_IMPLEMENTED = 501
 
 class RevProxyAuth():
@@ -32,15 +32,15 @@
         """
 
         if not template_config_path:
             template_config_path = os.path.join(Path(__file__).parent.resolve(), './config-template.yml')
 
         self._config = Config(root_class, template_config_path, 'revproxy_auth_config.yml', dry_run=dry_run)
 
-        self.logger = Logger(root_class, 'revproxy_auth', dry_run=dry_run)
+        self.logger = logging.getLogger()
 
         self.homevar = os.path.join(str(Path.home()), 'var', root_class)
 
         self.auth_cookie_folder = os.path.join(self.homevar, 'auth_cookies')
         if not os.path.exists(self.auth_cookie_folder):
             os.makedirs(self.auth_cookie_folder)
         self.session_cookie_folder = os.path.join(self.homevar, 'session_cookies')
@@ -67,15 +67,15 @@
     def get_auth_response(self, req, callback) -> Response:
         """ If valid auth token comes fromt he client, return none
             Otherwise, it will return a response so that the client opens again the Auth Popup
         Returns:
             Response: Http response with the auth popup, or 
                       None if auth request is not needed because already are authenticated
         """
-        self.logger.debug(f'Request from host --> {req.host} | endpoint --> {req.path}')
+        self.logger.debug('Request from host --> %s | endpoint --> %s', req.host, req.path)
 
         response = None
 
         if req.form.get('revproxy_auth', None):
             session_cookie, session_cookie_name = self._creates_session_token_from_popup_data(req)
             if session_cookie_name:
                 self.logger.info('Credentials validated.')
@@ -83,23 +83,23 @@
                 response = redirect(parse.urljoin(session_cookie['host'], session_cookie['endpoint']))
                 response.set_cookie('token', session_cookie_name, max_age=COOKIE_LIFE_MINUTES*60)
             else:
                 response = self._reask_credentials(req)
         else:
             # Try to get authentication from the cookie
             cookie_name = req.cookies.get('token', None)
-            self.logger.debug(f'Incomming Session token Cookie name: {cookie_name}')
+            self.logger.debug('Incomming Session token Cookie name: %s', cookie_name)
             if cookie_name:
                 # We get a session token... lets verify if its legitimate, and still alive
                 cookie = self._get_local_session_cookie(cookie_name)
                 if cookie: # Already authenticated --> Lets tunnel info back to client
-                    self.logger.debug(f'AUTHENTICATED: Session Token Cookie {cookie_name} exists in local')
+                    self.logger.debug('AUTHENTICATED: Session Token Cookie %s exists in local', cookie_name)
                     response = callback()
                 else: # We got a session, but its no longer valid --> ask again for credentials
-                    self.logger.debug(f'NOT AUTHENTICATED: Session Token Cookie {cookie_name} DOESNT exist in local')
+                    self.logger.debug('NOT AUTHENTICATED: Session Token Cookie %s DOESNT exist in local', cookie_name)
                     response = self._reask_credentials(req, old_cookie_name=cookie_name)
             else:  # No session cookie... and no form data with credendials
                 response = self._reask_credentials(req)
 
         return response
 
     def path_redirect(self, path) -> Response:
@@ -251,19 +251,19 @@
 
     def _reask_credentials(self, req: Request, old_cookie_name: str = None) -> Response:
         new_cookie, new_cookie_name = self._build_auth_cookie(req)
         if not new_cookie: # Unable to build cookie for requested path: host unknown
             return Response(f'Host {req.host} not found on revproxy_auth config translation table',
                             status=HTTP_501_NOT_IMPLEMENTED,
                             content_type='text/plain')
-        self.logger.info(f'Creating new auth cookie {new_cookie_name} and reasking to user...')
+        self.logger.info('Creating new auth cookie %s and reasking to user...', new_cookie_name)
         self._write_cookie(new_cookie, self.auth_cookie_folder, new_cookie_name)
         response = self._build_auth_popup(new_cookie_name)
         if old_cookie_name:
-            self.logger.info(f'Deleting cookie in response: {old_cookie_name}')
+            self.logger.info('Deleting cookie in response: %s', old_cookie_name)
             self._clear_local_cookie(self.auth_cookie_folder, old_cookie_name)
         return response
 
     def _creates_session_token_from_popup_data(self, req: Request) -> str:
         """ Creates valid session token if valid credentials sent from the auth popup
         Args:
             req (Request): Request fro client... hopefully with valod auth credentials
@@ -274,31 +274,31 @@
         """
         session_cookie_name = None
         session_cookie = None
         auth_cookie_name = req.form.get('revproxy_auth', None)
         auth_cookie = self._get_local_auth_cookie(auth_cookie_name)
         if auth_cookie:
             if self._credentials_valid(req.form):
-                self.logger.info(f'Auth Local cookie {auth_cookie_name} still alive and valid.')
+                self.logger.info('Auth Local cookie %s still alive and valid.', auth_cookie_name)
                 session_cookie, session_cookie_name = self._build_session_cookie(auth_cookie)
-                self.logger.info(f'Creating new session cookie {session_cookie_name}...')
+                self.logger.info('Creating new session cookie %s...', session_cookie_name)
                 self._write_cookie(session_cookie, self.session_cookie_folder, session_cookie_name)
             else:
-                self.logger.info(f'Auth Local cookie {auth_cookie_name} still alive but credentials are invalid.')
+                self.logger.info('Auth Local cookie %s still alive but credentials are invalid.', auth_cookie_name)
             # Auth token can only be used once.
             self._clear_local_cookie(self.auth_cookie_folder, auth_cookie_name)
         else:
-            self.logger.info(f'Auth Local cookie {auth_cookie_name} doesnt exist.')
+            self.logger.info('Auth Local cookie %s doesnt exist.', auth_cookie_name)
         return session_cookie, session_cookie_name
 
     def _first_auth_and_redirect(self, req: Request) -> Response:
         cookie_name = req.form.get('revproxy_auth', None)
         cookie = self._get_local_auth_cookie(cookie_name)
         if cookie:
-            self.logger.info(f'Local cookie {cookie_name} still alive')
+            self.logger.info('Local cookie %s still alive', cookie_name)
             if self._credentials_valid(req.form):
                 self.logger.info('Credentials validated.')
                 # Search for the cookie and redirect to related URL if present
                 if cookie['method'] == 'GET':
                     response = self._call_inner_get(cookie['host'],
                                                     cookie['endpoint'],
                                                     cookie['params'],
@@ -322,15 +322,15 @@
         Returns:
             http_response: response string
         """
         if req.path == '/favicon.ico':
             cookie, cookie_name = self._build_auth_cookie(req)
             if not cookie: # Unable to build cookie for requested path: host unknown
                 return Response(req.path, status=501, content_type='text/plain')
-            self.logger.debug(f"favicon.ico requested: Directly returning from inner endpoint {cookie['host']}")
+            self.logger.debug('favicon.ico requested: Directly returning from inner endpoint %s', cookie['host'])
             if req.url == parse.urljoin(cookie['host'], req.path):
                 return Response(req.path, status=400, content_type='text/plain')
             return self._call_inner_get(host=cookie['host'],
                                         endpoint=req.path,
                                         params=req.query_string.decode("utf-8"),
                                         headers=req.headers)
 
@@ -353,20 +353,20 @@
                 # response = redirect(session_cookie['endpoint'])
                 response.set_cookie('token', session_cookie_name, max_age=COOKIE_LIFE_MINUTES*60)
             else:
                 response = self._reask_credentials(req)
         else:
             # Try to get authentication from the cookie
             cookie_name = req.cookies.get('token', None)
-            self.logger.debug(f'Incomming Session token Cookie name: {cookie_name}')
+            self.logger.debug('Incomming Session token Cookie name: %s', cookie_name)
             if cookie_name:
                 # We get a session token... lets verify if its legitimate, and still alive
                 cookie = self._get_local_session_cookie(cookie_name)
                 if cookie: # Already authenticated --> Lets tunnel info back to client
-                    self.logger.debug(f'AUTHENTICATED: Session Token Cookie {cookie_name} exists in local')
+                    self.logger.debug('AUTHENTICATED: Session Token Cookie %s exists in local', cookie_name)
                     # response = callback()
                     if req.path == '/': # If path is the root, lets go to the configured initial entrypoint.
                         method = cookie['method']
                         path = cookie['endpoint']
                         headers = {}
                         if method == 'GET':
                             params = cookie['params']
@@ -380,13 +380,13 @@
                         data = req.data
                     # Lets get the response from the internal host, and tunnel it back to client
                     if method == 'GET':
                         response = self._call_inner_get(cookie['host'], path, params, headers)
                     else:
                         response = self._call_inner_post(cookie['host'], path, data, headers)
                 else: # We got a session, but its no longer valid --> ask again for credentials
-                    self.logger.debug(f'NOT AUTHENTICATED: Session Token Cookie {cookie_name} DOESNT exist in local')
+                    self.logger.debug('NOT AUTHENTICATED: Session Token Cookie %s DOESNT exist in local', cookie_name)
                     response = self._reask_credentials(req, old_cookie_name=cookie_name)
             else:  # No session cookie... and no form data with credendials
                 response = self._reask_credentials(req)
 
         return response
```

### Comparing `revproxy_auth-0.1.6/revproxy_auth/revproxy_auth_static/css/view.css` & `revproxy_auth-0.1.7/revproxy_auth/revproxy_auth_static/css/view.css`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.6/revproxy_auth/templates/form.html` & `revproxy_auth-0.1.7/revproxy_auth/templates/form.html`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.6/revproxy_auth.egg-info/PKG-INFO` & `revproxy_auth-0.1.7/revproxy_auth.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: revproxy-auth
-Version: 0.1.6
+Version: 0.1.7
 Summary: Reverse proxy with synology authentication
 Home-page: https://github.com/Phornee/revproxy_auth
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Description: # revproxy_auth
         This class implements a reverse proxy intended to work inside a Flask server, allows to use the synology auth credentials for all your services behind the synology service proxy.
```

### Comparing `revproxy_auth-0.1.6/setup.py` & `revproxy_auth-0.1.7/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="revproxy_auth",
-    version="0.1.6",
+    version="0.1.7",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Reverse proxy with synology authentication",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/revproxy_auth",
     packages=setuptools.find_packages(),
@@ -23,12 +23,11 @@
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Topic :: Home Automation"
     ],
     install_requires=[
         'Flask>=1.1.2',
         'config_yml>=0.3.0',
-        'log_mgr>=0.0.2',
         'beautifulsoup4>=4.10.0'
     ],
     python_requires='>=3.6',
 )
```

### Comparing `revproxy_auth-0.1.6/tests/test_000.py` & `revproxy_auth-0.1.7/tests/test_000.py`

 * *Files identical despite different names*

### Comparing `revproxy_auth-0.1.6/tests/test_001.py` & `revproxy_auth-0.1.7/tests/test_001.py`

 * *Files identical despite different names*

