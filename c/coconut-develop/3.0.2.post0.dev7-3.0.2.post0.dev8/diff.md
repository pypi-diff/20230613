# Comparing `tmp/coconut-develop-3.0.2.post0.dev7.tar.gz` & `tmp/coconut-develop-3.0.2.post0.dev8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/coconut-develop-3.0.2.post0.dev7.tar", last modified: Sun Jun 11 23:51:34 2023, max compression
+gzip compressed data, was "dist/coconut-develop-3.0.2.post0.dev8.tar", last modified: Tue Jun 13 09:32:30 2023, max compression
```

## Comparing `coconut-develop-3.0.2.post0.dev7.tar` & `coconut-develop-3.0.2.post0.dev8.tar`

### file list

```diff
@@ -1,111 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/
--rw-r--r--   0 runner    (1001) docker     (122)       63 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)    13803 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/conf.py
--rw-r--r--   0 runner    (1001) docker     (122)      470 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/LICENSE.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/xontrib/
--rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/xontrib/coconut.py
--rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/_coconut/
--rw-r--r--   0 runner    (1001) docker     (122)     4759 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/_coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/_coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/_coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7601 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut_develop.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut_develop.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/setup.py
--rw-r--r--   0 runner    (1001) docker     (122)    65131 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/HELP.md
--rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/FAQ.md
--rw-r--r--   0 runner    (1001) docker     (122)   199842 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/DOCS.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/highlighter.py
--rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/_pyparsing.py
--rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (122)      630 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/convenience.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/__coconut__.py
--rw-r--r--   0 runner    (1001) docker     (122)    15522 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/root.py
--rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/api.pyi
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut_py3/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut_py3/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)    10742 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/root.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut_py/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut_py/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/embed.py
--rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut_py2/
--rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut_py2/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)      783 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut/
--rw-r--r--   0 runner    (1001) docker     (122)      147 2023-06-11 23:51:33.000000 coconut-develop-3.0.2.post0.dev7/coconut/icoconut/coconut/kernel.json
--rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/__coconut__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/main.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/
--rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/mypy.py
--rw-r--r--   0 runner    (1001) docker     (122)    44611 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/command.py
--rw-r--r--   0 runner    (1001) docker     (122)     8489 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/cli.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)      688 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/command.pyi
--rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/watch.py
--rw-r--r--   0 runner    (1001) docker     (122)      778 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/resources/
--rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/resources/zcoconut.pth
--rw-r--r--   0 runner    (1001) docker     (122)    23531 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/command/util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/__main__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11623 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/api.py
--rw-r--r--   0 runner    (1001) docker     (122)      772 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/convenience.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     8406 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/integrations.py
--rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    19564 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/
--rw-r--r--   0 runner    (1001) docker     (122)    35187 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/header.py
--rw-r--r--   0 runner    (1001) docker     (122)    93362 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/grammar.py
--rw-r--r--   0 runner    (1001) docker     (122)    58872 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/matching.py
--rw-r--r--   0 runner    (1001) docker     (122)   196410 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/compiler.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/templates/
--rw-r--r--   0 runner    (1001) docker     (122)   102260 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/templates/header.py_template
--rw-r--r--   0 runner    (1001) docker     (122)      781 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    48882 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/compiler/util.py
--rw-r--r--   0 runner    (1001) docker     (122)    36611 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/constants.py
--rw-r--r--   0 runner    (1001) docker     (122)    11530 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/util.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/
--rw-r--r--   0 runner    (1001) docker     (122)     4577 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/constants_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/
--rw-r--r--   0 runner    (1001) docker     (122)      496 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/runner.coco
--rw-r--r--   0 runner    (1001) docker     (122)      192 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/runnable.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_35/
--rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_35/py35_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_38/
--rw-r--r--   0 runner    (1001) docker     (122)      255 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_38/py38_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_2/
--rw-r--r--   0 runner    (1001) docker     (122)      356 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_2/py2_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_36/
--rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_36/py36_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_sys/
--rw-r--r--   0 runner    (1001) docker     (122)     5206 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/non_strict/
--rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_3/
--rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_3/py3_test.coco
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/
--rw-r--r--   0 runner    (1001) docker     (122)    42163 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/suite.coco
--rw-r--r--   0 runner    (1001) docker     (122)       87 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/__init__.coco
--rw-r--r--   0 runner    (1001) docker     (122)    46282 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/util.coco
--rw-r--r--   0 runner    (1001) docker     (122)    63255 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/primary.coco
--rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/tutorial.coco
--rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/main.coco
--rw-r--r--   0 runner    (1001) docker     (122)     5219 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/specific.coco
--rw-r--r--   0 runner    (1001) docker     (122)    22378 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/src/extras.coco
--rw-r--r--   0 runner    (1001) docker     (122)      786 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    30524 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/coconut/tests/main_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-11 23:51:34.000000 coconut-develop-3.0.2.post0.dev7/__coconut__/
--rw-r--r--   0 runner    (1001) docker     (122)    42392 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/__coconut__/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/__coconut__/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-06-11 22:57:44.000000 coconut-develop-3.0.2.post0.dev7/__coconut__/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/
+-rw-r--r--   0 runner    (1001) docker     (122)       63 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)    13803 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (122)     2305 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      470 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    11358 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/xontrib/
+-rw-r--r--   0 runner    (1001) docker     (122)     1162 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/xontrib/coconut.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3569 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/_coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)     4759 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/_coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/_coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1253 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/_coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7601 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      109 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut_develop.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2315 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut_develop.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2797 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    65131 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/HELP.md
+-rw-r--r--   0 runner    (1001) docker     (122)    11350 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/FAQ.md
+-rw-r--r--   0 runner    (1001) docker     (122)   199842 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/DOCS.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)     4663 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/highlighter.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13505 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/_pyparsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9825 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)      630 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/convenience.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1315 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/__coconut__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15522 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/root.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2842 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/api.pyi
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/icoconut/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/icoconut/coconut_py3/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/icoconut/coconut_py3/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10742 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/icoconut/root.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/icoconut/coconut_py/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/icoconut/coconut_py/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     5621 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/icoconut/embed.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1387 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/icoconut/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/icoconut/coconut_py2/
+-rw-r--r--   0 runner    (1001) docker     (122)      174 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/icoconut/coconut_py2/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)      783 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/icoconut/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/icoconut/coconut/
+-rw-r--r--   0 runner    (1001) docker     (122)      147 2023-06-13 09:32:29.000000 coconut-develop-3.0.2.post0.dev8/coconut/icoconut/coconut/kernel.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1867 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/__coconut__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      956 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     1543 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/main.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/command/
+-rw-r--r--   0 runner    (1001) docker     (122)     2450 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/command/mypy.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44611 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/command/command.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8489 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/command/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/command/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)      688 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/command/command.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)     2177 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/command/watch.py
+-rw-r--r--   0 runner    (1001) docker     (122)      778 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/command/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/command/resources/
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/command/resources/zcoconut.pth
+-rw-r--r--   0 runner    (1001) docker     (122)    23531 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/command/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1210 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11623 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9278 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)      772 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/convenience.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     8406 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1444 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    19564 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/compiler/
+-rw-r--r--   0 runner    (1001) docker     (122)    35145 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/compiler/header.py
+-rw-r--r--   0 runner    (1001) docker     (122)    93362 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/compiler/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (122)    58872 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/compiler/matching.py
+-rw-r--r--   0 runner    (1001) docker     (122)   196410 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/compiler/compiler.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/compiler/templates/
+-rw-r--r--   0 runner    (1001) docker     (122)   102376 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/compiler/templates/header.py_template
+-rw-r--r--   0 runner    (1001) docker     (122)      781 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/compiler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    48880 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/compiler/util.py
+-rw-r--r--   0 runner    (1001) docker     (122)    36611 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11530 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/util.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     4577 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/constants_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1794 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/
+-rw-r--r--   0 runner    (1001) docker     (122)      496 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/runner.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      192 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/runnable.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_35/
+-rw-r--r--   0 runner    (1001) docker     (122)     2751 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_35/py35_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_38/
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_38/py38_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_2/
+-rw-r--r--   0 runner    (1001) docker     (122)      356 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_2/py2_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_36/
+-rw-r--r--   0 runner    (1001) docker     (122)      694 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_36/py36_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_sys/
+-rw-r--r--   0 runner    (1001) docker     (122)     5206 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_sys/target_sys_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/non_strict/
+-rw-r--r--   0 runner    (1001) docker     (122)     2186 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/non_strict/non_strict_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_3/
+-rw-r--r--   0 runner    (1001) docker     (122)     1155 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_3/py3_test.coco
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/agnostic/
+-rw-r--r--   0 runner    (1001) docker     (122)    42163 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/agnostic/suite.coco
+-rw-r--r--   0 runner    (1001) docker     (122)       87 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/agnostic/__init__.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    46282 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/agnostic/util.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    63255 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/agnostic/primary.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    15411 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/agnostic/tutorial.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     3872 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/agnostic/main.coco
+-rw-r--r--   0 runner    (1001) docker     (122)     5219 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/agnostic/specific.coco
+-rw-r--r--   0 runner    (1001) docker     (122)    22378 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/src/extras.coco
+-rw-r--r--   0 runner    (1001) docker     (122)      786 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30524 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/coconut/tests/main_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-06-13 09:32:30.000000 coconut-develop-3.0.2.post0.dev8/__coconut__/
+-rw-r--r--   0 runner    (1001) docker     (122)    42392 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/__coconut__/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/__coconut__/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     1245 2023-06-13 08:35:53.000000 coconut-develop-3.0.2.post0.dev8/__coconut__/__init__.py
```

### Comparing `coconut-develop-3.0.2.post0.dev7/CONTRIBUTING.md` & `coconut-develop-3.0.2.post0.dev8/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/conf.py` & `coconut-develop-3.0.2.post0.dev8/conf.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/LICENSE.txt` & `coconut-develop-3.0.2.post0.dev8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/xontrib/coconut.py` & `coconut-develop-3.0.2.post0.dev8/xontrib/coconut.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/README.rst` & `coconut-develop-3.0.2.post0.dev8/README.rst`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/_coconut/__init__.pyi` & `coconut-develop-3.0.2.post0.dev8/_coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/_coconut/__init__.py` & `coconut-develop-3.0.2.post0.dev8/_coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/PKG-INFO` & `coconut-develop-3.0.2.post0.dev8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coconut-develop
-Version: 3.0.2.post0.dev7
+Version: 3.0.2.post0.dev8
 Summary: Simple, elegant, Pythonic functional programming.
 Home-page: http://coconut-lang.org
 Author: Evan Hubinger
 Author-email: evanjhub@gmail.com
 License: Apache 2.0
 Description: |logo| Coconut
         ==============
```

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut_develop.egg-info/SOURCES.txt` & `coconut-develop-3.0.2.post0.dev8/coconut_develop.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/setup.py` & `coconut-develop-3.0.2.post0.dev8/setup.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/HELP.md` & `coconut-develop-3.0.2.post0.dev8/HELP.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/FAQ.md` & `coconut-develop-3.0.2.post0.dev8/FAQ.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/DOCS.md` & `coconut-develop-3.0.2.post0.dev8/DOCS.md`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/highlighter.py` & `coconut-develop-3.0.2.post0.dev8/coconut/highlighter.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/_pyparsing.py` & `coconut-develop-3.0.2.post0.dev8/coconut/_pyparsing.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/exceptions.py` & `coconut-develop-3.0.2.post0.dev8/coconut/exceptions.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/convenience.pyi` & `coconut-develop-3.0.2.post0.dev8/coconut/convenience.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/__coconut__.py` & `coconut-develop-3.0.2.post0.dev8/coconut/__coconut__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/root.py` & `coconut-develop-3.0.2.post0.dev8/coconut/root.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # -----------------------------------------------------------------------------------------------------------------------
 # VERSION:
 # -----------------------------------------------------------------------------------------------------------------------
 
 VERSION = "3.0.2"
 VERSION_NAME = None
 # False for release, int >= 1 for develop
-DEVELOP = 7
+DEVELOP = 8
 ALPHA = False  # for pre releases rather than post releases
 
 assert DEVELOP is False or DEVELOP >= 1, "DEVELOP must be False or an int >= 1"
 assert DEVELOP or not ALPHA, "alpha releases are only for develop"
 
 # -----------------------------------------------------------------------------------------------------------------------
 # UTILITIES:
```

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/api.pyi` & `coconut-develop-3.0.2.post0.dev8/coconut/api.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/icoconut/root.py` & `coconut-develop-3.0.2.post0.dev8/coconut/icoconut/root.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/icoconut/embed.py` & `coconut-develop-3.0.2.post0.dev8/coconut/icoconut/embed.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/icoconut/__main__.py` & `coconut-develop-3.0.2.post0.dev8/coconut/icoconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/icoconut/__init__.py` & `coconut-develop-3.0.2.post0.dev8/coconut/icoconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/__coconut__.pyi` & `coconut-develop-3.0.2.post0.dev8/coconut/__coconut__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/__init__.pyi` & `coconut-develop-3.0.2.post0.dev8/coconut/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/main.py` & `coconut-develop-3.0.2.post0.dev8/coconut/main.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/command/mypy.py` & `coconut-develop-3.0.2.post0.dev8/coconut/command/mypy.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/command/command.py` & `coconut-develop-3.0.2.post0.dev8/coconut/command/command.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/command/cli.py` & `coconut-develop-3.0.2.post0.dev8/coconut/command/cli.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/command/command.pyi` & `coconut-develop-3.0.2.post0.dev8/coconut/command/command.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/command/watch.py` & `coconut-develop-3.0.2.post0.dev8/coconut/command/watch.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/command/__init__.py` & `coconut-develop-3.0.2.post0.dev8/coconut/command/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/command/util.py` & `coconut-develop-3.0.2.post0.dev8/coconut/command/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/__main__.py` & `coconut-develop-3.0.2.post0.dev8/coconut/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/requirements.py` & `coconut-develop-3.0.2.post0.dev8/coconut/requirements.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/api.py` & `coconut-develop-3.0.2.post0.dev8/coconut/api.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/convenience.py` & `coconut-develop-3.0.2.post0.dev8/coconut/convenience.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/integrations.py` & `coconut-develop-3.0.2.post0.dev8/coconut/integrations.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/__init__.py` & `coconut-develop-3.0.2.post0.dev8/coconut/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/terminal.py` & `coconut-develop-3.0.2.post0.dev8/coconut/terminal.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/compiler/header.py` & `coconut-develop-3.0.2.post0.dev8/coconut/compiler/header.py`

 * *Files 1% similar despite different names*

```diff
@@ -679,23 +679,23 @@
             newline=True,
         ),
         import_asyncio=pycondition(
             (3, 4),
             if_lt='''
 try:
     import trollius as asyncio
-except ImportError as trollius_import_error:
-    class you_need_to_install_trollius{object}:
+except ImportError as trollius_import_err:
+    class you_need_to_install_trollius(_coconut_missing_module):
         __slots__ = ()
         @staticmethod
         def coroutine(func):
             def raise_import_error(*args, **kwargs):
-                raise trollius_import_error
+                raise trollius_import_err
             return raise_import_error
-    asyncio = you_need_to_install_trollius()
+    asyncio = you_need_to_install_trollius(trollius_import_err)
             '''.format(**format_dict),
             if_ge='''
 import asyncio
             ''',
             indent=1,
         ),
         class_amap=pycondition(
@@ -720,18 +720,16 @@
         ),
         maybe_bind_lru_cache=pycondition(
             (3, 2),
             if_lt='''
 try:
     from backports.functools_lru_cache import lru_cache
     functools.lru_cache = lru_cache
-except ImportError:
-    class you_need_to_install_backports_functools_lru_cache{object}:
-        __slots__ = ()
-    functools.lru_cache = you_need_to_install_backports_functools_lru_cache()
+except ImportError as lru_cache_import_err:
+    functools.lru_cache = _coconut_missing_module(lru_cache_import_err)
             '''.format(**format_dict),
             if_ge=None,
             indent=1,
             newline=True,
         ),
         def_multiset_ops=pycondition(
             (3,),
```

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/compiler/grammar.py` & `coconut-develop-3.0.2.post0.dev8/coconut/compiler/grammar.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/compiler/matching.py` & `coconut-develop-3.0.2.post0.dev8/coconut/compiler/matching.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/compiler/compiler.py` & `coconut-develop-3.0.2.post0.dev8/coconut/compiler/compiler.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/compiler/templates/header.py_template` & `coconut-develop-3.0.2.post0.dev8/coconut/compiler/templates/header.py_template`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+class _coconut_missing_module{object}:
+    __slots__ = ("_import_err",)
+    def __init__(self, error):
+        self._import_err = error
+    def __getattr__(self, name):
+        raise self._import_err
 @_coconut_wraps(_coconut_py_super)
 def _coconut_super(type=None, object_or_type=None):
     if type is None:
         if object_or_type is not None:
             raise _coconut.TypeError("invalid use of super()")
         frame = _coconut_sys._getframe(1)
         try:
@@ -15,18 +21,16 @@
 class _coconut{object}:{COMMENT.EVERYTHING_HERE_MUST_BE_COPIED_TO_STUB_FILE}
     import collections, copy, functools, types, itertools, operator, threading, os, warnings, contextlib, traceback, weakref, multiprocessing
     from multiprocessing import dummy as multiprocessing_dummy
 {maybe_bind_lru_cache}{import_copyreg}
 {import_asyncio}
     try:
         import async_generator
-    except ImportError:
-        class you_need_to_install_async_generator{object}:
-            __slots__ = ()
-        async_generator = you_need_to_install_async_generator()
+    except ImportError as async_generator_import_err:
+        async_generator = _coconut_missing_module(async_generator_import_err)
 {import_pickle}
 {import_OrderedDict}
 {import_collections_abc}
     typing = types.ModuleType(_coconut_py_str("typing"))
     try:
         import typing_extensions
     except ImportError:
@@ -41,18 +45,16 @@
     def _typing_getattr(name):
         raise _coconut.AttributeError("typing.%s is not available on the current Python version and couldn't be looked up in typing_extensions; try hiding your typedefs behind an 'if TYPE_CHECKING:' block" % (name,))
     typing.__getattr__ = _typing_getattr
     _typing_getattr = staticmethod(_typing_getattr)
 {set_zip_longest}
     try:
         import numpy
-    except ImportError:
-        class you_need_to_install_numpy{object}:
-            __slots__ = ()
-        numpy = you_need_to_install_numpy()
+    except ImportError as numpy_import_err:
+        numpy = _coconut_missing_module(numpy_import_err)
     else:
         abc.Sequence.register(numpy.ndarray)
     numpy_modules = {numpy_modules}
     pandas_numpy_modules = {pandas_numpy_modules}
     jax_numpy_modules = {jax_numpy_modules}
     tee_type = type(itertools.tee((), 1)[0])
     reiterables = abc.Sequence, abc.Mapping, abc.Set
```

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/compiler/__init__.py` & `coconut-develop-3.0.2.post0.dev8/coconut/compiler/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/compiler/util.py` & `coconut-develop-3.0.2.post0.dev8/coconut/compiler/util.py`

 * *Files 0% similar despite different names*

```diff
@@ -450,15 +450,15 @@
     internal_assert((start is None) == (stop is None), "invalid parse_where results", (start, stop))
     return start is not None
 
 
 def transform(grammar, text, inner=True):
     """Transform text by replacing matches to grammar."""
     with parsing_context(inner):
-        result = add_action(grammar, unpack).parseWithTabs().transformString(text)
+        result = prep_grammar(add_action(grammar, unpack)).transformString(text)
         if result == text:
             result = None
         return result
 
 
 # -----------------------------------------------------------------------------------------------------------------------
 # TARGETS:
```

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/constants.py` & `coconut-develop-3.0.2.post0.dev8/coconut/constants.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/util.py` & `coconut-develop-3.0.2.post0.dev8/coconut/util.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/constants_test.py` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/constants_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/__main__.py` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/__main__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_35/py35_test.coco` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_35/py35_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_36/py36_test.coco` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_36/py36_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_sys/target_sys_test.coco` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_sys/target_sys_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/non_strict/non_strict_test.coco` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/non_strict/non_strict_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/target_3/py3_test.coco` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/target_3/py3_test.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/suite.coco` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/agnostic/suite.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/util.coco` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/agnostic/util.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/primary.coco` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/agnostic/primary.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/tutorial.coco` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/agnostic/tutorial.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/main.coco` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/agnostic/main.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/cocotest/agnostic/specific.coco` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/src/cocotest/agnostic/specific.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/src/extras.coco` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/src/extras.coco`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/__init__.py` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/coconut/tests/main_test.py` & `coconut-develop-3.0.2.post0.dev8/coconut/tests/main_test.py`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/__coconut__/__init__.pyi` & `coconut-develop-3.0.2.post0.dev8/__coconut__/__init__.pyi`

 * *Files identical despite different names*

### Comparing `coconut-develop-3.0.2.post0.dev7/__coconut__/__init__.py` & `coconut-develop-3.0.2.post0.dev8/__coconut__/__init__.py`

 * *Files identical despite different names*

