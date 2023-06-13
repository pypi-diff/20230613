# Comparing `tmp/galaxy-test-driver-22.1.1.tar.gz` & `tmp/galaxy-test-driver-23.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "galaxy-test-driver-22.1.1.tar", last modified: Mon Aug 22 19:46:02 2022, max compression
+gzip compressed data, was "/home/runner/work/galaxy/galaxy/packages/test_driver/dist/.tmp-7_e31_r8/galaxy-test-driver-23.0.2.tar", last modified: Tue Jun 13 17:14:48 2023, max compression
```

## Comparing `galaxy-test-driver-22.1.1.tar` & `galaxy-test-driver-23.0.2.tar`

### file list

```diff
@@ -1,36 +1,27 @@
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:02.045473 galaxy-test-driver-22.1.1/
--rw-r--r--   0 mvandenb   (501) staff       (20)      332 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/HISTORY.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)    11109 2021-09-10 08:52:38.000000 galaxy-test-driver-22.1.1/LICENSE
--rw-r--r--   0 mvandenb   (501) staff       (20)       28 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/MANIFEST.in
--rw-r--r--   0 mvandenb   (501) staff       (20)     2954 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/Makefile
--rw-r--r--   0 mvandenb   (501) staff       (20)     1600 2022-08-22 19:46:02.045616 galaxy-test-driver-22.1.1/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      311 2022-03-24 19:47:11.000000 galaxy-test-driver-22.1.1/README.rst
--rw-r--r--   0 mvandenb   (501) staff       (20)       89 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/dev-requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:02.040782 galaxy-test-driver-22.1.1/galaxy/
--rw-r--r--   0 mvandenb   (501) staff       (20)       65 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/galaxy/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      418 2022-08-22 19:45:30.000000 galaxy-test-driver-22.1.1/galaxy/project_galaxy_test_driver.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:02.041046 galaxy-test-driver-22.1.1/galaxy_test/
--rw-r--r--   0 mvandenb   (501) staff       (20)       65 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/galaxy_test/__init__.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:02.042639 galaxy-test-driver-22.1.1/galaxy_test/driver/
--rw-r--r--   0 mvandenb   (501) staff       (20)        0 2022-03-24 19:47:11.000000 galaxy-test-driver-22.1.1/galaxy_test/driver/__init__.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    47633 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/galaxy_test/driver/driver_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2256 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/galaxy_test/driver/integration_setup.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     6460 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/galaxy_test/driver/integration_util.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      471 2022-03-24 19:47:11.000000 galaxy-test-driver-22.1.1/galaxy_test/driver/test_logging.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      275 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/galaxy_test/driver/testcase.py
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:02.044434 galaxy-test-driver-22.1.1/galaxy_test_driver.egg-info/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1600 2022-08-22 19:46:01.000000 galaxy-test-driver-22.1.1/galaxy_test_driver.egg-info/PKG-INFO
--rw-r--r--   0 mvandenb   (501) staff       (20)      801 2022-08-22 19:46:01.000000 galaxy-test-driver-22.1.1/galaxy_test_driver.egg-info/SOURCES.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:46:01.000000 galaxy-test-driver-22.1.1/galaxy_test_driver.egg-info/dependency_links.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       27 2022-08-22 19:46:01.000000 galaxy-test-driver-22.1.1/galaxy_test_driver.egg-info/entry_points.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)        1 2022-08-22 19:46:01.000000 galaxy-test-driver-22.1.1/galaxy_test_driver.egg-info/not-zip-safe
--rw-r--r--   0 mvandenb   (501) staff       (20)      124 2022-08-22 19:46:01.000000 galaxy-test-driver-22.1.1/galaxy_test_driver.egg-info/requires.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)       12 2022-08-22 19:46:01.000000 galaxy-test-driver-22.1.1/galaxy_test_driver.egg-info/top_level.txt
--rw-r--r--   0 mvandenb   (501) staff       (20)      124 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/requirements.txt
-drwxr-xr-x   0 mvandenb   (501) staff       (20)        0 2022-08-22 19:46:02.045245 galaxy-test-driver-22.1.1/scripts/
--rw-r--r--   0 mvandenb   (501) staff       (20)     1442 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/scripts/commit_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)     2166 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/scripts/new_version.py
--rw-r--r--   0 mvandenb   (501) staff       (20)      804 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/scripts/print_version_for_release.py
--rw-r--r--   0 mvandenb   (501) staff       (20)    33060 2022-08-22 19:46:02.052140 galaxy-test-driver-22.1.1/setup.cfg
--rw-r--r--   0 mvandenb   (501) staff       (20)     2745 2022-08-22 19:45:28.000000 galaxy-test-driver-22.1.1/setup.py
--rw-r--r--   0 mvandenb   (501) staff       (20)        7 2022-03-24 19:47:11.000000 galaxy-test-driver-22.1.1/test-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    12875 2023-06-13 17:04:36.000000 galaxy-test-driver-23.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/dev-requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43296 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/driver_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/integration_setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6467 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/integration_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/testcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/driver/uses_shed.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/galaxy_test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      606 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-06-13 17:14:48.000000 galaxy-test-driver-23.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-13 17:04:37.000000 galaxy-test-driver-23.0.2/test-requirements.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `galaxy-test-driver-22.1.1/LICENSE` & `galaxy-test-driver-23.0.2/LICENSE`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,61 @@
-Copyright (c) 2005-2016 Galaxy Contributors (see CONTRIBUTORS.md)
+Copyright (c) 2005-2022 Galaxy Contributors (see CONTRIBUTORS.md)
+
+Work contributed from 2021-04-07 onwards is licensed under the MIT License.
+Work contributed before this date is licensed under the Academic Free License
+version 3.0.
+See https://github.com/galaxyproject/galaxy/ for the contribution history.
+See below for the full text of both licenses.
+
+
+Some icons found in Galaxy are from the Silk Icons set, available under
+the Creative Commons Attribution 2.5 License, from:
+
+http://www.famfamfam.com/lab/icons/silk/
+
+
+Other images and documentation are licensed under the Creative Commons
+Attribution 3.0 (CC BY 3.0) License. See:
+
+http://creativecommons.org/licenses/by/3.0/
+
+
+--------------------------------------------------------------------------------
+
+
+MIT License
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
+
+
+--------------------------------------------------------------------------------
+
+
+Academic Free License ("AFL") v. 3.0
+
+This Academic Free License (the "License") applies to any original work of
+authorship (the "Original Work") whose owner (the "Licensor") has placed the
+following licensing notice adjacent to the copyright notice for the Original
+Work:
 
 Licensed under the Academic Free License version 3.0
 
  1) Grant of Copyright License. Licensor grants You a worldwide, royalty-free, 
     non-exclusive, sublicensable license, for the duration of the copyright, to 
     do the following:
 
@@ -169,18 +222,7 @@
     replace the notice specified in the first paragraph above with the 
     notice "Licensed under <insert your license name here>" or with a notice 
     of your own that is not confusingly similar to the notice in this 
     License; and (iii) You may not claim that your original works are open 
     source software unless your Modified License has been approved by Open 
     Source Initiative (OSI) and You comply with its license review and 
     certification process.
-
-
-Some icons found in Galaxy are from the Silk Icons set, available under
-the Creative Commons Attribution 2.5 License, from:
-
-http://www.famfamfam.com/lab/icons/silk/
-
-
-Other images and documentation are licensed under the Creative Commons Attribution 3.0 (CC BY 3.0) License.   See 
-
-http://creativecommons.org/licenses/by/3.0/
```

### Comparing `galaxy-test-driver-22.1.1/PKG-INFO` & `galaxy-test-driver-23.0.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 Metadata-Version: 2.1
 Name: galaxy-test-driver
-Version: 22.1.1
-Summary: Galaxy Test Driver
+Version: 23.0.2
+Summary: Galaxy test driver
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
-Keywords: galaxy
-Platform: UNKNOWN
+Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Testing
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: https://badge.fury.io/py/galaxy-test-driver.svg
    :target: https://pypi.org/project/galaxy-test-driver/
 
 
 
 Overview
 --------
 
 The Galaxy_ test driver package.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
-
-
-
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.1.dev0
----------------------
+-------------------
+23.0.2 (2023-06-13)
+-------------------
 
+No recorded changes since last release
 
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
----------------------
+No recorded changes since last release
+
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
-
-
```

### Comparing `galaxy-test-driver-22.1.1/galaxy_test/driver/driver_util.py` & `galaxy-test-driver-23.0.2/galaxy_test/driver/driver_util.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,143 +1,116 @@
 """Scripts for drivers of Galaxy functional tests."""
 
 import http.client
+import json
 import logging
 import os
 import random
-import re
-import shlex
 import shutil
-import signal
 import socket
 import string
 import subprocess
 import sys
 import tempfile
 import threading
 import time
-from typing import Optional
+from pathlib import Path
+from typing import (
+    List,
+    Optional,
+)
 from urllib.parse import urlparse
 
-import nose.config
-import nose.core
-import nose.loader
-import nose.plugins.manager
-import yaml
-from paste import httpserver
-
 from galaxy.app import UniverseApplication as GalaxyUniverseApplication
-from galaxy.app_unittest_utils.celery_helper import rebind_container_to_task
 from galaxy.config import LOGGING_CONFIG_DEFAULT
 from galaxy.model import mapping
-from galaxy.model.database_utils import create_database, database_exists
+from galaxy.model.database_utils import (
+    create_database,
+    database_exists,
+)
 from galaxy.model.tool_shed_install import mapping as toolshed_mapping
-from galaxy.tool_util.verify.interactor import GalaxyInteractorApi, verify_tool
-from galaxy.util import asbool, download_to_file, galaxy_directory
+from galaxy.tool_util.verify.interactor import (
+    GalaxyInteractorApi,
+    verify_tool,
+)
+from galaxy.tools import ToolBox
+from galaxy.util import (
+    asbool,
+    download_to_file,
+    galaxy_directory,
+)
 from galaxy.util.properties import load_app_properties
 from galaxy.webapps.galaxy import buildapp
