# Comparing `tmp/flask_signing-0.2.0.tar.gz` & `tmp/flask_signing-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_signing-0.2.0.tar", last modified: Mon Jun 12 20:08:18 2023, max compression
+gzip compressed data, was "flask_signing-0.2.1.tar", last modified: Tue Jun 13 00:44:40 2023, max compression
```

## Comparing `flask_signing-0.2.0.tar` & `flask_signing-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,22 @@
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-12 20:08:18.172595 flask_signing-0.2.0/
--rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.2.0/LICENSE
--rw-rw-r--   0 sig       (1000) sig       (1000)      690 2023-06-12 20:08:18.172595 flask_signing-0.2.0/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)     2736 2023-06-12 15:59:14.000000 flask_signing-0.2.0/README.md
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-12 20:08:18.168594 flask_signing-0.2.0/flask_signing/
--rw-rw-r--   0 sig       (1000) sig       (1000)     8210 2023-06-12 20:07:03.000000 flask_signing-0.2.0/flask_signing/__init__.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-12 20:08:18.168594 flask_signing-0.2.0/flask_signing.egg-info/
--rw-rw-r--   0 sig       (1000) sig       (1000)      690 2023-06-12 20:08:18.000000 flask_signing-0.2.0/flask_signing.egg-info/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)      264 2023-06-12 20:08:18.000000 flask_signing-0.2.0/flask_signing.egg-info/SOURCES.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-12 20:08:18.000000 flask_signing-0.2.0/flask_signing.egg-info/dependency_links.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-12 20:08:18.000000 flask_signing-0.2.0/flask_signing.egg-info/requires.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       14 2023-06-12 20:08:18.000000 flask_signing-0.2.0/flask_signing.egg-info/top_level.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-12 20:08:18.172595 flask_signing-0.2.0/setup.cfg
--rw-rw-r--   0 sig       (1000) sig       (1000)      869 2023-06-12 20:07:00.000000 flask_signing-0.2.0/setup.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-12 20:08:18.172595 flask_signing-0.2.0/tests/
--rw-rw-r--   0 sig       (1000) sig       (1000)     2996 2023-06-12 14:35:39.000000 flask_signing-0.2.0/tests/test_flask_signing.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 00:44:40.519516 flask_signing-0.2.1/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.2.1/LICENSE
+-rw-rw-r--   0 sig       (1000) sig       (1000)       99 2023-06-13 00:13:51.000000 flask_signing-0.2.1/MANIFEST.in
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3521 2023-06-13 00:44:40.519516 flask_signing-0.2.1/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)     2789 2023-06-13 00:23:09.000000 flask_signing-0.2.1/README.md
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 00:44:40.515516 flask_signing-0.2.1/docs/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.2.1/docs/combined.png
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 00:44:40.515516 flask_signing-0.2.1/docs/flask_signing/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    38642 2023-06-13 00:43:37.000000 flask_signing-0.2.1/docs/flask_signing/index.html
+-rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.2.1/docs/logo.png
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 00:44:40.515516 flask_signing-0.2.1/flask_signing/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     8165 2023-06-13 00:43:41.000000 flask_signing-0.2.1/flask_signing/__init__.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 00:44:40.519516 flask_signing-0.2.1/flask_signing.egg-info/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3521 2023-06-13 00:44:40.000000 flask_signing-0.2.1/flask_signing.egg-info/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)      338 2023-06-13 00:44:40.000000 flask_signing-0.2.1/flask_signing.egg-info/SOURCES.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-13 00:44:40.000000 flask_signing-0.2.1/flask_signing.egg-info/dependency_links.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-13 00:44:40.000000 flask_signing-0.2.1/flask_signing.egg-info/requires.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       14 2023-06-13 00:44:40.000000 flask_signing-0.2.1/flask_signing.egg-info/top_level.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-13 00:44:40.519516 flask_signing-0.2.1/setup.cfg
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1237 2023-06-13 00:43:30.000000 flask_signing-0.2.1/setup.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 00:44:40.519516 flask_signing-0.2.1/tests/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     4360 2023-06-12 20:36:20.000000 flask_signing-0.2.1/tests/test_flask_signing.py
```

### Comparing `flask_signing-0.2.0/LICENSE` & `flask_signing-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_signing-0.2.0/README.md` & `flask_signing-0.2.1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,15 @@
-[![License: BSD-3-Clause](https://img.shields.io/github/license/signebedi/Flask-Signing)](https://github.com/signebedi/Flask-Signing/blob/master/LICENSE) 
+![Signing logo](docs/combined.png)
+
+## Flask-Signing
+
+[![License: BSD-3-Clause](https://img.shields.io/github/license/signebedi/Flask-Signing?color=dark-green)](https://github.com/signebedi/Flask-Signing/blob/master/LICENSE) 
 [![PyPI version](https://badge.fury.io/py/Flask-Signing.svg)](https://pypi.org/project/flask-signing/)
 [![Flask-Signing tests](https://github.com/signebedi/Flask-Signing/workflows/tests/badge.svg)](https://github.com/signebedi/Flask-Signing/actions)
 
-
-## Flask-Signing
 a signing key extension for flask
 
 
 ### About
 
 The Flask-Signing library is a useful tool for Flask applications that requires secure and robust management of signing keys. This package aids in managing API keys, ensuring only clients with valid permissions can access your resources. Do you need to generate single-use tokens for one-time actions like email verification or password reset? Flask-Signing can handle that. In theory, it can also help manage session IDs. For applications that implement JWT or OAuth2, Flask-Signing can generate and manage the signing keys for your tokens. You can also use it to verify webhook payloads or to implement a licensing system for your software.
```

### Comparing `flask_signing-0.2.0/flask_signing/__init__.py` & `flask_signing-0.2.1/flask_signing/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 __name__ = "flask_signing"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi",]
-__version__ = "0.2.0"
+__version__ = "0.2.1"
 __license__ = "BSD-3-Clause"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 import datetime, secrets
 from flask_sqlalchemy import SQLAlchemy
 from typing import Union, List, Dict, Any
 
 class Signatures:
     """
     The Signatures class handles operations related to the creation, management, and validation 
     of signing keys in the database.
     """
-
+    
     def __init__(self, app, byte_len:int=24):
         """
         Initializes a new instance of the Signatures class.
 
         Args:
             app (Flask): A flask object to contain the context for database interactions. 
             byte_len (int, optional): The length of the generated signing keys. Defaults to 24.
@@ -149,31 +149,33 @@
         # if the signing key's scope doesn't match the required scope
         if signing_key.scope != scope:
             return False
 
         return True
 
     def get_model(self):
-        if not hasattr(self, '_model'):
-            class Signing(self.db.Model):
-                """
-                The Signing class represents the Signing table in the database.
 
-                Each instance of this class represents a row of data in the database table.
+        """
+        Generate an instance of the Signing class, which represents the Signing table in the database.
+
+        Each instance of this class represents a row of data in the database table.
 
-                Attributes:
-                    signature (str): The primary key of the Signing table. This field is unique for each entry.
-                    email (str): The email associated with a specific signing key.
-                    scope (str): The scope within which the key is valid.
-                    active (bool): The status of the signing key. If True, the key is active.
-                    timestamp (datetime): The date and time when the signing key was created.
-                    expiration (datetime): The date and time when the signing key is set to expire.
-                """
+        Attributes:
+            signature (str): The primary key of the Signing table. This field is unique for each entry.
+            email (str): The email associated with a specific signing key.
+            scope (str): The scope within which the key is valid.
+            active (bool): The status of the signing key. If True, the key is active.
+            timestamp (datetime): The date and time when the signing key was created.
+            expiration (datetime): The date and time when the signing key is set to expire.
+        """
+
+        if not hasattr(self, '_model'):
+            class Signing(self.db.Model):
                 __tablename__ = 'signing'
-                signature = self.db.Column(self.db.String, primary_key=True) 
+                signature = self.db.Column(self.db.String(1000), primary_key=True) 
                 email = self.db.Column(self.db.String(100))
                 scope = self.db.Column(self.db.String(100))
                 active = self.db.Column(self.db.Boolean)
                 timestamp = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
                 expiration = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
 
             self._model = Signing
```

### Comparing `flask_signing-0.2.0/setup.py` & `flask_signing-0.2.1/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,17 +1,27 @@
 from setuptools import setup, find_packages
 
+# Read README for long_description
+with open("README.md", "r", encoding="utf-8") as fh:
+    long_description = fh.read()
+
+# # Read requirements.txt for install_requires
+# with open("requirements.txt", "r", encoding="utf-8") as fr:
+#     install_requires = fr.read().splitlines()
+
 setup(
     name='flask_signing',
-    version='0.2.0',
+    version='0.2.1',
     url='https://github.com/signebedi/Flask-Signing',
     author='Sig Janoska-Bedi',
     author_email='signe@atreeus.com',
     description='a signing key extension for flask',
-    packages=find_packages(),  
+    long_description=long_description,
+    long_description_content_type="text/markdown",
+    packages=find_packages(),
     install_requires=[
         'Flask<3.0.0',
         'Flask-SQLAlchemy<4.0.0',
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

