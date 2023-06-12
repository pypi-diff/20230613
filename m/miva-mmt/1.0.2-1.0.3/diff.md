# Comparing `tmp/miva-mmt-1.0.2.tar.gz` & `tmp/miva-mmt-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miva-mmt-1.0.2.tar", last modified: Wed Nov 30 18:41:23 2022, max compression
+gzip compressed data, was "miva-mmt-1.0.3.tar", last modified: Tue Jun  6 16:29:12 2023, max compression
```

## Comparing `miva-mmt-1.0.2.tar` & `miva-mmt-1.0.3.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-11-30 18:41:23.207222 miva-mmt-1.0.2/
--rw-r-----   0 root         (0) root         (0)    13203 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/LICENSE
--rw-r-----   0 root         (0) root         (0)       60 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/MANIFEST.in
--rw-rw-rw-   0 root         (0) root         (0)     2316 2022-11-30 18:41:23.206222 miva-mmt-1.0.2/PKG-INFO
--rw-r-----   0 root         (0) root         (0)     1616 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-11-30 18:41:23.203222 miva-mmt-1.0.2/miva_mmt.egg-info/
--rw-rw-rw-   0 root         (0) root         (0)     2316 2022-11-30 18:41:23.000000 miva-mmt-1.0.2/miva_mmt.egg-info/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      881 2022-11-30 18:41:23.000000 miva-mmt-1.0.2/miva_mmt.egg-info/SOURCES.txt
--rw-rw-rw-   0 root         (0) root         (0)        1 2022-11-30 18:41:23.000000 miva-mmt-1.0.2/miva_mmt.egg-info/dependency_links.txt
--rw-rw-rw-   0 root         (0) root         (0)       34 2022-11-30 18:41:23.000000 miva-mmt-1.0.2/miva_mmt.egg-info/entry_points.txt
--rw-rw-rw-   0 root         (0) root         (0)       19 2022-11-30 18:41:23.000000 miva-mmt-1.0.2/miva_mmt.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)        9 2022-11-30 18:41:23.000000 miva-mmt-1.0.2/miva_mmt.egg-info/top_level.txt
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-11-30 18:41:23.204222 miva-mmt-1.0.2/mmt/
--rw-r-----   0 root         (0) root         (0)    16107 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-11-30 18:41:23.205222 miva-mmt-1.0.2/mmt/commands/
--rw-r-----   0 root         (0) root         (0)    27157 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/__init__.py
--rw-r-----   0 root         (0) root         (0)     4907 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/branch.py
--rw-r-----   0 root         (0) root         (0)    15779 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/checkout.py
--rw-r-----   0 root         (0) root         (0)     2393 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/config.py
--rw-r-----   0 root         (0) root         (0)     8425 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/credential.py
--rw-r-----   0 root         (0) root         (0)    12451 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/diff.py
--rw-r-----   0 root         (0) root         (0)     1745 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/info.py
--rw-r-----   0 root         (0) root         (0)     2199 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/log.py
--rw-r-----   0 root         (0) root         (0)    35862 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/pull.py
--rw-r-----   0 root         (0) root         (0)    15978 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/push.py
--rw-r-----   0 root         (0) root         (0)     3619 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/remote.py
--rw-r-----   0 root         (0) root         (0)    12544 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/revert.py
--rw-r-----   0 root         (0) root         (0)      834 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/status.py
--rw-r-----   0 root         (0) root         (0)    13448 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/switch.py
--rw-r-----   0 root         (0) root         (0)     1892 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/commands/tag.py
--rw-r-----   0 root         (0) root         (0)     1316 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/exceptions.py
--rw-r-----   0 root         (0) root         (0)     2023 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/file.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-11-30 18:41:23.206222 miva-mmt-1.0.2/mmt/managers/
--rw-r-----   0 root         (0) root         (0)        0 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/managers/__init__.py
--rw-r-----   0 root         (0) root         (0)     1654 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/managers/config.py
--rw-r-----   0 root         (0) root         (0)     6919 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/managers/credential.py
--rw-r-----   0 root         (0) root         (0)     2629 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/managers/remote.py
--rw-r-----   0 root         (0) root         (0)     1301 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/managers/setting.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2022-11-30 18:41:23.206222 miva-mmt-1.0.2/mmt/metadata/
--rw-r-----   0 root         (0) root         (0)     1425 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/metadata/__init__.py
--rw-r-----   0 root         (0) root         (0)     1762 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/metadata/config.py
--rw-r-----   0 root         (0) root         (0)     6382 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/metadata/globalconfig.py
--rw-r-----   0 root         (0) root         (0)     3695 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/metadata/localconfig.py
--rw-r-----   0 root         (0) root         (0)    16307 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/metadata/state.py
--rw-r-----   0 root         (0) root         (0)       22 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/mmt/version.py
--rw-rw-rw-   0 root         (0) root         (0)       38 2022-11-30 18:41:23.207222 miva-mmt-1.0.2/setup.cfg
--rw-r-----   0 root         (0) root         (0)      853 2022-11-30 18:41:22.000000 miva-mmt-1.0.2/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 16:29:12.671070 miva-mmt-1.0.3/
+-rw-r-----   0 root         (0) root         (0)    13203 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/LICENSE
+-rw-r-----   0 root         (0) root         (0)       60 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/MANIFEST.in
+-rw-rw-rw-   0 root         (0) root         (0)     2830 2023-06-06 16:29:12.671070 miva-mmt-1.0.3/PKG-INFO
+-rw-r-----   0 root         (0) root         (0)     2066 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 16:29:12.668070 miva-mmt-1.0.3/miva_mmt.egg-info/
+-rw-rw-rw-   0 root         (0) root         (0)     2830 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/miva_mmt.egg-info/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      881 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/miva_mmt.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)        1 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/miva_mmt.egg-info/dependency_links.txt
+-rw-rw-rw-   0 root         (0) root         (0)       34 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/miva_mmt.egg-info/entry_points.txt
+-rw-rw-rw-   0 root         (0) root         (0)       19 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/miva_mmt.egg-info/requires.txt
+-rw-rw-rw-   0 root         (0) root         (0)        9 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/miva_mmt.egg-info/top_level.txt
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 16:29:12.668070 miva-mmt-1.0.3/mmt/
+-rw-r-----   0 root         (0) root         (0)    16107 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 16:29:12.670070 miva-mmt-1.0.3/mmt/commands/
+-rw-r-----   0 root         (0) root         (0)    28791 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/__init__.py
+-rw-r-----   0 root         (0) root         (0)     4907 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/branch.py
+-rw-r-----   0 root         (0) root         (0)    15779 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/checkout.py
+-rw-r-----   0 root         (0) root         (0)     2393 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/config.py
+-rw-r-----   0 root         (0) root         (0)     8425 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/credential.py
+-rw-r-----   0 root         (0) root         (0)    12433 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/diff.py
+-rw-r-----   0 root         (0) root         (0)     1745 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/info.py
+-rw-r-----   0 root         (0) root         (0)     2199 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/log.py
+-rw-r-----   0 root         (0) root         (0)    36137 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/pull.py
+-rw-r-----   0 root         (0) root         (0)    15978 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/push.py
+-rw-r-----   0 root         (0) root         (0)     3619 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/remote.py
+-rw-r-----   0 root         (0) root         (0)    12530 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/revert.py
+-rw-r-----   0 root         (0) root         (0)      834 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/status.py
+-rw-r-----   0 root         (0) root         (0)    13448 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/switch.py
+-rw-r-----   0 root         (0) root         (0)     1892 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/commands/tag.py
+-rw-r-----   0 root         (0) root         (0)     1772 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/exceptions.py
+-rw-r-----   0 root         (0) root         (0)     2023 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/file.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 16:29:12.670070 miva-mmt-1.0.3/mmt/managers/
+-rw-r-----   0 root         (0) root         (0)        0 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/managers/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1654 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/managers/config.py
+-rw-r-----   0 root         (0) root         (0)     6919 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/managers/credential.py
+-rw-r-----   0 root         (0) root         (0)     2629 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/managers/remote.py
+-rw-r-----   0 root         (0) root         (0)     1301 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/managers/setting.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2023-06-06 16:29:12.671070 miva-mmt-1.0.3/mmt/metadata/
+-rw-r-----   0 root         (0) root         (0)     1425 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/metadata/__init__.py
+-rw-r-----   0 root         (0) root         (0)     1762 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/metadata/config.py
+-rw-r-----   0 root         (0) root         (0)     6382 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/metadata/globalconfig.py
+-rw-r-----   0 root         (0) root         (0)     3695 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/metadata/localconfig.py
+-rw-r-----   0 root         (0) root         (0)    16307 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/metadata/state.py
+-rw-r-----   0 root         (0) root         (0)       22 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/mmt/version.py
+-rw-rw-rw-   0 root         (0) root         (0)       38 2023-06-06 16:29:12.671070 miva-mmt-1.0.3/setup.cfg
+-rw-r-----   0 root         (0) root         (0)      853 2023-06-06 16:29:12.000000 miva-mmt-1.0.3/setup.py
```

### Comparing `miva-mmt-1.0.2/LICENSE` & `miva-mmt-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/PKG-INFO` & `miva-mmt-1.0.3/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miva-mmt
-Version: 1.0.2
+Version: 1.0.3
 Summary: Miva Managed Templates (MMT)
 Home-page: https://docs.miva.com/template-branches/template-branches-overview#mmt_overview
 Author: Miva, Inc.
 Author-email: support@miva.com
 License: MMT License Agreement
 Description: # MMT
         The Miva Managed Templates tool is a comprehensive command line
