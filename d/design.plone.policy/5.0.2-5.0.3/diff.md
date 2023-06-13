# Comparing `tmp/design.plone.policy-5.0.2.tar.gz` & `tmp/design.plone.policy-5.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "design.plone.policy-5.0.2.tar", last modified: Tue May  9 14:20:42 2023, max compression
+gzip compressed data, was "design.plone.policy-5.0.3.tar", last modified: Tue Jun 13 12:52:49 2023, max compression
```

## Comparing `design.plone.policy-5.0.2.tar` & `design.plone.policy-5.0.3.tar`

### file list

```diff
@@ -1,89 +1,90 @@
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5261 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/CHANGES.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       73 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/CONTRIBUTORS.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      585 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/DEVELOP.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    18092 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/LICENSE.GPL
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      670 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/LICENSE.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      107 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/MANIFEST.in
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    15494 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     9030 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/README.rst
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/docs/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     7993 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/docs/conf.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/docs/index.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       31 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/requirements.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      367 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/setup.cfg
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2887 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/setup.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/src/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/src/design/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/src/design/plone/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       80 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/src/design/plone/policy/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      173 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/browser/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      119 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/browser/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    19901 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/browser/config.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      540 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/browser/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5622 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/browser/trasparenza.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1623 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      441 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/interfaces.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/locales/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      611 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/locales/README.rst
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/locales/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/locales/design.plone.policy.pot
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/src/design/plone/policy/locales/en/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/locales/en/LC_MESSAGES/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.po
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1748 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/locales/update.py
--rwxrwxr-x   0 mauro     (1000) mauro     (1000)      494 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/locales/update.sh
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      273 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/permissions.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/src/design/plone/policy/profiles/
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      584 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/actions.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      175 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      122 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/catalog.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1027 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/metadata.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     1473 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/registry.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      341 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/rolemap.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/profiles/to_1400/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      237 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/to_1400/registry.xml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/profiles/uninstall/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      122 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/uninstall/browserlayer.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      268 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/profiles/uninstall/registry.xml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      311 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/rejectanonymous.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/restapi/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/__init__.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/restapi/bandi_search_filters/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/bandi_search_filters/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      534 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      996 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/bandi_search_filters/get.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      288 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/configure.zcml
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/restapi/search_filters/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/search_filters/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      519 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/search_filters/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3831 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/search_filters/get.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/restapi/twitter_feed/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/twitter_feed/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      513 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/twitter_feed/configure.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     6581 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/restapi/twitter_feed/get.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2342 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/sensitive.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3306 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/setuphandlers.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     5214 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/testing.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.847579 design.plone.policy-5.0.2/src/design/plone/policy/tests/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/tests/__init__.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4286 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/tests/test_bandi_search_filters_api.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4324 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/tests/test_initial_structure.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3864 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/tests/test_search_filters_api.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     3720 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/tests/test_setup.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    11068 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/upgrades.py
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     4771 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/upgrades.zcml
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    13116 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design/plone/policy/utils.py
-drwxrwxr-x   0 mauro     (1000) mauro     (1000)        0 2023-05-09 14:20:42.843579 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/
--rw-rw-r--   0 mauro     (1000) mauro     (1000)    15494 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/PKG-INFO
--rw-rw-r--   0 mauro     (1000) mauro     (1000)     2868 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/SOURCES.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/dependency_links.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       40 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/entry_points.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)       20 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/namespace_packages.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        1 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/not-zip-safe
--rw-rw-r--   0 mauro     (1000) mauro     (1000)      504 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/requires.txt
--rw-rw-r--   0 mauro     (1000) mauro     (1000)        7 2023-05-09 14:20:42.000000 design.plone.policy-5.0.2/src/design.plone.policy.egg-info/top_level.txt
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.886366 design.plone.policy-5.0.3/
+-rw-r--r--   0 cekk       (501) staff       (20)     5447 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/CHANGES.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       73 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/CONTRIBUTORS.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      585 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/DEVELOP.rst
+-rw-r--r--   0 cekk       (501) staff       (20)    18092 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/LICENSE.GPL
+-rw-r--r--   0 cekk       (501) staff       (20)      670 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/LICENSE.rst
+-rw-r--r--   0 cekk       (501) staff       (20)      139 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/MANIFEST.in
+-rw-r--r--   0 cekk       (501) staff       (20)    20651 2023-06-13 12:52:49.886753 design.plone.policy-5.0.3/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     9030 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/README.rst
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.868979 design.plone.policy-5.0.3/docs/
+-rw-r--r--   0 cekk       (501) staff       (20)     7993 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/docs/conf.py
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/docs/index.rst
+-rw-r--r--   0 cekk       (501) staff       (20)       31 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/requirements.txt
+-rw-r--r--   0 cekk       (501) staff       (20)      367 2023-06-13 12:52:49.887373 design.plone.policy-5.0.3/setup.cfg
+-rw-r--r--   0 cekk       (501) staff       (20)     2887 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/setup.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.863187 design.plone.policy-5.0.3/src/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.869273 design.plone.policy-5.0.3/src/design/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.871845 design.plone.policy-5.0.3/src/design/plone/
+-rw-r--r--   0 cekk       (501) staff       (20)       80 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.875266 design.plone.policy-5.0.3/src/design/plone/policy/
+-rw-r--r--   0 cekk       (501) staff       (20)      173 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.876644 design.plone.policy-5.0.3/src/design/plone/policy/browser/
+-rw-r--r--   0 cekk       (501) staff       (20)      119 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/browser/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)    19901 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/browser/config.py
+-rw-r--r--   0 cekk       (501) staff       (20)      540 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/browser/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     5622 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/browser/trasparenza.py
+-rw-r--r--   0 cekk       (501) staff       (20)     1623 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      441 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/interfaces.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.877985 design.plone.policy-5.0.3/src/design/plone/policy/locales/
+-rw-r--r--   0 cekk       (501) staff       (20)      611 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/locales/README.rst
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/locales/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/locales/design.plone.policy.pot
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.864024 design.plone.policy-5.0.3/src/design/plone/policy/locales/en/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.878687 design.plone.policy-5.0.3/src/design/plone/policy/locales/en/LC_MESSAGES/
+-rw-r--r--   0 cekk       (501) staff       (20)       28 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.mo
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.po
+-rw-r--r--   0 cekk       (501) staff       (20)     1748 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/locales/update.py
+-rwxr-xr-x   0 cekk       (501) staff       (20)      494 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/locales/update.sh
+-rw-r--r--   0 cekk       (501) staff       (20)      273 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/permissions.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.864558 design.plone.policy-5.0.3/src/design/plone/policy/profiles/
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.880369 design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/
+-rw-r--r--   0 cekk       (501) staff       (20)      584 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/actions.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      175 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      122 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/catalog.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     1027 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/metadata.xml
+-rw-r--r--   0 cekk       (501) staff       (20)     1473 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      341 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/rolemap.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.880654 design.plone.policy-5.0.3/src/design/plone/policy/profiles/to_1400/
+-rw-r--r--   0 cekk       (501) staff       (20)      237 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/to_1400/registry.xml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.881407 design.plone.policy-5.0.3/src/design/plone/policy/profiles/uninstall/
+-rw-r--r--   0 cekk       (501) staff       (20)      122 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/uninstall/browserlayer.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      268 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/profiles/uninstall/registry.xml
+-rw-r--r--   0 cekk       (501) staff       (20)      311 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/rejectanonymous.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.881947 design.plone.policy-5.0.3/src/design/plone/policy/restapi/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/__init__.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.882840 design.plone.policy-5.0.3/src/design/plone/policy/restapi/bandi_search_filters/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/bandi_search_filters/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      534 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)      996 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/bandi_search_filters/get.py
+-rw-r--r--   0 cekk       (501) staff       (20)      288 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/configure.zcml
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.883655 design.plone.policy-5.0.3/src/design/plone/policy/restapi/search_filters/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/search_filters/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      519 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/search_filters/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     3831 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/search_filters/get.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.884602 design.plone.policy-5.0.3/src/design/plone/policy/restapi/twitter_feed/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/twitter_feed/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)      513 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/twitter_feed/configure.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)     6581 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/restapi/twitter_feed/get.py
+-rw-r--r--   0 cekk       (501) staff       (20)     2342 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/sensitive.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3306 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/setuphandlers.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5214 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/testing.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.886142 design.plone.policy-5.0.3/src/design/plone/policy/tests/
+-rw-r--r--   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/tests/__init__.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4286 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/tests/test_bandi_search_filters_api.py
+-rw-r--r--   0 cekk       (501) staff       (20)     4625 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/tests/test_initial_structure.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3864 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/tests/test_search_filters_api.py
+-rw-r--r--   0 cekk       (501) staff       (20)     3720 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/tests/test_setup.py
+-rw-r--r--   0 cekk       (501) staff       (20)    12447 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/upgrades.py
+-rw-r--r--   0 cekk       (501) staff       (20)     5069 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/upgrades.zcml
+-rw-r--r--   0 cekk       (501) staff       (20)    13290 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design/plone/policy/utils.py
+drwxr-xr-x   0 cekk       (501) staff       (20)        0 2023-06-13 12:52:49.871405 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/
+-rw-r--r--   0 cekk       (501) staff       (20)    20651 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/PKG-INFO
+-rw-r--r--   0 cekk       (501) staff       (20)     2938 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/SOURCES.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/dependency_links.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       53 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/entry_points.txt
+-rw-r--r--   0 cekk       (501) staff       (20)       20 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/namespace_packages.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        1 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/not-zip-safe
+-rw-r--r--   0 cekk       (501) staff       (20)      504 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/requires.txt
+-rw-r--r--   0 cekk       (501) staff       (20)        7 2023-06-13 12:52:49.000000 design.plone.policy-5.0.3/src/design.plone.policy.egg-info/top_level.txt
```

### Comparing `design.plone.policy-5.0.2/CHANGES.rst` & `design.plone.policy-5.0.3/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,19 @@
 Changelog
 =========
 
