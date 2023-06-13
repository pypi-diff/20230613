# Comparing `tmp/zeroconf-0.64.1.tar.gz` & `tmp/zeroconf-0.65.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zeroconf-0.64.1.tar", max compression
+gzip compressed data, was "zeroconf-0.65.0.tar", max compression
```

## Comparing `zeroconf-0.64.1.tar` & `zeroconf-0.65.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    52504 2023-06-05 14:49:16.297094 zeroconf-0.64.1/CHANGELOG.md
--rw-r--r--   0        0        0    24380 2023-06-05 14:49:15.205081 zeroconf-0.64.1/COPYING
--rw-r--r--   0        0        0     4407 2023-06-05 14:49:15.209081 zeroconf-0.64.1/README.rst
--rw-r--r--   0        0        0     1060 2023-06-05 14:49:15.209081 zeroconf-0.64.1/build_ext.py
--rw-r--r--   0        0        0     6770 2023-06-05 14:49:15.209081 zeroconf-0.64.1/docs/Makefile
--rw-r--r--   0        0        0      234 2023-06-05 14:49:15.209081 zeroconf-0.64.1/docs/api.rst
--rw-r--r--   0        0        0     8145 2023-06-05 14:49:15.209081 zeroconf-0.64.1/docs/conf.py
--rw-r--r--   0        0        0      991 2023-06-05 14:49:15.209081 zeroconf-0.64.1/docs/index.rst
--rw-r--r--   0        0        0     3995 2023-06-05 14:49:16.401095 zeroconf-0.64.1/pyproject.toml
--rw-r--r--   0        0        0     3868 2023-06-05 14:49:16.309094 zeroconf-0.64.1/src/zeroconf/__init__.py
--rw-r--r--   0        0        0      897 2023-06-05 14:49:15.209081 zeroconf-0.64.1/src/zeroconf/_cache.pxd
--rw-r--r--   0        0        0    10036 2023-06-05 14:49:15.209081 zeroconf-0.64.1/src/zeroconf/_cache.py
--rw-r--r--   0        0        0    39337 2023-06-05 14:49:15.209081 zeroconf-0.64.1/src/zeroconf/_core.py
--rw-r--r--   0        0        0     2061 2023-06-05 14:49:15.209081 zeroconf-0.64.1/src/zeroconf/_dns.pxd
--rw-r--r--   0        0        0    18218 2023-06-05 14:49:15.209081 zeroconf-0.64.1/src/zeroconf/_dns.py
--rw-r--r--   0        0        0     2167 2023-06-05 14:49:15.209081 zeroconf-0.64.1/src/zeroconf/_exceptions.py
--rw-r--r--   0        0        0    24202 2023-06-05 14:49:15.209081 zeroconf-0.64.1/src/zeroconf/_handlers.py
--rw-r--r--   0        0        0     2916 2023-06-05 14:49:15.209081 zeroconf-0.64.1/src/zeroconf/_history.py
--rw-r--r--   0        0        0     2980 2023-06-05 14:49:15.209081 zeroconf-0.64.1/src/zeroconf/_logger.py
--rw-r--r--   0        0        0      971 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_protocol/__init__.py
--rw-r--r--   0        0        0     2661 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_protocol/incoming.pxd
--rw-r--r--   0        0        0    14335 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_protocol/incoming.py
--rw-r--r--   0        0        0     1950 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_protocol/outgoing.pxd
--rw-r--r--   0        0        0    17758 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_protocol/outgoing.py
--rw-r--r--   0        0        0     2355 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_services/__init__.py
--rw-r--r--   0        0        0    22413 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_services/browser.py
--rw-r--r--   0        0        0    26716 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_services/info.py
--rw-r--r--   0        0        0     3948 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_services/registry.py
--rw-r--r--   0        0        0     3003 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_services/types.py
--rw-r--r--   0        0        0     2909 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_updates.py
--rw-r--r--   0        0        0      971 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_utils/__init__.py
--rw-r--r--   0        0        0     4144 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_utils/asyncio.py
--rw-r--r--   0        0        0     6904 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_utils/name.py
--rw-r--r--   0        0        0    15252 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_utils/net.py
--rw-r--r--   0        0        0     1308 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/_utils/time.py
--rw-r--r--   0        0        0    11084 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/asyncio.py
--rw-r--r--   0        0        0     4515 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/const.py
--rw-r--r--   0        0        0        0 2023-06-05 14:49:15.213081 zeroconf-0.64.1/src/zeroconf/py.typed
--rw-r--r--   0        0        0     2416 2023-06-05 14:49:15.213081 zeroconf-0.64.1/tests/__init__.py
--rw-r--r--   0        0        0     1057 2023-06-05 14:49:15.213081 zeroconf-0.64.1/tests/conftest.py
--rw-r--r--   0        0        0      971 2023-06-05 14:49:15.213081 zeroconf-0.64.1/tests/services/__init__.py
--rw-r--r--   0        0        0    42949 2023-06-05 14:49:15.213081 zeroconf-0.64.1/tests/services/test_browser.py
--rw-r--r--   0        0        0    45240 2023-06-05 14:49:15.213081 zeroconf-0.64.1/tests/services/test_info.py
--rw-r--r--   0        0        0     4157 2023-06-05 14:49:15.213081 zeroconf-0.64.1/tests/services/test_registry.py
--rw-r--r--   0        0        0     4681 2023-06-05 14:49:15.213081 zeroconf-0.64.1/tests/services/test_types.py
--rw-r--r--   0        0        0    44525 2023-06-05 14:49:15.213081 zeroconf-0.64.1/tests/test_asyncio.py
--rw-r--r--   0        0        0     8830 2023-06-05 14:49:15.213081 zeroconf-0.64.1/tests/test_cache.py
--rw-r--r--   0        0        0    32162 2023-06-05 14:49:15.213081 zeroconf-0.64.1/tests/test_core.py
--rw-r--r--   0        0        0    14686 2023-06-05 14:49:15.213081 zeroconf-0.64.1/tests/test_dns.py
--rw-r--r--   0        0        0     5021 2023-06-05 14:49:15.213081 zeroconf-0.64.1/tests/test_exceptions.py
--rw-r--r--   0        0        0    67411 2023-06-05 14:49:15.217081 zeroconf-0.64.1/tests/test_handlers.py
--rw-r--r--   0        0        0     2580 2023-06-05 14:49:15.217081 zeroconf-0.64.1/tests/test_history.py
--rw-r--r--   0        0        0     6640 2023-06-05 14:49:15.217081 zeroconf-0.64.1/tests/test_init.py
--rw-r--r--   0        0        0     3396 2023-06-05 14:49:15.217081 zeroconf-0.64.1/tests/test_logger.py
--rw-r--r--   0        0        0    41672 2023-06-05 14:49:15.217081 zeroconf-0.64.1/tests/test_protocol.py
--rw-r--r--   0        0        0     8849 2023-06-05 14:49:15.217081 zeroconf-0.64.1/tests/test_services.py
--rw-r--r--   0        0        0     2240 2023-06-05 14:49:15.217081 zeroconf-0.64.1/tests/test_updates.py
--rw-r--r--   0        0        0      971 2023-06-05 14:49:15.217081 zeroconf-0.64.1/tests/utils/__init__.py
--rw-r--r--   0        0        0     5101 2023-06-05 14:49:15.217081 zeroconf-0.64.1/tests/utils/test_asyncio.py
--rw-r--r--   0        0        0     2045 2023-06-05 14:49:15.217081 zeroconf-0.64.1/tests/utils/test_name.py
--rw-r--r--   0        0        0     9413 2023-06-05 14:49:15.217081 zeroconf-0.64.1/tests/utils/test_net.py
--rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.64.1/setup.py
--rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.64.1/PKG-INFO
+-rw-r--r--   0        0        0    52788 2023-06-13 00:26:07.182440 zeroconf-0.65.0/CHANGELOG.md
+-rw-r--r--   0        0        0    24380 2023-06-13 00:26:06.394436 zeroconf-0.65.0/COPYING
+-rw-r--r--   0        0        0     4407 2023-06-13 00:26:06.394436 zeroconf-0.65.0/README.rst
+-rw-r--r--   0        0        0     1060 2023-06-13 00:26:06.394436 zeroconf-0.65.0/build_ext.py
+-rw-r--r--   0        0        0     6770 2023-06-13 00:26:06.394436 zeroconf-0.65.0/docs/Makefile
+-rw-r--r--   0        0        0      234 2023-06-13 00:26:06.394436 zeroconf-0.65.0/docs/api.rst
+-rw-r--r--   0        0        0     8145 2023-06-13 00:26:06.394436 zeroconf-0.65.0/docs/conf.py
+-rw-r--r--   0        0        0      991 2023-06-13 00:26:06.394436 zeroconf-0.65.0/docs/index.rst
+-rw-r--r--   0        0        0     3995 2023-06-13 00:26:07.258441 zeroconf-0.65.0/pyproject.toml
+-rw-r--r--   0        0        0     3868 2023-06-13 00:26:07.190440 zeroconf-0.65.0/src/zeroconf/__init__.py
+-rw-r--r--   0        0        0      897 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_cache.pxd
+-rw-r--r--   0        0        0    10036 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_cache.py
+-rw-r--r--   0        0        0    39337 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_core.py
+-rw-r--r--   0        0        0     2061 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_dns.pxd
+-rw-r--r--   0        0        0    18218 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_dns.py
+-rw-r--r--   0        0        0     2167 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_exceptions.py
+-rw-r--r--   0        0        0    24202 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_handlers.py
+-rw-r--r--   0        0        0     2916 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_history.py
+-rw-r--r--   0        0        0     2980 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_logger.py
+-rw-r--r--   0        0        0      971 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_protocol/__init__.py
+-rw-r--r--   0        0        0     2661 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_protocol/incoming.pxd
+-rw-r--r--   0        0        0    14335 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_protocol/incoming.py
+-rw-r--r--   0        0        0     1950 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_protocol/outgoing.pxd
+-rw-r--r--   0        0        0    17758 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_protocol/outgoing.py
+-rw-r--r--   0        0        0     2355 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_services/__init__.py
+-rw-r--r--   0        0        0    22413 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_services/browser.py
+-rw-r--r--   0        0        0    27259 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_services/info.py
+-rw-r--r--   0        0        0     3948 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_services/registry.py
+-rw-r--r--   0        0        0     3003 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_services/types.py
+-rw-r--r--   0        0        0     2909 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_updates.py
+-rw-r--r--   0        0        0      971 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_utils/__init__.py
+-rw-r--r--   0        0        0     4144 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_utils/asyncio.py
+-rw-r--r--   0        0        0     6904 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_utils/name.py
+-rw-r--r--   0        0        0    15252 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_utils/net.py
+-rw-r--r--   0        0        0     1308 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/_utils/time.py
+-rw-r--r--   0        0        0    11084 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/asyncio.py
+-rw-r--r--   0        0        0     4515 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/const.py
+-rw-r--r--   0        0        0        0 2023-06-13 00:26:06.398436 zeroconf-0.65.0/src/zeroconf/py.typed
+-rw-r--r--   0        0        0     2416 2023-06-13 00:26:06.398436 zeroconf-0.65.0/tests/__init__.py
+-rw-r--r--   0        0        0     1057 2023-06-13 00:26:06.398436 zeroconf-0.65.0/tests/conftest.py
+-rw-r--r--   0        0        0      971 2023-06-13 00:26:06.398436 zeroconf-0.65.0/tests/services/__init__.py
+-rw-r--r--   0        0        0    42949 2023-06-13 00:26:06.398436 zeroconf-0.65.0/tests/services/test_browser.py
+-rw-r--r--   0        0        0    45240 2023-06-13 00:26:06.398436 zeroconf-0.65.0/tests/services/test_info.py
+-rw-r--r--   0        0        0     4157 2023-06-13 00:26:06.398436 zeroconf-0.65.0/tests/services/test_registry.py
+-rw-r--r--   0        0        0     4681 2023-06-13 00:26:06.398436 zeroconf-0.65.0/tests/services/test_types.py
+-rw-r--r--   0        0        0    44525 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/test_asyncio.py
+-rw-r--r--   0        0        0     8830 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/test_cache.py
+-rw-r--r--   0        0        0    32162 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/test_core.py
+-rw-r--r--   0        0        0    14686 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/test_dns.py
+-rw-r--r--   0        0        0     5021 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/test_exceptions.py
+-rw-r--r--   0        0        0    67411 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/test_handlers.py
+-rw-r--r--   0        0        0     2580 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/test_history.py
+-rw-r--r--   0        0        0     6640 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/test_init.py
+-rw-r--r--   0        0        0     3396 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/test_logger.py
+-rw-r--r--   0        0        0    41672 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/test_protocol.py
+-rw-r--r--   0        0        0     8849 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/test_services.py
+-rw-r--r--   0        0        0     2240 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/test_updates.py
+-rw-r--r--   0        0        0      971 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/utils/__init__.py
+-rw-r--r--   0        0        0     5101 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/utils/test_asyncio.py
+-rw-r--r--   0        0        0     2045 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/utils/test_name.py
+-rw-r--r--   0        0        0     9413 2023-06-13 00:26:06.402436 zeroconf-0.65.0/tests/utils/test_net.py
+-rw-r--r--   0        0        0     5527 1970-01-01 00:00:00.000000 zeroconf-0.65.0/setup.py
+-rw-r--r--   0        0        0     6045 1970-01-01 00:00:00.000000 zeroconf-0.65.0/PKG-INFO
```

### Comparing `zeroconf-0.64.1/CHANGELOG.md` & `zeroconf-0.65.0/CHANGELOG.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 <!--next-version-placeholder-->
 
