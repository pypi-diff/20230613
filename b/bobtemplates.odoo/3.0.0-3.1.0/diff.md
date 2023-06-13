# Comparing `tmp/bobtemplates.odoo-3.0.0.tar.gz` & `tmp/bobtemplates.odoo-3.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bobtemplates.odoo-3.0.0.tar", last modified: Wed Dec 14 08:02:17 2022, max compression
+gzip compressed data, was "bobtemplates.odoo-3.1.0.tar", last modified: Tue Jun 13 11:40:11 2023, max compression
```

## Comparing `bobtemplates.odoo-3.0.0.tar` & `bobtemplates.odoo-3.1.0.tar`

### file list

```diff
@@ -1,76 +1,76 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.143549 bobtemplates.odoo-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      345 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.123548 bobtemplates.odoo-3.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.135548 bobtemplates.odoo-3.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      244 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      663 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (123)      423 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/DEVELOP.rst
--rw-r--r--   0 runner    (1001) docker     (123)     7651 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2022-12-14 08:02:17.143549 bobtemplates.odoo-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2592 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.135548 bobtemplates.odoo-3.0.0/bobtemplates/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.135548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.135548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/addon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.135548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/addon/+addon.name+/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/addon/+addon.name+/README.rst.bob
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/addon/+addon.name+/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      722 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/addon/+addon.name+/__openerp__.py.bob
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.135548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/addon/+addon.name+/readme/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/addon/+addon.name+/readme/dummy.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.127548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/addon/+addon.name+/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.139548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/addon/+addon.name+/static/description/
--rw-r--r--   0 runner    (1001) docker     (123)     9455 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/addon/+addon.name+/static/description/icon.png.oca
--rw-r--r--   0 runner    (1001) docker     (123)      806 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/addon/.mrbob.ini
--rw-r--r--   0 runner    (1001) docker     (123)     9790 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/hooks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.139548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/.mrbob.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.139548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/demo/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/demo/+model.name_underscored+.xml.bob
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.139548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/models/
--rw-r--r--   0 runner    (1001) docker     (123)      567 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/models/+model.name_underscored+.py.bob
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.139548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/security/
--rw-r--r--   0 runner    (1001) docker     (123)      899 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/security/+model.name_underscored+.xml.bob
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.139548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/views/
--rw-r--r--   0 runner    (1001) docker     (123)     3257 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/views/+model.name_underscored+.xml.bob
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.139548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/readme/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/readme/.mrbob.ini
--rw-r--r--   0 runner    (1001) docker     (123)      329 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/readme/README.rst.bob
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.139548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/readme/readme/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/readme/readme/dummy.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.139548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/test/
--rw-r--r--   0 runner    (1001) docker     (123)      684 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/test/.mrbob.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.139548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/test/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      734 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/test/tests/+test.name_underscored+.py.bob
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.139548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/wizard/
--rw-r--r--   0 runner    (1001) docker     (123)     1196 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/wizard/.mrbob.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.139548 bobtemplates.odoo-3.0.0/bobtemplates/odoo/wizard/wizards/
--rw-r--r--   0 runner    (1001) docker     (123)      946 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/wizard/wizards/+wizard.name_underscored+.py.bob
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/bobtemplates/odoo/wizard/wizards/+wizard.name_underscored+.xml.bob
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.135548 bobtemplates.odoo-3.0.0/bobtemplates.odoo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6818 2022-12-14 08:02:17.000000 bobtemplates.odoo-3.0.0/bobtemplates.odoo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1861 2022-12-14 08:02:17.000000 bobtemplates.odoo-3.0.0/bobtemplates.odoo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-14 08:02:17.000000 bobtemplates.odoo-3.0.0/bobtemplates.odoo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-14 08:02:17.000000 bobtemplates.odoo-3.0.0/bobtemplates.odoo.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-14 08:02:17.000000 bobtemplates.odoo-3.0.0/bobtemplates.odoo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2022-12-14 08:02:17.000000 bobtemplates.odoo-3.0.0/bobtemplates.odoo.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-14 08:02:17.143549 bobtemplates.odoo-3.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:17.143549 bobtemplates.odoo-3.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/tests/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      225 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/tests/test_odoo_addon_answers.ini
--rw-r--r--   0 runner    (1001) docker     (123)      225 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/tests/test_odoo_addon_no_readme_answers.ini
--rw-r--r--   0 runner    (1001) docker     (123)      225 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/tests/test_odoo_addon_oca_answers.ini
--rw-r--r--   0 runner    (1001) docker     (123)      225 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/tests/test_odoo_addon_oca_no_readme_answers.ini
--rw-r--r--   0 runner    (1001) docker     (123)      246 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/tests/test_odoo_model_answers.ini
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/tests/test_odoo_readme_answers.ini
--rw-r--r--   0 runner    (1001) docker     (123)       94 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/tests/test_odoo_readme_oca_answers.ini
--rw-r--r--   0 runner    (1001) docker     (123)      148 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/tests/test_odoo_test_answers.ini
--rw-r--r--   0 runner    (1001) docker     (123)      222 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/tests/test_odoo_wizard_answers.ini
--rw-r--r--   0 runner    (1001) docker     (123)     5564 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/tests/test_templates.py
--rw-r--r--   0 runner    (1001) docker     (123)      992 2022-12-14 08:02:04.000000 bobtemplates.odoo-3.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.955290 bobtemplates.odoo-3.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      345 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.935290 bobtemplates.odoo-3.1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.943290 bobtemplates.odoo-3.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3719 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/DEVELOP.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     7651 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-06-13 11:40:11.955290 bobtemplates.odoo-3.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2592 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.943290 bobtemplates.odoo-3.1.0/bobtemplates/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.947290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.947290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/addon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.947290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/addon/+addon.name+/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/addon/+addon.name+/README.rst.bob
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/addon/+addon.name+/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      722 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/addon/+addon.name+/__openerp__.py.bob
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.947290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/addon/+addon.name+/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/addon/+addon.name+/readme/dummy.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.939290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/addon/+addon.name+/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.947290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/addon/+addon.name+/static/description/
+-rw-r--r--   0 runner    (1001) docker     (123)     9455 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/addon/+addon.name+/static/description/icon.png.oca
+-rw-r--r--   0 runner    (1001) docker     (123)      806 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/addon/.mrbob.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/hooks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.947290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/.mrbob.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.947290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/demo/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/demo/+model.name_underscored+.xml.bob
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.947290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/models/+model.name_underscored+.py.bob
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.947290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/security/
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/security/+model.name_underscored+.xml.bob
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.951290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/views/
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/views/+model.name_underscored+.xml.bob
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.951290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/readme/.mrbob.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/readme/README.rst.bob
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.951290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/readme/readme/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/readme/readme/dummy.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.951290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/test/
+-rw-r--r--   0 runner    (1001) docker     (123)      684 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/test/.mrbob.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.951290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/test/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/test/tests/+test.name_underscored+.py.bob
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.951290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/wizard/
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/wizard/.mrbob.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.951290 bobtemplates.odoo-3.1.0/bobtemplates/odoo/wizard/wizards/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/wizard/wizards/+wizard.name_underscored+.py.bob
+-rw-r--r--   0 runner    (1001) docker     (123)     3028 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/bobtemplates/odoo/wizard/wizards/+wizard.name_underscored+.xml.bob
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.947290 bobtemplates.odoo-3.1.0/bobtemplates.odoo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6898 2023-06-13 11:40:11.000000 bobtemplates.odoo-3.1.0/bobtemplates.odoo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1861 2023-06-13 11:40:11.000000 bobtemplates.odoo-3.1.0/bobtemplates.odoo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 11:40:11.000000 bobtemplates.odoo-3.1.0/bobtemplates.odoo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 11:40:11.000000 bobtemplates.odoo-3.1.0/bobtemplates.odoo.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-06-13 11:40:11.000000 bobtemplates.odoo-3.1.0/bobtemplates.odoo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-13 11:40:11.000000 bobtemplates.odoo-3.1.0/bobtemplates.odoo.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-13 11:40:11.955290 bobtemplates.odoo-3.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:11.955290 bobtemplates.odoo-3.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/tests/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/tests/test_odoo_addon_answers.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/tests/test_odoo_addon_no_readme_answers.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/tests/test_odoo_addon_oca_answers.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/tests/test_odoo_addon_oca_no_readme_answers.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/tests/test_odoo_model_answers.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/tests/test_odoo_readme_answers.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/tests/test_odoo_readme_oca_answers.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/tests/test_odoo_test_answers.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/tests/test_odoo_wizard_answers.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     5563 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/tests/test_templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      992 2023-06-13 11:40:02.000000 bobtemplates.odoo-3.1.0/tox.ini
```

### Comparing `bobtemplates.odoo-3.0.0/.github/workflows/ci.yml` & `bobtemplates.odoo-3.1.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/.gitignore` & `bobtemplates.odoo-3.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/.pre-commit-config.yaml` & `bobtemplates.odoo-3.1.0/.pre-commit-config.yaml`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 repos:
 - repo: https://github.com/psf/black
-  rev: 22.10.0
+  rev: 23.3.0
   hooks:
   - id: black
 - repo: https://github.com/pre-commit/pre-commit-hooks
-  rev: v4.3.0
+  rev: v4.4.0
   hooks:
   - id: trailing-whitespace
   - id: end-of-file-fixer
   - id: check-yaml
   - id: debug-statements
 - repo: https://github.com/PyCQA/flake8
-  rev: "5.0.4"
+  rev: "6.0.0"
   hooks:
     - id: flake8
       additional_dependencies: ["flake8-bugbear==21.4.3"]
 - repo: https://github.com/asottile/pyupgrade
-  rev: v3.1.0
+  rev: v3.6.0
   hooks:
   - id: pyupgrade
 - repo: https://github.com/asottile/seed-isort-config
   rev: v2.2.0
   hooks:
   - id: seed-isort-config
 - repo: https://github.com/PyCQA/isort
-  rev: 5.10.1
+  rev: 5.12.0
   hooks:
   - id: isort
```

