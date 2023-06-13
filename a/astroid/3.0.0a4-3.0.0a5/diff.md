# Comparing `tmp/astroid-3.0.0a4.tar.gz` & `tmp/astroid-3.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astroid-3.0.0a4.tar", last modified: Tue Jun  6 20:01:11 2023, max compression
+gzip compressed data, was "astroid-3.0.0a5.tar", last modified: Tue Jun 13 07:54:08 2023, max compression
```

## Comparing `astroid-3.0.0a4.tar` & `astroid-3.0.0a5.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.654733 astroid-3.0.0a4/
--rw-r--r--   0 runner    (1001) docker     (123)     8055 2023-06-06 20:00:53.000000 astroid-3.0.0a4/CONTRIBUTORS.txt
--rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-06-06 20:00:53.000000 astroid-3.0.0a4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-06 20:00:53.000000 astroid-3.0.0a4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-06 20:01:11.654733 astroid-3.0.0a4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-06 20:00:53.000000 astroid-3.0.0a4/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.638733 astroid-3.0.0a4/astroid/
--rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/__pkginfo__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/_ast.py
--rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/_backport_stdlib_names.py
--rw-r--r--   0 runner    (1001) docker     (123)    12692 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/arguments.py
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/astroid_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    27278 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/bases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.646733 astroid-3.0.0a4/astroid/brain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_argparse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_attrs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_boto3.py
--rw-r--r--   0 runner    (1001) docker     (123)    35752 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_builtin_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_collections.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_crypt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_ctypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_curses.py
--rw-r--r--   0 runner    (1001) docker     (123)    22150 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_dataclasses.py
--rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_dateutil.py
--rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_fstrings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_functools.py
--rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_gi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_hashlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_http.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_hypothesis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_io.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_mechanize.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_multiprocessing.py
--rw-r--r--   0 runner    (1001) docker     (123)    23777 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_namedtuple_enum.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_nose.py
--rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_core_einsumfunc.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_core_fromnumeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_core_function_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_core_multiarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_core_numeric.py
--rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_core_numerictypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_core_umath.py
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_ma.py
--rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_ndarray.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_random_mtrand.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_numpy_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_pkg_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_pytest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_qt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_random.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_re.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_responses.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_scipy_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_six.py
--rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_sqlalchemy.py
--rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_ssl.py
--rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_threading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_type.py
--rw-r--r--   0 runner    (1001) docker     (123)    14690 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_unittest.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/brain_uuid.py
--rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/brain/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    18717 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    45357 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/inference.py
--rw-r--r--   0 runner    (1001) docker     (123)     4468 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/inference_tip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.646733 astroid-3.0.0a4/astroid/interpreter/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/interpreter/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.646733 astroid-3.0.0a4/astroid/interpreter/_import/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/interpreter/_import/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/interpreter/_import/spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/interpreter/_import/util.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/interpreter/dunder_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    34584 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/interpreter/objectmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)    17814 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/mixins.py
--rw-r--r--   0 runner    (1001) docker     (123)    23589 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/modutils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/node_classes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.646733 astroid-3.0.0a4/astroid/nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7355 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/_base_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/as_string.py
--rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/const.py
--rw-r--r--   0 runner    (1001) docker     (123)   132674 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/node_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    27934 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/node_ng.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.646733 astroid-3.0.0a4/astroid/nodes/scoped_nodes/
--rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/scoped_nodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/scoped_nodes/mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)   100971 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/scoped_nodes/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/scoped_nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/nodes/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    32620 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    25022 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/raw_building.py
--rw-r--r--   0 runner    (1001) docker     (123)    69315 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/rebuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/typing.py
--rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-06 20:00:53.000000 astroid-3.0.0a4/astroid/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.638733 astroid-3.0.0a4/astroid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-06 20:01:11.000000 astroid-3.0.0a4/astroid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-06 20:01:11.000000 astroid-3.0.0a4/astroid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-06 20:01:11.000000 astroid-3.0.0a4/astroid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-06 20:01:11.000000 astroid-3.0.0a4/astroid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-06 20:01:11.000000 astroid-3.0.0a4/astroid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-06 20:00:53.000000 astroid-3.0.0a4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-06 20:00:53.000000 astroid-3.0.0a4/requirements_dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-06 20:00:53.000000 astroid-3.0.0a4/requirements_full.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-06 20:00:53.000000 astroid-3.0.0a4/requirements_minimal.txt
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-06 20:01:11.654733 astroid-3.0.0a4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-06 20:01:11.654733 astroid-3.0.0a4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-06 20:00:53.000000 astroid-3.0.0a4/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/resources.py
--rw-r--r--   0 runner    (1001) docker     (123)    34673 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_constraint.py
--rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_decorators.py
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_filter_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_group_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)   221727 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_inference.py
--rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_inference_calls.py
--rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_lookup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)    22524 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_modutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    61209 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)    54462 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_nodes_lineno.py
--rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_nodes_position.py
--rw-r--r--   0 runner    (1001) docker     (123)    27699 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_object_model.py
--rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_protocols.py
--rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_python3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_raw_building.py
--rw-r--r--   0 runner    (1001) docker     (123)    14354 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_regrtest.py
--rw-r--r--   0 runner    (1001) docker     (123)    92790 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_scoped_nodes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_stdlib.py
--rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_transforms.py
--rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-06 20:00:54.000000 astroid-3.0.0a4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.648510 astroid-3.0.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)     8146 2023-06-13 07:53:44.000000 astroid-3.0.0a5/CONTRIBUTORS.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    26516 2023-06-13 07:53:44.000000 astroid-3.0.0a5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-06-13 07:53:44.000000 astroid-3.0.0a5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-13 07:54:08.648510 astroid-3.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-06-13 07:53:44.000000 astroid-3.0.0a5/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.624509 astroid-3.0.0a5/astroid/
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/__pkginfo__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2884 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/_ast.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7026 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/_backport_stdlib_names.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/arguments.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/astroid_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26966 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/bases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.640510 astroid-3.0.0a5/astroid/brain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_argparse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3137 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_attrs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_boto3.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35841 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_builtin_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_collections.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_crypt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2670 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_ctypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3487 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_curses.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22150 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_dataclasses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      777 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_dateutil.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2727 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_fstrings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6232 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_functools.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7553 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_gi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_hashlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10650 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_hypothesis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_mechanize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_multiprocessing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23777 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_namedtuple_enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2349 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_nose.py
+-rw-r--r--   0 runner    (1001) docker     (123)      835 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_core_einsumfunc.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_core_fromnumeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1341 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_core_function_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_core_multiarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_core_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8556 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_core_numerictypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_core_umath.py
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_ma.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9008 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_ndarray.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_random_mtrand.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_numpy_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2210 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_pkg_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2233 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_pytest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_qt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3128 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_re.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_responses.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2286 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_scipy_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3890 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7604 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_six.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1019 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_sqlalchemy.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6512 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_ssl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3006 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_threading.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14690 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_unittest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/brain_uuid.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/brain/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18824 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6324 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13127 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9401 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11457 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45357 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/inference_tip.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.640510 astroid-3.0.0a5/astroid/interpreter/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/interpreter/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.640510 astroid-3.0.0a5/astroid/interpreter/_import/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/interpreter/_import/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16576 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/interpreter/_import/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/interpreter/_import/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2515 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/interpreter/dunder_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34584 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/interpreter/objectmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18176 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/mixins.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23616 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/node_classes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.640510 astroid-3.0.0a5/astroid/nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     4910 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7407 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/_base_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25053 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/as_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)      807 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)   132674 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/node_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28138 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/node_ng.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.644510 astroid-3.0.0a5/astroid/nodes/scoped_nodes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1229 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/scoped_nodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7106 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/scoped_nodes/mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   101119 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/scoped_nodes/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1181 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/scoped_nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/nodes/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13447 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32620 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25341 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    69315 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/rebuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      968 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2444 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5365 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/typing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3870 2023-06-13 07:53:44.000000 astroid-3.0.0a5/astroid/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.628509 astroid-3.0.0a5/astroid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4369 2023-06-13 07:54:08.000000 astroid-3.0.0a5/astroid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3953 2023-06-13 07:54:08.000000 astroid-3.0.0a5/astroid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-13 07:54:08.000000 astroid-3.0.0a5/astroid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-06-13 07:54:08.000000 astroid-3.0.0a5/astroid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-13 07:54:08.000000 astroid-3.0.0a5/astroid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3213 2023-06-13 07:53:44.000000 astroid-3.0.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-06-13 07:53:44.000000 astroid-3.0.0a5/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-06-13 07:53:44.000000 astroid-3.0.0a5/requirements_full.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-06-13 07:53:44.000000 astroid-3.0.0a5/requirements_minimal.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-06-13 07:54:08.648510 astroid-3.0.0a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-13 07:54:08.648510 astroid-3.0.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2051 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34673 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15619 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3809 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_decorators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_filter_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3625 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_group_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9350 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)   223086 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_inference.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14712 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_inference_calls.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34833 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_lookup.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19676 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22658 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_modutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    62072 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54462 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_nodes_lineno.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4167 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_nodes_position.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27699 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_object_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21338 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14488 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_protocols.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14453 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_python3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5826 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_raw_building.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15110 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_regrtest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    92790 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_scoped_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_stdlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8969 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_transforms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6459 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-13 07:53:44.000000 astroid-3.0.0a5/tox.ini
```

### Comparing `astroid-3.0.0a4/CONTRIBUTORS.txt` & `astroid-3.0.0a5/CONTRIBUTORS.txt`

 * *Files 1% similar despite different names*

```diff
@@ -133,14 +133,15 @@
 - Michał Masłowski <m.maslowski@clearcode.cc>
 - Mateusz Bysiek <mb@mbdev.pl>
 - Leandro T. C. Melo <ltcmelo@gmail.com>
 - Konrad Weihmann <kweihmann@outlook.com>
 - Kian Meng, Ang <kianmeng.ang@gmail.com>
 - Kai Mueller <15907922+kasium@users.noreply.github.com>
 - Jörg Thalheim <Mic92@users.noreply.github.com>