+5.0.3 (2023-06-13)
+------------------
+
+- Fix creation script: now set default blocks and blocks_layout.
+  [cekk]
+- Upgrade-step to fix all contents with broken blocks_layout.
+  [cekk]
+
+
 5.0.2 (2023-05-09)
 ------------------
 
 - Fix setuphandlers' utils for robotframework
   [mamico]
```

### Comparing `design.plone.policy-5.0.2/DEVELOP.rst` & `design.plone.policy-5.0.3/DEVELOP.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/LICENSE.GPL` & `design.plone.policy-5.0.3/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/LICENSE.rst` & `design.plone.policy-5.0.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/README.rst` & `design.plone.policy-5.0.3/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/docs/conf.py` & `design.plone.policy-5.0.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/setup.py` & `design.plone.policy-5.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
         open("CHANGES.rst").read(),
     ]
 )
 
 
 setup(
     name="design.plone.policy",
-    version="5.0.2",
+    version="5.0.3",
     description="Pacchetto per creare un sito Agid su Plone",
     long_description=long_description,
     # Get more from https://pypi.org/classifiers/
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Environment :: Web Environment",
         "Framework :: Plone",
```

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/browser/config.py` & `design.plone.policy-5.0.3/src/design/plone/policy/browser/config.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/browser/configure.zcml` & `design.plone.policy-5.0.3/src/design/plone/policy/browser/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/browser/trasparenza.py` & `design.plone.policy-5.0.3/src/design/plone/policy/browser/trasparenza.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/configure.zcml` & `design.plone.policy-5.0.3/src/design/plone/policy/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/locales/README.rst` & `design.plone.policy-5.0.3/src/design/plone/policy/locales/README.rst`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/locales/update.py` & `design.plone.policy-5.0.3/src/design/plone/policy/locales/update.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/actions.xml` & `design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/actions.xml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/metadata.xml` & `design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/metadata.xml`

 * *Files 1% similar despite different names*

#### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/metadata.xml` & `design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/metadata.xml`

```diff
@@ -1,10 +1,10 @@
 <?xml version="1.0" encoding="utf-8"?>
 <metadata>
-  <version>3002</version>
+  <version>3100</version>
   <dependencies>
     <dependency>profile-plone.restapi:default</dependency>
     <dependency>profile-design.plone.contenttypes:default</dependency>
     <dependency>profile-redturtle.volto:default</dependency>
     <dependency>profile-collective.volto.dropdownmenu:default</dependency>
     <dependency>profile-collective.volto.socialsettings:default</dependency>
     <dependency>profile-collective.volto.secondarymenu:default</dependency>
```

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/profiles/default/registry.xml` & `design.plone.policy-5.0.3/src/design/plone/policy/profiles/default/registry.xml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml` & `design.plone.policy-5.0.3/src/design/plone/policy/restapi/bandi_search_filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/restapi/bandi_search_filters/get.py` & `design.plone.policy-5.0.3/src/design/plone/policy/restapi/bandi_search_filters/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/restapi/search_filters/configure.zcml` & `design.plone.policy-5.0.3/src/design/plone/policy/restapi/search_filters/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/restapi/search_filters/get.py` & `design.plone.policy-5.0.3/src/design/plone/policy/restapi/search_filters/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/restapi/twitter_feed/configure.zcml` & `design.plone.policy-5.0.3/src/design/plone/policy/restapi/twitter_feed/configure.zcml`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/restapi/twitter_feed/get.py` & `design.plone.policy-5.0.3/src/design/plone/policy/restapi/twitter_feed/get.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/sensitive.py` & `design.plone.policy-5.0.3/src/design/plone/policy/sensitive.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/setuphandlers.py` & `design.plone.policy-5.0.3/src/design/plone/policy/setuphandlers.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/testing.py` & `design.plone.policy-5.0.3/src/design/plone/policy/testing.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/tests/test_bandi_search_filters_api.py` & `design.plone.policy-5.0.3/src/design/plone/policy/tests/test_bandi_search_filters_api.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/tests/test_initial_structure.py` & `design.plone.policy-5.0.3/src/design/plone/policy/tests/test_initial_structure.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from design.plone.policy.utils import TASSONOMIA_AMMINISTRAZIONE
 from design.plone.policy.utils import TASSONOMIA_ARGOMENTI
 from design.plone.policy.utils import TASSONOMIA_NEWS
 from design.plone.policy.utils import TASSONOMIA_ORGANI_GOVERNO
 from design.plone.policy.utils import TASSONOMIA_SERVIZI
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
+from plone.restapi.behaviors import IBlocks
 from plone.i18n.normalizer.interfaces import IURLNormalizer
 from zope.component import getUtility
 
 import unittest
 
 
 # TODO: rework tests
@@ -23,15 +24,15 @@
 
         setRoles(self.portal, TEST_USER_ID, ["Manager"])
 
     def normalize_ids(self, string):
         return getUtility(IURLNormalizer).normalize(string)
 
     def check_initial_blocks(self, obj):
-        self.assertEqual(obj.portal_type, "Document")
+        self.assertTrue(IBlocks.providedBy(obj))
         self.assertEqual(len(obj.blocks.values()), 1)
         self.assertEqual(len(obj.blocks_layout["items"]), 1)
 
     def check_children_initial_blocks(self, obj):
         for child in obj.listFolderContents():
             self.check_initial_blocks(child)
 
@@ -104,7 +105,14 @@
             folder.keys(), [self.normalize_ids(x) for x in TASSONOMIA_ARGOMENTI]
         )
         self.assertEqual(folder.portal_type, "Document")
         for child in folder.listFolderContents():
             self.assertEqual(child.portal_type, "Pagina Argomento")
             self.assertEqual(len(child.blocks.values()), 1)
             self.assertEqual(len(child.blocks_layout["items"]), 1)
+
+    def test_enabled_blocks_contents_have_defaults(self):
+        brains = self.portal.portal_catalog(
+            object_provides="plone.restapi.behaviors.IBlocks"
+        )
+        for brain in brains:
+            self.check_initial_blocks(brain.getObject())
```

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/tests/test_search_filters_api.py` & `design.plone.policy-5.0.3/src/design/plone/policy/tests/test_search_filters_api.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/tests/test_setup.py` & `design.plone.policy-5.0.3/src/design/plone/policy/tests/test_setup.py`

 * *Files identical despite different names*

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/upgrades.py` & `design.plone.policy-5.0.3/src/design/plone/policy/upgrades.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 # -*- coding: utf-8 -*-
 from Acquisition import aq_base
 from collective.volto.blocksfield.field import BlocksField
 from copy import deepcopy
 from design.plone.policy.interfaces import IDesignPlonePolicySettings
 from design.plone.policy.setuphandlers import disable_searchable_types
 from design.plone.policy.setuphandlers import set_default_subsite_colors
+from design.plone.policy.utils import create_default_blocks
 from plone import api
 from plone.app.upgrade.utils import installOrReinstallProduct
 from plone.dexterity.utils import iterSchemata
 from plone.registry.interfaces import IRegistry
+from plone.restapi.behaviors import IBlocks
 from Products.CMFPlone.interfaces import IFilterSchema
 from Products.CMFPlone.interfaces import ISelectableConstrainTypes
 from zope.component import getUtility
 from zope.schema import getFields
 
 import json
 import logging
@@ -324,7 +326,41 @@
     )
     context.runImportStepFromProfile(
         "profile-design.plone.contenttypes:default",
         "plone.app.registry",
         run_dependencies=False,
     )
     installOrReinstallProduct(api.portal.get(), "collective.feedback")
+
+
+def to_3100(context):
+    already_modified = []
+    not_modified = []
+    brains = api.content.find(object_provides=IBlocks.__identifier__)
+    tot = len(brains)
+    i = 0
+    for brain in brains:
+        i += 1
+        if i % 1000 == 0:
+            logger.info(f"Progress: {i}/{tot}")
+        item = brain.getObject().aq_base
+        blocks = getattr(item, "blocks", {})
+        blocks_layout = getattr(item, "blocks_layout", {})
+
+        if blocks and blocks_layout == {"items": []}:
+            # case where document has been created without blocks, and has been modified
+            item.blocks_layout = {"items": [x for x in blocks.keys()]}
+            already_modified.append(brain.getPath())
+            continue
+        if not blocks and blocks_layout == {"items": []}:
+            create_default_blocks(item)
+            not_modified.append(brain.getPath())
+
+    if already_modified:
+        logger.info("### Items that were already modified ###")
+        for i, path in enumerate(already_modified):
+            logger.info(f"[{i+1}/{len(already_modified)}] - {path}")
+
+    if not_modified:
+        logger.info("### Items that were not modified ###")
+        for i, path in enumerate(not_modified):
+            logger.info(f"[{i+1}/{len(not_modified)}] - {path}")
```

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/upgrades.zcml` & `design.plone.policy-5.0.3/src/design/plone/policy/upgrades.zcml`

 * *Files 2% similar despite different names*

```diff
@@ -167,8 +167,18 @@
       destination="3002"
       >
     <genericsetup:upgradeStep
         title="Customize Access inactive portal content permission"
         handler=".upgrades.update_rolemap"
         />
   </genericsetup:upgradeSteps>
+  <genericsetup:upgradeSteps
+      profile="design.plone.policy:default"
+      source="3002"
+      destination="3100"
+      >
+    <genericsetup:upgradeStep
+        title="Fix default blocks on pages created with script"
+        handler=".upgrades.to_3100"
+        />
+  </genericsetup:upgradeSteps>
 </configure>
```

### Comparing `design.plone.policy-5.0.2/src/design/plone/policy/utils.py` & `design.plone.policy-5.0.3/src/design/plone/policy/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # -*- coding: utf-8 -*-
 from collective.volto.dropdownmenu.interfaces import IDropDownMenu
 from collective.volto.secondarymenu.interfaces import ISecondaryMenu
 from collective.volto.subfooter.interfaces import ISubfooter
 from plone import api
 from plone.i18n.normalizer.interfaces import IIDNormalizer
+from plone.restapi.behaviors import IBlocks
 from plone.restapi.interfaces import ISerializeToJsonSummary
 from Products.CMFPlone.interfaces import ISelectableConstrainTypes
 from redturtle.voltoplugin.editablefooter.interfaces import IEditableFooterSettings
 from uuid import uuid4
 from zope.component import getMultiAdapter
 from zope.component import getUtility
 from zope.globalrequest import getRequest
@@ -227,28 +228,30 @@
 def restrict_types(context, types):
     constraints = ISelectableConstrainTypes(context)
     constraints.setConstrainTypesMode(1)
     constraints.setLocallyAllowedTypes(types)
 
 
 def create_default_blocks(context):
-    title_uuid = str(uuid4())
-    context.blocks = {title_uuid: {"@type": "title"}}
-    context.blocks_layout = {"items": [title_uuid]}
+    if IBlocks.providedBy(context):
+        title_uuid = str(uuid4())
+        context.blocks = {title_uuid: {"@type": "title"}}
+        context.blocks_layout = {"items": [title_uuid]}
 
 
 def create_footer():
     container = api.portal.get()
     # Generate needed pages
     for item in TASSONOMIA_FOOTER:
         obj = api.content.create(
             container=container,
             type=item.get("type", "Pagina"),
             title=item.get("title", "Titolo"),
         )
+        create_default_blocks(context=obj)
         api.content.transition(obj=obj, transition="publish")
         item["path"] = f"/{obj.getId()}"
         obj.exclude_from_nav = True
         if obj.portal_type == "FaqFolder":
             setattr(obj, "icon", None)
             obj.reindexObject()
         if obj.portal_type == "Link":
@@ -330,14 +333,15 @@
     # generate content for subfooter
     # Generate needed pages
     obj = api.content.create(
         container=container,
         type="Document",
         title="Media Policy",
     )
+    create_default_blocks(context=obj)
     obj.exclude_from_nav = True
     obj.reindexObject()
 
     payload = json.dumps(
         [
             {
                 "rootPath": "/",
```

### Comparing `design.plone.policy-5.0.2/src/design.plone.policy.egg-info/SOURCES.txt` & `design.plone.policy-5.0.3/src/design.plone.policy.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -36,14 +36,15 @@
 src/design/plone/policy/browser/configure.zcml
 src/design/plone/policy/browser/trasparenza.py
 src/design/plone/policy/locales/README.rst
 src/design/plone/policy/locales/__init__.py
 src/design/plone/policy/locales/design.plone.policy.pot
 src/design/plone/policy/locales/update.py
 src/design/plone/policy/locales/update.sh
+src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.mo
 src/design/plone/policy/locales/en/LC_MESSAGES/design.plone.policy.po
 src/design/plone/policy/profiles/default/actions.xml
 src/design/plone/policy/profiles/default/browserlayer.xml
 src/design/plone/policy/profiles/default/catalog.xml
 src/design/plone/policy/profiles/default/metadata.xml
 src/design/plone/policy/profiles/default/registry.xml
 src/design/plone/policy/profiles/default/rolemap.xml
```