-from galaxy_test.base.api_util import get_admin_api_key, get_user_api_key
+from galaxy.webapps.galaxy.fast_app import initialize_fast_app as init_galaxy_fast_app
+from galaxy_test.base.api_util import (
+    get_admin_api_key,
+    get_user_api_key,
+)
 from galaxy_test.base.env import (
     DEFAULT_WEB_HOST,
     target_url_parts,
 )
-from galaxy_test.base.instrument import StructuredTestDataPlugin
-from galaxy_test.base.nose_util import run
 from tool_shed.webapp.app import UniverseApplication as ToolshedUniverseApplication
+from tool_shed.webapp.fast_app import initialize_fast_app as init_tool_shed_fast_app
 from .test_logging import logging_config_file
 
 galaxy_root = galaxy_directory()
 DEFAULT_CONFIG_PREFIX = "GALAXY"
 GALAXY_TEST_DIRECTORY = os.path.join(galaxy_root, "test")
 GALAXY_TEST_FILE_DIR = "test-data,https://github.com/galaxyproject/galaxy-test-data.git"
 TOOL_SHED_TEST_DATA = os.path.join(galaxy_root, "lib", "tool_shed", "test", "test_data")
 TEST_WEBHOOKS_DIR = os.path.join(galaxy_root, "test", "functional", "webhooks")
 FRAMEWORK_TOOLS_DIR = os.path.join(GALAXY_TEST_DIRECTORY, "functional", "tools")
 FRAMEWORK_UPLOAD_TOOL_CONF = os.path.join(FRAMEWORK_TOOLS_DIR, "upload_tool_conf.xml")
-FRAMEWORK_SAMPLE_TOOLS_CONF = os.path.join(FRAMEWORK_TOOLS_DIR, "samples_tool_conf.xml")
+FRAMEWORK_SAMPLE_TOOLS_CONF = os.path.join(FRAMEWORK_TOOLS_DIR, "sample_tool_conf.xml")
 FRAMEWORK_DATATYPES_CONF = os.path.join(FRAMEWORK_TOOLS_DIR, "sample_datatypes_conf.xml")
-MIGRATED_TOOL_PANEL_CONFIG = 'config/migrated_tools_conf.xml'
-INSTALLED_TOOL_PANEL_CONFIGS = [
-    os.environ.get('GALAXY_TEST_SHED_TOOL_CONF', 'config/shed_tool_conf.xml')
-]
-REALTIME_PROXY_TEMPLATE = string.Template(r"""
-uwsgi:
-  http-raw-body: true
-  interactivetools_map: $tempdir/interactivetools_map.sqlite
-  python-raw: scripts/interactivetools/key_type_token_mapping.py
-  # if interactive tool path, jump to interactive tool, else skip to
-  # endendend (default uwsgi params).
-  route-host: ^([A-Za-z0-9]+(?:-[A-Za-z0-9]+)*)-([A-Za-z0-9]+(?:-[A-Za-z0-9]+)*)\.([A-Za-z0-9]+(?:-[A-Za-z0-9]+)*)\.(interactivetool\.$test_host:$test_port)$ goto:interactivetool
-  route-run: goto:endendend
-
-  route-label: interactivetool
-  route-host: ^([A-Za-z0-9]+(?:-[A-Za-z0-9]+)*)-([A-Za-z0-9]+(?:-[A-Za-z0-9]+)*)\.([A-Za-z0-9]+(?:-[A-Za-z0-9]+)*)\.(interactivetool\.$test_host:$test_port)$ rpcvar:TARGET_HOST rtt_key_type_token_mapper_cached $1 $3 $2 $4 $0 5
-  route-if-not: empty:${TARGET_HOST} httpdumb:${TARGET_HOST}
-  route: .* break:404 Not Found
-
-  route-label: endendend
-""")
-
+MIGRATED_TOOL_PANEL_CONFIG = "config/migrated_tools_conf.xml"
+INSTALLED_TOOL_PANEL_CONFIGS = [os.environ.get("GALAXY_TEST_SHED_TOOL_CONF", "config/shed_tool_conf.xml")]
 DEFAULT_LOCALES = "en"
-USE_UVICORN = asbool(os.environ.get('GALAXY_TEST_USE_UVICORN', True))
 
 log = logging.getLogger("test_driver")
 
 
 # Global variables to pass database contexts around - only needed for older
 # Tool Shed twill tests that didn't utilize the API for such interactions.
-galaxy_context = None
 tool_shed_context = None
 install_context = None
 
 
 def setup_tool_shed_tmp_dir():
-    tool_shed_test_tmp_dir = os.environ.get('TOOL_SHED_TEST_TMP_DIR', None)
+    tool_shed_test_tmp_dir = os.environ.get("TOOL_SHED_TEST_TMP_DIR", None)
     if tool_shed_test_tmp_dir is None:
         tool_shed_test_tmp_dir = os.path.realpath(tempfile.mkdtemp())
     # Here's the directory where everything happens.  Temporary directories are created within this directory to contain
     # the hgweb.config file, the database, new repositories, etc.  Since the tool shed browses repository contents via HTTP,
     # the full path to the temporary directroy wher eht repositories are located cannot contain invalid url characters.
-    os.environ['TOOL_SHED_TEST_TMP_DIR'] = tool_shed_test_tmp_dir
+    os.environ["TOOL_SHED_TEST_TMP_DIR"] = tool_shed_test_tmp_dir
     return tool_shed_test_tmp_dir
 
 
 def get_galaxy_test_tmp_dir():
     """Create test directory for use by Galaxy server being setup for testing."""
-    galaxy_test_tmp_dir = os.environ.get('GALAXY_TEST_TMP_DIR', None)
+    galaxy_test_tmp_dir = os.environ.get("GALAXY_TEST_TMP_DIR", None)
     if galaxy_test_tmp_dir is None:
         galaxy_test_tmp_dir = tempfile.mkdtemp()
     return galaxy_test_tmp_dir
 
 
-def configure_environment():
-    """Hack up environment for test cases."""
-    # no op remove if unused
-    if 'HTTP_ACCEPT_LANGUAGE' not in os.environ:
-        os.environ['HTTP_ACCEPT_LANGUAGE'] = DEFAULT_LOCALES
-
-    # Used by get_filename in tool shed's twilltestcase.
-    if "TOOL_SHED_TEST_FILE_DIR" not in os.environ:
-        os.environ["TOOL_SHED_TEST_FILE_DIR"] = TOOL_SHED_TEST_DATA
-
-    os.environ["GALAXY_TEST_ENVIRONMENT_CONFIGURED"] = "1"
-
-
 def build_logger():
     """Build a logger for test driver script."""
     return log
 
 
 def ensure_test_file_dir_set():
     """Ensure GALAXY_TEST_FILE_DIR setup in environment for test data resolver.
 
     Return first directory for backward compat.
     """
-    galaxy_test_file_dir = os.environ.get('GALAXY_TEST_FILE_DIR', GALAXY_TEST_FILE_DIR)
-    os.environ['GALAXY_TEST_FILE_DIR'] = galaxy_test_file_dir
+    galaxy_test_file_dir = os.environ.get("GALAXY_TEST_FILE_DIR", GALAXY_TEST_FILE_DIR)
+    os.environ["GALAXY_TEST_FILE_DIR"] = galaxy_test_file_dir
     first_test_file_dir = galaxy_test_file_dir.split(",")[0]
     return first_test_file_dir
 
 
 def setup_galaxy_config(
     tmpdir,
     use_test_file_dir=False,
@@ -159,91 +132,94 @@
     allow_path_paste=False,
 ):
     """Setup environment and build config for test Galaxy instance."""
     # For certain docker operations this needs to be evaluated out - e.g. for cwltool.
     tmpdir = os.path.realpath(tmpdir)
     if not os.path.exists(tmpdir):
         os.makedirs(tmpdir)
-    template_cache_path = tempfile.mkdtemp(prefix='compiled_templates_', dir=tmpdir)
-    new_file_path = tempfile.mkdtemp(prefix='new_files_path_', dir=tmpdir)
-    job_working_directory = tempfile.mkdtemp(prefix='job_working_directory_', dir=tmpdir)
+    template_cache_path = tempfile.mkdtemp(prefix="compiled_templates_", dir=tmpdir)
+    new_file_path = tempfile.mkdtemp(prefix="new_files_path_", dir=tmpdir)
+    job_working_directory = tempfile.mkdtemp(prefix="job_working_directory_", dir=tmpdir)
 
     user_library_import_dir: Optional[str]
     if use_test_file_dir:
         first_test_file_dir = ensure_test_file_dir_set()
         if not os.path.isabs(first_test_file_dir):
             first_test_file_dir = os.path.join(galaxy_root, first_test_file_dir)
         library_import_dir = first_test_file_dir
-        import_dir = os.path.join(first_test_file_dir, 'users')
+        import_dir = os.path.join(first_test_file_dir, "users")
         if os.path.exists(import_dir):
             user_library_import_dir = import_dir
         else:
             user_library_import_dir = None
     else:
         user_library_import_dir = None
         library_import_dir = None
-    job_config_file = os.environ.get('GALAXY_TEST_JOB_CONFIG_FILE', default_job_config_file)
-    tool_path = os.environ.get('GALAXY_TEST_TOOL_PATH', 'tools')
+    job_config_file = os.environ.get("GALAXY_TEST_JOB_CONFIG_FILE", default_job_config_file)
+    tool_path = os.environ.get("GALAXY_TEST_TOOL_PATH", "tools")
     tool_data_table_config_path = _tool_data_table_config_path(default_tool_data_table_config_path)
     default_data_manager_config = None
