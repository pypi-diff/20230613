# Comparing `tmp/quiltplus-0.9.4.tar.gz` & `tmp/quiltplus-0.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quiltplus-0.9.4.tar", max compression
+gzip compressed data, was "quiltplus-0.9.5.tar", max compression
```

## Comparing `quiltplus-0.9.4.tar` & `quiltplus-0.9.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1069 2023-03-01 19:37:11.440551 quiltplus-0.9.4/LICENSE.md
--rw-r--r--   0        0        0      668 2023-05-31 14:03:42.566191 quiltplus-0.9.4/README.md
--rw-r--r--   0        0        0      916 2023-06-10 22:39:42.938650 quiltplus-0.9.4/pyproject.toml
--rw-r--r--   0        0        0      468 2023-06-05 00:41:34.765649 quiltplus-0.9.4/quiltplus/__init__.py
--rw-r--r--   0        0        0      716 2023-03-01 19:37:11.446051 quiltplus-0.9.4/quiltplus/ignore.py
--rw-r--r--   0        0        0     3794 2023-06-08 06:20:36.366907 quiltplus-0.9.4/quiltplus/local.py
--rw-r--r--   0        0        0     4287 2023-06-08 06:20:36.367537 quiltplus-0.9.4/quiltplus/package.py
--rw-r--r--   0        0        0      495 2023-06-08 06:20:36.368491 quiltplus-0.9.4/quiltplus/path.py
--rw-r--r--   0        0        0       80 2023-05-31 14:03:42.576780 quiltplus-0.9.4/quiltplus/property.py
--rw-r--r--   0        0        0        0 2023-06-03 15:46:39.663802 quiltplus-0.9.4/quiltplus/py.typed
--rw-r--r--   0        0        0      609 2023-06-03 15:46:39.664625 quiltplus-0.9.4/quiltplus/registry.py
--rw-r--r--   0        0        0      708 2023-06-03 15:46:39.666292 quiltplus-0.9.4/quiltplus/resource.py
--rw-r--r--   0        0        0      376 2023-06-07 23:40:53.197044 quiltplus-0.9.4/quiltplus/root.py
--rw-r--r--   0        0        0     1298 2023-06-08 06:20:36.368989 quiltplus-0.9.4/quiltplus/type.py
--rw-r--r--   0        0        0     1724 2023-06-07 23:40:53.198698 quiltplus-0.9.4/quiltplus/uri.py
--rw-r--r--   0        0        0      598 2023-06-10 22:39:42.939561 quiltplus-0.9.4/quiltplus/versions.py
--rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 quiltplus-0.9.4/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-03-01 19:37:11.440551 quiltplus-0.9.5/LICENSE.md
+-rw-r--r--   0        0        0      668 2023-05-31 14:03:42.566191 quiltplus-0.9.5/README.md
+-rw-r--r--   0        0        0      916 2023-06-13 04:52:22.532856 quiltplus-0.9.5/pyproject.toml
+-rw-r--r--   0        0        0      468 2023-06-05 00:41:34.765649 quiltplus-0.9.5/quiltplus/__init__.py
+-rw-r--r--   0        0        0      716 2023-03-01 19:37:11.446051 quiltplus-0.9.5/quiltplus/ignore.py
+-rw-r--r--   0        0        0     5026 2023-06-13 04:52:22.534454 quiltplus-0.9.5/quiltplus/local.py
+-rw-r--r--   0        0        0     4287 2023-06-08 06:20:36.367537 quiltplus-0.9.5/quiltplus/package.py
+-rw-r--r--   0        0        0      495 2023-06-08 06:20:36.368491 quiltplus-0.9.5/quiltplus/path.py
+-rw-r--r--   0        0        0       80 2023-05-31 14:03:42.576780 quiltplus-0.9.5/quiltplus/property.py
+-rw-r--r--   0        0        0        0 2023-06-03 15:46:39.663802 quiltplus-0.9.5/quiltplus/py.typed
+-rw-r--r--   0        0        0      609 2023-06-03 15:46:39.664625 quiltplus-0.9.5/quiltplus/registry.py
+-rw-r--r--   0        0        0      708 2023-06-03 15:46:39.666292 quiltplus-0.9.5/quiltplus/resource.py
+-rw-r--r--   0        0        0      376 2023-06-07 23:40:53.197044 quiltplus-0.9.5/quiltplus/root.py
+-rw-r--r--   0        0        0     1399 2023-06-13 04:52:22.535509 quiltplus-0.9.5/quiltplus/type.py
+-rw-r--r--   0        0        0     2875 2023-06-13 04:52:22.536375 quiltplus-0.9.5/quiltplus/uri.py
+-rw-r--r--   0        0        0      598 2023-06-10 22:39:42.939561 quiltplus-0.9.5/quiltplus/versions.py
+-rw-r--r--   0        0        0     1589 1970-01-01 00:00:00.000000 quiltplus-0.9.5/PKG-INFO
```

### Comparing `quiltplus-0.9.4/LICENSE.md` & `quiltplus-0.9.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.4/README.md` & `quiltplus-0.9.5/README.md`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.4/pyproject.toml` & `quiltplus-0.9.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "quiltplus"
-version = "0.9.4"
+version = "0.9.5"
 description = "Resource-oriented Python API/CLI for Quilt's decentralized social knowledge platform"
 authors = ["Ernest Prabhakar <ernest@quiltdata.io>"]
 license = "MIT"
 readme = "README.md"
 keywords = ["yaml", "api", "resource", "quilt"]
 packages = [
    { include = "quiltplus" }
```

