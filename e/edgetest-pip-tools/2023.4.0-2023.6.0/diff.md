# Comparing `tmp/edgetest-pip-tools-2023.4.0.tar.gz` & `tmp/edgetest-pip-tools-2023.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edgetest-pip-tools-2023.4.0.tar", last modified: Sun Apr 23 17:54:42 2023, max compression
+gzip compressed data, was "edgetest-pip-tools-2023.6.0.tar", last modified: Tue Jun 13 17:29:05 2023, max compression
```

## Comparing `edgetest-pip-tools-2023.4.0.tar` & `edgetest-pip-tools-2023.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:54:42.641824 edgetest-pip-tools-2023.4.0/
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-23 17:54:42.641824 edgetest-pip-tools-2023.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:54:42.637824 edgetest-pip-tools-2023.4.0/edgetest_pip_tools/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2808 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:54:42.641824 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-04-23 17:54:42.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      468 2023-04-23 17:54:42.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:54:42.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-23 17:54:42.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 17:54:12.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-23 17:54:42.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-23 17:54:42.000000 edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-04-23 17:54:42.645824 edgetest-pip-tools-2023.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 17:54:42.641824 edgetest-pip-tools-2023.4.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3909 2023-04-23 17:54:09.000000 edgetest-pip-tools-2023.4.0/tests/test_hook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:29:05.160282 edgetest-pip-tools-2023.6.0/
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-13 17:28:31.000000 edgetest-pip-tools-2023.6.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-06-13 17:28:31.000000 edgetest-pip-tools-2023.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 17:28:31.000000 edgetest-pip-tools-2023.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-13 17:29:05.160282 edgetest-pip-tools-2023.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1862 2023-06-13 17:28:31.000000 edgetest-pip-tools-2023.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:29:05.160282 edgetest-pip-tools-2023.6.0/edgetest_pip_tools/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-13 17:28:31.000000 edgetest-pip-tools-2023.6.0/edgetest_pip_tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3138 2023-06-13 17:28:31.000000 edgetest-pip-tools-2023.6.0/edgetest_pip_tools/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:29:05.160282 edgetest-pip-tools-2023.6.0/edgetest_pip_tools.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3072 2023-06-13 17:29:05.000000 edgetest-pip-tools-2023.6.0/edgetest_pip_tools.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-06-13 17:29:05.000000 edgetest-pip-tools-2023.6.0/edgetest_pip_tools.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:29:05.000000 edgetest-pip-tools-2023.6.0/edgetest_pip_tools.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-13 17:29:05.000000 edgetest-pip-tools-2023.6.0/edgetest_pip_tools.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:28:35.000000 edgetest-pip-tools-2023.6.0/edgetest_pip_tools.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      414 2023-06-13 17:29:05.000000 edgetest-pip-tools-2023.6.0/edgetest_pip_tools.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-06-13 17:29:05.000000 edgetest-pip-tools-2023.6.0/edgetest_pip_tools.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-06-13 17:28:31.000000 edgetest-pip-tools-2023.6.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2795 2023-06-13 17:29:05.160282 edgetest-pip-tools-2023.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-13 17:28:31.000000 edgetest-pip-tools-2023.6.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:29:05.160282 edgetest-pip-tools-2023.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:28:31.000000 edgetest-pip-tools-2023.6.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7271 2023-06-13 17:28:31.000000 edgetest-pip-tools-2023.6.0/tests/test_hook.py
```

### Comparing `edgetest-pip-tools-2023.4.0/LICENSE` & `edgetest-pip-tools-2023.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `edgetest-pip-tools-2023.4.0/PKG-INFO` & `edgetest-pip-tools-2023.6.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgetest-pip-tools
-Version: 2023.4.0
+Version: 2023.6.0
 Summary: pip-tools integration for edgetest
 Home-page: https://github.com/capitalone/edgetest-pip-tools
 Author: Akshay Gupta
 Author-email: akshay.gupta2@capitalone.com
 Maintainer: Akshay Gupta
 Maintainer-email: akshay.gupta2@capitalone.com
 Project-URL: Documentation, https://capitalone.github.io/edgetest-pip-tools/
```