-    for data_manager_config in ['config/data_manager_conf.xml', 'data_manager_conf.xml']:
+    for data_manager_config in ["config/data_manager_conf.xml", "data_manager_conf.xml"]:
         if os.path.exists(data_manager_config):
             default_data_manager_config = data_manager_config
-    data_manager_config_file = 'test/functional/tools/sample_data_manager_conf.xml'
+    data_manager_config_file = "test/functional/tools/sample_data_manager_conf.xml"
     if default_data_manager_config is not None:
         data_manager_config_file = f"{default_data_manager_config},{data_manager_config_file}"
     master_api_key = get_admin_api_key()
-    cleanup_job = 'never' if ("GALAXY_TEST_NO_CLEANUP" in os.environ
-                              or "TOOL_SHED_TEST_NO_CLEANUP" in os.environ) else 'onsuccess'
+    cleanup_job = (
+        "never"
+        if ("GALAXY_TEST_NO_CLEANUP" in os.environ or "TOOL_SHED_TEST_NO_CLEANUP" in os.environ)
+        else "onsuccess"
+    )
 
     # Data Manager testing temp path
     # For storing Data Manager outputs and .loc files so that real ones don't get clobbered
-    galaxy_data_manager_data_path = tempfile.mkdtemp(prefix='data_manager_tool-data', dir=tmpdir)
+    galaxy_data_manager_data_path = tempfile.mkdtemp(prefix="data_manager_tool-data", dir=tmpdir)
 
     if allow_tool_conf_override:
-        tool_conf = os.environ.get('GALAXY_TEST_TOOL_CONF', default_tool_conf)
+        tool_conf = os.environ.get("GALAXY_TEST_TOOL_CONF", default_tool_conf)
     else:
         tool_conf = default_tool_conf
-    conda_auto_install = os.environ.get('GALAXY_TEST_CONDA_AUTO_INSTALL', conda_auto_install)
-    conda_auto_init = os.environ.get('GALAXY_TEST_CONDA_AUTO_INIT', conda_auto_init)
-    conda_prefix = os.environ.get('GALAXY_TEST_CONDA_PREFIX')
+    conda_auto_install = os.environ.get("GALAXY_TEST_CONDA_AUTO_INSTALL", conda_auto_install)
+    conda_auto_init = os.environ.get("GALAXY_TEST_CONDA_AUTO_INIT", conda_auto_init)
+    conda_prefix = os.environ.get("GALAXY_TEST_CONDA_PREFIX")
     if tool_conf is None:
         # As a fallback always at least allow upload.
         tool_conf = FRAMEWORK_UPLOAD_TOOL_CONF
 
     if shed_tool_conf is not None:
         tool_conf = f"{tool_conf},{shed_tool_conf}"
 
     # Resolve these paths w.r.t. galaxy root; otherwise galaxy's config system will resolve them w.r.t.
     # their parent directories, as per schema.
     data_manager_config_file = _resolve_relative_config_paths(data_manager_config_file)
     tool_config_file = _resolve_relative_config_paths(tool_conf)
     tool_data_table_config_path = _resolve_relative_config_paths(tool_data_table_config_path)
 
     config = dict(
-        admin_users='test@bx.psu.edu',
+        admin_users="test@bx.psu.edu",
         allow_library_path_paste=True,
         allow_path_paste=allow_path_paste,
         allow_user_creation=True,
         allow_user_deletion=True,
-        api_allow_run_as='test@bx.psu.edu',
+        api_allow_run_as="test@bx.psu.edu",
         auto_configure_logging=logging_config_file is None,
         chunk_upload_size=100,
         conda_prefix=conda_prefix,
         conda_auto_init=conda_auto_init,
         conda_auto_install=conda_auto_install,
         cleanup_job=cleanup_job,
         retry_metadata_internally=False,
         data_dir=tmpdir,
         data_manager_config_file=data_manager_config_file,
         enable_beta_tool_formats=True,
         expose_dataset_path=True,
         ftp_upload_purge=False,
         galaxy_data_manager_data_path=galaxy_data_manager_data_path,
-        id_secret='changethisinproductiontoo',
+        id_secret="changethisinproductiontoo",
         job_config_file=job_config_file,
         job_working_directory=job_working_directory,
         library_import_dir=library_import_dir,
         log_destination="stdout",
         new_file_path=new_file_path,
         override_tempdir=False,
         master_api_key=master_api_key,
@@ -257,20 +233,25 @@
         use_tasked_jobs=True,
         use_heartbeat=False,
         user_library_import_dir=user_library_import_dir,
         webhooks_dir=TEST_WEBHOOKS_DIR,
         logging=LOGGING_CONFIG_DEFAULT,
         monitor_thread_join_timeout=5,
         object_store_store_by="uuid",
-        simplified_workflow_run_ui="off",
+        fetch_url_allowlist="127.0.0.1",
+        job_handler_monitor_sleep=0.2,
+        job_runner_monitor_sleep=0.2,
+        workflow_monitor_sleep=0.2,
     )
     if default_shed_tool_data_table_config:
         config["shed_tool_data_table_config"] = default_shed_tool_data_table_config
     if not use_shared_connection_for_amqp:
-        config["amqp_internal_connection"] = f"sqlalchemy+sqlite:///{os.path.join(tmpdir, 'control.sqlite')}?isolation_level=IMMEDIATE"
+        config[
+            "amqp_internal_connection"
+        ] = f"sqlalchemy+sqlite:///{os.path.join(tmpdir, 'control.sqlite')}?isolation_level=IMMEDIATE"
 
     config.update(database_conf(tmpdir, prefer_template_database=prefer_template_database))
     config.update(install_database_conf(tmpdir, default_merged=default_install_db_merged))
     if asbool(os.environ.get("GALAXY_TEST_USE_HIERARCHICAL_OBJECT_STORE")):
         object_store_config = os.path.join(tmpdir, "object_store_conf.yml")
         with open(object_store_config, "w") as f:
             contents = """
@@ -297,80 +278,52 @@
 """
             contents_template = string.Template(contents)
             expanded_contents = contents_template.safe_substitute(temp_directory=tmpdir)
             f.write(expanded_contents)
         config["object_store_config_file"] = object_store_config
 
     if datatypes_conf is not None:
-        config['datatypes_config_file'] = datatypes_conf
+        config["datatypes_config_file"] = datatypes_conf
     if enable_tool_shed_check:
         config["enable_tool_shed_check"] = enable_tool_shed_check
         config["hours_between_check"] = 0.001
-    tool_dependency_dir = os.environ.get('GALAXY_TOOL_DEPENDENCY_DIR')
+    tool_dependency_dir = os.environ.get("GALAXY_TOOL_DEPENDENCY_DIR")
     if tool_dependency_dir:
         config["tool_dependency_dir"] = tool_dependency_dir
     # Used by shed's twill dependency stuff
     # TODO: read from Galaxy's config API.
-    os.environ["GALAXY_TEST_TOOL_DEPENDENCY_DIR"] = tool_dependency_dir or os.path.join(tmpdir, 'dependencies')
+    os.environ["GALAXY_TEST_TOOL_DEPENDENCY_DIR"] = tool_dependency_dir or os.path.join(tmpdir, "dependencies")
     return config
 
 
 def _resolve_relative_config_paths(config_option):
     # If option is not None, split into paths, resolve each w.r.t. root, then rebuild as csv string.
     if config_option is not None:
         resolved = []
-        for path in config_option.split(','):
+        for path in config_option.split(","):
             resolved.append(os.path.join(galaxy_root, path.strip()))
-        return ','.join(resolved)
+        return ",".join(resolved)
 
 
 def _tool_data_table_config_path(default_tool_data_table_config_path=None):
-    tool_data_table_config_path = os.environ.get('GALAXY_TEST_TOOL_DATA_TABLE_CONF', default_tool_data_table_config_path)
+    tool_data_table_config_path = os.environ.get(
+        "GALAXY_TEST_TOOL_DATA_TABLE_CONF", default_tool_data_table_config_path
+    )
     if tool_data_table_config_path is None:
         # ... otherwise find whatever Galaxy would use as the default and
         # the sample data for functional tests to that.
-        default_tool_data_config = 'lib/galaxy/config/sample/tool_data_table_conf.xml.sample'
-        for tool_data_config in ['config/tool_data_table_conf.xml', 'tool_data_table_conf.xml']:
+        default_tool_data_config = "lib/galaxy/config/sample/tool_data_table_conf.xml.sample"
+        for tool_data_config in ["config/tool_data_table_conf.xml", "tool_data_table_conf.xml"]:
             if os.path.exists(tool_data_config):
                 default_tool_data_config = tool_data_config
-        test_tool_data_config = 'test/functional/tool-data/sample_tool_data_tables.xml'
-        tool_data_table_config_path = f'{default_tool_data_config},{test_tool_data_config}'
+        test_tool_data_config = "test/functional/tool-data/sample_tool_data_tables.xml"
+        tool_data_table_config_path = f"{default_tool_data_config},{test_tool_data_config}"
     return tool_data_table_config_path
 
 
-def nose_config_and_run(argv=None, env=None, ignore_files=None, plugins=None):
-    """Setup a nose context and run tests.
-
-    Tests are specified by argv (defaulting to sys.argv).
-    """
-    if env is None:
-        env = os.environ
-    if ignore_files is None:
-        ignore_files = []
-    if plugins is None:
-        plugins = nose.plugins.manager.DefaultPluginManager()
-    if argv is None:
-        argv = sys.argv
-
-    test_config = nose.config.Config(
-        env=os.environ,
-        ignoreFiles=ignore_files,
-        plugins=plugins,
-    )
-
-    # Add custom plugin to produce JSON data used by planemo.
-    test_config.plugins.addPlugin(StructuredTestDataPlugin())
-    test_config.configure(argv)
-
-    result = run(test_config)
-
-    success = result.wasSuccessful()
-    return success
-
-
 def copy_database_template(source, db_path):
     """Copy a 'clean' sqlite template database.
 
     From file or URL to specified path for sqlite database.
     """
     db_path_dir = os.path.dirname(db_path)
     if not os.path.exists(db_path_dir):