@@ -16,14 +16,22 @@
         
         # Requirements
         
         * Miva Merchant 10.00+
         * Python 3.6 or higher
         
         # Versions
+        ## 1.0.3
+        ### Bug Fixes
+        1. MMT-67: MMT should include a reason why Changeset_Create failed
+        1. MMT-71: MMT should handle a keyboard interrupt when requesting / receiving data
+        1. MMT-72: mmt diff should create a temporary file with the same file suffix as the file being diffed
+        1. MMT-79: Loading of properties no longer works with Miva Merchant 10.07.00
+        1. MMT-80: mmt pull does not handle resources converted from Inline / Local types to other types
+        
         ## 1.0.2
         ### New Features
         * Added --debug flag to view HTTP requests / responses
         ### Bug Fixes
         1. MMT-54: Add a --version flag
         1. MMT-55: Fatal error when attempting to checkout a file that contains invalid OS file name characters
         1. MMT-56: Add the ability to create a branch using a Remote key reference
```

### Comparing `miva-mmt-1.0.2/README.md` & `miva-mmt-1.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -8,14 +8,22 @@
 
 # Requirements
 
 * Miva Merchant 10.00+
 * Python 3.6 or higher
 
 # Versions
+## 1.0.3
+### Bug Fixes
+1. MMT-67: MMT should include a reason why Changeset_Create failed
+1. MMT-71: MMT should handle a keyboard interrupt when requesting / receiving data
+1. MMT-72: mmt diff should create a temporary file with the same file suffix as the file being diffed
+1. MMT-79: Loading of properties no longer works with Miva Merchant 10.07.00
+1. MMT-80: mmt pull does not handle resources converted from Inline / Local types to other types
+
 ## 1.0.2
 ### New Features
 * Added --debug flag to view HTTP requests / responses
 ### Bug Fixes
 1. MMT-54: Add a --version flag
 1. MMT-55: Fatal error when attempting to checkout a file that contains invalid OS file name characters
 1. MMT-56: Add the ability to create a branch using a Remote key reference
