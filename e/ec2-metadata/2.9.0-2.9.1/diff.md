# Comparing `tmp/ec2-metadata-2.9.0.tar.gz` & `tmp/ec2-metadata-2.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ec2-metadata-2.9.0.tar", last modified: Fri Mar 25 23:42:46 2022, max compression
+gzip compressed data, was "ec2-metadata-2.9.1.tar", last modified: Tue Mar 29 17:45:55 2022, max compression
```

## Comparing `ec2-metadata-2.9.0.tar` & `ec2-metadata-2.9.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-25 23:42:46.376884 ec2-metadata-2.9.0/
--rw-r--r--   0 chainz     (501) staff       (20)     4269 2022-03-25 23:42:33.000000 ec2-metadata-2.9.0/HISTORY.rst
--rw-r--r--   0 chainz     (501) staff       (20)     1069 2022-03-08 11:12:03.000000 ec2-metadata-2.9.0/LICENSE
--rw-r--r--   0 chainz     (501) staff       (20)      245 2022-03-08 11:12:03.000000 ec2-metadata-2.9.0/MANIFEST.in
--rw-r--r--   0 chainz     (501) staff       (20)    16166 2022-03-25 23:42:46.377102 ec2-metadata-2.9.0/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)    15109 2022-03-25 20:11:04.000000 ec2-metadata-2.9.0/README.rst
--rw-r--r--   0 chainz     (501) staff       (20)      635 2022-03-08 11:12:03.000000 ec2-metadata-2.9.0/pyproject.toml
--rw-r--r--   0 chainz     (501) staff       (20)     1430 2022-03-25 23:42:46.379242 ec2-metadata-2.9.0/setup.cfg
--rw-r--r--   0 chainz     (501) staff       (20)       74 2022-03-08 11:12:03.000000 ec2-metadata-2.9.0/setup.py
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-25 23:42:46.369276 ec2-metadata-2.9.0/src/
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-25 23:42:46.373592 ec2-metadata-2.9.0/src/ec2_metadata/
--rw-r--r--   0 chainz     (501) staff       (20)    13573 2022-03-25 20:11:04.000000 ec2-metadata-2.9.0/src/ec2_metadata/__init__.py
--rw-r--r--   0 chainz     (501) staff       (20)        0 2021-10-05 09:49:23.000000 ec2-metadata-2.9.0/src/ec2_metadata/py.typed
-drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-25 23:42:46.376496 ec2-metadata-2.9.0/src/ec2_metadata.egg-info/
--rw-r--r--   0 chainz     (501) staff       (20)    16166 2022-03-25 23:42:45.000000 ec2-metadata-2.9.0/src/ec2_metadata.egg-info/PKG-INFO
--rw-r--r--   0 chainz     (501) staff       (20)      369 2022-03-25 23:42:46.000000 ec2-metadata-2.9.0/src/ec2_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-03-25 23:42:45.000000 ec2-metadata-2.9.0/src/ec2_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 chainz     (501) staff       (20)        1 2022-03-25 23:42:44.000000 ec2-metadata-2.9.0/src/ec2_metadata.egg-info/not-zip-safe
--rw-r--r--   0 chainz     (501) staff       (20)       52 2022-03-25 23:42:46.000000 ec2-metadata-2.9.0/src/ec2_metadata.egg-info/requires.txt
--rw-r--r--   0 chainz     (501) staff       (20)       13 2022-03-25 23:42:46.000000 ec2-metadata-2.9.0/src/ec2_metadata.egg-info/top_level.txt
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-29 17:45:55.115100 ec2-metadata-2.9.1/
+-rw-r--r--   0 chainz     (501) staff       (20)     4499 2022-03-29 17:45:34.000000 ec2-metadata-2.9.1/HISTORY.rst
+-rw-r--r--   0 chainz     (501) staff       (20)     1069 2022-03-08 11:12:03.000000 ec2-metadata-2.9.1/LICENSE
+-rw-r--r--   0 chainz     (501) staff       (20)      245 2022-03-08 11:12:03.000000 ec2-metadata-2.9.1/MANIFEST.in
+-rw-r--r--   0 chainz     (501) staff       (20)    16180 2022-03-29 17:45:55.115567 ec2-metadata-2.9.1/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)    15123 2022-03-29 17:45:28.000000 ec2-metadata-2.9.1/README.rst
+-rw-r--r--   0 chainz     (501) staff       (20)      635 2022-03-08 11:12:03.000000 ec2-metadata-2.9.1/pyproject.toml
+-rw-r--r--   0 chainz     (501) staff       (20)     1430 2022-03-29 17:45:55.117088 ec2-metadata-2.9.1/setup.cfg
+-rw-r--r--   0 chainz     (501) staff       (20)       74 2022-03-08 11:12:03.000000 ec2-metadata-2.9.1/setup.py
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-29 17:45:55.109345 ec2-metadata-2.9.1/src/
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-29 17:45:55.112281 ec2-metadata-2.9.1/src/ec2_metadata/
+-rw-r--r--   0 chainz     (501) staff       (20)    13698 2022-03-29 17:45:28.000000 ec2-metadata-2.9.1/src/ec2_metadata/__init__.py
+-rw-r--r--   0 chainz     (501) staff       (20)        0 2021-10-05 09:49:23.000000 ec2-metadata-2.9.1/src/ec2_metadata/py.typed
+drwxr-xr-x   0 chainz     (501) staff       (20)        0 2022-03-29 17:45:55.114579 ec2-metadata-2.9.1/src/ec2_metadata.egg-info/
+-rw-r--r--   0 chainz     (501) staff       (20)    16180 2022-03-29 17:45:54.000000 ec2-metadata-2.9.1/src/ec2_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 chainz     (501) staff       (20)      369 2022-03-29 17:45:55.000000 ec2-metadata-2.9.1/src/ec2_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2022-03-29 17:45:54.000000 ec2-metadata-2.9.1/src/ec2_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 chainz     (501) staff       (20)        1 2022-03-29 17:45:53.000000 ec2-metadata-2.9.1/src/ec2_metadata.egg-info/not-zip-safe
+-rw-r--r--   0 chainz     (501) staff       (20)       52 2022-03-29 17:45:54.000000 ec2-metadata-2.9.1/src/ec2_metadata.egg-info/requires.txt
+-rw-r--r--   0 chainz     (501) staff       (20)       13 2022-03-29 17:45:55.000000 ec2-metadata-2.9.1/src/ec2_metadata.egg-info/top_level.txt
```

### Comparing `ec2-metadata-2.9.0/HISTORY.rst` & `ec2-metadata-2.9.1/HISTORY.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,18 @@
 =======
 History
 =======
 