+- Josef Kemetmüller <josef.kemetmueller@gmail.com>
 - Jonathan Striebel <jstriebel@users.noreply.github.com>
 - John Belmonte <john@neggie.net>
 - Jeff Widman <jeff@jeffwidman.com>
 - Jeff Quast <contact@jeffquast.com>
 - Jarrad Hope <me@jarradhope.com>
 - Jared Garst <jgarst@users.noreply.github.com>
 - Jakub Wilk <jwilk@jwilk.net>
@@ -178,14 +179,15 @@
 - Batuhan Taskaya <isidentical@gmail.com>
 - BasPH <BasPH@users.noreply.github.com>
 - Azeem Bande-Ali <A.BandeAli@gmail.com>
 - Avram Lubkin <aviso@rockhopper.net>
 - Aru Sahni <arusahni@gmail.com>
 - Artsiom Kaval <lezeroq@gmail.com>
 - Anubhav <35621759+anubh-v@users.noreply.github.com>
+- Antonio <antonioglez-23@hotmail.com>
 - Antoine Boellinger <aboellinger@hotmail.com>
 - Alphadelta14 <alpha@alphaservcomputing.solutions>
 - Alexander Scheel <alexander.m.scheel@gmail.com>
 - Alexander Presnyakov <flagist0@gmail.com>
 - Ahmed Azzaoui <ahmed.azzaoui@engie.com>
 
 Co-Author
```

### Comparing `astroid-3.0.0a4/LICENSE` & `astroid-3.0.0a5/LICENSE`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/PKG-INFO` & `astroid-3.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.0.0a4
+Version: 3.0.0a5
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
```

### Comparing `astroid-3.0.0a4/README.rst` & `astroid-3.0.0a5/README.rst`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/__init__.py` & `astroid-3.0.0a5/astroid/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/_ast.py` & `astroid-3.0.0a5/astroid/_ast.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/_backport_stdlib_names.py` & `astroid-3.0.0a5/astroid/_backport_stdlib_names.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/arguments.py` & `astroid-3.0.0a5/astroid/arguments.py`

 * *Files 0% similar despite different names*

