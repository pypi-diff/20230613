# Comparing `tmp/msmanager-0.1.3.tar.gz` & `tmp/msmanager-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "msmanager-0.1.3.tar", max compression
+gzip compressed data, was "msmanager-0.2.0.tar", max compression
```

## Comparing `msmanager-0.1.3.tar` & `msmanager-0.2.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1111 2023-05-14 16:04:08.180554 msmanager-0.1.3/LICENSE
--rw-r--r--   0        0        0      267 2023-05-15 20:57:42.797028 msmanager-0.1.3/msmanager/__init__.py
--rw-r--r--   0        0        0       67 2023-05-15 21:27:48.138274 msmanager-0.1.3/msmanager/__main__.py
--rw-r--r--   0        0        0     5968 2023-05-17 21:50:42.885439 msmanager-0.1.3/msmanager/cli.py
--rw-r--r--   0        0        0     2488 2023-05-15 19:04:10.101041 msmanager-0.1.3/msmanager/config.py
--rw-r--r--   0        0        0     2793 2023-05-15 20:31:27.149266 msmanager-0.1.3/msmanager/exceptions.py
--rw-r--r--   0        0        0     3441 2023-05-17 21:45:18.685171 msmanager-0.1.3/msmanager/functions.py
--rw-r--r--   0        0        0      384 2023-05-16 16:36:36.800666 msmanager-0.1.3/msmanager/models.py
--rw-r--r--   0        0        0     2997 2023-05-17 21:08:14.055219 msmanager-0.1.3/msmanager/msm.py
--rw-r--r--   0        0        0      143 2023-05-15 19:04:10.113824 msmanager-0.1.3/msmanager/types.py
--rw-r--r--   0        0        0      533 2023-05-17 21:01:49.385592 msmanager-0.1.3/msmanager/units.py
--rw-r--r--   0        0        0      547 2023-05-17 21:01:52.515921 msmanager-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      565 2023-05-16 18:14:53.984547 msmanager-0.1.3/README.md
--rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 msmanager-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1090 2023-06-12 18:50:30.767588 msmanager-0.2.0/LICENSE
+-rw-r--r--   0        0        0      543 2023-06-12 18:50:30.767588 msmanager-0.2.0/README.md
+-rw-r--r--   0        0        0      260 2023-06-12 18:50:30.767588 msmanager-0.2.0/msmanager/__init__.py
+-rw-r--r--   0        0        0       64 2023-06-12 18:50:30.767588 msmanager-0.2.0/msmanager/__main__.py
+-rw-r--r--   0        0        0     5797 2023-06-12 18:50:30.767588 msmanager-0.2.0/msmanager/cli.py
+-rw-r--r--   0        0        0     2419 2023-06-12 18:50:30.767588 msmanager-0.2.0/msmanager/config.py
+-rw-r--r--   0        0        0     2728 2023-06-12 18:50:30.767588 msmanager-0.2.0/msmanager/exceptions.py
+-rw-r--r--   0        0        0     3341 2023-06-12 18:50:30.767588 msmanager-0.2.0/msmanager/functions.py
+-rw-r--r--   0        0        0      371 2023-06-12 18:50:30.767588 msmanager-0.2.0/msmanager/models.py
+-rw-r--r--   0        0        0     2919 2023-06-12 22:06:33.408082 msmanager-0.2.0/msmanager/msm.py
+-rw-r--r--   0        0        0      138 2023-06-12 18:50:30.767588 msmanager-0.2.0/msmanager/types.py
+-rw-r--r--   0        0        0      514 2023-06-12 18:50:30.767588 msmanager-0.2.0/msmanager/units.py
+-rw-r--r--   0        0        0      524 2023-06-12 22:08:09.272672 msmanager-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1364 1970-01-01 00:00:00.000000 msmanager-0.2.0/PKG-INFO
```

### Comparing `msmanager-0.1.3/LICENSE` & `msmanager-0.2.0/LICENSE`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2023 RCR - Organization Of Programmers
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2023 RCR - Organization Of Programmers
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `msmanager-0.1.3/msmanager/config.py` & `msmanager-0.2.0/msmanager/config.py`

 * *Ordering differences only*

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,70 @@
-import os
-import json
-from pathlib import Path
-from typing import Optional, Dict, Any
-from .models import MainConfig, MindustryServerConfig
-from .exceptions import (
-    ServerExistsError, ServerNotExistsError
-)
-
-# ! Config Manager
-class MSManagerConfig:
-    @staticmethod
-    def load(filepath: str) -> MainConfig:
-        return MainConfig.parse_file(filepath)
-    
-    @staticmethod
-    def dump(filepath: str, data: MainConfig) -> None:
-        with open(filepath, "w") as file:
-            file.write(data.json())
-    
-    @staticmethod
-    def json_load(filepath: str) -> Dict[str, Any]:
-        with open(filepath) as file:
-            return json.load(file)
-    
-    @staticmethod
-    def json_dump(filepath: str, data: Dict[str, Any]) -> None:
-        with open(filepath, "w") as file:
-            json.dump(data, file)
-    
-    def refresh(self) -> None: self.dump(self.name, self.config)
-    
-    def __init__(self, config_path: str) -> None:
-        self.name = os.path.abspath(config_path)
-        self.name_path = Path(self.name)
-        
-        config_data = MainConfig().dict()
-        if self.name_path.exists():
-            try: config_data.update(self.json_load(self.name))
-            except: pass
-        try: self.config = MainConfig.parse_obj(config_data)
-        except: self.config = MainConfig()
-        self.refresh()
-
-    def get_server(self, screen_name: str) -> Optional[MindustryServerConfig]:
-        for server in self.config.servers:
-            if server.screen_name == screen_name:
-                return server
-    
-    def get_server_index(self, screen_name: str) -> Optional[int]:
-        for idx, server in enumerate(self.config.servers):
-            if server.screen_name == screen_name:
-                return idx
-    
-    def exists_server(self, screen_name: str) -> bool:
-        return self.get_server(screen_name) is not None
-    
-    def add_server(self, server: MindustryServerConfig) -> None:
-        if not self.exists_server(server.screen_name):
-            self.config.servers.append(server)
-            self.refresh()
-        else:
-            raise ServerExistsError(server.screen_name)
-    
-    def remove_server(self, screen_name: str) -> None:
-        if (server_index:=self.get_server_index(screen_name)) is not None:
-            self.config.servers.pop(server_index)
-            self.refresh()
-        else:
+import os
+import json
+from pathlib import Path
+from typing import Optional, Dict, Any
+from .models import MainConfig, MindustryServerConfig
+from .exceptions import (
+    ServerExistsError, ServerNotExistsError
+)
+
+# ! Config Manager
+class MSManagerConfig:
+    @staticmethod
+    def load(filepath: str) -> MainConfig:
+        return MainConfig.parse_file(filepath)
+    
+    @staticmethod
+    def dump(filepath: str, data: MainConfig) -> None:
+        with open(filepath, "w") as file:
+            file.write(data.json())
+    
+    @staticmethod
+    def json_load(filepath: str) -> Dict[str, Any]:
+        with open(filepath) as file:
+            return json.load(file)
+    
+    @staticmethod
+    def json_dump(filepath: str, data: Dict[str, Any]) -> None:
+        with open(filepath, "w") as file:
+            json.dump(data, file)
+    
+    def refresh(self) -> None: self.dump(self.name, self.config)
+    
+    def __init__(self, config_path: str) -> None:
+        self.name = os.path.abspath(config_path)
+        self.name_path = Path(self.name)
+        
+        config_data = MainConfig().dict()
+        if self.name_path.exists():
+            try: config_data.update(self.json_load(self.name))
+            except: pass
+        try: self.config = MainConfig.parse_obj(config_data)
+        except: self.config = MainConfig()
+        self.refresh()
+
+    def get_server(self, screen_name: str) -> Optional[MindustryServerConfig]:
+        for server in self.config.servers:
+            if server.screen_name == screen_name:
+                return server
+    
+    def get_server_index(self, screen_name: str) -> Optional[int]:
+        for idx, server in enumerate(self.config.servers):
+            if server.screen_name == screen_name:
+                return idx
+    
+    def exists_server(self, screen_name: str) -> bool:
+        return self.get_server(screen_name) is not None
+    
+    def add_server(self, server: MindustryServerConfig) -> None:
+        if not self.exists_server(server.screen_name):
+            self.config.servers.append(server)
+            self.refresh()
+        else:
+            raise ServerExistsError(server.screen_name)
+    
+    def remove_server(self, screen_name: str) -> None:
+        if (server_index:=self.get_server_index(screen_name)) is not None:
+            self.config.servers.pop(server_index)
+            self.refresh()
+        else:
             raise ServerNotExistsError(screen_name)
```