@@ -404,52 +357,52 @@
             template_name = database_template_parsed.path[1:]  # drop / from /galaxy
             actual_db = f"gxtest{''.join(random.choice(string.ascii_uppercase) for _ in range(10))}"
             actual_database_parsed = database_template_parsed._replace(path=f"/{actual_db}")
             database_connection = actual_database_parsed.geturl()
             if not database_exists(database_connection):
                 # We pass by migrations and instantiate the current table
                 create_database(database_connection)
-                mapping.init('/tmp', database_connection, create_tables=True, map_install_models=True)
+                mapping.init("/tmp", database_connection, create_tables=True, map_install_models=True)
                 toolshed_mapping.init(database_connection, create_tables=True)
                 check_migrate_databases = False
     else:
         default_db_filename = f"{prefix.lower()}.sqlite"
         template_var = f"{prefix}_TEST_DB_TEMPLATE"
         db_path = os.path.join(db_path, default_db_filename)
         if template_var in os.environ:
             # Middle ground between recreating a completely new
             # database and pointing at existing database with
             # GALAXY_TEST_DBURI. The former requires a lot of setup
             # time, the latter results in test failures in certain
             # cases (namely tool shed tests expecting clean database).
             copy_database_template(os.environ[template_var], db_path)
             database_auto_migrate = True
-        database_connection = f'sqlite:///{db_path}'
+        database_connection = f"sqlite:///{db_path}"
     config = {
         "check_migrate_databases": check_migrate_databases,
         "database_connection": database_connection,
-        "database_auto_migrate": database_auto_migrate
+        "database_auto_migrate": database_auto_migrate,
     }
     if not database_connection.startswith("sqlite://"):
         config["database_engine_option_max_overflow"] = "20"
         config["database_engine_option_pool_size"] = "10"
     if template_name:
         config["database_template"] = template_name
     return config
 
 
 def install_database_conf(db_path, default_merged=False):
     install_galaxy_database_connection: Optional[str]
-    if 'GALAXY_TEST_INSTALL_DBURI' in os.environ:
-        install_galaxy_database_connection = os.environ['GALAXY_TEST_INSTALL_DBURI']
-    elif asbool(os.environ.get('GALAXY_TEST_INSTALL_DB_MERGED', default_merged)):
+    if "GALAXY_TEST_INSTALL_DBURI" in os.environ:
+        install_galaxy_database_connection = os.environ["GALAXY_TEST_INSTALL_DBURI"]
+    elif asbool(os.environ.get("GALAXY_TEST_INSTALL_DB_MERGED", default_merged)):
         install_galaxy_database_connection = None
     else:
-        install_galaxy_db_path = os.path.join(db_path, 'install.sqlite')
-        install_galaxy_database_connection = f'sqlite:///{install_galaxy_db_path}'
+        install_galaxy_db_path = os.path.join(db_path, "install.sqlite")
+        install_galaxy_database_connection = f"sqlite:///{install_galaxy_db_path}"
     conf = {}
     if install_galaxy_database_connection is not None:
         conf["install_database_connection"] = install_galaxy_database_connection
     return conf
 
 
 def database_files_path(test_tmpdir, prefix="GALAXY"):
@@ -459,15 +412,15 @@
     GALAXY_TEST_DBPATH is set in the environment.
     """
     environ_var = f"{prefix}_TEST_DBPATH"
     if environ_var in os.environ:
         db_path = os.environ[environ_var]
     else:
         tempdir = tempfile.mkdtemp(dir=test_tmpdir)
-        db_path = os.path.join(tempdir, 'database')
+        db_path = os.path.join(tempdir, "database")
     return db_path
 
 
 def _get_static_settings():
     """Configuration required for Galaxy static middleware.
 
     Returns dictionary of the settings necessary for a galaxy App
@@ -479,105 +432,94 @@
     static_dir = os.path.join(galaxy_root, "static")
 
     # TODO: these should be copied from config/galaxy.ini
     return dict(
         static_enabled=True,
         static_cache_time=360,
         static_dir=static_dir,
-        static_images_dir=os.path.join(static_dir, 'images', ''),
-        static_favicon_dir=os.path.join(static_dir, 'favicon.ico'),
-        static_scripts_dir=os.path.join(static_dir, 'scripts', ''),
-        static_style_dir=os.path.join(static_dir, 'style'),
-        static_robots_txt=os.path.join(static_dir, 'robots.txt'),
+        static_images_dir=os.path.join(static_dir, "images", ""),
+        static_favicon_dir=os.path.join(static_dir, "favicon.ico"),
+        static_scripts_dir=os.path.join(static_dir, "scripts", ""),
+        static_style_dir=os.path.join(static_dir, "style"),
+        static_robots_txt=os.path.join(static_dir, "robots.txt"),
     )
 
 
 def get_webapp_global_conf():
     """Get the global_conf dictionary sent to ``app_factory``."""
     # (was originally sent 'dict()') - nothing here for now except static settings
     global_conf = dict()
     global_conf.update(_get_static_settings())
     return global_conf
 
 
 def wait_for_http_server(host, port, prefix=None, sleep_amount=0.1, sleep_tries=150):
     """Wait for an HTTP server to boot up."""
     # Test if the server is up
-    prefix = prefix or '/'
-    if not prefix.endswith('/'):
+    prefix = prefix or "/"
+    if not prefix.endswith("/"):
         prefix = f"{prefix}/"
     for _ in range(sleep_tries):
         # directly test the app, not the proxy
+        if port and isinstance(port, str):
+            port = int(port)
         conn = http.client.HTTPConnection(host, port)
         try:
             conn.request("GET", prefix)
             response = conn.getresponse()
             if response.status == 200:
                 break
         except OSError as e:
             if e.errno not in [61, 111]:
                 raise
         time.sleep(sleep_amount)
     else:
-        template = "Test HTTP server on host %s and port %s did not return '200 OK' after 10 tries"
-        message = template % (host, port)
+        message = f"Test HTTP server on host {host} and port {port} did not return '200 OK' after {sleep_tries} tries"
         raise Exception(message)
 
 
-def attempt_port(port):
+def attempt_port(port: int) -> Optional[int]:
     sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
     try:
-        sock.bind(('', port))
+        sock.bind(("", port))
         sock.close()
         return port
     except OSError:
         return None
 
 
-def attempt_ports(port):
+def attempt_ports(port=None, set_galaxy_web_port=True) -> str:
     if port is not None:
+        if not attempt_port(int(port)):
+            raise Exception(f"An existing process seems bound to specified test server port [{port}]")
         return port
-
-        raise Exception(f"An existing process seems bound to specified test server port [{port}]")
     else:
         random.seed()
         for _ in range(0, 9):
             port = attempt_port(random.randint(8000, 10000))
             if port:
                 port = str(port)
-                os.environ['GALAXY_WEB_PORT'] = port
+                if set_galaxy_web_port:
+                    os.environ["GALAXY_WEB_PORT"] = port
                 return port
 
         raise Exception(f"Unable to open a port between {8000} and {10000} to start Galaxy server")
 
 
-def serve_webapp(webapp, port=None, host=None):
-    """Serve the webapp on a recommend port or a free one.
-
-    Return the port the webapp is running on.
-    """
-    server = None
-    port = attempt_ports(port)
-    server = httpserver.serve(webapp, host=host, port=port, start_loop=False)
-    t = threading.Thread(target=server.serve_forever)
-    t.start()
-
-    return server, port
-
-
 def uvicorn_serve(app, port, host=None):
     """Serve the webapp on a recommend port or a free one.
 
     Return the port the webapp is running on.
     """
     import asyncio
-    from uvicorn.server import Server
+
     from uvicorn.config import Config
+    from uvicorn.server import Server
 
-    access_log = False if 'GALAXY_TEST_DISABLE_ACCESS_LOG' in os.environ else True
+    access_log = False if "GALAXY_TEST_DISABLE_ACCESS_LOG" in os.environ else True
     config = Config(app, host=host, port=int(port), access_log=access_log)
     server = Server(config=config)
 
     def run_in_loop(loop):
         try:
             asyncio.set_event_loop(loop)
             loop.run_until_complete(server.serve())
@@ -620,46 +562,38 @@
         # Eliminate the migrated_tool_panel_config from the app's tool_configs, append the list of installed_tool_panel_configs,
         # and reload the app's toolbox.
         relative_migrated_tool_panel_config = os.path.join(app.config.root, MIGRATED_TOOL_PANEL_CONFIG)
         if relative_migrated_tool_panel_config in tool_configs:
             tool_configs.remove(relative_migrated_tool_panel_config)
         for installed_tool_panel_config in INSTALLED_TOOL_PANEL_CONFIGS:
             tool_configs.append(installed_tool_panel_config)
-        from galaxy import tools  # delay import because this brings in so many modules for small tests # noqa: E402
-        app.toolbox = tools.ToolBox(tool_configs, app.config.tool_path, app)
+        app.toolbox = ToolBox(tool_configs, app.config.tool_path, app)
 
 
 def build_galaxy_app(simple_kwargs) -> GalaxyUniverseApplication:
     """Build a Galaxy app object from a simple keyword arguments.
 
     Construct paste style complex dictionary and use load_app_properties so
     Galaxy override variables are respected. Also setup "global" references
     to sqlalchemy database context for Galaxy and install databases.
     """
     log.info("Galaxy database connection: %s", simple_kwargs["database_connection"])
