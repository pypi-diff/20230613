# Comparing `tmp/dapp-manager-0.1.1.tar.gz` & `tmp/dapp_manager-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapp-manager-0.1.1.tar", max compression
+gzip compressed data, was "dapp_manager-0.1.2.tar", max compression
```

## Comparing `dapp-manager-0.1.1.tar` & `dapp_manager-0.1.2.tar`

### file list

```diff
@@ -1,27 +1,26 @@
--rw-r--r--   0        0        0    26526 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/LICENSE
--rw-r--r--   0        0        0     7276 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/README.md
--rw-r--r--   0        0        0      149 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/__init__.py
--rw-r--r--   0        0        0       97 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/__main__.py
--rw-r--r--   0        0        0     1261 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/autocomplete/__init__.py
--rw-r--r--   0        0        0      674 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/autocomplete/scripts/.dapp-manager.bash
--rw-r--r--   0        0        0      171 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/autocomplete/scripts/.dapp-manager.fish
--rw-r--r--   0        0        0      900 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/autocomplete/scripts/.dapp-manager.zsh
--rw-r--r--   0        0        0     4825 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/cli.py
--rw-r--r--   0        0        0     9265 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/dapp_manager.py
--rw-r--r--   0        0        0     4056 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/dapp_starter.py
--rw-r--r--   0        0        0     2067 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/py.typed
--rw-r--r--   0        0        0     4887 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_manager/storage.py
--rw-r--r--   0        0        0       50 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/README.md
--rw-r--r--   0        0        0       70 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/__init__.py
--rw-r--r--   0        0        0     1634 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/__main__.py
--rw-r--r--   0        0        0     4928 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/dapp_size_resolver.py
--rw-r--r--   0        0        0     1960 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/dapp_stats.py
--rw-r--r--   0        0        0      118 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/exceptions.py
--rw-r--r--   0        0        0        0 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/statistics/__init__.py
--rw-r--r--   0        0        0      360 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/statistics/enums.py
--rw-r--r--   0        0        0     1272 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/statistics/models.py
--rw-r--r--   0        0        0      257 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/dapp_stats/statistics/schemas.py
--rw-r--r--   0        0        0     4499 2023-04-11 16:28:42.105961 dapp-manager-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8658 1970-01-01 00:00:00.000000 dapp-manager-0.1.1/setup.py
--rw-r--r--   0        0        0     8499 1970-01-01 00:00:00.000000 dapp-manager-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    26526 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/LICENSE
+-rw-r--r--   0        0        0     7276 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/README.md
+-rw-r--r--   0        0        0      149 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/__init__.py
+-rw-r--r--   0        0        0       97 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/__main__.py
+-rw-r--r--   0        0        0     1261 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/autocomplete/__init__.py
+-rw-r--r--   0        0        0      674 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/autocomplete/scripts/.dapp-manager.bash
+-rw-r--r--   0        0        0      171 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/autocomplete/scripts/.dapp-manager.fish
+-rw-r--r--   0        0        0      900 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/autocomplete/scripts/.dapp-manager.zsh
+-rw-r--r--   0        0        0     4825 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/cli.py
+-rw-r--r--   0        0        0     9265 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/dapp_manager.py
+-rw-r--r--   0        0        0     4056 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/dapp_starter.py
+-rw-r--r--   0        0        0     2067 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/py.typed
+-rw-r--r--   0        0        0     4887 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_manager/storage.py
+-rw-r--r--   0        0        0       50 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/README.md
+-rw-r--r--   0        0        0       70 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/__init__.py
+-rw-r--r--   0        0        0     1634 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/__main__.py
+-rw-r--r--   0        0        0     4928 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/dapp_size_resolver.py
+-rw-r--r--   0        0        0     1960 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/dapp_stats.py
+-rw-r--r--   0        0        0      118 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/exceptions.py
+-rw-r--r--   0        0        0        0 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/statistics/__init__.py
+-rw-r--r--   0        0        0      360 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/statistics/enums.py
+-rw-r--r--   0        0        0     1272 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/statistics/models.py
+-rw-r--r--   0        0        0      257 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/dapp_stats/statistics/schemas.py
+-rw-r--r--   0        0        0     4499 2023-06-13 10:19:21.295325 dapp_manager-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     8500 1970-01-01 00:00:00.000000 dapp_manager-0.1.2/PKG-INFO
```

### Comparing `dapp-manager-0.1.1/LICENSE` & `dapp_manager-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.1/README.md` & `dapp_manager-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.1/dapp_manager/autocomplete/__init__.py` & `dapp_manager-0.1.2/dapp_manager/autocomplete/__init__.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.1/dapp_manager/autocomplete/scripts/.dapp-manager.bash` & `dapp_manager-0.1.2/dapp_manager/autocomplete/scripts/.dapp-manager.bash`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.1/dapp_manager/autocomplete/scripts/.dapp-manager.zsh` & `dapp_manager-0.1.2/dapp_manager/autocomplete/scripts/.dapp-manager.zsh`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.1/dapp_manager/cli.py` & `dapp_manager-0.1.2/dapp_manager/cli.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.1/dapp_manager/dapp_manager.py` & `dapp_manager-0.1.2/dapp_manager/dapp_manager.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.1/dapp_manager/dapp_starter.py` & `dapp_manager-0.1.2/dapp_manager/dapp_starter.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.1/dapp_manager/exceptions.py` & `dapp_manager-0.1.2/dapp_manager/exceptions.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.1/dapp_manager/storage.py` & `dapp_manager-0.1.2/dapp_manager/storage.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.1/dapp_stats/__main__.py` & `dapp_manager-0.1.2/dapp_stats/__main__.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.1/dapp_stats/dapp_size_resolver.py` & `dapp_manager-0.1.2/dapp_stats/dapp_size_resolver.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.1/dapp_stats/dapp_stats.py` & `dapp_manager-0.1.2/dapp_stats/dapp_stats.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.1/dapp_stats/statistics/models.py` & `dapp_manager-0.1.2/dapp_stats/statistics/models.py`

 * *Files identical despite different names*

### Comparing `dapp-manager-0.1.1/pyproject.toml` & `dapp_manager-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapp-manager"
-version = "0.1.1"
+version = "0.1.2"
 description = "Golem dapp-manager - run decetralized apps on the Golem Network using a 'docker-compose'-like interface"
 authors = ["Golem Factory <contact@golem.network>"]
 license = "LGPL-3.0"
 classifiers = [
   "Development Status :: 2 - Pre-Alpha",
   "Environment :: Console",
   "Intended Audience :: Developers",
@@ -31,15 +31,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 
 psutil = "^5.9"
 appdirs = "^1.4"
 click = "^7.0"  # requires bump to goth's dependencies https://github.com/golemfactory/goth/issues/605
 pydantic = "^1.9"
-dapp-runner = "^0.1.1"
+dapp-runner = "^0.1.2"
 
 [tool.poetry.group.dev.dependencies]
 setuptools = "*"  # implicitly required by liccehck
 pip = "*"  # implicitly required by liccehck
 
 autoflake = "^1"
 black = "^21.0b0"  # requires bump to goth's dependencies https://github.com/golemfactory/goth/issues/605
```

### Comparing `dapp-manager-0.1.1/setup.py` & `dapp_manager-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,42 +1,266 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: dapp-manager
+Version: 0.1.2
+Summary: Golem dapp-manager - run decetralized apps on the Golem Network using a 'docker-compose'-like interface
+Home-page: https://github.com/golemfactory/dapp-manager
+License: LGPL-3.0
+Author: Golem Factory
+Author-email: contact@golem.network
+Requires-Python: >=3.8,<4.0
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Topic :: Software Development
+Classifier: Topic :: System :: Distributed Computing
+Requires-Dist: appdirs (>=1.4,<2.0)
+Requires-Dist: click (>=7.0,<8.0)
+Requires-Dist: dapp-runner (>=0.1.2,<0.2.0)
+Requires-Dist: psutil (>=5.9,<6.0)
+Requires-Dist: pydantic (>=1.9,<2.0)
+Project-URL: Repository, https://github.com/golemfactory/dapp-manager
+Description-Content-Type: text/markdown
 
-packages = \
-['dapp_manager',
- 'dapp_manager.autocomplete',
- 'dapp_stats',
- 'dapp_stats.statistics']
-
-package_data = \
-{'': ['*'], 'dapp_manager.autocomplete': ['scripts/*']}
-
-install_requires = \
-['appdirs>=1.4,<2.0',
- 'click>=7.0,<8.0',
- 'dapp-runner>=0.1.1,<0.2.0',
- 'psutil>=5.9,<6.0',
- 'pydantic>=1.9,<2.0']
-
-entry_points = \
-{'console_scripts': ['dapp-manager = dapp_manager.__main__:main',
-                     'dapp-stats = dapp_stats.__main__:main']}
-
-setup_kwargs = {
-    'name': 'dapp-manager',
-    'version': '0.1.1',
-    'description': "Golem dapp-manager - run decetralized apps on the Golem Network using a 'docker-compose'-like interface",
-    'long_description': '# Golem dApp Manager\n\n`dapp-manager` is a purposefully minimalistic manager for decentralized applications running on\nGolem. It works together with the [dapp-runner](https://github.com/golemfactory/dapp-runner/).\nWhile the responsibility of the latter is to run a single Golem application, `dapp-manager` takes\ncare of spawning, interacting with, and stopping the running instances of the `dapp-runner`.\n\n## Quick start\n\n### Yagna daemon\n\nAs the `dapp-manager` uses the `dapp-runner`, which in turn requires a properly configured\n[yagna](https://github.com/golemfactory/yagna) daemon, you\'ll need to have it set up.\n\nFor now, please follow the ["Requestor development: a quick primer"](https://handbook.golem.network/requestor-tutorials/flash-tutorial-of-requestor-development)\ntutorial and ensure that your `yagna` is up and running. Only the first part of this\ntutorial is required - you don\'t need to run the blender example.\n\nMost importantly, make sure you have set the `YAGNA_APPKEY` in your environment, e.g. with:\n\n```bash\nexport YAGNA_APPKEY=insert-your-32-char-app-key-here\n```\n\nor, on Windows:\n\n```bash\nset YAGNA_APPKEY=insert-your-32-char-app-key-here\n```\n\nand if you don\'t know what your app-key is, you can always query `yagna` with:\n\n```bash\nyagna app-key list\n```\n\n### Python environment\n\nFirst, ensure you have Python 3.8 or later:\n\n```bash\npython3 --version\n```\n\n[ depending on the platform, it may be just `python` instead of `python3` ]\n\nIf your Python version is older, consider using [pyenv](https://github.com/pyenv/pyenv-installer).\n\nOnce your python interpreter reports a version 3.8 or later, you can set up your virtual\nenvironment:\n\n```bash\npython3 -m venv ~/.envs/dapp-manager\nsource ~/.envs/dapp-manager/bin/activate\n```\n\nor, if you\'re on Windows:\n\n```shell\npython -m venv --clear %HOMEDRIVE%%HOMEPATH%\\.envs\\dapp-manager\n%HOMEDRIVE%%HOMEPATH%\\.envs\\dapp-manager\\Scripts\\activate.bat\n```\n\n### DApp manager\n\n#### Clone the repository\n\n```bash\ngit clone --recurse-submodules https://github.com/golemfactory/dapp-manager.git\n```\n\n#### Install the dependencies\n\n```bash\ncd dapp-manager\npip install -U pip poetry\npoetry install\n```\n\n#### Run an example application\n\nMake sure your `yagna` daemon is running,\nyou have initialized the payment driver with `yagna payment init --sender`,\nand that you have set the `YAGNA_APPKEY` environment variable.\n\nThen run:\n\n```bash\ndapp-manager start --config sample_config.yml dapp-store/apps/webapp.yaml\n```\n\nThe app is started in a background `dapp-runner` process, and you\'re returned an application ID in\nthe form of a hexadecimal string. You can use this ID to query the state and other output streams\nusing `dapp-manager`\'s `read` command, e.g.:\n\n```bash\ndapp-manager read <the-hex-string> state\n```\n\nwill display the contents of the `state` stream of the running app:\n\n```shell\n{"db": {"0": "pending"}}\n{"db": {"0": "starting"}}\n{"db": {"0": "running"}}\n{"db": {"0": "running"}, "http": {"0": "pending"}}\n{"db": {"0": "running"}, "http": {"0": "starting"}}\n```\n\nIn case something goes amiss, `dapp-manager` will output:\n```App <the-hex-string> is not running.```\n\nWhatever the reason, you can still query the various streams of a terminated dapp by adding the\n`--no-ensure-alive` option, e.g.:\n\n```bash\ndapp-manager read <the-hex-string> --no-ensure-alive stderr\n```\n\n## Full usage\n\n```shell\nUsage: dapp-manager [OPTIONS] COMMAND [ARGS]...\n\nOptions:\n  --help  Show this message and exit.\n\nCommands:\n  autocomplete  Enable CLI shell completion for the given shell.\n  kill          Stop the given app forcibly.\n  list          List known app IDs (both active and dead).\n  prune         Remove data for non-running apps.\n  read          Read output from the given app.\n  start         Start a new app using the provided descriptor and config...\n  stop          Stop the given app gracefully.\n```\n\n### Start\n\nThe `start` command launches a new instance of the `dapp-runner` in a background process and\nreturns the hexadecimal string that is the identifier of the running `dapp-runner` instance.\n\n```shell\nUsage: dapp-manager start [OPTIONS] DESCRIPTORS...\n\n  Start a new app using the provided descriptor and config files.\n\nOptions:\n  -c, --config PATH  Path to the file containing yagna-specific config.\n                     [required]\n  --help             Show this message and exit.\n```\n\nImportantly, it requires a config file which contains the parameters used to connect to the `yagna`\ndaemon and initialize the requestor engine. We\'re providing a default, sample configuration as\n`sample_config.yml` in the root of the `dapp-manager` repository.\n\nOf course, it also requires one or more descriptor files that are used by the `dapp-runner` to\ndeploy the specified applications on Golem.\n\n### Stop / Kill\n\nThe `stop` and `kill` commands terminate the given `dapp-runner` instance, the main difference\nbeing the signal that\'s sent to do that. Essentially, `stop` should be enough and should give the\n`dapp-runner` a chance to shut the app down gracefully, correctly terminating the services,\nclosing the agreements and paying for them.\n\nIn case `stop` is stuck for whatever reason, you might want to resort to `kill` which terminates\nthe `dapp-runner` immediately without allowing for any graceful shutdown.\n\n### List\n\nThe `list` command shows the identifiers of all the previously-started apps, whether they\'re still\nrunning or not.\n\n### Prune\n\n`prune` causes `dapp-manager` to remove the data for those apps that it had previously identified as\ndefunct. Consequently, those apps will no longer appear on the list.\n\nUnless an app has been explicitly stopped with a `stop` or `kill` command, the `dapp-manager`\nwill not purge it until it has had a chance to notice the termination, e.g. by issuing a `read`\ncommand to the defunct app.\n\n### Read\n\nThe `read` command outputs the full contents of the specified stream. There are five streams as\nspecified by the usage below:\n\n```shell\nUsage: dapp-manager read [OPTIONS] APP_ID [state|data|log|stdout|stderr]\n\n  Read output from the given app.\n\nOptions:\n  --ensure-alive / --no-ensure-alive\n  -f, --follow\n  --help                          Show this message and exit.\n```\n\nBy default, the stream will only be output if the app is currently running. Otherwise, you\'ll get\nthe ```App <the-hex-string> is not running.``` message and no stream.\n\nIf you wish to query a stream of a terminated app, add the `--no-ensure-alive` parameter to the\nspecific `read` command.\n\n### Shell completion\n\nThis program supports shell completion for all of its commands, as well as existing dApp IDs (where applicable).\n\nTo enable completion, use the `autocomplete` command with your shell of choice:\n\n* **bash**:\n\n    ```bash\n    dapp-manager autocomplete bash\n    ```\n\n* **zsh**:\n\n    ```bash\n    dapp-manager autocomplete zsh\n    ```\n\n* **fish**:\n\n    ```bash\n    dapp-manager autocomplete fish\n    ```\n\nThe completion functions are defined in `dapp_manager/autocomplete/scripts`.\n\nShould the entrypoint name ever change, those files will need to be updated as well.\n\n**WARNING** Completion will **NOT WORK** when `autocomplete` is invoked with `python -m dapp_manager`.\nOnly the installed entrypoint (i.e. `dapp-manager`) is supported. To have it available, run `poetry install`.\n',
-    'author': 'Golem Factory',
-    'author_email': 'contact@golem.network',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/golemfactory/dapp-manager',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.8,<4.0',
-}
+# Golem dApp Manager
 
+`dapp-manager` is a purposefully minimalistic manager for decentralized applications running on
+Golem. It works together with the [dapp-runner](https://github.com/golemfactory/dapp-runner/).
+While the responsibility of the latter is to run a single Golem application, `dapp-manager` takes
+care of spawning, interacting with, and stopping the running instances of the `dapp-runner`.
+
+## Quick start
+
+### Yagna daemon
+
+As the `dapp-manager` uses the `dapp-runner`, which in turn requires a properly configured
+[yagna](https://github.com/golemfactory/yagna) daemon, you'll need to have it set up.
+
+For now, please follow the ["Requestor development: a quick primer"](https://handbook.golem.network/requestor-tutorials/flash-tutorial-of-requestor-development)
+tutorial and ensure that your `yagna` is up and running. Only the first part of this
+tutorial is required - you don't need to run the blender example.
+
+Most importantly, make sure you have set the `YAGNA_APPKEY` in your environment, e.g. with:
+
+```bash
+export YAGNA_APPKEY=insert-your-32-char-app-key-here
+```
+
+or, on Windows:
+
+```bash
+set YAGNA_APPKEY=insert-your-32-char-app-key-here
+```
+
+and if you don't know what your app-key is, you can always query `yagna` with:
+
+```bash
+yagna app-key list
+```
+
+### Python environment
+
+First, ensure you have Python 3.8 or later:
+
+```bash
+python3 --version
+```
+
+[ depending on the platform, it may be just `python` instead of `python3` ]
+
+If your Python version is older, consider using [pyenv](https://github.com/pyenv/pyenv-installer).
+
+Once your python interpreter reports a version 3.8 or later, you can set up your virtual
+environment:
+
+```bash
+python3 -m venv ~/.envs/dapp-manager
+source ~/.envs/dapp-manager/bin/activate
+```
+
+or, if you're on Windows:
+
+```shell
+python -m venv --clear %HOMEDRIVE%%HOMEPATH%\.envs\dapp-manager
+%HOMEDRIVE%%HOMEPATH%\.envs\dapp-manager\Scripts\activate.bat
+```
+
+### DApp manager
+
+#### Clone the repository
+
+```bash
+git clone --recurse-submodules https://github.com/golemfactory/dapp-manager.git
+```
+
+#### Install the dependencies
+
+```bash
+cd dapp-manager
+pip install -U pip poetry
+poetry install
+```
+
+#### Run an example application
+
+Make sure your `yagna` daemon is running,
+you have initialized the payment driver with `yagna payment init --sender`,
+and that you have set the `YAGNA_APPKEY` environment variable.
+
+Then run:
+
+```bash
+dapp-manager start --config sample_config.yml dapp-store/apps/webapp.yaml
+```
+
+The app is started in a background `dapp-runner` process, and you're returned an application ID in
+the form of a hexadecimal string. You can use this ID to query the state and other output streams
+using `dapp-manager`'s `read` command, e.g.:
+
+```bash
+dapp-manager read <the-hex-string> state
+```
+
+will display the contents of the `state` stream of the running app:
+
+```shell
+{"db": {"0": "pending"}}
+{"db": {"0": "starting"}}
+{"db": {"0": "running"}}
+{"db": {"0": "running"}, "http": {"0": "pending"}}
+{"db": {"0": "running"}, "http": {"0": "starting"}}
+```
+
+In case something goes amiss, `dapp-manager` will output:
+```App <the-hex-string> is not running.```
+
+Whatever the reason, you can still query the various streams of a terminated dapp by adding the
+`--no-ensure-alive` option, e.g.:
+
+```bash
+dapp-manager read <the-hex-string> --no-ensure-alive stderr
+```
+
+## Full usage
+
+```shell
+Usage: dapp-manager [OPTIONS] COMMAND [ARGS]...
+
+Options:
+  --help  Show this message and exit.
+
+Commands:
+  autocomplete  Enable CLI shell completion for the given shell.
+  kill          Stop the given app forcibly.
+  list          List known app IDs (both active and dead).
+  prune         Remove data for non-running apps.
+  read          Read output from the given app.
+  start         Start a new app using the provided descriptor and config...
+  stop          Stop the given app gracefully.
+```
+
+### Start
+
+The `start` command launches a new instance of the `dapp-runner` in a background process and
+returns the hexadecimal string that is the identifier of the running `dapp-runner` instance.
+
+```shell
+Usage: dapp-manager start [OPTIONS] DESCRIPTORS...
+
+  Start a new app using the provided descriptor and config files.
+
+Options:
+  -c, --config PATH  Path to the file containing yagna-specific config.
+                     [required]
+  --help             Show this message and exit.
+```
+
+Importantly, it requires a config file which contains the parameters used to connect to the `yagna`
+daemon and initialize the requestor engine. We're providing a default, sample configuration as
+`sample_config.yml` in the root of the `dapp-manager` repository.
+
+Of course, it also requires one or more descriptor files that are used by the `dapp-runner` to
+deploy the specified applications on Golem.
+
+### Stop / Kill
+
+The `stop` and `kill` commands terminate the given `dapp-runner` instance, the main difference
+being the signal that's sent to do that. Essentially, `stop` should be enough and should give the
+`dapp-runner` a chance to shut the app down gracefully, correctly terminating the services,
+closing the agreements and paying for them.
+
+In case `stop` is stuck for whatever reason, you might want to resort to `kill` which terminates
+the `dapp-runner` immediately without allowing for any graceful shutdown.
+
+### List
+
+The `list` command shows the identifiers of all the previously-started apps, whether they're still
+running or not.
+
+### Prune
+
+`prune` causes `dapp-manager` to remove the data for those apps that it had previously identified as
+defunct. Consequently, those apps will no longer appear on the list.
+
+Unless an app has been explicitly stopped with a `stop` or `kill` command, the `dapp-manager`
+will not purge it until it has had a chance to notice the termination, e.g. by issuing a `read`
+command to the defunct app.
+
+### Read
+
+The `read` command outputs the full contents of the specified stream. There are five streams as
+specified by the usage below:
+
+```shell
+Usage: dapp-manager read [OPTIONS] APP_ID [state|data|log|stdout|stderr]
+
+  Read output from the given app.
+
+Options:
+  --ensure-alive / --no-ensure-alive
+  -f, --follow
+  --help                          Show this message and exit.
+```
+
+By default, the stream will only be output if the app is currently running. Otherwise, you'll get
+the ```App <the-hex-string> is not running.``` message and no stream.
+
+If you wish to query a stream of a terminated app, add the `--no-ensure-alive` parameter to the
+specific `read` command.
+
+### Shell completion
+
+This program supports shell completion for all of its commands, as well as existing dApp IDs (where applicable).
+
+To enable completion, use the `autocomplete` command with your shell of choice:
+
+* **bash**:
+
+    ```bash
+    dapp-manager autocomplete bash
+    ```
+
+* **zsh**:
+
+    ```bash
+    dapp-manager autocomplete zsh
+    ```
+
+* **fish**:
+
+    ```bash
+    dapp-manager autocomplete fish
+    ```
+
+The completion functions are defined in `dapp_manager/autocomplete/scripts`.
+
+Should the entrypoint name ever change, those files will need to be updated as well.
+
+**WARNING** Completion will **NOT WORK** when `autocomplete` is invoked with `python -m dapp_manager`.
+Only the installed entrypoint (i.e. `dapp-manager`) is supported. To have it available, run `poetry install`.
 
-setup(**setup_kwargs)
```

