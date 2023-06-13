# Comparing `tmp/pf_dev_tools-1.0.4.tar.gz` & `tmp/pf_dev_tools-1.0.5.tar.gz`

## Comparing `pf_dev_tools-1.0.4.tar` & `pf_dev_tools-1.0.5.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/.flake8
--rw-r--r--   0        0        0    27037 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/.nova/Artwork
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/.nova/Configuration.json
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/Exceptions.py
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/__about__.py
--rw-r--r--   0        0        0     1214 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/__init__.py
--rw-r--r--   0        0        0     5927 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfBuildCore.py
--rw-r--r--   0        0        0     4342 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfConfig.py
--rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfSconsEnvironment.py
--rw-r--r--   0        0        0     2666 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfUtils.py
--rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/__main__.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfClean.py
--rw-r--r--   0        0        0     2396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfClone.py
--rw-r--r--   0        0        0     2965 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfCommand.py
--rw-r--r--   0        0        0     2341 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfConvert.py
--rw-r--r--   0        0        0     3534 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfDelete.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfDryRun.py
--rw-r--r--   0        0        0     1323 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfEject.py
--rw-r--r--   0        0        0     3388 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfInstall.py
--rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfMake.py
--rw-r--r--   0        0        0     9978 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfPackage.py
--rw-r--r--   0        0        0     4058 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfQfs.py
--rw-r--r--   0        0        0     1817 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfReverse.py
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/LICENSE
--rw-r--r--   0        0        0    10264 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/README.md
--rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/pyproject.toml
--rw-r--r--   0        0        0    11324 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.4/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/.flake8
+-rw-r--r--   0        0        0    27037 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/.nova/Artwork
+-rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/.nova/Configuration.json
+-rw-r--r--   0        0        0     4344 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/CoreConfig.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/Exceptions.py
+-rw-r--r--   0        0        0     5172 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/Git.py
+-rw-r--r--   0        0        0     7580 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/OpenFPGACore.py
+-rw-r--r--   0        0        0      422 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/Paths.py
+-rw-r--r--   0        0        0      325 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/SCons.py
+-rw-r--r--   0        0        0     2883 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/Utils.py
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/__about__.py
+-rw-r--r--   0        0        0     1289 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/__init__.py
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Clean.py
+-rw-r--r--   0        0        0     2060 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Clone.py
+-rw-r--r--   0        0        0     2339 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Convert.py
+-rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Delete.py
+-rw-r--r--   0        0        0      734 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/DryRun.py
+-rw-r--r--   0        0        0     1341 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Eject.py
+-rw-r--r--   0        0        0     3421 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Install.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Make.py
+-rw-r--r--   0        0        0     9925 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Package.py
+-rw-r--r--   0        0        0     4056 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Qfs.py
+-rw-r--r--   0        0        0     1815 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/Reverse.py
+-rwxr-xr-x   0        0        0     1080 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/__main__.py
+-rw-r--r--   0        0        0     4151 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pfDevTools/pfCommand/pfCommand.py
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/LICENSE
+-rw-r--r--   0        0        0    10346 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/README.md
+-rw-r--r--   0        0        0     1396 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/pyproject.toml
+-rw-r--r--   0        0        0    11406 2020-02-02 00:00:00.000000 pf_dev_tools-1.0.5/PKG-INFO
```

### Comparing `pf_dev_tools-1.0.4/.nova/Artwork` & `pf_dev_tools-1.0.5/.nova/Artwork`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.4/pfDevTools/__init__.py` & `pf_dev_tools-1.0.5/pfDevTools/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import sys
 
-from .pfCommand.pfClone import pfClone
-from .pfCommand.pfConvert import pfConvert
-from .pfCommand.pfDelete import pfDelete
-from .pfCommand.pfEject import pfEject
-from .pfCommand.pfInstall import pfInstall
-from .pfCommand.pfMake import pfMake
-from .pfCommand.pfPackage import pfPackage
-from .pfCommand.pfQfs import pfQfs
-from .pfCommand.pfReverse import pfReverse
-
-from .pfConfig import pfConfig
-from .pfSconsEnvironment import Environment
-from .pfUtils import pfUtils
+from .pfCommand.Clean import Clean
+from .pfCommand.Clone import Clone
+from .pfCommand.Convert import Convert
+from .pfCommand.Delete import Delete
+from .pfCommand.DryRun import DryRun
+from .pfCommand.Eject import Eject
+from .pfCommand.Install import Install
+from .pfCommand.Make import Make
+from .pfCommand.Package import Package
+from .pfCommand.Qfs import Qfs
+from .pfCommand.Reverse import Reverse
+
+from .CoreConfig import CoreConfig
+from .Git import Git
+from .Paths import Paths
+from .SCons import SConsEnvironment
+from .Utils import Utils
 
 from semver import Version
 
 from .__about__ import __version__
 
 
 # --- Makes sure current pfDevTools versions is supported
 def requires(version: str) -> bool:
     current = Version.parse(__version__, optional_minor_and_patch=True)
     required = Version.parse(version, optional_minor_and_patch=True)
 
     if not (required.major == current.major) and ((current.minor > required.minor) or ((current.minor == required.minor) and (current.patch >= required.patch))) and (required.prerelease == current.prerelease):
-        raise RuntimeError(f'pfDevTools v{str(current)} is not compatible with the required version v{str(required)}')
+        raise RuntimeError(f'pfDevTools v{str(current)} is not compatible with the required version v{str(required)}.')
```