```

### Comparing `miva-mmt-1.0.2/miva_mmt.egg-info/PKG-INFO` & `miva-mmt-1.0.3/miva_mmt.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miva-mmt
-Version: 1.0.2
+Version: 1.0.3
 Summary: Miva Managed Templates (MMT)
 Home-page: https://docs.miva.com/template-branches/template-branches-overview#mmt_overview
 Author: Miva, Inc.
 Author-email: support@miva.com
 License: MMT License Agreement
 Description: # MMT
         The Miva Managed Templates tool is a comprehensive command line
@@ -16,14 +16,22 @@
         
         # Requirements
         
         * Miva Merchant 10.00+
         * Python 3.6 or higher
         
         # Versions
+        ## 1.0.3
+        ### Bug Fixes
+        1. MMT-67: MMT should include a reason why Changeset_Create failed
+        1. MMT-71: MMT should handle a keyboard interrupt when requesting / receiving data
+        1. MMT-72: mmt diff should create a temporary file with the same file suffix as the file being diffed
+        1. MMT-79: Loading of properties no longer works with Miva Merchant 10.07.00
+        1. MMT-80: mmt pull does not handle resources converted from Inline / Local types to other types
+        
         ## 1.0.2
         ### New Features
         * Added --debug flag to view HTTP requests / responses
         ### Bug Fixes
         1. MMT-54: Add a --version flag
         1. MMT-55: Fatal error when attempting to checkout a file that contains invalid OS file name characters
         1. MMT-56: Add the ability to create a branch using a Remote key reference