```diff
@@ -211,15 +211,15 @@
 
                 if isinstance(boundnode, nodes.ClassDef):
                     # Verify that we're accessing a method
                     # of the metaclass through a class, as in
                     # `cls.metaclass_method`. In this case, the
                     # first argument is always the class.
                     method_scope = funcnode.parent.scope()
-                    if method_scope is boundnode.metaclass():
+                    if method_scope is boundnode.metaclass(context=context):
                         return iter((boundnode,))
 
                 if funcnode.type == "method":
                     if not isinstance(boundnode, Instance):
                         boundnode = boundnode.instantiate_class()
                     return iter((boundnode,))
                 if funcnode.type == "classmethod":
```

### Comparing `astroid-3.0.0a4/astroid/astroid_manager.py` & `astroid-3.0.0a5/astroid/astroid_manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/bases.py` & `astroid-3.0.0a5/astroid/bases.py`

 * *Files 1% similar despite different names*

```diff
@@ -273,22 +273,14 @@
         self, name: str, context: InferenceContext | None = None
     ) -> Iterator[InferenceResult]:
         """Inferred getattr."""
         if not context:
             context = InferenceContext()
         try:
             context.lookupname = name
-            # avoid recursively inferring the same attr on the same class
-            if context.push(self._proxied):
-                raise InferenceError(
-                    message="Cannot infer the same attribute again",
-                    node=self,
-                    context=context,
-                )
-
             # XXX frame should be self._proxied, or not ?
             get_attr = self.getattr(name, context, lookupclass=False)
             yield from _infer_stmts(
                 self._wrap_attr(get_attr, context), context, frame=self
             )
         except AttributeInferenceError:
             try:
```

### Comparing `astroid-3.0.0a4/astroid/brain/brain_argparse.py` & `astroid-3.0.0a5/astroid/brain/brain_argparse.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_attrs.py` & `astroid-3.0.0a5/astroid/brain/brain_attrs.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_boto3.py` & `astroid-3.0.0a5/astroid/brain/brain_boto3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_builtin_inference.py` & `astroid-3.0.0a5/astroid/brain/brain_builtin_inference.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,20 +125,22 @@
 
 def _extend_builtins(class_transforms):
     builtin_ast = AstroidManager().builtins_module
     for class_name, transform in class_transforms.items():
         transform(builtin_ast[class_name])
 
 