### Comparing `pf_dev_tools-1.0.4/pfDevTools/pfConfig.py` & `pf_dev_tools-1.0.5/pfDevTools/CoreConfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 try:
     import tomllib
 except ModuleNotFoundError:
     import tomli as tomllib
 
 
 # -- Classes
-class pfConfig:
+class CoreConfig:
     """A class for openFPGA core configurations"""
 
     def __init__(self, config_filename: str):
         """Constructor based on config file path."""
 
         self.config_filename: str = config_filename
         self._platform_short_name = None
```

### Comparing `pf_dev_tools-1.0.4/pfDevTools/pfUtils.py` & `pf_dev_tools-1.0.5/pfDevTools/Utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,20 +3,21 @@
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import subprocess
 import os
 import shutil
 import errno
 import stat
+import time
 
 from typing import List
 
 
 # -- Classes
-class pfUtils:
+class Utils:
     @classmethod
     def _handleRemoveReadonly(cls, func, path, exc):
         excvalue = exc[1]
         if func in (os.rmdir, os.remove, os.unlink) and excvalue.errno == errno.EACCES:
             os.chmod(path, stat.S_IRWXU | stat.S_IRWXG | stat.S_IRWXO)  # -- 0777
             func(path)
         else:
@@ -58,29 +59,36 @@
             raise
         except Exception as e:
             raise RuntimeError(str(e))
 
     @classmethod
     def commandExists(cls, command: str) -> bool:
         try:
-            pfUtils.shellCommand(f'{"where" if os.name == "nt" else "which"} {command}', silent_mode=True)
+            Utils.shellCommand(f'{"where" if os.name == "nt" else "which"} {command}', silent_mode=True)
         except Exception:
             return False
 
         return True
 
     @classmethod
     def requireCommand(cls, command: str):
-        if not pfUtils.commandExists(command):
+        if not Utils.commandExists(command):
             raise RuntimeError('❌ Cannot find command \'' + command + '\'.')
 
     @classmethod
     def deleteFolder(cls, folder: str, force_delete: bool = False):
         if os.path.exists(folder):
             if force_delete is True:
                 ignore_errors = False
-                on_error = pfUtils._handleRemoveReadonly
+                on_error = Utils._handleRemoveReadonly
             else:
                 ignore_errors = True
                 on_error = None
 
             shutil.rmtree(folder, ignore_errors=ignore_errors, onerror=on_error)
+
+    @classmethod
+    def fileOlderThan(cls, path: str, time_in_seconds: int):
+        if not os.path.exists(path):
+            return True
+
+        return (time.time() - os.path.getmtime(path)) > time_in_seconds
```

### Comparing `pf_dev_tools-1.0.4/pfDevTools/pfCommand/__main__.py` & `pf_dev_tools-1.0.5/pfDevTools/pfCommand/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfClean.py` & `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Clean.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-from pfDevTools.pfUtils import pfUtils
+import pfDevTools.Utils
 
 
 # -- Classes