```

### Comparing `miva-mmt-1.0.2/miva_mmt.egg-info/SOURCES.txt` & `miva-mmt-1.0.3/miva_mmt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/__init__.py` & `miva-mmt-1.0.3/mmt/__init__.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/commands/__init__.py` & `miva-mmt-1.0.3/mmt/commands/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This file and the source codes contained herein are the property of
 Miva, Inc.  Use of this file is restricted to the specific terms and
 conditions in the License Agreement associated with this file.  Distribution
 of this file or portions of this file for uses not covered by the License
 Agreement is not allowed without a written agreement signed by an officer of
 Miva, Inc.
 
-Copyright 1998-2022 Miva, Inc.  All rights reserved.
+Copyright 1998-2023 Miva, Inc.  All rights reserved.
 https://www.miva.com
 
 Prefix         : MMT-COMMAND-
 Next Error Code: 16
 """
 
 import os
@@ -24,17 +24,18 @@
 import hashlib
 
 import merchantapi.abstract
 import merchantapi.authenticator
 import merchantapi.client
 import merchantapi.model
 import merchantapi.logging
+import merchantapi.listquery
 
 from mmt.version import __version__ as version
-from mmt.exceptions import Error, APIRequestError
+from mmt.exceptions import Error, APIRequestError, APIResponseError
 from mmt.file import File, BinaryFile
 from mmt.managers.config import ConfigManager
 from mmt.managers.remote import Remote
 from mmt.managers.credential import CredentialToken, CredentialSSH
 from mmt.metadata.state import StateMetadataFile, StateMetadataEntryFile, StateMetadataBaseTemplateFile, StateMetadataBasePropertyFile, StateMetadataBaseJSResourceFile, StateMetadataBaseCSSResourceFile, StateMetadataBaseResourceGroupFile
 
 
@@ -120,14 +121,17 @@
 
 	@property
 	def state( self ) -> StateMetadataFile:
 		return self._state
 
 	# Helper Functions
 
+	def filter_expression( self ):
+		return MMTFilterExpression()
+
 	def load_remote( self, remote_key: str ) -> Remote:
 		if self._cached_remote is not None and self._cached_remote.key == remote_key:
 			return self._cached_remote
 
 		remote = self.configmanager.remote_lookup( remote_key )
 
 		if remote is None:
@@ -216,17 +220,19 @@
 				error_message = 'Invalid HTTP Basic Authentication credentials'
 			else:
 				error_message = 'Missing HTTP Basic Authentication credentials'
 
 			raise Error( 'MMT-COMMAND-00015', error_message )
 		except merchantapi.client.ClientException as e:
 			raise APIRequestError( request.get_function(), 'MMT-COMMAND-00002', str( e ) )
+		except KeyboardInterrupt:
+			quit()
 
 		if response.is_error():
-			raise APIRequestError( request.get_function(), response.get_error_code(), response.get_error_message() )
+			raise APIResponseError( response )
 
 		return response
 
 	def send_request_base64( self, request: merchantapi.abstract.Request ) -> merchantapi.abstract.Response:
 		request.set_binary_encoding( request.BINARY_ENCODING_BASE64 )
 
 		return self.send_request( request )
@@ -348,33 +354,51 @@
 			return branchpropertyversion.get_category().get( 'code' )
 
 		raise Error( 'MMT-COMMAND-00004', 'Failed to determine property code' )
 
 	def get_branchjavascriptresourceversion_code( self, branchjavascriptresourceversion: merchantapi.model.BranchJavaScriptResourceVersion ) -> str:
 		return branchjavascriptresourceversion.get_code()
 
+	def get_branchjavascriptresourceversion_type( self, branchjavascriptresourceversion: merchantapi.model.BranchJavaScriptResourceVersion ) -> str:
+		return branchjavascriptresourceversion.get_type()
+
 	def get_branchjavascriptresourceversion_settings_data( self, branchjavascriptresourceversion: merchantapi.model.BranchJavaScriptResourceVersion ) -> str:
 		return self.json_dumps( self.build_jsresource_settings( branchjavascriptresourceversion ) )
 
 	def get_branchjavascriptresourceversion_inline_data( self, branchjavascriptresourceversion: merchantapi.model.BranchJavaScriptResourceVersion ) -> bytes:
+		if self.get_branchjavascriptresourceversion_type( branchjavascriptresourceversion ) != 'I':
+			return b''
+
 		return self.base64_decode( branchjavascriptresourceversion.get_source() )
 
 	def get_branchjavascriptresourceversion_local_data( self, branchjavascriptresourceversion: merchantapi.model.BranchJavaScriptResourceVersion ) -> bytes:
+		if self.get_branchjavascriptresourceversion_type( branchjavascriptresourceversion ) != 'L':
+			return b''
+
 		return self.base64_decode( branchjavascriptresourceversion.get_source() )
 
 	def get_branchcssresourceversion_code( self, branchcssresourceversion: merchantapi.model.BranchCSSResourceVersion ):
 		return branchcssresourceversion.get_code()
 
+	def get_branchcssresourceversion_type( self, branchcssresourceversion: merchantapi.model.BranchCSSResourceVersion ) -> str:
+		return branchcssresourceversion.get_type()
+
 	def get_branchcssresourceversion_settings_data( self, branchcssresourceversion: merchantapi.model.BranchCSSResourceVersion ) -> str:
 		return self.json_dumps( self.build_cssresource_settings( branchcssresourceversion ) )
 
 	def get_branchcssresourceversion_inline_data( self, branchcssresourceversion: merchantapi.model.BranchCSSResourceVersion ) -> bytes:
+		if self.get_branchcssresourceversion_type( branchcssresourceversion ) != 'I':
+			return b''
+
 		return self.base64_decode( branchcssresourceversion.get_source() )
 
 	def get_branchcssresourceversion_local_data( self, branchcssresourceversion: merchantapi.model.BranchCSSResourceVersion ) -> bytes:
+		if self.get_branchcssresourceversion_type( branchcssresourceversion ) != 'L':
+			return b''
+
 		return self.base64_decode( branchcssresourceversion.get_source() )
 
 	def get_resourcegroup_code( self, resourcegroup: merchantapi.model.ResourceGroup ) -> str:
 		return resourcegroup.get_code()
 
 	def get_resourcegroup_settings_data( self, resourcegroup: merchantapi.model.ResourceGroup ) -> str:
 		return self.json_dumps( self.build_resourcegroup_settings( resourcegroup ) )
@@ -567,7 +591,41 @@
 			self._state.read()
 		except FileNotFoundError:
 			raise Error( 'MMT-COMMAND-00001', f'MMT has not been configured for path \'{self.root_directory}\'' )
 
 	@abc.abstractmethod
 	def run( self ):
 		raise NotImplementedError
+
+
+class MMTFilterExpression( merchantapi.listquery.FilterExpression ):
+	def to_list( self ) -> list:
+		def lowlevel():
+			filters = []
+
+			for e in self.expressions:
+				if isinstance( e[  'entry' ], MMTFilterExpression) and ( e[ 'type' ] in MMTFilterExpression.VALID_FILTERS ):
+					entry = {
+						'field':	e[ 'type' ],
+						'operator':	MMTFilterExpression.OPERATOR_SUBWHERE,
+						'value':	e[ 'entry' ].to_list()
+					}
+				else:
+					entry = {
+						'field':	e[ 'entry' ].get_left(),
+						'operator':	e[ 'entry' ].get_operator(),
+						'value':	e[ 'entry' ].get_right_joined()
+					}
+
+				filters.append(entry)
+
+			return filters
+
+		if self.is_child():
+			return lowlevel()
+
+		return [
+			{
+				'name': MMTFilterExpression.FILTER_SEARCH,
+				'value': lowlevel()
+			}
+		]
```

### Comparing `miva-mmt-1.0.2/mmt/commands/branch.py` & `miva-mmt-1.0.3/mmt/commands/branch.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/commands/checkout.py` & `miva-mmt-1.0.3/mmt/commands/checkout.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/commands/config.py` & `miva-mmt-1.0.3/mmt/commands/config.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/commands/credential.py` & `miva-mmt-1.0.3/mmt/commands/credential.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/commands/diff.py` & `miva-mmt-1.0.3/mmt/commands/diff.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This file and the source codes contained herein are the property of
 Miva, Inc.  Use of this file is restricted to the specific terms and
 conditions in the License Agreement associated with this file.  Distribution
 of this file or portions of this file for uses not covered by the License
 Agreement is not allowed without a written agreement signed by an officer of
 Miva, Inc.
 
-Copyright 1998-2022 Miva, Inc.  All rights reserved.
+Copyright 1998-2023 Miva, Inc.  All rights reserved.
 https://www.miva.com
 
 Prefix         : MMT-COMMAND-DIFF-
 Next Error Code: 11
 """
 
 import os