-_extend_builtins(
-    {
-        "bytes": partial(_extend_string_class, code=BYTES_CLASS, rvalue="b''"),
-        "str": partial(_extend_string_class, code=STR_CLASS, rvalue="''"),
-    }
-)
+def on_bootstrap():
+    """Called by astroid_bootstrapping()."""
+    _extend_builtins(
+        {
+            "bytes": partial(_extend_string_class, code=BYTES_CLASS, rvalue="b''"),
+            "str": partial(_extend_string_class, code=STR_CLASS, rvalue="''"),
+        }
+    )
 
 
 def _builtin_filter_predicate(node, builtin_name) -> bool:
     if (
         builtin_name == "type"
         and node.root().name == "re"
         and isinstance(node.func, nodes.Name)
```

### Comparing `astroid-3.0.0a4/astroid/brain/brain_collections.py` & `astroid-3.0.0a5/astroid/brain/brain_collections.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_crypt.py` & `astroid-3.0.0a5/astroid/brain/brain_crypt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_ctypes.py` & `astroid-3.0.0a5/astroid/brain/brain_ctypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_curses.py` & `astroid-3.0.0a5/astroid/brain/brain_curses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_dataclasses.py` & `astroid-3.0.0a5/astroid/brain/brain_dataclasses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_dateutil.py` & `astroid-3.0.0a5/astroid/brain/brain_dateutil.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_fstrings.py` & `astroid-3.0.0a5/astroid/brain/brain_fstrings.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_functools.py` & `astroid-3.0.0a5/astroid/brain/brain_functools.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_gi.py` & `astroid-3.0.0a5/astroid/brain/brain_gi.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_hashlib.py` & `astroid-3.0.0a5/astroid/brain/brain_hashlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_http.py` & `astroid-3.0.0a5/astroid/brain/brain_http.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_hypothesis.py` & `astroid-3.0.0a5/astroid/brain/brain_hypothesis.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_io.py` & `astroid-3.0.0a5/astroid/brain/brain_io.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_mechanize.py` & `astroid-3.0.0a5/astroid/brain/brain_mechanize.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_multiprocessing.py` & `astroid-3.0.0a5/astroid/brain/brain_multiprocessing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_namedtuple_enum.py` & `astroid-3.0.0a5/astroid/brain/brain_namedtuple_enum.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_nose.py` & `astroid-3.0.0a5/astroid/brain/brain_nose.py`

 * *Files 16% similar despite different names*

```diff
@@ -3,32 +3,31 @@
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Hooks for nose library."""
 
 import re
 import textwrap
 
-import astroid.builder
+from astroid.bases import BoundMethod
 from astroid.brain.helpers import register_module_extender
+from astroid.builder import AstroidBuilder
 from astroid.exceptions import InferenceError
 from astroid.manager import AstroidManager
-
-_BUILDER = astroid.builder.AstroidBuilder(AstroidManager())
-
+from astroid.nodes import List, Module
 
 CAPITALS = re.compile("([A-Z])")
 
 
 def _pep8(name, caps=CAPITALS):
     return caps.sub(lambda m: "_" + m.groups()[0].lower(), name)
 
 
 def _nose_tools_functions():
     """Get an iterator of names and bound methods."""
-    module = _BUILDER.string_build(
+    module = AstroidBuilder().string_build(
         textwrap.dedent(
             """
     import unittest
 
     class Test(unittest.TestCase):
         pass
     a = Test()
@@ -38,42 +37,42 @@
     try:
         case = next(module["a"].infer())
     except (InferenceError, StopIteration):
         return
     for method in case.methods():
         if method.name.startswith("assert") and "_" not in method.name:
             pep8_name = _pep8(method.name)
-            yield pep8_name, astroid.BoundMethod(method, case)
+            yield pep8_name, BoundMethod(method, case)
         if method.name == "assertEqual":
             # nose also exports assert_equals.
-            yield "assert_equals", astroid.BoundMethod(method, case)
+            yield "assert_equals", BoundMethod(method, case)
 
 
 def _nose_tools_transform(node):
     for method_name, method in _nose_tools_functions():
         node.locals[method_name] = [method]
 
 
 def _nose_tools_trivial_transform():
     """Custom transform for the nose.tools module."""
-    stub = _BUILDER.string_build("""__all__ = []""")
+    stub = AstroidBuilder().string_build("""__all__ = []""")
     all_entries = ["ok_", "eq_"]
 
     for pep8_name, method in _nose_tools_functions():
         all_entries.append(pep8_name)
         stub[pep8_name] = method
 
     # Update the __all__ variable, since nose.tools
     # does this manually with .append.
     all_assign = stub["__all__"].parent
-    all_object = astroid.List(all_entries)
+    all_object = List(all_entries)
     all_object.parent = all_assign
     all_assign.value = all_object
     return stub
 
 
 register_module_extender(
     AstroidManager(), "nose.tools.trivial", _nose_tools_trivial_transform
 )
 AstroidManager().register_transform(
-    astroid.Module, _nose_tools_transform, lambda n: n.name == "nose.tools"
+    Module, _nose_tools_transform, lambda n: n.name == "nose.tools"
 )
```

### Comparing `astroid-3.0.0a4/astroid/brain/brain_numpy_core_einsumfunc.py` & `astroid-3.0.0a5/astroid/brain/brain_numpy_core_einsumfunc.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_numpy_core_fromnumeric.py` & `astroid-3.0.0a5/astroid/brain/brain_numpy_core_fromnumeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_numpy_core_function_base.py` & `astroid-3.0.0a5/astroid/brain/brain_numpy_core_function_base.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_numpy_core_multiarray.py` & `astroid-3.0.0a5/astroid/brain/brain_numpy_core_multiarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_numpy_core_numeric.py` & `astroid-3.0.0a5/astroid/brain/brain_numpy_core_numeric.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_numpy_core_numerictypes.py` & `astroid-3.0.0a5/astroid/brain/brain_numpy_core_numerictypes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_numpy_core_umath.py` & `astroid-3.0.0a5/astroid/brain/brain_numpy_core_umath.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_numpy_ma.py` & `astroid-3.0.0a5/astroid/brain/brain_numpy_ma.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_numpy_ndarray.py` & `astroid-3.0.0a5/astroid/brain/brain_numpy_ndarray.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_numpy_random_mtrand.py` & `astroid-3.0.0a5/astroid/brain/brain_numpy_random_mtrand.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_numpy_utils.py` & `astroid-3.0.0a5/astroid/brain/brain_numpy_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_pathlib.py` & `astroid-3.0.0a5/astroid/brain/brain_pathlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_pkg_resources.py` & `astroid-3.0.0a5/astroid/brain/brain_pkg_resources.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_pytest.py` & `astroid-3.0.0a5/astroid/brain/brain_pytest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_qt.py` & `astroid-3.0.0a5/astroid/brain/brain_qt.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_random.py` & `astroid-3.0.0a5/astroid/brain/brain_random.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_re.py` & `astroid-3.0.0a5/astroid/brain/brain_re.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_regex.py` & `astroid-3.0.0a5/astroid/brain/brain_regex.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_responses.py` & `astroid-3.0.0a5/astroid/brain/brain_responses.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_scipy_signal.py` & `astroid-3.0.0a5/astroid/brain/brain_scipy_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_signal.py` & `astroid-3.0.0a5/astroid/brain/brain_signal.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_six.py` & `astroid-3.0.0a5/astroid/brain/brain_six.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_sqlalchemy.py` & `astroid-3.0.0a5/astroid/brain/brain_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_ssl.py` & `astroid-3.0.0a5/astroid/brain/brain_ssl.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_subprocess.py` & `astroid-3.0.0a5/astroid/brain/brain_subprocess.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_threading.py` & `astroid-3.0.0a5/astroid/brain/brain_threading.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_type.py` & `astroid-3.0.0a5/astroid/brain/brain_type.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_typing.py` & `astroid-3.0.0a5/astroid/brain/brain_typing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_unittest.py` & `astroid-3.0.0a5/astroid/brain/brain_unittest.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/brain_uuid.py` & `astroid-3.0.0a5/astroid/brain/brain_uuid.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/brain/helpers.py` & `astroid-3.0.0a5/astroid/brain/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/builder.py` & `astroid-3.0.0a5/astroid/builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,14 +65,16 @@
     """
 
     def __init__(
         self, manager: AstroidManager | None = None, apply_transforms: bool = True
     ) -> None:
         super().__init__(manager)
         self._apply_transforms = apply_transforms
+        if not raw_building.InspectBuilder.bootstrapped:
+            raw_building._astroid_bootstrapping()
 
     def module_build(
         self, module: types.ModuleType, modname: str | None = None
     ) -> nodes.Module:
         """Build an astroid from a living module instance."""
         node = None
         path = getattr(module, "__file__", None)
```

### Comparing `astroid-3.0.0a4/astroid/const.py` & `astroid-3.0.0a5/astroid/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/constraint.py` & `astroid-3.0.0a5/astroid/constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/context.py` & `astroid-3.0.0a5/astroid/context.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/decorators.py` & `astroid-3.0.0a5/astroid/decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/exceptions.py` & `astroid-3.0.0a5/astroid/exceptions.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/filter_statements.py` & `astroid-3.0.0a5/astroid/filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/helpers.py` & `astroid-3.0.0a5/astroid/helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/inference.py` & `astroid-3.0.0a5/astroid/inference.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/inference_tip.py` & `astroid-3.0.0a5/astroid/inference_tip.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,17 @@
             # test cases included with this commit.
             _CURRENTLY_INFERRING.add(partial_cache_key)
             try:
                 # May raise UseInferenceDefault
                 result = _cache[func, node, context] = list(
                     func(node, context, **kwargs)
                 )
+            except Exception as e:
+                # Suppress the KeyError from the cache miss.
+                raise e from None
             finally:
                 # Remove recursion guard.
                 try:
                     _CURRENTLY_INFERRING.remove(partial_cache_key)
                 except KeyError:
                     pass  # Recursion may beat us to the punch.
```

### Comparing `astroid-3.0.0a4/astroid/interpreter/_import/spec.py` & `astroid-3.0.0a5/astroid/interpreter/_import/spec.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/interpreter/_import/util.py` & `astroid-3.0.0a5/astroid/interpreter/_import/util.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/interpreter/dunder_lookup.py` & `astroid-3.0.0a5/astroid/interpreter/dunder_lookup.py`

 * *Files 21% similar despite different names*

```diff
@@ -8,54 +8,65 @@
 logic, found in ``.getattr()``. The difference between these two
 is that the dunder methods are looked with the type slots
 (you can find more about these here
 http://lucumr.pocoo.org/2014/8/16/the-python-i-would-like-to-see/)
 As such, the lookup for the special methods is actually simpler than
 the dot attribute access.
 """
+from __future__ import annotations
+
 import itertools
+from typing import TYPE_CHECKING
 
 import astroid
 from astroid.exceptions import AttributeInferenceError
 
+if TYPE_CHECKING:
+    from astroid import nodes
+    from astroid.context import InferenceContext
+
 
 def _lookup_in_mro(node, name) -> list:
     attrs = node.locals.get(name, [])
 
     nodes = itertools.chain.from_iterable(
         ancestor.locals.get(name, []) for ancestor in node.ancestors(recurs=True)
     )
     values = list(itertools.chain(attrs, nodes))
     if not values:
         raise AttributeInferenceError(attribute=name, target=node)
 
     return values
 
 
-def lookup(node, name) -> list:
+def lookup(
+    node: nodes.NodeNG, name: str, context: InferenceContext | None = None
+) -> list:
     """Lookup the given special method name in the given *node*.
 
     If the special method was found, then a list of attributes
     will be returned. Otherwise, `astroid.AttributeInferenceError`
     is going to be raised.
     """
     if isinstance(
         node, (astroid.List, astroid.Tuple, astroid.Const, astroid.Dict, astroid.Set)
     ):
         return _builtin_lookup(node, name)
     if isinstance(node, astroid.Instance):
         return _lookup_in_mro(node, name)
     if isinstance(node, astroid.ClassDef):
-        return _class_lookup(node, name)
+        return _class_lookup(node, name, context=context)
 
     raise AttributeInferenceError(attribute=name, target=node)
 
 
-def _class_lookup(node, name) -> list:
-    metaclass = node.metaclass()
+def _class_lookup(
+    node: nodes.ClassDef, name: str, context: InferenceContext | None = None
+) -> list:
+    metaclass = node.metaclass(context=context)
     if metaclass is None:
         raise AttributeInferenceError(attribute=name, target=node)
 
     return _lookup_in_mro(metaclass, name)
 
 
 def _builtin_lookup(node, name) -> list:
```

### Comparing `astroid-3.0.0a4/astroid/interpreter/objectmodel.py` & `astroid-3.0.0a5/astroid/interpreter/objectmodel.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/manager.py` & `astroid-3.0.0a5/astroid/manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,22 +65,36 @@
     max_inferable_values: ClassVar[int] = 100
 
     def __init__(self) -> None:
         # NOTE: cache entries are added by the [re]builder
         self.astroid_cache = AstroidManager.brain["astroid_cache"]
         self._mod_file_cache = AstroidManager.brain["_mod_file_cache"]
         self._failed_import_hooks = AstroidManager.brain["_failed_import_hooks"]
-        self.always_load_extensions = AstroidManager.brain["always_load_extensions"]
-        self.optimize_ast = AstroidManager.brain["optimize_ast"]
         self.extension_package_whitelist = AstroidManager.brain[
             "extension_package_whitelist"
         ]
         self._transform = AstroidManager.brain["_transform"]
 
     @property
+    def always_load_extensions(self) -> bool:
+        return AstroidManager.brain["always_load_extensions"]
+
+    @always_load_extensions.setter
+    def always_load_extensions(self, value: bool) -> None:
+        AstroidManager.brain["always_load_extensions"] = value
+
+    @property
+    def optimize_ast(self) -> bool:
+        return AstroidManager.brain["optimize_ast"]
+
+    @optimize_ast.setter
+    def optimize_ast(self, value: bool) -> None:
+        AstroidManager.brain["optimize_ast"] = value
+
+    @property
     def register_transform(self):
         # This and unregister_transform below are exported for convenience
         return self._transform.register_transform
 
     @property
     def unregister_transform(self):
         return self._transform.unregister_transform
```

### Comparing `astroid-3.0.0a4/astroid/mixins.py` & `astroid-3.0.0a5/astroid/mixins.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/modutils.py` & `astroid-3.0.0a5/astroid/modutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -426,15 +426,16 @@
     starti = 0
     if parts[0] == "":
         assert (
             context_file is not None
         ), "explicit relative import, but no context_file?"
         path = []  # prevent resolving the import non-relatively
         starti = 1
-    while parts[starti] == "":  # for all further dots: change context
+    # for all further dots: change context
+    while starti < len(parts) and parts[starti] == "":
         starti += 1
         assert (
             context_file is not None
         ), "explicit relative import, but no context_file?"
         context_file = os.path.dirname(context_file)
     for i in range(starti, len(parts)):
         try:
```

### Comparing `astroid-3.0.0a4/astroid/node_classes.py` & `astroid-3.0.0a5/astroid/node_classes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/nodes/__init__.py` & `astroid-3.0.0a5/astroid/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/nodes/_base_nodes.py` & `astroid-3.0.0a5/astroid/nodes/_base_nodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -126,16 +126,19 @@
         mymodule = self.root()
         level: int | None = getattr(self, "level", None)  # Import has no level
         if modname is None:
             modname = self.modname
         # If the module ImportNode is importing is a module with the same name
         # as the file that contains the ImportNode we don't want to use the cache
         # to make sure we use the import system to get the correct module.
-        # pylint: disable-next=no-member # pylint doesn't recognize type of mymodule
-        if mymodule.relative_to_absolute_name(modname, level) == mymodule.name:
+        if (
+            modname
+            # pylint: disable-next=no-member # pylint doesn't recognize type of mymodule
+            and mymodule.relative_to_absolute_name(modname, level) == mymodule.name
+        ):
             use_cache = False
         else:
             use_cache = True
 
         # pylint: disable-next=no-member # pylint doesn't recognize type of mymodule
         return mymodule.import_module(
             modname,
```

### Comparing `astroid-3.0.0a4/astroid/nodes/as_string.py` & `astroid-3.0.0a5/astroid/nodes/as_string.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/nodes/const.py` & `astroid-3.0.0a5/astroid/nodes/const.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/nodes/node_classes.py` & `astroid-3.0.0a5/astroid/nodes/node_classes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/nodes/node_ng.py` & `astroid-3.0.0a5/astroid/nodes/node_ng.py`

 * *Files 2% similar despite different names*

```diff
@@ -206,15 +206,15 @@
             string = "%(cname)s.%(rname)s(%(fields)s)"
             alignment = len(cname) + len(rname) + 2
         else:
             string = "%(cname)s(%(fields)s)"
             alignment = len(cname) + 1
         result = []
         for field in self._other_fields + self._astroid_fields:
-            value = getattr(self, field)
+            value = getattr(self, field, "Unknown")
             width = 80 - len(field) - alignment
             lines = pprint.pformat(value, indent=2, width=width).splitlines(True)
 
             inner = [lines[0]]
             for line in lines[1:]:
                 inner.append(" " * alignment + line)
             result.append(f"{field}={''.join(inner)}")
@@ -223,22 +223,27 @@
             "cname": cname,
             "rname": rname,
             "fields": (",\n" + " " * alignment).join(result),
         }
 
     def __repr__(self) -> str:
         rname = self.repr_name()
+        # The dependencies used to calculate fromlineno (if not cached) may not exist at the time
+        try:
+            lineno = self.fromlineno
+        except AttributeError:
+            lineno = 0
         if rname:
             string = "<%(cname)s.%(rname)s l.%(lineno)s at 0x%(id)x>"
         else:
             string = "<%(cname)s l.%(lineno)s at 0x%(id)x>"
         return string % {
             "cname": type(self).__name__,
             "rname": rname,
-            "lineno": self.fromlineno,
+            "lineno": lineno,
             "id": id(self),
         }
 
     def accept(self, visitor):
         """Visit this node using the given visitor."""
         func = getattr(visitor, "visit_" + self.__class__.__name__.lower())
         return func(self)
```

### Comparing `astroid-3.0.0a4/astroid/nodes/scoped_nodes/__init__.py` & `astroid-3.0.0a5/astroid/nodes/scoped_nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/nodes/scoped_nodes/mixin.py` & `astroid-3.0.0a5/astroid/nodes/scoped_nodes/mixin.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/nodes/scoped_nodes/scoped_nodes.py` & `astroid-3.0.0a5/astroid/nodes/scoped_nodes/scoped_nodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1662,54 +1662,54 @@
         if isinstance(arg, node_classes.Tuple):
             _rec_get_names(arg.elts, names)
         else:
             names.append(arg.name)
     return names
 
 
-def _is_metaclass(klass, seen=None) -> bool:
+def _is_metaclass(klass, seen=None, context: InferenceContext | None = None) -> bool:
     """Return if the given class can be
     used as a metaclass.
     """
     if klass.name == "type":
         return True
     if seen is None:
         seen = set()
     for base in klass.bases:
         try:
-            for baseobj in base.infer():
+            for baseobj in base.infer(context=context):
                 baseobj_name = baseobj.qname()
                 if baseobj_name in seen:
                     continue
 
                 seen.add(baseobj_name)
                 if isinstance(baseobj, bases.Instance):
                     # not abstract
                     return False
                 if baseobj is klass:
                     continue
                 if not isinstance(baseobj, ClassDef):
                     continue
                 if baseobj._type == "metaclass":
                     return True
-                if _is_metaclass(baseobj, seen):
+                if _is_metaclass(baseobj, seen, context=context):
                     return True
         except InferenceError:
             continue
     return False
 
 
-def _class_type(klass, ancestors=None):
+def _class_type(klass, ancestors=None, context: InferenceContext | None = None):
     """return a ClassDef node type to differ metaclass and exception
     from 'regular' classes
     """
     # XXX we have to store ancestors in case we have an ancestor loop
     if klass._type is not None:
         return klass._type
-    if _is_metaclass(klass):
+    if _is_metaclass(klass, context=context):
         klass._type = "metaclass"
     elif klass.name.endswith("Exception"):
         klass._type = "exception"
     else:
         if ancestors is None:
             ancestors = set()
         klass_name = klass.qname()
@@ -2498,15 +2498,15 @@
         :returns: The inferred value of a subscript to this class.
         :rtype: NodeNG
 
         :raises AstroidTypeError: If this class does not define a
             ``__getitem__`` method.
         """
         try:
-            methods = lookup(self, "__getitem__")
+            methods = lookup(self, "__getitem__", context=context)
         except AttributeInferenceError as exc:
             if isinstance(self, ClassDef):
                 # subscripting a class definition may be
                 # achieved thanks to __class_getitem__ method
                 # which is a classmethod defined in the class
                 # that supports subscript and not in the metaclass
                 try:
```

### Comparing `astroid-3.0.0a4/astroid/nodes/scoped_nodes/utils.py` & `astroid-3.0.0a5/astroid/nodes/scoped_nodes/utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/objects.py` & `astroid-3.0.0a5/astroid/objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/protocols.py` & `astroid-3.0.0a5/astroid/protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/raw_building.py` & `astroid-3.0.0a5/astroid/raw_building.py`

 * *Files 1% similar despite different names*

```diff
@@ -423,14 +423,16 @@
 class InspectBuilder:
     """class for building nodes from living object
 
     this is actually a really minimal representation, including only Module,
     FunctionDef and ClassDef nodes and some others as guessed.
     """
 
+    bootstrapped: bool = False
+
     def __init__(self, manager_instance: AstroidManager | None = None) -> None:
         self._manager = manager_instance or AstroidManager()
         self._done: dict[types.ModuleType | type, nodes.Module | nodes.ClassDef] = {}
         self._module: types.ModuleType
 
     def inspect_build(
         self,
@@ -721,9 +723,15 @@
                 body=[],
                 decorators=None,
                 doc_node=nodes.Const(value=_type.__doc__) if _type.__doc__ else None,
             )
             builder.object_build(klass, _type)
             astroid_builtin[_type.__name__] = klass
 
+    InspectBuilder.bootstrapped = True
+
+    # pylint: disable-next=import-outside-toplevel
+    from astroid.brain.brain_builtin_inference import on_bootstrap
 
-_astroid_bootstrapping()
+    # Instantiates an AstroidBuilder(), which is where
+    # InspectBuilder.bootstrapped is checked, so place after bootstrapped=True.
+    on_bootstrap()
```

### Comparing `astroid-3.0.0a4/astroid/rebuilder.py` & `astroid-3.0.0a5/astroid/rebuilder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/scoped_nodes.py` & `astroid-3.0.0a5/astroid/scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/test_utils.py` & `astroid-3.0.0a5/astroid/test_utils.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/transforms.py` & `astroid-3.0.0a5/astroid/transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/typing.py` & `astroid-3.0.0a5/astroid/typing.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid/util.py` & `astroid-3.0.0a5/astroid/util.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/astroid.egg-info/PKG-INFO` & `astroid-3.0.0a5/astroid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astroid
-Version: 3.0.0a4
+Version: 3.0.0a5
 Summary: An abstract syntax tree for Python with inference support.
 License: LGPL-2.1-or-later
 Project-URL: Docs, https://pylint.readthedocs.io/projects/astroid/en/latest/
 Project-URL: Source Code, https://github.com/pylint-dev/astroid
 Project-URL: Bug tracker, https://github.com/pylint-dev/astroid/issues
 Project-URL: Discord server, https://discord.gg/Egy6P8AMB5
 Keywords: static code analysis,python,abstract syntax tree
```

### Comparing `astroid-3.0.0a4/astroid.egg-info/SOURCES.txt` & `astroid-3.0.0a5/astroid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/pyproject.toml` & `astroid-3.0.0a5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/resources.py` & `astroid-3.0.0a5/tests/resources.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_builder.py` & `astroid-3.0.0a5/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_constraint.py` & `astroid-3.0.0a5/tests/test_constraint.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_decorators.py` & `astroid-3.0.0a5/tests/test_decorators.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_filter_statements.py` & `astroid-3.0.0a5/tests/test_filter_statements.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_group_exceptions.py` & `astroid-3.0.0a5/tests/test_group_exceptions.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_helpers.py` & `astroid-3.0.0a5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_inference.py` & `astroid-3.0.0a5/tests/test_inference.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 import pytest
 
 from astroid import (
     Slice,
     Uninferable,
     arguments,
     helpers,
+    manager,
     nodes,
     objects,
     test_utils,
     util,
 )
 from astroid import decorators as decoratorsmod
 from astroid.arguments import CallSite
@@ -987,14 +988,24 @@
         self.assertIsInstance(inferred[0], nodes.Module)
         self.assertEqual(inferred[0].name, "os.path")
         inferred = list(ast.igetattr("e"))
         self.assertEqual(len(inferred), 1)
         self.assertIsInstance(inferred[0], nodes.FunctionDef)
         self.assertEqual(inferred[0].name, "exists")
 
+    def test_do_import_module_performance(self) -> None:
+        import_node = extract_node("import importlib")
+        import_node.modname = ""
+        import_node.do_import_module()
+        # calling file_from_module_name() indicates we didn't hit the cache
+        with unittest.mock.patch.object(
+            manager.AstroidManager, "file_from_module_name", side_effect=AssertionError
+        ):
+            import_node.do_import_module()
+
     def _test_const_inferred(self, node: nodes.AssignName, value: float | str) -> None:
         inferred = list(node.infer())
         self.assertEqual(len(inferred), 1)
         self.assertIsInstance(inferred[0], nodes.Const)
         self.assertEqual(inferred[0].value, value)
 
     def test_unary_not(self) -> None:
@@ -4009,15 +4020,15 @@
                 return self
         flow = AttributeDict()
         flow['app'] = AttributeDict()
         flow['app']['config'] = AttributeDict()
         flow['app']['config']['doffing'] = AttributeDict() #@
         """
         )