### Comparing `msmanager-0.1.3/msmanager/exceptions.py` & `msmanager-0.2.0/msmanager/exceptions.py`

 * *Ordering differences only*

 * *Files 15% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-from .units import SUPPORT_PLATFORMS
-
-# ! System Exceptions
-class PlatformSupportError(Exception):
-    """Indicates that the `Screen (GNU)` is not working correctly or is missing."""
-    def __init__(self, currect_platform: str) -> None:
-        """Called if the program cannot work with the current platform."""
-        self.args = (
-            "Your platform ({0}) is not supported, only the following platforms are supported: {1}".format(
-                repr(currect_platform), ", ".join([repr(i) for i in SUPPORT_PLATFORMS])
-            ),
-        )
-
-class ScreenNotWorkingError(Exception):
-    """Indicates problems with the `GNU Screen`."""
-    def __init__(self) -> None:
-        """Called if there are problems when trying to work with `GNU Screen`."""
-        self.args = (
-            """The screen command returns an error when checked, check that the 'GNU Screen' program is working. \nIf the software is not available, the following program must be installed: https://www.gnu.org/software/screen""",
-        )
-
-class JavaNotFound(Exception):
-    """Indicates a lack of `Java`."""
-    def __init__(self) -> None:
-        """Called if the `Java` package environment could not be found."""
-        self.args = ("The `Java` environment package is not installed.",)
-
-# ! Parsing Error
-class VBMLParseError(Exception):
-    """Indicates a parsing error."""
-    def __init__(self) -> None:
-        """Calls if `vbml` was unable to finish parsing."""
-        self.args = ("There was an error parsing through vbml.",)
-
-
-# ! Config Exceptions
-class ServerExistsError(Exception):
-    """Indicates that there is a server with this name."""
-    def __init__(self, name: str) -> None:
-        """Called if a server with this name is already present in the config."""
-        self.args = (f"A server named {repr(name)} already exists in the config.",)
-
-class ServerNotExistsError(Exception):
-    """Indicates that north does not exist in the config."""
-    def __init__(self, name: str) -> None:
-        """Called if a server with this name does not exist in the config."""
-        self.args = (
-            f"A server named {repr(name)} does not exist in the config."
-        )
-
-# ! Server Actions Exceptions
-class ServerIsStartedError(Exception):
-    """Indicates that the server is already running."""
-    def __init__(self, name: str) -> None:
-        """Called when attempting to start an already running server."""
-        self.args = (
-            f"A server named {repr(name)} is already up and running."
-        )
-
-class ServerIsStoppedError(Exception):
-    """..."""
-    def __init__(self, name: str) -> None:
-        """..."""
-        self.args = (
-            f"The {repr(name)} server is stopped as it is."
+from .units import SUPPORT_PLATFORMS
+
+# ! System Exceptions
+class PlatformSupportError(Exception):
+    """Indicates that the `Screen (GNU)` is not working correctly or is missing."""
+    def __init__(self, currect_platform: str) -> None:
+        """Called if the program cannot work with the current platform."""
+        self.args = (
+            "Your platform ({0}) is not supported, only the following platforms are supported: {1}".format(
+                repr(currect_platform), ", ".join([repr(i) for i in SUPPORT_PLATFORMS])
+            ),
+        )
+
+class ScreenNotWorkingError(Exception):
+    """Indicates problems with the `GNU Screen`."""
+    def __init__(self) -> None:
+        """Called if there are problems when trying to work with `GNU Screen`."""
+        self.args = (
+            """The screen command returns an error when checked, check that the 'GNU Screen' program is working. \nIf the software is not available, the following program must be installed: https://www.gnu.org/software/screen""",
+        )
+
+class JavaNotFound(Exception):
+    """Indicates a lack of `Java`."""
+    def __init__(self) -> None:
+        """Called if the `Java` package environment could not be found."""
+        self.args = ("The `Java` environment package is not installed.",)
+
+# ! Parsing Error
+class VBMLParseError(Exception):
+    """Indicates a parsing error."""
+    def __init__(self) -> None:
+        """Calls if `vbml` was unable to finish parsing."""
+        self.args = ("There was an error parsing through vbml.",)
+
+
+# ! Config Exceptions
+class ServerExistsError(Exception):
+    """Indicates that there is a server with this name."""
+    def __init__(self, name: str) -> None:
+        """Called if a server with this name is already present in the config."""
+        self.args = (f"A server named {repr(name)} already exists in the config.",)
+
+class ServerNotExistsError(Exception):
+    """Indicates that north does not exist in the config."""
+    def __init__(self, name: str) -> None:
+        """Called if a server with this name does not exist in the config."""
+        self.args = (
+            f"A server named {repr(name)} does not exist in the config."
+        )
+
+# ! Server Actions Exceptions
+class ServerIsStartedError(Exception):
+    """Indicates that the server is already running."""
+    def __init__(self, name: str) -> None:
+        """Called when attempting to start an already running server."""
+        self.args = (
+            f"A server named {repr(name)} is already up and running."
+        )
+
+class ServerIsStoppedError(Exception):
+    """..."""
+    def __init__(self, name: str) -> None:
+        """..."""
+        self.args = (
+            f"The {repr(name)} server is stopped as it is."
         )
```

### Comparing `msmanager-0.1.3/pyproject.toml` & `msmanager-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,23 +1,23 @@
-[tool.poetry]
-name = "msmanager"
-version = "0.1.3"
-description = "Manager for managing Mindusrty servers."
-authors = ["Romanin <semina054@gmail.com>"]
-license = "MIT"
-readme = "README.md"
-packages = [{include = "msmanager"}]
-
-[tool.poetry.dependencies]
-python = "^3.9"
-pydantic = "^1.10.7"
-platformdirs = "^3.5.1"
-"versioner.py" = "^1.1.0"
-vbml = "^1.1.post1"
-click = "^8.1.3"
-screens-py = "^0.5.0"
-rich = "^13.3.5"
-pydustry-py = "^2.0.0"
-
-[build-system]
-requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
+[tool.poetry]
+name = "msmanager"
+version = "0.2.0"
+description = "Manager for managing Mindusrty servers."
+authors = ["Romanin <semina054@gmail.com>"]
+license = "MIT"
+readme = "README.md"
+packages = [{include = "msmanager"}]
+
+[tool.poetry.dependencies]
+python = "^3.9"
+pydantic = "^1.10.7"
+platformdirs = "^3.5.1"
+"versioner.py" = "^1.1.0"
+vbml = "^1.1.post1"
+click = "^8.1.3"
+screens-py = "^0.5.0"
+rich = "^13.3.5"
+pydustry-py = "^2.0.0"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `msmanager-0.1.3/README.md` & `msmanager-0.2.0/README.md`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,22 +1,22 @@
-# MSManager
-## Description
-Manager for managing Mindusrty servers.
-## Install
-```shell
-python3 -m pip install --upgrade msmanager
-```
-## Usage
-```
-Usage: python -m msmanager [OPTIONS] COMMAND [ARGS]...
-
-Options:
-  --not-check-environment  Disables checks for GNU Screen, Java and system support.
-  --help                   Show this message and exit.
-
-Commands:
-  add     Add a server to the config.
-  list    List of servers in the config.
-  remove  Remove the server from the config.
-  start   Run the server.
-  stop    Stop the server.
-```
+# MSManager
+## Description
+Manager for managing Mindusrty servers.
+## Install
+```shell
+python3 -m pip install --upgrade msmanager
+```
+## Usage
+```
+Usage: python -m msmanager [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --not-check-environment  Disables checks for GNU Screen, Java and system support.
+  --help                   Show this message and exit.
+
+Commands:
+  add     Add a server to the config.
+  list    List of servers in the config.
+  remove  Remove the server from the config.
+  start   Run the server.
+  stop    Stop the server.
+```
```

### Comparing `msmanager-0.1.3/PKG-INFO` & `msmanager-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: msmanager
-Version: 0.1.3
+Version: 0.2.0
 Summary: Manager for managing Mindusrty servers.
 License: MIT
 Author: Romanin
 Author-email: semina054@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