-    simple_kwargs['global_conf'] = get_webapp_global_conf()
-    simple_kwargs['global_conf']['__file__'] = "lib/galaxy/config/sample/galaxy.yml.sample"
-    simple_kwargs = load_app_properties(
-        kwds=simple_kwargs
-    )
+    simple_kwargs["global_conf"] = get_webapp_global_conf()
+    simple_kwargs["global_conf"]["__file__"] = "lib/galaxy/config/sample/galaxy.yml.sample"
+    simple_kwargs = load_app_properties(kwds=simple_kwargs)
     # Build the Universe Application
     app = GalaxyUniverseApplication(**simple_kwargs)
-    if not simple_kwargs.get("enable_celery_tasks"):
-        rebind_container_to_task(app)
-
     log.info("Embedded Galaxy application started")
 
-    global galaxy_context
     global install_context
-    galaxy_context = app.model.context
     install_context = app.install_model.context
 
     # Toolbox indexing happens via the work queue out of band recently, and,
     # beyond potentially running async after tests execute doesn't execute
-    # without building a uwsgi app (app.is_webapp = False for this test kit).
+    # without building a webapp (app.is_webapp = False for this test kit).
     # We need to ensure to build an index for the test galaxy app -- this is
     # pretty fast with the limited toolset
     app.reindex_tool_search()
 
     return app
 
 
@@ -667,16 +601,16 @@
     """Build a Galaxy app object from a simple keyword arguments.
 
     Construct paste style complex dictionary. Also setup "global" reference
     to sqlalchemy database context for tool shed database.
     """
     log.info("Tool shed database connection: %s", simple_kwargs["database_connection"])
     # TODO: Simplify global_conf to match Galaxy above...
-    simple_kwargs['__file__'] = 'tool_shed_wsgi.yml.sample'
-    simple_kwargs['global_conf'] = get_webapp_global_conf()
+    simple_kwargs["__file__"] = "tool_shed_wsgi.yml.sample"
+    simple_kwargs["global_conf"] = get_webapp_global_conf()
 
     app = ToolshedUniverseApplication(**simple_kwargs)
     log.info("Embedded Toolshed application started")
 
     global tool_shed_context
     tool_shed_context = app.model.context
 
@@ -698,45 +632,47 @@
 
     # If an explicit port wasn't assigned for this test or test case, set this
     # environment variable so we know it is random. We can then randomly re-assign
     # for new tests.
     if port is None:
         os.environ["GALAXY_TEST_PORT_RANDOM"] = "1"
     else:
-        os.environ['GALAXY_WEB_PORT'] = port
+        os.environ["GALAXY_WEB_PORT"] = port
 
     return host, port
 
 
 def set_and_wait_for_http_target(prefix, host, port, url_prefix, sleep_amount=0.1, sleep_tries=150):
     host_env_key = f"{prefix}_TEST_HOST"
     port_env_key = f"{prefix}_TEST_PORT"
     os.environ[host_env_key] = host
     os.environ[port_env_key] = port
     wait_for_http_server(host, port, url_prefix, sleep_amount=sleep_amount, sleep_tries=sleep_tries)
 
 
 class ServerWrapper:
-
     def __init__(self, name, host, port, prefix=""):
         self.name = name
         self.host = host
         self.port = port
         self.prefix = prefix
 
+    def get_logs(self) -> Optional[str]:
+        # Subclasses can implement a way to return relevant logs
+        pass
+
     @property
     def app(self):
         raise NotImplementedError("Test can be run against target - requires a Galaxy app object.")
 
     def stop(self):
         raise NotImplementedError()
 
 
 class EmbeddedServerWrapper(ServerWrapper):
-
     def __init__(self, app, server, name, host, port, prefix="", thread=None):
         super().__init__(name, host, port, prefix)
         self._app = app
         self._server = server
         self._thread = thread
 
     @property
@@ -762,264 +698,192 @@
             log.info("Embedded server thread stopped")
 
         if self._app is not None:
             log.info(f"Stopping application {self.name}")
             self._app.shutdown()
             log.info(f"Application {self.name} stopped.")
 
-        log.info(f"{threading.active_count()} active after stopping embedded server")
+        thread_count = threading.active_count()
+        log.info(f"{thread_count} active after stopping embedded server")
 
 
-class UwsgiServerWrapper(ServerWrapper):
-
-    def __init__(self, p, name, host, port):
+class GravityServerWrapper(ServerWrapper):
+    def __init__(self, name, host, port, state_dir, stop_command):
         super().__init__(name, host, port)
-        self._p = p
-        self._r = None
-        self._t = threading.Thread(target=self.wait)
-        self._t.start()
-
-    def __del__(self):
-        self._t.join()
+        self.url_prefix = os.environ.get("GALAXY_CONFIG_GALAXY_URL_PREFIX", "/")
+        self.state_dir = Path(state_dir)
+        self.stop_command = stop_command
 
-    def wait(self):
-        self._r = self._p.wait()
-
-    def stop(self):
+    def wait_for_server(self):
         try:
-            os.killpg(os.getpgid(self._p.pid), signal.SIGTERM)
+            set_and_wait_for_http_target(
+                "GALAXY",
+                self.host,
+                self.port,
+                url_prefix=self.url_prefix,
+                sleep_amount=0.4,
+            )
         except Exception:
-            pass
-        time.sleep(.1)
-        try:
-            os.killpg(os.getpgid(self._p.pid), signal.SIGKILL)
-        except Exception:
-            pass
-        self._t.join()
+            log.error("Gravity logs:\n%s", self.get_logs())
 
+    def get_logs(self):
+        gunicorn_logs = (self.state_dir / "log" / "gunicorn.log").read_text()
+        gxit_logs = (self.state_dir / "log" / "gx-it-proxy.log").read_text()
+        celery_logs = (self.state_dir / "log" / "celery.log").read_text()
+        return f"Gunicorn logs:{os.linesep}{gunicorn_logs}{os.linesep}gx-it-proxy logs:{os.linesep}{gxit_logs}celery logs:{os.linesep}{celery_logs}"
 
-def launch_uwsgi(kwargs, tempdir, prefix=DEFAULT_CONFIG_PREFIX, config_object=None):
-    name = prefix.lower()
-
-    host, port = explicitly_configured_host_and_port(prefix, config_object)
-
-    config = {}
-    config["galaxy"] = kwargs.copy()
-
-    enable_realtime_mapping = getattr(config_object, "enable_realtime_mapping", False)
-    if enable_realtime_mapping:
-        interactive_tool_defaults = {
-            "interactivetools_prefix": "interactivetool",
-            "interactivetools_map": os.path.join(tempdir, "interactivetools_map.sqlite"),
-            "interactivetools_enable": True
-        }
-        for key, value in interactive_tool_defaults.items():
-            if key not in config["galaxy"]:
-                config["galaxy"][key] = value
-
-    yaml_config_path = os.path.join(tempdir, "galaxy.yml")
-    with open(yaml_config_path, "w") as f:
-        yaml.dump(config, f)
-
-    if enable_realtime_mapping:
-        # Avoid YAML.dump configuration since uwsgi doesn't like real YAML :( -
-        # though maybe it would work?
-        with open(yaml_config_path) as f:
-            old_contents = f.read()
-        with open(yaml_config_path, "w") as f:
-            test_port = str(port) if port else r"[0-9]+"
-            test_host = re.escape(host) if host else "localhost"
-            uwsgi_section = REALTIME_PROXY_TEMPLATE.safe_substitute(test_host=test_host, test_port=test_port, tempdir=tempdir)
-            f.write(uwsgi_section)
-            f.write(old_contents)
-
-    def attempt_port_bind(port):
-        uwsgi_command = [
-            "uwsgi",
-            "--http",
-            f"{host}:{port}",
-            "--yaml",
-            yaml_config_path,
-            "--module",
-            "galaxy.webapps.galaxy.buildapp:uwsgi_app_factory()",
-            "--enable-threads",
-            "--die-on-term",
-        ]
-        for path in sys.path:
-            uwsgi_command.append('--pythonpath')
-            uwsgi_command.append(path)
+    def stop(self):
+        self.stop_command()
 
-        handle_uwsgi_cli_command = getattr(
-            config_object, "handle_uwsgi_cli_command", None
-        )
-        if handle_uwsgi_cli_command is not None:
-            handle_uwsgi_cli_command(uwsgi_command)
 