-class pfClean:
+class Clean:
     """A tool to clean the local project."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         if len(arguments) != 0:
             raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
 
     def run(self) -> None:
-        pfUtils.shellCommand('scons -c -Q -s')
+        pfDevTools.Utils.shellCommand('scons -c -Q -s')
 
     @classmethod
     def name(cls) -> str:
         return 'clean'
 
     @classmethod
     def usage(cls) -> None:
```

### Comparing `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfClone.py` & `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Clone.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
+import pfDevTools.Utils
+import pfDevTools.Git
 
-from pfDevTools.pfUtils import pfUtils
 from pfDevTools.Exceptions import ArgumentError
 
 
 # -- Classes
-class pfClone:
+class Clone:
     """A tool to clone the Github core template."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         self._tag_name: str = None
-        self._url: str = 'https://github.com/DidierMalenfant/pfCoreTemplate.git'
+        self._url: str = 'github.com/DidierMalenfant/pfCoreTemplate'
 
         nb_of_arguments = len(arguments)
         if nb_of_arguments == 1 or nb_of_arguments == 3:
             self._url: str = arguments[0]
             nb_of_arguments -= 1
             arguments = arguments[1:]
 
@@ -33,35 +34,25 @@
                 raise ArgumentError('Invalid cloning arguments. Maybe start with `pf --help?')
 
             self._destination_folder: str = arguments[1]
         else:
             raise ArgumentError('Invalid arguments. Maybe start with `pf --help?')
 
     def run(self) -> None:
-        if pfUtils.commandExists('git') is False:
-            raise RuntimeError('You must have git installed on your machine to continue.')
-
         repo_folder = os.path.join(self._destination_folder, 'pfCoreTemplate')
         if os.path.exists(repo_folder):
-            pfUtils.deleteFolder(repo_folder, force_delete=True)
+            pfDevTools.Utils.deleteFolder(repo_folder, force_delete=True)
 
         print('Cloning core template in \'' + repo_folder + '\'.')
 
-        command_line = 'git clone --depth 1 '
-
-        if self._tag_name is not None:
-            command_line += f'--branch {self._tag_name} '
-
-        command_line += self._url
-
-        pfUtils.shellCommand(command_line, from_dir=self._destination_folder, silent_mode=True)
+        pfDevTools.Git(self._url).cloneIn(repo_folder, self._tag_name)
 
         git_folder = os.path.join(repo_folder, '.git')
         if os.path.exists(git_folder):
-            pfUtils.deleteFolder(git_folder, force_delete=True)
+            pfDevTools.Utils.deleteFolder(git_folder, force_delete=True)
 
     @classmethod
     def name(cls) -> str:
         return 'clone'
 
     @classmethod
     def usage(cls) -> None:
```

### Comparing `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfConvert.py` & `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Convert.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import os
 
 from PIL import Image
 
 
 # -- Classes
-class pfConvert:
+class Convert:
     """A tool to install a zipped up core file onto a given volume (SD card or Pocket in USB access mode)."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         # -- Gather the arguments
         nb_of_arguments: int = len(arguments)
```

### Comparing `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfDelete.py` & `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Delete.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,27 +7,27 @@
 import contextlib
 import pfDevTools
 
 from pathlib import Path
 
 
 # -- Classes
-class pfDelete:
+class Delete:
     """A tool to delete a core from a given volume (SD card or Pocket in USB access mode)."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         nb_of_arguments = len(arguments)
         if nb_of_arguments == 2:
             self._volume_path = arguments[1]
             arguments = arguments[:0]
             nb_of_arguments -= 1
         else:
-            self._volume_path = pfDevTools.pfConfig.coreInstallVolumePath()
+            self._volume_path = pfDevTools.CoreConfig.coreInstallVolumePath()
 
         if len(arguments) != 1:
             raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
 
         self._name_of_core_to_delete: str = arguments[0]
 
     def _destCoresFolder(self) -> str:
@@ -49,23 +49,23 @@
             shutil.rmtree(core_folder, ignore_errors=True)
 
         hidden_core_data = os.path.join(self._destCoresFolder(), '._' + self._name_of_core_to_delete)
         if os.path.exists(hidden_core_data):
             print('Deleting ' + hidden_core_data + '...')
             self._deleteFile(hidden_core_data)
 