+2.9.1 (2022-03-29)
+------------------
+
+* Return ``None`` for ``availability_zone_id`` when the underlying endpoint returns HTTP 404.
+
+  Thanks to Amir Rossert in `PR #350 <https://github.com/adamchainz/ec2-metadata/pull/350>`__.
+
 2.9.0 (2022-03-25)
 ------------------
 
 * Add ``autoscaling_target_lifecycle_state`` attribute, as per `AWS announcement <https://aws.amazon.com/about-aws/whats-new/2022/03/amazon-ec2-auto-scaling-lifecycle-instance-metadata/>`__.
 
 2.8.0 (2022-03-08)
 ------------------
```

### Comparing `ec2-metadata-2.9.0/LICENSE` & `ec2-metadata-2.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ec2-metadata-2.9.0/PKG-INFO` & `ec2-metadata-2.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2-metadata
-Version: 2.9.0
+Version: 2.9.1
 Summary: An easy interface to query the EC2 metadata API, with caching.
 Home-page: https://github.com/adamchainz/ec2-metadata
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/ec2-metadata/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
@@ -156,16 +156,16 @@
 See AWS docs page `Retrieve the target lifecycle state through instance metadata <https://docs.aws.amazon.com/autoscaling/ec2/userguide/retrieving-target-lifecycle-state-through-imds.html>`__.
 
 ``availability_zone: str``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The name of the current AZ e.g. ``'eu-west-1a'``.
 