### Comparing `bobtemplates.odoo-3.0.0/CHANGES.rst` & `bobtemplates.odoo-3.1.0/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,19 @@
 Changes
 ~~~~~~~
 
 .. Future (?)
 .. ----------
 .. -
 
+3.1.0 (2023-06-13)
+------------------
+
+- [IMP] Remove view name for Odoo >= 12
+
 3.0.0 (2022-12-14)
 ------------------
 
 - Support python 3.11. Remove support of python 3.6.
 - [IMP] wizard: no api.multi decorator in Odoo >= 13
```

### Comparing `bobtemplates.odoo-3.0.0/LICENSE` & `bobtemplates.odoo-3.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/PKG-INFO` & `bobtemplates.odoo-3.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bobtemplates.odoo
-Version: 3.0.0
+Version: 3.1.0
 Summary: mr.bob templates for Odoo projects
 Home-page: http://github.com/acsone/bobtemplates.odoo
 Author: ACSONE SA/NV
 Author-email: info@acsone.eu
 License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -119,14 +119,19 @@
 Changes
 ~~~~~~~
 
 .. Future (?)
 .. ----------
 .. -
 
+3.1.0 (2023-06-13)
+------------------
+
+- [IMP] Remove view name for Odoo >= 12
+
 3.0.0 (2022-12-14)
 ------------------
 
 - Support python 3.11. Remove support of python 3.6.
 - [IMP] wizard: no api.multi decorator in Odoo >= 13