-        self.assertIsNone(helpers.safe_infer(ast_node.targets[0]))
+        self.assertIsInstance(helpers.safe_infer(ast_node.targets[0]), Instance)
 
     def test_classmethod_inferred_by_context(self) -> None:
         ast_node = extract_node(
             """
         class Super(object):
            def instance(cls):
               return cls()
@@ -4220,15 +4231,15 @@
             def __call__(cls):
                 return cls
         class Clazz(metaclass=_Meta):
             pass
         Clazz() #@
         """
         ).inferred()[0]
-        assert isinstance(cls, nodes.ClassDef) and cls.name == "Clazz"
+        assert isinstance(cls, Instance) and cls.name == "Clazz"
 
     def test_infer_subclass_attr_outer_class(self) -> None:
         node = extract_node(
             """
         class Outer:
             data = 123
 
@@ -4893,14 +4904,29 @@
         Foo[int]
         """
         )
         inferred = next(node.infer())
         self.assertIsInstance(inferred, nodes.ClassDef)
         self.assertEqual(inferred.name, "Foo")
 
+    def test_class_subscript_inference_context(self) -> None:
+        """Context path has a reference to any parents inferred by getitem()."""
+        code = """
+        class Parent: pass
+
+        class A(Parent):
+            def __class_getitem__(self, value):
+                return cls
+        """
+        klass = extract_node(code)
+        context = InferenceContext()
+        _ = klass.getitem(0, context=context)
+
+        assert list(context.path)[0][0].name == "Parent"
+
 
 class TestType(unittest.TestCase):
     def test_type(self) -> None:
         pairs = [
             ("type(1)", "int"),
             ("type(type)", "type"),
             ("type(None)", "NoneType"),
@@ -6105,14 +6131,28 @@
     # (https://github.com/pylint-dev/astroid/663, see 55076ca), this test was a
     # non-regression check for StopIteration leaking out of inference and
     # causing a RuntimeError. Hence, here just consume the inferred value
     # without checking it and rely on pytest to fail on raise
     next(node.infer())
 
 
+def test_igetattr_idempotent() -> None:
+    code = """
+    class InferMeTwice:
+        item = 10
+
+    InferMeTwice()
+    """
+    call = extract_node(code)
+    instance = call.inferred()[0]
+    context_to_be_used_twice = InferenceContext()
+    assert util.Uninferable not in instance.igetattr("item", context_to_be_used_twice)
+    assert util.Uninferable not in instance.igetattr("item", context_to_be_used_twice)
+
+
 def test_infer_context_manager_with_unknown_args() -> None:
     code = """
     class client_log(object):
         def __init__(self, client):
             self.client = client
         def __enter__(self):
             return self.client
```

### Comparing `astroid-3.0.0a4/tests/test_inference_calls.py` & `astroid-3.0.0a5/tests/test_inference_calls.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_lookup.py` & `astroid-3.0.0a5/tests/test_lookup.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_manager.py` & `astroid-3.0.0a5/tests/test_manager.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_modutils.py` & `astroid-3.0.0a5/tests/test_modutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,14 +143,17 @@
         self.assertEqual(modutils.get_module_part("sys.path", "__file__"), "sys")
 
     def test_get_module_part_exception(self) -> None:
         self.assertRaises(
             ImportError, modutils.get_module_part, "unknown.module", modutils.__file__
         )
 
+    def test_get_module_part_only_dot(self) -> None:
+        self.assertEqual(modutils.get_module_part(".", modutils.__file__), ".")
+
 
 class ModPathFromFileTest(unittest.TestCase):
     """Given an absolute file path return the python module's path as a list."""
 
     def test_known_values_modpath_from_file_1(self) -> None:
         self.assertEqual(
             modutils.modpath_from_file(ElementTree.__file__),
```

### Comparing `astroid-3.0.0a4/tests/test_nodes.py` & `astroid-3.0.0a5/tests/test_nodes.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,17 @@
 # Copyright (c) https://github.com/pylint-dev/astroid/blob/main/CONTRIBUTORS.txt
 
 """Tests for specific behaviour of astroid nodes."""
 
 from __future__ import annotations
 
 import copy
+import inspect
 import os
+import random
 import sys
 import textwrap
 import unittest
 from typing import Any
 
 import pytest
 
@@ -1876,7 +1878,39 @@
         return_from_match(10)  #@
         """
         ).strip()
         node = builder.extract_node(code)
         inferred = node.inferred()
         assert len(inferred) == 2
         assert [inf.value for inf in inferred] == [10, -1]
+
+
+@pytest.mark.parametrize(
+    "node",
+    [
+        node
+        for node in astroid.nodes.ALL_NODE_CLASSES
+        if node.__name__
+        not in ["_BaseContainer", "BaseContainer", "NodeNG", "const_factory"]
+    ],
+)
+@pytest.mark.filterwarnings("error")
+def test_str_repr_no_warnings(node):
+    parameters = inspect.signature(node.__init__).parameters
+
+    args = {}
+    for name, param_type in parameters.items():
+        if name == "self":
+            continue
+
+        if "int" in param_type.annotation:
+            args[name] = random.randint(0, 50)
+        elif "NodeNG" in param_type.annotation:
+            args[name] = nodes.Unknown()
+        elif "str" in param_type.annotation:
+            args[name] = ""
+        else:
+            args[name] = None
+
+    test_node = node(**args)
+    str(test_node)
+    repr(test_node)
```

### Comparing `astroid-3.0.0a4/tests/test_nodes_lineno.py` & `astroid-3.0.0a5/tests/test_nodes_lineno.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_nodes_position.py` & `astroid-3.0.0a5/tests/test_nodes_position.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_object_model.py` & `astroid-3.0.0a5/tests/test_object_model.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_objects.py` & `astroid-3.0.0a5/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_protocols.py` & `astroid-3.0.0a5/tests/test_protocols.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_python3.py` & `astroid-3.0.0a5/tests/test_python3.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_raw_building.py` & `astroid-3.0.0a5/tests/test_raw_building.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_regrtest.py` & `astroid-3.0.0a5/tests/test_regrtest.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 import textwrap
 import unittest
 from unittest import mock
 
 import pytest
 
-from astroid import MANAGER, Instance, bases, nodes, parse, test_utils
+from astroid import MANAGER, Instance, bases, manager, nodes, parse, test_utils
 from astroid.builder import AstroidBuilder, _extract_single_node, extract_node
 from astroid.context import InferenceContext
 from astroid.exceptions import InferenceError
 from astroid.raw_building import build_module
 from astroid.util import Uninferable
 
 from . import resources
@@ -32,30 +32,48 @@
         MANAGER.always_load_extensions = True
 
     def tearDown(self) -> None:
         MANAGER.always_load_extensions = False
         sys.path.pop(0)
         sys.path_importer_cache.pop(resources.find("data"), None)
 
+    def test_manager_instance_attributes_reference_global_MANAGER(self) -> None:
+        for expected in (True, False):
+            with mock.patch.dict(
+                manager.AstroidManager.brain,
+                values={"always_load_extensions": expected},
+            ):
+                assert (
+                    MANAGER.always_load_extensions
+                    == manager.AstroidManager.brain["always_load_extensions"]
+                )
+            with mock.patch.dict(
+                manager.AstroidManager.brain,
+                values={"optimize_ast": expected},
+            ):
+                assert (
+                    MANAGER.optimize_ast == manager.AstroidManager.brain["optimize_ast"]
+                )
+
     def test_module_path(self) -> None:
         man = test_utils.brainless_manager()
         mod = man.ast_from_module_name("package.import_package_subpackage_module")
         package = next(mod.igetattr("package"))
         self.assertEqual(package.name, "package")
         subpackage = next(package.igetattr("subpackage"))
         self.assertIsInstance(subpackage, nodes.Module)
         self.assertTrue(subpackage.package)
         self.assertEqual(subpackage.name, "package.subpackage")
         module = next(subpackage.igetattr("module"))
         self.assertEqual(module.name, "package.subpackage.module")
 
     def test_package_sidepackage(self) -> None:
-        manager = test_utils.brainless_manager()
+        brainless_manager = test_utils.brainless_manager()
         assert "package.sidepackage" not in MANAGER.astroid_cache
-        package = manager.ast_from_module_name("absimp")
+        package = brainless_manager.ast_from_module_name("absimp")
         self.assertIsInstance(package, nodes.Module)
         self.assertTrue(package.package)
         subpackage = next(package.getattr("sidepackage")[0].infer())
         self.assertIsInstance(subpackage, nodes.Module)
         self.assertTrue(subpackage.package)
         self.assertEqual(subpackage.name, "absimp.sidepackage")
```

### Comparing `astroid-3.0.0a4/tests/test_scoped_nodes.py` & `astroid-3.0.0a5/tests/test_scoped_nodes.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_stdlib.py` & `astroid-3.0.0a5/tests/test_stdlib.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_transforms.py` & `astroid-3.0.0a5/tests/test_transforms.py`

 * *Files identical despite different names*

### Comparing `astroid-3.0.0a4/tests/test_utils.py` & `astroid-3.0.0a5/tests/test_utils.py`

 * *Files identical despite different names*