+## v0.65.0 (2023-06-13)
+### Feature
+* Reduce overhead to enumerate ip addresses in ServiceInfo ([#1181](https://github.com/python-zeroconf/python-zeroconf/issues/1181)) ([`6a85cbf`](https://github.com/python-zeroconf/python-zeroconf/commit/6a85cbf2b872cb0abd184c2dd728d9ae3eb8115c))
+
 ## v0.64.1 (2023-06-05)
 ### Fix
 * Small internal typing cleanups ([#1180](https://github.com/python-zeroconf/python-zeroconf/issues/1180)) ([`f03e511`](https://github.com/python-zeroconf/python-zeroconf/commit/f03e511f7aae72c5ccd4f7514d89e168847bd7a2))
 
 ## v0.64.0 (2023-06-05)
 ### Feature
 * Speed up processing incoming records ([#1179](https://github.com/python-zeroconf/python-zeroconf/issues/1179)) ([`d919316`](https://github.com/python-zeroconf/python-zeroconf/commit/d9193160b05beeca3755e19fd377ba13fe37b071))
```

### Comparing `zeroconf-0.64.1/COPYING` & `zeroconf-0.65.0/COPYING`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/README.rst` & `zeroconf-0.65.0/README.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/build_ext.py` & `zeroconf-0.65.0/build_ext.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/docs/Makefile` & `zeroconf-0.65.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/docs/conf.py` & `zeroconf-0.65.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/docs/index.rst` & `zeroconf-0.65.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/pyproject.toml` & `zeroconf-0.65.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "zeroconf"
-version = "0.64.1"
+version = "0.65.0"
 description = "A pure python implementation of multicast DNS service discovery"
 authors = ["Paul Scott-Murphy", "William McBrine", "Jakub Stasiak", "J. Nick Koston"]
 license = "LGPL"
 readme = "README.rst"
 repository = "https://github.com/python-zeroconf/python-zeroconf"
 documentation = "https://python-zeroconf.readthedocs.io"
 classifiers=[
```

### Comparing `zeroconf-0.64.1/src/zeroconf/__init__.py` & `zeroconf-0.65.0/src/zeroconf/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
 from ._utils.time import (  # noqa # import needed for backwards compat
     current_time_millis,
     millis_to_seconds,
 )
 
 __author__ = 'Paul Scott-Murphy, William McBrine'
 __maintainer__ = 'Jakub Stasiak <jakub@stasiak.at>'
-__version__ = '0.64.1'
+__version__ = '0.65.0'
 __license__ = 'LGPL'
 
 
 __all__ = [
     "__version__",
     "Zeroconf",
     "ServiceInfo",
```

### Comparing `zeroconf-0.64.1/src/zeroconf/_cache.pxd` & `zeroconf-0.65.0/src/zeroconf/_cache.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_cache.py` & `zeroconf-0.65.0/src/zeroconf/_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_core.py` & `zeroconf-0.65.0/src/zeroconf/_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_dns.pxd` & `zeroconf-0.65.0/src/zeroconf/_dns.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_dns.py` & `zeroconf-0.65.0/src/zeroconf/_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_exceptions.py` & `zeroconf-0.65.0/src/zeroconf/_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_handlers.py` & `zeroconf-0.65.0/src/zeroconf/_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_history.py` & `zeroconf-0.65.0/src/zeroconf/_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_logger.py` & `zeroconf-0.65.0/src/zeroconf/_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_protocol/__init__.py` & `zeroconf-0.65.0/src/zeroconf/_protocol/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_protocol/incoming.pxd` & `zeroconf-0.65.0/src/zeroconf/_protocol/incoming.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_protocol/incoming.py` & `zeroconf-0.65.0/src/zeroconf/_protocol/incoming.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_protocol/outgoing.pxd` & `zeroconf-0.65.0/src/zeroconf/_protocol/outgoing.pxd`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_protocol/outgoing.py` & `zeroconf-0.65.0/src/zeroconf/_protocol/outgoing.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_services/__init__.py` & `zeroconf-0.65.0/src/zeroconf/_services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_services/browser.py` & `zeroconf-0.65.0/src/zeroconf/_services/browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_services/info.py` & `zeroconf-0.65.0/src/zeroconf/_services/info.py`

 * *Files 10% similar despite different names*

```diff
@@ -59,14 +59,16 @@
     _TYPE_AAAA,
     _TYPE_NSEC,
     _TYPE_PTR,
     _TYPE_SRV,
     _TYPE_TXT,
 )
 
+_IPVersion_All_value = IPVersion.All.value
+_IPVersion_V4Only_value = IPVersion.V4Only.value
 # https://datatracker.ietf.org/doc/html/rfc6762#section-5.2
 # The most common case for calling ServiceInfo is from a
 # ServiceBrowser. After the first request we add a few random
 # milliseconds to the delay between requests to reduce the chance
 # that there are multiple ServiceBrowser callbacks running on
 # the network that are firing at the same time when they
 # see the same multicast response and decide to refresh
@@ -241,50 +243,57 @@
 
         Addresses are guaranteed to be returned in LIFO (last in, first out)
         order with IPv4 addresses first and IPv6 addresses second.
 
         This means the first address will always be the most recently added
         address of the given IP version.
         """
-        if version == IPVersion.V4Only:
+        version_value = version.value
+        if version_value == _IPVersion_All_value:
+            return [
+                *(addr.packed for addr in self._ipv4_addresses),
+                *(addr.packed for addr in self._ipv6_addresses),
+            ]
+        if version_value == _IPVersion_V4Only_value:
             return [addr.packed for addr in self._ipv4_addresses]
-        if version == IPVersion.V6Only:
-            return [addr.packed for addr in self._ipv6_addresses]
-        return [
-            *(addr.packed for addr in self._ipv4_addresses),
-            *(addr.packed for addr in self._ipv6_addresses),
-        ]
+        return [addr.packed for addr in self._ipv6_addresses]
 
     def ip_addresses_by_version(
         self, version: IPVersion
     ) -> Union[List[ipaddress.IPv4Address], List[ipaddress.IPv6Address], List[ipaddress._BaseAddress]]:
         """List ip_address objects matching IP version.
 
         Addresses are guaranteed to be returned in LIFO (last in, first out)
         order with IPv4 addresses first and IPv6 addresses second.
 
         This means the first address will always be the most recently added
         address of the given IP version.
         """
-        if version == IPVersion.V4Only:
+        return self._ip_addresses_by_version_value(version.value)
+
+    def _ip_addresses_by_version_value(
+        self, version_value: int
+    ) -> Union[List[ipaddress.IPv4Address], List[ipaddress.IPv6Address], List[ipaddress._BaseAddress]]:
+        """Backend for addresses_by_version that uses the raw value."""
+        if version_value == _IPVersion_All_value:
+            return [*self._ipv4_addresses, *self._ipv6_addresses]
+        if version_value == _IPVersion_V4Only_value:
             return self._ipv4_addresses
-        if version == IPVersion.V6Only:
-            return self._ipv6_addresses
-        return [*self._ipv4_addresses, *self._ipv6_addresses]
+        return self._ipv6_addresses
 
     def parsed_addresses(self, version: IPVersion = IPVersion.All) -> List[str]:
         """List addresses in their parsed string form.
 
         Addresses are guaranteed to be returned in LIFO (last in, first out)
         order with IPv4 addresses first and IPv6 addresses second.
 
         This means the first address will always be the most recently added
         address of the given IP version.
         """
-        return [str(addr) for addr in self.ip_addresses_by_version(version)]
+        return [str(addr) for addr in self._ip_addresses_by_version_value(version.value)]
 
     def parsed_scoped_addresses(self, version: IPVersion = IPVersion.All) -> List[str]:
         """Equivalent to parsed_addresses, with the exception that IPv6 Link-Local
         addresses are qualified with %<interface_index> when available
 
         Addresses are guaranteed to be returned in LIFO (last in, first out)
         order with IPv4 addresses first and IPv6 addresses second.
@@ -292,15 +301,15 @@
         This means the first address will always be the most recently added
         address of the given IP version.
         """
         if self.interface_index is None:
             return self.parsed_addresses(version)
         return [
             f"{addr}%{self.interface_index}" if addr.version == 6 and addr.is_link_local else str(addr)
-            for addr in self.ip_addresses_by_version(version)
+            for addr in self._ip_addresses_by_version_value(version.value)
         ]
 
     def _set_properties(self, properties: Dict) -> None:
         """Sets properties and text of this info from a dictionary"""
         self._properties = properties
         list_ = []
         result = b''
@@ -490,15 +499,15 @@
                 name,
                 _TYPE_AAAA if address.version == 6 else _TYPE_A,
                 class_,
                 ttl,
                 address.packed,
                 created=created,
             )
-            for address in self.ip_addresses_by_version(version)
+            for address in self._ip_addresses_by_version_value(version.value)
         ]
 
     def dns_pointer(self, override_ttl: Optional[int] = None, created: Optional[float] = None) -> DNSPointer:
         """Return DNSPointer from ServiceInfo."""
         return DNSPointer(
             self.type,
             _TYPE_PTR,
```

### Comparing `zeroconf-0.64.1/src/zeroconf/_services/registry.py` & `zeroconf-0.65.0/src/zeroconf/_services/registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_services/types.py` & `zeroconf-0.65.0/src/zeroconf/_services/types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_updates.py` & `zeroconf-0.65.0/src/zeroconf/_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_utils/__init__.py` & `zeroconf-0.65.0/src/zeroconf/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_utils/asyncio.py` & `zeroconf-0.65.0/src/zeroconf/_utils/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_utils/name.py` & `zeroconf-0.65.0/src/zeroconf/_utils/name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_utils/net.py` & `zeroconf-0.65.0/src/zeroconf/_utils/net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/_utils/time.py` & `zeroconf-0.65.0/src/zeroconf/_utils/time.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/asyncio.py` & `zeroconf-0.65.0/src/zeroconf/asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/src/zeroconf/const.py` & `zeroconf-0.65.0/src/zeroconf/const.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/__init__.py` & `zeroconf-0.65.0/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/conftest.py` & `zeroconf-0.65.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/services/__init__.py` & `zeroconf-0.65.0/tests/services/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/services/test_browser.py` & `zeroconf-0.65.0/tests/services/test_browser.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/services/test_info.py` & `zeroconf-0.65.0/tests/services/test_info.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/services/test_registry.py` & `zeroconf-0.65.0/tests/services/test_registry.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/services/test_types.py` & `zeroconf-0.65.0/tests/services/test_types.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/test_asyncio.py` & `zeroconf-0.65.0/tests/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/test_cache.py` & `zeroconf-0.65.0/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/test_core.py` & `zeroconf-0.65.0/tests/test_core.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/test_dns.py` & `zeroconf-0.65.0/tests/test_dns.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/test_exceptions.py` & `zeroconf-0.65.0/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/test_handlers.py` & `zeroconf-0.65.0/tests/test_handlers.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/test_history.py` & `zeroconf-0.65.0/tests/test_history.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/test_init.py` & `zeroconf-0.65.0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/test_logger.py` & `zeroconf-0.65.0/tests/test_logger.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/test_protocol.py` & `zeroconf-0.65.0/tests/test_protocol.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/test_services.py` & `zeroconf-0.65.0/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/test_updates.py` & `zeroconf-0.65.0/tests/test_updates.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/utils/__init__.py` & `zeroconf-0.65.0/tests/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/utils/test_asyncio.py` & `zeroconf-0.65.0/tests/utils/test_asyncio.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/utils/test_name.py` & `zeroconf-0.65.0/tests/utils/test_name.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/tests/utils/test_net.py` & `zeroconf-0.65.0/tests/utils/test_net.py`

 * *Files identical despite different names*

### Comparing `zeroconf-0.64.1/setup.py` & `zeroconf-0.65.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 ['ifaddr>=0.1.7']
 
 extras_require = \
 {':python_version < "3.11"': ['async-timeout>=3.0.0']}
 
 setup_kwargs = {
     'name': 'zeroconf',
-    'version': '0.64.1',
+    'version': '0.65.0',
     'description': 'A pure python implementation of multicast DNS service discovery',
     'long_description': 'python-zeroconf\n===============\n\n.. image:: https://github.com/python-zeroconf/python-zeroconf/workflows/CI/badge.svg\n   :target: https://github.com/python-zeroconf/python-zeroconf?query=workflow%3ACI+branch%3Amaster\n\n.. image:: https://img.shields.io/pypi/v/zeroconf.svg\n    :target: https://pypi.python.org/pypi/zeroconf\n\n.. image:: https://codecov.io/gh/python-zeroconf/python-zeroconf/branch/master/graph/badge.svg\n   :target: https://codecov.io/gh/python-zeroconf/python-zeroconf\n\n`Documentation <https://python-zeroconf.readthedocs.io/en/latest/>`_.\n\nThis is fork of pyzeroconf, Multicast DNS Service Discovery for Python,\noriginally by Paul Scott-Murphy (https://github.com/paulsm/pyzeroconf),\nmodified by William McBrine (https://github.com/wmcbrine/pyzeroconf).\n\nThe original William McBrine\'s fork note::\n\n    This fork is used in all of my TiVo-related projects: HME for Python\n    (and therefore HME/VLC), Network Remote, Remote Proxy, and pyTivo.\n    Before this, I was tracking the changes for zeroconf.py in three\n    separate repos. I figured I should have an authoritative source.\n\n    Although I make changes based on my experience with TiVos, I expect that\n    they\'re generally applicable. This version also includes patches found\n    on the now-defunct (?) Launchpad repo of pyzeroconf, and elsewhere\n    around the net -- not always well-documented, sorry.\n\nCompatible with:\n\n* Bonjour\n* Avahi\n\nCompared to some other Zeroconf/Bonjour/Avahi Python packages, python-zeroconf:\n\n* isn\'t tied to Bonjour or Avahi\n* doesn\'t use D-Bus\n* doesn\'t force you to use particular event loop or Twisted (asyncio is used under the hood but not required)\n* is pip-installable\n* has PyPI distribution\n* has an optional cython extension for performance (pure python is supported as well)\n\nPython compatibility\n--------------------\n\n* CPython 3.7+\n* PyPy3.7 7.3+\n\nVersioning\n----------\n\nThis project uses semantic versioning.\n\nStatus\n------\n\nThis project is actively maintained.\n\nTraffic Reduction\n-----------------\n\nBefore version 0.32, most traffic reduction techniques described in https://datatracker.ietf.org/doc/html/rfc6762#section-7\nwhere not implemented which could lead to excessive network traffic.  It is highly recommended that version 0.32 or later\nis used if this is a concern.\n\nIPv6 support\n------------\n\nIPv6 support is relatively new and currently limited, specifically:\n\n* `InterfaceChoice.All` is an alias for `InterfaceChoice.Default` on non-POSIX\n  systems.\n* Dual-stack IPv6 sockets are used, which may not be supported everywhere (some\n  BSD variants do not have them).\n* Listening on localhost (`::1`) does not work. Help with understanding why is\n  appreciated.\n\nHow to get python-zeroconf?\n===========================\n\n* PyPI page https://pypi.org/project/zeroconf/\n* GitHub project https://github.com/python-zeroconf/python-zeroconf\n\nThe easiest way to install python-zeroconf is using pip::\n\n    pip install zeroconf\n\n\n\nHow do I use it?\n================\n\nHere\'s an example of browsing for a service:\n\n.. code-block:: python\n\n    from zeroconf import ServiceBrowser, ServiceListener, Zeroconf\n\n\n    class MyListener(ServiceListener):\n\n        def update_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} updated")\n\n        def remove_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            print(f"Service {name} removed")\n\n        def add_service(self, zc: Zeroconf, type_: str, name: str) -> None:\n            info = zc.get_service_info(type_, name)\n            print(f"Service {name} added, service info: {info}")\n\n\n    zeroconf = Zeroconf()\n    listener = MyListener()\n    browser = ServiceBrowser(zeroconf, "_http._tcp.local.", listener)\n    try:\n        input("Press enter to exit...\\n\\n")\n    finally:\n        zeroconf.close()\n\n.. note::\n\n    Discovery and service registration use *all* available network interfaces by default.\n    If you want to customize that you need to specify ``interfaces`` argument when\n    constructing ``Zeroconf`` object (see the code for details).\n\nIf you don\'t know the name of the service you need to browse for, try:\n\n.. code-block:: python\n\n    from zeroconf import ZeroconfServiceTypes\n    print(\'\\n\'.join(ZeroconfServiceTypes.find()))\n\nSee examples directory for more.\n\nChangelog\n=========\n\n`Changelog <CHANGELOG.md>`_\n\nLicense\n=======\n\nLGPL, see COPYING file for details.\n',
     'author': 'Paul Scott-Murphy',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/python-zeroconf/python-zeroconf',
```

### Comparing `zeroconf-0.64.1/PKG-INFO` & `zeroconf-0.65.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zeroconf
-Version: 0.64.1
+Version: 0.65.0
 Summary: A pure python implementation of multicast DNS service discovery
 Home-page: https://github.com/python-zeroconf/python-zeroconf
 License: LGPL
 Author: Paul Scott-Murphy
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