-        core_name = pfDelete._coreNameFrom(self._name_of_core_to_delete)
+        core_name = Delete._coreNameFrom(self._name_of_core_to_delete)
         if core_name is None:
             raise RuntimeError('Could not figure out the core name from \'' + self._name_of_core_to_delete + ' \'.')
 
         for p in Path(cores_folder).rglob('*'):
             if not os.path.isdir(p):
                 continue
 
-            if pfDelete._coreNameFrom(os.path.basename(p)) == core_name:
+            if Delete._coreNameFrom(os.path.basename(p)) == core_name:
                 print('Found another implementation of the ' + core_name + ' platform, not deleting any Plaform data for this core.')
                 return
 
         platforms_folder = self._destPlatformsFolder()
         core_name = core_name.lower()
         for p in Path(platforms_folder).rglob('*'):
             if os.path.isdir(p):
```

### Comparing `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfDryRun.py` & `pf_dev_tools-1.0.5/pfDevTools/pfCommand/DryRun.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-from pfDevTools.pfUtils import pfUtils
+import pfDevTools.Utils
 
 
 # -- Classes
-class pfDryRun:
+class DryRun:
     """A tool to clean the local project."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         if len(arguments) != 0:
             raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
 
     def run(self) -> None:
-        pfUtils.shellCommand('scons --dry-run --tree=all --debug=explain')
+        pfDevTools.Utils.shellCommand('scons --dry-run --tree=all --debug=explain')
 
     @classmethod
     def name(cls) -> str:
         return 'dryrun'
 
     @classmethod
     def usage(cls) -> None:
```

### Comparing `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfEject.py` & `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Eject.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,41 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 import pfDevTools
+import pfDevTools.Utils
+import pfDevTools.CoreConfig
 
 from sys import platform
 
-from pfDevTools.pfUtils import pfUtils
-
 
 # -- Classes
-class pfEject:
+class Eject:
     """A tool to eject given volume (SD card or Pocket in USB access mode)."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         nb_of_arguments = len(arguments)
         if nb_of_arguments == 0:
-            self._volume_path = pfDevTools.pfConfig.coreInstallVolumePath()
+            self._volume_path = pfDevTools.CoreConfig.coreInstallVolumePath()
         elif nb_of_arguments == 1:
             self._volume_path = arguments[0]
         else:
             raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
 
     def run(self) -> None:
         if not os.path.exists(self._volume_path):
             raise RuntimeError(f'Volume {self._volume_path} is not mounted.')
-    
+
         if platform == "darwin":
             print(f'Ejecting {self._volume_path}.')
-            pfUtils.shellCommand(f'diskutil eject {self._volume_path}')
+            pfDevTools.Utils.shellCommand(f'diskutil eject {self._volume_path}')
         else:
             print('Ejecting volumes is only supported on macOS right now.')
 
     @classmethod
     def name(cls) -> str:
         return 'eject'
```

### Comparing `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfInstall.py` & `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Install.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 import zipfile
 import tempfile
 import contextlib
-import pfDevTools
+import pfDevTools.Utils
+import pfDevTools.CoreConfig
 
 from sys import platform
 from distutils.dir_util import copy_tree
 
 
 # -- Classes