### Comparing `edgetest-pip-tools-2023.4.0/README.md` & `edgetest-pip-tools-2023.6.0/README.md`

 * *Files identical despite different names*

### Comparing `edgetest-pip-tools-2023.4.0/edgetest_pip_tools/plugin.py` & `edgetest-pip-tools-2023.6.0/edgetest_pip_tools/plugin.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Plugin for refreshing a locked requirements file."""
 
 from configparser import ConfigParser
 from pathlib import Path
-from typing import Dict, List
+from typing import Dict, List, Any
 
 import click
 import pluggy
 from edgetest.logger import get_logger
 from edgetest.schema import Schema
 from edgetest.utils import _run_command
+from tomlkit import load
 
 LOG = get_logger(__name__)
 
 hookimpl = pluggy.HookimplMarker("edgetest")
 
 
 @hookimpl
@@ -49,22 +50,29 @@
         The context for the CLI call.
 
     Returns
     -------
     Path
         Path to the requirements file.
     """
+    parser: Any
     if Path(ctx.params["config"]).name == "setup.cfg":
         # Check for the install_requires
         parser = ConfigParser()
         parser.read(Path(ctx.params["config"]))
         if "options" in parser and parser.get("options", "install_requires"):
             reqfile = Path(ctx.params["config"])
         else:
             reqfile = Path(ctx.params["requirements"])
+    elif Path(ctx.params["config"]).name == "pyproject.toml":
+        parser = load(open(Path(ctx.params["config"])))
+        if "dependencies" in parser["project"]:
+            reqfile = Path(ctx.params["config"])
+        else:
+            reqfile = Path(ctx.params["requirements"])
     else:
         reqfile = Path(ctx.params["requirements"])
 
     return reqfile
 
 
 @hookimpl(tryfirst=True)
```

### Comparing `edgetest-pip-tools-2023.4.0/edgetest_pip_tools.egg-info/PKG-INFO` & `edgetest-pip-tools-2023.6.0/edgetest_pip_tools.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edgetest-pip-tools
-Version: 2023.4.0
+Version: 2023.6.0
 Summary: pip-tools integration for edgetest
 Home-page: https://github.com/capitalone/edgetest-pip-tools
 Author: Akshay Gupta
 Author-email: akshay.gupta2@capitalone.com
 Maintainer: Akshay Gupta
 Maintainer-email: akshay.gupta2@capitalone.com
 Project-URL: Documentation, https://capitalone.github.io/edgetest-pip-tools/
```

### Comparing `edgetest-pip-tools-2023.4.0/requirements.txt` & `edgetest-pip-tools-2023.6.0/requirements.txt`

 * *Files 10% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     # via pip-tools
 cerberus==1.3.4
     # via edgetest
 click==8.1.3
     # via
     #   edgetest
     #   pip-tools
-edgetest==2023.4.0
+edgetest==2023.6.0
     # via edgetest-pip-tools (setup.cfg)
 packaging==23.0
     # via
     #   build
     #   edgetest
 pip-tools==6.13.0
     # via edgetest-pip-tools (setup.cfg)
```

### Comparing `edgetest-pip-tools-2023.4.0/setup.cfg` & `edgetest-pip-tools-2023.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 	bumpver
 
 [options.entry_points]
 edgetest = 
 	piptools = edgetest_pip_tools.plugin
 
 [bumpver]
-current_version = "2023.4.0"
+current_version = "2023.6.0"
 version_pattern = "YYYY.MM.INC0"
 commit_message = "Bump {old_version} to {new_version}"
 commit = True
 
 [bumpver:file_patterns]
 docs/source/conf.py = 
 	version = "{version}"
```

### Comparing `edgetest-pip-tools-2023.4.0/tests/test_hook.py` & `edgetest-pip-tools-2023.6.0/tests/test_hook.py`

 * *Files 24% similar despite different names*

```diff
@@ -4,26 +4,32 @@
 from pathlib import Path
 from unittest.mock import PropertyMock, call, patch
 
 import pytest
 from click.testing import CliRunner
 from edgetest.interface import cli
 from edgetest.schema import EdgetestValidator, Schema
-from edgetest.utils import parse_cfg
+from edgetest.utils import parse_cfg, parse_toml
 
 from edgetest_pip_tools.plugin import addoption
 
 CFG = """
 [edgetest.envs.myenv]
 upgrade =
     myupgrade
 command =
     pytest tests -m 'not integration'
 """
 
+TOML = """
+[edgetest.envs.myenv]
+upgrade = ["myupgrade"]
+command = "pytest tests -m 'not integration'"
+"""
+
 CFG_ART = """
 [options]
 install_requires =
     myupgrade
 
 [edgetest.envs.myenv]
 upgrade =