@@ -111,23 +111,23 @@
 		request.set_branch_id( self.configmanager.branch_id )
 		request.set_on_demand_columns( [ 'source', 'settings' ] )
 
 		return self.send_request_base64( request ).get_branch_template_versions()
 
 	def _listload_branchpropertyversions( self, property_groups_types_codes: typing.List[ typing.Tuple[ str, str, str ] ] ) -> typing.List[ merchantapi.model.BranchPropertyVersion ]:
 		request = merchantapi.request.BranchPropertyVersionListLoadQuery()
-		filters = request.filter_expression()
+		filters = self.filter_expression()
 
 		for property_group, property_type, property_code in property_groups_types_codes:
-			filter_expression = request.filter_expression().equal( 'type', property_type )
+			filter_expression = self.filter_expression().equal( 'type', property_type )
 
 			if property_group in [ 'product', 'category' ]:
-				filter_expression.and_is_null( 'code' )
+				filter_expression.is_null( 'code' )
 			else:
-				filter_expression.and_equal( 'code', property_code )
+				filter_expression.equal( 'code', property_code )
 
 			filters.or_x( filter_expression )
 
 		request.set_filters( filters )
 		request.set_changeset_id( self.state.changeset.id )
 		request.set_branch_id( self.configmanager.branch_id )
 		request.set_on_demand_columns( [ 'source', 'settings', 'category', 'product' ] )