-``availability_zone_id: str``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+``availability_zone_id: str | None``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The unique, cross-account ID of the current AZ e.g. ``'use1-az6'``.
 See AWS docs page `AZ IDs for your AWS resources
 <https://docs.aws.amazon.com/ram/latest/userguide/working-with-az-ids.html>`__.
 
 ``ami_launch_index: int``
 ~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `ec2-metadata-2.9.0/README.rst` & `ec2-metadata-2.9.1/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -129,16 +129,16 @@
 See AWS docs page `Retrieve the target lifecycle state through instance metadata <https://docs.aws.amazon.com/autoscaling/ec2/userguide/retrieving-target-lifecycle-state-through-imds.html>`__.
 
 ``availability_zone: str``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The name of the current AZ e.g. ``'eu-west-1a'``.
 
-``availability_zone_id: str``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+``availability_zone_id: str | None``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The unique, cross-account ID of the current AZ e.g. ``'use1-az6'``.
 See AWS docs page `AZ IDs for your AWS resources
 <https://docs.aws.amazon.com/ram/latest/userguide/working-with-az-ids.html>`__.
 
 ``ami_launch_index: int``
 ~~~~~~~~~~~~~~~~~~~~~~~~~
```

### Comparing `ec2-metadata-2.9.0/pyproject.toml` & `ec2-metadata-2.9.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ec2-metadata-2.9.0/setup.cfg` & `ec2-metadata-2.9.1/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ec2-metadata
-version = 2.9.0
+version = 2.9.1
 description = An easy interface to query the EC2 metadata API, with caching.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 author = Adam Johnson
 author_email = me@adamj.eu
 url = https://github.com/adamchainz/ec2-metadata
 project_urls =
```

### Comparing `ec2-metadata-2.9.0/src/ec2_metadata/__init__.py` & `ec2-metadata-2.9.1/src/ec2_metadata/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,16 +94,21 @@
         return resp.text
 
     @cached_property
     def availability_zone(self) -> str:
         return self._get_url(f"{self.metadata_url}placement/availability-zone").text
 
     @cached_property
-    def availability_zone_id(self) -> str:
-        return self._get_url(f"{self.metadata_url}placement/availability-zone-id").text
+    def availability_zone_id(self) -> str | None:
+        resp = self._get_url(
+            f"{self.metadata_url}placement/availability-zone-id", allow_404=True
+        )
+        if resp.status_code == 404:
+            return None
+        return resp.text
 
     @cached_property
     def ami_launch_index(self) -> int:
         return int(self._get_url(f"{self.metadata_url}ami-launch-index").text)
 
     @cached_property
     def ami_manifest_path(self) -> str:
```

### Comparing `ec2-metadata-2.9.0/src/ec2_metadata.egg-info/PKG-INFO` & `ec2-metadata-2.9.1/src/ec2_metadata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ec2-metadata
-Version: 2.9.0
+Version: 2.9.1
 Summary: An easy interface to query the EC2 metadata API, with caching.
 Home-page: https://github.com/adamchainz/ec2-metadata
 Author: Adam Johnson
 Author-email: me@adamj.eu
 License: MIT
 Project-URL: Changelog, https://github.com/adamchainz/ec2-metadata/blob/main/HISTORY.rst
 Project-URL: Twitter, https://twitter.com/adamchainz
@@ -156,16 +156,16 @@
 See AWS docs page `Retrieve the target lifecycle state through instance metadata <https://docs.aws.amazon.com/autoscaling/ec2/userguide/retrieving-target-lifecycle-state-through-imds.html>`__.
 
 ``availability_zone: str``
 ~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The name of the current AZ e.g. ``'eu-west-1a'``.
 
-``availability_zone_id: str``
-~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+``availability_zone_id: str | None``
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 
 The unique, cross-account ID of the current AZ e.g. ``'use1-az6'``.
 See AWS docs page `AZ IDs for your AWS resources
 <https://docs.aws.amazon.com/ram/latest/userguide/working-with-az-ids.html>`__.
 
 ``ami_launch_index: int``
 ~~~~~~~~~~~~~~~~~~~~~~~~~
```