-class pfInstall:
+class Install:
     """A tool to install a zipped up core file onto a given volume (SD card or Pocket in USB access mode)."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         self._zip_filename = None
         self._volume_path = None
@@ -25,15 +26,15 @@
         nb_of_arguments = len(arguments)
         if nb_of_arguments != 0:
             if nb_of_arguments == 2:
                 self._volume_path = arguments[1]
                 arguments = arguments[:0]
                 nb_of_arguments -= 1
             else:
-                self._volume_path = pfDevTools.pfConfig.coreInstallVolumePath()
+                self._volume_path = pfDevTools.CoreConfig.coreInstallVolumePath()
 
             if nb_of_arguments != 1:
                 raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
 
             self._zip_filename = arguments[0]
 
             components = os.path.splitext(self._zip_filename)
@@ -54,15 +55,15 @@
 
     def _deleteFile(self, filepath) -> None:
         with contextlib.suppress(FileNotFoundError):
             os.remove(filepath)
 
     def run(self) -> None:
         if self._volume_path is None:
-            pfDevTools.pfUtils.shellCommand('scons -Q -s install')
+            pfDevTools.Utils.shellCommand('scons -Q -s install')
             return
 
         # -- In a temporary folder.
         with tempfile.TemporaryDirectory() as tmp_dir:
             # -- Unzip the file.
             with zipfile.ZipFile(self._zip_filename, 'r') as zip_ref:
                 zip_ref.extractall(tmp_dir)
```

### Comparing `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfMake.py` & `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Make.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
-from pfDevTools.pfUtils import pfUtils
+import pfDevTools.Utils
 
 
 # -- Classes
-class pfMake:
+class Make:
     """A tool to make the local project."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         if len(arguments) != 0:
             raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
 
     def run(self) -> None:
-        pfUtils.shellCommand('scons -Q -s')
+        pfDevTools.Utils.shellCommand('scons -Q -s')
 
     @classmethod
     def name(cls) -> str:
         return 'make'
 
     @classmethod
     def usage(cls) -> None:
```

### Comparing `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfPackage.py` & `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Package.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,36 +1,32 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 import shutil
 import zipfile
+import pfDevTools
 
 from typing import List
 from pathlib import Path
 from datetime import date
 
-from pfDevTools.pfConfig import pfConfig
-
-from .pfConvert import pfConvert
-from .pfReverse import pfReverse
-
 
 # -- Classes
-class pfPackage:
+class Package:
     """A tool to package an analog pocket core"""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         if len(arguments) != 3:
             raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
 
-        self._config = pfConfig(arguments[0])
+        self._config = pfDevTools.CoreConfig(arguments[0])
         self._bitstream_file: str = arguments[1]
         self._destination_folder: str = arguments[2]
         self._core_folder = os.path.join(self._destination_folder, '_core')
         self._today = str(date.today())
 
     def _generateDefinitionFiles(self, cores_folder, platforms_folder) -> None:
         output_filename = os.path.join(cores_folder, 'audio.json')
@@ -142,18 +138,18 @@
             out_file.write('      }\n')
             out_file.write('    ]\n')
             out_file.write('  }\n')
             out_file.write('}\n')
 
     def _convertImages(self, cores_folder, platforms_image_folder) -> None:
         dest_bin_file = os.path.join(platforms_image_folder, '%s.bin' % (self._config.platformShortName()))
-        pfConvert([self._config.platformImage(), dest_bin_file]).run()
+        pfDevTools.Convert([self._config.platformImage(), dest_bin_file]).run()
 
         dest_bin_file = os.path.join(cores_folder, 'icon.bin')
-        pfConvert([self._config.authorIcon(), dest_bin_file]).run()
+        pfDevTools.Convert([self._config.authorIcon(), dest_bin_file]).run()
 
     def _packageCore(self):
         packaged_filename = os.path.abspath(os.path.join(self._destination_folder, self.packagedFilename()))
         if os.path.exists(packaged_filename):
             os.remove(packaged_filename)
 
         with zipfile.ZipFile(packaged_filename, 'w') as myzip:
@@ -195,15 +191,15 @@
         os.makedirs(platforms_folder, exist_ok=True)
 
         platforms_image_folder = os.path.join(platforms_folder, '_images')
         os.makedirs(platforms_image_folder, exist_ok=True)
 
         print('Reversing bitstream file...')
         bitstream_dest = os.path.join(cores_folder, '%s.rbf_r' % self._config.platformShortName())
-        pfReverse([self._bitstream_file, bitstream_dest]).run()
+        pfDevTools.Reverse([self._bitstream_file, bitstream_dest]).run()
 
         print('Generating definitions files...')
         self._generateDefinitionFiles(cores_folder, platforms_folder)
 
         print('Converting images...')
         self._convertImages(cores_folder, platforms_image_folder)
```

### Comparing `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfQfs.py` & `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Qfs.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 # -- Classes
 class EditingState(Enum):
     BEFORE_EDIT = 1
     DURING_EDIT = 2
     AFTER_EDIT = 3
 
 