@@ -214,15 +214,15 @@
 			mode = 'w'
 		elif isinstance( source, bytes ):
 			mode = 'wb'
 		else:
 			raise Error( 'MMT-COMMAND-DIFF-00008', 'Invalid diff source' )
 
 		try:
-			temp = tempfile.NamedTemporaryFile( mode = mode, prefix = f'mmt_diff_{os.path.basename( filepath )}_', suffix = '.tmp', delete = False )
+			temp = tempfile.NamedTemporaryFile( mode = mode, prefix = 'mmt_diff_', suffix = f'_{os.path.basename( filepath )}', delete = False )
 		except Exception as e:
 			raise Error( 'MMT-COMMAND-DIFF-00010', f'Failed to create temporary file: {str( e )}' )
 
 		try:
 			temp.write( source )
 			temp.close()
```

### Comparing `miva-mmt-1.0.2/mmt/commands/info.py` & `miva-mmt-1.0.3/mmt/commands/info.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/commands/log.py` & `miva-mmt-1.0.3/mmt/commands/log.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/commands/pull.py` & `miva-mmt-1.0.3/mmt/commands/pull.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This file and the source codes contained herein are the property of
 Miva, Inc.  Use of this file is restricted to the specific terms and
 conditions in the License Agreement associated with this file.  Distribution
 of this file or portions of this file for uses not covered by the License
 Agreement is not allowed without a written agreement signed by an officer of
 Miva, Inc.
 