-        # we don't want to quote every argument but we don't want to print unquoted ones either, so do this
-        log.info("Starting uwsgi with command line: %s", ' '.join(shlex.quote(x) for x in uwsgi_command))
-        p = subprocess.Popen(
-            uwsgi_command,
-            cwd=galaxy_root,
-            preexec_fn=os.setsid,
-        )
-        return UwsgiServerWrapper(
-            p, name, host, port
-        )
-
-    port = attempt_ports(port)
-    server_wrapper = attempt_port_bind(port)
-    try:
-        set_and_wait_for_http_target(prefix, host, port, url_prefix="/", sleep_tries=50)
-        log.info(f"Test-managed uwsgi web server for {name} started at {host}:{port}")
-        return server_wrapper
-    except Exception:
-        server_wrapper.stop()
+def launch_gravity(port, gxit_port=None, galaxy_config=None):
+    galaxy_config = galaxy_config or {}
+    if not gxit_port:
+        gxit_port = attempt_ports(set_galaxy_web_port=False)
+    if "interactivetools_proxy_host" not in galaxy_config:
+        galaxy_config["interactivetools_proxy_host"] = f"localhost:{gxit_port}"
+    # Can't use in-memory celery broker, just fall back to sqlalchemy
+    celery_conf = galaxy_config.get("celery_conf", {})
+    celery_conf.update({"broker_url": None})
+    galaxy_config["celery_conf"] = celery_conf
+    state_dir = tempfile.mkdtemp(suffix="state")
+    config = {
+        "gravity": {
+            "log_dir": os.path.join(state_dir, "log"),
+            "gunicorn": {"bind": f"localhost:{port}", "preload": "false"},
+            "gx_it_proxy": {
+                "enable": galaxy_config.get("interactivetools_enable", False),
+                "port": gxit_port,
+                "verbose": True,
+                "sessions": galaxy_config.get("interactivetools_map"),
+            },
+        },
+        "galaxy": galaxy_config,
+    }
+    with tempfile.NamedTemporaryFile("w", dir=state_dir, delete=False, suffix=".galaxy.yml") as config_fh:
+        json.dump(config, config_fh)
+    with tempfile.NamedTemporaryFile(delete=True) as socket:
+        supervisord_socket = socket.name
+    gravity_env = os.environ.copy()
+    gravity_env["SUPERVISORD_SOCKET"] = supervisord_socket
+    subprocess.check_output(["galaxyctl", "--config-file", config_fh.name, "update"], env=gravity_env)
+    subprocess.check_output(["galaxyctl", "--config-file", config_fh.name, "start"], env=gravity_env)
+    return state_dir, lambda: subprocess.check_output(
+        ["galaxyctl", "--config-file", config_fh.name, "shutdown"], env=gravity_env
+    )
 
 
-def launch_uvicorn(webapp_factory, prefix=DEFAULT_CONFIG_PREFIX, galaxy_config=None, config_object=None):
+def launch_server(app_factory, webapp_factory, prefix=DEFAULT_CONFIG_PREFIX, galaxy_config=None, config_object=None):
     name = prefix.lower()
-
     host, port = explicitly_configured_host_and_port(prefix, config_object)
     port = attempt_ports(port)
-    gx_app = build_galaxy_app(galaxy_config)
-
-    gx_wsgi_webapp = webapp_factory(
-        galaxy_config['global_conf'],
-        app=gx_app,
-        use_translogger=False,
-        static_enabled=True,
-        register_shutdown_at_exit=False
-    )
-    from galaxy.webapps.galaxy.fast_app import initialize_fast_app
-    app = initialize_fast_app(gx_wsgi_webapp, gx_app)
-    server, port, thread = uvicorn_serve(app, host=host, port=port)
-    set_and_wait_for_http_target(prefix, host, port, url_prefix=gx_app.config.galaxy_url_prefix)
-    log.info(f"Embedded uvicorn web server for {name} started at {host}:{port}{gx_app.config.galaxy_url_prefix}")
-    return EmbeddedServerWrapper(
-        gx_app, server, name, host, port, thread=thread, prefix=gx_app.config.galaxy_url_prefix
-    )
-
-
-def launch_server(app, webapp_factory, kwargs, prefix=DEFAULT_CONFIG_PREFIX, config_object=None):
-    """Launch a web server for a given app using supplied factory.
-
-    Consistently read either GALAXY_TEST_HOST and GALAXY_TEST_PORT or
-    TOOL_SHED_TEST_HOST and TOOL_SHED_TEST_PORT and ensure these are
-    all set after this method has been called.
-    """
-    name = prefix.lower()
 
-    host, port = explicitly_configured_host_and_port(prefix, config_object)
+    enable_realtime_mapping = getattr(config_object, "enable_realtime_mapping", False)
+    if enable_realtime_mapping:
+        interactive_tool_defaults = {
+            "interactivetools_map": tempfile.NamedTemporaryFile(
+                delete=False, suffix="interactivetools_map.sqlite"
+            ).name,
+            "interactivetools_enable": True,
+            "interactivetools_upstream_proxy": False,
+            "galaxy_infrastructure_url": f"http://localhost:{port}",
+        }
+        interactive_tool_defaults.update(galaxy_config or {})
+        galaxy_config = interactive_tool_defaults
 
