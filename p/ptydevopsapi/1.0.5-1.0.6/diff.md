# Comparing `tmp/ptydevopsapi-1.0.5.tar.gz` & `tmp/ptydevopsapi-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ptydevopsapi-1.0.5.tar", last modified: Mon Aug 15 11:43:50 2022, max compression
+gzip compressed data, was "ptydevopsapi-1.0.6.tar", last modified: Tue Jun 13 11:11:30 2023, max compression
```

## Comparing `ptydevopsapi-1.0.5.tar` & `ptydevopsapi-1.0.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-15 11:43:50.991177 ptydevopsapi-1.0.5/
--rw-rw-r--   0 anton     (1000) anton     (1000)      377 2022-08-15 11:43:50.991177 ptydevopsapi-1.0.5/PKG-INFO
--rw-rw-r--   0 anton     (1000) anton     (1000)      586 2022-08-15 11:43:01.000000 ptydevopsapi-1.0.5/README.md
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-15 11:43:50.991177 ptydevopsapi-1.0.5/ptydevopsapi/
--rw-rw-r--   0 anton     (1000) anton     (1000)        0 2022-08-15 11:29:06.000000 ptydevopsapi-1.0.5/ptydevopsapi/__init__.py
--rw-rw-r--   0 anton     (1000) anton     (1000)    13462 2022-08-15 11:38:26.000000 ptydevopsapi-1.0.5/ptydevopsapi/ptydevopsapi.py
-drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2022-08-15 11:43:50.991177 ptydevopsapi-1.0.5/ptydevopsapi.egg-info/
--rw-rw-r--   0 anton     (1000) anton     (1000)      377 2022-08-15 11:43:50.000000 ptydevopsapi-1.0.5/ptydevopsapi.egg-info/PKG-INFO
--rw-rw-r--   0 anton     (1000) anton     (1000)      251 2022-08-15 11:43:50.000000 ptydevopsapi-1.0.5/ptydevopsapi.egg-info/SOURCES.txt
--rw-rw-r--   0 anton     (1000) anton     (1000)        1 2022-08-15 11:43:50.000000 ptydevopsapi-1.0.5/ptydevopsapi.egg-info/dependency_links.txt
--rw-rw-r--   0 anton     (1000) anton     (1000)        9 2022-08-15 11:43:50.000000 ptydevopsapi-1.0.5/ptydevopsapi.egg-info/requires.txt
--rw-rw-r--   0 anton     (1000) anton     (1000)       13 2022-08-15 11:43:50.000000 ptydevopsapi-1.0.5/ptydevopsapi.egg-info/top_level.txt
--rw-rw-r--   0 anton     (1000) anton     (1000)       38 2022-08-15 11:43:50.991177 ptydevopsapi-1.0.5/setup.cfg
--rw-rw-r--   0 anton     (1000) anton     (1000)      691 2022-08-15 11:43:49.000000 ptydevopsapi-1.0.5/setup.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2023-06-13 11:11:30.859250 ptydevopsapi-1.0.6/
+-rw-rw-r--   0 anton     (1000) anton     (1000)      406 2023-06-13 11:11:30.859250 ptydevopsapi-1.0.6/PKG-INFO
+-rw-rw-r--   0 anton     (1000) anton     (1000)      575 2023-06-13 10:56:03.000000 ptydevopsapi-1.0.6/README.md
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2023-06-13 11:11:30.859250 ptydevopsapi-1.0.6/ptydevopsapi/
+-rw-rw-r--   0 anton     (1000) anton     (1000)        0 2022-08-15 11:29:06.000000 ptydevopsapi-1.0.6/ptydevopsapi/__init__.py
+-rw-rw-r--   0 anton     (1000) anton     (1000)    14168 2023-06-13 11:07:44.000000 ptydevopsapi-1.0.6/ptydevopsapi/ptydevopsapi.py
+drwxrwxr-x   0 anton     (1000) anton     (1000)        0 2023-06-13 11:11:30.859250 ptydevopsapi-1.0.6/ptydevopsapi.egg-info/
+-rw-rw-r--   0 anton     (1000) anton     (1000)      406 2023-06-13 11:11:30.000000 ptydevopsapi-1.0.6/ptydevopsapi.egg-info/PKG-INFO
+-rw-rw-r--   0 anton     (1000) anton     (1000)      251 2023-06-13 11:11:30.000000 ptydevopsapi-1.0.6/ptydevopsapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 anton     (1000) anton     (1000)        1 2023-06-13 11:11:30.000000 ptydevopsapi-1.0.6/ptydevopsapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 anton     (1000) anton     (1000)        9 2023-06-13 11:11:30.000000 ptydevopsapi-1.0.6/ptydevopsapi.egg-info/requires.txt
+-rw-rw-r--   0 anton     (1000) anton     (1000)       13 2023-06-13 11:11:30.000000 ptydevopsapi-1.0.6/ptydevopsapi.egg-info/top_level.txt
+-rw-rw-r--   0 anton     (1000) anton     (1000)       38 2023-06-13 11:11:30.859250 ptydevopsapi-1.0.6/setup.cfg
+-rw-rw-r--   0 anton     (1000) anton     (1000)      745 2023-06-13 11:09:04.000000 ptydevopsapi-1.0.6/setup.py
```

### Comparing `ptydevopsapi-1.0.5/ptydevopsapi/ptydevopsapi.py` & `ptydevopsapi-1.0.6/ptydevopsapi/ptydevopsapi.py`

 * *Files 2% similar despite different names*

```diff
@@ -395,14 +395,37 @@
         :param role_uid: role unique id
         :param member_uid: member unique id
         """
         return self.__get(
             "roles/{}/members/{}/users", role_uid, member_uid
         )
 
+    def list_alphabets(self):
+        """List all alphabets
+        """
+        return self.__get("alphabets")
+
+    def create_alphabet(self, alphabet: dict):
+        """Create a new alphabet
+        :param alphabet: alphabet payload
+        """
+        return self.__post("alphabets", alphabet)
+
+    def get_alphabet(self, alphabet_uid: str):
+        """Get a specific alphabet
+        :param alphabet_uid: alphabet identifier
+        """
+        return self.__get("alphabets/{}", alphabet_uid)
+
+    def delete_alphabet(self, alphabet_uid: str):
+        """Delete a specific alphabet
+        :param alphabet_uid: alphabet identifier
+        """
+        return self.__delete("alphabets/{}", alphabet_uid)
+
     def role_sync(self, role_uid: str):
         """Sync roles
 
         :param role_uid: role unique id
         """
         data = {}
         return self.__post("roles/{}/sync", data, role_uid)
```

### Comparing `ptydevopsapi-1.0.5/setup.py` & `ptydevopsapi-1.0.6/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,18 +7,19 @@
     long_description = fh.read()
 
 config = {
     "keywords": "devops api wrapper",
     "author": "Anton Andersson",
     "description": "A python wrapper for the PIM devops API",
     "long_description": "",
+    "long_description_content_type": "text/markdown",
     "url": "http://antonandersson.se",
     "download_url": "http://antonandersson.se",
     "author_email": "anton@antonandersson.se",
-    "version": "1.0.5",
+    "version": "1.0.6",
     "install_requires": ["requests"],
     "packages": ["ptydevopsapi"],
     "name": "ptydevopsapi",
     "classifiers": [
         "Programming Language :: Python :: 3.7",
     ],
 }
```