-Copyright 1998-2021 Miva, Inc.  All rights reserved.
+Copyright 1998-2023 Miva, Inc.  All rights reserved.
 https://www.miva.com
 
 Prefix         : MMT-COMMAND-PULL-
 Next Error Code: 6
 """
 
 import typing
@@ -204,21 +204,23 @@
 				for branchpropertyversion in branchpropertyversions:
 					if self.property_equals_branchpropertyversion( state_file, branchpropertyversion ):
 						found = True
 						break
 			elif state_file.is_jsresource():
 				for branchjavascriptresourceversion in branchjavascriptresourceversions:
 					if self.jsresource_equals_branchjavascriptresourceversion( state_file, branchjavascriptresourceversion ):
-						found = True
-						break
+						if state_file.is_jsresource_settings_file() or self.get_branchjavascriptresourceversion_type( branchjavascriptresourceversion ) in [ 'L', 'I' ]:
+							found = True
+							break
 			elif state_file.is_cssresource():
 				for branchcssresourceversion in branchcssresourceversions:
 					if self.cssresource_equals_branchcssresourceversion( state_file, branchcssresourceversion ):
-						found = True
-						break
+						if state_file.is_cssresource_settings_file() or self.get_branchcssresourceversion_type( branchcssresourceversion ) in [ 'L', 'I' ]:
+							found = True
+							break
 			elif state_file.is_resourcegroup():
 				for resourcegroup in resourcegroups:
 					if self.resourcegroup_equals_resourcegroup( state_file, resourcegroup ):
 						found = True
 						break
 			else:
 				raise Error( 'MMT-COMMAND-PULL-00005', 'Unknown state file' )
@@ -302,27 +304,27 @@
 		request.set_branch_id( self.configmanager.branch_id )
 		request.set_on_demand_columns( [ 'source', 'settings' ] )
 
 		return self.send_request_base64( request ).get_branch_template_versions()
 
 	def _listload_branchpropertyversions( self, changeset: merchantapi.model.Changeset, property_state_files: typing.Optional[ typing.List[ StateMetadataBasePropertyFile ] ] = None ) -> typing.List[ merchantapi.model.BranchPropertyVersion ]:
 		request = merchantapi.request.BranchPropertyVersionListLoadQuery()
-		filters = request.filter_expression()
+		filters = self.filter_expression()
 
 		if property_state_files is None:
 			if self.configmanager.ignore_unsynced_properties:
-				filters.and_is_true( 'sync' )
+				filters.is_true( 'sync' )
 		else:
 			for state_file in property_state_files:
-				filter_expression = request.filter_expression().equal( 'type', state_file.property_type )
+				filter_expression = self.filter_expression().equal( 'type', state_file.property_type )
 
 				if state_file.property_group in [ 'product', 'category' ]:
-					filter_expression.and_is_null( 'code' )
+					filter_expression.is_null( 'code' )
 				else:
-					filter_expression.and_equal( 'code', state_file.property_code )
+					filter_expression.equal( 'code', state_file.property_code )
 
 				filters.or_x( filter_expression )
 
 		request.set_filters( filters )
 		request.set_changeset_id( changeset.get_id() )
 		request.set_branch_id( self.configmanager.branch_id )
 		request.set_on_demand_columns( [ 'source', 'settings', 'category', 'product' ] )
```

### Comparing `miva-mmt-1.0.2/mmt/commands/push.py` & `miva-mmt-1.0.3/mmt/commands/push.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/commands/remote.py` & `miva-mmt-1.0.3/mmt/commands/remote.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/commands/revert.py` & `miva-mmt-1.0.3/mmt/commands/revert.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 This file and the source codes contained herein are the property of
 Miva, Inc.  Use of this file is restricted to the specific terms and
 conditions in the License Agreement associated with this file.  Distribution
 of this file or portions of this file for uses not covered by the License
 Agreement is not allowed without a written agreement signed by an officer of
 Miva, Inc.
 
-Copyright 1998-2021 Miva, Inc.  All rights reserved.
+Copyright 1998-2023 Miva, Inc.  All rights reserved.
 https://www.miva.com
 
 Prefix         : MMT-COMMAND-REVERT-
 Next Error Code: 7
 """
 
 import typing
@@ -116,23 +116,23 @@
 		request.set_branch_id( self.configmanager.branch_id )
 		request.set_on_demand_columns( [ 'source', 'settings' ] )
 
 		return self.send_request_base64( request ).get_branch_template_versions()
 
 	def _listload_branchpropertyversions( self, property_groups_types_codes: typing.List[ typing.Tuple[ str, str, str ] ] ) -> typing.List[ merchantapi.model.BranchPropertyVersion ]:
 		request = merchantapi.request.BranchPropertyVersionListLoadQuery()
