# Comparing `tmp/hyfi_template-0.3.4.tar.gz` & `tmp/hyfi_template-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_template-0.3.4.tar", max compression
+gzip compressed data, was "hyfi_template-0.3.5.tar", max compression
```

## Comparing `hyfi_template-0.3.4.tar` & `hyfi_template-0.3.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     1071 2023-06-11 10:03:27.804780 hyfi_template-0.3.4/LICENSE
--rw-r--r--   0        0        0     2001 2023-06-11 10:03:27.804780 hyfi_template-0.3.4/README.md
--rw-r--r--   0        0        0     3082 2023-06-11 10:03:51.585006 hyfi_template-0.3.4/pyproject.toml
--rw-r--r--   0        0        0      294 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/__cli__.py
--rw-r--r--   0        0        0      379 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/__init__.py
--rw-r--r--   0        0        0       22 2023-06-11 10:03:51.529006 hyfi_template-0.3.4/src/hyfi_template/_version.py
--rw-r--r--   0        0        0        0 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/__init__.py
--rw-r--r--   0        0        0      257 2023-06-11 10:03:51.529006 hyfi_template-0.3.4/src/hyfi_template/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       83 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/cmd/about.yaml
--rw-r--r--   0        0        0      167 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0      320 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/config.yaml
--rw-r--r--   0        0        0      552 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/copier/conf.yaml
--rw-r--r--   0        0        0      807 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      293 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/conf/project/__init__.yaml
--rw-r--r--   0        0        0        0 2023-06-11 10:03:27.808781 hyfi_template-0.3.4/src/hyfi_template/py.typed
--rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 hyfi_template-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-06-12 22:26:25.087535 hyfi_template-0.3.5/LICENSE
+-rw-r--r--   0        0        0     2215 2023-06-12 22:26:25.087535 hyfi_template-0.3.5/README.md
+-rw-r--r--   0        0        0     3052 2023-06-12 22:26:53.567951 hyfi_template-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/__cli__.py
+-rw-r--r--   0        0        0      379 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/__init__.py
+-rw-r--r--   0        0        0       22 2023-06-12 22:26:53.503950 hyfi_template-0.3.5/src/hyfi_template/_version.py
+-rw-r--r--   0        0        0        0 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/__init__.py
+-rw-r--r--   0        0        0      257 2023-06-12 22:26:53.503950 hyfi_template-0.3.5/src/hyfi_template/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0      320 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/config.yaml
+-rw-r--r--   0        0        0      552 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      701 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      293 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      717 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      496 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/path/__default__.yaml
+-rw-r--r--   0        0        0     1518 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      669 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/conf/project/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-06-12 22:26:25.091534 hyfi_template-0.3.5/src/hyfi_template/py.typed
+-rw-r--r--   0        0        0     2887 1970-01-01 00:00:00.000000 hyfi_template-0.3.5/PKG-INFO
```

### Comparing `hyfi_template-0.3.4/LICENSE` & `hyfi_template-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.3.4/README.md` & `hyfi_template-0.3.5/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,26 @@
 # HyFI Template
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![license-image]][license-url]
 [![jupyter-book-image]][docs-url]
+[![codecov][codecov-image]][codecov-url]
 
 <!-- Links: -->
 [pypi-image]: https://img.shields.io/pypi/v/hyfi-template
 [license-image]: https://img.shields.io/github/license/entelecheia/hyfi-template
 [license-url]: https://github.com/entelecheia/hyfi-template/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyfi-template?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyfi-template
 [release-url]: https://github.com/entelecheia/hyfi-template/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
+[codecov-image]: https://codecov.io/gh/entelecheia/hyfi-template/branch/main/graph/badge.svg?token=CEUCMPZM9F
+[codecov-url]: https://codecov.io/gh/entelecheia/hyfi-template
 
 [repo-url]: https://github.com/entelecheia/hyfi-template
 [pypi-url]: https://pypi.org/project/hyfi-template
 [docs-url]: https://hyfi-template.entelecheia.ai
 [changelog]: https://github.com/entelecheia/hyfi-template/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/hyfi-template/blob/main/CONTRIBUTING.md
 <!-- Links: -->
```

### Comparing `hyfi_template-0.3.4/pyproject.toml` & `hyfi_template-0.3.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "hyfi-template"
-version = "0.3.4"
+version = "0.3.5"
 description = "A GitHub Template Repository for HyFI-based Projects"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-template.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi-template"
 readme = "README.md"
 packages = [{ include = "hyfi_template", from = "src" }]
 
 [tool.poetry.scripts]
 hyfi_template = 'hyfi_template.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = {extras = ["all"], version = "^0.4.0"}
+hyfi = "^0.5.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
```

### Comparing `hyfi_template-0.3.4/src/hyfi_template/conf/copier/conf.yaml` & `hyfi_template-0.3.5/src/hyfi_template/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.3.4/src/hyfi_template/conf/hydra/help/help.yaml` & `hyfi_template-0.3.5/src/hyfi_template/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.3.4/src/hyfi_template/conf/mode/__init__.yaml` & `hyfi_template-0.3.5/src/hyfi_template/conf/mode/__init__.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -7,17 +7,17 @@
 logging_level: ${oc.env:HYFI_LOG_LEVEL,WARNING}
 
 hydra:
   job:
     name: ${project.project_name}
     chdir: true
   run:
-    dir: ${project.path.logs}/hydra/${hydra.job.name}/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
+    dir: ${project.path.project_logs}/hydra/${hydra.job.name}/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
   sweep:
-    dir: ${project.path.logs}/hydra/${hydra.job.name}/multiruns/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
+    dir: ${project.path.project_logs}/hydra/${hydra.job.name}/multiruns/${now:%Y-%m-%d}/${now:%Y-%m-%d_%H-%M-%S}
     subdir: ${hydra.job.num}
   verbose: false
   job_logging:
     handlers:
       console:
         level: ${hydra.job_logging.root.level}
       file:
```

### Comparing `hyfi_template-0.3.4/PKG-INFO` & `hyfi_template-0.3.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 Metadata-Version: 2.1
 Name: hyfi-template
-Version: 0.3.4
+Version: 0.3.5
 Summary: A GitHub Template Repository for HyFI-based Projects
 Home-page: https://hyfi-template.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi[all] (>=0.4.0,<0.5.0)
+Requires-Dist: hyfi (>=0.5.0,<0.6.0)
 Project-URL: Repository, https://github.com/entelecheia/hyfi-template
 Description-Content-Type: text/markdown
 
 # HyFI Template
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
 [![license-image]][license-url]
 [![jupyter-book-image]][docs-url]
+[![codecov][codecov-image]][codecov-url]
 
 <!-- Links: -->
 [pypi-image]: https://img.shields.io/pypi/v/hyfi-template
 [license-image]: https://img.shields.io/github/license/entelecheia/hyfi-template
 [license-url]: https://github.com/entelecheia/hyfi-template/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyfi-template?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyfi-template
 [release-url]: https://github.com/entelecheia/hyfi-template/releases
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
+[codecov-image]: https://codecov.io/gh/entelecheia/hyfi-template/branch/main/graph/badge.svg?token=CEUCMPZM9F
+[codecov-url]: https://codecov.io/gh/entelecheia/hyfi-template
 
 [repo-url]: https://github.com/entelecheia/hyfi-template
 [pypi-url]: https://pypi.org/project/hyfi-template
 [docs-url]: https://hyfi-template.entelecheia.ai
 [changelog]: https://github.com/entelecheia/hyfi-template/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/hyfi-template/blob/main/CONTRIBUTING.md
 <!-- Links: -->
```