-class pfQfs:
+class Qfs:
     """A tool to edit Quartus project files."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         if len(arguments) < 3:
             raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
```

### Comparing `pf_dev_tools-1.0.4/pfDevTools/pfCommand/pfReverse.py` & `pf_dev_tools-1.0.5/pfDevTools/pfCommand/Reverse.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 
 
 # -- Classes
-class pfReverse:
+class Reverse:
     """A tool to reverse the bitstream of an rbf file for an Analog Pocket core."""
 
     def __init__(self, arguments):
         """Constructor based on command line arguments."""
 
         if len(arguments) != 2:
             raise RuntimeError('Invalid arguments. Maybe start with `pf --help?')
```

### Comparing `pf_dev_tools-1.0.4/LICENSE` & `pf_dev_tools-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.4/README.md` & `pf_dev_tools-1.0.5/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -40,17 +40,17 @@
 ```
 Cleans the local project and deletes any intermediate build files. This should be executed in the same folder as the project's `SConstruct` file.
 
 #### `clone` command
 ```console
   pf clone <url> <tag=name> dest_folder
 ```
-Clones the repo found at `url`, optionally at a given tag/branch named `name` into the folder `dest_folder`.
+Clones the repo found at `url`, optionally at a given tag/branch named `name` into the folder `dest_folder`. 'url' does not need to be pre-fixed with `https://` or post-fixed with `.git`.
 
-If `url` is missing then `https://github.com/DidierMalenfant/pfCoreTemplate.git` is used.
+If `url` is missing then `github.com/DidierMalenfant/pfCoreTemplate` is used.
 
 #### `convert` command
 ```console
   pf convert src_filename dest_filename
 ```
 Converts an image to the openFGPA binary format used for core images and author icons.
 
@@ -118,30 +118,30 @@
 
 **pfDevTools** provides an entire toolchain needed to compile **openFPGA** cores. The build systems is based on the [**SCons**](https://scons.org) software construction tool which is entirely written in **Python**.
 
 A typical makefile is named `SConstruct` and for openFPGA projects can look as simple as this:
 ```python
   import pfDevTools
 
-  # -- We need pf-dev-tools version 1.x.x but at least 1.0.3.
-  pfDevTools.requires('1.0.3')
+  # -- We need pf-dev-tools version 1.x.x but at least 1.0.5.
+  pfDevTools.requires('1.0.5')
 
-  env = pfDevTools.Environment()
+  env = pfDevTools.SConsEnvironment()
   env.OpenFPGACore('src/config.toml')
 ```
 
 This will build, using `pf make`, a packaged core file based on the `toml` config [file](#core-config-file-format) and the source code found in the `src` folder.
 
 All projects should contain at least one `core/core_top.v` file at the root of their source tree. The content of this file should be based around **Analogue**'s own `core.top.v` [file](https://github.com/open-fpga/core-template/blob/main/src/fpga/core/core_top.v) but you do not need to provide any other files or **IP** found in the [core template](https://github.com/open-fpga/core-template). Those will be automatically brought in for you during the build.
 
 Good examples of simple core projects can be found in the examples provided as part of the [openFPGA tutorials](https://github.com/DidierMalenfant/openFPGA-tutorials).
 
-The build environment can be customized by passing variables to the `pfDevTools.Environment()` method call like so:
+The build environment can be customized by passing variables to the `pfDevTools.SConsEnvironment()` method call like so:
 ```python
-  env = pfDevTools.Environment(PF_BUILD_FOLDER='MyBuildFolder', PF_SRC_FOLDER='MySrcFolder')
+  env = pfDevTools.SConsEnvironment(PF_BUILD_FOLDER='MyBuildFolder', PF_SRC_FOLDER='MySrcFolder')
 ```
 
 The following variables are currently supported:
 
 - `PF_DOCKER_IMAGE` - Name of the **Docker** image used to compile the core's bitstream. Defaults to `didiermalenfant/quartus:22.1-apple-silicon`.
 - `PF_SRC_FOLDER` - Root folder for all the **Verilog** source files for the project. Defaults to the folder where the `toml` config [file]](#core-config-file-format) is located.
 - `PF_BUILD_FOLDER` - Folder where intermediate build files are created. Defaults to `_build`.
```

### Comparing `pf_dev_tools-1.0.4/pyproject.toml` & `pf_dev_tools-1.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pf_dev_tools-1.0.4/PKG-INFO` & `pf_dev_tools-1.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pf-dev-tools
-Version: 1.0.4
+Version: 1.0.5
 Summary: A collection of tools for Project Freedom projects
 Project-URL: Homepage, https://didier.malenfant.net/ProjectFreedom/
 Project-URL: Documentation, https://github.com/DidierMalenfant/pfDevTools#readme
 Project-URL: Bug Tracker, https://github.com/DidierMalenfant/pfDevTools/issues
 Project-URL: Source Code, https://github.com/DidierMalenfant/pfDevTools
 Author-email: Didier Malenfant <coding@malenfant.net>
 License-Expression: GPL-3.0-or-later
@@ -64,17 +64,17 @@
 ```
 Cleans the local project and deletes any intermediate build files. This should be executed in the same folder as the project's `SConstruct` file.
 
 #### `clone` command
 ```console
   pf clone <url> <tag=name> dest_folder
 ```
-Clones the repo found at `url`, optionally at a given tag/branch named `name` into the folder `dest_folder`.
+Clones the repo found at `url`, optionally at a given tag/branch named `name` into the folder `dest_folder`. 'url' does not need to be pre-fixed with `https://` or post-fixed with `.git`.
 
-If `url` is missing then `https://github.com/DidierMalenfant/pfCoreTemplate.git` is used.
+If `url` is missing then `github.com/DidierMalenfant/pfCoreTemplate` is used.
 
 #### `convert` command
 ```console
   pf convert src_filename dest_filename
 ```
 Converts an image to the openFGPA binary format used for core images and author icons.
 
@@ -142,30 +142,30 @@
 
 **pfDevTools** provides an entire toolchain needed to compile **openFPGA** cores. The build systems is based on the [**SCons**](https://scons.org) software construction tool which is entirely written in **Python**.
 
 A typical makefile is named `SConstruct` and for openFPGA projects can look as simple as this:
 ```python
   import pfDevTools
 
-  # -- We need pf-dev-tools version 1.x.x but at least 1.0.3.
-  pfDevTools.requires('1.0.3')
+  # -- We need pf-dev-tools version 1.x.x but at least 1.0.5.
+  pfDevTools.requires('1.0.5')
 
-  env = pfDevTools.Environment()
+  env = pfDevTools.SConsEnvironment()
   env.OpenFPGACore('src/config.toml')
 ```
 
 This will build, using `pf make`, a packaged core file based on the `toml` config [file](#core-config-file-format) and the source code found in the `src` folder.
 
 All projects should contain at least one `core/core_top.v` file at the root of their source tree. The content of this file should be based around **Analogue**'s own `core.top.v` [file](https://github.com/open-fpga/core-template/blob/main/src/fpga/core/core_top.v) but you do not need to provide any other files or **IP** found in the [core template](https://github.com/open-fpga/core-template). Those will be automatically brought in for you during the build.
 
 Good examples of simple core projects can be found in the examples provided as part of the [openFPGA tutorials](https://github.com/DidierMalenfant/openFPGA-tutorials).
 
-The build environment can be customized by passing variables to the `pfDevTools.Environment()` method call like so:
+The build environment can be customized by passing variables to the `pfDevTools.SConsEnvironment()` method call like so:
 ```python
-  env = pfDevTools.Environment(PF_BUILD_FOLDER='MyBuildFolder', PF_SRC_FOLDER='MySrcFolder')
+  env = pfDevTools.SConsEnvironment(PF_BUILD_FOLDER='MyBuildFolder', PF_SRC_FOLDER='MySrcFolder')
 ```
 
 The following variables are currently supported:
 
 - `PF_DOCKER_IMAGE` - Name of the **Docker** image used to compile the core's bitstream. Defaults to `didiermalenfant/quartus:22.1-apple-silicon`.
 - `PF_SRC_FOLDER` - Root folder for all the **Verilog** source files for the project. Defaults to the folder where the `toml` config [file]](#core-config-file-format) is located.
 - `PF_BUILD_FOLDER` - Folder where intermediate build files are created. Defaults to `_build`.
```