-		filters = request.filter_expression()
+		filters = self.filter_expression()
 
 		for property_group, property_type, property_code in property_groups_types_codes:
-			filter_expression = request.filter_expression().equal( 'type', property_type )
+			filter_expression = self.filter_expression().equal( 'type', property_type )
 
 			if property_group in [ 'product', 'category' ]:
-				filter_expression.and_is_null( 'code' )
+				filter_expression.is_null( 'code' )
 			else:
-				filter_expression.and_equal( 'code', property_code )
+				filter_expression.equal( 'code', property_code )
 
 			filters.or_x( filter_expression )
 
 		request.set_filters( filters )
 		request.set_changeset_id( self.state.changeset.id )
 		request.set_branch_id( self.configmanager.branch_id )
 		request.set_on_demand_columns( [ 'source', 'settings', 'category', 'product' ] )
```

### Comparing `miva-mmt-1.0.2/mmt/commands/status.py` & `miva-mmt-1.0.3/mmt/commands/status.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/commands/switch.py` & `miva-mmt-1.0.3/mmt/commands/switch.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/commands/tag.py` & `miva-mmt-1.0.3/mmt/commands/tag.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/exceptions.py` & `miva-mmt-1.0.3/mmt/exceptions.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,21 +4,23 @@
 This file and the source codes contained herein are the property of
 Miva, Inc.  Use of this file is restricted to the specific terms and
 conditions in the License Agreement associated with this file.  Distribution
 of this file or portions of this file for uses not covered by the License
 Agreement is not allowed without a written agreement signed by an officer of
 Miva, Inc.
 
-Copyright 1998-2020 Miva, Inc.  All rights reserved.
+Copyright 1998-2023 Miva, Inc.  All rights reserved.
 https://www.miva.com
 
 Prefix         : MMT-EXCEPTIONS-
 Next Error Code: 1
 """
 
+import merchantapi.abstract
+
 
 class Error( Exception ):
 	def __init__( self, error_code: str, error_message: str ):
 		super().__init__( f'{error_code}: {error_message}' )
 
 		self._error_code	= error_code
 		self._error_message	= error_message
@@ -41,7 +43,18 @@
 
 		super().__init__( error_code, built_error_message )
 
 
 class APIRequestError( Error ):
 	def __init__( self, function: str, error_code: str, error_message: str ):
 		super().__init__( error_code, f'{function}: {error_message}' )
+
+
+class APIResponseError( Error ):
+	def __init__( self, response: merchantapi.abstract.Response ):
+		error_code		= response.get_error_code()
+		error_message = f'{response.get_request().get_function()}: {response.get_error_message()}'
+
+		if response.is_validation_error():
+			error_message = f'{error_message}: {response.get_error_field()}: {response.get_error_field_message()}'
+
+		super().__init__( error_code, error_message )
```

### Comparing `miva-mmt-1.0.2/mmt/file.py` & `miva-mmt-1.0.3/mmt/file.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/managers/config.py` & `miva-mmt-1.0.3/mmt/managers/config.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/managers/credential.py` & `miva-mmt-1.0.3/mmt/managers/credential.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/managers/remote.py` & `miva-mmt-1.0.3/mmt/managers/remote.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/managers/setting.py` & `miva-mmt-1.0.3/mmt/managers/setting.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/metadata/__init__.py` & `miva-mmt-1.0.3/mmt/metadata/__init__.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/metadata/config.py` & `miva-mmt-1.0.3/mmt/metadata/config.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/metadata/globalconfig.py` & `miva-mmt-1.0.3/mmt/metadata/globalconfig.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/metadata/localconfig.py` & `miva-mmt-1.0.3/mmt/metadata/localconfig.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/mmt/metadata/state.py` & `miva-mmt-1.0.3/mmt/metadata/state.py`

 * *Files identical despite different names*

### Comparing `miva-mmt-1.0.2/setup.py` & `miva-mmt-1.0.3/setup.py`

 * *Files identical despite different names*

