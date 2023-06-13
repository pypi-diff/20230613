# Comparing `tmp/doe-dap-dl-0.2.0.tar.gz` & `tmp/doe-dap-dl-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "doe-dap-dl-0.2.0.tar", last modified: Thu Apr 27 21:02:21 2023, max compression
+gzip compressed data, was "doe-dap-dl-0.3.1.tar", last modified: Tue Jun 13 20:44:15 2023, max compression
```

## Comparing `doe-dap-dl-0.2.0.tar` & `doe-dap-dl-0.3.1.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 21:02:21.556713 doe-dap-dl-0.2.0/
--rw-rw-rw-   0        0        0     1103 2023-03-23 22:00:38.000000 doe-dap-dl-0.2.0/LICENSE.md
--rw-rw-rw-   0        0        0     1866 2023-04-27 21:02:21.554709 doe-dap-dl-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     1048 2023-04-14 22:02:21.000000 doe-dap-dl-0.2.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-27 21:02:21.426703 doe-dap-dl-0.2.0/doe_dap_dl/
--rw-rw-rw-   0        0        0       22 2023-04-11 16:40:22.000000 doe-dap-dl-0.2.0/doe_dap_dl/__init__.py
--rw-rw-rw-   0        0        0    25639 2023-04-27 20:00:16.000000 doe-dap-dl-0.2.0/doe_dap_dl/dap.py
-drwxrwxrwx   0        0        0        0 2023-04-27 21:02:21.530712 doe-dap-dl-0.2.0/doe_dap_dl/plot/
--rw-rw-rw-   0        0        0        0 2023-04-11 16:40:22.000000 doe-dap-dl-0.2.0/doe_dap_dl/plot/__init__.py
--rw-rw-rw-   0        0        0    11499 2023-04-11 16:40:22.000000 doe-dap-dl-0.2.0/doe_dap_dl/plot/plot.py
-drwxrwxrwx   0        0        0        0 2023-04-27 21:02:21.550705 doe-dap-dl-0.2.0/doe_dap_dl/utils/
--rw-rw-rw-   0        0        0        0 2023-04-11 16:40:22.000000 doe-dap-dl-0.2.0/doe_dap_dl/utils/__init__.py
--rw-rw-rw-   0        0        0      944 2023-04-11 16:40:22.000000 doe-dap-dl-0.2.0/doe_dap_dl/utils/scraper.py
-drwxrwxrwx   0        0        0        0 2023-04-27 21:02:21.505711 doe-dap-dl-0.2.0/doe_dap_dl.egg-info/
--rw-rw-rw-   0        0        0     1866 2023-04-27 21:02:21.000000 doe-dap-dl-0.2.0/doe_dap_dl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      381 2023-04-27 21:02:21.000000 doe-dap-dl-0.2.0/doe_dap_dl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 21:02:21.000000 doe-dap-dl-0.2.0/doe_dap_dl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2023-04-27 17:09:49.000000 doe-dap-dl-0.2.0/doe_dap_dl.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       34 2023-04-27 21:02:21.000000 doe-dap-dl-0.2.0/doe_dap_dl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-04-27 21:02:21.000000 doe-dap-dl-0.2.0/doe_dap_dl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-27 21:02:21.557706 doe-dap-dl-0.2.0/setup.cfg
--rw-rw-rw-   0        0        0     1291 2023-04-27 21:00:18.000000 doe-dap-dl-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:44:15.862207 doe-dap-dl-0.3.1/
+-rw-rw-rw-   0        0        0     1103 2023-03-23 22:00:38.000000 doe-dap-dl-0.3.1/LICENSE.md
+-rw-rw-rw-   0        0        0     1843 2023-06-13 20:44:15.860198 doe-dap-dl-0.3.1/PKG-INFO
+-rw-rw-rw-   0        0        0     1048 2023-04-14 22:02:21.000000 doe-dap-dl-0.3.1/README.md
+drwxrwxrwx   0        0        0        0 2023-06-13 20:44:15.792195 doe-dap-dl-0.3.1/doe_dap_dl/
+-rw-rw-rw-   0        0        0       22 2023-04-11 16:40:22.000000 doe-dap-dl-0.3.1/doe_dap_dl/__init__.py
+-rw-rw-rw-   0        0        0    26083 2023-06-13 20:30:21.000000 doe-dap-dl-0.3.1/doe_dap_dl/dap.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:44:15.844199 doe-dap-dl-0.3.1/doe_dap_dl/plot/
+-rw-rw-rw-   0        0        0        0 2023-04-11 16:40:22.000000 doe-dap-dl-0.3.1/doe_dap_dl/plot/__init__.py
+-rw-rw-rw-   0        0        0    11499 2023-04-11 16:40:22.000000 doe-dap-dl-0.3.1/doe_dap_dl/plot/plot.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:44:15.853199 doe-dap-dl-0.3.1/doe_dap_dl/utils/
+-rw-rw-rw-   0        0        0        0 2023-04-11 16:40:22.000000 doe-dap-dl-0.3.1/doe_dap_dl/utils/__init__.py
+-rw-rw-rw-   0        0        0      944 2023-04-11 16:40:22.000000 doe-dap-dl-0.3.1/doe_dap_dl/utils/scraper.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:44:15.838195 doe-dap-dl-0.3.1/doe_dap_dl.egg-info/
+-rw-rw-rw-   0        0        0     1843 2023-06-13 20:44:15.000000 doe-dap-dl-0.3.1/doe_dap_dl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      395 2023-06-13 20:44:15.000000 doe-dap-dl-0.3.1/doe_dap_dl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-13 20:44:15.000000 doe-dap-dl-0.3.1/doe_dap_dl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2023-04-27 17:09:49.000000 doe-dap-dl-0.3.1/doe_dap_dl.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       34 2023-06-13 20:44:15.000000 doe-dap-dl-0.3.1/doe_dap_dl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-06-13 20:44:15.000000 doe-dap-dl-0.3.1/doe_dap_dl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-06-13 20:44:15.863201 doe-dap-dl-0.3.1/setup.cfg
+-rw-rw-rw-   0        0        0     1291 2023-06-13 20:44:05.000000 doe-dap-dl-0.3.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-13 20:44:15.856196 doe-dap-dl-0.3.1/tests/
+-rw-rw-rw-   0        0        0    40764 2023-04-11 16:40:22.000000 doe-dap-dl-0.3.1/tests/test.py
```

### Comparing `doe-dap-dl-0.2.0/LICENSE.md` & `doe-dap-dl-0.3.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `doe-dap-dl-0.2.0/PKG-INFO` & `doe-dap-dl-0.3.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: doe-dap-dl
-Version: 0.2.0
+Version: 0.3.1
 Summary: Packages for Jupyter Notebook users to interact with data from A2e, Livewire, and the SPP data platform.
 Home-page: https://github.com/DAP-platform/dap-py
 Author: DAP-Platform
 Author-email: dapteam@pnnl.gov
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
@@ -45,9 +44,7 @@
 # download files
 files = a2e.download_files(file_names)
 ```
 
 [Main docs](https://github.com/DAP-platform/dap-py/blob/master/docs/doe_dap_dl.md)
 [Search query docs](https://github.com/DAP-platform/dap-py/blob/master/docs/download-README.md)
 [Plotting docs](https://github.com/DAP-platform/dap-py/blob/master/docs/plotting.md)
-
-
```

### Comparing `doe-dap-dl-0.2.0/README.md` & `doe-dap-dl-0.3.1/README.md`

 * *Files identical despite different names*

### Comparing `doe-dap-dl-0.2.0/doe_dap_dl/dap.py` & `doe-dap-dl-0.3.1/doe_dap_dl/dap.py`

 * *Files 5% similar despite different names*

```diff
@@ -90,16 +90,16 @@
         else:
             self.__print("Certificate not found.")
             self.__print_setup_authentication()
 
         if found_cert:
             self.__read_cert()
 
-            if self.__cert_is_valid():
-                self.__create_cert_auth()
+            if self.renew_cert(quiet=True):
+                self.__create_cert_auth_token()
                 self.__print(
                     "Authenticaion successfully created using valid certificate."
                 )
             else:
                 self.__print("Certificate was invalid.")
                 self.__print_setup_authentication()
 
@@ -134,27 +134,27 @@
 
         if not self.__validate_response(response):
             return
 
         self._cert = json.loads(response.text)["cert"]
         self.__save_cert()
 
-    def __create_cert_auth(self):
+    def __create_cert_auth_token(self):
         """Given an existing certificate, create an auth token"""
         if not self._cert:
             raise ValueError("Could not create cert auth, missing certificate.")
 
         encoded_cert = base64.b64encode(self._cert.encode("utf-8")).decode("ascii")
         self._auth = {"Authorization": f"Cert {encoded_cert}"}
 
     def __request_cert_auth(self, params):
         """Requests certificate and creates auth token"""
         try:
             self.__request_cert(params)
-            self.__create_cert_auth()
+            self.__create_cert_auth_token()
         except BadStatusCodeError:
             self.__print("Incorrect credentials")
             return False
         except Exception as e:
             self.__print(e)
             return False
         return True
@@ -190,16 +190,16 @@
             username (str, optional): Username, if None it will prompt. Defaults to None.
             password (str, optional): Password, if None it will prompt. Defaults to None.
 
         Returns:
             bool: Whether the requested certificate was valid.
         """
 
-        if self.__cert_is_valid():
-            self.__print("Valid certificate already created")
+        if self.renew_cert(quiet=True):
+            self.__print("Valid certificate already created, it has been renewed.")
             return True
 
         params = {
             "username": username or input("username: "),
             "password": password or getpass("password: "),
         }
 
@@ -207,15 +207,15 @@
             f"Setting up certificate authentication for user {params['username']}..."
         )
 
         if not self.__request_cert_auth(params):
             self.__print("Requesting a certificate failed.")
             return False
 
-        valid = self.__cert_is_valid()
+        valid = self.renew_cert(quiet=True)
         if valid:
             self.__print(
                 f"Successfully set up certificate authentication for user {params['username']}."
             )
         else:
             self.__print(
                 "Setting up certificate authentication failed: certificate was invalid."
@@ -230,17 +230,17 @@
             username (str, optional): Username, if None it will prompt. Defaults to None.
             password (str, optional): Password, if None it will prompt. Defaults to None.
             authcode (str, optional): Two factor auth code, if None it will prompt. Defaults to None.
 
         Returns:
             bool: Whether the requested certificate was valid.
         """
-        # we can't tell what kind of certification they
-        # have with our current API, so we'll just make
-        # them a new one
+        if self.renew_cert(quiet=True):
+            self.__print("Valid certificate already created, it has been renewed.")
+            return True
 
         params = {
             "username": username or input("username: "),
             "password": password or getpass("password: "),
             "authcode": authcode or getpass("authcode: "),
         }
 
@@ -248,46 +248,54 @@
             f"Setting up two-factor authentication for user {params['username']}..."
         )
 
         if not self.__request_cert_auth(params):
             self.__print(f"Setting up two-factor authentication failed.")
             return False
 
-        valid = self.__cert_is_valid()
+        valid = self.renew_cert(quiet=True)
         if valid:
             self.__print(
                 f"Successfully set up two-factor authentication for user {params['username']}."
             )
         else:
             self.__print(
                 "Setting up two-factor authentication failed: created certificate was invalid."
             )
         return valid
 
-    def __renew_cert(self):
+    def renew_cert(self, quiet=False):
         """Renews the certificate"""
         if not self._cert:
-            raise ValueError("No certificate to renew")
+            if not quiet:
+                self.__print("No certificate to renew")
+            return False
+
+        if not quiet:
+            self.__print("Renewing existing certificate...")
 
         params = {
             "cert": self._cert,
             "action": "renew",
         }
 
         resp = requests.put(f"{self._api_url}/creds", params=params)
 
         if resp.status_code != 200:
-            raise BadStatusCodeError(resp)
-
-        return "cert" in resp.json()
+            if not quiet:
+                self.__print(f"Request to renew certificate returned bad status code {resp.status_code}")
+            return False
 
-    def __cert_is_valid(self):
-        try:
-            return self.__renew_cert()
-        except (ValueError, BadStatusCodeError) as e:
+        if "cert" in resp.json():
+            if not quiet:
+                self.__print("Certificate successfully renewed")
+            return True
+        else:
+            if not quiet:
+                self.__print("Failed to renew certificate, it may be expired or invalid.")
             return False
 
     def __save_cert(self):
         """Save the cert to path"""
         path = Path(self.save_cert_dir) / f".{self.host_URL}.cert"
         with open(path, "w") as cf:
             cf.write(self._cert)
```

### Comparing `doe-dap-dl-0.2.0/doe_dap_dl/plot/plot.py` & `doe-dap-dl-0.3.1/doe_dap_dl/plot/plot.py`

 * *Files identical despite different names*

### Comparing `doe-dap-dl-0.2.0/doe_dap_dl/utils/scraper.py` & `doe-dap-dl-0.3.1/doe_dap_dl/utils/scraper.py`

 * *Files identical despite different names*

### Comparing `doe-dap-dl-0.2.0/doe_dap_dl.egg-info/PKG-INFO` & `doe-dap-dl-0.3.1/doe_dap_dl.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: doe-dap-dl
-Version: 0.2.0
+Version: 0.3.1
 Summary: Packages for Jupyter Notebook users to interact with data from A2e, Livewire, and the SPP data platform.
 Home-page: https://github.com/DAP-platform/dap-py
 Author: DAP-Platform
 Author-email: dapteam@pnnl.gov
 License: MIT
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Topic :: Scientific/Engineering
@@ -45,9 +44,7 @@
 # download files
 files = a2e.download_files(file_names)
 ```
 
 [Main docs](https://github.com/DAP-platform/dap-py/blob/master/docs/doe_dap_dl.md)
 [Search query docs](https://github.com/DAP-platform/dap-py/blob/master/docs/download-README.md)
 [Plotting docs](https://github.com/DAP-platform/dap-py/blob/master/docs/plotting.md)
-
-
```

### Comparing `doe-dap-dl-0.2.0/setup.py` & `doe-dap-dl-0.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pathlib import Path
 import setuptools
 
 # The text of the README file
 README = Path("README.md").read_text()
 
-version = "0.2.0"
+version = "0.3.1"
 assert "." in version
 
 setuptools.setup(
     name="doe-dap-dl",
     version=version,
     description="Packages for Jupyter Notebook users to interact with data from A2e, Livewire, and the SPP data platform.",
     long_description=README,
```