```

### Comparing `bobtemplates.odoo-3.0.0/README.rst` & `bobtemplates.odoo-3.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates/odoo/addon/+addon.name+/__openerp__.py.bob` & `bobtemplates.odoo-3.1.0/bobtemplates/odoo/addon/+addon.name+/__openerp__.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates/odoo/addon/+addon.name+/static/description/icon.png.oca` & `bobtemplates.odoo-3.1.0/bobtemplates/odoo/addon/+addon.name+/static/description/icon.png.oca`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates/odoo/addon/.mrbob.ini` & `bobtemplates.odoo-3.1.0/bobtemplates/odoo/addon/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates/odoo/hooks.py` & `bobtemplates.odoo-3.1.0/bobtemplates/odoo/hooks.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,14 @@
 def _rm_suffix(suffix, configurator, path):
     path = os.path.join(configurator.target_directory, path)
     assert path.endswith(suffix)
     os.rename(path, path[: -len(suffix)])
 
 
 def _get_oca_readme_fragments(configurator, addon_name):
-
     data = requests.get(OCA_GITHUB_URL).json()
     for node in data:
         if node["type"] != "file":
             continue
         file_name = node["name"]
         file_url = node["download_url"]
         r = requests.get(file_url)
```

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/.mrbob.ini` & `bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/demo/+model.name_underscored+.xml.bob` & `bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/demo/+model.name_underscored+.xml.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/models/+model.name_underscored+.py.bob` & `bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/models/+model.name_underscored+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/security/+model.name_underscored+.xml.bob` & `bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/security/+model.name_underscored+.xml.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates/odoo/model/views/+model.name_underscored+.xml.bob` & `bobtemplates.odoo-3.1.0/bobtemplates/odoo/model/views/+model.name_underscored+.xml.bob`

 * *Files 4% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 <data>
 {{% else %}}
 <odoo>
 {{% endif %}}
 
 {{% if model.view_form %}}
     <record model="ir.ui.view" id="{{{ model.name_underscored }}}_form_view">
+{{% if odoo.version < 12 %}}
         <field name="name">{{{ model.name_dotted }}}.form (in {{{ addon.name }}})</field>
+{{% endif %}}
         <field name="model">{{{ model.name_dotted }}}</field>
 {{% if model.inherit %}}
         <field name="inherit_id" ref="TODO othermodule.form_view"/>
 {{% endif %}}
         <field name="arch" type="xml">
 {{% if not model.inherit %}}
             <form>
@@ -35,15 +37,17 @@
 {{% endif %}}
         </field>
     </record>
 {{% endif %}}
 
 {{% if model.view_search %}}
     <record model="ir.ui.view" id="{{{ model.name_underscored }}}_search_view">
+{{% if odoo.version < 12 %}}
         <field name="name">{{{ model.name_dotted }}}.search (in {{{ addon.name }}})</field>
+{{% endif %}}
         <field name="model">{{{ model.name_dotted }}}</field>
 {{% if model.inherit %}}
         <field name="inherit_id" ref="TODO othermodule.search_view"/>
 {{% endif %}}
         <field name="arch" type="xml">
 {{% if not model.inherit %}}
             <search>
@@ -54,15 +58,17 @@
 {{% endif %}}
         </field>
     </record>
 {{% endif %}}
 
 {{% if model.view_tree %}}
     <record model="ir.ui.view" id="{{{ model.name_underscored }}}_tree_view">
+{{% if odoo.version < 12 %}}
         <field name="name">{{{ model.name_dotted }}}.tree (in {{{ addon.name }}})</field>
+{{% endif %}}
         <field name="model">{{{ model.name_dotted }}}</field>
 {{% if model.inherit %}}
         <field name="inherit_id" ref="TODO othermodule.tree_view"/>
 {{% endif %}}
         <field name="arch" type="xml">
 {{% if not model.inherit %}}
             <tree>
```

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates/odoo/test/.mrbob.ini` & `bobtemplates.odoo-3.1.0/bobtemplates/odoo/test/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates/odoo/test/tests/+test.name_underscored+.py.bob` & `bobtemplates.odoo-3.1.0/bobtemplates/odoo/test/tests/+test.name_underscored+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates/odoo/wizard/.mrbob.ini` & `bobtemplates.odoo-3.1.0/bobtemplates/odoo/wizard/.mrbob.ini`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates/odoo/wizard/wizards/+wizard.name_underscored+.py.bob` & `bobtemplates.odoo-3.1.0/bobtemplates/odoo/wizard/wizards/+wizard.name_underscored+.py.bob`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates/odoo/wizard/wizards/+wizard.name_underscored+.xml.bob` & `bobtemplates.odoo-3.1.0/bobtemplates/odoo/wizard/wizards/+wizard.name_underscored+.xml.bob`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,17 @@
 <data>
 {{% else %}}
 <odoo>
 {{% endif %}}
 
 {{% if wizard.view_form %}}
     <record model="ir.ui.view" id="{{{ wizard.name_underscored }}}_form_view">
+{{% if odoo.version < 12 %}}
         <field name="name">{{{ wizard.name_dotted }}}.form (in {{{ addon.name }}})</field>
+{{% endif %}}
         <field name="model">{{{ wizard.name_dotted }}}</field>
 {{% if wizard.inherit %}}
         <field name="inherit_id" ref="TODO othermodule.wizard"/>
 {{% endif %}}
         <field name="arch" type="xml">
 {{% if not wizard.inherit %}}
             <form string="{{{ wizard.name_camelwords }}}">
```

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates.odoo.egg-info/PKG-INFO` & `bobtemplates.odoo-3.1.0/bobtemplates.odoo.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bobtemplates.odoo
-Version: 3.0.0
+Version: 3.1.0
 Summary: mr.bob templates for Odoo projects
 Home-page: http://github.com/acsone/bobtemplates.odoo
 Author: ACSONE SA/NV
 Author-email: info@acsone.eu
 License: LGPLv3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -119,14 +119,19 @@
 Changes
 ~~~~~~~
 
 .. Future (?)
 .. ----------
 .. -
 