### Comparing `quiltplus-0.9.4/quiltplus/ignore.py` & `quiltplus-0.9.5/quiltplus/ignore.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.4/quiltplus/package.py` & `quiltplus-0.9.5/quiltplus/package.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.4/quiltplus/registry.py` & `quiltplus-0.9.5/quiltplus/registry.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.4/quiltplus/resource.py` & `quiltplus-0.9.5/quiltplus/resource.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.4/quiltplus/type.py` & `quiltplus-0.9.5/quiltplus/type.py`

 * *Files 16% similar despite different names*

```diff
@@ -23,14 +23,17 @@
     # Decomposed Package Name
     SEP_HASH = "@"
     SEP_TAG = ":"
     K_HASH = "_hash"
     K_TAG = "_tag"
     K_VER = "_version"
     SEP = {K_HASH: SEP_HASH, K_TAG: SEP_TAG, K_PKG: "/"}
+    K_PKG_NAME = "_package_name"
+    K_PKG_PRE = "_package_prefix"
+    K_PKG_SUF = "_package_suffix"
 
     @staticmethod
     def BaseType(attrs: dict) -> str:
         for key in QuiltType.FRAG_KEYS:
             if key in attrs:
                 return key
         return UnUri.K_HOST
```

### Comparing `quiltplus-0.9.4/quiltplus/uri.py` & `quiltplus-0.9.5/quiltplus/uri.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 
 from un_yaml import UnUri  # type: ignore
 
 from .type import QuiltType
 
 
 class QuiltUri(QuiltType):
+    """
+    Create and manage Quilt Resources from UnURI attrs.
+    """
+
     @classmethod
     def FromUnUri(cls, un: UnUri) -> "QuiltUri":
         return cls(un.attrs)
 
     @classmethod
     def FromUri(cls, uri: str) -> "QuiltUri":
         un = UnUri(uri)
@@ -17,19 +21,45 @@
 
     @staticmethod
     def AttrsFromUri(uri: str) -> dict:
         un = UnUri(uri)
         return un.attrs
 
     def __init__(self, attrs: dict):
+        """
+        Set local variables and additional attributes.
+
+        >>> reg = "s3://quilt-example"
+        >>> pkg = "quilt/data"
+        >>> pkg_full = f"{pkg}:latest"
+        >>> path = "foo/bar"
+        >>> uri = f"{QuiltUri.PREFIX}{reg}#package={pkg_full}&path={path}"
+        >>> attrs = UnUri(uri).attrs
+        >>> quilt = QuiltUri(attrs)
+        >>> quilt.uri == uri
+        True
+        >>> quilt.registry == reg
+        True
+        >>> quilt.package == pkg
+        True
+        >>> quilt.attrs[QuiltUri.K_PKG] == pkg_full
+        True
+        >>> quilt.attrs[QuiltUri.K_PKG_NAME]
+        'quilt/data'
+        >>> quilt.attrs[QuiltUri.K_PKG_PRE]
+        'quilt'
+        >>> quilt.attrs[QuiltUri.K_PKG_SUF]
+        'data'
+        >>> quilt.attrs[QuiltUri.K_PTH] == path
+        True
+        """
         self.attrs = attrs
         self.uri = attrs.get(UnUri.K_URI)
         self.registry = f"{attrs.get(UnUri.K_PROT)}://{attrs.get(UnUri.K_HOST)}"
-        package = self.parse_package()
-        self.package: str = package if isinstance(package, str) else ""
+        self.package = self.parse_package()
 
     def __repr__(self):
         return f"QuiltUri({self.uri})"
 
     def __eq__(self, other: object):
         if not isinstance(other, QuiltUri):
             return NotImplemented
@@ -43,16 +73,25 @@
         pkg = self.full_package()
         if isinstance(pkg, str) and sep in pkg:
             s = pkg.split(sep)
             self.attrs[key] = s[1]
             return s[0]
         return False
 
-    def parse_package(self) -> str | bool:
-        return (
+    def parse_package(self) -> str:
+        package = (
             self.split_package(QuiltUri.K_HASH)
             or self.split_package(QuiltUri.K_TAG)
             or self.full_package()
         )
+        sep = QuiltUri.SEP[QuiltUri.K_PKG]
+        if not isinstance(package, str) or sep not in package:
+            return ""
+
+        split = package.split(sep)
+        self.attrs[QuiltUri.K_PKG_NAME] = package
+        self.attrs[QuiltUri.K_PKG_PRE] = split[0]
+        self.attrs[QuiltUri.K_PKG_SUF] = split[1]
+        return package
 
     def has_package(self) -> bool:
         return QuiltUri.SEP[QuiltUri.K_PKG] in self.package if self.package else False
```

### Comparing `quiltplus-0.9.4/quiltplus/versions.py` & `quiltplus-0.9.5/quiltplus/versions.py`

 * *Files identical despite different names*

### Comparing `quiltplus-0.9.4/PKG-INFO` & `quiltplus-0.9.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quiltplus
-Version: 0.9.4
+Version: 0.9.5
 Summary: Resource-oriented Python API/CLI for Quilt's decentralized social knowledge platform
 License: MIT
 Keywords: yaml,api,resource,quilt
 Author: Ernest Prabhakar
 Author-email: ernest@quiltdata.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