@@ -32,27 +38,56 @@
     pytest tests -m 'not integration'
 
 [edgetest.pip_tools]
 index_url = myindexurl
 """
 
 
+TOML_ART = """
+[project]
+name = "toy_edgetest_toml"
+version = "0.1.0"
+description = "Fake description"
+requires-python = ">=3.7"
+
+dependencies = ["myupgrade"]
+
+[edgetest.envs.myenv]
+upgrade = ["myupgrade"]
+command = "pytest tests -m 'not integration'"
+
+[edgetest.pip_tools]
+index_url = "myindexurl"
+extras = "complete,another"
+"""
+
+
 CFG_EXTRAS = """
 [edgetest.envs.myenv]
 upgrade =
     myupgrade
 command =
     pytest tests -m 'not integration'
 
 [edgetest.pip_tools]
 extras =
     complete
 """
 
 
+TOML_EXTRAS = """
+[edgetest.envs.myenv]
+upgrade = ["myupgrade"]
+command = "pytest tests -m 'not integration'"
+
+[edgetest.pip_tools]
+extras = "complete,another"
+"""
+
+
 PIP_LIST = """
 [{"name": "myupgrade", "version": "0.2.0"}]
 """
 
 
 TABLE_OUTPUT = """
 
@@ -61,15 +96,15 @@
 ============= =============== =================== =================
 myenv         True            myupgrade           0.2.0
 ============= =============== =================== =================
 """
 
 
 @pytest.mark.parametrize("config", [CFG, CFG_ART, CFG_EXTRAS])
-def test_addoption(config, tmpdir):
+def test_addoption_cfg(config, tmpdir):
     """Test the addoption hook."""
     location = tmpdir.mkdir("mylocation")
     conf_loc = Path(str(location), "myconfig.cfg")
     with open(conf_loc, "w") as outfile:
         outfile.write(config)
 
     schema = Schema()
@@ -78,18 +113,36 @@
     cfg = parse_cfg(filename=conf_loc)
 
     validator = EdgetestValidator(schema=schema.schema)
 
     assert validator.validate(cfg)
 
 
+@pytest.mark.parametrize("config", [TOML, TOML_ART, TOML_EXTRAS])
+def test_addoption_toml(config, tmpdir):
+    """Test the addoption hook."""
+    location = tmpdir.mkdir("mylocation")
+    conf_loc = Path(str(location), "pyproject.toml")
+    with open(conf_loc, "w") as outfile:
+        outfile.write(config)
+
+    schema = Schema()
+    addoption(schema=schema)
+
+    cfg = parse_toml(filename=conf_loc)
+
+    validator = EdgetestValidator(schema=schema.schema)
+
+    assert validator.validate(cfg)
+
+
 @patch("edgetest.lib.EnvBuilder", autospec=True)
 @patch("edgetest.core.Popen", autospec=True)
 @patch("edgetest.utils.Popen", autospec=True)
-def test_update_reqs(mock_popen, mock_cpopen, mock_builder):
+def test_update_reqs_cfg(mock_popen, mock_cpopen, mock_builder):
     """Test calling ``pip-tools``."""
     mock_popen.return_value.communicate.return_value = (PIP_LIST, "error")
     type(mock_popen.return_value).returncode = PropertyMock(return_value=0)
     mock_cpopen.return_value.communicate.return_value = ("output", "error")
     type(mock_cpopen.return_value).returncode = PropertyMock(return_value=0)
 
     runner = CliRunner()
@@ -98,17 +151,17 @@
         with open("setup.cfg", "w") as outfile:
             outfile.write(CFG_ART)
 
         result = runner.invoke(cli, ["--config=setup.cfg", "--export"])
 
     env_loc = Path(loc) / ".edgetest" / "myenv"
     if platform.system() == "Windows":
-        py_loc = str(Path(env_loc)  / "Scripts" / "python")
+        py_loc = str(Path(env_loc) / "Scripts" / "python")
     else:
-        py_loc = str(Path(env_loc)  / "bin" / "python")
+        py_loc = str(Path(env_loc) / "bin" / "python")
 
     assert result.exit_code == 0
     assert mock_popen.call_args_list == [
         call(
             (f"{str(py_loc)}", "-m", "pip", "install", "."),
             stdout=-1,
             universal_newlines=True,
@@ -146,7 +199,77 @@
                 "--output-file=requirements.txt",
                 "setup.cfg",
             ),
             stdout=-1,
             universal_newlines=True,
         ),
     ]
+
+
+@patch("edgetest.lib.EnvBuilder", autospec=True)
+@patch("edgetest.core.Popen", autospec=True)
+@patch("edgetest.utils.Popen", autospec=True)
+def test_update_reqs_toml(mock_popen, mock_cpopen, mock_builder):
+    """Test calling ``pip-tools``."""
+    mock_popen.return_value.communicate.return_value = (PIP_LIST, "error")
+    type(mock_popen.return_value).returncode = PropertyMock(return_value=0)
+    mock_cpopen.return_value.communicate.return_value = ("output", "error")
+    type(mock_cpopen.return_value).returncode = PropertyMock(return_value=0)
+
+    runner = CliRunner()
+
+    with runner.isolated_filesystem() as loc:
+        with open("pyproject.toml", "w") as outfile:
+            outfile.write(TOML_ART)
+        result = runner.invoke(cli, [f"--config=pyproject.toml", "--export"])
+
+    env_loc = Path(loc) / ".edgetest" / "myenv"
+    if platform.system() == "Windows":
+        py_loc = str(Path(env_loc) / "Scripts" / "python")
+    else:
+        py_loc = str(Path(env_loc) / "bin" / "python")
+
+    assert result.exit_code == 0
+    assert mock_popen.call_args_list == [
+        call(
+            (f"{str(py_loc)}", "-m", "pip", "install", "."),
+            stdout=-1,
+            universal_newlines=True,
+        ),
+        call(
+            (
+                f"{str(py_loc)}",
+                "-m",
+                "pip",
+                "install",
+                "myupgrade",
+                "--upgrade",
+            ),
+            stdout=-1,
+            universal_newlines=True,
+        ),
+        call(
+            (f"{str(py_loc)}", "-m", "pip", "list", "--format", "json"),
+            stdout=-1,
+            universal_newlines=True,
+        ),
+        call(
+            (f"{str(py_loc)}", "-m", "pip", "list", "--format", "json"),
+            stdout=-1,
+            universal_newlines=True,
+        ),
+        call(
+            (
+                f"{str(py_loc)}",
+                "-m",
+                "piptools",
+                "compile",
+                "-U",
+                "--extra=complete,another",
+                "--index-url=myindexurl",
+                "--output-file=requirements.txt",
+                "pyproject.toml",
+            ),
+            stdout=-1,
+            universal_newlines=True,
+        ),
+    ]
```