+3.1.0 (2023-06-13)
+------------------
+
+- [IMP] Remove view name for Odoo >= 12
+
 3.0.0 (2022-12-14)
 ------------------
 
 - Support python 3.11. Remove support of python 3.6.
 - [IMP] wizard: no api.multi decorator in Odoo >= 13
```

### Comparing `bobtemplates.odoo-3.0.0/bobtemplates.odoo.egg-info/SOURCES.txt` & `bobtemplates.odoo-3.1.0/bobtemplates.odoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/setup.py` & `bobtemplates.odoo-3.1.0/setup.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/tests/test_hooks.py` & `bobtemplates.odoo-3.1.0/tests/test_hooks.py`

 * *Files identical despite different names*

### Comparing `bobtemplates.odoo-3.0.0/tests/test_templates.py` & `bobtemplates.odoo-3.1.0/tests/test_templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,14 @@
 import tempfile
 import unittest
 
 from scripttest import TestFileEnvironment
 
 
 class BaseTemplateTest(unittest.TestCase):
-
     # credit bobtemplates.plone
 
     def setUp(self):
         self.maxDiff = None
         self.tempdir = tempfile.mkdtemp()
         self.addCleanup(shutil.rmtree, self.tempdir)
```

### Comparing `bobtemplates.odoo-3.0.0/tox.ini` & `bobtemplates.odoo-3.1.0/tox.ini`

 * *Files identical despite different names*