-    webapp = webapp_factory(
-        kwargs['global_conf'],
+    if enable_realtime_mapping or os.environ.get("GALAXY_TEST_GRAVITY"):
+        galaxy_config["root"] = galaxy_root
+        state_dir, stop_command = launch_gravity(port=port, galaxy_config=galaxy_config)
+        gravity_wrapper = GravityServerWrapper(name, host, port, state_dir, stop_command)
+        gravity_wrapper.wait_for_server()
+        return gravity_wrapper
+
+    app = app_factory()
+    url_prefix = getattr(app.config, f"{name}_url_prefix", "/")
+    wsgi_webapp = webapp_factory(
+        galaxy_config["global_conf"],
         app=app,
         use_translogger=False,
         static_enabled=True,
-        register_shutdown_at_exit=False
-    )
-    server, port = serve_webapp(
-        webapp,
-        host=host, port=port
-    )
-    set_and_wait_for_http_target(prefix, host, port, url_prefix="/")
-    log.info(f"Embedded paste web server for {name} started at {host}:{port}")
-    return EmbeddedServerWrapper(
-        app, server, name, host, port
+        register_shutdown_at_exit=False,
     )
+    if name == "galaxy":
+        asgi_app = init_galaxy_fast_app(wsgi_webapp, app)
+    elif name == "tool_shed":
+        asgi_app = init_tool_shed_fast_app(wsgi_webapp, app)
+    else:
+        raise NotImplementedError(f"Launching {name} not implemented")
+
+    server, port, thread = uvicorn_serve(asgi_app, host=host, port=port)
+    set_and_wait_for_http_target(prefix, host, port, url_prefix=url_prefix)
+    log.debug(f"Embedded uvicorn web server for {name} started at {host}:{port}{url_prefix}")
+    return EmbeddedServerWrapper(app, server, name, host, port, thread=thread, prefix=url_prefix)
 
 
 class TestDriver:
     """Responsible for the life-cycle of a Galaxy-style functional test.
 
-    Sets up servers, configures tests, runs nose, and tears things
+    Sets up servers, configures tests, and tears things
     down. This is somewhat like a Python TestCase - but different
     because it is meant to provide a main() endpoint.
     """
+
     __test__ = False  # Prevent pytest from discovering this class (issue #12071)
 
     def __init__(self):
         """Setup tracked resources."""
         self.server_wrappers = []
         self.temp_directories = []
 
-    def setup(self):
+    def setup(self, config_object=None):
         """Called before tests are built."""
 
     def build_tests(self):
-        """After environment is setup, setup nose tests."""
+        """After environment is setup, setup tests."""
 
     def tear_down(self):
         """Cleanup resources tracked by this object."""
         self.stop_servers()
         for temp_directory in self.temp_directories:
             cleanup_directory(temp_directory)
 
     def stop_servers(self):
         for server_wrapper in self.server_wrappers:
             server_wrapper.stop()
+        for th in threading.enumerate():
+            log.debug(f"After stopping all servers thread {th} is alive.")
+        active_count = threading.active_count()
+        if active_count > 100:
+            # For an unknown reason running iRODS tests results in application threads not shutting down immediately,
+            # but if we've accumulated over 100 active threads something else is wrong that needs to be fixed.
+            raise Exception(
+                f"{active_count} active threads after stopping embedded server. Have all threads been shut down?"
+            )
         self.server_wrappers = []
 
-    def mkdtemp(self):
+    def mkdtemp(self) -> str:
         """Return a temp directory that is properly cleaned up or not based on the config."""
         temp_directory = tempfile.mkdtemp()
         self.temp_directories.append(temp_directory)
         return temp_directory
 
-    def run(self):
-        """Driver whole test.
-
-        Setup environment, build tests (if needed), run test,
-        and finally cleanup resources.
-        """
-        configure_environment()
-        self.setup()
-        self.build_tests()
-        try:
-            success = nose_config_and_run()
-            return 0 if success else 1
-        except Exception as e:
-            log.info("Failure running tests")
-            raise e
-        finally:
-            log.info("Shutting down")
-            self.tear_down()
-
 
 class GalaxyTestDriver(TestDriver):
-    """Instantial a Galaxy-style nose TestDriver for testing Galaxy."""
+    """Instantial a Galaxy-style TestDriver for testing Galaxy."""
 
+    server_wrappers: List[ServerWrapper]
     testing_shed_tools = False
 
     def _configure(self, config_object=None):
         """Setup various variables used to launch a Galaxy server."""
         config_object = self._ensure_config_object(config_object)
-        self.external_galaxy = os.environ.get('GALAXY_TEST_EXTERNAL', None)
-
-        # Allow a particular test to force uwsgi or any test to use uwsgi with
-        # the GALAXY_TEST_UWSGI environment variable.
-        use_uwsgi = bool(os.environ.get('GALAXY_TEST_UWSGI', None))
-        if not use_uwsgi:
-            if getattr(config_object, "require_uwsgi", None):
-                use_uwsgi = True
-        self.use_uwsgi = use_uwsgi
-
-        if getattr(config_object, "use_uvicorn", USE_UVICORN):
-            self.else_use_uvicorn = True
-        else:
-            self.else_use_uvicorn = False
+        self.external_galaxy = os.environ.get("GALAXY_TEST_EXTERNAL", None)
 
         # Allow controlling the log format
-        log_format = os.environ.get('GALAXY_TEST_LOG_FORMAT', None)
-        if not log_format and use_uwsgi:
-            log_format = "%(name)s %(levelname)-5.5s %(asctime)s " \
-                         "[p:%(process)s,w:%(worker_id)s,m:%(mule_id)s] " \
-                         "[%(threadName)s] %(message)s"
-
-        self.log_format = log_format
+        self.log_format = os.environ.get("GALAXY_TEST_LOG_FORMAT")
 
         self.galaxy_test_tmp_dir = get_galaxy_test_tmp_dir()
         self.temp_directories.append(self.galaxy_test_tmp_dir)
 
         self.testing_shed_tools = getattr(config_object, "testing_shed_tools", False)
 
         default_tool_conf: Optional[str]
@@ -1041,14 +905,19 @@
         Configuration options can be specified as attributes on the supplied
         ```config_object``` (defaults to self).
         """
         self._saved_galaxy_config = None
         self._configure(config_object)
         self._register_and_run_servers(config_object)
 
+    def get_logs(self):
+        if self.server_wrappers:
+            server_wrapper = self.server_wrappers[0]
+            return server_wrapper.get_logs()
+
     def restart(self, config_object=None, handle_config=None):
         self.stop_servers()
         self._register_and_run_servers(config_object, handle_config=handle_config)
 
     def _register_and_run_servers(self, config_object=None, handle_config=None):
         config_object = self._ensure_config_object(config_object)
         self.app = None
@@ -1085,74 +954,55 @@
                     isolate_galaxy_config = getattr(config_object, "isolate_galaxy_config", False)
                     if isolate_galaxy_config:
                         galaxy_config["config_dir"] = tempdir
 
                     self._saved_galaxy_config = galaxy_config
 
             if galaxy_config is not None:
-                handle_galaxy_config_kwds = handle_config or getattr(
-                    config_object, "handle_galaxy_config_kwds", None
-                )
+                handle_galaxy_config_kwds = handle_config or getattr(config_object, "handle_galaxy_config_kwds", None)
                 if handle_galaxy_config_kwds is not None:
                     handle_galaxy_config_kwds(galaxy_config)
 
-            if self.use_uwsgi:
-                server_wrapper = launch_uwsgi(
-                    galaxy_config,
-                    tempdir=tempdir,
-                    config_object=config_object,
-                )
-            elif self.else_use_uvicorn:
-                server_wrapper = launch_uvicorn(
-                    lambda *args, **kwd: buildapp.app_factory(*args, wsgi_preflight=False, **kwd),
-                    galaxy_config=galaxy_config,
-                    config_object=config_object,
-                )
-                self.app = server_wrapper.app
-            else:
-                # ---- Build Application --------------------------------------------------
-                self.app = build_galaxy_app(galaxy_config)
-                server_wrapper = launch_server(
-                    self.app,
-                    buildapp.app_factory,
-                    galaxy_config,
-                    config_object=config_object,
-                )
-                log.info(f"Functional tests will be run against external Galaxy server {server_wrapper.host}:{server_wrapper.port}")
+            server_wrapper = launch_server(
+                app_factory=lambda: self.build_galaxy_app(galaxy_config),
+                webapp_factory=lambda *args, **kwd: buildapp.app_factory(*args, wsgi_preflight=False, **kwd),
+                galaxy_config=galaxy_config,
+                config_object=config_object,
+            )
             self.server_wrappers.append(server_wrapper)
         else:
-            log.info(f"Functional tests will be run against test managed Galaxy server {self.external_galaxy}")
+            log.info(f"Functional tests will be run against test external Galaxy server {self.external_galaxy}")
             # Ensure test file directory setup even though galaxy config isn't built.
             ensure_test_file_dir_set()
 
+    def build_galaxy_app(self, galaxy_config):
+        self.app = build_galaxy_app(galaxy_config)
+        return self.app
+
     def _ensure_config_object(self, config_object):
         if config_object is None:
             config_object = self
         return config_object
 
     def setup_shed_tools(self, testing_migrated_tools=False, testing_installed_tools=True):
-        setup_shed_tools_for_test(
-            self.app,
-            self.galaxy_test_tmp_dir,
-            testing_migrated_tools,
-            testing_installed_tools
-        )
+        setup_shed_tools_for_test(self.app, self.galaxy_test_tmp_dir, testing_migrated_tools, testing_installed_tools)
 
     def build_tool_tests(self, testing_shed_tools=None, return_test_classes=False):
         if self.app is None:
             return
 
         if testing_shed_tools is None:
             testing_shed_tools = getattr(self, "testing_shed_tools", False)
 
         # We must make sure that functional.test_toolbox is always imported after
         # database_contexts.galaxy_content is set (which occurs in this method above).
         # If functional.test_toolbox is imported before database_contexts.galaxy_content
         # is set, sa_session will be None in all methods that use it.
         import functional.test_toolbox
+
         functional.test_toolbox.toolbox = self.app.toolbox
         # When testing data managers, do not test toolbox.
         test_classes = functional.test_toolbox.build_tests(
             app=self.app,
             testing_shed_tools=testing_shed_tools,
             master_api_key=get_admin_api_key(),
             user_api_key=get_user_api_key(),
@@ -1173,15 +1023,15 @@
         }
         galaxy_interactor = GalaxyInteractorApi(**galaxy_interactor_kwds)
         verify_tool(
             tool_id=tool_id,
             test_index=index,
             galaxy_interactor=galaxy_interactor,
             resource_parameters=resource_parameters,
-            **kwd
+            **kwd,
         )
 
 
 def drive_test(test_driver_class):
     """Instantiate driver class, run, and exit appropriately."""
     test_driver = test_driver_class()
     sys.exit(test_driver.run())
@@ -1192,12 +1042,11 @@
     "build_logger",
     "drive_test",
     "FRAMEWORK_UPLOAD_TOOL_CONF",
     "FRAMEWORK_SAMPLE_TOOLS_CONF",
     "FRAMEWORK_DATATYPES_CONF",
     "database_conf",
     "get_webapp_global_conf",
-    "nose_config_and_run",
     "setup_galaxy_config",
     "TestDriver",
     "wait_for_http_server",
 )
```

### Comparing `galaxy-test-driver-22.1.1/galaxy_test/driver/integration_setup.py` & `galaxy-test-driver-23.0.2/galaxy_test/driver/integration_setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,18 +2,20 @@
 Test classes that should be shared between test scenarios.
 """
 import os
 import shutil
 from tempfile import mkdtemp
 from typing import ClassVar
 
-from .driver_util import GalaxyTestDriver
+from galaxy_test.driver.driver_util import GalaxyTestDriver
 
-REQUIRED_ROLE = "user@bx.psu.edu"
-REQUIRED_GROUP = "fs_test_group"
+REQUIRED_ROLE_EXPRESSION = "user@bx.psu.edu"
+GROUP_A = "fs_test_group"
+GROUP_B = "group name with spaces"
+REQUIRED_GROUP_EXPRESSION = f"{GROUP_A} or '{GROUP_B}'"
 
 
 def get_posix_file_source_config(root_dir: str, roles: str, groups: str, include_test_data_dir: bool) -> str:
     rval = f"""
 - type: posix
   id: posix_test
   label: Posix
@@ -31,34 +33,56 @@
   doc: Galaxy's test-data directory.
   root: test-data
   writable: false
 """
     return rval
 
 
-def create_file_source_config_file_on(temp_dir, root_dir, include_test_data_dir):
-    file_contents = get_posix_file_source_config(root_dir, REQUIRED_ROLE, REQUIRED_GROUP, include_test_data_dir)
+def create_file_source_config_file_on(
+    temp_dir,
+    root_dir,
+    include_test_data_dir,
+    required_role_expression,
+    required_group_expression,
+):
+    file_contents = get_posix_file_source_config(
+        root_dir, required_role_expression, required_group_expression, include_test_data_dir
+    )
     file_path = os.path.join(temp_dir, "file_sources_conf_posix.yml")
     with open(file_path, "w") as f:
         f.write(file_contents)
     return file_path
 
 
 class PosixFileSourceSetup:
     _test_driver: GalaxyTestDriver
     root_dir: str
     include_test_data_dir: ClassVar[bool] = False
 
     @classmethod
-    def handle_galaxy_config_kwds(cls, config):
+    def handle_galaxy_config_kwds(
+        cls,
+        config,
+        clazz_=None,
+        # Require role for access but do not require groups by default on every test to simplify them
+        required_role_expression=REQUIRED_ROLE_EXPRESSION,
+        required_group_expression="",
+    ):
         temp_dir = os.path.realpath(mkdtemp())
-        cls._test_driver.temp_directories.append(temp_dir)
-        cls.root_dir = os.path.join(temp_dir, "root")
-
-        file_sources_config_file = create_file_source_config_file_on(temp_dir, cls.root_dir, cls.include_test_data_dir)
+        clazz_ = clazz_ or cls
+        clazz_._test_driver.temp_directories.append(temp_dir)
+        clazz_.root_dir = os.path.join(temp_dir, "root")
+
+        file_sources_config_file = create_file_source_config_file_on(
+            temp_dir,
+            clazz_.root_dir,
+            clazz_.include_test_data_dir,
+            required_role_expression,
+            required_group_expression,
+        )
         config["file_sources_config_file"] = file_sources_config_file
 
         # Disable all stock plugins
         config["ftp_upload_dir"] = None
         config["library_import_dir"] = None
         config["user_library_import_dir"] = None
```

### Comparing `galaxy-test-driver-22.1.1/galaxy_test/driver/integration_util.py` & `galaxy-test-driver-23.0.2/galaxy_test/driver/integration_util.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,29 +1,46 @@
 """Utilities for constructing Galaxy integration tests.
 
 Tests that start an actual Galaxy server with a particular configuration in
 order to test something that cannot be tested with the default functional/api
 testing configuration.
 """
 import os
-from typing import ClassVar
-from unittest import skip, SkipTest, TestCase
+from typing import (
+    ClassVar,
+    Iterator,
+    Optional,
+    Type,
+    TYPE_CHECKING,
+    TypeVar,
+)
+from unittest import (
+    skip,
+    SkipTest,
+)
 
 import pytest
 
 from galaxy.app import UniverseApplication
 from galaxy.tool_util.verify.test_data import TestDataResolver
 from galaxy.util.commands import which
-from galaxy_test.base.api import UsesApiTestCaseMixin
+from galaxy.util.unittest import TestCase
+from galaxy_test.base.api import (
+    UsesApiTestCaseMixin,
+    UsesCeleryTasks,
+)
 from .driver_util import GalaxyTestDriver
 
+if TYPE_CHECKING:
+    from galaxy_test.base.populators import BaseDatasetPopulator
+
 NO_APP_MESSAGE = "test_case._app called though no Galaxy has been configured."
 # Following should be for Homebrew Rabbitmq and Docker on Mac "amqp://guest:guest@localhost:5672//"
 AMQP_URL = os.environ.get("GALAXY_TEST_AMQP_URL", None)
-POSTGRES_CONFIGURED = 'postgres' in os.environ.get("GALAXY_TEST_DBURI", '')
+POSTGRES_CONFIGURED = "postgres" in os.environ.get("GALAXY_TEST_DBURI", "")
 
 
 def _identity(func):
     return func
 
 
 def skip_if_jenkins(cls):
@@ -56,15 +73,15 @@
 
 
 def skip_unless_kubernetes():
     return skip_unless_executable("kubectl")
 
 
 def k8s_config_path():
-    return os.environ.get('GALAXY_TEST_KUBE_CONFIG_PATH', '~/.kube/config')
+    return os.environ.get("GALAXY_TEST_KUBE_CONFIG_PATH", "~/.kube/config")
 
 
 def skip_unless_fixed_port():
     if os.environ.get("GALAXY_TEST_PORT_RANDOM") != "1":
         return _identity
 
     return pytest.mark.skip("GALAXY_TEST_PORT must be set for this test.")
@@ -73,28 +90,36 @@
 def skip_if_github_workflow():
     if os.environ.get("GITHUB_ACTIONS", None) is None:
         return _identity
 
     return pytest.mark.skip("This test is skipped for Github actions.")
 
 
-class IntegrationInstance(UsesApiTestCaseMixin):
+def skip_unless_environ(env_var):
+    if os.environ.get(env_var):
+        return _identity
+
+    return pytest.mark.skip(f"{env_var} must be set for this test")
+
+
+class IntegrationInstance(UsesApiTestCaseMixin, UsesCeleryTasks):
     """Unit test case with utilities for spinning up Galaxy."""
+
     _test_driver: GalaxyTestDriver  # Optional in parent class, but required for integration tests.
 
     _app_available: ClassVar[bool]
 
     prefer_template_database = True
-    # Subclasses can override this to force uwsgi for tests.
-    require_uwsgi = False
 
     # Don't pull in default configs for un-configured things from Galaxy's
     # config directory and such.
     isolate_galaxy_config = True
 
+    dataset_populator: Optional["BaseDatasetPopulator"]
+
     @classmethod
     def setUpClass(cls):
         """Configure and start Galaxy for a test."""
         cls._app_available = False
         cls._test_driver = GalaxyTestDriver()
         cls._prepare_galaxy()
         cls._test_driver.setup(config_object=cls)
@@ -103,24 +128,30 @@
 
     @classmethod
     def tearDownClass(cls):
         """Shutdown Galaxy server and cleanup temp directory."""
         cls._test_driver.tear_down()
         cls._app_available = False
 
+    def tearDown(self):
+        logs = self._test_driver.get_logs()
+        if logs:
+            print(logs)
+        return super().tearDown()
+
     def setUp(self):
         self.test_data_resolver = TestDataResolver()
         self._configure_interactor()
 
     def _configure_interactor(self):
         # Setup attributes needed for API testing...
         server_wrapper = self._test_driver.server_wrappers[0]
         host = server_wrapper.host
         port = server_wrapper.port
-        prefix = server_wrapper.prefix or ''
+        prefix = server_wrapper.prefix or ""
         self.url = f"http://{host}:{port}{prefix.rstrip('/')}/"
         self._setup_interactor()
 
     def restart(self, handle_reconfig=None):
         self._test_driver.restart(config_object=self.__class__, handle_config=handle_reconfig)
         self._configure_app()
         self._configure_interactor()
@@ -147,66 +178,45 @@
         ```self._app``` can be used to access Galaxy core app.
         """
 
     def _skip_unless_postgres(self):
         if not self._app.config.database_connection.startswith("post"):
             raise SkipTest("Test only valid for postgres")
 
-    @classmethod
-    def handle_galaxy_config_kwds(cls, galaxy_config_kwds):
-        """Extension point for subclasses to modify arguments used to configure Galaxy.
-
-        This method will be passed the keyword argument pairs used to call
-        Galaxy Config object and can modify the Galaxy instance created for
-        the test as needed.
-        """
-
-    @classmethod
-    def handle_uwsgi_cli_command(cls, command):
-        """Extension point sub subclasses to modify arguments used to launch uWSGI server.
-
-        Command will a list that can be modified.
-        """
-
     def _run_tool_test(self, *args, **kwargs):
         return self._test_driver.run_tool_test(*args, **kwargs)
 
     @classmethod
     def temp_config_dir(cls, name):
         # realpath here to get around problems with symlinks being blocked.
         return os.path.realpath(os.path.join(cls._test_driver.galaxy_test_tmp_dir, name))
 
-
-class UsesCeleryTasks:
-    enable_celery_tasks = True
-
-    @pytest.fixture(autouse=True)
-    def _request_celery_app(self, celery_app):
-        self._celery_app = celery_app
-
-    @pytest.fixture(autouse=True)
-    def _request_celery_worker(self, celery_worker):
-        self._celery_worker = celery_worker
+    @pytest.fixture
+    def history_id(self) -> Iterator[str]:
+        assert self.dataset_populator
+        with self.dataset_populator.test_history() as history_id:
+            yield history_id
 
 
 class IntegrationTestCase(IntegrationInstance, TestCase):
     """Unit TestCase with utilities for spinning up Galaxy."""
 
 
-def integration_module_instance(clazz):
+IntegrationInstanceObject = TypeVar("IntegrationInstanceObject", bound=IntegrationInstance)
 
-    def _instance():
+
+def integration_module_instance(clazz: Type[IntegrationInstanceObject]):
+    def _instance() -> Iterator[IntegrationInstanceObject]:
         instance = clazz()
         instance.setUpClass()
         instance.setUp()
         yield instance
         instance.tearDownClass()
 
-    return pytest.fixture(scope='module')(_instance)
+    return pytest.fixture(scope="module")(_instance)
 
 
 def integration_tool_runner(tool_ids):
-
     def test_tools(instance, tool_id):
         instance._run_tool_test(tool_id)
 
     return pytest.mark.parametrize("tool_id", tool_ids)(test_tools)
```

### Comparing `galaxy-test-driver-22.1.1/galaxy_test_driver.egg-info/PKG-INFO` & `galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,69 +1,71 @@
 Metadata-Version: 2.1
 Name: galaxy-test-driver
-Version: 22.1.1
-Summary: Galaxy Test Driver
+Version: 23.0.2
+Summary: Galaxy test driver
 Home-page: https://github.com/galaxyproject/galaxy
 Author: Galaxy Project and Community
 Author-email: galaxy-committers@lists.galaxyproject.org
 License: AFL
-Keywords: galaxy
-Platform: UNKNOWN
+Keywords: Galaxy
 Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
 Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Academic Free License (AFL)
-Classifier: Operating System :: POSIX
-Classifier: Topic :: Software Development
-Classifier: Topic :: Software Development :: Testing
 Classifier: Natural Language :: English
+Classifier: Operating System :: POSIX
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: Software Development :: Code Generators
+Classifier: Topic :: Software Development :: Testing
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: https://badge.fury.io/py/galaxy-test-driver.svg
    :target: https://pypi.org/project/galaxy-test-driver/
 
 
 
 Overview
 --------
 
 The Galaxy_ test driver package.
 
-* Free software: Academic Free License version 3.0
 * Code: https://github.com/galaxyproject/galaxy
 
 .. _Galaxy: http://galaxyproject.org/
 
-
-
-
 History
 -------
 
 .. to_doc
 
----------------------
-20.9.1.dev0
----------------------
+-------------------
+23.0.2 (2023-06-13)
+-------------------
 
+No recorded changes since last release
 
+-------------------
+23.0.1 (2023-06-08)
+-------------------
 
----------------------
+No recorded changes since last release
+
+-------------------
 20.9.0 (2020-10-15)
----------------------
+-------------------
 
 * First release from the 20.09 branch of Galaxy.
 
----------------------
+-------------------
 20.5.0 (2020-07-04)
----------------------
+-------------------
 
 * First release from the 20.05 branch of Galaxy.
-
-
```

### Comparing `galaxy-test-driver-22.1.1/galaxy_test_driver.egg-info/SOURCES.txt` & `galaxy-test-driver-23.0.2/galaxy_test_driver.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -1,29 +1,22 @@
 HISTORY.rst
 LICENSE
 MANIFEST.in
-Makefile
 README.rst
 dev-requirements.txt
-requirements.txt
+pyproject.toml
 setup.cfg
-setup.py
 test-requirements.txt
-galaxy/__init__.py
-galaxy/project_galaxy_test_driver.py
 galaxy_test/__init__.py
+galaxy_test/py.typed
 galaxy_test/driver/__init__.py
 galaxy_test/driver/driver_util.py
 galaxy_test/driver/integration_setup.py
 galaxy_test/driver/integration_util.py
 galaxy_test/driver/test_logging.py
 galaxy_test/driver/testcase.py
+galaxy_test/driver/uses_shed.py
 galaxy_test_driver.egg-info/PKG-INFO
 galaxy_test_driver.egg-info/SOURCES.txt
 galaxy_test_driver.egg-info/dependency_links.txt
-galaxy_test_driver.egg-info/entry_points.txt
-galaxy_test_driver.egg-info/not-zip-safe
 galaxy_test_driver.egg-info/requires.txt
-galaxy_test_driver.egg-info/top_level.txt
-scripts/commit_version.py
-scripts/new_version.py
-scripts/print_version_for_release.py
+galaxy_test_driver.egg-info/top_level.txt
```

