# Comparing `tmp/flask_signing-0.2.1.tar.gz` & `tmp/flask_signing-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flask_signing-0.2.1.tar", last modified: Tue Jun 13 00:44:40 2023, max compression
+gzip compressed data, was "flask_signing-0.3.0.tar", last modified: Tue Jun 13 20:48:32 2023, max compression
```

## Comparing `flask_signing-0.2.1.tar` & `flask_signing-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 00:44:40.519516 flask_signing-0.2.1/
--rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.2.1/LICENSE
--rw-rw-r--   0 sig       (1000) sig       (1000)       99 2023-06-13 00:13:51.000000 flask_signing-0.2.1/MANIFEST.in
--rw-rw-r--   0 sig       (1000) sig       (1000)     3521 2023-06-13 00:44:40.519516 flask_signing-0.2.1/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)     2789 2023-06-13 00:23:09.000000 flask_signing-0.2.1/README.md
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 00:44:40.515516 flask_signing-0.2.1/docs/
--rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.2.1/docs/combined.png
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 00:44:40.515516 flask_signing-0.2.1/docs/flask_signing/
--rw-rw-r--   0 sig       (1000) sig       (1000)    38642 2023-06-13 00:43:37.000000 flask_signing-0.2.1/docs/flask_signing/index.html
--rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.2.1/docs/logo.png
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 00:44:40.515516 flask_signing-0.2.1/flask_signing/
--rw-rw-r--   0 sig       (1000) sig       (1000)     8165 2023-06-13 00:43:41.000000 flask_signing-0.2.1/flask_signing/__init__.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 00:44:40.519516 flask_signing-0.2.1/flask_signing.egg-info/
--rw-rw-r--   0 sig       (1000) sig       (1000)     3521 2023-06-13 00:44:40.000000 flask_signing-0.2.1/flask_signing.egg-info/PKG-INFO
--rw-rw-r--   0 sig       (1000) sig       (1000)      338 2023-06-13 00:44:40.000000 flask_signing-0.2.1/flask_signing.egg-info/SOURCES.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-13 00:44:40.000000 flask_signing-0.2.1/flask_signing.egg-info/dependency_links.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-13 00:44:40.000000 flask_signing-0.2.1/flask_signing.egg-info/requires.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       14 2023-06-13 00:44:40.000000 flask_signing-0.2.1/flask_signing.egg-info/top_level.txt
--rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-13 00:44:40.519516 flask_signing-0.2.1/setup.cfg
--rw-rw-r--   0 sig       (1000) sig       (1000)     1237 2023-06-13 00:43:30.000000 flask_signing-0.2.1/setup.py
-drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 00:44:40.519516 flask_signing-0.2.1/tests/
--rw-rw-r--   0 sig       (1000) sig       (1000)     4360 2023-06-12 20:36:20.000000 flask_signing-0.2.1/tests/test_flask_signing.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 20:48:32.950978 flask_signing-0.3.0/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1503 2023-06-11 20:13:39.000000 flask_signing-0.3.0/LICENSE
+-rw-rw-r--   0 sig       (1000) sig       (1000)      117 2023-06-13 00:47:00.000000 flask_signing-0.3.0/MANIFEST.in
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3232 2023-06-13 20:48:32.950978 flask_signing-0.3.0/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)     2500 2023-06-13 19:42:53.000000 flask_signing-0.3.0/README.md
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 20:48:32.946978 flask_signing-0.3.0/docs/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    78889 2023-06-13 00:10:22.000000 flask_signing-0.3.0/docs/combined.png
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 20:48:32.946978 flask_signing-0.3.0/docs/flask_signing/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    45030 2023-06-13 20:45:57.000000 flask_signing-0.3.0/docs/flask_signing/index.html
+-rw-rw-r--   0 sig       (1000) sig       (1000)    65777 2023-06-13 00:01:06.000000 flask_signing-0.3.0/docs/logo.png
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 20:48:32.946978 flask_signing-0.3.0/flask_signing/
+-rw-rw-r--   0 sig       (1000) sig       (1000)    10013 2023-06-13 20:45:04.000000 flask_signing-0.3.0/flask_signing/__init__.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 20:48:32.950978 flask_signing-0.3.0/flask_signing.egg-info/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     3232 2023-06-13 20:48:32.000000 flask_signing-0.3.0/flask_signing.egg-info/PKG-INFO
+-rw-rw-r--   0 sig       (1000) sig       (1000)      338 2023-06-13 20:48:32.000000 flask_signing-0.3.0/flask_signing.egg-info/SOURCES.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)        1 2023-06-13 20:48:32.000000 flask_signing-0.3.0/flask_signing.egg-info/dependency_links.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       35 2023-06-13 20:48:32.000000 flask_signing-0.3.0/flask_signing.egg-info/requires.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       14 2023-06-13 20:48:32.000000 flask_signing-0.3.0/flask_signing.egg-info/top_level.txt
+-rw-rw-r--   0 sig       (1000) sig       (1000)       38 2023-06-13 20:48:32.950978 flask_signing-0.3.0/setup.cfg
+-rw-rw-r--   0 sig       (1000) sig       (1000)     1237 2023-06-13 20:47:12.000000 flask_signing-0.3.0/setup.py
+drwxrwxr-x   0 sig       (1000) sig       (1000)        0 2023-06-13 20:48:32.950978 flask_signing-0.3.0/tests/
+-rw-rw-r--   0 sig       (1000) sig       (1000)     4897 2023-06-13 20:39:09.000000 flask_signing-0.3.0/tests/test_flask_signing.py
```

### Comparing `flask_signing-0.2.1/LICENSE` & `flask_signing-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flask_signing-0.2.1/PKG-INFO` & `flask_signing-0.3.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask_signing
-Version: 0.2.1
+Version: 0.3.0
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -26,15 +26,15 @@
 [![Flask-Signing tests](https://github.com/signebedi/Flask-Signing/workflows/tests/badge.svg)](https://github.com/signebedi/Flask-Signing/actions)
 
 a signing key extension for flask
 
 
 ### About
 
-The Flask-Signing library is a useful tool for Flask applications that requires secure and robust management of signing keys. This package aids in managing API keys, ensuring only clients with valid permissions can access your resources. Do you need to generate single-use tokens for one-time actions like email verification or password reset? Flask-Signing can handle that. In theory, it can also help manage session IDs. For applications that implement JWT or OAuth2, Flask-Signing can generate and manage the signing keys for your tokens. You can also use it to verify webhook payloads or to implement a licensing system for your software. 
+The Flask-Signing library is a useful tool for Flask applications that require secure and robust management of signing keys. Do you need to generate single-use tokens for one-time actions like email verification or password reset? Flask-Signing can handle that. Are you looking for a simple method for managing API keys? Look no further. 
 
 ### Installation
 
 First, install the flask_signing package. You can do this with pip:
 
 ```bash
 pip install flask_signing
@@ -69,10 +69,10 @@
 @app.route('/expire/<key>')
 def expire(key):
     expired = signatures.expire_key(key)
     return f'Key expired: {expired}'
     
 ```
 
-In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. Finally, you can expire a key using the /expier/<key> route.
+In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. Finally, you can expire a key using the /expire/<key> route described above.
 
 Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
```

### Comparing `flask_signing-0.2.1/README.md` & `flask_signing-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 [![Flask-Signing tests](https://github.com/signebedi/Flask-Signing/workflows/tests/badge.svg)](https://github.com/signebedi/Flask-Signing/actions)
 
 a signing key extension for flask
 
 
 ### About
 
-The Flask-Signing library is a useful tool for Flask applications that requires secure and robust management of signing keys. This package aids in managing API keys, ensuring only clients with valid permissions can access your resources. Do you need to generate single-use tokens for one-time actions like email verification or password reset? Flask-Signing can handle that. In theory, it can also help manage session IDs. For applications that implement JWT or OAuth2, Flask-Signing can generate and manage the signing keys for your tokens. You can also use it to verify webhook payloads or to implement a licensing system for your software. 
+The Flask-Signing library is a useful tool for Flask applications that require secure and robust management of signing keys. Do you need to generate single-use tokens for one-time actions like email verification or password reset? Flask-Signing can handle that. Are you looking for a simple method for managing API keys? Look no further. 
 
 ### Installation
 
 First, install the flask_signing package. You can do this with pip:
 
 ```bash
 pip install flask_signing
@@ -50,10 +50,10 @@
 @app.route('/expire/<key>')
 def expire(key):
     expired = signatures.expire_key(key)
     return f'Key expired: {expired}'
     
 ```
 
-In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. Finally, you can expire a key using the /expier/<key> route.
+In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. Finally, you can expire a key using the /expire/<key> route described above.
 
 Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
```

### Comparing `flask_signing-0.2.1/docs/combined.png` & `flask_signing-0.3.0/docs/combined.png`

 * *Files identical despite different names*

### Comparing `flask_signing-0.2.1/docs/flask_signing/index.html` & `flask_signing-0.3.0/docs/flask_signing/index.html`

 * *Files 5% similar despite different names*

```diff
@@ -25,20 +25,21 @@
 <details class="source">
 <summary>
 <span>Expand source code</span>
 </summary>
 <pre><code class="python">__name__ = &#34;flask_signing&#34;
 __author__ = &#34;Sig Janoska-Bedi&#34;
 __credits__ = [&#34;Sig Janoska-Bedi&#34;,]
-__version__ = &#34;0.2.1&#34;
+__version__ = &#34;0.3.0&#34;
 __license__ = &#34;BSD-3-Clause&#34;
 __maintainer__ = &#34;Sig Janoska-Bedi&#34;
 __email__ = &#34;signe@atreeus.com&#34;
 
 import datetime, secrets
+from sqlalchemy import func, literal
 from flask_sqlalchemy import SQLAlchemy
 from typing import Union, List, Dict, Any
 
 class Signatures:
     &#34;&#34;&#34;
     The Signatures class handles operations related to the creation, management, and validation 
     of signing keys in the database.
@@ -96,17 +97,22 @@
         Signing = self.get_model()
 
         # loop until a unique key is generated
         while True:
             key = self.generate_key()
             if not Signing.query.filter_by(signature=key).first(): break
 
+        # Convert scope to a list if it&#39;s a string
+        if isinstance(scope, str):
+            scope = [scope]
+
         new_key = Signing(
                         signature=key, 
-                        scope=scope.lower() if scope else &#34;&#34;,
+                        # scope=scope.lower() if scope else &#34;&#34;,
+                        scope=[s.lower() for s in scope] if scope else [],
                         email=email.lower() if email else &#34;&#34;, 
                         active=active,
                         expiration=(datetime.datetime.utcnow() + datetime.timedelta(hours=expiration)) if expiration else 0,
                         timestamp=datetime.datetime.utcnow(),
         )
 
         self.db.session.add(new_key)
@@ -170,18 +176,26 @@
             self.expire_key(signature)
             return False
 
         # if the signing key is set to inactive
         if not signing_key.active:
             return False
 
-        # if the signing key&#39;s scope doesn&#39;t match the required scope
-        if signing_key.scope != scope:
+        # Convert scope to a list if it&#39;s a string
+        if isinstance(scope, str):
+            scope = [scope]
+
+        # if the signing key&#39;s scope doesn&#39;t match any of the required scopes
+        if not set(scope).intersection(set(signing_key.scope)):
             return False
 
+        # # if the signing key&#39;s scope doesn&#39;t match the required scope
+        # if signing_key.scope != scope:
+        #     return False
+
         return True
 
     def get_model(self):
 
         &#34;&#34;&#34;
         Generate an instance of the Signing class, which represents the Signing table in the database.
 
@@ -197,15 +211,17 @@
         &#34;&#34;&#34;
 
         if not hasattr(self, &#39;_model&#39;):
             class Signing(self.db.Model):
                 __tablename__ = &#39;signing&#39;
                 signature = self.db.Column(self.db.String(1000), primary_key=True) 
                 email = self.db.Column(self.db.String(100))
-                scope = self.db.Column(self.db.String(100))
+                # scope = self.db.Column(self.db.String(100))
+                # scope = self.db.Column(self.db.MutableList.as_mutable(self.db.String(100)), default=[]),
+                scope = self.db.Column(self.db.JSON())
                 active = self.db.Column(self.db.Boolean)
                 timestamp = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
                 expiration = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
 
             self._model = Signing
 
         return self._model
@@ -230,25 +246,55 @@
 
         Signing = self.get_model()
 
         query = Signing.query
 
         if active is not None:
             query = query.filter(Signing.active == active)
+
+        # Convert scope to a list if it&#39;s a string
+        if isinstance(scope, str):
+            scope = [scope]
+
         if scope:
-            query = query.filter(Signing.scope == scope)
+
+            for s in scope:
+                # https://stackoverflow.com/a/44250678/13301284
+                query = query.filter(Signing.scope.comparator.contains(s))
+
+                # https://stackoverflow.com/a/39470478/13301284
+                # query = query.filter(func.json_contains(Signing.scope, s) == 1)
+                # query = query.filter(literal(s).bool_op(&#39;MEMBER OF&#39;)(Signing.scope.self_group()))
+                
+            # query = query.filter(Signing.scope.in_(scope))
+            
+        # if scope:
+        #     query = query.filter(Signing.scope == scope)
+
         if email:
             query = query.filter(Signing.email == email)
 
         result = query.all()
 
         if not result:
             return False
 
-        return [{&#39;signature&#39;: key.signature, &#39;email&#39;: key.email, &#39;scope&#39;: key.scope, &#39;active&#39;: key.active, &#39;timestamp&#39;: key.timestamp, &#39;expiration&#39;: key.expiration} for key in result]</code></pre>
+        return [{&#39;signature&#39;: key.signature, &#39;email&#39;: key.email, &#39;scope&#39;: key.scope, &#39;active&#39;: key.active, &#39;timestamp&#39;: key.timestamp, &#39;expiration&#39;: key.expiration} for key in result]
+
+    def query_all(self) -&gt; List[Dict[str, Any]]:
+
+        &#34;&#34;&#34;
+        Query all values in the Signing table.
+        If no keys are found, it returns an empty list.
+
+        Returns:
+            List[Dict[str, Any]]: A list of dictionaries where each dictionary contains the details of a signing key.
+
+        &#34;&#34;&#34;
+        return [{&#39;signature&#39;: key.signature, &#39;email&#39;: key.email, &#39;scope&#39;: key.scope, &#39;active&#39;: key.active, &#39;timestamp&#39;: key.timestamp, &#39;expiration&#39;: key.expiration} for key in self.get_model().query.all()]</code></pre>
 </details>
 </section>
 <section>
 </section>
 <section>
 </section>
 <section>
@@ -333,17 +379,22 @@
         Signing = self.get_model()
 
         # loop until a unique key is generated
         while True:
             key = self.generate_key()
             if not Signing.query.filter_by(signature=key).first(): break
 
+        # Convert scope to a list if it&#39;s a string
+        if isinstance(scope, str):
+            scope = [scope]
+
         new_key = Signing(
                         signature=key, 
-                        scope=scope.lower() if scope else &#34;&#34;,
+                        # scope=scope.lower() if scope else &#34;&#34;,
+                        scope=[s.lower() for s in scope] if scope else [],
                         email=email.lower() if email else &#34;&#34;, 
                         active=active,
                         expiration=(datetime.datetime.utcnow() + datetime.timedelta(hours=expiration)) if expiration else 0,
                         timestamp=datetime.datetime.utcnow(),
         )
 
         self.db.session.add(new_key)
@@ -407,18 +458,26 @@
             self.expire_key(signature)
             return False
 
         # if the signing key is set to inactive
         if not signing_key.active:
             return False
 
-        # if the signing key&#39;s scope doesn&#39;t match the required scope
-        if signing_key.scope != scope:
+        # Convert scope to a list if it&#39;s a string
+        if isinstance(scope, str):
+            scope = [scope]
+
+        # if the signing key&#39;s scope doesn&#39;t match any of the required scopes
+        if not set(scope).intersection(set(signing_key.scope)):
             return False
 
+        # # if the signing key&#39;s scope doesn&#39;t match the required scope
+        # if signing_key.scope != scope:
+        #     return False
+
         return True
 
     def get_model(self):
 
         &#34;&#34;&#34;
         Generate an instance of the Signing class, which represents the Signing table in the database.
 
@@ -434,15 +493,17 @@
         &#34;&#34;&#34;
 
         if not hasattr(self, &#39;_model&#39;):
             class Signing(self.db.Model):
                 __tablename__ = &#39;signing&#39;
                 signature = self.db.Column(self.db.String(1000), primary_key=True) 
                 email = self.db.Column(self.db.String(100))
-                scope = self.db.Column(self.db.String(100))
+                # scope = self.db.Column(self.db.String(100))
+                # scope = self.db.Column(self.db.MutableList.as_mutable(self.db.String(100)), default=[]),
+                scope = self.db.Column(self.db.JSON())
                 active = self.db.Column(self.db.Boolean)
                 timestamp = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
                 expiration = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
 
             self._model = Signing
 
         return self._model
@@ -467,25 +528,55 @@
 
         Signing = self.get_model()
 
         query = Signing.query
 
         if active is not None:
             query = query.filter(Signing.active == active)
+
+        # Convert scope to a list if it&#39;s a string
+        if isinstance(scope, str):
+            scope = [scope]
+
         if scope:
-            query = query.filter(Signing.scope == scope)
+
+            for s in scope:
+                # https://stackoverflow.com/a/44250678/13301284
+                query = query.filter(Signing.scope.comparator.contains(s))
+
+                # https://stackoverflow.com/a/39470478/13301284
+                # query = query.filter(func.json_contains(Signing.scope, s) == 1)
+                # query = query.filter(literal(s).bool_op(&#39;MEMBER OF&#39;)(Signing.scope.self_group()))
+                
+            # query = query.filter(Signing.scope.in_(scope))
+            
+        # if scope:
+        #     query = query.filter(Signing.scope == scope)
+
         if email:
             query = query.filter(Signing.email == email)
 
         result = query.all()
 
         if not result:
             return False
 
-        return [{&#39;signature&#39;: key.signature, &#39;email&#39;: key.email, &#39;scope&#39;: key.scope, &#39;active&#39;: key.active, &#39;timestamp&#39;: key.timestamp, &#39;expiration&#39;: key.expiration} for key in result]</code></pre>
+        return [{&#39;signature&#39;: key.signature, &#39;email&#39;: key.email, &#39;scope&#39;: key.scope, &#39;active&#39;: key.active, &#39;timestamp&#39;: key.timestamp, &#39;expiration&#39;: key.expiration} for key in result]
+
+    def query_all(self) -&gt; List[Dict[str, Any]]:
+
+        &#34;&#34;&#34;
+        Query all values in the Signing table.
+        If no keys are found, it returns an empty list.
+
+        Returns:
+            List[Dict[str, Any]]: A list of dictionaries where each dictionary contains the details of a signing key.
+
+        &#34;&#34;&#34;
+        return [{&#39;signature&#39;: key.signature, &#39;email&#39;: key.email, &#39;scope&#39;: key.scope, &#39;active&#39;: key.active, &#39;timestamp&#39;: key.timestamp, &#39;expiration&#39;: key.expiration} for key in self.get_model().query.all()]</code></pre>
 </details>
 <h3>Methods</h3>
 <dl>
 <dt id="flask_signing.Signatures.expire_key"><code class="name flex">
 <span>def <span class="ident">expire_key</span></span>(<span>self, key)</span>
 </code></dt>
 <dd>
@@ -614,24 +705,54 @@
     &#34;&#34;&#34;
 
     if not hasattr(self, &#39;_model&#39;):
         class Signing(self.db.Model):
             __tablename__ = &#39;signing&#39;
             signature = self.db.Column(self.db.String(1000), primary_key=True) 
             email = self.db.Column(self.db.String(100))
-            scope = self.db.Column(self.db.String(100))
+            # scope = self.db.Column(self.db.String(100))
+            # scope = self.db.Column(self.db.MutableList.as_mutable(self.db.String(100)), default=[]),
+            scope = self.db.Column(self.db.JSON())
             active = self.db.Column(self.db.Boolean)
             timestamp = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
             expiration = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
 
         self._model = Signing
 
     return self._model</code></pre>
 </details>
 </dd>
+<dt id="flask_signing.Signatures.query_all"><code class="name flex">
+<span>def <span class="ident">query_all</span></span>(<span>self) ‑> List[Dict[str, Any]]</span>
+</code></dt>
+<dd>
+<div class="desc"><p>Query all values in the Signing table.
+If no keys are found, it returns an empty list.</p>
+<h2 id="returns">Returns</h2>
+<dl>
+<dt><code>List[Dict[str, Any]]</code></dt>
+<dd>A list of dictionaries where each dictionary contains the details of a signing key.</dd>
+</dl></div>
+<details class="source">
+<summary>
+<span>Expand source code</span>
+</summary>
+<pre><code class="python">def query_all(self) -&gt; List[Dict[str, Any]]:
+
+    &#34;&#34;&#34;
+    Query all values in the Signing table.
+    If no keys are found, it returns an empty list.
+
+    Returns:
+        List[Dict[str, Any]]: A list of dictionaries where each dictionary contains the details of a signing key.
+
+    &#34;&#34;&#34;
+    return [{&#39;signature&#39;: key.signature, &#39;email&#39;: key.email, &#39;scope&#39;: key.scope, &#39;active&#39;: key.active, &#39;timestamp&#39;: key.timestamp, &#39;expiration&#39;: key.expiration} for key in self.get_model().query.all()]</code></pre>
+</details>
+</dd>
 <dt id="flask_signing.Signatures.query_keys"><code class="name flex">
 <span>def <span class="ident">query_keys</span></span>(<span>self, active: bool = None, scope: str = None, email: str = None) ‑> Union[List[Dict[str, Any]], bool]</span>
 </code></dt>
 <dd>
 <div class="desc"><p>Query signing keys by active status, scope, and email.</p>
 <p>This function returns a list of signing keys that match the provided parameters.
 If no keys are found, it returns False.</p>
@@ -673,16 +794,34 @@
 
     Signing = self.get_model()
 
     query = Signing.query
 
     if active is not None:
         query = query.filter(Signing.active == active)
+
+    # Convert scope to a list if it&#39;s a string
+    if isinstance(scope, str):
+        scope = [scope]
+
     if scope:
-        query = query.filter(Signing.scope == scope)
+
+        for s in scope:
+            # https://stackoverflow.com/a/44250678/13301284
+            query = query.filter(Signing.scope.comparator.contains(s))
+
+            # https://stackoverflow.com/a/39470478/13301284
+            # query = query.filter(func.json_contains(Signing.scope, s) == 1)
+            # query = query.filter(literal(s).bool_op(&#39;MEMBER OF&#39;)(Signing.scope.self_group()))
+            
+        # query = query.filter(Signing.scope.in_(scope))
+        
+    # if scope:
+    #     query = query.filter(Signing.scope == scope)
+
     if email:
         query = query.filter(Signing.email == email)
 
     result = query.all()
 
     if not result:
         return False
@@ -744,18 +883,26 @@
         self.expire_key(signature)
         return False
 
     # if the signing key is set to inactive
     if not signing_key.active:
         return False
 
-    # if the signing key&#39;s scope doesn&#39;t match the required scope
-    if signing_key.scope != scope:
+    # Convert scope to a list if it&#39;s a string
+    if isinstance(scope, str):
+        scope = [scope]
+
+    # if the signing key&#39;s scope doesn&#39;t match any of the required scopes
+    if not set(scope).intersection(set(signing_key.scope)):
         return False
 
+    # # if the signing key&#39;s scope doesn&#39;t match the required scope
+    # if signing_key.scope != scope:
+    #     return False
+
     return True</code></pre>
 </details>
 </dd>
 <dt id="flask_signing.Signatures.write_key_to_database"><code class="name flex">
 <span>def <span class="ident">write_key_to_database</span></span>(<span>self, scope: str = None, expiration: int = 1, active: bool = True, email: str = None) ‑> str</span>
 </code></dt>
 <dd>
@@ -801,17 +948,22 @@
     Signing = self.get_model()
 
     # loop until a unique key is generated
     while True:
         key = self.generate_key()
         if not Signing.query.filter_by(signature=key).first(): break
 
+    # Convert scope to a list if it&#39;s a string
+    if isinstance(scope, str):
+        scope = [scope]
+
     new_key = Signing(
                     signature=key, 
-                    scope=scope.lower() if scope else &#34;&#34;,
+                    # scope=scope.lower() if scope else &#34;&#34;,
+                    scope=[s.lower() for s in scope] if scope else [],
                     email=email.lower() if email else &#34;&#34;, 
                     active=active,
                     expiration=(datetime.datetime.utcnow() + datetime.timedelta(hours=expiration)) if expiration else 0,
                     timestamp=datetime.datetime.utcnow(),
     )
 
     self.db.session.add(new_key)
@@ -835,14 +987,15 @@
 <ul>
 <li>
 <h4><code><a title="flask_signing.Signatures" href="#flask_signing.Signatures">Signatures</a></code></h4>
 <ul class="">
 <li><code><a title="flask_signing.Signatures.expire_key" href="#flask_signing.Signatures.expire_key">expire_key</a></code></li>
 <li><code><a title="flask_signing.Signatures.generate_key" href="#flask_signing.Signatures.generate_key">generate_key</a></code></li>
 <li><code><a title="flask_signing.Signatures.get_model" href="#flask_signing.Signatures.get_model">get_model</a></code></li>
+<li><code><a title="flask_signing.Signatures.query_all" href="#flask_signing.Signatures.query_all">query_all</a></code></li>
 <li><code><a title="flask_signing.Signatures.query_keys" href="#flask_signing.Signatures.query_keys">query_keys</a></code></li>
 <li><code><a title="flask_signing.Signatures.verify_signature" href="#flask_signing.Signatures.verify_signature">verify_signature</a></code></li>
 <li><code><a title="flask_signing.Signatures.write_key_to_database" href="#flask_signing.Signatures.write_key_to_database">write_key_to_database</a></code></li>
 </ul>
 </li>
 </ul>
 </li>
```

#### html2text {}

```diff
@@ -5,20 +5,21 @@
 
 
 ****** Package flask_signing ******
     Expand source code
 __name__ = "flask_signing"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi",]
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 __license__ = "BSD-3-Clause"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 import datetime, secrets
+from sqlalchemy import func, literal
 from flask_sqlalchemy import SQLAlchemy
 from typing import Union, List, Dict, Any
 
 class Signatures:
     """
     The Signatures class handles operations related to the creation,
 management, and validation
@@ -88,17 +89,22 @@
         Signing = self.get_model()
 
         # loop until a unique key is generated
         while True:
             key = self.generate_key()
             if not Signing.query.filter_by(signature=key).first(): break
 
+        # Convert scope to a list if it's a string
+        if isinstance(scope, str):
+            scope = [scope]
+
         new_key = Signing(
                         signature=key,
-                        scope=scope.lower() if scope else "",
+                        # scope=scope.lower() if scope else "",
+                        scope=[s.lower() for s in scope] if scope else [],
                         email=email.lower() if email else "",
                         active=active,
                         expiration=(datetime.datetime.utcnow() +
 datetime.timedelta(hours=expiration)) if expiration else 0,
                         timestamp=datetime.datetime.utcnow(),
         )
 
@@ -169,18 +175,26 @@
             self.expire_key(signature)
             return False
 
         # if the signing key is set to inactive
         if not signing_key.active:
             return False
 
-        # if the signing key's scope doesn't match the required scope
-        if signing_key.scope != scope:
+        # Convert scope to a list if it's a string
+        if isinstance(scope, str):
+            scope = [scope]
+
+        # if the signing key's scope doesn't match any of the required scopes
+        if not set(scope).intersection(set(signing_key.scope)):
             return False
 
+        # # if the signing key's scope doesn't match the required scope
+        # if signing_key.scope != scope:
+        #     return False
+
         return True
 
     def get_model(self):
 
         """
         Generate an instance of the Signing class, which represents the Signing
 table in the database.
@@ -203,15 +217,18 @@
 
         if not hasattr(self, '_model'):
             class Signing(self.db.Model):
                 __tablename__ = 'signing'
                 signature = self.db.Column(self.db.String(1000),
 primary_key=True)
                 email = self.db.Column(self.db.String(100))
-                scope = self.db.Column(self.db.String(100))
+                # scope = self.db.Column(self.db.String(100))
+                # scope = self.db.Column(self.db.MutableList.as_mutable
+(self.db.String(100)), default=[]),
+                scope = self.db.Column(self.db.JSON())
                 active = self.db.Column(self.db.Boolean)
                 timestamp = self.db.Column(self.db.DateTime, nullable=False,
 default=datetime.datetime.utcnow)
                 expiration = self.db.Column(self.db.DateTime, nullable=False,
 default=datetime.datetime.utcnow)
 
             self._model = Signing
@@ -244,28 +261,63 @@
 
         Signing = self.get_model()
 
         query = Signing.query
 
         if active is not None:
             query = query.filter(Signing.active == active)
+
+        # Convert scope to a list if it's a string
+        if isinstance(scope, str):
+            scope = [scope]
+
         if scope:
-            query = query.filter(Signing.scope == scope)
+
+            for s in scope:
+                # https://stackoverflow.com/a/44250678/13301284
+                query = query.filter(Signing.scope.comparator.contains(s))
+
+                # https://stackoverflow.com/a/39470478/13301284
+                # query = query.filter(func.json_contains(Signing.scope, s) ==
+1)
+                # query = query.filter(literal(s).bool_op('MEMBER OF')
+(Signing.scope.self_group()))
+
+            # query = query.filter(Signing.scope.in_(scope))
+
+        # if scope:
+        #     query = query.filter(Signing.scope == scope)
+
         if email:
             query = query.filter(Signing.email == email)
 
         result = query.all()
 
         if not result:
             return False
 
         return [{'signature': key.signature, 'email': key.email, 'scope':
 key.scope, 'active': key.active, 'timestamp': key.timestamp, 'expiration':
 key.expiration} for key in result]
 
+    def query_all(self) -> List[Dict[str, Any]]:
+
+        """
+        Query all values in the Signing table.
+        If no keys are found, it returns an empty list.
+
+        Returns:
+            List[Dict[str, Any]]: A list of dictionaries where each dictionary
+contains the details of a signing key.
+
+        """
+        return [{'signature': key.signature, 'email': key.email, 'scope':
+key.scope, 'active': key.active, 'timestamp': key.timestamp, 'expiration':
+key.expiration} for key in self.get_model().query.all()]
+
 ***** Classes *****
   class Signatures (app, byte_len:Â intÂ =Â 24)
       The Signatures class handles operations related to the creation,
       management, and validation of signing keys in the database.
       Initializes a new instance of the Signatures class.
       ***** Args *****
         app :&ensp;Flask
@@ -343,17 +395,23 @@
               Signing = self.get_model()
 
               # loop until a unique key is generated
               while True:
                   key = self.generate_key()
                   if not Signing.query.filter_by(signature=key).first(): break
 
+              # Convert scope to a list if it's a string
+              if isinstance(scope, str):
+                  scope = [scope]
+
               new_key = Signing(
                               signature=key,
-                              scope=scope.lower() if scope else "",
+                              # scope=scope.lower() if scope else "",
+                              scope=[s.lower() for s in scope] if scope else
+      [],
                               email=email.lower() if email else "",
                               active=active,
                               expiration=(datetime.datetime.utcnow() +
       datetime.timedelta(hours=expiration)) if expiration else 0,
                               timestamp=datetime.datetime.utcnow(),
               )
 
@@ -426,18 +484,27 @@
                   self.expire_key(signature)
                   return False
 
               # if the signing key is set to inactive
               if not signing_key.active:
                   return False
 
-              # if the signing key's scope doesn't match the required scope
-              if signing_key.scope != scope:
+              # Convert scope to a list if it's a string
+              if isinstance(scope, str):
+                  scope = [scope]
+
+              # if the signing key's scope doesn't match any of the required
+      scopes
+              if not set(scope).intersection(set(signing_key.scope)):
                   return False
 
+              # # if the signing key's scope doesn't match the required scope
+              # if signing_key.scope != scope:
+              #     return False
+
               return True
 
           def get_model(self):
 
               """
               Generate an instance of the Signing class, which represents the
       Signing table in the database.
@@ -461,15 +528,18 @@
 
               if not hasattr(self, '_model'):
                   class Signing(self.db.Model):
                       __tablename__ = 'signing'
                       signature = self.db.Column(self.db.String(1000),
       primary_key=True)
                       email = self.db.Column(self.db.String(100))
-                      scope = self.db.Column(self.db.String(100))
+                      # scope = self.db.Column(self.db.String(100))
+                      # scope = self.db.Column(self.db.MutableList.as_mutable
+      (self.db.String(100)), default=[]),
+                      scope = self.db.Column(self.db.JSON())
                       active = self.db.Column(self.db.Boolean)
                       timestamp = self.db.Column(self.db.DateTime,
       nullable=False, default=datetime.datetime.utcnow)
                       expiration = self.db.Column(self.db.DateTime,
       nullable=False, default=datetime.datetime.utcnow)
 
                   self._model = Signing
@@ -502,27 +572,63 @@
 
               Signing = self.get_model()
 
               query = Signing.query
 
               if active is not None:
                   query = query.filter(Signing.active == active)
+
+              # Convert scope to a list if it's a string
+              if isinstance(scope, str):
+                  scope = [scope]
+
               if scope:
-                  query = query.filter(Signing.scope == scope)
+
+                  for s in scope:
+                      # https://stackoverflow.com/a/44250678/13301284
+                      query = query.filter(Signing.scope.comparator.contains
+      (s))
+
+                      # https://stackoverflow.com/a/39470478/13301284
+                      # query = query.filter(func.json_contains(Signing.scope,
+      s) == 1)
+                      # query = query.filter(literal(s).bool_op('MEMBER OF')
+      (Signing.scope.self_group()))
+
+                  # query = query.filter(Signing.scope.in_(scope))
+
+              # if scope:
+              #     query = query.filter(Signing.scope == scope)
+
               if email:
                   query = query.filter(Signing.email == email)
 
               result = query.all()
 
               if not result:
                   return False
 
               return [{'signature': key.signature, 'email': key.email, 'scope':
       key.scope, 'active': key.active, 'timestamp': key.timestamp,
       'expiration': key.expiration} for key in result]
+
+          def query_all(self) -> List[Dict[str, Any]]:
+
+              """
+              Query all values in the Signing table.
+              If no keys are found, it returns an empty list.
+
+              Returns:
+                  List[Dict[str, Any]]: A list of dictionaries where each
+      dictionary contains the details of a signing key.
+
+              """
+              return [{'signature': key.signature, 'email': key.email, 'scope':
+      key.scope, 'active': key.active, 'timestamp': key.timestamp,
+      'expiration': key.expiration} for key in self.get_model().query.all()]
       **** Methods ****
         def expire_key(self, key)
             Expires a signing key in the database.
             This function finds the key in the database and disables it by
             setting its 'active' status to False. If the key does not exist,
             the function returns False and an HTTP status code 500.
             ***** Args *****
@@ -636,24 +742,50 @@
 
                 if not hasattr(self, '_model'):
                     class Signing(self.db.Model):
                         __tablename__ = 'signing'
                         signature = self.db.Column(self.db.String(1000),
             primary_key=True)
                         email = self.db.Column(self.db.String(100))
-                        scope = self.db.Column(self.db.String(100))
+                        # scope = self.db.Column(self.db.String(100))
+                        # scope = self.db.Column(self.db.MutableList.as_mutable
+            (self.db.String(100)), default=[]),
+                        scope = self.db.Column(self.db.JSON())
                         active = self.db.Column(self.db.Boolean)
                         timestamp = self.db.Column(self.db.DateTime,
             nullable=False, default=datetime.datetime.utcnow)
                         expiration = self.db.Column(self.db.DateTime,
             nullable=False, default=datetime.datetime.utcnow)
 
                     self._model = Signing
 
                 return self._model
+        def query_all(self) â>Â List[Dict[str,Â Any]]
+            Query all values in the Signing table. If no keys are found, it
+            returns an empty list.
+            ***** Returns *****
+              List[Dict[str, Any]]
+                  A list of dictionaries where each dictionary contains the
+                  details of a signing key.
+              Expand source code
+            def query_all(self) -> List[Dict[str, Any]]:
+
+                """
+                Query all values in the Signing table.
+                If no keys are found, it returns an empty list.
+
+                Returns:
+                    List[Dict[str, Any]]: A list of dictionaries where each
+            dictionary contains the details of a signing key.
+
+                """
+                return [{'signature': key.signature, 'email': key.email,
+            'scope': key.scope, 'active': key.active, 'timestamp':
+            key.timestamp, 'expiration': key.expiration} for key in
+            self.get_model().query.all()]
         def query_keys(self, active:Â boolÂ =Â None, scope:Â strÂ =Â None,
         email:Â strÂ =Â None) â>Â Union[List[Dict[str,Â Any]],Â bool]
             Query signing keys by active status, scope, and email.
             This function returns a list of signing keys that match the
             provided parameters. If no keys are found, it returns False.
             ***** Args *****
               active :&ensp;bool, optional
@@ -693,16 +825,37 @@
 
                 Signing = self.get_model()
 
                 query = Signing.query
 
                 if active is not None:
                     query = query.filter(Signing.active == active)
+
+                # Convert scope to a list if it's a string
+                if isinstance(scope, str):
+                    scope = [scope]
+
                 if scope:
-                    query = query.filter(Signing.scope == scope)
+
+                    for s in scope:
+                        # https://stackoverflow.com/a/44250678/13301284
+                        query = query.filter(Signing.scope.comparator.contains
+            (s))
+
+                        # https://stackoverflow.com/a/39470478/13301284
+                        # query = query.filter(func.json_contains
+            (Signing.scope, s) == 1)
+                        # query = query.filter(literal(s).bool_op('MEMBER OF')
+            (Signing.scope.self_group()))
+
+                    # query = query.filter(Signing.scope.in_(scope))
+
+                # if scope:
+                #     query = query.filter(Signing.scope == scope)
+
                 if email:
                     query = query.filter(Signing.email == email)
 
                 result = query.all()
 
                 if not result:
                     return False
@@ -761,18 +914,27 @@
                     self.expire_key(signature)
                     return False
 
                 # if the signing key is set to inactive
                 if not signing_key.active:
                     return False
 
-                # if the signing key's scope doesn't match the required scope
-                if signing_key.scope != scope:
+                # Convert scope to a list if it's a string
+                if isinstance(scope, str):
+                    scope = [scope]
+
+                # if the signing key's scope doesn't match any of the required
+            scopes
+                if not set(scope).intersection(set(signing_key.scope)):
                     return False
 
+                # # if the signing key's scope doesn't match the required scope
+                # if signing_key.scope != scope:
+                #     return False
+
                 return True
         def write_key_to_database(self, scope:Â strÂ =Â None, expiration:
         Â intÂ =Â 1, active:Â boolÂ =Â True, email:Â strÂ =Â None) â>Â str
             Writes a newly generated signing key to the database.
             This function will continuously attempt to generate a key until a
             unique one is created.
             ***** Args *****
@@ -818,17 +980,23 @@
 
                 # loop until a unique key is generated
                 while True:
                     key = self.generate_key()
                     if not Signing.query.filter_by(signature=key).first():
             break
 
+                # Convert scope to a list if it's a string
+                if isinstance(scope, str):
+                    scope = [scope]
+
                 new_key = Signing(
                                 signature=key,
-                                scope=scope.lower() if scope else "",
+                                # scope=scope.lower() if scope else "",
+                                scope=[s.lower() for s in scope] if scope else
+            [],
                                 email=email.lower() if email else "",
                                 active=active,
                                 expiration=(datetime.datetime.utcnow() +
             datetime.timedelta(hours=expiration)) if expiration else 0,
                                 timestamp=datetime.datetime.utcnow(),
                 )
 
@@ -839,12 +1007,13 @@
 
 ****** Index ******
     * **** Classes ****
           o *** Signatures ***
                 # expire_key
                 # generate_key
                 # get_model
+                # query_all
                 # query_keys
                 # verify_signature
                 # write_key_to_database
 
 Generated by pdoc0.10.0.
```

### Comparing `flask_signing-0.2.1/docs/logo.png` & `flask_signing-0.3.0/docs/logo.png`

 * *Files identical despite different names*

### Comparing `flask_signing-0.2.1/flask_signing/__init__.py` & `flask_signing-0.3.0/flask_signing/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 __name__ = "flask_signing"
 __author__ = "Sig Janoska-Bedi"
 __credits__ = ["Sig Janoska-Bedi",]
-__version__ = "0.2.1"
+__version__ = "0.3.0"
 __license__ = "BSD-3-Clause"
 __maintainer__ = "Sig Janoska-Bedi"
 __email__ = "signe@atreeus.com"
 
 import datetime, secrets
+from sqlalchemy import func, literal
 from flask_sqlalchemy import SQLAlchemy
 from typing import Union, List, Dict, Any
 
 class Signatures:
     """
     The Signatures class handles operations related to the creation, management, and validation 
     of signing keys in the database.
@@ -68,17 +69,22 @@
         Signing = self.get_model()
 
         # loop until a unique key is generated
         while True:
             key = self.generate_key()
             if not Signing.query.filter_by(signature=key).first(): break
 
+        # Convert scope to a list if it's a string
+        if isinstance(scope, str):
+            scope = [scope]
+
         new_key = Signing(
                         signature=key, 
-                        scope=scope.lower() if scope else "",
+                        # scope=scope.lower() if scope else "",
+                        scope=[s.lower() for s in scope] if scope else [],
                         email=email.lower() if email else "", 
                         active=active,
                         expiration=(datetime.datetime.utcnow() + datetime.timedelta(hours=expiration)) if expiration else 0,
                         timestamp=datetime.datetime.utcnow(),
         )
 
         self.db.session.add(new_key)
@@ -142,18 +148,26 @@
             self.expire_key(signature)
             return False
 
         # if the signing key is set to inactive
         if not signing_key.active:
             return False
 
-        # if the signing key's scope doesn't match the required scope
-        if signing_key.scope != scope:
+        # Convert scope to a list if it's a string
+        if isinstance(scope, str):
+            scope = [scope]
+
+        # if the signing key's scope doesn't match any of the required scopes
+        if not set(scope).intersection(set(signing_key.scope)):
             return False
 
+        # # if the signing key's scope doesn't match the required scope
+        # if signing_key.scope != scope:
+        #     return False
+
         return True
 
     def get_model(self):
 
         """
         Generate an instance of the Signing class, which represents the Signing table in the database.
 
@@ -169,15 +183,17 @@
         """
 
         if not hasattr(self, '_model'):
             class Signing(self.db.Model):
                 __tablename__ = 'signing'
                 signature = self.db.Column(self.db.String(1000), primary_key=True) 
                 email = self.db.Column(self.db.String(100))
-                scope = self.db.Column(self.db.String(100))
+                # scope = self.db.Column(self.db.String(100))
+                # scope = self.db.Column(self.db.MutableList.as_mutable(self.db.String(100)), default=[]),
+                scope = self.db.Column(self.db.JSON())
                 active = self.db.Column(self.db.Boolean)
                 timestamp = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
                 expiration = self.db.Column(self.db.DateTime, nullable=False, default=datetime.datetime.utcnow)
 
             self._model = Signing
 
         return self._model
@@ -202,18 +218,48 @@
 
         Signing = self.get_model()
 
         query = Signing.query
 
         if active is not None:
             query = query.filter(Signing.active == active)
+
+        # Convert scope to a list if it's a string
+        if isinstance(scope, str):
+            scope = [scope]
+
         if scope:
-            query = query.filter(Signing.scope == scope)
+
+            for s in scope:
+                # https://stackoverflow.com/a/44250678/13301284
+                query = query.filter(Signing.scope.comparator.contains(s))
+
+                # https://stackoverflow.com/a/39470478/13301284
+                # query = query.filter(func.json_contains(Signing.scope, s) == 1)
+                # query = query.filter(literal(s).bool_op('MEMBER OF')(Signing.scope.self_group()))
+                
+            # query = query.filter(Signing.scope.in_(scope))
+            
+        # if scope:
+        #     query = query.filter(Signing.scope == scope)
+
         if email:
             query = query.filter(Signing.email == email)
 
         result = query.all()
 
         if not result:
             return False
 
-        return [{'signature': key.signature, 'email': key.email, 'scope': key.scope, 'active': key.active, 'timestamp': key.timestamp, 'expiration': key.expiration} for key in result]
+        return [{'signature': key.signature, 'email': key.email, 'scope': key.scope, 'active': key.active, 'timestamp': key.timestamp, 'expiration': key.expiration} for key in result]
+
+    def query_all(self) -> List[Dict[str, Any]]:
+
+        """
+        Query all values in the Signing table.
+        If no keys are found, it returns an empty list.
+
+        Returns:
+            List[Dict[str, Any]]: A list of dictionaries where each dictionary contains the details of a signing key.
+
+        """
+        return [{'signature': key.signature, 'email': key.email, 'scope': key.scope, 'active': key.active, 'timestamp': key.timestamp, 'expiration': key.expiration} for key in self.get_model().query.all()]
```

### Comparing `flask_signing-0.2.1/flask_signing.egg-info/PKG-INFO` & `flask_signing-0.3.0/flask_signing.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flask-signing
-Version: 0.2.1
+Version: 0.3.0
 Summary: a signing key extension for flask
 Home-page: https://github.com/signebedi/Flask-Signing
 Author: Sig Janoska-Bedi
 Author-email: signe@atreeus.com
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
@@ -26,15 +26,15 @@
 [![Flask-Signing tests](https://github.com/signebedi/Flask-Signing/workflows/tests/badge.svg)](https://github.com/signebedi/Flask-Signing/actions)
 
 a signing key extension for flask
 
 
 ### About
 
-The Flask-Signing library is a useful tool for Flask applications that requires secure and robust management of signing keys. This package aids in managing API keys, ensuring only clients with valid permissions can access your resources. Do you need to generate single-use tokens for one-time actions like email verification or password reset? Flask-Signing can handle that. In theory, it can also help manage session IDs. For applications that implement JWT or OAuth2, Flask-Signing can generate and manage the signing keys for your tokens. You can also use it to verify webhook payloads or to implement a licensing system for your software. 
+The Flask-Signing library is a useful tool for Flask applications that require secure and robust management of signing keys. Do you need to generate single-use tokens for one-time actions like email verification or password reset? Flask-Signing can handle that. Are you looking for a simple method for managing API keys? Look no further. 
 
 ### Installation
 
 First, install the flask_signing package. You can do this with pip:
 
 ```bash
 pip install flask_signing
@@ -69,10 +69,10 @@
 @app.route('/expire/<key>')
 def expire(key):
     expired = signatures.expire_key(key)
     return f'Key expired: {expired}'
     
 ```
 
-In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. Finally, you can expire a key using the /expier/<key> route.
+In this example, a new signing key is generated and written to the database when you visit the /sign route, and the key is displayed on the page. Then, when you visit the /verify/<key> route (replace <key> with the actual key), the validity of the key is checked and displayed. Finally, you can expire a key using the /expire/<key> route described above.
 
 Please note that this is a very basic example and your actual use of the flask_signing package may be more complex depending on your needs. It's important to secure your signing keys and handle them appropriately according to your application's security requirements.
```

### Comparing `flask_signing-0.2.1/setup.py` & `flask_signing-0.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # # Read requirements.txt for install_requires
 # with open("requirements.txt", "r", encoding="utf-8") as fr:
 #     install_requires = fr.read().splitlines()
 
 setup(
     name='flask_signing',
-    version='0.2.1',
+    version='0.3.0',
     url='https://github.com/signebedi/Flask-Signing',
     author='Sig Janoska-Bedi',
     author_email='signe@atreeus.com',
     description='a signing key extension for flask',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(),
```

### Comparing `flask_signing-0.2.1/tests/test_flask_signing.py` & `flask_signing-0.3.0/tests/test_flask_signing.py`

 * *Files 17% similar despite different names*

```diff
@@ -47,22 +47,30 @@
     #     """
     #     with self.app.app_context():
     #         key = self.signatures.write_key_to_database(scope='test')
     #     self.assertIsNotNone(Signing.query.filter_by(signature=key).first())
     #     self.signatures.expire_key(key)
     #     self.assertFalse(Signing.query.filter_by(signature=key).first().active)
 
-    def test_write_and_expire_key(self):
+    def test_write_and_expire_key_string_scope(self):
         with self.app.app_context():
             key = self.signatures.write_key_to_database(scope='test')
             Signing = self.signatures.get_model()
             self.assertIsNotNone(Signing.query.filter_by(signature=key).first())
             self.signatures.expire_key(key)
             self.assertFalse(Signing.query.filter_by(signature=key).first().active)
 
+    def test_write_and_expire_key_list_scope(self):
+        with self.app.app_context():
+            key = self.signatures.write_key_to_database(scope=['test', 'task', 'tusk'])
+            Signing = self.signatures.get_model()
+            self.assertIsNotNone(Signing.query.filter_by(signature=key).first())
+            self.signatures.expire_key(key)
+            self.assertFalse(Signing.query.filter_by(signature=key).first().active)
+
     def test_verify_signature(self):
         """
         Test if a signature can be successfully verified.
         """
         with self.app.app_context():
             key = self.signatures.write_key_to_database(scope='test')
             self.assertTrue(self.signatures.verify_signature(signature=key, scope='test'))
@@ -84,15 +92,16 @@
 
             # Test querying by active status
             result = self.signatures.query_keys(active=True)
             self.assertTrue(all(record['active'] for record in result))
 
             # Test querying by scope
             result = self.signatures.query_keys(scope='test1')
-            self.assertTrue(all(record['scope'] == 'test1' for record in result))
+            self.assertTrue(all(record['scope'] == ['test1'] for record in result))
+            self.assertTrue(all(type(record['scope']) == list for record in result))
 
             # Test querying by email
             result = self.signatures.query_keys(email='test2@example.com')
             self.assertTrue(all(record['email'] == 'test2@example.com' for record in result))
 
             # Test querying by multiple fields
             result = self.signatures.query_keys(active=True, scope='test1', email='test1@example.com')
```

